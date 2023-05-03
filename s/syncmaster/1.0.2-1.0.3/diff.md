# Comparing `tmp/syncmaster-1.0.2.tar.gz` & `tmp/syncmaster-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncmaster-1.0.2.tar", last modified: Fri Apr 28 11:30:34 2023, max compression
+gzip compressed data, was "syncmaster-1.0.3.tar", last modified: Wed May  3 12:50:54 2023, max compression
```

## Comparing `syncmaster-1.0.2.tar` & `syncmaster-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-28 11:30:34.637973 syncmaster-1.0.2/
--rw-rw-r--   0 conor     (1000) conor     (1000)    11337 2023-01-20 02:50:04.000000 syncmaster-1.0.2/LICENSE
--rw-rw-r--   0 conor     (1000) conor     (1000)      111 2023-01-20 02:50:04.000000 syncmaster-1.0.2/MANIFEST.in
--rw-rw-r--   0 conor     (1000) conor     (1000)     3262 2023-04-28 11:30:34.637973 syncmaster-1.0.2/PKG-INFO
--rw-rw-r--   0 conor     (1000) conor     (1000)     2410 2023-04-17 17:49:29.000000 syncmaster-1.0.2/README.md
--rw-rw-r--   0 conor     (1000) conor     (1000)      929 2023-04-28 11:30:05.000000 syncmaster-1.0.2/settings.ini
--rw-rw-r--   0 conor     (1000) conor     (1000)       38 2023-04-28 11:30:34.637973 syncmaster-1.0.2/setup.cfg
--rw-rw-r--   0 conor     (1000) conor     (1000)     2560 2023-01-20 02:50:04.000000 syncmaster-1.0.2/setup.py
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-28 11:30:34.633973 syncmaster-1.0.2/syncmaster/
--rw-rw-r--   0 conor     (1000) conor     (1000)      235 2023-04-28 11:29:29.000000 syncmaster-1.0.2/syncmaster/__init__.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     1918 2023-04-28 11:29:29.000000 syncmaster-1.0.2/syncmaster/_modidx.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     2371 2023-04-28 11:29:29.000000 syncmaster-1.0.2/syncmaster/analysis.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     3546 2023-04-28 11:29:29.000000 syncmaster-1.0.2/syncmaster/device.py
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-04-28 11:30:34.637973 syncmaster-1.0.2/syncmaster.egg-info/
--rw-rw-r--   0 conor     (1000) conor     (1000)     3262 2023-04-28 11:30:34.000000 syncmaster-1.0.2/syncmaster.egg-info/PKG-INFO
--rw-rw-r--   0 conor     (1000) conor     (1000)      379 2023-04-28 11:30:34.000000 syncmaster-1.0.2/syncmaster.egg-info/SOURCES.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-28 11:30:34.000000 syncmaster-1.0.2/syncmaster.egg-info/dependency_links.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)       42 2023-04-28 11:30:34.000000 syncmaster-1.0.2/syncmaster.egg-info/entry_points.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 10:19:07.000000 syncmaster-1.0.2/syncmaster.egg-info/not-zip-safe
--rw-rw-r--   0 conor     (1000) conor     (1000)       41 2023-04-28 11:30:34.000000 syncmaster-1.0.2/syncmaster.egg-info/requires.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)       11 2023-04-28 11:30:34.000000 syncmaster-1.0.2/syncmaster.egg-info/top_level.txt
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-03 12:50:54.855698 syncmaster-1.0.3/
+-rw-rw-r--   0 conor     (1000) conor     (1000)    11337 2023-01-20 02:50:04.000000 syncmaster-1.0.3/LICENSE
+-rw-rw-r--   0 conor     (1000) conor     (1000)      111 2023-01-20 02:50:04.000000 syncmaster-1.0.3/MANIFEST.in
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3416 2023-05-03 12:50:54.855698 syncmaster-1.0.3/PKG-INFO
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2564 2023-05-03 12:49:23.000000 syncmaster-1.0.3/README.md
+-rw-rw-r--   0 conor     (1000) conor     (1000)      929 2023-05-03 12:36:43.000000 syncmaster-1.0.3/settings.ini
+-rw-rw-r--   0 conor     (1000) conor     (1000)       38 2023-05-03 12:50:54.855698 syncmaster-1.0.3/setup.cfg
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2560 2023-01-20 02:50:04.000000 syncmaster-1.0.3/setup.py
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-03 12:50:54.855698 syncmaster-1.0.3/syncmaster/
+-rw-rw-r--   0 conor     (1000) conor     (1000)      235 2023-05-03 12:50:06.000000 syncmaster-1.0.3/syncmaster/__init__.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2057 2023-05-03 12:50:06.000000 syncmaster-1.0.3/syncmaster/_modidx.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2371 2023-05-03 12:50:06.000000 syncmaster-1.0.3/syncmaster/analysis.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3674 2023-05-03 12:50:06.000000 syncmaster-1.0.3/syncmaster/device.py
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-03 12:50:54.855698 syncmaster-1.0.3/syncmaster.egg-info/
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3416 2023-05-03 12:50:54.000000 syncmaster-1.0.3/syncmaster.egg-info/PKG-INFO
+-rw-rw-r--   0 conor     (1000) conor     (1000)      379 2023-05-03 12:50:54.000000 syncmaster-1.0.3/syncmaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-05-03 12:50:54.000000 syncmaster-1.0.3/syncmaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)       42 2023-05-03 12:50:54.000000 syncmaster-1.0.3/syncmaster.egg-info/entry_points.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 10:19:07.000000 syncmaster-1.0.3/syncmaster.egg-info/not-zip-safe
+-rw-rw-r--   0 conor     (1000) conor     (1000)       41 2023-05-03 12:50:54.000000 syncmaster-1.0.3/syncmaster.egg-info/requires.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)       11 2023-05-03 12:50:54.000000 syncmaster-1.0.3/syncmaster.egg-info/top_level.txt
```

### Comparing `syncmaster-1.0.2/LICENSE` & `syncmaster-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.2/PKG-INFO` & `syncmaster-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncmaster
-Version: 1.0.2
+Version: 1.0.3
 Summary: Device and drivers for generating trigger signals to synchronise recorded signals with behavioural data
 Home-page: https://github.com/conorkeogh/syncmaster
 Author: Conor Keogh
 Author-email: conor.keogh@nds.ox.ac.uk
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -78,14 +78,18 @@
 # Close communication channel when finished
 device.close()
 ```
 
 On completion of the task, the communication channel with the device
 should be formally closed.
 
+Note that more complex task designs with up to 100 user-defined event
+types can be accommodated. This is outlined in detail in the
+`triggering` section.
+
 ## Output
 
 The device produced pulses of differing lengths on a single output
 channel. Each pulse length corresponds to a specific event type.
 
 The package includes a function for recovering the discrete event
 timings from this single-channel pulse data in order to facilitate data
```

