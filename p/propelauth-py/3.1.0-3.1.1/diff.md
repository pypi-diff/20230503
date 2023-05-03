# Comparing `tmp/propelauth-py-3.1.0.tar.gz` & `tmp/propelauth-py-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-py-3.1.0.tar", last modified: Fri Apr 21 18:23:38 2023, max compression
+gzip compressed data, was "propelauth-py-3.1.1.tar", last modified: Wed May  3 19:34:02 2023, max compression
```

## Comparing `propelauth-py-3.1.0.tar` & `propelauth-py-3.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:23:38.440192 propelauth-py-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-21 18:23:38.440192 propelauth-py-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:23:38.436191 propelauth-py-3.1.0/propelauth_py/
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20409 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/auth_fns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/propelauth_py/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:23:38.440192 propelauth-py-3.1.0/propelauth_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-21 18:23:38.000000 propelauth-py-3.1.0/propelauth_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-21 18:23:38.000000 propelauth-py-3.1.0/propelauth_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:23:38.000000 propelauth-py-3.1.0/propelauth_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 18:23:38.000000 propelauth-py-3.1.0/propelauth_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 18:23:38.000000 propelauth-py-3.1.0/propelauth_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 18:23:38.440192 propelauth-py-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-21 18:23:29.000000 propelauth-py-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:34:02.270700 propelauth-py-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-03 19:34:02.270700 propelauth-py-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:34:02.266700 propelauth-py-3.1.1/propelauth_py/
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20409 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/auth_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/propelauth_py/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:34:02.270700 propelauth-py-3.1.1/propelauth_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-03 19:34:02.000000 propelauth-py-3.1.1/propelauth_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-03 19:34:02.000000 propelauth-py-3.1.1/propelauth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:34:02.000000 propelauth-py-3.1.1/propelauth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 19:34:02.000000 propelauth-py-3.1.1/propelauth_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 19:34:02.000000 propelauth-py-3.1.1/propelauth_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:34:02.270700 propelauth-py-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-03 19:33:51.000000 propelauth-py-3.1.1/setup.py
```

### Comparing `propelauth-py-3.1.0/LICENSE` & `propelauth-py-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.0/PKG-INFO` & `propelauth-py-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-py
-Version: 3.1.0
+Version: 3.1.1
 Summary: A python authentication library
 Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.0 Summary: A python
+Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.1 Summary: A python
 authentication library Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth Author-email: support@propelauth.com License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE #
 PropelAuth Python SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A python library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-python). [PropelAuth](https://
```

### Comparing `propelauth-py-3.1.0/README.md` & `propelauth-py-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.0/propelauth_py/__init__.py` & `propelauth-py-3.1.1/propelauth_py/__init__.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.0/propelauth_py/api.py` & `propelauth-py-3.1.1/propelauth_py/api.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.0/propelauth_py/auth_fns.py` & `propelauth-py-3.1.1/propelauth_py/auth_fns.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.0/propelauth_py/errors.py` & `propelauth-py-3.1.1/propelauth_py/errors.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.0/propelauth_py/jwt.py` & `propelauth-py-3.1.1/propelauth_py/jwt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import datetime
+
 import jwt
 
 from propelauth_py.errors import UnauthorizedException
 from propelauth_py.user import _to_user
 
 OPTIONS = {
     "verify_signature": True,
@@ -14,13 +16,14 @@
 
 def _validate_access_token_and_get_user(access_token, token_verification_metadata):
     try:
         decoded_token = jwt.decode(access_token,
                                    token_verification_metadata.verifier_key,
                                    options=OPTIONS,
                                    issuer=token_verification_metadata.issuer,
-                                   algorithms=["RS256"])
+                                   algorithms=["RS256"],
+                                   leeway=datetime.timedelta(seconds=60))
         return _to_user(decoded_token)
     except UnauthorizedException as e:
         raise e
     except Exception:
         raise UnauthorizedException.invalid_access_token()
```

### Comparing `propelauth-py-3.1.0/propelauth_py/user.py` & `propelauth-py-3.1.1/propelauth_py/user.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.0/propelauth_py.egg-info/PKG-INFO` & `propelauth-py-3.1.1/propelauth_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-py
-Version: 3.1.0
+Version: 3.1.1
 Summary: A python authentication library
 Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.0 Summary: A python
+Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.1 Summary: A python
 authentication library Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth Author-email: support@propelauth.com License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE #
 PropelAuth Python SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A python library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-python). [PropelAuth](https://
```

### Comparing `propelauth-py-3.1.0/setup.py` & `propelauth-py-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-py",
-    version="3.1.0",
+    version="3.1.1",
     description="A python authentication library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-py",
     packages=find_packages(include=["propelauth_py"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
```

