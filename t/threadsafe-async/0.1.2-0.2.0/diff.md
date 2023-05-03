# Comparing `tmp/threadsafe-async-0.1.2.tar.gz` & `tmp/threadsafe-async-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadsafe-async-0.1.2.tar", last modified: Wed Apr 19 19:11:38 2023, max compression
+gzip compressed data, was "threadsafe-async-0.2.0.tar", last modified: Wed May  3 10:28:43 2023, max compression
```

## Comparing `threadsafe-async-0.1.2.tar` & `threadsafe-async-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 19:11:38.956094 threadsafe-async-0.1.2/
--rw-r--r--   0 gleero     (501) staff       (20)     1076 2023-04-12 16:02:26.000000 threadsafe-async-0.1.2/LICENSE
--rw-r--r--   0 gleero     (501) staff       (20)     3821 2023-04-19 19:11:38.955798 threadsafe-async-0.1.2/PKG-INFO
--rw-r--r--   0 gleero     (501) staff       (20)     3157 2023-04-19 15:34:19.000000 threadsafe-async-0.1.2/README.md
--rw-r--r--   0 gleero     (501) staff       (20)     1415 2023-04-19 19:09:05.000000 threadsafe-async-0.1.2/pyproject.toml
--rw-r--r--   0 gleero     (501) staff       (20)       38 2023-04-19 19:11:38.956197 threadsafe-async-0.1.2/setup.cfg
-drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 19:11:38.949518 threadsafe-async-0.1.2/tests/
--rw-r--r--   0 gleero     (501) staff       (20)     6329 2023-04-19 19:00:13.000000 threadsafe-async-0.1.2/tests/test_channel.py
--rw-r--r--   0 gleero     (501) staff       (20)     4242 2023-04-19 19:06:37.000000 threadsafe-async-0.1.2/tests/test_event.py
-drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 19:11:38.952007 threadsafe-async-0.1.2/threadsafe_async.egg-info/
--rw-r--r--   0 gleero     (501) staff       (20)     3821 2023-04-19 19:11:38.000000 threadsafe-async-0.1.2/threadsafe_async.egg-info/PKG-INFO
--rw-r--r--   0 gleero     (501) staff       (20)      349 2023-04-19 19:11:38.000000 threadsafe-async-0.1.2/threadsafe_async.egg-info/SOURCES.txt
--rw-r--r--   0 gleero     (501) staff       (20)        1 2023-04-19 19:11:38.000000 threadsafe-async-0.1.2/threadsafe_async.egg-info/dependency_links.txt
--rw-r--r--   0 gleero     (501) staff       (20)      181 2023-04-19 19:11:38.000000 threadsafe-async-0.1.2/threadsafe_async.egg-info/requires.txt
--rw-r--r--   0 gleero     (501) staff       (20)        8 2023-04-19 19:11:38.000000 threadsafe-async-0.1.2/threadsafe_async.egg-info/top_level.txt
-drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-04-19 19:11:38.955058 threadsafe-async-0.1.2/tsasync/
--rw-r--r--   0 gleero     (501) staff       (20)       89 2023-04-18 15:51:38.000000 threadsafe-async-0.1.2/tsasync/__init__.py
--rw-r--r--   0 gleero     (501) staff       (20)     3089 2023-04-19 19:06:27.000000 threadsafe-async-0.1.2/tsasync/_channel.py
--rw-r--r--   0 gleero     (501) staff       (20)     3681 2023-04-19 17:37:59.000000 threadsafe-async-0.1.2/tsasync/_event.py
--rw-r--r--   0 gleero     (501) staff       (20)      405 2023-04-19 19:05:02.000000 threadsafe-async-0.1.2/tsasync/_utils.py
+drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-05-03 10:28:43.483805 threadsafe-async-0.2.0/
+-rw-r--r--   0 gleero     (501) staff       (20)     1076 2023-04-12 16:02:26.000000 threadsafe-async-0.2.0/LICENSE
+-rw-r--r--   0 gleero     (501) staff       (20)     4140 2023-05-03 10:28:43.483503 threadsafe-async-0.2.0/PKG-INFO
+-rw-r--r--   0 gleero     (501) staff       (20)     3157 2023-05-03 10:17:40.000000 threadsafe-async-0.2.0/README.md
+-rw-r--r--   0 gleero     (501) staff       (20)     1715 2023-05-03 10:26:54.000000 threadsafe-async-0.2.0/pyproject.toml
+-rw-r--r--   0 gleero     (501) staff       (20)       38 2023-05-03 10:28:43.483922 threadsafe-async-0.2.0/setup.cfg
+drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-05-03 10:28:43.479110 threadsafe-async-0.2.0/tests/
+-rw-r--r--   0 gleero     (501) staff       (20)     7538 2023-05-03 10:25:05.000000 threadsafe-async-0.2.0/tests/test_channel.py
+-rw-r--r--   0 gleero     (501) staff       (20)     4242 2023-04-19 19:06:37.000000 threadsafe-async-0.2.0/tests/test_event.py
+drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-05-03 10:28:43.481297 threadsafe-async-0.2.0/threadsafe_async.egg-info/
+-rw-r--r--   0 gleero     (501) staff       (20)     4140 2023-05-03 10:28:43.000000 threadsafe-async-0.2.0/threadsafe_async.egg-info/PKG-INFO
+-rw-r--r--   0 gleero     (501) staff       (20)      349 2023-05-03 10:28:43.000000 threadsafe-async-0.2.0/threadsafe_async.egg-info/SOURCES.txt
+-rw-r--r--   0 gleero     (501) staff       (20)        1 2023-05-03 10:28:43.000000 threadsafe-async-0.2.0/threadsafe_async.egg-info/dependency_links.txt
+-rw-r--r--   0 gleero     (501) staff       (20)      181 2023-05-03 10:28:43.000000 threadsafe-async-0.2.0/threadsafe_async.egg-info/requires.txt
+-rw-r--r--   0 gleero     (501) staff       (20)        8 2023-05-03 10:28:43.000000 threadsafe-async-0.2.0/threadsafe_async.egg-info/top_level.txt
+drwxr-xr-x   0 gleero     (501) staff       (20)        0 2023-05-03 10:28:43.482992 threadsafe-async-0.2.0/tsasync/
+-rw-r--r--   0 gleero     (501) staff       (20)       89 2023-04-18 15:51:38.000000 threadsafe-async-0.2.0/tsasync/__init__.py
+-rw-r--r--   0 gleero     (501) staff       (20)     3923 2023-05-03 10:01:29.000000 threadsafe-async-0.2.0/tsasync/_channel.py
+-rw-r--r--   0 gleero     (501) staff       (20)     3681 2023-04-19 17:37:59.000000 threadsafe-async-0.2.0/tsasync/_event.py
+-rw-r--r--   0 gleero     (501) staff       (20)      405 2023-04-19 19:05:02.000000 threadsafe-async-0.2.0/tsasync/_utils.py
```

### Comparing `threadsafe-async-0.1.2/LICENSE` & `threadsafe-async-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threadsafe-async-0.1.2/PKG-INFO` & `threadsafe-async-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: threadsafe-async
-Version: 0.1.2
+Version: 0.2.0
 Summary: Thread-safe synchronization primitives
 Author-email: Vladimir Perekladov <gleero@gmail.com>
