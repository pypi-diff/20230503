# Comparing `tmp/pypawapi-1.2.0.tar.gz` & `tmp/pypawapi-2.0.0.tar.gz`

## Comparing `pypawapi-1.2.0.tar` & `pypawapi-2.0.0.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pypawapi-1.2.0/setup.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/__init__.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/abc.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/client.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/exceptions.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/interval.py
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/pawapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/py.typed
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/python.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/region.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/response.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/shell.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/system.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/version.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/api/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/api/base.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/api/console.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/api/cpu.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/api/file.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/api/python.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/api/students.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/api/system.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/api/task.py
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 pypawapi-1.2.0/src/pawapi/api/webapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawapi-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pypawapi-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pypawapi-1.2.0/tests/test_alwayson_task.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 pypawapi-1.2.0/tests/test_client.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 pypawapi-1.2.0/tests/test_console.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pypawapi-1.2.0/tests/test_cpu.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 pypawapi-1.2.0/tests/test_file.py
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 pypawapi-1.2.0/tests/test_python.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 pypawapi-1.2.0/tests/test_scheduled_task.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pypawapi-1.2.0/tests/test_shell.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pypawapi-1.2.0/tests/test_students.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pypawapi-1.2.0/tests/test_system.py
--rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 pypawapi-1.2.0/tests/test_webapp.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pypawapi-1.2.0/.gitignore
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 pypawapi-1.2.0/LICENSE
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 pypawapi-1.2.0/README.md
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 pypawapi-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 pypawapi-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 pypawapi-2.0.0/setup.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/__init__.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/client.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/exceptions.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/interval.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/pawapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/py.typed
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/python.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/region.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/shell.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/system.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/version.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/api/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/api/_types.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/api/base.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/api/console.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/api/cpu.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/api/file.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/api/python.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/api/students.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/api/system.py
+-rw-r--r--   0        0        0     6211 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/api/task.py
+-rw-r--r--   0        0        0    11767 2020-02-02 00:00:00.000000 pypawapi-2.0.0/src/pawapi/api/webapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypawapi-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pypawapi-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 pypawapi-2.0.0/tests/test_alwayson_task.py
+-rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 pypawapi-2.0.0/tests/test_client.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 pypawapi-2.0.0/tests/test_console.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pypawapi-2.0.0/tests/test_cpu.py
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 pypawapi-2.0.0/tests/test_file.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pypawapi-2.0.0/tests/test_python.py
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 pypawapi-2.0.0/tests/test_scheduled_task.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 pypawapi-2.0.0/tests/test_shell.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pypawapi-2.0.0/tests/test_students.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 pypawapi-2.0.0/tests/test_system.py
+-rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 pypawapi-2.0.0/tests/test_webapp.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pypawapi-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 pypawapi-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 pypawapi-2.0.0/README.md
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 pypawapi-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 pypawapi-2.0.0/PKG-INFO
```

### Comparing `pypawapi-1.2.0/src/pawapi/client.py` & `pypawapi-2.0.0/src/pawapi/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,56 @@
+from __future__ import annotations
+
 __all__ = ["Client"]
 
+from dataclasses import dataclass
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import requests
 
-from .abc import AbstractClient
+from .exceptions import BadRequestError
 from .exceptions import InvalidJSONError
 from .exceptions import InvalidTokenError
 from .exceptions import NotFoundError
 from .exceptions import PermissionDeniedError
 from .exceptions import RequestTimeoutError
 from .exceptions import StatusError
 from .region import Region
-from .response import Content
-from .response import Response
-from .utils import validate_credentials
+
+Content = Union[Dict[str, Union[str, int, bytes]], bytes]
 
 
-class Client(AbstractClient):
+class Client:
+    """Http client.
+
+    :param username: PythonAnywhere username.
+    :param token: API token.
+    :param region: Account region.
+    :param timeout: Request timeout.
+    """
 
     __slots__ = (
         "_url",
         "_headers",
-        "_raise_404",
         "_timeout",
     )
 
     def __init__(
         self,
         username: str,
         token: str,
         region: Region,
-        raise_404: bool,
         timeout: float,
     ) -> None:
-        validate_credentials("username", username)
-        validate_credentials("token", token)
-        prefix = "eu" if region == Region.EU else "www"
-        self._url = f"https://{prefix}.pythonanywhere.com/api/v0/user/{username}"  # noqa: E501
+        self._url = "https://{}.pythonanywhere.com/api/v0/user/{}".format(
+            "eu" if region is Region.EU else "www", username
+        )
         self._headers = {"Authorization": f"Token {token}"}
-        self._raise_404 = raise_404
         self._timeout = timeout
 
     def _request(
         self,
         method: str,
         path: str,
         *,
@@ -64,70 +69,59 @@
                 timeout=self._timeout,
             )
         except requests.Timeout:
             raise RequestTimeoutError(
                 f"Request timed out (timeout={self._timeout})"
             ) from None
 
-        return self._check_response(response)
+        if response.status_code >= 300:
+            self._raise_for_status(response)
 
-    def _check_status(self, response: requests.Response) -> None:
-        status = response.status_code
-        if status >= 400:
-            try:
-                json = response.json()
-                error = json.get("error", None)
-                detail = json.get("detail", None)
-                description = error if error is not None else detail
-            except requests.JSONDecodeError:
-                description = None
-
-            if status == 401:
-                raise InvalidTokenError(
-                    status_code=401,
-                    description=description,
-                    raw_content=response.content,
-                )
-            elif status == 403:
-                raise PermissionDeniedError(
-                    status_code=403,
-                    description=description,
-                    raw_content=response.content,
-                )
-            elif status == 404:
-                if self._raise_404:
-                    raise NotFoundError(
-                        status_code=404,
-                        description=description,
-                        raw_content=response.content,
-                    )
-            else:
-                raise StatusError(
-                    status_code=status,
-                    description=description,
-                    raw_content=response.content
-                )
+        return self._parse_content(response)
 
-    def _check_response(self, response: requests.Response) -> Response:
-        self._check_status(response)
+    def _raise_for_status(self, response: requests.Response) -> None:
+        try:
+            json = response.json()
+        except requests.JSONDecodeError:
+            json = {}
+
+        status_code = response.status_code
+        details = {
+            "status_code": status_code,
+            "description": json.get("error") or json.get("detail"),
+            "raw_content": response.content,
+        }
+
+        if status_code == 400:
+            raise BadRequestError(**details)
+        elif status_code == 401:
+            raise InvalidTokenError(**details)
+        elif status_code == 401:
+            raise InvalidTokenError(**details)
+        elif status_code == 403:
+            raise PermissionDeniedError(**details)
+        elif status_code == 404:
+            raise NotFoundError(**details)
+        else:
+            raise StatusError(**details)
+
+    def _parse_content(self, response: requests.Response) -> Response:
         content: Optional[Content] = None
         content_type = response.headers.get("Content-Type", None)
