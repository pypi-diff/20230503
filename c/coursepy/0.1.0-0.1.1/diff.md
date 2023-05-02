# Comparing `tmp/coursepy-0.1.0-py3-none-any.whl.zip` & `tmp/coursepy-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 4429 bytes, number of entries: 6
--rw-r--r--  2.0 unx        0 b- defN 23-May-01 00:26 coursepy/__init__.py
--rw-r--r--  2.0 unx    11087 b- defN 23-May-02 21:50 coursepy/all_functions.py
--rw-r--r--  2.0 unx      808 b- defN 23-May-02 21:57 coursepy-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 21:57 coursepy-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-02 21:57 coursepy-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      457 b- defN 23-May-02 21:57 coursepy-0.1.0.dist-info/RECORD
-6 files, 12453 bytes uncompressed, 3597 bytes compressed:  71.1%
+Zip file size: 5302 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       55 b- defN 23-May-02 22:26 coursepy/__init__.py
+-rw-r--r--  2.0 unx    10958 b- defN 23-May-02 22:05 coursepy/all_functions.py
+-rw-r--r--  2.0 unx     1122 b- defN 23-May-02 22:27 coursepy-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      834 b- defN 23-May-02 22:27 coursepy-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 22:27 coursepy-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-02 22:27 coursepy-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      551 b- defN 23-May-02 22:27 coursepy-0.1.1.dist-info/RECORD
+7 files, 13621 bytes uncompressed, 4322 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: coursepy/__init__.py
 Comment: 
 
 Filename: coursepy/all_functions.py
 Comment: 
 
-Filename: coursepy-0.1.0.dist-info/METADATA
+Filename: coursepy-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: coursepy-0.1.0.dist-info/WHEEL
+Filename: coursepy-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: coursepy-0.1.0.dist-info/top_level.txt
+Filename: coursepy-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: coursepy-0.1.0.dist-info/RECORD
+Filename: coursepy-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: coursepy-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## coursepy/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 6672 6f6d 2061 6c6c 5f66 756e 6374 696f  from all_functio
+00000010: 6e73 2069 6d70 6f72 7420 7370 6565 645f  ns import speed_
+00000020: 7363 6865 6475 6c65 2c20 636f 7374 5f76  schedule, cost_v
+00000030: 5f63 7265 6469 74                        _credit
```

## coursepy/all_functions.py

```diff
@@ -1,16 +1,13 @@
 # from collections import deque
 import json
 from pulp import *
 import sys, os
 
-oneUpPath = os.path.abspath('../')
-file = os.path.join(oneUpPath, 'send_in.txt')
-# file='send_in.txt'
-sys.stdin = open(file, 'r')
+
 
 
 class Graph:
 
     def __init__(self):
         """
         A directed graph class made with an adjacency dictionary where the key-value pairs uses the following format
```

## Comparing `coursepy-0.1.0.dist-info/METADATA` & `coursepy-0.1.1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: coursepy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A course organizer that lets students map their college courses
 Home-page: https://github.com/Le-Pro/CSCI354_Project_Group3
 Author: Hrishav Sapkota, Sameer Acharya, Victor Iyke-Osuji
 Author-email: hrishav.sapkota@bison.howard.edu, sameer.acharya@bison.howard.edu, victor.iykeosuji@bison.howard.edu
 License: MIT
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 # Coursepy
 A package that lets students map their college courses.
 
 ## How to use
 _Install the package by using this in the command-line:_ <br>
 ```sh
```

