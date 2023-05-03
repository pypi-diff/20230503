# Comparing `tmp/ddb_single-0.3.3.tar.gz` & `tmp/ddb_single-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddb_single-0.3.3.tar", last modified: Wed Feb 15 12:07:44 2023, max compression
+gzip compressed data, was "ddb_single-0.3.5.tar", last modified: Wed May  3 02:20:12 2023, max compression
```

## Comparing `ddb_single-0.3.3.tar` & `ddb_single-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 12:07:44.042202 ddb_single-0.3.3/
--rw-rw-rw-   0        0        0     9190 2023-02-15 12:07:44.042202 ddb_single-0.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-15 12:07:44.031201 ddb_single-0.3.3/ddb_single/
--rw-rw-rw-   0        0        0      144 2023-02-15 12:07:39.000000 ddb_single-0.3.3/ddb_single/__init__.py
--rw-rw-rw-   0        0        0    13297 2023-02-15 12:06:42.000000 ddb_single-0.3.3/ddb_single/model.py
--rw-rw-rw-   0        0        0     8953 2023-02-15 10:25:48.000000 ddb_single-0.3.3/ddb_single/query.py
--rw-rw-rw-   0        0        0    21654 2023-02-15 10:26:02.000000 ddb_single-0.3.3/ddb_single/table.py
--rw-rw-rw-   0        0        0     5899 2022-10-02 09:32:13.000000 ddb_single-0.3.3/ddb_single/utils_botos.py
-drwxrwxrwx   0        0        0        0 2023-02-15 12:07:44.041202 ddb_single-0.3.3/ddb_single.egg-info/
--rw-rw-rw-   0        0        0     9190 2023-02-15 12:07:43.000000 ddb_single-0.3.3/ddb_single.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-02-15 12:07:43.000000 ddb_single-0.3.3/ddb_single.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 12:07:43.000000 ddb_single-0.3.3/ddb_single.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-02-15 12:07:43.000000 ddb_single-0.3.3/ddb_single.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-15 12:07:43.000000 ddb_single-0.3.3/ddb_single.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-15 12:07:44.042202 ddb_single-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      671 2022-10-02 11:49:36.000000 ddb_single-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 02:20:12.909037 ddb_single-0.3.5/
+-rw-rw-rw-   0        0        0     9190 2023-05-03 02:20:12.909037 ddb_single-0.3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 02:20:12.888368 ddb_single-0.3.5/ddb_single/
+-rw-rw-rw-   0        0        0      144 2023-04-30 13:12:32.000000 ddb_single-0.3.5/ddb_single/__init__.py
+-rw-rw-rw-   0        0        0    13297 2023-02-15 12:06:42.000000 ddb_single-0.3.5/ddb_single/model.py
+-rw-rw-rw-   0        0        0     8975 2023-04-30 12:08:38.000000 ddb_single-0.3.5/ddb_single/query.py
+-rw-rw-rw-   0        0        0    21668 2023-04-30 13:12:19.000000 ddb_single-0.3.5/ddb_single/table.py
+-rw-rw-rw-   0        0        0     5899 2022-10-02 09:32:13.000000 ddb_single-0.3.5/ddb_single/utils_botos.py
+drwxrwxrwx   0        0        0        0 2023-05-03 02:20:12.906519 ddb_single-0.3.5/ddb_single.egg-info/
+-rw-rw-rw-   0        0        0     9190 2023-05-03 02:20:12.000000 ddb_single-0.3.5/ddb_single.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-05-03 02:20:12.000000 ddb_single-0.3.5/ddb_single.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 02:20:12.000000 ddb_single-0.3.5/ddb_single.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-03 02:20:12.000000 ddb_single-0.3.5/ddb_single.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 02:20:12.000000 ddb_single-0.3.5/ddb_single.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 02:20:12.909037 ddb_single-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      671 2022-10-02 11:49:36.000000 ddb_single-0.3.5/setup.py
```

### Comparing `ddb_single-0.3.3/PKG-INFO` & `ddb_single-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddb_single
-Version: 0.3.3
+Version: 0.3.5
 Summary: Python DynamoDB interface, specialized in single-table design.
 Home-page: https://github.com/medaka0213/DynamoDB-SingleTable
 Author: medaka
 License: MIT
 Keywords: aws dynamodb serverless
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ddb_single-0.3.3/ddb_single/model.py` & `ddb_single-0.3.5/ddb_single/model.py`

 * *Files identical despite different names*

### Comparing `ddb_single-0.3.3/ddb_single/query.py` & `ddb_single-0.3.5/ddb_single/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         return self.__model__.data[self.__model__.__unique_keys__[0]]
 
     def _search_items(self):
         items_add = []
         items_remove = []
         for k in self.__model__.__search_keys__:
             field:DBField = self.__model__.__class__.__dict__[k]
-            if k in self.__model__.data.keys() and field.value is not None:
+            if k in self.__model__.data.keys() and field.value is not None and field.value != "":
                 items_add.append(field.search_item(self.__model__.data[self.__model__.__primary_key__]))
             else:
                 items_remove.append(field.search_item(self.__model__.data[self.__model__.__primary_key__]))
         return items_add, items_remove
 
     # 検索
     def search(self, *queries, pk_only=False):
```

### Comparing `ddb_single-0.3.3/ddb_single/table.py` & `ddb_single-0.3.5/ddb_single/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
                     res_data += response['Items']
                 return util_b.json_export(res_data)
             else:
                 return []
 
     # クエリ
     def _query(self, **kwargs):
-        limit = kwargs.get("Limit")
+        limit = kwargs.get("Limit", float('inf'))
         try:
             response = self.__table__.query(**kwargs)
         except ClientError as e:
             traceback.print_exc()
         else:
             if len(response['Items']):
                 res_data =  response['Items']
```

### Comparing `ddb_single-0.3.3/ddb_single/utils_botos.py` & `ddb_single-0.3.5/ddb_single/utils_botos.py`

 * *Files identical despite different names*

### Comparing `ddb_single-0.3.3/ddb_single.egg-info/PKG-INFO` & `ddb_single-0.3.5/ddb_single.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddb-single
-Version: 0.3.3
+Version: 0.3.5
 Summary: Python DynamoDB interface, specialized in single-table design.
 Home-page: https://github.com/medaka0213/DynamoDB-SingleTable
 Author: medaka
 License: MIT
 Keywords: aws dynamodb serverless
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ddb_single-0.3.3/setup.py` & `ddb_single-0.3.5/setup.py`

 * *Files identical despite different names*

