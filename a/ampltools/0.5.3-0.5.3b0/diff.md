# Comparing `tmp/ampltools-0.5.3.tar.gz` & `tmp/ampltools-0.5.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampltools-0.5.3.tar", last modified: Wed May  3 11:06:17 2023, max compression
+gzip compressed data, was "ampltools-0.5.3b0.tar", last modified: Wed May  3 10:56:59 2023, max compression
```

## Comparing `ampltools-0.5.3.tar` & `ampltools-0.5.3b0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-03 11:06:17.914281 ampltools-0.5.3/
--rw-r--r--   0 fdabrandao   (501) staff       (20)     2822 2023-05-03 11:02:11.000000 ampltools-0.5.3/CHANGELOG.md
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1522 2023-03-08 15:44:27.000000 ampltools-0.5.3/LICENSE
--rw-r--r--   0 fdabrandao   (501) staff       (20)       57 2023-03-08 15:44:27.000000 ampltools-0.5.3/MANIFEST.in
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1280 2023-05-03 11:06:17.914033 ampltools-0.5.3/PKG-INFO
--rw-r--r--   0 fdabrandao   (501) staff       (20)      446 2023-03-08 15:44:27.000000 ampltools-0.5.3/README.md
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-03 11:06:17.906957 ampltools-0.5.3/ampltools/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      407 2023-05-03 11:02:47.000000 ampltools-0.5.3/ampltools/__init__.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-03 11:06:17.910255 ampltools-0.5.3/ampltools/modules/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      441 2023-05-03 11:02:47.000000 ampltools-0.5.3/ampltools/modules/__init__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)       93 2023-03-08 15:44:27.000000 ampltools-0.5.3/ampltools/modules/__main__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)    12683 2023-05-03 10:55:31.000000 ampltools-0.5.3/ampltools/modules/amplpypi.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3723 2023-03-09 15:01:44.000000 ampltools-0.5.3/ampltools/modules/commands.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     6017 2023-03-13 16:03:53.000000 ampltools-0.5.3/ampltools/notebooks.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-03 11:06:17.913565 ampltools-0.5.3/ampltools/tests/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      433 2023-03-08 15:44:27.000000 ampltools-0.5.3/ampltools/tests/TestBase.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)       24 2023-03-08 15:44:27.000000 ampltools-0.5.3/ampltools/tests/__init__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)      286 2023-03-08 15:44:27.000000 ampltools-0.5.3/ampltools/tests/__main__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3566 2023-03-08 15:44:27.000000 ampltools-0.5.3/ampltools/tests/test_install.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1951 2023-03-08 15:44:27.000000 ampltools-0.5.3/ampltools/tests/test_load.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     2411 2023-03-13 18:25:11.000000 ampltools-0.5.3/ampltools/tests/test_preload.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1751 2023-03-08 15:44:27.000000 ampltools-0.5.3/ampltools/tests/test_run.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3228 2023-03-09 15:37:57.000000 ampltools-0.5.3/ampltools/utils.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-03 11:06:17.908507 ampltools-0.5.3/ampltools.egg-info/
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1280 2023-05-03 11:06:17.000000 ampltools-0.5.3/ampltools.egg-info/PKG-INFO
--rw-r--r--   0 fdabrandao   (501) staff       (20)      621 2023-05-03 11:06:17.000000 ampltools-0.5.3/ampltools.egg-info/SOURCES.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        1 2023-05-03 11:06:17.000000 ampltools-0.5.3/ampltools.egg-info/dependency_links.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        9 2023-05-03 11:06:17.000000 ampltools-0.5.3/ampltools.egg-info/requires.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)       10 2023-05-03 11:06:17.000000 ampltools-0.5.3/ampltools.egg-info/top_level.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        8 2023-03-08 15:44:27.000000 ampltools-0.5.3/requirements.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)       38 2023-05-03 11:06:17.914360 ampltools-0.5.3/setup.cfg
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1715 2023-05-03 11:06:08.000000 ampltools-0.5.3/setup.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-03 10:56:59.872718 ampltools-0.5.3b0/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     2822 2023-05-03 10:56:16.000000 ampltools-0.5.3b0/CHANGELOG.md
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1522 2023-03-08 15:44:27.000000 ampltools-0.5.3b0/LICENSE
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       57 2023-03-08 15:44:27.000000 ampltools-0.5.3b0/MANIFEST.in
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1245 2023-05-03 10:56:59.872318 ampltools-0.5.3b0/PKG-INFO
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      446 2023-03-08 15:44:27.000000 ampltools-0.5.3b0/README.md
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-03 10:56:59.861236 ampltools-0.5.3b0/ampltools/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      409 2023-05-03 10:56:42.000000 ampltools-0.5.3b0/ampltools/__init__.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-03 10:56:59.867607 ampltools-0.5.3b0/ampltools/modules/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      443 2023-05-03 10:56:42.000000 ampltools-0.5.3b0/ampltools/modules/__init__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       93 2023-03-08 15:44:27.000000 ampltools-0.5.3b0/ampltools/modules/__main__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)    12683 2023-05-03 10:55:31.000000 ampltools-0.5.3b0/ampltools/modules/amplpypi.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3723 2023-03-09 15:01:44.000000 ampltools-0.5.3b0/ampltools/modules/commands.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     6017 2023-03-13 16:03:53.000000 ampltools-0.5.3b0/ampltools/notebooks.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-03 10:56:59.871656 ampltools-0.5.3b0/ampltools/tests/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      433 2023-03-08 15:44:27.000000 ampltools-0.5.3b0/ampltools/tests/TestBase.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       24 2023-03-08 15:44:27.000000 ampltools-0.5.3b0/ampltools/tests/__init__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      286 2023-03-08 15:44:27.000000 ampltools-0.5.3b0/ampltools/tests/__main__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3566 2023-03-08 15:44:27.000000 ampltools-0.5.3b0/ampltools/tests/test_install.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1951 2023-03-08 15:44:27.000000 ampltools-0.5.3b0/ampltools/tests/test_load.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     2411 2023-03-13 18:25:11.000000 ampltools-0.5.3b0/ampltools/tests/test_preload.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1751 2023-03-08 15:44:27.000000 ampltools-0.5.3b0/ampltools/tests/test_run.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3228 2023-03-09 15:37:57.000000 ampltools-0.5.3b0/ampltools/utils.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-03 10:56:59.864963 ampltools-0.5.3b0/ampltools.egg-info/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1245 2023-05-03 10:56:59.000000 ampltools-0.5.3b0/ampltools.egg-info/PKG-INFO
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      621 2023-05-03 10:56:59.000000 ampltools-0.5.3b0/ampltools.egg-info/SOURCES.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        1 2023-05-03 10:56:59.000000 ampltools-0.5.3b0/ampltools.egg-info/dependency_links.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        9 2023-05-03 10:56:59.000000 ampltools-0.5.3b0/ampltools.egg-info/requires.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       10 2023-05-03 10:56:59.000000 ampltools-0.5.3b0/ampltools.egg-info/top_level.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        8 2023-03-08 15:44:27.000000 ampltools-0.5.3b0/requirements.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       38 2023-05-03 10:56:59.872867 ampltools-0.5.3b0/setup.cfg
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1653 2023-05-03 10:56:42.000000 ampltools-0.5.3b0/setup.py
```

### Comparing `ampltools-0.5.3/CHANGELOG.md` & `ampltools-0.5.3b0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.3/LICENSE` & `ampltools-0.5.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.3/PKG-INFO` & `ampltools-0.5.3b0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: ampltools
-Version: 0.5.3
+Version: 0.5.3b0
 Summary: AMPL Python Tools
 Home-page: http://ampl.com/
 Author: Filipe Brandão
 Author-email: fdabrandao@ampl.com
 License: BSD-3
 Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
 Description: 
