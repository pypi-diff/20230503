# Comparing `tmp/pybgpasn-1.0.7.tar.gz` & `tmp/pybgpasn-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybgpasn-1.0.7.tar", max compression
+gzip compressed data, was "pybgpasn-1.0.9.tar", max compression
```

## Comparing `pybgpasn-1.0.7.tar` & `pybgpasn-1.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-05-03 10:16:14.287661 pybgpasn-1.0.7/LICENSE
--rw-r--r--   0        0        0       83 2023-05-03 10:55:28.693295 pybgpasn-1.0.7/README.md
--rw-r--r--   0        0        0      578 2023-05-03 13:45:50.535478 pybgpasn-1.0.7/pyproject.toml
--rw-r--r--   0        0        0       28 2023-05-03 13:45:19.884782 pybgpasn-1.0.7/src/pybgpasn/__init__.py
--rw-r--r--   0        0        0  1700712 2023-05-03 11:32:15.395382 pybgpasn-1.0.7/src/pybgpasn/bgp_asn_db.py
--rw-r--r--   0        0        0      210 2023-05-03 13:45:44.658569 pybgpasn-1.0.7/src/pybgpasn/pybgpasn.py
--rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 pybgpasn-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-03 10:16:14.287661 pybgpasn-1.0.9/LICENSE
+-rw-r--r--   0        0        0     2201 2023-05-03 14:08:48.516808 pybgpasn-1.0.9/README.md
+-rw-r--r--   0        0        0      578 2023-05-03 14:08:55.179848 pybgpasn-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-05-03 14:01:49.327536 pybgpasn-1.0.9/src/pybgpasn/__init__.py
+-rw-r--r--   0        0        0  1700712 2023-05-03 11:32:15.395382 pybgpasn-1.0.9/src/pybgpasn/bgp_asn_db.py
+-rw-r--r--   0        0        0      469 2023-05-03 14:02:25.597366 pybgpasn-1.0.9/src/pybgpasn/pybgpasn.py
+-rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 pybgpasn-1.0.9/PKG-INFO
```

### Comparing `pybgpasn-1.0.7/LICENSE` & `pybgpasn-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pybgpasn-1.0.7/pyproject.toml` & `pybgpasn-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pybgpasn"
-version = "1.0.7"
+version = "1.0.9"
 description = "A small package for obtaining the Registered ISP name per ASN number"
 authors = ["Melih Teke <me@mteke.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/melihteke/pybgpasn"
 repository = "https://github.com/melihteke/pybgpasn"
 documentation = "https://github.com/melihteke/pybgpasn/blob/master/README.md"
```

### Comparing `pybgpasn-1.0.7/src/pybgpasn/bgp_asn_db.py` & `pybgpasn-1.0.9/src/pybgpasn/bgp_asn_db.py`

 * *Files identical despite different names*

