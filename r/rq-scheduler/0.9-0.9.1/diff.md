# Comparing `tmp/rq-scheduler-0.9.tar.gz` & `tmp/rq-scheduler-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rq-scheduler-0.9.tar", last modified: Tue Dec 11 23:15:00 2018, max compression
+gzip compressed data, was "dist/rq-scheduler-0.9.1.tar", last modified: Tue Oct  8 03:24:47 2019, max compression
```

## Comparing `rq-scheduler-0.9.tar` & `rq-scheduler-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2018-12-11 23:15:00.000000 rq-scheduler-0.9/
--rw-r--r--   0 selwin     (501) staff       (20)    11797 2018-12-11 23:15:00.000000 rq-scheduler-0.9/PKG-INFO
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2018-12-11 23:15:00.000000 rq-scheduler-0.9/rq_scheduler.egg-info/
--rw-r--r--   0 selwin     (501) staff       (20)    11797 2018-12-11 23:15:00.000000 rq-scheduler-0.9/rq_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 selwin     (501) staff       (20)        1 2018-02-04 11:18:06.000000 rq-scheduler-0.9/rq_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 selwin     (501) staff       (20)      448 2018-12-11 23:15:00.000000 rq-scheduler-0.9/rq_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 selwin     (501) staff       (20)       82 2018-12-11 23:15:00.000000 rq-scheduler-0.9/rq_scheduler.egg-info/entry_points.txt
--rw-r--r--   0 selwin     (501) staff       (20)       25 2018-12-11 23:15:00.000000 rq-scheduler-0.9/rq_scheduler.egg-info/requires.txt
--rw-r--r--   0 selwin     (501) staff       (20)       13 2018-12-11 23:15:00.000000 rq-scheduler-0.9/rq_scheduler.egg-info/top_level.txt
--rw-r--r--   0 selwin     (501) staff       (20)        1 2018-12-11 23:15:00.000000 rq-scheduler-0.9/rq_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 selwin     (501) staff       (20)       74 2018-01-29 23:54:34.000000 rq-scheduler-0.9/MANIFEST.in
--rw-r--r--   0 selwin     (501) staff       (20)     1452 2018-12-11 23:14:04.000000 rq-scheduler-0.9/setup.py
--rw-r--r--   0 selwin     (501) staff       (20)       82 2018-12-11 23:15:00.000000 rq-scheduler-0.9/setup.cfg
--rw-r--r--   0 selwin     (501) staff       (20)     8877 2018-12-11 12:14:23.000000 rq-scheduler-0.9/README.rst
--rw-r--r--   0 selwin     (501) staff       (20)     1053 2018-01-29 23:54:34.000000 rq-scheduler-0.9/LICENSE.txt
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2018-12-11 23:15:00.000000 rq-scheduler-0.9/rq_scheduler/
--rw-r--r--   0 selwin     (501) staff       (20)       54 2018-12-11 23:14:11.000000 rq-scheduler-0.9/rq_scheduler/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)     1531 2018-01-29 23:54:34.000000 rq-scheduler-0.9/rq_scheduler/utils.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2018-12-11 23:15:00.000000 rq-scheduler-0.9/rq_scheduler/scripts/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2018-01-29 23:54:34.000000 rq-scheduler-0.9/rq_scheduler/scripts/__init__.py
--rwxr-xr-x   0 selwin     (501) staff       (20)     2653 2018-03-02 07:43:12.000000 rq-scheduler-0.9/rq_scheduler/scripts/rqscheduler.py
--rw-r--r--   0 selwin     (501) staff       (20)    16462 2018-12-11 23:09:19.000000 rq-scheduler-0.9/rq_scheduler/scheduler.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2019-10-08 03:24:47.000000 rq-scheduler-0.9.1/
+-rw-r--r--   0 selwin     (501) staff       (20)    12185 2019-10-08 03:24:47.000000 rq-scheduler-0.9.1/PKG-INFO
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2019-10-08 03:24:47.000000 rq-scheduler-0.9.1/rq_scheduler.egg-info/
+-rw-r--r--   0 selwin     (501) staff       (20)    12185 2019-10-08 03:24:47.000000 rq-scheduler-0.9.1/rq_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2018-02-04 11:18:06.000000 rq-scheduler-0.9.1/rq_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 selwin     (501) staff       (20)      448 2019-10-08 03:24:47.000000 rq-scheduler-0.9.1/rq_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       82 2019-10-08 03:24:47.000000 rq-scheduler-0.9.1/rq_scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       25 2019-10-08 03:24:47.000000 rq-scheduler-0.9.1/rq_scheduler.egg-info/requires.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       13 2019-10-08 03:24:47.000000 rq-scheduler-0.9.1/rq_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2019-10-08 03:24:47.000000 rq-scheduler-0.9.1/rq_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       74 2018-01-29 23:54:34.000000 rq-scheduler-0.9.1/MANIFEST.in
+-rw-r--r--   0 selwin     (501) staff       (20)     1405 2019-10-08 03:23:01.000000 rq-scheduler-0.9.1/setup.py
+-rw-r--r--   0 selwin     (501) staff       (20)       61 2019-10-08 03:24:47.000000 rq-scheduler-0.9.1/setup.cfg
+-rw-r--r--   0 selwin     (501) staff       (20)     9257 2019-10-08 03:17:48.000000 rq-scheduler-0.9.1/README.rst
+-rw-r--r--   0 selwin     (501) staff       (20)     1053 2018-01-29 23:54:34.000000 rq-scheduler-0.9.1/LICENSE.txt
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2019-10-08 03:24:47.000000 rq-scheduler-0.9.1/rq_scheduler/
+-rw-r--r--   0 selwin     (501) staff       (20)       54 2019-10-08 03:23:09.000000 rq-scheduler-0.9.1/rq_scheduler/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1531 2018-01-29 23:54:34.000000 rq-scheduler-0.9.1/rq_scheduler/utils.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2019-10-08 03:24:47.000000 rq-scheduler-0.9.1/rq_scheduler/scripts/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2018-01-29 23:54:34.000000 rq-scheduler-0.9.1/rq_scheduler/scripts/__init__.py
+-rwxr-xr-x   0 selwin     (501) staff       (20)     2653 2018-03-02 07:43:12.000000 rq-scheduler-0.9.1/rq_scheduler/scripts/rqscheduler.py
+-rw-r--r--   0 selwin     (501) staff       (20)    16636 2019-10-08 03:17:48.000000 rq-scheduler-0.9.1/rq_scheduler/scheduler.py
```

### Comparing `rq-scheduler-0.9/PKG-INFO` & `rq-scheduler-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rq-scheduler
-Version: 0.9
+Version: 0.9.1
 Summary: Provides job scheduling capabilities to RQ (Redis Queue)
 Home-page: https://github.com/rq/rq-scheduler
 Author: Selwin Ong
 Author-email: selwin.ong@gmail.com
 License: MIT
 Description: ============
         RQ Scheduler
