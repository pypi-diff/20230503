# Comparing `tmp/netpackAIO-0.0.5.tar.gz` & `tmp/netpackAIO-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpackAIO-0.0.5.tar", last modified: Tue Apr 25 18:36:58 2023, max compression
+gzip compressed data, was "netpackAIO-0.0.6.tar", last modified: Wed May  3 21:14:15 2023, max compression
```

## Comparing `netpackAIO-0.0.5.tar` & `netpackAIO-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 18:36:58.071283 netpackAIO-0.0.5/
--rw-rw-rw-   0        0        0     1089 2023-04-14 20:36:26.000000 netpackAIO-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3405 2023-04-25 18:36:58.072286 netpackAIO-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2894 2023-04-20 20:36:34.000000 netpackAIO-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 18:36:58.035286 netpackAIO-0.0.5/netpack/
--rw-rw-rw-   0        0        0        0 2023-04-12 17:33:48.000000 netpackAIO-0.0.5/netpack/__init__.py
--rw-rw-rw-   0        0        0    11570 2023-04-25 17:06:55.000000 netpackAIO-0.0.5/netpack/func.py
--rw-rw-rw-   0        0        0      877 2023-04-25 17:10:17.000000 netpackAIO-0.0.5/netpack/test.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:36:58.069281 netpackAIO-0.0.5/netpackAIO.egg-info/
--rw-rw-rw-   0        0        0     3405 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 18:36:57.000000 netpackAIO-0.0.5/netpackAIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-25 18:36:58.078282 netpackAIO-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-04-25 18:36:55.000000 netpackAIO-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 21:14:15.780385 netpackAIO-0.0.6/
+-rw-rw-rw-   0        0        0     1089 2023-04-14 20:36:26.000000 netpackAIO-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3405 2023-05-03 21:14:15.780385 netpackAIO-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2894 2023-04-20 20:36:34.000000 netpackAIO-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 21:14:15.711952 netpackAIO-0.0.6/netpack/
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:33:48.000000 netpackAIO-0.0.6/netpack/__init__.py
+-rw-rw-rw-   0        0        0    12693 2023-05-02 23:39:50.000000 netpackAIO-0.0.6/netpack/func.py
+-rw-rw-rw-   0        0        0      275 2023-05-02 23:42:34.000000 netpackAIO-0.0.6/netpack/test.py
+drwxrwxrwx   0        0        0        0 2023-05-03 21:14:15.775657 netpackAIO-0.0.6/netpackAIO.egg-info/
+-rw-rw-rw-   0        0        0     3405 2023-05-03 21:14:15.000000 netpackAIO-0.0.6/netpackAIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-03 21:14:15.000000 netpackAIO-0.0.6/netpackAIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 21:14:15.000000 netpackAIO-0.0.6/netpackAIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-03 21:14:15.000000 netpackAIO-0.0.6/netpackAIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 21:14:15.000000 netpackAIO-0.0.6/netpackAIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-03 21:14:15.787421 netpackAIO-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-05-03 21:14:08.000000 netpackAIO-0.0.6/setup.py
```

### Comparing `netpackAIO-0.0.5/LICENSE` & `netpackAIO-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `netpackAIO-0.0.5/PKG-INFO` & `netpackAIO-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpackAIO
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package for performing network-related tasks
 Home-page: https://github.com/crusaderay/netpack
 Author: Dongjie Zhang
 Author-email: crusade.ray@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `netpackAIO-0.0.5/README.md` & `netpackAIO-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `netpackAIO-0.0.5/netpack/func.py` & `netpackAIO-0.0.6/netpack/func.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import threading
 
 from bs4 import BeautifulSoup
 import requests
 import ipaddress
 import socket
 import time
@@ -254,32 +255,49 @@
         elif protocol.lower() == "tcp":
             # Use TCP protocol for both IPv4 and IPv6
             return NetPack._tcp_ping(host, packet_size, interval, timeout, packet_num)
         else:
             # Raise an error if an unsupported protocol is given
             raise ValueError("Unsupported protocol. Please use 'icmp' or 'tcp'.")
 
+    # @staticmethod
+    # def multiple_ping(hosts, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5):
+    #     multiping_results = {}
+    #
+    #     # Define a function to ping a host and store the result in the results dictionary
+    #     def ping_host(host):
+    #         try:
+    #             latency, success_rate = NetPack.ping(host, packet_size, protocol, interval, timeout, packet_num)
+    #             multiping_results[host] = {'success_rate': success_rate, 'latency': latency}
+    #         except Exception as e:
+    #             print(e)
+    #             multiping_results[host] = {'success_rate': 0, 'latency': None}
+    #
+    #     # Create a thread for each host and start them all simultaneously
+    #     threads = []
+    #     for host in hosts:
+    #         t = threading.Thread(target=ping_host, args=(host,))
+    #         threads.append(t)
+    #         t.start()
+    #
+    #     # Wait for all threads to finish before returning the results dictionary
+    #     for t in threads:
+    #         t.join()
+    #
+    #     return multiping_results
     @staticmethod
-    def multiple_ping(hosts, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5):
-        multiping_results = {}
+    async def ping_async(host, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5):
+        # Call the ping function with the given arguments and return the result as a dictionary
+        latency, success_rate = await asyncio.to_thread(NetPack.ping, host, packet_size, protocol, interval, timeout,
+                                                        packet_num)
+        return {'success_rate': success_rate, 'latency': latency}
 
-        # Define a function to ping a host and store the result in the results dictionary
-        def ping_host(host):
-            try:
-                latency, success_rate = NetPack.ping(host, packet_size, protocol, interval, timeout, packet_num)
-                multiping_results[host] = {'success_rate': success_rate, 'latency': latency}
-            except Exception as e:
-                print(e)
-                multiping_results[host] = {'success_rate': 0, 'latency': None}
-
-        # Create a thread for each host and start them all simultaneously
-        threads = []
-        for host in hosts:
-            t = threading.Thread(target=ping_host, args=(host,))
-            threads.append(t)
-            t.start()
-
-        # Wait for all threads to finish before returning the results dictionary
-        for t in threads:
-            t.join()
+    @staticmethod
+    async def multiple_ping(hosts, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5):
+        # Create a list of tasks to ping each host
+        tasks = [NetPack.ping_async(host, packet_size, protocol, interval, timeout, packet_num) for host in hosts]
+
+        # Run the tasks concurrently and wait for all of them to finish
+        results = await asyncio.gather(*tasks)
 
-        return multiping_results
+        # Combine the results into a dictionary keyed by the host address
+        return {host: result for host, result in zip(hosts, results)}
```

### Comparing `netpackAIO-0.0.5/netpackAIO.egg-info/PKG-INFO` & `netpackAIO-0.0.6/netpackAIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpackAIO
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python package for performing network-related tasks
 Home-page: https://github.com/crusaderay/netpack
 Author: Dongjie Zhang
 Author-email: crusade.ray@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `netpackAIO-0.0.5/setup.py` & `netpackAIO-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='netpackAIO',
-    version='0.0.5',
+    version='0.0.6',
     description='A Python package for performing network-related tasks',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Dongjie Zhang',
     author_email='crusade.ray@gmail.com',
     url='https://github.com/crusaderay/netpack',
     packages=find_packages(),
```

