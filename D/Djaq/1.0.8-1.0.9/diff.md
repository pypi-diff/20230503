# Comparing `tmp/Djaq-1.0.8.tar.gz` & `tmp/Djaq-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Djaq-1.0.8.tar", last modified: Fri Sep 23 08:54:15 2022, max compression
+gzip compressed data, was "Djaq-1.0.9.tar", last modified: Wed May  3 10:51:21 2023, max compression
```

## Comparing `Djaq-1.0.8.tar` & `Djaq-1.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2022-09-23 08:54:15.430770 Djaq-1.0.8/
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2022-09-23 08:54:15.403261 Djaq-1.0.8/Djaq.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)     4282 2022-09-23 08:54:15.000000 Djaq-1.0.8/Djaq.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)      954 2022-09-23 08:54:15.000000 Djaq-1.0.8/Djaq.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2022-09-23 08:54:15.000000 Djaq-1.0.8/Djaq.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)        5 2022-09-23 08:54:15.000000 Djaq-1.0.8/Djaq.egg-info/top_level.txt
--rw-r--r--   0 paul       (501) staff       (20)     1071 2020-07-28 20:13:57.000000 Djaq-1.0.8/LICENSE
--rw-r--r--   0 paul       (501) staff       (20)      136 2020-07-28 20:13:57.000000 Djaq-1.0.8/MANIFEST.in
--rw-r--r--   0 paul       (501) staff       (20)     4282 2022-09-23 08:54:15.430359 Djaq-1.0.8/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)     3553 2022-06-10 14:31:38.000000 Djaq-1.0.8/README.rst
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2022-09-23 08:54:15.409392 Djaq-1.0.8/djaq/
--rw-r--r--   0 paul       (501) staff       (20)      168 2022-09-23 08:53:19.000000 Djaq-1.0.8/djaq/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)     6959 2022-08-25 05:29:25.000000 Djaq-1.0.8/djaq/app_utils.py
--rw-r--r--   0 paul       (501) staff       (20)     1888 2022-08-24 18:26:13.000000 Djaq-1.0.8/djaq/conditions.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2022-09-23 08:54:15.416196 Djaq-1.0.8/djaq/djaq_api/
--rw-r--r--   0 paul       (501) staff       (20)        0 2020-07-28 20:13:57.000000 Djaq-1.0.8/djaq/djaq_api/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)       63 2020-07-28 20:13:57.000000 Djaq-1.0.8/djaq/djaq_api/admin.py
--rw-r--r--   0 paul       (501) staff       (20)      108 2022-06-26 05:46:26.000000 Djaq-1.0.8/djaq/djaq_api/apps.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2022-09-23 08:54:15.417300 Djaq-1.0.8/djaq/djaq_api/migrations/
--rw-r--r--   0 paul       (501) staff       (20)        0 2020-07-28 20:13:57.000000 Djaq-1.0.8/djaq/djaq_api/migrations/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)       57 2020-07-28 20:13:57.000000 Djaq-1.0.8/djaq/djaq_api/models.py
--rw-r--r--   0 paul       (501) staff       (20)      245 2022-05-21 10:43:52.000000 Djaq-1.0.8/djaq/djaq_api/tests.py
--rw-r--r--   0 paul       (501) staff       (20)      241 2020-07-28 20:13:57.000000 Djaq-1.0.8/djaq/djaq_api/urls.py
--rw-r--r--   0 paul       (501) staff       (20)     6366 2022-08-25 05:29:25.000000 Djaq-1.0.8/djaq/djaq_api/views.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2022-09-23 08:54:15.421887 Djaq-1.0.8/djaq/djaq_ui/
--rw-r--r--   0 paul       (501) staff       (20)       16 2020-07-28 20:13:57.000000 Djaq-1.0.8/djaq/djaq_ui/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)       63 2020-07-28 20:13:57.000000 Djaq-1.0.8/djaq/djaq_ui/admin.py
--rw-r--r--   0 paul       (501) staff       (20)      115 2022-02-26 10:25:40.000000 Djaq-1.0.8/djaq/djaq_ui/apps.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2022-09-23 08:54:15.422814 Djaq-1.0.8/djaq/djaq_ui/management/
--rw-r--r--   0 paul       (501) staff       (20)        0 2022-05-23 07:58:28.000000 Djaq-1.0.8/djaq/djaq_ui/management/__init__.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2022-09-23 08:54:15.426582 Djaq-1.0.8/djaq/djaq_ui/management/commands/
--rw-r--r--   0 paul       (501) staff       (20)        0 2022-05-23 07:58:28.000000 Djaq-1.0.8/djaq/djaq_ui/management/commands/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)      454 2022-05-23 07:58:28.000000 Djaq-1.0.8/djaq/djaq_ui/management/commands/build_data.py
--rw-r--r--   0 paul       (501) staff       (20)     3463 2022-06-26 05:46:26.000000 Djaq-1.0.8/djaq/djaq_ui/management/commands/djaq.py
--rw-r--r--   0 paul       (501) staff       (20)      581 2022-05-23 07:58:28.000000 Djaq-1.0.8/djaq/djaq_ui/management/commands/run.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2022-09-23 08:54:15.427794 Djaq-1.0.8/djaq/djaq_ui/migrations/
--rw-r--r--   0 paul       (501) staff       (20)        0 2020-07-28 20:13:57.000000 Djaq-1.0.8/djaq/djaq_ui/migrations/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)       57 2020-07-28 20:13:57.000000 Djaq-1.0.8/djaq/djaq_ui/models.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2022-09-23 08:54:15.428891 Djaq-1.0.8/djaq/djaq_ui/templates/
--rw-r--r--   0 paul       (501) staff       (20)      487 2021-04-02 10:29:12.000000 Djaq-1.0.8/djaq/djaq_ui/templates/base_query.html
--rw-r--r--   0 paul       (501) staff       (20)     9555 2022-05-27 07:21:51.000000 Djaq-1.0.8/djaq/djaq_ui/templates/query.html
--rw-r--r--   0 paul       (501) staff       (20)       60 2020-07-28 20:13:57.000000 Djaq-1.0.8/djaq/djaq_ui/tests.py
--rw-r--r--   0 paul       (501) staff       (20)      444 2020-07-28 20:13:57.000000 Djaq-1.0.8/djaq/djaq_ui/urls.py
--rw-r--r--   0 paul       (501) staff       (20)     4232 2022-08-25 05:29:25.000000 Djaq-1.0.8/djaq/djaq_ui/views.py
--rw-r--r--   0 paul       (501) staff       (20)      104 2020-07-28 20:13:57.000000 Djaq-1.0.8/djaq/exceptions.py
--rw-r--r--   0 paul       (501) staff       (20)     6562 2022-09-22 09:19:35.000000 Djaq-1.0.8/djaq/functions.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2022-09-23 08:54:15.429680 Djaq-1.0.8/djaq/query/
--rw-r--r--   0 paul       (501) staff       (20)    50346 2022-09-23 08:46:24.000000 Djaq-1.0.8/djaq/query/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)     2634 2021-04-01 09:11:56.000000 Djaq-1.0.8/djaq/result.py
--rw-r--r--   0 paul       (501) staff       (20)       38 2022-09-23 08:54:15.430896 Djaq-1.0.8/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)     1604 2022-06-06 15:35:54.000000 Djaq-1.0.8/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 10:51:21.857492 Djaq-1.0.9/
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 10:51:21.838736 Djaq-1.0.9/Djaq.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)     4282 2023-05-03 10:51:21.000000 Djaq-1.0.9/Djaq.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      954 2023-05-03 10:51:21.000000 Djaq-1.0.9/Djaq.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-05-03 10:51:21.000000 Djaq-1.0.9/Djaq.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)        5 2023-05-03 10:51:21.000000 Djaq-1.0.9/Djaq.egg-info/top_level.txt
+-rw-r--r--   0 paul       (501) staff       (20)     1071 2020-07-28 20:13:57.000000 Djaq-1.0.9/LICENSE
+-rw-r--r--   0 paul       (501) staff       (20)      136 2020-07-28 20:13:57.000000 Djaq-1.0.9/MANIFEST.in
+-rw-r--r--   0 paul       (501) staff       (20)     4282 2023-05-03 10:51:21.857212 Djaq-1.0.9/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     3553 2022-06-10 14:31:38.000000 Djaq-1.0.9/README.rst
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 10:51:21.842657 Djaq-1.0.9/djaq/
+-rw-r--r--   0 paul       (501) staff       (20)      168 2023-05-03 10:49:17.000000 Djaq-1.0.9/djaq/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)     6959 2022-08-25 05:29:25.000000 Djaq-1.0.9/djaq/app_utils.py
+-rw-r--r--   0 paul       (501) staff       (20)     1888 2022-08-24 18:26:13.000000 Djaq-1.0.9/djaq/conditions.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 10:51:21.846923 Djaq-1.0.9/djaq/djaq_api/
+-rw-r--r--   0 paul       (501) staff       (20)        0 2020-07-28 20:13:57.000000 Djaq-1.0.9/djaq/djaq_api/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)       63 2020-07-28 20:13:57.000000 Djaq-1.0.9/djaq/djaq_api/admin.py
+-rw-r--r--   0 paul       (501) staff       (20)      108 2022-06-26 05:46:26.000000 Djaq-1.0.9/djaq/djaq_api/apps.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 10:51:21.847531 Djaq-1.0.9/djaq/djaq_api/migrations/
+-rw-r--r--   0 paul       (501) staff       (20)        0 2020-07-28 20:13:57.000000 Djaq-1.0.9/djaq/djaq_api/migrations/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)       57 2020-07-28 20:13:57.000000 Djaq-1.0.9/djaq/djaq_api/models.py
+-rw-r--r--   0 paul       (501) staff       (20)      245 2022-05-21 10:43:52.000000 Djaq-1.0.9/djaq/djaq_api/tests.py
+-rw-r--r--   0 paul       (501) staff       (20)      241 2020-07-28 20:13:57.000000 Djaq-1.0.9/djaq/djaq_api/urls.py
+-rw-r--r--   0 paul       (501) staff       (20)     6366 2022-08-25 05:29:25.000000 Djaq-1.0.9/djaq/djaq_api/views.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 10:51:21.851279 Djaq-1.0.9/djaq/djaq_ui/
+-rw-r--r--   0 paul       (501) staff       (20)       16 2020-07-28 20:13:57.000000 Djaq-1.0.9/djaq/djaq_ui/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)       63 2020-07-28 20:13:57.000000 Djaq-1.0.9/djaq/djaq_ui/admin.py
+-rw-r--r--   0 paul       (501) staff       (20)      115 2022-02-26 10:25:40.000000 Djaq-1.0.9/djaq/djaq_ui/apps.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 10:51:21.851952 Djaq-1.0.9/djaq/djaq_ui/management/
+-rw-r--r--   0 paul       (501) staff       (20)        0 2022-05-23 07:58:28.000000 Djaq-1.0.9/djaq/djaq_ui/management/__init__.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 10:51:21.853710 Djaq-1.0.9/djaq/djaq_ui/management/commands/
+-rw-r--r--   0 paul       (501) staff       (20)        0 2022-05-23 07:58:28.000000 Djaq-1.0.9/djaq/djaq_ui/management/commands/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)      454 2022-05-23 07:58:28.000000 Djaq-1.0.9/djaq/djaq_ui/management/commands/build_data.py
+-rw-r--r--   0 paul       (501) staff       (20)     3463 2022-06-26 05:46:26.000000 Djaq-1.0.9/djaq/djaq_ui/management/commands/djaq.py
+-rw-r--r--   0 paul       (501) staff       (20)      581 2022-05-23 07:58:28.000000 Djaq-1.0.9/djaq/djaq_ui/management/commands/run.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 10:51:21.854311 Djaq-1.0.9/djaq/djaq_ui/migrations/
+-rw-r--r--   0 paul       (501) staff       (20)        0 2020-07-28 20:13:57.000000 Djaq-1.0.9/djaq/djaq_ui/migrations/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)       57 2020-07-28 20:13:57.000000 Djaq-1.0.9/djaq/djaq_ui/models.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 10:51:21.855200 Djaq-1.0.9/djaq/djaq_ui/templates/
+-rw-r--r--   0 paul       (501) staff       (20)      487 2021-04-02 10:29:12.000000 Djaq-1.0.9/djaq/djaq_ui/templates/base_query.html
+-rw-r--r--   0 paul       (501) staff       (20)     9555 2022-05-27 07:21:51.000000 Djaq-1.0.9/djaq/djaq_ui/templates/query.html
+-rw-r--r--   0 paul       (501) staff       (20)       60 2020-07-28 20:13:57.000000 Djaq-1.0.9/djaq/djaq_ui/tests.py
+-rw-r--r--   0 paul       (501) staff       (20)      444 2020-07-28 20:13:57.000000 Djaq-1.0.9/djaq/djaq_ui/urls.py
+-rw-r--r--   0 paul       (501) staff       (20)     4232 2022-08-25 05:29:25.000000 Djaq-1.0.9/djaq/djaq_ui/views.py
+-rw-r--r--   0 paul       (501) staff       (20)      104 2020-07-28 20:13:57.000000 Djaq-1.0.9/djaq/exceptions.py
+-rw-r--r--   0 paul       (501) staff       (20)     6562 2023-05-03 10:39:00.000000 Djaq-1.0.9/djaq/functions.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-03 10:51:21.855902 Djaq-1.0.9/djaq/query/
+-rw-r--r--   0 paul       (501) staff       (20)    50446 2023-05-03 10:41:29.000000 Djaq-1.0.9/djaq/query/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)     2634 2021-04-01 09:11:56.000000 Djaq-1.0.9/djaq/result.py
+-rw-r--r--   0 paul       (501) staff       (20)       38 2023-05-03 10:51:21.857577 Djaq-1.0.9/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)     1604 2022-06-06 15:35:54.000000 Djaq-1.0.9/setup.py
```

### Comparing `Djaq-1.0.8/Djaq.egg-info/PKG-INFO` & `Djaq-1.0.9/Djaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Djaq
-Version: 1.0.8
+Version: 1.0.9
 Summary: A string-based Django query language
 Home-page: https://github.com/paul-wolf/djaq
 Author: Paul Wolf
 Author-email: paul.wolf@yewleaf.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `Djaq-1.0.8/Djaq.egg-info/SOURCES.txt` & `Djaq-1.0.9/Djaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Djaq-1.0.8/LICENSE` & `Djaq-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Djaq-1.0.8/PKG-INFO` & `Djaq-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Djaq
-Version: 1.0.8
+Version: 1.0.9
 Summary: A string-based Django query language
 Home-page: https://github.com/paul-wolf/djaq
 Author: Paul Wolf
 Author-email: paul.wolf@yewleaf.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `Djaq-1.0.8/README.rst` & `Djaq-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `Djaq-1.0.8/djaq/app_utils.py` & `Djaq-1.0.9/djaq/app_utils.py`

 * *Files identical despite different names*

