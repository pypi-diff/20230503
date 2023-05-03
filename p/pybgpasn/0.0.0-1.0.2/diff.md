# Comparing `tmp/pybgpasn-0.0.0.tar.gz` & `tmp/pybgpasn-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybgpasn-0.0.0.tar", last modified: Wed May  3 10:08:04 2023, max compression
+gzip compressed data, was "pybgpasn-1.0.2.tar", max compression
```

## Comparing `pybgpasn-0.0.0.tar` & `pybgpasn-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,6 @@
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-03 10:08:04.335899 pybgpasn-0.0.0/
--rw-r--r--   0 MTeke1     (502) staff       (20)     1070 2023-05-03 09:53:36.000000 pybgpasn-0.0.0/LICENSE
--rw-r--r--   0 MTeke1     (502) staff       (20)       74 2023-05-03 10:08:04.335730 pybgpasn-0.0.0/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-05-03 09:51:45.000000 pybgpasn-0.0.0/README.md
--rw-r--r--   0 MTeke1     (502) staff       (20)      579 2023-05-03 10:03:47.000000 pybgpasn-0.0.0/pyproject.toml
--rw-r--r--   0 MTeke1     (502) staff       (20)       38 2023-05-03 10:08:04.335948 pybgpasn-0.0.0/setup.cfg
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-03 10:08:04.333228 pybgpasn-0.0.0/src/
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-03 10:08:04.334446 pybgpasn-0.0.0/src/pybgpasn/
--rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-05-03 09:31:10.000000 pybgpasn-0.0.0/src/pybgpasn/__init__.py
--rw-r--r--   0 MTeke1     (502) staff       (20)      235 2023-05-03 09:57:31.000000 pybgpasn-0.0.0/src/pybgpasn/pybgpasn.py
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-03 10:08:04.335518 pybgpasn-0.0.0/src/pybgpasn.egg-info/
--rw-r--r--   0 MTeke1     (502) staff       (20)       74 2023-05-03 10:08:04.000000 pybgpasn-0.0.0/src/pybgpasn.egg-info/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)      226 2023-05-03 10:08:04.000000 pybgpasn-0.0.0/src/pybgpasn.egg-info/SOURCES.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)        1 2023-05-03 10:08:04.000000 pybgpasn-0.0.0/src/pybgpasn.egg-info/dependency_links.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)        9 2023-05-03 10:08:04.000000 pybgpasn-0.0.0/src/pybgpasn.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1070 2023-05-03 10:16:14.287661 pybgpasn-1.0.2/LICENSE
+-rw-r--r--   0        0        0       83 2023-05-03 10:55:28.693295 pybgpasn-1.0.2/README.md
+-rw-r--r--   0        0        0      578 2023-05-03 10:54:27.829967 pybgpasn-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-03 09:31:10.190023 pybgpasn-1.0.2/src/pybgpasn/__init__.py
+-rw-r--r--   0        0        0      235 2023-05-03 10:56:54.323620 pybgpasn-1.0.2/src/pybgpasn/pybgpasn.py
+-rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 pybgpasn-1.0.2/PKG-INFO
```

### Comparing `pybgpasn-0.0.0/LICENSE` & `pybgpasn-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybgpasn-0.0.0/pyproject.toml` & `pybgpasn-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pybgpasn"
-version = "1.0.1"
+version = "1.0.2"
 description = "A small package for obtaining the Registered ISP name per ASN number"
 authors = ["Melih Teke <me@mteke.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/melihteke/pybgpasn"
 repository = "https://github.com/melihteke/pybgpasn"
 documentation = "https://github.com/melihteke/pybgpasn/blob/master/README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.4"
+pytest = "^6.2.4"
```

