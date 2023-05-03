# Comparing `tmp/rom-1.0.5.tar.gz` & `tmp/rom-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rom-1.0.5.tar", last modified: Tue Nov 15 19:09:30 2022, max compression
+gzip compressed data, was "dist/rom-1.0.6.tar", last modified: Wed May  3 04:05:06 2023, max compression
```

## Comparing `rom-1.0.5.tar` & `rom-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2022-11-15 19:09:30.000000 rom-1.0.5/
-drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2022-11-15 19:09:30.000000 rom-1.0.5/rom.egg-info/
--rw-rw-r--   0 josiah    (1000) josiah    (1000)       10 2022-11-15 19:09:30.000000 rom-1.0.5/rom.egg-info/requires.txt
--rw-rw-r--   0 josiah    (1000) josiah    (1000)       47 2018-09-26 03:30:44.000000 rom-1.0.5/rom.egg-info/pbr.json
--rw-rw-r--   0 josiah    (1000) josiah    (1000)        1 2022-11-15 19:09:30.000000 rom-1.0.5/rom.egg-info/dependency_links.txt
--rw-rw-r--   0 josiah    (1000) josiah    (1000)      328 2022-11-15 19:09:30.000000 rom-1.0.5/rom.egg-info/SOURCES.txt
--rw-rw-r--   0 josiah    (1000) josiah    (1000)        4 2022-11-15 19:09:30.000000 rom-1.0.5/rom.egg-info/top_level.txt
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     8584 2022-11-15 19:09:30.000000 rom-1.0.5/rom.egg-info/PKG-INFO
--rw-rw-r--   0 josiah    (1000) josiah    (1000)       38 2022-11-15 19:09:30.000000 rom-1.0.5/setup.cfg
-drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2022-11-15 19:09:30.000000 rom-1.0.5/rom/
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     1857 2021-08-20 00:45:03.000000 rom-1.0.5/rom/exceptions.py
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     6975 2021-08-20 01:25:13.000000 rom-1.0.5/rom/wrappers.py
--rw-r--r--   0 josiah    (1000) josiah    (1000)    36132 2021-01-11 23:16:53.000000 rom-1.0.5/rom/util.py
--rw-r--r--   0 josiah    (1000) josiah    (1000)    28751 2020-07-12 04:36:23.000000 rom-1.0.5/rom/query.py
--rw-rw-r--   0 josiah    (1000) josiah    (1000)    44531 2021-08-20 00:45:03.000000 rom-1.0.5/rom/model.py
--rw-r--r--   0 josiah    (1000) josiah    (1000)     8062 2022-11-15 19:06:56.000000 rom-1.0.5/rom/__init__.py
--rw-rw-r--   0 josiah    (1000) josiah    (1000)    39511 2021-08-20 00:48:17.000000 rom-1.0.5/rom/columns.py
--rw-r--r--   0 josiah    (1000) josiah    (1000)    19323 2020-07-12 04:36:14.000000 rom-1.0.5/rom/index.py
--rw-r--r--   0 josiah    (1000) josiah    (1000)        5 2022-11-15 19:07:30.000000 rom-1.0.5/VERSION
--rw-rw-r--   0 josiah    (1000) josiah    (1000)       35 2018-09-26 03:27:59.000000 rom-1.0.5/MANIFEST.in
-drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2022-11-15 19:09:30.000000 rom-1.0.5/test/
--rw-rw-r--   0 josiah    (1000) josiah    (1000)    73622 2022-11-15 18:45:54.000000 rom-1.0.5/test/test_rom.py
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     6228 2022-11-15 19:07:30.000000 rom-1.0.5/README.rst
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     1300 2022-11-05 00:00:22.000000 rom-1.0.5/setup.py
--rw-rw-r--   0 josiah    (1000) josiah    (1000)     8584 2022-11-15 19:09:30.000000 rom-1.0.5/PKG-INFO
+drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-05-03 04:05:06.000000 rom-1.0.6/
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)        5 2023-05-03 03:40:57.000000 rom-1.0.6/VERSION
+drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-05-03 04:05:06.000000 rom-1.0.6/rom.egg-info/
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)      328 2023-05-03 04:05:06.000000 rom-1.0.6/rom.egg-info/SOURCES.txt
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)        1 2023-05-03 04:05:06.000000 rom-1.0.6/rom.egg-info/dependency_links.txt
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)       10 2023-05-03 04:05:06.000000 rom-1.0.6/rom.egg-info/requires.txt
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)       47 2018-09-26 03:30:44.000000 rom-1.0.6/rom.egg-info/pbr.json
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)        4 2023-05-03 04:05:06.000000 rom-1.0.6/rom.egg-info/top_level.txt
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     8585 2023-05-03 04:05:06.000000 rom-1.0.6/rom.egg-info/PKG-INFO
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     8585 2023-05-03 04:05:06.000000 rom-1.0.6/PKG-INFO
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     1300 2022-11-05 00:00:22.000000 rom-1.0.6/setup.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     6229 2023-05-03 03:40:37.000000 rom-1.0.6/README.rst
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)       35 2018-09-26 03:27:59.000000 rom-1.0.6/MANIFEST.in
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)       38 2023-05-03 04:05:06.000000 rom-1.0.6/setup.cfg
+drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-05-03 04:05:06.000000 rom-1.0.6/rom/
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)    28748 2023-05-03 03:40:37.000000 rom-1.0.6/rom/query.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)    36133 2023-05-03 03:40:37.000000 rom-1.0.6/rom/util.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     8063 2023-05-03 03:40:57.000000 rom-1.0.6/rom/__init__.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     1743 2023-05-03 04:04:46.000000 rom-1.0.6/rom/exceptions.py
+-rw-r--r--   0 josiah    (1000) josiah    (1000)    19323 2020-07-12 04:36:14.000000 rom-1.0.6/rom/index.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)     6975 2021-08-20 01:25:13.000000 rom-1.0.6/rom/wrappers.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)    36972 2023-05-03 04:04:46.000000 rom-1.0.6/rom/columns.py
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)    44929 2023-05-03 04:04:46.000000 rom-1.0.6/rom/model.py
+drwxrwxr-x   0 josiah    (1000) josiah    (1000)        0 2023-05-03 04:05:06.000000 rom-1.0.6/test/
+-rw-rw-r--   0 josiah    (1000) josiah    (1000)    74178 2023-05-03 03:40:57.000000 rom-1.0.6/test/test_rom.py
```

### Comparing `rom-1.0.5/rom.egg-info/PKG-INFO` & `rom-1.0.6/rom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rom
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Redis object mapper for Python
 Home-page: https://github.com/josiahcarlson/rom
 Author: Josiah Carlson
 Author-email: josiah.carlson@gmail.com
 License: GNU LGPL v2.1
 Description: 
         Rom - the Redis object mapper for Python
