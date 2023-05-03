# Comparing `tmp/opnieuw-1.2.0.tar.gz` & `tmp/opnieuw-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opnieuw-1.2.0.tar", last modified: Wed May 18 12:19:07 2022, max compression
+gzip compressed data, was "dist/opnieuw-1.2.1.tar", last modified: Wed May  3 14:27:41 2023, max compression
```

## Comparing `opnieuw-1.2.0.tar` & `opnieuw-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2022-05-18 12:19:07.000000 opnieuw-1.2.0/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1508 2022-05-18 12:19:05.000000 opnieuw-1.2.0/LICENSE
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4979 2022-05-18 12:19:07.000000 opnieuw-1.2.0/PKG-INFO
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4569 2022-05-18 12:19:05.000000 opnieuw-1.2.0/README.md
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2022-05-18 12:19:07.000000 opnieuw-1.2.0/opnieuw/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      281 2022-05-18 12:19:05.000000 opnieuw-1.2.0/opnieuw/__init__.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      802 2022-05-18 12:19:05.000000 opnieuw-1.2.0/opnieuw/clock.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      298 2022-05-18 12:19:05.000000 opnieuw-1.2.0/opnieuw/exceptions.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        0 2022-05-18 12:19:05.000000 opnieuw-1.2.0/opnieuw/py.typed
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)    11747 2022-05-18 12:19:05.000000 opnieuw-1.2.0/opnieuw/retries.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      668 2022-05-18 12:19:05.000000 opnieuw-1.2.0/opnieuw/test_util.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      586 2022-05-18 12:19:05.000000 opnieuw-1.2.0/opnieuw/util.py
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2022-05-18 12:19:07.000000 opnieuw-1.2.0/opnieuw.egg-info/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4979 2022-05-18 12:19:06.000000 opnieuw-1.2.0/opnieuw.egg-info/PKG-INFO
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      282 2022-05-18 12:19:07.000000 opnieuw-1.2.0/opnieuw.egg-info/SOURCES.txt
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        1 2022-05-18 12:19:06.000000 opnieuw-1.2.0/opnieuw.egg-info/dependency_links.txt
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        8 2022-05-18 12:19:06.000000 opnieuw-1.2.0/opnieuw.egg-info/top_level.txt
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)       38 2022-05-18 12:19:07.000000 opnieuw-1.2.0/setup.cfg
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      912 2022-05-18 12:19:05.000000 opnieuw-1.2.0/setup.py
+drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2023-05-03 14:27:41.000000 opnieuw-1.2.1/
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1508 2023-05-03 14:27:39.000000 opnieuw-1.2.1/LICENSE
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4979 2023-05-03 14:27:41.000000 opnieuw-1.2.1/PKG-INFO
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4569 2023-05-03 14:27:39.000000 opnieuw-1.2.1/README.md
+drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw/
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      281 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/__init__.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      802 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/clock.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      298 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/exceptions.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        0 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/py.typed
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)    11018 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/retries.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      668 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/test_util.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      586 2023-05-03 14:27:39.000000 opnieuw-1.2.1/opnieuw/util.py
+drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw.egg-info/
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4979 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw.egg-info/PKG-INFO
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      399 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw.egg-info/SOURCES.txt
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        1 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw.egg-info/dependency_links.txt
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)       54 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw.egg-info/requires.txt
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        8 2023-05-03 14:27:41.000000 opnieuw-1.2.1/opnieuw.egg-info/top_level.txt
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)       38 2023-05-03 14:27:41.000000 opnieuw-1.2.1/setup.cfg
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1001 2023-05-03 14:27:39.000000 opnieuw-1.2.1/setup.py
+drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2023-05-03 14:27:41.000000 opnieuw-1.2.1/tests/
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     8433 2023-05-03 14:27:39.000000 opnieuw-1.2.1/tests/test_context_local.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      902 2023-05-03 14:27:39.000000 opnieuw-1.2.1/tests/test_exponential_multiplier.py
+-rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     3316 2023-05-03 14:27:39.000000 opnieuw-1.2.1/tests/test_opnieuw.py
```

### Comparing `opnieuw-1.2.0/LICENSE` & `opnieuw-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opnieuw-1.2.0/PKG-INFO` & `opnieuw-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opnieuw
-Version: 1.2.0
+Version: 1.2.1
 Summary: Retries for humans
 Home-page: https://github.com/channable/opnieuw
 Author: Channable
 Author-email: ruud@channable.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `opnieuw-1.2.0/README.md` & `opnieuw-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `opnieuw-1.2.0/opnieuw/clock.py` & `opnieuw-1.2.1/opnieuw/clock.py`

 * *Files identical despite different names*

### Comparing `opnieuw-1.2.0/opnieuw/retries.py` & `opnieuw-1.2.1/opnieuw/retries.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 # Opnieuw: Retries for humans
 # Copyright 2019 Channable
 #
 # Licensed under the 3-clause BSD license, see the LICENSE file in the repository root.
 
 # pylint: disable=raising-bad-type
