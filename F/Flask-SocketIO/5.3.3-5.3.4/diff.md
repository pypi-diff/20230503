# Comparing `tmp/Flask-SocketIO-5.3.3.tar.gz` & `tmp/Flask-SocketIO-5.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-SocketIO-5.3.3.tar", last modified: Fri Mar 17 12:34:05 2023, max compression
+gzip compressed data, was "Flask-SocketIO-5.3.4.tar", last modified: Wed May  3 10:34:08 2023, max compression
```

## Comparing `Flask-SocketIO-5.3.3.tar` & `Flask-SocketIO-5.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-17 12:34:05.453610 Flask-SocketIO-5.3.3/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1082 2019-11-17 19:18:09.000000 Flask-SocketIO-5.3.3/LICENSE
--rw-r--r--   0 mgrinberg   (502) staff       (20)       26 2019-11-17 19:18:09.000000 Flask-SocketIO-5.3.3/MANIFEST.in
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2504 2023-03-17 12:34:05.453796 Flask-SocketIO-5.3.3/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1867 2021-06-13 15:46:50.000000 Flask-SocketIO-5.3.3/README.md
--rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-13 15:46:50.000000 Flask-SocketIO-5.3.3/pyproject.toml
--rw-r--r--   0 mgrinberg   (502) staff       (20)      845 2023-03-17 12:34:05.454709 Flask-SocketIO-5.3.3/setup.cfg
--rw-r--r--   0 mgrinberg   (502) staff       (20)       38 2021-07-17 09:46:45.000000 Flask-SocketIO-5.3.3/setup.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-17 12:34:05.441220 Flask-SocketIO-5.3.3/src/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-17 12:34:05.449072 Flask-SocketIO-5.3.3/src/Flask_SocketIO.egg-info/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2504 2023-03-17 12:34:05.000000 Flask-SocketIO-5.3.3/src/Flask_SocketIO.egg-info/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)      410 2023-03-17 12:34:05.000000 Flask-SocketIO-5.3.3/src/Flask_SocketIO.egg-info/SOURCES.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-03-17 12:34:05.000000 Flask-SocketIO-5.3.3/src/Flask_SocketIO.egg-info/dependency_links.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-07 19:15:18.000000 Flask-SocketIO-5.3.3/src/Flask_SocketIO.egg-info/not-zip-safe
--rw-r--r--   0 mgrinberg   (502) staff       (20)       34 2023-03-17 12:34:05.000000 Flask-SocketIO-5.3.3/src/Flask_SocketIO.egg-info/requires.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)       15 2023-03-17 12:34:05.000000 Flask-SocketIO-5.3.3/src/Flask_SocketIO.egg-info/top_level.txt
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-03-17 12:34:05.452668 Flask-SocketIO-5.3.3/src/flask_socketio/
--rw-r--r--   0 mgrinberg   (502) staff       (20)    54670 2023-03-17 12:05:01.000000 Flask-SocketIO-5.3.3/src/flask_socketio/__init__.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2020 2021-06-13 15:46:50.000000 Flask-SocketIO-5.3.3/src/flask_socketio/namespace.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10030 2022-06-12 14:26:48.000000 Flask-SocketIO-5.3.3/src/flask_socketio/test_client.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-03 10:34:08.560341 Flask-SocketIO-5.3.4/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1082 2019-11-17 19:18:09.000000 Flask-SocketIO-5.3.4/LICENSE
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       26 2019-11-17 19:18:09.000000 Flask-SocketIO-5.3.4/MANIFEST.in
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2504 2023-05-03 10:34:08.560571 Flask-SocketIO-5.3.4/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1867 2021-06-13 15:46:50.000000 Flask-SocketIO-5.3.4/README.md
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-13 15:46:50.000000 Flask-SocketIO-5.3.4/pyproject.toml
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      845 2023-05-03 10:34:08.561552 Flask-SocketIO-5.3.4/setup.cfg
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       38 2021-07-17 09:46:45.000000 Flask-SocketIO-5.3.4/setup.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-03 10:34:08.548192 Flask-SocketIO-5.3.4/src/
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-03 10:34:08.555686 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2504 2023-05-03 10:34:08.000000 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      410 2023-05-03 10:34:08.000000 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/SOURCES.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-05-03 10:34:08.000000 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/dependency_links.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-07 19:15:18.000000 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/not-zip-safe
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       34 2023-05-03 10:34:08.000000 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/requires.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       15 2023-05-03 10:34:08.000000 Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/top_level.txt
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-05-03 10:34:08.559372 Flask-SocketIO-5.3.4/src/flask_socketio/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    54782 2023-03-21 19:59:26.000000 Flask-SocketIO-5.3.4/src/flask_socketio/__init__.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     2020 2021-06-13 15:46:50.000000 Flask-SocketIO-5.3.4/src/flask_socketio/namespace.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    10274 2023-05-03 10:28:48.000000 Flask-SocketIO-5.3.4/src/flask_socketio/test_client.py
```

### Comparing `Flask-SocketIO-5.3.3/LICENSE` & `Flask-SocketIO-5.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-SocketIO-5.3.3/PKG-INFO` & `Flask-SocketIO-5.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SocketIO
-Version: 5.3.3
+Version: 5.3.4
 Summary: Socket.IO integration for Flask applications
 Home-page: https://github.com/miguelgrinberg/flask-socketio
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/flask-socketio/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `Flask-SocketIO-5.3.3/README.md` & `Flask-SocketIO-5.3.4/README.md`

 * *Files identical despite different names*

