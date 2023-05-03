# Comparing `tmp/smashed-0.8.0.tar.gz` & `tmp/smashed-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smashed-0.8.0.tar", last modified: Tue Oct 18 00:07:19 2022, max compression
+gzip compressed data, was "smashed-0.9.0.tar", last modified: Tue Oct 18 00:39:28 2022, max compression
```

## Comparing `smashed-0.8.0.tar` & `smashed-0.9.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:07:19.496444 smashed-0.8.0/
--rw-r--r--   0 lucas      (502) staff       (20)    11357 2022-08-05 18:01:45.000000 smashed-0.8.0/LICENSE
--rw-r--r--   0 lucas      (502) staff       (20)     6220 2022-10-18 00:07:19.496298 smashed-0.8.0/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)     5430 2022-10-14 04:13:14.000000 smashed-0.8.0/README.md
--rw-r--r--   0 lucas      (502) staff       (20)     2512 2022-10-18 00:06:26.000000 smashed-0.8.0/pyproject.toml
--rw-r--r--   0 lucas      (502) staff       (20)       38 2022-10-18 00:07:19.496494 smashed-0.8.0/setup.cfg
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:07:19.490419 smashed-0.8.0/src/
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:07:19.491545 smashed-0.8.0/src/smashed/
--rw-r--r--   0 lucas      (502) staff       (20)      129 2022-10-14 04:13:14.000000 smashed-0.8.0/src/smashed/__init__.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:07:19.493227 smashed-0.8.0/src/smashed/base/
--rw-r--r--   0 lucas      (502) staff       (20)      235 2022-09-22 06:01:02.000000 smashed-0.8.0/src/smashed/base/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     3744 2022-10-14 23:34:17.000000 smashed-0.8.0/src/smashed/base/abstract.py
--rw-r--r--   0 lucas      (502) staff       (20)    11767 2022-10-17 15:31:04.000000 smashed-0.8.0/src/smashed/base/interfaces.py
--rw-r--r--   0 lucas      (502) staff       (20)    11180 2022-10-17 15:31:04.000000 smashed-0.8.0/src/smashed/base/mappers.py
--rw-r--r--   0 lucas      (502) staff       (20)      313 2022-10-14 23:34:17.000000 smashed-0.8.0/src/smashed/base/types.py
--rw-r--r--   0 lucas      (502) staff       (20)     3574 2022-10-14 23:34:17.000000 smashed-0.8.0/src/smashed/base/views.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:07:19.493598 smashed-0.8.0/src/smashed/interfaces/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2022-09-05 22:19:57.000000 smashed-0.8.0/src/smashed/interfaces/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)      196 2022-09-21 23:38:40.000000 smashed-0.8.0/src/smashed/interfaces/huggingface.py
--rw-r--r--   0 lucas      (502) staff       (20)      496 2022-09-21 23:38:43.000000 smashed-0.8.0/src/smashed/interfaces/simple.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:07:19.495487 smashed-0.8.0/src/smashed/mappers/
--rw-r--r--   0 lucas      (502) staff       (20)     2417 2022-10-17 21:41:06.000000 smashed-0.8.0/src/smashed/mappers/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     1996 2022-10-18 00:06:44.000000 smashed-0.8.0/src/smashed/mappers/batchers.py
--rw-r--r--   0 lucas      (502) staff       (20)    11150 2022-10-14 23:34:17.000000 smashed-0.8.0/src/smashed/mappers/cache.py
--rw-r--r--   0 lucas      (502) staff       (20)    15107 2022-10-17 23:30:19.000000 smashed-0.8.0/src/smashed/mappers/collators.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:07:19.495836 smashed-0.8.0/src/smashed/mappers/contrib/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2022-09-05 22:19:57.000000 smashed-0.8.0/src/smashed/mappers/contrib/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     2096 2022-10-17 21:41:06.000000 smashed-0.8.0/src/smashed/mappers/contrib/squad.py
--rw-r--r--   0 lucas      (502) staff       (20)     1195 2022-09-05 22:19:57.000000 smashed-0.8.0/src/smashed/mappers/contrib/sse.py
--rw-r--r--   0 lucas      (502) staff       (20)     4721 2022-10-14 23:34:17.000000 smashed-0.8.0/src/smashed/mappers/converters.py
--rw-r--r--   0 lucas      (502) staff       (20)     2033 2022-10-14 23:34:17.000000 smashed-0.8.0/src/smashed/mappers/debug.py
--rw-r--r--   0 lucas      (502) staff       (20)     4101 2022-10-14 04:13:14.000000 smashed-0.8.0/src/smashed/mappers/fields.py
--rw-r--r--   0 lucas      (502) staff       (20)     2440 2022-10-17 03:28:14.000000 smashed-0.8.0/src/smashed/mappers/filters.py
--rw-r--r--   0 lucas      (502) staff       (20)     5923 2022-09-22 06:01:02.000000 smashed-0.8.0/src/smashed/mappers/loaders.py
--rw-r--r--   0 lucas      (502) staff       (20)    19569 2022-10-18 00:06:45.000000 smashed-0.8.0/src/smashed/mappers/multiseq.py
--rw-r--r--   0 lucas      (502) staff       (20)    15192 2022-10-17 15:31:04.000000 smashed-0.8.0/src/smashed/mappers/prompting.py
--rw-r--r--   0 lucas      (502) staff       (20)     8556 2022-10-18 00:06:45.000000 smashed-0.8.0/src/smashed/mappers/shape.py
--rw-r--r--   0 lucas      (502) staff       (20)     1985 2022-10-17 15:31:04.000000 smashed-0.8.0/src/smashed/mappers/text.py
--rw-r--r--   0 lucas      (502) staff       (20)    11561 2022-10-17 02:19:09.000000 smashed-0.8.0/src/smashed/mappers/tokenize.py
--rw-r--r--   0 lucas      (502) staff       (20)     7594 2022-10-17 04:25:47.000000 smashed-0.8.0/src/smashed/mappers/types.py
--rw-r--r--   0 lucas      (502) staff       (20)        0 2022-09-05 22:19:57.000000 smashed-0.8.0/src/smashed/py.typed
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:07:19.496091 smashed-0.8.0/src/smashed/recipes/
--rw-r--r--   0 lucas      (502) staff       (20)       82 2022-10-14 04:13:14.000000 smashed-0.8.0/src/smashed/recipes/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     8369 2022-10-17 21:41:06.000000 smashed-0.8.0/src/smashed/recipes/prompting.py
--rw-r--r--   0 lucas      (502) staff       (20)     2847 2022-10-18 00:02:30.000000 smashed-0.8.0/src/smashed/utils.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:07:19.492454 smashed-0.8.0/src/smashed.egg-info/
--rw-r--r--   0 lucas      (502) staff       (20)     6220 2022-10-18 00:07:19.000000 smashed-0.8.0/src/smashed.egg-info/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)     1188 2022-10-18 00:07:19.000000 smashed-0.8.0/src/smashed.egg-info/SOURCES.txt
--rw-r--r--   0 lucas      (502) staff       (20)        1 2022-10-18 00:07:19.000000 smashed-0.8.0/src/smashed.egg-info/dependency_links.txt
--rw-r--r--   0 lucas      (502) staff       (20)      461 2022-10-18 00:07:19.000000 smashed-0.8.0/src/smashed.egg-info/requires.txt
--rw-r--r--   0 lucas      (502) staff       (20)        8 2022-10-18 00:07:19.000000 smashed-0.8.0/src/smashed.egg-info/top_level.txt
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:39:28.824943 smashed-0.9.0/
+-rw-r--r--   0 lucas      (502) staff       (20)    11357 2022-08-05 18:01:45.000000 smashed-0.9.0/LICENSE
+-rw-r--r--   0 lucas      (502) staff       (20)     6220 2022-10-18 00:39:28.824789 smashed-0.9.0/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     5430 2022-10-14 04:13:14.000000 smashed-0.9.0/README.md
+-rw-r--r--   0 lucas      (502) staff       (20)     2512 2022-10-18 00:38:51.000000 smashed-0.9.0/pyproject.toml
+-rw-r--r--   0 lucas      (502) staff       (20)       38 2022-10-18 00:39:28.824997 smashed-0.9.0/setup.cfg
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:39:28.812258 smashed-0.9.0/src/
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:39:28.814223 smashed-0.9.0/src/smashed/
+-rw-r--r--   0 lucas      (502) staff       (20)      129 2022-10-14 04:13:14.000000 smashed-0.9.0/src/smashed/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:39:28.817016 smashed-0.9.0/src/smashed/base/
+-rw-r--r--   0 lucas      (502) staff       (20)      235 2022-09-22 06:01:02.000000 smashed-0.9.0/src/smashed/base/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3744 2022-10-14 23:34:17.000000 smashed-0.9.0/src/smashed/base/abstract.py
+-rw-r--r--   0 lucas      (502) staff       (20)    11767 2022-10-17 15:31:04.000000 smashed-0.9.0/src/smashed/base/interfaces.py
+-rw-r--r--   0 lucas      (502) staff       (20)    11180 2022-10-17 15:31:04.000000 smashed-0.9.0/src/smashed/base/mappers.py
+-rw-r--r--   0 lucas      (502) staff       (20)      313 2022-10-14 23:34:17.000000 smashed-0.9.0/src/smashed/base/types.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3574 2022-10-14 23:34:17.000000 smashed-0.9.0/src/smashed/base/views.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:39:28.817678 smashed-0.9.0/src/smashed/interfaces/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2022-09-05 22:19:57.000000 smashed-0.9.0/src/smashed/interfaces/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)      196 2022-09-21 23:38:40.000000 smashed-0.9.0/src/smashed/interfaces/huggingface.py
+-rw-r--r--   0 lucas      (502) staff       (20)      496 2022-09-21 23:38:43.000000 smashed-0.9.0/src/smashed/interfaces/simple.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:39:28.823088 smashed-0.9.0/src/smashed/mappers/
+-rw-r--r--   0 lucas      (502) staff       (20)     2417 2022-10-17 21:41:06.000000 smashed-0.9.0/src/smashed/mappers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1996 2022-10-18 00:06:44.000000 smashed-0.9.0/src/smashed/mappers/batchers.py
+-rw-r--r--   0 lucas      (502) staff       (20)    11150 2022-10-14 23:34:17.000000 smashed-0.9.0/src/smashed/mappers/cache.py
+-rw-r--r--   0 lucas      (502) staff       (20)    15107 2022-10-17 23:30:19.000000 smashed-0.9.0/src/smashed/mappers/collators.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:39:28.823840 smashed-0.9.0/src/smashed/mappers/contrib/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2022-09-05 22:19:57.000000 smashed-0.9.0/src/smashed/mappers/contrib/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2614 2022-10-18 00:38:57.000000 smashed-0.9.0/src/smashed/mappers/contrib/squad.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1195 2022-09-05 22:19:57.000000 smashed-0.9.0/src/smashed/mappers/contrib/sse.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4721 2022-10-14 23:34:17.000000 smashed-0.9.0/src/smashed/mappers/converters.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2033 2022-10-14 23:34:17.000000 smashed-0.9.0/src/smashed/mappers/debug.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4101 2022-10-14 04:13:14.000000 smashed-0.9.0/src/smashed/mappers/fields.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2440 2022-10-17 03:28:14.000000 smashed-0.9.0/src/smashed/mappers/filters.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5923 2022-09-22 06:01:02.000000 smashed-0.9.0/src/smashed/mappers/loaders.py
+-rw-r--r--   0 lucas      (502) staff       (20)    19569 2022-10-18 00:38:57.000000 smashed-0.9.0/src/smashed/mappers/multiseq.py
+-rw-r--r--   0 lucas      (502) staff       (20)    15192 2022-10-18 00:08:16.000000 smashed-0.9.0/src/smashed/mappers/prompting.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8556 2022-10-18 00:38:57.000000 smashed-0.9.0/src/smashed/mappers/shape.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1985 2022-10-17 15:31:04.000000 smashed-0.9.0/src/smashed/mappers/text.py
+-rw-r--r--   0 lucas      (502) staff       (20)    11561 2022-10-17 02:19:09.000000 smashed-0.9.0/src/smashed/mappers/tokenize.py
+-rw-r--r--   0 lucas      (502) staff       (20)     7594 2022-10-17 04:25:47.000000 smashed-0.9.0/src/smashed/mappers/types.py
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2022-09-05 22:19:57.000000 smashed-0.9.0/src/smashed/py.typed
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:39:28.824559 smashed-0.9.0/src/smashed/recipes/
+-rw-r--r--   0 lucas      (502) staff       (20)       82 2022-10-14 04:13:14.000000 smashed-0.9.0/src/smashed/recipes/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8561 2022-10-18 00:38:57.000000 smashed-0.9.0/src/smashed/recipes/prompting.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2847 2022-10-18 00:02:30.000000 smashed-0.9.0/src/smashed/utils.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-10-18 00:39:28.815137 smashed-0.9.0/src/smashed.egg-info/
+-rw-r--r--   0 lucas      (502) staff       (20)     6220 2022-10-18 00:39:28.000000 smashed-0.9.0/src/smashed.egg-info/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     1188 2022-10-18 00:39:28.000000 smashed-0.9.0/src/smashed.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        1 2022-10-18 00:39:28.000000 smashed-0.9.0/src/smashed.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas      (502) staff       (20)      461 2022-10-18 00:39:28.000000 smashed-0.9.0/src/smashed.egg-info/requires.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        8 2022-10-18 00:39:28.000000 smashed-0.9.0/src/smashed.egg-info/top_level.txt
```

### Comparing `smashed-0.8.0/LICENSE` & `smashed-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/PKG-INFO` & `smashed-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smashed
-Version: 0.8.0
+Version: 0.9.0
 Summary: Sequential MAppers for Sequences of HEterogeneous Dictionaries is a set of Python interfaces designed to apply transformations to samples in datasets, which are often implemented as sequences of dictionaries.
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/allenai/smashed
 Project-URL: Repository, https://github.com/allenai/smashed
 Project-URL: Bug Tracker, https://github.com/allenai/smashed/issues
 Requires-Python: >=3.8
