# Comparing `tmp/toolkit_lennart-0.0.7.tar.gz` & `tmp/toolkit_lennart-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolkit_lennart-0.0.7.tar", last modified: Wed May  3 18:34:43 2023, max compression
+gzip compressed data, was "toolkit_lennart-0.0.8.tar", last modified: Wed May  3 18:44:53 2023, max compression
```

## Comparing `toolkit_lennart-0.0.7.tar` & `toolkit_lennart-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lrooden    (502) staff       (20)        0 2023-05-03 18:34:43.787632 toolkit_lennart-0.0.7/
--rw-r--r--   0 lrooden    (502) staff       (20)     1073 2023-04-15 11:01:47.000000 toolkit_lennart-0.0.7/LICENSE
--rw-r--r--   0 lrooden    (502) staff       (20)      655 2023-05-03 18:34:43.787413 toolkit_lennart-0.0.7/PKG-INFO
--rw-r--r--   0 lrooden    (502) staff       (20)      194 2023-05-03 18:21:09.000000 toolkit_lennart-0.0.7/README.md
--rw-r--r--   0 lrooden    (502) staff       (20)      572 2023-05-03 18:19:50.000000 toolkit_lennart-0.0.7/pyproject.toml
--rw-r--r--   0 lrooden    (502) staff       (20)       38 2023-05-03 18:34:43.787719 toolkit_lennart-0.0.7/setup.cfg
--rw-r--r--   0 lrooden    (502) staff       (20)      295 2023-05-03 18:19:50.000000 toolkit_lennart-0.0.7/setup.py
-drwxr-xr-x   0 lrooden    (502) staff       (20)        0 2023-05-03 18:34:43.785790 toolkit_lennart-0.0.7/toolkit_lennart/
--rw-r--r--   0 lrooden    (502) staff       (20)        0 2023-04-15 10:52:04.000000 toolkit_lennart-0.0.7/toolkit_lennart/__init__.py
--rw-r--r--   0 lrooden    (502) staff       (20)     1536 2023-04-15 18:03:42.000000 toolkit_lennart-0.0.7/toolkit_lennart/plot.py
-drwxr-xr-x   0 lrooden    (502) staff       (20)        0 2023-05-03 18:34:43.787051 toolkit_lennart-0.0.7/toolkit_lennart.egg-info/
--rw-r--r--   0 lrooden    (502) staff       (20)      655 2023-05-03 18:34:43.000000 toolkit_lennart-0.0.7/toolkit_lennart.egg-info/PKG-INFO
--rw-r--r--   0 lrooden    (502) staff       (20)      249 2023-05-03 18:34:43.000000 toolkit_lennart-0.0.7/toolkit_lennart.egg-info/SOURCES.txt
--rw-r--r--   0 lrooden    (502) staff       (20)        1 2023-05-03 18:34:43.000000 toolkit_lennart-0.0.7/toolkit_lennart.egg-info/dependency_links.txt
--rw-r--r--   0 lrooden    (502) staff       (20)       16 2023-05-03 18:34:43.000000 toolkit_lennart-0.0.7/toolkit_lennart.egg-info/top_level.txt
+drwxr-xr-x   0 lrooden    (502) staff       (20)        0 2023-05-03 18:44:53.638123 toolkit_lennart-0.0.8/
+-rw-r--r--   0 lrooden    (502) staff       (20)     1073 2023-04-15 11:01:47.000000 toolkit_lennart-0.0.8/LICENSE
+-rw-r--r--   0 lrooden    (502) staff       (20)      655 2023-05-03 18:44:53.637924 toolkit_lennart-0.0.8/PKG-INFO
+-rw-r--r--   0 lrooden    (502) staff       (20)      194 2023-05-03 18:21:09.000000 toolkit_lennart-0.0.8/README.md
+-rw-r--r--   0 lrooden    (502) staff       (20)      572 2023-05-03 18:35:15.000000 toolkit_lennart-0.0.8/pyproject.toml
+-rw-r--r--   0 lrooden    (502) staff       (20)       38 2023-05-03 18:44:53.638198 toolkit_lennart-0.0.8/setup.cfg
+-rw-r--r--   0 lrooden    (502) staff       (20)      295 2023-05-03 18:40:06.000000 toolkit_lennart-0.0.8/setup.py
+drwxr-xr-x   0 lrooden    (502) staff       (20)        0 2023-05-03 18:44:53.636531 toolkit_lennart-0.0.8/toolkit_lennart/
+-rw-r--r--   0 lrooden    (502) staff       (20)        0 2023-04-15 10:52:04.000000 toolkit_lennart-0.0.8/toolkit_lennart/__init__.py
+-rw-r--r--   0 lrooden    (502) staff       (20)     1536 2023-04-15 18:03:42.000000 toolkit_lennart-0.0.8/toolkit_lennart/plot.py
+drwxr-xr-x   0 lrooden    (502) staff       (20)        0 2023-05-03 18:44:53.637502 toolkit_lennart-0.0.8/toolkit_lennart.egg-info/
+-rw-r--r--   0 lrooden    (502) staff       (20)      655 2023-05-03 18:44:53.000000 toolkit_lennart-0.0.8/toolkit_lennart.egg-info/PKG-INFO
+-rw-r--r--   0 lrooden    (502) staff       (20)      249 2023-05-03 18:44:53.000000 toolkit_lennart-0.0.8/toolkit_lennart.egg-info/SOURCES.txt
+-rw-r--r--   0 lrooden    (502) staff       (20)        1 2023-05-03 18:44:53.000000 toolkit_lennart-0.0.8/toolkit_lennart.egg-info/dependency_links.txt
+-rw-r--r--   0 lrooden    (502) staff       (20)       16 2023-05-03 18:44:53.000000 toolkit_lennart-0.0.8/toolkit_lennart.egg-info/top_level.txt
```

### Comparing `toolkit_lennart-0.0.7/LICENSE` & `toolkit_lennart-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `toolkit_lennart-0.0.7/PKG-INFO` & `toolkit_lennart-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: toolkit_lennart
-Version: 0.0.7
+Version: 0.0.8
 Summary: Toolkit for data analysis
-Home-page: https://pypi.org/project/toolkit-lennart/0.0.6/
+Home-page: https://pypi.org/project/toolkit-lennart/0.0.8/
 Author: Lennart Rooden
 Author-email: Lennart Rooden <lennart.rs@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `toolkit_lennart-0.0.7/pyproject.toml` & `toolkit_lennart-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "toolkit_lennart"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Lennart Rooden", email="lennart.rs@gmail.com" },
 ]
 description = "Toolkit for data analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `toolkit_lennart-0.0.7/toolkit_lennart/plot.py` & `toolkit_lennart-0.0.8/toolkit_lennart/plot.py`

 * *Files identical despite different names*

### Comparing `toolkit_lennart-0.0.7/toolkit_lennart.egg-info/PKG-INFO` & `toolkit_lennart-0.0.8/toolkit_lennart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: toolkit-lennart
-Version: 0.0.7
+Version: 0.0.8
 Summary: Toolkit for data analysis
-Home-page: https://pypi.org/project/toolkit-lennart/0.0.6/
+Home-page: https://pypi.org/project/toolkit-lennart/0.0.8/
 Author: Lennart Rooden
 Author-email: Lennart Rooden <lennart.rs@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

