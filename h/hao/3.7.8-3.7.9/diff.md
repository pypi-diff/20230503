# Comparing `tmp/hao-3.7.8.tar.gz` & `tmp/hao-3.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hao-3.7.8.tar", max compression
+gzip compressed data, was "hao-3.7.9.tar", last modified: Wed Mar  1 10:24:43 2023, max compression
```

## Comparing `hao-3.7.8.tar` & `hao-3.7.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2020-08-14 05:40:38.118171 hao-3.7.8/LICENSE
--rw-r--r--   0        0        0     3739 2022-06-08 02:36:52.331347 hao-3.7.8/README.md
--rw-r--r--   0        0        0      920 2021-10-13 03:48:38.248130 hao-3.7.8/hao/__init__.py
--rw-r--r--   0        0        0     5118 2021-10-13 03:48:38.248130 hao-3.7.8/hao/arango.py
--rw-r--r--   0        0        0     1463 2022-09-14 10:30:07.881082 hao-3.7.8/hao/args.py
--rw-r--r--   0        0        0      456 2021-10-13 03:48:38.248130 hao-3.7.8/hao/asyncs.py
--rw-r--r--   0        0        0     3892 2022-07-07 15:53:33.912905 hao-3.7.8/hao/charsets.py
--rw-r--r--   0        0        0     1887 2022-07-08 07:58:21.251415 hao-3.7.8/hao/cli.py
--rw-r--r--   0        0        0     5505 2023-02-07 02:06:38.150275 hao-3.7.8/hao/config.py
--rw-r--r--   0        0        0     1465 2021-10-13 03:48:38.248130 hao-3.7.8/hao/currencies.py
--rw-r--r--   0        0        0     2189 2023-02-07 02:06:38.150275 hao-3.7.8/hao/db.py
--rw-r--r--   0        0        0     5691 2022-07-04 01:50:59.025545 hao-3.7.8/hao/decorators.py
--rw-r--r--   0        0        0     1499 2021-10-13 03:48:38.248130 hao-3.7.8/hao/dicts.py
--rw-r--r--   0        0        0    55769 2021-10-13 03:48:38.248130 hao-3.7.8/hao/english.py
--rw-r--r--   0        0        0     1411 2022-07-08 07:51:05.593745 hao-3.7.8/hao/envs.py
--rw-r--r--   0        0        0     7739 2023-01-28 10:30:59.346709 hao-3.7.8/hao/es.py
--rw-r--r--   0        0        0      190 2021-10-13 03:48:38.248130 hao-3.7.8/hao/exceptions.py
--rw-r--r--   0        0        0      517 2022-07-07 15:53:33.912905 hao-3.7.8/hao/exits.py
--rw-r--r--   0        0        0     1525 2022-06-03 16:02:48.521000 hao-3.7.8/hao/files.py
--rw-r--r--   0        0        0      253 2021-10-13 03:48:38.248130 hao-3.7.8/hao/invoker.py
--rw-r--r--   0        0        0     1785 2023-02-07 02:09:30.799331 hao-3.7.8/hao/jsons.py
--rw-r--r--   0        0        0     4600 2022-08-12 09:10:58.495157 hao-3.7.8/hao/kafka.py
--rw-r--r--   0        0        0     3568 2022-08-22 11:41:17.680133 hao-3.7.8/hao/lists.py
--rw-r--r--   0        0        0     5324 2022-07-04 01:50:59.025545 hao-3.7.8/hao/logs.py
--rw-r--r--   0        0        0     3860 2022-07-04 01:50:59.025545 hao-3.7.8/hao/meters.py
--rw-r--r--   0        0        0     8000 2022-08-12 09:10:58.495157 hao-3.7.8/hao/mongo.py
--rw-r--r--   0        0        0     3614 2023-01-28 10:30:59.346709 hao-3.7.8/hao/mysql.py
--rw-r--r--   0        0        0    10355 2022-09-16 06:22:19.443291 hao-3.7.8/hao/namespaces.py
--rw-r--r--   0        0        0     9785 2021-10-13 03:48:38.248130 hao-3.7.8/hao/nations.py
--rw-r--r--   0        0        0      295 2021-10-13 03:48:38.248130 hao-3.7.8/hao/networks.py
--rw-r--r--   0        0        0    14771 2023-01-28 10:30:59.346709 hao-3.7.8/hao/oss.py
--rw-r--r--   0        0        0     3693 2022-06-08 02:36:52.331347 hao-3.7.8/hao/paths.py
--rw-r--r--   0        0        0     2974 2022-06-08 02:36:52.331347 hao-3.7.8/hao/pg.py
--rw-r--r--   0        0        0   207169 2022-07-04 01:50:59.025545 hao-3.7.8/hao/places.py
--rw-r--r--   0        0        0     8687 2022-06-03 16:02:48.521000 hao-3.7.8/hao/rabbit.py
--rw-r--r--   0        0        0     2273 2021-10-13 03:48:38.252130 hao-3.7.8/hao/redis.py
--rw-r--r--   0        0        0     1124 2021-10-13 03:48:38.252130 hao-3.7.8/hao/regexes.py
--rw-r--r--   0        0        0     1152 2022-06-03 16:02:48.521000 hao-3.7.8/hao/singleton.py
--rw-r--r--   0        0        0     1837 2021-10-13 03:48:38.252130 hao-3.7.8/hao/slacks.py
--rw-r--r--   0        0        0     3712 2022-06-03 16:02:48.521000 hao-3.7.8/hao/stopwatch.py
--rw-r--r--   0        0        0    10182 2022-06-03 16:02:48.521000 hao-3.7.8/hao/strings.py
--rw-r--r--   0        0        0     1344 2023-01-28 10:30:59.346709 hao-3.7.8/hao/uuid.py
--rw-r--r--   0        0        0     1234 2022-06-03 16:02:48.521000 hao-3.7.8/hao/versions.py
--rw-r--r--   0        0        0     1524 2023-02-07 02:09:55.090371 hao-3.7.8/pyproject.toml
--rw-r--r--   0        0        0     4906 1970-01-01 00:00:00.000000 hao-3.7.8/setup.py
--rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 hao-3.7.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2020-08-07 06:50:14.000000 hao-3.7.9/LICENSE
+-rw-r--r--   0        0        0     3739 2022-06-07 01:48:03.916694 hao-3.7.9/README.md
+-rw-r--r--   0        0        0      943 2023-03-01 10:16:22.779940 hao-3.7.9/hao/__init__.py
+-rw-r--r--   0        0        0     5118 2020-12-12 06:15:30.000000 hao-3.7.9/hao/arango.py
+-rw-r--r--   0        0        0     1463 2022-12-15 02:37:38.682168 hao-3.7.9/hao/args.py
+-rw-r--r--   0        0        0      456 2021-10-11 06:01:32.961093 hao-3.7.9/hao/asyncs.py
+-rw-r--r--   0        0        0     3892 2022-07-07 15:53:51.747023 hao-3.7.9/hao/charsets.py
+-rw-r--r--   0        0        0     1887 2022-07-15 02:16:16.437933 hao-3.7.9/hao/cli.py
+-rw-r--r--   0        0        0     5505 2023-02-01 06:37:02.811014 hao-3.7.9/hao/config.py
+-rw-r--r--   0        0        0     1465 2021-03-15 02:51:40.000000 hao-3.7.9/hao/currencies.py
+-rw-r--r--   0        0        0     2189 2023-02-01 06:37:02.811193 hao-3.7.9/hao/db.py
+-rw-r--r--   0        0        0     5691 2022-06-22 07:06:27.934823 hao-3.7.9/hao/decorators.py
+-rw-r--r--   0        0        0     1499 2021-10-11 06:01:32.961661 hao-3.7.9/hao/dicts.py
+-rw-r--r--   0        0        0    55769 2021-07-02 17:32:59.523032 hao-3.7.9/hao/english.py
+-rw-r--r--   0        0        0      644 2023-03-01 06:26:39.760312 hao-3.7.9/hao/enums.py
+-rw-r--r--   0        0        0     1411 2022-07-04 04:39:24.666262 hao-3.7.9/hao/envs.py
+-rw-r--r--   0        0        0     7739 2022-12-23 07:07:30.698730 hao-3.7.9/hao/es.py
+-rw-r--r--   0        0        0      190 2020-12-12 06:15:30.000000 hao-3.7.9/hao/exceptions.py
+-rw-r--r--   0        0        0      556 2023-03-01 06:54:26.634968 hao-3.7.9/hao/exits.py
+-rw-r--r--   0        0        0     1525 2022-06-03 09:52:47.573948 hao-3.7.9/hao/files.py
+-rw-r--r--   0        0        0      253 2021-07-02 17:15:37.443456 hao-3.7.9/hao/invoker.py
+-rw-r--r--   0        0        0     1785 2023-02-20 04:50:54.293993 hao-3.7.9/hao/jsons.py
+-rw-r--r--   0        0        0     4600 2022-08-09 08:15:16.720213 hao-3.7.9/hao/kafka.py
+-rw-r--r--   0        0        0     3568 2022-08-22 11:27:40.439294 hao-3.7.9/hao/lists.py
+-rw-r--r--   0        0        0     5324 2022-07-04 04:39:24.667038 hao-3.7.9/hao/logs.py
+-rw-r--r--   0        0        0     3860 2022-06-22 06:07:43.102730 hao-3.7.9/hao/meters.py
+-rw-r--r--   0        0        0     8000 2022-07-18 09:50:08.774357 hao-3.7.9/hao/mongo.py
+-rw-r--r--   0        0        0     3614 2023-01-05 12:02:16.356472 hao-3.7.9/hao/mysql.py
+-rw-r--r--   0        0        0    10355 2022-12-15 02:37:38.683517 hao-3.7.9/hao/namespaces.py
+-rw-r--r--   0        0        0     9785 2020-12-12 06:15:30.000000 hao-3.7.9/hao/nations.py
+-rw-r--r--   0        0        0      295 2020-12-12 06:15:30.000000 hao-3.7.9/hao/networks.py
+-rw-r--r--   0        0        0    14771 2022-12-22 10:48:41.123629 hao-3.7.9/hao/oss.py
+-rw-r--r--   0        0        0     3693 2022-06-07 01:48:03.918436 hao-3.7.9/hao/paths.py
+-rw-r--r--   0        0        0     2974 2023-01-05 12:27:54.444115 hao-3.7.9/hao/pg.py
+-rw-r--r--   0        0        0   207169 2022-06-30 02:54:01.703468 hao-3.7.9/hao/places.py
+-rw-r--r--   0        0        0     8687 2022-03-04 09:24:53.157502 hao-3.7.9/hao/rabbit.py
+-rw-r--r--   0        0        0     2273 2021-07-02 17:23:00.529442 hao-3.7.9/hao/redis.py
+-rw-r--r--   0        0        0     1124 2020-12-12 06:15:30.000000 hao-3.7.9/hao/regexes.py
+-rw-r--r--   0        0        0     1152 2021-11-10 08:18:59.869145 hao-3.7.9/hao/singleton.py
+-rw-r--r--   0        0        0     1837 2021-10-11 06:01:32.963435 hao-3.7.9/hao/slacks.py
+-rw-r--r--   0        0        0     3712 2021-12-27 04:46:12.550138 hao-3.7.9/hao/stopwatch.py
+-rw-r--r--   0        0        0    10182 2022-06-03 09:52:47.575527 hao-3.7.9/hao/strings.py
+-rw-r--r--   0        0        0     1344 2023-01-05 07:21:17.373248 hao-3.7.9/hao/uuid.py
+-rw-r--r--   0        0        0     1234 2022-06-03 09:52:47.575748 hao-3.7.9/hao/versions.py
+-rw-r--r--   0        0        0     1233 2023-03-01 06:44:52.360083 hao-3.7.9/pyproject.toml
+-rw-r--r--   0        0        0     4860 1970-01-01 00:00:00.000000 hao-3.7.9/PKG-INFO
```

### Comparing `hao-3.7.8/LICENSE` & `hao-3.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/README.md` & `hao-3.7.9/README.md`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/__init__.py` & `hao-3.7.9/hao/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import importlib
 import pkgutil
 
 from . import (
-    logs,
+    asyncs,
     charsets,
     config,
     currencies,
+    decorators,
+    dicts,
+    english,
     envs,
+    exceptions,
+    files,
+    invoker,
     jsons,
     lists,
-    dicts,
+    logs,
+    namespaces,
     nations,
     paths,
     regexes,
-    decorators,
     singleton,
+    slacks,
     stopwatch,
     strings,
     versions,
-    exceptions,
-    files,
-    invoker,
-    slacks,
-    namespaces,
-    asyncs,
-    english,
 )
 
+__version__ = '3.7.9'
+
 
 def import_submodules(package, recursive=False):
     if isinstance(package, str):
         package = importlib.import_module(package)
     results = {}
     caller = paths.who_called_me()
     for loader, name, is_pkg in pkgutil.walk_packages(package.__path__):
```

