# Comparing `tmp/roboflow-1.0.5.tar.gz` & `tmp/roboflow-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboflow-1.0.5.tar", last modified: Fri Apr 14 18:46:32 2023, max compression
+gzip compressed data, was "roboflow-1.0.8.tar", last modified: Wed May  3 20:11:24 2023, max compression
```

## Comparing `roboflow-1.0.5.tar` & `roboflow-1.0.8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.691317 roboflow-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-04-14 18:46:10.000000 roboflow-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-14 18:46:32.691317 roboflow-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-04-14 18:46:10.000000 roboflow-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 18:46:10.000000 roboflow-1.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/roboflow/
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/roboflow/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/archive/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/roboflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    22648 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/core/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/core/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/roboflow/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/models/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/models/instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/models/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/models/semantic_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/roboflow/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/active_learning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/clip_compare_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/two_stage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-14 18:46:10.000000 roboflow-1.0.5/roboflow/util/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/roboflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-14 18:46:32.000000 roboflow-1.0.5/roboflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-14 18:46:32.000000 roboflow-1.0.5/roboflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:46:32.000000 roboflow-1.0.5/roboflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-14 18:46:32.000000 roboflow-1.0.5/roboflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 18:46:32.000000 roboflow-1.0.5/roboflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:46:32.691317 roboflow-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-14 18:46:10.000000 roboflow-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.687317 roboflow-1.0.5/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/models/test_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/models/test_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/models/test_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.691317 roboflow-1.0.5/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:46:32.691317 roboflow-1.0.5/tests/util/dummy_module/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/util/dummy_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/util/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-14 18:46:10.000000 roboflow-1.0.5/tests/util/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-05-03 20:10:55.000000 roboflow-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-03 20:11:24.586639 roboflow-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-05-03 20:10:55.000000 roboflow-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 20:10:55.000000 roboflow-1.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.582639 roboflow-1.0.8/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.582639 roboflow-1.0.8/roboflow/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/archive/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.582639 roboflow-1.0.8/roboflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23091 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/core/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27896 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/core/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/roboflow/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/models/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/models/instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/models/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/models/semantic_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/roboflow/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/active_learning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/clip_compare_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/two_stage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-03 20:10:55.000000 roboflow-1.0.8/roboflow/util/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.582639 roboflow-1.0.8/roboflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-05-03 20:11:24.000000 roboflow-1.0.8/roboflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-03 20:11:24.000000 roboflow-1.0.8/roboflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:11:24.000000 roboflow-1.0.8/roboflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 20:11:24.000000 roboflow-1.0.8/roboflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 20:11:24.000000 roboflow-1.0.8/roboflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:11:24.586639 roboflow-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-03 20:10:55.000000 roboflow-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/models/test_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/models/test_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/models/test_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:11:24.586639 roboflow-1.0.8/tests/util/dummy_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/util/dummy_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/util/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-03 20:10:55.000000 roboflow-1.0.8/tests/util/test_versions.py
```

### Comparing `roboflow-1.0.5/LICENSE` & `roboflow-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/PKG-INFO` & `roboflow-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.0.5
+Version: 1.0.8
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.0.5 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.0.8 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.0.5/README.md` & `roboflow-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow/__init__.py` & `roboflow-1.0.8/roboflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests
 
 from roboflow.config import API_URL, APP_URL, DEMO_KEYS, load_roboflow_api_key
 from roboflow.core.project import Project
 from roboflow.core.workspace import Workspace
 from roboflow.util.general import write_line
 
