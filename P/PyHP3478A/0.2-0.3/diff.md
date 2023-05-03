# Comparing `tmp/PyHP3478A-0.2.tar.gz` & `tmp/PyHP3478A-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHP3478A-0.2.tar", last modified: Tue Apr 25 19:24:07 2023, max compression
+gzip compressed data, was "PyHP3478A-0.3.tar", last modified: Wed May  3 19:03:43 2023, max compression
```

## Comparing `PyHP3478A-0.2.tar` & `PyHP3478A-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 19:24:07.903760 PyHP3478A-0.2/
--rw-rw-rw-   0        0        0     1091 2023-01-16 20:41:41.000000 PyHP3478A-0.2/LICENSE
--rw-rw-rw-   0        0        0      326 2023-04-25 19:24:07.902761 PyHP3478A-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 19:24:07.891323 PyHP3478A-0.2/PyHP3478A/
--rw-rw-rw-   0        0        0     6759 2023-04-25 19:22:27.000000 PyHP3478A-0.2/PyHP3478A/HP3478A.py
--rw-rw-rw-   0        0        0       30 2023-04-25 18:01:43.000000 PyHP3478A-0.2/PyHP3478A/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 19:24:07.901763 PyHP3478A-0.2/PyHP3478A.egg-info/
--rw-rw-rw-   0        0        0      326 2023-04-25 19:24:07.000000 PyHP3478A-0.2/PyHP3478A.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-25 19:24:07.000000 PyHP3478A-0.2/PyHP3478A.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 19:24:07.000000 PyHP3478A-0.2/PyHP3478A.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-25 19:24:07.000000 PyHP3478A-0.2/PyHP3478A.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-25 19:24:07.000000 PyHP3478A-0.2/PyHP3478A.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      128 2023-04-25 18:04:12.000000 PyHP3478A-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-25 19:24:07.903760 PyHP3478A-0.2/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-04-25 18:04:25.000000 PyHP3478A-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:03:43.796014 PyHP3478A-0.3/
+-rw-rw-rw-   0        0        0     1091 2023-01-16 20:41:41.000000 PyHP3478A-0.3/LICENSE
+-rw-rw-rw-   0        0        0      326 2023-05-03 19:03:43.795013 PyHP3478A-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 19:03:43.764041 PyHP3478A-0.3/PyHP3478A/
+-rw-rw-rw-   0        0        0     6932 2023-05-03 19:03:13.000000 PyHP3478A-0.3/PyHP3478A/HP3478A.py
+-rw-rw-rw-   0        0        0       28 2023-05-02 17:49:03.000000 PyHP3478A-0.3/PyHP3478A/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 19:03:43.793013 PyHP3478A-0.3/PyHP3478A.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-05-03 19:03:43.000000 PyHP3478A-0.3/PyHP3478A.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-03 19:03:43.000000 PyHP3478A-0.3/PyHP3478A.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 19:03:43.000000 PyHP3478A-0.3/PyHP3478A.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 19:03:43.000000 PyHP3478A-0.3/PyHP3478A.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-03 19:03:43.000000 PyHP3478A-0.3/PyHP3478A.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      128 2023-04-25 18:04:12.000000 PyHP3478A-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 19:03:43.796014 PyHP3478A-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-05-02 17:28:04.000000 PyHP3478A-0.3/setup.py
```

### Comparing `PyHP3478A-0.2/LICENSE` & `PyHP3478A-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyHP3478A-0.2/PyHP3478A/HP3478A.py` & `PyHP3478A-0.3/PyHP3478A/HP3478A.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 class HP3478A:
+    """HP3478A made simple with Python and the AR488 project!
+    use the PyAR488 module to comunicate with the AR488 board and make you lab bench smart
+    -> written by Minu"""
     from PyAR488 import AR488
 
     class Exceptions:
         class StatusByteException(Exception):
             def __init__(self) -> None:
                 super().__init__('error reading instrument status byte')
         class InvalidDigits(Exception):
@@ -112,15 +115,15 @@
             self.invalid_calibration = response_bits[5] == '1'
             self.srq = response_bits[6] == '1'
             self.power_on_srq = response_bits[7] == '1'
 
 
     def get_status_byte(self):
         """returns the status byte of the instrument as an int or a dict"""
-        response = self.interface.prologix_spoll(self.address)
+        response = self.interface.spoll(self.address)
         try:
             response = int(response)
         except ValueError:
             raise self.Exceptions.StatusByteException()
         
         return self.StatusByte(response)
```

### Comparing `PyHP3478A-0.2/setup.py` & `PyHP3478A-0.3/setup.py`

 * *Files identical despite different names*