### Comparing `syncmaster-1.0.2/README.md` & `syncmaster-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,18 @@
 # Close communication channel when finished
 device.close()
 ```
 
 On completion of the task, the communication channel with the device
 should be formally closed.
 
+Note that more complex task designs with up to 100 user-defined event
+types can be accommodated. This is outlined in detail in the
+`triggering` section.
+
 ## Output
 
 The device produced pulses of differing lengths on a single output
 channel. Each pulse length corresponds to a specific event type.
 
 The package includes a function for recovering the discrete event
 timings from this single-channel pulse data in order to facilitate data
```

### Comparing `syncmaster-1.0.2/settings.ini` & `syncmaster-1.0.3/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = syncmaster
 lib_name = syncmaster
-version = 1.0.2
+version = 1.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = syncmaster
 nbs_path = nbs
 recursive = True
```

### Comparing `syncmaster-1.0.2/setup.py` & `syncmaster-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.2/syncmaster/_modidx.py` & `syncmaster-1.0.3/syncmaster/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
                 'lib_path': 'syncmaster'},
   'syms': { 'syncmaster.analysis': {'syncmaster.analysis.getEvents': ('events.html#getevents', 'syncmaster/analysis.py')},
             'syncmaster.device': { 'syncmaster.device.SyncMaster': ('initialisation.html#syncmaster', 'syncmaster/device.py'),
                                    'syncmaster.device.SyncMaster.__init__': ( 'initialisation.html#syncmaster.__init__',
                                                                               'syncmaster/device.py'),
                                    'syncmaster.device.SyncMaster.close': ('initialisation.html#syncmaster.close', 'syncmaster/device.py'),
                                    'syncmaster.device.SyncMaster.end': ('initialisation.html#syncmaster.end', 'syncmaster/device.py'),
+                                   'syncmaster.device.SyncMaster.event': ('initialisation.html#syncmaster.event', 'syncmaster/device.py'),
                                    'syncmaster.device.SyncMaster.event1': ('initialisation.html#syncmaster.event1', 'syncmaster/device.py'),
                                    'syncmaster.device.SyncMaster.event2': ('initialisation.html#syncmaster.event2', 'syncmaster/device.py'),
                                    'syncmaster.device.SyncMaster.sendMessage': ( 'initialisation.html#syncmaster.sendmessage',
                                                                                  'syncmaster/device.py'),
                                    'syncmaster.device.SyncMaster.start': ('initialisation.html#syncmaster.start', 'syncmaster/device.py'),
                                    'syncmaster.device.SyncMaster.testSignal': ( 'initialisation.html#syncmaster.testsignal',
                                                                                 'syncmaster/device.py')}}}
