# Comparing `tmp/liteindex-0.0.1.dev3.tar.gz` & `tmp/liteindex-0.0.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteindex-0.0.1.dev3.tar", last modified: Mon May  1 14:17:06 2023, max compression
+gzip compressed data, was "liteindex-0.0.1.dev4.tar", last modified: Wed May  3 07:44:33 2023, max compression
```

## Comparing `liteindex-0.0.1.dev3.tar` & `liteindex-0.0.1.dev4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:17:06.024911 liteindex-0.0.1.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-01 14:16:51.000000 liteindex-0.0.1.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-01 14:17:06.024911 liteindex-0.0.1.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-01 14:16:51.000000 liteindex-0.0.1.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:17:06.024911 liteindex-0.0.1.dev3/liteindex/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-01 14:16:51.000000 liteindex-0.0.1.dev3/liteindex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-01 14:16:51.000000 liteindex-0.0.1.dev3/liteindex/any_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    19163 2023-05-01 14:16:51.000000 liteindex-0.0.1.dev3/liteindex/defined_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-01 14:16:51.000000 liteindex-0.0.1.dev3/liteindex/dict_index_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-01 14:16:51.000000 liteindex-0.0.1.dev3/liteindex/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-01 14:16:51.000000 liteindex-0.0.1.dev3/liteindex/number_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 14:17:06.024911 liteindex-0.0.1.dev3/liteindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-01 14:17:05.000000 liteindex-0.0.1.dev3/liteindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-01 14:17:05.000000 liteindex-0.0.1.dev3/liteindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 14:17:05.000000 liteindex-0.0.1.dev3/liteindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 14:17:05.000000 liteindex-0.0.1.dev3/liteindex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 14:17:05.000000 liteindex-0.0.1.dev3/liteindex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 14:17:06.024911 liteindex-0.0.1.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-01 14:16:51.000000 liteindex-0.0.1.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:33.026806 liteindex-0.0.1.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-03 07:44:33.026806 liteindex-0.0.1.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:33.026806 liteindex-0.0.1.dev4/liteindex/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/liteindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/liteindex/any_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19163 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/liteindex/defined_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/liteindex/dict_index_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/liteindex/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/liteindex/number_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:44:33.026806 liteindex-0.0.1.dev4/liteindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-03 07:44:32.000000 liteindex-0.0.1.dev4/liteindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 07:44:32.000000 liteindex-0.0.1.dev4/liteindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 07:44:32.000000 liteindex-0.0.1.dev4/liteindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 07:44:32.000000 liteindex-0.0.1.dev4/liteindex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 07:44:32.000000 liteindex-0.0.1.dev4/liteindex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 07:44:33.026806 liteindex-0.0.1.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-03 07:44:15.000000 liteindex-0.0.1.dev4/setup.py
```

### Comparing `liteindex-0.0.1.dev3/LICENSE` & `liteindex-0.0.1.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev3/PKG-INFO` & `liteindex-0.0.1.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteindex
-Version: 0.0.1.dev3
+Version: 0.0.1.dev4
 Summary: SQLite based queryable python indexes for dicts and lists
 Home-page: https://github.com/notAI-tech/liteindex
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `liteindex-0.0.1.dev3/liteindex/any_index.py` & `liteindex-0.0.1.dev4/liteindex/any_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev3/liteindex/defined_index.py` & `liteindex-0.0.1.dev4/liteindex/defined_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev3/liteindex/dict_index_helpers.py` & `liteindex-0.0.1.dev4/liteindex/dict_index_helpers.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev3/liteindex/file_index.py` & `liteindex-0.0.1.dev4/liteindex/file_index.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,76 @@
 import sqlite3
 import tempfile
 import os
 from typing import Optional, Dict, Iterator
+from contextlib import contextmanager
+from threading import Lock
 
 class FileIndex:
     def __init__(self, name: str, db_path: str = ":memory:"):
         self.name = name
         self.db_path = db_path
-        self._connection = sqlite3.connect(self.db_path, uri=True)
+        self._connection = sqlite3.connect(self.db_path, uri=True, check_same_thread=False)
+        self._lock = Lock()
         self._create_table()
 
+    @contextmanager
+    def _locked_cursor(self):
+        with self._lock:
+            cursor = self._connection.cursor()
+            try:
+                yield cursor
+                self._connection.commit()
+            finally:
+                cursor.close()
+
     def _create_table(self):
-        cursor = self._connection.cursor()
-        cursor.execute(
-            f"CREATE TABLE IF NOT EXISTS {self.name} (id INTEGER PRIMARY KEY AUTOINCREMENT, key TEXT, file_name TEXT, value BLOB)"
-        )
-        cursor.execute(f"CREATE INDEX IF NOT EXISTS idx_file_name ON {self.name} (file_name)")
-        self._connection.commit()
+        with self._locked_cursor() as cursor:
+            cursor.execute(
+                f"CREATE TABLE IF NOT EXISTS {self.name} (id INTEGER PRIMARY KEY AUTOINCREMENT, key TEXT, file_name TEXT, value BLOB)"
+            )
+            cursor.execute(f"CREATE INDEX IF NOT EXISTS idx_file_name ON {self.name} (file_name)")
 
     def __setitem__(self, key: str, value: Dict[str, bytes]):
-        cursor = self._connection.cursor()
-
-        for file_name, file_content in value.items():
-            cursor.execute(
+        with self._locked_cursor() as cursor:
+            data = [(key, file_name, file_content) for file_name, file_content in value.items()]
+            cursor.executemany(
                 f"INSERT OR REPLACE INTO {self.name} (key, file_name, value) VALUES (?, ?, ?)",
-                (key, file_name, file_content),
+                data
             )
 
-        self._connection.commit()
-
     def __getitem__(self, key: str) -> Dict[str, bytes]:
-        cursor = self._connection.cursor()
-        cursor.execute(f"SELECT file_name, value FROM {self.name} WHERE key=?", (key,))
-        results = cursor.fetchall()
+        with self._locked_cursor() as cursor:
+            cursor.execute(f"SELECT file_name, value FROM {self.name} WHERE key=?", (key,))
+            results = cursor.fetchall()
 
         if not results:
             raise KeyError(f"Key '{key}' not found in {self.name}")
 
         return {file_name: file_data for file_name, file_data in results}
 
     def get_file_paths(self, key: str) -> Iterator[str]:
-        cursor = self._connection.cursor()
-        cursor.execute(f"SELECT file_name, value FROM {self.name} WHERE key=?", (key,))
-        results = cursor.fetchall()
+        with self._locked_cursor() as cursor:
+            cursor.execute(f"SELECT file_name, value FROM {self.name} WHERE key=?", (key,))
+            results = cursor.fetchall()
 
         if not results:
             raise KeyError(f"Key '{key}' not found in {self.name}")
 
         temp_dir = tempfile.mkdtemp()
 
         for file_name, file_data in results:
             temp_path = os.path.join(temp_dir, file_name)
             with open(temp_path, "wb") as temp_file:
                 temp_file.write(file_data)
             yield temp_path
 
     def __delitem__(self, key: str):
-        cursor = self._connection.cursor()
-        cursor.execute(f"DELETE FROM {self.name} WHERE key=?", (key,))
-        self._connection.commit()
-
+        with self._locked_cursor() as cursor:
+            cursor.execute(f"DELETE FROM {self.name} WHERE key=?", (key,))
 if __name__ == "__main__":
     # Initialize the FileIndex
     file_index = FileIndex("my_files")
 
     # Add multiple files to the FileIndex
     file_key = "key_1"
     files = {
```

### Comparing `liteindex-0.0.1.dev3/liteindex/number_index.py` & `liteindex-0.0.1.dev4/liteindex/number_index.py`

 * *Files identical despite different names*

### Comparing `liteindex-0.0.1.dev3/liteindex.egg-info/PKG-INFO` & `liteindex-0.0.1.dev4/liteindex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liteindex
-Version: 0.0.1.dev3
+Version: 0.0.1.dev4
 Summary: SQLite based queryable python indexes for dicts and lists
 Home-page: https://github.com/notAI-tech/liteindex
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `liteindex-0.0.1.dev3/setup.py` & `liteindex-0.0.1.dev4/setup.py`

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
-VERSION = "0.0.1.dev3"
+VERSION = "0.0.1.dev4"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
 ]
 
 # What packages are optional?
 EXTRAS = {
```

