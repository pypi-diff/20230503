# Comparing `tmp/microns-utils-0.1.5.tar.gz` & `tmp/microns-utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/stelios/Documents/PyPI/microns-utils/dist/tmpomis0y1b/microns-utils-0.1.5.tar", last modified: Tue Oct  4 16:41:38 2022, max compression
+gzip compressed data, was "/home/stelios/Documents/PyPI/microns-utils/dist/tmp1h6ag7xy/microns-utils-0.1.7.tar", last modified: Wed May  3 15:58:58 2023, max compression
```

## Comparing `microns-utils-0.1.5.tar` & `microns-utils-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-04 16:41:38.000000 microns-utils-0.1.5/
--rw-rw-r--   0 root         (0) root         (0)       59 2022-05-16 07:20:39.000000 microns-utils-0.1.5/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-04 16:41:38.000000 microns-utils-0.1.5/microns_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      275 2022-10-04 16:41:38.000000 microns-utils-0.1.5/microns_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      105 2022-10-04 16:41:38.000000 microns-utils-0.1.5/microns_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-10-04 16:41:38.000000 microns-utils-0.1.5/microns_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-04 16:41:38.000000 microns-utils-0.1.5/microns_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      703 2022-10-04 16:41:38.000000 microns-utils-0.1.5/microns_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      275 2022-10-04 16:41:38.000000 microns-utils-0.1.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    26526 2022-05-16 07:18:26.000000 microns-utils-0.1.5/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      105 2022-08-31 14:10:29.000000 microns-utils-0.1.5/requirements.txt
--rw-rw-r--   0 root         (0) root         (0)      593 2022-05-16 07:10:32.000000 microns-utils-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-04 16:41:38.000000 microns-utils-0.1.5/microns_utils/
--rw-rw-r--   0 root         (0) root         (0)       60 2022-06-07 16:05:32.000000 microns-utils-0.1.5/microns_utils/misc_utils.py
--rw-rw-r--   0 root         (0) root         (0)      472 2022-05-16 07:10:32.000000 microns-utils-0.1.5/microns_utils/errors.py
--rw-rw-r--   0 root         (0) root         (0)     9509 2022-08-31 14:10:29.000000 microns-utils-0.1.5/microns_utils/model_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1060 2022-05-16 07:10:32.000000 microns-utils-0.1.5/microns_utils/mesh_utils.py
--rw-rw-r--   0 root         (0) root         (0)    26798 2022-08-31 14:10:29.000000 microns-utils-0.1.5/microns_utils/widget_utils.py
--rw-rw-r--   0 root         (0) root         (0)      177 2022-05-16 07:10:32.000000 microns-utils-0.1.5/microns_utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9627 2022-10-04 16:41:22.000000 microns-utils-0.1.5/microns_utils/datajoint_utils.py
--rw-rw-r--   0 root         (0) root         (0)     5513 2022-10-04 16:41:22.000000 microns-utils-0.1.5/microns_utils/ap_utils.py
--rw-rw-r--   0 root         (0) root         (0)      323 2022-06-07 16:05:32.000000 microns-utils-0.1.5/microns_utils/transform_utils.py
--rw-rw-r--   0 root         (0) root         (0)     2213 2022-05-19 11:29:51.000000 microns-utils-0.1.5/microns_utils/filepath_utils.py
--rw-rw-r--   0 root         (0) root         (0)       21 2022-10-04 16:41:22.000000 microns-utils-0.1.5/microns_utils/version.py
--rw-rw-r--   0 root         (0) root         (0)     1362 2022-05-16 07:10:32.000000 microns-utils-0.1.5/microns_utils/config_utils.py
--rw-rw-r--   0 root         (0) root         (0)     8075 2022-08-31 14:10:29.000000 microns-utils-0.1.5/microns_utils/version_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1303 2022-06-07 16:05:32.000000 microns-utils-0.1.5/microns_utils/datetime_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4862 2022-08-31 14:10:29.000000 microns-utils-0.1.5/microns_utils/adapter_utils.py
--rw-rw-r--   0 root         (0) root         (0)     3970 2022-08-31 14:10:29.000000 microns-utils-0.1.5/microns_utils/ng_utils.py
--rw-rw-r--   0 root         (0) root         (0)       34 2022-05-16 07:10:32.000000 microns-utils-0.1.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-04 16:41:38.000000 microns-utils-0.1.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:58:58.000000 microns-utils-0.1.7/
+-rw-rw-r--   0 root         (0) root         (0)       59 2022-05-16 07:20:39.000000 microns-utils-0.1.7/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:58:58.000000 microns-utils-0.1.7/microns_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-03 15:58:58.000000 microns-utils-0.1.7/microns_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-03 15:58:58.000000 microns-utils-0.1.7/microns_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-03 15:58:58.000000 microns-utils-0.1.7/microns_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 15:58:58.000000 microns-utils-0.1.7/microns_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-03 15:58:58.000000 microns-utils-0.1.7/microns_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-03 15:58:58.000000 microns-utils-0.1.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    26526 2022-05-16 07:18:26.000000 microns-utils-0.1.7/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      105 2022-08-31 14:10:29.000000 microns-utils-0.1.7/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)      593 2022-05-16 07:10:32.000000 microns-utils-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:58:58.000000 microns-utils-0.1.7/microns_utils/
+-rw-rw-r--   0 root         (0) root         (0)      540 2023-05-03 15:54:02.000000 microns-utils-0.1.7/microns_utils/misc_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      472 2022-05-16 07:10:32.000000 microns-utils-0.1.7/microns_utils/errors.py
+-rw-rw-r--   0 root         (0) root         (0)     9545 2023-05-03 15:54:02.000000 microns-utils-0.1.7/microns_utils/model_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1060 2022-05-16 07:10:32.000000 microns-utils-0.1.7/microns_utils/mesh_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    26798 2022-08-31 14:10:29.000000 microns-utils-0.1.7/microns_utils/widget_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      177 2022-05-16 07:10:32.000000 microns-utils-0.1.7/microns_utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9627 2022-10-04 16:41:22.000000 microns-utils-0.1.7/microns_utils/datajoint_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     7596 2023-05-03 15:54:02.000000 microns-utils-0.1.7/microns_utils/ap_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     8896 2023-05-03 15:54:02.000000 microns-utils-0.1.7/microns_utils/transform_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     2213 2022-05-19 11:29:51.000000 microns-utils-0.1.7/microns_utils/filepath_utils.py
+-rw-rw-r--   0 root         (0) root         (0)       21 2023-05-03 15:54:02.000000 microns-utils-0.1.7/microns_utils/version.py
+-rw-rw-r--   0 root         (0) root         (0)     1362 2022-05-16 07:10:32.000000 microns-utils-0.1.7/microns_utils/config_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     8075 2022-08-31 14:10:29.000000 microns-utils-0.1.7/microns_utils/version_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1303 2022-06-07 16:05:32.000000 microns-utils-0.1.7/microns_utils/datetime_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4862 2022-08-31 14:10:29.000000 microns-utils-0.1.7/microns_utils/adapter_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     8787 2023-05-03 15:54:02.000000 microns-utils-0.1.7/microns_utils/ng_utils.py
+-rw-rw-r--   0 root         (0) root         (0)       34 2022-05-16 07:10:32.000000 microns-utils-0.1.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 15:58:58.000000 microns-utils-0.1.7/setup.cfg
```

### Comparing `microns-utils-0.1.5/microns_utils.egg-info/SOURCES.txt` & `microns-utils-0.1.7/microns_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microns-utils-0.1.5/LICENSE` & `microns-utils-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `microns-utils-0.1.5/setup.py` & `microns-utils-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `microns-utils-0.1.5/microns_utils/model_utils.py` & `microns-utils-0.1.7/microns_utils/model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import numpy as np
 from functools import reduce
 import re
 from scipy.interpolate import griddata, RBFInterpolator
 
 class InterpModel:
-    def __init__(self, points, values, method, method_kws={}):
+    def __init__(self, points, values, method, method_kws=None):
         """
         Initialize with parameters for supported interpolation methods.
 
         :param points: (N x F array) N samples x F features
         :param values: (N x T array) N samples x T targets
         :param method: (str) Interpolation function to initialize.
             Options: 
@@ -23,15 +23,15 @@
         """
         valid_methods = ['griddata', 'rbf']
         assert method in valid_methods, f'Method provided not recognized. Valid methods: {valid_methods}'
 
         self._points = points
         self._values = values
         self._method = method
-        self.method_kws = method_kws
+        self.method_kws = method_kws if method_kws is not None else {}
     
     @property
     def points(self):
         return self._points
 
     @property
     def values(self):
```

### Comparing `microns-utils-0.1.5/microns_utils/mesh_utils.py` & `microns-utils-0.1.7/microns_utils/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `microns-utils-0.1.5/microns_utils/widget_utils.py` & `microns-utils-0.1.7/microns_utils/widget_utils.py`

 * *Files identical despite different names*

### Comparing `microns-utils-0.1.5/microns_utils/datajoint_utils.py` & `microns-utils-0.1.7/microns_utils/datajoint_utils.py`

 * *Files identical despite different names*

### Comparing `microns-utils-0.1.5/microns_utils/ap_utils.py` & `microns-utils-0.1.7/microns_utils/ap_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -155,7 +155,41 @@
 
     :returns: data stack
     """
     cv = CloudVolume(cv_path, use_https=True, progress=True, fill_missing=True, mip=mip)
     return cv.download(bbox=cv.bounds, segids=None if seg_ids is None else wrap(seg_ids)).squeeze()
 
 
+def query_nucleus_id_in_CAVE(nucleus_id, table_name=None, set_CAVEclient_kws=None, client=None):
+    """
+    Queries nucleus_detection_v0 or user provided table in CAVE with the given nucleus_id
+
+    :param nucleus_id (int): nucleus_id to query
+    :param table_name (str): table in CAVE to query
+        default is nucleus_detection_v0
+    :param set_CAVEclient (dict): - keywords to pass to set_CAVEclient
+        ignored if client is provided
+    :param client (CAVEclient): client to use for the query
+    """
+    if (set_CAVEclient_kws is not None) and (client is not None):
+        logger.warning('when both set_CAVEclient_kws and client are passed set_CAVEclient_kws will be ignored')
+    client = client if client is not None else set_CAVEclient(**set_CAVEclient_kws if set_CAVEclient_kws is not None else {})
+    df = client.materialize.query_table('nucleus_detection_v0' if table_name is None else table_name, filter_equal_dict={'id': nucleus_id}).rename(columns={'id': 'nucleus_id', 'pt_root_id': 'segment_id'})
+    return df
+
+
+def query_segment_id_in_CAVE(segment_id, table_name=None, set_CAVEclient_kws=None, client=None):
+    """
+    Queries nucleus_detection_v0 or user provided table in CAVE with the given segment_id
+
+    :param segment_id (int): segment_id to query
+    :param table_name (str): table in CAVE to query
+        default is nucleus_detection_v0
+    :param set_CAVEclient (dict): - keywords to pass to set_CAVEclient
+        ignored if client is provided
+    :param client (CAVEclient): client to use for the query
+    """
+    if (set_CAVEclient_kws is not None) and (client is not None):
+        logger.warning('when both set_CAVEclient_kws and client are passed set_CAVEclient_kws will be ignored')
+    client = client if client is not None else set_CAVEclient(**set_CAVEclient_kws if set_CAVEclient_kws is not None else {})
+    df = client.materialize.query_table('nucleus_detection_v0' if table_name is None else table_name, filter_equal_dict={'pt_root_id': segment_id}).rename(columns={'id': 'nucleus_id', 'pt_root_id': 'segment_id'})
+    return df
```

### Comparing `microns-utils-0.1.5/microns_utils/filepath_utils.py` & `microns-utils-0.1.7/microns_utils/filepath_utils.py`

 * *Files identical despite different names*

### Comparing `microns-utils-0.1.5/microns_utils/config_utils.py` & `microns-utils-0.1.7/microns_utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `microns-utils-0.1.5/microns_utils/version_utils.py` & `microns-utils-0.1.7/microns_utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `microns-utils-0.1.5/microns_utils/datetime_utils.py` & `microns-utils-0.1.7/microns_utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `microns-utils-0.1.5/microns_utils/adapter_utils.py` & `microns-utils-0.1.7/microns_utils/adapter_utils.py`

 * *Files identical despite different names*

