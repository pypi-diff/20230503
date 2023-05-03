# Comparing `tmp/HTTP-PyServer-0.1.tar.gz` & `tmp/HTTP-PyServer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTTP-PyServer-0.1.tar", last modified: Mon May  1 17:56:20 2023, max compression
+gzip compressed data, was "HTTP-PyServer-0.1.1.tar", last modified: Wed May  3 19:43:56 2023, max compression
```

## Comparing `HTTP-PyServer-0.1.tar` & `HTTP-PyServer-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 17:56:20.661136 HTTP-PyServer-0.1/
--rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1/LICENSE
--rw-rw-rw-   0        0        0     2017 2023-05-01 17:56:20.660143 HTTP-PyServer-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-05-01 16:32:34.000000 HTTP-PyServer-0.1/README.md
--rw-rw-rw-   0        0        0      639 2023-05-01 17:53:24.000000 HTTP-PyServer-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 17:56:20.661136 HTTP-PyServer-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 17:56:20.615958 HTTP-PyServer-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 17:56:20.635090 HTTP-PyServer-0.1/src/HTTP_PyServer.egg-info/
--rw-rw-rw-   0        0        0     2017 2023-05-01 17:56:20.000000 HTTP-PyServer-0.1/src/HTTP_PyServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-05-01 17:56:20.000000 HTTP-PyServer-0.1/src/HTTP_PyServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 17:56:20.000000 HTTP-PyServer-0.1/src/HTTP_PyServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 17:56:20.000000 HTTP-PyServer-0.1/src/HTTP_PyServer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 17:56:20.656208 HTTP-PyServer-0.1/src/server/
--rw-rw-rw-   0        0        0      318 2023-05-01 16:28:05.000000 HTTP-PyServer-0.1/src/server/__init__.py
--rw-rw-rw-   0        0        0     5344 2023-04-30 04:44:01.000000 HTTP-PyServer-0.1/src/server/render.py
--rw-rw-rw-   0        0        0     2358 2023-05-01 16:37:07.000000 HTTP-PyServer-0.1/src/server/request.py
--rw-rw-rw-   0        0        0     2122 2023-05-01 16:34:09.000000 HTTP-PyServer-0.1/src/server/response.py
--rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1/src/server/response_codes.py
--rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1/src/server/response_messages.py
--rw-rw-rw-   0        0        0     4265 2023-05-01 16:35:52.000000 HTTP-PyServer-0.1/src/server/routes.py
--rw-rw-rw-   0        0        0     5690 2023-05-01 17:12:39.000000 HTTP-PyServer-0.1/src/server/server.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:43:56.364440 HTTP-PyServer-0.1.1/
+-rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2033 2023-05-03 19:43:56.363441 HTTP-PyServer-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1470 2023-05-03 19:36:27.000000 HTTP-PyServer-0.1.1/README.md
+-rw-rw-rw-   0        0        0      641 2023-05-03 19:43:16.000000 HTTP-PyServer-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 19:43:56.365436 HTTP-PyServer-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 19:43:56.212844 HTTP-PyServer-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 19:43:56.271686 HTTP-PyServer-0.1.1/src/HTTP_PyServer.egg-info/
+-rw-rw-rw-   0        0        0     2033 2023-05-03 19:43:56.000000 HTTP-PyServer-0.1.1/src/HTTP_PyServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-05-03 19:43:56.000000 HTTP-PyServer-0.1.1/src/HTTP_PyServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 19:43:56.000000 HTTP-PyServer-0.1.1/src/HTTP_PyServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 19:43:56.000000 HTTP-PyServer-0.1.1/src/HTTP_PyServer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 19:43:56.358461 HTTP-PyServer-0.1.1/src/server/
+-rw-rw-rw-   0        0        0      318 2023-05-01 16:28:05.000000 HTTP-PyServer-0.1.1/src/server/__init__.py
+-rw-rw-rw-   0        0        0     5374 2023-05-03 19:35:13.000000 HTTP-PyServer-0.1.1/src/server/render.py
+-rw-rw-rw-   0        0        0     2358 2023-05-01 16:37:07.000000 HTTP-PyServer-0.1.1/src/server/request.py
+-rw-rw-rw-   0        0        0     2122 2023-05-01 16:34:09.000000 HTTP-PyServer-0.1.1/src/server/response.py
+-rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.1/src/server/response_codes.py
+-rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.1/src/server/response_messages.py
+-rw-rw-rw-   0        0        0     4773 2023-05-03 19:35:25.000000 HTTP-PyServer-0.1.1/src/server/routes.py
+-rw-rw-rw-   0        0        0     6872 2023-05-03 19:25:21.000000 HTTP-PyServer-0.1.1/src/server/server.py
```

### Comparing `HTTP-PyServer-0.1/LICENSE` & `HTTP-PyServer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1/PKG-INFO` & `HTTP-PyServer-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1
+Version: 0.1.1
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,12 +58,13 @@
 
 Although, no external packages were used, the following packages were imported. All packages are native in `Python 3.11.2`. Not tested on any other versions, however it should work.
 
 - `threading`
 - `socket`
 - `typing`
 - `logging`
