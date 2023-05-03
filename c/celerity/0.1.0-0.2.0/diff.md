# Comparing `tmp/celerity-0.1.0.tar.gz` & `tmp/celerity-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celerity-0.1.0.tar", max compression
+gzip compressed data, was "celerity-0.2.0.tar", max compression
```

## Comparing `celerity-0.1.0.tar` & `celerity-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1075 2023-04-29 15:00:44.273148 celerity-0.1.0/LICENSE
--rw-r--r--   0        0        0     4232 2023-05-02 17:04:05.156274 celerity-0.1.0/README.md
--rw-r--r--   0        0        0     1646 2023-04-30 11:58:57.315923 celerity-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      133 2023-04-30 13:25:19.740826 celerity-0.1.0/src/celerity/__init__.py
--rw-r--r--   0        0        0      997 2023-05-01 15:47:56.463380 celerity-0.1.0/src/celerity/constants.py
--rw-r--r--   0        0        0     3771 2023-05-02 16:54:14.880153 celerity-0.1.0/src/celerity/temporal.py
--rw-r--r--   0        0        0     4630 1970-01-01 00:00:00.000000 celerity-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-03 13:48:11.342589 celerity-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4346 2023-05-03 13:48:11.342589 celerity-0.2.0/README.md
+-rw-r--r--   0        0        0     1830 2023-05-03 13:48:11.342589 celerity-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-05-03 13:48:11.342589 celerity-0.2.0/src/celerity/__init__.py
+-rw-r--r--   0        0        0      997 2023-05-03 13:48:11.342589 celerity-0.2.0/src/celerity/constants.py
+-rw-r--r--   0        0        0     3771 2023-05-03 13:48:11.342589 celerity-0.2.0/src/celerity/temporal.py
+-rw-r--r--   0        0        0      961 2023-05-03 13:48:11.342589 celerity-0.2.0/src/celerity/utilities.py
+-rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 celerity-0.2.0/PKG-INFO
```

### Comparing `celerity-0.1.0/LICENSE` & `celerity-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `celerity-0.1.0/README.md` & `celerity-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Celerity
 
 Celerity is a lightweight, research-grade, zero-dependency type-safe Python library for astronomical calculations to plan your observations. It's only dependency is the Python 3.11+ standard library.
 
 It has been designed to be independent of any other popular astronomical libraries, with a focus on providing a simple and intuitive API for performing common astronomical calculations.
 
+**N.B.** _This project is currently in the early stages of development and is not yet ready for production use._
+
 ---
 
 ## Usage
 
 ### Installation
 
 Celerity can be installed using `pip`:
```

### Comparing `celerity-0.1.0/pyproject.toml` & `celerity-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 [tool.poetry]
 name = "celerity"
-version = "0.1.0"
+version = "0.2.0"
 description = "Celerity is a lightweight, zero-dependency and type-safe Python library for astronomical calculations."
-authors = ["Michael J. Roberts <michael@observerly.com>"]
+authors = [
+    "Michael J. Roberts <michael@observerly.com>"
+]
+maintainers = [
+    "Michael J. Roberts <michael@observerly.com>"
+]
 readme = "README.md"
 packages = [{include = "celerity", from = "src"}]
+repository = "https://github.com/michaelroberts/celerity"
+keywords = ["astronomy", "astrometry", "ephemeris"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.263"
```

### Comparing `celerity-0.1.0/src/celerity/constants.py` & `celerity-0.2.0/src/celerity/constants.py`

 * *Files identical despite different names*

### Comparing `celerity-0.1.0/src/celerity/temporal.py` & `celerity-0.2.0/src/celerity/temporal.py`

 * *Files identical despite different names*

### Comparing `celerity-0.1.0/PKG-INFO` & `celerity-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: celerity
-Version: 0.1.0
+Version: 0.2.0
 Summary: Celerity is a lightweight, zero-dependency and type-safe Python library for astronomical calculations.
+Home-page: https://github.com/michaelroberts/celerity
+Keywords: astronomy,astrometry,ephemeris
 Author: Michael J. Roberts
 Author-email: michael@observerly.com
+Maintainer: Michael J. Roberts
+Maintainer-email: michael@observerly.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/michaelroberts/celerity
 Description-Content-Type: text/markdown
 
 # Celerity
 
 Celerity is a lightweight, research-grade, zero-dependency type-safe Python library for astronomical calculations to plan your observations. It's only dependency is the Python 3.11+ standard library.
 
 It has been designed to be independent of any other popular astronomical libraries, with a focus on providing a simple and intuitive API for performing common astronomical calculations.
 
+**N.B.** _This project is currently in the early stages of development and is not yet ready for production use._
+
 ---
 
 ## Usage
 
 ### Installation
 
 Celerity can be installed using `pip`:
```

