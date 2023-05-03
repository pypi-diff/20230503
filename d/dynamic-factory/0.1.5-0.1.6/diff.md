# Comparing `tmp/dynamic_factory-0.1.5.tar.gz` & `tmp/dynamic_factory-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_factory-0.1.5.tar", max compression
+gzip compressed data, was "dynamic_factory-0.1.6.tar", max compression
```

## Comparing `dynamic_factory-0.1.5.tar` & `dynamic_factory-0.1.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4914 2023-05-03 10:36:06.044356 dynamic_factory-0.1.5/README.md
--rw-r--r--   0        0        0      376 2023-05-03 15:38:20.826874 dynamic_factory-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6256 2023-05-03 15:38:39.306899 dynamic_factory-0.1.5/src/dynamic_factory.py
--rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 dynamic_factory-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4914 2023-05-03 10:36:06.044356 dynamic_factory-0.1.6/README.md
+-rw-r--r--   0        0        0      376 2023-05-03 15:41:47.591147 dynamic_factory-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6256 2023-05-03 15:38:39.306899 dynamic_factory-0.1.6/src/dynamic_factory.py
+-rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 dynamic_factory-0.1.6/PKG-INFO
```

### Comparing `dynamic_factory-0.1.5/README.md` & `dynamic_factory-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dynamic_factory-0.1.5/src/dynamic_factory.py` & `dynamic_factory-0.1.6/src/dynamic_factory.py`

 * *Files identical despite different names*

### Comparing `dynamic_factory-0.1.5/PKG-INFO` & `dynamic_factory-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-factory
-Version: 0.1.5
+Version: 0.1.6
 Summary: This module contain dynamic implementations of factory pattern
 License: Apache-2.0
 Author: Wojciech Bogobowicz
 Author-email: wojciech.bogobowicz@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

