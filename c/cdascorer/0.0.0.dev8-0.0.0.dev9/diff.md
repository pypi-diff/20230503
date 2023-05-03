# Comparing `tmp/cdascorer-0.0.0.dev8.tar.gz` & `tmp/cdascorer-0.0.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdascorer-0.0.0.dev8.tar", last modified: Sat Mar 25 16:11:06 2023, max compression
+gzip compressed data, was "cdascorer-0.0.0.dev9.tar", last modified: Sat Mar 25 16:13:44 2023, max compression
```

## Comparing `cdascorer-0.0.0.dev8.tar` & `cdascorer-0.0.0.dev9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jowillia (15069) NR4\JIC_jc012 (113824)        0 2023-03-25 16:11:06.855693 cdascorer-0.0.0.dev8/
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      102 2023-03-12 12:53:21.000000 cdascorer-0.0.0.dev8/MANIFEST.in
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      441 2023-03-25 16:11:06.854819 cdascorer-0.0.0.dev8/PKG-INFO
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      164 2023-03-12 16:42:49.000000 cdascorer-0.0.0.dev8/README.md
-drwxr-xr-x   0 jowillia (15069) NR4\JIC_jc012 (113824)        0 2023-03-25 16:11:06.830396 cdascorer-0.0.0.dev8/cdascorer/
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)       92 2023-03-25 15:46:21.000000 cdascorer-0.0.0.dev8/cdascorer/__init__.py
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)     5249 2023-03-25 15:56:41.000000 cdascorer-0.0.0.dev8/cdascorer/cdametadata.py
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)    25799 2023-03-25 15:54:32.000000 cdascorer-0.0.0.dev8/cdascorer/cdascorer_gui.py
--rw-------   0 jowillia (15069) NR4\JIC_jc012 (113824)    25774 2023-03-25 16:05:11.000000 cdascorer-0.0.0.dev8/cdascorer/cdascorer_gui_windows.py
-drwxr-xr-x   0 jowillia (15069) NR4\JIC_jc012 (113824)        0 2023-03-25 16:11:06.838350 cdascorer-0.0.0.dev8/cdascorer-data/
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)        0 2023-03-12 12:36:02.000000 cdascorer-0.0.0.dev8/cdascorer-data/__init__.py
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)   771312 2023-03-12 12:36:02.000000 cdascorer-0.0.0.dev8/cdascorer-data/lesion_score_key.jpg
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)   184626 2023-03-12 12:36:02.000000 cdascorer-0.0.0.dev8/cdascorer-data/test_cda_img.jpg
-drwxr-xr-x   0 jowillia (15069) NR4\JIC_jc012 (113824)        0 2023-03-25 16:11:06.846423 cdascorer-0.0.0.dev8/cdascorer.egg-info/
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      441 2023-03-25 16:11:06.000000 cdascorer-0.0.0.dev8/cdascorer.egg-info/PKG-INFO
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      502 2023-03-25 16:11:06.000000 cdascorer-0.0.0.dev8/cdascorer.egg-info/SOURCES.txt
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)        1 2023-03-25 16:11:06.000000 cdascorer-0.0.0.dev8/cdascorer.egg-info/dependency_links.txt
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)       42 2023-03-25 16:11:06.000000 cdascorer-0.0.0.dev8/cdascorer.egg-info/requires.txt
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)       25 2023-03-25 16:11:06.000000 cdascorer-0.0.0.dev8/cdascorer.egg-info/top_level.txt
-drwxr-xr-x   0 jowillia (15069) NR4\JIC_jc012 (113824)        0 2023-03-25 16:11:06.852788 cdascorer-0.0.0.dev8/scripts/
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)     4804 2023-03-25 15:46:13.000000 cdascorer-0.0.0.dev8/scripts/cdascorer
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      220 2023-03-25 16:08:08.000000 cdascorer-0.0.0.dev8/scripts/cdascorer-test
--rw-------   0 jowillia (15069) NR4\JIC_jc012 (113824)      432 2023-03-25 16:04:10.000000 cdascorer-0.0.0.dev8/scripts/cdascorer-windows-test.py
--rw-------   0 jowillia (15069) NR4\JIC_jc012 (113824)     4858 2023-03-25 16:05:19.000000 cdascorer-0.0.0.dev8/scripts/cdascorer-windows.py
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)       38 2023-03-25 16:11:06.855930 cdascorer-0.0.0.dev8/setup.cfg
--rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      820 2023-03-25 15:51:31.000000 cdascorer-0.0.0.dev8/setup.py
+drwxr-xr-x   0 jowillia (15069) NR4\JIC_jc012 (113824)        0 2023-03-25 16:13:44.531001 cdascorer-0.0.0.dev9/
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      102 2023-03-12 12:53:21.000000 cdascorer-0.0.0.dev9/MANIFEST.in
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      441 2023-03-25 16:13:44.530231 cdascorer-0.0.0.dev9/PKG-INFO
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      164 2023-03-12 16:42:49.000000 cdascorer-0.0.0.dev9/README.md
+drwxr-xr-x   0 jowillia (15069) NR4\JIC_jc012 (113824)        0 2023-03-25 16:13:44.504610 cdascorer-0.0.0.dev9/cdascorer/
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)       92 2023-03-25 15:46:21.000000 cdascorer-0.0.0.dev9/cdascorer/__init__.py
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)     5249 2023-03-25 15:56:41.000000 cdascorer-0.0.0.dev9/cdascorer/cdametadata.py
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)    25799 2023-03-25 15:54:32.000000 cdascorer-0.0.0.dev9/cdascorer/cdascorer_gui.py
+-rw-------   0 jowillia (15069) NR4\JIC_jc012 (113824)    25774 2023-03-25 16:05:11.000000 cdascorer-0.0.0.dev9/cdascorer/cdascorer_gui_windows.py
+drwxr-xr-x   0 jowillia (15069) NR4\JIC_jc012 (113824)        0 2023-03-25 16:13:44.513059 cdascorer-0.0.0.dev9/cdascorer-data/
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)        0 2023-03-12 12:36:02.000000 cdascorer-0.0.0.dev9/cdascorer-data/__init__.py
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)   771312 2023-03-12 12:36:02.000000 cdascorer-0.0.0.dev9/cdascorer-data/lesion_score_key.jpg
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)   184626 2023-03-12 12:36:02.000000 cdascorer-0.0.0.dev9/cdascorer-data/test_cda_img.jpg
+drwxr-xr-x   0 jowillia (15069) NR4\JIC_jc012 (113824)        0 2023-03-25 16:13:44.522745 cdascorer-0.0.0.dev9/cdascorer.egg-info/
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      441 2023-03-25 16:13:44.000000 cdascorer-0.0.0.dev9/cdascorer.egg-info/PKG-INFO
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      502 2023-03-25 16:13:44.000000 cdascorer-0.0.0.dev9/cdascorer.egg-info/SOURCES.txt
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)        1 2023-03-25 16:13:44.000000 cdascorer-0.0.0.dev9/cdascorer.egg-info/dependency_links.txt
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)       42 2023-03-25 16:13:44.000000 cdascorer-0.0.0.dev9/cdascorer.egg-info/requires.txt
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)       25 2023-03-25 16:13:44.000000 cdascorer-0.0.0.dev9/cdascorer.egg-info/top_level.txt
+drwxr-xr-x   0 jowillia (15069) NR4\JIC_jc012 (113824)        0 2023-03-25 16:13:44.528856 cdascorer-0.0.0.dev9/scripts/
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)     4804 2023-03-25 15:46:13.000000 cdascorer-0.0.0.dev9/scripts/cdascorer
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      220 2023-03-25 16:08:08.000000 cdascorer-0.0.0.dev9/scripts/cdascorer-test
+-rw-------   0 jowillia (15069) NR4\JIC_jc012 (113824)      432 2023-03-25 16:04:10.000000 cdascorer-0.0.0.dev9/scripts/cdascorer-windows-test.py
+-rw-------   0 jowillia (15069) NR4\JIC_jc012 (113824)     4811 2023-03-25 16:12:45.000000 cdascorer-0.0.0.dev9/scripts/cdascorer-windows.py
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)       38 2023-03-25 16:13:44.531223 cdascorer-0.0.0.dev9/setup.cfg
+-rw-r--r--   0 jowillia (15069) NR4\JIC_jc012 (113824)      820 2023-03-25 16:13:34.000000 cdascorer-0.0.0.dev9/setup.py
```

### Comparing `cdascorer-0.0.0.dev8/cdascorer/cdametadata.py` & `cdascorer-0.0.0.dev9/cdascorer/cdametadata.py`

 * *Files identical despite different names*

### Comparing `cdascorer-0.0.0.dev8/cdascorer/cdascorer_gui.py` & `cdascorer-0.0.0.dev9/cdascorer/cdascorer_gui.py`

 * *Files identical despite different names*

### Comparing `cdascorer-0.0.0.dev8/cdascorer/cdascorer_gui_windows.py` & `cdascorer-0.0.0.dev9/cdascorer/cdascorer_gui_windows.py`

 * *Files identical despite different names*

### Comparing `cdascorer-0.0.0.dev8/cdascorer-data/lesion_score_key.jpg` & `cdascorer-0.0.0.dev9/cdascorer-data/lesion_score_key.jpg`

 * *Files identical despite different names*

### Comparing `cdascorer-0.0.0.dev8/cdascorer-data/test_cda_img.jpg` & `cdascorer-0.0.0.dev9/cdascorer-data/test_cda_img.jpg`

 * *Files identical despite different names*

### Comparing `cdascorer-0.0.0.dev8/scripts/cdascorer` & `cdascorer-0.0.0.dev9/scripts/cdascorer`

 * *Files identical despite different names*

### Comparing `cdascorer-0.0.0.dev8/scripts/cdascorer-windows.py` & `cdascorer-0.0.0.dev9/scripts/cdascorer-windows.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-#!C:\Users\joshu\AppData\Local\Programs\Python\Python311\python.exe
-
+#!/usr/bin/env python
 '''
 cdascorer-run
 
 A utility for running the cdascorer GUI on a folder of images.
 
 See the help:
```

### Comparing `cdascorer-0.0.0.dev8/setup.py` & `cdascorer-0.0.0.dev9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="cdascorer",
-    version='0.0.0.dev8',
+    version='0.0.0.dev9',
     packages = ['cdascorer', 'cdascorer-data'],
     url="https://github.com/joshuandwilliams/CDAScorer",
     license='LICENSE.txt',
     author="Joshua Williams",
     author_email="<jowillia@nbi.ac.uk>",
     description='Cell Death Area Data Collection',
     long_description=long_description,
```

