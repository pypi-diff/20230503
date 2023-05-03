# Comparing `tmp/expiringsqlitedict-6.1.0.tar.gz` & `tmp/expiringsqlitedict-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expiringsqlitedict-6.1.0.tar", last modified: Wed May  3 04:27:46 2023, max compression
+gzip compressed data, was "expiringsqlitedict-6.2.0.tar", last modified: Wed May  3 15:44:21 2023, max compression
```

## Comparing `expiringsqlitedict-6.1.0.tar` & `expiringsqlitedict-6.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-6.1.0/.gitignore
--rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-6.1.0/.travis.yml
--rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-6.1.0/CHANGELOG.txt
--rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-6.1.0/LICENSE.apache
--rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-6.1.0/LICENSE.rst
--rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-6.1.0/Makefile
--rw-r--r--   0        0        0     4042 2023-04-29 13:08:40.273027 expiringsqlitedict-6.1.0/README.rst
--rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-6.1.0/bench.py
--rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-6.1.0/docs/Makefile
--rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-6.1.0/docs/conf.py
--rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-6.1.0/docs/expiringsqlitedict.rst
--rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-6.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-6.1.0/docs/make.bat
--rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-6.1.0/docs/requirements.txt
--rw-r--r--   0        0        0     1030 2023-05-03 04:27:43.504659 expiringsqlitedict-6.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     1327 2023-05-02 19:49:18.673775 expiringsqlitedict-6.1.0/run_all_tests.sh
--rwxr-xr-x   0        0        0    17339 2023-05-03 04:27:02.414982 expiringsqlitedict-6.1.0/src/expiringsqlitedict/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-6.1.0/src/expiringsqlitedict/py.typed
--rwxr-xr-x   0        0        0    13689 2023-05-03 04:27:02.414982 expiringsqlitedict-6.1.0/test.py
--rw-r--r--   0        0        0     4961 1970-01-01 00:00:00.000000 expiringsqlitedict-6.1.0/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-6.2.0/.gitignore
+-rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-6.2.0/.travis.yml
+-rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-6.2.0/CHANGELOG.txt
+-rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-6.2.0/LICENSE.apache
+-rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-6.2.0/LICENSE.rst
+-rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-6.2.0/Makefile
+-rw-r--r--   0        0        0     4042 2023-04-29 13:08:40.273027 expiringsqlitedict-6.2.0/README.rst
+-rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-6.2.0/bench.py
+-rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-6.2.0/docs/Makefile
+-rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-6.2.0/docs/conf.py
+-rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-6.2.0/docs/expiringsqlitedict.rst
+-rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-6.2.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-6.2.0/docs/make.bat
+-rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-6.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1030 2023-05-03 15:44:11.565641 expiringsqlitedict-6.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1327 2023-05-02 19:49:18.673775 expiringsqlitedict-6.2.0/run_all_tests.sh
+-rwxr-xr-x   0        0        0    18087 2023-05-03 15:38:04.335548 expiringsqlitedict-6.2.0/src/expiringsqlitedict/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-6.2.0/src/expiringsqlitedict/py.typed
+-rwxr-xr-x   0        0        0    14334 2023-05-03 15:37:32.783024 expiringsqlitedict-6.2.0/test.py
+-rw-r--r--   0        0        0     4961 1970-01-01 00:00:00.000000 expiringsqlitedict-6.2.0/PKG-INFO
```

### Comparing `expiringsqlitedict-6.1.0/CHANGELOG.txt` & `expiringsqlitedict-6.2.0/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.1.0/LICENSE.apache` & `expiringsqlitedict-6.2.0/LICENSE.apache`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.1.0/README.rst` & `expiringsqlitedict-6.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.1.0/bench.py` & `expiringsqlitedict-6.2.0/bench.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.1.0/docs/Makefile` & `expiringsqlitedict-6.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.1.0/docs/conf.py` & `expiringsqlitedict-6.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.1.0/docs/index.rst` & `expiringsqlitedict-6.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.1.0/docs/make.bat` & `expiringsqlitedict-6.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.1.0/pyproject.toml` & `expiringsqlitedict-6.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'expiringsqlitedict'
 description = 'Persistent compressed expiring dict in Python, backed up by sqlite3 and json'
-version = '6.1.0'
+version = '6.2.0'
 readme = 'README.rst'
 requires-python = '>= 3.6, < 4'
 license = { text = 'Apache 2.0' }
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `expiringsqlitedict-6.1.0/run_all_tests.sh` & `expiringsqlitedict-6.2.0/run_all_tests.sh`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.1.0/src/expiringsqlitedict/__init__.py` & `expiringsqlitedict-6.2.0/src/expiringsqlitedict/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,30 @@
 import sqlite3
 from collections.abc import MutableMapping
 from contextlib import ExitStack, closing, contextmanager
 from datetime import timedelta
 from types import TracebackType
 from typing import Any, Generator, Iterable, Iterator, Optional, Reversible, Tuple, Type
 from weakref import finalize
+from enum import unique, Enum
+
+@unique
+class Order(str, Enum):
+    '''An ordering enum for iteration methods.
+    '''
+
+    ID = 'id'
+    KEY = 'key'
+    EXPIRE = 'expire'
+
+    def __str__(self) -> str:
+        return self.value
+
+    def __format__(self, format_spec: str) -> str:
+        return self.value.__format__(format_spec)
 
 @contextmanager
 def _transaction(
     connection: sqlite3.Connection,
     begin: str,
 ) -> Generator[None, None, None]:
     with closing(connection.cursor()) as cursor:
@@ -37,91 +53,101 @@
         with closing(connection.cursor()) as cursor:
             cursor.execute('COMMIT')
 
 class _Keys(Reversible, Iterable[str]):
     __slots__ = (
         '_connection',
         '_table',
+        '_order',
     )
 
     def __init__(
         self,
         connection: sqlite3.Connection,
         table: str,
+        order: Order,
     ) -> None:
 
         self._connection = connection
         self._table = table
-
+        self._order = order
+    
     def _iterator(self, order: str) -> Iterator[str]:
         with closing(self._connection.cursor()) as cursor:
             for row in cursor.execute(
-                f'SELECT key FROM "{self._table}" ORDER BY id {order}',
+                f'SELECT key FROM "{self._table}" ORDER BY {self._order} {order}',
             ):
                 yield row[0]
 
     def __iter__(self) -> Iterator[str]:
         return self._iterator('ASC')
 
     def __reversed__(self) -> Iterator[str]:
         return self._iterator('DESC')
 
 class _Values(Reversible, Iterable[Any]):
     __slots__ = (
         '_connection',
         '_table',
         '_serializer',
+        '_order',
     )
 
     def __init__(
         self,
         connection: sqlite3.Connection,
         table: str,
         serializer: Any,
+        order: Order,
     ) -> None:
 
         self._connection = connection
         self._table = table
         self._serializer = serializer
+        self._order = order
 
     def _iterator(self, order: str) -> Iterator[Any]:
         with closing(self._connection.cursor()) as cursor:
             for row in cursor.execute(
-                f'SELECT value FROM "{self._table}" ORDER BY id {order}',
+                f'SELECT value FROM "{self._table}" ORDER BY {self._order} {order}',
             ):
                 yield self._serializer.loads(row[0])
 
     def __iter__(self) -> Iterator[Any]:
         return self._iterator('ASC')
 
     def __reversed__(self) -> Iterator[Any]:
         return self._iterator('DESC')
 
 class _Items(Reversible, Iterable[Tuple[str, Any]]):
     __slots__ = (
         '_connection',
         '_table',
         '_serializer',
+        '_order',
     )
 
     def __init__(
         self,
         connection: sqlite3.Connection,
         table: str,
         serializer: Any,
+        order: Order,
     ) -> None:
         self._connection = connection
         self._table = table
         self._serializer = serializer
-
+        self._order = order
+    
     def _iterator(self, order: str) -> Iterator[Tuple[str, Any]]:
         with closing(self._connection.cursor()) as cursor:
-            for row in cursor.execute(
-                f'SELECT key, value FROM "{self._table}" ORDER BY id {order}',
-            ):
+            for row in cursor.execute(f'''
+                SELECT key, value FROM "{self._table}"
+                    ORDER BY {self._order} {order}
+            '''):
                 yield row[0], self._serializer.loads(row[1])
 
     def __iter__(self) -> Iterator[Tuple[str, Any]]:
         return self._iterator('ASC')
 
     def __reversed__(self) -> Iterator[Tuple[str, Any]]:
         return self._iterator('DESC')
@@ -419,47 +445,50 @@
         return 0
 
     def __bool__(self) -> bool:
         '''Check if the table is not empty.'''
 
         return len(self) > 0
 
-    def keys(self) -> _Keys:
+    def keys(self, order: Order = Order.ID) -> _Keys:
         '''Iterate over keys in the table.
         '''
 
         return _Keys(
             connection=self._connection,
             table=self._safe_table,
+            order=order,
         )
 
     def __iter__(self) -> Iterator[str]:
         return iter(self.keys())
 
     def __reversed__(self) -> Iterator[str]:
         return reversed(self.keys())
 
-    def values(self) -> _Values:
+    def values(self, order: Order = Order.ID) -> _Values:
         '''Iterate over values in the table.
         '''
 
         return _Values(
             connection=self._connection,
             table=self._safe_table,
             serializer=self._serializer,
+            order=order,
         )
 
-    def items(self) -> _Items:
+    def items(self, order: Order = Order.ID) -> _Items:
         '''Iterate over keys and values in the table.
         '''
 
         return _Items(
             connection=self._connection,
             table=self._safe_table,
             serializer=self._serializer,
+            order=order,
         )
 
     def __contains__(self, key: str) -> bool:
         '''Check if the table contains the given key.
         '''
 
         with closing(self._connection.cursor()) as cursor:
```

