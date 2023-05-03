# Comparing `tmp/django-rest-serializer-field-permissions-4.1.0.tar.gz` & `tmp/django-rest-serializer-field-permissions-4.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-rest-serializer-field-permissions-4.1.0.tar", last modified: Wed May  3 03:01:14 2023, max compression
+gzip compressed data, was "django-rest-serializer-field-permissions-4.1.0rc1.tar", last modified: Mon Apr 24 17:54:31 2023, max compression
```

## Comparing `django-rest-serializer-field-permissions-4.1.0.tar` & `django-rest-serializer-field-permissions-4.1.0rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 03:01:14.493671 django-rest-serializer-field-permissions-4.1.0/
--rw-rw-rw-   0        0        0    35797 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.1.0/LICENSE
--rw-rw-rw-   0        0        0       34 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8390 2023-05-03 03:01:14.493671 django-rest-serializer-field-permissions-4.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7475 2023-05-03 03:00:53.000000 django-rest-serializer-field-permissions-4.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 03:01:14.422573 django-rest-serializer-field-permissions-4.1.0/django_rest_serializer_field_permissions.egg-info/
--rw-rw-rw-   0        0        0     8390 2023-05-03 03:01:14.000000 django-rest-serializer-field-permissions-4.1.0/django_rest_serializer_field_permissions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      585 2023-05-03 03:01:14.000000 django-rest-serializer-field-permissions-4.1.0/django_rest_serializer_field_permissions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 03:01:14.000000 django-rest-serializer-field-permissions-4.1.0/django_rest_serializer_field_permissions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-03 03:01:14.000000 django-rest-serializer-field-permissions-4.1.0/django_rest_serializer_field_permissions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       44 2023-05-03 03:01:14.000000 django-rest-serializer-field-permissions-4.1.0/django_rest_serializer_field_permissions.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 03:01:14.487728 django-rest-serializer-field-permissions-4.1.0/rest_framework_serializer_field_permissions/
--rw-rw-rw-   0        0        0       83 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.1.0/rest_framework_serializer_field_permissions/__init__.py
--rw-rw-rw-   0        0        0     5277 2023-05-03 03:00:54.000000 django-rest-serializer-field-permissions-4.1.0/rest_framework_serializer_field_permissions/fields.py
--rw-rw-rw-   0        0        0     1491 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.1.0/rest_framework_serializer_field_permissions/permissions.py
--rw-rw-rw-   0        0        0     1323 2021-01-11 01:36:29.000000 django-rest-serializer-field-permissions-4.1.0/rest_framework_serializer_field_permissions/serializers.py
--rw-rw-rw-   0        0        0       42 2023-05-03 03:01:14.494671 django-rest-serializer-field-permissions-4.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1495 2023-05-03 03:00:54.000000 django-rest-serializer-field-permissions-4.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:54:31.079532 django-rest-serializer-field-permissions-4.1.0rc1/
+-rw-rw-rw-   0        0        0    35797 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.1.0rc1/LICENSE
+-rw-rw-rw-   0        0        0       34 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.1.0rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8393 2023-04-24 17:54:31.078387 django-rest-serializer-field-permissions-4.1.0rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     7475 2023-04-24 17:33:33.000000 django-rest-serializer-field-permissions-4.1.0rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 17:54:31.072173 django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/
+-rw-rw-rw-   0        0        0     8393 2023-04-24 17:54:31.000000 django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2023-04-24 17:54:31.000000 django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 17:54:31.000000 django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-24 17:54:31.000000 django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2023-04-24 17:54:31.000000 django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 17:54:31.077388 django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/
+-rw-rw-rw-   0        0        0       83 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/__init__.py
+-rw-rw-rw-   0        0        0     5277 2023-04-24 17:49:15.000000 django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/fields.py
+-rw-rw-rw-   0        0        0     1491 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/permissions.py
+-rw-rw-rw-   0        0        0     1323 2021-01-11 01:36:29.000000 django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/serializers.py
+-rw-rw-rw-   0        0        0       42 2023-04-24 17:54:31.079532 django-rest-serializer-field-permissions-4.1.0rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1498 2023-04-24 17:54:24.000000 django-rest-serializer-field-permissions-4.1.0rc1/setup.py
```

### Comparing `django-rest-serializer-field-permissions-4.1.0/LICENSE` & `django-rest-serializer-field-permissions-4.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-rest-serializer-field-permissions-4.1.0/PKG-INFO` & `django-rest-serializer-field-permissions-4.1.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rest-serializer-field-permissions
-Version: 4.1.0
+Version: 4.1.0rc1
 Summary: Field-by-field serializer permissions for Django Rest Framework.
 Home-page: https://github.com/InterSIS/django-rest-serializer-field-permissions/
 Author: The Intersis Foundation
 Author-email: dev@intersis.org
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -179,15 +179,15 @@
 Compatibility
 -------------
 
 This package is tested for compatibility against the following software versions:
 
 * Django Rest Framework 3.14.0
 * Django 3.2, 4.2
