# Comparing `tmp/prepup-0.0.19.tar.gz` & `tmp/prepup-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepup-0.0.19.tar", last modified: Wed May  3 18:31:48 2023, max compression
+gzip compressed data, was "prepup-0.1.1.tar", last modified: Wed May  3 18:44:57 2023, max compression
```

## Comparing `prepup-0.0.19.tar` & `prepup-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 18:31:48.452517 prepup-0.0.19/
--rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.0.19/AUTHORS.rst
--rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.0.19/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.0.19/MANIFEST.in
--rw-rw-rw-   0        0        0     4300 2023-05-03 18:31:48.451418 prepup-0.0.19/PKG-INFO
--rw-rw-rw-   0        0        0     3723 2023-05-03 18:29:37.000000 prepup-0.0.19/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 18:31:48.439900 prepup-0.0.19/prepup/
--rw-rw-rw-   0        0        0     7969 2023-05-03 18:15:40.000000 prepup-0.0.19/prepup/__init__.py
--rw-rw-rw-   0        0        0    33177 2023-05-03 18:14:07.000000 prepup-0.0.19/prepup/common.py
-drwxrwxrwx   0        0        0        0 2023-05-03 18:31:48.449415 prepup-0.0.19/prepup.egg-info/
--rw-rw-rw-   0        0        0     4300 2023-05-03 18:31:48.000000 prepup-0.0.19/prepup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-05-03 18:31:48.000000 prepup-0.0.19/prepup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 18:31:48.000000 prepup-0.0.19/prepup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-03 18:31:48.000000 prepup-0.0.19/prepup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      220 2023-05-03 18:31:48.000000 prepup-0.0.19/prepup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 18:31:48.000000 prepup-0.0.19/prepup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      367 2023-04-29 23:00:31.000000 prepup-0.0.19/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 18:31:48.453519 prepup-0.0.19/setup.cfg
--rw-rw-rw-   0        0        0     1489 2023-05-03 18:31:37.000000 prepup-0.0.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:44:57.597042 prepup-0.1.1/
+-rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4246 2023-05-03 18:44:57.595040 prepup-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3710 2023-05-03 18:43:20.000000 prepup-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 18:44:57.576451 prepup-0.1.1/prepup/
+-rw-rw-rw-   0        0        0     7969 2023-05-03 18:15:40.000000 prepup-0.1.1/prepup/__init__.py
+-rw-rw-rw-   0        0        0    33177 2023-05-03 18:14:07.000000 prepup-0.1.1/prepup/common.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:44:57.593027 prepup-0.1.1/prepup.egg-info/
+-rw-rw-rw-   0        0        0     4246 2023-05-03 18:44:57.000000 prepup-0.1.1/prepup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-05-03 18:44:57.000000 prepup-0.1.1/prepup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 18:44:57.000000 prepup-0.1.1/prepup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-03 18:44:57.000000 prepup-0.1.1/prepup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      220 2023-05-03 18:44:57.000000 prepup-0.1.1/prepup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 18:44:57.000000 prepup-0.1.1/prepup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      367 2023-04-29 23:00:31.000000 prepup-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 18:44:57.598040 prepup-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2023-05-03 18:44:52.000000 prepup-0.1.1/setup.py
```

### Comparing `prepup-0.0.19/LICENSE` & `prepup-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prepup-0.0.19/PKG-INFO` & `prepup-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prepup
-Version: 0.0.19
+Version: 0.1.1
 Summary: Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.
 Author: Sudhanshu Mukherjee
 Author-email: sudhanshumukherjeexx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
