# Comparing `tmp/pymx2-0.1.3.tar.gz` & `tmp/pymx2-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymx2-0.1.3.tar", last modified: Tue May  2 15:02:54 2023, max compression
+gzip compressed data, was "pymx2-0.1.4.tar", last modified: Wed May  3 08:13:45 2023, max compression
```

## Comparing `pymx2-0.1.3.tar` & `pymx2-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-02 15:02:54.003892 pymx2-0.1.3/
--rw-r--r--   0 vpaeder    (501) staff       (20)       39 2023-04-27 13:13:03.000000 pymx2-0.1.3/.gitignore
--rw-r--r--   0 vpaeder    (501) staff       (20)     1071 2023-04-27 13:41:31.000000 pymx2-0.1.3/LICENSE
--rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-02 15:02:54.003408 pymx2-0.1.3/PKG-INFO
--rw-r--r--   0 vpaeder    (501) staff       (20)     2938 2023-04-28 18:35:35.000000 pymx2-0.1.3/README.md
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-02 15:02:53.990566 pymx2-0.1.3/docs/
--rw-r--r--   0 vpaeder    (501) staff       (20)   214194 2023-05-02 15:01:56.000000 pymx2-0.1.3/docs/mx2.enums.html
--rw-r--r--   0 vpaeder    (501) staff       (20)    60476 2023-05-02 15:02:06.000000 pymx2-0.1.3/docs/mx2.exceptions.html
--rw-r--r--   0 vpaeder    (501) staff       (20)    22217 2023-05-02 15:01:50.000000 pymx2-0.1.3/docs/mx2.html
--rw-r--r--   0 vpaeder    (501) staff       (20)    10077 2023-05-02 15:02:00.000000 pymx2-0.1.3/docs/mx2.types.html
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-02 15:02:53.994374 pymx2-0.1.3/examples/
--rw-r--r--   0 vpaeder    (501) staff       (20)      431 2023-04-24 11:33:12.000000 pymx2-0.1.3/examples/01_connect.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      978 2023-04-24 11:35:16.000000 pymx2-0.1.3/examples/02_read_write_coil.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      903 2023-04-26 16:47:32.000000 pymx2-0.1.3/examples/03_read_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      841 2023-04-27 12:28:11.000000 pymx2-0.1.3/examples/04_write_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      954 2023-04-27 11:31:32.000000 pymx2-0.1.3/examples/05_read_write_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     1766 2023-04-27 12:08:57.000000 pymx2-0.1.3/examples/06_data_types.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-02 15:02:53.997564 pymx2-0.1.3/mx2/
--rw-r--r--   0 vpaeder    (501) staff       (20)    31996 2023-05-02 14:54:17.000000 pymx2-0.1.3/mx2/__init__.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    48702 2023-04-28 12:11:12.000000 pymx2-0.1.3/mx2/enums.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     2161 2023-04-21 11:17:50.000000 pymx2-0.1.3/mx2/exceptions.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    11345 2023-05-02 14:57:19.000000 pymx2-0.1.3/mx2/types.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-02 15:02:54.000048 pymx2-0.1.3/pymx2.egg-info/
--rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-02 15:02:53.000000 pymx2-0.1.3/pymx2.egg-info/PKG-INFO
--rw-r--r--   0 vpaeder    (501) staff       (20)      577 2023-05-02 15:02:53.000000 pymx2-0.1.3/pymx2.egg-info/SOURCES.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)        1 2023-05-02 15:02:53.000000 pymx2-0.1.3/pymx2.egg-info/dependency_links.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)        9 2023-05-02 15:02:53.000000 pymx2-0.1.3/pymx2.egg-info/requires.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)       10 2023-05-02 15:02:53.000000 pymx2-0.1.3/pymx2.egg-info/top_level.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)       38 2023-05-02 15:02:54.004025 pymx2-0.1.3/setup.cfg
--rw-r--r--   0 vpaeder    (501) staff       (20)     1056 2023-05-02 15:01:18.000000 pymx2-0.1.3/setup.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-02 15:02:54.002729 pymx2-0.1.3/tests/
--rw-r--r--   0 vpaeder    (501) staff       (20)      144 2023-04-27 07:40:09.000000 pymx2-0.1.3/tests/__init__.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    15021 2023-05-02 15:00:57.000000 pymx2-0.1.3/tests/inverter.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     4511 2023-05-02 14:58:17.000000 pymx2-0.1.3/tests/modbus.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     3616 2023-04-21 10:52:45.000000 pymx2-0.1.3/tests/ser.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    10281 2023-04-27 12:31:47.000000 pymx2-0.1.3/tests/types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-03 08:13:45.532081 pymx2-0.1.4/
+-rw-r--r--   0 vpaeder    (501) staff       (20)       39 2023-04-27 13:13:03.000000 pymx2-0.1.4/.gitignore
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1071 2023-04-27 13:41:31.000000 pymx2-0.1.4/LICENSE
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-03 08:13:45.531479 pymx2-0.1.4/PKG-INFO
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2938 2023-04-28 18:35:35.000000 pymx2-0.1.4/README.md
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-03 08:13:45.516489 pymx2-0.1.4/docs/
+-rw-r--r--   0 vpaeder    (501) staff       (20)   214194 2023-05-02 15:01:56.000000 pymx2-0.1.4/docs/mx2.enums.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    60476 2023-05-02 15:02:06.000000 pymx2-0.1.4/docs/mx2.exceptions.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    22217 2023-05-02 15:01:50.000000 pymx2-0.1.4/docs/mx2.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    10077 2023-05-02 15:02:00.000000 pymx2-0.1.4/docs/mx2.types.html
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-03 08:13:45.520691 pymx2-0.1.4/examples/
+-rw-r--r--   0 vpaeder    (501) staff       (20)      431 2023-04-24 11:33:12.000000 pymx2-0.1.4/examples/01_connect.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      978 2023-04-24 11:35:16.000000 pymx2-0.1.4/examples/02_read_write_coil.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      903 2023-04-26 16:47:32.000000 pymx2-0.1.4/examples/03_read_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      841 2023-04-27 12:28:11.000000 pymx2-0.1.4/examples/04_write_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      954 2023-04-27 11:31:32.000000 pymx2-0.1.4/examples/05_read_write_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1766 2023-04-27 12:08:57.000000 pymx2-0.1.4/examples/06_data_types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-03 08:13:45.523704 pymx2-0.1.4/mx2/
+-rw-r--r--   0 vpaeder    (501) staff       (20)    31998 2023-05-03 07:51:28.000000 pymx2-0.1.4/mx2/__init__.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    48702 2023-04-28 12:11:12.000000 pymx2-0.1.4/mx2/enums.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2161 2023-04-21 11:17:50.000000 pymx2-0.1.4/mx2/exceptions.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    11345 2023-05-02 14:57:19.000000 pymx2-0.1.4/mx2/types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-03 08:13:45.526567 pymx2-0.1.4/pymx2.egg-info/
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-03 08:13:45.000000 pymx2-0.1.4/pymx2.egg-info/PKG-INFO
+-rw-r--r--   0 vpaeder    (501) staff       (20)      577 2023-05-03 08:13:45.000000 pymx2-0.1.4/pymx2.egg-info/SOURCES.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)        1 2023-05-03 08:13:45.000000 pymx2-0.1.4/pymx2.egg-info/dependency_links.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)        9 2023-05-03 08:13:45.000000 pymx2-0.1.4/pymx2.egg-info/requires.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)       10 2023-05-03 08:13:45.000000 pymx2-0.1.4/pymx2.egg-info/top_level.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)       38 2023-05-03 08:13:45.532341 pymx2-0.1.4/setup.cfg
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1056 2023-05-03 07:51:39.000000 pymx2-0.1.4/setup.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-03 08:13:45.530263 pymx2-0.1.4/tests/
+-rw-r--r--   0 vpaeder    (501) staff       (20)      144 2023-04-27 07:40:09.000000 pymx2-0.1.4/tests/__init__.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    15021 2023-05-02 15:00:57.000000 pymx2-0.1.4/tests/inverter.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     4511 2023-05-02 14:58:17.000000 pymx2-0.1.4/tests/modbus.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3616 2023-04-21 10:52:45.000000 pymx2-0.1.4/tests/ser.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    10281 2023-04-27 12:31:47.000000 pymx2-0.1.4/tests/types.py
```

### Comparing `pymx2-0.1.3/LICENSE` & `pymx2-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/PKG-INFO` & `pymx2-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymx2
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python driver to communicate with an Omron MX2 inverter through Modbus
 Home-page: https://github.com/vpaeder/pymx2
 Author: Vincent Paeder
 Author-email: python@paeder.fi
 Project-URL: Bug Tracker, https://github.com/vpaeder/pymx2/issues
 Keywords: omron,mx2,inverter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymx2-0.1.3/README.md` & `pymx2-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/docs/mx2.enums.html` & `pymx2-0.1.4/docs/mx2.enums.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/docs/mx2.exceptions.html` & `pymx2-0.1.4/docs/mx2.exceptions.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/docs/mx2.html` & `pymx2-0.1.4/docs/mx2.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/docs/mx2.types.html` & `pymx2-0.1.4/docs/mx2.types.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/examples/02_read_write_coil.py` & `pymx2-0.1.4/examples/02_read_write_coil.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/examples/03_read_registers.py` & `pymx2-0.1.4/examples/03_read_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/examples/04_write_registers.py` & `pymx2-0.1.4/examples/04_write_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/examples/05_read_write_registers.py` & `pymx2-0.1.4/examples/05_read_write_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/examples/06_data_types.py` & `pymx2-0.1.4/examples/06_data_types.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/mx2/__init__.py` & `pymx2-0.1.4/mx2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -797,15 +797,15 @@
         if index<1 or index>6:
             raise BadParameterException("Fault monitor index can be between 1 and 6.")
         if value<0 or value>9:
             raise BadParameterException("Fault monitor data index can be between 0 and 9.")
         
         addr = [MonitoringFunctions.FaultMonitor1, MonitoringFunctions.FaultMonitor2,
                 MonitoringFunctions.FaultMonitor3, MonitoringFunctions.FaultMonitor4,
-                MonitoringFunctions.FaultMonitor5, MonitoringFunctions.FaultMonitor6][index] + value
+                MonitoringFunctions.FaultMonitor5, MonitoringFunctions.FaultMonitor6][index-1] + value
 
         if value in [FaultMonitorData.Frequency, FaultMonitorData.RunningTime, FaultMonitorData.PowerOnTime]:
             result = self.read_registers(addr, 2)
             return (result[0] << 16) + result[1]
         else:
             result = self.read_registers(addr, 1)
             return result[0]
