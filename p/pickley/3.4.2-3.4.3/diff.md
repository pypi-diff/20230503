# Comparing `tmp/pickley-3.4.2.tar.gz` & `tmp/pickley-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickley-3.4.2.tar", last modified: Wed May  3 18:07:31 2023, max compression
+gzip compressed data, was "pickley-3.4.3.tar", last modified: Wed May  3 18:49:49 2023, max compression
```

## Comparing `pickley-3.4.2.tar` & `pickley-3.4.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:07:31.444079 pickley-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 18:05:33.000000 pickley-3.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 18:05:33.000000 pickley-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-03 18:07:31.444079 pickley-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-03 18:05:33.000000 pickley-3.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-03 18:05:33.000000 pickley-3.4.2/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 18:05:33.000000 pickley-3.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 18:07:31.444079 pickley-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-03 18:05:33.000000 pickley-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:07:31.440079 pickley-3.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:07:31.444079 pickley-3.4.2/src/pickley/
--rw-r--r--   0 runner    (1001) docker     (123)    36403 2023-05-03 18:05:33.000000 pickley-3.4.2/src/pickley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-03 18:05:33.000000 pickley-3.4.2/src/pickley/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-05-03 18:05:33.000000 pickley-3.4.2/src/pickley/bstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    30237 2023-05-03 18:05:33.000000 pickley-3.4.2/src/pickley/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-03 18:05:33.000000 pickley-3.4.2/src/pickley/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-03 18:05:33.000000 pickley-3.4.2/src/pickley/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:07:31.444079 pickley-3.4.2/src/pickley.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-03 18:07:31.000000 pickley-3.4.2/src/pickley.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-03 18:07:31.000000 pickley-3.4.2/src/pickley.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:07:31.000000 pickley-3.4.2/src/pickley.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 18:07:31.000000 pickley-3.4.2/src/pickley.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-03 18:07:31.000000 pickley-3.4.2/src/pickley.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 18:07:31.000000 pickley-3.4.2/src/pickley.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:07:31.444079 pickley-3.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-03 18:05:33.000000 pickley-3.4.2/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-03 18:05:33.000000 pickley-3.4.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-03 18:05:33.000000 pickley-3.4.2/tests/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-05-03 18:05:33.000000 pickley-3.4.2/tests/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-03 18:05:33.000000 pickley-3.4.2/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-03 18:05:33.000000 pickley-3.4.2/tests/test_venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:49:49.117702 pickley-3.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 18:48:04.000000 pickley-3.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 18:48:04.000000 pickley-3.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-03 18:49:49.117702 pickley-3.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-03 18:48:04.000000 pickley-3.4.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-03 18:48:04.000000 pickley-3.4.3/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 18:48:04.000000 pickley-3.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 18:49:49.117702 pickley-3.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-03 18:48:04.000000 pickley-3.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:49:49.113702 pickley-3.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:49:49.113702 pickley-3.4.3/src/pickley/
+-rw-r--r--   0 runner    (1001) docker     (123)    36403 2023-05-03 18:48:04.000000 pickley-3.4.3/src/pickley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-03 18:48:04.000000 pickley-3.4.3/src/pickley/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-05-03 18:48:04.000000 pickley-3.4.3/src/pickley/bstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30237 2023-05-03 18:48:04.000000 pickley-3.4.3/src/pickley/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-03 18:48:04.000000 pickley-3.4.3/src/pickley/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-03 18:48:04.000000 pickley-3.4.3/src/pickley/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:49:49.117702 pickley-3.4.3/src/pickley.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-03 18:49:49.000000 pickley-3.4.3/src/pickley.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-03 18:49:49.000000 pickley-3.4.3/src/pickley.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:49:49.000000 pickley-3.4.3/src/pickley.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 18:49:49.000000 pickley-3.4.3/src/pickley.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-03 18:49:49.000000 pickley-3.4.3/src/pickley.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 18:49:49.000000 pickley-3.4.3/src/pickley.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:49:49.117702 pickley-3.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-03 18:48:04.000000 pickley-3.4.3/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-03 18:48:04.000000 pickley-3.4.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-03 18:48:04.000000 pickley-3.4.3/tests/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-05-03 18:48:04.000000 pickley-3.4.3/tests/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-03 18:48:04.000000 pickley-3.4.3/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-03 18:48:04.000000 pickley-3.4.3/tests/test_venv.py
```

### Comparing `pickley-3.4.2/LICENSE` & `pickley-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pickley-3.4.2/PKG-INFO` & `pickley-3.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.4.2
+Version: 3.4.3
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
```

### Comparing `pickley-3.4.2/README.rst` & `pickley-3.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `pickley-3.4.2/setup.py` & `pickley-3.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.2/src/pickley/__init__.py` & `pickley-3.4.3/src/pickley/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 from datetime import datetime
 
 import runez
 from runez.pyenv import PypiStd, PythonDepot, PythonInstallationScanner, Version
 
 
-__version__ = "3.4.2"
+__version__ = "3.4.3"
 LOG = logging.getLogger(__name__)
 PICKLEY = "pickley"
 DOT_META = ".pickley"
 K_CLI = {"delivery", "index", "python"}
 K_DIRECTIVES = {"include"}
 K_GROUPS = {"bundle", "pinned"}
 K_LEAVES = {
```

### Comparing `pickley-3.4.2/src/pickley/bstrap.py` & `pickley-3.4.3/src/pickley/bstrap.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.2/src/pickley/cli.py` & `pickley-3.4.3/src/pickley/cli.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.2/src/pickley/delivery.py` & `pickley-3.4.3/src/pickley/delivery.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.2/src/pickley/package.py` & `pickley-3.4.3/src/pickley/package.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.2/src/pickley.egg-info/PKG-INFO` & `pickley-3.4.3/src/pickley.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.4.2
+Version: 3.4.3
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
```

### Comparing `pickley-3.4.2/src/pickley.egg-info/SOURCES.txt` & `pickley-3.4.3/src/pickley.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pickley-3.4.2/tests/test_bootstrap.py` & `pickley-3.4.3/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.2/tests/test_config.py` & `pickley-3.4.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.2/tests/test_delivery.py` & `pickley-3.4.3/tests/test_delivery.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.2/tests/test_ops.py` & `pickley-3.4.3/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.2/tests/test_run.py` & `pickley-3.4.3/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.2/tests/test_venv.py` & `pickley-3.4.3/tests/test_venv.py`

 * *Files identical despite different names*

