# Comparing `tmp/semisup-segmentation-0.0.1.tar.gz` & `tmp/semisup-segmentation-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/semisup-segmentation-0.0.1.tar", last modified: Wed May  3 07:48:17 2023, max compression
+gzip compressed data, was "dist/semisup-segmentation-0.0.2.tar", last modified: Wed May  3 07:51:05 2023, max compression
```

## Comparing `semisup-segmentation-0.0.1.tar` & `semisup-segmentation-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 07:48:17.000000 semisup-segmentation-0.0.1/
--rw-rw-r--   0 adines    (1000) adines    (1000)      620 2023-05-03 07:48:17.000000 semisup-segmentation-0.0.1/PKG-INFO
--rw-rw-r--   0 adines    (1000) adines    (1000)     1071 2020-12-11 12:52:05.000000 semisup-segmentation-0.0.1/LICENSE.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)     1197 2020-12-16 16:41:18.000000 semisup-segmentation-0.0.1/README.rst
-drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 07:48:17.000000 semisup-segmentation-0.0.1/semisup_segmentation.egg-info/
--rw-rw-r--   0 adines    (1000) adines    (1000)      620 2023-05-03 07:48:17.000000 semisup-segmentation-0.0.1/semisup_segmentation.egg-info/PKG-INFO
--rw-rw-r--   0 adines    (1000) adines    (1000)      157 2023-05-03 07:48:17.000000 semisup-segmentation-0.0.1/semisup_segmentation.egg-info/requires.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)        1 2023-05-03 07:48:17.000000 semisup-segmentation-0.0.1/semisup_segmentation.egg-info/dependency_links.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)      344 2023-05-03 07:48:17.000000 semisup-segmentation-0.0.1/semisup_segmentation.egg-info/SOURCES.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)       11 2023-05-03 07:48:17.000000 semisup-segmentation-0.0.1/semisup_segmentation.egg-info/top_level.txt
--rw-rw-r--   0 adines    (1000) adines    (1000)     8385 2023-05-03 07:47:52.000000 semisup-segmentation-0.0.1/setup.py
--rw-rw-r--   0 adines    (1000) adines    (1000)       46 2020-12-11 12:52:32.000000 semisup-segmentation-0.0.1/MANIFEST.in
--rw-rw-r--   0 adines    (1000) adines    (1000)       67 2023-05-03 07:48:17.000000 semisup-segmentation-0.0.1/setup.cfg
-drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 07:48:17.000000 semisup-segmentation-0.0.1/SemiSegAPI/
--rw-rw-r--   0 adines    (1000) adines    (1000)     8342 2023-05-02 16:24:16.000000 semisup-segmentation-0.0.1/SemiSegAPI/semiSupervised.py
--rw-rw-r--   0 adines    (1000) adines    (1000)        0 2023-05-02 14:47:34.000000 semisup-segmentation-0.0.1/SemiSegAPI/__init__.py
--rw-rw-r--   0 adines    (1000) adines    (1000)    10472 2023-05-02 16:24:16.000000 semisup-segmentation-0.0.1/SemiSegAPI/utils.py
+drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 07:51:05.000000 semisup-segmentation-0.0.2/
+-rw-rw-r--   0 adines    (1000) adines    (1000)      620 2023-05-03 07:51:05.000000 semisup-segmentation-0.0.2/PKG-INFO
+-rw-rw-r--   0 adines    (1000) adines    (1000)     1071 2020-12-11 12:52:05.000000 semisup-segmentation-0.0.2/LICENSE.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)     1197 2020-12-16 16:41:18.000000 semisup-segmentation-0.0.2/README.rst
+drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 07:51:05.000000 semisup-segmentation-0.0.2/semisup_segmentation.egg-info/
+-rw-rw-r--   0 adines    (1000) adines    (1000)      620 2023-05-03 07:51:05.000000 semisup-segmentation-0.0.2/semisup_segmentation.egg-info/PKG-INFO
+-rw-rw-r--   0 adines    (1000) adines    (1000)      157 2023-05-03 07:51:05.000000 semisup-segmentation-0.0.2/semisup_segmentation.egg-info/requires.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)        1 2023-05-03 07:51:05.000000 semisup-segmentation-0.0.2/semisup_segmentation.egg-info/dependency_links.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)      344 2023-05-03 07:51:05.000000 semisup-segmentation-0.0.2/semisup_segmentation.egg-info/SOURCES.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)       11 2023-05-03 07:51:05.000000 semisup-segmentation-0.0.2/semisup_segmentation.egg-info/top_level.txt
+-rw-rw-r--   0 adines    (1000) adines    (1000)     8385 2023-05-03 07:51:02.000000 semisup-segmentation-0.0.2/setup.py
+-rw-rw-r--   0 adines    (1000) adines    (1000)       46 2020-12-11 12:52:32.000000 semisup-segmentation-0.0.2/MANIFEST.in
+-rw-rw-r--   0 adines    (1000) adines    (1000)       67 2023-05-03 07:51:05.000000 semisup-segmentation-0.0.2/setup.cfg
+drwxrwxr-x   0 adines    (1000) adines    (1000)        0 2023-05-03 07:51:05.000000 semisup-segmentation-0.0.2/SemiSegAPI/
+-rw-rw-r--   0 adines    (1000) adines    (1000)     8342 2023-05-02 16:24:16.000000 semisup-segmentation-0.0.2/SemiSegAPI/semiSupervised.py
+-rw-rw-r--   0 adines    (1000) adines    (1000)        0 2023-05-02 14:47:34.000000 semisup-segmentation-0.0.2/SemiSegAPI/__init__.py
+-rw-rw-r--   0 adines    (1000) adines    (1000)    10397 2023-05-03 07:51:02.000000 semisup-segmentation-0.0.2/SemiSegAPI/utils.py
```

### Comparing `semisup-segmentation-0.0.1/PKG-INFO` & `semisup-segmentation-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: semisup-segmentation
-Version: 0.0.1
+Version: 0.0.2
 Summary: API that provides methods to construct deep segmentation models using semi-supervised methods.
 Home-page: https://github.com/adines/SemiSeg
 Author: Adrian Ines
 Author-email: adines@unirioja.es
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: segmentation,deep learning,semi-supervised
```

### Comparing `semisup-segmentation-0.0.1/LICENSE.txt` & `semisup-segmentation-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `semisup-segmentation-0.0.1/README.rst` & `semisup-segmentation-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `semisup-segmentation-0.0.1/semisup_segmentation.egg-info/PKG-INFO` & `semisup-segmentation-0.0.2/semisup_segmentation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: semisup-segmentation
-Version: 0.0.1
+Version: 0.0.2
 Summary: API that provides methods to construct deep segmentation models using semi-supervised methods.
 Home-page: https://github.com/adines/SemiSeg
 Author: Adrian Ines
 Author-email: adines@unirioja.es
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: segmentation,deep learning,semi-supervised
```

### Comparing `semisup-segmentation-0.0.1/setup.py` & `semisup-segmentation-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.1',  # Required
+    version='0.0.2',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='API that provides methods to construct deep segmentation models using semi-supervised methods.',  # Required
 
     # This is an optional longer description of your project that represents
```

### Comparing `semisup-segmentation-0.0.1/SemiSegAPI/semiSupervised.py` & `semisup-segmentation-0.0.2/SemiSegAPI/semiSupervised.py`

 * *Files identical despite different names*

### Comparing `semisup-segmentation-0.0.1/SemiSegAPI/utils.py` & `semisup-segmentation-0.0.2/SemiSegAPI/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     CLAHE,
     ShiftScaleRotate
 )
 
 from tqdm import tqdm_notebook as tqdm
 
 
-availableModels=['ResNet18','ResNet50','ResNet101','EfficientNet','FBNet','MixNet','MNasNet','MobileNet','SqueezeNet','ShuffleNet']
+availableModels=['BiSeNet','CGNet', 'FPENet', 'DeepLab']
 availableTransforms=['H Flip','V Flip','H+V Flip','Blurring','Gamma','Gaussian Blur','Median Blur','Bilateral Filter','Equalize histogram','2D-Filter']
 
 def testNameModel(model):
     return model in availableModels
 
 def testPath(path):
     if os.path.isdir(path+os.sep+'train') and os.path.isdir(path+os.sep+'valid'):
```