-- `os`
+- `pathlib`
 - `json`
 - `urllib`
 - `mimetypes`
 - `enum`
+- `ssl`
```

### Comparing `HTTP-PyServer-0.1/README.md` & `HTTP-PyServer-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -44,12 +44,13 @@
 
 Although, no external packages were used, the following packages were imported. All packages are native in `Python 3.11.2`. Not tested on any other versions, however it should work.
 
 - `threading`
 - `socket`
 - `typing`
 - `logging`
-- `os`
+- `pathlib`
 - `json`
 - `urllib`
 - `mimetypes`
-- `enum`
+- `enum`
+- `ssl`
```

### Comparing `HTTP-PyServer-0.1/pyproject.toml` & `HTTP-PyServer-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HTTP-PyServer"
-version = "0.1"
+version = "0.1.1"
 authors = [
   { name="Alex-Jando", email="alexjando2007@outlook.com" },
 ]
 description = "Simple way to make complex HTTP servers with python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HTTP-PyServer-0.1/src/HTTP_PyServer.egg-info/PKG-INFO` & `HTTP-PyServer-0.1.1/src/HTTP_PyServer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1
+Version: 0.1.1
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,12 +58,13 @@
 
 Although, no external packages were used, the following packages were imported. All packages are native in `Python 3.11.2`. Not tested on any other versions, however it should work.
 
 - `threading`
 - `socket`
 - `typing`
 - `logging`
-- `os`
+- `pathlib`
 - `json`
 - `urllib`
 - `mimetypes`
 - `enum`
+- `ssl`
```

### Comparing `HTTP-PyServer-0.1/src/server/render.py` & `HTTP-PyServer-0.1.1/src/server/render.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import mimetypes
-import os
+import pathlib
 
 from . import response_codes
