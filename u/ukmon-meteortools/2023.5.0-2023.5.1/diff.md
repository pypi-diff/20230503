# Comparing `tmp/ukmon_meteortools-2023.5.0.tar.gz` & `tmp/ukmon_meteortools-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukmon_meteortools-2023.5.0.tar", last modified: Wed May  3 14:23:35 2023, max compression
+gzip compressed data, was "ukmon_meteortools-2023.5.1.tar", last modified: Wed May  3 14:27:11 2023, max compression
```

## Comparing `ukmon_meteortools-2023.5.0.tar` & `ukmon_meteortools-2023.5.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.289585 ukmon_meteortools-2023.5.0/
--rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.5.0/LICENSE
--rw-rw-rw-   0        0        0    42659 2023-05-03 14:23:35.287574 ukmon_meteortools-2023.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.5.0/README.md
--rw-rw-rw-   0        0        0     2204 2023-05-03 14:23:10.000000 ukmon_meteortools-2023.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 14:23:35.289585 ukmon_meteortools-2023.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.202576 ukmon_meteortools-2023.5.0/ukmon_meteortools/
--rw-rw-rw-   0        0        0      756 2023-05-02 21:24:36.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.240574 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/
--rw-rw-rw-   0        0        0    10159 2023-05-02 20:41:26.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py
--rw-rw-rw-   0        0        0     6742 2023-05-02 20:41:44.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/ReadUFOCapXML.py
--rw-rw-rw-   0        0        0      428 2023-05-02 20:42:29.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/__init__.py
--rw-rw-rw-   0        0        0    19243 2023-05-02 20:13:35.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/ftpDetectInfo.py
--rw-rw-rw-   0        0        0     7393 2023-05-02 21:34:25.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/imoWorkingShowerList.py
--rw-rw-rw-   0        0        0     2948 2023-05-02 20:46:56.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/platepar.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.249574 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/
--rw-rw-rw-   0        0        0      660 2023-05-02 20:33:20.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
--rw-rw-rw-   0        0        0     6077 2023-05-02 20:34:59.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/multiDayRadiant.py
--rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/multiEventGroundMap.py
--rw-rw-rw-   0        0        0     5242 2023-05-03 14:21:56.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/multiTrackStack.py
--rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
--rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/plotRMSOrbits.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.253577 ukmon_meteortools-2023.5.0/ukmon_meteortools/share/
--rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
--rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/share/__init__.py
--rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/share/streamfulldata.npy
-drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.272584 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/
--rw-rw-rw-   0        0        0      524 2023-04-16 21:29:05.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/__init__.py
--rw-rw-rw-   0        0        0     2088 2023-05-03 14:21:17.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/apiExampleCode.py
--rw-rw-rw-   0        0        0     2476 2023-05-02 20:12:42.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/drawFTPfile.py
--rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/findNearDuplicates.py
--rw-rw-rw-   0        0        0     5670 2023-05-03 14:21:17.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/getLiveImages.py
--rw-rw-rw-   0        0        0     3238 2023-05-02 20:18:14.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/getOverlappingFovs.py
--rw-rw-rw-   0        0        0     3589 2023-05-02 20:20:03.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/plotTrack.py
--rw-rw-rw-   0        0        0     2385 2023-05-02 20:58:19.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/retrieveECSV.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.286574 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/
--rw-rw-rw-   0        0        0    13798 2023-05-02 20:57:25.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/Math.py
--rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/VectorMaths.py
--rw-rw-rw-   0        0        0     1411 2023-05-02 21:38:00.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-05-02 21:35:02.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/annotateImage.py
--rw-rw-rw-   0        0        0     1313 2023-05-02 21:35:22.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/convertSolLon.py
--rw-rw-rw-   0        0        0     2114 2023-05-02 21:35:49.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/getActiveShowers.py
--rw-rw-rw-   0        0        0     3937 2023-05-02 21:41:36.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/getShowerDates.py
--rw-rw-rw-   0        0        0     5117 2023-05-02 21:11:53.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/kmlHandlers.py
--rw-rw-rw-   0        0        0     3699 2023-05-02 20:49:10.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/sendAnEmail.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.231573 ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/
--rw-rw-rw-   0        0        0    42659 2023-05-03 14:23:35.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1716 2023-05-03 14:23:35.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 14:23:35.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      263 2023-05-03 14:23:35.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-03 14:23:35.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 14:27:11.542605 ukmon_meteortools-2023.5.1/
+-rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.5.1/LICENSE
+-rw-rw-rw-   0        0        0    42659 2023-05-03 14:27:11.542605 ukmon_meteortools-2023.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.5.1/README.md
+-rw-rw-rw-   0        0        0     2204 2023-05-03 14:26:51.000000 ukmon_meteortools-2023.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 14:27:11.542605 ukmon_meteortools-2023.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 14:27:11.467605 ukmon_meteortools-2023.5.1/ukmon_meteortools/
+-rw-rw-rw-   0        0        0      756 2023-05-02 21:24:36.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 14:27:11.495620 ukmon_meteortools-2023.5.1/ukmon_meteortools/fileformats/
+-rw-rw-rw-   0        0        0    10159 2023-05-02 20:41:26.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py
+-rw-rw-rw-   0        0        0     6742 2023-05-02 20:41:44.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/fileformats/ReadUFOCapXML.py
+-rw-rw-rw-   0        0        0      428 2023-05-02 20:42:29.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/fileformats/__init__.py
+-rw-rw-rw-   0        0        0    19243 2023-05-02 20:13:35.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/fileformats/ftpDetectInfo.py
+-rw-rw-rw-   0        0        0     7393 2023-05-02 21:34:25.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/fileformats/imoWorkingShowerList.py
+-rw-rw-rw-   0        0        0     2948 2023-05-02 20:46:56.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/fileformats/platepar.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:27:11.502606 ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/
+-rw-rw-rw-   0        0        0      660 2023-05-02 20:33:20.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
+-rw-rw-rw-   0        0        0     6077 2023-05-02 20:34:59.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/multiDayRadiant.py
+-rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/multiEventGroundMap.py
+-rw-rw-rw-   0        0        0     5242 2023-05-03 14:21:56.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/multiTrackStack.py
+-rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
+-rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/plotRMSOrbits.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:27:11.508606 ukmon_meteortools-2023.5.1/ukmon_meteortools/share/
+-rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
+-rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/share/__init__.py
+-rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/share/streamfulldata.npy
+drwxrwxrwx   0        0        0        0 2023-05-03 14:27:11.527606 ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/
+-rw-rw-rw-   0        0        0      516 2023-05-03 14:26:10.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/__init__.py
+-rw-rw-rw-   0        0        0     2088 2023-05-03 14:21:17.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/apiExampleCode.py
+-rw-rw-rw-   0        0        0     2476 2023-05-02 20:12:42.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/drawFTPfile.py
+-rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/findNearDuplicates.py
+-rw-rw-rw-   0        0        0     5670 2023-05-03 14:21:17.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/getLiveImages.py
+-rw-rw-rw-   0        0        0     3238 2023-05-02 20:18:14.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/getOverlappingFovs.py
+-rw-rw-rw-   0        0        0     3589 2023-05-02 20:20:03.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/plotTrack.py
+-rw-rw-rw-   0        0        0     2385 2023-05-02 20:58:19.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/retrieveECSV.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:27:11.540608 ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/
+-rw-rw-rw-   0        0        0    13798 2023-05-02 20:57:25.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/Math.py
+-rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/VectorMaths.py
+-rw-rw-rw-   0        0        0     1411 2023-05-02 21:38:00.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-05-02 21:35:02.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/annotateImage.py
+-rw-rw-rw-   0        0        0     1313 2023-05-02 21:35:22.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/convertSolLon.py
+-rw-rw-rw-   0        0        0     2114 2023-05-02 21:35:49.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/getActiveShowers.py
+-rw-rw-rw-   0        0        0     3937 2023-05-02 21:41:36.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/getShowerDates.py
+-rw-rw-rw-   0        0        0     5117 2023-05-02 21:11:53.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/kmlHandlers.py
+-rw-rw-rw-   0        0        0     3699 2023-05-02 20:49:10.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/sendAnEmail.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:27:11.485614 ukmon_meteortools-2023.5.1/ukmon_meteortools.egg-info/
+-rw-rw-rw-   0        0        0    42659 2023-05-03 14:27:11.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1716 2023-05-03 14:27:11.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 14:27:11.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      263 2023-05-03 14:27:11.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-03 14:27:11.000000 ukmon_meteortools-2023.5.1/ukmon_meteortools.egg-info/top_level.txt
```

### Comparing `ukmon_meteortools-2023.5.0/LICENSE` & `ukmon_meteortools-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/PKG-INFO` & `ukmon_meteortools-2023.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon_meteortools
-Version: 2023.5.0
+Version: 2023.5.1
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.5.0/README.md` & `ukmon_meteortools-2023.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/pyproject.toml` & `ukmon_meteortools-2023.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ukmon_meteortools"
-version = "2023.05.0"
+version = "2023.05.1"
 description = "Python Tools for Meteor Data Analysis"
 readme = "ukmon_meteortools/README.md"
 authors = [{ name = "Mark McIntyre", email = "ukmon@markmcintyreastro.co.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -64,15 +64,15 @@
 #[tool.setuptools.packages.find]
 #where = ["ukmon_meteortools"]
 
 [tool.setuptools.package-data]
 "*" = ["*.npy", "*.xml"]
 
 [tool.bumpver]
-current_version = "2023.05.0"
+current_version = "2023.05.1"
 version_pattern = "YYYY.0M.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/README.md` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/ReadUFOCapXML.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/fileformats/ReadUFOCapXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/ftpDetectInfo.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/fileformats/ftpDetectInfo.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/imoWorkingShowerList.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/fileformats/imoWorkingShowerList.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/platepar.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/fileformats/platepar.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/__init__.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/multiDayRadiant.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/multiDayRadiant.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/multiEventGroundMap.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/multiEventGroundMap.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/multiTrackStack.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/multiTrackStack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/plotCAMSOrbits.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/plotCAMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/plotRMSOrbits.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/rmsutils/plotRMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/share/__init__.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/share/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/share/streamfulldata.npy` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/share/streamfulldata.npy`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/__init__.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 # flake8: noqa
 
-from .apiExampleCode import apiurl, matchApiCall, detailApiCall1, detailApiCall2
+from .apiExampleCode import matchApiCall, detailApiCall1, detailApiCall2
 from .drawFTPfile import drawFTPFile
 from .findNearDuplicates import findNearDuplicates
 from .getLiveImages import getLiveJpgs, getFBFiles, createTxtFile
 from .getOverlappingFovs import checkKMLOverlap, pointInsideFov, getOverlapWith, getOverlappingCameras
 from .plotTrack import trackToDistvsHeight, trackToTimevsVelocity, trackToTimevsHeight
 from .retrieveECSV import getECSVs
```

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/apiExampleCode.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/apiExampleCode.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/drawFTPfile.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/drawFTPfile.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/findNearDuplicates.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/findNearDuplicates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/getLiveImages.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/getLiveImages.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/getOverlappingFovs.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/getOverlappingFovs.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/plotTrack.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/plotTrack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/retrieveECSV.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/usertools/retrieveECSV.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/Math.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/Math.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/VectorMaths.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/VectorMaths.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/__init__.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/annotateImage.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/annotateImage.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/convertSolLon.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/convertSolLon.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/getActiveShowers.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/getActiveShowers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/getShowerDates.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/getShowerDates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/kmlHandlers.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/kmlHandlers.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/sendAnEmail.py` & `ukmon_meteortools-2023.5.1/ukmon_meteortools/utils/sendAnEmail.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/PKG-INFO` & `ukmon_meteortools-2023.5.1/ukmon_meteortools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon-meteortools
-Version: 2023.5.0
+Version: 2023.5.1
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/SOURCES.txt` & `ukmon_meteortools-2023.5.1/ukmon_meteortools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

