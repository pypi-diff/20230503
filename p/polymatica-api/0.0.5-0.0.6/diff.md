# Comparing `tmp/polymatica_api-0.0.5.tar.gz` & `tmp/polymatica_api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymatica_api-0.0.5.tar", last modified: Tue May  2 10:57:30 2023, max compression
+gzip compressed data, was "polymatica_api-0.0.6.tar", last modified: Wed May  3 06:53:32 2023, max compression
```

## Comparing `polymatica_api-0.0.5.tar` & `polymatica_api-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 10:57:30.856598 polymatica_api-0.0.5/
--rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.0.5/LICENSE
--rw-r--r--   0 leggnom    (501) staff       (20)      731 2023-05-02 10:57:30.856471 polymatica_api-0.0.5/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      538 2023-05-02 10:56:35.000000 polymatica_api-0.0.5/README.md
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 10:57:30.855290 polymatica_api-0.0.5/polymatica_api/
--rw-r--r--   0 leggnom    (501) staff       (20)     1463 2023-05-02 07:39:36.000000 polymatica_api-0.0.5/polymatica_api/__init__.py
--rw-r--r--   0 leggnom    (501) staff       (20)     3864 2023-05-02 01:33:28.000000 polymatica_api-0.0.5/polymatica_api/data_option.py
--rw-r--r--   0 leggnom    (501) staff       (20)      838 2023-05-02 07:39:25.000000 polymatica_api-0.0.5/polymatica_api/types.py
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 10:57:30.856049 polymatica_api-0.0.5/polymatica_api.egg-info/
--rw-r--r--   0 leggnom    (501) staff       (20)      731 2023-05-02 10:57:30.000000 polymatica_api-0.0.5/polymatica_api.egg-info/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      315 2023-05-02 10:57:30.000000 polymatica_api-0.0.5/polymatica_api.egg-info/SOURCES.txt
--rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-02 10:57:30.000000 polymatica_api-0.0.5/polymatica_api.egg-info/dependency_links.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-02 10:57:30.000000 polymatica_api-0.0.5/polymatica_api.egg-info/requires.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-02 10:57:30.000000 polymatica_api-0.0.5/polymatica_api.egg-info/top_level.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-02 10:57:30.856634 polymatica_api-0.0.5/setup.cfg
--rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-02 10:57:24.000000 polymatica_api-0.0.5/setup.py
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-02 10:57:30.856164 polymatica_api-0.0.5/tests/
--rw-r--r--   0 leggnom    (501) staff       (20)      508 2023-05-02 07:14:02.000000 polymatica_api-0.0.5/tests/test_base.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 06:53:32.711191 polymatica_api-0.0.6/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.0.6/LICENSE
+-rw-r--r--   0 leggnom    (501) staff       (20)      890 2023-05-03 06:53:32.711004 polymatica_api-0.0.6/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      697 2023-05-03 06:50:59.000000 polymatica_api-0.0.6/README.md
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 06:53:32.709759 polymatica_api-0.0.6/polymatica_api/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1573 2023-05-03 06:42:47.000000 polymatica_api-0.0.6/polymatica_api/__init__.py
+-rw-r--r--   0 leggnom    (501) staff       (20)      320 2023-05-03 06:52:44.000000 polymatica_api-0.0.6/polymatica_api/data.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     3864 2023-05-02 01:33:28.000000 polymatica_api-0.0.6/polymatica_api/data_option.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     1258 2023-05-03 06:46:48.000000 polymatica_api-0.0.6/polymatica_api/types.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 06:53:32.710758 polymatica_api-0.0.6/polymatica_api.egg-info/
+-rw-r--r--   0 leggnom    (501) staff       (20)      890 2023-05-03 06:53:32.000000 polymatica_api-0.0.6/polymatica_api.egg-info/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      319 2023-05-03 06:53:32.000000 polymatica_api-0.0.6/polymatica_api.egg-info/SOURCES.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-03 06:53:32.000000 polymatica_api-0.0.6/polymatica_api.egg-info/dependency_links.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-03 06:53:32.000000 polymatica_api-0.0.6/polymatica_api.egg-info/requires.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-03 06:53:32.000000 polymatica_api-0.0.6/polymatica_api.egg-info/top_level.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-03 06:53:32.711257 polymatica_api-0.0.6/setup.cfg
+-rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-03 06:53:21.000000 polymatica_api-0.0.6/setup.py
```

### Comparing `polymatica_api-0.0.5/LICENSE` & `polymatica_api-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.5/PKG-INFO` & `polymatica_api-0.0.6/polymatica_api.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 Metadata-Version: 2.1
-Name: polymatica_api
-Version: 0.0.5
+Name: polymatica-api
+Version: 0.0.6
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a simple example of getting data from a server Polymatica Platform
 
 ```python
 from polymatica_api import PolymaticaAPI
 from polymatica_api.types import DataOptionMethod
+import pandas as pd
 
 
 p = PolymaticaAPI('{SERVER_URL}', 'Token {TOKEN}')
-print(p.get_data([
+response = p.get_data([
     p.from_dataset('world_population.csv').
     method(DataOptionMethod.Aggregate).
     group("Country/Territory").
     sum(
         '2000 Population', 
         '2010 Population', 
         '2015 Population',
         '2020 Population',
         '2022 Population',
     )
-], False, False))
+])
+
+
+with response.get('default') as data:
+    frame = pd.DataFrame(data.rows)
+    frame.rename(columns=data.column_map, inplace=True)
+    print(frame)
 ```
