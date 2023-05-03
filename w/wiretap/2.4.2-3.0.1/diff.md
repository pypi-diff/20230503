# Comparing `tmp/wiretap-2.4.2-py3-none-any.whl.zip` & `tmp/wiretap-3.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4528 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      191 b- defN 23-Mar-15 19:56 wiretap/__init__.py
+Zip file size: 4707 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      201 b- defN 23-Apr-07 12:05 wiretap/__init__.py
 -rw-rw-rw-  2.0 fat      620 b- defN 23-Feb-08 09:16 wiretap/layers.py
--rw-rw-rw-  2.0 fat     9880 b- defN 23-Mar-16 09:54 wiretap/wiretap.py
--rw-rw-rw-  2.0 fat      223 b- defN 23-Mar-16 09:54 wiretap-2.4.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-16 09:54 wiretap-2.4.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-16 09:54 wiretap-2.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      519 b- defN 23-Mar-16 09:54 wiretap-2.4.2.dist-info/RECORD
-7 files, 11533 bytes uncompressed, 3610 bytes compressed:  68.7%
+-rw-rw-rw-  2.0 fat    10812 b- defN 23-Apr-28 12:28 wiretap/wiretap.py
+-rw-rw-rw-  2.0 fat      223 b- defN 23-May-03 11:19 wiretap-3.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-03 11:19 wiretap-3.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-03 11:19 wiretap-3.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      520 b- defN 23-May-03 11:19 wiretap-3.0.1.dist-info/RECORD
+7 files, 12476 bytes uncompressed, 3789 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: wiretap/layers.py
 Comment: 
 
 Filename: wiretap/wiretap.py
 Comment: 
 
-Filename: wiretap-2.4.2.dist-info/METADATA
+Filename: wiretap-3.0.1.dist-info/METADATA
 Comment: 
 
-Filename: wiretap-2.4.2.dist-info/WHEEL
+Filename: wiretap-3.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: wiretap-2.4.2.dist-info/top_level.txt
+Filename: wiretap-3.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: wiretap-2.4.2.dist-info/RECORD
+Filename: wiretap-3.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wiretap/__init__.py

```diff
@@ -1,12 +1,12 @@
 from .wiretap import (
     Logger,
     telemetry,
     OnStarted,
     OnCompleted,
     CannotContinue,
-    local,
+    begin_telemetry,
     SerializeDetails,
     MultiFormatter,
 )
 
 from . import layers
```

## wiretap/wiretap.py

