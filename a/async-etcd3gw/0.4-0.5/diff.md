# Comparing `tmp/async_etcd3gw-0.4.tar.gz` & `tmp/async_etcd3gw-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_etcd3gw-0.4.tar", last modified: Fri Apr 21 20:57:10 2023, max compression
+gzip compressed data, was "async_etcd3gw-0.5.tar", last modified: Wed May  3 06:51:57 2023, max compression
```

## Comparing `async_etcd3gw-0.4.tar` & `async_etcd3gw-0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:57:10.866848 async_etcd3gw-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-21 20:57:10.866848 async_etcd3gw-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:57:10.862848 async_etcd3gw-0.4/async_etcd3gw/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/async_lease.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/async_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/async_watch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:57:10.866848 async_etcd3gw-0.4/async_etcd3gw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-21 20:57:10.000000 async_etcd3gw-0.4/async_etcd3gw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-21 20:57:10.000000 async_etcd3gw-0.4/async_etcd3gw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:57:10.000000 async_etcd3gw-0.4/async_etcd3gw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 20:57:10.000000 async_etcd3gw-0.4/async_etcd3gw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 20:57:10.000000 async_etcd3gw-0.4/async_etcd3gw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:57:10.000000 async_etcd3gw-0.4/async_etcd3gw.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-21 20:57:10.866848 async_etcd3gw-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:57:10.866848 async_etcd3gw-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/tests/test_async_etcd3gw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:57.423133 async_etcd3gw-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-03 06:51:57.423133 async_etcd3gw-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:57.419133 async_etcd3gw-0.5/async_etcd3gw/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/async_lease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/async_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/async_watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/async_etcd3gw/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:57.423133 async_etcd3gw-0.5/async_etcd3gw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-03 06:51:57.000000 async_etcd3gw-0.5/async_etcd3gw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 06:51:57.000000 async_etcd3gw-0.5/async_etcd3gw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:51:57.000000 async_etcd3gw-0.5/async_etcd3gw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 06:51:57.000000 async_etcd3gw-0.5/async_etcd3gw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 06:51:57.000000 async_etcd3gw-0.5/async_etcd3gw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:51:57.000000 async_etcd3gw-0.5/async_etcd3gw.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-03 06:51:57.423133 async_etcd3gw-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:51:57.423133 async_etcd3gw-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/tests/test_async_etcd3gw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-03 06:51:30.000000 async_etcd3gw-0.5/tests/test_client.py
```

### Comparing `async_etcd3gw-0.4/LICENSE` & `async_etcd3gw-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.4/PKG-INFO` & `async_etcd3gw-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_etcd3gw
-Version: 0.4
+Version: 0.5
 Summary: An async Python client for etcd3 grpc-gateway v3 API
 Home-page: https://github.com/DLBD-Department/async_etcd3gw
 Author: Alkemy spa
 Author-email: DLBDDepartment@alkemy.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DLBD-Department/async_etcd3gw/issues
 Project-URL: Source Code, https://github.com/DLBD-Department/async_etcd3gw
```

### Comparing `async_etcd3gw-0.4/README.md` & `async_etcd3gw-0.5/README.md`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.4/async_etcd3gw/__init__.py` & `async_etcd3gw-0.5/async_etcd3gw/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #    https://opendev.org/openstack/etcd3gw/src/tag/2.1.0/etcd3gw/__init__.py
 
 from . import utils
 from .async_client import AsyncEtcd3Client, async_client
 from .async_lease import AsyncLease
 from .async_lock import AsyncLock
 
-__version__ = "0.4"
+__version__ = "0.5"
 
 __all__ = (
     "AsyncEtcd3Client",
     "AsyncLease",
     "AsyncLock",
     "async_client",
     "utils",
```

### Comparing `async_etcd3gw-0.4/async_etcd3gw/async_client.py` & `async_etcd3gw-0.5/async_etcd3gw/async_client.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.4/async_etcd3gw/async_lease.py` & `async_etcd3gw-0.5/async_etcd3gw/async_lease.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.4/async_etcd3gw/async_lock.py` & `async_etcd3gw-0.5/async_etcd3gw/async_lock.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.4/async_etcd3gw/async_watch.py` & `async_etcd3gw-0.5/async_etcd3gw/async_watch.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,11 +64,28 @@
             for event in payload["result"]["events"]:
                 event["kv"]["key"] = _decode(event["kv"]["key"])
                 if "value" in event["kv"]:
                     event["kv"]["value"] = _decode(event["kv"]["value"])
                 await self.callback(event)
 
     async def watch(self):