@@ -13,14 +13,20 @@
         `RQ Scheduler <https://github.com/rq/rq-scheduler>`_ is a small package that
         adds job scheduling capabilities to `RQ <https://github.com/nvie/rq>`_,
         a `Redis <http://redis.io/>`_ based Python queuing library.
         
         .. image:: https://travis-ci.org/rq/rq-scheduler.svg?branch=master
             :target: https://travis-ci.org/rq/rq-scheduler
         
+        ====================
+        Support RQ Scheduler
+        ====================
+        
+        If you find ``rq-scheduler`` useful, please consider supporting its development via `Tidelift <https://tidelift.com/subscription/pkg/pypi-rq_scheduler?utm_source=pypi-rq-scheduler&utm_medium=referral&utm_campaign=readme>`_.
+        
         ============
         Requirements
         ============
         
         * `RQ`_
         
         ============
@@ -52,17 +58,18 @@
         
             from redis import Redis
             from rq import Queue
             from rq_scheduler import Scheduler
             from datetime import datetime
         
             scheduler = Scheduler(connection=Redis()) # Get a scheduler for the "default" queue
+            scheduler = Scheduler('foo', connection=Redis()) # Get a scheduler for the "foo" queue
         
             # You can also instantiate a Scheduler using an RQ Queue
-            queue = Queue('foo', connection=Redis())
+            queue = Queue('bar', connection=Redis())
             scheduler = Scheduler(queue=queue)
         
             # Puts a job into the scheduler. The API is similar to RQ except that it
             # takes a datetime object as first argument. So for example to schedule a
             # job to run on Jan 1st 2020 we do:
             scheduler.enqueue_at(datetime(2020, 1, 1), func) # Date time should be in UTC
         
