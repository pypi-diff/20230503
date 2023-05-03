# Comparing `tmp/periodogram-0.0.12.tar.gz` & `tmp/periodogram-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periodogram-0.0.12.tar", last modified: Wed May  3 14:54:47 2023, max compression
+gzip compressed data, was "periodogram-0.0.13.tar", last modified: Wed May  3 14:58:55 2023, max compression
```

## Comparing `periodogram-0.0.12.tar` & `periodogram-0.0.13.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-03 14:54:47.470099 periodogram-0.0.12/
--rw-r--r--   0 daniel     (501) staff       (20)     1378 2023-05-03 14:54:47.469979 periodogram-0.0.12/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      977 2023-04-20 00:36:08.000000 periodogram-0.0.12/README.md
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-03 14:54:47.469172 periodogram-0.0.12/periodogram/
--rw-r--r--   0 daniel     (501) staff       (20)       56 2023-04-20 00:36:08.000000 periodogram-0.0.12/periodogram/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     2650 2023-04-19 22:30:49.000000 periodogram-0.0.12/periodogram/estimator.py
--rw-r--r--   0 daniel     (501) staff       (20)     3079 2023-04-20 00:36:08.000000 periodogram-0.0.12/periodogram/normalization.py
--rw-r--r--   0 daniel     (501) staff       (20)     4669 2023-04-20 00:36:08.000000 periodogram-0.0.12/periodogram/periodogram.py
--rw-r--r--   0 daniel     (501) staff       (20)      519 2023-04-19 22:39:05.000000 periodogram-0.0.12/periodogram/utils.py
--rw-r--r--   0 daniel     (501) staff       (20)       23 2023-05-03 14:53:11.000000 periodogram-0.0.12/periodogram/version.py
--rw-r--r--   0 daniel     (501) staff       (20)     3215 2023-04-19 22:23:07.000000 periodogram-0.0.12/periodogram/window.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-03 14:54:47.469830 periodogram-0.0.12/periodogram.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)     1378 2023-05-03 14:54:47.000000 periodogram-0.0.12/periodogram.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      363 2023-05-03 14:54:47.000000 periodogram-0.0.12/periodogram.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-03 14:54:47.000000 periodogram-0.0.12/periodogram.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)       25 2023-05-03 14:54:47.000000 periodogram-0.0.12/periodogram.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)       12 2023-05-03 14:54:47.000000 periodogram-0.0.12/periodogram.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-03 14:54:47.470135 periodogram-0.0.12/setup.cfg
--rw-r--r--   0 daniel     (501) staff       (20)      854 2023-05-03 14:53:45.000000 periodogram-0.0.12/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-03 14:58:55.222539 periodogram-0.0.13/
+-rw-r--r--   0 daniel     (501) staff       (20)     1378 2023-05-03 14:58:55.222401 periodogram-0.0.13/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      977 2023-04-20 00:36:08.000000 periodogram-0.0.13/README.md
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-03 14:58:55.221540 periodogram-0.0.13/periodogram/
+-rw-r--r--   0 daniel     (501) staff       (20)       56 2023-04-20 00:36:08.000000 periodogram-0.0.13/periodogram/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2650 2023-04-19 22:30:49.000000 periodogram-0.0.13/periodogram/estimator.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3079 2023-04-20 00:36:08.000000 periodogram-0.0.13/periodogram/normalization.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4669 2023-04-20 00:36:08.000000 periodogram-0.0.13/periodogram/periodogram.py
+-rw-r--r--   0 daniel     (501) staff       (20)      519 2023-04-19 22:39:05.000000 periodogram-0.0.13/periodogram/utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)       23 2023-05-03 14:53:11.000000 periodogram-0.0.13/periodogram/version.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3215 2023-04-19 22:23:07.000000 periodogram-0.0.13/periodogram/window.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-03 14:58:55.222215 periodogram-0.0.13/periodogram.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)     1378 2023-05-03 14:58:55.000000 periodogram-0.0.13/periodogram.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      363 2023-05-03 14:58:55.000000 periodogram-0.0.13/periodogram.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-03 14:58:55.000000 periodogram-0.0.13/periodogram.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       25 2023-05-03 14:58:55.000000 periodogram-0.0.13/periodogram.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       12 2023-05-03 14:58:55.000000 periodogram-0.0.13/periodogram.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-03 14:58:55.222585 periodogram-0.0.13/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)      855 2023-05-03 14:55:44.000000 periodogram-0.0.13/setup.py
```

### Comparing `periodogram-0.0.12/PKG-INFO` & `periodogram-0.0.13/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periodogram
-Version: 0.0.12
+Version: 0.0.13
 Summary: Simple periodogram manipulation in Python.
 Home-page: https://github.com/danhey/periodogram
 Author: Daniel Hey
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `periodogram-0.0.12/README.md` & `periodogram-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.12/periodogram/estimator.py` & `periodogram-0.0.13/periodogram/estimator.py`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.12/periodogram/normalization.py` & `periodogram-0.0.13/periodogram/normalization.py`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.12/periodogram/periodogram.py` & `periodogram-0.0.13/periodogram/periodogram.py`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.12/periodogram/utils.py` & `periodogram-0.0.13/periodogram/utils.py`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.12/periodogram/window.py` & `periodogram-0.0.13/periodogram/window.py`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.12/periodogram.egg-info/PKG-INFO` & `periodogram-0.0.13/periodogram.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periodogram
-Version: 0.0.12
+Version: 0.0.13
 Summary: Simple periodogram manipulation in Python.
 Home-page: https://github.com/danhey/periodogram
 Author: Daniel Hey
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `periodogram-0.0.12/setup.py` & `periodogram-0.0.13/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 import os
 import sys
 from setuptools import setup
 
-with open("requirements.txt") as f:
-    install_requires = f.read().splitlines()
+# with open("requirements.txt") as f:
+#     install_requires = f.read().splitlines()
 
 # Load the __version__ variable without importing the package already
 exec(open("periodogram/version.py").read())
 
 setup(
     name="periodogram",
-    version=__version__,
+    version="0.0.13",
     author="Daniel Hey",
     url="https://github.com/danhey/periodogram",
     packages=["periodogram"],
     description="Simple periodogram manipulation in Python.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
```