### Comparing `hao-3.7.8/hao/arango.py` & `hao-3.7.9/hao/arango.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/args.py` & `hao-3.7.9/hao/args.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/charsets.py` & `hao-3.7.9/hao/charsets.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/cli.py` & `hao-3.7.9/hao/cli.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/config.py` & `hao-3.7.9/hao/config.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/currencies.py` & `hao-3.7.9/hao/currencies.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/db.py` & `hao-3.7.9/hao/db.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/decorators.py` & `hao-3.7.9/hao/decorators.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/dicts.py` & `hao-3.7.9/hao/dicts.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/english.py` & `hao-3.7.9/hao/english.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/envs.py` & `hao-3.7.9/hao/envs.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/es.py` & `hao-3.7.9/hao/es.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/exits.py` & `hao-3.7.9/hao/exits.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 def _on_exit(*a, **kw):
     while _handlers:
         handler, args, kwargs = _handlers.pop()
         handler(*args, **kwargs)
 
 
 signal.signal(signal.SIGTERM, _on_exit)
+signal.signal(signal.SIGINT, _on_exit)
 
 
 def on_exit(func, *a, **kw):
     _handlers.append((func, a, kw))
     return func
```

### Comparing `hao-3.7.8/hao/files.py` & `hao-3.7.9/hao/files.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/jsons.py` & `hao-3.7.9/hao/jsons.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/kafka.py` & `hao-3.7.9/hao/kafka.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/lists.py` & `hao-3.7.9/hao/lists.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/logs.py` & `hao-3.7.9/hao/logs.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/meters.py` & `hao-3.7.9/hao/meters.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/mongo.py` & `hao-3.7.9/hao/mongo.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/mysql.py` & `hao-3.7.9/hao/mysql.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/namespaces.py` & `hao-3.7.9/hao/namespaces.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/nations.py` & `hao-3.7.9/hao/nations.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/oss.py` & `hao-3.7.9/hao/oss.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/paths.py` & `hao-3.7.9/hao/paths.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/pg.py` & `hao-3.7.9/hao/pg.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/places.py` & `hao-3.7.9/hao/places.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/rabbit.py` & `hao-3.7.9/hao/rabbit.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/redis.py` & `hao-3.7.9/hao/redis.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/regexes.py` & `hao-3.7.9/hao/regexes.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/singleton.py` & `hao-3.7.9/hao/singleton.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/slacks.py` & `hao-3.7.9/hao/slacks.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/stopwatch.py` & `hao-3.7.9/hao/stopwatch.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/strings.py` & `hao-3.7.9/hao/strings.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/uuid.py` & `hao-3.7.9/hao/uuid.py`

 * *Files identical despite different names*

### Comparing `hao-3.7.8/hao/versions.py` & `hao-3.7.9/hao/versions.py`

 * *Files identical despite different names*

