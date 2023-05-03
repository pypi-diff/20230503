# Comparing `tmp/pygame_gameover-0.0.1.tar.gz` & `tmp/pygame_gameover-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_gameover-0.0.1.tar", last modified: Wed May  3 09:25:05 2023, max compression
+gzip compressed data, was "pygame_gameover-0.0.2.tar", last modified: Wed May  3 11:09:25 2023, max compression
```

## Comparing `pygame_gameover-0.0.1.tar` & `pygame_gameover-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:25:05.073771 pygame_gameover-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-05-02 11:13:56.000000 pygame_gameover-0.0.1/LICENSE.TXT
--rw-rw-rw-   0        0        0      726 2023-05-03 09:25:05.070947 pygame_gameover-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 09:25:05.019950 pygame_gameover-0.0.1/pygame_gameover/
--rw-rw-rw-   0        0        0        0 2023-05-03 06:53:42.000000 pygame_gameover-0.0.1/pygame_gameover/__init__.py
--rw-rw-rw-   0        0        0     2635 2023-05-03 08:42:50.000000 pygame_gameover-0.0.1/pygame_gameover/gameover.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:25:05.069906 pygame_gameover-0.0.1/pygame_gameover.egg-info/
--rw-rw-rw-   0        0        0      726 2023-05-03 09:25:04.000000 pygame_gameover-0.0.1/pygame_gameover.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-03 09:25:04.000000 pygame_gameover-0.0.1/pygame_gameover.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:25:04.000000 pygame_gameover-0.0.1/pygame_gameover.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-03 09:25:04.000000 pygame_gameover-0.0.1/pygame_gameover.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-03 09:25:04.000000 pygame_gameover-0.0.1/pygame_gameover.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 09:25:05.075293 pygame_gameover-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1085 2023-05-03 09:23:00.000000 pygame_gameover-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:09:25.238433 pygame_gameover-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-05-02 11:13:56.000000 pygame_gameover-0.0.2/LICENSE.TXT
+-rw-rw-rw-   0        0        0      666 2023-05-03 11:09:25.238433 pygame_gameover-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 11:09:25.180915 pygame_gameover-0.0.2/pygame_gameover/
+-rw-rw-rw-   0        0        0        0 2023-05-03 06:53:42.000000 pygame_gameover-0.0.2/pygame_gameover/__init__.py
+-rw-rw-rw-   0        0        0     2635 2023-05-03 08:42:50.000000 pygame_gameover-0.0.2/pygame_gameover/gameover.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:09:25.238433 pygame_gameover-0.0.2/pygame_gameover.egg-info/
+-rw-rw-rw-   0        0        0      666 2023-05-03 11:09:24.000000 pygame_gameover-0.0.2/pygame_gameover.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-03 11:09:25.000000 pygame_gameover-0.0.2/pygame_gameover.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:09:24.000000 pygame_gameover-0.0.2/pygame_gameover.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-03 11:09:24.000000 pygame_gameover-0.0.2/pygame_gameover.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-03 11:09:24.000000 pygame_gameover-0.0.2/pygame_gameover.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:09:25.238433 pygame_gameover-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2023-05-03 11:05:56.000000 pygame_gameover-0.0.2/setup.py
```

### Comparing `pygame_gameover-0.0.1/LICENSE.TXT` & `pygame_gameover-0.0.2/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `pygame_gameover-0.0.1/PKG-INFO` & `pygame_gameover-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pygame_gameover
-Version: 0.0.1
-Summary: pygame_gameover to perfrm gameover
+Version: 0.0.2
+Summary: pygame_gameover to perfrom gameover
 Author: kurban hussain
 Author-email: kurbanhussain086@gmail.com
 Keywords: pygame_gameover,gameover,game over,python tutorial,kurban hussain,game over in python,gameover_pygame,game over pygame,over game
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
-
-C:\Users\Lenovo\Desktop\pygame package gameover\README.MD
```

### Comparing `pygame_gameover-0.0.1/pygame_gameover/gameover.py` & `pygame_gameover-0.0.2/pygame_gameover/gameover.py`

 * *Files identical despite different names*

### Comparing `pygame_gameover-0.0.1/pygame_gameover.egg-info/PKG-INFO` & `pygame_gameover-0.0.2/pygame_gameover.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pygame-gameover
-Version: 0.0.1
-Summary: pygame_gameover to perfrm gameover
+Version: 0.0.2
+Summary: pygame_gameover to perfrom gameover
 Author: kurban hussain
 Author-email: kurbanhussain086@gmail.com
 Keywords: pygame_gameover,gameover,game over,python tutorial,kurban hussain,game over in python,gameover_pygame,game over pygame,over game
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
-
-C:\Users\Lenovo\Desktop\pygame package gameover\README.MD
```

### Comparing `pygame_gameover-0.0.1/setup.py` & `pygame_gameover-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
-DESCRIPTION = 'pygame_gameover to perfrm gameover'
-loag_descciptionss=os.path.join("C:\\Users\\Lenovo\\Desktop\\pygame package gameover\\README.MD")
-
+VERSION = '0.0.2'
+DESCRIPTION = 'pygame_gameover to perfrom gameover'
+loag_descciptionss=''
 # Setting up
 setup(
     name="pygame_gameover",
     version=VERSION,
     author="kurban hussain",
     author_email="kurbanhussain086@gmail.com",
     description=DESCRIPTION,
```

