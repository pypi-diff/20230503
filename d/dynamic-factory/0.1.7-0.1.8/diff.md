# Comparing `tmp/dynamic_factory-0.1.7.tar.gz` & `tmp/dynamic_factory-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_factory-0.1.7.tar", max compression
+gzip compressed data, was "dynamic_factory-0.1.8.tar", max compression
```

## Comparing `dynamic_factory-0.1.7.tar` & `dynamic_factory-0.1.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4914 2023-05-03 10:36:06.044356 dynamic_factory-0.1.7/README.md
--rw-r--r--   0        0        0      376 2023-05-03 15:44:45.767368 dynamic_factory-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6243 2023-05-03 15:44:10.755325 dynamic_factory-0.1.7/src/dynamic_factory.py
--rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 dynamic_factory-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     5062 2023-05-03 15:51:05.352888 dynamic_factory-0.1.8/README.md
+-rw-r--r--   0        0        0      376 2023-05-03 15:51:27.493042 dynamic_factory-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6243 2023-05-03 15:44:10.755325 dynamic_factory-0.1.8/src/dynamic_factory.py
+-rw-r--r--   0        0        0     5713 1970-01-01 00:00:00.000000 dynamic_factory-0.1.8/PKG-INFO
```

### Comparing `dynamic_factory-0.1.7/README.md` & `dynamic_factory-0.1.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 # Table of content
 - [Table of content](#table-of-content)
 - [Overview](#overview)
+- [Installation](#installation)
 - [Usage tutorial](#usage-tutorial)
     - [Setup](#setup)
     - [Quick start](#quick-start)
     - [Groups](#groups)
     - [Functions with arguments](#functions-with-arguments)
     - [Aliases](#aliases)
 - [Limitations](#limitations)
 - [ToDo](#todo)
 
 # Overview
 
 `dynamic_factory` is package for dynamic implementations of factory pattern. Currently it has implemented only one class. `FuncFactory` that is designed to work with functions.
 
+# Installation
+Via pip:
+```bash
+pip install dynamic-factory
+```
+Via poetry:
+```bash
+poetry add dynamic-factory
+```
+
 # Usage tutorial
 
 ### Setup
 
 Lets define two python files `./src1.py` and `./src2.py`
```

### Comparing `dynamic_factory-0.1.7/src/dynamic_factory.py` & `dynamic_factory-0.1.8/src/dynamic_factory.py`

 * *Files identical despite different names*

### Comparing `dynamic_factory-0.1.7/PKG-INFO` & `dynamic_factory-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-factory
-Version: 0.1.7
+Version: 0.1.8
 Summary: This module contain dynamic implementations of factory pattern
 License: Apache-2.0
 Author: Wojciech Bogobowicz
 Author-email: wojciech.bogobowicz@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -14,27 +14,38 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Table of content
 - [Table of content](#table-of-content)
 - [Overview](#overview)
+- [Installation](#installation)
 - [Usage tutorial](#usage-tutorial)
     - [Setup](#setup)
     - [Quick start](#quick-start)
     - [Groups](#groups)
     - [Functions with arguments](#functions-with-arguments)
     - [Aliases](#aliases)
 - [Limitations](#limitations)
 - [ToDo](#todo)
 
 # Overview
 
 `dynamic_factory` is package for dynamic implementations of factory pattern. Currently it has implemented only one class. `FuncFactory` that is designed to work with functions.
 
+# Installation
+Via pip:
+```bash
+pip install dynamic-factory
+```
+Via poetry:
+```bash
+poetry add dynamic-factory
+```
+
 # Usage tutorial
 
 ### Setup
 
 Lets define two python files `./src1.py` and `./src2.py`
```