```

### Comparing `smashed-0.8.0/README.md` & `smashed-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/pyproject.toml` & `smashed-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "smashed"
-version = "0.8.0"
+version = "0.9.0"
 description = "Sequential MAppers for Sequences of HEterogeneous Dictionaries is a set of Python interfaces designed to apply transformations to samples in datasets, which are often implemented as sequences of dictionaries."
 authors = [
     {name = "Allen Institute for Artificial Intelligence", email = "contact@allenai.org" },
     {name = "Luca Soldaini", email = "luca@soldaini.net"}
 ]
 license = {text = "Apache-2.0"}
 readme = "README.md"
```

### Comparing `smashed-0.8.0/src/smashed/base/abstract.py` & `smashed-0.9.0/src/smashed/base/abstract.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/base/interfaces.py` & `smashed-0.9.0/src/smashed/base/interfaces.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/base/mappers.py` & `smashed-0.9.0/src/smashed/base/mappers.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/base/views.py` & `smashed-0.9.0/src/smashed/base/views.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/__init__.py` & `smashed-0.9.0/src/smashed/mappers/__init__.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/batchers.py` & `smashed-0.9.0/src/smashed/mappers/batchers.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/cache.py` & `smashed-0.9.0/src/smashed/mappers/cache.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/collators.py` & `smashed-0.9.0/src/smashed/mappers/collators.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/contrib/sse.py` & `smashed-0.9.0/src/smashed/mappers/contrib/sse.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/converters.py` & `smashed-0.9.0/src/smashed/mappers/converters.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/debug.py` & `smashed-0.9.0/src/smashed/mappers/debug.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/fields.py` & `smashed-0.9.0/src/smashed/mappers/fields.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/filters.py` & `smashed-0.9.0/src/smashed/mappers/filters.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/loaders.py` & `smashed-0.9.0/src/smashed/mappers/loaders.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/multiseq.py` & `smashed-0.9.0/src/smashed/mappers/multiseq.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/prompting.py` & `smashed-0.9.0/src/smashed/mappers/prompting.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/shape.py` & `smashed-0.9.0/src/smashed/mappers/shape.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/text.py` & `smashed-0.9.0/src/smashed/mappers/text.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/tokenize.py` & `smashed-0.9.0/src/smashed/mappers/tokenize.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/mappers/types.py` & `smashed-0.9.0/src/smashed/mappers/types.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed/recipes/prompting.py` & `smashed-0.9.0/src/smashed/recipes/prompting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, Optional, Sequence, Union
+from typing import Dict, List, Literal, Optional, Sequence, Union
 
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
 from ..mappers.fields import RenameFieldsMapper
 from ..mappers.prompting import (
     EncodeFieldsMapper,
     FillEncodedPromptMapper,
@@ -36,20 +36,24 @@
         ] = "labels",
         is_split_into_words: bool = False,
         max_source_length: Optional[int] = None,
         max_target_length: Optional[int] = None,
         strategy: Union[Literal["longest"], Literal["uniform"]] = "longest",
         return_attention_mask: bool = True,
         return_token_type_ids: bool = False,
