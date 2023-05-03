# Comparing `tmp/TPHATE-0.0.3.tar.gz` & `tmp/TPHATE-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/elb/Library/CloudStorage/GoogleDrive-erica.busch@yale.edu/My Drive/DriveLocal/Projects/NTB/poetry/TPHATE/dist/.tmp-frza9", last modified: Wed Apr 26 18:41:33 2023, max compression
+gzip compressed data, was "/Users/elb/Library/CloudStorage/GoogleDrive-erica.busch@yale.edu/My Drive/DriveLocal/Projects/NTB/poetry/TPHATE/dist/.tmp-d7vwj", last modified: Wed May  3 18:01:52 2023, max compression
```

## Comparing `TPHATE-0.0.3.tar` & `TPHATE-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-04-26 18:41:33.995239 TPHATE-0.0.3/
--rw-r--r--   0 elb        (501) staff       (20)    35149 2023-04-25 23:34:37.000000 TPHATE-0.0.3/LICENSE
--rw-r--r--   0 elb        (501) staff       (20)     1787 2023-04-26 18:41:33.994965 TPHATE-0.0.3/PKG-INFO
--rw-r--r--   0 elb        (501) staff       (20)     1155 2023-04-26 18:10:21.000000 TPHATE-0.0.3/README.md
--rw-r--r--   0 elb        (501) staff       (20)      761 2023-04-26 18:41:03.000000 TPHATE-0.0.3/pyproject.toml
--rw-r--r--   0 elb        (501) staff       (20)       38 2023-04-26 18:41:33.995336 TPHATE-0.0.3/setup.cfg
-drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-04-26 18:41:33.988628 TPHATE-0.0.3/src/
-drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-04-26 18:41:33.991077 TPHATE-0.0.3/src/TPHATE.egg-info/
--rw-r--r--   0 elb        (501) staff       (20)     1787 2023-04-26 18:41:33.000000 TPHATE-0.0.3/src/TPHATE.egg-info/PKG-INFO
--rw-r--r--   0 elb        (501) staff       (20)      390 2023-04-26 18:41:33.000000 TPHATE-0.0.3/src/TPHATE.egg-info/SOURCES.txt
--rw-r--r--   0 elb        (501) staff       (20)        1 2023-04-26 18:41:33.000000 TPHATE-0.0.3/src/TPHATE.egg-info/dependency_links.txt
--rw-r--r--   0 elb        (501) staff       (20)        7 2023-04-26 18:41:33.000000 TPHATE-0.0.3/src/TPHATE.egg-info/top_level.txt
-drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-04-26 18:41:33.994327 TPHATE-0.0.3/src/tphate/
--rw-r--r--   0 elb        (501) staff       (20)       59 2023-04-26 18:31:46.000000 TPHATE-0.0.3/src/tphate/__init__.py
--rw-r--r--   0 elb        (501) staff       (20)    11774 2023-04-25 23:34:38.000000 TPHATE-0.0.3/src/tphate/api.py
--rw-r--r--   0 elb        (501) staff       (20)    41142 2023-04-25 23:34:38.000000 TPHATE-0.0.3/src/tphate/base.py
--rw-r--r--   0 elb        (501) staff       (20)    54724 2023-04-25 23:34:38.000000 TPHATE-0.0.3/src/tphate/graphs.py
--rw-r--r--   0 elb        (501) staff       (20)     2090 2023-04-25 23:34:38.000000 TPHATE-0.0.3/src/tphate/matrix.py
--rw-r--r--   0 elb        (501) staff       (20)     7430 2023-04-25 23:34:38.000000 TPHATE-0.0.3/src/tphate/mds.py
--rw-r--r--   0 elb        (501) staff       (20)    37913 2023-04-25 23:34:38.000000 TPHATE-0.0.3/src/tphate/tphate.py
--rw-r--r--   0 elb        (501) staff       (20)     9569 2023-04-25 23:34:38.000000 TPHATE-0.0.3/src/tphate/utils.py
--rw-r--r--   0 elb        (501) staff       (20)       21 2023-04-26 18:29:27.000000 TPHATE-0.0.3/src/tphate/version.py
--rw-r--r--   0 elb        (501) staff       (20)     3966 2023-04-25 23:34:38.000000 TPHATE-0.0.3/src/tphate/vne.py
-drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-04-26 18:41:33.994617 TPHATE-0.0.3/tests/
--rw-r--r--   0 elb        (501) staff       (20)       83 2023-04-25 23:37:03.000000 TPHATE-0.0.3/tests/test_tphate.py
+drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-05-03 18:01:52.984699 TPHATE-0.0.4/
+-rw-r--r--   0 elb        (501) staff       (20)    35149 2023-04-25 23:34:37.000000 TPHATE-0.0.4/LICENSE
+-rw-r--r--   0 elb        (501) staff       (20)     1785 2023-05-03 18:01:52.984367 TPHATE-0.0.4/PKG-INFO
+-rw-r--r--   0 elb        (501) staff       (20)     1153 2023-05-03 17:57:42.000000 TPHATE-0.0.4/README.md
+-rw-r--r--   0 elb        (501) staff       (20)      952 2023-05-03 18:01:21.000000 TPHATE-0.0.4/pyproject.toml
+-rw-r--r--   0 elb        (501) staff       (20)       38 2023-05-03 18:01:52.984802 TPHATE-0.0.4/setup.cfg
+drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-05-03 18:01:52.970800 TPHATE-0.0.4/src/
+drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-05-03 18:01:52.974988 TPHATE-0.0.4/src/TPHATE.egg-info/
+-rw-r--r--   0 elb        (501) staff       (20)     1785 2023-05-03 18:01:52.000000 TPHATE-0.0.4/src/TPHATE.egg-info/PKG-INFO
+-rw-r--r--   0 elb        (501) staff       (20)      390 2023-05-03 18:01:52.000000 TPHATE-0.0.4/src/TPHATE.egg-info/SOURCES.txt
+-rw-r--r--   0 elb        (501) staff       (20)        1 2023-05-03 18:01:52.000000 TPHATE-0.0.4/src/TPHATE.egg-info/dependency_links.txt
+-rw-r--r--   0 elb        (501) staff       (20)        7 2023-05-03 18:01:52.000000 TPHATE-0.0.4/src/TPHATE.egg-info/top_level.txt
+drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-05-03 18:01:52.982926 TPHATE-0.0.4/src/tphate/
+-rw-r--r--   0 elb        (501) staff       (20)       59 2023-04-26 18:31:46.000000 TPHATE-0.0.4/src/tphate/__init__.py
+-rw-r--r--   0 elb        (501) staff       (20)    11774 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/api.py
+-rw-r--r--   0 elb        (501) staff       (20)    41142 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/base.py
+-rw-r--r--   0 elb        (501) staff       (20)    54724 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/graphs.py
+-rw-r--r--   0 elb        (501) staff       (20)     2090 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/matrix.py
+-rw-r--r--   0 elb        (501) staff       (20)     7430 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/mds.py
+-rw-r--r--   0 elb        (501) staff       (20)    37913 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/tphate.py
+-rw-r--r--   0 elb        (501) staff       (20)     9569 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/utils.py
+-rw-r--r--   0 elb        (501) staff       (20)       21 2023-04-26 18:29:27.000000 TPHATE-0.0.4/src/tphate/version.py
+-rw-r--r--   0 elb        (501) staff       (20)     3966 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/vne.py
+drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-05-03 18:01:52.983384 TPHATE-0.0.4/tests/
+-rw-r--r--   0 elb        (501) staff       (20)       83 2023-04-25 23:37:03.000000 TPHATE-0.0.4/tests/test_tphate.py
```

### Comparing `TPHATE-0.0.3/LICENSE` & `TPHATE-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TPHATE-0.0.3/PKG-INFO` & `TPHATE-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: TPHATE
-Version: 0.0.3
+Version: 0.0.4
 Summary: Temporal PHATE (TPHATE) is a python package for learning robust manifold representations of timeseries data with high temporal autocorrelation.
 Author-email: Erica Busch <ericalindseybusch@gmail.com>
 Project-URL: Homepage, https://github.com/KrishnaswamyLab/TPHATE/
 Project-URL: Bug Tracker, https://github.com/KrishnaswamyLab/TPHATE/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Quick Start