-        if content_type is not None:
-            if response.content:
-                # response from /webapps with "text/json" in Content-Type
-                if ("application/json" in content_type
-                        or "text/json" in content_type):  # noqa: W503
-                    try:
-                        content = response.json()
-                    except requests.JSONDecodeError:
-                        raise InvalidJSONError(
-                            f"Got invalid json: {response.content!r}"
-                        ) from None
-                elif "application/octet-stream" in content_type:
-                    content = response.content
+        if response.content and content_type is not None:
+            # response from /webapps with "text/json" in Content-Type
+            if "/json" in content_type:  # json
+                try:
+                    content = response.json()
+                except requests.JSONDecodeError:
+                    raise InvalidJSONError(
+                        f"Got invalid json: {response.content!r}"
+                    ) from None
+            elif "application/octet-stream" in content_type:  # file
+                content = response.content
         return Response(status=response.status_code, content=content)
 
     def get(
         self,
         path: str,
         params: Optional[Dict[str, Optional[Union[str, int]]]] = None,
     ) -> Response:
@@ -151,7 +145,13 @@
 
     def delete(
         self,
         path: str,
         params: Optional[Dict[str, Optional[Union[str, int]]]] = None,
     ) -> Response:
         return self._request("delete", path, params=params)
+
+
+@dataclass(frozen=True)
+class Response:
+    status: int
+    content: Optional[Content] = None
```

### Comparing `pypawapi-1.2.0/src/pawapi/exceptions.py` & `pypawapi-2.0.0/src/pawapi/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,19 @@
+from __future__ import annotations
+
 from typing import Optional
 
 
 class PythonAnywhereAPIException(Exception):
-    """ Base server side exception """
+    """Base server side exception.
+
+    :param status_code: HTTP status code.
+    :param description: Error description.
+    :param raw_content: Raw response content.
+    """
 
     def __init__(
         self,
         status_code: int,
         description: Optional[str] = None,
         raw_content: Optional[bytes] = None,
     ) -> None:
@@ -25,37 +32,41 @@
                 self.status_code,
                 self.description,
                 self.raw_content,
             ),
         )
 
 
+class BadRequestError(PythonAnywhereAPIException):
+    """Invalid request (status code 400)"""
+
+
 class InvalidTokenError(PythonAnywhereAPIException):
-    """ Invalid API token (status code 401) """
+    """Invalid API token (status code 401)"""
 
 
 class PermissionDeniedError(PythonAnywhereAPIException):
-    """ Wrong username or somthing else (status code 403) """
+    """Wrong username or somthing else (status code 403)"""
 
 
 class NotFoundError(PythonAnywhereAPIException):
-    """ Path not found (status code 404) """
+    """Path not found (status code 404)"""
 
 
 class StatusError(PythonAnywhereAPIException):
-    """ Status code >= 400 (except 401, 403, 404) """
+    """Status code >= 400 (except 401, 403, 404)"""
 
 
 class PawapiException(Exception):
-    """ Base client side exception """
+    """Base client side exception"""
 
 
 class InvalidJSONError(PawapiException):
-    """ Error while parsing json response """
+    """Error while parsing json response"""
 
 
 class InvalidCredentialsError(PawapiException):
-    """ Username or Token has an invalid character """
+    """Username or Token has an invalid character"""
 
 
 class RequestTimeoutError(PawapiException):
-    """ Request timed out """
+    """Request timed out"""
```

### Comparing `pypawapi-1.2.0/src/pawapi/pawapi.py` & `pypawapi-2.0.0/src/pawapi/pawapi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,43 @@
+from __future__ import annotations
+
 __all__ = ["Pawapi"]
 
-from typing import TYPE_CHECKING
 from typing import Optional
 
 from .api import AlwaysOnTask
 from .api import Console
 from .api import Cpu
 from .api import File
 from .api import Python
 from .api import ScheduledTask
 from .api import Students
 from .api import System
 from .api import Webapp
 from .client import Client
 from .region import Region
-
-if TYPE_CHECKING:
-    from .abc import AbstractClient
+from .utils import validate_credentials
 
 
 class Pawapi:
+    """Main `pawapi` object.
+
+    Usage::
+
+        token = '<your_token>'
+        user = '<your_username>'
+
+        api = Pawapi(user, token)
+        print(api.cpu.get_info())
+
+    :param username: PythonAnywhere username.
+    :param token: API token.
+    :param region: Account region.
+    :param timeout: Request timeout.
+    """
 
     __slots__ = (
         "_username",
         "_region",
         "_client",
         "_alwayson_task",
         "_console",
@@ -38,25 +52,26 @@
 
     def __init__(
         self,
         username: str,
         token: str,
         *,
         region: Region = Region.US,
-        raise_404: bool = True,
         timeout: float = 8,
     ) -> None:
+        validate_credentials("username", username)
+        validate_credentials("token", token)
+
         self._username = username
         self._region = region
 
-        self._client: "AbstractClient" = Client(
+        self._client = Client(
             username=username,
             token=token,
             region=region,
-            raise_404=raise_404,
             timeout=timeout,
         )
 
         self._alwayson_task: Optional[AlwaysOnTask] = None
         self._console: Optional[Console] = None
         self._cpu: Optional[Cpu] = None
         self._file: Optional[File] = None
@@ -78,58 +93,103 @@
 
     @property
     def region(self) -> Region:
         return self._region
 
     @property
     def console(self) -> Console:
+        """Console endpoint.
+
+        See: :class:`pawapi.api.Console`
+        """
+
         if self._console is None:
             self._console = Console(self._client)
         return self._console
 
     @property
     def cpu(self) -> Cpu:
+        """Cpu endpoint.
+
+        See: :class:`pawapi.api.Cpu`
+        """
+
         if self._cpu is None:
             self._cpu = Cpu(self._client)
         return self._cpu
 
     @property
     def file(self) -> File:
+        """File endpoint.
+
+        See: :class:`pawapi.api.File`
+        """
+
         if self._file is None:
             self._file = File(self._client)
         return self._file
 
     @property
     def python(self) -> Python:
+        """Python endpoint.
+
+        See: :class:`pawapi.api.Python`
+        """
+
         if self._python is None:
             self._python = Python(self._client)
         return self._python
 
     @property
     def scheduled_task(self) -> ScheduledTask:
+        """Scheduled task ednpoint.
+
+        See: :class:`pawapi.api.ScheduledTask`
+        """
+
         if self._scheduled_task is None:
             self._scheduled_task = ScheduledTask(self._client)
         return self._scheduled_task
 
     @property
     def students(self) -> Students:
+        """Students endpoint.
+
+        See: :class:`pawapi.api.Students`
+        """
+
         if self._students is None:
             self._students = Students(self._client)
         return self._students
 
     @property
     def system(self) -> System:
+        """System endpoint.
+
+        See: :class:`pawapi.api.System`
+        """
+
         if self._system is None:
             self._system = System(self._client)
         return self._system
 
     @property
     def alwayson_task(self) -> AlwaysOnTask:
+        """Always-On task endpoint
+
+        See: :class:`pawapi.api.AlwaysOnTask`
+        """
+
         if self._alwayson_task is None:
             self._alwayson_task = AlwaysOnTask(self._client)
         return self._alwayson_task
 
     @property
     def webapp(self) -> Webapp:
+        """Webapp endpoint.
+
+        See: :class:`pawapi.api.Webapp`
+        """
+
         if self._webapp is None:
             self._webapp = Webapp(self._client)
         return self._webapp
```

### Comparing `pypawapi-1.2.0/src/pawapi/utils.py` & `pypawapi-2.0.0/src/pawapi/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from .exceptions import InvalidCredentialsError
 
 
 def validate_credentials(name: str, value: str) -> None:
     if not isinstance(value, str):
         raise InvalidCredentialsError(
             f"{name} must be a str! {name} is {type(value)!r}"
```

### Comparing `pypawapi-1.2.0/src/pawapi/api/webapp.py` & `pypawapi-2.0.0/src/pawapi/api/task.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,262 +1,228 @@
-__all__ = ["Webapp"]
+from __future__ import annotations
 
+__all__ = [
+    "ScheduledTask",
+    "AlwaysOnTask",
+]
+
+from typing import List
 from typing import Optional
 from typing import Union
+from typing import cast
 
-from pawapi.python import Python2
-from pawapi.python import Python3
-from pawapi.response import Response
+from pawapi.interval import TaskInterval
 
+from ._types import Content
 from .base import BaseEndpoint
 
 
-class Webapp(BaseEndpoint):
-    __endpoint = "webapps"
+class ScheduledTask(BaseEndpoint):
+    """Scheduled task endpoint"""
+
+    __path = "schedule"
 
     __slots__ = ()
 
-    def list(self) -> Response:
-        """ List all webapps """
+    def list(self) -> List[Content]:
+        """List all tasks."""
 
-        return self._client.get(f"{self.__endpoint}/")
+        result = self._client.get(f"{self.__path}/")
+        return cast(List[Content], result.content)
 
     def create(
         self,
-        domain_name: str,
-        python_version: Union[Python2, Python3],
-    ) -> Response:
-        """ Create a new webapp with manual configuration """
+        command: str,
+        minute: Union[int, str],
+        *,
+        hour: Optional[Union[int, str]] = None,
+        enabled: bool = True,
+        interval: TaskInterval = TaskInterval.DAILY,
+        description: Optional[str] = None,
+    ) -> Content:
+        """Create a new task.
 
-        return self._client.post(
-            path="webapps/",
+        :param command: Command to execute.
+        :param minute: Start time (hourly task).
+        :param hour: Start time (daily task).
+        :param enabled: Enable task.
+        :param interval: Task start interval.
+        :param description: Task description.
+        :returns: Task information.
+        """
+
+        result = self._client.post(
+            path=f"{self.__path}/",
             data={
-                "domain_name": domain_name,
-                "python_version": python_version.format_value(dot=False),
+                "command": command,
+                "enabled": enabled,
+                "interval": interval.value,
+                "hour": hour,
+                "minute": minute,
+                "description": description,
             },
         )
+        return cast(Content, result.content)
+
+    def get_info(self, task_id: Union[int, str]) -> Content:
+        """Returns information about task.
 
-    def get_info(self, domain_name: str) -> Response:
-        """ Information about a web app's configuration """
+        :param task_id: Task id.
+        """
 
-        return self._client.get(f"{self.__endpoint}/{domain_name}/")
+        result = self._client.get(f"{self.__path}/{task_id}/")
+        return cast(Content, result.content)
 
     def update(
         self,
-        domain_name: str,
+        task_id: Union[int, str],
         *,
-        python_version: Optional[Union[Python2, Python3]] = None,
-        source_directory: Optional[str] = None,
-        virtualenv_path: Optional[str] = None,
-        force_https: Optional[bool] = None,
-        protection: Optional[bool] = None,
-        protection_username: Optional[str] = None,
-        protection_password: Optional[str] = None,
-    ) -> Response:
-        """ Modify configuration of a webapp
+        command: Optional[str] = None,
+        enabled: Optional[bool] = None,
+        interval: Optional[TaskInterval] = None,
+        hour: Optional[Union[int, str]] = None,
+        minute: Optional[Union[int, str]] = None,
+        description: Optional[str] = None,
+    ) -> Content:
+        """Update task.
 
-            NOTE: restart the webapp is required to apply the changes
+        :param task_id: Task id.
+        :param command: Command to execute.
+        :param minute: Start time (hourly task).
+        :param hour: Start time (daily task).
+        :param enabled: Enable task.
+        :param interval: Task start interval.
+        :param description: Task description.
+        :returns: Task information.
         """
 
-        pyver = None
-        if python_version is not None:
-            pyver = python_version.format_value(short=True)
-
-        return self._client.patch(
-            path=f"{self.__endpoint}/{domain_name}/",
+        result = self._client.patch(
+            path=f"{self.__path}/{task_id}/",
             data={
-                "python_version": pyver,
-                "source_directory": source_directory,
-                "virtualenv_path": virtualenv_path,
-                "force_https": force_https,
-                "password_protection_enabled": protection,
-                "password_protection_username": protection_username,
-                "password_protection_password": protection_password,
+                "command": command,
+                "enabled": enabled,
+                "interval": interval.value if interval is not None else None,
+                "hour": hour,
+                "minute": minute,
+                "description": description,
             },
         )
+        return cast(Content, result.content)
 
-    def delete(self, domain_name: str) -> Response:
-        """ Delete the webapp
+    def delete(self, task_id: Union[int, str]) -> bool:
+        """Stop and delete task.
 
-            NOTE: Config is backed up in /var/www, and your code is not touched
+        :param task_id: Task id.
+        :returns: True on success.
         """
 
-        return self._client.delete(f"{self.__endpoint}/{domain_name}/")
-
-    def enable(self, domain_name: str) -> Response:
-        """ Enable the webapp """
-
-        return self._client.post(f"{self.__endpoint}/{domain_name}/enable/")
-
-    def disable(self, domain_name: str) -> Response:
-        """ Disable the webapp """
-
-        return self._client.post(f"{self.__endpoint}/{domain_name}/disable/")
-
-    def reload(self, domain_name: str) -> Response:
-        """ Reload the webapp """
+        result = self._client.delete(f"{self.__path}/{task_id}/")
+        return result.status == 204
 
-        return self._client.post(f"{self.__endpoint}/{domain_name}/reload/")
 
-    def get_ssl_info(self, domain_name: str) -> Response:
-        """ Information about webapp's SSL """
+class AlwaysOnTask(BaseEndpoint):
+    """Always-on task endpoint"""
 
-        return self._client.get(f"{self.__endpoint}/{domain_name}/ssl/")
+    __path = "always_on"
 
-    def add_ssl(
-        self,
-        domain_name: str,
-        cert: str,
-        private_key: str,
-    ) -> Response:
-        """ Set SSL cert for webapp """
-
-        return self._client.post(
-            path=f"{self.__endpoint}/{domain_name}/ssl/",
-            data={
-                "cert": cert,
-                "private_key": private_key,
-            },
-        )
-
-    def delete_ssl(self, domain_name: str) -> Response:
-        """ Delete webapp's SSL """
-
-        return self._client.delete(f"{self.__endpoint}/{domain_name}/ssl/")
+    __slots__ = ()
 
-    def list_static_files(self, domain_name: str) -> Response:
-        """ List all the static files mappings for a domain """
+    def list(self) -> List[Content]:
+        """List all tasks."""
 
-        return self._client.get(
-            f"{self.__endpoint}/{domain_name}/static_files/"
-        )
+        result = self._client.get(f"{self.__path}/")
+        return cast(List[Content], result.content)
 
-    def add_static_file(
+    def create(
         self,
-        domain_name: str,
-        url: str,
-        path: str,
-    ) -> Response:
-        """ Create a new static files mapping
+        command: str,
+        *,
+        enabled: bool = True,
+        description: Optional[str] = None,
+    ) -> Content:
+        """Create a new task.
 
-            NOTE: webapp restart required
+        :param command: Command to execute.
+        :param enabled: Enable task.
+        :param description: Task description.
+        :returns: Task information.
         """
 
-        return self._client.post(
-            path=f"{self.__endpoint}/{domain_name}/static_files/",
+        result = self._client.post(
+            path=f"{self.__path}/",
             data={
-                "url": url,
-                "path": path,
+                "command": command,
+                "description": description,
+                "enabled": enabled,
             },
         )
+        return cast(Content, result.content)
 
-    def get_static_file_info(self, domain_name: str, file_id: int) -> Response:
-        """ URL and path of a particular mapping """
+    def get_info(self, task_id: Union[int, str]) -> Content:
+        """Returns information about task."""
 
-        return self._client.get(
-            f"{self.__endpoint}/{domain_name}/static_files/{file_id}/"
-        )
+        result = self._client.get(f"{self.__path}/{task_id}/")
+        return cast(Content, result.content)
 
-    def update_static_file(
+    def update(
         self,
-        domain_name: str,
-        file_id: int,
-        url: str,
-        path: str,
-    ) -> Response:
-        """ Modify a static files mapping
+        task_id: Union[int, str],
+        *,
+        command: Optional[str] = None,
+        description: Optional[str] = None,
+        enabled: Optional[bool] = None,
+    ) -> Content:
+        """Update task.
 
-            NOTE: webapp restart required
+        :param task_id: Task id.
+        :param command: Command to execute.
+        :param enabled: Enable task.
+        :param description: Task description.
+        :returns: Task information.
         """
 
-        return self._client.patch(
-            path=f"{self.__endpoint}/{domain_name}/static_files/{file_id}/",
+        result = self._client.patch(
+            path=f"{self.__path}/{task_id}/",
             data={
-                "url": url,
-                "path": path,
+                "command": command,
+                "description": description,
+                "enabled": enabled,
             },
         )
+        return cast(Content, result.content)
 
-    def delete_static_file(self, domain_name: str, file_id: int) -> Response:
-        """ Remove a static files mapping
+    def delete(self, task_id: Union[int, str]) -> bool:
+        """Stop and delete task.
 
-            NOTE: webapp restart required
+        :param task_id: Task id.
+        :returns: True on success.
         """
 
-        return self._client.delete(
-            f"{self.__endpoint}/{domain_name}/static_files/{file_id}/"
-        )
-
-    def list_static_headers(self, domain_name: str) -> Response:
-        """ List all the static headers for a domain """
+        result = self._client.delete(f"{self.__path}/{task_id}/")
+        return result.status == 204
 
-        return self._client.get(
-            f"{self.__endpoint}/{domain_name}/static_headers/"
-        )
-
-    def add_static_header(
+    def restart(
         self,
-        domain_name: str,
-        url: str,
-        name: str,
-        value: str,
-    ) -> Response:
-        """ Create a new static header
-
-            NOTE: webapp restart required
-        """
-
-        return self._client.post(
-            path=f"{self.__endpoint}/{domain_name}/static_headers/",
-            data={
-                "url": url,
-                "name": name,
-                "value": value,
-            },
-        )
-
-    def get_static_header_info(
-        self,
-        domain_name: str,
-        header_id: int,
-    ) -> Response:
-        """ URL, name and value of a particular header """
-
-        return self._client.get(
-            f"{self.__endpoint}/{domain_name}/static_headers/{header_id}/"
-        )
-
-    def update_static_header(
-        self,
-        domain_name: str,
-        header_id: int,
-        url: str,
-        name: str,
-        value: str,
-    ) -> Response:
-        """ Modify a static header
+        task_id: Union[int, str],
+        *,
+        command: Optional[str] = None,
+        description: Optional[str] = None,
+        enabled: Optional[bool] = None,
+    ) -> Content:
+        """Restart task.
 
-            NOTE: webapp restart required
+        :param task_id: Task id.
+        :param command: Command to execute.
+        :param enabled: Enable task.
+        :param description: Task description.
+        :returns: Task information
         """
 
-        return self._client.patch(
-            path=f"{self.__endpoint}/{domain_name}/static_headers/{header_id}/",
+        result = self._client.post(
+            path=f"{self.__path}/{task_id}/restart/",
             data={
-                "url": url,
-                "name": name,
-                "value": value,
+                "command": command,
+                "description": description,
+                "enabled": enabled,
             },
         )
-
-    def delete_static_header(
-        self,
-        domain_name: str,
-        header_id: int,
-    ) -> Response:
-        """ Remove a static header
-
-            NOTE: webapp restart required
-        """
-
-        return self._client.delete(
-            f"{self.__endpoint}/{domain_name}/static_headers/{header_id}/"
-        )
+        return cast(Content, result.content)
```

### Comparing `pypawapi-1.2.0/tests/conftest.py` & `pypawapi-2.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pypawapi-1.2.0/tests/test_alwayson_task.py` & `pypawapi-2.0.0/tests/test_alwayson_task.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,49 +42,64 @@
             url=f"{self.url}/always_on/",
             match=(
                 urlencoded_params_matcher({
                     k: str(v)
                     for k, v in params_create.items()
                 }),
             ),
+            json={},
         )
-        self.api.alwayson_task.create(**params_create)
+        res = self.api.alwayson_task.create(**params_create)
+        assert isinstance(res, dict), res
 
     def test_info(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.get(f"{self.url}/always_on/{self.task_id}/")
-        self.api.alwayson_task.get_info(self.task_id)
+        mock_responses.get(f"{self.url}/always_on/{self.task_id}/", json={})
+        res = self.api.alwayson_task.get_info(self.task_id)
+        assert isinstance(res, dict), res
 
     def test_update(
         self,
         mock_responses: 'RequestsMock',
         params_update: Dict[str, Any],
     ) -> None:
         mock_responses.patch(
             url=f"{self.url}/always_on/{self.task_id}/",
             match=(
                 urlencoded_params_matcher({
                     k: str(v)
                     for k, v in params_update.items()
                 }),
             ),
+            json={},
         )
-        self.api.alwayson_task.update(task_id=self.task_id, **params_update)
+        res = self.api.alwayson_task.update(
+            task_id=self.task_id,
+            **params_update,
+        )
+        assert isinstance(res, dict), res
 
     def test_delete(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.delete(f"{self.url}/always_on/{self.task_id}/")
-        self.api.alwayson_task.delete(self.task_id)
+        mock_responses.delete(
+            f"{self.url}/always_on/{self.task_id}/", status=204
+        )
+        assert self.api.alwayson_task.delete(self.task_id)
 
     def test_restart(
         self,
         mock_responses: 'RequestsMock',
         params_update: Dict[str, Any],
     ) -> None:
         mock_responses.post(
             url=f"{self.url}/always_on/{self.task_id}/restart/",
             match=(
                 urlencoded_params_matcher({
                     k: str(v)
                     for k, v in params_update.items()
                 }),
             ),
+            json={},
+        )
+        res = self.api.alwayson_task.restart(
+            task_id=self.task_id,
+            **params_update,
         )
-        self.api.alwayson_task.restart(task_id=self.task_id, **params_update)
+        assert isinstance(res, dict)
```

### Comparing `pypawapi-1.2.0/tests/test_client.py` & `pypawapi-2.0.0/tests/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import TYPE_CHECKING
 from typing import Union
 
 import pytest
 from requests.exceptions import Timeout
 from responses.matchers import header_matcher
 
-from pawapi.abc import AbstractClient
 from pawapi.client import Client
 from pawapi.exceptions import InvalidCredentialsError
 from pawapi.exceptions import InvalidTokenError
 from pawapi.exceptions import NotFoundError
 from pawapi.exceptions import PermissionDeniedError
 from pawapi.exceptions import RequestTimeoutError
 from pawapi.exceptions import StatusError
@@ -18,16 +17,16 @@
 from pawapi.utils import validate_credentials
 
 if TYPE_CHECKING:
     from respsonses import RequestsMock
 
 
 @pytest.fixture(scope="class")
-def client(test_user: str, test_token: str) -> AbstractClient:
-    return Client(test_user, test_token, Region.US, False, 8)
+def client(test_user: str, test_token: str) -> Client:
+    return Client(test_user, test_token, Region.US, 8)
 
 
 def test_region() -> None:
     assert Region.US.value == "us"
     assert Region.EU.value == "eu"
 
 
@@ -87,31 +86,28 @@
         region: Region,
         url: str,
     ) -> None:
         client = Client(
             test_user,
             test_token,
             region=region,
-            raise_404=False,
             timeout=8,
         )
         assert client._url == url + test_user
 
-    def test_api_auth_header(
-        self, client: AbstractClient, test_token: str
-    ) -> None:
+    def test_api_auth_header(self, client: Client, test_token: str) -> None:
         assert client._headers.get(
             "Authorization", None
         ) == f"Token {test_token}"
 
     @pytest.mark.parametrize("content_type", ("application/json", "text/json"))
     def test_response_json(
         self,
         mock_responses: 'RequestsMock',
-        client: AbstractClient,
+        client: Client,
         test_token: str,
         content_type: str,
     ) -> None:
         json_params = {
             "list": [1, 2, 3, 4],
             "dict": {
                 "key1": "value1",
@@ -137,15 +133,15 @@
             ("application/json", b"", None),
             ("text/html", b"<h>html here</h>", None),
         )
     )
     def test_response_content(
         self,
         mock_responses: 'RequestsMock',
-        client: AbstractClient,
+        client: Client,
         content_type: str,
         test_token: str,
         body: bytes,
         result: Union[bytes, None],
     ) -> None:
         mock_responses.get(
             url=f"{client._url}/content/",
@@ -155,15 +151,15 @@
         )
         resp = client.get("content/")
         assert resp.content == result
 
     def test_response_error_401(
         self,
         mock_responses: 'RequestsMock',
-        client: AbstractClient,
+        client: Client,
         test_token: str,
     ) -> None:
         url = "access401/"
         error = "Invalid token."
         mock_responses.get(
             url=f"{client._url}/{url}",
             json={"detail": error},
@@ -172,69 +168,68 @@
         )
         with pytest.raises(InvalidTokenError, match=f"401, {error}"):
             client.get(url)
 
     def test_response_error_403(
         self,
         mock_responses: 'RequestsMock',
-        client: AbstractClient,
+        client: Client,
     ) -> None:
         url = "access403/"
         error = "permission error details"
         mock_responses.get(
             url=f"{client._url}/{url}",
             json={"detail": error},
             status=403,
         )
         with pytest.raises(PermissionDeniedError, match=f"403, {error}"):
             client.get(url)
 
-    @pytest.mark.parametrize("status", (201, 204, 404))
+    @pytest.mark.parametrize("status", (201, 204))
     def test_response(
         self,
         mock_responses: 'RequestsMock',
-        client: AbstractClient,
+        client: Client,
         status: int,
     ) -> None:
         mock_responses.get(url=f"{client._url}/access/", status=status)
         response = client.get("access/")
         assert response.status == status
 
     def test_response_raise_404(
         self,
         mock_responses: 'RequestsMock',
-        client: AbstractClient,
+        client: Client,
     ) -> None:
-        client._raise_404 = True
         mock_responses.get(url=f"{client._url}/access/", status=404)
         with pytest.raises(NotFoundError):
             client.get("access/")
 
     def test_response_raise_timeout_eror(
         self,
         mock_responses: 'RequestsMock',
-        client: AbstractClient,
+        client: Client,
     ) -> None:
         mock_responses.get(url=f"{client._url}/timeout/", body=Timeout())
         with pytest.raises(RequestTimeoutError):
             client.get("timeout/")
 
     def test_response_raise_status_empty(
         self,
         mock_responses: 'RequestsMock',
-        client: AbstractClient,
+        client: Client,
     ) -> None:
-        mock_responses.get(url=f"{client._url}/status/", status=400)
-        with pytest.raises(StatusError, match="400"):
+        mock_responses.get(url=f"{client._url}/status/", status=500)
+        with pytest.raises(StatusError, match="500"):
             client.get("status/")
 
     def test_response_raise_status_description(
         self,
         mock_responses: 'RequestsMock',
-        client: AbstractClient,
+        client: Client,
     ) -> None:
         mock_responses.get(
             url=f"{client._url}/status/",
             status=418,
             json={"error": "I'm a teapot"},
         )
         with pytest.raises(StatusError, match="418, I'm a teapot"):
```

### Comparing `pypawapi-1.2.0/tests/test_console.py` & `pypawapi-2.0.0/tests/test_console.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import TYPE_CHECKING
 from typing import Dict
 from typing import Union
 
 import pytest
 from responses.matchers import urlencoded_params_matcher
 
-from pawapi.python import Python3
 from pawapi.shell import Shell
 
 if TYPE_CHECKING:
     from responses import RequestsMock
 
 
 @pytest.fixture
@@ -25,75 +24,109 @@
     return request.param
 
 
 @pytest.mark.usefixtures("paw_api_client")
 class TestConsole:
 
     def test_list(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.get(f"{self.url}/consoles/")
-        self.api.console.list()
+        mock_responses.get(
+            f"{self.url}/consoles/",
+            body=b"[]",
+            content_type="appclication/json",
+        )
+        res = self.api.console.list()
+        assert isinstance(res, list), res
 
     def test_list_shared(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.get(f"{self.url}/consoles/shared_with_you/")
-        self.api.console.list_shared()
+        mock_responses.get(
+            f"{self.url}/consoles/shared_with_you/",
+            body=b"[]",
+            content_type="appclication/json",
+        )
+        res = self.api.console.list_shared()
+        assert isinstance(res, list), res
 
     def test_create_python3(
         self, mock_responses: 'RequestsMock', params_create: Dict[str, str]
     ) -> None:
         mock_responses.post(
             url=f"{self.url}/consoles/",
             match=(urlencoded_params_matcher({**params_create}), ),
+            json={},
+            status=201,
+        )
+        params_create["executable"] = Shell(params_create["executable"])
+        res = self.api.console.create(**params_create)
+        assert isinstance(res, dict), res
+
+    def test_create_fail(
+        self, mock_responses: 'RequestsMock', params_create: Dict[str, str]
+    ) -> None:
+        mock_responses.post(
+            url=f"{self.url}/consoles/",
+            match=(urlencoded_params_matcher({**params_create}), ),
         )
-        params_create["executable"] = Python3(params_create["executable"])
-        self.api.console.create(**params_create)
+        params_create["executable"] = Shell(params_create["executable"])
+        res = self.api.console.create(**params_create)
+        assert res is None
 
     def test_create_bash(
         self, mock_responses: 'RequestsMock', params_create: Dict[str, str]
     ) -> None:
         params_create["executable"] = "bash"
         mock_responses.post(
             url=f"{self.url}/consoles/",
             match=(urlencoded_params_matcher({**params_create}), ),
+            json={},
+            status=201,
         )
         params_create["executable"] = Shell(params_create["executable"])
-        self.api.console.create(**params_create)
+        res = self.api.console.create(**params_create)
+        assert isinstance(res, dict), res
 
     def test_create_with_args(
         self, mock_responses: 'RequestsMock', params_create: Dict[str, str]
     ) -> None:
         params_create["arguments"] = "--useful-arg"
         mock_responses.post(
             url=f"{self.url}/consoles/",
             match=(urlencoded_params_matcher({**params_create}), ),
+            json={},
+            status=201,
         )
-        params_create["executable"] = Python3(params_create["executable"])
-        self.api.console.create(**params_create)
+        params_create["executable"] = Shell(params_create["executable"])
+        res = self.api.console.create(**params_create)
+        assert isinstance(res, dict), res
 
     def test_info(
         self, mock_responses: 'RequestsMock', console_id: int
     ) -> None:
-        mock_responses.get(f"{self.url}/consoles/{console_id}/")
-        self.api.console.get_info(console_id)
+        mock_responses.get(f"{self.url}/consoles/{console_id}/", json={})
+        res = self.api.console.get_info(console_id)
+        assert isinstance(res, dict), res
 
     def test_kill(
         self, mock_responses: 'RequestsMock', console_id: int
     ) -> None:
-        mock_responses.delete(f"{self.url}/consoles/{console_id}/")
-        self.api.console.kill(console_id)
+        mock_responses.delete(f"{self.url}/consoles/{console_id}/", status=204)
+        assert self.api.console.kill(console_id)
 
     def test_get_output(
         self, mock_responses: 'RequestsMock', console_id: int
     ) -> None:
+        output = "hello world!\n"
         mock_responses.get(
-            f"{self.url}/consoles/{console_id}/get_latest_output/"
+            f"{self.url}/consoles/{console_id}/get_latest_output/",
+            json={"output": output}
         )
-        self.api.console.get_output(console_id)
+        assert self.api.console.get_output(console_id) == output
 
     def test_send_input(
         self, mock_responses: 'RequestsMock', console_id: int
     ) -> None:
         console_input = "echo 123"
         mock_responses.post(
             url=f"{self.url}/consoles/{console_id}/send_input/",
             match=(urlencoded_params_matcher({"input": console_input}), ),
+            json={"status": "OK"},
         )
-        self.api.console.send_input(console_id, input_=console_input)
+        assert self.api.console.send_input(console_id, command=console_input)
```

### Comparing `pypawapi-1.2.0/tests/test_python.py` & `pypawapi-2.0.0/tests/test_python.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,50 +10,62 @@
     from responses import RequestsMock
 
 
 @pytest.mark.usefixtures("paw_api_client")
 class TestPython:
 
     def test_get_python_version(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.get(f"{self.url}/default_python_version/")
-        self.api.python.get_python_version()
+        mock_responses.get(f"{self.url}/default_python_version/", json={})
+        res = self.api.python.get_python_version()
+        assert isinstance(res, dict)
 
     def test_set_python_version(self, mock_responses: 'RequestsMock') -> None:
         mock_responses.patch(
             url=f"{self.url}/default_python_version/",
             match=(
                 urlencoded_params_matcher({"default_python_version": "2.7"}),
             ),
+            json={},
         )
-        self.api.python.set_python_version(Python2.PYTHON27)
+        res = self.api.python.set_python_version(Python2.PYTHON27)
+        assert isinstance(res, dict), res
 
     def test_get_python3_version(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.get(f"{self.url}/default_python3_version/")
-        self.api.python.get_python3_version()
+        mock_responses.get(f"{self.url}/default_python3_version/", json={})
+        res = self.api.python.get_python3_version()
+        assert isinstance(res, dict), res
 
     def test_set_python3_version(self, mock_responses: 'RequestsMock') -> None:
         mock_responses.patch(
             url=f"{self.url}/default_python3_version/",
             match=(
                 urlencoded_params_matcher({"default_python3_version": "3.8"}),
             ),
+            json={},
         )
-        self.api.python.set_python3_version(Python3.PYTHON38)
+        res = self.api.python.set_python3_version(Python3.PYTHON38)
+        assert isinstance(res, dict), res
 
     def test_get_python_sar_version(
         self, mock_responses: 'RequestsMock'
     ) -> None:
-        mock_responses.get(f"{self.url}/default_save_and_run_python_version/")
-        self.api.python.get_sar_version()
+        mock_responses.get(
+            f"{self.url}/default_save_and_run_python_version/",
+            json={},
+        )
+        res = self.api.python.get_sar_version()
+        assert isinstance(res, dict), res
 
     def test_set_python_sar_version(
         self, mock_responses: 'RequestsMock'
     ) -> None:
         mock_responses.patch(
             url=f"{self.url}/default_save_and_run_python_version/",
             match=(
                 urlencoded_params_matcher({
                     "default_save_and_run_python_version": "3.7",
                 }),
             ),
+            json={},
         )
-        self.api.python.set_sar_version(Python3.PYTHON37)
+        res = self.api.python.set_sar_version(Python3.PYTHON37)
+        assert isinstance(res, dict), res
```

### Comparing `pypawapi-1.2.0/tests/test_shell.py` & `pypawapi-2.0.0/tests/test_shell.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 from pawapi.python import Python3
 from pawapi.shell import Shell
 
 
 def test_console_executable() -> None:
     assert Shell.BASH.value == "bash"
     assert Shell.MYSQL.value == "mysql"
+    assert Shell.PYTHON310.value == "python3.10"
+    assert Shell.PYTHON39.value == "python3.9"
+    assert Shell.PYTHON38.value == "python3.8"
+    assert Shell.PYTHON37.value == "python3.7"
+    assert Shell.PYTHON36.value == "python3.6"
     assert Shell.IPYTHON310.value == "ipython3.10"
     assert Shell.IPYTHON39.value == "ipython3.9"
     assert Shell.IPYTHON38.value == "ipython3.8"
     assert Shell.IPYTHON37.value == "ipython3.7"
     assert Shell.IPYTHON36.value == "ipython3.6"
     assert Shell.PYPY2.value == "pypy2"
     assert Shell.PYPY3.value == "pypy3"
```

### Comparing `pypawapi-1.2.0/tests/test_students.py` & `pypawapi-2.0.0/tests/test_students.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     from responses import RequestsMock
 
 
 @pytest.mark.usefixtures("paw_api_client")
 class TestStudents:
 
     def test_list(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.get(f"{self.url}/students/")
-        self.api.students.list()
+        mock_responses.get(f"{self.url}/students/", json={})
+        res = self.api.students.list()
+        assert isinstance(res, list), res
 
     @pytest.mark.parametrize("student", ("student1", "anotherstudent2"))
     def test_delete(self, mock_responses: 'RequestsMock', student: str) -> None:
-        mock_responses.delete(f"{self.url}/students/{student}/")
-        self.api.students.delete(student)
+        mock_responses.delete(f"{self.url}/students/{student}/", status=204)
+        assert self.api.students.delete(student)
```

### Comparing `pypawapi-1.2.0/tests/test_system.py` & `pypawapi-2.0.0/tests/test_system.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,18 +17,21 @@
     assert SystemImage.HAGGIS.value == "haggis"
 
 
 @pytest.mark.usefixtures("paw_api_client")
 class TestSystem:
 
     def test_get_version(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.get(f"{self.url}/system_image/")
-        self.api.system.get_current_image()
+        mock_responses.get(f"{self.url}/system_image/", json={})
+        res = self.api.system.get_current_image()
+        assert isinstance(res, dict), res
 
     def test_set_version(self, mock_responses: 'RequestsMock') -> None:
         mock_responses.patch(
             url=f"{self.url}/system_image/",
             match=(
                 urlencoded_params_matcher({"system_image": "glastonbury"}),
             ),
+            json={},
         )
-        self.api.system.set_image(SystemImage.GLASTONBURY)
+        res = self.api.system.set_image(SystemImage.GLASTONBURY)
+        assert isinstance(res, dict), res
```

### Comparing `pypawapi-1.2.0/tests/test_webapp.py` & `pypawapi-2.0.0/tests/test_webapp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import TYPE_CHECKING
 from typing import Dict
 from typing import Union
 
 import pytest
 from responses.matchers import urlencoded_params_matcher
 
+from pawapi.exceptions import BadRequestError
 from pawapi.python import Python3
 
 if TYPE_CHECKING:
     from responses import RequestsMock
 
 
 @pytest.fixture
@@ -54,22 +55,23 @@
             match=(
                 urlencoded_params_matcher({
                     "domain_name": self.domain,
                     "python_version": "python38",
                 }),
             ),
         )
-        self.api.webapp.create(
+        assert self.api.webapp.create(
             domain_name=self.domain,
             python_version=Python3.PYTHON38,
         )
 
     def test_info(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.get(f"{self.url}/webapps/{self.domain}/")
-        self.api.webapp.get_info(self.domain)
+        mock_responses.get(f"{self.url}/webapps/{self.domain}/", json={})
+        res = self.api.webapp.get_info(self.domain)
+        assert isinstance(res, dict), res
 
     def test_update(self, mock_responses: 'RequestsMock') -> None:
         params = {
             "source_directory": "/home/user/appsrc",
             "virtualenv_path": "/home/user/venv",
             "force_https": True,
         }
@@ -78,159 +80,233 @@
             match=(
                 urlencoded_params_matcher({
                     "python_version": "3.9",
                     **{k: str(v)
                        for k, v in params.items()}
                 }),
             ),
+            json={},
         )
-        self.api.webapp.update(
+        res = self.api.webapp.update(
             domain_name=self.domain,
             python_version=Python3.PYTHON39,
             **params,
         )
+        assert isinstance(res, dict), res
 
     def test_update_protected(self, mock_responses: 'RequestsMock') -> None:
         user = "username"
         pwd = "password123"
 
         mock_responses.patch(
             url=f"{self.url}/webapps/{self.domain}/",
             match=(
                 urlencoded_params_matcher({
                     "password_protection_enabled": "True",
                     "password_protection_username": user,
                     "password_protection_password": pwd,
                 }),
             ),
+            json={},
         )
-        self.api.webapp.update(
+        res = self.api.webapp.update(
             domain_name=self.domain,
             protection=True,
             protection_username=user,
             protection_password=pwd,
         )
+        assert isinstance(res, dict), res
 
     def test_delete(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.delete(f"{self.url}/webapps/{self.domain}/")
-        self.api.webapp.delete(self.domain)
+        mock_responses.delete(f"{self.url}/webapps/{self.domain}/", status=204)
+        assert self.api.webapp.delete(self.domain)
 
     def test_enable(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.post(f"{self.url}/webapps/{self.domain}/enable/")
-        self.api.webapp.enable(self.domain)
+        json = {"status": "OK"}
+        mock_responses.post(
+            f"{self.url}/webapps/{self.domain}/enable/", json=json
+        )
+        assert self.api.webapp.enable(self.domain)
+
+    def test_enable_enabled(self, mock_responses: 'RequestsMock') -> None:
+        json = {"error": "You cannot create any more webapps - ..."}
+        mock_responses.post(
+            f"{self.url}/webapps/{self.domain}/enable/",
+            json=json,
+            status=400,
+        )
+        assert self.api.webapp.enable(self.domain)
 
     def test_disable(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.post(f"{self.url}/webapps/{self.domain}/disable/")
-        self.api.webapp.disable(self.domain)
+        json = {"status": "OK"}
+        mock_responses.post(
+            f"{self.url}/webapps/{self.domain}/disable/", json=json
+        )
+        assert self.api.webapp.disable(self.domain)
 
     def test_reload(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.post(f"{self.url}/webapps/{self.domain}/reload/")
-        self.api.webapp.reload(self.domain)
+        json = {"status": "OK"}
+        mock_responses.post(
+            f"{self.url}/webapps/{self.domain}/reload/", json=json
+        )
+        assert self.api.webapp.reload(self.domain)
+
+    def test_reload_disabled(self, mock_responses: 'RequestsMock') -> None:
+        mock_responses.post(
+            f"{self.url}/webapps/{self.domain}/reload/",
+            status=500,
+        )
+        assert not self.api.webapp.reload(self.domain)
 
     def test_ssl_info(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.get(f"{self.url}/webapps/{self.domain}/ssl/")
-        self.api.webapp.get_ssl_info(self.domain)
+        mock_responses.get(f"{self.url}/webapps/{self.domain}/ssl/", json={})
+        res = self.api.webapp.get_ssl_info(self.domain)
+        assert isinstance(res, dict), res
 
     def test_add_ssl(self, mock_responses: 'RequestsMock') -> None:
         params = {
             "cert": "cert",
             "private_key": "privete_key",
         }
         mock_responses.post(
             url=f"{self.url}/webapps/{self.domain}/ssl/",
             match=(urlencoded_params_matcher(params), ),
+            json={"status": "OK"},
+        )
+        assert self.api.webapp.add_ssl(domain_name=self.domain, **params)
+
+    def test_add_ssl_invalid_cred(self, mock_responses: 'RequestsMock') -> None:
+        params = {
+            "cert": "cert",
+            "private_key": "privete_key",
+        }
+        mock_responses.post(
+            url=f"{self.url}/webapps/{self.domain}/ssl/",
+            match=(urlencoded_params_matcher(params), ),
+            status=400,
         )
-        self.api.webapp.add_ssl(domain_name=self.domain, **params)
+        with pytest.raises(BadRequestError):
+            self.api.webapp.add_ssl(domain_name=self.domain, **params)
 
     def test_delete_ssl(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.delete(f"{self.url}/webapps/{self.domain}/ssl/")
-        self.api.webapp.delete_ssl(self.domain)
+        mock_responses.delete(
+            f"{self.url}/webapps/{self.domain}/ssl/",
+            json={"status": "OK"},
+        )
+        assert self.api.webapp.delete_ssl(self.domain)
 
     def test_list_static_files(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.get(f"{self.url}/webapps/{self.domain}/static_files/")
-        self.api.webapp.list_static_files(self.domain)
+        mock_responses.get(
+            f"{self.url}/webapps/{self.domain}/static_files/",
+            body=b"[]",
+            content_type="application/json",
+        )
+        res = self.api.webapp.list_static_files(self.domain)
+        assert isinstance(res, list)
 
     def test_add_static_file(
         self,
         mock_responses: 'RequestsMock',
         params_static_files: Dict[str, str],
     ) -> None:
         mock_responses.post(
             url=f"{self.url}/webapps/{self.domain}/static_files/",
             match=(urlencoded_params_matcher(params_static_files), ),
+            json={},
         )
-        self.api.webapp.add_static_file(
+        res = self.api.webapp.add_static_file(
             domain_name=self.domain,
             **params_static_files,
         )
+        assert isinstance(res, dict)
 
     def test_static_file_info(self, mock_responses: 'RequestsMock') -> None:
         mock_responses.get(
             f"{self.url}/webapps/{self.domain}/static_files/{self.file_id}/",
+            json={},
         )
-        self.api.webapp.get_static_file_info(self.domain, self.file_id)
+        res = self.api.webapp.get_static_file_info(self.domain, self.file_id)
+        assert isinstance(res, dict)
 
     def test_update_static_file(
         self,
         mock_responses: 'RequestsMock',
         params_static_files: Dict[str, str],
     ) -> None:
         mock_responses.patch(
             url=f"{self.url}/webapps/{self.domain}/static_files/{self.file_id}/",  # noqa: E501
             match=(urlencoded_params_matcher(params_static_files), ),
+            json={},
         )  # yapf: disable
-        self.api.webapp.update_static_file(
+        res = self.api.webapp.update_static_file(
             domain_name=self.domain,
             file_id=self.file_id,
             **params_static_files,
         )
+        assert isinstance(res, dict)
 
     def test_delete_static_file(self, mock_responses: 'RequestsMock') -> None:
         mock_responses.delete(
             f"{self.url}/webapps/{self.domain}/static_files/{self.file_id}/",
+            status=204,
         )
-        self.api.webapp.delete_static_file(self.domain, self.file_id)
+        assert self.api.webapp.delete_static_file(self.domain, self.file_id)
 
     def test_list_static_headers(self, mock_responses: 'RequestsMock') -> None:
-        mock_responses.get(f"{self.url}/webapps/{self.domain}/static_headers/")
-        self.api.webapp.list_static_headers(self.domain)
+        mock_responses.get(
+            f"{self.url}/webapps/{self.domain}/static_headers/",
+            content_type="application/json",
+            body=b"[]",
+        )
+        res = self.api.webapp.list_static_headers(self.domain)
+        assert isinstance(res, list)
 
     def test_add_static_header(
         self,
         mock_responses: 'RequestsMock',
         params_static_headers: Dict[str, str]
     ) -> None:
         mock_responses.post(
             url=f"{self.url}/webapps/{self.domain}/static_headers/",
             match=(urlencoded_params_matcher(params_static_headers), ),
+            json={},
         )
-        self.api.webapp.add_static_header(
+        res = self.api.webapp.add_static_header(
             domain_name=self.domain,
             **params_static_headers,
         )
+        assert isinstance(res, dict)
 
     def test_static_header_info(self, mock_responses: 'RequestsMock') -> None:
         mock_responses.get(
             f"{self.url}/webapps/{self.domain}/static_headers/{self.header_id}/",  # noqa: E501
+            json={},
+        )
+        res = self.api.webapp.get_static_header_info(
+            self.domain,
+            self.header_id,
         )
-        self.api.webapp.get_static_header_info(self.domain, self.header_id)
+        assert isinstance(res, dict)
 
     def test_update_static_header(
         self,
         mock_responses: 'RequestsMock',
         params_static_headers: Dict[str, str],
     ) -> None:
         mock_responses.patch(
             url=f"{self.url}/webapps/{self.domain}/static_headers/{self.header_id}/",  # noqa: E501
             match=(urlencoded_params_matcher(params_static_headers), ),
+            json={},
         )  # yapf: disable
-        self.api.webapp.update_static_header(
+        res = self.api.webapp.update_static_header(
             domain_name=self.domain,
             header_id=self.header_id,
             **params_static_headers,
         )
+        assert isinstance(res, dict)
 
     def test_delete_static_header(self, mock_responses: 'RequestsMock') -> None:
         mock_responses.delete(
             f"{self.url}/webapps/{self.domain}/static_headers/{self.header_id}/",  # noqa: E501
+            status=204,
         )
-        self.api.webapp.delete_static_header(self.domain, self.header_id)
+        assert self.api.webapp.delete_static_header(self.domain, self.header_id)
```

### Comparing `pypawapi-1.2.0/LICENSE` & `pypawapi-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypawapi-1.2.0/pyproject.toml` & `pypawapi-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Typing :: Typed",
 ]
 requires-python = ">=3.7"
 dependencies = [
   "requests >=2.22.0,<3.0.0",
 ]
 
 [project.urls]
```

### Comparing `pypawapi-1.2.0/PKG-INFO` & `pypawapi-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypawapi
-Version: 1.2.0
+Version: 2.0.0
 Summary: API wrapper for pythonanywhere
 Project-URL: Source, https://codeberg.org/maraudeur/pawapi
 Author-email: Maraudeur <maraudeur1@protonmail.ch>
 License:  The MIT License (MIT)
         
          Copyright (c) 2019 Maraudeur <maraudeur1 AT protonmail DOT ch>
         
@@ -33,14 +33,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: requests<3.0.0,>=2.22.0
 Provides-Extra: dev
 Requires-Dist: pre-commit<3.0.0,>=2.0.0; extra == 'dev'
 Provides-Extra: lint
 Requires-Dist: flake8-bugbear==22.6.22; extra == 'lint'
 Requires-Dist: flake8<6.0.0,>=5.0.0; extra == 'lint'
@@ -72,90 +73,27 @@
 ```python
 from pawapi import Pawapi, Python3
 
 TOKEN = "<your_token>"
 USER = "<your_username>"
 
 api = Pawapi(USER, TOKEN)
-cpu_usage = api.cpu.get_info().content
+cpu_usage = api.cpu.get_info()
 print(cpu_usage)
 
 domain = f"{USER}.pythonanywhere.com"
 api.webapp.create(domain, Python3.PYTHON39)
-app = api.webapp.list().content[-1]
+app = api.webapp.list()[-1]
 print(app["id"])
 ```
 
-### Available methods
-* always_on
-    * create
-    * delete
-    * get_info
-    * list
-    * restart
-    * update
-* console
-    * create
-    * get_info
-    * get_output
-    * kill
-    * list
-    * list_shared
-    * send_input
-* cpu
-    * get_info
-* file
-    * delete
-    * get_content
-    * get_sharing_status
-    * get_tree
-    * start_sharing
-    * stop_sharing
-    * upload
-* python
-    * get_python3_version
-    * set_python3_version
-    * get_python_version
-    * set_python_version
-    * get_sar_version
-    * set_sar_version
-* scheduled_task
-    * create
-    * delete
-    * get_info
-    * list
-    * update
-* students
-    * delete
-    * list
-* system
-    * get_current_image
-    * set_image
-* webapp
-    * list
-    * create
-    * get_info
-    * update
-    * delete
-    * enable
-    * disable
-    * reload
-    * add_ssl
-    * get_ssl_info
-    * delete_ssl
-    * add_static_file
-    * get_static_file_info
-    * list_static_files
-    * update_static_file
-    * delete_static_file
-    * add_static_header
-    * get_static_header_info
-    * update_static_header
-    * delete_static_header
-    * list_static_headers
+### Docs
+```shell
+$ python -c "import pawapi; help(pawapi.Pawapi)"
+```
 
 ## LICENSE
  The MIT License (MIT)    
 
  Copyright (c) 2019 Maraudeur    
 
  Permission is hereby granted, free of charge, to any person obtaining
```

