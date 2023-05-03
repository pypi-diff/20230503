# Comparing `tmp/python-selve-new-2.0.8.tar.gz` & `tmp/python-selve-new-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-selve-new-2.0.8.tar", last modified: Fri Nov  4 09:42:20 2022, max compression
+gzip compressed data, was "python-selve-new-2.0.9.tar", last modified: Fri Nov  4 10:00:53 2022, max compression
```

## Comparing `python-selve-new-2.0.8.tar` & `python-selve-new-2.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:42:20.771061 python-selve-new-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-11-04 09:42:20.771061 python-selve-new-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:42:20.767061 python-selve-new-2.0.8/python_selve_new.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-11-04 09:42:20.000000 python-selve-new-2.0.8/python_selve_new.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-04 09:42:20.000000 python-selve-new-2.0.8/python_selve_new.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 09:42:20.000000 python-selve-new-2.0.8/python_selve_new.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-04 09:42:20.000000 python-selve-new-2.0.8/python_selve_new.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-04 09:42:20.000000 python-selve-new-2.0.8/python_selve_new.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:42:20.767061 python-selve-new-2.0.8/selve/
--rw-r--r--   0 runner    (1001) docker     (121)    43387 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:42:20.771061 python-selve-new-2.0.8/selve/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6656 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     5230 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/commands/device.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/commands/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/commands/group.py
--rw-r--r--   0 runner    (1001) docker     (121)     4554 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/commands/iveo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/commands/param.py
--rw-r--r--   0 runner    (1001) docker     (121)     5956 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/commands/senSim.py
--rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/commands/sender.py
--rw-r--r--   0 runner    (1001) docker     (121)     3677 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/commands/sensor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/commands/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/device.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/gateway.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/group.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/iveo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/senSim.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/sender.py
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:42:20.771061 python-selve-new-2.0.8/selve/util/
--rw-r--r--   0 runner    (1001) docker     (121)     9741 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/selve/util/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 09:42:20.771061 python-selve-new-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2791 2022-11-04 09:42:13.000000 python-selve-new-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      905 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/python_selve_new.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      905 2022-11-04 10:00:53.000000 python-selve-new-2.0.9/python_selve_new.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-04 10:00:53.000000 python-selve-new-2.0.9/python_selve_new.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 10:00:53.000000 python-selve-new-2.0.9/python_selve_new.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-04 10:00:53.000000 python-selve-new-2.0.9/python_selve_new.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-04 10:00:53.000000 python-selve-new-2.0.9/python_selve_new.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/selve/
+-rw-r--r--   0 runner    (1001) docker     (121)    43489 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/selve/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6656 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5230 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/device.py
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4554 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/param.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5956 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/sender.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3677 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/commands/service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/device.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/group.py
+-rw-r--r--   0 runner    (1001) docker     (121)      814 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (121)      574 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/sender.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/selve/util/
+-rw-r--r--   0 runner    (1001) docker     (121)     9741 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      776 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/selve/util/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 10:00:53.497413 python-selve-new-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2791 2022-11-04 10:00:46.000000 python-selve-new-2.0.9/setup.py
```

### Comparing `python-selve-new-2.0.8/LICENSE` & `python-selve-new-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/PKG-INFO` & `python-selve-new-2.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `python-selve-new-2.0.8/python_selve_new.egg-info/PKG-INFO` & `python-selve-new-2.0.9/python_selve_new.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `python-selve-new-2.0.8/python_selve_new.egg-info/SOURCES.txt` & `python-selve-new-2.0.9/python_selve_new.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/__init__.py` & `python-selve-new-2.0.9/selve/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,55 @@
 from selve.sensor import SelveSensor
 from selve.util import *
 from selve.util import Command
 from selve.util.errors import *
 from selve.util.protocol import ParameterType
 
 
