# Comparing `tmp/propelauth-flask-2.1.0.tar.gz` & `tmp/propelauth-flask-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-flask-2.1.0.tar", last modified: Fri Apr 21 19:59:23 2023, max compression
+gzip compressed data, was "propelauth-flask-2.1.1.tar", last modified: Wed May  3 20:16:27 2023, max compression
```

## Comparing `propelauth-flask-2.1.0.tar` & `propelauth-flask-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:59:23.065268 propelauth-flask-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-21 19:59:05.000000 propelauth-flask-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-21 19:59:23.065268 propelauth-flask-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-21 19:59:05.000000 propelauth-flask-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:59:23.065268 propelauth-flask-2.1.0/propelauth_flask/
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-21 19:59:05.000000 propelauth-flask-2.1.0/propelauth_flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-21 19:59:05.000000 propelauth-flask-2.1.0/propelauth_flask/auth_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-21 19:59:05.000000 propelauth-flask-2.1.0/propelauth_flask/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:59:23.065268 propelauth-flask-2.1.0/propelauth_flask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-21 19:59:23.000000 propelauth-flask-2.1.0/propelauth_flask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-21 19:59:23.000000 propelauth-flask-2.1.0/propelauth_flask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:59:23.000000 propelauth-flask-2.1.0/propelauth_flask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 19:59:23.000000 propelauth-flask-2.1.0/propelauth_flask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 19:59:23.000000 propelauth-flask-2.1.0/propelauth_flask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 19:59:23.065268 propelauth-flask-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-21 19:59:05.000000 propelauth-flask-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:16:27.958166 propelauth-flask-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 20:16:14.000000 propelauth-flask-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-03 20:16:27.958166 propelauth-flask-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-03 20:16:14.000000 propelauth-flask-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:16:27.958166 propelauth-flask-2.1.1/propelauth_flask/
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-03 20:16:14.000000 propelauth-flask-2.1.1/propelauth_flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-03 20:16:14.000000 propelauth-flask-2.1.1/propelauth_flask/auth_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-03 20:16:14.000000 propelauth-flask-2.1.1/propelauth_flask/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:16:27.958166 propelauth-flask-2.1.1/propelauth_flask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-03 20:16:27.000000 propelauth-flask-2.1.1/propelauth_flask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-03 20:16:27.000000 propelauth-flask-2.1.1/propelauth_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:16:27.000000 propelauth-flask-2.1.1/propelauth_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 20:16:27.000000 propelauth-flask-2.1.1/propelauth_flask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 20:16:27.000000 propelauth-flask-2.1.1/propelauth_flask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:16:27.958166 propelauth-flask-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-03 20:16:14.000000 propelauth-flask-2.1.1/setup.py
```

### Comparing `propelauth-flask-2.1.0/LICENSE` & `propelauth-flask-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.1.0/PKG-INFO` & `propelauth-flask-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-flask
-Version: 2.1.0
+Version: 2.1.1
 Summary: A library for managing authentication in Flask
 Home-page: https://github.com/propelauth/propelauth-flask
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.0 Summary: A library
+Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.1 Summary: A library
 for managing authentication in Flask Home-page: https://github.com/propelauth/
 propelauth-flask Author: PropelAuth Author-email: support@propelauth.com
 License: MIT Platform: UNKNOWN Description-Content-Type: text/markdown License-
 File: LICENSE # PropelAuth Flask SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A Flask library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-flask). [PropelAuth](https://
```

### Comparing `propelauth-flask-2.1.0/README.md` & `propelauth-flask-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.1.0/propelauth_flask/__init__.py` & `propelauth-flask-2.1.1/propelauth_flask/__init__.py`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.1.0/propelauth_flask/auth_decorator.py` & `propelauth-flask-2.1.1/propelauth_flask/auth_decorator.py`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.1.0/propelauth_flask/user.py` & `propelauth-flask-2.1.1/propelauth_flask/user.py`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.1.0/propelauth_flask.egg-info/PKG-INFO` & `propelauth-flask-2.1.1/propelauth_flask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-flask
-Version: 2.1.0
+Version: 2.1.1
 Summary: A library for managing authentication in Flask
 Home-page: https://github.com/propelauth/propelauth-flask
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.0 Summary: A library
+Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.1 Summary: A library
 for managing authentication in Flask Home-page: https://github.com/propelauth/
 propelauth-flask Author: PropelAuth Author-email: support@propelauth.com
 License: MIT Platform: UNKNOWN Description-Content-Type: text/markdown License-
 File: LICENSE # PropelAuth Flask SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A Flask library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-flask). [PropelAuth](https://
```

### Comparing `propelauth-flask-2.1.0/setup.py` & `propelauth-flask-2.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-flask",
-    version="2.1.0",
+    version="2.1.1",
     description="A library for managing authentication in Flask",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-flask",
     packages=find_packages(include=["propelauth_flask"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
     license="MIT",
-    install_requires=["flask>=0.9", "propelauth-py==3.1.0", "requests"],
+    install_requires=["flask>=0.9", "propelauth-py==3.1.1", "requests"],
     setup_requires=pytest_runner,
     tests_require=["pytest==4.4.1"],
     test_suite="tests",
 )
```

