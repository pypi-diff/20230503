# Comparing `tmp/cylinter-0.0.8.tar.gz` & `tmp/cylinter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cylinter-0.0.8.tar", last modified: Mon Jan 25 14:58:44 2021, max compression
+gzip compressed data, was "dist/cylinter-0.0.9.tar", last modified: Mon Jan 25 16:57:25 2021, max compression
```

## Comparing `cylinter-0.0.8.tar` & `cylinter-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 greg       (502) staff       (20)        0 2021-01-25 14:58:44.189438 cylinter-0.0.8/
--rw-r--r--   0 greg       (502) staff       (20)     2146 2021-01-25 14:58:44.188892 cylinter-0.0.8/PKG-INFO
--rw-r--r--   0 greg       (502) staff       (20)     1255 2021-01-23 05:08:26.000000 cylinter-0.0.8/README.md
-drwxr-xr-x   0 greg       (502) staff       (20)        0 2021-01-25 14:58:44.184986 cylinter-0.0.8/cylinter/
--rw-r--r--   0 greg       (502) staff       (20)        0 2021-01-21 21:38:14.000000 cylinter-0.0.8/cylinter/__init__.py
--rw-r--r--   0 greg       (502) staff       (20)   140161 2021-01-22 19:44:44.000000 cylinter-0.0.8/cylinter/components.py
--rw-r--r--   0 greg       (502) staff       (20)     1442 2021-01-21 02:50:10.000000 cylinter-0.0.8/cylinter/config.py
--rw-r--r--   0 greg       (502) staff       (20)      695 2021-01-23 02:58:52.000000 cylinter-0.0.8/cylinter/config.yml
--rw-r--r--   0 greg       (502) staff       (20)     2095 2021-01-22 19:44:35.000000 cylinter-0.0.8/cylinter/cylinter.py
--rw-r--r--   0 greg       (502) staff       (20)     2581 2021-01-21 02:50:10.000000 cylinter-0.0.8/cylinter/pipeline.py
--rw-r--r--   0 greg       (502) staff       (20)      940 2021-01-24 18:56:28.000000 cylinter-0.0.8/cylinter/prep.py
--rw-r--r--   0 greg       (502) staff       (20)     2672 2021-01-25 03:55:57.000000 cylinter-0.0.8/cylinter/prep_subprocess.sh
--rw-r--r--   0 greg       (502) staff       (20)     8682 2021-01-21 02:50:10.000000 cylinter-0.0.8/cylinter/utils.py
-drwxr-xr-x   0 greg       (502) staff       (20)        0 2021-01-25 14:58:44.188191 cylinter-0.0.8/cylinter.egg-info/
--rw-r--r--   0 greg       (502) staff       (20)     2146 2021-01-25 14:58:44.000000 cylinter-0.0.8/cylinter.egg-info/PKG-INFO
--rw-r--r--   0 greg       (502) staff       (20)      431 2021-01-25 14:58:44.000000 cylinter-0.0.8/cylinter.egg-info/SOURCES.txt
--rw-r--r--   0 greg       (502) staff       (20)        1 2021-01-25 14:58:44.000000 cylinter-0.0.8/cylinter.egg-info/dependency_links.txt
--rw-r--r--   0 greg       (502) staff       (20)       79 2021-01-25 14:58:44.000000 cylinter-0.0.8/cylinter.egg-info/entry_points.txt
--rw-r--r--   0 greg       (502) staff       (20)        1 2021-01-25 14:58:44.000000 cylinter-0.0.8/cylinter.egg-info/not-zip-safe
--rw-r--r--   0 greg       (502) staff       (20)      235 2021-01-25 14:58:44.000000 cylinter-0.0.8/cylinter.egg-info/requires.txt
--rw-r--r--   0 greg       (502) staff       (20)        9 2021-01-25 14:58:44.000000 cylinter-0.0.8/cylinter.egg-info/top_level.txt
--rw-r--r--   0 greg       (502) staff       (20)       38 2021-01-25 14:58:44.189580 cylinter-0.0.8/setup.cfg
--rw-r--r--   0 greg       (502) staff       (20)     2044 2021-01-25 14:57:35.000000 cylinter-0.0.8/setup.py
+drwxr-xr-x   0 greg       (502) staff       (20)        0 2021-01-25 16:57:25.697473 cylinter-0.0.9/
+-rw-r--r--   0 greg       (502) staff       (20)     2146 2021-01-25 16:57:25.696936 cylinter-0.0.9/PKG-INFO
+-rw-r--r--   0 greg       (502) staff       (20)     1255 2021-01-23 05:08:26.000000 cylinter-0.0.9/README.md
+drwxr-xr-x   0 greg       (502) staff       (20)        0 2021-01-25 16:57:25.692129 cylinter-0.0.9/cylinter/
+-rw-r--r--   0 greg       (502) staff       (20)        0 2021-01-21 21:38:14.000000 cylinter-0.0.9/cylinter/__init__.py
+-rw-r--r--   0 greg       (502) staff       (20)   140161 2021-01-22 19:44:44.000000 cylinter-0.0.9/cylinter/components.py
+-rw-r--r--   0 greg       (502) staff       (20)     1442 2021-01-21 02:50:10.000000 cylinter-0.0.9/cylinter/config.py
+-rw-r--r--   0 greg       (502) staff       (20)      695 2021-01-23 02:58:52.000000 cylinter-0.0.9/cylinter/config.yml
+-rw-r--r--   0 greg       (502) staff       (20)     2095 2021-01-22 19:44:35.000000 cylinter-0.0.9/cylinter/cylinter.py
+-rw-r--r--   0 greg       (502) staff       (20)     2581 2021-01-21 02:50:10.000000 cylinter-0.0.9/cylinter/pipeline.py
+-rw-r--r--   0 greg       (502) staff       (20)      940 2021-01-24 18:56:28.000000 cylinter-0.0.9/cylinter/prep.py
+-rw-r--r--   0 greg       (502) staff       (20)     2672 2021-01-25 03:55:57.000000 cylinter-0.0.9/cylinter/prep_subprocess.sh
+-rw-r--r--   0 greg       (502) staff       (20)     8682 2021-01-21 02:50:10.000000 cylinter-0.0.9/cylinter/utils.py
+drwxr-xr-x   0 greg       (502) staff       (20)        0 2021-01-25 16:57:25.696109 cylinter-0.0.9/cylinter.egg-info/
+-rw-r--r--   0 greg       (502) staff       (20)     2146 2021-01-25 16:57:25.000000 cylinter-0.0.9/cylinter.egg-info/PKG-INFO
+-rw-r--r--   0 greg       (502) staff       (20)      431 2021-01-25 16:57:25.000000 cylinter-0.0.9/cylinter.egg-info/SOURCES.txt
+-rw-r--r--   0 greg       (502) staff       (20)        1 2021-01-25 16:57:25.000000 cylinter-0.0.9/cylinter.egg-info/dependency_links.txt
+-rw-r--r--   0 greg       (502) staff       (20)       79 2021-01-25 16:57:25.000000 cylinter-0.0.9/cylinter.egg-info/entry_points.txt
+-rw-r--r--   0 greg       (502) staff       (20)        1 2021-01-25 16:57:25.000000 cylinter-0.0.9/cylinter.egg-info/not-zip-safe
+-rw-r--r--   0 greg       (502) staff       (20)      235 2021-01-25 16:57:25.000000 cylinter-0.0.9/cylinter.egg-info/requires.txt
+-rw-r--r--   0 greg       (502) staff       (20)        9 2021-01-25 16:57:25.000000 cylinter-0.0.9/cylinter.egg-info/top_level.txt
+-rw-r--r--   0 greg       (502) staff       (20)       38 2021-01-25 16:57:25.697684 cylinter-0.0.9/setup.cfg
+-rw-r--r--   0 greg       (502) staff       (20)     1956 2021-01-25 16:55:43.000000 cylinter-0.0.9/setup.py
```

### Comparing `cylinter-0.0.8/PKG-INFO` & `cylinter-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: cylinter
-Version: 0.0.8
+Version: 0.0.9
 Summary: CyLinter
 Home-page: https://github.com/labsyspharm/cylinter
 Author: Gregory J. Baker
 Author-email: gregory_baker2@hms.harvard.edu
 License: MIT License
