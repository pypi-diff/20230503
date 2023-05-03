# Comparing `tmp/testapptmlc-0.1.2.tar.gz` & `tmp/testapptmlc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\testapptmlc-0.1.2.tar", last modified: Wed May  3 17:12:57 2023, max compression
+gzip compressed data, was "dist\testapptmlc-0.1.3.tar", last modified: Wed May  3 18:37:56 2023, max compression
```

## Comparing `testapptmlc-0.1.2.tar` & `testapptmlc-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 17:12:57.000000 testapptmlc-0.1.2/
--rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 testapptmlc-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      650 2023-05-03 17:12:57.000000 testapptmlc-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 testapptmlc-0.1.2/README.md
--rw-rw-rw-   0        0        0      565 2023-05-03 15:38:56.000000 testapptmlc-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      129 2023-05-03 17:12:57.000000 testapptmlc-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2081 2023-05-03 17:12:45.000000 testapptmlc-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 17:12:57.000000 testapptmlc-0.1.2/src/
--rw-rw-rw-   0        0        0       22 2023-05-03 09:58:30.000000 testapptmlc-0.1.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 17:12:57.000000 testapptmlc-0.1.2/src/runapp/
-drwxrwxrwx   0        0        0        0 2023-05-03 17:12:57.000000 testapptmlc-0.1.2/src/runapp/Vosk/
-drwxrwxrwx   0        0        0        0 2023-05-03 17:12:57.000000 testapptmlc-0.1.2/src/runapp/Vosk/vosk-model-en-us-daanzu-20200905-lgraph/
--rw-rw-rw-   0        0        0       31 2023-05-02 10:12:33.000000 testapptmlc-0.1.2/src/runapp/Vosk/vosk-model-en-us-daanzu-20200905-lgraph/AUTHORS.txt
--rw-rw-rw-   0        0        0    34523 2023-05-02 10:12:33.000000 testapptmlc-0.1.2/src/runapp/Vosk/vosk-model-en-us-daanzu-20200905-lgraph/LICENSE.txt
--rw-rw-rw-   0        0        0       94 2023-05-02 10:12:33.000000 testapptmlc-0.1.2/src/runapp/Vosk/vosk-model-en-us-daanzu-20200905-lgraph/README
--rw-rw-rw-   0        0        0       43 2023-05-03 15:39:02.000000 testapptmlc-0.1.2/src/runapp/__init__.py
--rw-rw-rw-   0        0        0     1185 2023-05-03 15:07:55.000000 testapptmlc-0.1.2/src/runapp/app.py
-drwxrwxrwx   0        0        0        0 2023-05-03 17:12:57.000000 testapptmlc-0.1.2/testapptmlc.egg-info/
--rw-rw-rw-   0        0        0      650 2023-05-03 17:12:56.000000 testapptmlc-0.1.2/testapptmlc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-05-03 17:12:57.000000 testapptmlc-0.1.2/testapptmlc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 17:12:56.000000 testapptmlc-0.1.2/testapptmlc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 17:12:56.000000 testapptmlc-0.1.2/testapptmlc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-03 17:12:56.000000 testapptmlc-0.1.2/testapptmlc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 18:37:56.000000 testapptmlc-0.1.3/
+-rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 testapptmlc-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      650 2023-05-03 18:37:56.000000 testapptmlc-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 testapptmlc-0.1.3/README.md
+-rw-rw-rw-   0        0        0      565 2023-05-03 18:37:43.000000 testapptmlc-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      129 2023-05-03 18:37:56.000000 testapptmlc-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2118 2023-05-03 18:37:38.000000 testapptmlc-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:37:56.000000 testapptmlc-0.1.3/src/
+-rw-rw-rw-   0        0        0       22 2023-05-03 09:58:30.000000 testapptmlc-0.1.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:37:56.000000 testapptmlc-0.1.3/src/runapp/
+-rw-rw-rw-   0        0        0       43 2023-05-03 18:37:45.000000 testapptmlc-0.1.3/src/runapp/__init__.py
+-rw-rw-rw-   0        0        0     1767 2023-05-03 18:34:11.000000 testapptmlc-0.1.3/src/runapp/app.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:37:56.000000 testapptmlc-0.1.3/testapptmlc.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-05-03 18:37:55.000000 testapptmlc-0.1.3/testapptmlc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-03 18:37:55.000000 testapptmlc-0.1.3/testapptmlc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 18:37:55.000000 testapptmlc-0.1.3/testapptmlc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-03 18:37:55.000000 testapptmlc-0.1.3/testapptmlc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-03 18:37:55.000000 testapptmlc-0.1.3/testapptmlc.egg-info/top_level.txt
```

### Comparing `testapptmlc-0.1.2/LICENSE` & `testapptmlc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `testapptmlc-0.1.2/PKG-INFO` & `testapptmlc-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testapptmlc
-Version: 0.1.2
+Version: 0.1.3
 Summary: TEST APP TMLC
 Home-page: https://github.com/visalakshi2001/tmlc-pypi
 Author: TMLC
 Author-email: TMLC <visalakshi2001@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/visalakshi2001/tmlc-pypi
 Project-URL: Bug Tracker, https://github.com/visalakshi2001/tmlc-pypi/issues
```

### Comparing `testapptmlc-0.1.2/pyproject.toml` & `testapptmlc-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "testapptmlc"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="TMLC", email="visalakshi2001@gmail.com" },
 ]
 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `testapptmlc-0.1.2/setup.py` & `testapptmlc-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 with open("README.md", "rb") as fh:
     long_description = fh.read().decode("utf-8")
 
 setup(
     name='testapptmlc',
-    version='0.1.2',
+    version='0.1.3',
     license='MIT',
     author="TMLC",
     author_email='visalakshi2001@gmail.com',
     description = "TEST APP TMLC",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages= ["testapptmlc", "testapptmlc.runapp"],
@@ -49,10 +49,10 @@
     url='https://github.com/visalakshi2001/tmlc-pypi',
     keywords='speech recognizer',
     setup_requires=['vosk'],
     install_requires=['vosk'],
     cmdclass={
         'install': CustomInstallCommand,
     },
-    data_files= glob("./src/runapp/Vosk/**/*"),
-    package_data= {'': glob("./src/runapp/Vosk/**/*")},
+    # data_files= glob("./src/runapp/Vosk/**/*", recursive=True),
+    # package_data= {'': glob("./src/runapp/Vosk/**/**", recursive=True)},
 )
```

### Comparing `testapptmlc-0.1.2/testapptmlc.egg-info/PKG-INFO` & `testapptmlc-0.1.3/testapptmlc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testapptmlc
-Version: 0.1.2
+Version: 0.1.3
 Summary: TEST APP TMLC
 Home-page: https://github.com/visalakshi2001/tmlc-pypi
 Author: TMLC
 Author-email: TMLC <visalakshi2001@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/visalakshi2001/tmlc-pypi
 Project-URL: Bug Tracker, https://github.com/visalakshi2001/tmlc-pypi/issues
```

