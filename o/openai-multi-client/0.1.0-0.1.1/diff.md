# Comparing `tmp/openai_multi_client-0.1.0.tar.gz` & `tmp/openai_multi_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_multi_client-0.1.0.tar", last modified: Mon May  1 15:40:17 2023, max compression
+gzip compressed data, was "openai_multi_client-0.1.1.tar", last modified: Wed May  3 13:05:21 2023, max compression
```

## Comparing `openai_multi_client-0.1.0.tar` & `openai_multi_client-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-01 15:40:17.930097 openai_multi_client-0.1.0/
--rw-r--r--   0 zh217      (501) staff       (20)     1065 2023-05-01 15:39:52.000000 openai_multi_client-0.1.0/LICENSE
--rw-r--r--   0 zh217      (501) staff       (20)      385 2023-05-01 15:40:17.929973 openai_multi_client-0.1.0/PKG-INFO
--rw-r--r--   0 zh217      (501) staff       (20)       50 2023-05-01 15:35:02.000000 openai_multi_client-0.1.0/README.md
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-01 15:40:17.929078 openai_multi_client-0.1.0/openai_multi_client/
--rw-r--r--   0 zh217      (501) staff       (20)     8202 2023-05-01 15:11:47.000000 openai_multi_client-0.1.0/openai_multi_client/__init__.py
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-01 15:40:17.929815 openai_multi_client-0.1.0/openai_multi_client.egg-info/
--rw-r--r--   0 zh217      (501) staff       (20)      385 2023-05-01 15:40:17.000000 openai_multi_client-0.1.0/openai_multi_client.egg-info/PKG-INFO
--rw-r--r--   0 zh217      (501) staff       (20)      287 2023-05-01 15:40:17.000000 openai_multi_client-0.1.0/openai_multi_client.egg-info/SOURCES.txt
--rw-r--r--   0 zh217      (501) staff       (20)        1 2023-05-01 15:40:17.000000 openai_multi_client-0.1.0/openai_multi_client.egg-info/dependency_links.txt
--rw-r--r--   0 zh217      (501) staff       (20)       30 2023-05-01 15:40:17.000000 openai_multi_client-0.1.0/openai_multi_client.egg-info/requires.txt
--rw-r--r--   0 zh217      (501) staff       (20)       20 2023-05-01 15:40:17.000000 openai_multi_client-0.1.0/openai_multi_client.egg-info/top_level.txt
--rw-r--r--   0 zh217      (501) staff       (20)      528 2023-05-01 15:39:05.000000 openai_multi_client-0.1.0/pyproject.toml
--rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-01 15:40:17.930141 openai_multi_client-0.1.0/setup.cfg
--rw-r--r--   0 zh217      (501) staff       (20)       37 2023-05-01 15:35:50.000000 openai_multi_client-0.1.0/setup.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-03 13:05:21.339974 openai_multi_client-0.1.1/
+-rw-r--r--   0 zh217      (501) staff       (20)     1065 2023-05-01 15:39:52.000000 openai_multi_client-0.1.1/LICENSE
+-rw-r--r--   0 zh217      (501) staff       (20)    22305 2023-05-03 13:05:21.339828 openai_multi_client-0.1.1/PKG-INFO
+-rw-r--r--   0 zh217      (501) staff       (20)    21970 2023-05-03 13:04:13.000000 openai_multi_client-0.1.1/README.md
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-03 13:05:21.338846 openai_multi_client-0.1.1/openai_multi_client/
+-rw-r--r--   0 zh217      (501) staff       (20)     8710 2023-05-03 09:42:59.000000 openai_multi_client-0.1.1/openai_multi_client/__init__.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-03 13:05:21.339617 openai_multi_client-0.1.1/openai_multi_client.egg-info/
+-rw-r--r--   0 zh217      (501) staff       (20)    22305 2023-05-03 13:05:21.000000 openai_multi_client-0.1.1/openai_multi_client.egg-info/PKG-INFO
+-rw-r--r--   0 zh217      (501) staff       (20)      287 2023-05-03 13:05:21.000000 openai_multi_client-0.1.1/openai_multi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 zh217      (501) staff       (20)        1 2023-05-03 13:05:21.000000 openai_multi_client-0.1.1/openai_multi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       30 2023-05-03 13:05:21.000000 openai_multi_client-0.1.1/openai_multi_client.egg-info/requires.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       20 2023-05-03 13:05:21.000000 openai_multi_client-0.1.1/openai_multi_client.egg-info/top_level.txt
+-rw-r--r--   0 zh217      (501) staff       (20)      528 2023-05-01 16:01:15.000000 openai_multi_client-0.1.1/pyproject.toml
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-03 13:05:21.340022 openai_multi_client-0.1.1/setup.cfg
+-rw-r--r--   0 zh217      (501) staff       (20)       37 2023-05-01 15:35:50.000000 openai_multi_client-0.1.1/setup.py
```

### Comparing `openai_multi_client-0.1.0/LICENSE` & `openai_multi_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_multi_client-0.1.0/openai_multi_client/__init__.py` & `openai_multi_client-0.1.1/openai_multi_client/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 import logging
 import asyncio
 from dataclasses import dataclass
 from threading import Thread