+
+from __future__ import annotations
+
 import asyncio
 import functools
 import logging
 import random
+import sys
 import time
 from collections import defaultdict
+from collections.abc import Awaitable, Callable, Iterator
 from contextlib import contextmanager
 from contextvars import ContextVar
-from typing import (
-    Awaitable,
-    cast,
-    Any,
-    Callable,
-    Iterator,
-    NamedTuple,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-    Dict,
-    Optional,
-)
+from typing import NamedTuple, TypeVar, Union
+
+if sys.version_info < (3, 10):
+    from typing_extensions import ParamSpec
+else:
+    from typing import ParamSpec
 
 from .clock import Clock, MonotonicClock
 
 logger = logging.getLogger(__name__)
 
-# Type variable to annotate decorators that take a function,
-# and return a function with the same signature.
-F = TypeVar("F", bound=Callable[..., Any])
-# Type variable to annotate decorators that take an async function,
-# and return a function with the same signature.
-AF = TypeVar("AF", bound=Callable[..., Awaitable[Any]])
+R = TypeVar("R")
+P = ParamSpec("P")
 
 
 def calculate_exponential_multiplier(
     max_calls_total: int, retry_window_after_first_call_in_seconds: int
 ) -> float:
     r"""
     Solve the following equation for `m`:
@@ -123,38 +116,38 @@
         )
 
     def __iter__(self) -> Iterator[Action]:
         for attempt in range(0, self.max_calls_total):
             # attempt the actual function call
             yield DoCall()
 
-            wait_seconds = self.base_in_seconds * 2 ** attempt
+            wait_seconds = self.base_in_seconds * 2**attempt
             seconds_left = self.deadline_second - self.clock.seconds_since_epoch()
 
             # signal that we need to sleep
             yield DoWait(
                 attempts_so_far=attempt + 1,
                 min_seconds=0.0,
                 max_seconds=wait_seconds,
                 seconds_left=seconds_left,
             )
 
 
-__retry_state_namespaces: Dict[
-    Optional[str], ContextVar[Type[RetryState]]
-] = defaultdict(lambda: ContextVar("opnieuw_default_retry_state", default=RetryState))
+__retry_state_namespaces: dict[str | None, ContextVar[type[RetryState]]] = defaultdict(
+    lambda: ContextVar("opnieuw_default_retry_state", default=RetryState)
+)
 
 
-def _get_retry_state_class(namespace: Optional[str]) -> Type[RetryState]:
+def _get_retry_state_class(namespace: str | None) -> type[RetryState]:
     return __retry_state_namespaces[namespace].get()
 
 
 @contextmanager
 def replace_retry_state(
-    state: Type[RetryState], *, namespace: Optional[str] = None
+    state: type[RetryState], *, namespace: str | None = None
 ) -> Iterator[None]:
     """
     A context manager that replaces the state of the specified namespace with the
     given `RetryState`.
     This can be useful to customize the retry behavior, such as disabling the sleep interval during
     tests (see `opnieuw.test_util.retry_immediately`).
 
@@ -167,19 +160,19 @@
         yield
     finally:
         __retry_state_namespaces[namespace].reset(token)
 
 
 def retry(
     *,
-    retry_on_exceptions: Union[Type[Exception], Tuple[Type[Exception], ...]],
+    retry_on_exceptions: type[Exception] | tuple[type[Exception], ...],
     max_calls_total: int = 3,
     retry_window_after_first_call_in_seconds: int = 60,
-    namespace: Optional[str] = None,
-) -> Callable[[F], F]:
+    namespace: str | None = None,
+) -> Callable[[Callable[P, R]], Callable[P, R]]:
     """
     Retry a function using a Full Jitter exponential backoff.
 
     This function exposes four settings:
 
      - `retry_on_exceptions` - A tuple of exception types to retry on.
      - `max_calls_total` - The maximum number of calls of the decorated
@@ -226,17 +219,17 @@
     seconds have elapsed after the first retry, the second retry is not
     scheduled.
 
     Opnieuw is based on a retry algorithm off of:
         https://aws.amazon.com/blogs/architecture/exponential-backoff-and-jitter/
     """
 
