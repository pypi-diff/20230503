# Comparing `tmp/alia-0.2.1.tar.gz` & `tmp/alia-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alia-0.2.1.tar", last modified: Thu Apr 20 19:42:17 2023, max compression
+gzip compressed data, was "alia-0.2.2.tar", last modified: Wed May  3 20:24:44 2023, max compression
```

## Comparing `alia-0.2.1.tar` & `alia-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-20 19:42:17.218699 alia-0.2.1/
--rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.2.1/LICENSE
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-20 19:42:17.218332 alia-0.2.1/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 19:00:09.000000 alia-0.2.1/README.md
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-20 19:42:17.214609 alia-0.2.1/alia/
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.2.1/alia/__init__.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    17437 2023-04-19 20:09:36.000000 alia-0.2.1/alia/colors.py
--rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.2.1/alia/df_tools.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    27520 2023-04-19 20:13:35.000000 alia-0.2.1/alia/tools.py
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-20 19:42:17.217693 alia-0.2.1/alia.egg-info/
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-20 19:42:17.000000 alia-0.2.1/alia.egg-info/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-04-20 19:42:17.000000 alia-0.2.1/alia.egg-info/SOURCES.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-04-20 19:42:17.000000 alia-0.2.1/alia.egg-info/dependency_links.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       94 2023-04-20 19:42:17.000000 alia-0.2.1/alia.egg-info/requires.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-04-20 19:42:17.000000 alia-0.2.1/alia.egg-info/top_level.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-04-20 19:42:17.218804 alia-0.2.1/setup.cfg
--rw-r--r--   0 aliavictor   (502) staff       (20)      926 2023-04-20 19:40:04.000000 alia-0.2.1/setup.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-05-03 20:24:44.740173 alia-0.2.2/
+-rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.2.2/LICENSE
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-05-03 20:24:44.739861 alia-0.2.2/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      529 2023-04-20 21:02:49.000000 alia-0.2.2/README.md
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-05-03 20:24:44.737644 alia-0.2.2/alia/
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.2.2/alia/__init__.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    17437 2023-04-19 20:09:36.000000 alia-0.2.2/alia/colors.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.2.2/alia/df_tools.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    28152 2023-05-03 20:23:20.000000 alia-0.2.2/alia/tools.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-05-03 20:24:44.739486 alia-0.2.2/alia.egg-info/
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-05-03 20:24:44.000000 alia-0.2.2/alia.egg-info/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-05-03 20:24:44.000000 alia-0.2.2/alia.egg-info/SOURCES.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-05-03 20:24:44.000000 alia-0.2.2/alia.egg-info/dependency_links.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       94 2023-05-03 20:24:44.000000 alia-0.2.2/alia.egg-info/requires.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-05-03 20:24:44.000000 alia-0.2.2/alia.egg-info/top_level.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-05-03 20:24:44.740274 alia-0.2.2/setup.cfg
+-rw-r--r--   0 aliavictor   (502) staff       (20)      926 2023-05-03 20:24:01.000000 alia-0.2.2/setup.py
```

### Comparing `alia-0.2.1/LICENSE` & `alia-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alia-0.2.1/PKG-INFO` & `alia-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.2.1/alia/colors.py` & `alia-0.2.2/alia/colors.py`

 * *Files identical despite different names*

### Comparing `alia-0.2.1/alia/df_tools.py` & `alia-0.2.2/alia/df_tools.py`

 * *Files identical despite different names*

### Comparing `alia-0.2.1/alia/tools.py` & `alia-0.2.2/alia/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import calendar
 import csv
 import difflib
 import os
 import pickle
-from datetime import datetime, date, timedelta
+from datetime import date, timedelta
 
 import pandas as pd
 import pyperclip
 from cryptography.fernet import Fernet
 from dateutil.parser import parse
 
 from .colors import *
@@ -546,23 +546,26 @@
     Args:
         string (str, re.compile): String or compiled re object to reference
         pattern (str): Regex pattern to search the string with
         ignore_case (bool): Whether or not to use re.IGNORECASE
 
     Returns:
         A string of the output of the passed regex."""
-    if isinstance(pattern, str):
-        if ignore_case:
-            return re.search(pattern, string, re.IGNORECASE).group(1)
-        else:
-            return re.search(pattern, string).group(1)
-    elif ignore_case:
-        return pattern.search(string, re.IGNORECASE).group(1)
-    else:
-        return pattern.search(string).group(1)
+    try:
+        if isinstance(pattern, str):
+            if ignore_case:
+                return re.search(pattern, string, re.IGNORECASE).group(1)
+            else:
+                return re.search(pattern, string).group(1)
+        elif ignore_case:
+            return pattern.search(string, re.IGNORECASE).group(1)
+        else:
+            return pattern.search(string).group(1)
+    except AttributeError:
+        print("Nothing matches the given regex pattern in the given string")
 
 
 def str_dedupe(txt):
     """Removes duplicate substrings from a string.
 
     Args:
         txt (str): String to dedupe
@@ -831,14 +834,28 @@
             num (int): The number of items each chunk should contain
 
         Returns:
             A list of lists where each list contains the passed number of items from the given list."""
     return [input_list[i: i + num] for i in range(0, len(input_list), num)]
 
 
+def split_data(data, ratio):
+    """Splits data into two chunks based on a given ratio.
+
+        Args:
+            data (list): The data to be split
+            ratio (float): The ratio at which to split the data. Should be between 0 and 1
+
+        Returns:
+            A tuple of 2 lists, the first containing the first 'ratio' proportion of the data,
+            the second containing the rest."""
+    split_index = int(len(data) * ratio)
+    return data[:split_index], data[split_index:]
+
+
 def ordinal(n):
     """Converts a number into its ordinal representation (e.g. 1st, 2nd, etc).
 
     Args:
         n (int, str): The string or integer to convert
 
     Returns:
```

### Comparing `alia-0.2.1/alia.egg-info/PKG-INFO` & `alia-0.2.2/alia.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.2.1/setup.py` & `alia-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="alia",
-    version="0.2.1",
+    version="0.2.2",
     description="A collection of random helper tools to make life easier",
     author="Alia",
     author_email="alia.jo.victor@gmail.com",
     url="https://github.com/aliavictor/alia",
     packages=find_packages(),
     install_requires=[
         # i.e. 'numpy>=1.18.0'
```

