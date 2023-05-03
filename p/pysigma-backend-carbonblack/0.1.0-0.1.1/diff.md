# Comparing `tmp/pysigma_backend_carbonblack-0.1.0.tar.gz` & `tmp/pysigma_backend_carbonblack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_carbonblack-0.1.0.tar", max compression
+gzip compressed data, was "pysigma_backend_carbonblack-0.1.1.tar", max compression
```

## Comparing `pysigma_backend_carbonblack-0.1.0.tar` & `pysigma_backend_carbonblack-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-04-30 03:38:06.267942 pysigma_backend_carbonblack-0.1.0/LICENSE
--rw-r--r--   0        0        0      575 2023-04-30 03:38:06.267942 pysigma_backend_carbonblack-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      371 2023-04-30 03:38:06.267942 pysigma_backend_carbonblack-0.1.0/sigma/backends/carbonblack/__init__.py
--rw-r--r--   0        0        0     6881 2023-04-30 03:38:06.267942 pysigma_backend_carbonblack-0.1.0/sigma/backends/carbonblack/carbonblack.py
--rw-r--r--   0        0        0      315 2023-04-30 03:38:06.267942 pysigma_backend_carbonblack-0.1.0/sigma/pipelines/carbonblack/__init__.py
--rw-r--r--   0        0        0    13283 2023-04-30 03:38:06.267942 pysigma_backend_carbonblack-0.1.0/sigma/pipelines/carbonblack/carbonblack.py
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pysigma_backend_carbonblack-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-03 01:45:25.452676 pysigma_backend_carbonblack-0.1.1/LICENSE
+-rw-r--r--   0        0        0      575 2023-05-03 01:45:25.452676 pysigma_backend_carbonblack-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      371 2023-05-03 01:45:25.452676 pysigma_backend_carbonblack-0.1.1/sigma/backends/carbonblack/__init__.py
+-rw-r--r--   0        0        0     6881 2023-05-03 01:45:25.452676 pysigma_backend_carbonblack-0.1.1/sigma/backends/carbonblack/carbonblack.py
+-rw-r--r--   0        0        0      315 2023-05-03 01:45:25.452676 pysigma_backend_carbonblack-0.1.1/sigma/pipelines/carbonblack/__init__.py
+-rw-r--r--   0        0        0    13283 2023-05-03 01:45:25.452676 pysigma_backend_carbonblack-0.1.1/sigma/pipelines/carbonblack/carbonblack.py
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pysigma_backend_carbonblack-0.1.1/PKG-INFO
```

### Comparing `pysigma_backend_carbonblack-0.1.0/LICENSE` & `pysigma_backend_carbonblack-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_carbonblack-0.1.0/pyproject.toml` & `pysigma_backend_carbonblack-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-carbonblack"
-version = "0.1.0"
+version = "0.1.1"
 description = "pySigma carbonblack backend"
 authors = ["Cori Smith <cs2718281@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/7RedViolin/pySigma-backend-carbonblack"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_carbonblack-0.1.0/sigma/backends/carbonblack/carbonblack.py` & `pysigma_backend_carbonblack-0.1.1/sigma/backends/carbonblack/carbonblack.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_carbonblack-0.1.0/sigma/pipelines/carbonblack/carbonblack.py` & `pysigma_backend_carbonblack-0.1.1/sigma/pipelines/carbonblack/carbonblack.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_carbonblack-0.1.0/PKG-INFO` & `pysigma_backend_carbonblack-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-carbonblack
-Version: 0.1.0
+Version: 0.1.1
 Summary: pySigma carbonblack backend
 Home-page: https://github.com/7RedViolin/pySigma-backend-carbonblack
 License: MIT
 Author: Cori Smith
 Author-email: cs2718281@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

