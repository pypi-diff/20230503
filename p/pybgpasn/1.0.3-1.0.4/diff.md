# Comparing `tmp/pybgpasn-1.0.3.tar.gz` & `tmp/pybgpasn-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybgpasn-1.0.3.tar", max compression
+gzip compressed data, was "pybgpasn-1.0.4.tar", max compression
```

## Comparing `pybgpasn-1.0.3.tar` & `pybgpasn-1.0.4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-05-03 10:16:14.287661 pybgpasn-1.0.3/LICENSE
--rw-r--r--   0        0        0       83 2023-05-03 10:55:28.693295 pybgpasn-1.0.3/README.md
--rw-r--r--   0        0        0      578 2023-05-03 11:08:36.166878 pybgpasn-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       61 2023-05-03 11:08:37.529595 pybgpasn-1.0.3/src/pybgpasn/__init__.py
--rw-r--r--   0        0        0      235 2023-05-03 10:56:54.323620 pybgpasn-1.0.3/src/pybgpasn/pybgpasn.py
--rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 pybgpasn-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-03 10:16:14.287661 pybgpasn-1.0.4/LICENSE
+-rw-r--r--   0        0        0       83 2023-05-03 10:55:28.693295 pybgpasn-1.0.4/README.md
+-rw-r--r--   0        0        0      578 2023-05-03 11:17:06.212969 pybgpasn-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-03 11:15:54.370270 pybgpasn-1.0.4/src/pybgpasn/__init__.py
+-rw-r--r--   0        0        0  1700701 2023-05-03 09:25:34.029925 pybgpasn-1.0.4/src/pybgpasn/bgp_asn.json
+-rw-r--r--   0        0        0      225 2023-05-03 11:16:38.828879 pybgpasn-1.0.4/src/pybgpasn/pybgpasn.py
+-rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 pybgpasn-1.0.4/PKG-INFO
```

### Comparing `pybgpasn-1.0.3/LICENSE` & `pybgpasn-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pybgpasn-1.0.3/pyproject.toml` & `pybgpasn-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pybgpasn"
-version = "1.0.3"
+version = "1.0.4"
 description = "A small package for obtaining the Registered ISP name per ASN number"
 authors = ["Melih Teke <me@mteke.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/melihteke/pybgpasn"
 repository = "https://github.com/melihteke/pybgpasn"
 documentation = "https://github.com/melihteke/pybgpasn/blob/master/README.md"
```

### Comparing `pybgpasn-1.0.3/PKG-INFO` & `pybgpasn-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybgpasn
-Version: 1.0.3
+Version: 1.0.4
 Summary: A small package for obtaining the Registered ISP name per ASN number
 Home-page: https://github.com/melihteke/pybgpasn
 License: MIT
 Author: Melih Teke
 Author-email: me@mteke.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

