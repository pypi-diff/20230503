# Comparing `tmp/mypackage_prince_boom-0.0.4.tar.gz` & `tmp/mypackage_prince_boom-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackage_prince_boom-0.0.4.tar", last modified: Thu Apr 27 13:10:05 2023, max compression
+gzip compressed data, was "mypackage_prince_boom-0.0.5.tar", last modified: Wed May  3 12:47:00 2023, max compression
```

## Comparing `mypackage_prince_boom-0.0.4.tar` & `mypackage_prince_boom-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 studio45  (1000) studio45  (1000)        0 2023-04-27 13:10:05.599801 mypackage_prince_boom-0.0.4/
--rw-rw-r--   0 studio45  (1000) studio45  (1000)     1073 2023-04-26 11:26:19.000000 mypackage_prince_boom-0.0.4/LICENSE
--rw-rw-r--   0 studio45  (1000) studio45  (1000)      451 2023-04-27 13:10:05.599801 mypackage_prince_boom-0.0.4/PKG-INFO
--rw-rw-r--   0 studio45  (1000) studio45  (1000)      170 2023-04-27 11:23:57.000000 mypackage_prince_boom-0.0.4/README.md
-drwxrwxr-x   0 studio45  (1000) studio45  (1000)        0 2023-04-27 13:10:05.595801 mypackage_prince_boom-0.0.4/mypackage_prince_boom/
--rw-rw-r--   0 studio45  (1000) studio45  (1000)     8720 2023-04-27 13:08:53.000000 mypackage_prince_boom-0.0.4/mypackage_prince_boom/__init__.py
--rw-rw-r--   0 studio45  (1000) studio45  (1000)      118 2023-04-27 13:08:06.000000 mypackage_prince_boom-0.0.4/mypackage_prince_boom/signals.py
-drwxrwxr-x   0 studio45  (1000) studio45  (1000)        0 2023-04-27 13:10:05.599801 mypackage_prince_boom-0.0.4/mypackage_prince_boom.egg-info/
--rw-rw-r--   0 studio45  (1000) studio45  (1000)      451 2023-04-27 13:10:05.000000 mypackage_prince_boom-0.0.4/mypackage_prince_boom.egg-info/PKG-INFO
--rw-rw-r--   0 studio45  (1000) studio45  (1000)      365 2023-04-27 13:10:05.000000 mypackage_prince_boom-0.0.4/mypackage_prince_boom.egg-info/SOURCES.txt
--rw-rw-r--   0 studio45  (1000) studio45  (1000)        1 2023-04-27 13:10:05.000000 mypackage_prince_boom-0.0.4/mypackage_prince_boom.egg-info/dependency_links.txt
--rw-rw-r--   0 studio45  (1000) studio45  (1000)       79 2023-04-27 13:10:05.000000 mypackage_prince_boom-0.0.4/mypackage_prince_boom.egg-info/entry_points.txt
--rw-rw-r--   0 studio45  (1000) studio45  (1000)        9 2023-04-27 13:10:05.000000 mypackage_prince_boom-0.0.4/mypackage_prince_boom.egg-info/requires.txt
--rw-rw-r--   0 studio45  (1000) studio45  (1000)       22 2023-04-27 13:10:05.000000 mypackage_prince_boom-0.0.4/mypackage_prince_boom.egg-info/top_level.txt
--rw-rw-r--   0 studio45  (1000) studio45  (1000)       38 2023-04-27 13:10:05.599801 mypackage_prince_boom-0.0.4/setup.cfg
--rw-rw-r--   0 studio45  (1000) studio45  (1000)      686 2023-04-27 13:09:09.000000 mypackage_prince_boom-0.0.4/setup.py
+drwxrwxr-x   0 studio45  (1000) studio45  (1000)        0 2023-05-03 12:47:00.599974 mypackage_prince_boom-0.0.5/
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)     1073 2023-04-26 11:26:19.000000 mypackage_prince_boom-0.0.5/LICENSE
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)      451 2023-05-03 12:47:00.599974 mypackage_prince_boom-0.0.5/PKG-INFO
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)      170 2023-04-27 11:23:57.000000 mypackage_prince_boom-0.0.5/README.md
+drwxrwxr-x   0 studio45  (1000) studio45  (1000)        0 2023-05-03 12:47:00.595974 mypackage_prince_boom-0.0.5/mypackage_prince_boom/
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)      117 2023-05-03 12:36:36.000000 mypackage_prince_boom-0.0.5/mypackage_prince_boom/__init__.py
+drwxrwxr-x   0 studio45  (1000) studio45  (1000)        0 2023-05-03 12:47:00.599974 mypackage_prince_boom-0.0.5/mypackage_prince_boom.egg-info/
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)      451 2023-05-03 12:47:00.000000 mypackage_prince_boom-0.0.5/mypackage_prince_boom.egg-info/PKG-INFO
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)      332 2023-05-03 12:47:00.000000 mypackage_prince_boom-0.0.5/mypackage_prince_boom.egg-info/SOURCES.txt
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)        1 2023-05-03 12:47:00.000000 mypackage_prince_boom-0.0.5/mypackage_prince_boom.egg-info/dependency_links.txt
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)       79 2023-05-03 12:47:00.000000 mypackage_prince_boom-0.0.5/mypackage_prince_boom.egg-info/entry_points.txt
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)        9 2023-05-03 12:47:00.000000 mypackage_prince_boom-0.0.5/mypackage_prince_boom.egg-info/requires.txt
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)       22 2023-05-03 12:47:00.000000 mypackage_prince_boom-0.0.5/mypackage_prince_boom.egg-info/top_level.txt
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)       38 2023-05-03 12:47:00.599974 mypackage_prince_boom-0.0.5/setup.cfg
+-rw-rw-r--   0 studio45  (1000) studio45  (1000)      686 2023-05-03 12:46:32.000000 mypackage_prince_boom-0.0.5/setup.py
```

### Comparing `mypackage_prince_boom-0.0.4/LICENSE` & `mypackage_prince_boom-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypackage_prince_boom-0.0.4/setup.py` & `mypackage_prince_boom-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='mypackage_prince_boom',
-    version='0.0.4',
+    version='0.0.5',
     packages=['mypackage_prince_boom'],
     install_requires=[
         'requests',
     ],
     entry_points={
         'console_scripts': [
             'mypackage_prince_boom = mypackage_prince_boom.__main__:main'
```

