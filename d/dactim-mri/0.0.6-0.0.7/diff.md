# Comparing `tmp/dactim_mri-0.0.6.tar.gz` & `tmp/dactim_mri-0.0.7.tar.gz`

## Comparing `dactim_mri-0.0.6.tar` & `dactim_mri-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/requirements.txt
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/src/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/src/dactim_mri/__init__.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/src/dactim_mri/anonymization.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/src/dactim_mri/computation.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/src/dactim_mri/conversion.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/src/dactim_mri/sorting.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/src/dactim_mri/spectroscopy.py
--rw-r--r--   0        0        0    18621 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/src/dactim_mri/transformation.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/src/dactim_mri/utils.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/src/dactim_mri/visualization.py
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/LICENSE
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/README.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 dactim_mri-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/setup.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/src/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/src/dactim_mri/__init__.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/src/dactim_mri/anonymization.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/src/dactim_mri/computation.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/src/dactim_mri/conversion.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/src/dactim_mri/sorting.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/src/dactim_mri/spectroscopy.py
+-rw-r--r--   0        0        0    18621 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/src/dactim_mri/transformation.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/src/dactim_mri/utils.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/src/dactim_mri/visualization.py
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/README.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 dactim_mri-0.0.7/PKG-INFO
```

### Comparing `dactim_mri-0.0.6/src/dactim_mri/anonymization.py` & `dactim_mri-0.0.7/src/dactim_mri/anonymization.py`

 * *Files identical despite different names*

### Comparing `dactim_mri-0.0.6/src/dactim_mri/conversion.py` & `dactim_mri-0.0.7/src/dactim_mri/conversion.py`

 * *Files identical despite different names*

### Comparing `dactim_mri-0.0.6/src/dactim_mri/sorting.py` & `dactim_mri-0.0.7/src/dactim_mri/sorting.py`

 * *Files identical despite different names*

### Comparing `dactim_mri-0.0.6/src/dactim_mri/spectroscopy.py` & `dactim_mri-0.0.7/src/dactim_mri/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `dactim_mri-0.0.6/src/dactim_mri/transformation.py` & `dactim_mri-0.0.7/src/dactim_mri/transformation.py`

 * *Files identical despite different names*

### Comparing `dactim_mri-0.0.6/src/dactim_mri/utils.py` & `dactim_mri-0.0.7/src/dactim_mri/utils.py`

 * *Files identical despite different names*

### Comparing `dactim_mri-0.0.6/src/dactim_mri/visualization.py` & `dactim_mri-0.0.7/src/dactim_mri/visualization.py`

 * *Files identical despite different names*

### Comparing `dactim_mri-0.0.6/.gitignore` & `dactim_mri-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `dactim_mri-0.0.6/LICENSE` & `dactim_mri-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dactim_mri-0.0.6/README.md` & `dactim_mri-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Dactim_MRI
 
 [![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
-[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![Python 3.7](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Naereen/badges)
 [![PyPI version](https://badge.fury.io/py/dactim_mri.svg)](https://badge.fury.io/py/dactim_mri)
 
 ## Description
 
 A MRI preprocessing tool which provides a dozen of functions easy to use made from some of the most popular Python libraries 🚀
```

### Comparing `dactim_mri-0.0.6/PKG-INFO` & `dactim_mri-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dactim_mri
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool to preprocess mri data
 Author-email: Pierre FAYOLLE <pierre.fayolle@chu-poitiers.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Dactim_MRI
 
 [![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
-[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![Python 3.7](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Naereen/badges)
 [![PyPI version](https://badge.fury.io/py/dactim_mri.svg)](https://badge.fury.io/py/dactim_mri)
 
 ## Description
 
 A MRI preprocessing tool which provides a dozen of functions easy to use made from some of the most popular Python libraries 🚀
```

