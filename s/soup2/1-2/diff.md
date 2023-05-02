# Comparing `tmp/soup2-1.tar.gz` & `tmp/soup2-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soup2-1.tar", last modified: Tue May  2 22:36:12 2023, max compression
+gzip compressed data, was "soup2-2.tar", last modified: Tue May  2 22:50:30 2023, max compression
```

## Comparing `soup2-1.tar` & `soup2-2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 22:36:12.122594 soup2-1/
--rw-rw-rw-   0        0        0    14720 2023-05-02 22:36:12.123585 soup2-1/PKG-INFO
--rw-rw-rw-   0        0        0    13715 2023-03-04 16:03:05.000000 soup2-1/README.md
--rw-rw-rw-   0        0        0       43 2023-05-02 22:36:12.128601 soup2-1/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-05-02 22:35:46.000000 soup2-1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 22:36:12.094596 soup2-1/soup2/
--rw-rw-rw-   0        0        0       61 2023-05-02 22:31:08.000000 soup2-1/soup2/__init__.py
--rw-rw-rw-   0        0        0    11735 2023-05-02 22:30:26.000000 soup2-1/soup2/src_file.py
-drwxrwxrwx   0        0        0        0 2023-05-02 22:36:12.120585 soup2-1/soup2.egg-info/
--rw-rw-rw-   0        0        0    14720 2023-05-02 22:36:12.000000 soup2-1/soup2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-05-02 22:36:12.000000 soup2-1/soup2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 22:36:12.000000 soup2-1/soup2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-02 22:36:12.000000 soup2-1/soup2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 22:36:12.000000 soup2-1/soup2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 22:50:30.219613 soup2-2/
+-rw-rw-rw-   0        0        0    14720 2023-05-02 22:50:30.219613 soup2-2/PKG-INFO
+-rw-rw-rw-   0        0        0    13715 2023-03-04 16:03:05.000000 soup2-2/README.md
+-rw-rw-rw-   0        0        0       43 2023-05-02 22:50:30.222613 soup2-2/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-05-02 22:48:35.000000 soup2-2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 22:50:30.194430 soup2-2/soup2/
+-rw-rw-rw-   0        0        0       61 2023-05-02 22:31:08.000000 soup2-2/soup2/__init__.py
+-rw-rw-rw-   0        0        0   351092 2023-05-02 22:48:28.000000 soup2-2/soup2/src_file.py
+drwxrwxrwx   0        0        0        0 2023-05-02 22:50:30.217614 soup2-2/soup2.egg-info/
+-rw-rw-rw-   0        0        0    14720 2023-05-02 22:50:30.000000 soup2-2/soup2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-05-02 22:50:30.000000 soup2-2/soup2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 22:50:30.000000 soup2-2/soup2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-02 22:50:30.000000 soup2-2/soup2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 22:50:30.000000 soup2-2/soup2.egg-info/top_level.txt
```

### Comparing `soup2-1/PKG-INFO` & `soup2-2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soup2
-Version: 1
+Version: 2
 Summary: Pure-python Colors implementation
 Home-page: https://github.com/tartley/colorama
 Author: Jonathan Hartley
 Author-email: tartley@tartley.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `soup2-1/README.md` & `soup2-2/README.md`

 * *Files identical despite different names*

### Comparing `soup2-1/setup.py` & `soup2-2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='soup2',
-    version='1',
+    version='2',
     author='Jonathan Hartley',
     author_email='tartley@tartley.com',
     description='Pure-python Colors implementation',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/tartley/colorama',
     packages=find_packages(),
```

### Comparing `soup2-1/soup2.egg-info/PKG-INFO` & `soup2-2/soup2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soup2
-Version: 1
+Version: 2
 Summary: Pure-python Colors implementation
 Home-page: https://github.com/tartley/colorama
 Author: Jonathan Hartley
 Author-email: tartley@tartley.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

