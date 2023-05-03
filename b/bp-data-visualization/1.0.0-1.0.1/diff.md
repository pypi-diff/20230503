# Comparing `tmp/bp-data-visualization-1.0.0.tar.gz` & `tmp/bp-data-visualization-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp-data-visualization-1.0.0.tar", last modified: Wed May  3 12:04:25 2023, max compression
+gzip compressed data, was "bp-data-visualization-1.0.1.tar", last modified: Wed May  3 12:06:01 2023, max compression
```

## Comparing `bp-data-visualization-1.0.0.tar` & `bp-data-visualization-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:04:25.579542 bp-data-visualization-1.0.0/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-19 06:01:44.000000 bp-data-visualization-1.0.0/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       53 2023-04-19 06:01:44.000000 bp-data-visualization-1.0.0/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      298 2023-05-03 12:04:25.579249 bp-data-visualization-1.0.0/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2513 2023-05-03 11:37:39.000000 bp-data-visualization-1.0.0/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:04:25.572816 bp-data-visualization-1.0.0/bp_data_visualization.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      298 2023-05-03 12:04:25.000000 bp-data-visualization-1.0.0/bp_data_visualization.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      527 2023-05-03 12:04:25.000000 bp-data-visualization-1.0.0/bp_data_visualization.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-03 12:04:25.000000 bp-data-visualization-1.0.0/bp_data_visualization.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-05-03 12:04:25.000000 bp-data-visualization-1.0.0/bp_data_visualization.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       19 2023-05-03 12:04:25.000000 bp-data-visualization-1.0.0/bp_data_visualization.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:04:25.573560 bp-data-visualization-1.0.0/data_visualization/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2091 2023-04-24 10:01:27.000000 bp-data-visualization-1.0.0/data_visualization/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:04:25.569889 bp-data-visualization-1.0.0/data_visualization/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:04:25.574694 bp-data-visualization-1.0.0/data_visualization/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:04:25.576026 bp-data-visualization-1.0.0/data_visualization/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-24 09:58:58.000000 bp-data-visualization-1.0.0/data_visualization/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1939975 2023-04-24 09:58:58.000000 bp-data-visualization-1.0.0/data_visualization/frontend/dist/assets/index-d7151b26.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      457 2023-04-24 09:59:08.000000 bp-data-visualization-1.0.0/data_visualization/frontend/dist/index.html
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-24 09:58:57.000000 bp-data-visualization-1.0.0/data_visualization/frontend/dist/vite.svg
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-19 06:01:44.000000 bp-data-visualization-1.0.0/data_visualization/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-03 12:04:25.579658 bp-data-visualization-1.0.0/setup.cfg
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      758 2023-05-03 12:04:22.000000 bp-data-visualization-1.0.0/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:06:01.922477 bp-data-visualization-1.0.1/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-19 06:01:44.000000 bp-data-visualization-1.0.1/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       53 2023-04-19 06:01:44.000000 bp-data-visualization-1.0.1/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3412 2023-05-03 12:06:01.922167 bp-data-visualization-1.0.1/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2513 2023-05-03 11:37:39.000000 bp-data-visualization-1.0.1/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:06:01.916174 bp-data-visualization-1.0.1/bp_data_visualization.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3412 2023-05-03 12:06:01.000000 bp-data-visualization-1.0.1/bp_data_visualization.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      527 2023-05-03 12:06:01.000000 bp-data-visualization-1.0.1/bp_data_visualization.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-03 12:06:01.000000 bp-data-visualization-1.0.1/bp_data_visualization.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-05-03 12:06:01.000000 bp-data-visualization-1.0.1/bp_data_visualization.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       19 2023-05-03 12:06:01.000000 bp-data-visualization-1.0.1/bp_data_visualization.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:06:01.917030 bp-data-visualization-1.0.1/data_visualization/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2091 2023-04-24 10:01:27.000000 bp-data-visualization-1.0.1/data_visualization/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:06:01.912552 bp-data-visualization-1.0.1/data_visualization/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:06:01.917927 bp-data-visualization-1.0.1/data_visualization/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-03 12:06:01.918870 bp-data-visualization-1.0.1/data_visualization/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-24 09:58:58.000000 bp-data-visualization-1.0.1/data_visualization/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1939975 2023-04-24 09:58:58.000000 bp-data-visualization-1.0.1/data_visualization/frontend/dist/assets/index-d7151b26.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      457 2023-04-24 09:59:08.000000 bp-data-visualization-1.0.1/data_visualization/frontend/dist/index.html
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-24 09:58:57.000000 bp-data-visualization-1.0.1/data_visualization/frontend/dist/vite.svg
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-19 06:01:44.000000 bp-data-visualization-1.0.1/data_visualization/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-03 12:06:01.922633 bp-data-visualization-1.0.1/setup.cfg
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      772 2023-05-03 12:05:59.000000 bp-data-visualization-1.0.1/setup.py
```

### Comparing `bp-data-visualization-1.0.0/LICENSE` & `bp-data-visualization-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.0/README.md` & `bp-data-visualization-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.0/bp_data_visualization.egg-info/SOURCES.txt` & `bp-data-visualization-1.0.1/bp_data_visualization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.0/data_visualization/__init__.py` & `bp-data-visualization-1.0.1/data_visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.0/data_visualization/frontend/dist/assets/index-d7151b26.js` & `bp-data-visualization-1.0.1/data_visualization/frontend/dist/assets/index-d7151b26.js`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.0/data_visualization/frontend/dist/vite.svg` & `bp-data-visualization-1.0.1/data_visualization/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.0/data_visualization/register.py` & `bp-data-visualization-1.0.1/data_visualization/register.py`

 * *Files identical despite different names*

### Comparing `bp-data-visualization-1.0.0/setup.py` & `bp-data-visualization-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="bp-data-visualization",
-    version="1.0.0",
+    version="1.0.1",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="Show data in charts",
-    long_description="",
+    long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[],
     python_requires=">=3.8.10",
     install_requires=[
```