-        # AMPL Python Tools
+        AMPL Python Tools
+        -----------------
         
-        This package includes tools to use with [AMPL](https://ampl.com) and [amplpy](https://amplpy.readthedocs.io).
+        This package includes tools to use with AMPL and amplpy.
         
-        ## Links
+        Links
+        `````
         
-        * GitHub Repository: https://github.com/ampl/amplpy/
+        * GitHub Repository: https://github.com/ampl/amplpy/tree/master/ampltools
         * PyPI Repository: https://pypi.python.org/pypi/ampltools
         
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -28,8 +30,7 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Description-Content-Type: text/markdown
```

### Comparing `ampltools-0.5.3/ampltools/modules/amplpypi.py` & `ampltools-0.5.3b0/ampltools/modules/amplpypi.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.3/ampltools/modules/commands.py` & `ampltools-0.5.3b0/ampltools/modules/commands.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.3/ampltools/notebooks.py` & `ampltools-0.5.3b0/ampltools/notebooks.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.3/ampltools/tests/test_install.py` & `ampltools-0.5.3b0/ampltools/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.3/ampltools/tests/test_load.py` & `ampltools-0.5.3b0/ampltools/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.3/ampltools/tests/test_preload.py` & `ampltools-0.5.3b0/ampltools/tests/test_preload.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.3/ampltools/tests/test_run.py` & `ampltools-0.5.3b0/ampltools/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.3/ampltools/utils.py` & `ampltools-0.5.3b0/ampltools/utils.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.3/ampltools.egg-info/PKG-INFO` & `ampltools-0.5.3b0/ampltools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: ampltools
-Version: 0.5.3
+Version: 0.5.3b0
 Summary: AMPL Python Tools
 Home-page: http://ampl.com/
 Author: Filipe Brandão
 Author-email: fdabrandao@ampl.com
 License: BSD-3
 Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
 Description: 
-        # AMPL Python Tools
+        AMPL Python Tools
+        -----------------
         
-        This package includes tools to use with [AMPL](https://ampl.com) and [amplpy](https://amplpy.readthedocs.io).
+        This package includes tools to use with AMPL and amplpy.
         
-        ## Links
+        Links
+        `````
         
-        * GitHub Repository: https://github.com/ampl/amplpy/
+        * GitHub Repository: https://github.com/ampl/amplpy/tree/master/ampltools
         * PyPI Repository: https://pypi.python.org/pypi/ampltools
         
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -28,8 +30,7 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Description-Content-Type: text/markdown
```

### Comparing `ampltools-0.5.3/ampltools.egg-info/SOURCES.txt` & `ampltools-0.5.3b0/ampltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.3/setup.py` & `ampltools-0.5.3b0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- coding: utf-8 -*-
 """
-# AMPL Python Tools
+AMPL Python Tools
+-----------------
 
-This package includes tools to use with [AMPL](https://ampl.com) and [amplpy](https://amplpy.readthedocs.io).
+This package includes tools to use with AMPL and amplpy.
 
-## Links
+Links
+`````
 
-* GitHub Repository: https://github.com/ampl/amplpy/
+* GitHub Repository: https://github.com/ampl/amplpy/tree/master/ampltools
 * PyPI Repository: https://pypi.python.org/pypi/ampltools
 """
 from setuptools import setup
 import os
 
 
 def ls_dir(base_dir):
@@ -20,18 +22,17 @@
         for (dirpath, dirnames, files) in os.walk(base_dir)
         for f in files
     ]
 
 
 setup(
     name="ampltools",
-    version="0.5.3",
+    version="0.5.3b0",
     description="AMPL Python Tools",
     long_description=__doc__,
-    long_description_content_type="text/markdown",
     license="BSD-3",
     platforms="any",
     author="Filipe Brandão",
     author_email="fdabrandao@ampl.com",
     url="http://ampl.com/",
     download_url="https://github.com/ampl/amplpy/tree/master/ampltools",
     classifiers=[
```

