# Comparing `tmp/redb-odm-1.1.8.tar.gz` & `tmp/redb-odm-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redb-odm-1.1.8.tar", last modified: Mon Apr 24 14:59:31 2023, max compression
+gzip compressed data, was "redb-odm-1.1.9.tar", last modified: Wed May  3 13:56:14 2023, max compression
```

## Comparing `redb-odm-1.1.8.tar` & `redb-odm-1.1.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.862716 redb-odm-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 14:59:14.000000 redb-odm-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-24 14:59:31.862716 redb-odm-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 14:59:14.000000 redb-odm-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.850715 redb-odm-1.1.8/redb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.850715 redb-odm-1.1.8/redb/behaviors/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/behaviors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/behaviors/soft_deletion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.854715 redb-odm-1.1.8/redb/core/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/core/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/core/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.854715 redb-odm-1.1.8/redb/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/interface/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.858716 redb-odm-1.1.8/redb/json_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/json_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/json_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/json_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/json_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.858716 redb-odm-1.1.8/redb/migo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/migo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/migo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/migo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/migo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.858716 redb-odm-1.1.8/redb/mongo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/mongo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/mongo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/mongo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-24 14:59:14.000000 redb-odm-1.1.8/redb/mongo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.858716 redb-odm-1.1.8/redb_odm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-24 14:59:31.000000 redb-odm-1.1.8/redb_odm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-24 14:59:31.000000 redb-odm-1.1.8/redb_odm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:59:31.000000 redb-odm-1.1.8/redb_odm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 14:59:31.000000 redb-odm-1.1.8/redb_odm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 14:59:31.000000 redb-odm-1.1.8/redb_odm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 14:59:14.000000 redb-odm-1.1.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 14:59:14.000000 redb-odm-1.1.8/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-24 14:59:14.000000 redb-odm-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:59:31.862716 redb-odm-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-24 14:59:14.000000 redb-odm-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:59:31.862716 redb-odm-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-24 14:59:14.000000 redb-odm-1.1.8/tests/test_bson_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-24 14:59:14.000000 redb-odm-1.1.8/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-24 14:59:14.000000 redb-odm-1.1.8/tests/test_json_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-04-24 14:59:14.000000 redb-odm-1.1.8/tests/test_mongo_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-24 14:59:14.000000 redb-odm-1.1.8/tests/test_return_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-24 14:59:14.000000 redb-odm-1.1.8/tests/test_soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.191357 redb-odm-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 13:55:56.000000 redb-odm-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-03 13:56:14.191357 redb-odm-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:55:56.000000 redb-odm-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.187357 redb-odm-1.1.9/redb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.187357 redb-odm-1.1.9/redb/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/behaviors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/behaviors/soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.187357 redb-odm-1.1.9/redb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/core/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/core/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.187357 redb-odm-1.1.9/redb/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/interface/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.187357 redb-odm-1.1.9/redb/json_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/json_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/json_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/json_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/json_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.187357 redb-odm-1.1.9/redb/migo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/migo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/migo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/migo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/migo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.191357 redb-odm-1.1.9/redb/mongo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/mongo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/mongo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/mongo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-03 13:55:56.000000 redb-odm-1.1.9/redb/mongo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.191357 redb-odm-1.1.9/redb_odm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-03 13:56:14.000000 redb-odm-1.1.9/redb_odm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-03 13:56:14.000000 redb-odm-1.1.9/redb_odm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:56:14.000000 redb-odm-1.1.9/redb_odm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 13:56:14.000000 redb-odm-1.1.9/redb_odm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 13:56:14.000000 redb-odm-1.1.9/redb_odm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 13:55:56.000000 redb-odm-1.1.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 13:55:56.000000 redb-odm-1.1.9/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 13:55:56.000000 redb-odm-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:56:14.191357 redb-odm-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-03 13:55:56.000000 redb-odm-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:14.191357 redb-odm-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-03 13:55:56.000000 redb-odm-1.1.9/tests/test_bson_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-03 13:55:56.000000 redb-odm-1.1.9/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-03 13:55:56.000000 redb-odm-1.1.9/tests/test_json_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-03 13:55:56.000000 redb-odm-1.1.9/tests/test_mongo_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-03 13:55:56.000000 redb-odm-1.1.9/tests/test_return_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-03 13:55:56.000000 redb-odm-1.1.9/tests/test_soft_deletion.py
```

### Comparing `redb-odm-1.1.8/redb/behaviors/soft_deletion.py` & `redb-odm-1.1.9/redb/behaviors/soft_deletion.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/core/base.py` & `redb-odm-1.1.9/redb/core/base.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/core/document.py` & `redb-odm-1.1.9/redb/core/document.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/core/instance.py` & `redb-odm-1.1.9/redb/core/instance.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/core/transaction.py` & `redb-odm-1.1.9/redb/core/transaction.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/core/utils.py` & `redb-odm-1.1.9/redb/core/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,26 @@
+import types
 from enum import Enum
 from typing import Any, Type, TypeVar
 
 from pydantic import BaseModel
+from pydantic.fields import ModelField
 
 T = TypeVar("T", bound=BaseModel)
 
