# Comparing `tmp/pygame_gameover-0.0.2.tar.gz` & `tmp/pygame_gameover-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_gameover-0.0.2.tar", last modified: Wed May  3 11:09:25 2023, max compression
+gzip compressed data, was "pygame_gameover-0.0.3.tar", last modified: Wed May  3 12:26:39 2023, max compression
```

## Comparing `pygame_gameover-0.0.2.tar` & `pygame_gameover-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:09:25.238433 pygame_gameover-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-05-02 11:13:56.000000 pygame_gameover-0.0.2/LICENSE.TXT
--rw-rw-rw-   0        0        0      666 2023-05-03 11:09:25.238433 pygame_gameover-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 11:09:25.180915 pygame_gameover-0.0.2/pygame_gameover/
--rw-rw-rw-   0        0        0        0 2023-05-03 06:53:42.000000 pygame_gameover-0.0.2/pygame_gameover/__init__.py
--rw-rw-rw-   0        0        0     2635 2023-05-03 08:42:50.000000 pygame_gameover-0.0.2/pygame_gameover/gameover.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:09:25.238433 pygame_gameover-0.0.2/pygame_gameover.egg-info/
--rw-rw-rw-   0        0        0      666 2023-05-03 11:09:24.000000 pygame_gameover-0.0.2/pygame_gameover.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-03 11:09:25.000000 pygame_gameover-0.0.2/pygame_gameover.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:09:24.000000 pygame_gameover-0.0.2/pygame_gameover.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-03 11:09:24.000000 pygame_gameover-0.0.2/pygame_gameover.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-03 11:09:24.000000 pygame_gameover-0.0.2/pygame_gameover.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 11:09:25.238433 pygame_gameover-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-05-03 11:05:56.000000 pygame_gameover-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:26:39.541924 pygame_gameover-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-05-02 11:13:56.000000 pygame_gameover-0.0.3/LICENSE.TXT
+-rw-rw-rw-   0        0        0      694 2023-05-03 12:26:39.541924 pygame_gameover-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 12:26:39.503375 pygame_gameover-0.0.3/pygame_gameover/
+-rw-rw-rw-   0        0        0        0 2023-05-03 06:53:42.000000 pygame_gameover-0.0.3/pygame_gameover/__init__.py
+-rw-rw-rw-   0        0        0     2635 2023-05-03 08:42:50.000000 pygame_gameover-0.0.3/pygame_gameover/gameover.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:26:39.539739 pygame_gameover-0.0.3/pygame_gameover.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-05-03 12:26:39.000000 pygame_gameover-0.0.3/pygame_gameover.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-05-03 12:26:39.000000 pygame_gameover-0.0.3/pygame_gameover.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 12:26:39.000000 pygame_gameover-0.0.3/pygame_gameover.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-03 12:26:39.000000 pygame_gameover-0.0.3/pygame_gameover.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 12:26:39.544433 pygame_gameover-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-05-03 12:24:23.000000 pygame_gameover-0.0.3/setup.py
```

### Comparing `pygame_gameover-0.0.2/LICENSE.TXT` & `pygame_gameover-0.0.3/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `pygame_gameover-0.0.2/PKG-INFO` & `pygame_gameover-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pygame_gameover
-Version: 0.0.2
-Summary: pygame_gameover to perfrom gameover
+Version: 0.0.3
+Summary: pygame_gameover is perfrom gameover
 Author: kurban hussain
 Author-email: kurbanhussain086@gmail.com
-Keywords: pygame_gameover,gameover,game over,python tutorial,kurban hussain,game over in python,gameover_pygame,game over pygame,over game
+Keywords: gameover in pygame,pygame gameover,gameover,over game,game over,pygame_gameover,gameover_pygame,pygame game,pygame,pygame GAMEOVER
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
+
+gameover pygame module
```

### Comparing `pygame_gameover-0.0.2/pygame_gameover/gameover.py` & `pygame_gameover-0.0.3/pygame_gameover/gameover.py`

 * *Files identical despite different names*

### Comparing `pygame_gameover-0.0.2/pygame_gameover.egg-info/PKG-INFO` & `pygame_gameover-0.0.3/pygame_gameover.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pygame-gameover
-Version: 0.0.2
-Summary: pygame_gameover to perfrom gameover
+Version: 0.0.3
+Summary: pygame_gameover is perfrom gameover
 Author: kurban hussain
 Author-email: kurbanhussain086@gmail.com
-Keywords: pygame_gameover,gameover,game over,python tutorial,kurban hussain,game over in python,gameover_pygame,game over pygame,over game
+Keywords: gameover in pygame,pygame gameover,gameover,over game,game over,pygame_gameover,gameover_pygame,pygame game,pygame,pygame GAMEOVER
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
+
+gameover pygame module
```

### Comparing `pygame_gameover-0.0.2/setup.py` & `pygame_gameover-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
-DESCRIPTION = 'pygame_gameover to perfrom gameover'
-loag_descciptionss=''
+VERSION = '0.0.3'
+DESCRIPTION = 'pygame_gameover is perfrom gameover'
+LONG_DESCRIPTION = 'gameover pygame module'
+
 # Setting up
 setup(
     name="pygame_gameover",
+    readme='README.MD',
     version=VERSION,
     author="kurban hussain",
     author_email="kurbanhussain086@gmail.com",
     description=DESCRIPTION,
-    long_description=  loag_descciptionss,
     long_description_content_type="text/markdown",
-    
+    long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=["pygame","os","sys","mixer"],
-    keywords=['pygame_gameover', 'gameover', 'game over', 'python tutorial', 'kurban hussain','game over in python','gameover_pygame','game over pygame','over game'],
+    install_requires=[],
+    keywords=['gameover in pygame','pygame gameover','gameover','over game','game over','pygame_gameover','gameover_pygame','pygame game','pygame','pygame GAMEOVER'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