-from . import request
 from . import response
 from . import response_messages
 
 def _get_template(data: bytes,
                   **template_vars) -> str:
     '''Replaces all template variables in a data with their values.
     Template variables are defined as {{var_name}},
@@ -22,82 +21,82 @@
     return data
 
 def text(text: str,
          *,
          filetype: str = 'txt',
          code: int | response_codes.ResponseCodes = 200,
          message: str | response_messages.ResponseMessages = 'OK',
-         ) -> response.Response:
+         headers: dict = None) -> response.Response:
     '''Returns a text response. Use this to return plain text, JSON, XML, etc.'''
 
+    if not headers:
+
+        headers = {}
+
     if type(code) == response_codes.ResponseCodes:
 
         code = code.value
 
     if type(message) == response_messages.ResponseMessages:
 
         message = message.value
 
     text = text.encode(encoding = 'utf-8',
                        errors = 'ignore')
+    
+    headers['Content-Length'] = str(len(text))
 
-    headers = {
-
-        'Content-Type': mimetypes.guess_type(f'file.{filetype.strip(".")}')[0],
-
-        'Content-Length': str(len(text)),
-
-    }
+    headers['Content-Type'] = mimetypes.guess_type(f'file.{filetype.strip(".")}')[0]\
+                              or 'text/plain'
 
     return response.Response(version = 1.1,
                              code = code,
                              message = message,
                              headers = headers,
                              body = text)
 
 def file(filepath: str,
          *,
-         request: request.Request = request.Request(),
          templated_vars: dict = {},
          code: int | response_codes.ResponseCodes = 200,
-         message: str | response_messages.ResponseMessages = 'OK'
+         message: str | response_messages.ResponseMessages = 'OK',
+         headers: dict = None
          ) -> response.Response:
     '''Returns a file as a response. Use this to return HTML, CSS, JS, images, etc.'''
 
+    if not headers:
+
+        headers = {}
+
     if type(code) == response_codes.ResponseCodes:
 
         code = code.value
 
     if type(message) == response_messages.ResponseMessages:
 
         message = message.value
 
-    if not filepath or not os.path.exists(filepath):
+    if not filepath or not pathlib.Path(filepath).exists():
 
         raise FileNotFoundError(f'File not found: {filepath}')
             
     else:
 
         with open(filepath, 'rb') as file:
 
             data = file.read()
 
     if templated_vars:
 
         data = _get_template(data = data,
                              **templated_vars)
 
-    headers = {
-
-        'Content-Type': mimetypes.guess_type(filepath)[0]\
-                        or 'application/octet-stream',
-
-        'Content-Length': str(len(data)),
-
-    }
+    headers['Content-Length'] = str(len(data))
+    headers['Content-Type'] = mimetypes.guess_type(filepath)[0]\
+                              or 'application/octet-stream'
 
     return response.Response(version = 1.1,
                              code = code,
                              message = message,
                              headers = headers,
                              body = data)
 
@@ -121,41 +120,37 @@
                                         'Content-Type': 'text/html',
                                         'Content-Length': str(len(redirect_request))},
                              body = redirect_request)
 
 def attachment(filepath: str = '',
                *,
                is_download: bool = False,
-               is_text: bool = False,
                filename: str = '',
-               request: request.Request = request.Request()) -> response.Response:
+               headers: dict = None) -> response.Response:
     '''Returns a file as an attachment.
     Use this to return files for download or viewing.
     Sometimes browsers will preview text files, so you can use is_text
     to force the browser to display the raw text instead of previewing it.'''
 
-    if not filepath or not os.path.exists(filepath):
+    if not headers:
+
+        headers = {}
+
+    if not filepath or not pathlib.Path(filepath).exists():
 
         raise FileNotFoundError(f'File not found: {filepath}')
 
     with open(filepath, 'rb') as f:
 
         data = f.read()
 
-    headers = {
-
-        'Content-Type': 'text/plain' if is_text else\
-                        mimetypes.guess_type(filepath)[0]\
-                        or 'application/octet-stream',
-
-        'Content-Length': str(len(data)),
-
-        'Content-Disposition': ('attachment' if is_download else 'inline')\
-                                + (f'; filename="{filename}"' if filename else '')
-
-    }
+    headers['Content-Length'] = str(len(data))
+    headers['Content-Type'] = mimetypes.guess_type(filepath)[0]\
+                              or 'application/octet-stream'
+    headers['Content-Disposition'] = ('attachment' if is_download else 'inline')\
+                                     + (f'; filename="{filename}"' if filename else '')
 
     return response.Response(version = 1.1,
                              code = response_codes.ResponseCodes.OK,
                              message = response_messages.ResponseMessages.OK,
                              headers = headers,
                              body = data)
```

### Comparing `HTTP-PyServer-0.1/src/server/request.py` & `HTTP-PyServer-0.1.1/src/server/request.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1/src/server/response.py` & `HTTP-PyServer-0.1.1/src/server/response.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1/src/server/response_codes.py` & `HTTP-PyServer-0.1.1/src/server/response_codes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1/src/server/response_messages.py` & `HTTP-PyServer-0.1.1/src/server/response_messages.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1/src/server/routes.py` & `HTTP-PyServer-0.1.1/src/server/routes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import os
+import pathlib
 
 from . import response_messages
 from . import response_codes
 from . import response
 from . import request
 from . import render
 
 class Routes:
     '''Stores, sorts, and handles a collection of routes.'''
 
     def __init__(self) -> None:
 
         self._routes: dict[str: callable] = {
-            '/404': lambda request: render.text('''<!DOCTYPE html>
+
+            self._404route: lambda request: render.text('''<!DOCTYPE html>
 
 <html>
 
 <head>
 <title>404 Not Found</title>
 </head>
 
@@ -29,35 +30,54 @@
 <p style="text-align: center;">HTTP-PyServer</p>
 
 </body>
 
 </html>''',
 filetype='html',
 code = response_codes.ResponseCodes.NOT_FOUND,
-message = response_messages.ResponseMessages.NOT_FOUND)
+message = response_messages.ResponseMessages.NOT_FOUND),
+
+            self._500route: lambda request: render.text('''<!DOCTYPE html>
+
+<html>
+
+<head>
+<title>500 Internal Server Error</title>
+</head>
+
+<body>
+
+<h1 style="text-align: center;">500 Internal Server Error</h1>
+
+<hr>
+
+<p style="text-align: center;">HTTP-PyServer</p>
+
+</body>
+
+</html>''',
+filetype='html',
+code = response_codes.ResponseCodes.INTERNAL_SERVER_ERROR,
+message = response_messages.ResponseMessages.INTERNAL_SERVER_ERROR)
+
     }
 
     def route(self,
               path: str,
               *,
               ressources: dict[str: str] = {}) -> callable:
         '''Adds a route to the routes dictionary.'''
 
         for ressource_file_path, ressource_reference_path in ressources.items():
 
             ressource_reference_path = '/' + ressource_reference_path.strip('/')
 
