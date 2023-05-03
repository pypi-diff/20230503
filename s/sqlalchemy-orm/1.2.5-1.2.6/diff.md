# Comparing `tmp/sqlalchemy-orm-1.2.5.tar.gz` & `tmp/sqlalchemy-orm-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-orm-1.2.5.tar", last modified: Thu Apr  6 23:15:31 2023, max compression
+gzip compressed data, was "sqlalchemy-orm-1.2.6.tar", last modified: Wed May  3 13:54:40 2023, max compression
```

## Comparing `sqlalchemy-orm-1.2.5.tar` & `sqlalchemy-orm-1.2.6.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 23:15:31.684888 sqlalchemy-orm-1.2.5/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1704 2023-04-06 23:15:31.684888 sqlalchemy-orm-1.2.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1036 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-06 23:15:31.000000 sqlalchemy-orm-1.2.5/VERSION
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-06 23:15:31.684888 sqlalchemy-orm-1.2.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1360 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 23:15:31.676888 sqlalchemy-orm-1.2.5/sqlalchemy_orm/
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 23:15:31.680888 sqlalchemy-orm-1.2.5/sqlalchemy_orm/base/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/base/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1184 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/base/base.py
--rwxrwxrwx   0 root         (0) root         (0)     4581 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/base/helper.py
--rwxrwxrwx   0 root         (0) root         (0)      655 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/base/inheritance.py
--rwxrwxrwx   0 root         (0) root         (0)     9913 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/base/mapper.py
--rw-rw-rw-   0 root         (0) root         (0)     1778 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/custom_types.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/database.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 23:15:31.682888 sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/cst.py
--rw-rw-rw-   0 root         (0) root         (0)     1325 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    10433 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/main.py
--rw-rw-rw-   0 root         (0) root         (0)     6250 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5233 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/sqla.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/version.py
--rwxrwxrwx   0 root         (0) root         (0)     1430 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/filter.py
--rwxrwxrwx   0 root         (0) root         (0)     1319 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/order_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 23:15:31.683888 sqlalchemy-orm-1.2.5/sqlalchemy_orm/patterns/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/patterns/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3855 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/patterns/tag.py
--rwxrwxrwx   0 root         (0) root         (0)     1814 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/patterns/tag_mixin.py
--rwxrwxrwx   0 root         (0) root         (0)      143 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/patterns/taggable.py
--rw-rw-rw-   0 root         (0) root         (0)     4982 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/query.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/session.py
--rw-rw-rw-   0 root         (0) root         (0)     2351 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/typemapper.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2023-04-06 23:15:21.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 23:15:31.678888 sqlalchemy-orm-1.2.5/sqlalchemy_orm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1704 2023-04-06 23:15:31.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1081 2023-04-06 23:15:31.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 23:15:31.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2023-04-06 23:15:31.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-06 23:15:31.000000 sqlalchemy-orm-1.2.5/sqlalchemy_orm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:54:40.118427 sqlalchemy-orm-1.2.6/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-03 13:54:40.118427 sqlalchemy-orm-1.2.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1036 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-03 13:54:39.000000 sqlalchemy-orm-1.2.6/VERSION
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-03 13:54:40.119427 sqlalchemy-orm-1.2.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:54:40.111426 sqlalchemy-orm-1.2.6/sqlalchemy_orm/
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:54:40.114426 sqlalchemy-orm-1.2.6/sqlalchemy_orm/base/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/base/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      855 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/base/base.py
+-rwxrwxrwx   0 root         (0) root         (0)    14522 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/base/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/base/mapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1779 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/custom_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6265 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:54:40.117427 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/cst.py
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    10155 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6089 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5089 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2732 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/sqla.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/version.py
+-rwxrwxrwx   0 root         (0) root         (0)     1401 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     1264 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/order_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:54:40.118427 sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3635 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/tag.py
+-rwxrwxrwx   0 root         (0) root         (0)     1718 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/tag_mixin.py
+-rwxrwxrwx   0 root         (0) root         (0)      143 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/taggable.py
+-rw-rw-rw-   0 root         (0) root         (0)     4983 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/query.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     2361 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/typemapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2023-05-03 13:54:29.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 13:54:40.113426 sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-03 13:54:40.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-05-03 13:54:40.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 13:54:40.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-03 13:54:40.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-03 13:54:40.000000 sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/top_level.txt
```

### Comparing `sqlalchemy-orm-1.2.5/LICENSE` & `sqlalchemy-orm-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.5/PKG-INFO` & `sqlalchemy-orm-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-orm
-Version: 1.2.5
+Version: 1.2.6
 Summary: Data Relation Mapping framework for Python.
 Home-page: https://gitlab.com/parob/sqlalchemy-orm
-Download-URL: https://gitlab.com/parob/sqlalchemy-orm/-/archive/v1.2.5/sqlalchemy-orm-v1.2.5.tar.gz
+Download-URL: https://gitlab.com/parob/sqlalchemy-orm/-/archive/v1.2.6/sqlalchemy-orm-v1.2.6.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: SQLAlchemy,ORM
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlalchemy-orm-1.2.5/README.md` & `sqlalchemy-orm-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.5/setup.py` & `sqlalchemy-orm-1.2.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,37 @@
 import io
 
 from setuptools import setup, find_packages
 
-with io.open('README.md', 'rt', encoding='utf8') as f:
+with io.open("README.md", "rt", encoding="utf8") as f:
     readme = f.read()
 