@@ -16,15 +16,15 @@
 
 
 [![image](https://img.shields.io/pypi/v/prepup.svg)](https://pypi.python.org/pypi/prepup)
 [![image](https://img.shields.io/conda/vn/conda-forge/prepup.svg)](https://anaconda.org/conda-forge/prepup)
 
 
 
-### Prepup is a free open-source package that lets you inspect, explore, visualize, and perform pre-processing tasks on datasets in your computerâ€™s terminal.
+### Prepup is a free open-source package that lets you inspect, explore, visualize, and perform pre-processing tasks on datasets in your windows/macOS terminal.
 
 ## Installation
 -   Prepup can be installed using the Pip package manager.
 
 ### !pip install prepup
 
 ## Motivation
@@ -69,22 +69,22 @@
 ## prepup <File name or File path> -visualize
 
 -   visualize flag plots the feature distribution directly on the terminal.
 
 ## prepup <File name or File path> -impute
 - There are 8 different strategies available to impute missing data using Prepup
 
-    - Option 1 â€“ Drops the Missing Data
-    - Option 2 â€“ Impute Missing values with a Specific value
-    - Option 3 â€“ Impute Missing values with Mean.
-    - Option 4 â€“ Impute Missing values with Median.
-    - Option 5 â€“ Impute Missing value based on the distribution of existing columns.
-    - Option 6 â€“ Impute Missing values based on Forward Fill Strategy where missing values are imputed based on the previous data points.
+    - Option 1 - Drops the Missing Data
+    - Option 2 - Impute Missing values with a Specific value
+    - Option 3 - Impute Missing values with Mean.
+    - Option 4 - Impute Missing values with Median.
+    - Option 5 - Impute Missing value based on the distribution of existing columns.
+    - Option 6 - Impute Missing values based on Forward Fill Strategy where missing values are imputed based on the previous data points.
     - Option 7 - Impute Missing values based on Backward Strategy where missing values are imputed based on the next data points.
-    - Option 8 â€“ Impute missing values based on K-Nearest Neighbors.
+    - Option 8 - Impute missing values based on K-Nearest Neighbors.
 
 ## prepup <File name or File path> -standardize
 
 -   Standardize allows you to standardize the dataset using two different methods:
     1. Robust Scaler
 
     2. Standard Scaler
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prepup-0.0.19/README.md` & `prepup-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 [![image](https://img.shields.io/pypi/v/prepup.svg)](https://pypi.python.org/pypi/prepup)
 [![image](https://img.shields.io/conda/vn/conda-forge/prepup.svg)](https://anaconda.org/conda-forge/prepup)
 
 
 
-### Prepup is a free open-source package that lets you inspect, explore, visualize, and perform pre-processing tasks on datasets in your computer’s terminal.
+### Prepup is a free open-source package that lets you inspect, explore, visualize, and perform pre-processing tasks on datasets in your windows/macOS terminal.
 
 ## Installation
 -   Prepup can be installed using the Pip package manager.
 
 ### !pip install prepup
 
 ## Motivation
@@ -55,22 +55,22 @@
 ## prepup <File name or File path> -visualize
 
 -   visualize flag plots the feature distribution directly on the terminal.
 
 ## prepup <File name or File path> -impute
 - There are 8 different strategies available to impute missing data using Prepup
 
-    - Option 1 – Drops the Missing Data
-    - Option 2 – Impute Missing values with a Specific value
-    - Option 3 – Impute Missing values with Mean.
-    - Option 4 – Impute Missing values with Median.
-    - Option 5 – Impute Missing value based on the distribution of existing columns.
-    - Option 6 – Impute Missing values based on Forward Fill Strategy where missing values are imputed based on the previous data points.
+    - Option 1 - Drops the Missing Data
+    - Option 2 - Impute Missing values with a Specific value
+    - Option 3 - Impute Missing values with Mean.
+    - Option 4 - Impute Missing values with Median.
+    - Option 5 - Impute Missing value based on the distribution of existing columns.
+    - Option 6 - Impute Missing values based on Forward Fill Strategy where missing values are imputed based on the previous data points.
     - Option 7 - Impute Missing values based on Backward Strategy where missing values are imputed based on the next data points.
-    - Option 8 – Impute missing values based on K-Nearest Neighbors.
+    - Option 8 - Impute missing values based on K-Nearest Neighbors.
 
 ## prepup <File name or File path> -standardize
 
 -   Standardize allows you to standardize the dataset using two different methods:
     1. Robust Scaler
 
     2. Standard Scaler
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prepup-0.0.19/prepup/__init__.py` & `prepup-0.1.1/prepup/__init__.py`

 * *Files identical despite different names*

### Comparing `prepup-0.0.19/prepup/common.py` & `prepup-0.1.1/prepup/common.py`

 * *Files identical despite different names*

### Comparing `prepup-0.0.19/prepup.egg-info/PKG-INFO` & `prepup-0.1.1/prepup.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prepup
-Version: 0.0.19
+Version: 0.1.1
 Summary: Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.
 Author: Sudhanshu Mukherjee
 Author-email: sudhanshumukherjeexx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
@@ -16,15 +16,15 @@
 
 
 [![image](https://img.shields.io/pypi/v/prepup.svg)](https://pypi.python.org/pypi/prepup)
 [![image](https://img.shields.io/conda/vn/conda-forge/prepup.svg)](https://anaconda.org/conda-forge/prepup)
 
 
 
-### Prepup is a free open-source package that lets you inspect, explore, visualize, and perform pre-processing tasks on datasets in your computerâ€™s terminal.
+### Prepup is a free open-source package that lets you inspect, explore, visualize, and perform pre-processing tasks on datasets in your windows/macOS terminal.
 
 ## Installation
 -   Prepup can be installed using the Pip package manager.
 
 ### !pip install prepup
 
 ## Motivation
@@ -69,22 +69,22 @@
 ## prepup <File name or File path> -visualize
 
 -   visualize flag plots the feature distribution directly on the terminal.
 
 ## prepup <File name or File path> -impute
 - There are 8 different strategies available to impute missing data using Prepup
 
-    - Option 1 â€“ Drops the Missing Data
-    - Option 2 â€“ Impute Missing values with a Specific value
-    - Option 3 â€“ Impute Missing values with Mean.
-    - Option 4 â€“ Impute Missing values with Median.
-    - Option 5 â€“ Impute Missing value based on the distribution of existing columns.
-    - Option 6 â€“ Impute Missing values based on Forward Fill Strategy where missing values are imputed based on the previous data points.
+    - Option 1 - Drops the Missing Data
+    - Option 2 - Impute Missing values with a Specific value
+    - Option 3 - Impute Missing values with Mean.
+    - Option 4 - Impute Missing values with Median.
+    - Option 5 - Impute Missing value based on the distribution of existing columns.
+    - Option 6 - Impute Missing values based on Forward Fill Strategy where missing values are imputed based on the previous data points.
     - Option 7 - Impute Missing values based on Backward Strategy where missing values are imputed based on the next data points.
-    - Option 8 â€“ Impute missing values based on K-Nearest Neighbors.
+    - Option 8 - Impute missing values based on K-Nearest Neighbors.
 
 ## prepup <File name or File path> -standardize
 
 -   Standardize allows you to standardize the dataset using two different methods:
     1. Robust Scaler
 
     2. Standard Scaler
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prepup-0.0.19/setup.py` & `prepup-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setuptools.setup(
     name="prepup",
-    version="0.0.19",
+    version="0.1.1",
     author="Sudhanshu Mukherjee",
     author_email="sudhanshumukherjeexx@gmail.com",
     description="Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     entry_points={
```

