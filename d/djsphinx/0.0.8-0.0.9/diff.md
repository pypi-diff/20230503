# Comparing `tmp/djsphinx-0.0.8.tar.gz` & `tmp/djsphinx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\djsphinx-0.0.8.tar", last modified: Mon May 13 11:21:11 2019, max compression
+gzip compressed data, was "dist\djsphinx-0.0.9.tar", last modified: Thu Jun  3 09:46:31 2021, max compression
```

## Comparing `djsphinx-0.0.8.tar` & `djsphinx-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2019-05-13 11:21:11.000000 djsphinx-0.0.8/
--rw-rw-rw-   0        0        0      498 2019-05-13 11:21:11.000000 djsphinx-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2019-05-13 11:21:11.000000 djsphinx-0.0.8/djsphinx/
--rw-rw-rw-   0        0        0      144 2019-05-13 11:16:56.000000 djsphinx-0.0.8/djsphinx/__init__.py
--rw-rw-rw-   0        0        0    33562 2019-05-13 11:12:38.000000 djsphinx-0.0.8/djsphinx/sphinxapi.py
--rw-rw-rw-   0        0        0    33686 2019-05-13 11:11:04.000000 djsphinx-0.0.8/djsphinx/sphinxapi_py3.py
--rw-rw-rw-   0        0        0      709 2019-05-13 11:14:47.000000 djsphinx-0.0.8/djsphinx/wrapper.py
--rw-rw-rw-   0        0        0      847 2019-05-13 05:36:05.000000 djsphinx-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-03 09:46:31.000000 djsphinx-0.0.9/
+-rw-rw-rw-   0        0        0      498 2021-06-03 09:46:31.000000 djsphinx-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2021-06-03 09:46:31.000000 djsphinx-0.0.9/djsphinx/
+-rw-rw-rw-   0        0        0      144 2021-06-03 09:40:53.000000 djsphinx-0.0.9/djsphinx/__init__.py
+-rw-rw-rw-   0        0        0    33562 2019-05-13 11:12:38.000000 djsphinx-0.0.9/djsphinx/sphinxapi.py
+-rw-rw-rw-   0        0        0    33649 2021-06-03 09:43:10.000000 djsphinx-0.0.9/djsphinx/sphinxapi_py3.py
+-rw-rw-rw-   0        0        0      798 2021-06-03 09:40:37.000000 djsphinx-0.0.9/djsphinx/wrapper.py
+-rw-rw-rw-   0        0        0      847 2019-05-13 05:36:05.000000 djsphinx-0.0.9/setup.py
```

### Comparing `djsphinx-0.0.8/djsphinx/sphinxapi.py` & `djsphinx-0.0.9/djsphinx/sphinxapi.py`

 * *Files identical despite different names*

### Comparing `djsphinx-0.0.8/djsphinx/sphinxapi_py3.py` & `djsphinx-0.0.9/djsphinx/sphinxapi_py3.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,16 +270,16 @@
         return response
 
 
     def SetLimits (self, offset, limit, maxmatches=0, cutoff=0):
         """
         Set offset and count into result set, and optionally set max-matches and cutoff limits.
         """
-        assert ( type(offset) in [int,long] and 0<=offset<16777216 )
-        assert ( type(limit) in [int,long] and 0<limit<16777216 )
+        assert ( type(offset) in [int] and 0<=offset<16777216 )
+        assert ( type(limit) in [int] and 0<limit<16777216 )
         assert(maxmatches>=0)
         self._offset = offset
         self._limit = limit
         if maxmatches>0:
             self._maxmatches = maxmatches
         if cutoff>=0:
             self._cutoff = cutoff
@@ -353,43 +353,43 @@
 
 
     def SetIDRange (self, minid, maxid):
         """
         Set IDs range to match.
         Only match records if document ID is beetwen $min and $max (inclusive).
         """
-        assert(isinstance(minid, (int, long)))
-        assert(isinstance(maxid, (int, long)))
+        assert(isinstance(minid, (int)))
+        assert(isinstance(maxid, (int)))
         assert(minid<=maxid)
         self._min_id = minid
         self._max_id = maxid
 
 
     def SetFilter ( self, attribute, values, exclude=0 ):
         """
         Set values set filter.
         Only match records where 'attribute' value is in given 'values' set.
         """
         assert(isinstance(attribute, str))
         assert iter(values)
 
         for value in values:
-            assert(isinstance(value, (int,long)))
+            assert(isinstance(value, (int)))
 
         self._filters.append ( { 'type':SPH_FILTER_VALUES, 'attr':attribute, 'exclude':exclude, 'values':values } )
 
 
     def SetFilterRange (self, attribute, min_, max_, exclude=0 ):
         """
         Set range filter.
         Only match records if 'attribute' value is beetwen 'min_' and 'max_' (inclusive).
         """
         assert(isinstance(attribute, str))
-        assert(isinstance(min_, (int,long)))
-        assert(isinstance(max_, (int,long)))
+        assert(isinstance(min_, (int)))
+        assert(isinstance(max_, (int)))
         assert(min_<=max_)
 
         self._filters.append ( { 'type':SPH_FILTER_RANGE, 'attr':attribute, 'exclude':exclude, 'min':min_, 'max':max_ } )
 
 
     def SetFilterFloatRange (self, attribute, min_, max_, exclude=0 ):
         assert(isinstance(attribute,str))
```

### Comparing `djsphinx-0.0.8/djsphinx/wrapper.py` & `djsphinx-0.0.9/djsphinx/wrapper.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,19 +7,24 @@
 
 py_ver = sys.version_info
 if py_ver[0] > 2:
     from .sphinxapi_py3 import *
 else:
     from .sphinxapi import *
 
-def sphinx_search(query_str, index=None):
+
+TOTAL_LIMIT = 10000
+
+
+def sphinx_search(query_str, index=None, offset=0, limit=TOTAL_LIMIT):
     host = getattr(settings, 'SPHINX_HOST', '127.0.0.1')
     port = getattr(settings, 'SPHINX_PORT', 9312)
     index = index or getattr(settings, 'SPHINX_DEFAULT_INDEX', 'index_name')
     cl = SphinxClient()
     cl.SetServer(host, port)
     cl.SetMatchMode(SPH_MATCH_ALL)
+    cl.SetLimits(offset, limit)
     res = cl.Query(query_str, index)
     if res and 'matches' in res:
         return list(map(lambda m: m['id'], res['matches']))
     else:
         return []
```

### Comparing `djsphinx-0.0.8/setup.py` & `djsphinx-0.0.9/setup.py`

 * *Files identical despite different names*

