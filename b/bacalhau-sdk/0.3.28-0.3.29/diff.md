# Comparing `tmp/bacalhau_sdk-0.3.28.tar.gz` & `tmp/bacalhau_sdk-0.3.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacalhau_sdk-0.3.28.tar", max compression
+gzip compressed data, was "bacalhau_sdk-0.3.29.tar", max compression
```

## Comparing `bacalhau_sdk-0.3.28.tar` & `bacalhau_sdk-0.3.29.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10247 2023-04-14 23:57:21.305805 bacalhau_sdk-0.3.28/LICENSE
--rw-r--r--   0        0        0     7459 2023-04-14 23:57:21.305805 bacalhau_sdk-0.3.28/README.md
--rw-r--r--   0        0        0      133 2023-04-14 23:57:21.305805 bacalhau_sdk-0.3.28/bacalhau_sdk/__init__.py
--rw-r--r--   0        0        0     3020 2023-04-14 23:57:21.305805 bacalhau_sdk-0.3.28/bacalhau_sdk/api.py
--rw-r--r--   0        0        0     5375 2023-04-14 23:57:21.305805 bacalhau_sdk-0.3.28/bacalhau_sdk/config.py
--rw-r--r--   0        0        0     2745 2023-04-14 23:57:46.123435 bacalhau_sdk-0.3.28/pyproject.toml
--rw-r--r--   0        0        0       42 2023-04-14 23:57:21.305805 bacalhau_sdk-0.3.28/tests/__init__.py
--rw-r--r--   0        0        0     6721 2023-04-14 23:57:21.305805 bacalhau_sdk-0.3.28/tests/test_config.py
--rw-r--r--   0        0        0     9315 1970-01-01 00:00:00.000000 bacalhau_sdk-0.3.28/PKG-INFO
+-rw-r--r--   0        0        0    10247 2023-05-03 01:57:47.303356 bacalhau_sdk-0.3.29/LICENSE
+-rw-r--r--   0        0        0     7459 2023-05-03 01:57:47.303356 bacalhau_sdk-0.3.29/README.md
+-rw-r--r--   0        0        0      133 2023-05-03 01:57:47.303356 bacalhau_sdk-0.3.29/bacalhau_sdk/__init__.py
+-rw-r--r--   0        0        0     3020 2023-05-03 01:57:47.303356 bacalhau_sdk-0.3.29/bacalhau_sdk/api.py
+-rw-r--r--   0        0        0     5375 2023-05-03 01:57:47.303356 bacalhau_sdk-0.3.29/bacalhau_sdk/config.py
+-rw-r--r--   0        0        0     2745 2023-05-03 01:58:12.947245 bacalhau_sdk-0.3.29/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-05-03 01:57:47.303356 bacalhau_sdk-0.3.29/tests/__init__.py
+-rw-r--r--   0        0        0     6721 2023-05-03 01:57:47.303356 bacalhau_sdk-0.3.29/tests/test_config.py
+-rw-r--r--   0        0        0     9315 1970-01-01 00:00:00.000000 bacalhau_sdk-0.3.29/PKG-INFO
```

### Comparing `bacalhau_sdk-0.3.28/LICENSE` & `bacalhau_sdk-0.3.29/LICENSE`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-0.3.28/README.md` & `bacalhau_sdk-0.3.29/README.md`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-0.3.28/bacalhau_sdk/api.py` & `bacalhau_sdk-0.3.29/bacalhau_sdk/api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-0.3.28/bacalhau_sdk/config.py` & `bacalhau_sdk-0.3.29/bacalhau_sdk/config.py`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-0.3.28/pyproject.toml` & `bacalhau_sdk-0.3.29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "bacalhau-sdk"
-version = "0.3.28"
+version = "0.3.29"
 homepage = "https://github.com/bacalhau-project/bacalhau/"
 repository = "https://github.com/bacalhau-project/bacalhau/"
 documentation = "https://docs.bacalhau.org/"
 keywords = ["bacalhau", "Filecoin", "IPFS", "cod", "compute over data", "verifiable computation"]
 description = "Compute over Data framework for public, transparent, and optionally verifiable computation using IPFS & Filecoin."
 authors = ["Enrico Rotundo <team@bacalhau.org>"]
 readme = "README.md"
```

### Comparing `bacalhau_sdk-0.3.28/tests/test_config.py` & `bacalhau_sdk-0.3.29/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-0.3.28/PKG-INFO` & `bacalhau_sdk-0.3.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacalhau-sdk
-Version: 0.3.28
+Version: 0.3.29
 Summary: Compute over Data framework for public, transparent, and optionally verifiable computation using IPFS & Filecoin.
 Home-page: https://github.com/bacalhau-project/bacalhau/
 License: Apache-2.0
 Keywords: bacalhau,Filecoin,IPFS,cod,compute over data,verifiable computation
 Author: Enrico Rotundo
 Author-email: team@bacalhau.org
 Requires-Python: >=3.8.1,<3.12
```