```diff
@@ -1,74 +1,80 @@
-import os
 import sys
-import logging
-import inspect
+import asyncio
+import contextlib
 import functools
+import inspect
 import json
-import asyncio
+import logging
+import sys
 import uuid
-import contextvars
-import contextlib
-from typing import Dict, Callable, Any, Protocol, Optional, TypeVar
-from timeit import default_timer as timer
+from collections.abc import Generator
+from contextvars import ContextVar
 from datetime import datetime, date
+from timeit import default_timer as timer
+from typing import Dict, Callable, Any, Protocol, Optional, Iterator
 
-_scope = contextvars.ContextVar("_scope", default=None)
+_scope: ContextVar[Optional["Logger"]] = ContextVar("_scope", default=None)
 
 
-class MultiFormatter(logging.Formatter):
+class SerializeDetails(Protocol):
+    def __call__(self, value: Optional[Dict[str, Any]]) -> str | None: ...
 
-    def __new__(cls, **kwargs):
-        instance = super().__new__(cls)
-        setattr(instance, "values", [])
-        return instance
 
-    def format(self, record: logging.LogRecord) -> str:
-        # record.__dict__["instance"] = self.instance
-        record.levelname = record.levelname.lower()
-        record.values = self.values
-        self._style._fmt = self.wiretap if hasattr(record, "status") else self.classic
-        return super().format(record)
+class SerializeDetailsToJson(SerializeDetails):
+    def __call__(self, value: Optional[Dict[str, Any]]) -> str | None:
+        return json.dumps(value, sort_keys=True, allow_nan=False, cls=_JsonDateTimeEncoder) if value else None
+
+
+class _JsonDateTimeEncoder(json.JSONEncoder):
+    def default(self, o: Any) -> Any:
+        if isinstance(o, (date, datetime)):
+            return o.isoformat()
 
 
-# @runtime_checkable
-# class LoggerContext(Protocol):
-#     parent: Any
-#     id: uuid.UUID
-#     elapsed: float
-#
-#     def running(self, **kwargs):
-#         ...
-#
-#     def canceled(self, **kwargs):
-#         ...
+DEFAULT_FORMATS: Dict[str, str] = {
+    "classic": "{asctime}.{msecs:.0f} | {levelname} | {module}.{funcName} | {message}",
+    "wiretap": "{asctime}.{msecs:.0f} [{indent}] {levelname} | {module}.{funcName} | {status} | {elapsed} | {details} | [{parent}/{node}] | {attachment}",
+}
 
 
-class Hierarchy(Protocol):
-    parent: Any
+class MultiFormatter(logging.Formatter):
+    formats: Dict[str, str] = DEFAULT_FORMATS
+    indent: str = "."
+    values: Optional[Dict[str, Any]] = None
+    serialize_details: SerializeDetails = SerializeDetailsToJson()
 
+    def format(self, record: logging.LogRecord) -> str:
+        record.levelname = record.levelname.lower()
+        record.values = self.values or {}
 
-class SerializeDetails(Protocol):
-    def __call__(self, **kwargs) -> str | None: ...
+        if hasattr(record, "details") and isinstance(record.details, dict):
+            record.indent = self.indent * record.details["depth"]
+            record.details = self.serialize_details(record.details)
 
+        self._style._fmt = self.formats["classic"]
 
-class DefaultSerializeDetails(SerializeDetails):
-    def __call__(self, **kwargs) -> str | None:
-        return json.dumps(kwargs, sort_keys=True, allow_nan=False, cls=_JsonDateTimeEncoder) if kwargs else None
+        if hasattr(record, "status"):
+            self._style._fmt = self.formats["wiretap"]
+
+        if hasattr(record, "format"):
+            self._style._fmt = record.format
+
+        self.formats = DEFAULT_FORMATS | self.formats
+        return super().format(record)
 
 
 class Logger:
-    serialize_details: SerializeDetails = DefaultSerializeDetails()
 
-    def __init__(self, module: Optional[str], scope: str, attachment: Optional[Any] = None, parent: Optional[Hierarchy] = None):
+    def __init__(self, module: Optional[str], scope: str, parent: Optional["Logger"] = None):
         self.id = uuid.uuid4()
         self.module = module
         self.scope = scope
-        self.attachment = attachment
         self.parent = parent
+        self.depth = sum(1 for _ in self)
         self._start = timer()
         self._finalized = False
         self._logger = logging.getLogger(f"{module}.{scope}")
 
     @property
     def elapsed(self) -> float:
         return round(timer() - self._start, 3)
@@ -79,104 +85,78 @@
         self._log(**kwargs)
 
     def running(self, **kwargs):
         self._logger.setLevel(logging.DEBUG)
         self._log(**kwargs)
 
     def completed(self, **kwargs):
-        if self._finalized:
-            return
-
         self._logger.setLevel(logging.INFO)
         self._log(**kwargs)
-        self._finalized = True
 
     def canceled(self, **kwargs):
-        if self._finalized:
-            return
-
         self._logger.setLevel(logging.WARNING)
         self._log(**kwargs)
-        self._finalized = True
 
     def faulted(self, **kwargs):
-        if self._finalized:
-            return
-
         self._logger.setLevel(logging.ERROR)
         self._log(**kwargs)
-        self._finalized = True
 
     def _log(self, **kwargs):
-        # kwargs["depth"] = sum(1 for _ in self)
+        if self._finalized:
+            return
+
         status = inspect.stack()[1][3]
-        details = Logger.serialize_details(**kwargs)
-        with _create_log_record(
+        with _use_custom_log_record_factory(
+                _set_exc_text,
                 functools.partial(_set_module_name, name=self.module),
-                functools.partial(_set_func_name, name=self.scope)
+                functools.partial(_set_func_name, name=self.scope),
+                functools.partial(_set_attachment, value=kwargs.pop("attachment", None)),
         ):
             # Exceptions must be logged with the exception method or otherwise the exception will be missing.
             is_error = all(sys.exc_info()) and sys.exc_info()[0] is not CannotContinue
             self._logger.log(level=self._logger.level, msg=None, exc_info=is_error, extra={
                 "parent": self.parent.id if self.parent else None,
                 "node": self.id,
                 "status": status,
                 "elapsed": self.elapsed,
-                "details": details,
-                "attachment": self.attachment
+                "details": kwargs | {"depth": self.depth}
             })
 
+        self._finalized = status in [self.completed.__name__, self.canceled.__name__, self.faulted.__name__]
+
     def __iter__(self):
         current = self
         while current:
             yield current
             current = current.parent
 
 
-@contextlib.contextmanager
-def local(name: str, details: Dict | None = None, attachment: Any = None) -> Logger:
-    work = Logger(None, name, attachment, _scope.get())
-    token = _scope.set(work)
-    try:
-        work.started(**details if details else dict())
-        yield work
-        work.completed()
-    except Exception:
-        work.faulted()
-        raise
-    finally:
-        _scope.reset(token)
-
-
 class AttachDetails(Protocol):
     def __call__(self, details: Dict[str, Any]) -> None: ...
 
 
 class OnStarted(Protocol):
     """Allows you to create details from function arguments."""
 
-    def __call__(self, kwargs: Dict[str, Any]) -> Optional[Dict[str, Any]]: ...
+    def __call__(self, params: Dict[str, Any]) -> Optional[Dict[str, Any]]: ...
 
 
 class OnCompleted(Protocol):
     """Allows you to create details from function result."""
 
     def __call__(self, result: Any) -> Optional[Dict[str, Any]]: ...
 
 
-#NoResult = TypeVar("NoResult")
-
-
 class CannotContinue(Exception):
     """Raise this error to gracefully handle a cancellation."""
 
     details: Dict[str, Any] = dict()
     result: Optional[Any] = None
 
-    def __new__(cls, reason: str, result: Optional[Any] = None, **details) -> Any:
+    def __new__(cls, reason: str, result: Optional[Any] = None, **details) -> "CannotContinue":
         instance = super().__new__(cls)
         details["reason"] = reason
         instance.details = details
         instance.result = result
         return instance
 
     def __init__(self, reason: str, result: Optional[Any] = None, **details):
@@ -185,27 +165,33 @@
 
 class ReturnValueMissing(Exception):
 
     def __init__(self, name: str):
         super().__init__(f"Function '{name}' expects a return value, but it wasn't provided.")
 
 
-def telemetry(on_started: Optional[OnStarted] = None, on_completed: Optional[OnCompleted] = None, **kwargs):
-    """Provides flow telemetry for the decorated function. Use named args to provide more static data."""
+def _default_on_started(params: Dict[str, Any]) -> Optional[Dict[str, Any]]:
+    return None
+
+
+def _default_on_completed(result: Any) -> Optional[Dict[str, Any]]:
+    return None
+
 
-    on_started = on_started or (lambda _: {})
-    on_completed = on_completed or (lambda _: {})
+def telemetry(on_started: OnStarted = _default_on_started, on_completed: OnCompleted = _default_on_completed, attachment: Optional[Any] = None):
+    """Provides flow telemetry for the decorated function. Use named args to provide more static data."""
 
     def factory(decoratee):
+        module = inspect.getmodule(decoratee)
+
         @contextlib.contextmanager
-        def logger_scope() -> Logger:
+        def logger_scope() -> Iterator[Logger]:
             logger = Logger(
-                module=inspect.getmodule(decoratee).__name__,
+                module=module.__name__ if module else None,
                 scope=decoratee.__name__,
-                attachment=kwargs.pop("attachment", None),
                 parent=_scope.get()
             )
 
             token = _scope.set(logger)
             try:
                 yield logger
             except Exception:
@@ -227,72 +213,93 @@
             return {t[0]: decoratee_args[t[1]] for t in arg_pairs} | decoratee_kwargs
 
         # returns = inspect.getfullargspec(decoratee).annotations.get("return", None) is not None
 
         if asyncio.iscoroutinefunction(decoratee):
             @functools.wraps(decoratee)
             async def decorator(*decoratee_args, **decoratee_kwargs):
+                if attachment:
+                    decoratee_kwargs["attachment"] = attachment
                 with logger_scope() as scope:
                     inject_logger(scope, decoratee_kwargs)
-                    scope.started(**on_started(params(*decoratee_args, **decoratee_kwargs)))
+                    scope.started(**(on_started(params(*decoratee_args, **decoratee_kwargs)) or {}))
                     try:
                         result = await decoratee(*decoratee_args, **decoratee_kwargs)
-                        scope.completed(**on_completed(result))
+                        scope.completed(**(on_completed(result) or {}))
                         return result
                     except CannotContinue as e:
-                        scope.canceled(**(on_completed(e.result) | e.details))
+                        scope.canceled(**((on_completed(result) or {}) | e.details))
                         return e.result
 
             decorator.__signature__ = inspect.signature(decoratee)
             return decorator
 
         else:
             @functools.wraps(decoratee)
             def decorator(*decoratee_args, **decoratee_kwargs):
+                if attachment:
+                    decoratee_kwargs["attachment"] = attachment
                 with logger_scope() as scope:
                     inject_logger(scope, decoratee_kwargs)
-                    scope.started(**on_started(params(*decoratee_args, **decoratee_kwargs)))
+                    scope.started(**(on_started(params(*decoratee_args, **decoratee_kwargs)) or {}))
                     try:
                         result = decoratee(*decoratee_args, **decoratee_kwargs)
-                        scope.completed(**on_completed(result))
+                        scope.completed(**(on_completed(result) or {}))
                         return result
                     except CannotContinue as e:
-                        scope.canceled(**(on_completed(e.result) | e.details))
+                        scope.canceled(**((on_completed(result) or {}) | e.details))
                         return e.result
 
             decorator.__signature__ = inspect.signature(decoratee)
             return decorator
 
     return factory
 
 
 @contextlib.contextmanager
-def _create_log_record(*actions: Callable[[logging.LogRecord], None]):
+def begin_telemetry(name: str, **kwargs) -> Iterator[Logger]:
+    """Begins a new telemetry scope."""
+    logger = Logger(None, name, _scope.get())
+    token = _scope.set(logger)
+    try:
+        logger.started(**kwargs)
+        yield logger
+        logger.completed()
+    except:  # noqa
+        logger.faulted()
+        raise
+    finally:
+        _scope.reset(token)
+
+
+@contextlib.contextmanager
+def _use_custom_log_record_factory(*actions: Callable[[logging.LogRecord], None]) -> Generator[None, None, None]:
     default = logging.getLogRecordFactory()
 
     def custom(*args, **kwargs):
         record = default(*args, **kwargs)
-
-        if record.exc_info:
-            record.exc_text = logging.Formatter().formatException(record.exc_info)
-
         for action in actions:
             action(record)
         return record
 
     logging.setLogRecordFactory(custom)
-    yield
-    logging.setLogRecordFactory(default)
+    try:
+        yield
+    finally:
+        logging.setLogRecordFactory(default)
 
 
 def _set_func_name(record: logging.LogRecord, name: str):
     record.funcName = name
 
 
 def _set_module_name(record: logging.LogRecord, name: str):
     record.module = name
 
 
-class _JsonDateTimeEncoder(json.JSONEncoder):
-    def default(self, o: Any) -> Any:
-        if isinstance(o, (date, datetime)):
-            return o.isoformat()
+def _set_exc_text(record: logging.LogRecord):
+    if record.exc_info:
+        record.exc_text = logging.Formatter().formatException(record.exc_info)
+
+
+def _set_attachment(record: logging.LogRecord, value: Optional[Any]):
+    record.attachment = record.exc_text or value
```

