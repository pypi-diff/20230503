# Comparing `tmp/Pyckson-1.8.1.tar.gz` & `tmp/Pyckson-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Pyckson-1.8.1.tar", last modified: Mon Feb  3 09:35:37 2020, max compression
+gzip compressed data, was "dist/Pyckson-1.9.0.tar", last modified: Mon May  4 09:03:46 2020, max compression
```

## Comparing `Pyckson-1.8.1.tar` & `Pyckson-1.9.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-02-03 09:35:37.000000 Pyckson-1.8.1/
--rw-r--r--   0 jean      (1000) jean      (1000)      355 2020-02-03 09:35:37.000000 Pyckson-1.8.1/PKG-INFO
--rw-rw-r--   0 jean      (1000) jean      (1000)     2048 2020-01-30 10:25:57.000000 Pyckson-1.8.1/README.md
--rw-r--r--   0 jean      (1000) jean      (1000)       38 2020-02-03 09:35:37.000000 Pyckson-1.8.1/setup.cfg
--rw-rw-r--   0 jean      (1000) jean      (1000)     1005 2018-04-24 14:44:43.000000 Pyckson-1.8.1/setup.py
-drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-02-03 09:35:37.000000 Pyckson-1.8.1/src/
-drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-02-03 09:35:37.000000 Pyckson-1.8.1/src/Pyckson.egg-info/
--rw-rw-r--   0 jean      (1000) jean      (1000)      355 2020-02-03 09:35:37.000000 Pyckson-1.8.1/src/Pyckson.egg-info/PKG-INFO
--rw-rw-r--   0 jean      (1000) jean      (1000)      933 2020-02-03 09:35:37.000000 Pyckson-1.8.1/src/Pyckson.egg-info/SOURCES.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)        1 2020-02-03 09:35:37.000000 Pyckson-1.8.1/src/Pyckson.egg-info/dependency_links.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)        6 2020-02-03 09:35:37.000000 Pyckson-1.8.1/src/Pyckson.egg-info/requires.txt
--rw-rw-r--   0 jean      (1000) jean      (1000)        8 2020-02-03 09:35:37.000000 Pyckson-1.8.1/src/Pyckson.egg-info/top_level.txt
-drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-02-03 09:35:37.000000 Pyckson-1.8.1/src/pyckson/
--rw-rw-r--   0 jean      (1000) jean      (1000)      330 2020-02-03 09:34:53.000000 Pyckson-1.8.1/src/pyckson/__init__.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      920 2020-02-03 09:32:17.000000 Pyckson-1.8.1/src/pyckson/const.py
-drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-02-03 09:35:37.000000 Pyckson-1.8.1/src/pyckson/dates/
--rw-rw-r--   0 jean      (1000) jean      (1000)        0 2018-04-24 14:44:43.000000 Pyckson-1.8.1/src/pyckson/dates/__init__.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      955 2018-04-24 14:44:43.000000 Pyckson-1.8.1/src/pyckson/dates/arrow.py
--rw-rw-r--   0 jean      (1000) jean      (1000)     1109 2020-01-30 09:11:15.000000 Pyckson-1.8.1/src/pyckson/dates/helpers.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      298 2018-04-24 14:44:43.000000 Pyckson-1.8.1/src/pyckson/dates/model.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      395 2018-04-24 14:44:43.000000 Pyckson-1.8.1/src/pyckson/dates/raw_formatter.py
--rw-rw-r--   0 jean      (1000) jean      (1000)     2425 2020-01-30 09:11:15.000000 Pyckson-1.8.1/src/pyckson/decorators.py
--rw-rw-r--   0 jean      (1000) jean      (1000)     3224 2020-01-30 09:10:02.000000 Pyckson-1.8.1/src/pyckson/helpers.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      669 2017-07-31 13:31:16.000000 Pyckson-1.8.1/src/pyckson/json.py
-drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-02-03 09:35:37.000000 Pyckson-1.8.1/src/pyckson/model/
--rw-rw-r--   0 jean      (1000) jean      (1000)        0 2017-07-31 13:31:16.000000 Pyckson-1.8.1/src/pyckson/model/__init__.py
--rw-rw-r--   0 jean      (1000) jean      (1000)     2581 2020-01-30 09:22:00.000000 Pyckson-1.8.1/src/pyckson/model/builder.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      963 2020-01-30 09:21:56.000000 Pyckson-1.8.1/src/pyckson/model/helpers.py
--rw-rw-r--   0 jean      (1000) jean      (1000)     1108 2018-03-08 09:58:55.000000 Pyckson-1.8.1/src/pyckson/model/model.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      784 2018-03-08 09:34:55.000000 Pyckson-1.8.1/src/pyckson/model/union.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      649 2019-01-29 15:36:19.000000 Pyckson-1.8.1/src/pyckson/parser.py
-drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-02-03 09:35:37.000000 Pyckson-1.8.1/src/pyckson/parsers/
--rw-rw-r--   0 jean      (1000) jean      (1000)        0 2017-07-31 13:31:16.000000 Pyckson-1.8.1/src/pyckson/parsers/__init__.py
--rw-rw-r--   0 jean      (1000) jean      (1000)     2844 2020-01-30 09:22:42.000000 Pyckson-1.8.1/src/pyckson/parsers/advanced.py
--rw-rw-r--   0 jean      (1000) jean      (1000)     1413 2019-01-29 16:00:55.000000 Pyckson-1.8.1/src/pyckson/parsers/base.py
--rw-rw-r--   0 jean      (1000) jean      (1000)     3532 2020-01-30 09:16:39.000000 Pyckson-1.8.1/src/pyckson/parsers/provider.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      447 2017-07-31 13:31:16.000000 Pyckson-1.8.1/src/pyckson/providers.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      382 2019-01-29 15:36:19.000000 Pyckson-1.8.1/src/pyckson/serializer.py
-drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-02-03 09:35:37.000000 Pyckson-1.8.1/src/pyckson/serializers/
--rw-rw-r--   0 jean      (1000) jean      (1000)        0 2017-07-31 13:31:16.000000 Pyckson-1.8.1/src/pyckson/serializers/__init__.py
--rw-rw-r--   0 jean      (1000) jean      (1000)     2234 2020-01-30 09:09:29.000000 Pyckson-1.8.1/src/pyckson/serializers/advanced.py
--rw-rw-r--   0 jean      (1000) jean      (1000)      815 2019-01-29 16:00:55.000000 Pyckson-1.8.1/src/pyckson/serializers/base.py
--rw-rw-r--   0 jean      (1000) jean      (1000)     2589 2020-01-30 09:22:58.000000 Pyckson-1.8.1/src/pyckson/serializers/provider.py
+drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-05-04 09:03:46.000000 Pyckson-1.9.0/
+-rw-r--r--   0 jean      (1000) jean      (1000)      355 2020-05-04 09:03:46.000000 Pyckson-1.9.0/PKG-INFO
+-rw-rw-r--   0 jean      (1000) jean      (1000)     2048 2020-01-30 10:25:57.000000 Pyckson-1.9.0/README.md
+-rw-r--r--   0 jean      (1000) jean      (1000)       38 2020-05-04 09:03:46.000000 Pyckson-1.9.0/setup.cfg
+-rw-rw-r--   0 jean      (1000) jean      (1000)     1005 2018-04-24 14:44:43.000000 Pyckson-1.9.0/setup.py
+drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-05-04 09:03:46.000000 Pyckson-1.9.0/src/
+drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-05-04 09:03:46.000000 Pyckson-1.9.0/src/Pyckson.egg-info/
+-rw-rw-r--   0 jean      (1000) jean      (1000)      355 2020-05-04 09:03:46.000000 Pyckson-1.9.0/src/Pyckson.egg-info/PKG-INFO
+-rw-rw-r--   0 jean      (1000) jean      (1000)      957 2020-05-04 09:03:46.000000 Pyckson-1.9.0/src/Pyckson.egg-info/SOURCES.txt
+-rw-rw-r--   0 jean      (1000) jean      (1000)        1 2020-05-04 09:03:46.000000 Pyckson-1.9.0/src/Pyckson.egg-info/dependency_links.txt
+-rw-rw-r--   0 jean      (1000) jean      (1000)        6 2020-05-04 09:03:46.000000 Pyckson-1.9.0/src/Pyckson.egg-info/requires.txt
+-rw-rw-r--   0 jean      (1000) jean      (1000)        8 2020-05-04 09:03:46.000000 Pyckson-1.9.0/src/Pyckson.egg-info/top_level.txt
+drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-05-04 09:03:46.000000 Pyckson-1.9.0/src/pyckson/
+-rw-rw-r--   0 jean      (1000) jean      (1000)      372 2020-05-04 09:02:36.000000 Pyckson-1.9.0/src/pyckson/__init__.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      968 2020-05-04 08:12:56.000000 Pyckson-1.9.0/src/pyckson/const.py
+drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-05-04 09:03:46.000000 Pyckson-1.9.0/src/pyckson/dates/
+-rw-rw-r--   0 jean      (1000) jean      (1000)        0 2018-04-24 14:44:43.000000 Pyckson-1.9.0/src/pyckson/dates/__init__.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      955 2018-04-24 14:44:43.000000 Pyckson-1.9.0/src/pyckson/dates/arrow.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)     1109 2020-05-04 08:27:39.000000 Pyckson-1.9.0/src/pyckson/dates/helpers.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      298 2018-04-24 14:44:43.000000 Pyckson-1.9.0/src/pyckson/dates/model.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      395 2018-04-24 14:44:43.000000 Pyckson-1.9.0/src/pyckson/dates/raw_formatter.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)     2938 2020-05-04 08:55:56.000000 Pyckson-1.9.0/src/pyckson/decorators.py
+-rw-r--r--   0 jean      (1000) jean      (1000)      610 2020-05-04 08:18:41.000000 Pyckson-1.9.0/src/pyckson/defaults.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)     3404 2020-05-04 08:12:56.000000 Pyckson-1.9.0/src/pyckson/helpers.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      669 2017-07-31 13:31:16.000000 Pyckson-1.9.0/src/pyckson/json.py
+drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-05-04 09:03:46.000000 Pyckson-1.9.0/src/pyckson/model/
+-rw-rw-r--   0 jean      (1000) jean      (1000)        0 2017-07-31 13:31:16.000000 Pyckson-1.9.0/src/pyckson/model/__init__.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)     2653 2020-05-04 08:00:04.000000 Pyckson-1.9.0/src/pyckson/model/builder.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      963 2020-01-30 09:21:56.000000 Pyckson-1.9.0/src/pyckson/model/helpers.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)     1108 2018-03-08 09:58:55.000000 Pyckson-1.9.0/src/pyckson/model/model.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      784 2018-03-08 09:34:55.000000 Pyckson-1.9.0/src/pyckson/model/union.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      649 2019-01-29 15:36:19.000000 Pyckson-1.9.0/src/pyckson/parser.py
+drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-05-04 09:03:46.000000 Pyckson-1.9.0/src/pyckson/parsers/
+-rw-rw-r--   0 jean      (1000) jean      (1000)        0 2017-07-31 13:31:16.000000 Pyckson-1.9.0/src/pyckson/parsers/__init__.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)     2844 2020-01-30 09:22:42.000000 Pyckson-1.9.0/src/pyckson/parsers/advanced.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)     1413 2019-01-29 16:00:55.000000 Pyckson-1.9.0/src/pyckson/parsers/base.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)     3532 2020-01-30 09:16:39.000000 Pyckson-1.9.0/src/pyckson/parsers/provider.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      447 2017-07-31 13:31:16.000000 Pyckson-1.9.0/src/pyckson/providers.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      382 2019-01-29 15:36:19.000000 Pyckson-1.9.0/src/pyckson/serializer.py
+drwxr-xr-x   0 jean      (1000) jean      (1000)        0 2020-05-04 09:03:46.000000 Pyckson-1.9.0/src/pyckson/serializers/
+-rw-rw-r--   0 jean      (1000) jean      (1000)        0 2017-07-31 13:31:16.000000 Pyckson-1.9.0/src/pyckson/serializers/__init__.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)     2234 2020-01-30 09:09:29.000000 Pyckson-1.9.0/src/pyckson/serializers/advanced.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)      815 2019-01-29 16:00:55.000000 Pyckson-1.9.0/src/pyckson/serializers/base.py
+-rw-rw-r--   0 jean      (1000) jean      (1000)     2589 2020-01-30 09:22:58.000000 Pyckson-1.9.0/src/pyckson/serializers/provider.py
```

### Comparing `Pyckson-1.8.1/README.md` & `Pyckson-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/setup.py` & `Pyckson-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/src/Pyckson.egg-info/SOURCES.txt` & `Pyckson-1.9.0/src/Pyckson.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/Pyckson.egg-info/SOURCES.txt
 src/Pyckson.egg-info/dependency_links.txt
 src/Pyckson.egg-info/requires.txt
 src/Pyckson.egg-info/top_level.txt
 src/pyckson/__init__.py
 src/pyckson/const.py
 src/pyckson/decorators.py
