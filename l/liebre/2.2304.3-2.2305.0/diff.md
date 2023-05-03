# Comparing `tmp/liebre-2.2304.3-py3-none-any.whl.zip` & `tmp/liebre-2.2305.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 20013 bytes, number of entries: 13
--rw-rw-r--  2.0 unx      222 b- defN 23-Apr-20 23:06 liebre/__init__.py
--rw-rw-r--  2.0 unx     8039 b- defN 23-Apr-20 11:36 liebre/consumer.py
+Zip file size: 20147 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      222 b- defN 23-May-03 10:32 liebre/__init__.py
+-rw-rw-r--  2.0 unx     8384 b- defN 23-Apr-27 22:14 liebre/consumer.py
 -rw-rw-r--  2.0 unx       46 b- defN 22-Dec-07 11:43 liebre/liebre.py
 -rw-rw-r--  2.0 unx       69 b- defN 22-Dec-07 11:44 liebre/logger.py
 -rw-rw-r--  2.0 unx      490 b- defN 23-Apr-19 20:41 liebre/message.py
--rw-rw-r--  2.0 unx     2535 b- defN 23-Jan-17 11:16 liebre/producer.py
--rw-rw-r--  2.0 unx     7800 b- defN 23-Apr-20 23:01 liebre/rabbit_store.py
--rw-rw-r--  2.0 unx     1018 b- defN 23-Apr-20 21:23 liebre/utils.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-Apr-20 23:06 liebre-2.2304.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx      730 b- defN 23-Apr-20 23:06 liebre-2.2304.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 23:06 liebre-2.2304.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-20 23:06 liebre-2.2304.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      985 b- defN 23-Apr-20 23:06 liebre-2.2304.3.dist-info/RECORD
-13 files, 57182 bytes uncompressed, 18385 bytes compressed:  67.8%
+-rw-rw-r--  2.0 unx     2535 b- defN 23-Apr-27 14:44 liebre/producer.py
+-rw-rw-r--  2.0 unx     8171 b- defN 23-Apr-27 22:14 liebre/rabbit_store.py
+-rw-rw-r--  2.0 unx     1018 b- defN 23-Apr-27 14:55 liebre/utils.py
+-rw-rw-r--  2.0 unx    35149 b- defN 23-May-03 10:32 liebre-2.2305.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      730 b- defN 23-May-03 10:32 liebre-2.2305.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-03 10:32 liebre-2.2305.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-03 10:32 liebre-2.2305.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      985 b- defN 23-May-03 10:32 liebre-2.2305.0.dist-info/RECORD
+13 files, 57898 bytes uncompressed, 18519 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: liebre/rabbit_store.py
 Comment: 
 
 Filename: liebre/utils.py
 Comment: 
 
-Filename: liebre-2.2304.3.dist-info/LICENSE
+Filename: liebre-2.2305.0.dist-info/LICENSE
 Comment: 
 
-Filename: liebre-2.2304.3.dist-info/METADATA
+Filename: liebre-2.2305.0.dist-info/METADATA
 Comment: 
 
-Filename: liebre-2.2304.3.dist-info/WHEEL
+Filename: liebre-2.2305.0.dist-info/WHEEL
 Comment: 
 
-Filename: liebre-2.2304.3.dist-info/top_level.txt
+Filename: liebre-2.2305.0.dist-info/top_level.txt
 Comment: 
 
-Filename: liebre-2.2304.3.dist-info/RECORD
+Filename: liebre-2.2305.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## liebre/__init__.py

```diff
@@ -2,10 +2,10 @@
 # -*- coding: utf-8 -*-
 
 from .consumer import Consumer  # noqa F401
 from .producer import Producer  # noqa F401
 
 import logging
 
-__version__ = '2.2304.3'
+__version__ = '2.2305.0'
 
 logging.getLogger('pika').propagate = False
```

## liebre/consumer.py

```diff
@@ -185,57 +185,67 @@
         except Exception:
             logger.exception('Could not process the message.')
             channel.basic_nack(
                 delivery_tag=callback.delivery_tag,
                 requeue=True,
             )
 
-    def reconnect(function):
+    def reconnect_consumer(function):
 
         def _(*args, **kwargs):
+            retries = 0
             instance = args[0]
 
-            retries = 0
             while True:
                 try:
                     channel = instance._get_channel()
                     return function(
-                        *args,
-                        channel=channel,
+                        instance,
+                        channel,
+                        *args[1:],
                         **kwargs,
                     )
 
                 except Exception as error:
+                    RabbitStore._close_channel(channel)
+
+                    time.sleep(instance._sleep_seconds_on_retry)
+
                     retries += 1
                     if (not instance._max_retries
                             or retries >= instance._max_retries):
                         raise error
 
                     logger.warning(
                         'Reconnecting... '
                         f'({retries}/{instance._max_retries})',
                         error=error
                     )
 
                     try:
+                        instance.connect(force=True)
                         channel = instance._get_channel()
+                        retries = 0
+
                     except Exception:
-                        pass
-                    time.sleep(instance._sleep_seconds_on_retry)
+                        logger.exception(
+                            'Reconnecting... '
+                            f'({retries}/{instance._max_retries})',
+                        )
 
         return _
 
-    @reconnect
+    @reconnect_consumer
     def _consume_target(
         self,
+        channel,
         queue,
         callback,
         backup,
         queue_options=None,
-        channel=None,
     ):
         self._callbacks[queue] = {'callback': callback}
 
         if queue not in self._declared_logical_queues:
             self.declare_queue(
                 queue,
                 options=queue_options,
```

