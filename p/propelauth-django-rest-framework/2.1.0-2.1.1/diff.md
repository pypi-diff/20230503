# Comparing `tmp/propelauth-django-rest-framework-2.1.0.tar.gz` & `tmp/propelauth-django-rest-framework-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-django-rest-framework-2.1.0.tar", last modified: Fri Apr 21 20:00:10 2023, max compression
+gzip compressed data, was "propelauth-django-rest-framework-2.1.1.tar", last modified: Wed May  3 20:16:46 2023, max compression
```

## Comparing `propelauth-django-rest-framework-2.1.0.tar` & `propelauth-django-rest-framework-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:00:10.183692 propelauth-django-rest-framework-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-21 19:59:56.000000 propelauth-django-rest-framework-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-21 20:00:10.183692 propelauth-django-rest-framework-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-21 19:59:56.000000 propelauth-django-rest-framework-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:00:10.183692 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-21 19:59:56.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-04-21 19:59:56.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework/auth_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:00:10.183692 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-21 20:00:10.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-21 20:00:10.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:00:10.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 20:00:10.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 20:00:10.000000 propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 20:00:10.183692 propelauth-django-rest-framework-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-21 19:59:56.000000 propelauth-django-rest-framework-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:16:46.411040 propelauth-django-rest-framework-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 20:16:31.000000 propelauth-django-rest-framework-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-03 20:16:46.407039 propelauth-django-rest-framework-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-03 20:16:31.000000 propelauth-django-rest-framework-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:16:46.407039 propelauth-django-rest-framework-2.1.1/propelauth_django_rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-03 20:16:31.000000 propelauth-django-rest-framework-2.1.1/propelauth_django_rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-05-03 20:16:31.000000 propelauth-django-rest-framework-2.1.1/propelauth_django_rest_framework/auth_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:16:46.407039 propelauth-django-rest-framework-2.1.1/propelauth_django_rest_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-03 20:16:46.000000 propelauth-django-rest-framework-2.1.1/propelauth_django_rest_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-03 20:16:46.000000 propelauth-django-rest-framework-2.1.1/propelauth_django_rest_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:16:46.000000 propelauth-django-rest-framework-2.1.1/propelauth_django_rest_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 20:16:46.000000 propelauth-django-rest-framework-2.1.1/propelauth_django_rest_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-03 20:16:46.000000 propelauth-django-rest-framework-2.1.1/propelauth_django_rest_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:16:46.411040 propelauth-django-rest-framework-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-03 20:16:31.000000 propelauth-django-rest-framework-2.1.1/setup.py
```

### Comparing `propelauth-django-rest-framework-2.1.0/LICENSE` & `propelauth-django-rest-framework-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.1.0/PKG-INFO` & `propelauth-django-rest-framework-2.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-django-rest-framework
-Version: 2.1.0
+Version: 2.1.1
 Summary: A library for managing authentication in Django Rest Framework
 Home-page: https://github.com/propelauth/propelauth-django-rest-framework
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.0
+Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.1
 Summary: A library for managing authentication in Django Rest Framework Home-
 page: https://github.com/propelauth/propelauth-django-rest-framework Author:
 PropelAuth Author-email: support@propelauth.com License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown License-File: LICENSE # PropelAuth
 Django Rest Framework Library
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A Django Rest Framework library for managing authentication, backed by
```

### Comparing `propelauth-django-rest-framework-2.1.0/README.md` & `propelauth-django-rest-framework-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework/__init__.py` & `propelauth-django-rest-framework-2.1.1/propelauth_django_rest_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework/auth_helpers.py` & `propelauth-django-rest-framework-2.1.1/propelauth_django_rest_framework/auth_helpers.py`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.1.0/propelauth_django_rest_framework.egg-info/PKG-INFO` & `propelauth-django-rest-framework-2.1.1/propelauth_django_rest_framework.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-django-rest-framework
-Version: 2.1.0
+Version: 2.1.1
 Summary: A library for managing authentication in Django Rest Framework
 Home-page: https://github.com/propelauth/propelauth-django-rest-framework
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.0
+Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.1
 Summary: A library for managing authentication in Django Rest Framework Home-
 page: https://github.com/propelauth/propelauth-django-rest-framework Author:
 PropelAuth Author-email: support@propelauth.com License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown License-File: LICENSE # PropelAuth
 Django Rest Framework Library
       [https://propelauth-logos.s3.us-west-2.amazonaws.com/logo-only.png]
 A Django Rest Framework library for managing authentication, backed by
```

### Comparing `propelauth-django-rest-framework-2.1.0/setup.py` & `propelauth-django-rest-framework-2.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 setup(
     name="propelauth-django-rest-framework",
-    version="2.1.0",
+    version="2.1.1",
     description="A library for managing authentication in Django Rest Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-django-rest-framework",
     packages=find_packages(include=["propelauth_django_rest_framework"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
     license="MIT",
-    install_requires=["django", "djangorestframework", "propelauth-py==3.1.0", "requests"],
+    install_requires=["django", "djangorestframework", "propelauth-py==3.1.1", "requests"],
     setup_requires=pytest_runner,
     tests_require=["pytest==4.4.1"],
     test_suite="tests",
 )
```