+src/pyckson/defaults.py
 src/pyckson/helpers.py
 src/pyckson/json.py
 src/pyckson/parser.py
 src/pyckson/providers.py
 src/pyckson/serializer.py
 src/pyckson/dates/__init__.py
 src/pyckson/dates/arrow.py
```

### Comparing `Pyckson-1.8.1/src/pyckson/const.py` & `Pyckson-1.9.0/src/pyckson/const.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 PYCKSON_MODEL = '__{cls}_pyckson_model'
 PYCKSON_ENUM_OPTIONS = '__{cls}_pyckson_enum'
 PYCKSON_NAMERULE = '__{cls}_pyckson_namerule'
 PYCKSON_SERIALIZER = '__{cls}_pyckson_serializer'
 PYCKSON_PARSER = '__{cls}_pyckson_parser'
 PYCKSON_DATE_FORMATTER = '__{cls}_pyckson_date_formatter'
 PYCKSON_EXPLICIT_NULLS = '__{cls}_pyckson_explicit_nulls'
+PYCKSON_RULE_ATTR = '__{cls}_pyckson_rule_attr'
 BASIC_TYPES = [int, str, float]
 EXTRA_TYPES = [bool, bytes, datetime.time]
 DATE_TYPES = [datetime.date, datetime.datetime]
 
 ENUM_CASE_INSENSITIVE = 'case-insensitive'
