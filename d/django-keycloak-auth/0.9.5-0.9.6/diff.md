# Comparing `tmp/django-keycloak-auth-0.9.5.tar.gz` & `tmp/django-keycloak-auth-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-keycloak-auth-0.9.5.tar", last modified: Mon Nov 29 16:26:29 2021, max compression
+gzip compressed data, was "django-keycloak-auth-0.9.6.tar", last modified: Wed May  3 13:57:22 2023, max compression
```

## Comparing `django-keycloak-auth-0.9.5.tar` & `django-keycloak-auth-0.9.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 marcelo   (1000) marcelo   (1000)        0 2021-11-29 16:26:29.309374 django-keycloak-auth-0.9.5/
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     1090 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/LICENSE
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      100 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/MANIFEST.in
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)    10404 2021-11-29 16:26:29.309374 django-keycloak-auth-0.9.5/PKG-INFO
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     7285 2021-11-25 16:42:56.000000 django-keycloak-auth-0.9.5/README.md
-drwxrwxr-x   0 marcelo   (1000) marcelo   (1000)        0 2021-11-29 16:26:29.309374 django-keycloak-auth-0.9.5/core/
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)        0 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/core/__init__.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)       63 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/core/admin.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)       83 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/core/apps.py
-drwxrwxr-x   0 marcelo   (1000) marcelo   (1000)        0 2021-11-29 16:26:29.309374 django-keycloak-auth-0.9.5/core/migrations/
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      619 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/core/migrations/0001_initial.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)        0 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/core/migrations/__init__.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      285 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/core/models.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      183 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/core/serializers.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)       60 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/core/tests.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      246 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/core/urls.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     2081 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/core/views.py
-drwxrwxr-x   0 marcelo   (1000) marcelo   (1000)        0 2021-11-29 16:26:29.309374 django-keycloak-auth-0.9.5/django-keycloak-auth/
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)        0 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/django-keycloak-auth/__init__.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     7413 2021-11-29 16:04:30.000000 django-keycloak-auth-0.9.5/django-keycloak-auth/keycloak.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     5479 2021-11-25 15:49:16.000000 django-keycloak-auth-0.9.5/django-keycloak-auth/middleware.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     4009 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/django-keycloak-auth/settings.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)    11223 2021-11-25 16:38:48.000000 django-keycloak-auth-0.9.5/django-keycloak-auth/tests.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      939 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/django-keycloak-auth/urls.py
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      417 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.5/django-keycloak-auth/wsgi.py
-drwxrwxr-x   0 marcelo   (1000) marcelo   (1000)        0 2021-11-29 16:26:29.309374 django-keycloak-auth-0.9.5/django_keycloak_auth.egg-info/
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)    10404 2021-11-29 16:26:29.000000 django-keycloak-auth-0.9.5/django_keycloak_auth.egg-info/PKG-INFO
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      669 2021-11-29 16:26:29.000000 django-keycloak-auth-0.9.5/django_keycloak_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)        1 2021-11-29 16:26:29.000000 django-keycloak-auth-0.9.5/django_keycloak_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)       52 2021-11-29 16:26:29.000000 django-keycloak-auth-0.9.5/django_keycloak_auth.egg-info/requires.txt
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)       26 2021-11-29 16:26:29.000000 django-keycloak-auth-0.9.5/django_keycloak_auth.egg-info/top_level.txt
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)       79 2021-11-29 16:26:29.309374 django-keycloak-auth-0.9.5/setup.cfg
--rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     1619 2021-11-25 16:39:40.000000 django-keycloak-auth-0.9.5/setup.py
+drwxrwxr-x   0 marcelo   (1000) marcelo   (1000)        0 2023-05-03 13:57:22.767361 django-keycloak-auth-0.9.6/
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     1090 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/LICENSE
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      100 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/MANIFEST.in
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)    10624 2023-05-03 13:57:22.767361 django-keycloak-auth-0.9.6/PKG-INFO
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     7449 2023-05-03 13:55:31.000000 django-keycloak-auth-0.9.6/README.md
+drwxrwxr-x   0 marcelo   (1000) marcelo   (1000)        0 2023-05-03 13:57:22.767361 django-keycloak-auth-0.9.6/core/
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)        0 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/core/__init__.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)       63 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/core/admin.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)       83 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/core/apps.py
+drwxrwxr-x   0 marcelo   (1000) marcelo   (1000)        0 2023-05-03 13:57:22.767361 django-keycloak-auth-0.9.6/core/migrations/
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      619 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/core/migrations/0001_initial.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)        0 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/core/migrations/__init__.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      285 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/core/models.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      183 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/core/serializers.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)       60 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/core/tests.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      246 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/core/urls.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     2081 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/core/views.py
+drwxrwxr-x   0 marcelo   (1000) marcelo   (1000)        0 2023-05-03 13:57:22.767361 django-keycloak-auth-0.9.6/django-keycloak-auth/
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)        0 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/django-keycloak-auth/__init__.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     8485 2023-05-03 13:54:16.000000 django-keycloak-auth-0.9.6/django-keycloak-auth/keycloak.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     5479 2023-05-03 13:45:44.000000 django-keycloak-auth-0.9.6/django-keycloak-auth/middleware.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     4009 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/django-keycloak-auth/settings.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)    12408 2023-05-03 13:54:16.000000 django-keycloak-auth-0.9.6/django-keycloak-auth/tests.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      939 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/django-keycloak-auth/urls.py
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      417 2021-11-25 15:39:50.000000 django-keycloak-auth-0.9.6/django-keycloak-auth/wsgi.py
+drwxrwxr-x   0 marcelo   (1000) marcelo   (1000)        0 2023-05-03 13:57:22.767361 django-keycloak-auth-0.9.6/django_keycloak_auth.egg-info/
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)    10624 2023-05-03 13:57:22.000000 django-keycloak-auth-0.9.6/django_keycloak_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)      669 2023-05-03 13:57:22.000000 django-keycloak-auth-0.9.6/django_keycloak_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)        1 2023-05-03 13:57:22.000000 django-keycloak-auth-0.9.6/django_keycloak_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)       52 2023-05-03 13:57:22.000000 django-keycloak-auth-0.9.6/django_keycloak_auth.egg-info/requires.txt
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)       26 2023-05-03 13:57:22.000000 django-keycloak-auth-0.9.6/django_keycloak_auth.egg-info/top_level.txt
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)       79 2023-05-03 13:57:22.771361 django-keycloak-auth-0.9.6/setup.cfg
+-rw-rw-r--   0 marcelo   (1000) marcelo   (1000)     1619 2023-05-03 13:56:46.000000 django-keycloak-auth-0.9.6/setup.py
```

### Comparing `django-keycloak-auth-0.9.5/LICENSE` & `django-keycloak-auth-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-keycloak-auth-0.9.5/PKG-INFO` & `django-keycloak-auth-0.9.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: django-keycloak-auth
-Version: 0.9.5
+Version: 0.9.6
 Summary: Django Keycloak Auth is Python package providing access to the Keycloak API.
 Home-page: https://github.com/marcelo225/django-keycloak-auth
 Author: Marcelo Vinicius
 Author-email: mr.225@hotmail.com
 License: UNKNOWN
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, https://github.com/marcelo225/django-keycloak-auth
 Project-URL: Source, https://github.com/marcelo225/django-keycloak-auth
 Project-URL: Tracker, https://github.com/marcelo225/django-keycloak-auth/issues
 Description: # Django Keycloak Auth
         
         - [Django Keycloak Auth](#django-keycloak-auth)
           - [What is it?](#what-is-it)
+          - [Buy me a coffee](#buy-me-a-coffee)
           - [Installation](#installation)
             - [Via Pypi Package:](#via-pypi-package)
             - [Manually](#manually)
           - [Dependencies](#dependencies)
           - [Test dependences](#test-dependences)
           - [How to contribute](#how-to-contribute)
           - [Licence](#licence)
@@ -60,14 +61,20 @@
           ...
         ```
         
         For review see https://github.com/marcelo225/django-keycloak-auth
         
         Package link: https://pypi.org/project/django-keycloak-auth/
         
+        ## Buy me a coffee
+        
+        If you have recognized my effort in this initiative, please buy me a coffee when possible.
+        
+        ![coffee](qr_code.png)
+        
         ## Installation
         
         ### Via Pypi Package:
         
         ``` $ pip install django-keycloak-auth ```
         
         ### Manually
@@ -250,15 +257,15 @@
         If you interested contribute to developing this project, it was prepared a tiny tutorial to install the environment before you begin:
         
         ```bash
         # Install venv in root project folder
         $ python3 -m venv env && source env/bin/activate
         
         # Update packages for development
-        $ python -m pip install --upgrade -r requirements-development.txt
+        $ python -m pip install --upgrade -r requirements.txt
         
         # Generate distribuition -> it's on me for while ;)
         $ python setup.py sdist
         
         # Checks if the package has no errors
         $ twine check dist/*
```

### Comparing `django-keycloak-auth-0.9.5/README.md` & `django-keycloak-auth-0.9.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Django Keycloak Auth
 
 - [Django Keycloak Auth](#django-keycloak-auth)
   - [What is it?](#what-is-it)
+  - [Buy me a coffee](#buy-me-a-coffee)
   - [Installation](#installation)
     - [Via Pypi Package:](#via-pypi-package)
     - [Manually](#manually)
   - [Dependencies](#dependencies)
   - [Test dependences](#test-dependences)
   - [How to contribute](#how-to-contribute)
   - [Licence](#licence)
@@ -48,14 +49,20 @@
   ...
 ```
 
 For review see https://github.com/marcelo225/django-keycloak-auth
 
 Package link: https://pypi.org/project/django-keycloak-auth/
 
+## Buy me a coffee
+
+If you have recognized my effort in this initiative, please buy me a coffee when possible.
+
+![coffee](qr_code.png)
+
 ## Installation
 
 ### Via Pypi Package:
 
 ``` $ pip install django-keycloak-auth ```
 
 ### Manually
@@ -238,15 +245,15 @@
 If you interested contribute to developing this project, it was prepared a tiny tutorial to install the environment before you begin:
 
 ```bash
 # Install venv in root project folder
 $ python3 -m venv env && source env/bin/activate
 
 # Update packages for development
-$ python -m pip install --upgrade -r requirements-development.txt
+$ python -m pip install --upgrade -r requirements.txt
 
 # Generate distribuition -> it's on me for while ;)
 $ python setup.py sdist
 
 # Checks if the package has no errors
 $ twine check dist/*
```

### Comparing `django-keycloak-auth-0.9.5/core/migrations/0001_initial.py` & `django-keycloak-auth-0.9.6/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-auth-0.9.5/core/views.py` & `django-keycloak-auth-0.9.6/core/views.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-auth-0.9.5/django-keycloak-auth/middleware.py` & `django-keycloak-auth-0.9.6/django-keycloak-auth/middleware.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-auth-0.9.5/django-keycloak-auth/settings.py` & `django-keycloak-auth-0.9.6/django-keycloak-auth/settings.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-auth-0.9.5/django-keycloak-auth/tests.py` & `django-keycloak-auth-0.9.6/django-keycloak-auth/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.test import TestCase, Client, RequestFactory
+from requests import HTTPError
 from rest_framework import status
 from django.conf import settings
 from .middleware import KeycloakMiddleware, KeycloakConnect
 from core import views
 from unittest.mock import Mock
 
 
@@ -269,7 +270,35 @@
                                    settings.KEYCLOAK_CONFIG['KEYCLOAK_CLIENT_ID'])
         keycloak.introspect = Mock(return_value=fake_token)
         keycloak.userinfo = Mock(return_value=fake_token)
         
         userinfo = keycloak.userinfo(Mock())        
         
         self.assertEquals(fake_token['sub'], userinfo['sub'])
+
+    def test_keycloak_connect_well_known(self):
+        """Test keycloak endpoint well_known when status >= 400"""
+        keycloak = KeycloakConnect(
+            settings.KEYCLOAK_CONFIG['KEYCLOAK_REALM'],
+            settings.KEYCLOAK_CONFIG['KEYCLOAK_REALM'],
+            settings.KEYCLOAK_CONFIG['KEYCLOAK_CLIENT_ID'],
+        )
+        keycloak._send_request = Mock(side_effect=HTTPError)
+        result = keycloak.well_known(raise_exception=False)
+        self.assertDictEqual({}, result)
+
+        with self.assertRaises(HTTPError):
+            keycloak.well_known()
+
+    def test_keycloak_connect_introspect(self):
+        """Test keycloak endpoint introspect when status >= 400"""
+        keycloak = KeycloakConnect(
+            settings.KEYCLOAK_CONFIG['KEYCLOAK_REALM'],
+            settings.KEYCLOAK_CONFIG['KEYCLOAK_REALM'],
+            settings.KEYCLOAK_CONFIG['KEYCLOAK_CLIENT_ID'],
+        )
+        keycloak._send_request = Mock(side_effect=HTTPError)
+        result = keycloak.introspect('', raise_exception=False)
+        self.assertDictEqual({}, result)
+
+        with self.assertRaises(HTTPError):
+            keycloak.introspect('')
```

### Comparing `django-keycloak-auth-0.9.5/django-keycloak-auth/urls.py` & `django-keycloak-auth-0.9.6/django-keycloak-auth/urls.py`

 * *Files identical despite different names*

### Comparing `django-keycloak-auth-0.9.5/django_keycloak_auth.egg-info/PKG-INFO` & `django-keycloak-auth-0.9.6/django_keycloak_auth.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: django-keycloak-auth
-Version: 0.9.5
+Version: 0.9.6
 Summary: Django Keycloak Auth is Python package providing access to the Keycloak API.
 Home-page: https://github.com/marcelo225/django-keycloak-auth
 Author: Marcelo Vinicius
 Author-email: mr.225@hotmail.com
 License: UNKNOWN
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, https://github.com/marcelo225/django-keycloak-auth
 Project-URL: Source, https://github.com/marcelo225/django-keycloak-auth
 Project-URL: Tracker, https://github.com/marcelo225/django-keycloak-auth/issues
 Description: # Django Keycloak Auth
         
         - [Django Keycloak Auth](#django-keycloak-auth)
           - [What is it?](#what-is-it)
+          - [Buy me a coffee](#buy-me-a-coffee)
           - [Installation](#installation)
             - [Via Pypi Package:](#via-pypi-package)
             - [Manually](#manually)
           - [Dependencies](#dependencies)
           - [Test dependences](#test-dependences)
           - [How to contribute](#how-to-contribute)
           - [Licence](#licence)
@@ -60,14 +61,20 @@
           ...
         ```
         
         For review see https://github.com/marcelo225/django-keycloak-auth
         
         Package link: https://pypi.org/project/django-keycloak-auth/
         
+        ## Buy me a coffee
+        
+        If you have recognized my effort in this initiative, please buy me a coffee when possible.
+        
+        ![coffee](qr_code.png)
+        
         ## Installation
         
         ### Via Pypi Package:
         
         ``` $ pip install django-keycloak-auth ```
         
         ### Manually
@@ -250,15 +257,15 @@
         If you interested contribute to developing this project, it was prepared a tiny tutorial to install the environment before you begin:
         
         ```bash
         # Install venv in root project folder
         $ python3 -m venv env && source env/bin/activate
         
         # Update packages for development
-        $ python -m pip install --upgrade -r requirements-development.txt
+        $ python -m pip install --upgrade -r requirements.txt
         
         # Generate distribuition -> it's on me for while ;)
         $ python setup.py sdist
         
         # Checks if the package has no errors
         $ twine check dist/*
```

### Comparing `django-keycloak-auth-0.9.5/django_keycloak_auth.egg-info/SOURCES.txt` & `django-keycloak-auth-0.9.6/django_keycloak_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-keycloak-auth-0.9.5/setup.py` & `django-keycloak-auth-0.9.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="django-keycloak-auth",
-    version="0.9.5",
+    version="0.9.6",
     packages=find_packages(),
 
     # Project uses reStructuredText, so ensure that the docutils get
     # installed or upgraded on the target machine
     install_requires=[
         "Django",
         "djangorestframework>=3.10.0",
```

