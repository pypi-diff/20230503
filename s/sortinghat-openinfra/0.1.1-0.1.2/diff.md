# Comparing `tmp/sortinghat_openinfra-0.1.1.tar.gz` & `tmp/sortinghat_openinfra-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortinghat_openinfra-0.1.1.tar", max compression
+gzip compressed data, was "sortinghat_openinfra-0.1.2.tar", max compression
```

## Comparing `sortinghat_openinfra-0.1.1.tar` & `sortinghat_openinfra-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/LICENSE
--rw-r--r--   0        0        0     2244 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/README.md
--rw-r--r--   0        0        0     1248 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       86 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/sortinghat/core/importer/backends/_version.py
--rw-r--r--   0        0        0     7864 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/sortinghat/core/importer/backends/openinfra.py
--rw-r--r--   0        0        0        0 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     6403 2023-04-27 12:20:41.000426 sortinghat_openinfra-0.1.1/tests/data/openinfra_page_1.json
--rw-r--r--   0        0        0     5073 2023-04-27 12:20:41.004426 sortinghat_openinfra-0.1.1/tests/data/openinfra_page_2.json
--rw-r--r--   0        0        0     2595 2023-04-27 12:20:41.004426 sortinghat_openinfra-0.1.1/tests/data/openinfra_private.json
--rw-r--r--   0        0        0    17771 2023-04-27 12:20:41.004426 sortinghat_openinfra-0.1.1/tests/test_openinfra.py
--rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 sortinghat_openinfra-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-02 22:36:20.344076 sortinghat_openinfra-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2244 2023-05-02 22:36:20.344076 sortinghat_openinfra-0.1.2/README.md
+-rw-r--r--   0        0        0     1268 2023-05-02 22:36:20.344076 sortinghat_openinfra-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/sortinghat/core/importer/backends/_version.py
+-rw-r--r--   0        0        0     7864 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/sortinghat/core/importer/backends/openinfra.py
+-rw-r--r--   0        0        0        0 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     6403 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/tests/data/openinfra_page_1.json
+-rw-r--r--   0        0        0     5073 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/tests/data/openinfra_page_2.json
+-rw-r--r--   0        0        0     2595 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/tests/data/openinfra_private.json
+-rw-r--r--   0        0        0    17771 2023-05-02 22:36:20.348076 sortinghat_openinfra-0.1.2/tests/test_openinfra.py
+-rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 sortinghat_openinfra-0.1.2/PKG-INFO
```

### Comparing `sortinghat_openinfra-0.1.1/LICENSE` & `sortinghat_openinfra-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.1/README.md` & `sortinghat_openinfra-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.1/pyproject.toml` & `sortinghat_openinfra-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sortinghat-openinfra"
-version = "0.1.1"
+version = "0.1.2"
 description = "SortingHat backend to import identities from OpenInfraID"
 authors = [
     "Bitergia Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -36,14 +36,15 @@
 "Bug Tracker" = "https://github.com/bitergia-analytics/sortinghat-openinfra/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 
 sortinghat = { version = ">=0.8.1", allow-prereleases = true}
 grimoirelab-toolkit = { version = ">=0.3", allow-prereleases = true}
+django-rq = "2.7.0"
 
 [tool.poetry.group.dev.dependencies]
 httpretty = "^1.1.4"
 flake8 = "^4.0.1"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `sortinghat_openinfra-0.1.1/sortinghat/core/importer/backends/openinfra.py` & `sortinghat_openinfra-0.1.2/sortinghat/core/importer/backends/openinfra.py`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.1/tests/data/openinfra_page_1.json` & `sortinghat_openinfra-0.1.2/tests/data/openinfra_page_1.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.1/tests/data/openinfra_page_2.json` & `sortinghat_openinfra-0.1.2/tests/data/openinfra_page_2.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.1/tests/data/openinfra_private.json` & `sortinghat_openinfra-0.1.2/tests/data/openinfra_private.json`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.1/tests/test_openinfra.py` & `sortinghat_openinfra-0.1.2/tests/test_openinfra.py`

 * *Files identical despite different names*

### Comparing `sortinghat_openinfra-0.1.1/PKG-INFO` & `sortinghat_openinfra-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortinghat-openinfra
-Version: 0.1.1
+Version: 0.1.2
 Summary: SortingHat backend to import identities from OpenInfraID
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab,sortinghat
 Author: Bitergia Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
+Requires-Dist: django-rq (==2.7.0)
 Requires-Dist: grimoirelab-toolkit (>=0.3)
 Requires-Dist: sortinghat (>=0.8.1)
 Project-URL: Bug Tracker, https://github.com/bitergia-analytics/sortinghat-openinfra/issues
 Project-URL: Repository, https://github.com/bitergia-analytics/sortinghat-openinfra
 Description-Content-Type: text/markdown
 
 # sortinghat-openinfra
```

