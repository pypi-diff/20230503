# Comparing `tmp/yuna-db-0.2.1.tar.gz` & `tmp/yuna-db-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuna-db-0.2.1.tar", last modified: Thu Apr 27 23:09:58 2023, max compression
+gzip compressed data, was "yuna-db-0.2.2.tar", last modified: Wed May  3 00:03:14 2023, max compression
```

## Comparing `yuna-db-0.2.1.tar` & `yuna-db-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.2.1/LICENSE
--rw-r--r--   0        0        0     1579 2023-04-27 18:41:03.641249 yuna-db-0.2.1/README.md
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.1/__init__.py
--rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.2.1/requirements.txt
--rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.1/src/__init__.py
--rw-r--r--   0        0        0    14786 2023-04-27 23:07:25.921181 yuna-db-0.2.1/src/yuna/__init__.py
--rw-r--r--   0        0        0     8857 2023-04-26 20:56:38.448341 yuna-db-0.2.1/src/yuna/lmdb_util.py
--rw-r--r--   0        0        0    31092 2023-04-27 23:04:52.461639 yuna-db-0.2.1/src/yuna/plugins.py
--rwxr-xr-x   0        0        0     3304 2023-04-27 23:05:51.399000 yuna-db-0.2.1/test_yuna.py
--rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      417 2023-04-11 08:21:59.924544 yuna-db-0.2.1/tests/test_simple.py
--rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.2.1/version.txt
--rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 yuna-db-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-22 07:26:06.954355 yuna-db-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1579 2023-04-27 18:41:03.641249 yuna-db-0.2.2/README.md
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.2/__init__.py
+-rwxr-xr-x   0        0        0     3472 2023-05-03 00:01:55.987176 yuna-db-0.2.2/example.py
+-rw-r--r--   0        0        0      424 2023-04-22 07:50:30.728671 yuna-db-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        5 2023-04-12 07:21:23.231733 yuna-db-0.2.2/requirements.txt
+-rw-r--r--   0        0        0       24 2023-04-12 07:24:53.395821 yuna-db-0.2.2/src/__init__.py
+-rw-r--r--   0        0        0    15394 2023-05-02 23:16:33.172343 yuna-db-0.2.2/src/yuna/__init__.py
+-rw-r--r--   0        0        0     8917 2023-05-02 19:00:09.307489 yuna-db-0.2.2/src/yuna/lmdb_util.py
+-rw-r--r--   0        0        0    31423 2023-05-03 00:01:23.886587 yuna-db-0.2.2/src/yuna/plugins.py
+-rw-r--r--   0        0        0       99 2023-04-11 08:21:59.924544 yuna-db-0.2.2/tests/__init__.py
+-rwxr-xr-x   0        0        0     9470 2023-05-02 23:48:28.489421 yuna-db-0.2.2/tests/test_yuna.py
+-rw-r--r--   0        0        0        6 2023-04-22 05:31:29.343725 yuna-db-0.2.2/version.txt
+-rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 yuna-db-0.2.2/PKG-INFO
```

### Comparing `yuna-db-0.2.1/LICENSE` & `yuna-db-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yuna-db-0.2.1/README.md` & `yuna-db-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `yuna-db-0.2.1/src/yuna/__init__.py` & `yuna-db-0.2.2/src/yuna/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,20 +19,19 @@
 db.tables.foo.put(key, x)
 
 After that .put() you can call .get():
 
 x = db.tables.foo.get(key)
 """
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
+import os
 import types
 
-from dataclasses import dataclass
-
 from typing import Any, Iterator, Optional
 
 import lmdb
 
 
 from .lmdb_util import YUNA_DEFAULT_MAX_DB_SIZE, YUNA_DEFAULT_MAX_TABLES
 from .lmdb_util import YUNA_DB_META_KEY, YUNA_FILE_EXTENSION
@@ -46,23 +45,23 @@
 from .plugins import SERIALIZE_JSON, SERIALIZE_MSGPACK, SERIALIZE_STR
 from .plugins import COMPRESS_LZ4, COMPRESS_ZLIB, COMPRESS_ZSTD
 from .plugins import serialize_json, deserialize_json
 from .plugins import serialize_str, deserialize_str
 from .plugins import _empty_string_key_check
 
 
-@dataclass
 class YunaSharedData:
     """
     Private data for Yuna, in a class by itself so it can be shared
     among the multiple classes implementing Yuna.
     """
-    env: lmdb.Environment
-    tables_map: dict
-    metadata: dict
+    def __init__(self, env: lmdb.Environment, tables_map: dict, metadata: dict):
+        self.env = env
+        self.tables_map = tables_map
+        self.metadata = metadata
 
 
 class YunaReservedTable:
     """
     This class provides method functions to get/put values from the
     LMDB reserved table.
 
@@ -73,14 +72,16 @@
     # format, create a table and use that.  The reserved table should be mostly left alone.
     # Note that LMDB stores things in the reserved table, and Bad Things would happen if
     # you clobbered one of their special values.  In particular, any name used for a table
     # must not be clobbered.
     #
     # If you somehow have a real need to put something other than JSON into the reserved
     # table, serialize it yourself and use .raw_put() to store it.
+    #
+    # LMDB lets you have any number of tables; use those and leave the reserved table alone.
 
     def __init__(self, env: lmdb.Environment):
         self.env = env
 
     def delete(self, key: str) -> None:
         bytes_key = serialize_str(key)
         _lmdb_reserved_delete(self.env, bytes_key)
@@ -190,20 +191,26 @@
     A trvial class, just used as a container for instances of YunaTable.
 
     This will be .tables in the open Yuna instance.
     """
     pass
 
 
-@dataclass
 class YunaTableMetadata:
-    name: str
-    key_serialize: Optional[str] = None
-    serialize: Optional[str] = None
-    compress: Optional[str] = None
+    def __init__(self,
+        name: str,
+        key_serialize: Optional[str] = None,
+        serialize: Optional[str] = None,
+        compress: Optional[str] = None,
+    ):
+        self.name = name
+        self.key_serialize = key_serialize
+        self.serialize = serialize
+        self.compress = compress
+
 
 class YunaTable:
     """
     This class implements a table for Yuna.
 
     Provides method functions for delete, get, put, etc.
     """
@@ -337,14 +344,15 @@
             metadata = _yuna_new_meta(name=name, version=version)
         else:
             metadata = _yuna_get_meta(env, name=name, version=version)
 
         tables = YunaTablesMap()
         reserved = YunaReservedTable(env=env)
 
+        self.pathname = os.path.abspath(fname)
         self.metadata = metadata
         self.reserved = reserved
         self._shared = YunaSharedData(env=env, tables_map=vars(tables), metadata=metadata)
         self.tables = tables
 
         # Set up an entry in .tables for each table listed in metadata, with delete/get/put functions ready to use.
         for meta in metadata["tables"].values():
@@ -391,7 +399,14 @@
 
         # YunaTable takes care of adding the new table to self.tables
         assert name in vars(self.tables)
         # YunaTable also updates the metadata
         assert name in self._shared.metadata["tables"]
 
         return tbl
+
+class YunaReadOnly(Yuna):
+    def __init__(self, *args, **kwargs):
+        kwargs["read_only"] = True
+        kwargs["create"] = False
+        kwargs["safety_mode"] = 'u'
+        super().__init__(*args, **kwargs)
```

