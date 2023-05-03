# Comparing `tmp/dscustom-libs-0.1.tar.gz` & `tmp/dscustom-libs-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscustom-libs-0.1.tar", last modified: Mon May  1 17:58:55 2023, max compression
+gzip compressed data, was "dscustom-libs-0.2.tar", last modified: Wed May  3 01:10:51 2023, max compression
```

## Comparing `dscustom-libs-0.1.tar` & `dscustom-libs-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 17:58:55.368256 dscustom-libs-0.1/
--rw-rw-rw-   0        0        0     1103 2023-05-01 17:08:16.000000 dscustom-libs-0.1/LICENSE
--rw-rw-rw-   0        0        0      288 2023-05-01 17:58:55.368256 dscustom-libs-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       92 2023-05-01 17:08:16.000000 dscustom-libs-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 17:58:55.273205 dscustom-libs-0.1/TSDataProcessing/
--rw-rw-rw-   0        0        0     5018 2023-05-01 17:55:37.000000 dscustom-libs-0.1/TSDataProcessing/TSDataProcessing.py
-drwxrwxrwx   0        0        0        0 2023-05-01 17:58:55.316625 dscustom-libs-0.1/TSFeatures/
--rw-rw-rw-   0        0        0    10799 2023-05-01 17:55:37.000000 dscustom-libs-0.1/TSFeatures/TSFeatures.py
-drwxrwxrwx   0        0        0        0 2023-05-01 17:58:55.368256 dscustom-libs-0.1/dscustom_libs.egg-info/
--rw-rw-rw-   0        0        0      288 2023-05-01 17:58:55.000000 dscustom-libs-0.1/dscustom_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-05-01 17:58:55.000000 dscustom-libs-0.1/dscustom_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 17:58:55.000000 dscustom-libs-0.1/dscustom_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 17:58:55.000000 dscustom-libs-0.1/dscustom_libs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-05-01 17:58:55.000000 dscustom-libs-0.1/dscustom_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 17:58:55.368256 dscustom-libs-0.1/setup.cfg
--rw-rw-rw-   0        0        0      610 2023-05-01 17:56:37.000000 dscustom-libs-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:10:51.888709 dscustom-libs-0.2/
+-rw-rw-rw-   0        0        0     1103 2023-05-01 17:08:16.000000 dscustom-libs-0.2/LICENSE
+-rw-rw-rw-   0        0        0      288 2023-05-03 01:10:51.888709 dscustom-libs-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2023-05-01 17:08:16.000000 dscustom-libs-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 01:10:51.870145 dscustom-libs-0.2/TSDataProcessing/
+-rw-rw-rw-   0        0        0     5018 2023-05-01 17:55:37.000000 dscustom-libs-0.2/TSDataProcessing/TSDataProcessing.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:10:51.876202 dscustom-libs-0.2/TSFeatures/
+-rw-rw-rw-   0        0        0    10799 2023-05-03 01:06:53.000000 dscustom-libs-0.2/TSFeatures/TSFeatures.py
+drwxrwxrwx   0        0        0        0 2023-05-03 01:10:51.887228 dscustom-libs-0.2/dscustom_libs.egg-info/
+-rw-rw-rw-   0        0        0      288 2023-05-03 01:10:51.000000 dscustom-libs-0.2/dscustom_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-05-03 01:10:51.000000 dscustom-libs-0.2/dscustom_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 01:10:51.000000 dscustom-libs-0.2/dscustom_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 17:58:55.000000 dscustom-libs-0.2/dscustom_libs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-05-03 01:10:51.000000 dscustom-libs-0.2/dscustom_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 01:10:51.888709 dscustom-libs-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      610 2023-05-03 01:06:57.000000 dscustom-libs-0.2/setup.py
```

### Comparing `dscustom-libs-0.1/LICENSE` & `dscustom-libs-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dscustom-libs-0.1/TSDataProcessing/TSDataProcessing.py` & `dscustom-libs-0.2/TSDataProcessing/TSDataProcessing.py`

 * *Files identical despite different names*

### Comparing `dscustom-libs-0.1/TSFeatures/TSFeatures.py` & `dscustom-libs-0.2/TSFeatures/TSFeatures.py`

 * *Files identical despite different names*

### Comparing `dscustom-libs-0.1/setup.py` & `dscustom-libs-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # (C) Copyright IBM Corporation 2019, 2020, 2021, 2022
 # U.S. Government Users Restricted Rights:  Use, duplication or disclosure restricted
 # by GSA ADP Schedule Contract with IBM Corp.
 
 from setuptools import setup
 
 setup(name='dscustom-libs',
-      version='0.1',
+      version='0.2',
       description='Often used functions in Digital Smelter project',
       url='https://github.com/luisgustavob78/dscustom-libs',
       author='Luis Gustavo Silva Barros',
       author_email='luisgustavob78@gmail.com',
       license='MIT',
       packages=['TSDataProcessing',
                 'TSFeatures'],
```