+Project-URL: homepage, https://github.com/gleero/python-threadsafe-async
+Project-URL: documentation, https://github.com/gleero/python-threadsafe-async/blob/main/README.md
+Project-URL: changelog, https://github.com/gleero/python-threadsafe-async/blob/main/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # Asyncio ↔ Thread Synchronisation library
```

### Comparing `threadsafe-async-0.1.2/README.md` & `threadsafe-async-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `threadsafe-async-0.1.2/pyproject.toml` & `threadsafe-async-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "threadsafe-async"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
     {name = "Vladimir Perekladov", email = "gleero@gmail.com"},
 ]
 description = "Thread-safe synchronization primitives"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -12,14 +12,15 @@
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black==23.3.0",
     "flake8==6.0.0",
     "Flake8-pyproject==1.2.3",
@@ -30,14 +31,19 @@
 ]
 test = [
     "pytest==7.3.0",
     "pytest-asyncio==0.21.0",
     "pytest-cov==4.0.0",
 ]
 
+[project.urls]
+homepage = "https://github.com/gleero/python-threadsafe-async"
+documentation = "https://github.com/gleero/python-threadsafe-async/blob/main/README.md"
+changelog = "https://github.com/gleero/python-threadsafe-async/blob/main/CHANGELOG.md"
+
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.distutils.bdist_wheel]
 universal = true
```

### Comparing `threadsafe-async-0.1.2/tests/test_channel.py` & `threadsafe-async-0.2.0/tests/test_channel.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,34 +3,36 @@
 
 import pytest
 from utils import PropagatingThread, all_for_one
 
 from tsasync import Channel
 
 
-async def asender(ch: Channel[Optional[int]], data: list):
+async def asender(ch: Channel[Optional[int]], data: list, close: bool = False):
     for item in data:
         await ch.send(item)
