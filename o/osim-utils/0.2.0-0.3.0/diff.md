# Comparing `tmp/osim_utils-0.2.0.tar.gz` & `tmp/osim_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osim_utils-0.2.0.tar", max compression
+gzip compressed data, was "osim_utils-0.3.0.tar", max compression
```

## Comparing `osim_utils-0.2.0.tar` & `osim_utils-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0      232 2023-03-29 13:31:01.256966 osim_utils-0.2.0/README.md
--rw-r--r--   0        0        0     6886 2023-03-29 13:24:23.094734 osim_utils-0.2.0/osim_utils/clients/epmc.py
--rw-r--r--   0        0        0      665 2023-03-29 13:18:29.418093 osim_utils-0.2.0/osim_utils/exceptions.py
--rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.2.0/osim_utils/logger.py
--rw-r--r--   0        0        0      408 2023-03-29 13:26:26.409977 osim_utils-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 osim_utils-0.2.0/setup.py
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 osim_utils-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-05-03 10:56:19.733098 osim_utils-0.3.0/README.md
+-rw-r--r--   0        0        0     6886 2023-05-03 10:56:19.733447 osim_utils-0.3.0/osim_utils/clients/epmc.py
+-rw-r--r--   0        0        0     3034 2023-05-03 13:04:39.071296 osim_utils-0.3.0/osim_utils/clients/openalex.py
+-rw-r--r--   0        0        0      271 2023-05-03 13:04:39.071567 osim_utils-0.3.0/osim_utils/common.py
+-rw-r--r--   0        0        0      311 2023-05-03 13:04:39.071765 osim_utils-0.3.0/osim_utils/constants.py
+-rw-r--r--   0        0        0     1515 2023-05-03 13:04:39.071924 osim_utils-0.3.0/osim_utils/decorators.py
+-rw-r--r--   0        0        0      665 2023-05-03 10:56:19.733679 osim_utils-0.3.0/osim_utils/exceptions.py
+-rw-r--r--   0        0        0     2532 2023-01-12 14:22:33.188019 osim_utils-0.3.0/osim_utils/logger.py
+-rw-r--r--   0        0        0      408 2023-05-03 14:43:36.318178 osim_utils-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 osim_utils-0.3.0/setup.py
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 osim_utils-0.3.0/PKG-INFO
```

### Comparing `osim_utils-0.2.0/osim_utils/clients/epmc.py` & `osim_utils-0.3.0/osim_utils/clients/epmc.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.2.0/osim_utils/exceptions.py` & `osim_utils-0.3.0/osim_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.2.0/osim_utils/logger.py` & `osim_utils-0.3.0/osim_utils/logger.py`

 * *Files identical despite different names*

### Comparing `osim_utils-0.2.0/setup.py` & `osim_utils-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['python-json-logger>=2.0.4,<3.0.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'osim-utils',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': '',
     'long_description': '# osim-utils\n\nThis package contains resources that are useful to more than one OSIM project. It includes, for\nexample, API clients to common literature resources, such as Europe PMC.\n\n## Installation\n\n```\npip install osim-utils\n```\n',
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `osim_utils-0.2.0/PKG-INFO` & `osim_utils-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osim-utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

