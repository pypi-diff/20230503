# Comparing `tmp/john-0.1.5.tar.gz` & `tmp/john-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "john-0.1.5.tar", max compression
+gzip compressed data, was "john-0.1.5a0.tar", max compression
```

## Comparing `john-0.1.5.tar` & `john-0.1.5a0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1108 2023-04-24 10:27:11.710010 john-0.1.5/LICENSE
--rw-r--r--   0        0        0      268 2023-04-24 10:27:11.710010 john-0.1.5/README.md
--rw-r--r--   0        0        0       85 2023-04-24 13:37:39.992745 john-0.1.5/john/__init__.py
--rw-r--r--   0        0        0      106 2023-04-24 10:27:11.710010 john-0.1.5/john/factory.py
--rw-r--r--   0        0        0     2090 2023-05-03 15:54:44.915729 john-0.1.5/john/tdd.py
--rw-r--r--   0        0        0     7943 2023-05-03 15:55:42.420797 john-0.1.5/john/test_case.py
--rw-r--r--   0        0        0      679 2023-05-03 17:13:20.071433 john-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 john-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-04-24 10:27:11.710010 john-0.1.5a0/LICENSE
+-rw-r--r--   0        0        0      268 2023-04-24 10:27:11.710010 john-0.1.5a0/README.md
+-rw-r--r--   0        0        0       85 2023-04-24 13:37:39.992745 john-0.1.5a0/john/__init__.py
+-rw-r--r--   0        0        0      106 2023-04-24 10:27:11.710010 john-0.1.5a0/john/factory.py
+-rw-r--r--   0        0        0     2090 2023-05-03 15:54:44.915729 john-0.1.5a0/john/tdd.py
+-rw-r--r--   0        0        0     7943 2023-05-03 15:55:42.420797 john-0.1.5a0/john/test_case.py
+-rw-r--r--   0        0        0      681 2023-05-03 17:03:16.264584 john-0.1.5a0/pyproject.toml
+-rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 john-0.1.5a0/PKG-INFO
```

### Comparing `john-0.1.5/LICENSE` & `john-0.1.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `john-0.1.5/john/tdd.py` & `john-0.1.5a0/john/tdd.py`

 * *Files identical despite different names*

### Comparing `john-0.1.5/john/test_case.py` & `john-0.1.5a0/john/test_case.py`

 * *Files identical despite different names*

### Comparing `john-0.1.5/pyproject.toml` & `john-0.1.5a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "john"
-version = "0.1.5"
+version = "0.1.5a0"
 description = "Jeneral Outlying Helper Nuggetoids"
 authors = [
   "WideOpenTech <fossie@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `john-0.1.5/PKG-INFO` & `john-0.1.5a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: john
-Version: 0.1.5
+Version: 0.1.5a0
 Summary: Jeneral Outlying Helper Nuggetoids
 Home-page: https://github.com/wideopensource/john
 Author: WideOpenTech
 Author-email: fossie@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

