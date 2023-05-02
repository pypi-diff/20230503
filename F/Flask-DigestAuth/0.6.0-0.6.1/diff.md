# Comparing `tmp/Flask-DigestAuth-0.6.0.tar.gz` & `tmp/Flask-DigestAuth-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-DigestAuth-0.6.0.tar", last modified: Wed Apr 26 15:41:19 2023, max compression
+gzip compressed data, was "Flask-DigestAuth-0.6.1.tar", last modified: Tue May  2 23:00:54 2023, max compression
```

## Comparing `Flask-DigestAuth-0.6.0.tar` & `Flask-DigestAuth-0.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.199127 Flask-DigestAuth-0.6.0/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2018-06-01 15:46:07.000000 Flask-DigestAuth-0.6.0/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     3708 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     2787 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     2154 2023-04-26 15:40:40.000000 Flask-DigestAuth-0.6.0/docs/source/changelog.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1071 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     6657 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)      678 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/flask_digest_auth.rst
--rw-r--r--   0 imacat    (1000) users      (100)      915 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     4318 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       60 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.0/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1845 2023-04-26 15:30:27.000000 Flask-DigestAuth-0.6.0/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-26 15:41:19.199127 Flask-DigestAuth-0.6.0/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.191127 Flask-DigestAuth-0.6.0/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     3708 2023-04-26 15:41:19.000000 Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)      708 2023-04-26 15:41:19.000000 Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-26 15:41:19.000000 Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)       37 2023-04-26 15:41:19.000000 Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       18 2023-04-26 15:41:19.000000 Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/src/flask_digest_auth/
--rw-r--r--   0 imacat    (1000) users      (100)      939 2023-04-26 15:35:16.000000 Flask-DigestAuth-0.6.0/src/flask_digest_auth/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     4103 2023-04-26 15:30:30.000000 Flask-DigestAuth-0.6.0/src/flask_digest_auth/algo.py
--rw-r--r--   0 imacat    (1000) users      (100)    17722 2023-04-26 15:30:30.000000 Flask-DigestAuth-0.6.0/src/flask_digest_auth/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)     5538 2023-04-26 15:30:30.000000 Flask-DigestAuth-0.6.0/src/flask_digest_auth/test.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-26 15:41:19.195127 Flask-DigestAuth-0.6.0/tests/
--rw-r--r--   0 imacat    (1000) users      (100)     1956 2023-04-26 15:30:30.000000 Flask-DigestAuth-0.6.0/tests/test_algo.py
--rw-r--r--   0 imacat    (1000) users      (100)     7829 2023-04-26 15:30:30.000000 Flask-DigestAuth-0.6.0/tests/test_auth.py
--rw-r--r--   0 imacat    (1000) users      (100)    10505 2023-04-26 15:30:30.000000 Flask-DigestAuth-0.6.0/tests/test_flask_login.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2018-06-01 15:46:07.000000 Flask-DigestAuth-0.6.1/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     3708 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     2787 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.136977 Flask-DigestAuth-0.6.1/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.136977 Flask-DigestAuth-0.6.1/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     2254 2023-05-02 22:59:26.000000 Flask-DigestAuth-0.6.1/docs/source/changelog.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1071 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6657 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      678 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/flask_digest_auth.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      915 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     4318 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       60 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1845 2023-04-26 15:30:27.000000 Flask-DigestAuth-0.6.1/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.136977 Flask-DigestAuth-0.6.1/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     3708 2023-05-02 23:00:54.000000 Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)      708 2023-05-02 23:00:54.000000 Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-05-02 23:00:54.000000 Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       37 2023-05-02 23:00:54.000000 Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       18 2023-05-02 23:00:54.000000 Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/src/flask_digest_auth/
+-rw-r--r--   0 imacat    (1000) users      (100)      939 2023-05-02 22:59:26.000000 Flask-DigestAuth-0.6.1/src/flask_digest_auth/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4103 2023-04-27 01:07:49.000000 Flask-DigestAuth-0.6.1/src/flask_digest_auth/algo.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17796 2023-05-02 22:37:13.000000 Flask-DigestAuth-0.6.1/src/flask_digest_auth/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5569 2023-05-02 22:57:59.000000 Flask-DigestAuth-0.6.1/src/flask_digest_auth/test.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/tests/
+-rw-r--r--   0 imacat    (1000) users      (100)     1956 2023-04-27 01:07:49.000000 Flask-DigestAuth-0.6.1/tests/test_algo.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7849 2023-05-02 22:57:59.000000 Flask-DigestAuth-0.6.1/tests/test_auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)    10525 2023-05-02 22:57:59.000000 Flask-DigestAuth-0.6.1/tests/test_flask_login.py
```

### Comparing `Flask-DigestAuth-0.6.0/LICENSE` & `Flask-DigestAuth-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/MANIFEST.in` & `Flask-DigestAuth-0.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/PKG-INFO` & `Flask-DigestAuth-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-DigestAuth
-Version: 0.6.0
+Version: 0.6.1
 Summary: The Flask HTTP Digest Authentication project.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://flask-digestauth.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/flask-digestauth
 Project-URL: Bug Tracker, https://github.com/imacat/flask-digestauth/issues
 Keywords: flask,digest-authentication
