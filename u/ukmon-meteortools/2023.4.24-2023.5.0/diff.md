# Comparing `tmp/ukmon_meteortools-2023.4.24.tar.gz` & `tmp/ukmon_meteortools-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukmon_meteortools-2023.4.24.tar", last modified: Sun Apr 30 07:19:42 2023, max compression
+gzip compressed data, was "ukmon_meteortools-2023.5.0.tar", last modified: Wed May  3 14:23:35 2023, max compression
```

## Comparing `ukmon_meteortools-2023.4.24.tar` & `ukmon_meteortools-2023.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 07:19:42.576211 ukmon_meteortools-2023.4.24/
--rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.4.24/LICENSE
--rw-rw-rw-   0        0        0    42683 2023-04-30 07:19:42.575211 ukmon_meteortools-2023.4.24/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.4.24/README.md
--rw-rw-rw-   0        0        0     2202 2023-04-30 07:18:19.000000 ukmon_meteortools-2023.4.24/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 07:19:42.576211 ukmon_meteortools-2023.4.24/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-30 07:19:42.471213 ukmon_meteortools-2023.4.24/ukmon_meteortools/
--rw-rw-rw-   0        0        0      779 2023-04-30 07:18:23.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 07:19:42.513211 ukmon_meteortools-2023.4.24/ukmon_meteortools/fileformats/
--rw-rw-rw-   0        0        0    12830 2023-04-18 13:55:16.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py
--rw-rw-rw-   0        0        0     6608 2023-04-27 21:05:51.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/fileformats/ReadUFOCapXML.py
--rw-rw-rw-   0        0        0      593 2023-04-29 18:31:34.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/fileformats/__init__.py
--rw-rw-rw-   0        0        0    19234 2023-04-29 18:22:08.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/fileformats/ftpDetectInfo.py
--rw-rw-rw-   0        0        0     7513 2023-04-18 22:30:53.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/fileformats/imoWorkingShowerList.py
--rw-rw-rw-   0        0        0     2330 2023-03-08 12:49:15.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/fileformats/platepar.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:19:42.524212 ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/
--rw-rw-rw-   0        0        0      944 2023-04-29 22:53:32.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/__init__.py
--rw-rw-rw-   0        0        0     1842 2023-04-29 22:37:52.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
--rw-rw-rw-   0        0        0     5980 2023-04-29 22:16:26.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/multiDayRadiant.py
--rw-rw-rw-   0        0        0     3609 2023-04-29 23:33:48.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/multiEventGroundMap.py
--rw-rw-rw-   0        0        0     4977 2023-04-29 22:14:49.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/multiTrackStack.py
--rw-rw-rw-   0        0        0     2232 2023-04-29 23:15:36.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
--rw-rw-rw-   0        0        0     2210 2023-04-29 23:19:16.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/plotRMSOrbits.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:19:42.544210 ukmon_meteortools-2023.4.24/ukmon_meteortools/share/
--rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
--rw-rw-rw-   0        0        0       41 2023-04-18 21:54:45.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/share/__init__.py
--rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/share/streamfulldata.npy
-drwxrwxrwx   0        0        0        0 2023-04-30 07:19:42.561211 ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/
--rw-rw-rw-   0        0        0      524 2023-04-16 21:29:05.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-04-13 21:43:11.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/apiExampleCode.py
--rw-rw-rw-   0        0        0     2317 2023-04-18 22:57:34.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/drawFTPfile.py
--rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/findNearDuplicates.py
--rw-rw-rw-   0        0        0     6386 2023-04-18 22:55:02.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/getLiveImages.py
--rw-rw-rw-   0        0        0     2984 2023-04-18 22:49:26.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/getOverlappingFovs.py
--rw-rw-rw-   0        0        0     3253 2023-04-18 22:44:54.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/plotTrack.py
--rw-rw-rw-   0        0        0     2369 2023-04-18 22:43:12.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/retrieveECSV.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:19:42.574219 ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/
--rw-rw-rw-   0        0        0    13528 2023-04-12 22:11:48.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/Math.py
--rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/VectorMaths.py
--rw-rw-rw-   0        0        0     1536 2023-04-29 16:46:55.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/__init__.py
--rw-rw-rw-   0        0        0     2494 2023-04-18 20:38:58.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/annotateImage.py
--rw-rw-rw-   0        0        0     1298 2023-04-18 21:00:49.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/convertSolLon.py
--rw-rw-rw-   0        0        0     2088 2023-04-18 20:58:02.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/getActiveShowers.py
--rw-rw-rw-   0        0        0     3525 2023-04-18 13:55:45.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/getShowerDates.py
--rw-rw-rw-   0        0        0     3988 2023-04-29 16:41:40.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/kmlHandlers.py
--rw-rw-rw-   0        0        0     3668 2023-04-29 17:26:52.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/sendAnEmail.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:19:42.505210 ukmon_meteortools-2023.4.24/ukmon_meteortools.egg-info/
--rw-rw-rw-   0        0        0    42683 2023-04-30 07:19:42.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1716 2023-04-30 07:19:42.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 07:19:42.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      265 2023-04-30 07:19:42.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-30 07:19:42.000000 ukmon_meteortools-2023.4.24/ukmon_meteortools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.289585 ukmon_meteortools-2023.5.0/
+-rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.5.0/LICENSE
+-rw-rw-rw-   0        0        0    42659 2023-05-03 14:23:35.287574 ukmon_meteortools-2023.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.5.0/README.md
+-rw-rw-rw-   0        0        0     2204 2023-05-03 14:23:10.000000 ukmon_meteortools-2023.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 14:23:35.289585 ukmon_meteortools-2023.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.202576 ukmon_meteortools-2023.5.0/ukmon_meteortools/
+-rw-rw-rw-   0        0        0      756 2023-05-02 21:24:36.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.240574 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/
+-rw-rw-rw-   0        0        0    10159 2023-05-02 20:41:26.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py
+-rw-rw-rw-   0        0        0     6742 2023-05-02 20:41:44.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/ReadUFOCapXML.py
+-rw-rw-rw-   0        0        0      428 2023-05-02 20:42:29.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/__init__.py
+-rw-rw-rw-   0        0        0    19243 2023-05-02 20:13:35.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/ftpDetectInfo.py
+-rw-rw-rw-   0        0        0     7393 2023-05-02 21:34:25.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/imoWorkingShowerList.py
+-rw-rw-rw-   0        0        0     2948 2023-05-02 20:46:56.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/platepar.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.249574 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/
+-rw-rw-rw-   0        0        0      660 2023-05-02 20:33:20.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
+-rw-rw-rw-   0        0        0     6077 2023-05-02 20:34:59.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/multiDayRadiant.py
+-rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/multiEventGroundMap.py
+-rw-rw-rw-   0        0        0     5242 2023-05-03 14:21:56.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/multiTrackStack.py
+-rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
+-rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/plotRMSOrbits.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.253577 ukmon_meteortools-2023.5.0/ukmon_meteortools/share/
+-rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
+-rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/share/__init__.py
+-rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/share/streamfulldata.npy
+drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.272584 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/
+-rw-rw-rw-   0        0        0      524 2023-04-16 21:29:05.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/__init__.py
+-rw-rw-rw-   0        0        0     2088 2023-05-03 14:21:17.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/apiExampleCode.py
+-rw-rw-rw-   0        0        0     2476 2023-05-02 20:12:42.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/drawFTPfile.py
+-rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/findNearDuplicates.py
+-rw-rw-rw-   0        0        0     5670 2023-05-03 14:21:17.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/getLiveImages.py
+-rw-rw-rw-   0        0        0     3238 2023-05-02 20:18:14.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/getOverlappingFovs.py
+-rw-rw-rw-   0        0        0     3589 2023-05-02 20:20:03.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/plotTrack.py
+-rw-rw-rw-   0        0        0     2385 2023-05-02 20:58:19.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/retrieveECSV.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.286574 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/
+-rw-rw-rw-   0        0        0    13798 2023-05-02 20:57:25.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/Math.py
+-rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/VectorMaths.py
+-rw-rw-rw-   0        0        0     1411 2023-05-02 21:38:00.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-05-02 21:35:02.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/annotateImage.py
+-rw-rw-rw-   0        0        0     1313 2023-05-02 21:35:22.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/convertSolLon.py
+-rw-rw-rw-   0        0        0     2114 2023-05-02 21:35:49.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/getActiveShowers.py
+-rw-rw-rw-   0        0        0     3937 2023-05-02 21:41:36.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/getShowerDates.py
+-rw-rw-rw-   0        0        0     5117 2023-05-02 21:11:53.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/kmlHandlers.py
+-rw-rw-rw-   0        0        0     3699 2023-05-02 20:49:10.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/sendAnEmail.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:23:35.231573 ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/
+-rw-rw-rw-   0        0        0    42659 2023-05-03 14:23:35.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1716 2023-05-03 14:23:35.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 14:23:35.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      263 2023-05-03 14:23:35.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-03 14:23:35.000000 ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/top_level.txt
```

### Comparing `ukmon_meteortools-2023.4.24/LICENSE` & `ukmon_meteortools-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.24/PKG-INFO` & `ukmon_meteortools-2023.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon_meteortools
-Version: 2023.4.24
+Version: 2023.5.0
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -687,15 +687,14 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # ukmon_meteortools
-## Version 2023.04.24
 
 Python tools and utilities to work with meteor data from the UK Meteor Network
 
 To get more information about the submodules and functions use Python's built-in help capability
 
 ``` python
 from ukmon_meteortools import utils
```

