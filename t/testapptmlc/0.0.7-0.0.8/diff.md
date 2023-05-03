# Comparing `tmp/testapptmlc-0.0.7.tar.gz` & `tmp/testapptmlc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\testapptmlc-0.0.7.tar", last modified: Wed May  3 14:41:57 2023, max compression
+gzip compressed data, was "dist\testapptmlc-0.0.8.tar", last modified: Wed May  3 14:51:04 2023, max compression
```

## Comparing `testapptmlc-0.0.7.tar` & `testapptmlc-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 14:41:57.000000 testapptmlc-0.0.7/
--rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 testapptmlc-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      650 2023-05-03 14:41:57.000000 testapptmlc-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 testapptmlc-0.0.7/README.md
--rw-rw-rw-   0        0        0      565 2023-05-03 14:31:11.000000 testapptmlc-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      129 2023-05-03 14:41:57.000000 testapptmlc-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1910 2023-05-03 14:41:39.000000 testapptmlc-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:41:57.000000 testapptmlc-0.0.7/src/
--rw-rw-rw-   0        0        0       22 2023-05-03 09:58:30.000000 testapptmlc-0.0.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:41:57.000000 testapptmlc-0.0.7/src/runapp/
--rw-rw-rw-   0        0        0       43 2023-05-03 14:31:19.000000 testapptmlc-0.0.7/src/runapp/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-05-03 13:06:07.000000 testapptmlc-0.0.7/src/runapp/app.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:41:57.000000 testapptmlc-0.0.7/testapptmlc.egg-info/
--rw-rw-rw-   0        0        0      650 2023-05-03 14:41:57.000000 testapptmlc-0.0.7/testapptmlc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-03 14:41:57.000000 testapptmlc-0.0.7/testapptmlc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 14:41:57.000000 testapptmlc-0.0.7/testapptmlc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 14:41:57.000000 testapptmlc-0.0.7/testapptmlc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-03 14:41:57.000000 testapptmlc-0.0.7/testapptmlc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 14:51:04.000000 testapptmlc-0.0.8/
+-rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 testapptmlc-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      650 2023-05-03 14:51:04.000000 testapptmlc-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 testapptmlc-0.0.8/README.md
+-rw-rw-rw-   0        0        0      565 2023-05-03 14:48:58.000000 testapptmlc-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      129 2023-05-03 14:51:04.000000 testapptmlc-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1954 2023-05-03 14:50:55.000000 testapptmlc-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:51:04.000000 testapptmlc-0.0.8/src/
+-rw-rw-rw-   0        0        0       22 2023-05-03 09:58:30.000000 testapptmlc-0.0.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:51:04.000000 testapptmlc-0.0.8/src/runapp/
+-rw-rw-rw-   0        0        0       43 2023-05-03 14:49:02.000000 testapptmlc-0.0.8/src/runapp/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-05-03 13:06:07.000000 testapptmlc-0.0.8/src/runapp/app.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:51:04.000000 testapptmlc-0.0.8/testapptmlc.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-05-03 14:51:04.000000 testapptmlc-0.0.8/testapptmlc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-03 14:51:04.000000 testapptmlc-0.0.8/testapptmlc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 14:51:04.000000 testapptmlc-0.0.8/testapptmlc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-03 14:51:04.000000 testapptmlc-0.0.8/testapptmlc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-03 14:51:04.000000 testapptmlc-0.0.8/testapptmlc.egg-info/top_level.txt
```

### Comparing `testapptmlc-0.0.7/LICENSE` & `testapptmlc-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `testapptmlc-0.0.7/PKG-INFO` & `testapptmlc-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testapptmlc
-Version: 0.0.7
+Version: 0.0.8
 Summary: TEST APP TMLC
 Home-page: https://github.com/visalakshi2001/tmlc-pypi
 Author: TMLC
 Author-email: TMLC <visalakshi2001@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/visalakshi2001/tmlc-pypi
 Project-URL: Bug Tracker, https://github.com/visalakshi2001/tmlc-pypi/issues
```

### Comparing `testapptmlc-0.0.7/pyproject.toml` & `testapptmlc-0.0.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "testapptmlc"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="TMLC", email="visalakshi2001@gmail.com" },
 ]
 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `testapptmlc-0.0.7/setup.py` & `testapptmlc-0.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,23 +31,24 @@
 
 
 with open("README.md", "rb") as fh:
     long_description = fh.read().decode("utf-8")
 
 setup(
     name='testapptmlc',
-    version='0.0.7',
+    version='0.0.8',
     license='MIT',
     author="TMLC",
     author_email='visalakshi2001@gmail.com',
     description = "TEST APP TMLC",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages= ["testapptmlc", "testapptmlc.runapp"],
     package_dir={'testapptmlc': 'src'},
+    py_modules=["testapptmlc.runapp.app"],
     url='https://github.com/visalakshi2001/tmlc-pypi',
     keywords='speech recognizer',
     setup_requires=['vosk'],
     install_requires=['vosk'],
     cmdclass={
         'install': CustomInstallCommand,
     },
```

### Comparing `testapptmlc-0.0.7/src/runapp/app.py` & `testapptmlc-0.0.8/src/runapp/app.py`

 * *Files identical despite different names*

### Comparing `testapptmlc-0.0.7/testapptmlc.egg-info/PKG-INFO` & `testapptmlc-0.0.8/testapptmlc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testapptmlc
-Version: 0.0.7
+Version: 0.0.8
 Summary: TEST APP TMLC
 Home-page: https://github.com/visalakshi2001/tmlc-pypi
 Author: TMLC
 Author-email: TMLC <visalakshi2001@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/visalakshi2001/tmlc-pypi
 Project-URL: Bug Tracker, https://github.com/visalakshi2001/tmlc-pypi/issues
```