```

### Comparing `Pyckson-1.8.1/src/pyckson/dates/arrow.py` & `Pyckson-1.9.0/src/pyckson/dates/arrow.py`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/src/pyckson/dates/helpers.py` & `Pyckson-1.9.0/src/pyckson/dates/helpers.py`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/src/pyckson/decorators.py` & `Pyckson-1.9.0/src/pyckson/decorators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 
 from pyckson.const import PYCKSON_TYPEINFO, PYCKSON_NAMERULE, PYCKSON_ENUM_OPTIONS, \
     ENUM_CASE_INSENSITIVE, PYCKSON_SERIALIZER, PYCKSON_PARSER, PYCKSON_DATE_FORMATTER, PYCKSON_EXPLICIT_NULLS, \
     get_cls_attr, set_cls_attr
 from pyckson.dates.model import DateFormatter
-from pyckson.helpers import same_name, name_by_dict, get_name_rule
+from pyckson.helpers import same_name, name_by_dict, get_name_rule, camel_case_name, using
 from pyckson.model.helpers import ModelProviderImpl
 from pyckson.parser import parse
 
 
 def listtype(param_name, param_sub_type):
     def class_decorator(cls):
         type_info = get_cls_attr(cls, PYCKSON_TYPEINFO, dict())
@@ -24,66 +24,86 @@
 
 def pyckson(cls):
     ModelProviderImpl().get_or_build(cls)
     setattr(cls, 'parse', lambda json: parse(cls, json))
     return cls
 
 