## liebre/producer.py

 * *Ordering differences only*

```diff
@@ -1,19 +1,19 @@
 import random
 import uuid
 from pika import BasicProperties
 from pika import DeliveryMode
+from threading import Lock
 from .logger import logger
 from .utils import (
     get_partition_queue_name,
     serialize_content,
     get_backup_queue_name,
 )
 from .rabbit_store import RabbitStore
-from threading import Lock
 
 
 class Producer(RabbitStore):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._producer_lock = Lock()  # Make produce() thread-safe
```

## liebre/rabbit_store.py

```diff
@@ -89,21 +89,21 @@
 
         self._initialized = False
 
     def reconnect(function):
 
         def _(*args, **kwargs):
             retries = 0
+            instance = args[0]
 
             while True:
                 try:
                     return function(*args, **kwargs)
 
                 except Exception as error:
-                    instance = args[0]
                     time.sleep(instance._sleep_seconds_on_retry)
 
                     retries += 1
                     if (not instance._max_retries
                             or retries >= instance._max_retries):
                         raise error
 
@@ -111,14 +111,16 @@
                         'Reconnecting... '
                         f'({retries}/{instance._max_retries})',
                         error=error
                     )
 
                     try:
                         instance.connect(force=True)
+                        retries = 0
+
                     except Exception:
                         logger.exception(
                             'Reconnecting... '
                             f'({retries}/{instance._max_retries})',
                         )
 
         return _
@@ -129,16 +131,18 @@
             instance = args[0]
             with instance._lock:
                 return function(*args, **kwargs)
 
         return _
 
     def connect(self, force=False):
-        if not force and self._initialized:
+        if self._initialized and not force:
             return
+        elif force:
+            RabbitStore._close_channel(self._channel)
 
         self._channel = self._get_channel()
         self._declare_exchange()
 
         self._initialized = True
 
     @reconnect
@@ -272,7 +276,19 @@
         )
 
         channel = connection.channel()
         channel.confirm_delivery()
         channel.basic_qos(prefetch_count=prefetch)
 
         return channel
+
+    @staticmethod
+    def _close_channel(channel):
+        try:
+            connection = channel._connection
+            channel.close()
+        except Exception:
+            pass
+        try:
+            connection.close()
+        except Exception:
+            pass
```

## Comparing `liebre-2.2304.3.dist-info/LICENSE` & `liebre-2.2305.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `liebre-2.2304.3.dist-info/METADATA` & `liebre-2.2305.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liebre
-Version: 2.2304.3
+Version: 2.2305.0
 Home-page: https://github.com/councilbox/liebre-python
 Author: 
 Author-email: 
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

## Comparing `liebre-2.2304.3.dist-info/RECORD` & `liebre-2.2305.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-liebre/__init__.py,sha256=bp0JR3Iy4UXJA7JEbrJa00ZmagqK09L4Bj9nsa4Wbek,222
-liebre/consumer.py,sha256=gcsx34BpR4ermuBz0FACiqZsVKIZ2fhv_4THzcfZ7EU,8039
+liebre/__init__.py,sha256=lagqSobqe189CGJzaJCLOxZuL4RX1kAfeaROcVGvaCI,222
+liebre/consumer.py,sha256=5ZWDGJPsb6k_rLpMKdN4597jL8SCgI1WyCq5tSqBWxU,8384
 liebre/liebre.py,sha256=FZk9hm7vBsK8G16pNugputbrrEciYqJc_XRAhTCcojI,46
 liebre/logger.py,sha256=gFdT_UHqta9GXzzGK44_sDagnInpWDLKXDJ3J4ZJkmc,69
 liebre/message.py,sha256=LsyOktRKgYOs5FzllpmfuoWWKM8t9mB7-OSRFVnjXxE,490
-liebre/producer.py,sha256=P3pM3PWePHbMKj3BPGvFgCaT_lrJS336GyHREYmyx0M,2535
-liebre/rabbit_store.py,sha256=4VjriEuVcBz0JLthvbv_xD0F9PnPS2CJAZjimSCLLWY,7800
+liebre/producer.py,sha256=JFjqRpR5k7Sl2c3ZM2I-HoWOIbjMOUb-sQ4uk3JXa00,2535
+liebre/rabbit_store.py,sha256=Eg_Crj1e1LH3KkENMlVROWmvhT8yac8P3BMlLWIuMkI,8171
 liebre/utils.py,sha256=2SElH6GLKFTuLpSzZwWfLa2VTzHetfxtXPfGuEuLcWM,1018
-liebre-2.2304.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-liebre-2.2304.3.dist-info/METADATA,sha256=jgEkxDg5opJhuXcKYOwhDhwnAgYJdFQ8WXev6ybKA-c,730
-liebre-2.2304.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-liebre-2.2304.3.dist-info/top_level.txt,sha256=cl5ALalM53myFXDcFp7jtynIzvwoKF4RqF1x1Aw4WwY,7
-liebre-2.2304.3.dist-info/RECORD,,
+liebre-2.2305.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+liebre-2.2305.0.dist-info/METADATA,sha256=khfOlvYmOOIbawqkcoONKA28IQQXfpVFcKcbfltnm44,730
+liebre-2.2305.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+liebre-2.2305.0.dist-info/top_level.txt,sha256=cl5ALalM53myFXDcFp7jtynIzvwoKF4RqF1x1Aw4WwY,7
+liebre-2.2305.0.dist-info/RECORD,,
```