+def _worker(selve: Selve):
+    # Infinite loop to collect all incoming data
+    selve._LOGGER.debug("Reader started")
+    try:
+        while True:
+            if not selve._pauseReader:
+                with selve._readLock:
+                    if selve._serial.in_waiting > 0:
+                        msg = ""
+                        while True:
+                            response = selve._serial.readline().strip()
+                            msg += response.decode()
+                            if response.decode() == '':
+                                break
+
+                        # do something with the received data
+                        selve.processResponse(msg)
+
+                        # if msg.rstrip() == b' ':
+                        selve._LOGGER.debug(f'Received: {msg}')
+
+            if not selve._pauseWriter:
+                if not selve.txQ.empty():
+                    with selve._writeLock:
+                        data = selve.txQ.get_nowait()
+
+                        selve._sendCommandToGateway(data)
+
+                        selve.txQ.task_done()
+
+                        # always sleep after writing
+                        time.sleep(0.5)
+
+            time.sleep(0.01)
+    # serial port exceptions, all of these notify that we are in some
+    # serious trouble
+    except serial.SerialException:
+        # log message
+        selve._LOGGER.error('Serial Port RX error')
+
+
 class Selve:
     """Implementation of the serial communication to the Selve Gateway"""
 
     def __init__(self, port, discover=True, develop=False, logger=None):
         # Gateway state
         self._callbacks = set()
         self.lastLogEvent = None
@@ -63,19 +104,23 @@
         self._pauseWriter = False
 
         # Port where the Selve gateway was found
         self._port = port
 
         # Write lock to safely write to the gateway
         self._writeLock = threading.Lock()
+        self._readLock = threading.Lock()
 
         self._LOGGER = logger
 
         self._setup()
-        self._start()
+        
+        self.readLoopTask = threading.Thread(target=_worker, args=(self, ))
+        self.readLoopTask.daemon = False
+        self.readLoopTask.start()
 
         if discover:
             self._LOGGER.info("Discovering devices")
             self.discover()
 
     def _setup(self):
         self._LOGGER.info("Setup")
@@ -114,71 +159,27 @@
         """Register callback, called when Roller changes state."""
         self._callbacks.add(callback)
 
     def remove_callback(self, callback: Callable[[], None]) -> None:
         """Remove previously registered callback."""
         self._callbacks.discard(callback)
 
-    def _worker(self, selve):
-        # Infinite loop to collect all incoming data
-        selve._LOGGER.debug("Reader started")
-        try:
-            while True:
-                if not selve._pauseReader:
-                    if selve._serial.in_waiting > 0:
-                        msg = ""
-                        while True:
-                            response = selve._serial.readline().strip()
-                            msg += response.decode()
-                            if response.decode() == '':
-                                break
-
-                        # do something with the received data
-                        selve.processResponse(msg)
-
-                        # if msg.rstrip() == b' ':
-                        selve._LOGGER.debug(f'Received: {msg}')
-
-                if not selve._pauseWriter:
-                    if not selve.txQ.empty():
-                        data = selve.txQ.get_nowait()
-
-                        selve._sendCommandToGateway(data)
-
-                        selve.txQ.task_done()
-
-                        # always sleep after writing
-                        time.sleep(0.5)
-
-                time.sleep(0.01)
-        # serial port exceptions, all of these notify that we are in some
-        # serious trouble
-        except serial.SerialException:
-            # log message
-            selve._LOGGER.error('Serial Port RX error')
-
     def _sendCommandToGateway(self, command: Command):
         commandstr = command.serializeToXML()
         self._LOGGER.debug('Gateway writing: ' + str(commandstr))
         try:
             with self._writeLock:
                 if not self._serial.is_open:
                     self._serial.open()
                 self._serial.write(commandstr)
                 self._serial.flush()
         except Exception as e:
             self._LOGGER.error("error communicating: " + str(e))
         # self.writer.close()
 
-    async def _start(self):
-        """Start all looping threads."""
-        self.readLoopTask = threading.Thread(target=self._worker, args=(self, ))
-        self.readLoopTask.daemon = False
-        self.readLoopTask.start()
-
     # close the serial port, do the cleanup
     def close(self):
         # wait for the rx/tx thread to end, these need to be gathered to
         # collect all the exceptions
         self.readLoopTask.join(5)
         self._serial.close()
 
