# Comparing `tmp/gammy-0.4.9.tar.gz` & `tmp/gammy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammy-0.4.9.tar", last modified: Wed Nov 10 22:36:00 2021, max compression
+gzip compressed data, was "gammy-0.5.0.tar", last modified: Wed May  3 07:45:27 2023, max compression
```

## Comparing `gammy-0.4.9.tar` & `gammy-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 stastr    (1000) stastr    (1000)        0 2021-11-10 22:36:00.609077 gammy-0.4.9/
--rw-rw-r--   0 stastr    (1000) stastr    (1000)     1083 2021-09-21 21:46:20.000000 gammy-0.4.9/LICENSE.txt
--rw-rw-r--   0 stastr    (1000) stastr    (1000)       20 2021-09-21 21:46:20.000000 gammy-0.4.9/MANIFEST.in
--rw-rw-r--   0 stastr    (1000) stastr    (1000)    14714 2021-11-10 22:36:00.610077 gammy-0.4.9/PKG-INFO
--rw-rw-r--   0 stastr    (1000) stastr    (1000)    10731 2021-11-10 13:09:53.000000 gammy-0.4.9/README.md
-drwxrwxr-x   0 stastr    (1000) stastr    (1000)        0 2021-11-10 22:36:00.608077 gammy-0.4.9/gammy/
--rw-rw-r--   0 stastr    (1000) stastr    (1000)      535 2021-11-10 22:34:36.000000 gammy-0.4.9/gammy/__init__.py
--rw-rw-r--   0 stastr    (1000) stastr    (1000)      649 2021-11-10 22:34:36.000000 gammy-0.4.9/gammy/__version__.py
--rw-rw-r--   0 stastr    (1000) stastr    (1000)     3739 2021-10-27 21:55:49.000000 gammy-0.4.9/gammy/arraymapper.py
--rw-rw-r--   0 stastr    (1000) stastr    (1000)      561 2021-09-21 22:53:56.000000 gammy-0.4.9/gammy/conftest.py
--rw-rw-r--   0 stastr    (1000) stastr    (1000)    13795 2021-11-10 13:09:53.000000 gammy-0.4.9/gammy/formulae.py
-drwxrwxr-x   0 stastr    (1000) stastr    (1000)        0 2021-11-10 22:36:00.609077 gammy-0.4.9/gammy/models/
--rw-rw-r--   0 stastr    (1000) stastr    (1000)      125 2021-10-27 07:09:52.000000 gammy-0.4.9/gammy/models/__init__.py
--rw-rw-r--   0 stastr    (1000) stastr    (1000)    11466 2021-10-27 21:55:49.000000 gammy-0.4.9/gammy/models/bayespy.py
--rw-rw-r--   0 stastr    (1000) stastr    (1000)    11117 2021-10-27 07:09:52.000000 gammy-0.4.9/gammy/models/numpy.py
--rw-rw-r--   0 stastr    (1000) stastr    (1000)     7315 2021-11-10 21:26:35.000000 gammy-0.4.9/gammy/plot.py
--rw-rw-r--   0 stastr    (1000) stastr    (1000)     9626 2021-10-27 21:55:49.000000 gammy-0.4.9/gammy/utils.py
-drwxrwxr-x   0 stastr    (1000) stastr    (1000)        0 2021-11-10 22:36:00.609077 gammy-0.4.9/gammy.egg-info/
--rw-rw-r--   0 stastr    (1000) stastr    (1000)    14714 2021-11-10 22:36:00.000000 gammy-0.4.9/gammy.egg-info/PKG-INFO
--rw-rw-r--   0 stastr    (1000) stastr    (1000)      392 2021-11-10 22:36:00.000000 gammy-0.4.9/gammy.egg-info/SOURCES.txt
--rw-rw-r--   0 stastr    (1000) stastr    (1000)        1 2021-11-10 22:36:00.000000 gammy-0.4.9/gammy.egg-info/dependency_links.txt
--rw-rw-r--   0 stastr    (1000) stastr    (1000)       79 2021-11-10 22:36:00.000000 gammy-0.4.9/gammy.egg-info/requires.txt
--rw-rw-r--   0 stastr    (1000) stastr    (1000)        6 2021-11-10 22:36:00.000000 gammy-0.4.9/gammy.egg-info/top_level.txt
--rw-rw-r--   0 stastr    (1000) stastr    (1000)       67 2021-11-10 22:36:00.610077 gammy-0.4.9/setup.cfg
--rw-rw-r--   0 stastr    (1000) stastr    (1000)     1336 2021-11-10 22:27:32.000000 gammy-0.4.9/setup.py
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2023-05-03 07:45:27.722921 gammy-0.5.0/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     1083 2023-05-03 06:42:24.000000 gammy-0.5.0/LICENSE.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)       20 2023-05-03 06:42:24.000000 gammy-0.5.0/MANIFEST.in
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    11506 2023-05-03 07:45:27.722921 gammy-0.5.0/PKG-INFO
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    10730 2023-05-03 07:41:26.000000 gammy-0.5.0/README.md
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2023-05-03 07:45:27.721921 gammy-0.5.0/gammy/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      466 2023-05-03 07:31:01.000000 gammy-0.5.0/gammy/__init__.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     3739 2023-05-03 06:42:24.000000 gammy-0.5.0/gammy/arraymapper.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      561 2023-05-03 06:42:24.000000 gammy-0.5.0/gammy/conftest.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    13795 2023-05-03 06:42:24.000000 gammy-0.5.0/gammy/formulae.py
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2023-05-03 07:45:27.722921 gammy-0.5.0/gammy/models/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      125 2023-05-03 06:42:24.000000 gammy-0.5.0/gammy/models/__init__.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    11466 2023-05-03 06:42:24.000000 gammy-0.5.0/gammy/models/bayespy.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    11117 2023-05-03 06:42:24.000000 gammy-0.5.0/gammy/models/numpy.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     7315 2023-05-03 06:42:24.000000 gammy-0.5.0/gammy/plot.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     9626 2023-05-03 06:42:24.000000 gammy-0.5.0/gammy/utils.py
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2023-05-03 07:45:27.722921 gammy-0.5.0/gammy.egg-info/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)    11506 2023-05-03 07:45:27.000000 gammy-0.5.0/gammy.egg-info/PKG-INFO
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      386 2023-05-03 07:45:27.000000 gammy-0.5.0/gammy.egg-info/SOURCES.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        1 2023-05-03 07:45:27.000000 gammy-0.5.0/gammy.egg-info/dependency_links.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      105 2023-05-03 07:45:27.000000 gammy-0.5.0/gammy.egg-info/requires.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        6 2023-05-03 07:45:27.000000 gammy-0.5.0/gammy.egg-info/top_level.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      151 2023-05-03 07:31:01.000000 gammy-0.5.0/pyproject.toml
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      928 2023-05-03 07:45:27.723921 gammy-0.5.0/setup.cfg
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      148 2023-05-03 07:31:01.000000 gammy-0.5.0/setup.py
```

### Comparing `gammy-0.4.9/LICENSE.txt` & `gammy-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gammy-0.4.9/README.md` & `gammy-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,22 +52,22 @@
 
 ### Polynomial regression on 'roids
 
 A typical simple (but sometimes non-trivial) modeling task is to estimate an
 unknown function from noisy data. First we import the bare minimum dependencies to be used in the below examples:
 
 ```python
->>> from functools import reduce
-
->>> import matplotlib.pyplot as plt
 >>> import numpy as np
 
 >>> import gammy
 >>> from gammy.models.bayespy import GAM
 
+>>> gammy.__version__
+'0.5.0'
+
 ```
 
 Let's simulate a dataset:
 
 ```python
 >>> np.random.seed(42)
 
@@ -309,15 +309,15 @@
 
 ![](https://raw.githubusercontent.com/malmgrek/gammy/develop/doc/resources/spline-density.png)
 
 ### Non-linear manifold regression
 
 In this example we try estimating the bivariate "MATLAB function" using a
 Gaussian process model with Kronecker tensor structure (see e.g.
-[PyMC3](https://docs.pymc.io/notebooks/GP-Kron.html)). The main point in the
+[PyMC3](https://docs.pymc.io/en/v3/pymc-examples/examples/gaussian_processes/GP-Kron.html)). The main point in the
 below example is that it is quite straightforward to build models that can learn
 arbitrary 2D-surfaces.
 
 Let us first create some artificial data using the MATLAB function!
 
 ```python
 >>> n = 100
```

### Comparing `gammy-0.4.9/gammy/arraymapper.py` & `gammy-0.5.0/gammy/arraymapper.py`

 * *Files identical despite different names*

### Comparing `gammy-0.4.9/gammy/conftest.py` & `gammy-0.5.0/gammy/conftest.py`

 * *Files identical despite different names*

### Comparing `gammy-0.4.9/gammy/formulae.py` & `gammy-0.5.0/gammy/formulae.py`

 * *Files identical despite different names*

### Comparing `gammy-0.4.9/gammy/models/bayespy.py` & `gammy-0.5.0/gammy/models/bayespy.py`

 * *Files identical despite different names*

### Comparing `gammy-0.4.9/gammy/models/numpy.py` & `gammy-0.5.0/gammy/models/numpy.py`

 * *Files identical despite different names*

### Comparing `gammy-0.4.9/gammy/plot.py` & `gammy-0.5.0/gammy/plot.py`

 * *Files identical despite different names*

### Comparing `gammy-0.4.9/gammy/utils.py` & `gammy-0.5.0/gammy/utils.py`

 * *Files identical despite different names*

