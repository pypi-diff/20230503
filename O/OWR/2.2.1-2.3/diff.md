# Comparing `tmp/OWR-2.2.1.tar.gz` & `tmp/OWR-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OWR-2.2.1.tar", last modified: Wed May  3 18:00:34 2023, max compression
+gzip compressed data, was "OWR-2.3.tar", last modified: Wed May  3 18:01:39 2023, max compression
```

## Comparing `OWR-2.2.1.tar` & `OWR-2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 18:00:34.663567 OWR-2.2.1/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-2.2.1/LICENSE
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 18:00:34.663567 OWR-2.2.1/OWR/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6921 2023-05-03 16:39:31.000000 OWR-2.2.1/OWR/__init__.py
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 18:00:34.663567 OWR-2.2.1/OWR/data/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     2719 2023-05-03 17:59:31.000000 OWR-2.2.1/OWR/data/obscenity_words.json
-drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 18:00:34.663567 OWR-2.2.1/OWR.egg-info/
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      278 2023-05-03 18:00:34.000000 OWR-2.2.1/OWR.egg-info/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-03 18:00:34.000000 OWR-2.2.1/OWR.egg-info/SOURCES.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-03 18:00:34.000000 OWR-2.2.1/OWR.egg-info/dependency_links.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-03 18:00:34.000000 OWR-2.2.1/OWR.egg-info/requires.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-03 18:00:34.000000 OWR-2.2.1/OWR.egg-info/top_level.txt
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      278 2023-05-03 18:00:34.663567 OWR-2.2.1/PKG-INFO
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-2.2.1/README.md
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-03 18:00:34.663567 OWR-2.2.1/setup.cfg
--rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      719 2023-05-03 18:00:21.000000 OWR-2.2.1/setup.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 18:01:39.416102 OWR-2.3/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)    35149 2023-05-01 12:22:39.000000 OWR-2.3/LICENSE
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 18:01:39.416102 OWR-2.3/OWR/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     6921 2023-05-03 16:39:31.000000 OWR-2.3/OWR/__init__.py
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 18:01:39.416102 OWR-2.3/OWR/data/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)     2719 2023-05-03 17:59:31.000000 OWR-2.3/OWR/data/obscenity_words.json
+drwxrwxr-x   0 vladislav  (1000) vladislav  (1000)        0 2023-05-03 18:01:39.416102 OWR-2.3/OWR.egg-info/
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-03 18:01:39.000000 OWR-2.3/OWR.egg-info/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      206 2023-05-03 18:01:39.000000 OWR-2.3/OWR.egg-info/SOURCES.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        1 2023-05-03 18:01:39.000000 OWR-2.3/OWR.egg-info/dependency_links.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       87 2023-05-03 18:01:39.000000 OWR-2.3/OWR.egg-info/requires.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)        4 2023-05-03 18:01:39.000000 OWR-2.3/OWR.egg-info/top_level.txt
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      276 2023-05-03 18:01:39.416102 OWR-2.3/PKG-INFO
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       75 2023-05-01 12:22:39.000000 OWR-2.3/README.md
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)       38 2023-05-03 18:01:39.416102 OWR-2.3/setup.cfg
+-rw-rw-r--   0 vladislav  (1000) vladislav  (1000)      717 2023-05-03 18:01:33.000000 OWR-2.3/setup.py
```

### Comparing `OWR-2.2.1/LICENSE` & `OWR-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `OWR-2.2.1/OWR/__init__.py` & `OWR-2.3/OWR/__init__.py`

 * *Files identical despite different names*

### Comparing `OWR-2.2.1/OWR/data/obscenity_words.json` & `OWR-2.3/OWR/data/obscenity_words.json`

 * *Files identical despite different names*

### Comparing `OWR-2.2.1/setup.py` & `OWR-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='OWR',
-    version='2.2.1',
+    version='2.3',
     description='Obscene word recognition package',
     url='https://github.com/VladVslv/OWR',
     author='Vlad Vasilev',
     author_email='vpvasilev.work@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['OWR'],
     package_data={'': ['data/obscenity_words.json']},
```

