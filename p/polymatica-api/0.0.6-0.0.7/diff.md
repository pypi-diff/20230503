# Comparing `tmp/polymatica_api-0.0.6.tar.gz` & `tmp/polymatica_api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymatica_api-0.0.6.tar", last modified: Wed May  3 06:53:32 2023, max compression
+gzip compressed data, was "polymatica_api-0.0.7.tar", last modified: Wed May  3 07:09:37 2023, max compression
```

## Comparing `polymatica_api-0.0.6.tar` & `polymatica_api-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 06:53:32.711191 polymatica_api-0.0.6/
--rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.0.6/LICENSE
--rw-r--r--   0 leggnom    (501) staff       (20)      890 2023-05-03 06:53:32.711004 polymatica_api-0.0.6/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      697 2023-05-03 06:50:59.000000 polymatica_api-0.0.6/README.md
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 06:53:32.709759 polymatica_api-0.0.6/polymatica_api/
--rw-r--r--   0 leggnom    (501) staff       (20)     1573 2023-05-03 06:42:47.000000 polymatica_api-0.0.6/polymatica_api/__init__.py
--rw-r--r--   0 leggnom    (501) staff       (20)      320 2023-05-03 06:52:44.000000 polymatica_api-0.0.6/polymatica_api/data.py
--rw-r--r--   0 leggnom    (501) staff       (20)     3864 2023-05-02 01:33:28.000000 polymatica_api-0.0.6/polymatica_api/data_option.py
--rw-r--r--   0 leggnom    (501) staff       (20)     1258 2023-05-03 06:46:48.000000 polymatica_api-0.0.6/polymatica_api/types.py
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 06:53:32.710758 polymatica_api-0.0.6/polymatica_api.egg-info/
--rw-r--r--   0 leggnom    (501) staff       (20)      890 2023-05-03 06:53:32.000000 polymatica_api-0.0.6/polymatica_api.egg-info/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      319 2023-05-03 06:53:32.000000 polymatica_api-0.0.6/polymatica_api.egg-info/SOURCES.txt
--rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-03 06:53:32.000000 polymatica_api-0.0.6/polymatica_api.egg-info/dependency_links.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-03 06:53:32.000000 polymatica_api-0.0.6/polymatica_api.egg-info/requires.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-03 06:53:32.000000 polymatica_api-0.0.6/polymatica_api.egg-info/top_level.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-03 06:53:32.711257 polymatica_api-0.0.6/setup.cfg
--rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-03 06:53:21.000000 polymatica_api-0.0.6/setup.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 07:09:37.458497 polymatica_api-0.0.7/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.0.7/LICENSE
+-rw-r--r--   0 leggnom    (501) staff       (20)      870 2023-05-03 07:09:37.458295 polymatica_api-0.0.7/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      677 2023-05-03 07:03:34.000000 polymatica_api-0.0.7/README.md
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 07:09:37.456890 polymatica_api-0.0.7/polymatica_api/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1573 2023-05-03 06:42:47.000000 polymatica_api-0.0.7/polymatica_api/__init__.py
+-rw-r--r--   0 leggnom    (501) staff       (20)      320 2023-05-03 06:52:44.000000 polymatica_api-0.0.7/polymatica_api/data.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     3864 2023-05-02 01:33:28.000000 polymatica_api-0.0.7/polymatica_api/data_option.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     1258 2023-05-03 06:46:48.000000 polymatica_api-0.0.7/polymatica_api/types.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 07:09:37.458006 polymatica_api-0.0.7/polymatica_api.egg-info/
+-rw-r--r--   0 leggnom    (501) staff       (20)      870 2023-05-03 07:09:37.000000 polymatica_api-0.0.7/polymatica_api.egg-info/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      319 2023-05-03 07:09:37.000000 polymatica_api-0.0.7/polymatica_api.egg-info/SOURCES.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-03 07:09:37.000000 polymatica_api-0.0.7/polymatica_api.egg-info/dependency_links.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-03 07:09:37.000000 polymatica_api-0.0.7/polymatica_api.egg-info/requires.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-03 07:09:37.000000 polymatica_api-0.0.7/polymatica_api.egg-info/top_level.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-03 07:09:37.458556 polymatica_api-0.0.7/setup.cfg
+-rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-03 07:09:31.000000 polymatica_api-0.0.7/setup.py
```

### Comparing `polymatica_api-0.0.6/LICENSE` & `polymatica_api-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.6/PKG-INFO` & `polymatica_api-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymatica_api
-Version: 0.0.6
+Version: 0.0.7
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a simple example of getting data from a server Polymatica Platform
 
@@ -24,13 +24,12 @@
         '2010 Population', 
         '2015 Population',
         '2020 Population',
         '2022 Population',
     )
 ])
 
-
-with response.get('default') as data:
-    frame = pd.DataFrame(data.rows)
-    frame.rename(columns=data.column_map, inplace=True)
-    print(frame)
+data = response.get('default')
+frame = pd.DataFrame(data.rows)
+frame.rename(columns=data.column_map, inplace=True)
+print(frame)
 ```
```

### Comparing `polymatica_api-0.0.6/README.md` & `polymatica_api-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,13 +16,12 @@
         '2010 Population', 
         '2015 Population',
         '2020 Population',
         '2022 Population',
     )
 ])
 
-
-with response.get('default') as data:
-    frame = pd.DataFrame(data.rows)
-    frame.rename(columns=data.column_map, inplace=True)
-    print(frame)
+data = response.get('default')
+frame = pd.DataFrame(data.rows)
+frame.rename(columns=data.column_map, inplace=True)
+print(frame)
 ```
```

### Comparing `polymatica_api-0.0.6/polymatica_api/__init__.py` & `polymatica_api-0.0.7/polymatica_api/__init__.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.6/polymatica_api/data_option.py` & `polymatica_api-0.0.7/polymatica_api/data_option.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.6/polymatica_api/types.py` & `polymatica_api-0.0.7/polymatica_api/types.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.6/polymatica_api.egg-info/PKG-INFO` & `polymatica_api-0.0.7/polymatica_api.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymatica-api
-Version: 0.0.6
+Version: 0.0.7
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a simple example of getting data from a server Polymatica Platform
 
@@ -24,13 +24,12 @@
         '2010 Population', 
         '2015 Population',
         '2020 Population',
         '2022 Population',
     )
 ])
 
-
-with response.get('default') as data:
-    frame = pd.DataFrame(data.rows)
-    frame.rename(columns=data.column_map, inplace=True)
-    print(frame)
+data = response.get('default')
+frame = pd.DataFrame(data.rows)
+frame.rename(columns=data.column_map, inplace=True)
+print(frame)
 ```
```

### Comparing `polymatica_api-0.0.6/setup.py` & `polymatica_api-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 requires = [
     "pydantic==1.10.7",
     "requests==2.29.0"
 ]
 
 setuptools.setup(
     name="polymatica_api",
-    version="0.0.6",
+    version="0.0.7",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3"
     ],
     python_requires='>=3.7',
```