```

### Comparing `Flask-DigestAuth-0.6.0/README.rst` & `Flask-DigestAuth-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/docs/Makefile` & `Flask-DigestAuth-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/docs/make.bat` & `Flask-DigestAuth-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/docs/source/changelog.rst` & `Flask-DigestAuth-0.6.1/docs/source/changelog.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 Change Log
 ==========
 
 
+Version 0.6.1
+-------------
+
+Released 2023/5/3
+
+* Revised the code for the upcoming Werkzeug 2.4.
+
+
 Version 0.6.0
 -------------
 
 Released 2023/4/26
 
 * Updated the minimal Python version to 3.8.
 * Switched from ``setup.cfg`` to ``pyproject.toml``.
```

### Comparing `Flask-DigestAuth-0.6.0/docs/source/conf.py` & `Flask-DigestAuth-0.6.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/docs/source/examples.rst` & `Flask-DigestAuth-0.6.1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/docs/source/flask_digest_auth.rst` & `Flask-DigestAuth-0.6.1/docs/source/flask_digest_auth.rst`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/docs/source/index.rst` & `Flask-DigestAuth-0.6.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/docs/source/intro.rst` & `Flask-DigestAuth-0.6.1/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/pyproject.toml` & `Flask-DigestAuth-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/PKG-INFO` & `Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-DigestAuth
-Version: 0.6.0
+Version: 0.6.1
 Summary: The Flask HTTP Digest Authentication project.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://flask-digestauth.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/flask-digestauth
 Project-URL: Bug Tracker, https://github.com/imacat/flask-digestauth/issues
 Keywords: flask,digest-authentication
```

### Comparing `Flask-DigestAuth-0.6.0/src/Flask_DigestAuth.egg-info/SOURCES.txt` & `Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/src/flask_digest_auth/__init__.py` & `Flask-DigestAuth-0.6.1/src/flask_digest_auth/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 """The HTTP digest authentication.
 
 """
 from flask_digest_auth.algo import make_password_hash, calc_response
 from flask_digest_auth.auth import DigestAuth
 from flask_digest_auth.test import Client
 
-VERSION: str = "0.6.0"
+VERSION: str = "0.6.1"
 """The package version."""
```

### Comparing `Flask-DigestAuth-0.6.0/src/flask_digest_auth/algo.py` & `Flask-DigestAuth-0.6.1/src/flask_digest_auth/algo.py`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/src/flask_digest_auth/auth.py` & `Flask-DigestAuth-0.6.1/src/flask_digest_auth/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         if len(self.__domain) > 0:
             domain_list: str = ",".join(self.__domain)
             header += f", domain=\"{domain_list}\""
         header += f", nonce=\"{nonce}\""
         if opaque is not None:
             header += f", opaque=\"{opaque}\""
         if state.stale is not None:
-            header += f", stale=TRUE" if state.stale else f", stale=FALSE"
+            header += ", stale=TRUE" if state.stale else ", stale=FALSE"
         if self.algorithm is not None:
             header += f", algorithm=\"{self.algorithm}\""
         if len(self.__qop) > 0:
             qop_list: str = ",".join(self.__qop)
             header += f", qop=\"{qop_list}\""
         return header
 
@@ -340,58 +340,65 @@
         :return: None.
         """
         app.extensions["digest_auth"] = self
         if "DIGEST_AUTH_REALM" in app.config:
             self.realm = app.config["DIGEST_AUTH_REALM"]
 
         if hasattr(app, "login_manager"):
