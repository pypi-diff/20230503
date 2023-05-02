# Comparing `tmp/coursepy-0.1.2-py3-none-any.whl.zip` & `tmp/coursepy-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5304 bytes, number of entries: 7
--rw-r--r--  2.0 unx       55 b- defN 23-May-02 22:26 coursepy/__init__.py
+Zip file size: 5325 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      102 b- defN 23-May-02 22:43 coursepy/__init__.py
 -rw-r--r--  2.0 unx    10958 b- defN 23-May-02 22:05 coursepy/all_functions.py
--rw-r--r--  2.0 unx     1122 b- defN 23-May-02 22:36 coursepy-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      834 b- defN 23-May-02 22:36 coursepy-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 22:36 coursepy-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-02 22:36 coursepy-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      551 b- defN 23-May-02 22:36 coursepy-0.1.2.dist-info/RECORD
-7 files, 13621 bytes uncompressed, 4324 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx     1122 b- defN 23-May-02 22:44 coursepy-1.0.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      834 b- defN 23-May-02 22:44 coursepy-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 22:44 coursepy-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-02 22:44 coursepy-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      552 b- defN 23-May-02 22:44 coursepy-1.0.0.dist-info/RECORD
+7 files, 13669 bytes uncompressed, 4345 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: coursepy/__init__.py
 Comment: 
 
 Filename: coursepy/all_functions.py
 Comment: 
 
-Filename: coursepy-0.1.2.dist-info/LICENSE.txt
+Filename: coursepy-1.0.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: coursepy-0.1.2.dist-info/METADATA
+Filename: coursepy-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: coursepy-0.1.2.dist-info/WHEEL
+Filename: coursepy-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: coursepy-0.1.2.dist-info/top_level.txt
+Filename: coursepy-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: coursepy-0.1.2.dist-info/RECORD
+Filename: coursepy-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## coursepy/__init__.py

```diff
@@ -1 +1,2 @@
-from all_functions import speed_schedule, cost_v_credit
+from .all_functions import speed_schedule, cost_v_credit
+__all__ = ['speed_schedule', 'cost_v_credit']
```

## Comparing `coursepy-0.1.2.dist-info/LICENSE.txt` & `coursepy-1.0.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `coursepy-0.1.2.dist-info/METADATA` & `coursepy-1.0.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coursepy
-Version: 0.1.2
+Version: 1.0.0
 Summary: A course organizer that lets students map their college courses
 Home-page: https://github.com/Le-Pro/CSCI354_Project_Group3
 Author: Hrishav Sapkota, Sameer Acharya, Victor Iyke-Osuji
 Author-email: hrishav.sapkota@bison.howard.edu, sameer.acharya@bison.howard.edu, victor.iykeosuji@bison.howard.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

