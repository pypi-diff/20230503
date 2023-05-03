# Comparing `tmp/pitchtools-1.9.2.tar.gz` & `tmp/pitchtools-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pitchtools-1.9.2.tar", last modified: Tue Mar 14 09:00:32 2023, max compression
+gzip compressed data, was "pitchtools-1.9.3.tar", last modified: Wed May  3 13:03:42 2023, max compression
```

## Comparing `pitchtools-1.9.2.tar` & `pitchtools-1.9.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-03-14 09:00:32.510439 pitchtools-1.9.2/
--rw-rw-r--   0 em        (1000) em        (1000)     2877 2023-03-14 09:00:32.510439 pitchtools-1.9.2/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     2561 2022-09-18 11:05:23.000000 pitchtools-1.9.2/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-03-14 09:00:32.510439 pitchtools-1.9.2/pitchtools.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     2877 2023-03-14 09:00:32.000000 pitchtools-1.9.2/pitchtools.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      169 2023-03-14 09:00:32.000000 pitchtools-1.9.2/pitchtools.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-03-14 09:00:32.000000 pitchtools-1.9.2/pitchtools.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       11 2023-03-14 09:00:32.000000 pitchtools-1.9.2/pitchtools.egg-info/top_level.txt
--rwxrwxr-x   0 em        (1000) em        (1000)    57711 2023-03-14 08:58:13.000000 pitchtools-1.9.2/pitchtools.py
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-03-14 09:00:32.510439 pitchtools-1.9.2/setup.cfg
--rwxrwxr-x   0 em        (1000) em        (1000)      536 2023-03-14 08:58:28.000000 pitchtools-1.9.2/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-03 13:03:42.291076 pitchtools-1.9.3/
+-rw-rw-r--   0 em        (1000) em        (1000)     2877 2023-05-03 13:03:42.290076 pitchtools-1.9.3/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     2561 2022-09-18 11:05:23.000000 pitchtools-1.9.3/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-03 13:03:42.290076 pitchtools-1.9.3/pitchtools/
+-rwxrwxr-x   0 em        (1000) em        (1000)    57711 2023-03-15 23:13:35.000000 pitchtools-1.9.3/pitchtools/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)        0 2021-11-25 01:40:16.000000 pitchtools-1.9.3/pitchtools/py.typed
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-03 13:03:42.290076 pitchtools-1.9.3/pitchtools.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     2877 2023-05-03 13:03:42.000000 pitchtools-1.9.3/pitchtools.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      198 2023-05-03 13:03:42.000000 pitchtools-1.9.3/pitchtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-05-03 13:03:42.000000 pitchtools-1.9.3/pitchtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       11 2023-05-03 13:03:42.000000 pitchtools-1.9.3/pitchtools.egg-info/top_level.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-05-03 13:03:42.291076 pitchtools-1.9.3/setup.cfg
+-rwxrwxr-x   0 em        (1000) em        (1000)      583 2023-05-03 13:03:30.000000 pitchtools-1.9.3/setup.py
```

### Comparing `pitchtools-1.9.2/PKG-INFO` & `pitchtools-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pitchtools
-Version: 1.9.2
+Version: 1.9.3
 Summary: Utilities to convert between midinotes, frequency and notenames
 Home-page: https://github.com/gesellkammer/pitchtools
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
```

### Comparing `pitchtools-1.9.2/README.rst` & `pitchtools-1.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `pitchtools-1.9.2/pitchtools.egg-info/PKG-INFO` & `pitchtools-1.9.3/pitchtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pitchtools
-Version: 1.9.2
+Version: 1.9.3
 Summary: Utilities to convert between midinotes, frequency and notenames
 Home-page: https://github.com/gesellkammer/pitchtools
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
```

### Comparing `pitchtools-1.9.2/pitchtools.py` & `pitchtools-1.9.3/pitchtools/__init__.py`

 * *Files identical despite different names*

