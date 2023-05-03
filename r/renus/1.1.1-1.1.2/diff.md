# Comparing `tmp/renus-1.1.1.tar.gz` & `tmp/renus-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renus-1.1.1.tar", last modified: Sun Apr 30 01:03:54 2023, max compression
+gzip compressed data, was "renus-1.1.2.tar", last modified: Wed May  3 09:44:01 2023, max compression
```

## Comparing `renus-1.1.1.tar` & `renus-1.1.2.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.803207 renus-1.1.1/
--rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      220 2023-04-30 01:03:54.802196 renus-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 01:03:53.806980 renus-1.1.1/renus/
--rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.1/renus/__init__.py
--rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.1/renus/app.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:03:53.909525 renus-1.1.1/renus/commands/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:03:53.987582 renus-1.1.1/renus/commands/app/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/app/__init__.py
--rw-rw-rw-   0        0        0     1787 2023-04-18 05:34:21.000000 renus-1.1.1/renus/commands/app/controller.temp
--rw-rw-rw-   0        0        0     1033 2023-04-20 17:58:46.000000 renus-1.1.1/renus/commands/app/model.temp
--rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.1/renus/commands/app/route.temp
--rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.1.1/renus/commands/app/run.py
--rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.1/renus/commands/app/vue.temp
-drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.016918 renus-1.1.1/renus/commands/backup/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/backup/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.1/renus/commands/backup/run.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.035919 renus-1.1.1/renus/commands/copy/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/copy/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.1/renus/commands/copy/run.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.074492 renus-1.1.1/renus/commands/default/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/default/__init__.py
--rw-rw-rw-   0        0        0     2153 2023-04-20 05:35:39.000000 renus-1.1.1/renus/commands/default/run.py
--rw-rw-rw-   0        0        0     1416 2023-04-15 07:24:18.000000 renus-1.1.1/renus/commands/help.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.171744 renus-1.1.1/renus/commands/install/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/install/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.1.1/renus/commands/install/build.py
--rw-rw-rw-   0        0        0     3946 2023-03-12 07:22:04.000000 renus-1.1.1/renus/commands/install/run.py
--rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.1/renus/commands/install/service.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.197297 renus-1.1.1/renus/commands/permission/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/permission/__init__.py
--rw-rw-rw-   0        0        0      704 2023-04-20 05:35:39.000000 renus-1.1.1/renus/commands/permission/run.py
--rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.1/renus/commands/run.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.716928 renus-1.1.1/renus/core/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/__init__.py
--rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.1/renus/core/cache.py
--rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/concurrency.py
--rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/config.py
--rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.1/renus/core/crypt.py
--rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/datastructures.py
--rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.1/renus/core/exception.py
--rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.1/renus/core/formparsers.py
--rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.1/renus/core/injection.py
--rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/log.py
--rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/middleware.py
--rw-rw-rw-   0        0        0    14800 2023-04-20 18:01:14.000000 renus-1.1.1/renus/core/model.py
--rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.1/renus/core/request.py
--rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.1/renus/core/response.py
--rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.1/renus/core/routing.py
--rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.1/renus/core/schedule.py
--rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.1.1/renus/core/serialize.py
--rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/status.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.779210 renus-1.1.1/renus/core/validation/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/validation/__init__.py
--rw-rw-rw-   0        0        0     8773 2022-10-23 08:35:28.000000 renus-1.1.1/renus/core/validation/rules.py
--rw-rw-rw-   0        0        0     3235 2022-08-31 08:30:44.000000 renus-1.1.1/renus/core/validation/validate.py
--rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.1/renus/core/websockets.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:03:54.799195 renus-1.1.1/renus/util/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.1/renus/util/__init__.py
--rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.1/renus/util/helper.py
-drwxrwxrwx   0        0        0        0 2023-04-30 01:03:53.838979 renus-1.1.1/renus.egg-info/
--rw-rw-rw-   0        0        0      220 2023-04-30 01:03:53.000000 renus-1.1.1/renus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1405 2023-04-30 01:03:53.000000 renus-1.1.1/renus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 01:03:53.000000 renus-1.1.1/renus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-30 01:03:53.000000 renus-1.1.1/renus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 01:03:54.804209 renus-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      334 2023-04-30 01:02:27.000000 renus-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.442286 renus-1.1.2/
+-rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      220 2023-05-03 09:44:01.442286 renus-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:00.871275 renus-1.1.2/renus/
+-rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.2/renus/__init__.py
+-rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.2/renus/app.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:00.936277 renus-1.1.2/renus/commands/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:00.983274 renus-1.1.2/renus/commands/app/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/app/__init__.py
+-rw-rw-rw-   0        0        0     1786 2023-05-03 04:46:26.000000 renus-1.1.2/renus/commands/app/controller.temp
+-rw-rw-rw-   0        0        0     1008 2023-05-03 09:35:45.000000 renus-1.1.2/renus/commands/app/model.temp
+-rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.2/renus/commands/app/route.temp
+-rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.1.2/renus/commands/app/run.py
+-rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.2/renus/commands/app/vue.temp
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.008397 renus-1.1.2/renus/commands/backup/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/backup/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.2/renus/commands/backup/run.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.017381 renus-1.1.2/renus/commands/copy/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/copy/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.2/renus/commands/copy/run.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.025397 renus-1.1.2/renus/commands/default/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/default/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-04-30 01:41:46.000000 renus-1.1.2/renus/commands/default/run.py
+-rw-rw-rw-   0        0        0     1416 2023-04-15 07:24:18.000000 renus-1.1.2/renus/commands/help.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.082191 renus-1.1.2/renus/commands/install/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/install/__init__.py
+-rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.1.2/renus/commands/install/build.py
+-rw-rw-rw-   0        0        0     3946 2023-03-12 07:22:04.000000 renus-1.1.2/renus/commands/install/run.py
+-rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.2/renus/commands/install/service.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.090174 renus-1.1.2/renus/commands/permission/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/permission/__init__.py
+-rw-rw-rw-   0        0        0      763 2023-04-30 01:38:29.000000 renus-1.1.2/renus/commands/permission/run.py
+-rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.2/renus/commands/run.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.393490 renus-1.1.2/renus/core/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/__init__.py
+-rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.2/renus/core/cache.py
+-rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/concurrency.py
+-rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/config.py
+-rw-rw-rw-   0        0        0     2158 2023-05-03 09:30:03.000000 renus-1.1.2/renus/core/cprint.py
+-rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.2/renus/core/crypt.py
+-rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/datastructures.py
+-rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.2/renus/core/exception.py
+-rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.2/renus/core/formparsers.py
+-rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.2/renus/core/injection.py
+-rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/log.py
+-rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/middleware.py
+-rw-rw-rw-   0        0        0    14800 2023-04-20 18:01:14.000000 renus-1.1.2/renus/core/model.py
+-rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.2/renus/core/request.py
+-rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.2/renus/core/response.py
+-rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.2/renus/core/routing.py
+-rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.2/renus/core/schedule.py
+-rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.1.2/renus/core/serialize.py
+-rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/status.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.431285 renus-1.1.2/renus/core/validation/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/validation/__init__.py
+-rw-rw-rw-   0        0        0     8773 2022-10-23 08:35:28.000000 renus-1.1.2/renus/core/validation/rules.py
+-rw-rw-rw-   0        0        0     3235 2022-08-31 08:30:44.000000 renus-1.1.2/renus/core/validation/validate.py
+-rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.2/renus/core/websockets.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:01.441302 renus-1.1.2/renus/util/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.2/renus/util/__init__.py
+-rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.2/renus/util/helper.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:44:00.890276 renus-1.1.2/renus.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-05-03 09:44:00.000000 renus-1.1.2/renus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1426 2023-05-03 09:44:00.000000 renus-1.1.2/renus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 09:44:00.000000 renus-1.1.2/renus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-03 09:44:00.000000 renus-1.1.2/renus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 09:44:01.443285 renus-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      334 2023-05-03 09:20:03.000000 renus-1.1.2/setup.py
```

### Comparing `renus-1.1.1/LICENSE` & `renus-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/app.py` & `renus-1.1.2/renus/app.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/commands/app/controller.temp` & `renus-1.1.2/renus/commands/app/controller.temp`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         :method: get
         :return: JsonResponse of CRUD table
         """
         m={name_camel}(self.request)
         m.fields = {
             '_id': {"type": "text-input", "formInput": False},
             'updated_at': {"type": "time-ago", "formInput": False},
-            'created_at': {"type": "date-picker", "formInput": False, "sortable": False, }
+            'created_at': {"type": "date-input", "formInput": False, "sortable": False, }
             }
         m.search_fields = []
         return JsonResponse(m.index())
 
     def store(self):
         """
         Add new {name_camel} Item
```

