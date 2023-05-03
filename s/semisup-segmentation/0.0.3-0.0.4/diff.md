# Comparing `tmp/semisup-segmentation-0.0.3.tar.gz` & `tmp/semisup-segmentation-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/semisup-segmentation-0.0.3.tar", last modified: Wed May  3 11:04:37 2023, max compression
+gzip compressed data, was "dist/semisup-segmentation-0.0.4.tar", last modified: Wed May  3 11:11:55 2023, max compression
```

## Comparing `semisup-segmentation-0.0.3.tar` & `semisup-segmentation-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:04:37.000000 semisup-segmentation-0.0.3/
--rw-rw-r--   0 adines    (1000) adines    (1000)      620 2023-05-03 11:04:37.000000 semisup-segmentation-0.0.3/PKG-INFO
--rw-rw-r--   0 adines    (1000) adines    (1000)     1071 2020-12-11 12:52:05.000000 semisup-segmentation-0.0.3/LICENSE.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)     1197 2020-12-16 16:41:18.000000 semisup-segmentation-0.0.3/README.rst
-drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:04:37.000000 semisup-segmentation-0.0.3/semisup_segmentation.egg-info/
--rw-rw-r--   0 adines    (1000) adines    (1000)      620 2023-05-03 11:04:37.000000 semisup-segmentation-0.0.3/semisup_segmentation.egg-info/PKG-INFO
--rw-rw-r--   0 adines    (1000) adines    (1000)      157 2023-05-03 11:04:37.000000 semisup-segmentation-0.0.3/semisup_segmentation.egg-info/requires.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)        1 2023-05-03 11:04:37.000000 semisup-segmentation-0.0.3/semisup_segmentation.egg-info/dependency_links.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)      344 2023-05-03 11:04:37.000000 semisup-segmentation-0.0.3/semisup_segmentation.egg-info/SOURCES.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)       11 2023-05-03 11:04:37.000000 semisup-segmentation-0.0.3/semisup_segmentation.egg-info/top_level.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)     8386 2023-05-03 11:04:35.000000 semisup-segmentation-0.0.3/setup.py
--rw-rw-r--   0 adines    (1000) adines    (1000)       46 2020-12-11 12:52:32.000000 semisup-segmentation-0.0.3/MANIFEST.in
--rw-rw-r--   0 adines    (1000) adines    (1000)       67 2023-05-03 11:04:37.000000 semisup-segmentation-0.0.3/setup.cfg
-drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:04:37.000000 semisup-segmentation-0.0.3/SemiSegAPI/
--rw-rw-r--   0 adines    (1000) adines    (1000)     8342 2023-05-02 16:24:16.000000 semisup-segmentation-0.0.3/SemiSegAPI/semiSupervised.py
--rw-rw-r--   0 adines    (1000) adines    (1000)        0 2023-05-02 14:47:34.000000 semisup-segmentation-0.0.3/SemiSegAPI/__init__.py
--rw-rw-r--   0 adines    (1000) adines    (1000)    10397 2023-05-03 07:51:02.000000 semisup-segmentation-0.0.3/SemiSegAPI/utils.py
+drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:11:55.000000 semisup-segmentation-0.0.4/
+-rw-rw-r--   0 adines    (1000) adines    (1000)      635 2023-05-03 11:11:55.000000 semisup-segmentation-0.0.4/PKG-INFO
+-rw-rw-r--   0 adines    (1000) adines    (1000)     1071 2020-12-11 12:52:05.000000 semisup-segmentation-0.0.4/LICENSE.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)     1197 2020-12-16 16:41:18.000000 semisup-segmentation-0.0.4/README.rst
+drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:11:55.000000 semisup-segmentation-0.0.4/semisup_segmentation.egg-info/
+-rw-rw-r--   0 adines    (1000) adines    (1000)      635 2023-05-03 11:11:55.000000 semisup-segmentation-0.0.4/semisup_segmentation.egg-info/PKG-INFO
+-rw-rw-r--   0 adines    (1000) adines    (1000)      157 2023-05-03 11:11:55.000000 semisup-segmentation-0.0.4/semisup_segmentation.egg-info/requires.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)        1 2023-05-03 11:11:55.000000 semisup-segmentation-0.0.4/semisup_segmentation.egg-info/dependency_links.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)      344 2023-05-03 11:11:55.000000 semisup-segmentation-0.0.4/semisup_segmentation.egg-info/SOURCES.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)       11 2023-05-03 11:11:55.000000 semisup-segmentation-0.0.4/semisup_segmentation.egg-info/top_level.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)     8386 2023-05-03 11:11:52.000000 semisup-segmentation-0.0.4/setup.py
+-rw-rw-r--   0 adines    (1000) adines    (1000)       46 2020-12-11 12:52:32.000000 semisup-segmentation-0.0.4/MANIFEST.in
+-rw-rw-r--   0 adines    (1000) adines    (1000)       67 2023-05-03 11:11:55.000000 semisup-segmentation-0.0.4/setup.cfg
+drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 11:11:55.000000 semisup-segmentation-0.0.4/SemiSegAPI/
+-rw-rw-r--   0 adines    (1000) adines    (1000)     8342 2023-05-02 16:24:16.000000 semisup-segmentation-0.0.4/SemiSegAPI/semiSupervised.py
+-rw-rw-r--   0 adines    (1000) adines    (1000)        0 2023-05-02 14:47:34.000000 semisup-segmentation-0.0.4/SemiSegAPI/__init__.py
+-rw-rw-r--   0 adines    (1000) adines    (1000)    10397 2023-05-03 07:51:02.000000 semisup-segmentation-0.0.4/SemiSegAPI/utils.py
```

### Comparing `semisup-segmentation-0.0.3/PKG-INFO` & `semisup-segmentation-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: semisup-segmentation
-Version: 0.0.3
+Version: 0.0.4
 Summary: API that provides methods to construct deep segmentation models using semi-supervised methods.
 Home-page: https://github.com/adines/SemiSeg
 Author: Adrian Ines
 Author-email: adines@unirioja.es
 License: UNKNOWN
