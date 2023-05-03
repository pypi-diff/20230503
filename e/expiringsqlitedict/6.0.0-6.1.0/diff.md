# Comparing `tmp/expiringsqlitedict-6.0.0.tar.gz` & `tmp/expiringsqlitedict-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expiringsqlitedict-6.0.0.tar", last modified: Tue May  2 23:14:22 2023, max compression
+gzip compressed data, was "expiringsqlitedict-6.1.0.tar", last modified: Wed May  3 04:27:46 2023, max compression
```

## Comparing `expiringsqlitedict-6.0.0.tar` & `expiringsqlitedict-6.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-6.0.0/.gitignore
--rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-6.0.0/.travis.yml
--rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-6.0.0/CHANGELOG.txt
--rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-6.0.0/LICENSE.apache
--rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-6.0.0/LICENSE.rst
--rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-6.0.0/Makefile
--rw-r--r--   0        0        0     4042 2023-04-29 13:08:40.273027 expiringsqlitedict-6.0.0/README.rst
--rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-6.0.0/bench.py
--rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-6.0.0/docs/Makefile
--rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-6.0.0/docs/conf.py
--rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-6.0.0/docs/expiringsqlitedict.rst
--rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-6.0.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-6.0.0/docs/make.bat
--rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-6.0.0/docs/requirements.txt
--rw-r--r--   0        0        0     1030 2023-05-02 21:56:50.703943 expiringsqlitedict-6.0.0/pyproject.toml
--rwxr-xr-x   0        0        0     1327 2023-05-02 19:49:18.673775 expiringsqlitedict-6.0.0/run_all_tests.sh
--rwxr-xr-x   0        0        0    15087 2023-05-02 23:13:52.877889 expiringsqlitedict-6.0.0/src/expiringsqlitedict/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-6.0.0/src/expiringsqlitedict/py.typed
--rwxr-xr-x   0        0        0     9625 2023-05-02 23:02:32.536415 expiringsqlitedict-6.0.0/test.py
--rw-r--r--   0        0        0     4961 1970-01-01 00:00:00.000000 expiringsqlitedict-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-6.1.0/.gitignore
+-rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-6.1.0/.travis.yml
+-rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-6.1.0/CHANGELOG.txt
+-rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-6.1.0/LICENSE.apache
+-rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-6.1.0/LICENSE.rst
+-rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-6.1.0/Makefile
+-rw-r--r--   0        0        0     4042 2023-04-29 13:08:40.273027 expiringsqlitedict-6.1.0/README.rst
+-rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-6.1.0/bench.py
+-rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-6.1.0/docs/Makefile
+-rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-6.1.0/docs/conf.py
+-rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-6.1.0/docs/expiringsqlitedict.rst
+-rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-6.1.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-6.1.0/docs/make.bat
+-rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-6.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1030 2023-05-03 04:27:43.504659 expiringsqlitedict-6.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1327 2023-05-02 19:49:18.673775 expiringsqlitedict-6.1.0/run_all_tests.sh
+-rwxr-xr-x   0        0        0    17339 2023-05-03 04:27:02.414982 expiringsqlitedict-6.1.0/src/expiringsqlitedict/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-6.1.0/src/expiringsqlitedict/py.typed
+-rwxr-xr-x   0        0        0    13689 2023-05-03 04:27:02.414982 expiringsqlitedict-6.1.0/test.py
+-rw-r--r--   0        0        0     4961 1970-01-01 00:00:00.000000 expiringsqlitedict-6.1.0/PKG-INFO
```

### Comparing `expiringsqlitedict-6.0.0/CHANGELOG.txt` & `expiringsqlitedict-6.1.0/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.0.0/LICENSE.apache` & `expiringsqlitedict-6.1.0/LICENSE.apache`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.0.0/README.rst` & `expiringsqlitedict-6.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.0.0/bench.py` & `expiringsqlitedict-6.1.0/bench.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.0.0/docs/Makefile` & `expiringsqlitedict-6.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.0.0/docs/conf.py` & `expiringsqlitedict-6.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.0.0/docs/index.rst` & `expiringsqlitedict-6.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.0.0/docs/make.bat` & `expiringsqlitedict-6.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.0.0/pyproject.toml` & `expiringsqlitedict-6.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'expiringsqlitedict'
 description = 'Persistent compressed expiring dict in Python, backed up by sqlite3 and json'
-version = '6.0.0'
+version = '6.1.0'
 readme = 'README.rst'
 requires-python = '>= 3.6, < 4'
 license = { text = 'Apache 2.0' }
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `expiringsqlitedict-6.0.0/run_all_tests.sh` & `expiringsqlitedict-6.1.0/run_all_tests.sh`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-6.0.0/src/expiringsqlitedict/__init__.py` & `expiringsqlitedict-6.1.0/src/expiringsqlitedict/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -271,14 +271,16 @@
 _trailer = ', '.join(_trailers)
 
 if sqlite3.sqlite_version_info >= (3, 38):
     _unixepoch = 'UNIXEPOCH()'
 else:
     _unixepoch = "CAST(strftime('%s', 'now') AS INTEGER)"
 
+APPLICATION_ID = 1820903862
+
 class Connection(MutableMapping):
     '''The actual connection object, as a MutableMapping[str, Any].
 
     Items are expired when a value is inserted or updated.  Deletion or
     postponement does not expire items.
     '''
 
@@ -300,48 +302,99 @@
         self._lifespan = lifespan.total_seconds()
         self._serializer = serializer
         self._connection = connection
         self._table = table
         self._safe_table = table.replace('"', '""')
 
         with closing(self._connection.cursor()) as cursor:
-
-
-            cursor.execute(f'''
-                CREATE TABLE IF NOT EXISTS "{self._safe_table}" (
-                    id INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL,
-                    key TEXT UNIQUE NOT NULL,
-                    expire INTEGER NOT NULL,
-                    value {_valuetype} NOT NULL){_trailer}
-            ''')
-
-            cursor.execute(f'''
-                CREATE INDEX IF NOT EXISTS "{self._safe_table}_expire_index"
-                 ON "{self._safe_table}" (expire)
-            ''')
-
-            cursor.execute(
-                f'''
-                CREATE TRIGGER IF NOT EXISTS "{self._safe_table}_insert_trigger"
-                    AFTER INSERT ON "{self._safe_table}"
-                BEGIN
-                    DELETE FROM "{self._safe_table}" WHERE expire <= {_unixepoch};
-                END
-                '''
-            )
-
-            cursor.execute(
-                f'''
-                CREATE TRIGGER IF NOT EXISTS "{self._safe_table}_update_trigger"
-                    AFTER UPDATE OF value ON "{self._safe_table}"
-                BEGIN
-                    DELETE FROM "{self._safe_table}" WHERE expire <= {_unixepoch};
-                END
-                '''
-            )
+            application_id = next(cursor.execute('PRAGMA application_id'))[0]
+            if application_id == 0:
+                cursor.execute(f'PRAGMA application_id = {APPLICATION_ID}')
+            elif application_id != APPLICATION_ID:
+                raise ValueError(f'illegal application ID {application_id}')
+
+            user_version = next(cursor.execute('PRAGMA user_version'))[0]
+
+            if user_version < 1:
+                # Attempt to migrate, because of pre-6.1 versions.  We can't
+                # otherwise tell the difference between a fresh database and a
+                # pre-set one.
+                cursor.execute(
+                    "SELECT 1 FROM sqlite_master WHERE type='table' AND name=?",
+                    (self._table,),
+                )
+                migrate = bool(cursor.fetchall())
+
+                if migrate:
+                    cursor.execute(f'''
+                        DROP INDEX IF EXISTS "{self._safe_table}_expire_index"
+                    ''')
+                    cursor.execute(f'''
+                        DROP TRIGGER IF EXISTS "{self._safe_table}_insert_trigger"
+                    ''')
+                    cursor.execute(f'''
+                        DROP TRIGGER IF EXISTS "{self._safe_table}_update_trigger"
+                    ''')
+                    cursor.execute(f'''
+                        ALTER TABLE "{self._safe_table}"
+                        RENAME TO "{self._safe_table}_v0"
+                    ''')
+
+
+                cursor.execute(f'''
+                    CREATE TABLE "{self._safe_table}" (
+                        id INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL,
+                        key TEXT UNIQUE NOT NULL,
+                        expire INTEGER NOT NULL,
+                        value {_valuetype} NOT NULL){_trailer}
+                ''')
+
+                cursor.execute(f'''
+                    CREATE INDEX "{self._safe_table}_expire_index"
+                     ON "{self._safe_table}" (expire)
+                ''')
+
+                cursor.execute(
+                    f'''
+                    CREATE TRIGGER "{self._safe_table}_insert_trigger"
+                        AFTER INSERT ON "{self._safe_table}"
+                    BEGIN
+                        DELETE FROM "{self._safe_table}" WHERE expire <= {_unixepoch};
+                    END
+                    '''
+                )
+
+                cursor.execute(
+                    f'''
+                    CREATE TRIGGER "{self._safe_table}_update_trigger"
+                        AFTER UPDATE OF value ON "{self._safe_table}"
+                    BEGIN
+                        DELETE FROM "{self._safe_table}" WHERE expire <= {_unixepoch};
+                    END
+                    '''
+                )
+
+                if migrate:
+                    cursor.execute(f'''
+                        INSERT INTO "{self._safe_table}"
+                            (key, expire, value)
+                        SELECT key, expire, value
+                            FROM "{self._safe_table}_v0"
+                    ''')
+                    cursor.execute(f'DROP TABLE "{self._safe_table}_v0"')
+
+                cursor.execute('PRAGMA user_version = 1')
+
+                user_version = 1
+
+            if user_version > 1:
+                raise ValueError(
+                    'this version of expiringsqlitedict is not'
+                    ' compatible with this schema version'
+                )
     @property
     def connection(self) -> sqlite3.Connection:
         return self._connection
 
     @property
     def lifespan(self) -> timedelta:
         '''The current lifespan.
```

