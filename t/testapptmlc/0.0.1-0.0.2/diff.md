# Comparing `tmp/testapptmlc-0.0.1.tar.gz` & `tmp/testapptmlc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\testapptmlc-0.0.1.tar", last modified: Wed May  3 09:15:32 2023, max compression
+gzip compressed data, was "dist\testapptmlc-0.0.2.tar", last modified: Wed May  3 09:42:52 2023, max compression
```

## Comparing `testapptmlc-0.0.1.tar` & `testapptmlc-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:15:32.000000 testapptmlc-0.0.1/
--rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 testapptmlc-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      652 2023-05-03 09:15:32.000000 testapptmlc-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 testapptmlc-0.0.1/README.md
--rw-rw-rw-   0        0        0      569 2023-05-02 13:01:57.000000 testapptmlc-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 09:15:32.000000 testapptmlc-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1879 2023-05-03 08:56:54.000000 testapptmlc-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:15:32.000000 testapptmlc-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 09:15:32.000000 testapptmlc-0.0.1/src/runapp/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:24:47.000000 testapptmlc-0.0.1/src/runapp/__init__.py
--rw-rw-rw-   0        0        0      793 2023-05-03 08:47:21.000000 testapptmlc-0.0.1/src/runapp/app.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:15:32.000000 testapptmlc-0.0.1/src/testapptmlc.egg-info/
--rw-rw-rw-   0        0        0      652 2023-05-03 09:15:32.000000 testapptmlc-0.0.1/src/testapptmlc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-05-03 09:15:32.000000 testapptmlc-0.0.1/src/testapptmlc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:15:32.000000 testapptmlc-0.0.1/src/testapptmlc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 09:15:32.000000 testapptmlc-0.0.1/src/testapptmlc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 09:15:32.000000 testapptmlc-0.0.1/src/testapptmlc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/
+-rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 testapptmlc-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      650 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-05-02 10:35:43.000000 testapptmlc-0.0.2/README.md
+-rw-rw-rw-   0        0        0      565 2023-05-03 09:40:33.000000 testapptmlc-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1888 2023-05-03 09:41:02.000000 testapptmlc-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/src/
+-rw-rw-rw-   0        0        0       20 2023-05-03 09:36:36.000000 testapptmlc-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/testapptmlc.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/testapptmlc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/testapptmlc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/testapptmlc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/testapptmlc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-03 09:42:52.000000 testapptmlc-0.0.2/testapptmlc.egg-info/top_level.txt
```

### Comparing `testapptmlc-0.0.1/LICENSE` & `testapptmlc-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `testapptmlc-0.0.1/PKG-INFO` & `testapptmlc-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: testapptmlc
-Version: 0.0.1
+Version: 0.0.2
 Summary: TEST APP TMLC
 Home-page: https://github.com/visalakshi2001/tmlc-pypi
 Author: TMLC
-Author-email: Example Author <author@example.com>
+Author-email: TMLC <visalakshi2001@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/visalakshi2001/tmlc-pypi
 Project-URL: Bug Tracker, https://github.com/visalakshi2001/tmlc-pypi/issues
-Keywords: example project
+Keywords: speech recognizer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `testapptmlc-0.0.1/pyproject.toml` & `testapptmlc-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "testapptmlc"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
-  { name="Example Author", email="author@example.com" },
+  { name="TMLC", email="visalakshi2001@gmail.com" },
 ]
 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `testapptmlc-0.0.1/setup.py` & `testapptmlc-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,25 +31,25 @@
 
 
 with open("README.md", "rb") as fh:
     long_description = fh.read().decode("utf-8")
 
 setup(
     name='testapptmlc',
-    version='0.0.1',
+    version='0.0.2',
     license='MIT',
     author="TMLC",
     author_email='visalakshi2001@gmail.com',
     description = "TEST APP TMLC",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    packages=find_packages('src'),
-    package_dir={'': 'src'},
+    packages= ["testapptmlc"],
+    package_dir={'testapptmlc': 'src'},
     url='https://github.com/visalakshi2001/tmlc-pypi',
-    keywords='example project',
+    keywords='speech recognizer',
     setup_requires=['vosk'],
     install_requires=['vosk'],
     cmdclass={
         'install': CustomInstallCommand,
     },
 
 )
```

### Comparing `testapptmlc-0.0.1/src/testapptmlc.egg-info/PKG-INFO` & `testapptmlc-0.0.2/testapptmlc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: testapptmlc
-Version: 0.0.1
+Version: 0.0.2
 Summary: TEST APP TMLC
 Home-page: https://github.com/visalakshi2001/tmlc-pypi
 Author: TMLC
-Author-email: Example Author <author@example.com>
+Author-email: TMLC <visalakshi2001@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/visalakshi2001/tmlc-pypi
 Project-URL: Bug Tracker, https://github.com/visalakshi2001/tmlc-pypi/issues
-Keywords: example project
+Keywords: speech recognizer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

