# Comparing `tmp/little_conf-0.0.3.tar.gz` & `tmp/little_conf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "little_conf-0.0.3.tar", max compression
+gzip compressed data, was "little_conf-0.0.4.tar", max compression
```

## Comparing `little_conf-0.0.3.tar` & `little_conf-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0       29 2022-12-27 09:37:40.708933 little_conf-0.0.3/little_conf/__init__.py
--rw-r--r--   0        0        0     3194 2022-12-27 10:04:56.229547 little_conf-0.0.3/little_conf/lc.py
--rw-r--r--   0        0        0      556 2022-12-27 12:19:37.513722 little_conf-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 little_conf-0.0.3/setup.py
--rw-r--r--   0        0        0      722 1970-01-01 00:00:00.000000 little_conf-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       29 2022-12-27 09:37:40.708933 little_conf-0.0.4/little_conf/__init__.py
+-rw-r--r--   0        0        0     3194 2022-12-27 10:04:56.229547 little_conf-0.0.4/little_conf/lc.py
+-rw-r--r--   0        0        0       99 2023-05-03 07:12:29.351686 little_conf-0.0.4/little_conf/template_settings/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-03 07:12:29.351686 little_conf-0.0.4/little_conf/template_settings/base.py
+-rw-r--r--   0        0        0      927 2023-05-03 07:12:29.351686 little_conf-0.0.4/little_conf/template_settings/database.py
+-rw-r--r--   0        0        0     1614 2023-05-03 07:12:29.355686 little_conf-0.0.4/little_conf/template_settings/redis.py
+-rw-r--r--   0        0        0      394 2023-05-03 07:12:29.355686 little_conf-0.0.4/little_conf/template_settings/s3.py
+-rw-r--r--   0        0        0      556 2023-05-03 07:25:21.139603 little_conf-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 little_conf-0.0.4/setup.py
+-rw-r--r--   0        0        0      722 1970-01-01 00:00:00.000000 little_conf-0.0.4/PKG-INFO
```

### Comparing `little_conf-0.0.3/little_conf/lc.py` & `little_conf-0.0.4/little_conf/lc.py`

 * *Files identical despite different names*

### Comparing `little_conf-0.0.3/pyproject.toml` & `little_conf-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "little-conf"
-version = "0.0.3"  # update automatically by CI
+version = "0.0.4"  # update automatically by CI
 description = "Simple library for service configuration"
 authors = ["smartleks"]
 repository = "https://github.com/smartleks/little-conf"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pyyaml = ">5.0.0"
```

### Comparing `little_conf-0.0.3/setup.py` & `little_conf-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['little_conf']
+['little_conf', 'little_conf.template_settings']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['deepmerge>=1.1.0,<2.0.0',
  'pydantic>=1.8.0,<2.0.0',
  'pytest>=6.2.4,<7.0.0',
  'pyyaml>5.0.0']
 
 setup_kwargs = {
     'name': 'little-conf',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Simple library for service configuration',
     'long_description': 'None',
     'author': 'smartleks',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/smartleks/little-conf',
```

### Comparing `little_conf-0.0.3/PKG-INFO` & `little_conf-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: little-conf
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple library for service configuration
 Home-page: https://github.com/smartleks/little-conf
 Author: smartleks
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