-            from flask_login import LoginManager, login_user
+            self.__init_login_manager(app)
 
-            login_manager: LoginManager = getattr(app, "login_manager")
+    def __init_login_manager(self, app: Flask) -> None:
+        """Initializes the Flask-Login login manager.
 
-            @login_manager.unauthorized_handler
-            def unauthorized() -> None:
-                """Handles when the user is unauthorized.
+        :param app: The Flask application.
+        :return: None.
+        """
+        from flask_login import LoginManager, login_user
+        login_manager: LoginManager = getattr(app, "login_manager")
 
-                :return: None.
-                """
-                state: AuthState = getattr(request, "_digest_auth_state") \
-                    if hasattr(request, "_digest_auth_state") \
-                    else AuthState()
-                response: Response = Response()
-                response.status = 401
-                response.headers["WWW-Authenticate"] \
-                    = self.__make_response_header(state)
-                abort(response)
-
-            @login_manager.request_loader
-            def load_user_from_request(req: Request) -> Optional[Any]:
-                """Loads the user from the request header.
-
-                :param req: The request.
-                :return: The authenticated user, or None if the
-                    authentication fails
-                """
-                request._digest_auth_state = AuthState()
-                authorization: Authorization = req.authorization
-                try:
-                    if authorization is None:
-                        raise UnauthorizedException
-                    if authorization.type != "digest":
-                        raise UnauthorizedException(
-                            "Not an HTTP digest authorization")
-                    self.__authenticate(request._digest_auth_state)
-                    user = login_manager.user_callback(authorization.username)
-                    login_user(user)
-                    self.__on_login(user)
-                    return user
-                except UnauthorizedException as e:
-                    if str(e) != "":
-                        app.logger.warning(str(e))
-                    return None
+        @login_manager.unauthorized_handler
+        def unauthorized() -> None:
+            """Handles when the user is unauthorized.
+
+            :return: None.
+            """
+            state: AuthState = getattr(request, "_digest_auth_state") \
+                if hasattr(request, "_digest_auth_state") \
+                else AuthState()
+            response: Response = Response()
+            response.status = 401
+            response.headers["WWW-Authenticate"] \
+                = self.__make_response_header(state)
+            abort(response)
+
+        @login_manager.request_loader
+        def load_user_from_request(req: Request) -> Optional[Any]:
+            """Loads the user from the request header.
+
+            :param req: The request.
+            :return: The authenticated user, or None if the
+                authentication fails
+            """
+            request._digest_auth_state = AuthState()
+            authorization: Authorization = req.authorization
+            try:
+                if authorization is None:
+                    raise UnauthorizedException
+                if authorization.type != "digest":
+                    raise UnauthorizedException(
+                        "Not an HTTP digest authorization")
+                self.__authenticate(request._digest_auth_state)
+                user = login_manager.user_callback(authorization.username)
+                login_user(user)
+                self.__on_login(user)
+                return user
+            except UnauthorizedException as e:
+                if str(e) != "":
+                    app.logger.warning(str(e))
+                return None
 
     def logout(self) -> None:
         """Logs out the user.
         This actually causes the next authentication to fail, which forces
         the browser to ask the user for the username and password again.
 
         :Example:
```

### Comparing `Flask-DigestAuth-0.6.0/src/flask_digest_auth/test.py` & `Flask-DigestAuth-0.6.1/src/flask_digest_auth/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 """
 from secrets import token_urlsafe
 from typing import Optional, Literal, Tuple, Dict
 
 from flask import g
 from werkzeug.datastructures import Authorization, WWWAuthenticate
+from werkzeug.http import parse_set_header
 from werkzeug.test import TestResponse, Client as WerkzeugClient
 
 from flask_digest_auth.algo import calc_response, make_password_hash
 
 
 class Client(WerkzeugClient):
     """The test client with HTTP digest authentication enabled.
@@ -114,15 +115,15 @@
         :param www_authenticate: The ``WWW-Authenticate`` response.
         :param uri: The request URI.
         :param username: The username.
         :param password: The password.
         :return: The request authorization.
         """
         qop: Optional[Literal["auth", "auth-int"]] = None
