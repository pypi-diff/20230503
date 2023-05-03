# Comparing `tmp/pybgpasn-1.0.5.tar.gz` & `tmp/pybgpasn-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybgpasn-1.0.5.tar", max compression
+gzip compressed data, was "pybgpasn-1.0.6.tar", max compression
```

## Comparing `pybgpasn-1.0.5.tar` & `pybgpasn-1.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-05-03 10:16:14.287661 pybgpasn-1.0.5/LICENSE
--rw-r--r--   0        0        0       83 2023-05-03 10:55:28.693295 pybgpasn-1.0.5/README.md
--rw-r--r--   0        0        0      578 2023-05-03 11:32:39.941690 pybgpasn-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-03 11:32:23.229858 pybgpasn-1.0.5/src/pybgpasn/__init__.py
--rw-r--r--   0        0        0  1700712 2023-05-03 11:32:15.395382 pybgpasn-1.0.5/src/pybgpasn/bgp_asn_db.py
--rw-r--r--   0        0        0      201 2023-05-03 11:32:13.667246 pybgpasn-1.0.5/src/pybgpasn/pybgpasn.py
--rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 pybgpasn-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-03 10:16:14.287661 pybgpasn-1.0.6/LICENSE
+-rw-r--r--   0        0        0       83 2023-05-03 10:55:28.693295 pybgpasn-1.0.6/README.md
+-rw-r--r--   0        0        0      578 2023-05-03 11:42:09.644181 pybgpasn-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-03 11:32:23.229858 pybgpasn-1.0.6/src/pybgpasn/__init__.py
+-rw-r--r--   0        0        0  1700712 2023-05-03 11:32:15.395382 pybgpasn-1.0.6/src/pybgpasn/bgp_asn_db.py
+-rw-r--r--   0        0        0      210 2023-05-03 11:42:01.747627 pybgpasn-1.0.6/src/pybgpasn/pybgpasn.py
+-rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 pybgpasn-1.0.6/PKG-INFO
```

### Comparing `pybgpasn-1.0.5/LICENSE` & `pybgpasn-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pybgpasn-1.0.5/pyproject.toml` & `pybgpasn-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pybgpasn"
-version = "1.0.5"
+version = "1.0.6"
 description = "A small package for obtaining the Registered ISP name per ASN number"
 authors = ["Melih Teke <me@mteke.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/melihteke/pybgpasn"
 repository = "https://github.com/melihteke/pybgpasn"
 documentation = "https://github.com/melihteke/pybgpasn/blob/master/README.md"
```

### Comparing `pybgpasn-1.0.5/src/pybgpasn/bgp_asn_db.py` & `pybgpasn-1.0.6/src/pybgpasn/bgp_asn_db.py`

 * *Files identical despite different names*

### Comparing `pybgpasn-1.0.5/PKG-INFO` & `pybgpasn-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybgpasn
-Version: 1.0.5
+Version: 1.0.6
 Summary: A small package for obtaining the Registered ISP name per ASN number
 Home-page: https://github.com/melihteke/pybgpasn
 License: MIT
 Author: Melih Teke
 Author-email: me@mteke.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

