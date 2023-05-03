# Comparing `tmp/findmyorder-1.1.2.tar.gz` & `tmp/findmyorder-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.1.2.tar", max compression
+gzip compressed data, was "findmyorder-1.1.3.tar", max compression
```

## Comparing `findmyorder-1.1.2.tar` & `findmyorder-1.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-03 14:19:24.563765 findmyorder-1.1.2/LICENSE
--rw-r--r--   0        0        0     2180 2023-05-03 14:19:24.563765 findmyorder-1.1.2/README.md
--rw-r--r--   0        0        0      113 2023-05-03 14:19:25.327777 findmyorder-1.1.2/findmyorder/__init__.py
--rw-r--r--   0        0        0      392 2023-05-03 14:19:24.563765 findmyorder-1.1.2/findmyorder/config.py
--rw-r--r--   0        0        0      312 2023-05-03 14:19:24.563765 findmyorder-1.1.2/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     3866 2023-05-03 14:19:24.563765 findmyorder-1.1.2/findmyorder/main.py
--rw-r--r--   0        0        0     1223 2023-05-03 14:19:25.327777 findmyorder-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 findmyorder-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-03 14:31:53.492649 findmyorder-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2180 2023-05-03 14:31:53.492649 findmyorder-1.1.3/README.md
+-rw-r--r--   0        0        0      113 2023-05-03 14:31:54.192642 findmyorder-1.1.3/findmyorder/__init__.py
+-rw-r--r--   0        0        0      392 2023-05-03 14:31:53.492649 findmyorder-1.1.3/findmyorder/config.py
+-rw-r--r--   0        0        0      312 2023-05-03 14:31:53.492649 findmyorder-1.1.3/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     3866 2023-05-03 14:31:53.492649 findmyorder-1.1.3/findmyorder/main.py
+-rw-r--r--   0        0        0     1259 2023-05-03 14:31:54.192642 findmyorder-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 findmyorder-1.1.3/PKG-INFO
```

### Comparing `findmyorder-1.1.2/LICENSE` & `findmyorder-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.2/README.md` & `findmyorder-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.2/findmyorder/main.py` & `findmyorder-1.1.3/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.2/pyproject.toml` & `findmyorder-1.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.1.2"
+version = "1.1.3"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 
 
@@ -30,14 +30,15 @@
   "*Test"
 ]
 log_format = "%(asctime)s - %(levelname)s - %(name)s - %(message)s"
 log_level = "DEBUG"
 pythonpath = [
   "."
 ]
+addopts = "--ignore-glob=example_*"
 
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","findmyorder/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
```

### Comparing `findmyorder-1.1.2/PKG-INFO` & `findmyorder-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.1.2
+Version: 1.1.3
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