-Description: UNKNOWN
 Keywords: segmentation,deep learning,semi-supervised
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE.txt
+
+UNKNOWN
+
```

### Comparing `semisup-segmentation-0.0.3/LICENSE.txt` & `semisup-segmentation-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `semisup-segmentation-0.0.3/README.rst` & `semisup-segmentation-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `semisup-segmentation-0.0.3/semisup_segmentation.egg-info/PKG-INFO` & `semisup-segmentation-0.0.4/semisup_segmentation.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: semisup-segmentation
-Version: 0.0.3
+Version: 0.0.4
 Summary: API that provides methods to construct deep segmentation models using semi-supervised methods.
 Home-page: https://github.com/adines/SemiSeg
 Author: Adrian Ines
 Author-email: adines@unirioja.es
 License: UNKNOWN
-Description: UNKNOWN
 Keywords: segmentation,deep learning,semi-supervised
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE.txt
+
+UNKNOWN
+
```

### Comparing `semisup-segmentation-0.0.3/setup.py` & `semisup-segmentation-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.3',  # Required
+    version='0.0.4',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='API that provides methods to construct deep segmentation models using semi-supervised methods.',  # Required
 
     # This is an optional longer description of your project that represents
```

### Comparing `semisup-segmentation-0.0.3/SemiSegAPI/semiSupervised.py` & `semisup-segmentation-0.0.4/SemiSegAPI/semiSupervised.py`

 * *Files identical despite different names*

### Comparing `semisup-segmentation-0.0.3/SemiSegAPI/utils.py` & `semisup-segmentation-0.0.4/SemiSegAPI/utils.py`

 * *Files identical despite different names*