-Download-URL: https://github.com/labsyspharm/cylinter/archive/v0.0.8.tar.gz
+Download-URL: https://github.com/labsyspharm/cylinter/archive/v0.0.9.tar.gz
 Description: ![alt text](https://github.com/labsyspharm/cylinter/blob/master/docs/logo.png?raw=true)
         
         # An Interactive Image Segmentation Filter for Multiplex Microscopy.
         
         CyLinter identifies and removes cell segmentation instances (i.e. cells) in multiplexed whole tissue and tissue microarray images corrupted by optical and/or image preprocessing (e.g. stitching, registration, segmentation) artifacts. The tool comprises a set of user-guided, quality control (QC) modules instantiated as a configurable [Python](https://www.python.org) Class; module results are cached to allow for dynamic restarts and iterative QC strategies. The tool is used to clean image-derived, single-cell data prior to downstream analysis.
         
         CyLinter development is led by [Greg Baker](https://github.com/gjbaker) at [Laboratory of Systems Pharmacology](https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/about/), Harvard Medical School.
```

### Comparing `cylinter-0.0.8/README.md` & `cylinter-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cylinter-0.0.8/cylinter/components.py` & `cylinter-0.0.9/cylinter/components.py`

 * *Files identical despite different names*

### Comparing `cylinter-0.0.8/cylinter/config.py` & `cylinter-0.0.9/cylinter/config.py`

 * *Files identical despite different names*

### Comparing `cylinter-0.0.8/cylinter/config.yml` & `cylinter-0.0.9/cylinter/config.yml`

 * *Files identical despite different names*

### Comparing `cylinter-0.0.8/cylinter/cylinter.py` & `cylinter-0.0.9/cylinter/cylinter.py`

 * *Files identical despite different names*

### Comparing `cylinter-0.0.8/cylinter/pipeline.py` & `cylinter-0.0.9/cylinter/pipeline.py`

 * *Files identical despite different names*

### Comparing `cylinter-0.0.8/cylinter/prep.py` & `cylinter-0.0.9/cylinter/prep.py`

 * *Files identical despite different names*

### Comparing `cylinter-0.0.8/cylinter/prep_subprocess.sh` & `cylinter-0.0.9/cylinter/prep_subprocess.sh`

 * *Files identical despite different names*

### Comparing `cylinter-0.0.8/cylinter/utils.py` & `cylinter-0.0.9/cylinter/utils.py`

 * *Files identical despite different names*

### Comparing `cylinter-0.0.8/cylinter.egg-info/PKG-INFO` & `cylinter-0.0.9/cylinter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: cylinter
-Version: 0.0.8
+Version: 0.0.9
 Summary: CyLinter
 Home-page: https://github.com/labsyspharm/cylinter
 Author: Gregory J. Baker
 Author-email: gregory_baker2@hms.harvard.edu
 License: MIT License
-Download-URL: https://github.com/labsyspharm/cylinter/archive/v0.0.8.tar.gz
+Download-URL: https://github.com/labsyspharm/cylinter/archive/v0.0.9.tar.gz
 Description: ![alt text](https://github.com/labsyspharm/cylinter/blob/master/docs/logo.png?raw=true)
         
         # An Interactive Image Segmentation Filter for Multiplex Microscopy.
         
         CyLinter identifies and removes cell segmentation instances (i.e. cells) in multiplexed whole tissue and tissue microarray images corrupted by optical and/or image preprocessing (e.g. stitching, registration, segmentation) artifacts. The tool comprises a set of user-guided, quality control (QC) modules instantiated as a configurable [Python](https://www.python.org) Class; module results are cached to allow for dynamic restarts and iterative QC strategies. The tool is used to clean image-derived, single-cell data prior to downstream analysis.
         
         CyLinter development is led by [Greg Baker](https://github.com/gjbaker) at [Laboratory of Systems Pharmacology](https://hits.harvard.edu/the-program/laboratory-of-systems-pharmacology/about/), Harvard Medical School.
```

### Comparing `cylinter-0.0.8/setup.py` & `cylinter-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     'napari==0.3.6',  # points layer doesn't work with napari[all] (v0.4.3)
     'PyQt5==5.15.2',  # must include if not installing napari[all]
     'zarr==2.6.1',
     'natsort==7.1.0',
     'rpy2==3.4.2',
     'bridson==0.1.0',
     'hurry.filesize==0.9',
-    'synapseclient==2.0.0',  # v2.2.2 (current version as of 01/25/21 fails to transfer under current distribution)
+    'synapseclient==2.2.2',
 ]
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'CyLinter'
 AUTHOR = 'Gregory J. Baker'
 AUTHOR_EMAIL = 'gregory_baker2@hms.harvard.edu'
 LICENSE = 'MIT License'
 HOMEPAGE = 'https://github.com/labsyspharm/cylinter'
 
 setup(
```