-* Python 3.8
+* Python 3.7
 
 This package may incidentally be compatible with other similar versions of the above software. See tox.ini for specific minor versions tested.
 
 Additional Requirements
 -----------------------
 
 None
```

### Comparing `django-rest-serializer-field-permissions-4.1.0/README.md` & `django-rest-serializer-field-permissions-4.1.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 Compatibility
 -------------
 
 This package is tested for compatibility against the following software versions:
 
 * Django Rest Framework 3.14.0
 * Django 3.2, 4.2
-* Python 3.8
+* Python 3.7
 
 This package may incidentally be compatible with other similar versions of the above software. See tox.ini for specific minor versions tested.
 
 Additional Requirements
 -----------------------
 
 None
```

### Comparing `django-rest-serializer-field-permissions-4.1.0/django_rest_serializer_field_permissions.egg-info/PKG-INFO` & `django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rest-serializer-field-permissions
-Version: 4.1.0
+Version: 4.1.0rc1
 Summary: Field-by-field serializer permissions for Django Rest Framework.
 Home-page: https://github.com/InterSIS/django-rest-serializer-field-permissions/
 Author: The Intersis Foundation
 Author-email: dev@intersis.org
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -179,15 +179,15 @@
 Compatibility
 -------------
 
 This package is tested for compatibility against the following software versions:
 
 * Django Rest Framework 3.14.0
 * Django 3.2, 4.2
-* Python 3.8
+* Python 3.7
 
 This package may incidentally be compatible with other similar versions of the above software. See tox.ini for specific minor versions tested.
 
 Additional Requirements
 -----------------------
 
 None
```

### Comparing `django-rest-serializer-field-permissions-4.1.0/django_rest_serializer_field_permissions.egg-info/SOURCES.txt` & `django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-rest-serializer-field-permissions-4.1.0/rest_framework_serializer_field_permissions/fields.py` & `django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/fields.py`

 * *Files identical despite different names*

### Comparing `django-rest-serializer-field-permissions-4.1.0/rest_framework_serializer_field_permissions/permissions.py` & `django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/permissions.py`

 * *Files identical despite different names*

### Comparing `django-rest-serializer-field-permissions-4.1.0/rest_framework_serializer_field_permissions/serializers.py` & `django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/serializers.py`

 * *Files identical despite different names*

### Comparing `django-rest-serializer-field-permissions-4.1.0/setup.py` & `django-rest-serializer-field-permissions-4.1.0rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-rest-serializer-field-permissions',
-    version='4.1.0',
+    version='4.1.0rc1',
     packages=['rest_framework_serializer_field_permissions'],
     include_package_data=True,
     license='GNU General Public License v3 (GPLv3)',
     description='Field-by-field serializer permissions for Django Rest Framework.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/InterSIS/django-rest-serializer-field-permissions/',
```