### Comparing `renus-1.1.1/renus/commands/app/model.temp` & `renus-1.1.2/renus/commands/app/model.temp`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import typing
 from datetime import datetime
 from bson import ObjectId
 from renus.core.model import ModelBase
 from app.extension.renus.activity.service import ActivityService
 from app.extension.renus.crud.model import CRUD
 
-class _Base:
-    _id:ObjectId
-    created_at:datetime
-    updated_at:datetime
-
-    def __init__(self,doc) -> None:
-        for k,v in doc.items():
-            self[k]=v
-
-    def __setitem__(self, key, value):
-        self[key] = value
+class _Base(dict):
+    _id: ObjectId
+    created_at: datetime
+    updated_at: datetime
+
+    def __init__(self, doc):
+        super().__init__(doc)
+        for k, v in doc.items():
+            setattr(self, k, v)
 
 
 class {name_camel}(ModelBase,CRUD):
     collection_name="{name_db}"
     document_model=_Base
 
     def __init__(self,request) -> None:
```

### Comparing `renus-1.1.1/renus/commands/app/route.temp` & `renus-1.1.2/renus/commands/app/route.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/commands/app/run.py` & `renus-1.1.2/renus/commands/app/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/commands/backup/run.py` & `renus-1.1.2/renus/commands/backup/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/commands/copy/run.py` & `renus-1.1.2/renus/commands/copy/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/commands/help.py` & `renus-1.1.2/renus/commands/help.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/commands/install/build.py` & `renus-1.1.2/renus/commands/install/build.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/commands/install/run.py` & `renus-1.1.2/renus/commands/install/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/commands/install/service.py` & `renus-1.1.2/renus/commands/install/service.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/cache.py` & `renus-1.1.2/renus/core/cache.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/concurrency.py` & `renus-1.1.2/renus/core/concurrency.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/crypt.py` & `renus-1.1.2/renus/core/crypt.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/datastructures.py` & `renus-1.1.2/renus/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/exception.py` & `renus-1.1.2/renus/core/exception.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/formparsers.py` & `renus-1.1.2/renus/core/formparsers.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/injection.py` & `renus-1.1.2/renus/core/injection.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/log.py` & `renus-1.1.2/renus/core/log.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/model.py` & `renus-1.1.2/renus/core/model.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/request.py` & `renus-1.1.2/renus/core/request.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/response.py` & `renus-1.1.2/renus/core/response.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/routing.py` & `renus-1.1.2/renus/core/routing.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/schedule.py` & `renus-1.1.2/renus/core/schedule.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/serialize.py` & `renus-1.1.2/renus/core/serialize.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/status.py` & `renus-1.1.2/renus/core/status.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/validation/rules.py` & `renus-1.1.2/renus/core/validation/rules.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/validation/validate.py` & `renus-1.1.2/renus/core/validation/validate.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/core/websockets.py` & `renus-1.1.2/renus/core/websockets.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus/util/helper.py` & `renus-1.1.2/renus/util/helper.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.1/renus.egg-info/SOURCES.txt` & `renus-1.1.2/renus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 renus/commands/install/service.py
 renus/commands/permission/__init__.py
 renus/commands/permission/run.py
 renus/core/__init__.py
 renus/core/cache.py
 renus/core/concurrency.py
 renus/core/config.py
+renus/core/cprint.py
 renus/core/crypt.py
 renus/core/datastructures.py
 renus/core/exception.py
 renus/core/formparsers.py
 renus/core/injection.py
 renus/core/log.py
 renus/core/middleware.py
```