-            if not os.path.exists(ressource_file_path):
-
-                self._routes[ressource_reference_path] = \
-                    lambda _: self._routes['/404'](request = request.Request())
-
-            else:
+            if pathlib.Path(ressource_file_path).exists():
 
-                ressource = render.attachment(filepath = ressource_file_path)
+                ressource = render.file(filepath = ressource_file_path)
 
                 self._routes[ressource_reference_path] = \
                 lambda _, ressource = ressource: ressource
 
         def callable_route(route_function):
 
             self._routes[path.rstrip('/')] = route_function
@@ -103,25 +123,25 @@
                 if isinstance(message, str):
 
                     return bytes(render.text(message))
                 
                 elif isinstance(message, bytes):
 
                     return message
-                
+
                 elif isinstance(message, response.Response):
 
                     return bytes(message)
                 
                 else:
 
                     raise TypeError(f'Expected function for {request.path} \
 to return str, bytes, or Response, got {type(message)}.')
 
-        return self._get_route('/404', request = request)
+        return self._get_route(self._404route, request = request)
 
     def _get_route(self,
                   path: str,
                   *,
                   request: request.Request = request.Request()) -> bytes:
         '''Gets a route from the _routes dictionary.'''
 
@@ -141,12 +161,17 @@
 
                 return bytes(message)
             
             else:
 
                 raise TypeError(f'Expected function for {request.path} \
 to return str, bytes, or Response, got {type(message)}.')
+            
+        elif pathlib.Path(path).is_relative_to(
+             pathlib.Path('/' + self._static_dir.as_posix().strip('/'))):
+
+            return bytes(render.file(filepath = path.strip('/')))
 
         else:
 
             return self._get_wildcard_path(path = path,
                                           request = request)
```

### Comparing `HTTP-PyServer-0.1/src/server/server.py` & `HTTP-PyServer-0.1.1/src/server/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,60 @@
 import threading
 import socket
 import logging
 from typing import Self
+import ssl
+import pathlib
 
 from . import request
 from . import routes
 
 class Server(routes.Routes):
     '''HTTP server running on a specified host and port.'''
 
     def __init__(self,
                  *,
                  host: str = '127.0.0.1',
                  port: int = 80,
-                 logger: logging.Logger = None) -> None:
+                 logger: logging.Logger = None,
+                 _404route: str = '/404',
+                 _500route: str = '/500',
+                 static_dir: str = '/static/',
+                 ssl_context: ssl.SSLContext = None) -> None:
         '''Initializes the server class.'''
         
-        super().__init__()
-        
         self._host: str = host
 
         self._port: int = port
 
         self._logger: logging.Logger = logger
 
+        self._404route: str = _404route
+
+        self._500route: str = _500route
+
+        self._static_dir: pathlib.Path = pathlib.Path(static_dir.strip('/'))
+
+        if not self._static_dir.exists():
+
+            self._logger.warning('Static directory does not exist.')
+
+        self._ssl_context: ssl.SSLContext = ssl_context
+
+        super().__init__()
+
     def start(self) -> None:
         '''Starts the server.'''
+
+        if self._logger:
+
+            self._logger.info('Starting server...')
         
         threading.Thread(target = self._listen,
-                         daemon = True).start()
+                        daemon = True).start()
         
     def wait(self) -> None:
         '''Waits for Enter key press or KeyboardInterrupt.'''
 
         try:
 
             input('Press Enter to continue...\n')
@@ -56,21 +78,27 @@
 
     def _listen(self) -> None:
         '''Listens for incoming connections 
         and spawns a thread to handle each request.'''
 
         self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
+        if self._ssl_context:
+
+            self._socket = self._ssl_context.wrap_socket(self._socket,
+                                                         server_side = True)
+
         self._socket.bind((self._host, self._port))
 
         self._socket.listen()
 
         if self._logger:
 
-            self._logger.info(f'Server hosted on {self._host}:{self._port}.')
+            self._logger.info(f'Server hosted on http{"s" if self._ssl_context else ""}\
+://{self._host}:{self._port}.')
             
         while True:
 
             try:
 
                 connection, address = self._socket.accept()
 
@@ -174,15 +202,26 @@
                     return None
 
             except Exception as e:
 
                 if self._logger:
 
                     self._logger.error(f'Error while handling request from \
-{address[0]}:{address[1]}: "{e}".')                
+{address[0]}:{address[1]} for {parsed_request.path} : "{e}".') 
+
+                try:
+
+                    connection.send(self._get_route(path = self._500route,
+                                                    request = parsed_request))
+                    
+                    connection.close()
+
+                except Exception:
+
+                    pass
 
                 return None
 
     def __enter__(self) -> Self:
         '''Starts the server.'''
 
         self.start()
```

