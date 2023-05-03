# Comparing `tmp/testapptmlc-0.0.2.tar.gz` & `tmp/testapptmlc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\testapptmlc-0.0.2.tar", last modified: Wed May  3 09:42:52 2023, max compression
+gzip compressed data, was "dist\testapptmlc-0.0.3.tar", last modified: Wed May  3 09:48:08 2023, max compression
```

## Comparing `testapptmlc-0.0.2.tar` & `testapptmlc-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/
--rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 testapptmlc-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      650 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 testapptmlc-0.0.2/README.md
--rw-rw-rw-   0        0        0      565 2023-05-03 09:40:33.000000 testapptmlc-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1888 2023-05-03 09:41:02.000000 testapptmlc-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/src/
--rw-rw-rw-   0        0        0       20 2023-05-03 09:36:36.000000 testapptmlc-0.0.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/testapptmlc.egg-info/
--rw-rw-rw-   0        0        0      650 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/testapptmlc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/testapptmlc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/testapptmlc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/testapptmlc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/testapptmlc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:08.000000 testapptmlc-0.0.3/
+-rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 testapptmlc-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      650 2023-05-03 09:48:08.000000 testapptmlc-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 testapptmlc-0.0.3/README.md
+-rw-rw-rw-   0        0        0      565 2023-05-03 09:48:00.000000 testapptmlc-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 09:48:08.000000 testapptmlc-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1888 2023-05-03 09:48:01.000000 testapptmlc-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:08.000000 testapptmlc-0.0.3/src/
+-rw-rw-rw-   0        0        0       35 2023-05-03 09:47:37.000000 testapptmlc-0.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:48:08.000000 testapptmlc-0.0.3/testapptmlc.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-05-03 09:48:07.000000 testapptmlc-0.0.3/testapptmlc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-03 09:48:07.000000 testapptmlc-0.0.3/testapptmlc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 09:48:07.000000 testapptmlc-0.0.3/testapptmlc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-03 09:48:07.000000 testapptmlc-0.0.3/testapptmlc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-03 09:48:07.000000 testapptmlc-0.0.3/testapptmlc.egg-info/top_level.txt
```

### Comparing `testapptmlc-0.0.2/LICENSE` & `testapptmlc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `testapptmlc-0.0.2/PKG-INFO` & `testapptmlc-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testapptmlc
-Version: 0.0.2
+Version: 0.0.3
 Summary: TEST APP TMLC
 Home-page: https://github.com/visalakshi2001/tmlc-pypi
 Author: TMLC
 Author-email: TMLC <visalakshi2001@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/visalakshi2001/tmlc-pypi
 Project-URL: Bug Tracker, https://github.com/visalakshi2001/tmlc-pypi/issues
```

### Comparing `testapptmlc-0.0.2/pyproject.toml` & `testapptmlc-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "testapptmlc"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="TMLC", email="visalakshi2001@gmail.com" },
 ]
 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `testapptmlc-0.0.2/setup.py` & `testapptmlc-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 with open("README.md", "rb") as fh:
     long_description = fh.read().decode("utf-8")
 
 setup(
     name='testapptmlc',
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     author="TMLC",
     author_email='visalakshi2001@gmail.com',
     description = "TEST APP TMLC",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages= ["testapptmlc"],
```

### Comparing `testapptmlc-0.0.2/testapptmlc.egg-info/PKG-INFO` & `testapptmlc-0.0.3/testapptmlc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testapptmlc
-Version: 0.0.2
+Version: 0.0.3
 Summary: TEST APP TMLC
 Home-page: https://github.com/visalakshi2001/tmlc-pypi
 Author: TMLC
 Author-email: TMLC <visalakshi2001@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/visalakshi2001/tmlc-pypi
 Project-URL: Bug Tracker, https://github.com/visalakshi2001/tmlc-pypi/issues
```

