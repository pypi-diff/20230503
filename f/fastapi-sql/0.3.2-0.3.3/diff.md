# Comparing `tmp/fastapi_sql-0.3.2.tar.gz` & `tmp/fastapi_sql-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sql-0.3.2.tar", max compression
+gzip compressed data, was "fastapi_sql-0.3.3.tar", max compression
```

## Comparing `fastapi_sql-0.3.2.tar` & `fastapi_sql-0.3.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2735 2023-04-29 15:45:15.036947 fastapi_sql-0.3.2/fastapi_sql/__init__.py
--rw-r--r--   0        0        0      771 2023-04-28 17:38:33.791293 fastapi_sql-0.3.2/fastapi_sql/middleware.py
--rw-r--r--   0        0        0     1562 2023-04-29 15:43:30.819501 fastapi_sql-0.3.2/fastapi_sql/migrate.py
--rw-r--r--   0        0        0     5135 2023-04-27 18:51:50.354029 fastapi_sql-0.3.2/fastapi_sql/model.py
--rw-r--r--   0        0        0      417 2023-05-01 18:43:47.293365 fastapi_sql-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 fastapi_sql-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2818 2023-05-03 16:42:04.761041 fastapi_sql-0.3.3/fastapi_sql/__init__.py
+-rw-r--r--   0        0        0      771 2023-04-28 17:38:33.791293 fastapi_sql-0.3.3/fastapi_sql/middleware.py
+-rw-r--r--   0        0        0     1562 2023-04-29 15:43:30.819501 fastapi_sql-0.3.3/fastapi_sql/migrate.py
+-rw-r--r--   0        0        0     5135 2023-04-27 18:51:50.354029 fastapi_sql-0.3.3/fastapi_sql/model.py
+-rw-r--r--   0        0        0      417 2023-05-03 16:44:48.822864 fastapi_sql-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 fastapi_sql-0.3.3/PKG-INFO
```

### Comparing `fastapi_sql-0.3.2/fastapi_sql/__init__.py` & `fastapi_sql-0.3.3/fastapi_sql/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from typing import Any, Type
 
 from sqlalchemy.ext.asyncio import (AsyncEngine, AsyncSession, async_sessionmaker,
                                     create_async_engine)
-from sqlalchemy import MetaData, Table, Column, Integer, Text, String, DateTime, Date, select
+from sqlalchemy import MetaData, Table, Column, Integer, Text, String, DateTime, Date, select, ForeignKey
 from sqlalchemy.sql import Select
 from sqlalchemy.orm import declarative_base
 from .model import Model as DefaultModel, DefaultMeta
 from .migrate import Migration
 from fastapi import FastAPI
 from .middleware import Middleware
 
 
 class SQLAlchemy:
     __engine__: AsyncEngine
     session: AsyncSession
-    __metadata__: MetaData
+    __metadata__: MetaData = None
     migration = Migration
     __naming_conventions__: 'dict[str, str]' = {
         "ix": "ix_%(column_0_label)s",
         "uq": "uq_%(table_name)s_%(column_0_name)s",
         "ck": "ck_%(table_name)s_%(constraint_name)s",
         "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
         "pk": "pk_%(table_name)s"
     }
     
     middleware = Middleware
     
     Model: DefaultModel
-    Table = Table
+    ForeignKey = ForeignKey
     
     Column = Column
     Integer = Integer
     Text = Text
     String = String
     DateTime = DateTime
     Date = Date
@@ -42,15 +42,16 @@
         self.__sessionmaker__ = async_sessionmaker(
                     bind=self.__engine__, 
                     autoflush=session_options.get('session_autoflush', True),
                     expire_on_commit=session_options.get('expire_on_commit', True)
         )
         if kwargs.get('naming_convention') is not None:
             self.__naming_conventions__ = kwargs.get('naming_convention', {})
-        self.__metadata__ = MetaData(naming_convention=self.__naming_conventions__)
+        if SQLAlchemy.__metadata__ is None:
+            SQLAlchemy.__metadata__ = MetaData(naming_convention=self.__naming_conventions__)
         self.Model = self._make_declarative_base() # type: ignore
         self.__engine_uri__ = database_uri
         self.migration.cfg.set_main_option('sqlalchemy.url', database_uri)
         self.migration.cfg.config_file_name = 'alembic.ini'
         if app is not None:
             app.add_middleware(self.middleware, sqlalchemy=self)
```

### Comparing `fastapi_sql-0.3.2/fastapi_sql/middleware.py` & `fastapi_sql-0.3.3/fastapi_sql/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.2/fastapi_sql/migrate.py` & `fastapi_sql-0.3.3/fastapi_sql/migrate.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.2/fastapi_sql/model.py` & `fastapi_sql-0.3.3/fastapi_sql/model.py`

 * *Files identical despite different names*

### Comparing `fastapi_sql-0.3.2/PKG-INFO` & `fastapi_sql-0.3.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Author: Michael Piccirillo
 Author-email: 70709374+Khrysys@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

