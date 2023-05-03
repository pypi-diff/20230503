# Comparing `tmp/findmyorder-1.1.3.tar.gz` & `tmp/findmyorder-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.1.3.tar", max compression
+gzip compressed data, was "findmyorder-1.1.4.tar", max compression
```

## Comparing `findmyorder-1.1.3.tar` & `findmyorder-1.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-03 14:31:53.492649 findmyorder-1.1.3/LICENSE
--rw-r--r--   0        0        0     2180 2023-05-03 14:31:53.492649 findmyorder-1.1.3/README.md
--rw-r--r--   0        0        0      113 2023-05-03 14:31:54.192642 findmyorder-1.1.3/findmyorder/__init__.py
--rw-r--r--   0        0        0      392 2023-05-03 14:31:53.492649 findmyorder-1.1.3/findmyorder/config.py
--rw-r--r--   0        0        0      312 2023-05-03 14:31:53.492649 findmyorder-1.1.3/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     3866 2023-05-03 14:31:53.492649 findmyorder-1.1.3/findmyorder/main.py
--rw-r--r--   0        0        0     1259 2023-05-03 14:31:54.192642 findmyorder-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 findmyorder-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-03 15:09:53.553183 findmyorder-1.1.4/LICENSE
+-rw-r--r--   0        0        0     2180 2023-05-03 15:09:53.553183 findmyorder-1.1.4/README.md
+-rw-r--r--   0        0        0      113 2023-05-03 15:09:54.493189 findmyorder-1.1.4/findmyorder/__init__.py
+-rw-r--r--   0        0        0      392 2023-05-03 15:09:53.557183 findmyorder-1.1.4/findmyorder/config.py
+-rw-r--r--   0        0        0      383 2023-05-03 15:09:53.557183 findmyorder-1.1.4/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     3866 2023-05-03 15:09:53.557183 findmyorder-1.1.4/findmyorder/main.py
+-rw-r--r--   0        0        0     1280 2023-05-03 15:09:54.493189 findmyorder-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 findmyorder-1.1.4/PKG-INFO
```

### Comparing `findmyorder-1.1.3/LICENSE` & `findmyorder-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.3/README.md` & `findmyorder-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.3/findmyorder/main.py` & `findmyorder-1.1.4/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.3/pyproject.toml` & `findmyorder-1.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.1.3"
+version = "1.1.4"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 
 
@@ -18,14 +18,15 @@
 dynaconf = ">=3.1.12"
 pyparsing = ">=3.0.9"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 pytest = "*"
 pytest-cov = "*"
+pytest-asyncio = "*"
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 python_classes = [
   "Test*",
   "*Test"
 ]
```

### Comparing `findmyorder-1.1.3/PKG-INFO` & `findmyorder-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.1.3
+Version: 1.1.4
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

