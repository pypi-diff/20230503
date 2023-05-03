# Comparing `tmp/dynamic_factory-0.1.0.tar.gz` & `tmp/dynamic_factory-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_factory-0.1.0.tar", max compression
+gzip compressed data, was "dynamic_factory-0.1.1.tar", max compression
```

## Comparing `dynamic_factory-0.1.0.tar` & `dynamic_factory-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4914 2023-05-03 10:36:06.044356 dynamic_factory-0.1.0/README.md
--rw-r--r--   0        0        0      398 2023-05-03 10:32:31.881574 dynamic_factory-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6252 2023-05-03 10:21:22.205408 dynamic_factory-0.1.0/src/dynamic_factory.py
--rw-r--r--   0        0        0     5596 1970-01-01 00:00:00.000000 dynamic_factory-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4914 2023-05-03 10:36:06.044356 dynamic_factory-0.1.1/README.md
+-rw-r--r--   0        0        0      377 2023-05-03 15:10:34.854906 dynamic_factory-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6252 2023-05-03 10:21:22.205408 dynamic_factory-0.1.1/src/dynamic_factory.py
+-rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 dynamic_factory-0.1.1/PKG-INFO
```

### Comparing `dynamic_factory-0.1.0/README.md` & `dynamic_factory-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dynamic_factory-0.1.0/src/dynamic_factory.py` & `dynamic_factory-0.1.1/src/dynamic_factory.py`

 * *Files identical despite different names*

### Comparing `dynamic_factory-0.1.0/PKG-INFO` & `dynamic_factory-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: dynamic-factory
-Version: 0.1.0
+Version: 0.1.1
 Summary: This module contain dynamic implementations of factory pattern
 License: Apache-2.0
 Author: Wojciech Bogobowicz
 Author-email: wojciech.bogobowicz@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dynamic_factory
 Description-Content-Type: text/markdown
 
 # Table of content
 - [Table of content](#table-of-content)
 - [Overview](#overview)
 - [Usage tutorial](#usage-tutorial)
     - [Setup](#setup)
```

