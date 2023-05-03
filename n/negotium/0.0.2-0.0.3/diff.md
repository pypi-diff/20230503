# Comparing `tmp/negotium-0.0.2.tar.gz` & `tmp/negotium-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "negotium-0.0.2.tar", last modified: Wed May  3 19:51:36 2023, max compression
+gzip compressed data, was "negotium-0.0.3.tar", last modified: Wed May  3 21:54:21 2023, max compression
```

## Comparing `negotium-0.0.2.tar` & `negotium-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:51:36.767448 negotium-0.0.2/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1140 2023-05-03 19:51:36.767448 negotium-0.0.2/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      973 2023-05-03 19:17:50.000000 negotium-0.0.2/README.md
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:51:36.763447 negotium-0.0.2/negotium/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.0.2/negotium/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3276 2023-05-03 19:18:24.000000 negotium-0.0.2/negotium/base.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:51:36.767448 negotium-0.0.2/negotium/mq/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.0.2/negotium/mq/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3917 2023-05-03 19:30:35.000000 negotium-0.0.2/negotium/mq/consumer.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1451 2023-05-03 13:25:19.000000 negotium-0.0.2/negotium/mq/publisher.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      510 2023-05-03 18:50:00.000000 negotium-0.0.2/negotium/settings.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      490 2023-05-03 12:19:38.000000 negotium-0.0.2/negotium/task.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:51:36.767448 negotium-0.0.2/negotium/utils/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.0.2/negotium/utils/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.0.2/negotium/utils/logger.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 19:51:36.763447 negotium-0.0.2/negotium.egg-info/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1140 2023-05-03 19:51:36.000000 negotium-0.0.2/negotium.egg-info/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      384 2023-05-03 19:51:36.000000 negotium-0.0.2/negotium.egg-info/SOURCES.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-03 19:51:36.000000 negotium-0.0.2/negotium.egg-info/dependency_links.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      100 2023-05-03 19:51:36.000000 negotium-0.0.2/negotium.egg-info/requires.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-03 19:51:36.000000 negotium-0.0.2/negotium.egg-info/top_level.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      405 2023-05-03 19:51:25.000000 negotium-0.0.2/pyproject.toml
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-03 19:51:36.767448 negotium-0.0.2/setup.cfg
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 21:54:21.601055 negotium-0.0.3/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       51 2023-05-03 19:58:57.000000 negotium-0.0.3/.gitignore
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1140 2023-05-03 21:54:21.601055 negotium-0.0.3/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      973 2023-05-03 19:17:50.000000 negotium-0.0.3/README.md
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 21:54:21.597054 negotium-0.0.3/negotium/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.0.3/negotium/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3314 2023-05-03 21:11:57.000000 negotium-0.0.3/negotium/base.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 21:54:21.601055 negotium-0.0.3/negotium/mq/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.0.3/negotium/mq/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     5197 2023-05-03 21:51:34.000000 negotium-0.0.3/negotium/mq/consumer.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1569 2023-05-03 21:22:40.000000 negotium-0.0.3/negotium/mq/publisher.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      510 2023-05-03 18:50:00.000000 negotium-0.0.3/negotium/settings.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      490 2023-05-03 12:19:38.000000 negotium-0.0.3/negotium/task.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 21:54:21.601055 negotium-0.0.3/negotium/utils/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.0.3/negotium/utils/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.0.3/negotium/utils/logger.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 21:54:21.601055 negotium-0.0.3/negotium.egg-info/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1140 2023-05-03 21:54:21.000000 negotium-0.0.3/negotium.egg-info/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      430 2023-05-03 21:54:21.000000 negotium-0.0.3/negotium.egg-info/SOURCES.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-03 21:54:21.000000 negotium-0.0.3/negotium.egg-info/dependency_links.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      100 2023-05-03 21:54:21.000000 negotium-0.0.3/negotium.egg-info/requires.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-03 21:54:21.000000 negotium-0.0.3/negotium.egg-info/top_level.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      405 2023-05-03 21:54:08.000000 negotium-0.0.3/pyproject.toml
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      455 2023-05-03 19:02:07.000000 negotium-0.0.3/requirements.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-03 21:54:21.601055 negotium-0.0.3/setup.cfg
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 21:54:21.601055 negotium-0.0.3/tests/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 09:50:29.000000 negotium-0.0.3/tests/__init__.py
```

### Comparing `negotium-0.0.2/PKG-INFO` & `negotium-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negotium
-Version: 0.0.2
+Version: 0.0.3
 Summary: A very simple asynchronous task/job queue
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Negotium
 
 A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. It runs on a single machine, and it is designed to be used in a single process.