-        extra_keep_fields: Optional[Sequence[str]] = None,
+        extra_keep_field_names: Union[None, List[str], Dict[str, str]] = None,
         extra_encode_fields: Optional[Sequence[str]] = None,
     ):
         fields_to_truncate = fields_to_truncate or []
         fields_to_stride = fields_to_stride or []
-        extra_keep_fields = extra_keep_fields or []
+
+        extra_keep_field_names = extra_keep_field_names or []
+        if isinstance(extra_keep_field_names, list):
+            extra_keep_field_names = {f: f for f in extra_keep_field_names}
+
         extra_encode_fields = extra_encode_fields or []
 
         source_prompt_mapper = FillEncodedPromptMapper(
             template=source_template,
             tokenizer=tokenizer,
             output_prefix=None,
             add_bos_token=source_add_bos_token,
@@ -114,17 +118,16 @@
         # filler for the input.
         self.chain(source_prompt_mapper)
 
         # we need to rename some fields to make sure there is no conflict
         # between the source and target prompts; further this will eliminate
         # all fields that are not needed for this recipe.
         rename_fields_map = {
-            k: k
-            for k in source_prompt_mapper.output_fields
-            + tuple(extra_keep_fields)
+            **{k: k for k in source_prompt_mapper.output_fields},
+            **{k: v for k, v in extra_keep_field_names.items()},
         }
 
         if target_prompt_mapper:
 
             # we add the target prompt template filler to the chain in case
             # we have a target template
             self.chain(target_prompt_mapper)
```

### Comparing `smashed-0.8.0/src/smashed/utils.py` & `smashed-0.9.0/src/smashed/utils.py`

 * *Files identical despite different names*

### Comparing `smashed-0.8.0/src/smashed.egg-info/PKG-INFO` & `smashed-0.9.0/src/smashed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smashed
-Version: 0.8.0
+Version: 0.9.0
 Summary: Sequential MAppers for Sequences of HEterogeneous Dictionaries is a set of Python interfaces designed to apply transformations to samples in datasets, which are often implemented as sequences of dictionaries.
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>, Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/allenai/smashed
 Project-URL: Repository, https://github.com/allenai/smashed
 Project-URL: Bug Tracker, https://github.com/allenai/smashed/issues
 Requires-Python: >=3.8
```

### Comparing `smashed-0.8.0/src/smashed.egg-info/SOURCES.txt` & `smashed-0.9.0/src/smashed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