```

### Comparing `polymatica_api-0.0.5/README.md` & `polymatica_api-0.0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 This is a simple example of getting data from a server Polymatica Platform
 
 ```python
 from polymatica_api import PolymaticaAPI
 from polymatica_api.types import DataOptionMethod
+import pandas as pd
 
 
 p = PolymaticaAPI('{SERVER_URL}', 'Token {TOKEN}')
-print(p.get_data([
+response = p.get_data([
     p.from_dataset('world_population.csv').
     method(DataOptionMethod.Aggregate).
     group("Country/Territory").
     sum(
         '2000 Population', 
         '2010 Population', 
         '2015 Population',
         '2020 Population',
         '2022 Population',
     )
-], False, False))
+])
+
+
+with response.get('default') as data:
+    frame = pd.DataFrame(data.rows)
+    frame.rename(columns=data.column_map, inplace=True)
+    print(frame)
 ```
```

### Comparing `polymatica_api-0.0.5/polymatica_api/__init__.py` & `polymatica_api-0.0.6/polymatica_api/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .types import Dataset
+from .types import Dataset, Data
 from .data_option import DataOption
 
 import typing
 import requests
 import urllib.parse
 
 
@@ -40,13 +40,17 @@
     def get_data(self, options, get_columns: bool = True, get_dataset: bool = False):
         data = self._session.post(self.route('data_dataset'), json=dict(
             data_options=list(map(lambda item: item.make(), options)),
             get_columns=get_columns,
             get_dataset=get_dataset
         )).json()
 
-        return data
+        result = dict()
+        for key in data:
+            result[key] = Data.parse_obj(data[key])
+
+        return result
 
     def route(self, name: str) -> str:
         if name not in HOST_ROUTE:
             raise Exception(f'Route "{name}" not found')
         return urllib.parse.urljoin(self._host, HOST_ROUTE[name])
```

### Comparing `polymatica_api-0.0.5/polymatica_api/data_option.py` & `polymatica_api-0.0.6/polymatica_api/data_option.py`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.5/polymatica_api.egg-info/PKG-INFO` & `polymatica_api-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 Metadata-Version: 2.1
-Name: polymatica-api
-Version: 0.0.5
+Name: polymatica_api
+Version: 0.0.6
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a simple example of getting data from a server Polymatica Platform
 
 ```python
 from polymatica_api import PolymaticaAPI
 from polymatica_api.types import DataOptionMethod
+import pandas as pd
 
 
 p = PolymaticaAPI('{SERVER_URL}', 'Token {TOKEN}')
-print(p.get_data([
+response = p.get_data([
     p.from_dataset('world_population.csv').
     method(DataOptionMethod.Aggregate).
     group("Country/Territory").
     sum(
         '2000 Population', 
         '2010 Population', 
         '2015 Population',
         '2020 Population',
         '2022 Population',
     )
-], False, False))
+])
+
+
+with response.get('default') as data:
+    frame = pd.DataFrame(data.rows)
+    frame.rename(columns=data.column_map, inplace=True)
+    print(frame)
 ```
```

### Comparing `polymatica_api-0.0.5/setup.py` & `polymatica_api-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 requires = [
     "pydantic==1.10.7",
     "requests==2.29.0"
 ]
 
 setuptools.setup(
     name="polymatica_api",
-    version="0.0.5",
+    version="0.0.6",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3"
     ],
     python_requires='>=3.7',
```