-    await ch.send(None)
+    if close:
+        ch.close()
 
 
 async def areceiver(ch: Channel[int]) -> list:
     ret = []
     while True:
         item = await ch.receive()
         if item is None:
             break
         ret.append(item)
     return ret
 
 
-def ssender(ch: Channel[Optional[int]], data: list):
+def ssender(ch: Channel[Optional[int]], data: list, close: bool = False):
     for item in data:
         ch.send(item)
-    ch.send(None)
+    if close:
+        ch.close()
 
 
 def sreceiver(ch: Channel[int]) -> list:
     ret = []
     while True:
         item = ch.receive()
         if item is None:
@@ -38,15 +40,15 @@
         ret.append(item)
     return ret
 
 
 @pytest.mark.asyncio
 async def test_channel_between_async_and_coroutine_sender():
     channel = Channel[Optional[int]]()
-    sender_task = asyncio.create_task(asender(channel, [1, 2, 3, 4, 5]))
+    sender_task = asyncio.create_task(asender(channel, [1, 2, 3, 4, 5], close=True))
     result = []
     while True:
         item = await channel.receive()
         if item is None:
             break
         result.append(item)
     await sender_task
@@ -56,24 +58,20 @@
 @pytest.mark.asyncio
 async def test_channel_between_async_and_many_coroutine_senders():
     channel = Channel[Optional[int]]()
     senders = []
     for x in range(5):
         senders.append(asyncio.create_task(asender(channel, [1, 2])))
     result = []
-    cnt = 0
-    while True:
+    for x in range(10):
         item = await channel.receive()
-        if item is None:
-            cnt += 1
-        else:
-            result.append(item)
-        if cnt == 5:
-            break
+        result.append(item)
     await asyncio.gather(*senders)
+    channel.close()
+    assert await channel.receive() is None
     assert len(result) == 10
 
 
 @pytest.mark.asyncio
 async def test_channel_between_async_and_many_mixed_senders():
     channel = Channel[Optional[int]]()
     senders_coro = []
@@ -81,102 +79,98 @@
     for x in range(5):
         senders_coro.append(asyncio.create_task(asender(channel, [1, 2])))
         t = PropagatingThread(target=ssender, args=(channel, [3, 4]))
         t.start()
         senders_threads.append(t)
 
     result = []
-    cnt = 0
-    while True:
+    for x in range(20):
         item = await channel.receive()
-        if item is None:
-            cnt += 1
-        else:
-            result.append(item)
-        if cnt == 10:
-            break
+        result.append(item)
     await asyncio.gather(*senders_coro)
     for t in senders_threads:
         t.join()
+    channel.close()
+    assert await channel.receive() is None
     assert len(result) == 20
 
 
 @pytest.mark.asyncio
 async def test_channel_between_async_and_coroutine_receiver():
     channel = Channel[Optional[int]]()
     receiver_task = asyncio.create_task(areceiver(channel))
     for item in [1, 2, 3, 4, 5]:
         await channel.send(item)
-    await channel.send(None)
+    channel.close()
     result = await receiver_task
     assert result == [1, 2, 3, 4, 5]
 
 
 @pytest.mark.asyncio
 async def test_channel_between_async_and_many_coroutine_receivers():
     channel = Channel[Optional[int]]()
     receivers = []
-    rcv_count = 7
-    for x in range(rcv_count):
+    for x in range(7):
         receivers.append(asyncio.create_task(areceiver(channel)))
     for item in list(range(50)):
         await channel.send(item)
-    for x in range(rcv_count):
-        await channel.send(None)
+    channel.close()
     result = list(all_for_one(await asyncio.gather(*receivers)))
     assert sorted(result) == list(range(50))
 
 
 @pytest.mark.asyncio
 async def test_channel_between_async_and_many_mixed_receivers():
     channel = Channel[Optional[int]]()
     receivers_coro = []
     receivers_threads = []
-    rcv_count = 7
-    for x in range(rcv_count):
+    for x in range(7):
         receivers_coro.append(asyncio.create_task(areceiver(channel)))
         t = PropagatingThread(target=sreceiver, args=(channel,))
         t.start()
         receivers_threads.append(t)
     for item in list(range(100)):
         await channel.send(item)
-    for x in range(rcv_count * 2):
-        await channel.send(None)
+    channel.close()
     result = list(all_for_one(await asyncio.gather(*receivers_coro)))
     for t in receivers_threads:
         t.join()
         result += t.ret
     assert sorted(result) == list(range(100))
 
 
 @pytest.mark.asyncio
 async def test_channel_between_two_coroutines():
     channel = Channel[Optional[int]]()
