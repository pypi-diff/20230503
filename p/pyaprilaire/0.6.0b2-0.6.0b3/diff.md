# Comparing `tmp/pyaprilaire-0.6.0b2.tar.gz` & `tmp/pyaprilaire-0.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaprilaire-0.6.0b2.tar", last modified: Tue May  2 00:18:26 2023, max compression
+gzip compressed data, was "pyaprilaire-0.6.0b3.tar", last modified: Wed May  3 21:05:55 2023, max compression
```

## Comparing `pyaprilaire-0.6.0b2.tar` & `pyaprilaire-0.6.0b3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:18:26.694633 pyaprilaire-0.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-02 00:18:26.694633 pyaprilaire-0.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:18:26.690633 pyaprilaire-0.6.0b2/pyaprilaire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyaprilaire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyaprilaire/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyaprilaire/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    25603 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyaprilaire/mock_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyaprilaire/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyaprilaire/socket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:18:26.694633 pyaprilaire-0.6.0b2/pyaprilaire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-02 00:18:26.000000 pyaprilaire-0.6.0b2/pyaprilaire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-02 00:18:26.000000 pyaprilaire-0.6.0b2/pyaprilaire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:18:26.000000 pyaprilaire-0.6.0b2/pyaprilaire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 00:18:26.000000 pyaprilaire-0.6.0b2/pyaprilaire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 00:18:26.000000 pyaprilaire-0.6.0b2/pyaprilaire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 00:18:26.694633 pyaprilaire-0.6.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:18:26.694633 pyaprilaire-0.6.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/tests/test_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-02 00:18:08.000000 pyaprilaire-0.6.0b2/tests/test_socket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:05:55.244890 pyaprilaire-0.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-03 21:05:55.244890 pyaprilaire-0.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:05:55.244890 pyaprilaire-0.6.0b3/pyaprilaire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyaprilaire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyaprilaire/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyaprilaire/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25603 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyaprilaire/mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyaprilaire/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyaprilaire/socket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:05:55.244890 pyaprilaire-0.6.0b3/pyaprilaire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-03 21:05:55.000000 pyaprilaire-0.6.0b3/pyaprilaire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-03 21:05:55.000000 pyaprilaire-0.6.0b3/pyaprilaire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:05:55.000000 pyaprilaire-0.6.0b3/pyaprilaire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 21:05:55.000000 pyaprilaire-0.6.0b3/pyaprilaire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 21:05:55.000000 pyaprilaire-0.6.0b3/pyaprilaire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:05:55.244890 pyaprilaire-0.6.0b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:05:55.244890 pyaprilaire-0.6.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/tests/test_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-05-03 21:05:41.000000 pyaprilaire-0.6.0b3/tests/test_socket_client.py
```

### Comparing `pyaprilaire-0.6.0b2/LICENSE` & `pyaprilaire-0.6.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b2/PKG-INFO` & `pyaprilaire-0.6.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaprilaire
-Version: 0.6.0b2
+Version: 0.6.0b3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyaprilaire
 
 pyaprilaire is a library to interact with Aprilaire thermostats.
```

### Comparing `pyaprilaire-0.6.0b2/README.md` & `pyaprilaire-0.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b2/pyaprilaire/client.py` & `pyaprilaire-0.6.0b3/pyaprilaire/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,16 +212,20 @@
                     "fan_mode": fan_mode,
                     "heat_setpoint": 0,
                     "cool_setpoint": 0,
                 },
             )
         )
 
-    async def update_setpoint(self, cool_setpoint: int, heat_setpoint: int):
+    async def update_setpoint(self, cool_setpoint: float, heat_setpoint: float):
         """Send a request to update the setpoint"""
+
+        cool_setpoint = round(cool_setpoint * 2) / 2
+        heat_setpoint = round(heat_setpoint * 2) / 2
+
         await self._send_packet(
             Packet(
                 Action.WRITE,
                 FunctionalDomain.CONTROL,
                 1,
                 data={
                     "mode": 0,
@@ -475,15 +479,15 @@
         """Send a request to update the mode"""
         await self.protocol.update_mode(mode)
 
     async def update_fan_mode(self, fan_mode: int):
         """Send a request to update the fan mode"""
         await self.protocol.update_fan_mode(fan_mode)
 
-    async def update_setpoint(self, cool_setpoint: int, heat_setpoint: int):
+    async def update_setpoint(self, cool_setpoint: float, heat_setpoint: float):
         """Send a request to update the setpoint"""
         await self.protocol.update_setpoint(cool_setpoint, heat_setpoint)
 
     async def set_hold(self, hold: int):
         """Send a request to update the away status"""
         await self.protocol.set_hold(hold)
```

### Comparing `pyaprilaire-0.6.0b2/pyaprilaire/const.py` & `pyaprilaire-0.6.0b3/pyaprilaire/const.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b2/pyaprilaire/mock_server.py` & `pyaprilaire-0.6.0b3/pyaprilaire/mock_server.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b2/pyaprilaire/packet.py` & `pyaprilaire-0.6.0b3/pyaprilaire/packet.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b2/pyaprilaire/socket_client.py` & `pyaprilaire-0.6.0b3/pyaprilaire/socket_client.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b2/pyaprilaire.egg-info/PKG-INFO` & `pyaprilaire-0.6.0b3/pyaprilaire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaprilaire
-Version: 0.6.0b2
+Version: 0.6.0b3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # pyaprilaire
 
 pyaprilaire is a library to interact with Aprilaire thermostats.
```

### Comparing `pyaprilaire-0.6.0b2/pyproject.toml` & `pyaprilaire-0.6.0b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyaprilaire"
-version = "0.6.0b2"
+version = "0.6.0b3"
 readme = "README.md"
 dependencies = [
     "crc >= 4"
 ]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "coverage"]
 
 [tool.bumpver]
-current_version = "0.6.0b2"
+current_version = "0.6.0b3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyaprilaire-0.6.0b2/tests/test_client.py` & `pyaprilaire-0.6.0b3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b2/tests/test_packet.py` & `pyaprilaire-0.6.0b3/tests/test_packet.py`

 * *Files identical despite different names*

### Comparing `pyaprilaire-0.6.0b2/tests/test_socket_client.py` & `pyaprilaire-0.6.0b3/tests/test_socket_client.py`

 * *Files identical despite different names*

