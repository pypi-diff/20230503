# Comparing `tmp/astrojs-aws.construct-0.0.8.tar.gz` & `tmp/astrojs-aws.construct-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrojs-aws.construct-0.0.8.tar", last modified: Fri Apr 14 11:34:08 2023, max compression
+gzip compressed data, was "astrojs-aws.construct-0.0.9.tar", last modified: Fri Apr 14 11:48:49 2023, max compression
```

## Comparing `astrojs-aws.construct-0.0.8.tar` & `astrojs-aws.construct-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.150971 astrojs-aws.construct-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-14 11:34:08.150971 astrojs-aws.construct-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 11:34:08.150971 astrojs-aws.construct-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.146971 astrojs-aws.construct-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.146971 astrojs-aws.construct-0.0.8/src/astrojs_aws/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.150971 astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/
--rw-r--r--   0 runner    (1001) docker     (123)   144514 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.150971 astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25711 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/_jsii/construct@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.150971 astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-14 11:34:08.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 11:34:08.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:34:08.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 11:34:08.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 11:34:08.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:48:49.023298 astrojs-aws.construct-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 11:48:26.000000 astrojs-aws.construct-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 11:48:26.000000 astrojs-aws.construct-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-14 11:48:49.023298 astrojs-aws.construct-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-14 11:48:26.000000 astrojs-aws.construct-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 11:48:26.000000 astrojs-aws.construct-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 11:48:49.023298 astrojs-aws.construct-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-14 11:48:26.000000 astrojs-aws.construct-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:48:49.011298 astrojs-aws.construct-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:48:49.011298 astrojs-aws.construct-0.0.9/src/astrojs_aws/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:48:49.019298 astrojs-aws.construct-0.0.9/src/astrojs_aws/construct/
+-rw-r--r--   0 runner    (1001) docker     (123)   144514 2023-04-14 11:48:26.000000 astrojs-aws.construct-0.0.9/src/astrojs_aws/construct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:48:49.023298 astrojs-aws.construct-0.0.9/src/astrojs_aws/construct/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 11:48:26.000000 astrojs-aws.construct-0.0.9/src/astrojs_aws/construct/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25711 2023-04-14 11:48:26.000000 astrojs-aws.construct-0.0.9/src/astrojs_aws/construct/_jsii/construct@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:48:26.000000 astrojs-aws.construct-0.0.9/src/astrojs_aws/construct/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:48:49.019298 astrojs-aws.construct-0.0.9/src/astrojs_aws.construct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-14 11:48:48.000000 astrojs-aws.construct-0.0.9/src/astrojs_aws.construct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 11:48:48.000000 astrojs-aws.construct-0.0.9/src/astrojs_aws.construct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:48:48.000000 astrojs-aws.construct-0.0.9/src/astrojs_aws.construct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 11:48:48.000000 astrojs-aws.construct-0.0.9/src/astrojs_aws.construct.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 11:48:48.000000 astrojs-aws.construct-0.0.9/src/astrojs_aws.construct.egg-info/top_level.txt
```

### Comparing `astrojs-aws.construct-0.0.8/LICENSE` & `astrojs-aws.construct-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `astrojs-aws.construct-0.0.8/PKG-INFO` & `astrojs-aws.construct-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrojs-aws.construct
-Version: 0.0.8
+Version: 0.0.9
 Summary: The CDK Construct Library of Astro
 Home-page: https://astro-aws.org/
 Author: helbing
 License: MIT
 Project-URL: Source, https://github.com/helbing/astrojs-aws.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `astrojs-aws.construct-0.0.8/README.md` & `astrojs-aws.construct-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `astrojs-aws.construct-0.0.8/setup.py` & `astrojs-aws.construct-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "astrojs-aws.construct",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "The CDK Construct Library of Astro",
     "license": "MIT",
     "url": "https://astro-aws.org/",
     "long_description_content_type": "text/markdown",
     "author": "helbing",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "astrojs_aws.construct",
         "astrojs_aws.construct._jsii"
     ],
     "package_data": {
         "astrojs_aws.construct._jsii": [
-            "construct@0.0.8.jsii.tgz"
+            "construct@0.0.9.jsii.tgz"
         ],
         "astrojs_aws.construct": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/__init__.py` & `astrojs-aws.construct-0.0.9/src/astrojs_aws/construct/__init__.py`

 * *Files identical despite different names*

### Comparing `astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/PKG-INFO` & `astrojs-aws.construct-0.0.9/src/astrojs_aws.construct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrojs-aws.construct
-Version: 0.0.8
+Version: 0.0.9
 Summary: The CDK Construct Library of Astro
 Home-page: https://astro-aws.org/
 Author: helbing
 License: MIT
 Project-URL: Source, https://github.com/helbing/astrojs-aws.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