### Comparing `yuna-db-0.2.1/src/yuna/lmdb_util.py` & `yuna-db-0.2.2/src/yuna/lmdb_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,25 @@
 # as "databases" or "named databases".  Yuna will simply call these "tables".
 #
 # Every LMDB file has one, default key/value store that the user can store
 # data in, but that LMDB also stores some data in.  LMDB calls this
 # the "unnamed database".  Yuna calls this the "reserved table".
 #
 # LMDB calls the open LMDB file an "environment" and uses "env" as
-# the variable name for what is returned.  Yuna just calls it "the database"
-# and uses "lmdb" to refer to the open LMDB instance.
+# the variable name for what is returned.  Yuna's low-level LMDB code
+# uses this terminology but Yuna in general just refers to "the database".
 
 # LMDB files have to be declared with limits: maximum number of tables,
 # maximum total file size.  In practice it works quite well to simply give
 # very large limit numbers; the database will not actually take up the
 # maximum declared size.  On Linux, the file may appear to be that size,
 # but in that case the "yuna_repack" utility can be used to make a copy
 # of the database file that is minimum size.
+#
+# TODO: implement the "yuna_repack" utility
 
 
 class YunaInvalidDB(ValueError):
     pass
 
 YUNA_FILE_EXTENSION = ".ydb"
