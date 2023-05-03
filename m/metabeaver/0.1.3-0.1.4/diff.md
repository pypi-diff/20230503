# Comparing `tmp/metabeaver-0.1.3.tar.gz` & `tmp/metabeaver-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabeaver-0.1.3.tar", last modified: Wed May  3 11:15:01 2023, max compression
+gzip compressed data, was "metabeaver-0.1.4.tar", last modified: Wed May  3 11:24:26 2023, max compression
```

## Comparing `metabeaver-0.1.3.tar` & `metabeaver-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:15:01.432107 metabeaver-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-05-03 11:15:01.405990 metabeaver-0.1.3/Google Cloud Platform/
-drwxrwxrwx   0        0        0        0 2023-05-03 11:15:01.410037 metabeaver-0.1.3/Google Cloud Platform/Google BigQuery/
--rw-rw-rw-   0        0        0     2913 2023-05-02 16:05:58.000000 metabeaver-0.1.3/Google Cloud Platform/Google BigQuery/TableManagement.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.3/Google Cloud Platform/Google BigQuery/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-02 11:50:11.000000 metabeaver-0.1.3/Google Cloud Platform/Google BigQuery/testingTables.py
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.3/Google Cloud Platform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:15:01.411996 metabeaver-0.1.3/InstallationScripts/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.3/InstallationScripts/__init__.py
--rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.1.3/InstallationScripts/autoGenerateRequirementsText.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:15:01.414016 metabeaver-0.1.3/MetaProgramming/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.3/MetaProgramming/__init__.py
--rw-rw-rw-   0        0        0      221 2023-05-03 11:15:01.431105 metabeaver-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 11:15:01.429107 metabeaver-0.1.3/metabeaver.egg-info/
--rw-rw-rw-   0        0        0      221 2023-05-03 11:15:01.000000 metabeaver-0.1.3/metabeaver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2023-05-03 11:15:01.000000 metabeaver-0.1.3/metabeaver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:15:01.000000 metabeaver-0.1.3/metabeaver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-03 11:15:01.000000 metabeaver-0.1.3/metabeaver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       58 2023-05-03 11:15:01.000000 metabeaver-0.1.3/metabeaver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 11:15:01.433107 metabeaver-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-05-03 11:14:55.000000 metabeaver-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:24:26.572859 metabeaver-0.1.4/
+-rw-rw-rw-   0        0        0      221 2023-05-03 11:24:26.571859 metabeaver-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 11:24:26.533540 metabeaver-0.1.4/metabeaver/
+drwxrwxrwx   0        0        0        0 2023-05-03 11:24:26.558315 metabeaver-0.1.4/metabeaver/Google Cloud Platform/
+drwxrwxrwx   0        0        0        0 2023-05-03 11:24:26.562357 metabeaver-0.1.4/metabeaver/Google Cloud Platform/Google BigQuery/
+-rw-rw-rw-   0        0        0     2913 2023-05-02 16:05:58.000000 metabeaver-0.1.4/metabeaver/Google Cloud Platform/Google BigQuery/TableManagement.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.4/metabeaver/Google Cloud Platform/Google BigQuery/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 11:50:11.000000 metabeaver-0.1.4/metabeaver/Google Cloud Platform/Google BigQuery/testingTables.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.4/metabeaver/Google Cloud Platform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:24:26.565355 metabeaver-0.1.4/metabeaver/InstallationScripts/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.4/metabeaver/InstallationScripts/__init__.py
+-rw-rw-rw-   0        0        0     1246 2023-04-07 12:06:41.000000 metabeaver-0.1.4/metabeaver/InstallationScripts/autoGenerateRequirementsText.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:24:26.566853 metabeaver-0.1.4/metabeaver/MetaProgramming/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.4/metabeaver/MetaProgramming/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:24:26.569857 metabeaver-0.1.4/metabeaver/Testing/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.4/metabeaver/Testing/__init__.py
+-rw-rw-rw-   0        0        0     1804 2023-04-26 12:07:06.000000 metabeaver-0.1.4/metabeaver/Testing/concatenateDataXLSX.py
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:11:32.000000 metabeaver-0.1.4/metabeaver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:24:26.556270 metabeaver-0.1.4/metabeaver.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-05-03 11:24:26.000000 metabeaver-0.1.4/metabeaver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-05-03 11:24:26.000000 metabeaver-0.1.4/metabeaver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:24:26.000000 metabeaver-0.1.4/metabeaver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-03 11:24:26.000000 metabeaver-0.1.4/metabeaver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 11:24:26.000000 metabeaver-0.1.4/metabeaver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:24:26.573869 metabeaver-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      697 2023-05-03 11:23:10.000000 metabeaver-0.1.4/setup.py
```

### Comparing `metabeaver-0.1.3/Google Cloud Platform/Google BigQuery/TableManagement.py` & `metabeaver-0.1.4/metabeaver/Google Cloud Platform/Google BigQuery/TableManagement.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.1.3/InstallationScripts/autoGenerateRequirementsText.py` & `metabeaver-0.1.4/metabeaver/InstallationScripts/autoGenerateRequirementsText.py`

 * *Files identical despite different names*

### Comparing `metabeaver-0.1.3/setup.py` & `metabeaver-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metabeaver',
-    version='0.1.3', # Major, minor, patch
+    version='0.1.4', # Major, minor, patch
     packages=find_packages(exclude=['Testing', '*.xlsx', '*.xls']),
     install_requires=[
         'numpy',
         'pandas',
         'google-cloud-core',
         'google-cloud-bigquery',
     ],
```

