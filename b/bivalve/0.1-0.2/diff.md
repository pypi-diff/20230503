# Comparing `tmp/bivalve-0.1.tar.gz` & `tmp/bivalve-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bivalve-0.1.tar", last modified: Wed Feb 22 19:21:58 2023, max compression
+gzip compressed data, was "bivalve-0.2.tar", last modified: Wed May  3 07:11:32 2023, max compression
```

## Comparing `bivalve-0.1.tar` & `bivalve-0.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-02-22 19:21:58.386787 bivalve-0.1/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1636 2023-02-22 19:21:53.000000 bivalve-0.1/LICENSE
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1086 2023-02-22 19:21:58.386787 bivalve-0.1/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      434 2023-02-20 21:56:09.000000 bivalve-0.1/README.md
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-02-22 19:21:58.383454 bivalve-0.1/bivalve/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        0 2023-02-20 21:56:09.000000 bivalve-0.1/bivalve/__init__.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5208 2023-02-20 21:56:09.000000 bivalve-0.1/bivalve/agent.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2808 2023-02-20 21:56:09.000000 bivalve-0.1/bivalve/aio.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-02-22 19:21:58.386787 bivalve-0.1/bivalve/example/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        0 2023-02-20 21:56:09.000000 bivalve-0.1/bivalve/example/__init__.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2249 2023-02-20 21:56:09.000000 bivalve-0.1/bivalve/example/client.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1592 2023-02-20 21:56:09.000000 bivalve-0.1/bivalve/example/server.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2908 2023-02-20 21:56:09.000000 bivalve-0.1/bivalve/logging.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1634 2023-02-20 21:56:09.000000 bivalve-0.1/bivalve/nio.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1895 2023-02-20 21:56:09.000000 bivalve-0.1/bivalve/util.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-02-22 19:21:58.383454 bivalve-0.1/bivalve.egg-info/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1086 2023-02-22 19:21:58.000000 bivalve-0.1/bivalve.egg-info/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      332 2023-02-22 19:21:58.000000 bivalve-0.1/bivalve.egg-info/SOURCES.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-02-22 19:21:58.000000 bivalve-0.1/bivalve.egg-info/dependency_links.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        8 2023-02-22 19:21:58.000000 bivalve-0.1/bivalve.egg-info/top_level.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-02-22 19:21:58.386787 bivalve-0.1/setup.cfg
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1194 2023-02-22 19:21:07.000000 bivalve-0.1/setup.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 07:11:32.305411 bivalve-0.2/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1064 2023-05-03 07:11:32.302078 bivalve-0.2/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      434 2023-04-04 02:24:44.000000 bivalve-0.2/README.md
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 07:11:32.302078 bivalve-0.2/bivalve/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-04 02:24:44.000000 bivalve-0.2/bivalve/__init__.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5262 2023-05-03 07:07:36.000000 bivalve-0.2/bivalve/agent.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2847 2023-05-03 07:07:36.000000 bivalve-0.2/bivalve/aio.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 07:11:32.302078 bivalve-0.2/bivalve/example/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-04 02:24:44.000000 bivalve-0.2/bivalve/example/__init__.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2249 2023-05-03 07:05:37.000000 bivalve-0.2/bivalve/example/client.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1592 2023-04-04 02:24:44.000000 bivalve-0.2/bivalve/example/server.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2908 2023-04-04 02:24:44.000000 bivalve-0.2/bivalve/logging.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1634 2023-04-04 02:24:44.000000 bivalve-0.2/bivalve/nio.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1895 2023-04-04 02:24:44.000000 bivalve-0.2/bivalve/util.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 07:11:32.302078 bivalve-0.2/bivalve.egg-info/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1064 2023-05-03 07:11:32.000000 bivalve-0.2/bivalve.egg-info/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      324 2023-05-03 07:11:32.000000 bivalve-0.2/bivalve.egg-info/SOURCES.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-03 07:11:32.000000 bivalve-0.2/bivalve.egg-info/dependency_links.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        8 2023-05-03 07:11:32.000000 bivalve-0.2/bivalve.egg-info/top_level.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-03 07:11:32.305411 bivalve-0.2/setup.cfg
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1194 2023-05-03 07:11:27.000000 bivalve-0.2/setup.py
```

### Comparing `bivalve-0.1/PKG-INFO` & `bivalve-0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: bivalve
-Version: 0.1
+Version: 0.2
 Summary: A bi-directional shell-like socket protocol framework using asyncio.
 Home-page: https://github.com/lainproliant/bivalve
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: network sockets protocol shell
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Bivalve - Bi-Directional Shell Sockets
 This is a library implementing bi-directional shell sockets, a method of
 IPC where applications send and receive shell-formatted commands over
 simple TCP sockets.
 
 It also serves as an  example of asynchronous input handling while maintaining a
