# Comparing `tmp/skyndo-0.5.tar.gz` & `tmp/skyndo-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyndo-0.5.tar", last modified: Wed May  3 10:46:22 2023, max compression
+gzip compressed data, was "skyndo-0.6.tar", last modified: Wed May  3 10:51:42 2023, max compression
```

## Comparing `skyndo-0.5.tar` & `skyndo-0.6.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 10:46:22.213299 skyndo-0.5/
--rw-rw-rw-   0        0        0      376 2023-05-03 10:46:22.210310 skyndo-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2175 2023-04-12 06:02:34.000000 skyndo-0.5/predict.py
--rw-rw-rw-   0        0        0       42 2023-05-03 10:46:22.213299 skyndo-0.5/setup.cfg
--rw-rw-rw-   0        0        0      540 2023-05-03 10:44:24.000000 skyndo-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:46:22.207315 skyndo-0.5/skyndo.egg-info/
--rw-rw-rw-   0        0        0      376 2023-05-03 10:46:22.000000 skyndo-0.5/skyndo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-05-03 10:46:22.000000 skyndo-0.5/skyndo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 10:46:22.000000 skyndo-0.5/skyndo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-03 10:46:22.000000 skyndo-0.5/skyndo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 10:46:22.000000 skyndo-0.5/skyndo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 10:51:42.636724 skyndo-0.6/
+-rw-rw-rw-   0        0        0      376 2023-05-03 10:51:42.551951 skyndo-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-03 10:51:42.637722 skyndo-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      539 2023-05-03 10:50:19.000000 skyndo-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:51:42.549957 skyndo-0.6/skyndo.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-05-03 10:51:40.000000 skyndo-0.6/skyndo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-05-03 10:51:40.000000 skyndo-0.6/skyndo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 10:51:40.000000 skyndo-0.6/skyndo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-03 10:51:40.000000 skyndo-0.6/skyndo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 10:51:40.000000 skyndo-0.6/skyndo.egg-info/top_level.txt
```

### Comparing `skyndo-0.5/setup.py` & `skyndo-0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='skyndo',
-    version='0.5',
+    version='0.6',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'scikit-learn',
         'numpy'],
-    py_modules=['predict'],
+    py_modules=['skyndo'],
     author='Nishan Obeyesekera',
     author_email='nishandhanu21@gmail.com',
     description='A package to predict the class of astronomical objects for given parameters using a Random Forest model',
     url='https://github.com/NishanD21/Astronomical-Objects-Classification/tree/main/skyndo',
 )
```