@@ -162,15 +162,15 @@
         delete that data, you have to run a cleanup function that literally has to
         scan over every entity in order to determine if the model had been expired. That
         is a huge waste and is the antithesis of good design.
         
         Instead, if you create a new ``expire_at`` float column with ``index=True``,
         the column can store when the entity is to expire. Then to expire the data, you
         can use: ``Model.query.filter(expire_at=(0, time.time())).limit(10)`` to (for
-        example) get up to the 10 oldest entites that need to be expired.
+        example) get up to the 10 oldest entities that need to be expired.
         
         Now, I know what you are thinking. You are thinking, "but I wish the data would
         just go away on its own." And I don't disagree. But for that to happen, Redis
         needs to grow Lua-script triggers, or you need to run a separate daemon to
         periodically clean up left-over data. But ... if you need to run a separate
         daemon to clean up left-over data by scanning all of your rom entities,
         wouldn't it just be better/faster in every way to keep an explicit column and do
```

### Comparing `rom-1.0.5/rom/exceptions.py` & `rom-1.0.6/rom/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,10 +36,7 @@
     'Raised when a model has a required column, but it is not provided on construction'
 
 class InvalidColumnValue(ColumnError):
     'Raised when you attempt to pass a primary key on entity creation or when data assigned to a column is the wrong type'
 
 class BulkError(ORMError):
     'Raised when using session.commit(fast=True) or equivalent, and there is at least one error.'
-
-class UnsafeError(ColumnError):
-    'Raised when an UnsafeColumn is accessed after the parent entity is deleted'
```

### Comparing `rom-1.0.5/rom/wrappers.py` & `rom-1.0.6/rom/wrappers.py`

 * *Files identical despite different names*

### Comparing `rom-1.0.5/rom/util.py` & `rom-1.0.6/rom/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
     This is a basic "equality" index keygen, primarily meant to be used for
     things like::
 
         Model.query.filter(col='value')
 
     Where ``FULL_TEXT`` would transform a sentence like "A Simple Sentence" into
     an inverted index searchable by the words "a", "simple", and/or "sentence",
-    ``IDENTITY`` will only be searchable by the orginal full sentence with the
+    ``IDENTITY`` will only be searchable by the original full sentence with the
     same capitalization - "A Simple Sentence". See ``IDENTITY_CI`` for the
     same function, only case-insensitive.
     '''
     if not val:
         return None
     if not isinstance(val, six.string_types_ex):
         val = str(val)
@@ -418,15 +418,15 @@
     loaded entities, offering the ability to call ``.save()`` on modified (or
     all) entities with ``.flush()`` or ``.commit()``.
 
     This is exposed via the ``session`` global variable, which is available
     when you ``import rom`` as ``rom.session``.
 
     .. note:: calling ``.flush()`` or ``.commit()`` doesn't cause all objects
-        to be written simultanously. They are written one-by-one, with any
+        to be written simultaneously. They are written one-by-one, with any
         error causing the call to fail.
     '''
     def __init__(self, *args, **kwargs):
         threading.local.__init__(self, *args, **kwargs)
         self._init()
 
     def _init(self):