-        async with aiohttp.ClientSession(**self.async_client.client_session_kwargs) as session:
-            async with session.post(self.async_client.get_url("/watch"), json=self.create_request) as resp:
-                async for data in resp.content.iter_any():
-                    await self.process_chunk(data)
+        try:
+            # Set timeout
+            kwargs = dict(self.async_client.client_session_kwargs)
+            timeout = aiohttp.ClientTimeout(total=None, sock_read=None)
+            kwargs["timeout"] = timeout
+            async with aiohttp.ClientSession(**kwargs) as session:
+                async with session.post(self.async_client.get_url("/watch"), json=self.create_request) as resp:
+                    await self.read_and_process_chunk(resp.content)
+        except Exception:
+            await self.callback(None)
+
+    async def read_and_process_chunk(self, content):
+        while True:
+            if content._exception is not None:
+                raise content._exception
+
+            if not content._buffer and not content._eof:
+                await content._wait("readany")
+
+            data = content._read_nowait(-1)
+            await self.process_chunk(data)
```

### Comparing `async_etcd3gw-0.4/async_etcd3gw/exceptions.py` & `async_etcd3gw-0.5/async_etcd3gw/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.4/async_etcd3gw/utils.py` & `async_etcd3gw-0.5/async_etcd3gw/utils.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.4/async_etcd3gw.egg-info/PKG-INFO` & `async_etcd3gw-0.5/async_etcd3gw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-etcd3gw
-Version: 0.4
+Version: 0.5
 Summary: An async Python client for etcd3 grpc-gateway v3 API
 Home-page: https://github.com/DLBD-Department/async_etcd3gw
 Author: Alkemy spa
 Author-email: DLBDDepartment@alkemy.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DLBD-Department/async_etcd3gw/issues
 Project-URL: Source Code, https://github.com/DLBD-Department/async_etcd3gw
```

### Comparing `async_etcd3gw-0.4/setup.cfg` & `async_etcd3gw-0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.4/tests/test_async_etcd3gw.py` & `async_etcd3gw-0.5/tests/test_async_etcd3gw.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,43 +14,45 @@
 import os
 import uuid
 from time import perf_counter
 
 import pytest
 
 from async_etcd3gw import exceptions, utils, AsyncEtcd3Client
+from async_etcd3gw.async_client import DEFAULT_API_PATH
 
 ETCD_HOST = os.environ.get("ETCD_HOST", "localhost")
+API_PATH = os.environ.get("API_PATH", DEFAULT_API_PATH)
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_status():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     response = await client.status()
     assert response is not None
     assert "version" in response
     assert "header" in response
     assert "cluster_id" in response["header"]
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_members():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     response = await client.members()
     assert len(response) > 0
     assert "clientURLs" in response[0]
     assert "peerURLs" in response[0]
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_with_keys_and_values():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     assert await client.put("foo0", "bar0")
     assert await client.put("foo1", 2001)
     assert await client.put("foo2", b"bar2")
 
     assert [b"bar0"] == await client.get("foo0")
     assert [b"2001"] == await client.get("foo1")
     assert [b"bar2"] == await client.get("foo2")
@@ -61,15 +63,15 @@
     assert not await client.delete("foo0")
     assert len(await client.get_all()) > 0
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_get_and_delete_prefix():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     for i in range(20):
         await client.put(f"/doot1/range{i}", "i am a range")
 
     values = list(await client.get_prefix("/doot1/range"))
     assert len(values) == 20
     for value, metadata in values:
         assert b"i am a range" == value
@@ -79,15 +81,15 @@
     values = list(await client.get_prefix("/doot1/range"))
     assert len(values) == 0
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_get_prefix_sort_order():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
 
     def remove_prefix(string, prefix):
         return string[len(prefix) :]
 
     initial_keys = "abcde"
     initial_values = "qwert"
 
@@ -106,15 +108,15 @@
 
     assert reverse_keys == "".join(reversed(initial_keys)).encode("latin-1")
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_get_prefix_sort_order_explicit_sort_target_key():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
 
     def remove_prefix(string, prefix):
         return string[len(prefix) :]
 
     initial_keys_ordered = "abcde"
     initial_keys = "aebdc"
     initial_values = "qwert"
@@ -134,15 +136,15 @@
 
     assert reverse_keys == "".join(reversed(initial_keys_ordered)).encode("latin-1")
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_get_prefix_sort_order_explicit_sort_target_rev():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
 
     def remove_prefix(string, prefix):
         return string[len(prefix) :]
 
     initial_keys = "aebdc"
     initial_values = "qwert"
 
