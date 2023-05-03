# Comparing `tmp/local_migrator-0.1.8.tar.gz` & `tmp/local-migrator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_migrator-0.1.8.tar", last modified: Tue May  2 19:49:48 2023, max compression
+gzip compressed data, was "local-migrator-0.1.9.tar", last modified: Wed May  3 21:43:36 2023, max compression
```

## Comparing `local_migrator-0.1.8.tar` & `local-migrator-0.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.273054 local_migrator-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.269054 local_migrator-0.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-02 19:49:25.000000 local_migrator-0.1.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.269054 local_migrator-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-02 19:49:25.000000 local_migrator-0.1.8/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-02 19:49:25.000000 local_migrator-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-02 19:49:25.000000 local_migrator-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-02 19:49:25.000000 local_migrator-0.1.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-02 19:49:25.000000 local_migrator-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-02 19:49:48.273054 local_migrator-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-02 19:49:25.000000 local_migrator-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.269054 local_migrator-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 19:49:25.000000 local_migrator-0.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.273054 local_migrator-0.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-02 19:49:25.000000 local_migrator-0.1.8/examples/base_cbor_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-02 19:49:25.000000 local_migrator-0.1.8/examples/base_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-02 19:49:25.000000 local_migrator-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:49:48.273054 local_migrator-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.269054 local_migrator-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.273054 local_migrator-0.1.8/src/local_migrator/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/local_migrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/local_migrator/_class_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/local_migrator/_serialize_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/local_migrator/_testsupport.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.273054 local_migrator-0.1.8/src/local_migrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 19:49:48.000000 local_migrator-0.1.8/src/local_migrator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:49:48.273054 local_migrator-0.1.8/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/tests/class_register_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/tests/nme_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/tests/test_cbor_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/tests/test_class_register.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-02 19:49:25.000000 local_migrator-0.1.8/src/tests/test_json_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-02 19:49:25.000000 local_migrator-0.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:43:36.698457 local-migrator-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:43:36.694457 local-migrator-0.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-03 21:43:19.000000 local-migrator-0.1.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:43:36.694457 local-migrator-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-03 21:43:19.000000 local-migrator-0.1.9/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-03 21:43:19.000000 local-migrator-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-03 21:43:19.000000 local-migrator-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 21:43:19.000000 local-migrator-0.1.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-03 21:43:19.000000 local-migrator-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-03 21:43:36.698457 local-migrator-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-03 21:43:19.000000 local-migrator-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:43:36.694457 local-migrator-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 21:43:19.000000 local-migrator-0.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 21:43:19.000000 local-migrator-0.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-03 21:43:19.000000 local-migrator-0.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-03 21:43:19.000000 local-migrator-0.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-03 21:43:19.000000 local-migrator-0.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-03 21:43:19.000000 local-migrator-0.1.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 21:43:19.000000 local-migrator-0.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:43:36.698457 local-migrator-0.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-03 21:43:19.000000 local-migrator-0.1.9/examples/base_cbor_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-03 21:43:19.000000 local-migrator-0.1.9/examples/base_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-03 21:43:19.000000 local-migrator-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:43:36.698457 local-migrator-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:43:36.694457 local-migrator-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:43:36.698457 local-migrator-0.1.9/src/local_migrator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-03 21:43:19.000000 local-migrator-0.1.9/src/local_migrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-05-03 21:43:19.000000 local-migrator-0.1.9/src/local_migrator/_class_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-03 21:43:19.000000 local-migrator-0.1.9/src/local_migrator/_serialize_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-03 21:43:19.000000 local-migrator-0.1.9/src/local_migrator/_testsupport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 21:43:36.000000 local-migrator-0.1.9/src/local_migrator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:43:36.698457 local-migrator-0.1.9/src/local_migrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-03 21:43:36.000000 local-migrator-0.1.9/src/local_migrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-03 21:43:36.000000 local-migrator-0.1.9/src/local_migrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:43:36.000000 local-migrator-0.1.9/src/local_migrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 21:43:36.000000 local-migrator-0.1.9/src/local_migrator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 21:43:36.000000 local-migrator-0.1.9/src/local_migrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 21:43:36.000000 local-migrator-0.1.9/src/local_migrator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:43:36.698457 local-migrator-0.1.9/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 21:43:19.000000 local-migrator-0.1.9/src/tests/class_register_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-03 21:43:19.000000 local-migrator-0.1.9/src/tests/nme_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-03 21:43:19.000000 local-migrator-0.1.9/src/tests/test_cbor_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-03 21:43:19.000000 local-migrator-0.1.9/src/tests/test_class_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-03 21:43:19.000000 local-migrator-0.1.9/src/tests/test_json_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-03 21:43:19.000000 local-migrator-0.1.9/tox.ini
```

### Comparing `local_migrator-0.1.8/.github/workflows/tests.yml` & `local-migrator-0.1.9/.github/workflows/tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     steps:
       - uses: actions/checkout@v3
         with:
           path: "local_migrator_repo"
           fetch-depth: 0
       - uses: actions/checkout@v3
         with:
-          repo: "czaki/nme"
+          repository: "czaki/nme"
           path: "nme_repo"
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
       - name: Install dependencies
         run: |
```

### Comparing `local_migrator-0.1.8/.gitignore` & `local-migrator-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/.pre-commit-config.yaml` & `local-migrator-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/.readthedocs.yml` & `local-migrator-0.1.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/LICENSE.txt` & `local-migrator-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/PKG-INFO` & `local-migrator-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: local_migrator
-Version: 0.1.8
+Name: local-migrator
+Version: 0.1.9
 Summary: Package for simplify data structures migrations
 Author: Grzegorz Bokota
 Author-email: g.bokota@uw.edu.pl
 License: MIT
 Project-URL: Homepage, https://github.com/Czaki/local_migrator
-Project-URL: Documentation, https://local_migrator.readthedocs.io/en/latest/
+Project-URL: Documentation, https://local-migrator.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Czaki/local_migrator
-Keywords: napari,migration,persistance
+Keywords: migration,persistance
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -25,32 +25,32 @@
 Provides-Extra: cbor
 License-File: LICENSE.txt
 
 **************
 Local Migrator
 **************
 
-.. image:: https://codecov.io/gh/Czaki/local_migrator/branch/main/graph/badge.svg?token=KGEGEQYYRH
-  :target: https://codecov.io/gh/Czaki/local_migrator
+.. image:: https://codecov.io/gh/Czaki/local-migrator/branch/main/graph/badge.svg?token=KGEGEQYYRH
+  :target: https://codecov.io/gh/Czaki/local-migrator
   :alt: Codecov
 
-.. image:: https://github.com/Czaki/local_migrator/actions/workflows/tests.yml/badge.svg
-  :target: https://github.com/Czaki/local_migrator/actions/workflows/tests.yml
+.. image:: https://github.com/Czaki/local-migrator/actions/workflows/tests.yml/badge.svg
+  :target: https://github.com/Czaki/local-migrator/actions/workflows/tests.yml
   :alt: Test
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
   :target: https://github.com/psf/black
   :alt: Code Style
 
-.. image:: https://readthedocs.org/projects/local_migrator/badge/?version=latest
-  :target: https://local_migrator.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/local-migrator/badge/?version=latest
+  :target: https://local-migrator.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status
 
-.. image:: https://badge.fury.io/py/local_migrator.svg
-  :target: https://badge.fury.io/py/local_migrator
+.. image:: https://badge.fury.io/py/local-migrator.svg
+  :target: https://badge.fury.io/py/local-migrator
   :alt: PyPI version
 
 .. image:: https://anaconda.org/conda-forge/local_migrator/badges/version.svg
   :target: https://anaconda.org/conda-forge/local_migrator
   :alt: Anaconda version
