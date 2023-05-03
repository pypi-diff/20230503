# Comparing `tmp/AshenDB-0.0.3.tar.gz` & `tmp/AshenDB-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshenDB-0.0.3.tar", last modified: Wed Apr 26 02:01:43 2023, max compression
+gzip compressed data, was "AshenDB-0.0.4.tar", last modified: Wed May  3 01:48:01 2023, max compression
```

## Comparing `AshenDB-0.0.3.tar` & `AshenDB-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-04-26 02:01:43.259629 AshenDB-0.0.3/
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-04-26 02:01:43.258629 AshenDB-0.0.3/AshenDB.egg-info/
--rw-r--r--   0 aurka     (1000) aurka     (1000)     2248 2023-04-26 02:01:43.000000 AshenDB-0.0.3/AshenDB.egg-info/PKG-INFO
--rw-r--r--   0 aurka     (1000) aurka     (1000)      360 2023-04-26 02:01:43.000000 AshenDB-0.0.3/AshenDB.egg-info/SOURCES.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        1 2023-04-26 02:01:43.000000 AshenDB-0.0.3/AshenDB.egg-info/dependency_links.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)       50 2023-04-26 02:01:43.000000 AshenDB-0.0.3/AshenDB.egg-info/entry_points.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        9 2023-04-26 02:01:43.000000 AshenDB-0.0.3/AshenDB.egg-info/requires.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)        8 2023-04-26 02:01:43.000000 AshenDB-0.0.3/AshenDB.egg-info/top_level.txt
--rw-r--r--   0 aurka     (1000) aurka     (1000)     1065 2023-04-18 23:23:36.000000 AshenDB-0.0.3/LICENSE
--rw-r--r--   0 aurka     (1000) aurka     (1000)     2248 2023-04-26 02:01:43.259629 AshenDB-0.0.3/PKG-INFO
--rw-r--r--   0 aurka     (1000) aurka     (1000)      300 2023-04-23 07:22:33.000000 AshenDB-0.0.3/README.rst
-drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-04-26 02:01:43.259629 AshenDB-0.0.3/ashendb/
--rw-r--r--   0 aurka     (1000) aurka     (1000)      786 2023-04-26 01:59:48.000000 AshenDB-0.0.3/ashendb/__init__.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     6569 2023-04-25 03:31:02.000000 AshenDB-0.0.3/ashendb/client.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     7836 2023-04-26 01:57:22.000000 AshenDB-0.0.3/ashendb/collection.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     7416 2023-04-25 03:31:05.000000 AshenDB-0.0.3/ashendb/database.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)      923 2023-04-22 08:20:09.000000 AshenDB-0.0.3/ashendb/document.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)      128 2023-04-23 19:49:22.000000 AshenDB-0.0.3/ashendb/exception.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)     3719 2023-04-26 01:56:22.000000 AshenDB-0.0.3/ashendb/helper.py
--rw-r--r--   0 aurka     (1000) aurka     (1000)      906 2023-04-26 01:58:34.000000 AshenDB-0.0.3/pyproject.toml
--rw-r--r--   0 aurka     (1000) aurka     (1000)       38 2023-04-26 02:01:43.259629 AshenDB-0.0.3/setup.cfg
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-05-03 01:48:01.262858 AshenDB-0.0.4/
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-05-03 01:48:01.261859 AshenDB-0.0.4/AshenDB.egg-info/
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     2248 2023-05-03 01:48:01.000000 AshenDB-0.0.4/AshenDB.egg-info/PKG-INFO
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      360 2023-05-03 01:48:01.000000 AshenDB-0.0.4/AshenDB.egg-info/SOURCES.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        1 2023-05-03 01:48:01.000000 AshenDB-0.0.4/AshenDB.egg-info/dependency_links.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)       50 2023-05-03 01:48:01.000000 AshenDB-0.0.4/AshenDB.egg-info/entry_points.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        9 2023-05-03 01:48:01.000000 AshenDB-0.0.4/AshenDB.egg-info/requires.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)        8 2023-05-03 01:48:01.000000 AshenDB-0.0.4/AshenDB.egg-info/top_level.txt
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     1065 2023-04-18 23:23:36.000000 AshenDB-0.0.4/LICENSE
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     2248 2023-05-03 01:48:01.262858 AshenDB-0.0.4/PKG-INFO
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      300 2023-04-23 07:22:33.000000 AshenDB-0.0.4/README.rst
+drwxr-xr-x   0 aurka     (1000) aurka     (1000)        0 2023-05-03 01:48:01.262858 AshenDB-0.0.4/ashendb/
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      786 2023-04-26 01:59:48.000000 AshenDB-0.0.4/ashendb/__init__.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     6886 2023-04-29 23:18:14.000000 AshenDB-0.0.4/ashendb/client.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     9216 2023-05-03 01:37:15.000000 AshenDB-0.0.4/ashendb/collection.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     7751 2023-04-29 23:18:41.000000 AshenDB-0.0.4/ashendb/database.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     1257 2023-05-03 00:01:33.000000 AshenDB-0.0.4/ashendb/document.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      128 2023-04-23 19:49:22.000000 AshenDB-0.0.4/ashendb/exception.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)     7961 2023-05-03 01:30:12.000000 AshenDB-0.0.4/ashendb/helper.py
+-rw-r--r--   0 aurka     (1000) aurka     (1000)      906 2023-05-03 01:26:30.000000 AshenDB-0.0.4/pyproject.toml
+-rw-r--r--   0 aurka     (1000) aurka     (1000)       38 2023-05-03 01:48:01.262858 AshenDB-0.0.4/setup.cfg
```

### Comparing `AshenDB-0.0.3/AshenDB.egg-info/PKG-INFO` & `AshenDB-0.0.4/AshenDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshenDB
-Version: 0.0.3
+Version: 0.0.4
 Summary: Another stupid library for using json as Database
 Author-email: Abdullah Al Muaz <abdullahalmuaz15@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ashenite
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `AshenDB-0.0.3/LICENSE` & `AshenDB-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.3/PKG-INFO` & `AshenDB-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshenDB
-Version: 0.0.3
+Version: 0.0.4
 Summary: Another stupid library for using json as Database
 Author-email: Abdullah Al Muaz <abdullahalmuaz15@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ashenite
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `AshenDB-0.0.3/ashendb/__init__.py` & `AshenDB-0.0.4/ashendb/__init__.py`

 * *Files identical despite different names*

### Comparing `AshenDB-0.0.3/ashendb/client.py` & `AshenDB-0.0.4/ashendb/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,18 @@
             NotFound: If one of the databases does not exist.
 
         Example:
             >>> async for db in AshenDB.iterate_dbs(["test", "test2"]):
             ...     print(db)
             <Database: test>
             <Database: test2>