```

### Comparing `yuna-db-0.2.1/src/yuna/plugins.py` & `yuna-db-0.2.2/src/yuna/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 
 If you have an old version of Yuna and you try to open a new Yuna DB file
 you may have a lookup failure because a serialization or compression format
 is not present in this file.  In that case, try checking for a newer
 release of Yuna DB.
 """
 
-from dataclasses import dataclass
-
 from json import dumps as json_dumps
 from json import loads as json_loads
 
 from typing import Any, Callable, Dict, Iterator, List, Optional
 
 
 import lmdb
@@ -44,28 +42,39 @@
 
 
 # Create a unique object used to detect if optional arg not provided.
 # Can't use None because user might want to provide None.
 _YUNA_NOT_PROVIDED = object()
 
 
-@dataclass
 class SerializePlugins:
-    serialize: Callable
-    deserialize: Callable
-    init: Optional[Callable] = None
-    options: Optional[Callable] = None
+    def __init__(self,
+        serialize: Callable,
+        deserialize: Callable,
+        init: Optional[Callable] = None,
+        options: Optional[Callable] = None,
+    ):
+        self.serialize = serialize
+        self.deserialize = deserialize
+        self.init = init
+        self.options = options
 
-@dataclass
 class CompressPlugins:
-    compress: Callable
-    decompress: Callable
-    init: Optional[Callable] = None
-    options: Optional[Callable] = None
-    train: Optional[Callable] = None
+    def __init__(self,
+        compress: Callable,
+        decompress: Callable,
+        init: Optional[Callable] = None,
+        options: Optional[Callable] = None,
+        train: Optional[Callable] = None,
+    ):
+        self.compress = compress
+        self.decompress = decompress
+        self.init = init
+        self.options = options
+        self.train = train
 
 
 YUNA_SERIALIZE_CACHE: Dict[str, SerializePlugins] = {}
 
 
 def _not_implemented(*args, **kwargs) -> None:
     raise NotImplemented("not implemented yet")
```

### Comparing `yuna-db-0.2.1/test_yuna.py` & `yuna-db-0.2.2/example.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,28 @@
 We need a set of unit tests, but for now we have this.
 
 Exercise several Yuna features to make sure that at least
 the basics are working.
 
 """
 
-from src import yuna
-from src.yuna import Yuna
-from src.yuna.lmdb_util import _delete_file_or_dir
+import os
+import sys
 
-TEST_FILE = "/tmp/junk.ydb"
+# Hack sys.path so that this file will run against Yuna from this directory tree,
+# even if someone ran "pip install yuna-db" before running this.
+THIS_DIR = os.path.dirname(os.path.abspath(__file__))
+sys.path.insert(0, os.path.abspath(os.path.join(THIS_DIR, "src")))
+
+import yuna
+from yuna import Yuna
+from yuna.lmdb_util import _delete_file_or_dir
 
-#import pdb; pdb.set_trace()
-#db = Yuna(TEST_FILE, "test", 1, create=False)
+TEST_FILE = "/tmp/junk.ydb"
 
-#import pdb; pdb.set_trace()
 _delete_file_or_dir(TEST_FILE)
 with Yuna(TEST_FILE, "test", 1, create=True) as db:
     db.new_table("a26", serialize=yuna.SERIALIZE_STR, compress=yuna.COMPRESS_LZ4)
     tbl_a26 = db.tables.a26
     tbl_a26.put("a", "1")
     tbl_a26.put("b", "2")
     #tbl_a26.put("c", "3")
```

### Comparing `yuna-db-0.2.1/PKG-INFO` & `yuna-db-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuna-db
-Version: 0.2.1
+Version: 0.2.2
 Summary: Yuna DB: dict-like semantics for LMDB
 Author-email: "Steve R. Hastings" <steve@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: lmdb >=1.4.1,<2
```

