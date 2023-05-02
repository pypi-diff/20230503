# Comparing `tmp/coursepy-0.1.1-py3-none-any.whl.zip` & `tmp/coursepy-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5302 bytes, number of entries: 7
+Zip file size: 5304 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       55 b- defN 23-May-02 22:26 coursepy/__init__.py
 -rw-r--r--  2.0 unx    10958 b- defN 23-May-02 22:05 coursepy/all_functions.py
--rw-r--r--  2.0 unx     1122 b- defN 23-May-02 22:27 coursepy-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      834 b- defN 23-May-02 22:27 coursepy-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 22:27 coursepy-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-02 22:27 coursepy-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      551 b- defN 23-May-02 22:27 coursepy-0.1.1.dist-info/RECORD
-7 files, 13621 bytes uncompressed, 4322 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx     1122 b- defN 23-May-02 22:36 coursepy-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      834 b- defN 23-May-02 22:36 coursepy-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 22:36 coursepy-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-02 22:36 coursepy-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      551 b- defN 23-May-02 22:36 coursepy-0.1.2.dist-info/RECORD
+7 files, 13621 bytes uncompressed, 4324 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: coursepy/__init__.py
 Comment: 
 
 Filename: coursepy/all_functions.py
 Comment: 
 
-Filename: coursepy-0.1.1.dist-info/LICENSE.txt
+Filename: coursepy-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: coursepy-0.1.1.dist-info/METADATA
+Filename: coursepy-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: coursepy-0.1.1.dist-info/WHEEL
+Filename: coursepy-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: coursepy-0.1.1.dist-info/top_level.txt
+Filename: coursepy-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: coursepy-0.1.1.dist-info/RECORD
+Filename: coursepy-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `coursepy-0.1.1.dist-info/LICENSE.txt` & `coursepy-0.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `coursepy-0.1.1.dist-info/METADATA` & `coursepy-0.1.2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coursepy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A course organizer that lets students map their college courses
 Home-page: https://github.com/Le-Pro/CSCI354_Project_Group3
 Author: Hrishav Sapkota, Sameer Acharya, Victor Iyke-Osuji
 Author-email: hrishav.sapkota@bison.howard.edu, sameer.acharya@bison.howard.edu, victor.iykeosuji@bison.howard.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

## Comparing `coursepy-0.1.1.dist-info/RECORD` & `coursepy-0.1.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 coursepy/__init__.py,sha256=aWGK7Y9Lby0rfqo5iJZpwq-voLUh_aCOoV2DXLx7kuQ,55
 coursepy/all_functions.py,sha256=rIWcO5XKIgbpmtl8Fh78g3PbXKk-iRE_k8RMPicbwZE,10958
-coursepy-0.1.1.dist-info/LICENSE.txt,sha256=vqQAQni0yZZcerVvw6hXCPjEH43xTgFjHSsnkCYW8L0,1122
-coursepy-0.1.1.dist-info/METADATA,sha256=r3ppedOJFP0artY-O_YyWhY1_XvQGLcT01hYs4wxyPE,834
-coursepy-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-coursepy-0.1.1.dist-info/top_level.txt,sha256=Gs2UaweuMStgQvf2clESKk62ZIyts7X1nK6vYagGlCc,9
-coursepy-0.1.1.dist-info/RECORD,,
+coursepy-0.1.2.dist-info/LICENSE.txt,sha256=vqQAQni0yZZcerVvw6hXCPjEH43xTgFjHSsnkCYW8L0,1122
+coursepy-0.1.2.dist-info/METADATA,sha256=lwbGYmZbV2MxK2BJESfqYJhpmWTQGuH258XT4gjUrMg,834
+coursepy-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+coursepy-0.1.2.dist-info/top_level.txt,sha256=Gs2UaweuMStgQvf2clESKk62ZIyts7X1nK6vYagGlCc,9
+coursepy-0.1.2.dist-info/RECORD,,
```