+@using(PYCKSON_ENUM_OPTIONS)
 def caseinsensitive(cls):
     """Annotation function to set an Enum to be case insensitive on parsing"""
     if not issubclass(cls, Enum):
         raise TypeError('caseinsensitive decorator can only be applied to subclasses of enum.Enum')
     enum_options = get_cls_attr(cls, PYCKSON_ENUM_OPTIONS, {})
     enum_options[ENUM_CASE_INSENSITIVE] = True
     set_cls_attr(cls, PYCKSON_ENUM_OPTIONS, enum_options)
     return cls
 
 
 def namerule(name_function):
+    @using(PYCKSON_NAMERULE)
     def class_decorator(cls):
         set_cls_attr(cls, PYCKSON_NAMERULE, name_function)
         return cls
 
     return class_decorator
 
 
+@using(PYCKSON_NAMERULE)
 def no_camel_case(cls):
     set_cls_attr(cls, PYCKSON_NAMERULE, same_name)
     return cls
 
 
+@using(PYCKSON_NAMERULE)
+def use_camel_case(cls):
+    set_cls_attr(cls, PYCKSON_NAMERULE, camel_case_name)
+    return cls
+
+
 def rename(**kwargs):
+    @using(PYCKSON_NAMERULE)
     def class_decorator(cls):
         name_function = name_by_dict(kwargs, get_name_rule(cls))
         set_cls_attr(cls, PYCKSON_NAMERULE, name_function)
         return cls
 
     return class_decorator
 
 
 def custom_serializer(serializer_cls):
+    @using(PYCKSON_SERIALIZER)
     def class_decorator(cls):
         set_cls_attr(cls, PYCKSON_SERIALIZER, serializer_cls)
         return cls
 
     return class_decorator
 
 
 def custom_parser(parser_cls):
