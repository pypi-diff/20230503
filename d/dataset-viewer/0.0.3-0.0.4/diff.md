# Comparing `tmp/dataset-viewer-0.0.3.tar.gz` & `tmp/dataset-viewer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-viewer-0.0.3.tar", last modified: Wed May  3 04:03:13 2023, max compression
+gzip compressed data, was "dataset-viewer-0.0.4.tar", last modified: Wed May  3 04:23:38 2023, max compression
```

## Comparing `dataset-viewer-0.0.3.tar` & `dataset-viewer-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 04:03:13.823310 dataset-viewer-0.0.3/
--rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      697 2023-05-03 04:03:13.821742 dataset-viewer-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       95 2023-05-03 02:56:56.000000 dataset-viewer-0.0.3/README.md
--rw-rw-rw-   0        0        0      747 2023-05-03 04:02:42.000000 dataset-viewer-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 04:03:13.823310 dataset-viewer-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 04:03:13.800186 dataset-viewer-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 04:03:13.805207 dataset-viewer-0.0.3/src/dataset_viewer/
--rw-rw-rw-   0        0        0        0 2023-05-03 03:38:08.000000 dataset-viewer-0.0.3/src/dataset_viewer/__init__.py
--rw-rw-rw-   0        0        0       79 2023-05-03 03:33:50.000000 dataset-viewer-0.0.3/src/dataset_viewer/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 04:03:13.821742 dataset-viewer-0.0.3/src/dataset_viewer.egg-info/
--rw-rw-rw-   0        0        0      697 2023-05-03 04:03:13.000000 dataset-viewer-0.0.3/src/dataset_viewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-03 04:03:13.000000 dataset-viewer-0.0.3/src/dataset_viewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 04:03:13.000000 dataset-viewer-0.0.3/src/dataset_viewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-03 04:03:13.000000 dataset-viewer-0.0.3/src/dataset_viewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-03 04:03:13.000000 dataset-viewer-0.0.3/src/dataset_viewer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 04:23:38.340161 dataset-viewer-0.0.4/
+-rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      696 2023-05-03 04:23:38.339160 dataset-viewer-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       95 2023-05-03 02:56:56.000000 dataset-viewer-0.0.4/README.md
+-rw-rw-rw-   0        0        0      746 2023-05-03 04:22:45.000000 dataset-viewer-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 04:23:38.340161 dataset-viewer-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 04:23:38.315067 dataset-viewer-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 04:23:38.321064 dataset-viewer-0.0.4/src/dataset_viewer/
+-rw-rw-rw-   0        0        0        0 2023-05-03 03:38:08.000000 dataset-viewer-0.0.4/src/dataset_viewer/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-05-03 03:33:50.000000 dataset-viewer-0.0.4/src/dataset_viewer/main.py
+drwxrwxrwx   0        0        0        0 2023-05-03 04:23:38.338159 dataset-viewer-0.0.4/src/dataset_viewer.egg-info/
+-rw-rw-rw-   0        0        0      696 2023-05-03 04:23:38.000000 dataset-viewer-0.0.4/src/dataset_viewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-03 04:23:38.000000 dataset-viewer-0.0.4/src/dataset_viewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 04:23:38.000000 dataset-viewer-0.0.4/src/dataset_viewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-03 04:23:38.000000 dataset-viewer-0.0.4/src/dataset_viewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-03 04:23:38.000000 dataset-viewer-0.0.4/src/dataset_viewer.egg-info/top_level.txt
```

### Comparing `dataset-viewer-0.0.3/LICENSE` & `dataset-viewer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-viewer-0.0.3/PKG-INFO` & `dataset-viewer-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: gui
 License-File: LICENSE
 
 # Dataset Viewer
 
 Allow to view a dataset image by image and edit their labels using napari
```

### Comparing `dataset-viewer-0.0.3/pyproject.toml` & `dataset-viewer-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataset-viewer"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Hillpro", email="66534835+Hillpro@users.noreply.github.com" },
 ]
 description = "Allow to view a dataset image by image and edit their labels"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "napari",
```

### Comparing `dataset-viewer-0.0.3/src/dataset_viewer.egg-info/PKG-INFO` & `dataset-viewer-0.0.4/src/dataset_viewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: gui
 License-File: LICENSE
 
 # Dataset Viewer
 
 Allow to view a dataset image by image and edit their labels using napari
```