### Comparing `expiringsqlitedict-6.1.0/test.py` & `expiringsqlitedict-6.2.0/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from contextlib import closing
 import sqlite3
 import unittest
 from datetime import timedelta
 from tempfile import TemporaryDirectory
 from pathlib import Path
-from expiringsqlitedict import SqliteDict, SimpleSqliteDict
+from expiringsqlitedict import SqliteDict, SimpleSqliteDict, Order
 import json
 import marshal
 import pickle
 import orjson
 
 class TestExpiringDict(unittest.TestCase):
     def test_simple(self):
@@ -42,14 +42,28 @@
                 self.assertEqual(tuple(reversed(d.keys())), ('baz', 'foo'))
                 self.assertEqual(
                     tuple(reversed(d.items())),
                     (('baz', 1337), ('foo', 'bar')),
                 )
                 self.assertEqual(tuple(reversed(d.values())), (1337, 'bar'))
 
+                self.assertEqual(tuple(d.keys(Order.KEY)), ('baz', 'foo'))
+                self.assertEqual(
+                    tuple(d.items(Order.KEY)),
+                    (('baz', 1337), ('foo', 'bar')),
+                )
+                self.assertEqual(tuple(d.values(Order.KEY)), (1337, 'bar'))
+
+                self.assertEqual(tuple(reversed(d.keys(Order.KEY))), ('foo', 'baz'))
+                self.assertEqual(
+                    tuple(reversed(d.items(Order.KEY))),
+                    (('foo', 'bar'), ('baz', 1337)),
+                )
+                self.assertEqual(tuple(reversed(d.values(Order.KEY))), ('bar', 1337))
+
             with SqliteDict(str(db_path)) as d:
                 d['foo'] = 'barbar'
 
             with SqliteDict(str(db_path)) as d:
                 self.assertTrue(bool(d))
                 self.assertEqual(tuple(d), ('foo', 'baz'))
                 self.assertEqual(tuple(d.keys()), ('foo', 'baz'))
```

### Comparing `expiringsqlitedict-6.1.0/PKG-INFO` & `expiringsqlitedict-6.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expiringsqlitedict
-Version: 6.1.0
+Version: 6.2.0
 Summary: Persistent compressed expiring dict in Python, backed up by sqlite3 and json
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >= 3.6, < 4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

