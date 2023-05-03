# Comparing `tmp/dataset-viewer-0.0.2.tar.gz` & `tmp/dataset-viewer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-viewer-0.0.2.tar", last modified: Wed May  3 03:47:59 2023, max compression
+gzip compressed data, was "dataset-viewer-0.0.3.tar", last modified: Wed May  3 04:03:13 2023, max compression
```

## Comparing `dataset-viewer-0.0.2.tar` & `dataset-viewer-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 03:47:59.326279 dataset-viewer-0.0.2/
--rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      697 2023-05-03 03:47:59.326279 dataset-viewer-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       95 2023-05-03 02:56:56.000000 dataset-viewer-0.0.2/README.md
--rw-rw-rw-   0        0        0      747 2023-05-03 03:45:44.000000 dataset-viewer-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 03:47:59.326279 dataset-viewer-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 03:47:59.297105 dataset-viewer-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 03:47:59.306676 dataset-viewer-0.0.2/src/dataset-viewer/
--rw-rw-rw-   0        0        0        0 2023-05-03 03:38:08.000000 dataset-viewer-0.0.2/src/dataset-viewer/__init__.py
--rw-rw-rw-   0        0        0       79 2023-05-03 03:33:50.000000 dataset-viewer-0.0.2/src/dataset-viewer/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:47:59.324280 dataset-viewer-0.0.2/src/dataset_viewer.egg-info/
--rw-rw-rw-   0        0        0      697 2023-05-03 03:47:59.000000 dataset-viewer-0.0.2/src/dataset_viewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-03 03:47:59.000000 dataset-viewer-0.0.2/src/dataset_viewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 03:47:59.000000 dataset-viewer-0.0.2/src/dataset_viewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-03 03:47:59.000000 dataset-viewer-0.0.2/src/dataset_viewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-03 03:47:59.000000 dataset-viewer-0.0.2/src/dataset_viewer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 04:03:13.823310 dataset-viewer-0.0.3/
+-rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      697 2023-05-03 04:03:13.821742 dataset-viewer-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       95 2023-05-03 02:56:56.000000 dataset-viewer-0.0.3/README.md
+-rw-rw-rw-   0        0        0      747 2023-05-03 04:02:42.000000 dataset-viewer-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 04:03:13.823310 dataset-viewer-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 04:03:13.800186 dataset-viewer-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 04:03:13.805207 dataset-viewer-0.0.3/src/dataset_viewer/
+-rw-rw-rw-   0        0        0        0 2023-05-03 03:38:08.000000 dataset-viewer-0.0.3/src/dataset_viewer/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-05-03 03:33:50.000000 dataset-viewer-0.0.3/src/dataset_viewer/main.py
+drwxrwxrwx   0        0        0        0 2023-05-03 04:03:13.821742 dataset-viewer-0.0.3/src/dataset_viewer.egg-info/
+-rw-rw-rw-   0        0        0      697 2023-05-03 04:03:13.000000 dataset-viewer-0.0.3/src/dataset_viewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-03 04:03:13.000000 dataset-viewer-0.0.3/src/dataset_viewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 04:03:13.000000 dataset-viewer-0.0.3/src/dataset_viewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-03 04:03:13.000000 dataset-viewer-0.0.3/src/dataset_viewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-03 04:03:13.000000 dataset-viewer-0.0.3/src/dataset_viewer.egg-info/top_level.txt
```

### Comparing `dataset-viewer-0.0.2/LICENSE` & `dataset-viewer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-viewer-0.0.2/PKG-INFO` & `dataset-viewer-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dataset-viewer-0.0.2/pyproject.toml` & `dataset-viewer-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataset-viewer"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Hillpro", email="66534835+Hillpro@users.noreply.github.com" },
 ]
 description = "Allow to view a dataset image by image and edit their labels"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `dataset-viewer-0.0.2/src/dataset_viewer.egg-info/PKG-INFO` & `dataset-viewer-0.0.3/src/dataset_viewer.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

