# Comparing `tmp/django-admin-easy-0.6.1.tar.gz` & `tmp/django-admin-easy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-admin-easy-0.6.1.tar", last modified: Sun Apr 25 00:05:27 2021, max compression
+gzip compressed data, was "django-admin-easy-0.7.0.tar", last modified: Wed May  3 20:21:52 2023, max compression
```

## Comparing `django-admin-easy-0.6.1.tar` & `django-admin-easy-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2021-04-25 00:05:27.000000 django-admin-easy-0.6.1/
-drwxrwxrwx   0        0        0        0 2021-04-25 00:05:27.000000 django-admin-easy-0.6.1/django_admin_easy.egg-info/
--rw-rw-rw-   0        0        0        1 2021-04-25 00:05:26.000000 django-admin-easy-0.6.1/django_admin_easy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2018-01-21 19:09:28.000000 django-admin-easy-0.6.1/django_admin_easy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0    19338 2021-04-25 00:05:26.000000 django-admin-easy-0.6.1/django_admin_easy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        7 2021-04-25 00:05:26.000000 django-admin-easy-0.6.1/django_admin_easy.egg-info/requires.txt
--rw-rw-rw-   0        0        0      528 2021-04-25 00:05:27.000000 django-admin-easy-0.6.1/django_admin_easy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       14 2021-04-25 00:05:26.000000 django-admin-easy-0.6.1/django_admin_easy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-04-25 00:05:27.000000 django-admin-easy-0.6.1/easy/
-drwxrwxrwx   0        0        0        0 2021-04-25 00:05:27.000000 django-admin-easy-0.6.1/easy/admin/
--rw-rw-rw-   0        0        0     3909 2019-05-15 18:52:10.000000 django-admin-easy-0.6.1/easy/admin/decorators.py
--rw-rw-rw-   0        0        0     8559 2020-02-05 20:04:52.000000 django-admin-easy-0.6.1/easy/admin/field.py
--rw-rw-rw-   0        0        0     1605 2018-09-15 21:55:52.000000 django-admin-easy-0.6.1/easy/admin/mixin.py
--rw-rw-rw-   0        0        0        0 2018-09-15 21:58:38.000000 django-admin-easy-0.6.1/easy/admin/__init__.py
--rw-rw-rw-   0        0        0     2615 2018-09-15 21:56:56.000000 django-admin-easy-0.6.1/easy/helper.py
--rw-rw-rw-   0        0        0        0 2018-09-15 21:56:57.000000 django-admin-easy-0.6.1/easy/models.py
--rw-rw-rw-   0        0        0      395 2018-09-15 21:57:56.000000 django-admin-easy-0.6.1/easy/six.py
--rw-rw-rw-   0        0        0    16200 2021-04-24 23:52:30.000000 django-admin-easy-0.6.1/easy/tests.py
--rw-rw-rw-   0        0        0      407 2018-01-21 19:00:45.000000 django-admin-easy-0.6.1/easy/util.py
--rw-rw-rw-   0        0        0      521 2020-02-05 20:04:52.000000 django-admin-easy-0.6.1/easy/__init__.py
--rw-rw-rw-   0        0        0     1072 2018-01-21 19:00:45.000000 django-admin-easy-0.6.1/LICENSE.md
--rw-rw-rw-   0        0        0       18 2018-01-21 19:00:45.000000 django-admin-easy-0.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0    19338 2021-04-25 00:05:27.000000 django-admin-easy-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0    14173 2021-04-24 23:58:55.000000 django-admin-easy-0.6.1/README.rst
--rw-rw-rw-   0        0        0       42 2021-04-25 00:05:27.000000 django-admin-easy-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1364 2021-04-24 23:58:55.000000 django-admin-easy-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-04-25 00:05:27.000000 django-admin-easy-0.6.1/test_app/
-drwxrwxrwx   0        0        0        0 2021-04-25 00:05:27.000000 django-admin-easy-0.6.1/test_app/migrations/
--rw-rw-rw-   0        0        0     1690 2018-09-15 21:24:08.000000 django-admin-easy-0.6.1/test_app/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2018-09-15 21:23:53.000000 django-admin-easy-0.6.1/test_app/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:21:52.773424 django-admin-easy-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-05-03 20:21:52.773424 django-admin-easy-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14575 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:21:52.769424 django-admin-easy-0.7.0/django_admin_easy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-05-03 20:21:52.000000 django-admin-easy-0.7.0/django_admin_easy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-03 20:21:52.000000 django-admin-easy-0.7.0/django_admin_easy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:21:52.000000 django-admin-easy-0.7.0/django_admin_easy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:21:52.000000 django-admin-easy-0.7.0/django_admin_easy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 20:21:52.000000 django-admin-easy-0.7.0/django_admin_easy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 20:21:52.000000 django-admin-easy-0.7.0/django_admin_easy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:21:52.773424 django-admin-easy-0.7.0/easy/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/easy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:21:52.773424 django-admin-easy-0.7.0/easy/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/easy/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/easy/admin/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/easy/admin/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/easy/admin/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/easy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/easy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/easy/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/easy/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/easy/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:21:52.773424 django-admin-easy-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:21:52.769424 django-admin-easy-0.7.0/test_app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:21:52.773424 django-admin-easy-0.7.0/test_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/test_app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:21:40.000000 django-admin-easy-0.7.0/test_app/migrations/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-admin-easy-0.6.1/django_admin_easy.egg-info/SOURCES.txt` & `django-admin-easy-0.7.0/django_admin_easy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-easy-0.6.1/easy/admin/decorators.py` & `django-admin-easy-0.7.0/easy/admin/decorators.py`

 * *Files identical despite different names*

### Comparing `django-admin-easy-0.6.1/easy/admin/field.py` & `django-admin-easy-0.7.0/easy/admin/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from _weakref import ref
-
 from django.contrib.admin.templatetags.admin_urls import admin_urlname
 from django.db.models import Model, ImageField as ModelImageField, ForeignKey
 from django.conf import settings
 from django.utils.html import conditional_escape
 from django.template.loader import render_to_string
 from django.utils.safestring import mark_safe