### Comparing `ukmon_meteortools-2023.4.24/README.md` & `ukmon_meteortools-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.24/pyproject.toml` & `ukmon_meteortools-2023.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ukmon_meteortools"
-version = "2023.04.24"
+version = "2023.05.0"
 description = "Python Tools for Meteor Data Analysis"
 readme = "ukmon_meteortools/README.md"
 authors = [{ name = "Mark McIntyre", email = "ukmon@markmcintyreastro.co.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -36,20 +36,21 @@
     "Shapely",
     "simplekml",
     "s3fs",
     "xmltodict",
     "requests",
     "pytest",
     "pyproj",
+    "pdoc",
     "Cython"
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
-dev = ["bumpver", "gitpython", "behave", "pip-tools", "pytest"]
+dev = ["bumpver", "gitpython", "behave", "pip-tools"]
 
 [project.urls]
 "Homepage" = "https://github.com/markmac99/UKMon-shared/ukmon_meteortools/"
 "Bug Tracker" = "https://github.com/markmac99/UKMon-shared/issues"
 
 #[project.scripts]
 #realpython = "reader.__main__:main"
@@ -63,19 +64,19 @@
 #[tool.setuptools.packages.find]
 #where = ["ukmon_meteortools"]
 
 [tool.setuptools.package-data]
 "*" = ["*.npy", "*.xml"]
 
 [tool.bumpver]
-current_version = "2023.04.24"
+current_version = "2023.05.0"
 version_pattern = "YYYY.0M.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['version = "{version}"',]
 "ukmon_meteortools/__init__.py" = ["{version}",]
-"ukmon_meteortools/README.md" = ["{version}",]
+#"ukmon_meteortools/README.md" = ["{version}",]
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/README.md` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # ukmon_meteortools
-## Version 2023.04.24
 
 Python tools and utilities to work with meteor data from the UK Meteor Network
 
 To get more information about the submodules and functions use Python's built-in help capability
 
 ``` python
 from ukmon_meteortools import utils
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/ReadUFOAnalyzerXML.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,167 +6,88 @@
 import datetime
 import math
 import numpy
 from ukmon_meteortools.utils import datetime2JD, altAz2RADec
 
 
 class UAXml:
+    """" Load and manage a UFO-Analyser XML file containing meteor detections """
     def __init__(self, fname):
-        """Construct the object from a filename
-
-        Arguments:
-            fname string -- The full path and filename to the XML file
-        """
+        """Construct a UAxml object from fname"""
         with open(fname) as fd:
             self.uaxml = xmltodict.parse(fd.read())
 
     def getDateTime(self):
         y, m, d = UAXml.getDateYMD(self)
         h, mi, s = UAXml.getTimeHMS(self)
         ss = int(math.floor(s))
         ms = int((s - ss) * 1000000)
 
         dtim = datetime.datetime(y, m, d, h, mi, ss, ms)
         return dtim
 
     def getDate(self):
-        """ Get the event date as an int
-
-        Returns:
-            int -- date as YYYYMMDD
-        """
         ur = self.uaxml['ufoanalyzer_record']
         return int(ur['@y']) * 10000 + int(ur['@mo']) * 100 + int(ur['@d'])
 
     def getDateYMD(self):
-        """Get the event date as a tuple y,n,d
-
-        Returns:
-            int -- year
-            int -- month
-            int -- day
-        """
         yr = int(self.uaxml['ufoanalyzer_record']['@y'])
         mo = int(self.uaxml['ufoanalyzer_record']['@mo'])
         dy = int(self.uaxml['ufoanalyzer_record']['@d'])
         return yr, mo, dy
 
     def getDateStr(self):
-        """get the event date as a string
-        Returns:
-            string -- YYYY-MM-DD
-        """
         ur = self.uaxml['ufoanalyzer_record']
         return ur['@y'] + "-" + ur['@mo'] + "-" + ur['@d']
 
     def getTime(self):
-        """Get the time as a number of seconds since midnight
-
-        Returns:
-            int -- secs
-        """
         ur = self.uaxml['ufoanalyzer_record']
         return int(ur['@h']) * 3600 + int(ur['@m']) * 60 + float(ur['@s'])
 
     def getTimeStr(self):
-        """Get time as a string
-
-        Returns:
-            string -- hh:mm:ss.sss
-        """
         ur = self.uaxml['ufoanalyzer_record']
         return ur['@h'] + ":" + ur['@m'] + ":" + ur['@s']
 
     def getTimeHMS(self):
-        """Get time as H,M and S
-
-        Returns:
-            int -- hour
-            int -- minute
-            float -- seconds and milliseconds
-        """
         h = int(self.uaxml['ufoanalyzer_record']['@h'])
         m = int(self.uaxml['ufoanalyzer_record']['@m'])
         s = float(self.uaxml['ufoanalyzer_record']['@s'])
         return h, m, s
 
     def getCameraDetails(self):
-        """Get basic camera details
-
-        Returns:
-            float -- frames per second
-            float -- horizontal resolution cx
-            float -- vertical resolution cy
-        """
         fps = float(self.uaxml['ufoanalyzer_record']['@fps'])
         cx = float(self.uaxml['ufoanalyzer_record']['@cx'])
         cy = float(self.uaxml['ufoanalyzer_record']['@cy'])
         isintl = int(self.uaxml['ufoanalyzer_record']['@interlaced'])
         return fps, cx, cy, isintl
 
     def getStationDetails(self):
-        """Get station details
-
-        Returns:
-            string -- station name eg TACKLEY_TC
-            string -- LID eg TACKLEY
-            string -- SID eg TC
-            float -- latitude
-            float -- longitude (W negative)
-            float -- altitude (metres)
-        """
         sta = self.uaxml['ufoanalyzer_record']['@lid'] + "_" + self.uaxml['ufoanalyzer_record']['@sid']
         lid = self.uaxml['ufoanalyzer_record']['@lid']
         sid = self.uaxml['ufoanalyzer_record']['@sid']
         lat = float(self.uaxml['ufoanalyzer_record']['@lat'])
         lng = float(self.uaxml['ufoanalyzer_record']['@lng'])
         alt = float(self.uaxml['ufoanalyzer_record']['@alt'])
         return sta, lid, sid, lat, lng, alt
 
     def getProfDetails(self):
-        """Get details of the profile used to determine the track
-
-        Returns:
-            float -- azimuth, elevation and rotation
-            float -- horizontal field of view in degrees
-            float -- yx, dz, dy (some fit parameters)
-            float -- number of linked stars
-        """
         az = float(self.uaxml['ufoanalyzer_record']['@az'])
         ev = float(self.uaxml['ufoanalyzer_record']['@ev'])
         rot = float(self.uaxml['ufoanalyzer_record']['@rot'])
         fovh = float(self.uaxml['ufoanalyzer_record']['@vx'])
         yx = float(self.uaxml['ufoanalyzer_record']['@yx'])
         dx = float(self.uaxml['ufoanalyzer_record']['@dx'])
         dy = float(self.uaxml['ufoanalyzer_record']['@dy'])
         lnk = float(self.uaxml['ufoanalyzer_record']['@dl'])
         return az, ev, rot, fovh, yx, dx, dy, lnk
 
     def getObjectCount(self):
-        """Returns the number of objects in this file
-
-        Returns:
-            int - number of objects
-        """
         return int(self.uaxml['ufoanalyzer_record']['@o'])
 
     def getObjectBasics(self, objno):
-        """Get basic details about an object
-
-        Arguments:
-            objno int -- the object number zero based
-
-        Returns:
-            float -- duration in seconds
-            float -- angular velocity
-            int -- pix count
-            float -- max brightness
-            float -- magnitude estimate
-            int -- number of frames with a moving object in
-        """
         uos = self.uaxml['ufoanalyzer_record']['ua2_objects']
         oc = int(self.uaxml['ufoanalyzer_record']['@o'])
         if oc == 1:
             uo = uos['ua2_object']
         else:
             uo = uos['ua2_object'][objno]
         sec = float(uo['@sec'])
@@ -174,22 +95,14 @@
         pix = int(uo['@pix'])
         bmax = float(uo['@bmax'])
         mag = float(uo['@mag'])
         fcount = int(uo['@sN'])
         return sec, av, pix, bmax, mag, fcount
 
     def getObjectStart(self, objno):
-        """Get the details of the start point of an object
-
-        Arguments:
-            objno int -- object to retrieve
-
-        Returns:
-            floats - ra, dec, height, distance, latitude and longitude
-        """
         uos = self.uaxml['ufoanalyzer_record']['ua2_objects']
         oc = int(self.uaxml['ufoanalyzer_record']['@o'])
         if oc == 1:
             uo = uos['ua2_object']
         else:
             uo = uos['ua2_object'][objno]
         ra1 = uo['@ra1']
@@ -200,22 +113,14 @@
         lat1 = uo['@lat1']
         az1 = uo['@az1']
         ev1 = uo['@ev1']
         fs = uo['@fs']
         return ra1, dc1, h1, dist1, lng1, lat1, az1, ev1, fs
 
     def getObjectEnd(self, objno):
-        """Get the details of the end point of an object
-
-        Arguments:
-            objno int -- object to retrieve
-
-        Returns:
-            floats - ra, dec, height, distance, latitude and longitude
-        """
         uos = self.uaxml['ufoanalyzer_record']['ua2_objects']
         oc = int(self.uaxml['ufoanalyzer_record']['@o'])
         if oc == 1:
             uo = uos['ua2_object']
         else:
             uo = uos['ua2_object'][objno]
         ra2 = uo['@ra2']
@@ -224,24 +129,14 @@
         dist2 = uo['@dist2']
         lng2 = uo['@lng2']
         lat2 = uo['@lat2']
         fe = uo['@fe']
         return ra2, dc2, h2, dist2, lng2, lat2, fe
 
     def getObjectFrameDetails(self, objno, fno):
-        """Get details of a specific frame
-
-        Arguments:
-            objno int -- object number
-            fno int -- frame number
-
-        Returns:
-            float -- frame no,ra, dec, magnitude, az, ev, total brightness
-            int -- b
-        """
         uos = self.uaxml['ufoanalyzer_record']['ua2_objects']
         oc = int(self.uaxml['ufoanalyzer_record']['@o'])
         if oc == 1:
             uo = uos['ua2_object']
         else:
             uo = uos['ua2_object'][objno]
         uop = uo['ua2_objpath']['ua2_fdata2'][fno]
@@ -291,14 +186,15 @@
             # the framenumber of this is stored in "fs"
             us = int((fno[fc] - fs) / fps * 1000000)
             tt[fc] = round((dtim + datetime.timedelta(microseconds=us)).timestamp(), 2)
         return fno, tt, ra, dec, mag, fcount, alt, az, b, lsum
 
 
     def makePlateParEntry(self, statid):
+        """ Make a fake platepar file from the data, so it can be processed with RMS/WMPL """
         imgdt = self.getDateTime()
         _, cx, cy, _ = self.getCameraDetails()
         az, ev, _, fovh, yx, _, _, _ = self.getProfDetails()
         _, lid, sid, lat, lng, alt = self.getStationDetails()
 
         ff_name = 'FF_' + statid +'_'
         ff_name = ff_name + imgdt.strftime('%Y%m%d_%H%M%S_')
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/fileformats/ReadUFOCapXML.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/ReadUFOCapXML.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 
 import xmltodict
 import numpy
 
 
 class UCXml:
+    """ Load and manage a UFOCapture XML file containing potential detections """
     MAXGAP = 50
 
     def setMaxGap(self, mg):
         self.MAXGAP = mg
 
     def __init__(self, fname):
+        """ Construct a UCXML object from fname """
         with open(fname) as fd:
             self.ucxml = xmltodict.parse(fd.read())
 
     def getDate(self):
         ur = self.ucxml['ufocapture_record']
         return int(ur['@y']) * 10000 + int(ur['@mo']) * 100 + int(ur['@d'])
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/fileformats/ftpDetectInfo.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/ftpDetectInfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,121 +9,25 @@
 import configparser as crp
 import json
 import datetime
 
 from ukmon_meteortools.utils import date2JD, angleBetweenSphericalCoords
 
 
-class MeteorObservation(object):
-    """ Container for meteor observations. Lifted from WMPL
-        
-        The points in arrays are RA and Dec in J2000 epoch, in radians.
-
-        Arguments:
-            jdt_ref: [float] Reference Julian date when the relative time is t = 0s.
-            station_id: [str] Station ID.
-            latitude: [float] Latitude +N in radians.
-            longitude: [float] Longitude +E in radians.
-            height: [float] Elevation above sea level (MSL) in meters.
-            fps: [float] Frames per second.
-
-        Keyword arguments:
-            ff_name: [str] Name of the originating FF file.
-
-    """
-    def __init__(self, jdt_ref, station_id, latitude, longitude, height, fps, ff_name=None):
-
-        self.jdt_ref = jdt_ref
-        self.station_id = station_id
-        self.latitude = latitude
-        self.longitude = longitude
-        self.height = height
-        self.fps = fps
-
-        self.ff_name = ff_name
-
-        self.frames = []
-        self.time_data = []
-        self.x_data = []
-        self.y_data = []
-        self.azim_data = []
-        self.elev_data = []
-        self.ra_data = []
-        self.dec_data = []
-        self.mag_data = []
-        self.abs_mag_data = []
-
-
-
-    def addPoint(self, frame_n, x, y, azim, elev, ra, dec, mag):
-        """ Adds the measurement point to the meteor.
-
-        Arguments:
-            frame_n: [flaot] Frame number from the reference time.
-            x: [float] X image coordinate.
-            y: [float] X image coordinate.
-            azim: [float] Azimuth, J2000 in degrees.
-            elev: [float] Elevation angle, J2000 in degrees.
-            ra: [float] Right ascension, J2000 in degrees.
-            dec: [float] Declination, J2000 in degrees.
-            mag: [float] Visual magnitude.
-
-        """
-
-        self.frames.append(frame_n)
-
-        # Calculate the time in seconds w.r.t. to the reference JD
-        point_time = float(frame_n)/self.fps
-
-        self.time_data.append(point_time)
-
-        self.x_data.append(x)
-        self.y_data.append(y)
-
-        # Angular coordinates converted to radians
-        self.azim_data.append(np.radians(azim))
-        self.elev_data.append(np.radians(elev))
-        self.ra_data.append(np.radians(ra))
-        self.dec_data.append(np.radians(dec))
-        self.mag_data.append(mag)
-
-
-
-    def finish(self):
-        """ When the initialization is done, convert data lists to numpy arrays. """
-
-        self.frames = np.array(self.frames)
-        self.time_data = np.array(self.time_data)
-        self.x_data = np.array(self.x_data)
-        self.y_data = np.array(self.y_data)
-        self.azim_data = np.array(self.azim_data)
-        self.elev_data = np.array(self.elev_data)
-        self.ra_data = np.array(self.ra_data)
-        self.dec_data = np.array(self.dec_data)
-        self.mag_data = np.array(self.mag_data)
-
-        # Sort by frame
-        temp_arr = np.c_[self.frames, self.time_data, self.x_data, self.y_data, self.azim_data, 
-        self.elev_data, self.ra_data, self.dec_data, self.mag_data]
-        temp_arr = temp_arr[np.argsort(temp_arr[:, 0])]
-        self.frames, self.time_data, self.x_data, self.y_data, self.azim_data, self.elev_data, self.ra_data, \
-            self.dec_data, self.mag_data = temp_arr.T
-
-
 def filterFTPforSpecificTime(ftpfile, dtstr):
-    """ filter FTPdetect file for a specific event, by time, and copy it into a new file
+    """ filter FTPdetect file for a specific event, by time, and copy it into a new file  
 
-    Arguments:
-        ftpfile - [string] full path to the ftpdetect file to filter
-        dtstr   - [string] date/time of required event in yyyymmdd_hhmmss format
-
-    Returns:
-        tuple containing 
-            full name of the new file containing just matching events
-            the number of matching events
+    Arguments:  
+        ftpfile - [string] full path to the ftpdetect file to filter  
+        dtstr   - [string] date/time of required event in yyyymmdd_hhmmss format  
+
+    Returns:  
+        tuple containing  
+            full name of the new file containing just matching events  
+            the number of matching events  
     """
     meteor_list = loadFTPDetectInfo(ftpfile, time_offsets=None, join_broken_meteors=True, locdata=None)
     refdt = datetime.datetime.strptime(dtstr, '%Y%m%d_%H%M%S')
     #print(refdt)
     new_met_list = []
     for met in meteor_list:
         #print(met.ff_name)
@@ -134,136 +38,69 @@
             print('adding one entry')
             new_met_list.append(met)
     newname = writeNewFTPFile(ftpfile, new_met_list)
     return newname, len(new_met_list)
 
 
 def writeNewFTPFile(srcname, metlist):
-    """ creates an FTPDetect file from a list of MeteorObservation objects 
-
-    This function creates a replacement FTPdetect file 
-    
-    Arguments:
-        srcname     - [string] full path to the original FTP file
-        metlist     - list of MeteorObservation objects
+    """ creates a FTPDetect file from a list of MeteorObservation objects  
+        
+    Arguments: 
+        srcname     - [string] full path to the original FTP file  
+        metlist     - list of MeteorObservation objects  
 
-    Returns:
-        the full path to the created file
+    Returns: 
+        the full path to the created file 
 
     """
     outdir, fname = os.path.split(srcname)
     newname = os.path.join(outdir, f'{fname}.old')
     try:
         os.rename(srcname, newname)
     except:
         pass
     if os.path.isfile(srcname):
         srcname = srcname[:-4] + '_new.txt'
     with open(srcname, 'w') as ftpf:
-        writeFTPHeader(ftpf, len(metlist), outdir, False)
+        _writeFTPHeader(ftpf, len(metlist), outdir, False)
         metno = 1
         ffname = ''
         for met in metlist:
             if ffname == met.ff_name:
                 metno = metno + 1
             else:
                 metno = 1
                 ffname = met.ff_name
-            writeOneMeteor(ftpf, metno, met.station_id, met.time_data, len(met.frames), met.fps, met.frames, 
+            _writeOneMeteor(ftpf, metno, met.station_id, met.time_data, len(met.frames), met.fps, met.frames, 
                 np.degrees(met.ra_data), np.degrees(met.dec_data), 
                 np.degrees(met.azim_data), np.degrees(met.elev_data),
                 None, met.mag_data, False, met.x_data, met.y_data, met.ff_name)
     return srcname
 
 
-def writeFTPHeader(ftpf, metcount, fldr, ufo=True):
-    """
-    Create the header of the FTPDetect file
-    """
-    l1 = 'Meteor Count = {:06d}\n'.format(metcount)
-    ftpf.write(l1)
-    ftpf.write('-----------------------------------------------------\n')
-    if ufo is True:
-        ftpf.write('Processed with UFOAnalyser\n')
-    else:
-        ftpf.write('Processed with RMS 1.0\n')
-    ftpf.write('-----------------------------------------------------\n')
-    l1 = 'FF  folder = {:s}\n'.format(fldr)
-    ftpf.write(l1)
-    l1 = 'CAL folder = {:s}\n'.format(fldr)
-    ftpf.write(l1)
-    ftpf.write('-----------------------------------------------------\n')
-    ftpf.write('FF  file processed\n')
-    ftpf.write('CAL file processed\n')
-    ftpf.write('Cam# Meteor# #Segments fps hnr mle bin Pix/fm Rho Phi\n')
-    ftpf.write('Per segment:  Frame# Col Row RA Dec Azim Elev Inten Mag\n')
-
-
-def writeOneMeteor(ftpf, metno, sta, evttime, fcount, fps, fno, ra, dec, az, alt, b, mag, 
-        ufo=True, x=None, y=None, ffname = None):
-    """
-    Write one meteor event into the file in FTPDetectInfo style
-    """
-    ftpf.write('-------------------------------------------------------\n')
-    if ffname is None:
-        ms = '{:03d}'.format(int(evttime.microsecond / 1000))
-
-        fname = 'FF_' + sta + '_' + evttime.strftime('%Y%m%d_%H%M%S_') + ms + '_0000000.fits\n'
-    else:
-        fname = ffname + '\n'
-    ftpf.write(fname)
-
-    if ufo is True:
-        ftpf.write('UFO UKMON DATA Recalibrated on: ')
-    else:
-        ftpf.write('RMS data reprocessed on: ')
-    ftpf.write(datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S.%f UTC\n'))
-    li = f'{sta} {metno:04d} {fcount:04d} {fps:04.2f} 000.0 000.0  00.0 000.0 0000.0 0000.0\n'
-    ftpf.write(li)
-
-    for i in range(len(fno)):
-        #    204.4909 0422.57 0353.46 262.3574 +16.6355 267.7148 +23.0996 000120 3.41
-        bri = 0
-        if b is not None:
-            bri = int(b[i])
-        if ufo is True:
-            # UFO is timestamped as at the first detection
-            thisfn = fno[i] - fno[0]
-            thisx = 0
-            thisy = 0
-        else:
-            thisfn = fno[i]
-            thisx = x[i]
-            thisy = y[i]
-        li = f'{thisfn:.4f} {thisx:07.2f} {thisy:07.2f} '
-        li = li + f'{ra[i]:8.4f} {dec[i]:+7.4f} {az[i]:8.4f} '
-        li = li + f'{alt[i]:+7.4f} {bri:06d} {mag[i]:.02f}\n'
-        ftpf.write(li)
-
-
 def loadFTPDetectInfo(ftpdetectinfo_file_name, time_offsets=None,
         join_broken_meteors=True, locdata=None):
-    """ Loads an FTPDEtect file into a list of MeteorObservation objects
+    """ Loads an FTPDEtect file into a list of MeteorObservation objects  
 
-    Arguments:
-        ftpdetectinfo_file_name: [str] Path to the FTPdetectinfo file.
-        stations: [dict] A dictionary where the keys are stations IDs, and values are lists of:
-            - latitude +N in radians
-            - longitude +E in radians
-            - height in meters
+    Arguments:  
+        ftpdetectinfo_file_name: [str] Path to the FTPdetectinfo file.  
+        stations: [dict] A dictionary where the keys are stations IDs, and values are lists of:  
+            - latitude +N in radians  
+            - longitude +E in radians  
+            - height in meters  
         
 
-    Keyword arguments:
+    Keyword arguments:  
         time_offsets: [dict] (key, value) pairs of (stations_id, time_offset) for every station. None by 
             default.
         join_broken_meteors: [bool] Join meteors broken across 2 FF files.
 
 
-    Return:
-        meteor_list: [list] A list of MeteorObservation objects filled with data from the FTPdetectinfo file.
+    Return:  
+        meteor_list: [list] A list of MeteorObservation objects filled with data from the FTPdetectinfo file.  
 
     """
     stations={}
     if locdata is None:
         dirname, fname = os.path.split(ftpdetectinfo_file_name)
         cfgfile = os.path.join(dirname, '.config')
         cfg = crp.ConfigParser()
@@ -425,19 +262,19 @@
                         mag = None
                     else:
                         mag = float(mag)
                 else:
                     mag = None
 
                 # Add the measurement point to the current meteor 
-                current_meteor.addPoint(frame_n, x, y, azim, elev, ra, dec, mag)
+                current_meteor._addPoint(frame_n, x, y, azim, elev, ra, dec, mag)
 
         # Add the last meteor the the meteor list
         if current_meteor is not None:
-            current_meteor.finish()
+            current_meteor._finish()
             meteor_list.append(current_meteor)
 
     # Concatenate observations across different FF files ###
     if join_broken_meteors:
 
         # Go through all meteors and compare the next observation
         merged_indices = []
@@ -520,14 +357,159 @@
 
         # Removed merged meteors from the list
         meteor_list = [element for i, element in enumerate(meteor_list) if i not in merged_indices]
 
     return meteor_list
 
 
+class MeteorObservation(object):
+    """ Container for meteor observations.  
+    """
+    def __init__(self, jdt_ref, station_id, latitude, longitude, height, fps, ff_name=None):
+        """ Construct the MeteorObservation object.  
+        Arguments:  
+            jdt_ref: [float] Reference Julian date when the relative time is t = 0s.  
+            station_id: [str] Station ID.  
+            latitude: [float] Latitude +N in radians.  
+            longitude: [float] Longitude +E in radians.  
+            height: [float] Elevation above sea level (MSL) in meters. 
+            fps: [float] Frames per second. 
+
+        Keyword arguments:  
+            ff_name: [str] Name of the originating FF file. 
+        """
+        self.jdt_ref = jdt_ref
+        self.station_id = station_id
+        self.latitude = latitude
+        self.longitude = longitude
+        self.height = height
+        self.fps = fps
+        self.ff_name = ff_name
+        self.frames = []
+        self.time_data = []
+        self.x_data = []
+        self.y_data = []
+        self.azim_data = []
+        self.elev_data = []
+        self.ra_data = []
+        self.dec_data = []
+        self.mag_data = []
+        self.abs_mag_data = []
+
+    def _addPoint(self, frame_n, x, y, azim, elev, ra, dec, mag):
+        """ Adds the measurement point to the meteor.
+
+        Arguments:
+            frame_n: [flaot] Frame number from the reference time.
+            x: [float] X image coordinate.
+            y: [float] X image coordinate.
+            azim: [float] Azimuth, J2000 in degrees.
+            elev: [float] Elevation angle, J2000 in degrees.
+            ra: [float] Right ascension, J2000 in degrees.
+            dec: [float] Declination, J2000 in degrees.
+            mag: [float] Visual magnitude.
+        """
+        self.frames.append(frame_n)
+
+        # Calculate the time in seconds w.r.t. to the reference JD
+        point_time = float(frame_n)/self.fps
+        self.time_data.append(point_time)
+        self.x_data.append(x)
+        self.y_data.append(y)
+
+        # Angular coordinates converted to radians
+        self.azim_data.append(np.radians(azim))
+        self.elev_data.append(np.radians(elev))
+        self.ra_data.append(np.radians(ra))
+        self.dec_data.append(np.radians(dec))
+        self.mag_data.append(mag)
+
+    def _finish(self):
+        """ When the initialization is done, convert data lists to numpy arrays. """
+        self.frames = np.array(self.frames)
+        self.time_data = np.array(self.time_data)
+        self.x_data = np.array(self.x_data)
+        self.y_data = np.array(self.y_data)
+        self.azim_data = np.array(self.azim_data)
+        self.elev_data = np.array(self.elev_data)
+        self.ra_data = np.array(self.ra_data)
+        self.dec_data = np.array(self.dec_data)
+        self.mag_data = np.array(self.mag_data)
+        # Sort by frame
+        temp_arr = np.c_[self.frames, self.time_data, self.x_data, self.y_data, self.azim_data, 
+        self.elev_data, self.ra_data, self.dec_data, self.mag_data]
+        temp_arr = temp_arr[np.argsort(temp_arr[:, 0])]
+        self.frames, self.time_data, self.x_data, self.y_data, self.azim_data, self.elev_data, self.ra_data, \
+            self.dec_data, self.mag_data = temp_arr.T
+
+
+def _writeFTPHeader(ftpf, metcount, fldr, ufo=True):
+    """
+    Internal function to create the header of the FTPDetect file  
+    """
+    l1 = 'Meteor Count = {:06d}\n'.format(metcount)
+    ftpf.write(l1)
+    ftpf.write('-----------------------------------------------------\n')
+    if ufo is True:
+        ftpf.write('Processed with UFOAnalyser\n')
+    else:
+        ftpf.write('Processed with RMS 1.0\n')
+    ftpf.write('-----------------------------------------------------\n')
+    l1 = 'FF  folder = {:s}\n'.format(fldr)
+    ftpf.write(l1)
+    l1 = 'CAL folder = {:s}\n'.format(fldr)
+    ftpf.write(l1)
+    ftpf.write('-----------------------------------------------------\n')
+    ftpf.write('FF  file processed\n')
+    ftpf.write('CAL file processed\n')
+    ftpf.write('Cam# Meteor# #Segments fps hnr mle bin Pix/fm Rho Phi\n')
+    ftpf.write('Per segment:  Frame# Col Row RA Dec Azim Elev Inten Mag\n')
+
+
+def _writeOneMeteor(ftpf, metno, sta, evttime, fcount, fps, fno, ra, dec, az, alt, b, mag, 
+        ufo=True, x=None, y=None, ffname = None):
+    """   Internal function to write one meteor event into the file in FTPDetectInfo style
+    """
+    ftpf.write('-------------------------------------------------------\n')
+    if ffname is None:
+        ms = '{:03d}'.format(int(evttime.microsecond / 1000))
+
+        fname = 'FF_' + sta + '_' + evttime.strftime('%Y%m%d_%H%M%S_') + ms + '_0000000.fits\n'
+    else:
+        fname = ffname + '\n'
+    ftpf.write(fname)
+
+    if ufo is True:
+        ftpf.write('UFO UKMON DATA Recalibrated on: ')
+    else:
+        ftpf.write('RMS data reprocessed on: ')
+    ftpf.write(datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S.%f UTC\n'))
+    li = f'{sta} {metno:04d} {fcount:04d} {fps:04.2f} 000.0 000.0  00.0 000.0 0000.0 0000.0\n'
+    ftpf.write(li)
+
+    for i in range(len(fno)):
+        #    204.4909 0422.57 0353.46 262.3574 +16.6355 267.7148 +23.0996 000120 3.41
+        bri = 0
+        if b is not None:
+            bri = int(b[i])
+        if ufo is True:
+            # UFO is timestamped as at the first detection
+            thisfn = fno[i] - fno[0]
+            thisx = 0
+            thisy = 0
+        else:
+            thisfn = fno[i]
+            thisx = x[i]
+            thisy = y[i]
+        li = f'{thisfn:.4f} {thisx:07.2f} {thisy:07.2f} '
+        li = li + f'{ra[i]:8.4f} {dec[i]:+7.4f} {az[i]:8.4f} '
+        li = li + f'{alt[i]:+7.4f} {bri:06d} {mag[i]:.02f}\n'
+        ftpf.write(li)
+
+
 if __name__ == '__main__':
     if len(sys.argv) < 1:
         print('usage: python ftpDetectInfo.py ftpfile')
         print('note: requires .config and platepar to be in the same folder')
         exit(0)
         
     ftpname = sys.argv[1]
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/fileformats/imoWorkingShowerList.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/imoWorkingShowerList.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,25 +15,22 @@
 except:
     majorlist = ['QUA', 'LYR', 'ETA', 'CAP', 'SDA', 'PER', 'AUR', 'ORI', 'NTA', 'STA', 'LEO', 'GEM', 'URS']
     minorlist = ['SPE','OCT','DRA','EGE','MON','HYD','COM','NOO']
 
 
 class IMOshowerList:
     """
-    Class that loads and parses the IMO Working Shower list XML file
+    Class that loads and parses the IMO Working Shower list, or if needed, the unconfirmed list. 
+    Not all known showers are in the IMO working list. If a shower is not in the Working List then 
+    this library will reference the full shower list curated by Peter Jenniskens which contains 
+    debated and unconfirmed showers. 
 
-    Notes:
-        During initialisation the class attempt to load IMO_Working_Meteor_Shower_list.xml from
-        $DATADIR/share, if it exists and if DATADIR is defined in your environment. Failing this,
-        it will use a reference copy that is distributed with this library. If you want to force
-        the library to use a newer version, define DATADIR and put the file in $DATADIR/share.
-
-        Not all known showers are in the IMO working list. If a shower is not in the Working List then 
-        this library will reference the full shower list curated by Peter Jenniskens. 
-        This contains debated and unconfirmed showers. 
+    These list are updated whenever the library version is bumped, but if you want to override the files, define an 
+    environment variable DATADIR, and place your own copies of the files at $DATADIR/share. See the share submodule 
+    for more information. 
 
     """
     def __init__(self, fname=None, fullstreamname=None):
         if fname is None:
             datadir = os.getenv('DATADIR', default='/home/ec2-user/prod/data')
             fname = os.path.join(datadir, '..', 'share', 'IMO_Working_Meteor_Shower_List.xml')
             if not os.path.isfile(fname):
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/fileformats/platepar.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/fileformats/platepar.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 import json
 import os
 import glob
 
 
 class platepar:
+    """ Load and manage an RMS platepar object, used to map an image to the sky """
     def __init__(self, plateparfile):
+        """" Create and load a platepar object from a file plateparfile """
         with open(plateparfile, 'r') as pp:
             self.jsd = json.load(pp)
             try: 
                 self.id = self.jsd['station_code']
                 # field of view details
                 self.alt_centre = self.jsd['alt_centre']
                 self.az_centre = self.jsd['az_centre']
@@ -42,24 +44,35 @@
                 # FOV scale (px/deg)
                 self.F_scale = self.jsd['F_scale']
 
             except:
                 print('invalid json file')
 
     def getLocation(self):
+        """ get the lat, lon and elevation from the platepar"""
         return [self.lat, self.lon, self.elev]
 
     def getView(self):
+        """ get the pointing direction (alt/az), field of view (h/v) and rotation """
         return [self.altcentre, self.azcentre, self.fov_h, self.fov_v, self.rot]
 
     def getResolution(self):
+        """ Get the reported camera resolution """
         return [self.xres, self.yres]
 
 
 def loadPlatepars(fldr):
+    """ Create a dictionary of multiple platepars  
+    
+    Arguments:  
+        fldr:   [string] A folder containing one or more platepar files  
+
+    Returns:  
+        a json dict containing each platepar indexed by the corresponding filename  
+    """
     platepars ='{'
     pth = os.path.join(fldr, '*.json')
     pps = glob.glob(pth)
     for pp in pps:
         thispl = platepar(pp)
         if thispl is not None:
             if len(platepars) > 1: # and pp != pps[-1]:
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 #
 # analyse a UFO dataset using RMS - well, a start at it anyway ! 
 #
 import os
 import argparse
-import RMS.ConfigReader as cr
-from RMS.DetectStarsAndMeteors import detectStarsAndMeteors
+try: 
+    import RMS.ConfigReader as cr
+    from RMS.DetectStarsAndMeteors import detectStarsAndMeteors
+except:
+    print('RMS not available')
 
 
 def analyseUFOwithRMS(config, ff_directory, ff_name):
     """
-    Analyse a UFO video clip using RMS, to get a list of stars and meteors
+    Analyse a UFO video clip using RMS, to get a list of stars and meteors  
 
     Arguments:
-        config: [string] An RMS-style config file for the  UFO camera
-        ff_directory: [string] The location of the file to analyse
-        ff_name: [string] A video file to analyse. 
+        config: [string] An RMS-style config file for the  UFO camera  
+        ff_directory: [string] The location of the file to analyse  
+        ff_name: [string] A video file to analyse.   
 
-    Returns:
-        (star_list, meteor_list): tuble containing a list of stars and a list of meteors
+    Returns:  
+        (star_list, meteor_list): tuple containing a list of stars and a list of meteors  
         
-    Note: the name of the video clip must be in %Y%m%d_%H%M%S.%f format. 
+    Note: the name of the video clip must be in %Y%m%d_%H%M%S.%f format.   
     """ 
     flat_struct=None
     dark=None
     mask=None
     _, star_list, meteor_list = detectStarsAndMeteors(ff_directory, ff_name, config, flat_struct, dark, mask)
 
     return star_list, meteor_list
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/multiDayRadiant.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/multiDayRadiant.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 
 import os
 import glob
 import datetime
-from Utils.ShowerAssociation import showerAssociation
-import RMS.ConfigReader as cr
+try:
+    from Utils.ShowerAssociation import showerAssociation
+    import RMS.ConfigReader as cr
+except Exception:
+    print('RMS not available')
 import argparse
 import shutil
 
 
 def multiDayRadiant(camlist, start, end, outdir=None, shwr=None, datadir=None):
     """
-    Create a multi-day and/or multi-camera radiant map, for cameras at the same geographic location. 
+    Create a multi-day and/or multi-camera radiant map for cameras at the same geographic location. 
 
-    Arguments:
-        camlist:    [list] list of camera IDs eg ['UK0006','UK000F']
-        start:      [string] start date in YYYYMMDD format
-        end:        [string] end date in YYYYMMDD format
-        outdir:     [string] where to save the file to. Default is current directory
-        shwr:       [string] Filter by shower eg PER. Default all showers. 
-        datadir:    [string] Where to look for the data. Default f:/videos/meteorcam.
-
-    Notes:
-        The function expects data to be stored in RMS folder structures as follows
-            {datadir}/{cameraid}/ConfirmedFiles/{cameraid_date_time_*}
+    Arguments:  
+        camlist:    [list] list of camera IDs eg ['UK0006','UK000F']  
+        start:      [string] start date in YYYYMMDD format  
+        end:        [string] end date in YYYYMMDD format  
+        outdir:     [string] where to save the file to. Default is current directory  
+        shwr:       [string] Filter by shower eg PER. Default all showers.   
+        datadir:    [string] Where to look for the data. Default f:/videos/meteorcam.  
+
+    Notes:  
+        The function expects data to be stored in RMS folder structures as follows  
+            {datadir}/{cameraid}/ConfirmedFiles/{cameraid_date_time_*}  
 
-        Each folder must contain FTPdetectinfo file, platepars_all file
-        The first-named folder must contain a valid RMS config file. 
+        Each folder must contain an FTPdetectinfo file and a platepars_all file. 
+        The first-named folder must contain a valid RMS config file.  
 
-        It is assumed that all cameras are at the same location. The output for cameras
-        at different locations has not been tested. 
+        It is assumed that all cameras are at the same location. The output for cameras 
+        at different locations has not been tested.  
 
     Output:
         creates two files in outdir, a PNG containing an all-sky image of the radiants and 
         meteor tracks, and a text file containing the same information
 
     """
     if datadir is None:
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/multiEventGroundMap.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/multiEventGroundMap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 
 import datetime
 import pandas as pd
 import argparse
 import os
 import matplotlib.pyplot as plt
-from wmpl.Utils.PlotMap_OSM import OSMMap
+try:
+    from wmpl.Utils.PlotMap_OSM import OSMMap
+except:
+    print('WMPL not available')
 
 RAD2DEG=57.2958
 
 
 def multiEventGroundMap(startdt, enddt, statid=None, shwr=None, outdir=None):
     """
-    Plots a ground track diagram of all events between two dates, with filters by station and shower
+    Plots a ground track diagram of all events between two dates, with filters by station and shower  
 
-    Arguments:
-        start:      [string] start date in YYYYMMDD format
-        end:        [string] end date in YYYYMMDD format
-        statid:     [string] station to filter for. Default all stations. 
-        shwr:       [string] Filter by shower eg PER. Default All showers. 
-        outdir:     [string] where to save the file to. if this parameter is omitted, the image will be displayed not saved
+    Arguments:  
+        start:      [string] start date in YYYYMMDD format  
+        end:        [string] end date in YYYYMMDD format  
+        statid:     [string] station to filter for. Default all stations.  
+        shwr:       [string] Filter by shower eg PER. Default All showers.  
+        outdir:     [string] where to save the file to. if this parameter is omitted, the image will be displayed not saved  
 
-    Output:
-        A jpg map of the detections. 
+    Output:  
+        A jpg map of the detections.   
+
+    Note:  
+        This function reads directly from the UKMON public dataset.  
 
     """
     yr = startdt[:4]
 
     cols=['_lat1', '_lng1','_lat2','_lng2','_stream','dtstamp', 'stations']
     matchfile = f'https://archive.ukmeteornetwork.co.uk/browse/parquet/matches-full-{yr}.parquet.snap'
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/multiTrackStack.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/multiTrackStack.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 
 # python script to call TrackStack to stack several nights/cameras
 
 import os
 import glob
 import datetime
-from Utils.TrackStack import trackStack
-import RMS.ConfigReader as cr
 import argparse
+try:
+    from Utils.TrackStack import trackStack
+    import RMS.ConfigReader as cr
+except Exception:
+    print('RMS not available')
 
 
 def multiTrackStack(camlist, start, end, outdir=None, shwr=None, scale=None, draw_cons=False, noplot=True, datadir=None):
     """
-    create a multi camera and/or multi night trackstack
+    create a multi camera and/or multi night trackstack  
 
-    Arguments:
-        camlist: a list of one or more cameras 
-        start: start date as a string yyyymmdd 
-        end: end date as a string yyyymmdd 
+    Arguments:  
+        camlist:    [list] list of camera IDs eg ['UK0006','UK000F']  
+        start:      [string] start date as a string yyyymmdd  
+        end:        [string] end date as a string yyyymmdd  
     
     Keyword Arguments: 
-        camlist:    [list] list of camera IDs eg ['UK0006','UK000F']
-        shwr:       [string] filter for a specific shower eg 'PER'. Default all showers.
-        scale:      [int] scale the image to avoid cropping. Default 1.
-        draw_cons:  [bool] Draw constellation stick figures. Default false
-        noplot:     [bool] Don't display the plot, just save it. Default true
-        datadir:    [string] where to read the data from. 
-
-    Notes:
-        The function expects data to be stored in RMS folder structures as follows
-            {datadir}/{cameraid}/ConfirmedFiles/{cameraid_date_time_*}
+        outdir:     [string] where to save to. Default current working directory.  
+        shwr:       [string] filter for a specific shower eg 'PER'. Default all showers.  
+        scale:      [int] scale the image to avoid cropping. Default 1.  
+        draw_cons:  [bool] Draw constellation stick figures. Default false.  
+        noplot:     [bool] Don't display the plot, just save it. Default true.  
+        datadir:    [string] Root of where to read the data from.   
+
+    Notes:  
+        The function expects data to be stored in RMS folder structures as follows  
+            {datadir}/{cameraid}/ConfirmedFiles/{cameraid_date_time_*}  
 
-        Each folder must contain FTPdetectinfo file, platepars_all file and FITS files
-        The first-named folder must contain a valid RMS config file. 
+        Each folder must contain an FTPdetectinfo file and a platepars_all file. 
+        The first-named folder must contain a valid RMS config file.  
 
-        It is assumed that all cameras are at the same location. The output for cameras
-        at different locations has not been tested. 
+        It is assumed that all cameras are at the same location. The output for cameras 
+        at different locations has not been tested.  
+
+        If you find the image is being cropped, try increasing scale. This will use more memory.  
 
     """
     if datadir is None:
         locfld = os.getenv('LOCALFOLDER', default='f:/videos/meteorcam/fireballs')
         datadir, _ = os.path.split(locfld)
     if outdir is None:
         outdir = '.'
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/plotCAMSOrbits.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/plotCAMSOrbits.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 #
 # python code to plot orbits given a CAMS style Orbit Info file
 #
 
 import sys
 import os
 import datetime
-from wmpl.Utils.PlotOrbits import plotOrbits
 import matplotlib.pyplot as plt
+try:
+    from wmpl.Utils.PlotOrbits import plotOrbits
+except:
+    print('WMPL not available')
 
 
 def plotCAMSOrbits(orbitFile, outdir=None, hideplot=True):
     """
-    plots a set of orbits from CAMS data, with one line per set of osculations 
+    plots a set of orbits from CAMS data, with one line per set of osculations  
 
-    Arguments:
-        orbitFile:  [string] full path to CAMS orbit details file
-        outdir:     [string] the location to write to. defaults to folder of CAMS file
-        hideplot:   [bool] don't display the plot. Default true
+    Arguments:  
+        orbitFile:  [string] full path to CAMS orbit details file  
+        outdir:     [string] the location to write to. defaults to folder of CAMS file  
+        hideplot:   [bool] don't display the plot. Default true  
 
-    Returns:
-        none
+    Returns:  
+        none  
     """
     if outdir is None:
         outdir, _ = os.path.split(orbitFile)
     
     evttime = None
 
     # read in the data file as a list of lines
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/rmsutils/plotRMSOrbits.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/rmsutils/plotRMSOrbits.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,33 +4,36 @@
 # python code to plot orbits given a CAMS style Orbit Info file
 #
 
 import sys
 import os
 import pandas as pd
 import datetime
-from wmpl.Utils.PlotOrbits import plotOrbits
 import matplotlib.pyplot as plt
+try:
+    from wmpl.Utils.PlotOrbits import plotOrbits
+except:
+    print('WMPL not available')
 
 
 def plotRMSOrbits(orbitFile, outdir=None, hideplot=True):
     """
-    plots a set of orbits from RMS data, with one line per set of osculations 
+    plots a set of orbits from RMS data, with one line per set of osculations  
 
-    Arguments:
-        orbitFile:  [string] full path to RMS orbit details file 
-        outdir:     [string] the location to write to. defaults to folder of source file
-        hideplot:   [bool] don't display the plot. Default true
-
-    Returns:
-        none
-
-    Notes: 
-        Orbitfile should be a csv file with the following labelled columns:
-            _a, _e, _incl, _peri, _node, _datetime
+    Arguments:  
+        orbitFile:  [string] full path to RMS orbit details file   
+        outdir:     [string] the location to write to. defaults to folder of source file  
+        hideplot:   [bool] don't display the plot. Default true  
+
+    Returns:  
+        none  
+
+    Notes:   
+        Orbitfile should be a csv file with the following labelled columns:  
+            _a, _e, _incl, _peri, _node, _datetime  
 
         _datetime should be in the format YYYY-MM-DDTHH-MM-SS
 
     """
     if outdir is None:
         outdir, _ = os.path.split(orbitFile)
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/share/streamfulldata.npy` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/share/streamfulldata.npy`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/__init__.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/drawFTPfile.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/drawFTPfile.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 import sys 
 import os
 import configparser as cr 
 from matplotlib import pyplot as plt
 
 
-def readFTPfile(filename, h):
+def _readFTPfile(filename, h):
+    """ Internal function to load ftpfile into arrays """
     events = []
     with open(filename) as f:
         # Skip the header
         for i in range(11):
             next(f)
 
         for line in f:
@@ -38,31 +39,31 @@
             events.append(dta)
 
     return events
 
 
 def drawFTPFile(ftpfile, cfgfile=None):
     """
-    Creates a simple graph of an FTPdetect file, showing the locations of each meteor.
-    Useful for diagnosing false detections. 
+    Creates a simple representation of an FTPdetect file, showing the locations of each meteor trail.  
+    Its like a stack of the night's detections but in a much simpler format. Useful for diagnosing false detections.   
 
-    Arguments:
-        ftpfile:   [str] full path to the FTPdetect file.
-        cfgfile:   [str] full path to RMS config file to read image dimensions. Default is 1280x720.
+    Arguments:  
+        ftpfile:   [str] full path to the FTPdetect file.  
+        cfgfile:   [str] full path to RMS config file to read image dimensions. Default is 1280x720.  
     """
     config = cr.ConfigParser()
     config.read(cfgfile)
     if len(config) == 1: 
         width=1280
         height=720
     else:
         width = int(config['Capture']['width'])
         height = int(config['Capture']['height'])
     print('plotting field of view {}x{}'.format(width, height))
-    events = readFTPfile(ftpfile, height)
+    events = _readFTPfile(ftpfile, height)
     for ev in events: 
         plt.plot(ev['x'],ev['y'])
     pth, ftpf = os.path.split(ftpfile)
     spls = ftpf.split('_')
     outfname = f'{spls[1]}_{spls[2]}_{spls[3]}_{spls[3]}_ftpmap.png'
     plt.savefig(os.path.join(pth, outfname))
     plt.close()
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/findNearDuplicates.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/findNearDuplicates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/getLiveImages.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/getLiveImages.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,67 +2,51 @@
 #
 # python script to get all live JPGs for a specified time
 #
 import os
 import sys
 import boto3
 import datetime
-from ukmon_meteortools.fileformats import ReadUFOCapXML as ufoc
+import pandas as pd
+import requests
 
 
-def getLiveJpgs(dtstr, outdir=None, create_txt=False, buck_name=None):
+def getLiveJpgs(dtstr, outdir=None, create_txt=False):
     """
-    Retrieve live images from the ukmon website that match a pattern
+    Retrieve live images from the ukmon website that match a pattern  
 
-    Arguments:
-        dtstr:      [str] Date in YYYYMMDD_HHMMSS format. Partial strings allowed 
-        outdir:     [str] Where to save the file. Default is to create a folder named dtstr
-        create_txt: [bool] If true, create a text file containing the pattern matches
-        buck_name:  [str] S3 bucket to read. Default ukmon-live. 
+    Arguments:  
+        dtstr:      [str] Date in YYYYMMDD_HHMMSS format. Partial strings allowed  
+        outdir:     [str] Where to save the file. Default is to create a folder named dtstr  
+        create_txt: [bool] If true, create a text file containing the pattern matches  
 
-    Notes:
-        This function will fail if you do not have access to the bucket. 
+    Notes:  
+        We only keep the last few thousand live images so this function will return nothing
+        for older data. 
     """
     if outdir is None:
         outdir = dtstr
     os.makedirs(outdir, exist_ok=True)
-    if buck_name is None:
-        buck_name = os.getenv('UKMONLIVEBUCKET', default='s3://ukmon-live')[5:]
-    s3 = boto3.client('s3')
-    print(f'looking for {dtstr} in {buck_name}')
-    try:
-        x = s3.list_objects_v2(Bucket=buck_name,Prefix=f'M{dtstr}')
-        if x['KeyCount'] > 0:
-            print(f"found {x['KeyCount']} records, saving to {outdir}")
-            for k in x['Contents']:
-                key = k['Key']
-                if '.xml' in key:
-                    s3.download_file(buck_name, key, os.path.join(outdir, key))
-                    x = ufoc.UCXml(os.path.join(outdir, key))
-                    fn = x.ucxml['ufocapture_record']['@cap'].strip()
-                    os.remove(os.path.join(outdir, key))
-                    key = key.replace('.xml', 'P.jpg')
-                    if len(fn) < 5:
-                        outkey = key
-                        #spls = key.split('_')
-                        #stationid = spls[-1][:6].lower()
-                        #dtime = key[1:16]
-                        #patt = f'FF_{stationid}_{dtime}'
-                    else:
-                        outkey = fn.replace('.fits', '.jpg')
-                        #patt = fn[:26]
-                        #stationid = fn[3:9].lower()
-                    print(key)
-                    s3.download_file(buck_name, key, os.path.join(outdir, outkey))
-                    if create_txt is True:
-                        createTxtFile(key, outdir)
-        else:
-            print('no records found')
-    except:
-        print('Error accessing AWS S3 - do you have access?')
+
+    apiurl = 'https://api.ukmeteornetwork.co.uk/liveimages/getlive'
+    liveimgs = pd.read_json(f'{apiurl}?pattern={dtstr}')
+
+    weburl = 'https://live.ukmeteornetwork.co.uk/'
+
+    for _, img in liveimgs.iterrows():
+        try:
+            jpgurl = f'{weburl}{img.image_name}'
+            _download(jpgurl, outdir)
+            xmlurl = jpgurl.replace('P.jpg', '.xml')
+            _download(xmlurl, outdir)
+            print(f'retrieved {jpgurl}')
+            if create_txt:
+                _createTxtFile(img.image_name, outdir)
+        except:
+            print(f'{img.image_name} unavailable')
 
 
 def getFBFiles(patt, outdir='.'):
     """
     Retrieve fireball files from the ukmon website that match a pattern
 
     Arguments:
@@ -121,15 +105,15 @@
                         s3.download_file(buck_name, key, os.path.join(outdir, fname))
                         gotcfg = True
     except:
         print('Error accessing AWS S3 - do you have access?')
     return 
 
 
-def createTxtFile(fname, outdir='.'):
+def _createTxtFile(fname, outdir='.'):
     """
     Create a text file named after the cameraID, containing a list of fireball files 
     to be retrieved from a remote camera
 
     Arguments:
         fname:  [str] the name of the FF file to be retrieved
         outdir: [str] where to save the files. Default '.'
@@ -152,9 +136,18 @@
         os.remove(txtf)
     patt = patt.upper()
     with open(txtf,'w') as outf:
         outf.write(f'{patt}\n{patt.replace("FF_", "FR_")}\n')
     return txtf
 
 
+def _download(url, outdir):
+    get_response = requests.get(url, stream=True)
+    file_name = url.split("/")[-1]
+    with open(os.path.join(outdir, file_name), 'wb') as f:
+        for chunk in get_response.iter_content(chunk_size=4096):
+            if chunk: # filter out keep-alive new chunks
+                f.write(chunk)
+
+
 if __name__ == '__main__':
     getLiveJpgs(sys.argv[1])
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/getOverlappingFovs.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/getOverlappingFovs.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,49 +8,57 @@
 
 from ukmon_meteortools.utils import munchKML
 from shapely.geometry import Point
 
 
 def pointInsideFov(latDegs,lngDegs, kmlFilename):
     """
-    Test if a point is inside the field of view of a KML file
+    Test if a point is inside the field of view of a KML file  
 
-    Arguments:
-        latDegs:        [degrees] latitude of the point
-        lngDegs:        [degrees] latitude of the point
-        kmlFileName:    [str] full path to the KML file to test
+    Arguments:  
+        latDegs:        [degrees] latitude of the point  
+        lngDegs:        [degrees] latitude of the point  
+        kmlFileName:    [str] full path to the KML file to test  
+
+    Returns:  
+        True or False  
     """
 
     c1, p1 = munchKML(kmlFilename, True)
     pt = Point(latDegs, lngDegs)
     return p1.contains(pt)
 
 
 def checkKMLOverlap(kmfile1, kmfile2):
     """
-    Test if two KML files overlap
+    Test if two KML files overlap  
+
+    Arguments:  
+        kmlfile1:       [str] full path to first KML file  
+        kmlfile2:       [str] full path to second KML file  
 
-    Arguments:
-        kmlfile1:       [str] full path to first KML file
-        kmlfile2:       [str] full path to second KML file
+    Returns:  
+        True or False
     """
     _,p1 = munchKML(kmfile1, True)
     _,p2 = munchKML(kmfile2, True)
     return p1.intersects(p2)
 
 
 def getOverlapWith(srcfolder, kmlpattern='*-25km.kml', refcam='UK0006'):
     """
-    Check for overlap between the named camera, and every KML file in a folder, at the pattern altitude
+    Check for overlap between the named camera, and every KML file in a folder, at the pattern altitude  
 
-    Arguments:
-        srcfolder:  [str] path to folder containing KML files to test. 
-        kmlpattern: [str] kml pattern to match. Default "*-25km.kml"
-        refcam:     [str] Cameraid to check against. Its KML must be in srcfolder
+    Arguments:  
+        srcfolder:  [str] path to folder containing KML files to test.   
+        kmlpattern: [str] kml pattern to match. Default "*-25km.kml"  
+        refcam:     [str] Cameraid to check against. Its KML must be in srcfolder  
      
+    Returns:  
+        list of camera IDs that overlap with the target  
     """
     kmllist = glob.glob1(srcfolder, kmlpattern)
     currmatches=[]
     refkml = f'{refcam}{kmlpattern[1:]}'
     currmatches.append(refcam[:6])
     print('checking ', refkml)
     for testkml in kmllist:
@@ -62,19 +70,22 @@
                 currmatches.append(testcam[:6])
     return currmatches
 
 
 
 def getOverlappingCameras(srcfolder, kmlpattern='*-25km.kml'):
     """
-    Check for all overlaps in the folder at the pattern altitude
+    Check for all overlaps in the folder at the pattern altitude  
+
+    Arguments:  
+        srcfolder:  [str] path to folder containing KML files to test.   
+        kmlpattern: [str] kml pattern to match. Default "*-25km.kml"  
 
-    Arguments:
-        srcfolder:  [str] path to folder containing KML files to test. 
-        kmlpattern: [str] kml pattern to match. Default "*-25km.kml"
+    Returns:  
+        list of lists of groups of overlaping IDs 
      
     """
     kmllist = glob.glob1(srcfolder, kmlpattern)
     kmllist2 = kmllist
     matches = []
 
     for refkml in kmllist:
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/plotTrack.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/plotTrack.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 import numpy as np
 
 from ukmon_meteortools.utils import greatCircleDistance
 
 
 def trackToDistvsHeight(trackcsvfile):
     """
-    Plot a distance vs height graph from the supplied CSV file
+    Plot a distance vs height graph from the supplied CSV file  
 
-    Arguments:
-        trackcsvfile:   [str] full path to a CSV file containing columns of lat, long, height, time
+    Arguments:  
+        trackcsvfile:   [str] full path to a CSV file containing columns of lat, long, height, time  
+
+    Returns:  
+        nothing, but it creates a PNG in the source folder containing the track plot  
     """
     inputfile = csv.reader(open(trackcsvfile))
     dists = []
     alts = []
     lat0 = -99   # use impossible value
     lng0 = 0
     for row in inputfile:
@@ -40,18 +43,21 @@
     outname = trackcsvfile.replace('.csv','_dist_alt.png')
     plt.savefig(outname)
     plt.close()
 
 
 def trackToTimevsVelocity(trackcsvfile):
     """
-    Plot a distance vs velocity graph from the supplied CSV file
+    Plot a distance vs velocity graph from the supplied CSV file  
+
+    Arguments:  
+        trackcsvfile:   [str] full path to a CSV file containing columns of lat, long, height, time  
 
-    Arguments:
-        trackcsvfile:   [str] full path to a CSV file containing columns of lat, long, height, time
+    Returns:  
+        nothing, but it creates a PNG in the source folder containing the track plot  
     """
     inputfile = csv.reader(open(trackcsvfile))
     dists = []
     tims = []
     lat0 = -99   # use impossible value
     lng0 = 0
     for row in inputfile:
@@ -80,18 +86,21 @@
     outname = trackcsvfile.replace('.csv','_tim_vel.png')
     plt.savefig(outname)
     plt.close()
 
 
 def trackToTimevsHeight(trackcsvfile):
     """
-    Plot a time vs height graph from the supplied CSV file
+    Plot a time vs height graph from the supplied CSV file  
+
+    Arguments:  
+        trackcsvfile:   [str] full path to a CSV file containing columns of lat, long, height, time  
 
-    Arguments:
-        trackcsvfile:   [str] full path to a CSV file containing columns of lat, long, height, time
+    Returns:  
+        nothing, but it creates a PNG in the source folder containing the track plot  
     """
     inputfile = csv.reader(open(trackcsvfile))
     tims = []
     alts = []
     for row in inputfile:
         #columns are lat, long, height, times
         if row[0] == 'lats':
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/usertools/retrieveECSV.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/usertools/retrieveECSV.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import requests
 import sys
 import os
 
 
 def getECSVs(stationID, dateStr, savefiles=False, outdir='.'):
     """
-    Retrieve a detection in ECSV format for the specified date
+    Retrieve a detection in ECSV format for the specified date  
 
-    Arguments:
-        stationID:  [str] RMS Station ID code
-        dateStr:    [str] Date/time to retrieve for in ISO1601 format 
-                          eg 2021-07-17T02:41:05.05
+    Arguments:  
+        stationID:  [str] RMS Station ID code  
+        dateStr:    [str] Date/time to retrieve for in ISO1601 format   
+                          eg 2021-07-17T02:41:05.05  
     
-    Keyword Arguments:
-        saveFiles:  [bool] save to file, or print to screen. Default False
-        outdir:     [str] path to save files into. Default '.'
+    Keyword Arguments:  
+        saveFiles:  [bool] save to file, or print to screen. Default False  
+        outdir:     [str] path to save files into. Default '.'  
     """
     apiurl='https://jpaq0huazc.execute-api.eu-west-1.amazonaws.com/Prod/getecsv?stat={}&dt={}'
     res = requests.get(apiurl.format(stationID, dateStr))
     ecsvlines=''
     if res.status_code == 200:
         rawdata=res.text.strip()
         if len(rawdata) > 10:
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/Math.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/Math.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 
 # Define Julian epoch
 JULIAN_EPOCH = datetime(2000, 1, 1, 12) # J2000.0 noon
 J2000_JD = timedelta(2451545) # J2000.0 epoch in julian days
 
 
 def jd2Date(jd, UT_corr=0, dt_obj=False):
-    """ Converts the given Julian date to (year, month, day, hour, minute, second, millisecond) tuple. 
+    """ Converts the given Julian date to (year, month, day, hour, minute, second, millisecond) tuple or a datetime.  
 
-    Arguments:
-        jd: [float] Julian date
+    Arguments:  
+        jd: [float] Julian date  
 
-    Keyword arguments:
-        UT_corr: [float] UT correction in hours (difference from local time to UT)
-        dt_obj: [bool] returns a datetime object if True. False by default.
+    Keyword arguments:  
+        UT_corr: [float] UT correction in hours (difference from local time to UT)  
+        dt_obj: [bool] returns a datetime object if True. False by default.  
 
-    Return:
-        (year, month, day, hour, minute, second, millisecond)
+    Return:  
+        (year, month, day, hour, minute, second, millisecond) or a datetime
 
     """
 
     try:
 
         dt = timedelta(days=jd)
         
@@ -41,50 +41,37 @@
     if dt_obj:
         return date
 
     return date.year, date.month, date.day, date.hour, date.minute, date.second, date.microsecond/1000.0
 
 
 def datetime2JD(dt):
-    return date2JD(dt.year, dt.month, dt.day, dt.hour, dt.minute, dt.second, dt.microsecond/1000.0)
-
-
-def angleBetweenSphericalCoords(phi1, lambda1, phi2, lambda2):
-    """ Calculates the angle between two points on a sphere. 
-    
-    Arguments:
-        phi1: [float] Latitude 1 (radians).
-        lambda1: [float] Longitude 1 (radians).
-        phi2: [float] Latitude 2 (radians).
-        lambda2: [float] Longitude 2 (radians).
-
-    Return:
-        [float] Angle between two coordinates (radians).
+    """ Convert a datetime to a julian date  
     """
 
-    return np.arccos(np.sin(phi1)*np.sin(phi2) + np.cos(phi1)*np.cos(phi2)*np.cos(lambda2 - lambda1))
+    return date2JD(dt.year, dt.month, dt.day, dt.hour, dt.minute, dt.second, dt.microsecond/1000.0)
 
 
 def date2JD(year, month, day, hour, minute, second, millisecond=0, UT_corr=0.0):
-    """ Convert date and time to Julian Date in J2000.0. 
+    """ Convert date and time to Julian Date in J2000.0.  
     
-    Arguments:
-        year: [int] year
-        month: [int] month
-        day: [int] day of the date
-        hour: [int] hours
-        minute: [int] minutes
-        second: [int] seconds
-
-    Kwargs:
-        millisecond: [int] milliseconds (optional)
-        UT_corr: [float] UT correction in hours (difference from local time to UT)
+    Arguments:  
+        year: [int] year  
+        month: [int] month  
+        day: [int] day of the date  
+        hour: [int] hours  
+        minute: [int] minutes  
+        second: [int] seconds  
+
+    Kwargs:  
+        millisecond: [int] milliseconds (optional)  
+        UT_corr: [float] UT correction in hours (difference from local time to UT)  
     
-    Return:
-        [float] julian date, J2000.0 epoch
+    Return:  
+        [float] julian date, J2000.0 epoch  
     """
 
     # Convert all input arguments to integer (except milliseconds)
     year, month, day, hour, minute, second = map(int, (year, month, day, hour, minute, second))
 
     # Create datetime object of current time
     dt = datetime(year, month, day, hour, minute, second, int(millisecond*1000))
@@ -92,28 +79,129 @@
     # Calculate Julian date
     julian = dt - JULIAN_EPOCH + J2000_JD - timedelta(hours=UT_corr)
     
     # Convert seconds to day fractions
     return julian.days + (julian.seconds + julian.microseconds/1000000.0)/86400.0
 
 
+def jd2LST(julian_date, lon):
+    """ Convert Julian date to Local Sidereal Time and Greenwich Sidereal Time. The times used are apparent 
+        times, not mean times.  
+
+    Source: J. Meeus: Astronomical Algorithms  
+
+    Arguments:  
+        julian_date: [float] decimal julian date, epoch J2000.0  
+        lon: [float] longitude of the observer in degrees  
+    
+    Return:  
+        (LST, GST): [tuple of floats] a tuple of Local Sidereal Time and Greenwich Sidereal Time  
+    """
+
+    # t = (julian_date - J2000_JD.days)/36525.0
+
+    # Greenwich Sidereal Time
+    #GST = 280.46061837 + 360.98564736629*(julian_date - J2000_JD.days) + 0.000387933*t**2 - (t**3)/38710000
+    #GST = (GST + 360)%360
+
+    GST = np.degrees(calcApparentSiderealEarthRotation(julian_date))
+
+    # Local Sidereal Time
+    LST = (GST + lon + 360) % 360
+    
+    return LST, GST
+
+
+def jd2DynamicalTimeJD(jd):
+    """ Converts the given Julian date to dynamical time (i.e. Terrestrial Time, TT) Julian date. The 
+        conversion takes care of leap seconds.   
+
+    Arguments:  
+        jd: [float] Julian date.  
+
+    Return:  
+        [float] Dynamical time Julian date.  
+    """
+
+    # Leap seconds as of 2017 (default)
+    leap_secs = 37.0
+
+
+    # Get the relevant number of leap seconds for the given JD
+    # COMMENTED OUT as tai-utc.dat is empty
+    #for jd_leap, ls in config.leap_seconds:
+    #    
+    #    if jd > jd_leap:
+    #        leap_secs = ls
+            
+
+    # Calculate the dynamical JD
+    jd_dyn = jd + (leap_secs + 32.184)/86400.0
+
+
+    return jd_dyn
+
+
+def greatCircleDistance(lat1, lon1, lat2, lon2):
+    """ Calculate the great circle distance in kilometers between two points on the Earth. 
+        Source: https://gis.stackexchange.com/a/56589/15183  
+
+    Arguments:  
+        lat1: [float] Latitude 1 (radians).  
+        lon1: [float] Longitude 1 (radians).  
+        lat2: [float] Latitude 2 (radians).  
+        lon2: [float] Longitude 2 (radians).  
+
+    Return:  
+        [float]: Distance in kilometers.  
+    """
+    
+    # Haversine formula
+    dlon = lon2 - lon1 
+    dlat = lat2 - lat1 
+
+    a = np.sin(dlat/2)**2 + np.cos(lat1)*np.cos(lat2)*np.sin(dlon/2)**2
+    c = 2*np.arcsin(np.sqrt(a))
+
+    # Distance in kilometers.
+    dist = 6371*c
+
+    return dist
+
+
+def angleBetweenSphericalCoords(phi1, lambda1, phi2, lambda2):
+    """ Calculates the angle between two points on a sphere.  
+    
+    Arguments:  
+        phi1: [float] Latitude 1 (radians).  
+        lambda1: [float] Longitude 1 (radians).  
+        phi2: [float] Latitude 2 (radians).  
+        lambda2: [float] Longitude 2 (radians).  
+
+    Return:  
+        [float] Angle between two coordinates (radians).  
+    """
+
+    return np.arccos(np.sin(phi1)*np.sin(phi2) + np.cos(phi1)*np.cos(phi2)*np.cos(lambda2 - lambda1))
+
+
 def equatorialCoordPrecession(start_epoch, final_epoch, ra, dec):
     """ Precess right Ascension and declination from one epoch to another, taking only precession into 
-        account.
+        account.  
 
-        Implemented from: Jean Meeus - Astronomical Algorithms, 2nd edition, pages 134-135
+        Implemented from: Jean Meeus - Astronomical Algorithms, 2nd edition, pages 134-135  
     
-    Arguments:
-        start_epoch: [float] Julian date of the starting epoch
-        final_epoch: [float] Julian date of the final epoch
-        ra: [float] non-corrected right ascension in radians
-        dec: [float] non-corrected declination in radians
+    Arguments:  
+        start_epoch: [float] Julian date of the starting epoch  
+        final_epoch: [float] Julian date of the final epoch  
+        ra: [float] non-corrected right ascension in radians  
+        dec: [float] non-corrected declination in radians  
     
-    Return:
-        (ra, dec): [tuple of floats] precessed equatorial coordinates in radians
+    Return:  
+        (ra, dec): [tuple of floats] precessed equatorial coordinates in radians  
 
     """
 
 
     T = (start_epoch - J2000_JD.days)/36525.0
     t = (final_epoch - start_epoch)/36525.0
 
@@ -144,32 +232,32 @@
 
     # Wrap declination to [-pi/2, pi/2] range
     dec_corr = (dec_corr + np.pi/2) % np.pi - np.pi/2
 
     return ra_corr, dec_corr
 
 
-# Vectorize the equatorialCoordPrecession, so ra and dec can be passed as numpy arrays
 equatorialCoordPrecession_vect = np.vectorize(equatorialCoordPrecession, excluded=['start_epoch'])
+"""Vectorize the equatorialCoordPrecession, so ra and dec can be passed as numpy arrays"""
 
 
 def raDec2AltAz(ra, dec, jd, lat, lon):
-    """ Convert right ascension and declination to azimuth (+east of sue north) and altitude. 
+    """ Convert right ascension and declination to azimuth (+east of sue north) and altitude.  
 
-    Arguments:
-        ra: [float] right ascension in radians
-        dec: [float] declination in radians
-        jd: [float] Julian date
-        lat: [float] latitude in radians
-        lon: [float] longitude in radians
-
-    Return:
-        (azim, elev): [tuple]
-            azim: [float] azimuth (+east of due north) in radians
-            elev: [float] elevation above horizon in radians
+    Arguments:  
+        ra: [float] right ascension in radians  
+        dec: [float] declination in radians  
+        jd: [float] Julian date  
+        lat: [float] latitude in radians  
+        lon: [float] longitude in radians  
+
+    Return:  
+        (azim, elev): [tuple]  
+            azim: [float] azimuth (+east of due north) in radians  
+            elev: [float] elevation above horizon in radians  
 
         """
 
     # Calculate Local Sidereal Time
     lst = np.radians(jd2LST(jd, np.degrees(lon))[0])
 
     # Calculate the hour angle
@@ -188,52 +276,60 @@
     sin_elev = (sin_elev + 1) % 2 - 1
 
     elev = np.arcsin(sin_elev)
 
     return azim, elev
 
 
-# Vectorize the raDec2AltAz function so it can take numpy arrays for: ra, dec, jd
 raDec2AltAz_vect = np.vectorize(raDec2AltAz, excluded=['lat', 'lon'])
+"""Vectorize the raDec2AltAz function so it can take numpy arrays for: ra, dec, jd"""
 
 
-def jd2LST(julian_date, lon):
-    """ Convert Julian date to Local Sidereal Time and Greenwich Sidereal Time. The times used are apparent
-        times, not mean times.
+def altAz2RADec(azim, elev, jd, lat, lon):
+    """ Convert azimuth and altitude in a given time and position on Earth to right ascension and 
+        declination.   
 
-    Source: J. Meeus: Astronomical Algorithms
+    Arguments:  
+        azim: [float] azimuth (+east of due north) in radians  
+        elev: [float] elevation above horizon in radians  
+        jd: [float] Julian date  
+        lat: [float] latitude of the observer in radians  
+        lon: [float] longitde of the observer in radians  
+
+    Return:  
+        (RA, dec): [tuple]  
+            RA: [float] right ascension (radians)  
+            dec: [float] declination (radians)  
+    """
+    
+    # Calculate hour angle
+    ha = np.arctan2(-np.sin(azim), np.tan(elev)*np.cos(lat) - np.cos(azim)*np.sin(lat))
 
-    Arguments:
-        julian_date: [float] decimal julian date, epoch J2000.0
-        lon: [float] longitude of the observer in degrees
+    # Calculate Local Sidereal Time
+    lst = np.radians(jd2LST(jd, np.degrees(lon))[0])
     
-    Return:
-        (LST, GST): [tuple of floats] a tuple of Local Sidereal Time and Greenwich Sidereal Time
-    """
+    # Calculate right ascension
+    ra = (lst - ha) % (2*np.pi)
 
-    # t = (julian_date - J2000_JD.days)/36525.0
+    # Calculate declination
+    dec = np.arcsin(np.sin(lat)*np.sin(elev) + np.cos(lat)*np.cos(elev)*np.cos(azim))
 
-    # Greenwich Sidereal Time
-    #GST = 280.46061837 + 360.98564736629*(julian_date - J2000_JD.days) + 0.000387933*t**2 - (t**3)/38710000
-    #GST = (GST + 360)%360
+    return ra, dec
 
-    GST = np.degrees(calcApparentSiderealEarthRotation(julian_date))
 
-    # Local Sidereal Time
-    LST = (GST + lon + 360) % 360
-    
-    return LST, GST
+altAz2RADec_vect = np.vectorize(altAz2RADec, excluded=['lat', 'lon'])
+""" Vectorize the altAz2RADec function so it can take numpy arrays for: azim, elev, jd """
 
 
 def calcApparentSiderealEarthRotation(julian_date):
-    """ Calculate apparent sidereal rotation GST of the Earth. 
+    """ Calculate apparent sidereal rotation GST of the Earth.  
         
-        Calculated according to: 
+        Calculated according to:  
         Clark, D. L. (2010). Searching for fireball pre-detections in sky surveys. The School of Graduate and 
-        Postdoctoral Studies. University of Western Ontario, London, Ontario, Canada, MSc Thesis.
+        Postdoctoral Studies. University of Western Ontario, London, Ontario, Canada, MSc Thesis.  
 
     """
 
     t = (julian_date - J2000_JD.days)/36525.0
 
     # Calculate the Mean sidereal rotation of the Earth in radians (Greenwich Sidereal Time)
     GST = 280.46061837 + 360.98564736629*(julian_date - J2000_JD.days) + 0.000387933*t**2 - (t**3)/38710000
@@ -267,27 +363,27 @@
     # Calculate apparent sidereal Earth's rotation
     app_sid_rot = (GST + delta_psi*math.cos(eps0 + delta_eps)) % (2*math.pi)
 
     return app_sid_rot
 
 
 def calcNutationComponents(jd_dyn):
-    """ Calculate Earth's nutation components from the given Julian date.
+    """ Calculate Earth's nutation components from the given Julian date.  
 
-    Source: Meeus (1998) Astronomical algorithms, 2nd edition, chapter 22.
+    Source: Meeus (1998) Astronomical algorithms, 2nd edition, chapter 22.  
     
-    The precision is limited to 0.5" in nutation in longitude and 0.1" in nutation in obliquity. The errata
+    The precision is limited to 0.5" in nutation in longitude and 0.1" in nutation in obliquity. The errata 
     for the 2nd edition was used to correct the equation for delta_psi.
     
-    Arguments:
-        jd_dyn: [float] Dynamical Julian date. See wmpl.Utils.TrajConversions.jd2DynamicalTimeJD function.
+    Arguments:  
+        jd_dyn: [float] Dynamical Julian date. See wmpl.Utils.TrajConversions.jd2DynamicalTimeJD function.  
 
-    Return:
+    Return:  
         (delta_psi, delta_eps): [tuple of floats] Differences from mean nutation due to the influence of
-            the Moon and minor effects (radians).
+            the Moon and minor effects (radians).  
     """
 
 
     T = (jd_dyn - J2000_JD.days)/36525.0
 
     # # Mean Elongation of the Moon from the Sun
     # D = 297.85036 + 445267.11148*T - 0.0019142*T**2 + (T**3)/189474
@@ -324,100 +420,7 @@
 
 
     # Convert to radians
     delta_psi = np.radians(delta_psi/3600)
     delta_eps = np.radians(delta_eps/3600)
 
     return delta_psi, delta_eps
-
-
-def jd2DynamicalTimeJD(jd):
-    """ Converts the given Julian date to dynamical time (i.e. Terrestrial Time, TT) Julian date. The 
-        conversion takes care of leap seconds. 
-
-    Arguments:
-        jd: [float] Julian date.
-
-    Return:
-        [float] Dynamical time Julian date.
-    """
-
-    # Leap seconds as of 2017 (default)
-    leap_secs = 37.0
-
-
-    # Get the relevant number of leap seconds for the given JD
-    # COMMENTED OUT as tai-utc.dat is empty
-    #for jd_leap, ls in config.leap_seconds:
-    #    
-    #    if jd > jd_leap:
-    #        leap_secs = ls
-            
-
-    # Calculate the dynamical JD
-    jd_dyn = jd + (leap_secs + 32.184)/86400.0
-
-
-    return jd_dyn
-
-
-def greatCircleDistance(lat1, lon1, lat2, lon2):
-    """ Calculate the great circle distance in kilometers between two points on the Earth.
-        Source: https://gis.stackexchange.com/a/56589/15183
-
-    Arguments:
-        lat1: [float] Latitude 1 (radians).
-        lon1: [float] Longitude 1 (radians).
-        lat2: [float] Latitude 2 (radians).
-        lon2: [float] Longitude 2 (radians).
-
-    Return:
-        [float]: Distance in kilometers.
-    """
-    
-    # Haversine formula
-    dlon = lon2 - lon1 
-    dlat = lat2 - lat1 
-
-    a = np.sin(dlat/2)**2 + np.cos(lat1)*np.cos(lat2)*np.sin(dlon/2)**2
-    c = 2*np.arcsin(np.sqrt(a))
-
-    # Distance in kilometers.
-    dist = 6371*c
-
-    return dist
-
-
-def altAz2RADec(azim, elev, jd, lat, lon):
-    """ Convert azimuth and altitude in a given time and position on Earth to right ascension and 
-        declination. 
-
-    Arguments:
-        azim: [float] azimuth (+east of due north) in radians
-        elev: [float] elevation above horizon in radians
-        jd: [float] Julian date
-        lat: [float] latitude of the observer in radians
-        lon: [float] longitde of the observer in radians
-
-    Return:
-        (RA, dec): [tuple]
-            RA: [float] right ascension (radians)
-            dec: [float] declination (radians)
-    """
-    
-    # Calculate hour angle
-    ha = np.arctan2(-np.sin(azim), np.tan(elev)*np.cos(lat) - np.cos(azim)*np.sin(lat))
-
-    # Calculate Local Sidereal Time
-    lst = np.radians(jd2LST(jd, np.degrees(lon))[0])
-    
-    # Calculate right ascension
-    ra = (lst - ha) % (2*np.pi)
-
-    # Calculate declination
-    dec = np.arcsin(np.sin(lat)*np.sin(elev) + np.cos(lat)*np.cos(elev)*np.cos(azim))
-
-    return ra, dec
-
-
-# Vectorize the altAz2RADec function so it can take numpy arrays for: azim, elev, jd
-altAz2RADec_vect = np.vectorize(altAz2RADec, excluded=['lat', 'lon'])
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/VectorMaths.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/VectorMaths.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/__init__.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 # flake8: noqa
 """
 Utility functions used across the UKMON toolset
 
-List of Functions:
-jd2Date, date2JD, datetime2JD, jd2DynamicalTimeJD, jd2LST, sollon2jd
-greatCircleDistance, angleBetweenSphericalCoords, calcApparentSiderealEarthRotation
-calcNutationComponents, equatorialCoordPrecession,  raDec2AltAz, altAz2RADec
-altAz2RADec_vect, raDec2AltAz_vect, equatorialCoordPrecession_vect
-annotateImage, annotateImageArbitrary
-getActiveShowers, getActiveShowersStr, getShowerDets, getShowerPeak
-trackCsvtoKML, getTrackDetails, getTrajPickle, munchKML
-sendAnEmail
-shortestDistance2Lines
+List of Functions:  
+jd2Date, date2JD, datetime2JD, jd2DynamicalTimeJD, jd2LST, sollon2jd  
+greatCircleDistance, angleBetweenSphericalCoords, calcApparentSiderealEarthRotation  
+calcNutationComponents, equatorialCoordPrecession,  raDec2AltAz, altAz2RADec  
+altAz2RADec_vect, raDec2AltAz_vect, equatorialCoordPrecession_vect  
+annotateImage, annotateImageArbitrary  
+getActiveShowers, getActiveShowersStr, getShowerDets, getShowerPeak  
+trackCsvtoKML, getTrackDetails, getTrajPickle, munchKML  
+sendAnEmail  
+shortestDistance2Lines  
 """
 
 from .Math import jd2Date, date2JD,datetime2JD, jd2DynamicalTimeJD, JULIAN_EPOCH, J2000_JD, jd2LST
 from .Math import greatCircleDistance, angleBetweenSphericalCoords, calcApparentSiderealEarthRotation
 from .Math import calcNutationComponents, equatorialCoordPrecession,  raDec2AltAz, altAz2RADec
 from .Math import altAz2RADec_vect, raDec2AltAz_vect, equatorialCoordPrecession_vect
 
 from .annotateImage import annotateImage, annotateImageArbitrary
 
 from .convertSolLon import sollon2jd
 
 from .getActiveShowers import getActiveShowers, getActiveShowersStr
 
 from .getShowerDates import getShowerDets, getShowerPeak
-#from .getShowerDates import loadJenniskensShowers, loadDataFile, loadFullData, refreshShowerData
-#from .getShowerDates import loadLookupTable
 
 from .kmlHandlers import trackCsvtoKML, getTrackDetails, getTrajPickle, munchKML
 
 from .sendAnEmail import sendAnEmail
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/annotateImage.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/annotateImage.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from PIL import Image, ImageFont, ImageDraw 
 import datetime
 
 
 def annotateImage(img_path, statid, metcount, rundate=None):
     """
-    Annotate an image with the station ID and date in the bottom left and meteor count in the 
-    bottom right
+    Annotate an image with the station ID and date in the bottom left and meteor count in the  
+    bottom right  
 
-    Arguments:
-        img_path:   [str] full path and filename of the image to be annotated
-        statid:     [str] station ID string to use
-        metcount:   [int] number of meteors in the image
+    Arguments:  
+        img_path:   [str] full path and filename of the image to be annotated  
+        statid:     [str] station ID string to use  
+        metcount:   [int] number of meteors in the image  
 
     
-    Keyword Args:
-        rundate:    [str] rundate in 'YYYYMM' or 'YYYYMMDD' format. Default is today. 
+    Keyword Args:  
+        rundate:    [str] rundate in 'YYYYMM' or 'YYYYMMDD' format. Default is today.   
 
     """
     if rundate is not None:
         if len(rundate) > 6:
             now = datetime.datetime.strptime(rundate, '%Y%m%d')
             title = '{} {}'.format(statid, now.strftime('%Y-%m-%d'))
         else:
@@ -43,20 +43,20 @@
     metmsg = 'meteors: {:04d}'.format(metcount)
     image_editable.text((width-7*fntheight-15,height-fntheight-15), metmsg, font=fnt, fill=(255))
     my_image.save(img_path)
 
 
 def annotateImageArbitrary(img_path, message, color='#000'):
     """
-    Annotate an image with an arbitrary message in the selected colour at the bottom left
+    Annotate an image with an arbitrary message in the selected colour at the bottom left  
 
-    Arguments:
-        img_path:   [str] full path and filename of the image to be annotated
-        message:    [str] message to put on the image
-        color:      [str] hex colour string, default '#000' which is black
+    Arguments:  
+        img_path:   [str] full path and filename of the image to be annotated  
+        message:    [str] message to put on the image  
+        color:      [str] hex colour string, default '#000' which is black  
 
     """
     my_image = Image.open(img_path)
     width, height = my_image.size
     image_editable = ImageDraw.Draw(my_image)
     fntheight=30
     try:
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/convertSolLon.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/convertSolLon.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from ukmon_meteortools.utils import date2JD
 
 
 def sollon2jd(Year, Month, Long):
     """
     Calculate the julian date corresponding to a solar longitude. 
     Because Solar Longitude is relative to the Spring equinox, the exact date 
-    of a given LS varies from year to year. 
+    of a given LS varies from year to year.  
 
-    Parameters:
-        Year: [int] year you wish to calculate in.
-        Month: [int] month you wish to calculate in.
-        Long:  [float] The solar longitude to convert. 
+    Parameters:  
+        Year: [int] year you wish to calculate in.  
+        Month: [int] month you wish to calculate in.  
+        Long:  [float] The solar longitude to convert.   
 
-    Returns:
-        [float] julian date 
+    Returns:  
+        [float] julian date  
 
-    Notes:
-        The function is only stable for date ranges from 1900-2100. 
+    Notes:  
+        The function is only stable for date ranges from 1900-2100.  
     """
 
     Long = np.radians(Long)
     N = Year - 2000
     if abs(N) > 100:
         print("Algorithm is not stable for years below 1900 or above 2100")
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/getActiveShowers.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/getActiveShowers.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,45 +5,45 @@
 from ukmon_meteortools.fileformats import imoWorkingShowerList as iwsl
 import datetime
 import argparse
 
 
 def getActiveShowers(targdate, retlist=False, inclMinor=False):
     """
-    Return a list of showers active at the specified date
+    Return a list of showers active at the specified date  
 
-    Arguments:
-        targdate:   [str] Date in YYYYMMDD format
+    Arguments:  
+        targdate:   [str] Date in YYYYMMDD format  
 
-    Keyword Arguments:
-        retlist:    [bool] return a list, or print to console. Default False=print
-        inclMinor:  [bool] include minor showers or only return major showers
+    Keyword Arguments:  
+        retlist:    [bool] return a list, or print to console. Default False=print  
+        inclMinor:  [bool] include minor showers or only return major showers  
 
-    Returns:
-        If retlist is true, returns a python list of shower short-codes eg ['PER','LYR']
+    Returns:  
+        If retlist is true, returns a python list of shower short-codes eg ['PER','LYR']  
 
     """
     sl = iwsl.IMOshowerList()
     listofshowers=sl.getActiveShowers(targdate,True, inclMinor=inclMinor)
     if retlist is False:
         for shwr in listofshowers:
             print(shwr)
     else:
         return listofshowers
 
 
 def getActiveShowersStr(targdatestr):
     """
-    Prints a comma-separated list of showers active at the specified date
+    Prints a comma-separated list of showers active at the specified date  
 
-    Arguments:
-        targdate:   [str] Date in YYYYMMDD format
+    Arguments:  
+        targdate:   [str] Date in YYYYMMDD format  
 
-    Returns:
-        nothing
+    Returns:  
+        nothing  
 
     """
     targdate = datetime.datetime.strptime(targdatestr, '%Y%m%d')
     shwrs = getActiveShowers(targdate, retlist=True)
     shwrs.append('spo')
     for s in shwrs:
         print(s)
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/getShowerDates.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/getShowerDates.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 try:
     from UpdateOrbitFiles import updateOrbitFiles ## to update WMPL raw data files
     gotupdater = True
 except:
     gotupdater = False
 
 
-def loadFullData(pth=None):
-    return loadDataFile(1, pth)
+def _loadFullData(pth=None):
+    return _loadDataFile(1, pth)
 
 
-def loadLookupTable(pth=None):
-    return loadDataFile(2, pth)
+def _loadLookupTable(pth=None):
+    return _loadDataFile(2, pth)
 
 
-def loadJenniskensShowers(dir_path, file_name):
+def _loadJenniskensShowers(dir_path, file_name):
     """ Load the showers from the Jenniskens et al. (2018) table and init MeteorShower objects. """
     jenniskens_shower_list = []
     with open(os.path.join(dir_path, file_name), encoding='cp1252') as f:
         data_start = 0
         for line in f:
             if "====================================" in line:
                 data_start += 1
@@ -41,29 +41,29 @@
                 break
             l0, L_l0, B_g, v_g, IAU_no = line.split()
             jenniskens_shower_list.append([np.radians(float(l0)), np.radians(float(L_l0)), 
                 np.radians(float(B_g)), 1000*float(v_g), int(IAU_no)])
     return np.array(jenniskens_shower_list)
 
 
-def refreshShowerData():
+def _refreshShowerData():
     if gotupdater is True:
         updateOrbitFiles()
     abs_path = os.getenv('WMPL_LOC', default='/home/ec2-user/src/WesternMeteorPyLib')
     jenniskens_shower_table_file = os.path.join(abs_path, 'wmpl', 'share', 'ShowerLookUpTable.txt')
     jenniskens_shower_table_npy = os.path.join(abs_path, 'wmpl', 'share', 'ShowerLookUpTable.npy')
-    jenniskens_shower_list = loadJenniskensShowers(*os.path.split(jenniskens_shower_table_file))
+    jenniskens_shower_list = _loadJenniskensShowers(*os.path.split(jenniskens_shower_table_file))
     np.save(jenniskens_shower_table_npy, jenniskens_shower_list)
     iau_shower_table_file = os.path.join(abs_path, 'wmpl', 'share', 'streamfulldata.csv')
     iau_shower_table_npy = os.path.join(abs_path, 'wmpl', 'share', 'streamfulldata.npy')
     iau_shower_list = np.loadtxt(iau_shower_table_file, delimiter="|", usecols=range(20), dtype=str)
     np.save(iau_shower_table_npy, iau_shower_list)
 
 
-def loadDataFile(typ, pth=None):
+def _loadDataFile(typ, pth=None):
     if typ == 1:
         fname='streamfulldata.npy'
     elif typ == 2:
         fname='ShowerLookupTable.npy'
     else:
         return 'invalid type code'
 
@@ -73,15 +73,23 @@
         else:
             pth = '/home/ec2-user/src/WesternMeteorPyLib/wmpl/share'
     dfil = np.load(os.path.join(pth, fname))
     return dfil
 
 
 def getShowerDets(shwr):
-    sfd = loadFullData()
+    """ Get details of a shower 
+    
+    Arguments:  
+        shwr:   [string] three-letter shower code eg PER  
+         
+    Returns:  
+        (id, full name, peak solar longitude, peak date mm-dd)  
+    """
+    sfd = _loadFullData()
     sfdfltr = sfd[sfd[:,3] == shwr]
     mtch = [sh for sh in sfdfltr if sh[6] != '-2']
     if len(mtch) == 0:
         return 0, 'Unknown', 0, 'Unknown'
 
     id = int(mtch[-1][1])
     nam = mtch[-1][4].strip()
@@ -91,18 +99,26 @@
     mth = dt.month
     jd = sollon2jd(yr, mth, pksollong)
     pkdt = jd2Date(jd, dt_obj=True)
     return id, nam, pksollong, pkdt.strftime('%m-%d')
 
 
 def getShowerPeak(shwr):
+    """ Get date of a shower peak in MM-DD format
+    
+    Arguments:  
+        shwr:   [string] three-letter shower code eg PER  
+         
+    Returns:  
+        peak date mm-dd  
+    """
     _, _, _, pk = getShowerDets(shwr)
     return pk
 
  
 if __name__ == '__main__':
     if sys.argv[1] == 'refresh':
-        refreshShowerData()
+        _refreshShowerData()
         exit(0)
     else:
         id, nam, sl, dt = getShowerDets(sys.argv[1])
         print('{},{},{},{}'.format(sl, dt, nam, sys.argv[1]))
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools/utils/sendAnEmail.py` & `ukmon_meteortools-2023.5.0/ukmon_meteortools/utils/sendAnEmail.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 
 # If modifying these scopes, delete the file token.json.
 SCOPES =['https://mail.google.com/']
 
 
-def getGmailCreds():
+def _getGmailCreds():
     creds = None
     # The file token.json stores the user's access and refresh tokens, and is
     # created automatically when the authorization flow completes for the first
     # time.
     tokfile = os.path.expanduser('~/.ssh/gmailtoken.json')
     crdfile = os.path.expanduser('~/.ssh/gmailcreds.json')
     if os.path.exists(tokfile):
@@ -36,57 +36,57 @@
             creds = flow.run_local_server(port=0)
         # Save the credentials for the next run
         with open(tokfile, 'w') as token:
             token.write(creds.to_json())
     return creds
 
 
-def create_message(sender, to, subject, message_text):
+def _create_message(sender, to, subject, message_text):
     msg = MIMEText(message_text)
     msg['to'] = to
     msg['from'] = sender
     msg['subject'] = subject
     return {'raw': base64.urlsafe_b64encode(msg.as_string().encode('utf-8')).decode('utf-8')}
 
 
 
 def sendAnEmail(mailrecip, message, msgtype, mailfrom, files=None):
-    """ sends an email using gmail.
+    """ sends an email using gmail. 
     
-        Arguments:
-            mailrecip:  [string] email address of recipient.
-            message:    [string] the message to send.
-            msgtype:    [string] Prefix for the subject line, eg Test, Warning.
-            mailfrom:   [string] email address of sender. 
-            files:      [list]   list of files to attach, not currently implemented.
-
-        Returns:
-            Nothing, though a message is printed onscreen.
-
-        Notes:
-            You must have gmail OAUTH2 set up. The gmail credentials must be stored as follows:
-                token: $HOME/.ssh/gmailtoken.json
-                creds: $HOME/.ssh/gmailcreds.json
+        Arguments:  
+            mailrecip:  [string] email address of recipient.  
+            message:    [string] the message to send.  
+            msgtype:    [string] Prefix for the subject line, eg Test, Warning.  
+            mailfrom:   [string] email address of sender.   
+            files:      [list]   list of files to attach, not currently implemented.  
+
+        Returns:  
+            Nothing, though a message is printed onscreen.  
+
+        Notes:  
+            You must have gmail OAUTH2 set up. The gmail credentials must be stored as follows:  
+                token: $HOME/.ssh/gmailtoken.json  
+                creds: $HOME/.ssh/gmailcreds.json  
 
-            On Windows, $HOME corresponds to c:/users/yourid. If there is no .ssh folder, create it. 
+            On Windows, $HOME corresponds to c:/users/yourid. If there is no .ssh folder, create it.   
         """
     
     if msgtype is None:
         msgtype = platform.uname()[1]
 
     # email a summary to the mailrecip
-    creds = getGmailCreds()
+    creds = _getGmailCreds()
     if not creds:
         return 
     service = build('gmail', 'v1', credentials=creds)
 
     subj ='{:s}: {:s}'.format(msgtype, message[:30])
     message = '{:s}: {:s}'.format(msgtype, message)
 
-    mailmsg = create_message(mailfrom, mailrecip, subj, message)
+    mailmsg = _create_message(mailfrom, mailrecip, subj, message)
 
     try:
         retval = (service.users().messages().send(userId='me', body=mailmsg).execute())
         print('Message Id: %s' % retval['id'])
     except:
         print('An error occurred sending the message')
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools.egg-info/PKG-INFO` & `ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon-meteortools
-Version: 2023.4.24
+Version: 2023.5.0
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -687,15 +687,14 @@
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # ukmon_meteortools
-## Version 2023.04.24
 
 Python tools and utilities to work with meteor data from the UK Meteor Network
 
 To get more information about the submodules and functions use Python's built-in help capability
 
 ``` python
 from ukmon_meteortools import utils
```

### Comparing `ukmon_meteortools-2023.4.24/ukmon_meteortools.egg-info/SOURCES.txt` & `ukmon_meteortools-2023.5.0/ukmon_meteortools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

