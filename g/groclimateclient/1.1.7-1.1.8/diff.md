# Comparing `tmp/groclimateclient-1.1.7.tar.gz` & `tmp/groclimateclient-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groclimateclient-1.1.7.tar", max compression
+gzip compressed data, was "groclimateclient-1.1.8.tar", max compression
```

## Comparing `groclimateclient-1.1.7.tar` & `groclimateclient-1.1.8.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1073 2022-05-04 12:56:56.412579 groclimateclient-1.1.7/LICENSE
--rw-r--r--   0        0        0      158 2022-05-04 12:56:56.412732 groclimateclient-1.1.7/README.md
--rw-r--r--   0        0        0     3243 2022-05-04 12:56:56.412984 groclimateclient-1.1.7/groclimateclient/CONTRIBUTING.md
--rw-r--r--   0        0        0       60 2022-05-04 12:56:56.413140 groclimateclient-1.1.7/groclimateclient/__init__.py
--rw-r--r--   0        0        0    16450 2022-08-03 18:47:53.926385 groclimateclient-1.1.7/groclimateclient/climate_client.py
--rw-r--r--   0        0        0    13268 2023-02-02 19:01:33.271054 groclimateclient-1.1.7/groclimateclient/constants.py
--rw-r--r--   0        0        0      706 2023-02-06 22:57:35.218176 groclimateclient-1.1.7/pyproject.toml
--rw-r--r--   0        0        0      901 2023-02-06 22:59:08.028856 groclimateclient-1.1.7/setup.py
--rw-r--r--   0        0        0      895 2023-02-06 22:59:08.029341 groclimateclient-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-02 20:23:28.721809 groclimateclient-1.1.8/LICENSE
+-rw-r--r--   0        0        0      158 2023-05-02 20:23:28.721908 groclimateclient-1.1.8/README.md
+-rw-r--r--   0        0        0     3243 2023-05-02 20:23:28.722091 groclimateclient-1.1.8/groclimateclient/CONTRIBUTING.md
+-rw-r--r--   0        0        0       60 2023-05-02 20:23:28.722188 groclimateclient-1.1.8/groclimateclient/__init__.py
+-rw-r--r--   0        0        0    16450 2023-05-02 20:23:28.722539 groclimateclient-1.1.8/groclimateclient/climate_client.py
+-rw-r--r--   0        0        0    13745 2023-05-02 20:23:28.722706 groclimateclient-1.1.8/groclimateclient/constants.py
+-rw-r--r--   0        0        0      706 2023-05-02 20:27:41.848894 groclimateclient-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 groclimateclient-1.1.8/PKG-INFO
```

### Comparing `groclimateclient-1.1.7/LICENSE` & `groclimateclient-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `groclimateclient-1.1.7/groclimateclient/CONTRIBUTING.md` & `groclimateclient-1.1.8/groclimateclient/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `groclimateclient-1.1.7/groclimateclient/climate_client.py` & `groclimateclient-1.1.8/groclimateclient/climate_client.py`

 * *Files identical despite different names*

### Comparing `groclimateclient-1.1.7/groclimateclient/constants.py` & `groclimateclient-1.1.8/groclimateclient/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -161,15 +161,16 @@
     23832: "Tropical cyclones within 50 km, Saffir-Simpson Category 1-5",
     23833: "Tropical cyclones within 50 km, Saffir-Simpson Category 2-5",
     23834: "Tropical cyclones within 50 km, Saffir-Simpson Category 3-5",
     23835: "Tropical cyclones within 50 km, Saffir-Simpson Category 4-5",
     23836: "Tropical cyclones within 50 km, Saffir-Simpson Category 5",
     25884: "Ocean",
     25885: "Sea surface",
-    26971: "Heat stress"
+    26971: "Heat stress",
+    26968: "Water stress",
 }
 
 CLIMATE_METRICS = {
     1585211: "Aspect",
     1585297: "Atmospheric Greenhouse Gas Concentration",
     1585297: "Atmospheric Greenhouse Gas Concentration, Seasonally Corrected",
     1553109: "Availability in soil (amount of substance)",
@@ -252,15 +253,23 @@
     15853883: "Change since 2015, 5th percentile",
     15853858: "Change since 2015, 50th percentile",
     15853859: "Change since 2015, 95th percentile",
     15853860: "Change since 2015, 99th percentile",
     15853878: "Temperature Humidity Index (max)",
     15853879: "Temperature Humidity Index (min)",
     15853880: "Heat Index (max)",
-    15853881: "Heat Index (min)"
+    15853881: "Heat Index (min)",
+    15854674: "Actual water stress index (percent)",
+    15854066: "Maximum water stress index (percent)",
+    15854080: "Minimum water stress index (percent)",
+    15854094: "Weighted mean water stress index (percent)",
+    15854688: "Actual water stress score (number)",
+    15854109: "Maximum water stress score (number)",
+    15854123: "Minimum water stress score (number)",
+    15854137: "Weighted mean water stress score (number)",
 }
 
 CLIMATE_SOURCES = [
     3,
     20,
     22,
     26,
@@ -306,10 +315,11 @@
     319,
     320,
     322,
     323,
     324,
     325,
     326,
-    327
+    327,
+    343,
 ]
 CMIP6_SOURCES = [178, 189, 190, 191, 192, 300, 301, 302, 303, 304, 305, 306, 307, 308, 309]
```

### Comparing `groclimateclient-1.1.7/pyproject.toml` & `groclimateclient-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "groclimateclient"
 # Note: we use poetry-dynamic-versioning to set the version from git tags.
-version = "1.1.7"
+version = "1.1.8"
 description = "Python client library for accessing Gro Intelligence's climate data"
 authors = ["Gro Intelligence developers <dev@gro-intelligence.com>"]
 readme = "README.md"
 homepage = "https://www.gro-intelligence.com"
 repository = ""
 documentation = ""
 license = "MIT"
```

### Comparing `groclimateclient-1.1.7/PKG-INFO` & `groclimateclient-1.1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: groclimateclient
-Version: 1.1.7
+Version: 1.1.8
 Summary: Python client library for accessing Gro Intelligence's climate data
 Home-page: https://www.gro-intelligence.com
 License: MIT
 Author: Gro Intelligence developers
 Author-email: dev@gro-intelligence.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fuzzywuzzy
 Requires-Dist: groclient
 Requires-Dist: numpy
 Requires-Dist: pandas
 Description-Content-Type: text/markdown
 
 <p align="center"><img width="20%" src="https://gro-images.s3.amazonaws.com/Gro-Logo-Emble-Blue-LARGE.svg"></p>
```