-__version__ = "1.0.5"
+__version__ = "1.0.8"
 
 
 def check_key(api_key, model, notebook, num_retries=0):
     if type(api_key) is not str:
         raise RuntimeError(
             "API Key is of Incorrect Type \n Expected Type: "
             + str(type(""))
```

### Comparing `roboflow-1.0.5/roboflow/archive/plot.py` & `roboflow-1.0.8/roboflow/archive/plot.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow/config.py` & `roboflow-1.0.8/roboflow/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 INSTANCE_SEGMENTATION_URL = get_conditional_configuration_variable(
     "INSTANCE_SEGMENTATION_URL", "https://outline.roboflow.com"
 )
 SEMANTIC_SEGMENTATION_URL = get_conditional_configuration_variable(
     "SEMANTIC_SEGMENTATION_URL", "https://segment.roboflow.com"
 )
 OBJECT_DETECTION_URL = get_conditional_configuration_variable(
-    "SEMANTIC_SEGMENTATION_URL", "https://detect.roboflow.com"
+    "OBJECT_DETECTION_URL", "https://detect.roboflow.com"
 )
 
 CLIP_FEATURIZE_URL = get_conditional_configuration_variable(
     "CLIP_FEATURIZE_URL", "CLIP FEATURIZE URL NOT IN ENV"
 )
 OCR_URL = get_conditional_configuration_variable("OCR_URL", "OCR URL NOT IN ENV")
```

### Comparing `roboflow-1.0.5/roboflow/core/project.py` & `roboflow-1.0.8/roboflow/core/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -342,15 +342,17 @@
             )
             # Get response
             response = requests.post(upload_url)
         # Return response
 
         return response
 
-    def __annotation_upload(self, annotation_path: str, image_id: str):
+    def __annotation_upload(
+        self, annotation_path: str, image_id: str, is_prediction: bool = False
+    ):
         """function to upload annotation to the specific project
         :param annotation_path: path to annotation you'd like to upload
         :param image_id: image id you'd like to upload that has annotations for it.
         """
 
         # stop on empty string
         if len(annotation_path) == 0:
@@ -385,14 +387,15 @@
                 API_URL + "/dataset/",
                 self.__project_name,
                 "/annotate/",
                 image_id,
                 "?api_key=",
                 self.__api_key,
                 "&name=" + os.path.basename(annotation_path),
+                "&is_prediction=true" if is_prediction else "",
             ]
         )
 
         # Get annotation response
         annotation_response = requests.post(
             self.annotation_upload_url,
             data=annotation_string,
@@ -418,27 +421,29 @@
         annotation_path: str = None,
         hosted_image: bool = False,
         image_id: int = None,
         split: str = "train",
         num_retry_uploads: int = 0,
         batch_name: str = DEFAULT_BATCH_NAME,
         tag_names: list = [],
+        is_prediction: bool = False,
         **kwargs,
     ):
         """Upload image function based on the RESTful API
 
         Args:
             image_path (str) - path to image you'd like to upload
             annotation_path (str) - if you're upload annotation, path to it
             hosted_image (bool) - whether the image is hosted
             image_id (int) - id of the image
             split (str) - to upload the image to
             num_retry_uploads (int) - how many times to retry upload on failure
             batch_name (str) - name of batch to upload to within project
             tag_names (list[str]) - tags to be applied to an image
+            is_prediction (bool) - whether the annotation data is a prediction rather than ground truth
 
         Returns:
             None - returns nothing
         """
 
         is_hosted = image_path.startswith("http://") or image_path.startswith(
             "https://"
@@ -469,30 +474,33 @@
                 annotation_path=annotation_path,
                 hosted_image=hosted_image,
                 image_id=image_id,
                 split=split,
                 num_retry_uploads=num_retry_uploads,
                 batch_name=batch_name,
                 tag_names=tag_names,
+                is_prediction=is_prediction,
                 **kwargs,
             )
+
         else:
             images = os.listdir(image_path)
             for image in images:
                 path = image_path + "/" + image
                 if self.check_valid_image(image):
                     self.single_upload(
                         image_path=path,
                         annotation_path=annotation_path,
                         hosted_image=hosted_image,
                         image_id=image_id,
                         split=split,
                         num_retry_uploads=num_retry_uploads,
                         batch_name=batch_name,
                         tag_names=tag_names,
+                        is_prediction=is_prediction,
                         **kwargs,
                     )
                     print("[ " + path + " ] was uploaded succesfully.")
                 else:
                     print("[ " + path + " ] was skipped.")
                     continue
 
@@ -502,14 +510,15 @@
         annotation_path=None,
         hosted_image=False,
         image_id=None,
         split="train",
         num_retry_uploads=0,
         batch_name=DEFAULT_BATCH_NAME,
         tag_names=[],
+        is_prediction: bool = False,
         **kwargs,
     ):
         success = False
         annotation_success = False
         # User gives image path
         if image_path is not None:
             # Upload Image Response
@@ -568,15 +577,17 @@
                         + image_path
                         + ", failed to upload! You can specify num_retry_uploads to retry a number of times."
                     )
 
         # Upload only annotations to image based on image Id (no image)
         if annotation_path is not None and image_id is not None and success:
             # Get annotation upload response
