# Comparing `tmp/relative_dose_1d-0.0.4.tar.gz` & `tmp/relative_dose_1d-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relative_dose_1d-0.0.4.tar", last modified: Wed May  3 01:21:06 2023, max compression
+gzip compressed data, was "relative_dose_1d-0.1.0.tar", last modified: Wed May  3 01:24:55 2023, max compression
```

## Comparing `relative_dose_1d-0.0.4.tar` & `relative_dose_1d-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 01:21:06.192163 relative_dose_1d-0.0.4/
--rw-rw-rw-   0        0        0     1108 2023-04-05 01:02:18.000000 relative_dose_1d-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3376 2023-05-03 01:21:06.188173 relative_dose_1d-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2341 2023-05-03 01:06:42.000000 relative_dose_1d-0.0.4/README.md
--rw-rw-rw-   0        0        0     1353 2023-05-03 01:19:50.000000 relative_dose_1d-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 01:21:06.192163 relative_dose_1d-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 01:21:06.107392 relative_dose_1d-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 01:21:06.142298 relative_dose_1d-0.0.4/src/relative_dose_1d/
--rw-rw-rw-   0        0        0     9264 2023-05-03 01:13:40.000000 relative_dose_1d-0.0.4/src/relative_dose_1d/GUI.py
--rw-rw-rw-   0        0        0        0 2023-04-05 01:08:12.000000 relative_dose_1d-0.0.4/src/relative_dose_1d/__init__.py
--rw-rw-rw-   0        0        0     8809 2023-05-03 00:08:27.000000 relative_dose_1d-0.0.4/src/relative_dose_1d/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-03 01:21:06.178202 relative_dose_1d-0.0.4/src/relative_dose_1d.egg-info/
--rw-rw-rw-   0        0        0     3376 2023-05-03 01:21:06.000000 relative_dose_1d-0.0.4/src/relative_dose_1d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-05-03 01:21:06.000000 relative_dose_1d-0.0.4/src/relative_dose_1d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 01:21:06.000000 relative_dose_1d-0.0.4/src/relative_dose_1d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-03 01:21:06.000000 relative_dose_1d-0.0.4/src/relative_dose_1d.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-03 01:21:06.000000 relative_dose_1d-0.0.4/src/relative_dose_1d.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 01:24:55.727014 relative_dose_1d-0.1.0/
+-rw-rw-rw-   0        0        0     1108 2023-04-05 01:02:18.000000 relative_dose_1d-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3376 2023-05-03 01:24:55.721025 relative_dose_1d-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2341 2023-05-03 01:06:42.000000 relative_dose_1d-0.1.0/README.md
+-rw-rw-rw-   0        0        0     1353 2023-05-03 01:24:25.000000 relative_dose_1d-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 01:24:55.728011 relative_dose_1d-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 01:24:55.638123 relative_dose_1d-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 01:24:55.670038 relative_dose_1d-0.1.0/src/relative_dose_1d/
+-rw-rw-rw-   0        0        0     9264 2023-05-03 01:13:40.000000 relative_dose_1d-0.1.0/src/relative_dose_1d/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 01:08:12.000000 relative_dose_1d-0.1.0/src/relative_dose_1d/__init__.py
+-rw-rw-rw-   0        0        0     8809 2023-05-03 00:08:27.000000 relative_dose_1d-0.1.0/src/relative_dose_1d/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:24:55.710879 relative_dose_1d-0.1.0/src/relative_dose_1d.egg-info/
+-rw-rw-rw-   0        0        0     3376 2023-05-03 01:24:55.000000 relative_dose_1d-0.1.0/src/relative_dose_1d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-05-03 01:24:55.000000 relative_dose_1d-0.1.0/src/relative_dose_1d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 01:24:55.000000 relative_dose_1d-0.1.0/src/relative_dose_1d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-03 01:24:55.000000 relative_dose_1d-0.1.0/src/relative_dose_1d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-03 01:24:55.000000 relative_dose_1d-0.1.0/src/relative_dose_1d.egg-info/top_level.txt
```

### Comparing `relative_dose_1d-0.0.4/LICENSE` & `relative_dose_1d-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.0.4/PKG-INFO` & `relative_dose_1d-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relative_dose_1d
-Version: 0.0.4
+Version: 0.1.0
 Summary: Tool to read 1-dimensional dose profiles and perform gamma index comparison.
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
 Project-URL: homepage, https://github.com/LuisOlivaresJ/relative_dose_1d
 Project-URL: repository, https://github.com/LuisOlivaresJ/relative_dose_1d
 Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d
 Keywords: Radiotherapy,Relative dose distribution,gamma index,python,w2CAD,mcc
 Classifier: Programming Language :: Python :: 3
```

### Comparing `relative_dose_1d-0.0.4/README.md` & `relative_dose_1d-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.0.4/pyproject.toml` & `relative_dose_1d-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "relative_dose_1d"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
   { name="Luis Alfonso Olivares Jimenez", email="alfonso.cucei.udg@gmail.com" },
 ]
 description = "Tool to read 1-dimensional dose profiles and perform gamma index comparison."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENCE"}
```

### Comparing `relative_dose_1d-0.0.4/src/relative_dose_1d/GUI.py` & `relative_dose_1d-0.1.0/src/relative_dose_1d/GUI.py`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.0.4/src/relative_dose_1d/tools.py` & `relative_dose_1d-0.1.0/src/relative_dose_1d/tools.py`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.0.4/src/relative_dose_1d.egg-info/PKG-INFO` & `relative_dose_1d-0.1.0/src/relative_dose_1d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relative-dose-1d
-Version: 0.0.4
+Version: 0.1.0
 Summary: Tool to read 1-dimensional dose profiles and perform gamma index comparison.
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
 Project-URL: homepage, https://github.com/LuisOlivaresJ/relative_dose_1d
 Project-URL: repository, https://github.com/LuisOlivaresJ/relative_dose_1d
 Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/relative_dose_1d
 Keywords: Radiotherapy,Relative dose distribution,gamma index,python,w2CAD,mcc
 Classifier: Programming Language :: Python :: 3
```

