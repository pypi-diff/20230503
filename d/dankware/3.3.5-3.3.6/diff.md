# Comparing `tmp/dankware-3.3.5.tar.gz` & `tmp/dankware-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dankware-3.3.5.tar", last modified: Sat Apr 15 10:09:28 2023, max compression
+gzip compressed data, was "dankware-3.3.6.tar", last modified: Wed May  3 10:16:02 2023, max compression
```

## Comparing `dankware-3.3.5.tar` & `dankware-3.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:28.407583 dankware-3.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-15 10:09:15.000000 dankware-3.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-04-15 10:09:28.407583 dankware-3.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-04-15 10:09:15.000000 dankware-3.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:28.407583 dankware-3.3.5/dankware/
--rw-r--r--   0 runner    (1001) docker     (123)    45628 2023-04-15 10:09:15.000000 dankware-3.3.5/dankware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:28.407583 dankware-3.3.5/dankware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-04-15 10:09:28.000000 dankware-3.3.5/dankware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 10:09:28.000000 dankware-3.3.5/dankware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:09:28.000000 dankware-3.3.5/dankware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-15 10:09:28.000000 dankware-3.3.5/dankware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 10:09:28.000000 dankware-3.3.5/dankware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 10:09:28.407583 dankware-3.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-15 10:09:15.000000 dankware-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:16:02.504831 dankware-3.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 10:15:48.000000 dankware-3.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-03 10:16:02.500831 dankware-3.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-05-03 10:15:48.000000 dankware-3.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:16:02.500831 dankware-3.3.6/dankware/
+-rw-r--r--   0 runner    (1001) docker     (123)    45681 2023-05-03 10:15:48.000000 dankware-3.3.6/dankware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:16:02.500831 dankware-3.3.6/dankware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-03 10:16:02.000000 dankware-3.3.6/dankware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 10:16:02.000000 dankware-3.3.6/dankware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:16:02.000000 dankware-3.3.6/dankware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-03 10:16:02.000000 dankware-3.3.6/dankware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 10:16:02.000000 dankware-3.3.6/dankware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 10:16:02.504831 dankware-3.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-03 10:15:48.000000 dankware-3.3.6/setup.py
```

### Comparing `dankware-3.3.5/LICENSE` & `dankware-3.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dankware-3.3.5/PKG-INFO` & `dankware-3.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.3.5
+Version: 3.3.6
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
@@ -280,15 +280,15 @@
 print(align(banner)) # also works with single text line (even coloured)
 ```
 > <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722230-1f3b6103-6d8a-4537-9828-1718a6bd3367.png">
 
 ## ♦️ Align Coloured Banner ♦️
 ```py
 from dankware import align, clr
-print(align(clr(banner,4)))
+print(clr(align(banner),4)) # OR print(align(clr(banner,4)))
 ```
 > <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722373-9925dd25-83bb-4d1c-83eb-bfaae1802088.png">
 
 <p>&nbsp;</p>    
 
 ---
```

### Comparing `dankware-3.3.5/README.md` & `dankware-3.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
 print(align(banner)) # also works with single text line (even coloured)
 ```
 > <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722230-1f3b6103-6d8a-4537-9828-1718a6bd3367.png">
 
 ## ♦️ Align Coloured Banner ♦️
 ```py
 from dankware import align, clr
-print(align(clr(banner,4)))
+print(clr(align(banner),4)) # OR print(align(clr(banner,4)))
 ```
 > <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722373-9925dd25-83bb-4d1c-83eb-bfaae1802088.png">
 
 <p>&nbsp;</p>    
 
 ---
```

### Comparing `dankware-3.3.5/dankware.egg-info/PKG-INFO` & `dankware-3.3.6/dankware.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.3.5
+Version: 3.3.6
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
@@ -280,15 +280,15 @@
 print(align(banner)) # also works with single text line (even coloured)
 ```
 > <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722230-1f3b6103-6d8a-4537-9828-1718a6bd3367.png">
 
 ## ♦️ Align Coloured Banner ♦️
 ```py
 from dankware import align, clr
-print(align(clr(banner,4)))
+print(clr(align(banner),4)) # OR print(align(clr(banner,4)))
 ```
 > <img width="800" alt="image" src="https://user-images.githubusercontent.com/52797753/153722373-9925dd25-83bb-4d1c-83eb-bfaae1802088.png">
 
 <p>&nbsp;</p>    
 
 ---
```

### Comparing `dankware-3.3.5/setup.py` & `dankware-3.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
 
     license = "MIT",
     name = "dankware",
-    version = "3.3.5",
+    version = "3.3.6",
     author = "SirDank",
     
     author_email = "SirDankenstein@protonmail.com",
     description = "Python package with various features!",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = "text/markdown",
     url = "https://github.com/SirDank/dankware",
```