### Comparing `expiringsqlitedict-6.0.0/test.py` & `expiringsqlitedict-6.1.0/test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Copyright © 2021 Taylor C. Richberger
 # This code is released under the license described in the LICENSE file
 
+from contextlib import closing
+import sqlite3
 import unittest
 from datetime import timedelta
 from tempfile import TemporaryDirectory
 from pathlib import Path
 from expiringsqlitedict import SqliteDict, SimpleSqliteDict
 import json
 import marshal
@@ -46,14 +48,105 @@
 
             with SqliteDict(str(db_path)) as d:
                 d['foo'] = 'barbar'
 
             with SqliteDict(str(db_path)) as d:
                 self.assertTrue(bool(d))
                 self.assertEqual(tuple(d), ('foo', 'baz'))
+                self.assertEqual(tuple(d.keys()), ('foo', 'baz'))
+                self.assertEqual(tuple(d.items()), (('foo', 'barbar'), ('baz', 1337)))
+                self.assertEqual(tuple(d.values()), ('barbar', 1337))
+                self.assertEqual(len(d), 2)
+
+            with SqliteDict(str(db_path)) as d:
+                del d['foo']
+
+            with SqliteDict(str(db_path)) as d:
+                self.assertTrue(bool(d))
+                self.assertEqual(tuple(d), ('baz',))
+                self.assertEqual(tuple(d.keys()), ('baz',))
+                self.assertEqual(tuple(d.items()), (('baz', 1337),))
+                self.assertEqual(tuple(d.values()), (1337,))
+                self.assertEqual(len(d), 1)
+
+            with self.assertRaises(KeyError):
+                with SqliteDict(str(db_path)) as d:
+                    del d['foo']
+
+            
+            with SqliteDict(str(db_path)) as d:
+                d['foo'] = 'spam'
+
+            with SqliteDict(str(db_path)) as d:
+                self.assertTrue(bool(d))
+                self.assertEqual(tuple(d), ('baz', 'foo'))
+                self.assertEqual(tuple(d.keys()), ('baz', 'foo'))
+                self.assertEqual(tuple(d.items()), (('baz', 1337), ('foo', 'spam')))
+                self.assertEqual(tuple(d.values()), (1337, 'spam'))
+                self.assertEqual(len(d), 2)
+
+    def test_migration(self):
+        with TemporaryDirectory() as temporary_directory:
+            db_path = Path(temporary_directory) / 'test.db'
+
+            with closing(sqlite3.connect(str(db_path))) as connection:
+                with closing(connection.cursor()) as cursor:
+                    cursor.execute('''
+                        CREATE TABLE expiringsqlitedict (
+                            key TEXT UNIQUE PRIMARY KEY NOT NULL,
+                            expire INTEGER NOT NULL,
+                            value BLOB NOT NULL
+                        )
+                    ''')
+                    cursor.execute('''
+                        CREATE INDEX expiringsqlitedict_expire_index
+                            ON expiringsqlitedict (expire)
+                    ''')
+                    cursor.execute('''
+                        CREATE TRIGGER expiringsqlitedict_insert_trigger
+                            AFTER INSERT ON expiringsqlitedict
+                        BEGIN
+                            DELETE FROM expiringsqlitedict
+                                WHERE expire <= strftime('%s', 'now');
+                        END
+                    ''')
+                    cursor.execute('''
+                        CREATE TRIGGER expiringsqlitedict_update_trigger
+                            AFTER UPDATE ON expiringsqlitedict
+                        BEGIN
+                            DELETE FROM expiringsqlitedict
+                                WHERE expire <= strftime('%s', 'now');
+                        END
+                    ''')
+                    cursor.executemany(
+                        '''
+                            INSERT INTO expiringsqlitedict (key, expire, value)
+                            VALUES (?, strftime('%s', 'now', '+7 days'), ?)
+                        ''',
+                        (
+                            ('foo', '"bar"'),
+                            ('baz', '1337'),
+                        ),
+                    )
+                connection.commit()
+
+            with SqliteDict(str(db_path)) as d:
+                self.assertTrue(bool(d))
+                self.assertEqual(set(d), {'foo', 'baz'})
+                self.assertEqual(set(d.keys()), {'foo', 'baz'})
+                self.assertEqual(set(d.items()), {('foo', 'bar'), ('baz', 1337)})
+                self.assertEqual(set(d.values()), {'bar', 1337})
+                self.assertEqual(len(d), 2)
+
+            with SqliteDict(str(db_path)) as d:
+                d['foo'] = 'barbar'
+
+            with SqliteDict(str(db_path)) as d:
+                self.assertTrue(bool(d))
+                self.assertEqual(tuple(d), ('foo', 'baz'))
                 self.assertEqual(tuple(d.keys()), ('foo', 'baz'))
                 self.assertEqual(tuple(d.items()), (('foo', 'barbar'), ('baz', 1337)))
                 self.assertEqual(tuple(d.values()), ('barbar', 1337))
                 self.assertEqual(len(d), 2)
 
             with SqliteDict(str(db_path)) as d:
                 del d['foo']
```

### Comparing `expiringsqlitedict-6.0.0/PKG-INFO` & `expiringsqlitedict-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expiringsqlitedict
-Version: 6.0.0
+Version: 6.1.0
 Summary: Persistent compressed expiring dict in Python, backed up by sqlite3 and json
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >= 3.6, < 4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