@@ -264,12 +271,11 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `rq-scheduler-0.9/rq_scheduler.egg-info/PKG-INFO` & `rq-scheduler-0.9.1/rq_scheduler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rq-scheduler
-Version: 0.9
+Version: 0.9.1
 Summary: Provides job scheduling capabilities to RQ (Redis Queue)
 Home-page: https://github.com/rq/rq-scheduler
 Author: Selwin Ong
 Author-email: selwin.ong@gmail.com
 License: MIT
 Description: ============
         RQ Scheduler
@@ -13,14 +13,20 @@
         `RQ Scheduler <https://github.com/rq/rq-scheduler>`_ is a small package that
         adds job scheduling capabilities to `RQ <https://github.com/nvie/rq>`_,
         a `Redis <http://redis.io/>`_ based Python queuing library.
         
         .. image:: https://travis-ci.org/rq/rq-scheduler.svg?branch=master
             :target: https://travis-ci.org/rq/rq-scheduler
         
+        ====================
+        Support RQ Scheduler
+        ====================
+        
+        If you find ``rq-scheduler`` useful, please consider supporting its development via `Tidelift <https://tidelift.com/subscription/pkg/pypi-rq_scheduler?utm_source=pypi-rq-scheduler&utm_medium=referral&utm_campaign=readme>`_.
+        
         ============
         Requirements
         ============
         
         * `RQ`_
         
         ============
@@ -52,17 +58,18 @@
         
             from redis import Redis
             from rq import Queue
             from rq_scheduler import Scheduler
             from datetime import datetime
         
             scheduler = Scheduler(connection=Redis()) # Get a scheduler for the "default" queue
+            scheduler = Scheduler('foo', connection=Redis()) # Get a scheduler for the "foo" queue
         
             # You can also instantiate a Scheduler using an RQ Queue
-            queue = Queue('foo', connection=Redis())
+            queue = Queue('bar', connection=Redis())
             scheduler = Scheduler(queue=queue)
         
             # Puts a job into the scheduler. The API is similar to RQ except that it
             # takes a datetime object as first argument. So for example to schedule a
             # job to run on Jan 1st 2020 we do:
             scheduler.enqueue_at(datetime(2020, 1, 1), func) # Date time should be in UTC
         
@@ -264,12 +271,11 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `rq-scheduler-0.9/setup.py` & `rq-scheduler-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 tests_require = []
 if sys.version_info < (2, 7):
     tests_require.append('discover==0.4.0')
 
 
 setup(
     name='rq-scheduler',
-    version='0.9',
+    version='0.9.1',
     author='Selwin Ong',
     author_email='selwin.ong@gmail.com',
     packages=['rq_scheduler'],
     url='https://github.com/rq/rq-scheduler',
     license='MIT',
     description='Provides job scheduling capabilities to RQ (Redis Queue)',
     long_description=open('README.rst').read(),
@@ -32,14 +32,13 @@
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ]
 )
```

### Comparing `rq-scheduler-0.9/README.rst` & `rq-scheduler-0.9.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 `RQ Scheduler <https://github.com/rq/rq-scheduler>`_ is a small package that
 adds job scheduling capabilities to `RQ <https://github.com/nvie/rq>`_,
 a `Redis <http://redis.io/>`_ based Python queuing library.
 
 .. image:: https://travis-ci.org/rq/rq-scheduler.svg?branch=master
     :target: https://travis-ci.org/rq/rq-scheduler
 
+====================
+Support RQ Scheduler
+====================
+
+If you find ``rq-scheduler`` useful, please consider supporting its development via `Tidelift <https://tidelift.com/subscription/pkg/pypi-rq_scheduler?utm_source=pypi-rq-scheduler&utm_medium=referral&utm_campaign=readme>`_.
+
 ============
 Requirements
 ============
 
 * `RQ`_
 
 ============
@@ -44,17 +50,18 @@
 
     from redis import Redis
     from rq import Queue
     from rq_scheduler import Scheduler
     from datetime import datetime
 
     scheduler = Scheduler(connection=Redis()) # Get a scheduler for the "default" queue
+    scheduler = Scheduler('foo', connection=Redis()) # Get a scheduler for the "foo" queue
 
     # You can also instantiate a Scheduler using an RQ Queue
-    queue = Queue('foo', connection=Redis())
+    queue = Queue('bar', connection=Redis())
     scheduler = Scheduler(queue=queue)
 
     # Puts a job into the scheduler. The API is similar to RQ except that it
     # takes a datetime object as first argument. So for example to schedule a
     # job to run on Jan 1st 2020 we do:
     scheduler.enqueue_at(datetime(2020, 1, 1), func) # Date time should be in UTC
