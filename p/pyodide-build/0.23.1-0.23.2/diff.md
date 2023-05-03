# Comparing `tmp/pyodide-build-0.23.1.tar.gz` & `tmp/pyodide-build-0.23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide-build-0.23.1.tar", last modified: Fri Apr 14 22:15:34 2023, max compression
+gzip compressed data, was "pyodide-build-0.23.2.tar", last modified: Wed May  3 06:08:44 2023, max compression
```

## Comparing `pyodide-build-0.23.1.tar` & `pyodide-build-0.23.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.221459 pyodide-build-0.23.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-14 22:15:34.221459 pyodide-build-0.23.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.217459 pyodide-build-0.23.1/pyodide_build/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1408 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/_f2c_fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/_py_compile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27665 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/buildall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31327 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/buildpkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.217459 pyodide-build-0.23.1/pyodide_build/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/build_recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/create_zipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/py_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/skeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/cli/xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/create_pypa_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/create_xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/install_xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8595 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/mkpkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.217459 pyodide-build-0.23.1/pyodide_build/out_of_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/out_of_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/out_of_tree/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/out_of_tree/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/out_of_tree/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/out_of_tree/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/pypabuild.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20853 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/pywasmcross.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/pyzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.217459 pyodide-build-0.23.1/pyodide_build/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.213459 pyodide-build-0.23.1/pyodide_build/tools/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.213459 pyodide-build-0.23.1/pyodide_build/tools/cmake/Modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.217459 pyodide-build-0.23.1/pyodide_build/tools/cmake/Modules/Platform/
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyodide_build/tools/pyo3_config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:15:34.221459 pyodide-build-0.23.1/pyodide_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-14 22:15:34.000000 pyodide-build-0.23.1/pyodide_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-14 22:15:34.000000 pyodide-build-0.23.1/pyodide_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 22:15:34.000000 pyodide-build-0.23.1/pyodide_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-14 22:15:34.000000 pyodide-build-0.23.1/pyodide_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-14 22:15:34.000000 pyodide-build-0.23.1/pyodide_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 22:15:34.000000 pyodide-build-0.23.1/pyodide_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-14 22:15:34.221459 pyodide-build-0.23.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-14 22:15:20.000000 pyodide-build-0.23.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/pyodide_build/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1408 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/_f2c_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/_py_compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27665 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/buildall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31135 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/buildpkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/pyodide_build/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/build_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/create_zipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/py_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/xbuildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/create_pypa_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/create_xbuildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/install_xbuildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8595 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/mkpkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/pyodide_build/out_of_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/out_of_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/out_of_tree/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/out_of_tree/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/out_of_tree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/out_of_tree/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/pypabuild.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20853 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/pywasmcross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/pyzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/pyodide_build/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.731597 pyodide-build-0.23.2/pyodide_build/tools/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.731597 pyodide-build-0.23.2/pyodide_build/tools/cmake/Modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/pyodide_build/tools/cmake/Modules/Platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/tools/pyo3_config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/pyodide_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-03 06:08:44.000000 pyodide-build-0.23.2/pyodide_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-03 06:08:44.000000 pyodide-build-0.23.2/pyodide_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:08:44.000000 pyodide-build-0.23.2/pyodide_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-03 06:08:44.000000 pyodide-build-0.23.2/pyodide_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-03 06:08:44.000000 pyodide-build-0.23.2/pyodide_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 06:08:44.000000 pyodide-build-0.23.2/pyodide_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-03 06:08:44.743598 pyodide-build-0.23.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/setup.py
```

### Comparing `pyodide-build-0.23.1/LICENSE` & `pyodide-build-0.23.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/PKG-INFO` & `pyodide-build-0.23.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-build
-Version: 0.23.1
+Version: 0.23.2
 Summary: "Tools for building Pyodide"
 Home-page: https://github.com/pyodide/pyodide
 Author: Pyodide developers
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyodide-build-0.23.1/pyodide_build/__main__.py` & `pyodide-build-0.23.2/pyodide_build/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/_f2c_fixes.py` & `pyodide-build-0.23.2/pyodide_build/_f2c_fixes.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/_py_compile.py` & `pyodide-build-0.23.2/pyodide_build/_py_compile.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/buildall.py` & `pyodide-build-0.23.2/pyodide_build/buildall.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/buildpkg.py` & `pyodide-build-0.23.2/pyodide_build/buildpkg.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,21 +422,15 @@
             with BashRunnerWithSharedEnvironment(build_env) as runner:
                 runner.run(build_metadata.cross_script, cwd=srcpath)
                 build_env = runner.env
 
         from .pypabuild import build
 
         outpath = srcpath / "dist"
-        try:
-            build(srcpath, outpath, build_env, backend_flags)
-        except BaseException:
-            build_log_path = Path("build.log")
-            if build_log_path.exists():
-                build_log_path.unlink()
-            raise
+        build(srcpath, outpath, build_env, backend_flags)
 
 
 def replace_so_abi_tags(wheel_dir: Path) -> None:
     """Replace native abi tag with emscripten abi tag in .so file names"""
     build_soabi = sysconfig.get_config_var("SOABI")
     assert build_soabi
     ext_suffix = sysconfig.get_config_var("EXT_SUFFIX")