-
-DEFAULT_VALUES = {"str": "string", "float": 0.0, "int": 0, "dict": {}, "list": []}
+DEFAULT_CONTAINER_VALUES = {"list": [], "tuple": (), "set": set()}
+DEFAULT_PRIMITIVE_VALUES = {
+    "str": "string",
+    "float": 0.0,
+    "int": 0,
+    "bool": False,
+    "None": None,
+    "bytes": b"",
+}
+DEFAULT_VALUES = DEFAULT_PRIMITIVE_VALUES | DEFAULT_CONTAINER_VALUES
 
 
 def generate_examples(pydantic_models: list[Type[T]]) -> dict[str, dict[str, Any]]:
     out = {}
     for model in pydantic_models:
         example = get_example_from_pydantic(model)
         out[example["summary"]] = example
@@ -40,30 +50,63 @@
 
 
 def _get_value(pydantic_model: Type[T]) -> dict:
     value = {}
     for name, field in pydantic_model.__fields__.items():
         if field.default is not None or field.default_factory is not None:
             field_value = field.default
-            if field_value is None:
+            if field_value is None and field.default_factory is not None:
                 field_value = field.default_factory()
 
             if isinstance(field_value, Enum):
                 field_value = field_value.value
             elif isinstance(field_value, BaseModel):
                 field_value = _get_value(field_value.__class__)
 
             value[name] = field_value
             continue
 
-        if issubclass(field.type_, BaseModel):
-            value[name] = _get_value(field.type_)
-        elif issubclass(field.type_, Enum):
-            value[name] = next(iter(field.type_)).value
-        elif field.outer_type_.__name__ in DEFAULT_VALUES:
-            value[name] = DEFAULT_VALUES[field.outer_type_.__name__]
-        elif field.type_.__name__ in DEFAULT_VALUES:
-            value[name] = DEFAULT_VALUES[field.type_.__name__]
-        else:
-            value[name] = field.type_.__name__
+        value[name] = _parse_value(field)
+
+    return value
+
 
+def _parse_value(field: ModelField):
+    value = None
+    if isinstance(field.type_, types.UnionType):
+        field.type_ = field.type_.__args__[0]
+
+    if isinstance(field.outer_type_, types.UnionType):
+        field.outer_type_ = field.outer_type_.__args__[0]
+
+    if field.type_.__name__ in DEFAULT_CONTAINER_VALUES:
+        try:
+            tmp = field.type_
+            field.type_ = field.type_.__args__[0]
+            field.outer_type_ = tmp
+        except:
+            return DEFAULT_CONTAINER_VALUES[field.type_.__name__]
+
+    if field.type_.__name__ in DEFAULT_PRIMITIVE_VALUES:
+        value = DEFAULT_PRIMITIVE_VALUES[field.type_.__name__]
+    elif issubclass(field.type_, BaseModel):
+        value = _get_value(field.type_)
+    elif issubclass(field.type_, Enum):
+        value = next(iter(field.type_)).value
+    else:
+        value = field.type_.__name__
+
+    if field.outer_type_.__name__ in DEFAULT_CONTAINER_VALUES:
+        value = _build_container(value, field)
+    
     return value
+        
+
+
+def _build_container(value: Any, field: ModelField):
+    if field.outer_type_.__name__ == "list":
+        return [value] if value is not None else []
+    elif field.outer_type_.__name__ == "set":
+        return {value,} if value is not None else set()
+    elif field.outer_type_.__name__ == "tuple":
+        return (value,) if value is not None else tuple()
+    return value
```

### Comparing `redb-odm-1.1.8/redb/interface/client.py` & `redb-odm-1.1.9/redb/interface/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/interface/collection.py` & `redb-odm-1.1.9/redb/interface/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/interface/configs.py` & `redb-odm-1.1.9/redb/interface/configs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/interface/database.py` & `redb-odm-1.1.9/redb/interface/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/interface/fields.py` & `redb-odm-1.1.9/redb/interface/fields.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/interface/results.py` & `redb-odm-1.1.9/redb/interface/results.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/json_system/client.py` & `redb-odm-1.1.9/redb/json_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/json_system/collection.py` & `redb-odm-1.1.9/redb/json_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/json_system/database.py` & `redb-odm-1.1.9/redb/json_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/migo_system/client.py` & `redb-odm-1.1.9/redb/migo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/migo_system/collection.py` & `redb-odm-1.1.9/redb/migo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/migo_system/database.py` & `redb-odm-1.1.9/redb/migo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/mongo_system/client.py` & `redb-odm-1.1.9/redb/mongo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/mongo_system/collection.py` & `redb-odm-1.1.9/redb/mongo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb/mongo_system/database.py` & `redb-odm-1.1.9/redb/mongo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/redb_odm.egg-info/SOURCES.txt` & `redb-odm-1.1.9/redb_odm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/setup.py` & `redb-odm-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/tests/test_bson_objs.py` & `redb-odm-1.1.9/tests/test_bson_objs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/tests/test_hashing.py` & `redb-odm-1.1.9/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/tests/test_json_client.py` & `redb-odm-1.1.9/tests/test_json_client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/tests/test_mongo_system.py` & `redb-odm-1.1.9/tests/test_mongo_system.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/tests/test_return_cls.py` & `redb-odm-1.1.9/tests/test_return_cls.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.1.8/tests/test_soft_deletion.py` & `redb-odm-1.1.9/tests/test_soft_deletion.py`

 * *Files identical despite different names*

