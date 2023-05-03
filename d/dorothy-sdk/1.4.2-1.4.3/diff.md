# Comparing `tmp/dorothy-sdk-1.4.2.tar.gz` & `tmp/dorothy-sdk-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorothy-sdk-1.4.2.tar", last modified: Tue Apr 25 02:19:00 2023, max compression
+gzip compressed data, was "dorothy-sdk-1.4.3.tar", last modified: Wed May  3 01:47:35 2023, max compression
```

## Comparing `dorothy-sdk-1.4.2.tar` & `dorothy-sdk-1.4.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:19:00.474599 dorothy-sdk-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-25 02:19:00.470599 dorothy-sdk-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:19:00.470599 dorothy-sdk-1.4.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6058 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/bin/model_run
--rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/bin/model_train
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:19:00.466599 dorothy-sdk-1.4.2/dorothy_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:19:00.470599 dorothy-sdk-1.4.2/dorothy_sdk/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/resources/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/resources/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/resources/folds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/resources/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/resources/quality_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/dorothy_sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:19:00.470599 dorothy-sdk-1.4.2/dorothy_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-25 02:19:00.000000 dorothy-sdk-1.4.2/dorothy_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-25 02:19:00.000000 dorothy-sdk-1.4.2/dorothy_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 02:19:00.000000 dorothy-sdk-1.4.2/dorothy_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-25 02:19:00.000000 dorothy-sdk-1.4.2/dorothy_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 02:19:00.000000 dorothy-sdk-1.4.2/dorothy_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 02:19:00.474599 dorothy-sdk-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-25 02:18:47.000000 dorothy-sdk-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6058 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/bin/model_run
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/bin/model_train
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/dorothy_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/dorothy_sdk/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/resources/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/resources/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/resources/folds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/resources/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/resources/quality_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/dorothy_sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/dorothy_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-03 01:47:35.000000 dorothy-sdk-1.4.3/dorothy_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-03 01:47:35.000000 dorothy-sdk-1.4.3/dorothy_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 01:47:35.000000 dorothy-sdk-1.4.3/dorothy_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 01:47:35.000000 dorothy-sdk-1.4.3/dorothy_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 01:47:35.000000 dorothy-sdk-1.4.3/dorothy_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 01:47:35.400338 dorothy-sdk-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-03 01:47:25.000000 dorothy-sdk-1.4.3/setup.py
```

### Comparing `dorothy-sdk-1.4.2/PKG-INFO` & `dorothy-sdk-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorothy-sdk
-Version: 1.4.2
+Version: 1.4.3
 Summary: UNKNOWN
 Home-page: https://github.com/tb-brics/dorothy-sdk
 Author: Patrick Braz
 Author-email: patrickfbraz@poli.ufrj.br
 Maintainer: Patrick Braz
 Maintainer-email: patrickfbraz@poli.ufrj.br
 License: UNKNOWN
```

### Comparing `dorothy-sdk-1.4.2/README.rst` & `dorothy-sdk-1.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/bin/model_run` & `dorothy-sdk-1.4.3/bin/model_run`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/bin/model_train` & `dorothy-sdk-1.4.3/bin/model_train`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/dorothy_sdk/core.py` & `dorothy-sdk-1.4.3/dorothy_sdk/core.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/dorothy_sdk/dataset_wrapper.py` & `dorothy-sdk-1.4.3/dorothy_sdk/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/dorothy_sdk/git_repo.py` & `dorothy-sdk-1.4.3/dorothy_sdk/git_repo.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/dorothy_sdk/mlflow.py` & `dorothy-sdk-1.4.3/dorothy_sdk/mlflow.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/dorothy_sdk/operation.py` & `dorothy-sdk-1.4.3/dorothy_sdk/operation.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/dorothy_sdk/resources/dataset.py` & `dorothy-sdk-1.4.3/dorothy_sdk/resources/dataset.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/dorothy_sdk/resources/folders.py` & `dorothy-sdk-1.4.3/dorothy_sdk/resources/folders.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/dorothy_sdk/resources/folds.py` & `dorothy-sdk-1.4.3/dorothy_sdk/resources/folds.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/dorothy_sdk/resources/image.py` & `dorothy-sdk-1.4.3/dorothy_sdk/resources/image.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/dorothy_sdk/resources/quality_annotation.py` & `dorothy-sdk-1.4.3/dorothy_sdk/resources/quality_annotation.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/dorothy_sdk/session.py` & `dorothy-sdk-1.4.3/dorothy_sdk/session.py`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/dorothy_sdk.egg-info/PKG-INFO` & `dorothy-sdk-1.4.3/dorothy_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorothy-sdk
-Version: 1.4.2
+Version: 1.4.3
 Summary: UNKNOWN
 Home-page: https://github.com/tb-brics/dorothy-sdk
 Author: Patrick Braz
 Author-email: patrickfbraz@poli.ufrj.br
 Maintainer: Patrick Braz
 Maintainer-email: patrickfbraz@poli.ufrj.br
 License: UNKNOWN
```

### Comparing `dorothy-sdk-1.4.2/dorothy_sdk.egg-info/SOURCES.txt` & `dorothy-sdk-1.4.3/dorothy_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dorothy-sdk-1.4.2/setup.py` & `dorothy-sdk-1.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import platform
 from os.path import join, abspath, dirname
 from setuptools import find_packages, setup
 
 
 def get_version() -> str:
     """Get the package version
@@ -30,20 +29,20 @@
 PACKAGE_DESCRIPTION = ""
 PACKAGE_DOWNLOAD_URL = None
 PACKAGE_AUTHOR = "Patrick Braz"
 PACKAGE_AUTHOR_EMAIL = "patrickfbraz@poli.ufrj.br"
 PACKAGE_MAINTAINER = "Patrick Braz"
 PACKAGE_EMAIL = "patrickfbraz@poli.ufrj.br"
 INSTALL_REQUIRES = {
-    "requests-cache==0.9.5",
+    "requests-cache==1.0.1",
     "GitPython==3.1.29",
     "py-cpuinfo==9.0.0",
     "nvsmi==0.4.2",
-    "psutil==5.8.0",
-    "Pillow==9.2.0",
+    "psutil==5.9.5",
+    "Pillow==9.5.0",
 }
 
 setup(
     name=PACKAGE_NAME,
     url="https://github.com/tb-brics/dorothy-sdk",
     description=PACKAGE_DESCRIPTION,
     long_description=long_description,
```