```

### Comparing `rq-scheduler-0.9/LICENSE.txt` & `rq-scheduler-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rq-scheduler-0.9/rq_scheduler/utils.py` & `rq-scheduler-0.9.1/rq_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `rq-scheduler-0.9/rq_scheduler/scripts/rqscheduler.py` & `rq-scheduler-0.9.1/rq_scheduler/scripts/rqscheduler.py`

 * *Files identical despite different names*

### Comparing `rq-scheduler-0.9/rq_scheduler/scheduler.py` & `rq-scheduler-0.9.1/rq_scheduler/scheduler.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,28 +107,31 @@
         signal.signal(signal.SIGINT, stop)
         signal.signal(signal.SIGTERM, stop)
 
     def _create_job(self, func, args=None, kwargs=None, commit=True,
                     result_ttl=None, ttl=None, id=None, description=None,
                     queue_name=None, timeout=None, meta=None):
         """
-        Creates an RQ job and saves it to Redis.
+        Creates an RQ job and saves it to Redis. The job is assigned to the
+        given queue name if not None else it is assigned to scheduler queue by
+        default.
         """
         if args is None:
             args = ()
         if kwargs is None:
             kwargs = {}
         job = self.job_class.create(
                 func, args=args, connection=self.connection,
                 kwargs=kwargs, result_ttl=result_ttl, ttl=ttl, id=id,
                 description=description, timeout=timeout, meta=meta)
-        if self._queue is not None:
-            job.origin = self._queue.name
+        if queue_name:
+            job.origin = queue_name
         else:
-            job.origin = queue_name or self.queue_name
+            job.origin = self.queue_name
+
         if commit:
             job.save()
         return job
 
     def enqueue_at(self, scheduled_time, func, *args, **kwargs):
         """
         Pushes a job to the scheduler queue. The scheduled queue is a Redis sorted
@@ -156,18 +159,19 @@
         """
         timeout = kwargs.pop('timeout', None)
         job_id = kwargs.pop('job_id', None)
         job_ttl = kwargs.pop('job_ttl', None)
         job_result_ttl = kwargs.pop('job_result_ttl', None)
         job_description = kwargs.pop('job_description', None)
         meta = kwargs.pop('meta', None)
+        queue_name = kwargs.pop('queue_name', None)
 
         job = self._create_job(func, args=args, kwargs=kwargs, timeout=timeout,
                                id=job_id, result_ttl=job_result_ttl, ttl=job_ttl,
-                               description=job_description, meta=meta)
+                               description=job_description, meta=meta, queue_name=queue_name)
         self.connection.zadd(self.scheduled_jobs_key,
                               {job.id: to_unix(scheduled_time)})
         return job
 
     def enqueue_in(self, time_delta, func, *args, **kwargs):
         """
         Similar to ``enqueue_at``, but accepts a timedelta instead of datetime object.
@@ -176,18 +180,19 @@
         """
         timeout = kwargs.pop('timeout', None)
         job_id = kwargs.pop('job_id', None)
         job_ttl = kwargs.pop('job_ttl', None)
         job_result_ttl = kwargs.pop('job_result_ttl', None)
         job_description = kwargs.pop('job_description', None)
         meta = kwargs.pop('meta', None)
+        queue_name = kwargs.pop('queue_name', None)
 
         job = self._create_job(func, args=args, kwargs=kwargs, timeout=timeout,
                                id=job_id, result_ttl=job_result_ttl, ttl=job_ttl,
-                               description=job_description, meta=meta)
+                               description=job_description, meta=meta, queue_name=queue_name)
         self.connection.zadd(self.scheduled_jobs_key,
                               {job.id: to_unix(datetime.utcnow() + time_delta)})
         return job
 
     def schedule(self, scheduled_time, func, args=None, kwargs=None,
                  interval=None, repeat=None, result_ttl=None, ttl=None,
                  timeout=None, id=None, description=None, queue_name=None,
@@ -333,16 +338,14 @@
         """
         return self.get_jobs(to_unix(datetime.utcnow()), with_times=with_times)
 
     def get_queue_for_job(self, job):
         """
         Returns a queue to put job into.
         """
-        if self._queue is not None:
-            return self._queue
         key = '{0}{1}'.format(self.queue_class.redis_queue_namespace_prefix,
                               job.origin)
         return self.queue_class.from_queue_key(
                 key, connection=self.connection, job_class=self.job_class)
 
     def enqueue_job(self, job):
         """
```