```

### Comparing `pymx2-0.1.3/mx2/enums.py` & `pymx2-0.1.4/mx2/enums.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/mx2/exceptions.py` & `pymx2-0.1.4/mx2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/mx2/types.py` & `pymx2-0.1.4/mx2/types.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/pymx2.egg-info/PKG-INFO` & `pymx2-0.1.4/pymx2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymx2
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python driver to communicate with an Omron MX2 inverter through Modbus
 Home-page: https://github.com/vpaeder/pymx2
 Author: Vincent Paeder
 Author-email: python@paeder.fi
 Project-URL: Bug Tracker, https://github.com/vpaeder/pymx2/issues
 Keywords: omron,mx2,inverter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymx2-0.1.3/pymx2.egg-info/SOURCES.txt` & `pymx2-0.1.4/pymx2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/setup.py` & `pymx2-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymx2",
-    version="0.1.3",
+    version="0.1.4",
     author="Vincent Paeder",
     author_email="python@paeder.fi",
     description="A Python driver to communicate with an Omron MX2 inverter through Modbus",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['omron', 'mx2', 'inverter'],
     url="https://github.com/vpaeder/pymx2",
```

### Comparing `pymx2-0.1.3/tests/inverter.py` & `pymx2-0.1.4/tests/inverter.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/tests/modbus.py` & `pymx2-0.1.4/tests/modbus.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/tests/ser.py` & `pymx2-0.1.4/tests/ser.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.3/tests/types.py` & `pymx2-0.1.4/tests/types.py`

 * *Files identical despite different names*