```

### Comparing `pyodide-build-0.23.1/pyodide_build/cli/build.py` & `pyodide-build-0.23.2/pyodide_build/cli/build.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import shutil
+import sys
 import tempfile
 from pathlib import Path
 from typing import Optional
 from urllib.parse import urlparse
 
 import requests
 import typer
@@ -109,17 +110,20 @@
 # simple 'pyodide build' command
 def main(
     source_location: "Optional[str]" = typer.Argument(
         "",
         help="Build source, can be source folder, pypi version specification, or url to a source dist archive or wheel file. If this is blank, it will build the current directory.",
     ),
     output_directory: str = typer.Option(
-        "./dist",
+        "",
+        "--outdir",
+        "-o",
         help="which directory should the output be placed into?",
     ),
+    output_directory_compat: str = typer.Option("", "--output-directory", hidden=True),
     requirements_txt: str = typer.Option(
         "",
         "--requirements",
         "-r",
         help="Build a list of package requirements from a requirements.txt file",
     ),
     exports: str = typer.Option(
@@ -139,14 +143,24 @@
     ),
     compression_level: int = typer.Option(
         6, help="Compression level to use for the created zip file"
     ),
     ctx: typer.Context = typer.Context,
 ) -> None:
     """Use pypa/build to build a Python package from source, pypi or url."""
+    if output_directory_compat:
+        print(
+            "--output-directory is deprecated, use --outdir or -o instead",
+            file=sys.stderr,
+        )
+    if output_directory_compat and output_directory:
+        print("Cannot provide both --outdir and --output-directory", file=sys.stderr)
+        sys.exit(1)
+    output_directory = output_directory_compat or output_directory or "./dist"
+
     outpath = Path(output_directory).resolve()
     outpath.mkdir(exist_ok=True)
     extras: list[str] = []
 
     if len(requirements_txt) > 0:
         # a requirements.txt - build it (and optionally deps)
         if not Path(requirements_txt).exists():
```

### Comparing `pyodide-build-0.23.1/pyodide_build/cli/build_recipes.py` & `pyodide-build-0.23.2/pyodide_build/cli/build_recipes.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/cli/config.py` & `pyodide-build-0.23.2/pyodide_build/cli/config.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/cli/create_zipfile.py` & `pyodide-build-0.23.2/pyodide_build/cli/create_zipfile.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/cli/py_compile.py` & `pyodide-build-0.23.2/pyodide_build/cli/py_compile.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/cli/skeleton.py` & `pyodide-build-0.23.2/pyodide_build/cli/skeleton.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/cli/xbuildenv.py` & `pyodide-build-0.23.2/pyodide_build/cli/xbuildenv.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/common.py` & `pyodide-build-0.23.2/pyodide_build/common.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/create_pypa_index.py` & `pyodide-build-0.23.2/pyodide_build/create_pypa_index.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/create_xbuildenv.py` & `pyodide-build-0.23.2/pyodide_build/create_xbuildenv.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/install_xbuildenv.py` & `pyodide-build-0.23.2/pyodide_build/install_xbuildenv.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/io.py` & `pyodide-build-0.23.2/pyodide_build/io.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/logger.py` & `pyodide-build-0.23.2/pyodide_build/logger.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/mkpkg.py` & `pyodide-build-0.23.2/pyodide_build/mkpkg.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/out_of_tree/build.py` & `pyodide-build-0.23.2/pyodide_build/out_of_tree/build.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/out_of_tree/pypi.py` & `pyodide-build-0.23.2/pyodide_build/out_of_tree/pypi.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/out_of_tree/utils.py` & `pyodide-build-0.23.2/pyodide_build/out_of_tree/utils.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/out_of_tree/venv.py` & `pyodide-build-0.23.2/pyodide_build/out_of_tree/venv.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/pypabuild.py` & `pyodide-build-0.23.2/pyodide_build/pypabuild.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/pywasmcross.py` & `pyodide-build-0.23.2/pyodide_build/pywasmcross.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/pyzip.py` & `pyodide-build-0.23.2/pyodide_build/pyzip.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/recipe.py` & `pyodide-build-0.23.2/pyodide_build/recipe.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/serve.py` & `pyodide-build-0.23.2/pyodide_build/serve.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake` & `pyodide-build-0.23.2/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/pyodide_build.egg-info/PKG-INFO` & `pyodide-build-0.23.2/pyodide_build.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-build
-Version: 0.23.1
+Version: 0.23.2
 Summary: "Tools for building Pyodide"
 Home-page: https://github.com/pyodide/pyodide
 Author: Pyodide developers
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyodide-build-0.23.1/pyodide_build.egg-info/SOURCES.txt` & `pyodide-build-0.23.2/pyodide_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.1/setup.cfg` & `pyodide-build-0.23.2/setup.cfg`

 * *Files identical despite different names*

