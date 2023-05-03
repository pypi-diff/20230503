# Comparing `tmp/AshenDB-0.0.4.tar.gz` & `tmp/AshenDB-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshenDB-0.0.4.tar", last modified: Wed May  3 01:48:01 2023, max compression
+gzip compressed data, was "AshenDB-0.0.5.tar", last modified: Wed May  3 10:06:17 2023, max compression
```

## Comparing `AshenDB-0.0.4.tar` & `AshenDB-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-05-03 01:48:01.262858 AshenDB-0.0.4/
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-05-03 01:48:01.261859 AshenDB-0.0.4/AshenDB.egg-info/
--rw-r--r--   0 aurka     (1000) aurka     (1000)     2248 2023-05-03 01:48:01.000000 AshenDB-0.0.4/AshenDB.egg-info/PKG-INFO
--rw-r--r--   0 aurka     (1000) aurka     (1000)      360 2023-05-03 01:48:01.000000 AshenDB-0.0.4/AshenDB.egg-info/SOURCES.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        1 2023-05-03 01:48:01.000000 AshenDB-0.0.4/AshenDB.egg-info/dependency_links.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)       50 2023-05-03 01:48:01.000000 AshenDB-0.0.4/AshenDB.egg-info/entry_points.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        9 2023-05-03 01:48:01.000000 AshenDB-0.0.4/AshenDB.egg-info/requires.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        8 2023-05-03 01:48:01.000000 AshenDB-0.0.4/AshenDB.egg-info/top_level.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)     1065 2023-04-18 23:23:36.000000 AshenDB-0.0.4/LICENSE
--rw-r--r--   0 aurka     (1000) aurka     (1000)     2248 2023-05-03 01:48:01.262858 AshenDB-0.0.4/PKG-INFO
--rw-r--r--   0 aurka     (1000) aurka     (1000)      300 2023-04-23 07:22:33.000000 AshenDB-0.0.4/README.rst
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-05-03 01:48:01.262858 AshenDB-0.0.4/ashendb/
--rw-r--r--   0 aurka     (1000) aurka     (1000)      786 2023-04-26 01:59:48.000000 AshenDB-0.0.4/ashendb/__init__.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     6886 2023-04-29 23:18:14.000000 AshenDB-0.0.4/ashendb/client.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     9216 2023-05-03 01:37:15.000000 AshenDB-0.0.4/ashendb/collection.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     7751 2023-04-29 23:18:41.000000 AshenDB-0.0.4/ashendb/database.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     1257 2023-05-03 00:01:33.000000 AshenDB-0.0.4/ashendb/document.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)      128 2023-04-23 19:49:22.000000 AshenDB-0.0.4/ashendb/exception.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     7961 2023-05-03 01:30:12.000000 AshenDB-0.0.4/ashendb/helper.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)      906 2023-05-03 01:26:30.000000 AshenDB-0.0.4/pyproject.toml
--rw-r--r--   0 aurka     (1000) aurka     (1000)       38 2023-05-03 01:48:01.262858 AshenDB-0.0.4/setup.cfg
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-05-03 10:06:17.056774 AshenDB-0.0.5/
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-05-03 10:06:17.055774 AshenDB-0.0.5/AshenDB.egg-info/
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     4028 2023-05-03 10:06:17.000000 AshenDB-0.0.5/AshenDB.egg-info/PKG-INFO
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      360 2023-05-03 10:06:17.000000 AshenDB-0.0.5/AshenDB.egg-info/SOURCES.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        1 2023-05-03 10:06:17.000000 AshenDB-0.0.5/AshenDB.egg-info/dependency_links.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)       50 2023-05-03 10:06:17.000000 AshenDB-0.0.5/AshenDB.egg-info/entry_points.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        9 2023-05-03 10:06:17.000000 AshenDB-0.0.5/AshenDB.egg-info/requires.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        8 2023-05-03 10:06:17.000000 AshenDB-0.0.5/AshenDB.egg-info/top_level.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     1065 2023-04-18 23:23:36.000000 AshenDB-0.0.5/LICENSE
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     4028 2023-05-03 10:06:17.056774 AshenDB-0.0.5/PKG-INFO
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     2080 2023-05-03 08:58:55.000000 AshenDB-0.0.5/README.rst
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-05-03 10:06:17.056774 AshenDB-0.0.5/ashendb/
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      786 2023-04-26 01:59:48.000000 AshenDB-0.0.5/ashendb/__init__.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     6886 2023-04-29 23:18:14.000000 AshenDB-0.0.5/ashendb/client.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     9216 2023-05-03 01:37:15.000000 AshenDB-0.0.5/ashendb/collection.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     7751 2023-04-29 23:18:41.000000 AshenDB-0.0.5/ashendb/database.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     1257 2023-05-03 00:01:33.000000 AshenDB-0.0.5/ashendb/document.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      128 2023-04-23 19:49:22.000000 AshenDB-0.0.5/ashendb/exception.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)    10256 2023-05-03 10:05:21.000000 AshenDB-0.0.5/ashendb/helper.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      906 2023-05-03 10:02:22.000000 AshenDB-0.0.5/pyproject.toml
+-rw-r--r--   0 aurka     (1000) aurka     (1000)       38 2023-05-03 10:06:17.056774 AshenDB-0.0.5/setup.cfg
```

### Comparing `AshenDB-0.0.4/LICENSE` & `AshenDB-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.4/ashendb/__init__.py` & `AshenDB-0.0.5/ashendb/__init__.py`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.4/ashendb/client.py` & `AshenDB-0.0.5/ashendb/client.py`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.4/ashendb/collection.py` & `AshenDB-0.0.5/ashendb/collection.py`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.4/ashendb/database.py` & `AshenDB-0.0.5/ashendb/database.py`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.4/ashendb/document.py` & `AshenDB-0.0.5/ashendb/document.py`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.4/pyproject.toml` & `AshenDB-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AshenDB"
-version = "0.0.4"
+version = "0.0.5"
 description = "Another stupid library for using json as Database"
 readme = "README.rst"
 authors = [{name = "Abdullah Al Muaz", email = "abdullahalmuaz15@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 1 - Planning",
     "License :: OSI Approved :: MIT License",
```

