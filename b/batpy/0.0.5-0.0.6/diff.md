# Comparing `tmp/batpy-0.0.5.tar.gz` & `tmp/batpy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batpy-0.0.5.tar", max compression
+gzip compressed data, was "batpy-0.0.6.tar", max compression
```

## Comparing `batpy-0.0.5.tar` & `batpy-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1073 2023-05-03 15:32:02.682992 batpy-0.0.5/LICENSE
--rw-r--r--   0        0        0     3840 2023-05-03 15:32:02.682992 batpy-0.0.5/README.md
--rw-r--r--   0        0        0     1825 2023-05-03 15:32:37.207071 batpy-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      172 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/__init__.py
--rw-r--r--   0        0        0     5157 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/batpac_battery.py
--rw-r--r--   0        0        0    27747 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/batpac_tool.py
--rw-r--r--   0        0        0     2158 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/data/batpy_batpac_calculation_and_validation_results.toml
--rw-r--r--   0        0        0    30586 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/data/batpy_batpac_config.toml
--rw-r--r--   0        0        0    83193 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/data/batpy_batpac_user_input_cells.toml
--rw-r--r--   0        0        0    48369 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/data/batpy_batteries_config.toml
--rw-r--r--   0        0        0     2177 2023-05-03 15:32:02.686992 batpy-0.0.5/src/batpy/is_version_compatible.py
--rw-r--r--   0        0        0     4795 1970-01-01 00:00:00.000000 batpy-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-05-03 15:48:08.040242 batpy-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4365 2023-05-03 15:48:08.044242 batpy-0.0.6/README.md
+-rw-r--r--   0        0        0     1825 2023-05-03 15:48:41.992636 batpy-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-05-03 15:48:08.044242 batpy-0.0.6/src/batpy/__init__.py
+-rw-r--r--   0        0        0     5157 2023-05-03 15:48:08.044242 batpy-0.0.6/src/batpy/batpac_battery.py
+-rw-r--r--   0        0        0    27747 2023-05-03 15:48:08.044242 batpy-0.0.6/src/batpy/batpac_tool.py
+-rw-r--r--   0        0        0     2158 2023-05-03 15:48:08.044242 batpy-0.0.6/src/batpy/data/batpy_batpac_calculation_and_validation_results.toml
+-rw-r--r--   0        0        0    30586 2023-05-03 15:48:08.044242 batpy-0.0.6/src/batpy/data/batpy_batpac_config.toml
+-rw-r--r--   0        0        0    83193 2023-05-03 15:48:08.044242 batpy-0.0.6/src/batpy/data/batpy_batpac_user_input_cells.toml
+-rw-r--r--   0        0        0    48369 2023-05-03 15:48:08.044242 batpy-0.0.6/src/batpy/data/batpy_batteries_config.toml
+-rw-r--r--   0        0        0     2177 2023-05-03 15:48:08.044242 batpy-0.0.6/src/batpy/is_version_compatible.py
+-rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 batpy-0.0.6/PKG-INFO
```

### Comparing `batpy-0.0.5/LICENSE` & `batpy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `batpy-0.0.5/README.md` & `batpy-0.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 [![ci-cd](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml)
-[![PyPI version](https://badge.fury.io/py/batpy.svg)](https://badge.fury.io/py/batpy)
-
+[![Docs](https://github.com/rginster/batpy/actions/workflows/documentation.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/documentation.yaml)
+[![pages-build-deployment](https://github.com/rginster/batpy/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/rginster/batpy/actions/workflows/pages/pages-build-deployment)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/batpy)
+[![PyPi](https://img.shields.io/pypi/v/batpy.svg)](https://pypi.python.org/pypi/batpy)
+[![PyPi](https://img.shields.io/pypi/dm/batpy.svg)](https://pypi.python.org/pypi/batpy)
 
 # batpy
 
 `batpy` is a Python wrapper for [Argonne National Laboratory's](https://www.anl.gov) Microsoft Excel-based [software modeling tool BatPaC](https://www.anl.gov/partnerships/batpac-battery-manufacturing-cost-estimation).
 
 ## Installation
```

### Comparing `batpy-0.0.5/pyproject.toml` & `batpy-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "batpy"
-version = "0.0.5"
+version = "0.0.6"
 description = "A python package to read, write, and calculate batteries in the BatPaC tool."
 authors = ["Raphael Ginster <r.ginster@tu-braunschweig.de>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://rginster.github.io/batpy/"
 repository = "https://github.com/rginster/batpy"
```

### Comparing `batpy-0.0.5/src/batpy/batpac_battery.py` & `batpy-0.0.6/src/batpy/batpac_battery.py`

 * *Files identical despite different names*

### Comparing `batpy-0.0.5/src/batpy/batpac_tool.py` & `batpy-0.0.6/src/batpy/batpac_tool.py`

 * *Files identical despite different names*

### Comparing `batpy-0.0.5/src/batpy/data/batpy_batpac_calculation_and_validation_results.toml` & `batpy-0.0.6/src/batpy/data/batpy_batpac_calculation_and_validation_results.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.0.5/src/batpy/data/batpy_batpac_config.toml` & `batpy-0.0.6/src/batpy/data/batpy_batpac_config.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.0.5/src/batpy/data/batpy_batpac_user_input_cells.toml` & `batpy-0.0.6/src/batpy/data/batpy_batpac_user_input_cells.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.0.5/src/batpy/data/batpy_batteries_config.toml` & `batpy-0.0.6/src/batpy/data/batpy_batteries_config.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.0.5/src/batpy/is_version_compatible.py` & `batpy-0.0.6/src/batpy/is_version_compatible.py`

 * *Files identical despite different names*

### Comparing `batpy-0.0.5/PKG-INFO` & `batpy-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batpy
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package to read, write, and calculate batteries in the BatPaC tool.
 Home-page: https://github.com/rginster/batpy
 License: MIT
 Author: Raphael Ginster
 Author-email: r.ginster@tu-braunschweig.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -19,16 +19,19 @@
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: xlwings (>=0.30.4,<0.31.0)
 Project-URL: Documentation, https://rginster.github.io/batpy/
 Project-URL: Repository, https://github.com/rginster/batpy
 Description-Content-Type: text/markdown
 
 [![ci-cd](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/ci-cd.yaml)
-[![PyPI version](https://badge.fury.io/py/batpy.svg)](https://badge.fury.io/py/batpy)
-
+[![Docs](https://github.com/rginster/batpy/actions/workflows/documentation.yaml/badge.svg)](https://github.com/rginster/batpy/actions/workflows/documentation.yaml)
+[![pages-build-deployment](https://github.com/rginster/batpy/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/rginster/batpy/actions/workflows/pages/pages-build-deployment)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/batpy)
+[![PyPi](https://img.shields.io/pypi/v/batpy.svg)](https://pypi.python.org/pypi/batpy)
+[![PyPi](https://img.shields.io/pypi/dm/batpy.svg)](https://pypi.python.org/pypi/batpy)
 
 # batpy
 
 `batpy` is a Python wrapper for [Argonne National Laboratory's](https://www.anl.gov) Microsoft Excel-based [software modeling tool BatPaC](https://www.anl.gov/partnerships/batpac-battery-manufacturing-cost-estimation).
 
 ## Installation
```