-with io.open('VERSION') as version_file:
+with io.open("VERSION") as version_file:
     version = version_file.read().strip().lower()
     if version.startswith("v"):
         version = version[1:]
 
 setup(
-    name='sqlalchemy-orm',
+    name="sqlalchemy-orm",
     version=version,
-    license='MIT',
+    license="MIT",
     packages=find_packages(),
     include_package_data=True,
-    author='Robert Parker',
-    author_email='rob@parob.com',
-    url='https://gitlab.com/parob/sqlalchemy-orm',
-    download_url=f'https://gitlab.com/parob/sqlalchemy-orm/-/archive/v{version}/sqlalchemy-orm-v{version}.tar.gz',
-    keywords=['SQLAlchemy', 'ORM'],
-    description='Data Relation Mapping framework for Python.',
+    author="Robert Parker",
+    author_email="rob@parob.com",
+    url="https://gitlab.com/parob/sqlalchemy-orm",
+    download_url=f"https://gitlab.com/parob/sqlalchemy-orm/-/archive/v{version}"
+                 f"/sqlalchemy-orm-v{version}.tar.gz",
+    keywords=["SQLAlchemy", "ORM"],
+    description="Data Relation Mapping framework for Python.",
     long_description=readme,
-    long_description_content_type='text/markdown',
-    install_requires=[
-        'SQLAlchemy',
-        'inflection',
-        'cached-property',
-        'typing_inspect'
-    ],
-    extras_require={
-        'dev': [
-            'pytest',
-            'pytest-cov',
-            'coverage',
-            'faker'
-        ]
-    },
+    long_description_content_type="text/markdown",
+    install_requires=["SQLAlchemy", "inflection", "cached-property", "typing_inspect"],
+    extras_require={"dev": ["pytest", "pytest-cov", "coverage", "faker"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
-
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/base/base.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/base/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,34 @@
-from typing import Callable, Type
+from typing import Type
 
 from sqlalchemy.orm.decl_api import declarative_base, DeclarativeMeta
 
-from sqlalchemy_orm.base.helper import HelperBase
-from sqlalchemy_orm.base.inheritance import InheritanceBase
-from sqlalchemy_orm.base.mapper import MapperBase
+from sqlalchemy_orm.base.helper import Base
 from sqlalchemy_orm.typemapper import TypeMapper
 
 
-class SQLAlchemyORMBase(MapperBase, InheritanceBase, HelperBase):
-    pass
-
-
 class BaseDeclarativeMeta(DeclarativeMeta):
-
     def __init__(cls, classname, bases, dict_, **kw):
         dict_.update(cls.__dict__)
         super().__init__(classname, bases, dict_, **kw)
 
 
-def base_factory(type_map=None, base=None):
-    if base and type_map is not None:
-        base.type_mapper = type_map
-
+def base_factory(type_map: TypeMapper = None, base: Type = None) -> Type[Base]:
     if base:
-        combined_base = type("Base", (base, SQLAlchemyORMBase), {})
+        combined_base = type("Base", (base, Base), {})
     else:
-        combined_base = SQLAlchemyORMBase
+        combined_base = Base
 
-    if base is None and type_map is not None:
+    if type_map:
         combined_base.type_mapper = type_map
 
-    model: SQLAlchemyORMBase = declarative_base(
-        cls=combined_base,
-        name="Base",
-        metaclass=BaseDeclarativeMeta
+    model: Type[Base] = declarative_base(
+        cls=combined_base, name="Base", metaclass=BaseDeclarativeMeta
     )
     model.declarative_base = model
 
     return model
 
 
-Model: Callable[[TypeMapper, Type], Type] = base_factory
+Model = base_factory
+
+ModelBase = base_factory()
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/custom_types.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/custom_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,31 +13,32 @@
 class UUIDType(TypeDecorator):
     """Platform-independent GUID type.
 
     Uses PostgreSQL's UUID type, otherwise uses
     CHAR(32), storing as stringified hex values.
 
     """
+
     impl = CHAR
     cache_ok = True
 
     @property
     def python_type(self):
         return uuid.UUID
 
     def load_dialect_impl(self, dialect):
-        if dialect.name == 'postgresql':
+        if dialect.name == "postgresql":
             return dialect.type_descriptor(UUID())
         else:
             return dialect.type_descriptor(CHAR(32))
 
     def process_bind_param(self, value, dialect):
         if value is None:
             return value
-        elif dialect.name == 'postgresql':
+        elif dialect.name == "postgresql":
             return str(value)
         else:
             if not isinstance(value, uuid.UUID):
                 return "%.32x" % uuid.UUID(value).int
             else:
                 # hexstring
                 return "%.32x" % value.int
@@ -48,17 +49,17 @@
         else:
             if not isinstance(value, uuid.UUID):
                 value = uuid.UUID(value)
             return value
 
 
 class EnumType(TypeFactory):
-
     def to_type(self, python_type: Type) -> Optional[Type[TypeEngine]]:
         if issubclass(python_type, enum.Enum):
+
             class Enum(SQLAlchemyEnum):
                 _python_type = python_type
 
                 def __init__(self, *enums, **kw):
                     super().__init__(Enum._python_type, *enums, **kw)
 
             return Enum
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/database.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,121 +1,113 @@
 from typing import Iterable
 
 from sqlalchemy import create_engine, inspect, MetaData
 from sqlalchemy.orm import sessionmaker, RelationshipProperty
 from sqlalchemy.orm.clsregistry import _ModuleMarker
 
-from sqlalchemy_orm.base.helper import HelperBase
+from sqlalchemy_orm.base.helper import Base
 from sqlalchemy_orm.query import Query
 from sqlalchemy_orm.session import Session
 from sqlalchemy_orm.utils import find_subclasses
 
 
 class DatabaseException(BaseException):
     pass
 
 
 class Database:
-
     def __init__(self, url, session_cls=Session, query_cls=Query):
         self.url = url
         self.engine = create_engine(url)
         self.session_maker = sessionmaker(
-            class_=session_cls,
-            bind=self.engine,
-            query_cls=query_cls
+            class_=session_cls, bind=self.engine, query_cls=query_cls
         )
         self.declarative_base = None
 
     def entity_relationship_diagram(self, embed_html=True) -> str:
         """
         ERD in dot format
         """
 
-        from sqlalchemy_orm.eralchemy.main import \
-            _intermediary_to_dot, \
-            all_to_intermediary
+        from sqlalchemy_orm.eralchemy.main import (
+            _intermediary_to_dot,
+            all_to_intermediary,
+        )
 
         tables, relationships = all_to_intermediary(
-            self.declarative_base.metadata,
-            schema="Schema"
+            self.declarative_base.metadata, schema="Schema"
         )
         output = _intermediary_to_dot(tables, relationships)
 
         if embed_html:
             # flake8: noqa
-            output = """
+            output = (
+                """
             <!DOCTYPE html><meta charset="utf-8"><body>
             <script src="https://d3js.org/d3.v5.min.js"></script>
             <script src="https://unpkg.com/@hpcc-js/wasm@0.3.11/dist/index.min.js"></script>
             <script src="https://unpkg.com/d3-graphviz@3.0.5/build/d3-graphviz.js"></script>
             <div id="graph" style="text-align: center;"></div>
             <script>d3.select("#graph").graphviz().renderDot('DOT');</script>
-            """.replace("DOT", output).replace('\n', '').replace('\r', '')
+            """.replace(
+                    "DOT", output
+                )
+                .replace("\n", "")
+                .replace("\r", "")
+            )
 
         return output
 
     def session(self) -> Session:
         return self.session_maker()
 
     def create_all(self, base):
         base.metadata.create_all(bind=self.engine, checkfirst=True)
         self.declarative_base = base
 
-    def create(
-            self,
-            *models,
-            create_relations=True,
-            create_polymorphic_parents=True
-    ):
+    def create(self, *models, create_relations=True, create_polymorphic_parents=True):
         if create_relations:
             models_with_relations = {*models}
 
             for model in models:
-                if issubclass(model, HelperBase):
+                if issubclass(model, Base):
                     models_with_relations.update(model.relations())
                     self.declarative_base = model.declarative_base
 
             models = models_with_relations
 
         if create_polymorphic_parents:
             parents = set()
 
             for model in models:
-                if issubclass(model, HelperBase):
+                if issubclass(model, Base):
                     parents.update(model.parents())
 
             models.update(parents)
 
         get_metadata(models).create_all(
             bind=self.engine,
             tables=[model.__table__ for model in models],
-            checkfirst=True
+            checkfirst=True,
         )
 
     def delete(self, *models):
         get_metadata(models).drop_all(
             bind=self.engine,
             tables=[model.__table__ for model in models],
-            checkfirst=True
+            checkfirst=True,
         )
 
     def wipe(self):
         meta = MetaData()
         meta.reflect(bind=self.engine)
-        meta.drop_all(
-            bind=self.engine,
-            tables=meta.sorted_tables,
-            checkfirst=True
-        )
+        meta.drop_all(bind=self.engine, tables=meta.sorted_tables, checkfirst=True)
 
         if not self.is_empty():
-            raise DatabaseException(
-                f"Database '{self}' was not empty after wipe."
-            )
+            raise DatabaseException(f"Database '{self}' was not empty after wipe.")
 
     def is_empty(self):
         table_names = inspect(self.engine).get_table_names()
         return not table_names
 
     def validate(self, base, logger=None):
         """Check whether the current db matches the models
@@ -137,15 +129,15 @@
 
         tables = iengine.get_table_names()
 
         # Go through all Model subclasses
         for model_class in find_subclasses(base):
             module_marker = isinstance(model_class, _ModuleMarker)
 
-            is_abstract = model_class.__dict__.get('__abstract__', False)
+            is_abstract = model_class.__dict__.get("__abstract__", False)
 
             if module_marker or is_abstract:
                 continue
 
             table = model_class.__tablename__
             if table in tables:
                 # Check all columns are found
@@ -165,17 +157,15 @@
                                     logger.info(
                                         f"Column '{table}.{column.key}' does"
                                         f" not exist in db '{self.engine}'"
                                     )
                                 errors = True
             else:
                 if logger:
-                    logger.info(
-                        "Table '{table}' does not exist in db '{self.engine}'"
-                    )
+                    logger.info("Table '{table}' does not exist in db '{self.engine}'")
 
                 errors = True
 
         return not errors
 
     def __contains__(self, model):
         connect_ = self.engine.connect()
@@ -188,15 +178,15 @@
 def get_metadata(models: Iterable[object]):
     if not models:
         raise ValueError("Metadata must have at least one model specified")
 
     metadata = None
 
     for model in models:
-        if hasattr(model, 'metadata'):
+        if hasattr(model, "metadata"):
             if metadata is None:
                 metadata = model.metadata
 
             if model.metadata != metadata:
                 raise ValueError("Metadata mismatch within list of models")
         else:
             raise ValueError("All models must specify a 'metadata' attribute")
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/cst.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/cst.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # flake8: noqa
 # -*- coding: utf-8 -*-
 
 """
 All the constants used in the module.
 """
-TABLE = '"{}" [label=<<FONT FACE="Helvetica"><TABLE BORDER="0" ' \
-        'CELLBORDER="1"' \
-        ' CELLPADDING="4" CELLSPACING="0">{}{}</TABLE></FONT>>];'
+TABLE = (
+    '"{}" [label=<<FONT FACE="Helvetica"><TABLE BORDER="0" '
+    'CELLBORDER="1"'
+    ' CELLPADDING="4" CELLSPACING="0">{}{}</TABLE></FONT>>];'
+)
 
 START_CELL = '<TR><TD ALIGN="LEFT"><FONT>'
-FONT_TAGS = '<FONT>{}</FONT>'
+FONT_TAGS = "<FONT>{}</FONT>"
 # Used for each row in the table.
-ROW_TAGS = '<TR><TD{}>{}</TD></TR>'
-GRAPH_BEGINNING = (' graph {\n'
-                   '    graph [rankdir=LR];\n'
-                   '    node [label=\"\\N\",\n'
-                   '        shape=plaintext\n'
-                   '    ];\n'
-                   '    edge [color=gray50,\n'
-                   '        minlen=2,\n'
-                   '        style=dashed\n'
-                   '    ];\n'
-                   )
+ROW_TAGS = "<TR><TD{}>{}</TD></TR>"
+GRAPH_BEGINNING = (
+    " graph {\n"
+    "    graph [rankdir=LR];\n"
+    '    node [label="\\N",\n'
+    "        shape=plaintext\n"
+    "    ];\n"
+    "    edge [color=gray50,\n"
+    "        minlen=2,\n"
+    "        style=dashed\n"
+    "    ];\n"
+)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa # -*- coding: utf-8 -*- """ All the constants used in the
-module. """ TABLE = '"{}" [label=<
- \ 'CELLBORDER="1"' \ ' CELLPADDING="4" CELLSPACING="0">{}{}
->];' START_CELL = '
-' FONT_TAGS = '{}' # Used for each row in the table. ROW_TAGS = '
+module. """ TABLE = ( '"{}" [label=<
+ 'CELLBORDER="1"' ' CELLPADDING="4" CELLSPACING="0">{}{}
+>];' ) START_CELL = '
+' FONT_TAGS = "{}" # Used for each row in the table. ROW_TAGS = "
 }>{}
-' GRAPH_BEGINNING = (' graph {\n' ' graph [rankdir=LR];\n' ' node
-[label=\"\\N\",\n' ' shape=plaintext\n' ' ];\n' ' edge [color=gray50,\n' '
-minlen=2,\n' ' style=dashed\n' ' ];\n' )
+" GRAPH_BEGINNING = ( " graph {\n" " graph [rankdir=LR];\n" ' node
+[label="\\N",\n' " shape=plaintext\n" " ];\n" " edge [color=gray50,\n" "
+minlen=2,\n" " style=dashed\n" " ];\n" )
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/main.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # flake8: noqa
 # -*- coding: utf-8 -*-
 import argparse
 import copy
 
 import sys
+
 # from pygraphviz.agraph import AGraph
 from sqlalchemy.engine.url import make_url
 from sqlalchemy.exc import ArgumentError
 
 from .cst import GRAPH_BEGINNING
 from .helpers import check_args
-from .parser import markdown_file_to_intermediary, \
-    line_iterator_to_intermediary, ParsingException
-from .sqla import metadata_to_intermediary, declarative_to_intermediary, \
-    database_to_intermediary
+from .parser import (
+    markdown_file_to_intermediary,
+    line_iterator_to_intermediary,
+    ParsingException,
+)
+from .sqla import (
+    metadata_to_intermediary,
+    declarative_to_intermediary,
+    database_to_intermediary,
+)
 from .version import version as __version__
 
 try:
     basestring
 except NameError:
     basestring = str
 
@@ -25,56 +32,61 @@
 def cli():
     """Entry point for the application script"""
     parser = get_argparser()
 
     args = parser.parse_args()
     check_args(args)
     if args.v:
-        print('ERAlchemy version {}.'.format(__version__))
+        print("ERAlchemy version {}.".format(__version__))
         exit(0)
     render_er(
         args.i,
         args.o,
         include_tables=args.include_tables,
         include_columns=args.include_columns,
         exclude_tables=args.exclude_tables,
         exclude_columns=args.exclude_columns,
-        schema=args.s
+        schema=args.s,
     )
 
 
 def get_argparser():
-    parser = argparse.ArgumentParser(prog='ERAlchemy')
-    parser.add_argument('-i', nargs='?', help='Database URI to process.')
-    parser.add_argument('-o', nargs='?', help='Name of the file to write.')
-    parser.add_argument('-s', nargs='?', help='Name of the schema.')
-    parser.add_argument('--exclude-tables', '-x', nargs='+',
-                        help='Name of tables not to be displayed.')
-    parser.add_argument('--exclude-columns', nargs='+',
-                        help='Name of columns not to be displayed (for all '
-                             'tables).')
-    parser.add_argument('--include-tables', nargs='+',
-                        help='Name of tables to be displayed alone.')
-    parser.add_argument('--include-columns', nargs='+',
-                        help='Name of columns to be displayed alone (for all '
-                             'tables).')
-    parser.add_argument('-v', help='Prints version number.',
-                        action='store_true')
+    parser = argparse.ArgumentParser(prog="ERAlchemy")
+    parser.add_argument("-i", nargs="?", help="Database URI to process.")
+    parser.add_argument("-o", nargs="?", help="Name of the file to write.")
+    parser.add_argument("-s", nargs="?", help="Name of the schema.")
+    parser.add_argument(
+        "--exclude-tables", "-x", nargs="+", help="Name of tables not to be displayed."
+    )
+    parser.add_argument(
+        "--exclude-columns",
+        nargs="+",
+        help="Name of columns not to be displayed (for all " "tables).",
+    )
+    parser.add_argument(
+        "--include-tables", nargs="+", help="Name of tables to be displayed alone."
+    )
+    parser.add_argument(
+        "--include-columns",
+        nargs="+",
+        help="Name of columns to be displayed alone (for all " "tables).",
+    )
+    parser.add_argument("-v", help="Prints version number.", action="store_true")
     return parser
 
 
 def intermediary_to_markdown(tables, relationships, output):
-    """ Saves the intermediary representation to markdown. """
+    """Saves the intermediary representation to markdown."""
     er_markup = _intermediary_to_markdown(tables, relationships)
     with open(output, "w") as file_out:
         file_out.write(er_markup)
 
 
 def intermediary_to_dot(tables, relationships, output):
-    """ Save the intermediary representation to dot format. """
+    """Save the intermediary representation to dot format."""
     dot_file = _intermediary_to_dot(tables, relationships)
     with open(output, "w") as file_out:
         file_out.write(dot_file)
 
 
 def intermediary_to_schema(tables, relationships, output):
     pass
@@ -84,56 +96,56 @@
     # graph = AGraph()
     # graph = graph.from_string(dot_file)
     # extension = output.split('.')[-1]
     # graph.draw(path=output, prog='dot', format=extension)
 
 
 def _intermediary_to_markdown(tables, relationships):
-    """ Returns the er markup source in a string. """
-    t = '\n'.join(t.to_markdown() for t in tables)
-    r = '\n'.join(r.to_markdown() for r in relationships)
-    return '{}\n{}'.format(t, r)
+    """Returns the er markup source in a string."""
+    t = "\n".join(t.to_markdown() for t in tables)
+    r = "\n".join(r.to_markdown() for r in relationships)
+    return "{}\n{}".format(t, r)
 
 
 def _intermediary_to_dot(tables, relationships):
-    """ Returns the dot source representing the database in a string. """
-    t = '\n'.join(t.to_dot() for t in tables)
-    r = '\n'.join(r.to_dot() for r in relationships)
-    return '{}\n{}\n{}\n}}'.format(GRAPH_BEGINNING, t, r)
+    """Returns the dot source representing the database in a string."""
+    t = "\n".join(t.to_dot() for t in tables)
+    r = "\n".join(r.to_dot() for r in relationships)
+    return "{}\n{}\n{}\n}}".format(GRAPH_BEGINNING, t, r)
 
 
 # Routes from the class name to the function transforming this class in
 # the intermediary representation.
 switch_input_class_to_method = {
-    'MetaData': metadata_to_intermediary,
-    'DeclarativeMeta': declarative_to_intermediary,
+    "MetaData": metadata_to_intermediary,
+    "DeclarativeMeta": declarative_to_intermediary,
     # For compatibility with Flask-SQLAlchemy
-    '_BoundDeclarativeMeta': declarative_to_intermediary,
+    "_BoundDeclarativeMeta": declarative_to_intermediary,
     # Renamed in Flask-SQLAlchemy 2.3
-    'DefaultMeta': declarative_to_intermediary
+    "DefaultMeta": declarative_to_intermediary,
 }
 
 # Routes from the mode to the method to transform the intermediary
 #  representation to the desired output.
 switch_output_mode_auto = {
-    'er': intermediary_to_markdown,
-    'graph': intermediary_to_schema,
-    'dot': intermediary_to_dot
+    "er": intermediary_to_markdown,
+    "graph": intermediary_to_schema,
+    "dot": intermediary_to_dot,
 }
 
 # Routes from the file extension to the method to transform
 # the intermediary representation to the desired output.
 switch_output_mode = {
-    'er': intermediary_to_markdown,
-    'dot': intermediary_to_dot,
+    "er": intermediary_to_markdown,
+    "dot": intermediary_to_dot,
 }
 
 
 def all_to_intermediary(filename_or_input, schema=None):
-    """ Dispatch the filename_or_input to the different function to produce
+    """Dispatch the filename_or_input to the different function to produce
     the intermediary syntax.
     All the supported classes names are in `swich_input_class_to_method`.
     The input can also be a list of strings in markdown format or a filename
     finishing by '.er' containing markdown
     format.
     """
     # Try to convert from the name of the class
@@ -143,55 +155,60 @@
         tables, relationships = this_to_intermediary(filename_or_input)
         return tables, relationships
     except KeyError:
         pass
 
     # try to read markdown file.
     if isinstance(filename_or_input, basestring):
-        if filename_or_input.split('.')[-1] == 'er':
+        if filename_or_input.split(".")[-1] == "er":
             return markdown_file_to_intermediary(filename_or_input)
 
     # try to read a markdown in a string
     if not isinstance(filename_or_input, basestring):
         if all(isinstance(e, basestring) for e in filename_or_input):
             return line_iterator_to_intermediary(filename_or_input)
 
     # try to read DB URI.
     try:
         make_url(filename_or_input)
         return database_to_intermediary(filename_or_input, schema=schema)
     except ArgumentError:
         pass
 
-    msg = 'Cannot process filename_or_input {}'.format(input_class_name)
+    msg = "Cannot process filename_or_input {}".format(input_class_name)
     raise ValueError(msg)
 
 
 def get_output_mode(output, mode):
     """
     From the output name and the mode returns a the function that will
     transform the intermediary
     representation to the output.
     """
-    if mode != 'auto':
+    if mode != "auto":
         try:
             return switch_output_mode_auto[mode]
         except KeyError:
             raise ValueError('Mode "{}" is not supported.')
 
-    extension = output.split('.')[-1]
+    extension = output.split(".")[-1]
     try:
         return switch_output_mode[extension]
     except KeyError:
         return intermediary_to_schema
 
 
-def filter_resources(tables, relationships,
-                     include_tables=None, include_columns=None,
-                     exclude_tables=None, exclude_columns=None):
+def filter_resources(
+    tables,
+    relationships,
+    include_tables=None,
+    include_columns=None,
+    exclude_tables=None,
+    exclude_columns=None,
+):
     """
     Include the following:
         1. Tables and relationships with tables present in the
         include_tables (lst of str, tables names)
         2. Columns (of whichever table) present in the include_columns (lst
         of str, columns names)
     Exclude the following:
@@ -204,38 +221,50 @@
         In other words, if one excludes primary or foreign keys, it will
         still keep the relations display amongst tables
     """
     _tables = copy.deepcopy(tables)
     _relationships = copy.deepcopy(relationships)
 
     include_tables = include_tables or [t.name for t in _tables]
-    include_columns = include_columns or [c.name for t in _tables for c in
-                                          t.columns]
+    include_columns = include_columns or [c.name for t in _tables for c in t.columns]
     exclude_tables = exclude_tables or list()
     exclude_columns = exclude_columns or list()
 
-    _tables = [t for t in _tables if
-               t.name not in exclude_tables and t.name in include_tables]
-    _relationships = [r for r in _relationships
-                      if r.right_col not in exclude_tables
-                      and r.left_col not in exclude_tables
-                      and r.right_col in include_tables
-                      and r.left_col in include_tables]
+    _tables = [
+        t for t in _tables if t.name not in exclude_tables and t.name in include_tables
+    ]
+    _relationships = [
+        r
+        for r in _relationships
+        if r.right_col not in exclude_tables
+        and r.left_col not in exclude_tables
+        and r.right_col in include_tables
+        and r.left_col in include_tables
+    ]
 
     for t in _tables:
-        t.columns = [c for c in t.columns if
-                     c.name not in exclude_columns and c.name in
-                     include_columns]
+        t.columns = [
+            c
+            for c in t.columns
+            if c.name not in exclude_columns and c.name in include_columns
+        ]
 
     return _tables, _relationships
 
 
-def render_er(input, output, mode='auto', include_tables=None,
-              include_columns=None,
-              exclude_tables=None, exclude_columns=None, schema=None):
+def render_er(
+    input,
+    output,
+    mode="auto",
+    include_tables=None,
+    include_columns=None,
+    exclude_tables=None,
+    exclude_columns=None,
+    schema=None,
+):
     """
     Transform the metadata into a representation.
     :param input: Possible inputs are instances of:
         MetaData: SQLAlchemy Metadata
         DeclarativeMeta: SQLAlchemy declarative Base
     :param output: name of the file to output the
     :param mode: str in list:
@@ -255,24 +284,26 @@
     exclude nothing
     :param exclude_columns: lst of str, field names to exclude, None means
     exclude nothing
     :param schema: name of the schema
     """
     try:
         tables, relationships = all_to_intermediary(input, schema=schema)
-        tables, relationships = filter_resources(tables, relationships,
-                                                 include_tables=include_tables,
-                                                 include_columns=include_columns,
-                                                 exclude_tables=exclude_tables,
-                                                 exclude_columns=exclude_columns)
+        tables, relationships = filter_resources(
+            tables,
+            relationships,
+            include_tables=include_tables,
+            include_columns=include_columns,
+            exclude_tables=exclude_tables,
+            exclude_columns=exclude_columns,
+        )
         intermediary_to_output = get_output_mode(output, mode)
         intermediary_to_output(tables, relationships, output)
     except ImportError as e:
         module_name = e.message.split()[-1]
-        print(
-            'Please install {0} using "pip install {0}".'.format(module_name))
+        print('Please install {0} using "pip install {0}".'.format(module_name))
     except ParsingException as e:
         sys.stderr.write(e.message)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/models.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,52 +8,54 @@
 """
 All the intermediary syntax.
 We can several kinds of models can be translated to this syntax.
 """
 
 
 class Drawable:
-    """ Abstract class to represent all the objects which are drawable."""
+    """Abstract class to represent all the objects which are drawable."""
+
     RE = None
 
     def to_markdown(self):
         """Transforms the intermediary object to it's syntax in the er
-        markup. """
+        markup."""
         raise NotImplementedError()
 
     def to_dot(self):
         """Transforms the intermediary object to it's syntax in the dot
-        format. """
+        format."""
         raise NotImplementedError()
 
     def __eq__(self, other):
         return self.__dict__ == other.__dict__
 
     @staticmethod
     def make_from_match(self):
-        """ Used in the parsing of files. Transforms a regex match to a
-        Drawable object. """
+        """Used in the parsing of files. Transforms a regex match to a
+        Drawable object."""
         raise NotImplementedError()
 
     def __str__(self):
         return self.to_markdown()
 
 
 class Column(Drawable):
-    """ Represents a Column in the intermediaty syntax """
+    """Represents a Column in the intermediaty syntax"""
+
     RE = re.compile(
-        '(?P<primary>\*?)(?P<name>[^\s]+)\s*(\{label:\s*"(?P<label>['
-        '^"]+)"\})?')
+        '(?P<primary>\*?)(?P<name>[^\s]+)\s*(\{label:\s*"(?P<label>[' '^"]+)"\})?'
+    )
 
     @staticmethod
     def make_from_match(match):
         return Column(
-            name=match.group('name'),
-            type=match.group('label'),
-            is_key='*' in match.group('primary'),  # TODO foreign key
+            name=match.group("name"),
+            type=match.group("label"),
+            is_key="*" in match.group("primary"),  # TODO foreign key
         )
 
     def __init__(self, name, type=None, is_key=False):
         """
         :param name: (str) Name of the column
         :param type:
         :param is_key:
@@ -61,139 +63,142 @@
         """
         self.name = name
         self.type = type
         self.is_key = is_key
 
     @property
     def key_symbol(self):
-        return '*' if self.is_key else ''
+        return "*" if self.is_key else ""
 
     def to_markdown(self):
-        return '    {}{} {{label:"{}"}}'.format(self.key_symbol, self.name,
-                                                self.type)
+        return '    {}{} {{label:"{}"}}'.format(self.key_symbol, self.name, self.type)
 
     def to_dot(self):
-        base = ROW_TAGS.format(' ALIGN="LEFT"',
-                               '{key_opening}{col_name}{key_closing}{type}')
+        base = ROW_TAGS.format(
+            ' ALIGN="LEFT"', "{key_opening}{col_name}{key_closing}{type}"
+        )
         return base.format(
-            key_opening='<u>' if self.is_key else '',
-            key_closing='</u>' if self.is_key else '',
+            key_opening="<u>" if self.is_key else "",
+            key_closing="</u>" if self.is_key else "",
             col_name=FONT_TAGS.format(self.name),
-            type=FONT_TAGS.format(' [{}]').format(
-                self.type) if self.type is not None else ''
+            type=FONT_TAGS.format(" [{}]").format(self.type)
+            if self.type is not None
+            else "",
         )
 
 
 class Relation(Drawable):
-    """ Represents a Relation in the intermediaty syntax """
+    """Represents a Relation in the intermediaty syntax"""
+
     RE = re.compile(
-        '(?P<left_name>[^\s]+)\s*(?P<left_cardinality>[*?+1])--('
-        '?P<right_cardinality>[*?+1])\s*(?P<right_name>[^\s]+)')  # noqa: E501
-    cardinalities = {
-        '*': '0..N',
-        '?': '{0,1}',
-        '+': '1..N',
-        '1': '1',
-        '': None
-    }
+        "(?P<left_name>[^\s]+)\s*(?P<left_cardinality>[*?+1])--("
+        "?P<right_cardinality>[*?+1])\s*(?P<right_name>[^\s]+)"
+    )  # noqa: E501
+    cardinalities = {"*": "0..N", "?": "{0,1}", "+": "1..N", "1": "1", "": None}
 
     @staticmethod
     def make_from_match(match):
         return Relation(
-            right_col=match.group('right_name'),
-            left_col=match.group('left_name'),
-            right_cardinality=match.group('right_cardinality'),
-            left_cardinality=match.group('left_cardinality'),
-        )
-
-    def __init__(self, right_col, left_col, right_cardinality=None,
-                 left_cardinality=None):
-        if right_cardinality not in self.cardinalities.keys() \
-                or left_cardinality not in self.cardinalities.keys():
-            raise ValueError('Cardinality should be in {}"'.format(
-                self.cardinalities.keys()))
+            right_col=match.group("right_name"),
+            left_col=match.group("left_name"),
+            right_cardinality=match.group("right_cardinality"),
+            left_cardinality=match.group("left_cardinality"),
+        )
+
+    def __init__(
+        self, right_col, left_col, right_cardinality=None, left_cardinality=None
+    ):
+        if (
+            right_cardinality not in self.cardinalities.keys()
+            or left_cardinality not in self.cardinalities.keys()
+        ):
+            raise ValueError(
+                'Cardinality should be in {}"'.format(self.cardinalities.keys())
+            )
         self.right_col = right_col
         self.left_col = left_col
         self.right_cardinality = right_cardinality
         self.left_cardinality = left_cardinality
 
     def to_markdown(self):
         return "{} {}--{} {}".format(
             self.left_col,
             self.left_cardinality,
             self.right_cardinality,
             self.right_col,
         )
 
     def graphviz_cardinalities(self, card):
-        if card == '':
-            return ''
-        return 'label=<<FONT>{}</FONT>>'.format(self.cardinalities[card])
+        if card == "":
+            return ""
+        return "label=<<FONT>{}</FONT>>".format(self.cardinalities[card])
 
     def to_dot(self):
-        if self.right_cardinality == self.left_cardinality == '':
-            return ''
+        if self.right_cardinality == self.left_cardinality == "":
+            return ""
         cards = []
-        if self.left_cardinality != '':
-            cards.append('tail' +
-                         self.graphviz_cardinalities(self.left_cardinality))
-        if self.right_cardinality != '':
-            cards.append('head' +
-                         self.graphviz_cardinalities(self.right_cardinality))
-        return '"{}" -- "{}" [{}];'.format(self.left_col, self.right_col,
-                                           ','.join(cards))
+        if self.left_cardinality != "":
+            cards.append("tail" + self.graphviz_cardinalities(self.left_cardinality))
+        if self.right_cardinality != "":
+            cards.append("head" + self.graphviz_cardinalities(self.right_cardinality))
+        return '"{}" -- "{}" [{}];'.format(
+            self.left_col, self.right_col, ",".join(cards)
+        )
 
     def __eq__(self, other):
         if Drawable.__eq__(self, other):
             return True
         other_inversed = Relation(
             right_col=other.left_col,
             left_col=other.right_col,
             right_cardinality=other.left_cardinality,
             left_cardinality=other.right_cardinality,
         )
         return other_inversed.__dict__ == self.__dict__
 
 
 class Table(Drawable):
-    """ Represents a Table in the intermediaty syntax """
-    RE = re.compile('\[(?P<name>[^]]+)\]')
+    """Represents a Table in the intermediaty syntax"""
+
+    RE = re.compile("\[(?P<name>[^]]+)\]")
 
     def __init__(self, name, columns):
         self.name = name
         self.columns = columns
 
     @staticmethod
     def make_from_match(match):
         return Table(
-            name=match.group('name'),
+            name=match.group("name"),
             columns=[],
         )
 
     @property
     def header_markdown(self):
-        return '[{}]'.format(self.name)
+        return "[{}]".format(self.name)
 
     def to_markdown(self):
-        return self.header_markdown + '\n' + '\n'.join(
-            c.to_markdown() for c in self.columns)
+        return (
+            self.header_markdown
+            + "\n"
+            + "\n".join(c.to_markdown() for c in self.columns)
+        )
 
     @property
     def columns_sorted(self):
-        return sorted(self.columns, key=operator.attrgetter('name'))
+        return sorted(self.columns, key=operator.attrgetter("name"))
 
     @property
     def header_dot(self):
-        return ROW_TAGS.format('',
-                               '<B><FONT POINT-SIZE="16">{'
-                               '}</FONT></B>').format(
-            self.name)
+        return ROW_TAGS.format("", '<B><FONT POINT-SIZE="16">{' "}</FONT></B>").format(
+            self.name
+        )
 
     def to_dot(self):
-        body = ''.join(c.to_dot() for c in self.columns)
+        body = "".join(c.to_dot() for c in self.columns)
         return TABLE.format(self.name, self.header_dot, body)
 
     def __str__(self):
         return self.header_markdown
 
     def __eq__(self, other):
         if not isinstance(other, Table):
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/parser.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 # flake8: noqa
 # -*- coding: utf-8 -*-
 from .models import Table, Relation, Column
 
 
 class ParsingException(Exception):
-    base_traceback = 'Error on line {line_nb}: {line}\n{error}'
+    base_traceback = "Error on line {line_nb}: {line}\n{error}"
     hint = None
 
     @property
     def traceback(self):
         rv = self.base_traceback.format(
-            line_nb=getattr(self, 'line_nb', '?'),
-            line=getattr(self, 'line', ''),
+            line_nb=getattr(self, "line_nb", "?"),
+            line=getattr(self, "line", ""),
             error=self.args[0],
         )
         if self.hint is not None:
-            rv += '\nHINT: {}'.format(self.hint)
+            rv += "\nHINT: {}".format(self.hint)
         return rv
 
 
 class DuplicateTableException(ParsingException):
     pass
 
 
 class DuplicateColumnException(ParsingException):
     pass
 
 
 class RelationNoColException(ParsingException):
-    hint = 'Try to declare the tables before the relationships.'
+    hint = "Try to declare the tables before the relationships."
 
 
 class NoCurrentTableException(ParsingException):
-    hint = 'Try to declare the tables before the relationships and columns.'
+    hint = "Try to declare the tables before the relationships and columns."
 
 
 def remove_comments_from_line(line):
-    if '#' not in line:
+    if "#" not in line:
         return line.strip()
-    return line[:line.index('#')].strip()
+    return line[: line.index("#")].strip()
 
 
 def filter_lines_from_comments(lines):
-    """ Filter the lines from comments and non code lines. """
+    """Filter the lines from comments and non code lines."""
     for line_nb, raw_line in enumerate(lines):
         clean_line = remove_comments_from_line(raw_line)
-        if clean_line == '':
+        if clean_line == "":
             continue
         yield line_nb, clean_line, raw_line
 
 
 def parse_line(line):
     for typ in [Table, Relation, Column]:
         match = typ.RE.match(line)
         if match:
             return typ.make_from_match(match)
     msg = 'Line "{}" could not be parsed to an object.'
     raise ValueError(msg.format(line))
 
 
 def _check_no_current_table(new_obj, current_table):
-    """ Raises exception if we try to add a relation or a column
-    with no current table. """
+    """Raises exception if we try to add a relation or a column
+    with no current table."""
     if current_table is None:
-        msg = 'Cannot add {} before adding table'
+        msg = "Cannot add {} before adding table"
         if isinstance(new_obj, Relation):
-            raise NoCurrentTableException(msg.format('relation'))
+            raise NoCurrentTableException(msg.format("relation"))
         if isinstance(new_obj, Column):
-            raise NoCurrentTableException(msg.format('column'))
+            raise NoCurrentTableException(msg.format("column"))
 
 
 def _update_check_inputs(current_table, tables, relations):
     assert current_table is None or isinstance(current_table, Table)
     assert isinstance(tables, list)
     assert all(isinstance(t, Table) for t in tables)
     assert all(isinstance(r, Relation) for r in relations)
@@ -82,70 +82,72 @@
     if column_name not in columns_names:
         msg = 'Cannot add a relation with column "{}" which is undefined'
         raise RelationNoColException(msg.format(column_name))
 
 
 def _check_not_creating_duplicates(new_name, names, type, exc):
     if new_name in names:
-        msg = 'Cannot add {} named "{}" which is ' \
-              'already present in the schema.'
+        msg = 'Cannot add {} named "{}" which is ' "already present in the schema."
         raise exc(msg.format(type, new_name))
 
 
 def update_models(new_obj, current_table, tables, relations):
-    """ Update the state of the parsing. """
+    """Update the state of the parsing."""
     _update_check_inputs(current_table, tables, relations)
     _check_no_current_table(new_obj, current_table)
 
     if isinstance(new_obj, Table):
         tables_names = [t.name for t in tables]
-        _check_not_creating_duplicates(new_obj.name, tables_names, 'table',
-                                       DuplicateTableException)
+        _check_not_creating_duplicates(
+            new_obj.name, tables_names, "table", DuplicateTableException
+        )
         return new_obj, tables + [new_obj], relations
 
     if isinstance(new_obj, Relation):
         tables_names = [t.name for t in tables]
         _check_colname_in_lst(new_obj.right_col, tables_names)
         _check_colname_in_lst(new_obj.left_col, tables_names)
         return current_table, tables, relations + [new_obj]
 
     if isinstance(new_obj, Column):
         columns_names = [c.name for c in current_table.columns]
-        _check_not_creating_duplicates(new_obj.name, columns_names, 'column',
-                                       DuplicateColumnException)
+        _check_not_creating_duplicates(
+            new_obj.name, columns_names, "column", DuplicateColumnException
+        )
         current_table.columns.append(new_obj)
         return current_table, tables, relations
 
     msg = "new_obj cannot be of type {}"
     raise ValueError(msg.format(new_obj.__class__.__name__))
 
 
 def markdown_file_to_intermediary(filename):
-    """ Parse a file and return to intermediary syntax. """
+    """Parse a file and return to intermediary syntax."""
     with open(filename) as f:
         lines = f.readlines()
     return line_iterator_to_intermediary(lines)
 
 
 def line_iterator_to_intermediary(line_iterator):
-    """ Parse an iterator of str (one string per line) to the intermediary
+    """Parse an iterator of str (one string per line) to the intermediary
     syntax"""
     current_table = None
     tables = []
     relations = []
     errors = []
     for line_nb, line, raw_line in filter_lines_from_comments(line_iterator):
         try:
             new_obj = parse_line(line)
-            current_table, tables, relations = update_models(new_obj,
-                                                             current_table,
-                                                             tables, relations)
+            current_table, tables, relations = update_models(
+                new_obj, current_table, tables, relations
+            )
         except ParsingException as e:
             e.line_nb = line_nb
             e.line = raw_line
             errors.append(e)
     if len(errors) != 0:
-        msg = 'ERAlchemy couldn\'t complete the generation due the {} ' \
-              'following errors'.format(
-            len(errors))
-        raise ParsingException(msg + '\n\n'.join(e.traceback for e in errors))
+        msg = (
+            "ERAlchemy couldn't complete the generation due the {} "
+            "following errors".format(len(errors))
+        )
+        raise ParsingException(msg + "\n\n".join(e.traceback for e in errors))
     return tables, relations
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/eralchemy/sqla.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/eralchemy/sqla.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,85 +11,87 @@
 
 if sys.version_info[0] == 3:
     unicode = str
 
 
 def relation_to_intermediary(fk):
     """Transform an SQLAlchemy ForeignKey object to it's intermediary
-    representation. """
+    representation."""
     return Relation(
         right_col=format_name(fk.parent.table.fullname),
         left_col=format_name(fk._column_tokens[1]),
-        right_cardinality='?',
-        left_cardinality='*',
+        right_cardinality="?",
+        left_cardinality="*",
     )
 
 
 def format_type(typ):
-    """ Transforms the type into a nice string representation. """
+    """Transforms the type into a nice string representation."""
     try:
         return unicode(typ)
     except CompileError:
-        return 'Null'
+        return "Null"
 
 
 def format_name(name):
-    """ Transforms the name into a nice string representation. """
+    """Transforms the name into a nice string representation."""
     return unicode(name)
 
 
 def column_to_intermediary(col, type_formatter=format_type):
     """Transform an SQLAlchemy Column object to it's intermediary
-    representation. """
+    representation."""
     return Column(
         name=col.name,
         type=type_formatter(col.type),
         is_key=col.primary_key,
     )
 
 
 def table_to_intermediary(table):
     """Transform an SQLAlchemy Table object to it's intermediary
-    representation. """
+    representation."""
     return Table(
         name=table.fullname,
-        columns=[column_to_intermediary(col) for col in
-                 table.c._colset]
+        columns=[column_to_intermediary(col) for col in table.c._colset],
     )
 
 
 def metadata_to_intermediary(metadata):
-    """ Transforms SQLAlchemy metadata to the intermediary representation. """
-    tables = [table_to_intermediary(table) for table in
-              metadata.tables.values()]
-    relationships = [relation_to_intermediary(fk) for table in
-                     metadata.tables.values() for fk in table.foreign_keys]
+    """Transforms SQLAlchemy metadata to the intermediary representation."""
+    tables = [table_to_intermediary(table) for table in metadata.tables.values()]
+    relationships = [
+        relation_to_intermediary(fk)
+        for table in metadata.tables.values()
+        for fk in table.foreign_keys
+    ]
     return tables, relationships
 
 
 def declarative_to_intermediary(base):
-    """ Transform an SQLAlchemy Declarative Base to the intermediary
-    representation. """
+    """Transform an SQLAlchemy Declarative Base to the intermediary
+    representation."""
     return metadata_to_intermediary(base.metadata)
 
 
 def name_for_scalar_relationship(base, local_cls, referred_cls, constraint):
-    """ Overriding naming schemes. """
+    """Overriding naming schemes."""
     name = referred_cls.__name__.lower() + "_ref"
     return name
 
 
 def database_to_intermediary(database_uri, schema=None):
-    """ Introspect from the database (given the database_uri) to create the
-    intermediary representation. """
+    """Introspect from the database (given the database_uri) to create the
+    intermediary representation."""
     from sqlalchemy.ext.automap import automap_base
     from sqlalchemy import create_engine
 
     Base = automap_base()
     engine = create_engine(database_uri)
     if schema is not None:
         Base.metadata.schema = schema
 
     # reflect the tables
-    Base.prepare(engine, reflect=True,
-                 name_for_scalar_relationship=name_for_scalar_relationship)
+    Base.prepare(
+        engine, reflect=True, name_for_scalar_relationship=name_for_scalar_relationship
+    )
     return declarative_to_intermediary(Base)
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/filter.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/filter.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,55 +6,51 @@
 
 try:
     from dataclasses import dataclass
 
 except ImportError:
 
     class FilterBase(QueryAdapter):
-
         # noinspection PyPep8Naming
-        def __init__(
-                self,
-                or_: List['Filter'] = None,
-                and_: List['Filter'] = None
-        ):
+        def __init__(self, or_: List["Filter"] = None, and_: List["Filter"] = None):
             self.or_ = or_
             self.and_ = and_
+
 else:
 
     @dataclass
     class FilterBase(QueryAdapter):
-        and_: List['Filter'] = None
-        or_: List['Filter'] = None
+        and_: List["Filter"] = None
+        or_: List["Filter"] = None
 
 
 class Filter(FilterBase):
-
     def apply(self, query, entities=None):
         return query.filter(*self.criterion(entities=entities))
 
     # noinspection PyMethodMayBeStatic,PyUnusedLocal
     def criterion(self, entities=None):
         if self.or_ and self.and_:
             raise ValueError(
                 "Filter applied with both logical operators 'OR' and 'AND'"
             )
 
         criterion = []
 
         if self.or_:
             criterion = [
-                or_(*[
-                    and_(*filter.criterion(entities=entities))
-                    for filter in self.or_
-                ])
+                or_(
+                    *[and_(*filter.criterion(entities=entities)) for filter in self.or_]
+                )
             ]
 
         if self.and_:
             criterion = [
-                and_(*[
-                    and_(*filter.criterion(entities=entities))
-                    for filter in self.and_
-                ])
+                and_(
+                    *[
+                        and_(*filter.criterion(entities=entities))
+                        for filter in self.and_
+                    ]
+                )
             ]
 
         return criterion
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/order_by.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/order_by.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,19 +14,16 @@
 
 try:
     from dataclasses import dataclass
 
 except ImportError:
 
     class OrderByBase(QueryAdapter):
-
         def __init__(
-                self,
-                key: str,
-                direction: OrderByDirection = OrderByDirection.asc
+            self, key: str, direction: OrderByDirection = OrderByDirection.asc
         ):
             """
             The `OrderBy` ObjectType describes an
             order_by clause for a collection.
             """
             self.key = key
             self.direction = direction
@@ -36,21 +33,18 @@
     @dataclass
     class OrderByBase(QueryAdapter):
         key: str
         direction: OrderByDirection = OrderByDirection.asc
 
 
 class OrderBy(OrderByBase):
-
     def apply(self, query, entities=None):
-
         if len(entities) != 1:
             raise OrderByMultipleEntitiesException(
-                f"Cannot use a OrderBy when querying"
-                f" multiple models: '{entities}'"
+                f"Cannot use a OrderBy when querying" f" multiple models: '{entities}'"
             )
 
         model = entities[0]
 
         sort_attr = getattr(model, self.key)
 
         if self.direction == OrderByDirection.asc:
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/patterns/tag.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import uuid
 from typing import Type
 
 from sqlalchemy.ext.associationproxy import association_proxy
 from sqlalchemy.orm import relationship, validates, object_session
 from sqlalchemy.orm.decl_api import declared_attr
 
-from sqlalchemy_orm.base.helper import HelperBase
+from sqlalchemy_orm.base.helper import Base
 from sqlalchemy_orm.patterns.taggable import Taggable
 
 
-class TagBase(HelperBase):
-    tag: str
+class TagBase(Base):
+    id: uuid.UUID = uuid.uuid4
+    tag: str = ""
 
     __inheritance__ = False
     cached_mixin = None
 
     @classmethod
     def mixin(cls) -> Type[Taggable]:
         if cls.cached_mixin:
             return cls.cached_mixin
         tag_cls: Type[TagBase] = cls
 
-        class Mixin(Taggable, HelperBase):
+        class Mixin(Taggable, Base):
             cached_tag_association_cls = None
 
             @classmethod
             def relations(cls, checked=None):
                 super_relations = super().relations(checked=checked)
                 return super_relations & {cls.tag_association_cls()}
 
@@ -35,30 +36,28 @@
                     return cls.cached_tag_association_cls
 
                 class TagAssociation(tag_cls.declarative_base):
                     id: uuid.UUID = uuid.uuid4
                     tag: tag_cls
                     parent: cls = None
 
-                    __tablename__ = cls.__tablename__ + '_tag'
+                    __tablename__ = cls.__tablename__ + "_tag"
                     __inheritance__ = False
 
                     @declared_attr
                     def tag_str(self):
-                        return association_proxy('tag', 'tag')
+                        return association_proxy("tag", "tag")
 
                     @validates("tag")
                     def _validate_tag(self, key, value):
                         session = object_session(self)
                         if session is not None:
                             v = value.value
                             with session.no_autoflush:
-                                uvalue = session.query(tag_cls) \
-                                    .filter_by(tag=v) \
-                                    .first()
+                                uvalue = session.query(tag_cls).filter_by(tag=v).first()
                                 if uvalue:
                                     session.expunge(value)
                                     return uvalue
                         return value
 
                 tag_name = TagAssociation.__name__
                 tag_module = TagAssociation.__module__
@@ -69,42 +68,35 @@
                 cls.cached_tag_association_cls = TagAssociation
 
                 return TagAssociation
 
             @declared_attr
             def tag_associations(self):
                 return relationship(
-                    self.tag_association_cls(),
-                    cascade="all, delete, delete-orphan"
+                    self.tag_association_cls(), cascade="all, delete, delete-orphan"
                 )
 
             @validates("tag_associations")
             def _validate_tag_associations(self, key, value):
                 session = object_session(self)
                 if session is not None:
                     tag = value.tag
                     with session.no_autoflush:
-                        existing_tag = session.query(tag_cls) \
-                            .filter_by(tag=tag) \
-                            .first()
+                        existing_tag = session.query(tag_cls).filter_by(tag=tag).first()
                         if existing_tag:
                             session.expunge(existing_tag)
                             value.tag = existing_tag
                 return value
 
             @declared_attr
             def tags(self):
                 TagAssociation = self.tag_association_cls()
                 Tag: Type[TagBase] = tag_cls
 
                 def creator(_tag):
                     # from context_helper import ctx
                     return TagAssociation(tag=Tag(tag=_tag))
 
-                return association_proxy(
-                    'tag_associations',
-                    'tag_str',
-                    creator=creator
-                )
+                return association_proxy("tag_associations", "tag_str", creator=creator)
 
         cls.cached_mixin = Mixin
         return Mixin
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/patterns/tag_mixin.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/patterns/tag_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,44 +2,39 @@
 from typing import List
 
 from sqlalchemy import ForeignKey
 from sqlalchemy.ext.associationproxy import association_proxy
 from sqlalchemy.orm import relationship, mapped_column
 from sqlalchemy.orm.decl_api import declared_attr
 
-from sqlalchemy_orm.base.helper import HelperBase
+from sqlalchemy_orm.base.helper import Base
 from sqlalchemy_orm.patterns.taggable import Taggable
 
 
 class TagMixin(Taggable):
-
     cached_tag_class = None
 
     @classmethod
     def tag_cls(cls):
         if cls.cached_tag_class is not None:
             return cls.cached_tag_class
 
-        if not issubclass(cls, HelperBase):
-            raise TypeError(
-                f"TagMixin class {cls} must be a subclass of {HelperBase}."
-            )
+        if not issubclass(cls, Base):
+            raise TypeError(f"TagMixin class {cls} must be a subclass of {Base}.")
 
         parent_table = cls.__tablename__
         primary_key = cls.primary_keys()[0].name
 
         class Tag(cls.declarative_base):
-            id: str = uuid.uuid4
+            id: uuid.UUID = uuid.uuid4
             tag: str
-            parent_id = mapped_column(
-                ForeignKey(f"{parent_table}.{primary_key}")
-            )
+            parent_id = mapped_column(ForeignKey(f"{parent_table}.{primary_key}"))
             parent = relationship(cls)
 
-            __tablename__ = cls.__tablename__ + '_tag'
+            __tablename__ = cls.__tablename__ + "_tag"
             __inheritance__ = False
             __parent_cls__ = cls
 
         Tag.__name__ = cls.__name__ + Tag.__name__
         Tag.__qualname__ = Tag.__name__
         Tag.__module__ = cls.__module__ + Tag.__module__
         cls.cached_tag_class = Tag
@@ -47,19 +42,17 @@
         return Tag
 
     @declared_attr
     def tag_objects(self):
         tag_class = self.tag_cls()
         return relationship(
             tag_class,
-            back_populates='parent',
+            back_populates="parent",
             cascade="all, delete, delete-orphan",
-            lazy='dynamic'
+            lazy="dynamic",
         )
 
     @declared_attr
     def tags(self) -> List[str]:
         return association_proxy(
-            'tag_objects',
-            'tag',
-            creator=lambda tag: self.tag_cls()(tag=tag)
+            "tag_objects", "tag", creator=lambda tag: self.tag_cls()(tag=tag)
         )
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/proxy.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,49 +2,50 @@
 
 
 class Proxy:
     """Acts as a proxy.  Forwards all operations to
     a proxied object.  The only operations not supported for forwarding
     are right handed operands and any kind of assignment.
     """
-    __slots__ = ('__local', '__dict__', '__name__', '__wrapped__')
+
+    __slots__ = ("__local", "__dict__", "__name__", "__wrapped__")
 
     def __init__(self, local, name=None):
-        object.__setattr__(self, '_Proxy__local', local)
-        object.__setattr__(self, '__name__', name)
-        if callable(local) and not hasattr(local, '__release_local__'):
-            object.__setattr__(self, '__wrapped__', local)
+        object.__setattr__(self, "_Proxy__local", local)
+        object.__setattr__(self, "__name__", name)
+        if callable(local) and not hasattr(local, "__release_local__"):
+            object.__setattr__(self, "__wrapped__", local)
 
     def _get_current_object(self):
-        if not hasattr(self.__local, '__release_local__'):
+        if not hasattr(self.__local, "__release_local__"):
             return self.__local()
         try:
             return getattr(self.__local, self.__name__)
         except AttributeError:
-            raise RuntimeError('no object bound to %s' % self.__name__)
+            raise RuntimeError("no object bound to %s" % self.__name__)
 
     @property
     def __class__(self):
         try:
             return self._get_current_object().__class__
         except Exception as _:
             return Proxy
 
     @property
     def __dict__(self):
         try:
             return self._get_current_object().__dict__
         except RuntimeError:
-            raise AttributeError('__dict__')
+            raise AttributeError("__dict__")
 
     def __repr__(self):
         try:
             obj = self._get_current_object()
         except RuntimeError:
-            return '<%s unbound>' % self.__class__.__name__
+            return "<%s unbound>" % self.__class__.__name__
         return repr(obj)
 
     def __bool__(self):
         try:
             return bool(self._get_current_object())
         except RuntimeError:
             return False
@@ -55,15 +56,15 @@
     def __dir__(self):
         try:
             return dir(self._get_current_object())
         except RuntimeError:
             return []
 
     def __getattr__(self, name):
-        if name == '__members__':
+        if name == "__members__":
             return dir(self._get_current_object())
         return getattr(self._get_current_object(), name)
 
     def __setitem__(self, key, value):
         self._get_current_object()[key] = value
 
     def __delitem__(self, key):
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/query.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/query.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 from sqlalchemy.orm import Query as SQLAlchemyQuery
 
 
 class QueryAdapter:
-
     def apply(self, query, entities=None):
         return query
 
 
 class Query(SQLAlchemyQuery):
-
     def _apply_adapters(self, *criterion):
         query = self
-        criterion = [
-            criteria
-            for criteria in criterion
-            if criteria is not None
-        ]
-        entities = [cd['type'] for cd in self.column_descriptions]
+        criterion = [criteria for criteria in criterion if criteria is not None]
+        entities = [cd["type"] for cd in self.column_descriptions]
         for criteria in [*criterion]:
             if isinstance(criteria, QueryAdapter):
                 criterion.remove(criteria)
                 query = criteria.apply(query, entities)
 
         return criterion, query
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/typemapper.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/typemapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 
 from sqlalchemy.sql.type_api import TypeEngine
 
 from sqlalchemy_orm.utils import get_all_subclasses
 
 
 class TypeFactory:
-
     def __init__(self, type_map=None):
         pass
 
     def to_type(self, python_type: Type) -> Optional[Type[TypeEngine]]:
         pass
 
 
 class TypeMapper:
-
     def __init__(self, type_map=None, types=None):
         if not types:
             types = []
 
         if not type_map:
             type_map = {}
 
@@ -33,30 +31,31 @@
 
             try:
                 if callable(type_):
                     type_obj = type_()
                 else:
                     type_obj = type_
 
-                if not hasattr(type_obj, '__visit_name__'):
+                if not hasattr(type_obj, "__visit_name__"):
                     continue
 
                 python_type = type_obj.python_type
 
             except (NotImplementedError, AssertionError, TypeError):
                 if type_ in types:
                     raise TypeError(
                         f"Custom type '{type}' did not specify a Python type"
                     )
             except Exception:
                 pass
             else:
                 type_map = self.type_map
-                if python_type not in type_map.keys() or \
-                        issubclass(type_map[python_type].__class__, type_):
+                if python_type not in type_map.keys() or issubclass(
+                    type_map[python_type].__class__, type_
+                ):
                     self.type_map[python_type] = type_obj
                 elif type_obj in self.type_map.values():
                     raise TypeError(
                         f"Types must be consistently mapped in both "
                         f"directions, '{type}' already mapped."
                     )
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm/utils.py` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm/utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm.egg-info/PKG-INFO` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-orm
-Version: 1.2.5
+Version: 1.2.6
 Summary: Data Relation Mapping framework for Python.
 Home-page: https://gitlab.com/parob/sqlalchemy-orm
-Download-URL: https://gitlab.com/parob/sqlalchemy-orm/-/archive/v1.2.5/sqlalchemy-orm-v1.2.5.tar.gz
+Download-URL: https://gitlab.com/parob/sqlalchemy-orm/-/archive/v1.2.6/sqlalchemy-orm-v1.2.6.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: SQLAlchemy,ORM
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlalchemy-orm-1.2.5/sqlalchemy_orm.egg-info/SOURCES.txt` & `sqlalchemy-orm-1.2.6/sqlalchemy_orm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 sqlalchemy_orm.egg-info/SOURCES.txt
 sqlalchemy_orm.egg-info/dependency_links.txt
 sqlalchemy_orm.egg-info/requires.txt
 sqlalchemy_orm.egg-info/top_level.txt
 sqlalchemy_orm/base/__init__.py
 sqlalchemy_orm/base/base.py
 sqlalchemy_orm/base/helper.py
-sqlalchemy_orm/base/inheritance.py
 sqlalchemy_orm/base/mapper.py
 sqlalchemy_orm/eralchemy/__init__.py
 sqlalchemy_orm/eralchemy/cst.py
 sqlalchemy_orm/eralchemy/helpers.py
 sqlalchemy_orm/eralchemy/main.py
 sqlalchemy_orm/eralchemy/models.py
 sqlalchemy_orm/eralchemy/parser.py
```

