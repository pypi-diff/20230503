# Comparing `tmp/dynamic_factory-0.1.3.tar.gz` & `tmp/dynamic_factory-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_factory-0.1.3.tar", max compression
+gzip compressed data, was "dynamic_factory-0.1.4.tar", max compression
```

## Comparing `dynamic_factory-0.1.3.tar` & `dynamic_factory-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4914 2023-05-03 10:36:06.044356 dynamic_factory-0.1.3/README.md
--rw-r--r--   0        0        0      377 2023-05-03 15:29:37.446046 dynamic_factory-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6253 2023-05-03 15:27:46.761827 dynamic_factory-0.1.3/src/dynamic_factory.py
--rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 dynamic_factory-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4914 2023-05-03 10:36:06.044356 dynamic_factory-0.1.4/README.md
+-rw-r--r--   0        0        0      377 2023-05-03 15:36:43.886738 dynamic_factory-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6252 2023-05-03 15:36:21.202706 dynamic_factory-0.1.4/src/dynamic_factory.py
+-rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 dynamic_factory-0.1.4/PKG-INFO
```

### Comparing `dynamic_factory-0.1.3/README.md` & `dynamic_factory-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dynamic_factory-0.1.3/src/dynamic_factory.py` & `dynamic_factory-0.1.4/src/dynamic_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 from typing import Iterable, Union, Callable
 from dataclasses import dataclass
 import warnings
 
-from .config import DEFAULT_GROUP_NAME
+from config import DEFAULT_GROUP_NAME
 
 
 __all__ = ["FuncFactory"]
 
 
 class FuncFactory:
     """Dynamic implementation of factory design pattern,
```

### Comparing `dynamic_factory-0.1.3/PKG-INFO` & `dynamic_factory-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-factory
-Version: 0.1.3
+Version: 0.1.4
 Summary: This module contain dynamic implementations of factory pattern
 License: Apache-2.0
 Author: Wojciech Bogobowicz
 Author-email: wojciech.bogobowicz@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

