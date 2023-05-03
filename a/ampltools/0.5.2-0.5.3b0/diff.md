# Comparing `tmp/ampltools-0.5.2.tar.gz` & `tmp/ampltools-0.5.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampltools-0.5.2.tar", last modified: Wed Apr  5 07:50:15 2023, max compression
+gzip compressed data, was "ampltools-0.5.3b0.tar", last modified: Wed May  3 10:56:59 2023, max compression
```

## Comparing `ampltools-0.5.2.tar` & `ampltools-0.5.3b0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-04-05 07:50:15.164322 ampltools-0.5.2/
--rw-r--r--   0 fdabrandao   (501) staff       (20)     2758 2023-04-05 07:49:38.000000 ampltools-0.5.2/CHANGELOG.md
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1522 2023-03-08 15:44:27.000000 ampltools-0.5.2/LICENSE
--rw-r--r--   0 fdabrandao   (501) staff       (20)       57 2023-03-08 15:44:27.000000 ampltools-0.5.2/MANIFEST.in
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1243 2023-04-05 07:50:15.163968 ampltools-0.5.2/PKG-INFO
--rw-r--r--   0 fdabrandao   (501) staff       (20)      446 2023-03-08 15:44:27.000000 ampltools-0.5.2/README.md
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-04-05 07:50:15.153891 ampltools-0.5.2/ampltools/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      407 2023-04-05 07:49:54.000000 ampltools-0.5.2/ampltools/__init__.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-04-05 07:50:15.157791 ampltools-0.5.2/ampltools/modules/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      441 2023-04-05 07:49:54.000000 ampltools-0.5.2/ampltools/modules/__init__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)       93 2023-03-08 15:44:27.000000 ampltools-0.5.2/ampltools/modules/__main__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)    12304 2023-03-13 18:25:06.000000 ampltools-0.5.2/ampltools/modules/amplpypi.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3723 2023-03-09 15:01:44.000000 ampltools-0.5.2/ampltools/modules/commands.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     6017 2023-03-13 16:03:53.000000 ampltools-0.5.2/ampltools/notebooks.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-04-05 07:50:15.163271 ampltools-0.5.2/ampltools/tests/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      433 2023-03-08 15:44:27.000000 ampltools-0.5.2/ampltools/tests/TestBase.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)       24 2023-03-08 15:44:27.000000 ampltools-0.5.2/ampltools/tests/__init__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)      286 2023-03-08 15:44:27.000000 ampltools-0.5.2/ampltools/tests/__main__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3566 2023-03-08 15:44:27.000000 ampltools-0.5.2/ampltools/tests/test_install.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1951 2023-03-08 15:44:27.000000 ampltools-0.5.2/ampltools/tests/test_load.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     2411 2023-03-13 18:25:11.000000 ampltools-0.5.2/ampltools/tests/test_preload.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1751 2023-03-08 15:44:27.000000 ampltools-0.5.2/ampltools/tests/test_run.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3228 2023-03-09 15:37:57.000000 ampltools-0.5.2/ampltools/utils.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-04-05 07:50:15.155518 ampltools-0.5.2/ampltools.egg-info/
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1243 2023-04-05 07:50:15.000000 ampltools-0.5.2/ampltools.egg-info/PKG-INFO
--rw-r--r--   0 fdabrandao   (501) staff       (20)      621 2023-04-05 07:50:15.000000 ampltools-0.5.2/ampltools.egg-info/SOURCES.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        1 2023-04-05 07:50:15.000000 ampltools-0.5.2/ampltools.egg-info/dependency_links.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        9 2023-04-05 07:50:15.000000 ampltools-0.5.2/ampltools.egg-info/requires.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)       10 2023-04-05 07:50:15.000000 ampltools-0.5.2/ampltools.egg-info/top_level.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        8 2023-03-08 15:44:27.000000 ampltools-0.5.2/requirements.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)       38 2023-04-05 07:50:15.164440 ampltools-0.5.2/setup.cfg
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1651 2023-04-05 07:49:54.000000 ampltools-0.5.2/setup.py
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

