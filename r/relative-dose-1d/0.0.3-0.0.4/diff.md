# Comparing `tmp/relative_dose_1d-0.0.3.tar.gz` & `tmp/relative_dose_1d-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relative_dose_1d-0.0.3.tar", last modified: Wed Apr  5 01:57:03 2023, max compression
+gzip compressed data, was "relative_dose_1d-0.0.4.tar", last modified: Wed May  3 01:21:06 2023, max compression
```

## Comparing `relative_dose_1d-0.0.3.tar` & `relative_dose_1d-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 01:57:03.340260 relative_dose_1d-0.0.3/
--rw-rw-rw-   0        0        0     1108 2023-04-05 01:02:18.000000 relative_dose_1d-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3340 2023-04-05 01:57:03.336263 relative_dose_1d-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2329 2023-04-05 01:40:18.000000 relative_dose_1d-0.0.3/README.md
--rw-rw-rw-   0        0        0     1329 2023-04-05 01:56:21.000000 relative_dose_1d-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 01:57:03.341261 relative_dose_1d-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-05 01:57:03.238544 relative_dose_1d-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-05 01:57:03.280431 relative_dose_1d-0.0.3/src/relative_dose_1d/
--rw-rw-rw-   0        0        0    10579 2023-04-05 01:56:06.000000 relative_dose_1d-0.0.3/src/relative_dose_1d/GUI.py
--rw-rw-rw-   0        0        0        0 2023-04-05 01:08:12.000000 relative_dose_1d-0.0.3/src/relative_dose_1d/__init__.py
--rw-rw-rw-   0        0        0     4337 2023-04-05 01:28:21.000000 relative_dose_1d-0.0.3/src/relative_dose_1d/read_1D_data.py
-drwxrwxrwx   0        0        0        0 2023-04-05 01:57:03.324927 relative_dose_1d-0.0.3/src/relative_dose_1d.egg-info/
--rw-rw-rw-   0        0        0     3340 2023-04-05 01:57:03.000000 relative_dose_1d-0.0.3/src/relative_dose_1d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-04-05 01:57:03.000000 relative_dose_1d-0.0.3/src/relative_dose_1d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 01:57:03.000000 relative_dose_1d-0.0.3/src/relative_dose_1d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-05 01:57:03.000000 relative_dose_1d-0.0.3/src/relative_dose_1d.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-05 01:57:03.000000 relative_dose_1d-0.0.3/src/relative_dose_1d.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 01:21:06.192163 relative_dose_1d-0.0.4/
+-rw-rw-rw-   0        0        0     1108 2023-04-05 01:02:18.000000 relative_dose_1d-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3376 2023-05-03 01:21:06.188173 relative_dose_1d-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2341 2023-05-03 01:06:42.000000 relative_dose_1d-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1353 2023-05-03 01:19:50.000000 relative_dose_1d-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 01:21:06.192163 relative_dose_1d-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 01:21:06.107392 relative_dose_1d-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 01:21:06.142298 relative_dose_1d-0.0.4/src/relative_dose_1d/
+-rw-rw-rw-   0        0        0     9264 2023-05-03 01:13:40.000000 relative_dose_1d-0.0.4/src/relative_dose_1d/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-04-05 01:08:12.000000 relative_dose_1d-0.0.4/src/relative_dose_1d/__init__.py
+-rw-rw-rw-   0        0        0     8809 2023-05-03 00:08:27.000000 relative_dose_1d-0.0.4/src/relative_dose_1d/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:21:06.178202 relative_dose_1d-0.0.4/src/relative_dose_1d.egg-info/
+-rw-rw-rw-   0        0        0     3376 2023-05-03 01:21:06.000000 relative_dose_1d-0.0.4/src/relative_dose_1d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-05-03 01:21:06.000000 relative_dose_1d-0.0.4/src/relative_dose_1d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 01:21:06.000000 relative_dose_1d-0.0.4/src/relative_dose_1d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-03 01:21:06.000000 relative_dose_1d-0.0.4/src/relative_dose_1d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-03 01:21:06.000000 relative_dose_1d-0.0.4/src/relative_dose_1d.egg-info/top_level.txt
```

### Comparing `relative_dose_1d-0.0.3/LICENSE` & `relative_dose_1d-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `relative_dose_1d-0.0.3/pyproject.toml` & `relative_dose_1d-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,19 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "relative_dose_1d"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Luis Alfonso Olivares Jimenez", email="alfonso.cucei.udg@gmail.com" },
 ]
-description = "Tool for 1-dimensional dose analysis in radiotherapy"
+description = "Tool to read 1-dimensional dose profiles and perform gamma index comparison."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENCE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
```

