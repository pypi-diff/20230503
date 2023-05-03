# Comparing `tmp/pysigma_backend_carbonblack-0.1.1.tar.gz` & `tmp/pysigma_backend_carbonblack-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_carbonblack-0.1.1.tar", max compression
+gzip compressed data, was "pysigma_backend_carbonblack-0.1.2.tar", max compression
```

## Comparing `pysigma_backend_carbonblack-0.1.1.tar` & `pysigma_backend_carbonblack-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-03 01:45:25.452676 pysigma_backend_carbonblack-0.1.1/LICENSE
--rw-r--r--   0        0        0      575 2023-05-03 01:45:25.452676 pysigma_backend_carbonblack-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      371 2023-05-03 01:45:25.452676 pysigma_backend_carbonblack-0.1.1/sigma/backends/carbonblack/__init__.py
--rw-r--r--   0        0        0     6881 2023-05-03 01:45:25.452676 pysigma_backend_carbonblack-0.1.1/sigma/backends/carbonblack/carbonblack.py
--rw-r--r--   0        0        0      315 2023-05-03 01:45:25.452676 pysigma_backend_carbonblack-0.1.1/sigma/pipelines/carbonblack/__init__.py
--rw-r--r--   0        0        0    13283 2023-05-03 01:45:25.452676 pysigma_backend_carbonblack-0.1.1/sigma/pipelines/carbonblack/carbonblack.py
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pysigma_backend_carbonblack-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-03 02:12:08.905275 pysigma_backend_carbonblack-0.1.2/LICENSE
+-rw-r--r--   0        0        0      575 2023-05-03 02:12:08.905275 pysigma_backend_carbonblack-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      371 2023-05-03 02:12:08.905275 pysigma_backend_carbonblack-0.1.2/sigma/backends/carbonblack/__init__.py
+-rw-r--r--   0        0        0     6915 2023-05-03 02:12:08.905275 pysigma_backend_carbonblack-0.1.2/sigma/backends/carbonblack/carbonblack.py
+-rw-r--r--   0        0        0      315 2023-05-03 02:12:08.905275 pysigma_backend_carbonblack-0.1.2/sigma/pipelines/carbonblack/__init__.py
+-rw-r--r--   0        0        0    13283 2023-05-03 02:12:08.905275 pysigma_backend_carbonblack-0.1.2/sigma/pipelines/carbonblack/carbonblack.py
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pysigma_backend_carbonblack-0.1.2/PKG-INFO
```

### Comparing `pysigma_backend_carbonblack-0.1.1/LICENSE` & `pysigma_backend_carbonblack-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_carbonblack-0.1.1/pyproject.toml` & `pysigma_backend_carbonblack-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-carbonblack"
-version = "0.1.1"
+version = "0.1.2"
 description = "pySigma carbonblack backend"
 authors = ["Cori Smith <cs2718281@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/7RedViolin/pySigma-backend-carbonblack"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_carbonblack-0.1.1/sigma/backends/carbonblack/carbonblack.py` & `pysigma_backend_carbonblack-0.1.2/sigma/backends/carbonblack/carbonblack.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from typing import ClassVar, Dict, Tuple, Pattern, List, Any, Union
 
 class CarbonBlackBackend(TextQueryBackend):
     """CarbonBlack backend."""
 
     name : ClassVar[str] = "CarbonBlack backend"
     formats : Dict[str, str] = {
-        "default": "Plain CarbonBlack queries",        
+        "default": "Plain CarbonBlack queries",
+        "json": "CarbonBlack JSON query",
     }
 
     requires_pipeline : bool = False
 
     precedence : ClassVar[Tuple[ConditionItem, ConditionItem, ConditionItem]] = (ConditionNOT, ConditionAND, ConditionOR)
     group_expression : ClassVar[str] = "({expr})"   # Expression for precedence override grouping as format string with {expr} placeholder
     parenthesize : bool = True
```

### Comparing `pysigma_backend_carbonblack-0.1.1/sigma/pipelines/carbonblack/carbonblack.py` & `pysigma_backend_carbonblack-0.1.2/sigma/pipelines/carbonblack/carbonblack.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_carbonblack-0.1.1/PKG-INFO` & `pysigma_backend_carbonblack-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-carbonblack
-Version: 0.1.1
+Version: 0.1.2
 Summary: pySigma carbonblack backend
 Home-page: https://github.com/7RedViolin/pySigma-backend-carbonblack
 License: MIT
 Author: Cori Smith
 Author-email: cs2718281@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

