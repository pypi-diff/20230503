# Comparing `tmp/dynamic_factory-0.1.6.tar.gz` & `tmp/dynamic_factory-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_factory-0.1.6.tar", max compression
+gzip compressed data, was "dynamic_factory-0.1.7.tar", max compression
```

## Comparing `dynamic_factory-0.1.6.tar` & `dynamic_factory-0.1.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4914 2023-05-03 10:36:06.044356 dynamic_factory-0.1.6/README.md
--rw-r--r--   0        0        0      376 2023-05-03 15:41:47.591147 dynamic_factory-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6256 2023-05-03 15:38:39.306899 dynamic_factory-0.1.6/src/dynamic_factory.py
--rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 dynamic_factory-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     4914 2023-05-03 10:36:06.044356 dynamic_factory-0.1.7/README.md
+-rw-r--r--   0        0        0      376 2023-05-03 15:44:45.767368 dynamic_factory-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6243 2023-05-03 15:44:10.755325 dynamic_factory-0.1.7/src/dynamic_factory.py
+-rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 dynamic_factory-0.1.7/PKG-INFO
```

### Comparing `dynamic_factory-0.1.6/README.md` & `dynamic_factory-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dynamic_factory-0.1.6/src/dynamic_factory.py` & `dynamic_factory-0.1.7/src/dynamic_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import inspect
 from typing import Iterable, Union, Callable
 from dataclasses import dataclass
 import warnings
 
-from src.config import DEFAULT_GROUP_NAME
-
 
 __all__ = ["FuncFactory"]
-
+DEFAULT_GROUP_NAME = "DEFAULT"
 
 class FuncFactory:
     """Dynamic implementation of factory design pattern,
      that is designed to work with functions.
     """
     _all_groups = set()
```

### Comparing `dynamic_factory-0.1.6/PKG-INFO` & `dynamic_factory-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-factory
-Version: 0.1.6
+Version: 0.1.7
 Summary: This module contain dynamic implementations of factory pattern
 License: Apache-2.0
 Author: Wojciech Bogobowicz
 Author-email: wojciech.bogobowicz@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