### Comparing `ampltools-0.5.2/CHANGELOG.md` & `ampltools-0.5.3b0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/).
 
+## 0.5.3 - 2023-05-03
+- Set ampl_libpath when loading modules.
+
 ## 0.5.2 - 2023-04-05
 - Add message to append to AMPLException messages.
 
 ## 0.5.1 - 2023-03-14
 - When a module is not available, try to indicate a bundle with it.
 - Add unit tests for modules.
 - Make it compatible with Python 3.5.
```

### Comparing `ampltools-0.5.2/LICENSE` & `ampltools-0.5.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.2/PKG-INFO` & `ampltools-0.5.3b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ampltools
-Version: 0.5.2
+Version: 0.5.3b0
 Summary: AMPL Python Tools
 Home-page: http://ampl.com/
 Author: Filipe Brandão
 Author-email: fdabrandao@ampl.com
 License: BSD-3
 Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
 Description:
```

### Comparing `ampltools-0.5.2/ampltools/modules/amplpypi.py` & `ampltools-0.5.3b0/ampltools/modules/amplpypi.py`

 * *Files 12% similar despite different names*

```diff
@@ -332,14 +332,23 @@
     if head:
         os.environ["PATH"] = os.pathsep.join(path_modules + path_others)
     else:
         os.environ["PATH"] = os.pathsep.join(path_others + path_modules)
 
     _prepare_amplkey_env()
 
+    # Add all modules to ampl_libpath (necessary for plugins)
+    ampl_libpath = os.environ.get("ampl_libpath", "").split("\n")
+    for path in path_modules:
+        if path not in ampl_libpath:
+            ampl_libpath.append(path)
+    if ampl_libpath:
+        ampl_libpath = [path for path in ampl_libpath if path]
+        os.environ["ampl_libpath"] = "\n".join(ampl_libpath)
+
 
 def unload_modules(modules=[]):
     """
     Unload AMPL modules.
     Args:
         modules: list of modules to be unloaded.
     """
```

### Comparing `ampltools-0.5.2/ampltools/modules/commands.py` & `ampltools-0.5.3b0/ampltools/modules/commands.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.2/ampltools/notebooks.py` & `ampltools-0.5.3b0/ampltools/notebooks.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.2/ampltools/tests/test_install.py` & `ampltools-0.5.3b0/ampltools/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.2/ampltools/tests/test_load.py` & `ampltools-0.5.3b0/ampltools/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.2/ampltools/tests/test_preload.py` & `ampltools-0.5.3b0/ampltools/tests/test_preload.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.2/ampltools/tests/test_run.py` & `ampltools-0.5.3b0/ampltools/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.2/ampltools/utils.py` & `ampltools-0.5.3b0/ampltools/utils.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.2/ampltools.egg-info/PKG-INFO` & `ampltools-0.5.3b0/ampltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ampltools
-Version: 0.5.2
+Version: 0.5.3b0
 Summary: AMPL Python Tools
 Home-page: http://ampl.com/
 Author: Filipe Brandão
 Author-email: fdabrandao@ampl.com
 License: BSD-3
 Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
 Description:
```

### Comparing `ampltools-0.5.2/ampltools.egg-info/SOURCES.txt` & `ampltools-0.5.3b0/ampltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.2/setup.py` & `ampltools-0.5.3b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         for (dirpath, dirnames, files) in os.walk(base_dir)
         for f in files
     ]
 
 
 setup(
     name="ampltools",
-    version="0.5.2",
+    version="0.5.3b0",
     description="AMPL Python Tools",
     long_description=__doc__,
     license="BSD-3",
     platforms="any",
     author="Filipe Brandão",
     author_email="fdabrandao@ampl.com",
     url="http://ampl.com/",
```

