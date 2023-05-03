# Comparing `tmp/atppy-0.1.2.tar.gz` & `tmp/atppy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atppy-0.1.2.tar", last modified: Sun Apr 30 06:27:23 2023, max compression
+gzip compressed data, was "atppy-0.1.3.tar", last modified: Wed May  3 06:38:16 2023, max compression
```

## Comparing `atppy-0.1.2.tar` & `atppy-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 josephfarrell   (501) staff       (20)        0 2023-04-30 06:27:23.026150 atppy-0.1.2/
--rw-r--r--   0 josephfarrell   (501) staff       (20)      599 2023-04-30 06:27:23.026216 atppy-0.1.2/PKG-INFO
-drwxr-xr-x   0 josephfarrell   (501) staff       (20)        0 2023-04-30 06:27:23.026116 atppy-0.1.2/atppy/
--rw-r--r--   0 josephfarrell   (501) staff       (20)      138 2023-04-30 06:20:09.466641 atppy-0.1.2/atppy/__init__.py
--rw-r--r--   0 josephfarrell   (501) staff       (20)       39 2023-04-29 04:24:57.772239 atppy-0.1.2/setup.cfg
--rw-r--r--   0 josephfarrell   (501) staff       (20)      656 2023-04-30 06:26:54.368401 atppy-0.1.2/setup.py
+drwxr-xr-x   0 josephfarrell   (501) staff       (20)        0 2023-05-03 06:38:16.891319 atppy-0.1.3/
+-rw-r--r--   0 josephfarrell   (501) staff       (20)      599 2023-05-03 06:38:16.891397 atppy-0.1.3/PKG-INFO
+drwxr-xr-x   0 josephfarrell   (501) staff       (20)        0 2023-05-03 06:38:16.891290 atppy-0.1.3/atppy/
+-rw-r--r--   0 josephfarrell   (501) staff       (20)      152 2023-04-30 20:22:02.671041 atppy-0.1.3/atppy/__init__.py
+-rw-r--r--   0 josephfarrell   (501) staff       (20)       39 2023-04-29 04:24:57.772239 atppy-0.1.3/setup.cfg
+-rw-r--r--   0 josephfarrell   (501) staff       (20)      656 2023-05-03 06:37:15.310430 atppy-0.1.3/setup.py
```

### Comparing `atppy-0.1.2/PKG-INFO` & `atppy-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atppy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python library for AT Protocol
 Home-page: https://github.com/Gladdstone/atppy
 Author: Joseph Farrell
 Author-email: joe.farrell373@gmail.com
 License: MIT
 Download-URL: https://github.com/Gladdstone/atppy/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `atppy-0.1.2/setup.py` & `atppy-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'atppy',
   packages = ['atppy'],
-  version = '0.1.2',
+  version = '0.1.3',
   license='MIT',
   description = 'Python library for AT Protocol',
   author = 'Joseph Farrell',
   author_email = 'joe.farrell373@gmail.com',
   url = 'https://github.com/Gladdstone/atppy',
   download_url = 'https://github.com/Gladdstone/atppy/archive/v_01.tar.gz',
   keywords = ['at protocol', 'bluesky', 'bsky'],
```

