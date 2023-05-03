# Comparing `tmp/liteindex-0.0.1.dev4.tar.gz` & `tmp/liteindex-0.0.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteindex-0.0.1.dev4.tar", last modified: Wed May  3 07:44:33 2023, max compression
+gzip compressed data, was "liteindex-0.0.1.dev5.tar", last modified: Wed May  3 10:21:32 2023, max compression
```

## Comparing `liteindex-0.0.1.dev4.tar` & `liteindex-0.0.1.dev5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:33.026806 liteindex-0.0.1.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-03 07:44:33.026806 liteindex-0.0.1.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:33.026806 liteindex-0.0.1.dev4/liteindex/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/liteindex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/liteindex/any_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    19163 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/liteindex/defined_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/liteindex/dict_index_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/liteindex/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/liteindex/number_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:33.026806 liteindex-0.0.1.dev4/liteindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-03 07:44:32.000000 liteindex-0.0.1.dev4/liteindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 07:44:32.000000 liteindex-0.0.1.dev4/liteindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 07:44:32.000000 liteindex-0.0.1.dev4/liteindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 07:44:32.000000 liteindex-0.0.1.dev4/liteindex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 07:44:32.000000 liteindex-0.0.1.dev4/liteindex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 07:44:33.026806 liteindex-0.0.1.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:21:32.071393 liteindex-0.0.1.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-03 10:21:32.071393 liteindex-0.0.1.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:21:32.071393 liteindex-0.0.1.dev5/liteindex/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/liteindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/liteindex/any_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18737 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/liteindex/defined_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/liteindex/dict_index_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/liteindex/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/liteindex/number_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:21:32.071393 liteindex-0.0.1.dev5/liteindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-03 10:21:32.000000 liteindex-0.0.1.dev5/liteindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 10:21:32.000000 liteindex-0.0.1.dev5/liteindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:21:32.000000 liteindex-0.0.1.dev5/liteindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 10:21:32.000000 liteindex-0.0.1.dev5/liteindex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 10:21:32.000000 liteindex-0.0.1.dev5/liteindex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 10:21:32.071393 liteindex-0.0.1.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-03 10:21:17.000000 liteindex-0.0.1.dev5/setup.py
```

### Comparing `liteindex-0.0.1.dev4/LICENSE` & `liteindex-0.0.1.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev4/PKG-INFO` & `liteindex-0.0.1.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteindex
-Version: 0.0.1.dev4
+Version: 0.0.1.dev5
 Summary: SQLite based queryable python indexes for dicts and lists
 Home-page: https://github.com/notAI-tech/liteindex
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `liteindex-0.0.1.dev4/liteindex/defined_index.py` & `liteindex-0.0.1.dev5/liteindex/defined_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import sqlite3
 from typing import Any, Union, List, Iterator, Optional, Dict
 from collections.abc import MutableMapping
 
-
 class CustomList(list):
     def __init__(
         self, parent: MutableMapping, parent_key: str, key: str, *args, **kwargs
     ):
         super().__init__(*args, **kwargs)
         self.parent = parent
         self.parent_key = parent_key
@@ -184,20 +183,14 @@
                     f"Invalid schema value for key {key}: {value}. Values must be strings, numbers, or lists."
                 )
             if isinstance(value, list):
                 if not all(isinstance(item, allowed_types) for item in value):
                     raise ValueError(
                         f"Invalid schema value for key {key}: {value}. List items must be strings or numbers."
                     )
-            
-            # if isinstance(value, dict):
-            #     if not all(isinstance(item, allowed_types) for item in value.keys()) and not all(isinstance(item, allowed_types) for item in value.values()):
-            #         raise ValueError(
-            #             f"Invalid schema value for key {key}: {value}. List items must be strings or numbers."
-            #         )
 
     def _create_table(self):
         columns = []
         for key, value in self.schema.items():
             column_type = self._get_column_type(value)
             columns.append(f"{key} {column_type}")
         columns_str = ", ".join(columns)
@@ -205,27 +198,27 @@
             f"CREATE TABLE IF NOT EXISTS {self.name} (id TEXT PRIMARY KEY, {columns_str})"
         )
         self._connection.commit()
 
     def _get_column_type(self, value: Any) -> str:
         if isinstance(value, (int, float)):
             return "NUMBER"
-        elif isinstance(value, (list, tuple)): #, dict)):
+        elif isinstance(value, (list, tuple)):
             return "JSON"
         else:
             return "TEXT"
 
     def _serialize_value(self, value: Any) -> Union[str, float, int]:
-        if isinstance(value, (list, tuple)): #, dict)):
+        if isinstance(value, (list, tuple)):
             return json.dumps(value)
         else:
             return value
 
     def _deserialize_value(self, value: Any, example: Any) -> Any:
-        if isinstance(example, (list, tuple)): #, dict)):
+        if isinstance(example, (list, tuple)):
             return json.loads(value)
         else:
             return value
 
     def __getitem__(self, key: str) -> dict:
         result = self._connection.execute(
             f"SELECT * FROM {self.name} WHERE id = ?", (key,)
```

