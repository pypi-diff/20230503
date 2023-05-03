# Comparing `tmp/navigation-utilities-0.2.0.tar.gz` & `tmp/navigation-utilities-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navigation-utilities-0.2.0.tar", last modified: Mon May  1 12:11:55 2023, max compression
+gzip compressed data, was "navigation-utilities-0.2.1.tar", last modified: Wed May  3 17:00:28 2023, max compression
```

## Comparing `navigation-utilities-0.2.0.tar` & `navigation-utilities-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-01 12:11:55.212311 navigation-utilities-0.2.0/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1073 2023-03-28 18:04:54.000000 navigation-utilities-0.2.0/LICENSE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1130 2023-05-01 12:11:55.212311 navigation-utilities-0.2.0/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      522 2023-04-03 09:41:32.000000 navigation-utilities-0.2.0/README.md
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      697 2023-05-01 12:11:43.000000 navigation-utilities-0.2.0/pyproject.toml
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-01 12:11:55.212311 navigation-utilities-0.2.0/setup.cfg
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-01 12:11:55.208311 navigation-utilities-0.2.0/src/
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-01 12:11:55.212311 navigation-utilities-0.2.0/src/navigation_utilities/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-03-28 18:04:54.000000 navigation-utilities-0.2.0/src/navigation_utilities/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1455 2023-05-01 12:01:13.000000 navigation-utilities-0.2.0/src/navigation_utilities/coordinate.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     4187 2023-05-01 12:01:01.000000 navigation-utilities-0.2.0/src/navigation_utilities/gngga.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1936 2023-05-01 11:56:39.000000 navigation-utilities-0.2.0/src/navigation_utilities/nmea.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2749 2023-05-01 11:56:49.000000 navigation-utilities-0.2.0/src/navigation_utilities/oxts.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-01 12:11:55.212311 navigation-utilities-0.2.0/src/navigation_utilities/utils/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2515 2023-05-01 12:01:32.000000 navigation-utilities-0.2.0/src/navigation_utilities/utils/time.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-01 12:11:55.212311 navigation-utilities-0.2.0/src/navigation_utilities.egg-info/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1130 2023-05-01 12:11:55.000000 navigation-utilities-0.2.0/src/navigation_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      439 2023-05-01 12:11:55.000000 navigation-utilities-0.2.0/src/navigation_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-01 12:11:55.000000 navigation-utilities-0.2.0/src/navigation_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       21 2023-05-01 12:11:55.000000 navigation-utilities-0.2.0/src/navigation_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1073 2023-05-03 16:59:00.000000 navigation-utilities-0.2.1/LICENSE
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1130 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/PKG-INFO
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      522 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/README.md
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      715 2023-05-03 16:59:24.000000 navigation-utilities-0.2.1/pyproject.toml
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       38 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/setup.cfg
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/src/
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/src/navigation_utilities/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)        0 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/src/navigation_utilities/__init__.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1455 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/src/navigation_utilities/coordinate.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     4187 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/src/navigation_utilities/gngga.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1936 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/src/navigation_utilities/nmea.py
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     2749 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/src/navigation_utilities/oxts.py
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/src/navigation_utilities/utils/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     2515 2023-05-03 18:22:37.000000 navigation-utilities-0.2.1/src/navigation_utilities/utils/time.py
+drwxr-xr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-03 17:00:28.802038 navigation-utilities-0.2.1/src/navigation_utilities.egg-info/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)     1130 2023-05-03 17:00:28.000000 navigation-utilities-0.2.1/src/navigation_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      486 2023-05-03 17:00:28.000000 navigation-utilities-0.2.1/src/navigation_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 pablo     (1000) pablo     (1000)        1 2023-05-03 17:00:28.000000 navigation-utilities-0.2.1/src/navigation_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       14 2023-05-03 17:00:28.000000 navigation-utilities-0.2.1/src/navigation_utilities.egg-info/requires.txt
+-rw-r--r--   0 pablo     (1000) pablo     (1000)       21 2023-05-03 17:00:28.000000 navigation-utilities-0.2.1/src/navigation_utilities.egg-info/top_level.txt
```

### Comparing `navigation-utilities-0.2.0/LICENSE` & `navigation-utilities-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `navigation-utilities-0.2.0/PKG-INFO` & `navigation-utilities-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navigation-utilities
-Version: 0.2.0
+Version: 0.2.1
 Summary: Collection of utilities for driverless navigation systems and gnss tools
 Author-email: Pablo Dorrio Vazquez <pablo.dorrio.vazquez@gmail.com>
 Project-URL: Homepage, https://github.com/pablodorrio/navigation-utilities
 Project-URL: Bug Tracker, https://github.com/pablodorrio/navigation-utilities/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `navigation-utilities-0.2.0/README.md` & `navigation-utilities-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `navigation-utilities-0.2.0/pyproject.toml` & `navigation-utilities-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [build-system]
 requires = [
-  "setuptools",
-  "numpy>=1.24.1"
+  "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "navigation-utilities"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Pablo Dorrio Vazquez", email="pablo.dorrio.vazquez@gmail.com" },
 ]
 description = "Collection of utilities for driverless navigation systems and gnss tools"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "numpy>=1.24.1"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/pablodorrio/navigation-utilities"
 "Bug Tracker" = "https://github.com/pablodorrio/navigation-utilities/issues"
```

### Comparing `navigation-utilities-0.2.0/src/navigation_utilities/coordinate.py` & `navigation-utilities-0.2.1/src/navigation_utilities/coordinate.py`

 * *Files identical despite different names*

### Comparing `navigation-utilities-0.2.0/src/navigation_utilities/gngga.py` & `navigation-utilities-0.2.1/src/navigation_utilities/gngga.py`

 * *Files identical despite different names*

### Comparing `navigation-utilities-0.2.0/src/navigation_utilities/nmea.py` & `navigation-utilities-0.2.1/src/navigation_utilities/nmea.py`

 * *Files identical despite different names*

### Comparing `navigation-utilities-0.2.0/src/navigation_utilities/oxts.py` & `navigation-utilities-0.2.1/src/navigation_utilities/oxts.py`

 * *Files identical despite different names*

### Comparing `navigation-utilities-0.2.0/src/navigation_utilities/utils/time.py` & `navigation-utilities-0.2.1/src/navigation_utilities/utils/time.py`

 * *Files identical despite different names*

### Comparing `navigation-utilities-0.2.0/src/navigation_utilities.egg-info/PKG-INFO` & `navigation-utilities-0.2.1/src/navigation_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navigation-utilities
-Version: 0.2.0
+Version: 0.2.1
 Summary: Collection of utilities for driverless navigation systems and gnss tools
 Author-email: Pablo Dorrio Vazquez <pablo.dorrio.vazquez@gmail.com>
 Project-URL: Homepage, https://github.com/pablodorrio/navigation-utilities
 Project-URL: Bug Tracker, https://github.com/pablodorrio/navigation-utilities/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

