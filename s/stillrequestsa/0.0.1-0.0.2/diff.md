# Comparing `tmp/stillrequestsa-0.0.1.tar.gz` & `tmp/stillrequestsa-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stillrequestsa-0.0.1.tar", last modified: Tue May  2 22:47:48 2023, max compression
+gzip compressed data, was "stillrequestsa-0.0.2.tar", last modified: Wed May  3 03:46:17 2023, max compression
```

## Comparing `stillrequestsa-0.0.1.tar` & `stillrequestsa-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 22:47:48.464702 stillrequestsa-0.0.1/
--rw-rw-rw-   0        0        0      536 2023-05-02 22:47:48.464702 stillrequestsa-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-05-02 22:46:35.458732 stillrequestsa-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 22:47:48.464702 stillrequestsa-0.0.1/stillrequestsa/
--rw-rw-rw-   0        0        0     1052 2023-05-02 22:47:27.240282 stillrequestsa-0.0.1/stillrequestsa/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:46:17.409797 stillrequestsa-0.0.2/
+-rw-rw-rw-   0        0        0      536 2023-05-03 03:46:17.409797 stillrequestsa-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-05-03 03:46:15.843327 stillrequestsa-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:46:17.409797 stillrequestsa-0.0.2/stillrequestsa/
+-rw-rw-rw-   0        0        0     1100 2023-05-03 03:46:00.151730 stillrequestsa-0.0.2/stillrequestsa/__init__.py
```

### Comparing `stillrequestsa-0.0.1/PKG-INFO` & `stillrequestsa-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: stillrequestsa
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: WS
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `stillrequestsa-0.0.1/setup.py` & `stillrequestsa-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
   name = 'stillrequestsa',
   packages = ['stillrequestsa'],
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = '',
   author = 'WS',
   keywords = [],
   install_requires=['requests', 'tryquests'],
   classifiers=[
     'Operating System :: OS Independent',
```