```

### Comparing `negotium-0.0.2/README.md` & `negotium-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `negotium-0.0.2/negotium/base.py` & `negotium-0.0.3/negotium/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         if not broker_url:
             broker_url = f"redis://{DEFAULT_HOST}:{DEFAULT_PORT}/0"
 
         db = int(broker_url.split('/')[-1])
         host = broker_url.split('/')[2].split(':')[0]
         port = int(broker_url.split('/')[2].split(':')[1])
 
-        self.consumer = _Consumer(db=db, host=host, port=port, logfile=logfile)
-        self.publisher = _Publisher(db=db, host=host, port=port, logfile=logfile)
+        self.consumer = _Consumer(db=db, host=host, port=port, app_name=app_name, logfile=logfile)
+        self.publisher = _Publisher(db=db, host=host, port=port, app_name=app_name, logfile=logfile)
         self.logfile = logfile
 
     def start(self, *args, **kwargs):
         """Use this method to consume tasks from the message broker
 
         Example:
             negotium.start()
```

### Comparing `negotium-0.0.2/negotium/mq/publisher.py` & `negotium-0.0.3/negotium/mq/publisher.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 import json
 import redis
 
 from negotium.settings import DEFAULT_QUEUE, DEFAULT_SCHEDULER_QUEUE, DEFAULT_SCHEDULER_SORTED_SET
 from negotium.utils.logger import log
 
 class _Publisher:
-    def __init__(self, db: int, host: str, port: int, logfile: str=None):
+    def __init__(self, db: int, host: str, port: int, app_name: str, logfile: str=None):
         self.connection = None
-        self.logfile = logfile
         self.db = db
         self.host = host
         self.port = port
+        self.app_name = app_name
+        self.logfile = logfile
 
     def _create_connection(self):
         """Create a connection to the message broker
         """
         self.connection = redis.Redis(db=self.db, host=self.host, port=self.port)
 
     def _close_connection(self):
@@ -28,13 +29,14 @@
         """
         log(self.logfile, data.get('app_name'), f"Received task: {data.get('function_name')}")
         if eta:
             data = {
                 '_task': data,
                 '_eta': eta.strftime('%Y-%m-%d %H:%M:%S.%f')
             }
-            self.connection.rpush(DEFAULT_SCHEDULER_QUEUE, json.dumps(data))
+            self.connection.rpush(DEFAULT_SCHEDULER_QUEUE + "__" + self.app_name, json.dumps(data))
             # zadd
             timestamp = datetime.datetime.strptime(eta.strftime('%Y-%m-%d %H:%M:%S.%f'), '%Y-%m-%d %H:%M:%S.%f').timestamp()
-            self.connection.zadd(DEFAULT_SCHEDULER_SORTED_SET, {json.dumps(data): timestamp})
+            self.connection.zadd(DEFAULT_SCHEDULER_SORTED_SET + "__" + self.app_name, {json.dumps(data): timestamp})
         else:
-            self.connection.rpush(DEFAULT_QUEUE, json.dumps(data))
+            self.connection.rpush(DEFAULT_QUEUE + "__" + self.app_name, json.dumps(data))
+
```

### Comparing `negotium-0.0.2/negotium/utils/logger.py` & `negotium-0.0.3/negotium/utils/logger.py`

 * *Files identical despite different names*

### Comparing `negotium-0.0.2/negotium.egg-info/PKG-INFO` & `negotium-0.0.3/negotium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negotium
-Version: 0.0.2
+Version: 0.0.3
 Summary: A very simple asynchronous task/job queue
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Negotium
 
 A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. It runs on a single machine, and it is designed to be used in a single process.
```

