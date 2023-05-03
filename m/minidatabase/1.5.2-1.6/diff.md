# Comparing `tmp/minidatabase-1.5.2.tar.gz` & `tmp/minidatabase-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidatabase-1.5.2.tar", last modified: Tue May  2 10:03:13 2023, max compression
+gzip compressed data, was "minidatabase-1.6.tar", last modified: Tue May  2 10:15:39 2023, max compression
```

## Comparing `minidatabase-1.5.2.tar` & `minidatabase-1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 10:03:13.616055 minidatabase-1.5.2/
--rw-rw-rw-   0        0        0    35796 2023-05-01 10:46:49.000000 minidatabase-1.5.2/LICENSE.txt
--rw-rw-rw-   0        0        0     4477 2023-05-02 10:03:13.615061 minidatabase-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     3620 2023-05-02 09:58:09.000000 minidatabase-1.5.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 10:03:13.601865 minidatabase-1.5.2/minidatabase/
--rw-rw-rw-   0        0        0     1623 2023-05-02 09:56:27.000000 minidatabase-1.5.2/minidatabase/WebMDB.py
--rw-rw-rw-   0        0        0       65 2023-05-02 04:28:10.000000 minidatabase-1.5.2/minidatabase/__init__.py
--rw-rw-rw-   0        0        0     9446 2023-05-02 09:56:02.000000 minidatabase-1.5.2/minidatabase/minidb.py
-drwxrwxrwx   0        0        0        0 2023-05-02 10:03:13.613063 minidatabase-1.5.2/minidatabase.egg-info/
--rw-rw-rw-   0        0        0     4477 2023-05-02 10:03:13.000000 minidatabase-1.5.2/minidatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-05-02 10:03:13.000000 minidatabase-1.5.2/minidatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 10:03:13.000000 minidatabase-1.5.2/minidatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-02 10:03:13.000000 minidatabase-1.5.2/minidatabase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-02 10:03:13.000000 minidatabase-1.5.2/minidatabase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 10:03:13.000000 minidatabase-1.5.2/minidatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 10:03:13.616055 minidatabase-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1234 2023-05-02 10:02:00.000000 minidatabase-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:15:39.285803 minidatabase-1.6/
+-rw-rw-rw-   0        0        0    35796 2023-05-01 10:46:49.000000 minidatabase-1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     3824 2023-05-02 10:15:39.284803 minidatabase-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2929 2023-05-02 10:12:16.000000 minidatabase-1.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 10:15:39.268562 minidatabase-1.6/minidatabase/
+-rw-rw-rw-   0        0        0     1623 2023-05-02 09:56:27.000000 minidatabase-1.6/minidatabase/WebMDB.py
+-rw-rw-rw-   0        0        0       65 2023-05-02 04:28:10.000000 minidatabase-1.6/minidatabase/__init__.py
+-rw-rw-rw-   0        0        0     9446 2023-05-02 09:56:02.000000 minidatabase-1.6/minidatabase/minidb.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:15:39.282136 minidatabase-1.6/minidatabase.egg-info/
+-rw-rw-rw-   0        0        0     3824 2023-05-02 10:15:39.000000 minidatabase-1.6/minidatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-05-02 10:15:39.000000 minidatabase-1.6/minidatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 10:15:39.000000 minidatabase-1.6/minidatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-02 10:15:39.000000 minidatabase-1.6/minidatabase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-05-02 10:15:39.000000 minidatabase-1.6/minidatabase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 10:15:39.000000 minidatabase-1.6/minidatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 10:15:39.285803 minidatabase-1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-05-02 10:15:29.000000 minidatabase-1.6/setup.py
```

### Comparing `minidatabase-1.5.2/LICENSE.txt` & `minidatabase-1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `minidatabase-1.5.2/minidatabase/WebMDB.py` & `minidatabase-1.6/minidatabase/WebMDB.py`

 * *Files identical despite different names*

### Comparing `minidatabase-1.5.2/minidatabase/minidb.py` & `minidatabase-1.6/minidatabase/minidb.py`

 * *Files identical despite different names*

### Comparing `minidatabase-1.5.2/setup.py` & `minidatabase-1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.rst", "r",encoding='gb18030',errors='ignore') as f:
   long_description = f.read()
 setup(name='minidatabase',  
-      version='1.5.2',  
+      version='1.6',  
       description='A tiny database system based on  python dictionary.',
       long_description=long_description,
       author='HansenL',
       author_email='hansenl@foxmail.com',
       url='http://osdn.xyz',
       install_requires=["requests","flask"],
       license=' GNU GENERAL PUBLIC LICENSE',
```

