# Comparing `tmp/msrc-0.0.2.tar.gz` & `tmp/msrc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msrc-0.0.2.tar", last modified: Tue Sep  6 05:12:41 2022, max compression
+gzip compressed data, was "msrc-0.2.0.tar", last modified: Wed May  3 06:48:21 2023, max compression
```

## Comparing `msrc-0.0.2.tar` & `msrc-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 05:12:41.228474 msrc-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-09-06 05:12:41.228474 msrc-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-09-06 05:12:38.000000 msrc-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 05:12:41.228474 msrc-0.0.2/msrc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-09-06 05:12:41.000000 msrc-0.0.2/msrc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-06 05:12:41.000000 msrc-0.0.2/msrc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 05:12:41.000000 msrc-0.0.2/msrc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-06 05:12:41.000000 msrc-0.0.2/msrc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-06 05:12:41.000000 msrc-0.0.2/msrc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-06 05:12:41.000000 msrc-0.0.2/msrc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6665 2022-09-06 05:12:38.000000 msrc-0.0.2/msrc.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 05:12:41.228474 msrc-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-09-06 05:12:38.000000 msrc-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:48:21.919770 msrc-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-03 06:48:21.919770 msrc-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-03 06:48:14.000000 msrc-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:48:21.919770 msrc-0.2.0/msrc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-03 06:48:21.000000 msrc-0.2.0/msrc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 06:48:21.000000 msrc-0.2.0/msrc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:48:21.000000 msrc-0.2.0/msrc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 06:48:21.000000 msrc-0.2.0/msrc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 06:48:21.000000 msrc-0.2.0/msrc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 06:48:21.000000 msrc-0.2.0/msrc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 06:48:21.919770 msrc-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-03 06:48:14.000000 msrc-0.2.0/setup.py
```

### Comparing `msrc-0.0.2/PKG-INFO` & `msrc-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: msrc
-Version: 0.0.2
+Version: 0.2.0
 Summary: MSRC Search tool
 Home-page: https://github.com/haginara/msrc-python
 Author: Jonghak Choi
 Author-email: haginara@gmail.com
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 MSRC(Microsoft Security Research Center) API for python
 ============================================
 
 Installation
 ------------
```

### Comparing `msrc-0.0.2/msrc.egg-info/PKG-INFO` & `msrc-0.2.0/msrc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: msrc
-Version: 0.0.2
+Version: 0.2.0
 Summary: MSRC Search tool
 Home-page: https://github.com/haginara/msrc-python
 Author: Jonghak Choi
 Author-email: haginara@gmail.com
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 MSRC(Microsoft Security Research Center) API for python
 ============================================
 
 Installation
 ------------
```

### Comparing `msrc-0.0.2/setup.py` & `msrc-0.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,40 @@
 from os import path
+from pathlib import Path
 from setuptools import setup
 
-long_description = open(
-    path.join(path.dirname(__file__), 'README.md')
-).read().strip() if path.exists('README.md') else ''
-
-_locals = {}
-with open("msrc.py") as f:
-    for line in f.readlines():
-        if line.startswith('__version_'):
-            exec(line, None, _locals)
-
-version = _locals['__version__']
-
+long_description = (Path(__file__).parent / "README.md").read_text().strip()
 install_requires = [
     "requests"
 ]
 
 setup(
     name="msrc",
     description="MSRC Search tool",
+    version="0.2.0",
     license="MIT License",
     url="https://github.com/haginara/msrc-python",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version=version,
     author='Jonghak Choi',
     author_email='haginara@gmail.com',
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
-            'msrc=msrc:main',
+            'msrc=msrc.cli:main',
         ]
     },
     py_modules=['msrc'],
     package_data={
         '': ['README.md', ]
     },
     include_package_data=True,
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ]
 )
```