-            annotation_response = self.__annotation_upload(annotation_path, image_id)
+            annotation_response = self.__annotation_upload(
+                annotation_path, image_id, is_prediction=is_prediction
+            )
             # Check if upload was a success
             try:
                 response_data = annotation_response.json()
                 if "success" in response_data.keys():
                     annotation_success = True
                 elif "error" in response_data.keys():
                     warnings.warn(
```

### Comparing `roboflow-1.0.5/roboflow/core/version.py` & `roboflow-1.0.8/roboflow/core/version.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow/core/workspace.py` & `roboflow-1.0.8/roboflow/core/workspace.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow/models/classification.py` & `roboflow-1.0.8/roboflow/models/classification.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow/models/inference.py` & `roboflow-1.0.8/roboflow/models/inference.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow/models/instance_segmentation.py` & `roboflow-1.0.8/roboflow/models/instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow/models/object_detection.py` & `roboflow-1.0.8/roboflow/models/object_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import requests
 import wget
 from PIL import Image
 
-from roboflow.config import API_URL, OBJECT_DETECTION_MODEL
+from roboflow.config import API_URL, OBJECT_DETECTION_MODEL, OBJECT_DETECTION_URL
 from roboflow.util.image_utils import check_image_url
 from roboflow.util.prediction import PredictionGroup
 from roboflow.util.versions import (
     print_warn_for_wrong_dependencies_versions,
     warn_for_wrong_dependencies_versions,
 )
 
@@ -76,15 +76,15 @@
         self.labels = labels
         self.format = format
         self.colors = {} if colors is None else colors
         self.preprocessing = {} if preprocessing is None else preprocessing
 
         # local needs to be passed from Project
         if local is None:
-            self.base_url = "https://detect.roboflow.com/"
+            self.base_url = OBJECT_DETECTION_URL + "/"
         else:
             print("initalizing local object detection model hosted at :" + local)
             self.base_url = local
 
         # If dataset slug not none, instantiate API URL
         if name is not None and version is not None:
             self.__generate_url()
@@ -511,15 +511,15 @@
         labels=None,
         format=None,
         inference_engine_url=None,
     ):
         # Reassign parameters if any parameters are changed
         if local is not None:
             if not local:
-                self.base_url = "https://detect.roboflow.com/"
+                self.base_url = OBJECT_DETECTION_URL + "/"
             else:
                 self.base_url = "http://localhost:9001/"
 
         if inference_engine_url is not None:
             self.base_url = inference_engine_url
 
         # Change any variables that the user wants to change
```

### Comparing `roboflow-1.0.5/roboflow/models/semantic_segmentation.py` & `roboflow-1.0.8/roboflow/models/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow/util/active_learning_utils.py` & `roboflow-1.0.8/roboflow/util/active_learning_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow/util/clip_compare_utils.py` & `roboflow-1.0.8/roboflow/util/clip_compare_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow/util/image_utils.py` & `roboflow-1.0.8/roboflow/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow/util/prediction.py` & `roboflow-1.0.8/roboflow/util/prediction.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow/util/two_stage_utils.py` & `roboflow-1.0.8/roboflow/util/two_stage_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow/util/versions.py` & `roboflow-1.0.8/roboflow/util/versions.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/roboflow.egg-info/PKG-INFO` & `roboflow-1.0.8/roboflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.0.5
+Version: 1.0.8
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.0.5 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.0.8 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.0.5/roboflow.egg-info/SOURCES.txt` & `roboflow-1.0.8/roboflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/setup.py` & `roboflow-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/tests/models/test_instance_segmentation.py` & `roboflow-1.0.8/tests/models/test_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/tests/models/test_object_detection.py` & `roboflow-1.0.8/tests/models/test_object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/tests/models/test_semantic_segmentation.py` & `roboflow-1.0.8/tests/models/test_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/tests/test_project.py` & `roboflow-1.0.8/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/tests/test_queries.py` & `roboflow-1.0.8/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/tests/test_version.py` & `roboflow-1.0.8/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/tests/util/test_image_utils.py` & `roboflow-1.0.8/tests/util/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.0.5/tests/util/test_versions.py` & `roboflow-1.0.8/tests/util/test_versions.py`

 * *Files identical despite different names*