+
+            >>> dbs = [db async for db in AshenDB.iterate_dbs()]
+            >>> dbs
+            [<Database: test>, <Database: test2>, <Database: test3>]
         """
         if db_names is None or len(db_names) == 0:
             for name in await aios.listdir(cls.base):
                 yield Database(cls.base + name + "/")
         elif isinstance(db_names, list) and len(db_names) > 0:
             for name in db_names:
                 yield await cls.get_db(name)
@@ -156,14 +160,18 @@
             InvalidArgumentType: If the argument is not a list or Empty or No Argument was passed.
 
         Example:
             >>> async for db in AshenDB.iterate_create_dbs(["test", "test2"]):
             ...     print(db)
             <Database: test>
             <Database: test2>
+
+            >>> dbs = [db async for db in AshenDB.iterate_create_dbs()]
+            >>> dbs
+            [<Database: test>, <Database: test2>, <Database: test3>]
         """
         if db_names is None or len(db_names) == 0 or not isinstance(db_names, list):
             raise InvalidArgumentType(f"Expected list, got {type(db_names)}.")
         for name in db_names:
             yield await cls.create_one(name)
 
     @classmethod
```

### Comparing `AshenDB-0.0.3/ashendb/collection.py` & `AshenDB-0.0.4/ashendb/collection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import aiofiles, json
 import aiofiles.os as aios
 from typing import Generator
 from uuid import uuid4
 
-from .helper import match_data
+from .helper import match_data, update_data
 from .document import Document
 from .exception import *
 
 
 def gen_id() -> str:
     """Generate a random id.
 
@@ -39,32 +39,33 @@
             >>> doc
             <Document: 1>
 
             >>> doc = await coll.get_doc(query={"name": "test"})
             >>> print(doc)
             {"name": "test"}
         """
-        if id:
+        try:
             # check if the "{self.path}/{id}.json" file exists
             path = f"{self.path}/{id}.json"
             if not await aios.path.exists(path):
                 raise NotFound("No document found")
             doc = Document(path)
             await doc.__ainit__()
             return doc
-        elif query:
+        except NotFound:
             for file in await aios.scandir(self.path):
                 async with aiofiles.open(file.path, "r") as f:
                     data = json.loads(await f.read())
                     if await match_data(data, query):
                         doc = Document(file.path)
                         await doc.__ainit__()
                         return doc
             raise NotFound("No document found")
