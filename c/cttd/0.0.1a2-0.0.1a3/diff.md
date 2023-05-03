# Comparing `tmp/cttd-0.0.1a2.tar.gz` & `tmp/cttd-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cttd-0.0.1a2.tar", max compression
+gzip compressed data, was "cttd-0.0.1a3.tar", max compression
```

## Comparing `cttd-0.0.1a2.tar` & `cttd-0.0.1a3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 cttd-0.0.1a2/LICENSE
--rw-r--r--   0        0        0     2025 2023-05-03 18:54:09.035294 cttd-0.0.1a2/README.md
--rw-r--r--   0        0        0       28 2023-05-03 18:15:09.070117 cttd-0.0.1a2/cttd/__init__.py
--rw-r--r--   0        0        0       55 2023-05-03 18:26:42.187993 cttd-0.0.1a2/cttd/factory.py
--rw-r--r--   0        0        0     2175 2023-05-03 18:28:56.276959 cttd-0.0.1a2/cttd/tester.py
--rw-r--r--   0        0        0      704 2023-05-03 18:56:38.372977 cttd-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 cttd-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-03 17:25:05.122292 cttd-0.0.1a3/LICENSE
+-rw-r--r--   0        0        0     2025 2023-05-03 18:54:09.035294 cttd-0.0.1a3/README.md
+-rw-r--r--   0        0        0       28 2023-05-03 18:15:09.070117 cttd-0.0.1a3/cttd/__init__.py
+-rw-r--r--   0        0        0       55 2023-05-03 18:26:42.187993 cttd-0.0.1a3/cttd/factory.py
+-rw-r--r--   0        0        0     2175 2023-05-03 18:28:56.276959 cttd-0.0.1a3/cttd/tester.py
+-rw-r--r--   0        0        0      738 2023-05-03 19:53:57.721984 cttd-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 cttd-0.0.1a3/PKG-INFO
```

### Comparing `cttd-0.0.1a2/LICENSE` & `cttd-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `cttd-0.0.1a2/README.md` & `cttd-0.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `cttd-0.0.1a2/cttd/tester.py` & `cttd-0.0.1a3/cttd/tester.py`

 * *Files identical despite different names*

### Comparing `cttd-0.0.1a2/pyproject.toml` & `cttd-0.0.1a3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cttd"
-version = "0.0.1a2"
+version = "0.0.1a3"
 description = "C test-driven development framework implemented in Python"
 authors = [
   "WideOpenTech <fossie@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -15,15 +15,16 @@
 
 [project.urls]
 "Homepage" = "https://github.com/wideopensource/cttd"
 "Bug Tracker" = "https://github.com/wideopensource/cttd/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-
+crelm = "^0.0.32"
+john = "^0.1.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cttd-0.0.1a2/PKG-INFO` & `cttd-0.0.1a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: cttd
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: C test-driven development framework implemented in Python
 Home-page: https://github.com/wideopensource/cttd
 Author: WideOpenTech
 Author-email: fossie@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
+Requires-Dist: crelm (>=0.0.32,<0.0.33)
+Requires-Dist: john (>=0.1.5,<0.2.0)
 Project-URL: Repository, https://github.com/wideopensource/cttd
 Description-Content-Type: text/markdown
 
 # cttd
 
 ## tl:dr
```

