# Comparing `tmp/FixedFloatApi-1.0.0.tar.gz` & `tmp/FixedFloatApi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/FixedFloatApi-1.0.0.tar", last modified: Tue May  2 20:37:21 2023, max compression
+gzip compressed data, was "dist/FixedFloatApi-1.0.1.tar", last modified: Tue May  2 21:55:05 2023, max compression
```

## Comparing `FixedFloatApi-1.0.0.tar` & `FixedFloatApi-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,16 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 20:37:21.000000 FixedFloatApi-1.0.0/
--rw-rw-r--   0 root         (0) root         (0)     3210 2023-05-02 20:37:21.000000 FixedFloatApi-1.0.0/PKG-INFO
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 20:37:21.000000 FixedFloatApi-1.0.0/fixedfloatapi/
--rw-rw-r--   0 root         (0) root         (0)     1522 2023-05-02 20:34:32.000000 FixedFloatApi-1.0.0/fixedfloatapi/FixedFloatAPI.py
--rw-rw-r--   0 root         (0) root         (0)       38 2023-05-02 20:34:32.000000 FixedFloatApi-1.0.0/fixedfloatapi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       39 2023-05-02 20:34:32.000000 FixedFloatApi-1.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1036 2023-05-02 20:34:32.000000 FixedFloatApi-1.0.0/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/FixedFloatApi.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     3250 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/FixedFloatApi.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      293 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/FixedFloatApi.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/FixedFloatApi.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/FixedFloatApi.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       14 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/FixedFloatApi.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     1060 2023-05-02 21:50:09.000000 FixedFloatApi-1.0.1/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-05-02 21:50:09.000000 FixedFloatApi-1.0.1/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)     3250 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1848 2023-05-02 21:50:09.000000 FixedFloatApi-1.0.1/README.md
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/fixedfloatapi/
+-rw-rw-r--   0 root         (0) root         (0)     1522 2023-05-02 21:50:09.000000 FixedFloatApi-1.0.1/fixedfloatapi/FixedFloatAPI.py
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-05-02 21:50:09.000000 FixedFloatApi-1.0.1/fixedfloatapi/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       79 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1017 2023-05-02 21:50:09.000000 FixedFloatApi-1.0.1/setup.py
```

### Comparing `FixedFloatApi-1.0.0/PKG-INFO` & `FixedFloatApi-1.0.1/FixedFloatApi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: FixedFloatApi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python wrapper for interacting with the FixedFloat API to exchange cryptocurrencies.
 Home-page: https://github.com/Jobians/FixedFloatApi
 Author: JobiansTechie
 Author-email: jobianstechie@gmail.com
 License: MIT
 Description: FixedFloatApi
         =============
@@ -91,7 +91,8 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
```

### Comparing `FixedFloatApi-1.0.0/fixedfloatapi/FixedFloatAPI.py` & `FixedFloatApi-1.0.1/fixedfloatapi/FixedFloatAPI.py`

 * *Files identical despite different names*

### Comparing `FixedFloatApi-1.0.0/setup.py` & `FixedFloatApi-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from distutils.core import setup
-
-with open('README.md', 'r') as f:
-    long_description = f.read()
+from setuptools import setup, find_packages
 
 setup(
     name='FixedFloatApi',
-    packages=['fixedfloatapi'],
-    version='1.0.0',
+    packages=find_packages(),
+    include_package_data=True,
+    version='1.0.1',
     license='MIT',
     description='Python wrapper for interacting with the FixedFloat API to exchange cryptocurrencies.',
-    long_description=long_description,
+    long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='JobiansTechie',
     author_email='jobianstechie@gmail.com',
     url='https://github.com/Jobians/FixedFloatApi',
     keywords=['FixedFloat', 'Api', 'FixedFloat Python'],
     install_requires=[
         'requests'
```

