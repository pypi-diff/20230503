# Comparing `tmp/diator-0.1.1.tar.gz` & `tmp/diator-0.1.2.tar.gz`

## Comparing `diator-0.1.1.tar` & `diator-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 diator-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/__init__.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/mediator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/py.typed
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/container/__init__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/container/di.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/container/protocol.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/container/rodi.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/dispatcher/__init__.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/dispatcher/default.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/dispatcher/dispatch_result.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/dispatcher/protocol.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/events/__init__.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/events/event.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/events/event_emitter.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/events/event_handler.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/events/map.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/message_brokers/__init__.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/message_brokers/azure.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/message_brokers/protocol.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/message_brokers/redis.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/middlewares/__init__.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/middlewares/base.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/middlewares/logging.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/requests/__init__.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/requests/map.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/requests/request.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 diator-0.1.1/src/diator/requests/request_handler.py
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 diator-0.1.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 diator-0.1.1/LICENSE.rst
--rw-r--r--   0        0        0    10944 2020-02-02 00:00:00.000000 diator-0.1.1/README.md
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 diator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 diator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 diator-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 diator-0.1.2/mkdocs.yml
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 diator-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0    13763 2020-02-02 00:00:00.000000 diator-0.1.2/assets/logo_diator.svg
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/__init__.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/mediator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/py.typed
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/container/__init__.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/container/di.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/container/protocol.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/container/rodi.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/dispatcher/__init__.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/dispatcher/default.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/dispatcher/dispatch_result.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/dispatcher/protocol.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/events/__init__.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/events/event.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/events/event_emitter.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/events/event_handler.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/events/map.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/message_brokers/__init__.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/message_brokers/azure.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/message_brokers/protocol.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/message_brokers/redis.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/middlewares/__init__.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/middlewares/base.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/middlewares/logging.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/requests/__init__.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/requests/map.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/requests/request.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 diator-0.1.2/src/diator/requests/request_handler.py
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 diator-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 diator-0.1.2/LICENSE.rst
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 diator-0.1.2/README.md
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 diator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 diator-0.1.2/PKG-INFO
```

### Comparing `diator-0.1.1/src/diator/mediator.py` & `diator-0.1.2/src/diator/mediator.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     """
 
     def __init__(
         self,
         request_map: RequestMap,
         container: Container,
-        event_emitter: EventEmitter,
+        event_emitter: EventEmitter | None = None,
         middleware_chain: MiddlewareChain | None = None,
         *,
         dispatcher_type: Type[Dispatcher] = DefaultDispatcher,
     ) -> None:
         self._event_emitter = event_emitter
         self._dispatcher = dispatcher_type(
             request_map=request_map, container=container, middleware_chain=middleware_chain  # type: ignore
@@ -52,10 +52,13 @@
 
         if dispatch_result.events:
             await self._send_events(dispatch_result.events.copy())
 
         return dispatch_result.response
 
     async def _send_events(self, events: list[Event]) -> None:
+        if not self._event_emitter:
+            return
+
         while events:
             event = events.pop()
             await self._event_emitter.emit(event)
```

### Comparing `diator-0.1.1/src/diator/response.py` & `diator-0.1.2/src/diator/response.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/container/di.py` & `diator-0.1.2/src/diator/container/di.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/container/rodi.py` & `diator-0.1.2/src/diator/container/rodi.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/dispatcher/default.py` & `diator-0.1.2/src/diator/dispatcher/default.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/events/event.py` & `diator-0.1.2/src/diator/events/event.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/events/event_emitter.py` & `diator-0.1.2/src/diator/events/event_emitter.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/events/event_handler.py` & `diator-0.1.2/src/diator/events/event_handler.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/events/map.py` & `diator-0.1.2/src/diator/events/map.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/message_brokers/azure.py` & `diator-0.1.2/src/diator/message_brokers/azure.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/message_brokers/protocol.py` & `diator-0.1.2/src/diator/message_brokers/protocol.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/message_brokers/redis.py` & `diator-0.1.2/src/diator/message_brokers/redis.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/middlewares/base.py` & `diator-0.1.2/src/diator/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/middlewares/logging.py` & `diator-0.1.2/src/diator/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/requests/map.py` & `diator-0.1.2/src/diator/requests/map.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/requests/request.py` & `diator-0.1.2/src/diator/requests/request.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/src/diator/requests/request_handler.py` & `diator-0.1.2/src/diator/requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/.gitignore` & `diator-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/LICENSE.rst` & `diator-0.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `diator-0.1.1/pyproject.toml` & `diator-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "diator"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name = "Murad Akhundov", email = "akhundov1murad@gmail.com" }]
 description = "Diator is a Python library for implementing CQRS pattern in your Python applications."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.10"
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -64,16 +64,24 @@
 
 [project.optional-dependencies]
 redis = ["redis"]
 azure = ["azure-servicebus"]
 test = [
   "pytest",
   "pytest-asyncio",
+  "types-redis",
+  "mkdocs",
+  "mkdocs-material",
+  "mkdocstrings",
   "black",
   "vulture",
   "mypy",
-  "types-redis",
   "isort",
+  "flake8",
+  "azure-servicebus",
+  "redis",
+  "di[anyio]",
+  "rodi",
 ]
 
 [tool.isort]
 profile = "black"
```

