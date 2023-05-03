# Comparing `tmp/easy_crud_repo_service-0.1.1.tar.gz` & `tmp/easy_crud_repo_service-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_crud_repo_service-0.1.1.tar", max compression
+gzip compressed data, was "easy_crud_repo_service-0.1.2.tar", max compression
```

## Comparing `easy_crud_repo_service-0.1.1.tar` & `easy_crud_repo_service-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-04-23 19:13:52.339918 easy_crud_repo_service-0.1.1/easy_crud_repo_service/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 19:59:22.482391 easy_crud_repo_service-0.1.1/easy_crud_repo_service/model/__init__.py
--rw-r--r--   0        0        0      183 2023-04-23 20:02:18.331784 easy_crud_repo_service-0.1.1/easy_crud_repo_service/model/player.py
--rw-r--r--   0        0        0      146 2023-04-23 20:02:18.341597 easy_crud_repo_service-0.1.1/easy_crud_repo_service/model/team.py
--rw-r--r--   0        0        0        0 2023-04-23 20:00:48.714154 easy_crud_repo_service-0.1.1/easy_crud_repo_service/repo/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 20:36:23.143148 easy_crud_repo_service-0.1.1/easy_crud_repo_service/repo/connections/__init__.py
--rw-r--r--   0        0        0     3560 2023-05-01 09:50:13.152568 easy_crud_repo_service-0.1.1/easy_crud_repo_service/repo/connections/builders.py
--rw-r--r--   0        0        0     1044 2023-05-01 10:25:18.841964 easy_crud_repo_service-0.1.1/easy_crud_repo_service/repo/connections/get_connection_pool.py
--rw-r--r--   0        0        0     5106 2023-05-01 11:13:02.644420 easy_crud_repo_service-0.1.1/easy_crud_repo_service/repo/crud_repo.py
--rw-r--r--   0        0        0      582 2023-05-01 18:06:47.718354 easy_crud_repo_service-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    12849 2023-05-01 15:30:38.823058 easy_crud_repo_service-0.1.1/README.md
--rw-r--r--   0        0        0    12991 1970-01-01 00:00:00.000000 easy_crud_repo_service-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-23 19:13:52.339918 easy_crud_repo_service-0.1.2/easy_crud_repo_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:59:22.482391 easy_crud_repo_service-0.1.2/easy_crud_repo_service/model/__init__.py
+-rw-r--r--   0        0        0      183 2023-04-23 20:02:18.331784 easy_crud_repo_service-0.1.2/easy_crud_repo_service/model/player.py
+-rw-r--r--   0        0        0      146 2023-04-23 20:02:18.341597 easy_crud_repo_service-0.1.2/easy_crud_repo_service/model/team.py
+-rw-r--r--   0        0        0        0 2023-04-23 20:00:48.714154 easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-23 20:36:23.143148 easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/connections/__init__.py
+-rw-r--r--   0        0        0     3974 2023-05-03 04:14:11.478426 easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/connections/builders.py
+-rw-r--r--   0        0        0     1121 2023-05-03 04:14:11.503306 easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/connections/get_connection_pool.py
+-rw-r--r--   0        0        0     5605 2023-05-03 04:20:43.332850 easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/crud_repo.py
+-rw-r--r--   0        0        0      582 2023-05-03 04:56:01.714891 easy_crud_repo_service-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9657 2023-05-03 04:07:14.199155 easy_crud_repo_service-0.1.2/README.md
+-rw-r--r--   0        0        0     9862 1970-01-01 00:00:00.000000 easy_crud_repo_service-0.1.2/PKG-INFO
```

### Comparing `easy_crud_repo_service-0.1.1/easy_crud_repo_service/repo/connections/builders.py` & `easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/connections/builders.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,46 +37,55 @@
                 'password': {Constraint.IS_TYPE: str},
                 'port': {Constraint.IS_TYPE: int},
             })
         except TypeError:
             raise ConnectionError("File is invalid or doesn't exist")
 
     def set_pool_name(self, new_pool_name: str) -> Self:
+        """ Setting up new pool name"""
         self._pool_config_['pool_name'] = new_pool_name
         return self
 
     def set_pool_size(self, new_size: int) -> Self:
+        """ Setting up new pool size"""
         self._pool_config_['pool_size'] = new_size
         return self
 
     def set_pool_reset_session(self, new_pool_reset_session: bool) -> Self:
+        """ Setting up new value for pool_reset_session"""
         self._pool_config_['pool_reset_session'] = new_pool_reset_session
         return self
 
     def set_new_host(self, new_host: str) -> Self:
+        """ Setting up new host"""
         self._pool_config_['host'] = new_host
         return self
 
     def set_new_database(self, new_database: str) -> Self:
+        """ Setting up new db name"""
         self._pool_config_['database'] = new_database
         return self
 
     def set_username(self, new_username: str) -> Self:
+        """ Setting up new username"""
         self._pool_config_['user'] = new_username
         return self
 
     def set_password(self, new_password: str) -> Self:
+        """ Setting up new password"""
         self._pool_config_['password'] = new_password
         return self
 
     def set_new_port(self, new_port: int) -> Self:
+        """ Setting up new port"""
         self._pool_config_['port'] = new_port
         return self
 
     def build(self) -> MySQLConnectionPool:
+        """ Validation of _pool_config_ dict and creation of connection pool"""
         validate_json_data(self._pool_config_, constraints={
             'pool_name': {Constraint.IS_TYPE: str},
             'pool_size': {Constraint.IS_TYPE: int},
             'pool_reset_session': {Constraint.IS_TYPE: bool},
             'host': {Constraint.IS_TYPE: str},
             'database': {Constraint.IS_TYPE: str},
             'user': {Constraint.IS_TYPE: str},
```

### Comparing `easy_crud_repo_service-0.1.1/easy_crud_repo_service/repo/connections/get_connection_pool.py` & `easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/connections/get_connection_pool.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 
 def get_connection_pool(absolute_dotenv_path: str) -> MySQLConnectionPool:
     """ Function creates and returns connection pool for MySQLDatabase using variables stored in .env file"""
     for v in ['POOL_NAME', 'POOL_SIZE', 'POOL_RESET_SESSION', 'HOST', 'DATABASE', 'USER', 'PASSWORD', 'PORT']:
         if v in os.environ:
             del os.environ[v]
+    # loading of .env file
     load_dotenv(absolute_dotenv_path, override=True)
+    # attempt of creation a new connection pool
     try:
         return MySQLConnectionPool(
             pool_name=os.getenv('POOL_NAME'),
             pool_size=int(os.getenv('POOL_SIZE')),
             pool_reset_session=bool(os.getenv('POOL_RESET_SESSION')),
             host=os.getenv('HOST'),
             database=os.getenv('DATABASE'),
```

### Comparing `easy_crud_repo_service-0.1.1/easy_crud_repo_service/repo/crud_repo.py` & `easy_crud_repo_service-0.1.2/easy_crud_repo_service/repo/crud_repo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,123 +1,123 @@
 import inflection
-import logging
-
 from datetime import datetime, date
-from dotenv import load_dotenv
-from mysql.connector import pooling, Error
 from typing import Any
 from contextlib import contextmanager
 
-logging.basicConfig(level=logging.DEBUG, handlers=[logging.StreamHandler()])
-
-load_dotenv()
-
+from mysql.connector import pooling, Error
 
 class CrudRepo:
 
     def __init__(self, connection_pool: pooling.MySQLConnectionPool,  entity: type) -> None:
         self._connection_pool = connection_pool
         self._entity = entity
         self._entity_type = type(entity())
 
     @contextmanager
     def _get_cursor_object(self):
+        """ Context manager that allows us to work on cursor in safe manner """
         connection_object = self._connection_pool.get_connection()
 
         try:
             if connection_object.is_connected():
                 cursor_object = connection_object.cursor()
-                logging.debug(cursor_object)
                 yield cursor_object
-                logging.debug(cursor_object)
                 connection_object.commit()
         except Error as e:
             connection_object.rollback()
         finally:
             if connection_object.is_connected():
                 cursor_object.close()
                 connection_object.close()
 
     def _table_name(self) -> str:
-        # ta biblioteka pomaga w pracy na stringach, .tableize(), jeśli dostanie Car to zwróci cars
+        """ Creates table name using inflection.tableize() that will change expression for lowercase plural"""
         return inflection.tableize(self._entity_type.__name__)
 
     def _fields_names(self) -> list[str]:
-        # dict zwraca namespaces, keys() wyciąga tylko nazwy
+        """ Returns namespace keys of entity"""
         return list(self._entity().__dict__.keys())
 
     def _column_names_for_insert(self) -> str:
-        # zwraca wszystkie nazwy poza id
+        """ Returns all namespace keys of entity accept id"""
         return ', '.join([field for field in self._fields_names() if field.lower() != 'id'])
 
     def insert(self, item: Any) -> int:
+        """ Inserts one new row into database table """
         with self._get_cursor_object() as cur:
             sql = f'insert into {self._table_name()} ' \
                   f'({self._column_names_for_insert()}) ' \
                   f'values ({self._column_values_for_insert(item)});'
             cur.execute(sql)
             return cur.lastrowid
 
     def insert_many(self, items: list[Any]) -> list[int]:
+        """ Inserts multiple new rows into database table """
         with self._get_cursor_object() as cur:
             values = ", ".join([f"({CrudRepo._column_values_for_insert(item)})" for item in items])
             sql = f"insert into {self._table_name()} ({self._column_names_for_insert()}) values {values}"
             cur.execute(sql)
             return [item.id for item in self.find_n_last(len(items))]
 
     def update(self, item_id: int, item: Any) -> Any:
+        """ Updates database table row using provided id and object containing new values"""
         with self._get_cursor_object() as cur:
             sql = f"update {self._table_name()} set {CrudRepo._column_names_and_values_for_update(item)} where id = {item_id}"
-            logging.debug(sql)
             cur.execute(sql)
             return self.find_one(item_id)
 
-    def find_n_last(self, n) -> list[Any]:
+    def find_n_last(self, n: int) -> list[Any]:
+        """ Finds n last rows in table """
         with self._get_cursor_object() as cur:
             sql = f'select * from {self._table_name()} order by id desc limit {n}'
             cur.execute(sql)
             return [self._entity(*row) for row in cur.fetchall()]
 
     def find_one(self, item_id: int) -> Any:
+        """ Finds one row in table using provided id"""
         with self._get_cursor_object() as cur:
             sql = f"select * from {self._table_name()} where id = {item_id}"
             cur.execute(sql)
             result = cur.fetchone()
             if not result:
                 raise RuntimeError(f"Item with id {item_id} wasn't found")
             return self._entity(*result)
 
     def find_all(self) -> list[Any]:
+        """ Finds all rows in table """
         with self._get_cursor_object() as cur:
             sql = f"select * from {self._table_name()}"
             cur.execute(sql)
             return [self._entity(*row) for row in cur.fetchall()]
 
-    def delete_one(self, item_id) -> int:
+    def delete_one(self, item_id: int) -> int:
+        """ Deletes one row in table using provided id"""
         with self._get_cursor_object() as cur:
             sql = f"delete from {self._table_name()} where id = {item_id}"
             self.find_one(item_id)
             cur.execute(sql)
             return item_id
 
     def delete_all(self) -> list[int]:
+        """ Deletes all rows from a table """
         with self._get_cursor_object() as cur:
             all_deleted_items = [item.id for item in self.find_all()]
             sql = f'delete from {self._table_name()} where id >= 1'
             cur.execute(sql)
             return all_deleted_items
 
     @classmethod
     def _column_values_for_insert(cls, item: Any) -> str:
-
+        """ Creates expression with values that we want to put into sql. (All accept id) """
         def to_str(entry: Any) -> str:
             # funkcja pomocnicza, która zwraca f-string z wartością jeżeli jest ona napisem albo datą
             return f"'{entry[1]}'" if isinstance(entry[1], (str, datetime, date)) else str(entry[1])
 
         return ", ".join([to_str(entry) for entry in item.__dict__.items() if entry[0].lower() != 'id'])
 
     @classmethod
     def _column_names_and_values_for_update(cls, entity) -> str:
+        """ Method creates expression that will be responsible for updating row values. (All accept id) """
         def to_str(entry: Any) -> str:
             return entry[0] + '=' + (f"'{entry[1]}'" if isinstance(entry[1], (str, datetime, date)) else str(entry[1]))
 
         return ', '.join([to_str(item) for item in entity.__dict__.items() if item[0].lower() != 'id'])
```

### Comparing `easy_crud_repo_service-0.1.1/pyproject.toml` & `easy_crud_repo_service-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy-crud-repo-service"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Smolke <d.smolczynski1@gmail.com>"]
 readme = "README.md"
 packages = [{include = "easy_crud_repo_service"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