```

### Comparing `local_migrator-0.1.8/README.rst` & `local-migrator-0.1.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 **************
 Local Migrator
 **************
 
-.. image:: https://codecov.io/gh/Czaki/local_migrator/branch/main/graph/badge.svg?token=KGEGEQYYRH
-  :target: https://codecov.io/gh/Czaki/local_migrator
+.. image:: https://codecov.io/gh/Czaki/local-migrator/branch/main/graph/badge.svg?token=KGEGEQYYRH
+  :target: https://codecov.io/gh/Czaki/local-migrator
   :alt: Codecov
 
-.. image:: https://github.com/Czaki/local_migrator/actions/workflows/tests.yml/badge.svg
-  :target: https://github.com/Czaki/local_migrator/actions/workflows/tests.yml
+.. image:: https://github.com/Czaki/local-migrator/actions/workflows/tests.yml/badge.svg
+  :target: https://github.com/Czaki/local-migrator/actions/workflows/tests.yml
   :alt: Test
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
   :target: https://github.com/psf/black
   :alt: Code Style
 
-.. image:: https://readthedocs.org/projects/local_migrator/badge/?version=latest
-  :target: https://local_migrator.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/local-migrator/badge/?version=latest
+  :target: https://local-migrator.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status
 
-.. image:: https://badge.fury.io/py/local_migrator.svg
-  :target: https://badge.fury.io/py/local_migrator
+.. image:: https://badge.fury.io/py/local-migrator.svg
+  :target: https://badge.fury.io/py/local-migrator
   :alt: PyPI version
 
 .. image:: https://anaconda.org/conda-forge/local_migrator/badges/version.svg
   :target: https://anaconda.org/conda-forge/local_migrator
   :alt: Anaconda version
```

### Comparing `local_migrator-0.1.8/docs/Makefile` & `local-migrator-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/docs/conf.py` & `local-migrator-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/docs/examples.rst` & `local-migrator-0.1.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/docs/index.rst` & `local-migrator-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/docs/make.bat` & `local-migrator-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/pyproject.toml` & `local-migrator-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
-name = "local_migrator"
+name = "local-migrator"
 description = "Package for simplify data structures migrations"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "MIT"}
-keywords = ["napari", "migration", "persistance"]
+keywords = ["migration", "persistance"]
 authors = [
   {email = "g.bokota@uw.edu.pl"},
   {name = "Grzegorz Bokota"}
 ]
 maintainers = []
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -42,15 +42,15 @@
 ]
 
 [project.entry-points.pytest11]
 local_migrator = "local_migrator._testsupport"
 
 [project.urls]
 Homepage = "https://github.com/Czaki/local_migrator"
-Documentation = "https://local_migrator.readthedocs.io/en/latest/"
+Documentation = "https://local-migrator.readthedocs.io/en/latest/"
 Repository = "https://github.com/Czaki/local_migrator"
 
 [build-system]
 # Minimum requirements for the build system to execute.
 requires = ["setuptools>=61.0.0", "wheel>=0.37.0", "setuptools_scm[toml]>=6.4"]  # PEP 508 specifications.
 build-backend = "setuptools.build_meta"
```

### Comparing `local_migrator-0.1.8/src/local_migrator/__init__.py` & `local-migrator-0.1.9/src/local_migrator/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,34 @@
+from importlib import metadata
+
 from ._class_register import (
     REGISTER,
     MigrationInfo,
     MigrationRegistration,
     class_to_str,
     register_class,
     rename_key,
     update_argument,
 )
 from ._serialize_hooks import Encoder, check_for_errors_in_dkt_values, object_encoder, object_hook
 from .version import version as __version__
 
 try:
-    import nme
-except ImportError:
+    nme_version = metadata.version("nme")
+except metadata.PackageNotFoundError:
     pass