### Comparing `Flask-SocketIO-5.3.3/setup.cfg` & `Flask-SocketIO-5.3.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Flask-SocketIO
-version = 5.3.3
+version = 5.3.4
 author = Miguel Grinberg
 author_email = miguel.grinberg@gmail.com
 description = Socket.IO integration for Flask applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/miguelgrinberg/flask-socketio
 project_urls =
```

### Comparing `Flask-SocketIO-5.3.3/src/Flask_SocketIO.egg-info/PKG-INFO` & `Flask-SocketIO-5.3.4/src/Flask_SocketIO.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SocketIO
-Version: 5.3.3
+Version: 5.3.4
 Summary: Socket.IO integration for Flask applications
 Home-page: https://github.com/miguelgrinberg/flask-socketio
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/flask-socketio/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `Flask-SocketIO-5.3.3/src/flask_socketio/__init__.py` & `Flask-SocketIO-5.3.4/src/flask_socketio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -822,14 +822,16 @@
                     auth = args[1] if len(args) > 1 else None
                     try:
                         ret = handler(auth)
                     except TypeError:
                         ret = handler()
                 else:
                     ret = handler(*args)
+            except ConnectionRefusedError:
+                raise  # let this error bubble up to python-socketio
             except:
                 err_handler = self.exception_handlers.get(
                     namespace, self.default_exception_handler)
                 if err_handler is None:
                     raise
                 type, value, traceback = sys.exc_info()
                 return err_handler(value)
```

### Comparing `Flask-SocketIO-5.3.3/src/flask_socketio/namespace.py` & `Flask-SocketIO-5.3.4/src/flask_socketio/namespace.py`

 * *Files identical despite different names*

### Comparing `Flask-SocketIO-5.3.3/src/flask_socketio/test_client.py` & `Flask-SocketIO-5.3.4/src/flask_socketio/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,20 @@
             if query_string[0] != '?':
                 query_string = '?' + query_string
             url += query_string
         environ = EnvironBuilder(url, headers=headers).get_environ()
         environ['flask.app'] = self.app
         if self.flask_test_client:
             # inject cookies from Flask
-            self.flask_test_client.cookie_jar.inject_wsgi(environ)
+            if hasattr(self.flask_test_client, '_add_cookies_to_wsgi'):
+                # flask >= 2.3
+                self.flask_test_client._add_cookies_to_wsgi(environ)
+            else:  # pragma: no cover
+                # flask < 2.3
+                self.flask_test_client.cookie_jar.inject_wsgi(environ)
         self.socketio.server._handle_eio_connect(self.eio_sid, environ)
         pkt = packet.Packet(packet.CONNECT, auth, namespace=namespace)
         self.socketio.server._handle_eio_message(self.eio_sid, pkt.encode())
         sid = self.socketio.server.manager.sid_from_eio_sid(self.eio_sid,
                                                             namespace)
         if sid:
             self.connected[namespace] = True
```