-    sender_task = asyncio.create_task(asender(channel, [1, 2, 3, 4, 5]))
+    sender_task = asyncio.create_task(asender(channel, [1, 2, 3, 4, 5], close=True))
     receiver_task = asyncio.create_task(areceiver(channel))
     await sender_task
     result = await receiver_task
     assert result == [1, 2, 3, 4, 5]
 
 
 def test_channel_between_two_threads():
     channel = Channel[Optional[int]]()
-    sender_thread = PropagatingThread(target=ssender, args=(channel, [1, 2, 3, 4, 5]))
+    sender_thread = PropagatingThread(
+        target=ssender, args=(channel, [1, 2, 3, 4, 5], True)
+    )
     sender_thread.start()
     receiver_thread = PropagatingThread(target=sreceiver, args=(channel,))
     receiver_thread.start()
     sender_thread.join()
     receiver_thread.join()
     assert receiver_thread.ret == [1, 2, 3, 4, 5]
 
 
 def test_channel_between_sync_and_thread_sender():
     channel = Channel[Optional[int]]()
     result = []
-    sender_thread = PropagatingThread(target=ssender, args=(channel, [1, 2, 3, 4, 5]))
+    sender_thread = PropagatingThread(
+        target=ssender, args=(channel, [1, 2, 3, 4, 5], True)
+    )
     sender_thread.start()
     while True:
         item = channel.receive()
         if item is None:
             break
         result.append(item)
     sender_thread.join()
@@ -185,24 +179,26 @@
 
 def test_channel_between_sync_and_thread_receiver():
     channel = Channel[Optional[int]]()
     receiver_thread = PropagatingThread(target=sreceiver, args=(channel,))
     receiver_thread.start()
     for item in [1, 2, 3, 4, 5]:
         channel.send(item)
-    channel.send(None)
+    channel.close()
     receiver_thread.join()
     assert receiver_thread.ret == [1, 2, 3, 4, 5]
 
 
 @pytest.mark.asyncio
 async def test_channel_between_async_and_thread_sender():
     channel = Channel[Optional[int]]()
     result = []
-    sender_thread = PropagatingThread(target=ssender, args=(channel, [1, 2, 3, 4, 5]))
+    sender_thread = PropagatingThread(
+        target=ssender, args=(channel, [1, 2, 3, 4, 5], True)
+    )
     sender_thread.start()
     while True:
         item = await channel.receive()
         if item is None:
             break
         result.append(item)
     sender_thread.join()
@@ -212,10 +208,60 @@
 @pytest.mark.asyncio
 async def test_channel_between_async_and_thread_receiver():
     channel = Channel[Optional[int]]()
     receiver_thread = PropagatingThread(target=sreceiver, args=(channel,))
     receiver_thread.start()
     for item in [1, 2, 3, 4, 5]:
         await channel.send(item)
-    await channel.send(None)
+    channel.close()
     receiver_thread.join()
     assert receiver_thread.ret == [1, 2, 3, 4, 5]
+
+
+def test_channel_not_closed():
+    channel = Channel[Optional[int]]()
+    assert channel.closed is False
+
+
+def test_channel_closed():
+    channel = Channel[Optional[int]]()
+    channel.close()
+    assert channel.closed is True
+
+
+def test_channel_send_if_closed():
+    channel = Channel[Optional[int]]()
+    channel.close()
+    with pytest.raises(IOError):
+        channel.send(1)
+
+
+def test_channel_send_none():
+    channel = Channel[Optional[int]]()
+    with pytest.raises(ValueError):
+        channel.send(None)
+
+
+@pytest.mark.asyncio
+async def test_channel_close_buffered_read():
+    channel = Channel[Optional[int]](buffered=100)
+    for x in range(10):
+        await channel.send(x)
+    channel.close()
+    for x in range(10):
+        assert await channel.receive() == x
+    assert await channel.receive() is None
+
+
+@pytest.mark.asyncio
+async def test_channel_close_many_mixed_pending_receive():
+    channel = Channel[Optional[int]]()
+    receivers_coros = []
+    receivers_threads = []
+    for x in range(10):
+        receivers_coros.append(asyncio.create_task(areceiver(channel)))
+        receiver_thread = PropagatingThread(target=sreceiver, args=(channel,))
+        receiver_thread.start()
+    channel.close()
+    await asyncio.gather(*receivers_coros)
+    for t in receivers_threads:
+        t.join()
```

### Comparing `threadsafe-async-0.1.2/tests/test_event.py` & `threadsafe-async-0.2.0/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `threadsafe-async-0.1.2/threadsafe_async.egg-info/PKG-INFO` & `threadsafe-async-0.2.0/threadsafe_async.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: threadsafe-async
-Version: 0.1.2
+Version: 0.2.0
 Summary: Thread-safe synchronization primitives
 Author-email: Vladimir Perekladov <gleero@gmail.com>
+Project-URL: homepage, https://github.com/gleero/python-threadsafe-async
+Project-URL: documentation, https://github.com/gleero/python-threadsafe-async/blob/main/README.md
+Project-URL: changelog, https://github.com/gleero/python-threadsafe-async/blob/main/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # Asyncio ↔ Thread Synchronisation library
```

