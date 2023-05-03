# Comparing `tmp/propelauth-fastapi-2.1.0.tar.gz` & `tmp/propelauth-fastapi-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-fastapi-2.1.0.tar", last modified: Fri Apr 21 19:59:54 2023, max compression
+gzip compressed data, was "propelauth-fastapi-2.1.1.tar", last modified: Wed May  3 20:17:11 2023, max compression
```

## Comparing `propelauth-fastapi-2.1.0.tar` & `propelauth-fastapi-2.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:59:54.875137 propelauth-fastapi-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-21 19:59:39.000000 propelauth-fastapi-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-21 19:59:54.871137 propelauth-fastapi-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-21 19:59:39.000000 propelauth-fastapi-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:59:54.871137 propelauth-fastapi-2.1.0/propelauth_fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-21 19:59:39.000000 propelauth-fastapi-2.1.0/propelauth_fastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:59:54.871137 propelauth-fastapi-2.1.0/propelauth_fastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-21 19:59:54.000000 propelauth-fastapi-2.1.0/propelauth_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-21 19:59:54.000000 propelauth-fastapi-2.1.0/propelauth_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:59:54.000000 propelauth-fastapi-2.1.0/propelauth_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-21 19:59:54.000000 propelauth-fastapi-2.1.0/propelauth_fastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 19:59:54.000000 propelauth-fastapi-2.1.0/propelauth_fastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 19:59:54.875137 propelauth-fastapi-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-21 19:59:39.000000 propelauth-fastapi-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:17:11.450207 propelauth-fastapi-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 20:16:56.000000 propelauth-fastapi-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-03 20:17:11.450207 propelauth-fastapi-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-03 20:16:56.000000 propelauth-fastapi-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:17:11.450207 propelauth-fastapi-2.1.1/propelauth_fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-03 20:16:56.000000 propelauth-fastapi-2.1.1/propelauth_fastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:17:11.450207 propelauth-fastapi-2.1.1/propelauth_fastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-03 20:17:11.000000 propelauth-fastapi-2.1.1/propelauth_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 20:17:11.000000 propelauth-fastapi-2.1.1/propelauth_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:17:11.000000 propelauth-fastapi-2.1.1/propelauth_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-03 20:17:11.000000 propelauth-fastapi-2.1.1/propelauth_fastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 20:17:11.000000 propelauth-fastapi-2.1.1/propelauth_fastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:17:11.450207 propelauth-fastapi-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-03 20:16:56.000000 propelauth-fastapi-2.1.1/setup.py
```

### Comparing `propelauth-fastapi-2.1.0/LICENSE` & `propelauth-fastapi-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-fastapi-2.1.0/PKG-INFO` & `propelauth-fastapi-2.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-fastapi
-Version: 2.1.0
+Version: 2.1.1
 Summary: A FastAPI library for managing authentication, backed by PropelAuth
 Home-page: https://github.com/propelauth/propelauth-fastapi
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-fastapi Version: 2.1.0 Summary: A
+Metadata-Version: 2.1 Name: propelauth-fastapi Version: 2.1.1 Summary: A
 FastAPI library for managing authentication, backed by PropelAuth Home-page:
 https://github.com/propelauth/propelauth-fastapi Author: PropelAuth Author-
 email: support@propelauth.com License: MIT Platform: UNKNOWN Description-
 Content-Type: text/markdown License-File: LICENSE # PropelAuth FastAPI SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A FastAPI library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-fastapi). [PropelAuth](https://
```

### Comparing `propelauth-fastapi-2.1.0/README.md` & `propelauth-fastapi-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-fastapi-2.1.0/propelauth_fastapi/__init__.py` & `propelauth-fastapi-2.1.1/propelauth_fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propelauth-fastapi-2.1.0/propelauth_fastapi.egg-info/PKG-INFO` & `propelauth-fastapi-2.1.1/propelauth_fastapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-fastapi
-Version: 2.1.0
+Version: 2.1.1
 Summary: A FastAPI library for managing authentication, backed by PropelAuth
 Home-page: https://github.com/propelauth/propelauth-fastapi
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-fastapi Version: 2.1.0 Summary: A
+Metadata-Version: 2.1 Name: propelauth-fastapi Version: 2.1.1 Summary: A
 FastAPI library for managing authentication, backed by PropelAuth Home-page:
 https://github.com/propelauth/propelauth-fastapi Author: PropelAuth Author-
 email: support@propelauth.com License: MIT Platform: UNKNOWN Description-
 Content-Type: text/markdown License-File: LICENSE # PropelAuth FastAPI SDK
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A FastAPI library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-fastapi). [PropelAuth](https://
```

### Comparing `propelauth-fastapi-2.1.0/setup.py` & `propelauth-fastapi-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-fastapi",
-    version="2.1.0",
+    version="2.1.1",
     description="A FastAPI library for managing authentication, backed by PropelAuth",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-fastapi",
     packages=find_packages(include=["propelauth_fastapi"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
     license="MIT",
-    install_requires=["propelauth-py==3.1.0", "requests"],
+    install_requires=["propelauth-py==3.1.1", "requests"],
     setup_requires=pytest_runner,
     tests_require=["pytest==4.4.1"],
     test_suite="tests",
 )
```

