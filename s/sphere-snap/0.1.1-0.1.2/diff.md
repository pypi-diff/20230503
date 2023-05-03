# Comparing `tmp/sphere_snap-0.1.1-py3-none-any.whl.zip` & `tmp/sphere_snap-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 16486 bytes, number of entries: 10
--rw-r--r--  2.0 unx     3128 b- defN 23-May-03 13:43 sphere_snap/__init__.py
+Zip file size: 16893 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     3128 b- defN 23-May-03 13:47 sphere_snap/__init__.py
 -rw-r--r--  2.0 unx     7092 b- defN 23-May-03 13:14 sphere_snap/snap_config.py
 -rw-r--r--  2.0 unx    12774 b- defN 23-May-03 13:14 sphere_snap/sphere_coor_projections.py
 -rw-r--r--  2.0 unx    19890 b- defN 23-May-03 13:14 sphere_snap/sphere_snap.py
 -rw-r--r--  2.0 unx     6660 b- defN 23-May-03 12:39 sphere_snap/utils.py
--rw-r--r--  2.0 unx     1073 b- defN 23-May-03 13:44 sphere_snap-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      841 b- defN 23-May-03 13:44 sphere_snap-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 13:44 sphere_snap-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-03 13:44 sphere_snap-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      825 b- defN 23-May-03 13:44 sphere_snap-0.1.1.dist-info/RECORD
-10 files, 52387 bytes uncompressed, 15080 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx     1073 b- defN 23-May-03 13:47 sphere_snap-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1952 b- defN 23-May-03 13:47 sphere_snap-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 13:47 sphere_snap-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-03 13:47 sphere_snap-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      826 b- defN 23-May-03 13:47 sphere_snap-0.1.2.dist-info/RECORD
+10 files, 53499 bytes uncompressed, 15487 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: sphere_snap/sphere_snap.py
 Comment: 
 
 Filename: sphere_snap/utils.py
 Comment: 
 
-Filename: sphere_snap-0.1.1.dist-info/LICENSE
+Filename: sphere_snap-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: sphere_snap-0.1.1.dist-info/METADATA
+Filename: sphere_snap-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: sphere_snap-0.1.1.dist-info/WHEEL
+Filename: sphere_snap-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: sphere_snap-0.1.1.dist-info/top_level.txt
+Filename: sphere_snap-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sphere_snap-0.1.1.dist-info/RECORD
+Filename: sphere_snap-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sphere_snap/__init__.py

```diff
@@ -4,15 +4,15 @@
 A quick and easy to use library for reprojecting various image types.
 """
 from __future__ import absolute_import
 import logging
 import numpy as np
 
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __author__ = 'Andrei Georgescu'
 __credits__ = ''
 
 
 is_cupy_available = None
 
 def __init_cupy():
```

## Comparing `sphere_snap-0.1.1.dist-info/LICENSE` & `sphere_snap-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

