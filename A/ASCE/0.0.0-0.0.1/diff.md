# Comparing `tmp/ASCE-0.0.0.tar.gz` & `tmp/ASCE-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASCE-0.0.0.tar", last modified: Wed May  3 08:01:26 2023, max compression
+gzip compressed data, was "ASCE-0.0.1.tar", last modified: Wed May  3 07:56:04 2023, max compression
```

## Comparing `ASCE-0.0.0.tar` & `ASCE-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 08:01:26.914883 ASCE-0.0.0/
-drwxrwxrwx   0        0        0        0 2023-05-03 08:01:26.869788 ASCE-0.0.0/ASCE/
--rw-rw-rw-   0        0        0    11885 2023-05-01 18:10:04.000000 ASCE-0.0.0/ASCE/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:01:26.909361 ASCE-0.0.0/ASCE.egg-info/
--rw-rw-rw-   0        0        0      515 2023-05-03 08:01:26.000000 ASCE-0.0.0/ASCE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-05-03 08:01:26.000000 ASCE-0.0.0/ASCE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 08:01:26.000000 ASCE-0.0.0/ASCE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-03 08:01:26.000000 ASCE-0.0.0/ASCE.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 08:01:26.000000 ASCE-0.0.0/ASCE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1061 2023-05-01 18:09:54.000000 ASCE-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      515 2023-05-03 08:01:26.913886 ASCE-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      561 2023-05-01 18:09:58.000000 ASCE-0.0.0/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 08:01:26.915880 ASCE-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      670 2023-05-03 08:00:13.000000 ASCE-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:56:04.931811 ASCE-0.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-03 07:56:04.901242 ASCE-0.0.1/ASCE/
+-rw-rw-rw-   0        0        0    11885 2023-05-01 18:10:04.000000 ASCE-0.0.1/ASCE/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:56:04.927294 ASCE-0.0.1/ASCE.egg-info/
+-rw-rw-rw-   0        0        0      515 2023-05-03 07:56:04.000000 ASCE-0.0.1/ASCE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-05-03 07:56:04.000000 ASCE-0.0.1/ASCE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 07:56:04.000000 ASCE-0.0.1/ASCE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-03 07:56:04.000000 ASCE-0.0.1/ASCE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-03 07:56:04.000000 ASCE-0.0.1/ASCE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1061 2023-05-01 18:09:54.000000 ASCE-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0      515 2023-05-03 07:56:04.930498 ASCE-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      561 2023-05-01 18:09:58.000000 ASCE-0.0.1/README.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 07:56:04.932809 ASCE-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      670 2023-05-03 07:55:36.000000 ASCE-0.0.1/setup.py
```

### Comparing `ASCE-0.0.0/ASCE/__init__.py` & `ASCE-0.0.1/ASCE/__init__.py`

 * *Files identical despite different names*

### Comparing `ASCE-0.0.0/ASCE.egg-info/PKG-INFO` & `ASCE-0.0.1/ASCE.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASCE
-Version: 0.0.0
+Version: 0.0.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: CZB ASCE GROUP
 Author-email: sandrine.sila@net.usj.edu.lb
 License: MIT
 Keywords: library
 Platform: UNKNOWN
```

### Comparing `ASCE-0.0.0/LICENSE` & `ASCE-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ASCE-0.0.0/PKG-INFO` & `ASCE-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASCE
-Version: 0.0.0
+Version: 0.0.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: CZB ASCE GROUP
 Author-email: sandrine.sila@net.usj.edu.lb
 License: MIT
 Keywords: library
 Platform: UNKNOWN
```

### Comparing `ASCE-0.0.0/README.txt` & `ASCE-0.0.1/README.txt`

 * *Files identical despite different names*

### Comparing `ASCE-0.0.0/setup.py` & `ASCE-0.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='ASCE',
-  VERSION='0.0.1',
+  version='0.0.1',
 #   description='A fast library/similar to numpy',
 #   long_description=open('README.txt').read()
   url='',  
   author='CZB ASCE GROUP',
   author_email='sandrine.sila@net.usj.edu.lb',
   license='MIT', 
   classifiers=classifiers,
```

