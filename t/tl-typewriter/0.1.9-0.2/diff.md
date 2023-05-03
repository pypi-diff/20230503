# Comparing `tmp/tl_typewriter-0.1.9.tar.gz` & `tmp/tl_typewriter-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tl_typewriter-0.1.9.tar", last modified: Sun Apr 16 11:31:12 2023, max compression
+gzip compressed data, was "tl_typewriter-0.2.tar", last modified: Wed May  3 07:02:49 2023, max compression
```

## Comparing `tl_typewriter-0.1.9.tar` & `tl_typewriter-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 11:31:12.138488 tl_typewriter-0.1.9/
--rw-rw-rw-   0        0        0    11558 2023-04-16 06:54:47.000000 tl_typewriter-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      302 2023-04-16 11:31:12.138488 tl_typewriter-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      594 2023-04-16 09:41:19.000000 tl_typewriter-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 11:31:12.139513 tl_typewriter-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      659 2023-04-16 11:23:50.000000 tl_typewriter-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 11:31:12.133018 tl_typewriter-0.1.9/tl_typewriter.egg-info/
--rw-rw-rw-   0        0        0      302 2023-04-16 11:31:12.000000 tl_typewriter-0.1.9/tl_typewriter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-04-16 11:31:12.000000 tl_typewriter-0.1.9/tl_typewriter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 11:31:12.000000 tl_typewriter-0.1.9/tl_typewriter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-16 11:31:12.000000 tl_typewriter-0.1.9/tl_typewriter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-04-16 11:31:12.000000 tl_typewriter-0.1.9/tl_typewriter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-16 11:31:12.000000 tl_typewriter-0.1.9/tl_typewriter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 11:31:12.136467 tl_typewriter-0.1.9/typewriter/
--rw-rw-rw-   0        0        0      127 2023-04-16 11:21:18.000000 tl_typewriter-0.1.9/typewriter/__main__.py
--rw-rw-rw-   0        0        0     1763 2023-04-16 11:21:09.000000 tl_typewriter-0.1.9/typewriter/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:02:49.764046 tl_typewriter-0.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-16 06:54:47.000000 tl_typewriter-0.2/LICENSE
+-rw-rw-rw-   0        0        0      300 2023-05-03 07:02:49.764046 tl_typewriter-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2023-04-16 09:41:19.000000 tl_typewriter-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 07:02:49.765058 tl_typewriter-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      657 2023-05-03 07:02:06.000000 tl_typewriter-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:02:49.757360 tl_typewriter-0.2/tl_typewriter.egg-info/
+-rw-rw-rw-   0        0        0      300 2023-05-03 07:02:49.000000 tl_typewriter-0.2/tl_typewriter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-03 07:02:49.000000 tl_typewriter-0.2/tl_typewriter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 07:02:49.000000 tl_typewriter-0.2/tl_typewriter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-03 07:02:49.000000 tl_typewriter-0.2/tl_typewriter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-05-03 07:02:49.000000 tl_typewriter-0.2/tl_typewriter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 07:02:49.000000 tl_typewriter-0.2/tl_typewriter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 07:02:49.762033 tl_typewriter-0.2/typewriter/
+-rw-rw-rw-   0        0        0      127 2023-04-16 11:21:18.000000 tl_typewriter-0.2/typewriter/__main__.py
+-rw-rw-rw-   0        0        0     1770 2023-05-03 06:58:24.000000 tl_typewriter-0.2/typewriter/writer.py
```

### Comparing `tl_typewriter-0.1.9/LICENSE` & `tl_typewriter-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tl_typewriter-0.1.9/README.md` & `tl_typewriter-0.2/README.md`

 * *Files identical despite different names*

### Comparing `tl_typewriter-0.1.9/setup.py` & `tl_typewriter-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from setuptools import setup
 
 
 setup(
     name="tl_typewriter",
-    version='0.1.9',
+    version='0.2',
     description="pagination and bubble typewriter in translating manga",
     url="https://github.com/AbangTanYiHan/tl_typewriter",
     author="abangtan",
     license="Apache License 2.0",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
```

### Comparing `tl_typewriter-0.1.9/typewriter/writer.py` & `tl_typewriter-0.2/typewriter/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,11 +43,11 @@
     elif event.name == 'space':
         picture += 1
         box = bubble = text = 0
     elif event.name == 'z':
         page += 1
         box = bubble = text = 0
         picture = 1
-        result = "Page " + str(page) + "\n"
+        result = "\n" + "Page " + str(page) + "\n"
     else:
         result = ""
     return result, page, picture, bubble, text, box
```