### Comparing `threadsafe-async-0.1.2/tsasync/_channel.py` & `threadsafe-async-0.2.0/tsasync/_channel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 import inspect
 import threading
 from collections import deque
 from dataclasses import dataclass
-from enum import Enum
 from typing import Any, Awaitable, Deque, Generic, Optional, Union
 
 from ._event import Event
 from ._utils import T, in_loop, wrapret
 
 
-class ChannelState(Enum):
-    IDLE = 1
-
-
 @dataclass
 class OperationContext:
     event: Event
     value: Any
     destination: Optional[Event] = None
 
 
 class Channel(Generic[T]):
     _ts_lock: threading.RLock
     _queue: Deque[OperationContext]
     _waiters: Deque[Event]
     _max_size: int
+    _is_closed: bool
+
+    @property
+    def closed(self) -> bool:
+        with self._ts_lock:
+            return self._is_closed
 
     def __init__(self, buffered: int = 0):
         """
         Create a new channel
         """
         self._ts_lock = threading.RLock()
         self._queue = deque()
         self._waiters = deque()
         self._max_size = buffered
+        self._is_closed = False
 
     def send(self, value: T) -> Union[Awaitable, None]:
         """
         Send any object to the channel.
         This method locks main thread until receive fired.
         :param value: any object
         """
-        ctx = OperationContext(event=Event(), value=value)
+        if value is None:
+            raise ValueError("None is not allowed")
 
         with self._ts_lock:
+            if self._is_closed:
+                raise IOError("Channel is closed")
+
+            ctx = OperationContext(event=Event(), value=value)
+
             # No need to wait because enought buffered slots
             if len(self._queue) < self._max_size:
                 ctx.event.set()
 
             # Put item to the queue
             self._queue.append(ctx)
 
@@ -75,40 +83,60 @@
         Get item from the queue
         """
         with self._ts_lock:
             # Queue has pending objects, return it immediately
             if len(self._queue) > 0 and len(self._waiters) == 0:
                 return wrapret(self._next_item())
 
+            if self._is_closed:
+                return wrapret(None)
+
             # Create event and wait for data
             event = Event()
             self._waiters.append(event)
 
         # Wait for event
         if in_loop():
             return self._areceive(event)
 
         # Get item from the queue
         event.wait()
+        return self._next_item(event)
+
+    def close(self):
+        """
+        Close the channel.
+        All buffered items will be passed.
+        """
         with self._ts_lock:
-            return self._next_item(event)
+            self._is_closed = True
+
+            # Unlock for waiter in needed
+            while len(self._waiters) > 0:
+                try:
+                    event = self._waiters.popleft()
+                    event.set()
+                except IndexError:
+                    pass
 
     async def _areceive(self, event: Event) -> T:
         """
         Receive item asynchronly
         :param event: event instance
         """
         waiter = event.wait()
         if inspect.isawaitable(waiter):
             await waiter
-        with self._ts_lock:
-            return self._next_item(event)
+        return self._next_item(event)
 
     def _next_item(self, event: Optional[Event] = None) -> T:
         """
         Get next item from the queue
         """
-        ctx = self._queue.popleft()
-        if ctx.destination is not None:
-            assert ctx.destination == event, f"{ctx.destination} != {event}"
-        ctx.event.set()
-        return ctx.value
+        with self._ts_lock:
+            if self._is_closed and len(self._queue) == 0:
+                return None
+            ctx = self._queue.popleft()
+            if ctx.destination is not None:
+                assert ctx.destination == event, f"{ctx.destination} != {event}"
+            ctx.event.set()
+            return ctx.value
```

### Comparing `threadsafe-async-0.1.2/tsasync/_event.py` & `threadsafe-async-0.2.0/tsasync/_event.py`

 * *Files identical despite different names*

