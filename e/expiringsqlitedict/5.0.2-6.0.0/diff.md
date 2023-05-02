# Comparing `tmp/expiringsqlitedict-5.0.2.tar.gz` & `tmp/expiringsqlitedict-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expiringsqlitedict-5.0.2.tar", last modified: Tue May  2 21:06:41 2023, max compression
+gzip compressed data, was "expiringsqlitedict-6.0.0.tar", last modified: Tue May  2 23:14:22 2023, max compression
```

## Comparing `expiringsqlitedict-5.0.2.tar` & `expiringsqlitedict-6.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-5.0.2/.gitignore
--rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-5.0.2/.travis.yml
--rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-5.0.2/CHANGELOG.txt
--rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-5.0.2/LICENSE.apache
--rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-5.0.2/LICENSE.rst
--rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-5.0.2/Makefile
--rw-r--r--   0        0        0     4042 2023-04-29 13:08:40.273027 expiringsqlitedict-5.0.2/README.rst
--rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-5.0.2/bench.py
--rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-5.0.2/docs/Makefile
--rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-5.0.2/docs/conf.py
--rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-5.0.2/docs/expiringsqlitedict.rst
--rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-5.0.2/docs/index.rst
--rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-5.0.2/docs/make.bat
--rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-5.0.2/docs/requirements.txt
--rw-r--r--   0        0        0     1030 2023-05-02 21:02:47.090474 expiringsqlitedict-5.0.2/pyproject.toml
--rwxr-xr-x   0        0        0     1327 2023-05-02 19:49:18.673775 expiringsqlitedict-5.0.2/run_all_tests.sh
--rwxr-xr-x   0        0        0    11820 2023-05-02 21:01:50.906531 expiringsqlitedict-5.0.2/src/expiringsqlitedict/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-5.0.2/src/expiringsqlitedict/py.typed
--rwxr-xr-x   0        0        0     9712 2023-05-02 21:06:03.726774 expiringsqlitedict-5.0.2/test.py
--rw-r--r--   0        0        0     4961 1970-01-01 00:00:00.000000 expiringsqlitedict-5.0.2/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-6.0.0/.gitignore
+-rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-6.0.0/.travis.yml
+-rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-6.0.0/CHANGELOG.txt
+-rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-6.0.0/LICENSE.apache
+-rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-6.0.0/LICENSE.rst
+-rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-6.0.0/Makefile
+-rw-r--r--   0        0        0     4042 2023-04-29 13:08:40.273027 expiringsqlitedict-6.0.0/README.rst
+-rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-6.0.0/bench.py
+-rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-6.0.0/docs/Makefile
+-rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-6.0.0/docs/conf.py
+-rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-6.0.0/docs/expiringsqlitedict.rst
+-rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-6.0.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-6.0.0/docs/make.bat
+-rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-6.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1030 2023-05-02 21:56:50.703943 expiringsqlitedict-6.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1327 2023-05-02 19:49:18.673775 expiringsqlitedict-6.0.0/run_all_tests.sh
+-rwxr-xr-x   0        0        0    15087 2023-05-02 23:13:52.877889 expiringsqlitedict-6.0.0/src/expiringsqlitedict/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-6.0.0/src/expiringsqlitedict/py.typed
+-rwxr-xr-x   0        0        0     9625 2023-05-02 23:02:32.536415 expiringsqlitedict-6.0.0/test.py
+-rw-r--r--   0        0        0     4961 1970-01-01 00:00:00.000000 expiringsqlitedict-6.0.0/PKG-INFO
```

### Comparing `expiringsqlitedict-5.0.2/CHANGELOG.txt` & `expiringsqlitedict-6.0.0/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.2/LICENSE.apache` & `expiringsqlitedict-6.0.0/LICENSE.apache`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.2/README.rst` & `expiringsqlitedict-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.2/bench.py` & `expiringsqlitedict-6.0.0/bench.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.2/docs/Makefile` & `expiringsqlitedict-6.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.2/docs/conf.py` & `expiringsqlitedict-6.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.2/docs/index.rst` & `expiringsqlitedict-6.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.2/docs/make.bat` & `expiringsqlitedict-6.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.2/pyproject.toml` & `expiringsqlitedict-6.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'expiringsqlitedict'
 description = 'Persistent compressed expiring dict in Python, backed up by sqlite3 and json'
-version = '5.0.2'
+version = '6.0.0'
 readme = 'README.rst'
 requires-python = '>= 3.6, < 4'
 license = { text = 'Apache 2.0' }
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `expiringsqlitedict-5.0.2/run_all_tests.sh` & `expiringsqlitedict-6.0.0/run_all_tests.sh`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-5.0.2/src/expiringsqlitedict/__init__.py` & `expiringsqlitedict-6.0.0/src/expiringsqlitedict/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import json
 import sqlite3
 from collections.abc import MutableMapping
 from contextlib import ExitStack, closing, contextmanager
 from datetime import timedelta
 from types import TracebackType
-from typing import Any, Generator, Iterator, Optional, Tuple, Type
+from typing import Any, Generator, Iterable, Iterator, Optional, Reversible, Tuple, Type
 from weakref import finalize
 
 @contextmanager
 def _transaction(
     connection: sqlite3.Connection,
     begin: str,
 ) -> Generator[None, None, None]:
@@ -33,14 +33,103 @@
         with closing(connection.cursor()) as cursor:
             cursor.execute('ROLLBACK')
         raise
     else:
         with closing(connection.cursor()) as cursor:
             cursor.execute('COMMIT')
 
+class _Keys(Reversible, Iterable[str]):
+    __slots__ = (
+        '_connection',
+        '_table',
+    )
+
+    def __init__(
+        self,
+        connection: sqlite3.Connection,
+        table: str,
+    ) -> None:
+
+        self._connection = connection
+        self._table = table
+
+    def _iterator(self, order: str) -> Iterator[str]:
+        with closing(self._connection.cursor()) as cursor:
+            for row in cursor.execute(
+                f'SELECT key FROM "{self._table}" ORDER BY id {order}',
+            ):
+                yield row[0]
+
+    def __iter__(self) -> Iterator[str]:
+        return self._iterator('ASC')
+
+    def __reversed__(self) -> Iterator[str]:
+        return self._iterator('DESC')
+
+class _Values(Reversible, Iterable[Any]):
+    __slots__ = (
+        '_connection',
+        '_table',
+        '_serializer',
+    )
+
+    def __init__(
+        self,
+        connection: sqlite3.Connection,
+        table: str,
+        serializer: Any,
+    ) -> None:
+
+        self._connection = connection
+        self._table = table
+        self._serializer = serializer
+
+    def _iterator(self, order: str) -> Iterator[Any]:
+        with closing(self._connection.cursor()) as cursor:
+            for row in cursor.execute(
+                f'SELECT value FROM "{self._table}" ORDER BY id {order}',
+            ):
+                yield self._serializer.loads(row[0])
+
+    def __iter__(self) -> Iterator[Any]:
+        return self._iterator('ASC')
+
+    def __reversed__(self) -> Iterator[Any]:
+        return self._iterator('DESC')
+
+class _Items(Reversible, Iterable[Tuple[str, Any]]):
+    __slots__ = (
+        '_connection',
+        '_table',
+        '_serializer',
+    )
+
+    def __init__(
+        self,
+        connection: sqlite3.Connection,
+        table: str,
+        serializer: Any,
+    ) -> None:
+        self._connection = connection
+        self._table = table
+        self._serializer = serializer
+
+    def _iterator(self, order: str) -> Iterator[Tuple[str, Any]]:
+        with closing(self._connection.cursor()) as cursor:
+            for row in cursor.execute(
+                f'SELECT key, value FROM "{self._table}" ORDER BY id {order}',
+            ):
+                yield row[0], self._serializer.loads(row[1])
+
+    def __iter__(self) -> Iterator[Tuple[str, Any]]:
+        return self._iterator('ASC')
+
+    def __reversed__(self) -> Iterator[Tuple[str, Any]]:
+        return self._iterator('DESC')
+
 class SqliteDict:
     """
     Set up the sqlite dictionary manager.
 
     This needs to be used as a context manager.  It will not operate at all
     otherwise. args and kwargs are directly passed to sqlite3.connect.  Use
     these to customize your connection, such as making it read-only.
@@ -168,16 +257,14 @@
             cursor.execute('PRAGMA optimize')
 
     finalize(connection, _close)
 
     return connection
 
 _trailers = []
-if sqlite3.sqlite_version_info >= (3, 8, 2):
-    _trailers.append('WITHOUT ROWID')
 
 if sqlite3.sqlite_version_info >= (3, 37):
     _trailers.append('STRICT')
     _valuetype = 'ANY'
 else:
     _valuetype = 'BLOB'
 
@@ -213,41 +300,43 @@
         self._lifespan = lifespan.total_seconds()
         self._serializer = serializer
         self._connection = connection
         self._table = table
         self._safe_table = table.replace('"', '""')
 
         with closing(self._connection.cursor()) as cursor:
-            create_statement = f'''
-            CREATE TABLE IF NOT EXISTS "{self._safe_table}" (
-                key TEXT PRIMARY KEY NOT NULL,
-                expire INTEGER NOT NULL,
-                value {_valuetype} NOT NULL){_trailer}'''
 
 
-            cursor.execute(create_statement)
-            cursor.execute(
-                f'CREATE INDEX IF NOT EXISTS "{self._safe_table}_expire_index"'
-                f' ON "{self._safe_table}" (expire)'
-            )
+            cursor.execute(f'''
+                CREATE TABLE IF NOT EXISTS "{self._safe_table}" (
+                    id INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL,
+                    key TEXT UNIQUE NOT NULL,
+                    expire INTEGER NOT NULL,
+                    value {_valuetype} NOT NULL){_trailer}
+            ''')
+
+            cursor.execute(f'''
+                CREATE INDEX IF NOT EXISTS "{self._safe_table}_expire_index"
+                 ON "{self._safe_table}" (expire)
+            ''')
 
             cursor.execute(
                 f'''
-                CREATE TRIGGER IF NOT EXISTS "{self._safe_table}_insert_trigger"'''
-                f''' AFTER INSERT ON "{self._safe_table}"
+                CREATE TRIGGER IF NOT EXISTS "{self._safe_table}_insert_trigger"
+                    AFTER INSERT ON "{self._safe_table}"
                 BEGIN
                     DELETE FROM "{self._safe_table}" WHERE expire <= {_unixepoch};
                 END
                 '''
             )
 
             cursor.execute(
                 f'''
-                CREATE TRIGGER IF NOT EXISTS "{self._safe_table}_update_trigger"'''
-                f''' AFTER UPDATE OF value ON "{self._safe_table}"
+                CREATE TRIGGER IF NOT EXISTS "{self._safe_table}_update_trigger"
+                    AFTER UPDATE OF value ON "{self._safe_table}"
                 BEGIN
                     DELETE FROM "{self._safe_table}" WHERE expire <= {_unixepoch};
                 END
                 '''
             )
     @property
     def connection(self) -> sqlite3.Connection:
@@ -277,39 +366,48 @@
         return 0
 
     def __bool__(self) -> bool:
         '''Check if the table is not empty.'''
 
         return len(self) > 0
 
-    def keys(self) -> Iterator[str]:
+    def keys(self) -> _Keys:
         '''Iterate over keys in the table.
         '''
 
-        with closing(self._connection.cursor()) as cursor:
-            for row in cursor.execute(f'SELECT key FROM "{self._safe_table}"'):
-                yield row[0]
+        return _Keys(
+            connection=self._connection,
+            table=self._safe_table,
+        )
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(self.keys())
 
-    __iter__ = keys
+    def __reversed__(self) -> Iterator[str]:
+        return reversed(self.keys())
 
-    def values(self) -> Iterator[Any]:
+    def values(self) -> _Values:
         '''Iterate over values in the table.
         '''
 
-        with closing(self._connection.cursor()) as cursor:
-            for row in cursor.execute(f'SELECT value FROM "{self._safe_table}"'):
-                yield self._serializer.loads(row[0])
+        return _Values(
+            connection=self._connection,
+            table=self._safe_table,
+            serializer=self._serializer,
+        )
 
-    def items(self) -> Iterator[Tuple[str, Any]]:
+    def items(self) -> _Items:
         '''Iterate over keys and values in the table.
         '''
 
-        with closing(self._connection.cursor()) as cursor:
-            for row in cursor.execute(f'SELECT key, value FROM "{self._safe_table}"'):
-                yield row[0], self._serializer.loads(row[1])
+        return _Items(
+            connection=self._connection,
+            table=self._safe_table,
+            serializer=self._serializer,
+        )
 
     def __contains__(self, key: str) -> bool:
         '''Check if the table contains the given key.
         '''
 
         with closing(self._connection.cursor()) as cursor:
             for _ in cursor.execute(
@@ -333,18 +431,38 @@
     def __setitem__(self, key: str, value: Any) -> None:
         '''Set or replace the item.
 
         This also triggers cleaning up expired values.
         '''
 
         with closing(self._connection.cursor()) as cursor:
-            cursor.execute(
-                f'REPLACE INTO "{self._safe_table}" (key, expire, value)'
-                f'VALUES (?, {_unixepoch} + ?, ?)',
-                (key, self._lifespan, self._serializer.dumps(value)),
+            if sqlite3.sqlite_version_info >= (3, 24):
+                cursor.execute(f'''
+                        INSERT INTO "{self._safe_table}" (key, expire, value)
+                            VALUES (?, {_unixepoch} + ?, ?)
+                            ON CONFLICT (key) DO UPDATE
+                            SET value=excluded.value, expire=excluded.expire
+                    ''',
+                    (key, self._lifespan, self._serializer.dumps(value)),
+                )
+            elif key in self:
+                cursor.execute(f'''
+                        UPDATE "{self._safe_table}"
+                            SET expire={_unixepoch} + ?,
+                                value=?
+                            WHERE key=?
+                    ''',
+                    (self._lifespan, self._serializer.dumps(value), key),
+                )
+            else:
+                cursor.execute(f'''
+                        INSERT INTO "{self._safe_table}" (key, expire, value)
+                            VALUES (?, {_unixepoch} + ?, ?)
+                    ''',
+                    (key, self._lifespan, self._serializer.dumps(value)),
                 )
 
     def __delitem__(self, key: str) -> None:
         '''Delete an item from the table.
         '''
 
         with closing(self._connection.cursor()) as cursor:
```

### Comparing `expiringsqlitedict-5.0.2/PKG-INFO` & `expiringsqlitedict-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expiringsqlitedict
-Version: 5.0.2
+Version: 6.0.0
 Summary: Persistent compressed expiring dict in Python, backed up by sqlite3 and json
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >= 3.6, < 4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

