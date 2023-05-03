# Comparing `tmp/Pipx40-1.31.tar.gz` & `tmp/Pipx40-1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pipx40-1.31.tar", last modified: Mon Mar 20 09:17:48 2023, max compression
+gzip compressed data, was "Pipx40-1.32.tar", last modified: Wed May  3 10:13:21 2023, max compression
```

## Comparing `Pipx40-1.31.tar` & `Pipx40-1.32.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 09:17:48.919798 Pipx40-1.31/
--rw-rw-rw-   0        0        0    10213 2023-03-20 09:17:48.919798 Pipx40-1.31/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-20 09:17:48.912797 Pipx40-1.31/Pipx40/
--rw-rw-rw-   0        0        0    53468 2023-02-14 12:54:36.000000 Pipx40-1.31/Pipx40/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-20 09:17:48.918797 Pipx40-1.31/Pipx40.egg-info/
--rw-rw-rw-   0        0        0    10213 2023-03-20 09:17:48.000000 Pipx40-1.31/Pipx40.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-03-20 09:17:48.000000 Pipx40-1.31/Pipx40.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 09:17:48.000000 Pipx40-1.31/Pipx40.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-20 09:17:48.000000 Pipx40-1.31/Pipx40.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-03-20 09:17:48.000000 Pipx40-1.31/Pipx40.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-20 09:17:48.000000 Pipx40-1.31/Pipx40.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9876 2023-01-20 08:34:47.000000 Pipx40-1.31/README.md
--rw-rw-rw-   0        0        0      388 2023-03-20 09:17:25.000000 Pipx40-1.31/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-20 09:17:48.919798 Pipx40-1.31/setup.cfg
--rw-rw-rw-   0        0        0      330 2023-01-20 08:36:02.000000 Pipx40-1.31/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:13:21.775829 Pipx40-1.32/
+-rw-rw-rw-   0        0        0    10301 2023-05-03 10:13:21.775664 Pipx40-1.32/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 10:13:21.767305 Pipx40-1.32/Pipx40/
+-rw-rw-rw-   0        0        0    53493 2023-05-02 12:47:08.000000 Pipx40-1.32/Pipx40/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:13:21.774226 Pipx40-1.32/Pipx40.egg-info/
+-rw-rw-rw-   0        0        0    10301 2023-05-03 10:13:21.000000 Pipx40-1.32/Pipx40.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-05-03 10:13:21.000000 Pipx40-1.32/Pipx40.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 10:13:21.000000 Pipx40-1.32/Pipx40.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-20 09:17:48.000000 Pipx40-1.32/Pipx40.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-05-03 10:13:21.000000 Pipx40-1.32/Pipx40.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 10:13:21.000000 Pipx40-1.32/Pipx40.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9964 2023-05-02 12:48:28.000000 Pipx40-1.32/README.md
+-rw-rw-rw-   0        0        0      388 2023-05-02 12:49:32.000000 Pipx40-1.32/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 10:13:21.775829 Pipx40-1.32/setup.cfg
+-rw-rw-rw-   0        0        0      330 2023-01-20 08:36:02.000000 Pipx40-1.32/setup.py
```

### Comparing `Pipx40-1.31/PKG-INFO` & `Pipx40-1.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: Pipx40
-Version: 1.31
+Version: 1.32
 Summary: Python Pipx40 is a Python wrapper for Pickering Pipx40 VISA driver.
 Home-page: 
 Author: Pickering Interfaces
 Author-email: Pickering Interfaces <support@pickeringtest.com>
 Project-URL: homepage, https://www.pickeringtest.com/
 Description-Content-Type: text/markdown
 
 # Python Pipx40 #
 
 Python Pipx40 is a Python wrapper for Pickering Pipx40 VISA driver. It supports both Python 2.x and 3.x and has one python dependency (`pyvisa`). 
 
 ----------
 # Changelog #
 
+> - 1.32 - Added attribute helper functions, fixed occasional ctypes.utils import bug.
 > - 1.31 - Added non precision resistor example.
 > - 1.3 - Updates thermocouple functions, adds error/status/attribute code dicts, adds VSourceInfo(), VSourceGetTemperature(), 
 >Updated example code and readme with Python 2.x/3.x compatibility improvements. Functions return native strings in both Python 2.x and 3.x.
 >string `decode()` workaround no longer necessary in Python 3.
 > - 1.2 - Added functions for Thermocouple, error/status codes etc, and modified a few other functions
 > - 1.1 - Refactor for use with pip installer and adds 64 bit support
 > - 1.0 - Initial Release
```

### Comparing `Pipx40-1.31/Pipx40/__init__.py` & `Pipx40-1.32/Pipx40/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import pyvisa
 import platform
 from ctypes import *
+from ctypes import util
 from array import array
 
 def tohex(val, nbits):
     return hex((val + (1 << nbits)) % (1 << nbits))
 
 def Version():
-    return "2023.02.02"
+    return "2023.05.02"
 
 def calc_dwords(bits):
     dwords = bits / 32
     dwords = int(dwords)
     if bits % 32 > 0:
         dwords = dwords + 1
     return dwords
```

### Comparing `Pipx40-1.31/Pipx40.egg-info/PKG-INFO` & `Pipx40-1.32/Pipx40.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: Pipx40
-Version: 1.31
+Version: 1.32
 Summary: Python Pipx40 is a Python wrapper for Pickering Pipx40 VISA driver.
 Home-page: 
 Author: Pickering Interfaces
 Author-email: Pickering Interfaces <support@pickeringtest.com>
 Project-URL: homepage, https://www.pickeringtest.com/
 Description-Content-Type: text/markdown
 
 # Python Pipx40 #
 
 Python Pipx40 is a Python wrapper for Pickering Pipx40 VISA driver. It supports both Python 2.x and 3.x and has one python dependency (`pyvisa`). 
 
 ----------
 # Changelog #
 
+> - 1.32 - Added attribute helper functions, fixed occasional ctypes.utils import bug.
 > - 1.31 - Added non precision resistor example.
 > - 1.3 - Updates thermocouple functions, adds error/status/attribute code dicts, adds VSourceInfo(), VSourceGetTemperature(), 
 >Updated example code and readme with Python 2.x/3.x compatibility improvements. Functions return native strings in both Python 2.x and 3.x.
 >string `decode()` workaround no longer necessary in Python 3.
 > - 1.2 - Added functions for Thermocouple, error/status codes etc, and modified a few other functions
 > - 1.1 - Refactor for use with pip installer and adds 64 bit support
 > - 1.0 - Initial Release
```

### Comparing `Pipx40-1.31/README.md` & `Pipx40-1.32/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Python Pipx40 #
 
 Python Pipx40 is a Python wrapper for Pickering Pipx40 VISA driver. It supports both Python 2.x and 3.x and has one python dependency (`pyvisa`). 
 
 ----------
 # Changelog #
 
+> - 1.32 - Added attribute helper functions, fixed occasional ctypes.utils import bug.
 > - 1.31 - Added non precision resistor example.
 > - 1.3 - Updates thermocouple functions, adds error/status/attribute code dicts, adds VSourceInfo(), VSourceGetTemperature(), 
 >Updated example code and readme with Python 2.x/3.x compatibility improvements. Functions return native strings in both Python 2.x and 3.x.
 >string `decode()` workaround no longer necessary in Python 3.
 > - 1.2 - Added functions for Thermocouple, error/status codes etc, and modified a few other functions
 > - 1.1 - Refactor for use with pip installer and adds 64 bit support
 > - 1.0 - Initial Release
```

