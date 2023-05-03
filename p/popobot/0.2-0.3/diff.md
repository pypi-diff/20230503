# Comparing `tmp/popobot-0.2.tar.gz` & `tmp/popobot-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/popobot-0.2.tar", last modified: Wed May  3 05:14:45 2023, max compression
+gzip compressed data, was "dist/popobot-0.3.tar", last modified: Wed May  3 05:26:36 2023, max compression
```

## Comparing `popobot-0.2.tar` & `popobot-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:14:45.000000 popobot-0.2/
--rw-r--r--   0 root         (0) root         (0)     1842 2023-05-03 05:14:45.000000 popobot-0.2/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     1025 2023-05-03 04:01:13.000000 popobot-0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:14:45.000000 popobot-0.2/popobot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1842 2023-05-03 05:14:45.000000 popobot-0.2/popobot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      183 2023-05-03 05:14:45.000000 popobot-0.2/popobot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 05:14:45.000000 popobot-0.2/popobot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-03 05:14:45.000000 popobot-0.2/popobot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-03 05:14:45.000000 popobot-0.2/popobot.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)    11128 2023-05-03 05:12:37.000000 popobot-0.2/popobot.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 05:14:45.000000 popobot-0.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1227 2023-05-03 04:09:16.000000 popobot-0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:26:36.000000 popobot-0.3/
+-rw-r--r--   0 root         (0) root         (0)     1842 2023-05-03 05:26:36.000000 popobot-0.3/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     1025 2023-05-03 04:01:13.000000 popobot-0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:26:36.000000 popobot-0.3/popobot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1842 2023-05-03 05:26:36.000000 popobot-0.3/popobot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      183 2023-05-03 05:26:36.000000 popobot-0.3/popobot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 05:26:36.000000 popobot-0.3/popobot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-03 05:26:36.000000 popobot-0.3/popobot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-03 05:26:36.000000 popobot-0.3/popobot.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)    11140 2023-05-03 05:26:07.000000 popobot-0.3/popobot.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 05:26:36.000000 popobot-0.3/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1227 2023-05-03 04:09:16.000000 popobot-0.3/setup.py
```

### Comparing `popobot-0.2/PKG-INFO` & `popobot-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popobot
-Version: 0.2
+Version: 0.3
 Summary: 泡泡aiM机器人库
 Home-page: https://github.com/HydroGest/PoPoBot
 Author: HydroGest
 Author-email: me@mkc.icu
 License: MIT
 Classifier: Topic :: Games/Entertainment 
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
```

### Comparing `popobot-0.2/README.md` & `popobot-0.3/README.md`

 * *Files identical despite different names*

### Comparing `popobot-0.2/popobot.egg-info/PKG-INFO` & `popobot-0.3/popobot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popobot
-Version: 0.2
+Version: 0.3
 Summary: 泡泡aiM机器人库
 Home-page: https://github.com/HydroGest/PoPoBot
 Author: HydroGest
 Author-email: me@mkc.icu
 License: MIT
 Classifier: Topic :: Games/Entertainment 
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
```

### Comparing `popobot-0.2/popobot.py` & `popobot-0.3/popobot.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 使用方法:
     :from popobot import *
     
 
 开源包，任何人都可以使用并修改！
 """
 
-__version__ = '0.2'
+__version__ = '0.3'
 
+import time
 from requests import get,post
 from json import loads,dumps
 
 class Account:
     def __init__(self, cookie):
         self.cookie = cookie
```

### Comparing `popobot-0.2/setup.py` & `popobot-0.3/setup.py`

 * *Files identical despite different names*