-        else:
+        except Exception as e:
+            print(e)
             raise ValueError("Either id or query must be provided")
 
     async def get_docs(
         self, ids: list[str or int] = None, query: dict = None
     ) -> list[Document]:
         """Get multiple documents.
 
@@ -129,14 +130,18 @@
             {"name": "test3"}
 
             >>> async for doc in coll.iterate_docs(query={"name": "test"}):
             ...     print(doc)
             {"name": "test1"}
             {"name": "test2"}
             {"name": "test3"}
+
+            >>> docs = [doc async for doc in coll.iterate_docs([1, 2, 3])]
+            >>> docs
+            [<Document: 1>, <Document: 2>, <Document: 3>]
         """
         if ids:
             for id in ids:
                 yield await self.get_doc(id=id)
         elif query:
             for file in await aios.scandir(self.path):
                 async with aiofiles.open(file.path, "r") as f:
@@ -241,7 +246,38 @@
             for id in ids:
                 await self.delete_doc(id)
         elif query:
             for doc in await self.get_docs(query=query):
                 await doc.delete()
         else:
             raise ValueError("Either ids or query must be provided")
+
+    async def update_doc(
+        self, id: str or int = None, query: dict = None, data: dict = None
+    ) -> Document:
+        """Update a document.
+
+        You can pass either an id or a query. If both are passed then the id will be tried first, if it fails then the query will be used.
+
+        Note:
+            Not all update operators are supported. See helper_module for more info.
+        Args:
+            id: The id of the document.
+            query: A query to match the document.
+            data: The data to update the document with.
+
+        Raises:
+            ValueError: If neither id nor query is passed.
+            NotFound: If no document is found.
+
+        Example:
+            >>> old_doc = await coll.update_doc(query={"name": "test"}}
+            >>> old_doc
+            {"name": "test"}
+            >>> await coll.update_doc(query={"name": "test"}, data={"$set":{"name": "test2"})}
+            >>> new_doc = await coll.get_doc(query={"name": "test2"})
+            >>> new_doc
+            {"name": "test2"}
+        """
+        doc = await self.get_doc(id=id, query=query)
+        new_doc = await update_data(doc, data)
+        return new_doc
```

### Comparing `AshenDB-0.0.3/ashendb/database.py` & `AshenDB-0.0.4/ashendb/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,14 +85,18 @@
             <Collection: test2>
 
             >>> async for coll in db.iterate_colls():
             ...     print(coll)
             <Collection: test>
             <Collection: test2>
             <Collection: test3>
+
+            >>> colls = [coll async for coll in db.iterate_colls()]
+            >>> colls
+            [<Collection: test>, <Collection: test2>, <Collection: test3>]
         """
         if collection_names is None or len(collection_names) == 0:
             for name in await aios.listdir(self.path):
                 yield Collection(self.path + name + "/")
         elif isinstance(collection_names, list) and len(collection_names) > 0:
             for name in collection_names:
                 yield await self.get_coll(name)
@@ -161,14 +165,18 @@
             InvalidArgumentType: If the argument is not a list or Empty or No Argument was passed.
 
         Example:
             >>> async for coll in db.iterate_create_colls(["test", "test2"]):
             ...     print(coll)
             <Collection: test>
             <Collection: test2>
+
+            >>> colls = [coll async for coll in db.iterate_create_colls(["test", "test2"])]
+            >>> colls
+            [<Collection: test>, <Collection: test2>]
         """
         if (
             collection_names is None
             or len(collection_names) == 0
             or not isinstance(collection_names, list)
         ):
             raise InvalidArgumentType(
```

### Comparing `AshenDB-0.0.3/ashendb/document.py` & `AshenDB-0.0.4/ashendb/document.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,13 +17,25 @@
             super().__init__(json.loads(contents))
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         async with aiofiles.open(self.filepath, mode="w") as f:
             contents = json.dumps(self)
             await f.write(contents)
-        self.update(json.loads(contents))
+        await self.update(json.loads(contents))
+
+    async def update(self, update: dict):
+        super().update(update)
+        async with aiofiles.open(self.filepath, mode="w") as f:
+            contents = json.dumps(self)
+            await f.write(contents)
+        return self
 
     async def save(self):
+        """Save changes made as dict
+
+        Returns:
+            Document: self
+        """
         async with aiofiles.open(self.filepath, mode="w") as f:
             contents = json.dumps(self)
             await f.write(contents)
```

### Comparing `AshenDB-0.0.3/pyproject.toml` & `AshenDB-0.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AshenDB"
-version = "0.0.3"
+version = "0.0.4"
 description = "Another stupid library for using json as Database"
 readme = "README.rst"
 authors = [{name = "Abdullah Al Muaz", email = "abdullahalmuaz15@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 1 - Planning",
     "License :: OSI Approved :: MIT License",
```

