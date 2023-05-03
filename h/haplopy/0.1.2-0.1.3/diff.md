# Comparing `tmp/haplopy-0.1.2.tar.gz` & `tmp/haplopy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haplopy-0.1.2.tar", last modified: Wed May  3 09:36:57 2023, max compression
+gzip compressed data, was "haplopy-0.1.3.tar", last modified: Wed May  3 09:42:16 2023, max compression
```

## Comparing `haplopy-0.1.2.tar` & `haplopy-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2023-05-03 09:36:57.558399 haplopy-0.1.2/
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     4871 2023-05-03 09:36:57.558399 haplopy-0.1.2/PKG-INFO
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     4160 2023-05-03 09:05:18.000000 haplopy-0.1.2/README.md
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2023-05-03 09:36:57.558399 haplopy-0.1.2/haplopy/
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      199 2023-05-03 09:05:18.000000 haplopy-0.1.2/haplopy/__init__.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     8368 2023-05-03 09:07:17.000000 haplopy-0.1.2/haplopy/datautils.py
--rwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)     9760 2023-05-03 09:05:18.000000 haplopy-0.1.2/haplopy/multinomial.py
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     2032 2023-05-03 09:35:51.000000 haplopy-0.1.2/haplopy/plot.py
-drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2023-05-03 09:36:57.558399 haplopy-0.1.2/haplopy.egg-info/
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     4871 2023-05-03 09:36:57.000000 haplopy-0.1.2/haplopy.egg-info/PKG-INFO
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      277 2023-05-03 09:36:57.000000 haplopy-0.1.2/haplopy.egg-info/SOURCES.txt
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        1 2023-05-03 09:36:57.000000 haplopy-0.1.2/haplopy.egg-info/dependency_links.txt
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)       69 2023-05-03 09:36:57.000000 haplopy-0.1.2/haplopy.egg-info/requires.txt
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        8 2023-05-03 09:36:57.000000 haplopy-0.1.2/haplopy.egg-info/top_level.txt
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      151 2023-05-03 09:05:18.000000 haplopy-0.1.2/pyproject.toml
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      867 2023-05-03 09:36:57.559399 haplopy-0.1.2/setup.cfg
--rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      148 2023-05-03 09:05:18.000000 haplopy-0.1.2/setup.py
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2023-05-03 09:42:16.931915 haplopy-0.1.3/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     4871 2023-05-03 09:42:16.931915 haplopy-0.1.3/PKG-INFO
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     4160 2023-05-03 09:05:18.000000 haplopy-0.1.3/README.md
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2023-05-03 09:42:16.931915 haplopy-0.1.3/haplopy/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      297 2023-05-03 09:41:20.000000 haplopy-0.1.3/haplopy/__init__.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     8368 2023-05-03 09:07:17.000000 haplopy-0.1.3/haplopy/datautils.py
+-rwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)     9760 2023-05-03 09:05:18.000000 haplopy-0.1.3/haplopy/multinomial.py
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     1994 2023-05-03 09:41:20.000000 haplopy-0.1.3/haplopy/plot.py
+drwxr-xr-x   0 malmgrek  (1000) malmgrek  (1000)        0 2023-05-03 09:42:16.931915 haplopy-0.1.3/haplopy.egg-info/
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)     4871 2023-05-03 09:42:16.000000 haplopy-0.1.3/haplopy.egg-info/PKG-INFO
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      277 2023-05-03 09:42:16.000000 haplopy-0.1.3/haplopy.egg-info/SOURCES.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        1 2023-05-03 09:42:16.000000 haplopy-0.1.3/haplopy.egg-info/dependency_links.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)       69 2023-05-03 09:42:16.000000 haplopy-0.1.3/haplopy.egg-info/requires.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)        8 2023-05-03 09:42:16.000000 haplopy-0.1.3/haplopy.egg-info/top_level.txt
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      151 2023-05-03 09:05:18.000000 haplopy-0.1.3/pyproject.toml
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      867 2023-05-03 09:42:16.932915 haplopy-0.1.3/setup.cfg
+-rw-r--r--   0 malmgrek  (1000) malmgrek  (1000)      148 2023-05-03 09:05:18.000000 haplopy-0.1.3/setup.py
```

### Comparing `haplopy-0.1.2/PKG-INFO` & `haplopy-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haplopy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Haplotype reconstruction from unphased diplotypes
 Home-page: https://github.com/malmgrek/haplopy
 Author: Stratos Staboulis <stratos@stratokraft.fi>
 Maintainer: Stratos Staboulis <stratos@stratokraft.fi>
 License: MIT
 Keywords: statistics,modeling,population genetics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `haplopy-0.1.2/README.md` & `haplopy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `haplopy-0.1.2/haplopy/datautils.py` & `haplopy-0.1.3/haplopy/datautils.py`

 * *Files identical despite different names*

### Comparing `haplopy-0.1.2/haplopy/multinomial.py` & `haplopy-0.1.3/haplopy/multinomial.py`

 * *Files identical despite different names*

### Comparing `haplopy-0.1.2/haplopy/plot.py` & `haplopy-0.1.3/haplopy/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 
 """
 
 from collections import Counter
 from typing import Dict, List, Tuple
 
 import numpy as np
-try:
-    import matplotlib.pyplot as plt
-except ImportError:
-    pass
+import matplotlib.pyplot as plt
 
 
 def plot_haplotypes(
         proba_haplotypes: Dict[Tuple[str], float],
         thres=1e-3,
         title=r"Haplotype relative frequencies (area $\sim$ p)",
         **kwargs
```

### Comparing `haplopy-0.1.2/haplopy.egg-info/PKG-INFO` & `haplopy-0.1.3/haplopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haplopy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Haplotype reconstruction from unphased diplotypes
 Home-page: https://github.com/malmgrek/haplopy
 Author: Stratos Staboulis <stratos@stratokraft.fi>
 Maintainer: Stratos Staboulis <stratos@stratokraft.fi>
 License: MIT
 Keywords: statistics,modeling,population genetics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `haplopy-0.1.2/setup.cfg` & `haplopy-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.1.2
+version = 0.1.3
 name = haplopy
 author = Stratos Staboulis <stratos@stratokraft.fi>
 maintainer = Stratos Staboulis <stratos@stratokraft.fi>
 license = MIT
 classifiers = 
 	Programming Language :: Python :: 3
 	Development Status :: 3 - Alpha
```