-else:
+else:  # pragma: no cover
     from packaging.version import parse
 
-    if parse(nme.__version__) <= parse("0.1.6"):
+    if parse(nme_version) <= parse("0.1.6"):
         raise ImportError("local_migrator is incompatible with nme<=0.1.6. You need to upgrade or uninstall nme.")
+    del parse
+    del nme_version
+
+del metadata
 
 
 def cbor_encoder(encoder, value):
     """
     Cbor encoder hook. Use :py:func:`nme_object_encoder` to encode objects.
 
     :param encoder: cbor2.Encoder
```

### Comparing `local_migrator-0.1.8/src/local_migrator/_class_register.py` & `local-migrator-0.1.9/src/local_migrator/_class_register.py`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/src/local_migrator/_serialize_hooks.py` & `local-migrator-0.1.9/src/local_migrator/_serialize_hooks.py`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/src/local_migrator.egg-info/PKG-INFO` & `local-migrator-0.1.9/src/local_migrator.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: local-migrator
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package for simplify data structures migrations
 Author: Grzegorz Bokota
 Author-email: g.bokota@uw.edu.pl
 License: MIT
 Project-URL: Homepage, https://github.com/Czaki/local_migrator
-Project-URL: Documentation, https://local_migrator.readthedocs.io/en/latest/
+Project-URL: Documentation, https://local-migrator.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/Czaki/local_migrator
-Keywords: napari,migration,persistance
+Keywords: migration,persistance
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -25,32 +25,32 @@
 Provides-Extra: cbor
 License-File: LICENSE.txt
 
 **************
 Local Migrator
 **************
 
-.. image:: https://codecov.io/gh/Czaki/local_migrator/branch/main/graph/badge.svg?token=KGEGEQYYRH
-  :target: https://codecov.io/gh/Czaki/local_migrator
+.. image:: https://codecov.io/gh/Czaki/local-migrator/branch/main/graph/badge.svg?token=KGEGEQYYRH
+  :target: https://codecov.io/gh/Czaki/local-migrator
   :alt: Codecov
 
-.. image:: https://github.com/Czaki/local_migrator/actions/workflows/tests.yml/badge.svg
-  :target: https://github.com/Czaki/local_migrator/actions/workflows/tests.yml
+.. image:: https://github.com/Czaki/local-migrator/actions/workflows/tests.yml/badge.svg
+  :target: https://github.com/Czaki/local-migrator/actions/workflows/tests.yml
   :alt: Test
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
   :target: https://github.com/psf/black
   :alt: Code Style
 
-.. image:: https://readthedocs.org/projects/local_migrator/badge/?version=latest
-  :target: https://local_migrator.readthedocs.io/en/latest/?badge=latest
+.. image:: https://readthedocs.org/projects/local-migrator/badge/?version=latest
+  :target: https://local-migrator.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status
 
-.. image:: https://badge.fury.io/py/local_migrator.svg
-  :target: https://badge.fury.io/py/local_migrator
+.. image:: https://badge.fury.io/py/local-migrator.svg
+  :target: https://badge.fury.io/py/local-migrator
   :alt: PyPI version
 
 .. image:: https://anaconda.org/conda-forge/local_migrator/badges/version.svg
   :target: https://anaconda.org/conda-forge/local_migrator
   :alt: Anaconda version
```

### Comparing `local_migrator-0.1.8/src/local_migrator.egg-info/SOURCES.txt` & `local-migrator-0.1.9/src/local_migrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/src/tests/test_cbor_hooks.py` & `local-migrator-0.1.9/src/tests/test_cbor_hooks.py`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/src/tests/test_class_register.py` & `local-migrator-0.1.9/src/tests/test_class_register.py`

 * *Files identical despite different names*

### Comparing `local_migrator-0.1.8/src/tests/test_json_hooks.py` & `local-migrator-0.1.9/src/tests/test_json_hooks.py`

 * *Files identical despite different names*