-from typing import Any
+from typing import Any, Optional
 
 from aioprocessing import AioJoinableQueue, AioQueue
 from tenacity import wait_random_exponential, stop_after_attempt, AsyncRetrying, RetryError
 import openai
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Payload:
     endpoint: str
     data: dict
-    metadata: dict | None
+    metadata: Optional[dict]
     max_retries: int
     retry_multiplier: float
     retry_max: float
     attempt: int = 0
     failed: bool = False
     response: Any = None
+    callback: Any = None
+
+    def call_callback(self):
+        if self.callback:
+            self.callback(self)
 
 
 class OpenAIMultiClient:
     def __init__(self,
                  concurrency: int = 10,
                  max_retries: int = 10,
                  wait_interval: float = 0,
                  retry_multiplier: float = 1,
                  retry_max: float = 60,
-                 endpoint: str | None = None,
-                 data_template: dict | None = None,
-                 metadata_template: dict | None = None,
+                 endpoint: Optional[str] = None,
+                 data_template: Optional[dict] = None,
+                 metadata_template: Optional[dict] = None,
                  custom_api=None):
         self._endpoint = endpoint
         self._wait_interval = wait_interval
         self._data_template = data_template or {}
         self._metadata_template = metadata_template or {}
         self._max_retries = max_retries
         self._retry_multiplier = retry_multiplier
@@ -130,33 +135,40 @@
     def __iter__(self):
         return self
 
     def __next__(self):
         out = self._out_queue.get()
         if out is None:
             raise StopIteration
+        out.call_callback()
         return out
 
     def request(self,
                 data: dict,
-                endpoint: str | None = None,
-                metadata: dict | None = None,
-                max_retries: int | None = None,
-                retry_multiplier: float | None = None,
-                retry_max: float | None = None):
+                endpoint: Optional[str] = None,
+                metadata: Optional[dict] = None,
+                callback: Any = None,
+                max_retries: Optional[int] = None,
+                retry_multiplier: Optional[float] = None,
+                retry_max: Optional[float] = None):
         payload = Payload(
             endpoint=endpoint or self._endpoint,
             data={**self._data_template, **data},
             metadata={**self._metadata_template, **(metadata or {})},
+            callback=callback,
             max_retries=max_retries or self._max_retries,
             retry_multiplier=retry_multiplier or self._retry_multiplier,
             retry_max=retry_max or self._retry_max
         )
         self._in_queue.put(payload)
 
+    def pull_all(self):
+        for _ in self:
+            pass
+
 
 class OrderedPayload(Payload):
     put_counter: int
 
     def __init__(self, *args, put_counter, **kwargs):
         super().__init__(*args, **kwargs)
         self.put_counter = put_counter
@@ -183,38 +195,43 @@
                 self._stopped = True
                 if self._get_counter == self._put_counter:
                     raise StopIteration
                 else:
                     out = self._get_cache[self._get_counter]
                     del self._get_cache[self._get_counter]
                     self._get_counter += 1
+                    out.call_callback()
                     return out
 
             data_counter = out.put_counter
             if data_counter == self._get_counter:
                 self._get_counter += 1
+                out.call_callback()
                 return out
             self._get_cache[data_counter] = out
             if self._get_counter in self._get_cache:
                 out = self._get_cache[self._get_counter]
                 del self._get_cache[self._get_counter]
                 self._get_counter += 1
+                out.call_callback()
                 return out
 
     def request(self,
                 data: dict,
-                endpoint: str | None = None,
-                metadata: dict | None = None,
-                max_retries: int | None = None,
-                retry_multiplier: float | None = None,
-                retry_max: float | None = None):
+                endpoint: Optional[str] = None,
+                metadata: Optional[dict] = None,
+                callback: Any = None,
+                max_retries: Optional[int] = None,
+                retry_multiplier: Optional[float] = None,
+                retry_max: Optional[float] = None):
         payload = OrderedPayload(
             endpoint=endpoint or self._endpoint,
             data={**self._data_template, **data},
             metadata={**self._metadata_template, **(metadata or {})},
+            callback=callback,
             max_retries=max_retries or self._max_retries,
             retry_multiplier=retry_multiplier or self._retry_multiplier,
             retry_max=retry_max or self._retry_max,
             put_counter=self._put_counter
         )
         self._put_counter += 1
         self._in_queue.put(payload)
```

### Comparing `openai_multi_client-0.1.0/pyproject.toml` & `openai_multi_client-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "openai",
     "tenacity",
     "aioprocessing",
 ]
-version = "0.1.0"
+version = "0.1.1"
```