-        if www_authenticate.qop is not None and "auth" in www_authenticate.qop:
+        if "auth" in parse_set_header(www_authenticate.get("qop")):
             qop = "auth"
 
         cnonce: Optional[str] = None
         if qop is not None or www_authenticate.algorithm == "MD5-sess":
             cnonce = token_urlsafe(8)
         nc: Optional[str] = None
         count: int = 1
```

### Comparing `Flask-DigestAuth-0.6.0/tests/test_algo.py` & `Flask-DigestAuth-0.6.1/tests/test_algo.py`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.0/tests/test_auth.py` & `Flask-DigestAuth-0.6.1/tests/test_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,32 +154,32 @@
         www_authenticate: WWWAuthenticate
         auth_data: Authorization
 
         response = super(Client, self.client).get(admin_uri)
         self.assertEqual(response.status_code, 401)
         www_authenticate = response.www_authenticate
         self.assertEqual(www_authenticate.type, "digest")
-        self.assertEqual(www_authenticate.stale, None)
+        self.assertIsNone(www_authenticate.get("stale"))
         opaque: str = www_authenticate.opaque
 
         www_authenticate.nonce = "bad"
         auth_data = Client.make_authorization(
             www_authenticate, admin_uri, _USERNAME, _PASSWORD)
         response = super(Client, self.client).get(admin_uri, auth=auth_data)
         self.assertEqual(response.status_code, 401)
         www_authenticate = response.www_authenticate
-        self.assertEqual(www_authenticate.stale, True)
+        self.assertEqual(www_authenticate.get("stale"), "TRUE")
         self.assertEqual(www_authenticate.opaque, opaque)
 
         auth_data = Client.make_authorization(
             www_authenticate, admin_uri, _USERNAME, _PASSWORD + "2")
         response = super(Client, self.client).get(admin_uri, auth=auth_data)
         self.assertEqual(response.status_code, 401)
         www_authenticate = response.www_authenticate
-        self.assertEqual(www_authenticate.stale, False)
+        self.assertEqual(www_authenticate.get("stale"), "FALSE")
         self.assertEqual(www_authenticate.opaque, opaque)
 
         auth_data = Client.make_authorization(
             www_authenticate, admin_uri, _USERNAME, _PASSWORD)
         response = super(Client, self.client).get(admin_uri, auth=auth_data)
         self.assertEqual(response.status_code, 200)
```

### Comparing `Flask-DigestAuth-0.6.0/tests/test_flask_login.py` & `Flask-DigestAuth-0.6.1/tests/test_flask_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,36 +191,36 @@
         www_authenticate: WWWAuthenticate
         auth_data: Authorization
 
         response = super(Client, self.client).get(admin_uri)
         self.assertEqual(response.status_code, 401)
         www_authenticate = response.www_authenticate
         self.assertEqual(www_authenticate.type, "digest")
-        self.assertEqual(www_authenticate.stale, None)
+        self.assertIsNone(www_authenticate.get("stale"))
         opaque: str = www_authenticate.opaque
 
         if hasattr(g, "_login_user"):
             delattr(g, "_login_user")
         www_authenticate.nonce = "bad"
         auth_data = Client.make_authorization(
             www_authenticate, admin_uri, _USERNAME, _PASSWORD)
         response = super(Client, self.client).get(admin_uri, auth=auth_data)
         self.assertEqual(response.status_code, 401)
         www_authenticate = response.www_authenticate
-        self.assertEqual(www_authenticate.stale, True)
+        self.assertEqual(www_authenticate.get("stale"), "TRUE")
         self.assertEqual(www_authenticate.opaque, opaque)
 
         if hasattr(g, "_login_user"):
             delattr(g, "_login_user")
         auth_data = Client.make_authorization(
             www_authenticate, admin_uri, _USERNAME, _PASSWORD + "2")
         response = super(Client, self.client).get(admin_uri, auth=auth_data)
         self.assertEqual(response.status_code, 401)
         www_authenticate = response.www_authenticate
-        self.assertEqual(www_authenticate.stale, False)
+        self.assertEqual(www_authenticate.get("stale"), "FALSE")
         self.assertEqual(www_authenticate.opaque, opaque)
 
         if hasattr(g, "_login_user"):
             delattr(g, "_login_user")
         auth_data = Client.make_authorization(
             www_authenticate, admin_uri, _USERNAME, _PASSWORD)
         response = super(Client, self.client).get(admin_uri, auth=auth_data)
```

