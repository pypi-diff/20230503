# Comparing `tmp/dtn7zero-0.0.5.tar.gz` & `tmp/dtn7zero-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Data\Benutzer\Lukas\PyCharmProjects\dtn7zero\dist\.tmp-5f_zb515\dtn7zero-0.0.5.tar", last modified: Fri Apr 28 23:19:10 2023, max compression
+gzip compressed data, was "D:\Data\Benutzer\Lukas\PyCharmProjects\dtn7zero\dist\.tmp-xjrmxvmo\dtn7zero-0.0.6.tar", last modified: Wed May  3 14:39:49 2023, max compression
```

## Comparing `dtn7zero-0.0.5.tar` & `dtn7zero-0.0.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/
--rw-rw-rw-   0        0        0    35184 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/LICENSE
--rw-rw-rw-   0        0        0    10080 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     9755 2023-04-28 23:14:49.000000 dtn7zero-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero/
--rw-rw-rw-   0        0        0      261 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/__init__.py
--rw-rw-rw-   0        0        0     9731 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/api.py
--rw-rw-rw-   0        0        0    21246 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/bundle_protocol_agent.py
--rw-rw-rw-   0        0        0     1506 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/
--rw-rw-rw-   0        0        0      615 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/__init__.py
--rw-rw-rw-   0        0        0     3282 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py
--rw-rw-rw-   0        0        0    13077 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/mtcp.py
--rw-rw-rw-   0        0        0     2435 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/data.py
--rw-rw-rw-   0        0        0     7598 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/endpoints.py
--rw-rw-rw-   0        0        0    13381 2023-04-28 22:59:08.000000 dtn7zero-0.0.5/dtn7zero/ipnd.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero/routers/
--rw-rw-rw-   0        0        0     3128 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/routers/__init__.py
--rw-rw-rw-   0        0        0     4380 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/routers/simple_epidemic_router.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero/storage/
--rw-rw-rw-   0        0        0     1402 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/storage/__init__.py
--rw-rw-rw-   0        0        0     2941 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/storage/simple_in_memory_storage.py
--rw-rw-rw-   0        0        0     4307 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/dtn7zero/utility.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero.egg-info/
--rw-rw-rw-   0        0        0    10080 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/dtn7zero.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      644 2023-04-28 23:18:36.000000 dtn7zero-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 23:19:10.000000 dtn7zero-0.0.5/test/
--rw-rw-rw-   0        0        0      956 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-api-background.py
--rw-rw-rw-   0        0        0      694 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-api-ping.py
--rw-rw-rw-   0        0        0      563 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-api-pong.py
--rw-rw-rw-   0        0        0      899 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-api-synchronous.py
--rw-rw-rw-   0        0        0     1944 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-bundle-protocol-agent-receiver.py
--rw-rw-rw-   0        0        0     2095 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-bundle-protocol-agent-sender.py
--rw-rw-rw-   0        0        0     1443 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-bundle-protocol-agent.py
--rw-rw-rw-   0        0        0     1711 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-bundle-serialization.py
--rw-rw-rw-   0        0        0    15498 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-bundle-size.py
--rw-rw-rw-   0        0        0     1688 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-dtn7rs-rest-cla.py
--rw-rw-rw-   0        0        0     1236 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-ipnd.py
--rw-rw-rw-   0        0        0     2028 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-mtcp-intermediate.py
--rw-rw-rw-   0        0        0     2260 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-mtcp-receiver.py
--rw-rw-rw-   0        0        0     2563 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-mtcp-sender.py
--rw-rw-rw-   0        0        0     5282 2023-04-28 22:29:12.000000 dtn7zero-0.0.5/test/test-py-dtn7-functionality.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/
+-rw-rw-rw-   0        0        0    35184 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0    10080 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9755 2023-04-28 23:14:49.000000 dtn7zero-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero/
+-rw-rw-rw-   0        0        0      261 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/__init__.py
+-rw-rw-rw-   0        0        0     9731 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/api.py
+-rw-rw-rw-   0        0        0    21246 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/bundle_protocol_agent.py
+-rw-rw-rw-   0        0        0     1506 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/
+-rw-rw-rw-   0        0        0      615 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/__init__.py
+-rw-rw-rw-   0        0        0     3282 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py
+-rw-rw-rw-   0        0        0    13077 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/mtcp.py
+-rw-rw-rw-   0        0        0     2435 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/data.py
+-rw-rw-rw-   0        0        0     7598 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/endpoints.py
+-rw-rw-rw-   0        0        0    13482 2023-05-03 14:33:51.000000 dtn7zero-0.0.6/dtn7zero/ipnd.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero/routers/
+-rw-rw-rw-   0        0        0     3128 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/routers/__init__.py
+-rw-rw-rw-   0        0        0     4380 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/routers/simple_epidemic_router.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero/storage/
+-rw-rw-rw-   0        0        0     1402 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/storage/__init__.py
+-rw-rw-rw-   0        0        0     2941 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/dtn7zero/storage/simple_in_memory_storage.py
+-rw-rw-rw-   0        0        0     4715 2023-05-03 14:30:38.000000 dtn7zero-0.0.6/dtn7zero/utility.py
+drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero.egg-info/
+-rw-rw-rw-   0        0        0    10080 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1095 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/dtn7zero.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      654 2023-05-03 13:35:28.000000 dtn7zero-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 14:39:49.000000 dtn7zero-0.0.6/test/
+-rw-rw-rw-   0        0        0      956 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-api-background.py
+-rw-rw-rw-   0        0        0      694 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-api-ping.py
+-rw-rw-rw-   0        0        0      563 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-api-pong.py
+-rw-rw-rw-   0        0        0      899 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-api-synchronous.py
+-rw-rw-rw-   0        0        0     1944 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-bundle-protocol-agent-receiver.py
+-rw-rw-rw-   0        0        0     2095 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-bundle-protocol-agent-sender.py
+-rw-rw-rw-   0        0        0     1443 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-bundle-protocol-agent.py
+-rw-rw-rw-   0        0        0     1711 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-bundle-serialization.py
+-rw-rw-rw-   0        0        0    15498 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-bundle-size.py
+-rw-rw-rw-   0        0        0     1688 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-dtn7rs-rest-cla.py
+-rw-rw-rw-   0        0        0     1236 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-ipnd.py
+-rw-rw-rw-   0        0        0     2028 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-mtcp-intermediate.py
+-rw-rw-rw-   0        0        0     2260 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-mtcp-receiver.py
+-rw-rw-rw-   0        0        0     2563 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-mtcp-sender.py
+-rw-rw-rw-   0        0        0     5282 2023-04-28 22:29:12.000000 dtn7zero-0.0.6/test/test-py-dtn7-functionality.py
```

### Comparing `dtn7zero-0.0.5/LICENSE` & `dtn7zero-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/PKG-INFO` & `dtn7zero-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtn7zero
-Version: 0.0.5
+Version: 0.0.6
 Author-email: Lukas Holst <lh700@proton.me>
 License: AGPL-3.0
 Project-URL: Homepage, https://github.com/dtn7/dtn7zero
 Project-URL: Repository, https://github.com/dtn7/dtn7zero
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dtn7zero-0.0.5/README.md` & `dtn7zero-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/dtn7zero/api.py` & `dtn7zero-0.0.6/dtn7zero/api.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/dtn7zero/bundle_protocol_agent.py` & `dtn7zero-0.0.6/dtn7zero/bundle_protocol_agent.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/dtn7zero/constants.py` & `dtn7zero-0.0.6/dtn7zero/constants.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/__init__.py` & `dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py` & `dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/dtn7rs_rest.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/dtn7zero/convergence_layer_adapters/mtcp.py` & `dtn7zero-0.0.6/dtn7zero/convergence_layer_adapters/mtcp.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/dtn7zero/data.py` & `dtn7zero-0.0.6/dtn7zero/data.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/dtn7zero/endpoints.py` & `dtn7zero-0.0.6/dtn7zero/endpoints.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/dtn7zero/ipnd.py` & `dtn7zero-0.0.6/dtn7zero/ipnd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import socket
 from typing import Tuple, Optional, List, Dict
 
 from dtn7zero.constants import RUNNING_MICROPYTHON, IPND_IDENTIFIER_MTCP, PORT_MTCP, PORT_IPND, IPND_SEND_INTERVAL_MILLISECONDS, IPND_BEACON_MAX_SIZE
 from dtn7zero.data import Node
 from dtn7zero.storage import Storage