+    @using(PYCKSON_PARSER)
     def class_decorator(cls):
         set_cls_attr(cls, PYCKSON_PARSER, parser_cls)
         return cls
 
     return class_decorator
 
 
 def date_formatter(formatter: DateFormatter):
+    @using(PYCKSON_DATE_FORMATTER)
     def class_decorator(cls):
         set_cls_attr(cls, PYCKSON_DATE_FORMATTER, formatter)
         return cls
 
     return class_decorator
 
 
+@using(PYCKSON_EXPLICIT_NULLS)
 def explicit_nulls(cls):
     set_cls_attr(cls, PYCKSON_EXPLICIT_NULLS, True)
     return cls
+
+
+@using(PYCKSON_EXPLICIT_NULLS)
+def no_explicit_nulls(cls):
+    set_cls_attr(cls, PYCKSON_EXPLICIT_NULLS, False)
+    return cls
```

### Comparing `Pyckson-1.8.1/src/pyckson/helpers.py` & `Pyckson-1.9.0/src/pyckson/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 try:
     from typing import _ForwardRef as ForwardRef
 except ImportError:
     from typing import ForwardRef
 
 from pyckson.const import PYCKSON_ATTR, BASIC_TYPES, PYCKSON_NAMERULE, PYCKSON_SERIALIZER, PYCKSON_PARSER, EXTRA_TYPES, \
-    get_cls_attr
+    get_cls_attr, set_cls_attr, PYCKSON_RULE_ATTR
 from pyckson.parsers.base import Parser
 from pyckson.serializers.base import Serializer
 
 
 def is_pyckson(obj_type):
     return get_cls_attr(obj_type, PYCKSON_ATTR, False)
 
@@ -121,7 +121,15 @@
     if hasattr(annotation, '_name'):
         return annotation._name == 'Dict'
     else:
         try:
             return issubclass(annotation, Dict)
         except TypeError:
             return False
+
+
+def using(attr):
+    def class_decorator(cls):
+        set_cls_attr(cls, PYCKSON_RULE_ATTR, attr)
+        return cls
+
+    return class_decorator
```

### Comparing `Pyckson-1.8.1/src/pyckson/json.py` & `Pyckson-1.9.0/src/pyckson/json.py`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/src/pyckson/model/builder.py` & `Pyckson-1.9.0/src/pyckson/model/builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from inspect import Parameter, getmembers, signature
 
 from pyckson.const import PYCKSON_TYPEINFO, get_cls_attr
+from pyckson.defaults import apply_defaults
 from pyckson.helpers import get_name_rule
 from pyckson.model.model import PycksonModel, PycksonAttribute
 from pyckson.model.union import inspect_optional_typing
 from pyckson.providers import SerializerProvider, ParserProvider
 
 
 class PycksonModelBuilder:
     def __init__(self, cls, serializer_provider: SerializerProvider, parser_provider: ParserProvider):
         self.cls = cls
+        apply_defaults(cls)
         self.serializer_provider = serializer_provider
         self.parser_provider = parser_provider
         self.type_info = get_cls_attr(cls, PYCKSON_TYPEINFO, dict())
         self.name_rule = get_name_rule(cls)
 
     def find_constructor(self):
         for member in getmembers(self.cls):
```

### Comparing `Pyckson-1.8.1/src/pyckson/model/helpers.py` & `Pyckson-1.9.0/src/pyckson/model/helpers.py`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/src/pyckson/model/model.py` & `Pyckson-1.9.0/src/pyckson/model/model.py`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/src/pyckson/model/union.py` & `Pyckson-1.9.0/src/pyckson/model/union.py`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/src/pyckson/parser.py` & `Pyckson-1.9.0/src/pyckson/parser.py`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/src/pyckson/parsers/advanced.py` & `Pyckson-1.9.0/src/pyckson/parsers/advanced.py`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/src/pyckson/parsers/base.py` & `Pyckson-1.9.0/src/pyckson/parsers/base.py`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/src/pyckson/parsers/provider.py` & `Pyckson-1.9.0/src/pyckson/parsers/provider.py`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/src/pyckson/serializers/advanced.py` & `Pyckson-1.9.0/src/pyckson/serializers/advanced.py`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/src/pyckson/serializers/base.py` & `Pyckson-1.9.0/src/pyckson/serializers/base.py`

 * *Files identical despite different names*

### Comparing `Pyckson-1.8.1/src/pyckson/serializers/provider.py` & `Pyckson-1.9.0/src/pyckson/serializers/provider.py`

 * *Files identical despite different names*