-    def decorator(f: F) -> F:
+    def decorator(f: Callable[P, R]) -> Callable[P, R]:
         @functools.wraps(f)
-        def wrapper(*args: Any, **kwargs: Any) -> Any:
+        def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
 
             last_exception = None
 
             retry_state = _get_retry_state_class(namespace)(
                 MonotonicClock(),
                 max_calls_total=max_calls_total,
                 retry_window_after_first_call_in_seconds=retry_window_after_first_call_in_seconds,
@@ -268,40 +261,32 @@
 
                     logger.debug(
                         f"Sleeping for {sleep_seconds:.3f} seconds after "
                         f"attempt {retry_action.attempts_so_far}"
                     )
                     time.sleep(sleep_seconds)
 
-            if last_exception is not None:
-                raise last_exception
+            assert last_exception is not None
+            raise last_exception
 
-        # `wrapper` has type `Callable[..., Any]`, whereas we should return something
-        # of type F, where F is some subtype of Callable[..., Any]. Note that inside
-        # this function, F is bound. That is, a particular type F has been fixed.
-        # The reason we use a type variable in the first place is not just to say
-        # "we take and return some callable function", but to say "this function
-        # returns something of exactly the same type as what you pass in". The thing
-        # you pass in has type F. And we construct `wrapped` in such a way to have
-        # type F too, therefore this cast is appropriate.
-        return cast(F, wrapper)
+        return wrapper
 
     return decorator
 
 
 def retry_async(
     *,
-    retry_on_exceptions: Union[Type[Exception], Tuple[Type[Exception], ...]],
+    retry_on_exceptions: type[Exception] | tuple[type[Exception], ...],
     max_calls_total: int = 3,
     retry_window_after_first_call_in_seconds: int = 60,
-    namespace: Optional[str] = None,
-) -> Callable[[AF], AF]:
-    def decorator(f: AF) -> AF:
+    namespace: str | None = None,
+) -> Callable[[Callable[P, Awaitable[R]]], Callable[P, Awaitable[R]]]:
+    def decorator(f: Callable[P, Awaitable[R]]) -> Callable[P, Awaitable[R]]:
         @functools.wraps(f)
-        async def wrapper(*args: Any, **kwargs: Any) -> Any:
+        async def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
 
             last_exception = None
 
             retry_state = _get_retry_state_class(namespace)(
                 MonotonicClock(),
                 max_calls_total=max_calls_total,
                 retry_window_after_first_call_in_seconds=retry_window_after_first_call_in_seconds,
@@ -333,16 +318,16 @@
 
                     logger.debug(
                         f"Sleeping for {sleep_seconds:.3f} seconds after "
                         f"attempt {retry_action.attempts_so_far}"
                     )
                     await asyncio.sleep(sleep_seconds)
 
-            if last_exception is not None:
-                raise last_exception
+            assert last_exception is not None
+            raise last_exception
 
-        return cast(AF, wrapper)
+        return wrapper
 
     return decorator
 
 
 retry_async.__doc__ = retry.__doc__
```

### Comparing `opnieuw-1.2.0/opnieuw/test_util.py` & `opnieuw-1.2.1/opnieuw/test_util.py`

 * *Files identical despite different names*

### Comparing `opnieuw-1.2.0/opnieuw/util.py` & `opnieuw-1.2.1/opnieuw/util.py`

 * *Files identical despite different names*

### Comparing `opnieuw-1.2.0/opnieuw.egg-info/PKG-INFO` & `opnieuw-1.2.1/opnieuw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opnieuw
-Version: 1.2.0
+Version: 1.2.1
 Summary: Retries for humans
 Home-page: https://github.com/channable/opnieuw
 Author: Channable
 Author-email: ruud@channable.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `opnieuw-1.2.0/setup.py` & `opnieuw-1.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Licensed under the 3-clause BSD license, see the LICENSE file in the repository root.
 
 import setuptools  # type: ignore
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 setuptools.setup(
     name="opnieuw",
     version=__version__,
     author="Channable",
     author_email="ruud@channable.com",
     description="Retries for humans",
@@ -25,8 +25,11 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
+    install_requires=[
+        "typing-extensions>=3.10.0;python_version<'3.10'",
+    ],
 )
```

