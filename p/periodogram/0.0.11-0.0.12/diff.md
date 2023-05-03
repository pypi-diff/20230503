# Comparing `tmp/periodogram-0.0.11.tar.gz` & `tmp/periodogram-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periodogram-0.0.11.tar", last modified: Thu Apr 20 00:38:03 2023, max compression
+gzip compressed data, was "periodogram-0.0.12.tar", last modified: Wed May  3 14:54:47 2023, max compression
```

## Comparing `periodogram-0.0.11.tar` & `periodogram-0.0.12.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-20 00:38:03.316663 periodogram-0.0.11/
--rw-r--r--   0 daniel     (501) staff       (20)     1378 2023-04-20 00:38:03.316532 periodogram-0.0.11/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      977 2023-04-20 00:36:08.000000 periodogram-0.0.11/README.md
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-20 00:38:03.315600 periodogram-0.0.11/periodogram/
--rw-r--r--   0 daniel     (501) staff       (20)       56 2023-04-20 00:36:08.000000 periodogram-0.0.11/periodogram/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)     2650 2023-04-19 22:30:49.000000 periodogram-0.0.11/periodogram/estimator.py
--rw-r--r--   0 daniel     (501) staff       (20)     3079 2023-04-20 00:36:08.000000 periodogram-0.0.11/periodogram/normalization.py
--rw-r--r--   0 daniel     (501) staff       (20)     4669 2023-04-20 00:36:08.000000 periodogram-0.0.11/periodogram/periodogram.py
--rw-r--r--   0 daniel     (501) staff       (20)      519 2023-04-19 22:39:05.000000 periodogram-0.0.11/periodogram/utils.py
--rw-r--r--   0 daniel     (501) staff       (20)       23 2023-04-19 23:05:55.000000 periodogram-0.0.11/periodogram/version.py
--rw-r--r--   0 daniel     (501) staff       (20)     3215 2023-04-19 22:23:07.000000 periodogram-0.0.11/periodogram/window.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-20 00:38:03.316372 periodogram-0.0.11/periodogram.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)     1378 2023-04-20 00:38:03.000000 periodogram-0.0.11/periodogram.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      363 2023-04-20 00:38:03.000000 periodogram-0.0.11/periodogram.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-04-20 00:38:03.000000 periodogram-0.0.11/periodogram.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)       25 2023-04-20 00:38:03.000000 periodogram-0.0.11/periodogram.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)       12 2023-04-20 00:38:03.000000 periodogram-0.0.11/periodogram.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-04-20 00:38:03.316700 periodogram-0.0.11/setup.cfg
--rw-r--r--   0 daniel     (501) staff       (20)      836 2023-04-19 23:04:31.000000 periodogram-0.0.11/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-03 14:54:47.470099 periodogram-0.0.12/
+-rw-r--r--   0 daniel     (501) staff       (20)     1378 2023-05-03 14:54:47.469979 periodogram-0.0.12/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      977 2023-04-20 00:36:08.000000 periodogram-0.0.12/README.md
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-03 14:54:47.469172 periodogram-0.0.12/periodogram/
+-rw-r--r--   0 daniel     (501) staff       (20)       56 2023-04-20 00:36:08.000000 periodogram-0.0.12/periodogram/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2650 2023-04-19 22:30:49.000000 periodogram-0.0.12/periodogram/estimator.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3079 2023-04-20 00:36:08.000000 periodogram-0.0.12/periodogram/normalization.py
+-rw-r--r--   0 daniel     (501) staff       (20)     4669 2023-04-20 00:36:08.000000 periodogram-0.0.12/periodogram/periodogram.py
+-rw-r--r--   0 daniel     (501) staff       (20)      519 2023-04-19 22:39:05.000000 periodogram-0.0.12/periodogram/utils.py
+-rw-r--r--   0 daniel     (501) staff       (20)       23 2023-05-03 14:53:11.000000 periodogram-0.0.12/periodogram/version.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3215 2023-04-19 22:23:07.000000 periodogram-0.0.12/periodogram/window.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-03 14:54:47.469830 periodogram-0.0.12/periodogram.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)     1378 2023-05-03 14:54:47.000000 periodogram-0.0.12/periodogram.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      363 2023-05-03 14:54:47.000000 periodogram-0.0.12/periodogram.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-03 14:54:47.000000 periodogram-0.0.12/periodogram.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       25 2023-05-03 14:54:47.000000 periodogram-0.0.12/periodogram.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       12 2023-05-03 14:54:47.000000 periodogram-0.0.12/periodogram.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-03 14:54:47.470135 periodogram-0.0.12/setup.cfg
+-rw-r--r--   0 daniel     (501) staff       (20)      854 2023-05-03 14:53:45.000000 periodogram-0.0.12/setup.py
```

### Comparing `periodogram-0.0.11/PKG-INFO` & `periodogram-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periodogram
-Version: 0.0.11
+Version: 0.0.12
 Summary: Simple periodogram manipulation in Python.
 Home-page: https://github.com/danhey/periodogram
 Author: Daniel Hey
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `periodogram-0.0.11/README.md` & `periodogram-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.11/periodogram/estimator.py` & `periodogram-0.0.12/periodogram/estimator.py`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.11/periodogram/normalization.py` & `periodogram-0.0.12/periodogram/normalization.py`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.11/periodogram/periodogram.py` & `periodogram-0.0.12/periodogram/periodogram.py`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.11/periodogram/utils.py` & `periodogram-0.0.12/periodogram/utils.py`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.11/periodogram/window.py` & `periodogram-0.0.12/periodogram/window.py`

 * *Files identical despite different names*

### Comparing `periodogram-0.0.11/periodogram.egg-info/PKG-INFO` & `periodogram-0.0.12/periodogram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periodogram
-Version: 0.0.11
+Version: 0.0.12
 Summary: Simple periodogram manipulation in Python.
 Home-page: https://github.com/danhey/periodogram
 Author: Daniel Hey
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `periodogram-0.0.11/setup.py` & `periodogram-0.0.12/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     long_description_content_type="text/markdown",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
     ],
-    install_requires=install_requires,
+    install_requires=["astropy", "numpy", "matplotlib"],
 )
```

