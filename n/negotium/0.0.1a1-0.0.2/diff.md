# Comparing `tmp/negotium-0.0.1a1.tar.gz` & `tmp/negotium-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "negotium-0.0.1a1.tar", last modified: Wed May  3 19:49:18 2023, max compression
+gzip compressed data, was "negotium-0.0.2.tar", last modified: Wed May  3 19:51:36 2023, max compression
```

## Comparing `negotium-0.0.1a1.tar` & `negotium-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:49:18.178283 negotium-0.0.1a1/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1142 2023-05-03 19:49:18.178283 negotium-0.0.1a1/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      973 2023-05-03 19:17:50.000000 negotium-0.0.1a1/README.md
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:49:18.178283 negotium-0.0.1a1/negotium/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.0.1a1/negotium/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3276 2023-05-03 19:18:24.000000 negotium-0.0.1a1/negotium/base.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:49:18.178283 negotium-0.0.1a1/negotium/mq/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.0.1a1/negotium/mq/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3917 2023-05-03 19:30:35.000000 negotium-0.0.1a1/negotium/mq/consumer.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1451 2023-05-03 13:25:19.000000 negotium-0.0.1a1/negotium/mq/publisher.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      510 2023-05-03 18:50:00.000000 negotium-0.0.1a1/negotium/settings.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      490 2023-05-03 12:19:38.000000 negotium-0.0.1a1/negotium/task.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:49:18.178283 negotium-0.0.1a1/negotium/utils/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.0.1a1/negotium/utils/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.0.1a1/negotium/utils/logger.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:49:18.178283 negotium-0.0.1a1/negotium.egg-info/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1142 2023-05-03 19:49:18.000000 negotium-0.0.1a1/negotium.egg-info/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      384 2023-05-03 19:49:18.000000 negotium-0.0.1a1/negotium.egg-info/SOURCES.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-03 19:49:18.000000 negotium-0.0.1a1/negotium.egg-info/dependency_links.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      100 2023-05-03 19:49:18.000000 negotium-0.0.1a1/negotium.egg-info/requires.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-03 19:49:18.000000 negotium-0.0.1a1/negotium.egg-info/top_level.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      413 2023-05-03 19:49:04.000000 negotium-0.0.1a1/pyproject.toml
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-03 19:49:18.178283 negotium-0.0.1a1/setup.cfg
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:51:36.767448 negotium-0.0.2/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1140 2023-05-03 19:51:36.767448 negotium-0.0.2/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      973 2023-05-03 19:17:50.000000 negotium-0.0.2/README.md
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:51:36.763447 negotium-0.0.2/negotium/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.0.2/negotium/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3276 2023-05-03 19:18:24.000000 negotium-0.0.2/negotium/base.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:51:36.767448 negotium-0.0.2/negotium/mq/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.0.2/negotium/mq/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3917 2023-05-03 19:30:35.000000 negotium-0.0.2/negotium/mq/consumer.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1451 2023-05-03 13:25:19.000000 negotium-0.0.2/negotium/mq/publisher.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      510 2023-05-03 18:50:00.000000 negotium-0.0.2/negotium/settings.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      490 2023-05-03 12:19:38.000000 negotium-0.0.2/negotium/task.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:51:36.767448 negotium-0.0.2/negotium/utils/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.0.2/negotium/utils/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.0.2/negotium/utils/logger.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:51:36.763447 negotium-0.0.2/negotium.egg-info/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1140 2023-05-03 19:51:36.000000 negotium-0.0.2/negotium.egg-info/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      384 2023-05-03 19:51:36.000000 negotium-0.0.2/negotium.egg-info/SOURCES.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-03 19:51:36.000000 negotium-0.0.2/negotium.egg-info/dependency_links.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      100 2023-05-03 19:51:36.000000 negotium-0.0.2/negotium.egg-info/requires.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-03 19:51:36.000000 negotium-0.0.2/negotium.egg-info/top_level.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      405 2023-05-03 19:51:25.000000 negotium-0.0.2/pyproject.toml
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-03 19:51:36.767448 negotium-0.0.2/setup.cfg
```

### Comparing `negotium-0.0.1a1/PKG-INFO` & `negotium-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negotium
-Version: 0.0.1a1
+Version: 0.0.2
 Summary: A very simple asynchronous task/job queue
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Negotium
 
 A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. It runs on a single machine, and it is designed to be used in a single process.
```

### Comparing `negotium-0.0.1a1/README.md` & `negotium-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `negotium-0.0.1a1/negotium/base.py` & `negotium-0.0.2/negotium/base.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.1a1/negotium/mq/consumer.py` & `negotium-0.0.2/negotium/mq/consumer.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.1a1/negotium/mq/publisher.py` & `negotium-0.0.2/negotium/mq/publisher.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.1a1/negotium/utils/logger.py` & `negotium-0.0.2/negotium/utils/logger.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.1a1/negotium.egg-info/PKG-INFO` & `negotium-0.0.2/negotium.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negotium
-Version: 0.0.1a1
+Version: 0.0.2
 Summary: A very simple asynchronous task/job queue
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Negotium
 
 A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. It runs on a single machine, and it is designed to be used in a single process.
```

