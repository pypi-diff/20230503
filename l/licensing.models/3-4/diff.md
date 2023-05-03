# Comparing `tmp/licensing.models-3.tar.gz` & `tmp/licensing.models-4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "licensing.models-3.tar", last modified: Tue Apr 25 21:23:24 2023, max compression
+gzip compressed data, was "licensing.models-4.tar", last modified: Wed May  3 18:32:13 2023, max compression
```

## Comparing `licensing.models-3.tar` & `licensing.models-4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 21:23:24.684450 licensing.models-3/
--rw-rw-rw-   0        0        0    14731 2023-04-25 21:23:24.684450 licensing.models-3/PKG-INFO
--rw-rw-rw-   0        0        0    13715 2023-03-04 16:03:05.000000 licensing.models-3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 21:23:24.682450 licensing.models-3/licensing.models.egg-info/
--rw-rw-rw-   0        0        0    14731 2023-04-25 21:23:24.000000 licensing.models-3/licensing.models.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-25 21:23:24.000000 licensing.models-3/licensing.models.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 21:23:24.000000 licensing.models-3/licensing.models.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 21:23:24.000000 licensing.models-3/licensing.models.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 21:23:24.000000 licensing.models-3/licensing.models.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-04-25 21:23:24.686449 licensing.models-3/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-04-25 21:23:01.000000 licensing.models-3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 18:32:13.393525 licensing.models-4/
+-rw-rw-rw-   0        0        0    14731 2023-05-03 18:32:13.393525 licensing.models-4/PKG-INFO
+-rw-rw-rw-   0        0        0    13715 2023-03-04 16:03:05.000000 licensing.models-4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 18:32:13.390508 licensing.models-4/licensing.models.egg-info/
+-rw-rw-rw-   0        0        0    14731 2023-05-03 18:32:13.000000 licensing.models-4/licensing.models.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-03 18:32:13.000000 licensing.models-4/licensing.models.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 18:32:13.000000 licensing.models-4/licensing.models.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-03 18:32:13.000000 licensing.models-4/licensing.models.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 18:32:13.000000 licensing.models-4/licensing.models.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-05-03 18:32:13.395506 licensing.models-4/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2023-05-03 18:31:45.000000 licensing.models-4/setup.py
```

### Comparing `licensing.models-3/PKG-INFO` & `licensing.models-4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensing.models
-Version: 3
+Version: 4
 Summary: Pure-python Colors implementation
 Home-page: https://github.com/tartley/colorama
 Author: Jonathan Hartley
 Author-email: tartley@tartley.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `licensing.models-3/README.md` & `licensing.models-4/README.md`

 * *Files identical despite different names*

### Comparing `licensing.models-3/licensing.models.egg-info/PKG-INFO` & `licensing.models-4/licensing.models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: licensing.models
-Version: 3
+Version: 4
 Summary: Pure-python Colors implementation
 Home-page: https://github.com/tartley/colorama
 Author: Jonathan Hartley
 Author-email: tartley@tartley.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `licensing.models-3/setup.py` & `licensing.models-4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='licensing.models',
-    version='3',
+    version='4',
     author='Jonathan Hartley',
     author_email='tartley@tartley.com',
     description='Pure-python Colors implementation',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/tartley/colorama',
     packages=find_packages(),
     install_requires=[
-        'requests'
+        'requests','colorama'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