-from dtn7zero.utility import is_timestamp_older_than_timeout, get_current_clock_millis, debug, warning
+from dtn7zero.utility import is_timestamp_older_than_timeout, get_current_clock_millis, debug, warning, \
+    build_broadcast_ipv4_address
 from py_dtn7.bundle import Flags
 
 if RUNNING_MICROPYTHON:
     import wlan
 else:
     import netifaces
 
@@ -263,33 +264,31 @@
     def get_micropython_ipv4_broadcast_addresses() -> (list, list):
         address, subnet, _, _ = wlan.ifconfig()
 
         if address == '0.0.0.0':
             warning('wlan is not connected, cannot form broadcast address')
             return []
 
-        address_parts = address.split('.')
-
-        for idx, subnet_part_str in enumerate(subnet.split('.')):
-            subnet_part = int(subnet_part_str)
-            inverse_subnet_part = ~subnet_part & 0xff
-
-            address_parts[idx] = str(int(address_parts[idx]) & subnet_part | inverse_subnet_part)
-
-        return ['.'.join(address_parts)], [address]
+        return [build_broadcast_ipv4_address(address, subnet)], [address]
 
     @staticmethod
     def get_cpython_ipv4_broadcast_addresses() -> (list, list):
-        address_dicts = []
+        broadcast_addresses = []
+        own_addresses = []
 
         for interface in netifaces.interfaces():
             interface_information = netifaces.ifaddresses(interface).get(netifaces.AF_INET, [])
 
