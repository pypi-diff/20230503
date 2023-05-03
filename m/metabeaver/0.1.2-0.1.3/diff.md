# Comparing `tmp/metabeaver-0.1.2.tar.gz` & `tmp/metabeaver-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabeaver-0.1.2.tar", last modified: Wed May  3 11:03:09 2023, max compression
+gzip compressed data, was "metabeaver-0.1.3.tar", last modified: Wed May  3 11:15:01 2023, max compression
```

## Comparing `metabeaver-0.1.2.tar` & `metabeaver-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:03:09.476634 metabeaver-0.1.2/
--rw-rw-rw-   0        0        0      221 2023-05-03 11:03:09.475261 metabeaver-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 11:03:09.474259 metabeaver-0.1.2/metabeaver.egg-info/
--rw-rw-rw-   0        0        0      221 2023-05-03 11:03:09.000000 metabeaver-0.1.2/metabeaver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-03 11:03:09.000000 metabeaver-0.1.2/metabeaver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:03:09.000000 metabeaver-0.1.2/metabeaver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-03 11:03:09.000000 metabeaver-0.1.2/metabeaver.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:03:09.000000 metabeaver-0.1.2/metabeaver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 11:03:09.476634 metabeaver-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-05-03 10:59:26.000000 metabeaver-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:15:01.432107 metabeaver-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-05-03 11:15:01.405990 metabeaver-0.1.3/Google Cloud Platform/
+drwxrwxrwx   0        0        0        0 2023-05-03 11:15:01.410037 metabeaver-0.1.3/Google Cloud Platform/Google BigQuery/
+-rw-rw-rw-   0        0        0     2913 2023-05-02 16:05:58.000000 metabeaver-0.1.3/Google Cloud Platform/Google BigQuery/TableManagement.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.3/Google Cloud Platform/Google BigQuery/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 11:50:11.000000 metabeaver-0.1.3/Google Cloud Platform/Google BigQuery/testingTables.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.3/Google Cloud Platform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:15:01.411996 metabeaver-0.1.3/InstallationScripts/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.3/InstallationScripts/__init__.py
+-rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.1.3/InstallationScripts/autoGenerateRequirementsText.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:15:01.414016 metabeaver-0.1.3/MetaProgramming/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.3/MetaProgramming/__init__.py
+-rw-rw-rw-   0        0        0      221 2023-05-03 11:15:01.431105 metabeaver-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 11:15:01.429107 metabeaver-0.1.3/metabeaver.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-05-03 11:15:01.000000 metabeaver-0.1.3/metabeaver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2023-05-03 11:15:01.000000 metabeaver-0.1.3/metabeaver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:15:01.000000 metabeaver-0.1.3/metabeaver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-03 11:15:01.000000 metabeaver-0.1.3/metabeaver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       58 2023-05-03 11:15:01.000000 metabeaver-0.1.3/metabeaver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:15:01.433107 metabeaver-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      697 2023-05-03 11:14:55.000000 metabeaver-0.1.3/setup.py
```

### Comparing `metabeaver-0.1.2/setup.py` & `metabeaver-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metabeaver',
-    version='0.1.2', # Major, minor, patch
+    version='0.1.3', # Major, minor, patch
     packages=find_packages(exclude=['Testing', '*.xlsx', '*.xls']),
     install_requires=[
         'numpy',
         'pandas',
         'google-cloud-core',
         'google-cloud-bigquery',
     ],
```

