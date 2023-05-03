# Comparing `tmp/crelm-0.0.32.tar.gz` & `tmp/crelm-0.0.32a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crelm-0.0.32.tar", max compression
+gzip compressed data, was "crelm-0.0.32a0.tar", max compression
```

## Comparing `crelm-0.0.32.tar` & `crelm-0.0.32a0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1108 2023-04-06 18:21:20.719078 crelm-0.0.32/LICENSE
--rw-r--r--   0        0        0      600 2023-04-06 18:21:20.719078 crelm-0.0.32/README.md
--rw-r--r--   0        0        0      187 2023-04-06 18:21:20.719078 crelm-0.0.32/crelm/__init__.py
--rw-r--r--   0        0        0     3071 2023-04-06 18:21:20.719078 crelm-0.0.32/crelm/factory.py
--rw-r--r--   0        0        0      391 2023-04-06 18:21:20.720078 crelm-0.0.32/crelm/libcrelm.py
--rw-r--r--   0        0        0   107326 2023-04-06 18:21:20.721078 crelm-0.0.32/crelm/makeheaders.c
--rw-r--r--   0        0        0     1987 2023-04-06 18:21:20.721078 crelm-0.0.32/crelm/makeheaders_crelm.c
--rw-r--r--   0        0        0    13575 2023-05-03 16:52:52.748523 crelm-0.0.32/crelm/tube.py
--rw-r--r--   0        0        0      776 2023-05-03 17:12:11.249349 crelm-0.0.32/pyproject.toml
--rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 crelm-0.0.32/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-04-06 18:21:20.719078 crelm-0.0.32a0/LICENSE
+-rw-r--r--   0        0        0      600 2023-04-06 18:21:20.719078 crelm-0.0.32a0/README.md
+-rw-r--r--   0        0        0      187 2023-04-06 18:21:20.719078 crelm-0.0.32a0/crelm/__init__.py
+-rw-r--r--   0        0        0     3071 2023-04-06 18:21:20.719078 crelm-0.0.32a0/crelm/factory.py
+-rw-r--r--   0        0        0      391 2023-04-06 18:21:20.720078 crelm-0.0.32a0/crelm/libcrelm.py
+-rw-r--r--   0        0        0   107326 2023-04-06 18:21:20.721078 crelm-0.0.32a0/crelm/makeheaders.c
+-rw-r--r--   0        0        0     1987 2023-04-06 18:21:20.721078 crelm-0.0.32a0/crelm/makeheaders_crelm.c
+-rw-r--r--   0        0        0    13575 2023-05-03 16:52:52.748523 crelm-0.0.32a0/crelm/tube.py
+-rw-r--r--   0        0        0      778 2023-05-03 17:07:52.738205 crelm-0.0.32a0/pyproject.toml
+-rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 crelm-0.0.32a0/PKG-INFO
```

### Comparing `crelm-0.0.32/LICENSE` & `crelm-0.0.32a0/LICENSE`

 * *Files identical despite different names*

### Comparing `crelm-0.0.32/README.md` & `crelm-0.0.32a0/README.md`

 * *Files identical despite different names*

### Comparing `crelm-0.0.32/crelm/factory.py` & `crelm-0.0.32a0/crelm/factory.py`

 * *Files identical despite different names*

### Comparing `crelm-0.0.32/crelm/makeheaders.c` & `crelm-0.0.32a0/crelm/makeheaders.c`

 * *Files identical despite different names*

### Comparing `crelm-0.0.32/crelm/makeheaders_crelm.c` & `crelm-0.0.32a0/crelm/makeheaders_crelm.c`

 * *Files identical despite different names*

### Comparing `crelm-0.0.32/crelm/tube.py` & `crelm-0.0.32a0/crelm/tube.py`

 * *Files identical despite different names*

### Comparing `crelm-0.0.32/pyproject.toml` & `crelm-0.0.32a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crelm"
-version = "0.0.32"
+version = "0.0.32a0"
 description = "Utility that automates turning simple C classes into Python objects"
 authors = [
   "WideOpenTech <foss@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `crelm-0.0.32/PKG-INFO` & `crelm-0.0.32a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crelm
-Version: 0.0.32
+Version: 0.0.32a0
 Summary: Utility that automates turning simple C classes into Python objects
 Home-page: https://github.com/wideopensource/crelm
 Author: WideOpenTech
 Author-email: foss@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