-            # linux 'lo' local interface provides 'peer' instead of 'broadcast'
-            # d['peer']=='127.0.0.1' which is no broadcast address
-            # as a hacky solution we hardcode the broadcast address
-            if interface == 'lo':
-                interface_information[0]['broadcast'] = '127.255.255.255'
+            for address_information in interface_information:
+                address = address_information['addr']
+                netmask = address_information['netmask']
+
+                # in case 'peer' exists => on linux 'lo' interface there is no 'broadcast', only 'peer', but 'netmask' exists
+                # in case 'addr' == 'broadcast' => on linux CORE emulator, no correct 'broadcast' address is provided
+                if 'peer' in address_information or address_information['broadcast'] == address:
+                    broadcast_addresses.append(build_broadcast_ipv4_address(address, netmask))
+                else:
+                    broadcast_addresses.append(address_information['broadcast'])
 
-            address_dicts += interface_information
+                own_addresses.append(address)
 
-        return list(map(lambda d: d['broadcast'], address_dicts)), list(map(lambda d: d['addr'], address_dicts))
+        return broadcast_addresses, own_addresses
```

### Comparing `dtn7zero-0.0.5/dtn7zero/routers/__init__.py` & `dtn7zero-0.0.6/dtn7zero/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/dtn7zero/routers/simple_epidemic_router.py` & `dtn7zero-0.0.6/dtn7zero/routers/simple_epidemic_router.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/dtn7zero/storage/__init__.py` & `dtn7zero-0.0.6/dtn7zero/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/dtn7zero/storage/simple_in_memory_storage.py` & `dtn7zero-0.0.6/dtn7zero/storage/simple_in_memory_storage.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/dtn7zero/utility.py` & `dtn7zero-0.0.6/dtn7zero/utility.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,7 +107,19 @@
     """match description:
     dtn -> one or more characters (except "~" or "/"), then zero or more "/"+one or more characters (except "~" or "/"), ending with "/~"+one or more characters (except "~" or "/")
     ipn -> no group registration
 
     Currently used only on group-endpoint registration by the bpa to check the validity of a full-group-uri.
     """
     return bool(GROUP_URI_REGEX.match(group_uri))
+
+
+def build_broadcast_ipv4_address(address: str, subnet: str) -> str:
+    address_parts = address.split('.')
+
+    for idx, subnet_part_str in enumerate(subnet.split('.')):
+        subnet_part = int(subnet_part_str)
+        inverse_subnet_part = ~subnet_part & 0xff
+
+        address_parts[idx] = str(int(address_parts[idx]) & subnet_part | inverse_subnet_part)
+
+    return '.'.join(address_parts)
```

### Comparing `dtn7zero-0.0.5/dtn7zero.egg-info/PKG-INFO` & `dtn7zero-0.0.6/dtn7zero.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtn7zero
-Version: 0.0.5
+Version: 0.0.6
 Author-email: Lukas Holst <lh700@proton.me>
 License: AGPL-3.0
 Project-URL: Homepage, https://github.com/dtn7/dtn7zero
 Project-URL: Repository, https://github.com/dtn7/dtn7zero
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dtn7zero-0.0.5/dtn7zero.egg-info/SOURCES.txt` & `dtn7zero-0.0.6/dtn7zero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/pyproject.toml` & `dtn7zero-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dtn7zero"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     {name = "Lukas Holst", email = "lh700@proton.me"},
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "AGPL-3.0"}
 dependencies = [
-    "requests",
+    "requests >= 2.27.1",
     "cbor2",
     "netifaces",
     "py-dtn7 >= 0.3.0a1"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dtn7/dtn7zero"
```

### Comparing `dtn7zero-0.0.5/test/test-api-background.py` & `dtn7zero-0.0.6/test/test-api-background.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-api-ping.py` & `dtn7zero-0.0.6/test/test-api-ping.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-api-pong.py` & `dtn7zero-0.0.6/test/test-api-pong.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-api-synchronous.py` & `dtn7zero-0.0.6/test/test-api-synchronous.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-bundle-protocol-agent-receiver.py` & `dtn7zero-0.0.6/test/test-bundle-protocol-agent-receiver.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-bundle-protocol-agent-sender.py` & `dtn7zero-0.0.6/test/test-bundle-protocol-agent-sender.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-bundle-protocol-agent.py` & `dtn7zero-0.0.6/test/test-bundle-protocol-agent.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-bundle-serialization.py` & `dtn7zero-0.0.6/test/test-bundle-serialization.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-bundle-size.py` & `dtn7zero-0.0.6/test/test-bundle-size.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-dtn7rs-rest-cla.py` & `dtn7zero-0.0.6/test/test-dtn7rs-rest-cla.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-ipnd.py` & `dtn7zero-0.0.6/test/test-ipnd.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-mtcp-intermediate.py` & `dtn7zero-0.0.6/test/test-mtcp-intermediate.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-mtcp-receiver.py` & `dtn7zero-0.0.6/test/test-mtcp-receiver.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-mtcp-sender.py` & `dtn7zero-0.0.6/test/test-mtcp-sender.py`

 * *Files identical despite different names*

### Comparing `dtn7zero-0.0.5/test/test-py-dtn7-functionality.py` & `dtn7zero-0.0.6/test/test-py-dtn7-functionality.py`

 * *Files identical despite different names*

