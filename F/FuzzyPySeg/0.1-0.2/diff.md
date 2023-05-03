# Comparing `tmp/FuzzyPySeg-0.1.tar.gz` & `tmp/FuzzyPySeg-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuzzyPySeg-0.1.tar", last modified: Wed May  3 03:08:56 2023, max compression
+gzip compressed data, was "FuzzyPySeg-0.2.tar", last modified: Wed May  3 03:41:40 2023, max compression
```

## Comparing `FuzzyPySeg-0.1.tar` & `FuzzyPySeg-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 03:08:56.391829 FuzzyPySeg-0.1/
-drwxrwxrwx   0        0        0        0 2023-05-03 03:08:56.383500 FuzzyPySeg-0.1/FuzzyPySeg/
--rw-rw-rw-   0        0        0    25128 2023-05-03 03:02:53.000000 FuzzyPySeg-0.1/FuzzyPySeg/FuzzyPySeg.py
--rw-rw-rw-   0        0        0       17 2023-05-03 03:03:28.000000 FuzzyPySeg-0.1/FuzzyPySeg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:08:56.390621 FuzzyPySeg-0.1/FuzzyPySeg.egg-info/
--rw-rw-rw-   0        0        0     1112 2023-05-03 03:08:56.000000 FuzzyPySeg-0.1/FuzzyPySeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-05-03 03:08:56.000000 FuzzyPySeg-0.1/FuzzyPySeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 03:08:56.000000 FuzzyPySeg-0.1/FuzzyPySeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-03 03:08:56.000000 FuzzyPySeg-0.1/FuzzyPySeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-03 03:08:56.000000 FuzzyPySeg-0.1/FuzzyPySeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1077 2023-05-03 02:55:20.000000 FuzzyPySeg-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1112 2023-05-03 03:08:56.391829 FuzzyPySeg-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2488 2023-05-03 03:05:54.000000 FuzzyPySeg-0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-05-03 03:08:56.392834 FuzzyPySeg-0.1/setup.cfg
--rw-rw-rw-   0        0        0     2074 2023-05-03 02:55:20.000000 FuzzyPySeg-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:41:40.732337 FuzzyPySeg-0.2/
+drwxrwxrwx   0        0        0        0 2023-05-03 03:41:40.726125 FuzzyPySeg-0.2/FuzzyPySeg/
+-rw-rw-rw-   0        0        0    25128 2023-05-03 03:02:53.000000 FuzzyPySeg-0.2/FuzzyPySeg/FuzzyPySeg.py
+-rw-rw-rw-   0        0        0       26 2023-05-03 03:34:29.000000 FuzzyPySeg-0.2/FuzzyPySeg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:41:40.732337 FuzzyPySeg-0.2/FuzzyPySeg.egg-info/
+-rw-rw-rw-   0        0        0     1112 2023-05-03 03:41:40.000000 FuzzyPySeg-0.2/FuzzyPySeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-03 03:41:40.000000 FuzzyPySeg-0.2/FuzzyPySeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 03:41:40.000000 FuzzyPySeg-0.2/FuzzyPySeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-03 03:41:40.000000 FuzzyPySeg-0.2/FuzzyPySeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 03:41:40.000000 FuzzyPySeg-0.2/FuzzyPySeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1077 2023-05-03 02:55:20.000000 FuzzyPySeg-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1112 2023-05-03 03:41:40.732337 FuzzyPySeg-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2488 2023-05-03 03:05:54.000000 FuzzyPySeg-0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-03 03:41:40.732337 FuzzyPySeg-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2074 2023-05-03 03:41:07.000000 FuzzyPySeg-0.2/setup.py
```

### Comparing `FuzzyPySeg-0.1/FuzzyPySeg/FuzzyPySeg.py` & `FuzzyPySeg-0.2/FuzzyPySeg/FuzzyPySeg.py`

 * *Files identical despite different names*

### Comparing `FuzzyPySeg-0.1/FuzzyPySeg.egg-info/PKG-INFO` & `FuzzyPySeg-0.2/FuzzyPySeg.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: FuzzyPySeg
-Version: 0.1
+Version: 0.2
 Summary: FuzzyPySeg is a package for segmenting images using Fuzzy C Means clustering with either a Euclidean or Mahalanobis distance. You may also specify a centroid initialization using the firefly algorithm, genetic algorithm, or the Biogeography-based optimization algorithm.
 Home-page: https://github.com/Danyulll/FuzzyPySeg
-Download-URL: https://github.com/Danyulll/FuzzyPySeg/archive/refs/tags/v0.0.1.tar.gz
+Download-URL: https://github.com/Danyulll/FuzzyPySeg/archive/refs/tags/v0.0.2.tar.gz
 Author: Daniel Krasnov
 Author-email: dkrasnov@student.ubc.ca
 License: MIT
 Keywords: image segmentation,clustering,fuzzy c-means,firefly algorithm,genetic algorithm,biogeography-based optimization algorithm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `FuzzyPySeg-0.1/LICENSE.txt` & `FuzzyPySeg-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FuzzyPySeg-0.1/PKG-INFO` & `FuzzyPySeg-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: FuzzyPySeg
-Version: 0.1
+Version: 0.2
 Summary: FuzzyPySeg is a package for segmenting images using Fuzzy C Means clustering with either a Euclidean or Mahalanobis distance. You may also specify a centroid initialization using the firefly algorithm, genetic algorithm, or the Biogeography-based optimization algorithm.
 Home-page: https://github.com/Danyulll/FuzzyPySeg
-Download-URL: https://github.com/Danyulll/FuzzyPySeg/archive/refs/tags/v0.0.1.tar.gz
+Download-URL: https://github.com/Danyulll/FuzzyPySeg/archive/refs/tags/v0.0.2.tar.gz
 Author: Daniel Krasnov
 Author-email: dkrasnov@student.ubc.ca
 License: MIT
 Keywords: image segmentation,clustering,fuzzy c-means,firefly algorithm,genetic algorithm,biogeography-based optimization algorithm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `FuzzyPySeg-0.1/README.md` & `FuzzyPySeg-0.2/README.md`

 * *Files identical despite different names*

### Comparing `FuzzyPySeg-0.1/setup.py` & `FuzzyPySeg-0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'FuzzyPySeg',         # How you named your package folder (MyLib)
   packages = ['FuzzyPySeg'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'FuzzyPySeg is a package for segmenting images using Fuzzy C Means clustering with either a Euclidean or Mahalanobis distance. You may also specify a centroid initialization using the firefly algorithm, genetic algorithm, or the Biogeography-based optimization algorithm.',   # Give a short description about your library
   author = 'Daniel Krasnov',                   # Type in your name
   author_email = 'dkrasnov@student.ubc.ca',      # Type in your E-Mail
   url = 'https://github.com/Danyulll/FuzzyPySeg',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/Danyulll/FuzzyPySeg/archive/refs/tags/v0.0.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/Danyulll/FuzzyPySeg/archive/refs/tags/v0.0.2.tar.gz',    # I explain this later on
   keywords = ['image segmentation', 'clustering', 'fuzzy c-means', 'firefly algorithm', 'genetic algorithm', 'biogeography-based optimization algorithm'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'Image',
           'numba',
           'scipy'
       ],
```

