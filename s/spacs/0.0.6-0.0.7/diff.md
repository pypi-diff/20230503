# Comparing `tmp/spacs-0.0.6.tar.gz` & `tmp/spacs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacs-0.0.6.tar", max compression
+gzip compressed data, was "spacs-0.0.7.tar", max compression
```

## Comparing `spacs-0.0.6.tar` & `spacs-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1093 2023-04-26 20:46:06.053000 spacs-0.0.6/LICENSE
--rw-r--r--   0        0        0      418 2023-05-02 00:12:34.769907 spacs-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1763 2023-05-01 18:22:46.781118 spacs-0.0.6/README.md
--rw-r--r--   0        0        0      184 2023-05-01 15:11:43.780995 spacs-0.0.6/spacs/__init__.py
--rw-r--r--   0        0        0     8008 2023-05-01 23:51:14.334661 spacs-0.0.6/spacs/client.py
--rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 spacs-0.0.6/setup.py
--rw-r--r--   0        0        0     2172 1970-01-01 00:00:00.000000 spacs-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-26 20:46:06.053000 spacs-0.0.7/LICENSE
+-rw-r--r--   0        0        0      418 2023-05-02 22:45:32.426000 spacs-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1763 2023-05-01 18:22:46.781118 spacs-0.0.7/README.md
+-rw-r--r--   0        0        0      184 2023-05-01 15:11:43.780995 spacs-0.0.7/spacs/__init__.py
+-rw-r--r--   0        0        0     8397 2023-05-02 22:42:09.370541 spacs-0.0.7/spacs/client.py
+-rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 spacs-0.0.7/setup.py
+-rw-r--r--   0        0        0     2172 1970-01-01 00:00:00.000000 spacs-0.0.7/PKG-INFO
```

### Comparing `spacs-0.0.6/LICENSE` & `spacs-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spacs-0.0.6/README.md` & `spacs-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `spacs-0.0.6/spacs/client.py` & `spacs-0.0.7/spacs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
+import json
 import logging
 from collections.abc import Callable
 from enum import StrEnum
-from typing import Any, ClassVar, Self, Awaitable, Type
+from typing import Any, Awaitable, ClassVar, Self, Type
 
 import aiohttp
 from aiohttp import ClientConnectorError, ClientResponse
 from pydantic import BaseModel
 
 ResponseModel = Type[BaseModel] | None
 ModelContent = BaseModel | list[BaseModel]
@@ -108,15 +109,15 @@
             "path": request.path,
         }
 
         try:
             async with action(
                 request.path,
                 params=request.params,
-                json=request.body,
+                data=request.body,
                 headers=request.headers,
             ) as response:
                 end_time = datetime.datetime.now(tz=datetime.timezone.utc)
                 self._logger.debug(
                     {
                         "msg": "Request completed",
                         **base_log_info,
@@ -153,14 +154,21 @@
         if result.headers is None:
             result.headers = {}
 
         result.headers["Content-Type"] = result.content_type.value
         result.path = self._build_path(result.path)
         result.params = self._prepare_content(result.params)
         result.body = self._prepare_content(result.body)
+
+        # All request actions pass the `data` kwarg instead of `json` to
+        # simplify the API, so when we specify that `application/json` is the
+        # `content-type`, automatically stringify/encode the payload.
+        if result.body is not None and result.content_type == ContentType.JSON:
+            result.body = json.dumps(result.body).encode("utf-8")
+
         return result
 
     def _build_path(self, path: str) -> str:
         result = f"/{path.strip('/')}"
         if self.path_prefix:
             result = f"/{self.path_prefix}{result}"
         return result
```

### Comparing `spacs-0.0.6/setup.py` & `spacs-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'spacs',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'Simple Pydantic AIOHTTP Client Sessions',
     'long_description': '# SPACS: Simple Pydantic AIOHTTP Client Sessions\n\nA package to assist in managing and using long-lived AIOHTTP client sessions with simplicity. Built to handle Pydantic objects.\n\n## Features\n\n- Handles request params and bodies as either Pydantic objects or native Python dictionaries, converting items to JSON-safe format.\n- Abstracts away internals of managing the request/response objects, instead either returning parsed response content on success, or raising a specialized error object.\n- Automatically manages persistent connections to be shared over extended lifespan across application, cleaning up all open connections on teardown.\n- Utilizes modern Python type hinting.\n\n## Installation\n\nUsing poetry (preferred):\n\n```bash\npoetry add spacs\n```\n\nUsing pip:\n\n```bash\npip install spacs\n```\n\n## Usage\n\n```python\nfrom spacs import SpacsClient, SpacsRequest, SpacsRequestError\nfrom pydantic import BaseModel\n\n...\n\nexample_client = SpacsClient(base_url="http://example.com")\n\n# Basic request with error handling\ntry:\n    request = SpacsRequest(path="/fruit/apple", params={"cultivar": "honeycrisp"})\n    apples = await example_client.get(request)\nexcept SpacsRequestError as error:\n    print({"code": error.status_code, "reason": error.reason})\n\n# Sending Pydantic objects via HTTP POST\nclass MyModel(BaseModel):\n    name: str\n    age: int\n\nexample_object = MyModel(name="James", age=25)\nrequest = SpacsRequest(path="/person", body=example_object, response_model=MyModel)\ncreated_person = await example_client.post(request)\n\n# Manually closing a session\nawait example_client.close()\n# Alternatively, to close all open sessions:\nawait SpacsClient.close_all()\n```\n\n## Building\n\n```\npoetry build\n```\n',
     'author': 'rlebel12',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rlebel12/spacs',
```

### Comparing `spacs-0.0.6/PKG-INFO` & `spacs-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacs
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple Pydantic AIOHTTP Client Sessions
 Home-page: https://github.com/rlebel12/spacs
 Author: rlebel12
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
```

