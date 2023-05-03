# Comparing `tmp/dlclibrary-0.0.2.tar.gz` & `tmp/dlclibrary-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlclibrary-0.0.2.tar", last modified: Fri Dec 23 21:47:55 2022, max compression
+gzip compressed data, was "dlclibrary-0.0.3.tar", last modified: Wed May  3 12:04:27 2023, max compression
```

## Comparing `dlclibrary-0.0.2.tar` & `dlclibrary-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-12-23 21:47:55.769438 dlclibrary-0.0.2/
--rw-r--r--   0 alex       (501) staff       (20)     7652 2022-11-27 10:48:36.000000 dlclibrary-0.0.2/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)      441 2022-11-27 10:54:12.000000 dlclibrary-0.0.2/NOTICE.yml
--rw-r--r--   0 alex       (501) staff       (20)     1084 2022-12-23 21:47:55.769293 dlclibrary-0.0.2/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      558 2022-12-14 22:46:03.000000 dlclibrary-0.0.2/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-12-23 21:47:55.768186 dlclibrary-0.0.2/dlclibrary/
--rw-r--r--   0 alex       (501) staff       (20)      407 2022-12-20 20:16:30.000000 dlclibrary-0.0.2/dlclibrary/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-12-23 21:47:55.769127 dlclibrary-0.0.2/dlclibrary/dlcmodelzoo/
--rw-r--r--   0 alex       (501) staff       (20)      274 2022-12-20 20:16:30.000000 dlclibrary-0.0.2/dlclibrary/dlcmodelzoo/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2722 2022-12-23 21:40:20.000000 dlclibrary-0.0.2/dlclibrary/dlcmodelzoo/modelzoo_download.py
--rw-r--r--   0 alex       (501) staff       (20)     1912 2022-12-23 21:40:20.000000 dlclibrary-0.0.2/dlclibrary/modelzoo_urls.yaml
--rw-r--r--   0 alex       (501) staff       (20)      319 2022-12-23 21:45:24.000000 dlclibrary-0.0.2/dlclibrary/version.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-12-23 21:47:55.768738 dlclibrary-0.0.2/dlclibrary.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     1084 2022-12-23 21:47:55.000000 dlclibrary-0.0.2/dlclibrary.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      360 2022-12-23 21:47:55.000000 dlclibrary-0.0.2/dlclibrary.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2022-12-23 21:47:55.000000 dlclibrary-0.0.2/dlclibrary.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       36 2022-12-23 21:47:55.000000 dlclibrary-0.0.2/dlclibrary.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       11 2022-12-23 21:47:55.000000 dlclibrary-0.0.2/dlclibrary.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2022-12-23 21:47:55.769483 dlclibrary-0.0.2/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     1252 2022-12-23 21:45:24.000000 dlclibrary-0.0.2/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-03 12:04:27.285834 dlclibrary-0.0.3/
+-rw-r--r--   0 alex       (501) staff       (20)     7652 2022-11-27 10:48:36.000000 dlclibrary-0.0.3/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)      441 2022-11-27 10:54:12.000000 dlclibrary-0.0.3/NOTICE.yml
+-rw-r--r--   0 alex       (501) staff       (20)     1212 2023-05-03 12:04:27.285666 dlclibrary-0.0.3/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      686 2023-05-02 16:26:26.000000 dlclibrary-0.0.3/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-03 12:04:27.283018 dlclibrary-0.0.3/dlclibrary/
+-rw-r--r--   0 alex       (501) staff       (20)      449 2023-05-02 16:26:26.000000 dlclibrary-0.0.3/dlclibrary/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-03 12:04:27.284682 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/
+-rw-r--r--   0 alex       (501) staff       (20)      274 2022-12-20 20:16:30.000000 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2984 2023-05-03 12:03:32.000000 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/modelzoo_download.py
+-rw-r--r--   0 alex       (501) staff       (20)     1913 2023-05-02 16:27:02.000000 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/modelzoo_urls.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-03 12:04:27.285195 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/superanimal_configs/
+-rw-r--r--   0 alex       (501) staff       (20)     2329 2023-05-02 16:26:26.000000 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/superanimal_configs/superquadruped.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     1962 2023-05-02 16:26:26.000000 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/superanimal_configs/supertopview.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      108 2023-05-02 16:26:26.000000 dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/superanimal_models.json
+-rw-r--r--   0 alex       (501) staff       (20)      319 2023-05-03 12:03:32.000000 dlclibrary-0.0.3/dlclibrary/version.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-03 12:04:27.283696 dlclibrary-0.0.3/dlclibrary.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     1212 2023-05-03 12:04:27.000000 dlclibrary-0.0.3/dlclibrary.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      571 2023-05-03 12:04:27.000000 dlclibrary-0.0.3/dlclibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-05-03 12:04:27.000000 dlclibrary-0.0.3/dlclibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       36 2023-05-03 12:04:27.000000 dlclibrary-0.0.3/dlclibrary.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       11 2023-05-03 12:04:27.000000 dlclibrary-0.0.3/dlclibrary.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-05-03 12:04:27.285877 dlclibrary-0.0.3/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     1492 2023-05-03 12:03:32.000000 dlclibrary-0.0.3/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-03 12:04:27.285345 dlclibrary-0.0.3/tests/
+-rw-r--r--   0 alex       (501) staff       (20)     1330 2023-05-02 16:26:26.000000 dlclibrary-0.0.3/tests/test_modeldownload.py
```

### Comparing `dlclibrary-0.0.2/LICENSE` & `dlclibrary-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dlclibrary-0.0.2/PKG-INFO` & `dlclibrary-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlclibrary
-Version: 0.0.2
+Version: 0.0.3
 Summary: Lightweight library supporting universal functions for the DeepLabCut ecosystem
 Home-page: https://github.com/DeepLabCut/DLClib
 Author: A. & M. Mathis Labs
 Author-email: alexander@deeplabcut.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