-If you would like to get started using T-PHATE, check out our [guided example](https://github.com/KrishnaswamyLab/TPHATE/blob/main/example/usage.ipynb).
+If you would like to get started using T-PHATE, check out our [guided example](https://github.com/KrishnaswamyLab/TPHATE/blob/main/tests/usage.ipynb).
 
 If you have loaded a data matrix `data` in python (with samples on rows, features on columns, where you believe the samples are non-independent), you can run TPHATE as follows:
 
 ```
 import tphate
 
 tphate_op = tphate.TPHATE()
```

### Comparing `TPHATE-0.0.3/README.md` & `TPHATE-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ## Quick Start
-If you would like to get started using T-PHATE, check out our [guided example](https://github.com/KrishnaswamyLab/TPHATE/blob/main/example/usage.ipynb).
+If you would like to get started using T-PHATE, check out our [guided example](https://github.com/KrishnaswamyLab/TPHATE/blob/main/tests/usage.ipynb).
 
 If you have loaded a data matrix `data` in python (with samples on rows, features on columns, where you believe the samples are non-independent), you can run TPHATE as follows:
 
 ```
 import tphate
 
 tphate_op = tphate.TPHATE()
```

### Comparing `TPHATE-0.0.3/pyproject.toml` & `TPHATE-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 [build-system]
 requires = [
 	"setuptools>=61.0", 
 	"statsmodels>=0.13.5",
 	"pytest>=7.2.1",
-	"phate"
+	"phate",
+	"numpy>=1.16.0",
+	"scipy>=1.1.0",
+	"scikit-learn>=0.20.0",
+	"future",
+	"tasklogger>=1.0",
+	"graphtools>=1.5.3",
+	"scprep>=1.0",
+	"matplotlib>=3.0",
+	"s_gd2>=1.8.1",
+	"pygsp",
+	"Deprecated"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TPHATE"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Erica Busch", email="ericalindseybusch@gmail.com" },
 ]
 description = "Temporal PHATE (TPHATE) is a python package for learning robust manifold representations of timeseries data with high temporal autocorrelation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `TPHATE-0.0.3/src/TPHATE.egg-info/PKG-INFO` & `TPHATE-0.0.4/src/TPHATE.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: TPHATE
-Version: 0.0.3
+Version: 0.0.4
 Summary: Temporal PHATE (TPHATE) is a python package for learning robust manifold representations of timeseries data with high temporal autocorrelation.
 Author-email: Erica Busch <ericalindseybusch@gmail.com>
 Project-URL: Homepage, https://github.com/KrishnaswamyLab/TPHATE/
 Project-URL: Bug Tracker, https://github.com/KrishnaswamyLab/TPHATE/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Quick Start
-If you would like to get started using T-PHATE, check out our [guided example](https://github.com/KrishnaswamyLab/TPHATE/blob/main/example/usage.ipynb).
+If you would like to get started using T-PHATE, check out our [guided example](https://github.com/KrishnaswamyLab/TPHATE/blob/main/tests/usage.ipynb).
 
 If you have loaded a data matrix `data` in python (with samples on rows, features on columns, where you believe the samples are non-independent), you can run TPHATE as follows:
 
 ```
 import tphate
 
 tphate_op = tphate.TPHATE()
```

### Comparing `TPHATE-0.0.3/src/tphate/api.py` & `TPHATE-0.0.4/src/tphate/api.py`

 * *Files identical despite different names*

### Comparing `TPHATE-0.0.3/src/tphate/base.py` & `TPHATE-0.0.4/src/tphate/base.py`

 * *Files identical despite different names*

### Comparing `TPHATE-0.0.3/src/tphate/graphs.py` & `TPHATE-0.0.4/src/tphate/graphs.py`

 * *Files identical despite different names*

### Comparing `TPHATE-0.0.3/src/tphate/matrix.py` & `TPHATE-0.0.4/src/tphate/matrix.py`

 * *Files identical despite different names*

### Comparing `TPHATE-0.0.3/src/tphate/mds.py` & `TPHATE-0.0.4/src/tphate/mds.py`

 * *Files identical despite different names*

### Comparing `TPHATE-0.0.3/src/tphate/tphate.py` & `TPHATE-0.0.4/src/tphate/tphate.py`

 * *Files identical despite different names*

### Comparing `TPHATE-0.0.3/src/tphate/utils.py` & `TPHATE-0.0.4/src/tphate/utils.py`

 * *Files identical despite different names*

### Comparing `TPHATE-0.0.3/src/tphate/vne.py` & `TPHATE-0.0.4/src/tphate/vne.py`

 * *Files identical despite different names*