@@ -561,15 +561,15 @@
 
 
             session.delete(obj)
             session.delete(obj1, obj2, ...)
             session.delete([obj1, obj2, ...])
 
         The keyword argument ``force=True`` can be provided, which can force
-        the deletion of an entitiy again, even if we believe it to already be
+        the deletion of an entity again, even if we believe it to already be
         deleted.
 
         If ``force=True``, we won't re-call the object's ``_before_delete()``
         method, but we will re-call ``_after_delete()``.
 
         .. note:: Objects are automatically dropped from the session after
             delete for the sake of cache coherency.
```

### Comparing `rom-1.0.5/rom/query.py` & `rom-1.0.6/rom/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             * *``rom.query._tuple_data_factory``* - when you want tuples instead
             * *``rom.query._namedtuple_data_factory``* - get namedtuples, see
               see warning below
 
         .. warning:: If you use the ``_namedtuple_data_factory``, and your
           columns include underscore prefixes, they will be stripped. If this
           results in a name collision, you *will* get an exception. If you want
-          differerent behavior, write your own 20 line factory function that
+          different behavior, write your own 20 line factory function that
           does exactly what you want, and pass it; they are really easy!
 
         '''
         include_pk = kwargs.pop('include_pk', False)
         decode = kwargs.pop('decode', True)
         ff = kwargs.pop('ff', _dict_data_factory)
 
@@ -246,15 +246,15 @@
 
         '''
         cur_filters = list(self._filters)
         for attr, value in kwargs.items():
             value = self._check(attr, value, which='filter')
 
             if isinstance(value, NUMERIC_TYPES):
-                # for simple numeric equiality filters
+                # for simple numeric equality filters
                 value = (value, value)
 
             if isinstance(value, six.string_types):
                 cur_filters.append('%s:%s'%(attr, value))
 
             elif six.PY3 and isinstance(value, bytes):
                 cur_filters.append('%s:%s'%(attr, value.decode('latin-1')))
```

### Comparing `rom-1.0.5/rom/model.py` & `rom-1.0.6/rom/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         seen = {}
         for comp in composite_unique:
             key = tuple(sorted(set(comp)))
             if len(key) == 1:
                 raise ColumnError("Single-column unique constraint: %r should be defined via 'unique=True' on the %r column"%(
                     comp, key[0]))
             if key in seen:
-                raise ColumnError("Multi-column unique constraint: %r not different than earlier constrant: %r"%(
+                raise ColumnError("Multi-column unique constraint: %r not different than earlier constraint: %r"%(
                     comp, seen[key]))
             for col in key:
                 if col not in columns:
                     raise ColumnError("Multi-column unique index %r references non-existant column %r"%(
                         comp, col))
                 if pkey == col:
                     raise ColumnError("Multi-column unique index %r references primary key column %r"%(
@@ -236,15 +236,15 @@
             y = Integer()
 
             unique_together = [
                 ('x', 'y'),
             ]
 
     .. note:: If one or more of the column values on an entity that is part of a
-        unique constrant is None in Python, the unique constraint won't apply.
+        unique constraint is None in Python, the unique constraint won't apply.
         This is the typical behavior of nulls in unique constraints inside both
         MySQL and Postgres.
     '''
     def __init__(self, **kwargs):
         self._new = not kwargs.pop('_loading', False)
         loading = not self._new
         extra_ok = kwargs.pop('_extra_ok', False)
@@ -337,30 +337,29 @@
         prefix = []
         suffix = []
         geo = []
         redis_data = {}
 
         # update individual columns
         for attr in cls._columns:
-            ikey = None
-            if attr in cls._unique:
-                ikey = "%s:%s:uidx"%(model, attr)
+            is_unique = attr in cls._unique
 
             ca = columns[attr]
             roval = None if is_new else old.get(attr)
             oval = ca._from_redis(roval) if roval is not None else None
 
             nval = new.get(attr)
             rnval = ca._to_redis(nval) if nval is not None else None
             if rnval is not None:
                 redis_data[attr] = rnval
 
             # Add/update standard index
             if ca._keygen and not delete and (nval is not None or not ca._allowed) and (ca._index or ca._prefix or ca._suffix):
                 generated = ca._keygen(attr, new)
+
                 if not generated:
                     # No index entries, we'll clean out old entries later
                     pass
 
                 elif isinstance(generated, (list, tuple, set)):
                     if ca._index:
                         for k in generated:
@@ -409,38 +408,52 @@
                                     suffix.append([attr, ex(nval[::-1])])
                             else:
                                 suffix.append([attr, ex(nval[::-1])])
 
                 else:
                     raise ColumnError("Don't know how to turn %r into a sequence of keys"%(generated,))
 
+            if is_unique:
+                if ca._keygen and not ca._index:
+                    roval = ca._keygen(attr, old) or [roval]
+                    rnval = ca._keygen(attr, new) or [rnval]
+                    generated = (roval if delete else rnval) or []
+                    roval = list(roval)[0] if roval else None
+                    rnval = list(rnval)[0] if rnval else None
+
+                    if not isinstance(generated, (tuple, list, set)):
+                        raise TypeError("keygen must return a tuple, list, or set not " + str(type(generated)))
+                elif delete:
+                    generated = [roval] if roval else []
+                else:
+                    generated = [rnval] if rnval else []
+
+                # only 1 item per column
+                for k in generated:
+                    if k is not None:
+                        (udeleted if delete else unique)[attr] = k
+                        break
+
+                if roval and roval != rnval and not delete:
+                    udeleted[attr] = roval
+
             if nval == oval and not full:
                 continue
 
             changes += 1
 
             # Delete removed columns
             if nval is None and oval is not None:
                 deleted.append(attr)
-                if ikey:
-                    udeleted[attr] = roval
                 continue
 
             # Add/update column value
             if nval is not None:
                 data[attr] = rnval
 
-            # Add/update unique index
-            if ikey:
-                if not isinstance(roval, str) and roval is not None:
-                    roval = columns[attr]._to_redis(roval)
-                if oval is not None and roval != rnval:
-                    udeleted[attr] = oval
-                if rnval is not None:
-                    unique[attr] = rnval
 
         # Add/update multi-column unique constraint
         for uniq in cls._cunique:
             attr = ':'.join(uniq)
 
             odata = [old.get(c) for c in uniq]
             ndata = [new.get(c) for c in uniq]
@@ -652,16 +665,14 @@
             if isinstance(value, tuple):
                 # this is a numeric range query, we'll just pull it directly
                 args = list(value)
                 for i, a in enumerate(args):
                     # Handle the ranges where None is -inf on the left and inf
                     # on the right when used in the context of a range tuple.
                     args[i] = ('-inf', 'inf')[i] if a is None else cls._columns[attr]._to_redis(a)
-                    # if args[i] is None and a is not None:
-                    #     args[i] = a
                 if _limit:
                     args.extend(_limit)
                 ids = conn.zrangebyscore('%s:%s:idx'%(model, attr), *args)
                 if not ids:
                     return []
                 return cls.get(ids)
 
@@ -745,15 +756,14 @@
             if psv not in exclude:
                 exclude[psv] = set()
             exclude[psv].add(v)
 
         excludes = ['inf'] + sorted(exclude, reverse=True)
         last = 0
         c = cls._connection
-        print(exclude)
         while excludes:
             exc = excludes.pop()
             # things that are between the matched items
             for chunk in _zrange_limit_iterator(c, idx, last, "(" + exc, blocksize):
                 ids = set(int(p.rpartition(b"\0")[-1]) for p in chunk)
                 if ids:
                     found = cls.get(list(ids))
@@ -837,15 +847,15 @@
           * *decimal_places* - the number of decimal places to the right of the
             decimal to round to inside Redis / Lua; note that for values ``>0``,
             this *will* introduce binary/decimal rounding problems; so small
             epsilon credit may go away, and you will want to explicitly round on
             the client on read + display. Or better yet; stick to integers.
           * *refresh_entities* - will refresh the entity data on transfer if
             ``True``-ish
-          * *refresh_index* - will refresh the update any relevant indexs after
+          * *refresh_index* - will refresh the update any relevant indexes after
             the transfer, if ``True``-ish; implies ``refresh_entities``
 
         ..warning: This doesn't magically create more bits for you. Values in
           Redis are either stored as up-to 64 bit integers (0 decimal places) or
           64 bit doubles with 53 bits of precision. For doubles, that means
           15-16 decimal digits. For 64 bit integers, that is 19+ digits, but
           only integers. So if you want to maximize both precision, and your
@@ -1174,15 +1184,14 @@
 def _zrange_limit_iterator(conn, key, vstart, end, count=100):
     """
     Utility function for iterating over chunks of a sorted-set index.
     """
     start = 0
     lc = count
     while lc == count:
-        print(vstart, end, start, count)
         chunk = conn.execute_command("zrangebyscore", key, vstart, end, "LIMIT", start, count)
         yield chunk
         lc = len(chunk)
         start += lc
 
 
 __all__ = [k for k, v in globals().items() if getattr(v, '__doc__', None) and k not in _skip]
```

### Comparing `rom-1.0.5/rom/__init__.py` & `rom-1.0.6/rom/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 delete that data, you have to run a cleanup function that literally has to
 scan over every entity in order to determine if the model had been expired. That
 is a huge waste and is the antithesis of good design.
 
 Instead, if you create a new ``expire_at`` float column with ``index=True``,
 the column can store when the entity is to expire. Then to expire the data, you
 can use: ``Model.query.filter(expire_at=(0, time.time())).limit(10)`` to (for
-example) get up to the 10 oldest entites that need to be expired.
+example) get up to the 10 oldest entities that need to be expired.
 
 Now, I know what you are thinking. You are thinking, "but I wish the data would
 just go away on its own." And I don't disagree. But for that to happen, Redis
 needs to grow Lua-script triggers, or you need to run a separate daemon to
 periodically clean up left-over data. But ... if you need to run a separate
 daemon to clean up left-over data by scanning all of your rom entities,
 wouldn't it just be better/faster in every way to keep an explicit column and do
@@ -188,15 +188,15 @@
 from .index import GeneralIndex, GeoIndex, Pattern, Prefix, Suffix
 from .model import _ModelMetaclass, Model
 from .query import NOT_NULL, Query
 from .util import (ClassProperty, _connect, session,
     _prefix_score, _script_load, _encode_unique_constraint,
     FULL_TEXT, CASE_INSENSITIVE, SIMPLE, SIMPLE_CI, IDENTITY, IDENTITY_CI)
 
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 
 COLUMN_TYPES = [Column, Integer, Boolean, Float, Decimal, DateTime, Date,
 Time, String, Text, Json, PrimaryKey, ManyToOne, ForeignModel, OneToMany,
 OneToOne, IndexOnly]
 
 NUMERIC_TYPES = six.integer_types + (float, _Decimal, datetime, date, dtime)
```

### Comparing `rom-1.0.5/rom/columns.py` & `rom-1.0.6/rom/columns.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 
 from .exceptions import (ORMError, InvalidOperation, ColumnError,
     MissingColumn, InvalidColumnValue, RestrictError)
 from .util import (_numeric_keygen, _string_keygen, _many_to_one_keygen,
     _boolean_keygen, dt2ts, ts2dt, t2ts, ts2t, session, _connect,
     STRING_INDEX_KEYGENS_STR)
 
-from .wrappers import ListWrapper, SetWrapper, HashWrapper, ZsetWrapper
-
 
 NULL = object()
 MODELS = {}
 MODELS_REFERENCED = {}
 _NUMERIC = (0, 0.0, _Decimal('0'), datetime(1970, 1, 1), date(1970, 1, 1), dtime(0, 0, 0))
 NO_ACTION_DEFAULT = object()
 SKIP_ON_DELETE = object()
@@ -198,15 +196,15 @@
           columns, and 2 convenient options for string/text columns)
         * If you set *required* to True, then you must have the column set
           during object construction: ``MyModel(col=val)``
         * If *index* and *prefix*, or *index* and *suffix* are set, the same
           keygen will be used for both the regular *index* as well as the
           *prefix* and/or *suffix* searches
         * If *prefix* is set, you can perform pattern matches over your data.
-          See documention on ``Query.like()`` for details.
+          See documentation on ``Query.like()`` for details.
         * Pattern matching over data is only guaranteed to be valid or correct
           for ANSI strings that do not include nulls, though we make an effort
           to support unicode strings and strings with embedded nulls
         * Prefix, suffix, and pattern matching are performed within a Lua
           script, so may have substantial execution time if there are a large
           number of matching prefix or suffix entries
         * Whenever possible, pattern matching will attempt to use any
@@ -247,24 +245,25 @@
         self._prefix = prefix
         self._suffix = suffix
         self._init = False
         self._model = None
         self._attr = None
         self._keygen = None
 
-        if (keygen or keygen2) and not (index or prefix or suffix):
-            raise ColumnError("Explicit keygen provided, but no index type spcified (index, prefix, and suffix all False)")
+        if (keygen or keygen2) and not (index or prefix or suffix or unique):
+            raise ColumnError("Explicit keygen provided, but no index type spcified (index, prefix, suffix, and unique all False)")
 
-        if not self._allowed and not hasattr(self, '_fmodel') and not hasattr(self, '_ftable') and not isinstance(self, IndexOnly):
+        indexonly = isinstance(self, IndexOnly)
+        if not self._allowed and not hasattr(self, '_fmodel') and not hasattr(self, '_ftable') and not indexonly:
             raise ColumnError("Missing valid class-level _allowed attribute on %r"%(type(self),))
 
         allowed = (self._allowed,) if isinstance(self._allowed, type) else self._allowed
         is_integer = all(issubclass(x, six.integer_types) for x in allowed)
         if unique:
-            if not (is_string or is_integer):
+            if not (is_string(allowed) or is_integer):
                 raise ColumnError("Unique columns can only be strings or integers")
 
         if keygen and keygen2:
             raise ColumnError("Can only specify one of 'keygen' and 'keygen2' arguments at a time, you provided both")
 
         if keygen2:
             # new-style keygen is ready :D
@@ -697,40 +696,43 @@
         MyModel.query.filter(elookup=['user', 'host']).all()
 
     .. note:: I've been using a variation of this internally for some of my
         own work, and I thought I'd release it as a convenience column.
 
     '''
 
-    def __init__(self, column=None, keygen=None, prefix=False, suffix=False, keygen2=None):
+    def __init__(self, column=None, keygen=None, prefix=False, suffix=False, keygen2=None, index=False, unique=False):
         '''
         Two ways to use:
 
             * With ``column`` AND ``keygen`` - automatically index an external column
             a second way using standard keygens
             * With ``keygen2`` - generate an arbitrary index on arbitrary model data
 
         Standard Arguments:
 
             * *column* - column with the data you want to index
             * *keygen* - passed through, see ``Column`` docs for more information
             * *prefix* - passed through, see ``Column`` docs for more information
             * *suffix* - passed through, see ``Column`` docs for more information
             * *keygen2* - passed through, see ``Column`` docs for more information
+            * *unique* - passed through, see ``Column`` docs for more information
+            * *index* - really means: (index or prefix or suffix) or (not unique)
 
         .. note:: `unique` is not available or passed through, as it relies on
             data in the column (IndexOnly columns only store data in index(es)).
         '''
         if column and keygen:
             keygen2 = lambda _,dct: keygen(dct.get(column))
         elif keygen2:
             pass
         else:
             raise ValueError("Need both of `column` and `keygen` or just `keygen2` argument")
-        Column.__init__(self, index=True, keygen2=keygen2, prefix=prefix, suffix=suffix)
+        index = (index or prefix or suffix) or (not unique)
+        Column.__init__(self, index=index, keygen2=keygen2, prefix=prefix, suffix=suffix, unique=unique)
 
     def _validate(self, value):
         if value is not None:
             raise InvalidColumnValue("%s.%s has type %r but column cannot hold data"%(
                 self._model, self._attr, type(value)))
 
     def _from_redis(self, value):
@@ -978,97 +980,10 @@
     def get_related_model(self):
         try:
             model = MODELS[self._ftable]
         except KeyError:
             model = None
         return model
 
-class UnsafeColumn(object):
-    '''
-    UnsafeColumns are attributes on models that allow for explicit model-related
-    data to be stored in native Redis lists, sets, hashes, and sorted sets. Data
-    stored in these columns are not synchronized with the underlying
-    race-condition-prevention locking mechanism used during ``Model.save()``
-    and ``Model.delete()``, though this data is deleted during ``Model.delete()``.
-
-    If it so happens that::
-
-        >>> rom.util.use_null_session()
-        >>> class MyModel(rom.Model):
-        ...    tlist = rom.UnsafeList()
-        ...
-        >>> a = MyModel()
-        >>> a.save()
-        1
-        >>> b = Model.get(a.id)
-        >>> assert a != b
-        >>> a.delete()
-        # data was deleted, list is gone
-        >>> b.tlist.append('test')
-        # list is restored, has 'test', no underlying other data.
-
-    Use of rom.util.
-
-    '''
-    __slots__ = '_attr', '_type'
-    def __init__(self, type):
-        '''
-        By default, UnsafeColumn data is stored:
-        ``'%s:%s:%s' % (ent._namespace, ent._pkey, column_name)``
-
-        Which is separate from where most normal column data is stored, and can
-        be accessed directly if wanted. Hence why it is "unsafe".
-
-        '''
-        self._attr = None
-        self._type = type
-
-    def _init_(self, attr):
-        self._attr = attr
-
-    def __get__(self, obj, objtype):
-        if not obj or not self._attr:
-            raise AttributeError
-
-        if self._attr not in obj._cached_unsafe:
-            obj._cached_unsafe[self._attr] = self._type(self._key(obj), obj)
-
-        return obj._cached_unsafe[self._attr]
-
-    def __set__(self, obj, value):
-        if not obj or not self._attr:
-            raise AttributeError
-
-        if self._attr not in obj._cached_unsafe:
-            obj._cached_unsafe[self._attr] = self._type(self._key(obj))
-        obj._cached_unsafe[self._attr]._set(value)
-
-    def __delete__(self, obj):
-        if not obj or not self._attr:
-            raise AttributeError
-
-        obj._cached_unsafe.pop(self._attr, None)
-        return obj._connection.delete(self._key(obj))
-
-    def _key(self, obj):
-        return '%s:%s' % (obj._pkey, self._attr)
-
-class UnsafeList(UnsafeColumn):
-    def __init__(self, encode=None, decode=None):
-        UnsafeColumn.__init__(self, ListWrapper, encode, decode)
-
-class UnsafeSet(UnsafeColumn):
-    def __init__(self, encode=None, decode=None):
-        UnsafeColumn.__init__(self, SetWrapper, encode, decode)
-
-class UnsafeHash(UnsafeColumn):
-    def __init__(self, encode=None, decode=None):
-        UnsafeColumn.__init__(self, HashWrapper, encode, decode)
-
-class UnsafeZset(UnsafeColumn):
-    def __init__(self, encode=None, decode=None):
-        UnsafeColumn.__init__(self, ZsetWrapper, encode, decode)
-
-
 COLUMN_TYPES = [v for v in globals().values() if isinstance(v, type) and issubclass(v, Column)]
 __all__ = [v.__name__ for v in COLUMN_TYPES] + 'MODELS MODELS_REFERENCED ON_DELETE'.split()
 __all__.sort()
```

### Comparing `rom-1.0.5/rom/index.py` & `rom-1.0.6/rom/index.py`

 * *Files identical despite different names*

### Comparing `rom-1.0.5/test/test_rom.py` & `rom-1.0.6/test/test_rom.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 connect = util._connect
 
 from rom import *
 from rom.exceptions import *
 
 string = String if six.PY2 else Text
 
+def plain2(a, d):
+    a = 'attr'
+    ret = [d[a].lower()] if d.get(a) else None
+    return ret
 
 def global_setup(a=1):
     c = connect(None)
     for p in ('RomTest*', 'RestrictA*', 'RestrictB*'):
         keys = c.keys(p)
         if keys:
             c.delete(*keys)
@@ -237,23 +241,25 @@
         self.assertFalse(x.save())
         session.commit()
 
         self.assertTrue(x is RomTestNormal.get(x.id))
 
     def test_index(self):
         plain = lambda x: [x.lower()] if x else None
-        plain2 = lambda a,d: [d['attr'].lower()] if d.get('attr') else None
         class RomTestIndexedModel(Model):
             attr = Text(index=True, keygen=FULL_TEXT)
             attr2 = Text(index=True, keygen=FULL_TEXT)
             attr3 = Integer(index=True)
             attr4 = Float(index=True)
             attr5 = Decimal(index=True)
             attr6 = IndexOnly('attr', keygen=plain, suffix=True)
             attr7 = IndexOnly(keygen2=plain2, suffix=True)
+            attr8 = IndexOnly(keygen2=plain2, unique=True)
+            def __repr__(self):
+                return "<RTIM " + str(self.id) + " attr=" + str(self.attr) + ">"
 
         x = RomTestIndexedModel(
             attr='hello world',
             attr2='how are you doing?',
             attr3=7,
             attr4=4.5,
             attr5=_Decimal('2.643'),
@@ -262,26 +268,36 @@
         RomTestIndexedModel(
             attr='world',
             attr3=100,
             attr4=-1000,
             attr5=_Decimal('2.643'),
         ).save()
 
+        session.rollback()
+
+        self.assertRaises(UniqueKeyViolation, RomTestIndexedModel(
+                attr='world',
+                attr3=100,
+                attr4=-1000,
+                attr5=_Decimal('2.643'),
+            ).save)
+        session.rollback()
+
         self.assertEqual(RomTestIndexedModel.query.filter(attr='hello').count(), 1)
         self.assertEqual(RomTestIndexedModel.query.filter(attr2='how').filter(attr2='are').count(), 1)
         self.assertEqual(RomTestIndexedModel.query.filter(attr='hello').filter(attr2='how').filter(attr2='are').count(), 1)
         self.assertRaises(QueryError, lambda: RomTestIndexedModel.query.filter(attr='hello', noattr='bad'))
         self.assertEqual(RomTestIndexedModel.query.filter(attr='hello', attr3=(None, None)).count(), 1)
         self.assertEqual(RomTestIndexedModel.query.filter(attr='hello', attr3=(None, 10)).count(), 1)
         self.assertEqual(RomTestIndexedModel.query.filter(attr='hello', attr3=(None, 10)).execute()[0].id, 1)
         self.assertEqual(RomTestIndexedModel.query.filter(attr='hello', attr3=(5, None)).count(), 1)
         self.assertEqual(RomTestIndexedModel.query.filter(attr='hello', attr3=(5, 10), attr4=(4,5), attr5=(2.5, 2.7)).count(), 1)
         first = RomTestIndexedModel.query.filter(attr='hello', attr3=(5, 10), attr4=(4,5), attr5=(2.5, 2.7)).first()
         self.assertTrue(first)
-        self.assertTrue(first is x)
+        self.assertEqual(first._pk, x._pk)
         self.assertEqual(RomTestIndexedModel.query.filter(attr='hello', attr3=(10, 20), attr4=(4,5), attr5=(2.5, 2.7)).count(), 0)
         self.assertEqual(RomTestIndexedModel.query.filter(attr3=100).count(), 1)
         self.assertEqual(RomTestIndexedModel.query.filter(attr='world', attr5=_Decimal('2.643')).count(), 2)
 
         results = RomTestIndexedModel.query.filter(attr='world').order_by('attr4').execute()
         self.assertEqual([y.id for y in results], [2,1])
 
@@ -294,35 +310,39 @@
         self.assertEqual(len(RomTestIndexedModel.get_by(attr3=(10, 25), _limit=(0,5))), 5)
 
         key = RomTestIndexedModel.query.filter(attr='hello').filter(attr2='how').filter(attr2='are').cached_result(30)
         conn = connect(None)
         self.assertTrue(conn.ttl(key) <= 30)
         self.assertEqual(conn.zcard(key), 1)
         conn.delete(key)
-        self.assertRaises(QueryError, lambda: RomTestIndexedModel.query.order_by('attr8'))
+        self.assertRaises(QueryError, lambda: RomTestIndexedModel.query.order_by('attr9'))
 
         # Only the first call raises the warning, so only bother to call it
         # for our first pass through tests (non-Lua case).
         with warnings.catch_warnings(record=True) as w:
             RomTestIndexedModel.query.order_by('attr')
             self.assertEqual(len(w), 1)
 
         for aname in ('attr6', 'attr7'):
             self.assertEqual(RomTestIndexedModel.query.endswith(**{aname:'world'}).count(), 2)
             self.assertEqual(RomTestIndexedModel.query.endswith(**{aname:' world'}).count(), 1)
             self.assertRaises(InvalidColumnValue, lambda: RomTestIndexedModel(**{aname:'hello'}))
             a = RomTestIndexedModel(**{aname:None})
+            a.save()
 
             self.assertRaises(InvalidColumnValue, lambda: a.update(**{aname:'blah'}))
-            a.update(attr='another world').save()
+            name = 'another world'
+            a.update(attr=name).save()
             self.assertEqual(RomTestIndexedModel.query.endswith(**{aname:' world'}).count(), 2)
             if sys.version_info >= (3,6):
-                a.update('different world').save()
-                self.assertEqual(RomTestIndexedModel.query.endswith(**{aname:'different world'}).count(), 1)
-                a.update('overwritten', attr='kept').save()
+                name = 'different world'
+                a.update(attr=name).save()
+                self.assertEqual(RomTestIndexedModel.query.endswith(**{aname:name}).count(), 1)
+                name = 'different kept'
+                a.update(attr=name).save()
                 self.assertEqual(RomTestIndexedModel.query.endswith(**{aname:'kept'}).count(), 1)
             a.delete()
             session.rollback()
 
     def test_alternate_models(self):
         ctr = [0]
         class RomTestAlternate(object):
```

### Comparing `rom-1.0.5/README.rst` & `rom-1.0.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 delete that data, you have to run a cleanup function that literally has to
 scan over every entity in order to determine if the model had been expired. That
 is a huge waste and is the antithesis of good design.
 
 Instead, if you create a new ``expire_at`` float column with ``index=True``,
 the column can store when the entity is to expire. Then to expire the data, you
 can use: ``Model.query.filter(expire_at=(0, time.time())).limit(10)`` to (for
-example) get up to the 10 oldest entites that need to be expired.
+example) get up to the 10 oldest entities that need to be expired.
 
 Now, I know what you are thinking. You are thinking, "but I wish the data would
 just go away on its own." And I don't disagree. But for that to happen, Redis
 needs to grow Lua-script triggers, or you need to run a separate daemon to
 periodically clean up left-over data. But ... if you need to run a separate
 daemon to clean up left-over data by scanning all of your rom entities,
 wouldn't it just be better/faster in every way to keep an explicit column and do
```

### Comparing `rom-1.0.5/setup.py` & `rom-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `rom-1.0.5/PKG-INFO` & `rom-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rom
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Redis object mapper for Python
 Home-page: https://github.com/josiahcarlson/rom
 Author: Josiah Carlson
 Author-email: josiah.carlson@gmail.com
 License: GNU LGPL v2.1
 Description: 
         Rom - the Redis object mapper for Python
@@ -162,15 +162,15 @@
         delete that data, you have to run a cleanup function that literally has to
         scan over every entity in order to determine if the model had been expired. That
         is a huge waste and is the antithesis of good design.
         
         Instead, if you create a new ``expire_at`` float column with ``index=True``,
         the column can store when the entity is to expire. Then to expire the data, you
         can use: ``Model.query.filter(expire_at=(0, time.time())).limit(10)`` to (for
-        example) get up to the 10 oldest entites that need to be expired.
+        example) get up to the 10 oldest entities that need to be expired.
         
         Now, I know what you are thinking. You are thinking, "but I wish the data would
         just go away on its own." And I don't disagree. But for that to happen, Redis
         needs to grow Lua-script triggers, or you need to run a separate daemon to
         periodically clean up left-over data. But ... if you need to run a separate
         daemon to clean up left-over data by scanning all of your rom entities,
         wouldn't it just be better/faster in every way to keep an explicit column and do
```