@@ -452,38 +453,39 @@
         if not self._serial.is_open:
             self._serial.open()
 
         self._sendCommandToGateway(command)
 
         start_time = time.time()
         while True:
-            if self._serial.in_waiting > 0:
-                msg = ""
-                while True:
-                    response = self._serial.readline().strip()
-                    msg += response.decode()
-                    if response.decode() == '':
-                        break
-                # if msg.rstrip() == b' ':
-                self._LOGGER.debug(f'Received: {msg}')
-
-                self._pauseReader = False
-                self._pauseWriter = False
-                self._pauseWorker = False
-
-                resp = self.processResponse(msg)
-                if isinstance(resp, ErrorResponse):
-                    self._LOGGER.error(resp.message)
-                    raise GatewayError
-                else:
-                    #time.sleep(0.5)
-                    return resp
-            if time.time() - start_time > 10:
-                time.sleep(0.05)
-                return None
+            with self._readLock:
+                if self._serial.in_waiting > 0:
+                    msg = ""
+                    while True:
+                        response = self._serial.readline().strip()
+                        msg += response.decode()
+                        if response.decode() == '':
+                            break
+                    # if msg.rstrip() == b' ':
+                    self._LOGGER.debug(f'Received: {msg}')
+
+                    self._pauseReader = False
+                    self._pauseWriter = False
+                    self._pauseWorker = False
+
+                    resp = self.processResponse(msg)
+                    if isinstance(resp, ErrorResponse):
+                        self._LOGGER.error(resp.message)
+                        raise GatewayError
+                    else:
+                        #time.sleep(0.5)
+                        return resp
+                if time.time() - start_time > 10:
+                    time.sleep(0.05)
+                    return None
 
 
     def discover(self):
         if self.gatewayReady():
             iveoIds: IveoGetIdsResponse = self.executeCommandSyncWithResponse(IveoGetIds())
             deviceIds: DeviceGetIdsResponse = self.executeCommandSyncWithResponse(DeviceGetIds())
             groupIds: GroupGetIdsResponse = self.executeCommandSyncWithResponse(GroupGetIds())
```

### Comparing `python-selve-new-2.0.8/selve/commands/command.py` & `python-selve-new-2.0.9/selve/commands/command.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/commands/device.py` & `python-selve-new-2.0.9/selve/commands/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/commands/event.py` & `python-selve-new-2.0.9/selve/commands/event.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/commands/group.py` & `python-selve-new-2.0.9/selve/commands/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/commands/iveo.py` & `python-selve-new-2.0.9/selve/commands/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/commands/param.py` & `python-selve-new-2.0.9/selve/commands/param.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/commands/senSim.py` & `python-selve-new-2.0.9/selve/commands/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/commands/sender.py` & `python-selve-new-2.0.9/selve/commands/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/commands/sensor.py` & `python-selve-new-2.0.9/selve/commands/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/commands/service.py` & `python-selve-new-2.0.9/selve/commands/service.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/device.py` & `python-selve-new-2.0.9/selve/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/group.py` & `python-selve-new-2.0.9/selve/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/iveo.py` & `python-selve-new-2.0.9/selve/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/senSim.py` & `python-selve-new-2.0.9/selve/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/sender.py` & `python-selve-new-2.0.9/selve/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/sensor.py` & `python-selve-new-2.0.9/selve/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/util/__init__.py` & `python-selve-new-2.0.9/selve/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/util/errors.py` & `python-selve-new-2.0.9/selve/util/errors.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/selve/util/protocol.py` & `python-selve-new-2.0.9/selve/util/protocol.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.0.8/setup.py` & `python-selve-new-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     
     name='python-selve-new',  # Required    
-    version='2.0.8',  # Required
+    version='2.0.9',  # Required
     description='Python library for interfacing with selve devices using the USB-RF controller. Written completely new.',  # Required   
     long_description=long_description,  # Optional 
     long_description_content_type="text/markdown",   
     url='https://github.com/Kannix2005/python-selve-new',  # Optional
     author='Stefan Altheimer',  # Optional
    
     author_email='me@stefan-altheimer.de',  # Optional
```