```

### Comparing `syncmaster-1.0.2/syncmaster/analysis.py` & `syncmaster-1.0.3/syncmaster/analysis.py`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.2/syncmaster/device.py` & `syncmaster-1.0.3/syncmaster/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,28 +32,24 @@
         Device object for controlling synchronisation
         '''
 
         '''
         Define constants for device configuration
         '''
         # Define messages
-        self.STARTMARKER = b'1'
-        self.ENDMARKER = b'2'
-        self.EVENT1 = b'3'
-        self.EVENT2 = b'4'
+        self.GREETING = b'<best wishes>'
+        self.RESPONSE = b'warmest regards'
+        self.startMarker = '<'
+        self.endMarker = '>'
     
-        # Define trigger pulse widths (milliseconds)
-        self.STARTPULSE = 50
-        self.ENDPULSE = 100
-        self.EVENT1PULSE = 150
-        self.EVENT2PULSE = 200
-    
-        # Define host acknowledge messages
-        self.HOST_MESSAGE = b'5'
-        self.ACKNOWLEDGE = 42
+        # Define trigger pulse widths (val*10, milliseconds)
+        self.STARTPULSE = 5 # 50ms
+        self.ENDPULSE = 10 # 100ms
+        self.EVENT1PULSE = 15 # 150ms
+        self.EVENT2PULSE = 20 # 200ms
     
         # Define COM port settings
         self.BAUDRATE = 115200
         
         # Get all serial ports
         ports = serial.tools.list_ports.comports()
 
@@ -66,16 +62,15 @@
 
                 # Send test message and read response; repeat 3 times and keep third
                 for _ in range(3):
                     self.sendMessage(self.HOST_MESSAGE)
                     response = self.ser.readline()
 
                 # Check if response is appropriate
-                response = int(response)
-                if response == self.ACKNOWLEDGE:
+                if response.decode().strip() == self.RESPONSE:
                     self.target_port = port.device
                     port_found = True
 
                 # Close port
                 self.ser.close()
 
             except Exception as e:
@@ -104,22 +99,27 @@
     def event1(self):
         ''' Send event 1 signal '''
         self.sendMessage(self.EVENT1)
 
     def event2(self):
         ''' Send event 2 signal '''
         self.sendMessage(self.EVENT2)
+        
+    def event(self, eventID):
+        ''' Create event marker '''
+        self.sendMessage(eventID)
 
     # Send message via serial port
     def sendMessage(self, message):
         '''
         Send message over serial port
         Takes message to send
         '''
-        self.ser.write(message)
+        message_prepared = self.startMarker + str(message) + self.endMarker
+        self.ser.write(message_prepared.encode())
 
     # Close channel
     def close(self):
         '''
         Closes device connection
         '''
         self.ser.close()
```

### Comparing `syncmaster-1.0.2/syncmaster.egg-info/PKG-INFO` & `syncmaster-1.0.3/syncmaster.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncmaster
-Version: 1.0.2
+Version: 1.0.3
 Summary: Device and drivers for generating trigger signals to synchronise recorded signals with behavioural data
 Home-page: https://github.com/conorkeogh/syncmaster
 Author: Conor Keogh
 Author-email: conor.keogh@nds.ox.ac.uk
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -78,14 +78,18 @@
 # Close communication channel when finished
 device.close()
 ```
 
 On completion of the task, the communication channel with the device
 should be formally closed.
 
+Note that more complex task designs with up to 100 user-defined event
+types can be accommodated. This is outlined in detail in the
+`triggering` section.
+
 ## Output
 
 The device produced pulses of differing lengths on a single output
 channel. Each pulse length corresponds to a specific event type.
 
 The package includes a function for recovering the discrete event
 timings from this single-channel pulse data in order to facilitate data
```

