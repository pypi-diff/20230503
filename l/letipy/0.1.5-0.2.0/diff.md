# Comparing `tmp/letipy-0.1.5.tar.gz` & `tmp/letipy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\letipy-0.1.5.tar", last modified: Wed May  3 15:56:54 2023, max compression
+gzip compressed data, was "dist\letipy-0.2.0.tar", last modified: Wed May  3 16:04:05 2023, max compression
```

## Comparing `letipy-0.1.5.tar` & `letipy-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 15:56:54.815794 letipy-0.1.5/
--rw-rw-rw-   0        0        0      400 2023-05-03 15:56:54.812794 letipy-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 15:56:54.783793 letipy-0.1.5/code/
--rw-rw-rw-   0        0        0     7338 2023-05-03 15:29:13.000000 letipy-0.1.5/code/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 15:56:54.808794 letipy-0.1.5/letipy.egg-info/
--rw-rw-rw-   0        0        0      400 2023-05-03 15:56:54.000000 letipy-0.1.5/letipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-05-03 15:56:54.000000 letipy-0.1.5/letipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 15:56:54.000000 letipy-0.1.5/letipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-03 15:56:54.000000 letipy-0.1.5/letipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 15:56:54.000000 letipy-0.1.5/letipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 15:56:54.815794 letipy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      498 2023-05-03 15:56:28.000000 letipy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:04:05.530182 letipy-0.2.0/
+-rw-rw-rw-   0        0        0      400 2023-05-03 16:04:05.514582 letipy-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 16:04:05.498981 letipy-0.2.0/code/
+-rw-rw-rw-   0        0        0     7325 2023-05-03 16:00:15.000000 letipy-0.2.0/code/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:04:05.514582 letipy-0.2.0/letipy.egg-info/
+-rw-rw-rw-   0        0        0      400 2023-05-03 16:04:04.000000 letipy-0.2.0/letipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-05-03 16:04:05.000000 letipy-0.2.0/letipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 16:04:04.000000 letipy-0.2.0/letipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-03 16:04:04.000000 letipy-0.2.0/letipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-03 16:04:04.000000 letipy-0.2.0/letipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 16:04:05.530182 letipy-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-05-03 16:03:38.000000 letipy-0.2.0/setup.py
```

### Comparing `letipy-0.1.5/code/__init__.py` & `letipy-0.2.0/code/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # This is a powerful scientific strings-processing called "StiPy"
 
 import numpy as np
 import re
 import os
 from afinn import Afinn
 import nltk
-import math
 import gmpy2
 import afinn
 
 def arrex(words):
     """
     Convert a string or list of strings to a numerical representation using a numpy array.
     """
```

