# Comparing `tmp/permmod-0.1.tar.gz` & `tmp/permmod-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permmod-0.1.tar", last modified: Wed Dec 21 12:05:12 2022, max compression
+gzip compressed data, was "permmod-0.2.tar", last modified: Wed May  3 07:06:58 2023, max compression
```

## Comparing `permmod-0.1.tar` & `permmod-0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-12-21 12:05:12.785728 permmod-0.1/
--rw-rw-rw-   0        0        0      517 2022-12-21 12:05:12.785728 permmod-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        9 2022-12-21 11:17:13.000000 permmod-0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-21 12:05:12.785728 permmod-0.1/permmod/
--rw-rw-rw-   0        0        0      171 2022-12-21 09:26:03.000000 permmod-0.1/permmod/__init__.py
--rw-rw-rw-   0        0        0    12009 2022-12-21 10:03:59.000000 permmod-0.1/permmod/import_data.py
--rw-rw-rw-   0        0        0     5769 2022-12-21 09:15:33.000000 permmod-0.1/permmod/linear_system.py
--rw-rw-rw-   0        0        0     7194 2022-12-21 10:16:32.000000 permmod-0.1/permmod/measurement.py
--rw-rw-rw-   0        0        0     2737 2022-12-21 09:51:21.000000 permmod-0.1/permmod/optimize.py
--rw-rw-rw-   0        0        0    10423 2022-12-21 07:05:07.000000 permmod-0.1/permmod/plots.py
-drwxrwxrwx   0        0        0        0 2022-12-21 12:05:12.785728 permmod-0.1/permmod.egg-info/
--rw-rw-rw-   0        0        0      517 2022-12-21 12:05:12.000000 permmod-0.1/permmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2022-12-21 12:05:12.000000 permmod-0.1/permmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-21 12:05:12.000000 permmod-0.1/permmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2022-12-21 12:05:12.000000 permmod-0.1/permmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-12-21 12:05:12.000000 permmod-0.1/permmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      676 2022-12-21 12:04:45.000000 permmod-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-21 12:05:12.785728 permmod-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 07:06:58.917872 permmod-0.2/
+-rw-rw-rw-   0        0        0     1876 2023-05-03 07:06:58.917872 permmod-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1367 2023-03-06 12:08:24.000000 permmod-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 07:06:58.886620 permmod-0.2/permmod/
+-rw-rw-rw-   0        0        0      216 2023-03-08 09:11:06.000000 permmod-0.2/permmod/__init__.py
+-rw-rw-rw-   0        0        0    12009 2023-03-08 10:01:54.000000 permmod-0.2/permmod/import_data.py
+-rw-rw-rw-   0        0        0     5769 2023-03-08 11:13:05.000000 permmod-0.2/permmod/linear_system.py
+-rw-rw-rw-   0        0        0     7194 2023-03-06 12:08:24.000000 permmod-0.2/permmod/measurement.py
+-rw-rw-rw-   0        0        0     2737 2023-03-06 12:08:24.000000 permmod-0.2/permmod/optimize.py
+-rw-rw-rw-   0        0        0    10423 2023-03-06 12:08:24.000000 permmod-0.2/permmod/plots.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:06:58.902246 permmod-0.2/permmod.egg-info/
+-rw-rw-rw-   0        0        0     1876 2023-05-03 07:06:58.000000 permmod-0.2/permmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-03 07:06:58.000000 permmod-0.2/permmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 07:06:58.000000 permmod-0.2/permmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-03 07:06:58.000000 permmod-0.2/permmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 07:06:58.000000 permmod-0.2/permmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      677 2023-05-03 07:03:52.000000 permmod-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 07:06:58.917872 permmod-0.2/setup.cfg
```

### Comparing `permmod-0.1/permmod/import_data.py` & `permmod-0.2/permmod/import_data.py`

 * *Files identical despite different names*

### Comparing `permmod-0.1/permmod/linear_system.py` & `permmod-0.2/permmod/linear_system.py`

 * *Files identical despite different names*

### Comparing `permmod-0.1/permmod/measurement.py` & `permmod-0.2/permmod/measurement.py`

 * *Files identical despite different names*

### Comparing `permmod-0.1/permmod/optimize.py` & `permmod-0.2/permmod/optimize.py`

 * *Files identical despite different names*

### Comparing `permmod-0.1/permmod/plots.py` & `permmod-0.2/permmod/plots.py`

 * *Files identical despite different names*

### Comparing `permmod-0.1/pyproject.toml` & `permmod-0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "permmod"
-version = "0.1"
+version = "0.2"
 authors = [
   { name='Martin Kirch', email='mkirch@web.de' },
 ]
 description = "A package to calculate the permeability of rock samples"
 dependencies = ['pandas', 'numpy', 'CoolProp', 'scipy', 'plotly']
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