@@ -161,39 +163,39 @@
 
     assert reverse_keys == "".join(reversed(initial_keys)).encode("latin-1")
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_replace_success():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/doot/thing" + str(uuid.uuid4())
     await client.put(key, "toot")
     status = await client.replace(key, "toot", "doot")
     v = await client.get(key)
     assert [b"doot"] == v
     assert status
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_replace_fail():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/doot/thing" + str(uuid.uuid4())
     await client.put(key, "boot")
     status = await client.replace(key, "toot", "doot")
     v = await client.get(key)
     assert [b"boot"] == v
     assert not status
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_lease():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     lease = await client.lease(ttl=60)
     assert lease is not None
 
     ttl = await lease.ttl()
     assert 0 <= ttl <= 60
 
     keys = await lease.keys()
@@ -204,15 +206,15 @@
 
     assert await lease.revoke()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_lease_with_keys():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     lease = await client.lease(ttl=60)
     assert lease is not None
 
     assert await client.put("foo12", "bar12", lease)
     assert await client.put("foo13", "bar13", lease)
 
     keys = await lease.keys()
@@ -225,15 +227,15 @@
 
     assert await lease.revoke()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_watch_key():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/%s-watch_key/watch" % str(uuid.uuid4())
 
     async def update_etcd(v):
         await client.put(key, v)
         out = await client.get(key)
         assert [v.encode("latin-1")] == out
 
@@ -267,15 +269,15 @@
 
     await t
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_watch_prefix():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/%s-watch_prefix/watch/prefix/" % str(uuid.uuid4())
 
     async def update_etcd(v):
         await client.put(key + v, v)
         out = await client.get(key + v)
         assert [v.encode("latin-1")] == out
 
@@ -311,15 +313,15 @@
 
     await t
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_sequential_watch_prefix_once():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     try:
         await client.watch_prefix_once("/doot/", 1)
     except exceptions.WatchTimedOut:
         pass
     try:
         await client.watch_prefix_once("/doot/", 1)
     except exceptions.WatchTimedOut:
@@ -329,28 +331,28 @@
     except exceptions.WatchTimedOut:
         pass
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_lock_acquire_release():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     async with await client.lock(ttl=60) as lock:
         ttl = await lock.refresh()
         assert 0 <= ttl <= 60
     assert not await lock.is_acquired()
 
     async with await client.lock(ttl=60) as lock:
         assert not await lock.acquire()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_locks():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     lock = await client.lock(id="xyz-%s" % perf_counter(), ttl=60)
     assert lock is not None
 
     assert await lock.acquire()
     assert lock.uuid is not None
 
     ttl = await lock.refresh()
@@ -361,44 +363,44 @@
     assert not await lock.release()
     assert not await lock.is_acquired()
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_create_success():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/foo/unique" + str(uuid.uuid4())
     # Verify that key is empty
     assert [] == await client.get(key)
 
     status = await client.create(key, "bar")
     # Verify that key is 'bar'
     assert [b"bar"] == await client.get(key)
     assert status
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_create_fail():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/foo/" + str(uuid.uuid4())
     # Assign value to the key
     await client.put(key, "bar")
     assert [b"bar"] == await client.get(key)
 
     status = await client.create(key, "goo")
     # Verify that key is still 'bar'
     assert [b"bar"] == await client.get(key)
     assert not status
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_create_with_lease_success():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     key = "/foo/unique" + str(uuid.uuid4())
     # Verify that key is empty
     assert [] == await client.get(key)
     lease = await client.lease()
 
     status = await client.create(key, "bar", lease=lease)
     # Verify that key is 'bar'
@@ -415,27 +417,27 @@
         payload["value"] = utils._encode(key_name)
     await client.post(client.get_url("/kv/put"), json=payload)
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_keys_with_metadata_and_value():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     test_key_value = b"some_key"
     await _post_key(client, test_key_value)
     result = await client.get(test_key_value, metadata=True)
     assert len(result) > 0
     value, metadata = result[0]
     assert value == test_key_value
 
 
 @pytest.mark.etcd
 @pytest.mark.asyncio
 async def test_client_keys_with_metadata_and_no_value():
-    client = AsyncEtcd3Client(host=ETCD_HOST)
+    client = AsyncEtcd3Client(host=ETCD_HOST, api_path=API_PATH)
     value_is_not_set_default = b""
     test_key = b"some_key"
     await _post_key(client, test_key, provide_value=False)
     result = await client.get(test_key, metadata=True)
     assert len(result) > 0
     value, metadata = result[0]
     assert value == value_is_not_set_default
```

### Comparing `async_etcd3gw-0.4/tests/test_client.py` & `async_etcd3gw-0.5/tests/test_client.py`

 * *Files identical despite different names*