### Comparing `Djaq-1.0.8/djaq/conditions.py` & `Djaq-1.0.9/djaq/conditions.py`

 * *Files identical despite different names*

### Comparing `Djaq-1.0.8/djaq/djaq_api/views.py` & `Djaq-1.0.9/djaq/djaq_api/views.py`

 * *Files identical despite different names*

### Comparing `Djaq-1.0.8/djaq/djaq_ui/management/commands/djaq.py` & `Djaq-1.0.9/djaq/djaq_ui/management/commands/djaq.py`

 * *Files identical despite different names*

### Comparing `Djaq-1.0.8/djaq/djaq_ui/management/commands/run.py` & `Djaq-1.0.9/djaq/djaq_ui/management/commands/run.py`

 * *Files identical despite different names*

### Comparing `Djaq-1.0.8/djaq/djaq_ui/templates/query.html` & `Djaq-1.0.9/djaq/djaq_ui/templates/query.html`

 * *Files identical despite different names*

### Comparing `Djaq-1.0.8/djaq/djaq_ui/views.py` & `Djaq-1.0.9/djaq/djaq_ui/views.py`

 * *Files identical despite different names*

### Comparing `Djaq-1.0.8/djaq/functions.py` & `Djaq-1.0.9/djaq/functions.py`

 * *Files identical despite different names*

### Comparing `Djaq-1.0.8/djaq/query/__init__.py` & `Djaq-1.0.9/djaq/query/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,18 @@
 
         TODO: Only works for Postgresql.
 
         """
 
         conn = connections[self.using]
         cursor = conn.cursor()
-        return cursor.mogrify(sql, parameters).decode()
+        mogrified = cursor.mogrify(sql, parameters)
+        if isinstance(mogrified, bytes):
+            return mogrified.decode()
+        return mogrified
 
     def dump(self):
         for k, v in self.__dict__.items():
             print(f"{k}={v}")
 
     def conditions(self, node: B):
         self.condition_node = node
```

### Comparing `Djaq-1.0.8/djaq/result.py` & `Djaq-1.0.9/djaq/result.py`

 * *Files identical despite different names*

### Comparing `Djaq-1.0.8/setup.py` & `Djaq-1.0.9/setup.py`

 * *Files identical despite different names*