### Comparing `liteindex-0.0.1.dev4/liteindex/dict_index_helpers.py` & `liteindex-0.0.1.dev5/liteindex/dict_index_helpers.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev4/liteindex/file_index.py` & `liteindex-0.0.1.dev5/liteindex/file_index.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,38 +35,32 @@
             data = [(key, file_name, file_content) for file_name, file_content in value.items()]
             cursor.executemany(
                 f"INSERT OR REPLACE INTO {self.name} (key, file_name, value) VALUES (?, ?, ?)",
                 data
             )
 
     def __getitem__(self, key: str) -> Dict[str, bytes]:
-        with self._locked_cursor() as cursor:
+        with self._connection.cursor() as cursor:
             cursor.execute(f"SELECT file_name, value FROM {self.name} WHERE key=?", (key,))
             results = cursor.fetchall()
 
         if not results:
             raise KeyError(f"Key '{key}' not found in {self.name}")
 
         return {file_name: file_data for file_name, file_data in results}
 
     def get_file_paths(self, key: str) -> Iterator[str]:
-        with self._locked_cursor() as cursor:
+        with self._connection.cursor() as cursor:
+            temp_dir = tempfile.mkdtemp()
             cursor.execute(f"SELECT file_name, value FROM {self.name} WHERE key=?", (key,))
-            results = cursor.fetchall()
-
-        if not results:
-            raise KeyError(f"Key '{key}' not found in {self.name}")
-
-        temp_dir = tempfile.mkdtemp()
-
-        for file_name, file_data in results:
-            temp_path = os.path.join(temp_dir, file_name)
-            with open(temp_path, "wb") as temp_file:
-                temp_file.write(file_data)
-            yield temp_path
+            for file_name, file_data in cursor:
+                temp_path = os.path.join(temp_dir, file_name)
+                with open(temp_path, "wb") as temp_file:
+                    temp_file.write(file_data)
+                yield temp_path
 
     def __delitem__(self, key: str):
         with self._locked_cursor() as cursor:
             cursor.execute(f"DELETE FROM {self.name} WHERE key=?", (key,))
 if __name__ == "__main__":
     # Initialize the FileIndex
     file_index = FileIndex("my_files")
```

### Comparing `liteindex-0.0.1.dev4/liteindex/number_index.py` & `liteindex-0.0.1.dev5/liteindex/number_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev4/liteindex.egg-info/PKG-INFO` & `liteindex-0.0.1.dev5/liteindex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteindex
-Version: 0.0.1.dev4
+Version: 0.0.1.dev5
 Summary: SQLite based queryable python indexes for dicts and lists
 Home-page: https://github.com/notAI-tech/liteindex
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `liteindex-0.0.1.dev4/setup.py` & `liteindex-0.0.1.dev5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "liteindex"
 DESCRIPTION = "SQLite based queryable python indexes for dicts and lists"
 URL = "https://github.com/notAI-tech/liteindex"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev4"
+VERSION = "0.0.1.dev5"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
 ]
 
 # What packages are optional?
 EXTRAS = {
```

