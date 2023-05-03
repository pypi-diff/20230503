# Comparing `tmp/polymatica_api-0.0.8.tar.gz` & `tmp/polymatica_api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymatica_api-0.0.8.tar", last modified: Wed May  3 13:17:38 2023, max compression
+gzip compressed data, was "polymatica_api-0.0.9.tar", last modified: Wed May  3 13:20:10 2023, max compression
```

## Comparing `polymatica_api-0.0.8.tar` & `polymatica_api-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 13:17:38.190461 polymatica_api-0.0.8/
--rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.0.8/LICENSE
--rw-r--r--   0 leggnom    (501) staff       (20)      870 2023-05-03 13:17:38.190294 polymatica_api-0.0.8/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      677 2023-05-03 07:03:34.000000 polymatica_api-0.0.8/README.md
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 13:17:38.188931 polymatica_api-0.0.8/polymatica_api/
--rw-r--r--   0 leggnom    (501) staff       (20)     1573 2023-05-03 06:42:47.000000 polymatica_api-0.0.8/polymatica_api/__init__.py
--rw-r--r--   0 leggnom    (501) staff       (20)      320 2023-05-03 06:52:44.000000 polymatica_api-0.0.8/polymatica_api/data.py
--rw-r--r--   0 leggnom    (501) staff       (20)     3899 2023-05-03 13:16:57.000000 polymatica_api-0.0.8/polymatica_api/data_option.py
--rw-r--r--   0 leggnom    (501) staff       (20)     1258 2023-05-03 06:46:48.000000 polymatica_api-0.0.8/polymatica_api/types.py
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 13:17:38.190060 polymatica_api-0.0.8/polymatica_api.egg-info/
--rw-r--r--   0 leggnom    (501) staff       (20)      870 2023-05-03 13:17:38.000000 polymatica_api-0.0.8/polymatica_api.egg-info/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      319 2023-05-03 13:17:38.000000 polymatica_api-0.0.8/polymatica_api.egg-info/SOURCES.txt
--rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-03 13:17:38.000000 polymatica_api-0.0.8/polymatica_api.egg-info/dependency_links.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-03 13:17:38.000000 polymatica_api-0.0.8/polymatica_api.egg-info/requires.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-03 13:17:38.000000 polymatica_api-0.0.8/polymatica_api.egg-info/top_level.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-03 13:17:38.190521 polymatica_api-0.0.8/setup.cfg
--rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-03 13:16:57.000000 polymatica_api-0.0.8/setup.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 13:20:10.833235 polymatica_api-0.0.9/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.0.9/LICENSE
+-rw-r--r--   0 leggnom    (501) staff       (20)      870 2023-05-03 13:20:10.833053 polymatica_api-0.0.9/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      677 2023-05-03 07:03:34.000000 polymatica_api-0.0.9/README.md
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 13:20:10.831435 polymatica_api-0.0.9/polymatica_api/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1573 2023-05-03 06:42:47.000000 polymatica_api-0.0.9/polymatica_api/__init__.py
+-rw-r--r--   0 leggnom    (501) staff       (20)      320 2023-05-03 06:52:44.000000 polymatica_api-0.0.9/polymatica_api/data.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     3874 2023-05-03 13:19:54.000000 polymatica_api-0.0.9/polymatica_api/data_option.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     1258 2023-05-03 06:46:48.000000 polymatica_api-0.0.9/polymatica_api/types.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 13:20:10.832755 polymatica_api-0.0.9/polymatica_api.egg-info/
+-rw-r--r--   0 leggnom    (501) staff       (20)      870 2023-05-03 13:20:10.000000 polymatica_api-0.0.9/polymatica_api.egg-info/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      319 2023-05-03 13:20:10.000000 polymatica_api-0.0.9/polymatica_api.egg-info/SOURCES.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-03 13:20:10.000000 polymatica_api-0.0.9/polymatica_api.egg-info/dependency_links.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-03 13:20:10.000000 polymatica_api-0.0.9/polymatica_api.egg-info/requires.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-03 13:20:10.000000 polymatica_api-0.0.9/polymatica_api.egg-info/top_level.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-03 13:20:10.833315 polymatica_api-0.0.9/setup.cfg
+-rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-03 13:19:54.000000 polymatica_api-0.0.9/setup.py
```

### Comparing `polymatica_api-0.0.8/LICENSE` & `polymatica_api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.8/PKG-INFO` & `polymatica_api-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymatica_api
-Version: 0.0.8
+Version: 0.0.9
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a simple example of getting data from a server Polymatica Platform
```

### Comparing `polymatica_api-0.0.8/README.md` & `polymatica_api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.8/polymatica_api/__init__.py` & `polymatica_api-0.0.9/polymatica_api/__init__.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.8/polymatica_api/data_option.py` & `polymatica_api-0.0.9/polymatica_api/data_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,15 @@
     agg_fn: DataOptionBlockAggFn
 
 
 class DataOption:
     def __init__(self, name: str, api):
         self._api = api
         self._name = name
-
         self._key = "default"
-        self._name = ""
         self._method: DataOptionMethod = DataOptionMethod.Table
         self._sort = []
         self._filters = []
         self._offset = 0
         self._limit = 1000
         self._blocks: List[_DataOptionBlock] = []
```

### Comparing `polymatica_api-0.0.8/polymatica_api/types.py` & `polymatica_api-0.0.9/polymatica_api/types.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.8/polymatica_api.egg-info/PKG-INFO` & `polymatica_api-0.0.9/polymatica_api.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymatica-api
-Version: 0.0.8
+Version: 0.0.9
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a simple example of getting data from a server Polymatica Platform
```

### Comparing `polymatica_api-0.0.8/setup.py` & `polymatica_api-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 requires = [
     "pydantic==1.10.7",
     "requests==2.29.0"
 ]
 
 setuptools.setup(
     name="polymatica_api",
-    version="0.0.8",
+    version="0.0.9",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3"
     ],
     python_requires='>=3.7',
```