```

### Comparing `bivalve-0.1/bivalve/agent.py` & `bivalve-0.2/bivalve/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,23 +27,23 @@
         self.syn_timeout = timedelta(seconds=5)
         self.max_conns = 0  # no maximum connections
 
     @property
     def running(self) -> bool:
         return bool(self.connections or self.servers)
 
-    async def serve(self, host: str, port: int):
-        server = await Stream.start_server(self.on_client_connect, host, port)
+    async def serve(self, host: str, port: int, ssl=None):
+        server = await Stream.start_server(self.on_client_connect, host, port, ssl)
         self.servers.append(server)
-        log.info(f"Serving peers on {host}:{port}.")
+        log.info(f"Serving peers on {host}:{port} (ssl={ssl}).")
 
-    async def connect(self, host: str, port: int):
-        stream = await Stream.connect(host, port)
+    async def connect(self, host: str, port: int, ssl=None):
+        stream = await Stream.connect(host, port, ssl)
         conn = Connection(stream, asyncio.create_task(self.communicate(stream)))
-        log.info("Connected to peer on {host}:{port}.")
+        log.info("Connected to peer on {host}:{port} (ssl={ssl}).")
         self.connections[conn.id] = conn
 
     async def on_client_connect(self, stream: Stream):
         if self.max_conns and len(self.connections) >= self.max_conns:
             await stream.close()
             log.warning(
                 f"Maximum number of connections reached ({self.max_conns}), rejected connection."
```

### Comparing `bivalve-0.1/bivalve/aio.py` & `bivalve-0.2/bivalve/aio.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,40 +16,41 @@
 from uuid import UUID, uuid4
 
 from bivalve.logging import LogManager
 
 # --------------------------------------------------------------------
 log = LogManager().get(__name__)
 
+
 # --------------------------------------------------------------------
 @dataclass
 class Stream:
     ID = UUID
     reader: asyncio.StreamReader
     writer: asyncio.StreamWriter
     id: UUID = field(default_factory=uuid4)
 
     async def close(self):
         self.writer.close()
         await self.writer.wait_closed()
 
     @staticmethod
-    async def connect(host: str, port: int):
-        reader, writer = await asyncio.open_connection(host, port)
+    async def connect(host: str, port: int, ssl=None):
+        reader, writer = await asyncio.open_connection(host, port, ssl=ssl)
         return Stream(reader, writer)
 
     @staticmethod
-    async def start_server(callback, host: str, port: int):
+    async def start_server(callback, host: str, port: int, ssl=None):
         async def connected_callback(reader, writer):
             if inspect.iscoroutinefunction(callback):
                 await callback(Stream(reader, writer))
             else:
                 callback(Stream(reader, writer))
 
-        return await asyncio.start_server(connected_callback, host, port)
+        return await asyncio.start_server(connected_callback, host, port, ssl=ssl)
 
 
 # --------------------------------------------------------------------
 @dataclass
 class Connection:
     ID = Stream.ID
     stream: Stream
```

### Comparing `bivalve-0.1/bivalve/example/client.py` & `bivalve-0.2/bivalve/example/client.py`

 * *Files identical despite different names*

### Comparing `bivalve-0.1/bivalve/example/server.py` & `bivalve-0.2/bivalve/example/server.py`

 * *Files identical despite different names*

### Comparing `bivalve-0.1/bivalve/logging.py` & `bivalve-0.2/bivalve/logging.py`

 * *Files identical despite different names*

### Comparing `bivalve-0.1/bivalve/nio.py` & `bivalve-0.2/bivalve/nio.py`

 * *Files identical despite different names*

### Comparing `bivalve-0.1/bivalve/util.py` & `bivalve-0.2/bivalve/util.py`

 * *Files identical despite different names*

### Comparing `bivalve-0.1/bivalve.egg-info/PKG-INFO` & `bivalve-0.2/bivalve.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: bivalve
-Version: 0.1
+Version: 0.2
 Summary: A bi-directional shell-like socket protocol framework using asyncio.
 Home-page: https://github.com/lainproliant/bivalve
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: network sockets protocol shell
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Bivalve - Bi-Directional Shell Sockets
 This is a library implementing bi-directional shell sockets, a method of
 IPC where applications send and receive shell-formatted commands over
 simple TCP sockets.
 
 It also serves as an  example of asynchronous input handling while maintaining a
```

### Comparing `bivalve-0.1/setup.py` & `bivalve-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="bivalve",
-    version="0.1",
+    version="0.2",
     description="A bi-directional shell-like socket protocol framework using asyncio.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lainproliant/bivalve",
     author="Lain Musgrove (lainproliant)",
     author_email="lainproliant@gmail.com",
     license="BSD",
```

