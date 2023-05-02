# Comparing `tmp/coursepy-1.0.0-py3-none-any.whl.zip` & `tmp/coursepy-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5325 bytes, number of entries: 7
+Zip file size: 5314 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      102 b- defN 23-May-02 22:43 coursepy/__init__.py
--rw-r--r--  2.0 unx    10958 b- defN 23-May-02 22:05 coursepy/all_functions.py
--rw-r--r--  2.0 unx     1122 b- defN 23-May-02 22:44 coursepy-1.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      834 b- defN 23-May-02 22:44 coursepy-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 22:44 coursepy-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-02 22:44 coursepy-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      552 b- defN 23-May-02 22:44 coursepy-1.0.0.dist-info/RECORD
-7 files, 13669 bytes uncompressed, 4345 bytes compressed:  68.2%
+-rw-r--r--  2.0 unx    10939 b- defN 23-May-02 22:45 coursepy/all_functions.py
+-rw-r--r--  2.0 unx     1122 b- defN 23-May-02 22:49 coursepy-1.0.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      834 b- defN 23-May-02 22:49 coursepy-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 22:49 coursepy-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-02 22:49 coursepy-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      552 b- defN 23-May-02 22:49 coursepy-1.0.1.dist-info/RECORD
+7 files, 13650 bytes uncompressed, 4334 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: coursepy/__init__.py
 Comment: 
 
 Filename: coursepy/all_functions.py
 Comment: 
 
-Filename: coursepy-1.0.0.dist-info/LICENSE.txt
+Filename: coursepy-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: coursepy-1.0.0.dist-info/METADATA
+Filename: coursepy-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: coursepy-1.0.0.dist-info/WHEEL
+Filename: coursepy-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: coursepy-1.0.0.dist-info/top_level.txt
+Filename: coursepy-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: coursepy-1.0.0.dist-info/RECORD
+Filename: coursepy-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## coursepy/all_functions.py

```diff
@@ -1,10 +1,9 @@
 # from collections import deque
 import json
-from pulp import *
 import sys, os
 
 
 
 
 class Graph:
```

## Comparing `coursepy-1.0.0.dist-info/LICENSE.txt` & `coursepy-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `coursepy-1.0.0.dist-info/METADATA` & `coursepy-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coursepy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A course organizer that lets students map their college courses
 Home-page: https://github.com/Le-Pro/CSCI354_Project_Group3
 Author: Hrishav Sapkota, Sameer Acharya, Victor Iyke-Osuji
 Author-email: hrishav.sapkota@bison.howard.edu, sameer.acharya@bison.howard.edu, victor.iykeosuji@bison.howard.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

