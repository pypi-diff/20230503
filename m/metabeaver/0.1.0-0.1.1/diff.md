# Comparing `tmp/metabeaver-0.1.0.tar.gz` & `tmp/metabeaver-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabeaver-0.1.0.tar", last modified: Tue May  2 20:10:16 2023, max compression
+gzip compressed data, was "metabeaver-0.1.1.tar", last modified: Wed May  3 08:37:01 2023, max compression
```

## Comparing `metabeaver-0.1.0.tar` & `metabeaver-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 20:10:16.847708 metabeaver-0.1.0/
--rw-rw-rw-   0        0        0      221 2023-05-02 20:10:16.846700 metabeaver-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 20:10:16.845163 metabeaver-0.1.0/metabeaver.egg-info/
--rw-rw-rw-   0        0        0      221 2023-05-02 20:10:16.000000 metabeaver-0.1.0/metabeaver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-02 20:10:16.000000 metabeaver-0.1.0/metabeaver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 20:10:16.000000 metabeaver-0.1.0/metabeaver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-02 20:10:16.000000 metabeaver-0.1.0/metabeaver.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 20:10:16.000000 metabeaver-0.1.0/metabeaver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 20:10:16.847708 metabeaver-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      635 2023-05-02 20:03:36.000000 metabeaver-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 08:37:01.872162 metabeaver-0.1.1/
+-rw-rw-rw-   0        0        0      221 2023-05-03 08:37:01.870123 metabeaver-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 08:37:01.868050 metabeaver-0.1.1/metabeaver.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-05-03 08:37:01.000000 metabeaver-0.1.1/metabeaver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-05-03 08:37:01.000000 metabeaver-0.1.1/metabeaver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 08:37:01.000000 metabeaver-0.1.1/metabeaver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-03 08:37:01.000000 metabeaver-0.1.1/metabeaver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 08:37:01.000000 metabeaver-0.1.1/metabeaver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 08:37:01.872162 metabeaver-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      637 2023-05-03 07:56:38.000000 metabeaver-0.1.1/setup.py
```

### Comparing `metabeaver-0.1.0/setup.py` & `metabeaver-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metabeaver',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'google-cloud-core',
         'google-cloud-bigquery',
     ],
@@ -21,12 +21,13 @@
 
 #QHFG25#DQLPMeEy
 
 #python setup.py sdist bdist_wheel
 
 #pip show twine
 #dir /s twine.exe
-#twine upload dist/*
 
+
+#twine upload dist/*
 #twine upload *
 
 ##### ERRATA #####
```