@@ -17,7 +17,13 @@
 
 # DLClibrary
 
 DLClibrary is a lightweight library supporting universal functions for the DeepLabCut ecosystem.
 
 Supported functions (at this point):
 - API for downloading model weights from the model zoo
+
+# Quick start 
+
+`pip install dlclibrary`
+
+- warning, the closely named package `dlclib` is not an official DeepLabCut product.
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1 Name: dlclibrary Version: 0.0.2 Summary: Lightweight
+Metadata-Version: 2.1 Name: dlclibrary Version: 0.0.3 Summary: Lightweight
 library supporting universal functions for the DeepLabCut ecosystem Home-page:
 https://github.com/DeepLabCut/DLClib Author: A. & M. Mathis Labs Author-email:
 alexander@deeplabcut.org Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
 (LGPLv3) Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE License-File: NOTICE.yml [![Generic
 badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)]
 (README.md) [Code_style:_black][![License: LGPL v3](https://img.shields.io/
 badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0) #
 DLClibrary DLClibrary is a lightweight library supporting universal functions
 for the DeepLabCut ecosystem. Supported functions (at this point): - API for
-downloading model weights from the model zoo
+downloading model weights from the model zoo # Quick start `pip install
+dlclibrary` - warning, the closely named package `dlclib` is not an official
+DeepLabCut product.
```

### Comparing `dlclibrary-0.0.2/README.md` & `dlclibrary-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -3,7 +3,13 @@
 
 # DLClibrary
 
 DLClibrary is a lightweight library supporting universal functions for the DeepLabCut ecosystem.
 
 Supported functions (at this point):
 - API for downloading model weights from the model zoo
+
+# Quick start 
+
+`pip install dlclibrary`
+
+- warning, the closely named package `dlclib` is not an official DeepLabCut product.
```

#### html2text {}

```diff
@@ -1,6 +1,8 @@
 [![Generic badge](https://img.shields.io/badge/Contributions-Welcome-
 brightgreen.svg)](README.md) [Code_style:_black][![License: LGPL v3](https://
 img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/
 lgpl-3.0) # DLClibrary DLClibrary is a lightweight library supporting universal
 functions for the DeepLabCut ecosystem. Supported functions (at this point): -
-API for downloading model weights from the model zoo
+API for downloading model weights from the model zoo # Quick start `pip install
+dlclibrary` - warning, the closely named package `dlclib` is not an official
+DeepLabCut product.
```

### Comparing `dlclibrary-0.0.2/dlclibrary/dlcmodelzoo/modelzoo_download.py` & `dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/modelzoo_download.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 # https://github.com/DeepLabCut/DeepLabCut
 #
 # Please see AUTHORS for contributors.
 # https://github.com/DeepLabCut/DeepLabCut/blob/master/AUTHORS
 #
 # Licensed under GNU Lesser General Public License v3.0
 #
+import json
 import os
 
 # just expand this list when adding new models:
 MODELOPTIONS = [
     "full_human",
     "full_cat",
+    "full_dog",
     "primate_face",
     "mouse_pupil_vclose",
     "horse_sideview",
     "full_macaque",
     "superanimal_topviewmouse",
     "superanimal_quadruped",
 ]
@@ -30,19 +32,26 @@
     return os.path.split(importlib.util.find_spec("dlclibrary").origin)[0]
 
 
 def _load_model_names():
     """Load URLs and commit hashes for available models."""
     from ruamel.yaml import YAML
 
-    fn = os.path.join(_get_dlclibrary_path(), "modelzoo_urls.yaml")
+    fn = os.path.join(_get_dlclibrary_path(), "dlcmodelzoo", "modelzoo_urls.yaml")
     with open(fn) as file:
         return YAML().load(file)
 
 
+def parse_available_supermodels():
+    libpath = _get_dlclibrary_path()
+    json_path = os.path.join(libpath, "dlcmodelzoo", "superanimal_models.json")
+    with open(json_path) as file:
+        return json.load(file)
+
+
 def download_huggingface_model(modelname, target_dir=".", remove_hf_folder=True):
     """
     Download a DeepLabCut Model Zoo Project from Hugging Face
 
     Parameters
     ----------
     modelname : string
```

### Comparing `dlclibrary-0.0.2/dlclibrary/modelzoo_urls.yaml` & `dlclibrary-0.0.3/dlclibrary/dlcmodelzoo/modelzoo_urls.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 
 
 #Model Zoo from HuggingFace
 full_human: mwmathis/DeepLabCutModelZoo-DLC_human_fullbody_resnet_101/DLC_human_dancing_resnet_101_iteration-0_shuffle-1.tar.gz
 full_human_commit: 01acf989bfec7a25110b94677449d9e861b5ea81
 full_cat: AlexEMG/DeepLabCutModelZoo-cat/DLC_Cat_resnet_50_iteration-0_shuffle-0.tar.gz
-full_cat_commit: 972f82dc575c820ce556e140465495a32d18ee9b
+full_cat_commit: d39b3922a04d7077a84a05d141243c044cc18af6
 full_dog: AlexEMG/DeepLabCutModelZoo-dog/DLC_Dog_resnet_50_iteration-0_shuffle-0.tar.gz
-full_dog_commit: 3d7cae9dff2625fadffb11e25190119c9ff936a1
+full_dog_commit: b420a859f881b3cabdfd0cc4a0eb2d1c7fb592c5
 
 primate_face: mwmathis/DeepLabCutModelZoo-primate_face/DLC_primate_face_resnet_50_iteration-1_shuffle-1.tar.gz
 primate_face_commit: df7e8f6ad38899489758e5a890b58905cfb4d893
 
 mouse_pupil_vclose: mwmathis/DeepLabCutModelZoo-mouse_pupil_vclose/DLC_mouse_pupil_vclose_resnet_50_iteration-0_shuffle-1.tar.gz
 mouse_pupil_vclose_commit: 93557f0e74390596a2b9fddaab7628a1cc79fb2d
 
@@ -31,8 +31,8 @@
 full_macaque: mwmathis/DeepLabCutModelZoo-macaque_full/DLC_macaque_full_resnet50.tar.gz
 full_macaque_commit: 4c7ebf2628d5b7eb0483356595256fb01b7e1a9e
 
 superanimal_topviewmouse: mwmathis/DeepLabCutModelZoo-SuperAnimal-TopViewMouse/DLC_ma_supertopview5k_resnet_50_iteration-0_shuffle-1.tar.gz
 superanimal_topviewmouse_commit: a7d7df40c3307a3c7a0ceeb2593d46a783235b28
 
 superanimal_quadruped: mwmathis/DeepLabCutModelZoo-SuperAnimal-Quadruped/DLC_ma_superquadruped_resnet_50_iteration-0_shuffle-1.tar.gz
-superanimal_quadruped_commit: 829b336a52fff0e03f2f87c75b1e2638989122c7
+superanimal_quadruped_commit: 829b336a52fff0e03f2f87c75b1e2638989122c7
```

### Comparing `dlclibrary-0.0.2/dlclibrary.egg-info/PKG-INFO` & `dlclibrary-0.0.3/dlclibrary.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlclibrary
-Version: 0.0.2
+Version: 0.0.3
 Summary: Lightweight library supporting universal functions for the DeepLabCut ecosystem
 Home-page: https://github.com/DeepLabCut/DLClib
 Author: A. & M. Mathis Labs
 Author-email: alexander@deeplabcut.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
@@ -17,7 +17,13 @@
 
 # DLClibrary
 
 DLClibrary is a lightweight library supporting universal functions for the DeepLabCut ecosystem.
 
 Supported functions (at this point):
 - API for downloading model weights from the model zoo
+
+# Quick start 
+
+`pip install dlclibrary`
+
+- warning, the closely named package `dlclib` is not an official DeepLabCut product.
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1 Name: dlclibrary Version: 0.0.2 Summary: Lightweight
+Metadata-Version: 2.1 Name: dlclibrary Version: 0.0.3 Summary: Lightweight
 library supporting universal functions for the DeepLabCut ecosystem Home-page:
 https://github.com/DeepLabCut/DLClib Author: A. & M. Mathis Labs Author-email:
 alexander@deeplabcut.org Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
 (LGPLv3) Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE License-File: NOTICE.yml [![Generic
 badge](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)]
 (README.md) [Code_style:_black][![License: LGPL v3](https://img.shields.io/
 badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0) #
 DLClibrary DLClibrary is a lightweight library supporting universal functions
 for the DeepLabCut ecosystem. Supported functions (at this point): - API for
-downloading model weights from the model zoo
+downloading model weights from the model zoo # Quick start `pip install
+dlclibrary` - warning, the closely named package `dlclib` is not an official
+DeepLabCut product.
```