```

### Comparing `django-admin-easy-0.6.1/easy/admin/mixin.py` & `django-admin-easy-0.7.0/easy/admin/mixin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from django.conf.urls import url
 from django.contrib import messages
 from django.http.response import HttpResponseRedirect
 
 from easy.helper import get_model_name
-from easy.six import reverse
+from easy.six import reverse, url
 
 
 class MixinEasyViews(object):
 
     def _get_info(self):
         return self.model._meta.app_label, get_model_name(self.model)
```

### Comparing `django-admin-easy-0.6.1/easy/helper.py` & `django-admin-easy-0.7.0/easy/helper.py`

 * *Files identical despite different names*

### Comparing `django-admin-easy-0.6.1/easy/tests.py` & `django-admin-easy-0.7.0/easy/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,17 +286,15 @@
     def test_decorators(self):
 
         @easy.utils('html.escape')
         @easy.utils('html.conditional_escape')
         @easy.utils('html.strip_tags')
         @easy.utils('text.slugify')
         @easy.utils('translation.gettext')
-        @easy.utils('translation.ugettext')
         @easy.utils('translation.gettext_noop')
-        @easy.utils('translation.ugettext_noop')
         def field(self, obj):
             return obj
 
         self.assertEquals(field(object(), 'asd'), 'asd')
 
     def test_function_not_exist(self):
```

### Comparing `django-admin-easy-0.6.1/easy/__init__.py` & `django-admin-easy-0.7.0/easy/__init__.py`

 * *Files identical despite different names*

### Comparing `django-admin-easy-0.6.1/LICENSE.md` & `django-admin-easy-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-admin-easy-0.6.1/README.rst` & `django-admin-easy-0.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 django-admin-easy
 =================
 
 Collection of admin fields, decorators and mixin to help to create computed or custom fields more friendly and easy way
 
 
