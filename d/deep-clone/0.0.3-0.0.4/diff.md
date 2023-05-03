# Comparing `tmp/deep-clone-0.0.3.tar.gz` & `tmp/deep-clone-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep-clone-0.0.3.tar", last modified: Wed May  3 17:36:00 2023, max compression
+gzip compressed data, was "deep-clone-0.0.4.tar", last modified: Wed May  3 17:41:19 2023, max compression
```

## Comparing `deep-clone-0.0.3.tar` & `deep-clone-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 17:36:00.808851 deep-clone-0.0.3/
--rw-rw-rw-   0        0        0     1092 2023-05-03 14:09:43.000000 deep-clone-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      918 2023-05-03 17:36:00.807851 deep-clone-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-05-03 14:08:07.000000 deep-clone-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 17:36:00.806860 deep-clone-0.0.3/deep_clone.egg-info/
--rw-rw-rw-   0        0        0      918 2023-05-03 17:36:00.000000 deep-clone-0.0.3/deep_clone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-05-03 17:36:00.000000 deep-clone-0.0.3/deep_clone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 17:36:00.000000 deep-clone-0.0.3/deep_clone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-03 17:36:00.000000 deep-clone-0.0.3/deep_clone.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-05-03 17:36:00.000000 deep-clone-0.0.3/deep_clone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 17:36:00.809974 deep-clone-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      739 2023-05-03 17:23:40.000000 deep-clone-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 17:41:19.516277 deep-clone-0.0.4/
+-rw-rw-rw-   0        0        0     1092 2023-05-03 14:09:43.000000 deep-clone-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      918 2023-05-03 17:41:19.516277 deep-clone-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-05-03 14:08:07.000000 deep-clone-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 17:41:19.514266 deep-clone-0.0.4/deep_clone.egg-info/
+-rw-rw-rw-   0        0        0      918 2023-05-03 17:41:19.000000 deep-clone-0.0.4/deep_clone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-05-03 17:41:19.000000 deep-clone-0.0.4/deep_clone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 17:41:19.000000 deep-clone-0.0.4/deep_clone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-03 17:41:19.000000 deep-clone-0.0.4/deep_clone.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 17:41:19.000000 deep-clone-0.0.4/deep_clone.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 17:41:19.517269 deep-clone-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      739 2023-05-03 17:40:52.000000 deep-clone-0.0.4/setup.py
```

### Comparing `deep-clone-0.0.3/LICENSE` & `deep-clone-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deep-clone-0.0.3/PKG-INFO` & `deep-clone-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-clone
-Version: 0.0.3
+Version: 0.0.4
 Summary: Deep clone specific folder from a GitHub repo
 Home-page: https://github.com/rajan-personal/deep-clone
 Author: Rajan Gupta
 Author-email: 96rajangupta@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `deep-clone-0.0.3/deep_clone.egg-info/PKG-INFO` & `deep-clone-0.0.4/deep_clone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-clone
-Version: 0.0.3
+Version: 0.0.4
 Summary: Deep clone specific folder from a GitHub repo
 Home-page: https://github.com/rajan-personal/deep-clone
 Author: Rajan Gupta
 Author-email: 96rajangupta@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `deep-clone-0.0.3/setup.py` & `deep-clone-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="deep-clone",
-    version="0.0.3",
+    version="0.0.4",
     py_modules=["deep_clone"],
     install_requires=[],
     entry_points={
         "console_scripts": [
-            "deep_clone=deep_clone.main:main",
+            "deep-clone=deep_clone.main:main",
         ],
     },
     author="Rajan Gupta",
     author_email="96rajangupta@gmail.com",
     description="Deep clone specific folder from a GitHub repo",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

