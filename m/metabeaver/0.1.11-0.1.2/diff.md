# Comparing `tmp/metabeaver-0.1.11.tar.gz` & `tmp/metabeaver-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabeaver-0.1.11.tar", last modified: Wed May  3 10:56:35 2023, max compression
+gzip compressed data, was "metabeaver-0.1.2.tar", last modified: Wed May  3 11:03:09 2023, max compression
```

## Comparing `metabeaver-0.1.11.tar` & `metabeaver-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 10:56:35.604907 metabeaver-0.1.11/
--rw-rw-rw-   0        0        0      222 2023-05-03 10:56:35.603400 metabeaver-0.1.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 10:56:35.602397 metabeaver-0.1.11/metabeaver.egg-info/
--rw-rw-rw-   0        0        0      222 2023-05-03 10:56:35.000000 metabeaver-0.1.11/metabeaver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-03 10:56:35.000000 metabeaver-0.1.11/metabeaver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 10:56:35.000000 metabeaver-0.1.11/metabeaver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-03 10:56:35.000000 metabeaver-0.1.11/metabeaver.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 10:56:35.000000 metabeaver-0.1.11/metabeaver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 10:56:35.604907 metabeaver-0.1.11/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-05-03 10:56:17.000000 metabeaver-0.1.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:03:09.476634 metabeaver-0.1.2/
+-rw-rw-rw-   0        0        0      221 2023-05-03 11:03:09.475261 metabeaver-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 11:03:09.474259 metabeaver-0.1.2/metabeaver.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-05-03 11:03:09.000000 metabeaver-0.1.2/metabeaver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-05-03 11:03:09.000000 metabeaver-0.1.2/metabeaver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:03:09.000000 metabeaver-0.1.2/metabeaver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-03 11:03:09.000000 metabeaver-0.1.2/metabeaver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:03:09.000000 metabeaver-0.1.2/metabeaver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:03:09.476634 metabeaver-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      697 2023-05-03 10:59:26.000000 metabeaver-0.1.2/setup.py
```

### Comparing `metabeaver-0.1.11/setup.py` & `metabeaver-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metabeaver',
-    version='0.1.11', # Major, minor, patch
+    version='0.1.2', # Major, minor, patch
     packages=find_packages(exclude=['Testing', '*.xlsx', '*.xls']),
     install_requires=[
         'numpy',
         'pandas',
         'google-cloud-core',
         'google-cloud-bigquery',
     ],
```