-.. image:: https://img.shields.io/badge/django-1.8%201.9%201.10%201.11%202.0%202.1%202.2%203.0%203.1%203.2-brightgreen.svg
+.. image:: https://img.shields.io/badge/django-1.8%201.9%201.10%201.11-brightgreen.svg
+  :target: http://pypi.python.org/pypi/django-admin-easy
+
+.. image:: https://img.shields.io/badge/django-2.0%202.1%202.2-brightgreen.svg
+  :target: http://pypi.python.org/pypi/django-admin-easy
+
+.. image:: https://img.shields.io/badge/django-3.0%203.1%203.2%204.0%204.1%204.2-brightgreen.svg
+  :target: http://pypi.python.org/pypi/django-admin-easy
+
+.. image:: https://img.shields.io/badge/django-4.0%204.1%204.2-brightgreen.svg
   :target: http://pypi.python.org/pypi/django-admin-easy
 
 .. image:: https://img.shields.io/pypi/v/django-admin-easy.svg?style=flat
   :target: http://pypi.python.org/pypi/django-admin-easy
 
 .. image:: https://img.shields.io/pypi/pyversions/django-admin-easy.svg?maxAge=2592000
   :target: http://pypi.python.org/pypi/django-admin-easy
 
 .. image:: https://img.shields.io/pypi/format/django-admin-easy.svg?maxAge=2592000
   :target: http://pypi.python.org/pypi/django-admin-easy
 
 .. image:: https://img.shields.io/pypi/status/django-admin-easy.svg?maxAge=2592000
   :target: http://pypi.python.org/pypi/django-admin-easy
 
-.. image:: https://img.shields.io/travis/ebertti/django-admin-easy/master.svg?maxAge=2592000
-  :target: https://travis-ci.org/ebertti/django-admin-easy
-
-.. image:: https://img.shields.io/requires/github/ebertti/django-admin-easy.svg?maxAge=2592000
-  :target: https://requires.io/github/ebertti/django-admin-easy/requirements/
+.. image:: https://github.com/ebertti/django-admin-easy/actions/workflows/test.yml/badge.svg
+  :target: https://github.com/ebertti/django-admin-easy/actions/workflows/test.yml
 
 .. image:: https://img.shields.io/coveralls/ebertti/django-admin-easy/master.svg?maxAge=2592000
   :target: https://coveralls.io/r/ebertti/django-admin-easy?branch=master
 
 
 Installation
 ------------
 
 1. Requirements: **Django > 1.8** and **Python > 3.5**
 
-2. ``pip install django-admin-easy==0.6.1``
+2. ``pip install django-admin-easy==0.7.0``
 
 
 * For **Django < 1.8** or **Python 2.x**
 
   ``pip install django-admin-easy==0.4.1``
 
 
@@ -409,50 +415,58 @@
 
 Authors
 -------
 The django-admin-easy was originally created by Ezequiel Bertti `@ebertti <https://github.com/ebertti>`_ October 2014.
 
 Changelog
 ---------
+* 0.7.0
+
+   Add support for Django 4.0, 4.1 and 4.2
+   Add support for Python 3.10 and 3.11
+   Add Github Actions for testing
+   Add job to realease on pypi
+   Thanks @Lex98
+
 * 0.6.1
 
-   * Add Support do Django 3.2 and Python 3.9
+   Add support for Django 3.2 and Python 3.9
 
 * 0.6
 
-   * Add RawIdAdminField
+   Add RawIdAdminField
 
 * 0.5.1
 
-   * Add permission on action decorator
+   Add permission on action decorator
 
 * 0.4.1
 
-  * Django 2.0
+   Django 2.0
 
 * 0.4
 
-  * Django 1.11
-  * Create module utils with action_response
+   Django 1.11
+   Create module utils with action_response
 
 * 0.3.2
 
-  * Add params_static to LinkChangeListAdminField
+   Add params_static to LinkChangeListAdminField
 
 * 0.3.1
 
-  * Add FormatAdminField
+   Add FormatAdminField
 
 * 0.3
 
-  * Add import from `__future__` on all files
-  * Django 1.10
-  * More decorators
-  * More admin fields
+   Add import from `__future__` on all files
+   Django 1.10
+   More decorators
+   More admin fields
 
 * 0.2.2
 
-  * Add MixinEasyViews
+   Add MixinEasyViews
 
 * 0.2.1
 
-  * Fix for Django 1.7 from `@kevgathuku <https://github.com/kevgathuku>`_
+   Fix for Django 1.7 from `@kevgathuku <https://github.com/kevgathuku>`_
```

### Comparing `django-admin-easy-0.6.1/setup.py` & `django-admin-easy-0.7.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(
     name='django-admin-easy',
-    version='0.6.1',
+    version='0.7.0',
     url='http://github.com/ebertti/django-admin-easy/',
     author='Ezequiel Bertti',
     author_email='ebertti@gmail.com',
     install_requires=['django',],
     packages=find_packages(exclude=('test_app', 'test_project')),
     include_package_data=True,
     license='MIT License',
@@ -26,10 +26,12 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     zip_safe=False,
 )
```

