# Comparing `tmp/toori-1.1.0.tar.gz` & `tmp/toori-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\toori-1.1.0.tar", last modified: Wed May  3 04:25:44 2023, max compression
+gzip compressed data, was "dist\toori-1.1.1.tar", last modified: Wed May  3 04:30:00 2023, max compression
```

## Comparing `toori-1.1.0.tar` & `toori-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/
--rw-rw-rw-   0        0        0     1442 2023-05-03 04:25:44.000000 toori-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      842 2023-05-03 04:25:02.000000 toori-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/external/
-drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/external/WinDivert-2.2.2-A/
-drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/external/WinDivert-2.2.2-A/include/
--rw-rw-rw-   0        0        0    20671 2023-05-03 04:25:02.000000 toori-1.1.0/external/WinDivert-2.2.2-A/include/windivert.h
-drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/external/WinDivert-2.2.2-A/x64/
--rw-rw-rw-   0        0        0    47616 2023-05-03 04:25:02.000000 toori-1.1.0/external/WinDivert-2.2.2-A/x64/WinDivert.dll
--rw-rw-rw-   0        0        0    25422 2023-05-03 04:25:02.000000 toori-1.1.0/external/WinDivert-2.2.2-A/x64/WinDivert.lib
--rw-rw-rw-   0        0        0    94144 2023-05-03 04:25:02.000000 toori-1.1.0/external/WinDivert-2.2.2-A/x64/WinDivert64.sys
--rw-rw-rw-   0        0        0      120 2023-05-03 04:25:02.000000 toori-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 04:25:44.000000 toori-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2241 2023-05-03 04:25:02.000000 toori-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/toori/
--rw-rw-rw-   0        0        0      504 2023-05-03 04:25:02.000000 toori-1.1.0/toori/console.py
--rw-rw-rw-   0        0        0     3578 2023-05-03 04:25:02.000000 toori-1.1.0/toori/main.cpp
--rw-rw-rw-   0        0        0     2166 2023-05-03 04:25:02.000000 toori-1.1.0/toori/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/toori.egg-info/
--rw-rw-rw-   0        0        0     1442 2023-05-03 04:25:43.000000 toori-1.1.0/toori.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      467 2023-05-03 04:25:44.000000 toori-1.1.0/toori.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 04:25:43.000000 toori-1.1.0/toori.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-03 04:25:43.000000 toori-1.1.0/toori.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 04:25:43.000000 toori-1.1.0/toori.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       24 2023-05-03 04:25:43.000000 toori-1.1.0/toori.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-03 04:25:43.000000 toori-1.1.0/toori.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 04:30:00.000000 toori-1.1.1/
+-rw-rw-rw-   0        0        0     1442 2023-05-03 04:30:00.000000 toori-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2023-05-03 04:29:14.000000 toori-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 04:30:00.000000 toori-1.1.1/external/
+drwxrwxrwx   0        0        0        0 2023-05-03 04:30:00.000000 toori-1.1.1/external/WinDivert-2.2.2-A/
+drwxrwxrwx   0        0        0        0 2023-05-03 04:30:00.000000 toori-1.1.1/external/WinDivert-2.2.2-A/include/
+-rw-rw-rw-   0        0        0    20671 2023-05-03 04:29:14.000000 toori-1.1.1/external/WinDivert-2.2.2-A/include/windivert.h
+drwxrwxrwx   0        0        0        0 2023-05-03 04:30:00.000000 toori-1.1.1/external/WinDivert-2.2.2-A/x64/
+-rw-rw-rw-   0        0        0    47616 2023-05-03 04:29:14.000000 toori-1.1.1/external/WinDivert-2.2.2-A/x64/WinDivert.dll
+-rw-rw-rw-   0        0        0    25422 2023-05-03 04:29:14.000000 toori-1.1.1/external/WinDivert-2.2.2-A/x64/WinDivert.lib
+-rw-rw-rw-   0        0        0    94144 2023-05-03 04:29:14.000000 toori-1.1.1/external/WinDivert-2.2.2-A/x64/WinDivert64.sys
+-rw-rw-rw-   0        0        0      120 2023-05-03 04:29:14.000000 toori-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 04:30:00.000000 toori-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2241 2023-05-03 04:29:14.000000 toori-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 04:30:00.000000 toori-1.1.1/toori/
+-rw-rw-rw-   0        0        0      504 2023-05-03 04:29:14.000000 toori-1.1.1/toori/console.py
+-rw-rw-rw-   0        0        0     3578 2023-05-03 04:29:14.000000 toori-1.1.1/toori/main.cpp
+-rw-rw-rw-   0        0        0     2167 2023-05-03 04:29:14.000000 toori-1.1.1/toori/main.py
+drwxrwxrwx   0        0        0        0 2023-05-03 04:30:00.000000 toori-1.1.1/toori.egg-info/
+-rw-rw-rw-   0        0        0     1442 2023-05-03 04:30:00.000000 toori-1.1.1/toori.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2023-05-03 04:30:00.000000 toori-1.1.1/toori.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 04:30:00.000000 toori-1.1.1/toori.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-03 04:30:00.000000 toori-1.1.1/toori.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 04:30:00.000000 toori-1.1.1/toori.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2023-05-03 04:30:00.000000 toori-1.1.1/toori.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 04:30:00.000000 toori-1.1.1/toori.egg-info/top_level.txt
```

### Comparing `toori-1.1.0/PKG-INFO` & `toori-1.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toori
-Version: 1.1.0
+Version: 1.1.1
 Summary: A minimal layer 3 tunnel over http(s).
 Home-page: https://github.com/kokseen1/toori
 License: UNKNOWN
 Description: # ![icon](https://github.com/kokseen1/toori/blob/master/toori/icon.png?raw=true) toori 
         
         [![PyPI Release](https://github.com/kokseen1/toori/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/toori/actions/workflows/release.yml)
         [![PyPI Version](https://img.shields.io/pypi/v/toori.svg)](https://pypi.python.org/pypi/toori/)
```

### Comparing `toori-1.1.0/README.md` & `toori-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `toori-1.1.0/external/WinDivert-2.2.2-A/include/windivert.h` & `toori-1.1.1/external/WinDivert-2.2.2-A/include/windivert.h`

 * *Files identical despite different names*

### Comparing `toori-1.1.0/external/WinDivert-2.2.2-A/x64/WinDivert.dll` & `toori-1.1.1/external/WinDivert-2.2.2-A/x64/WinDivert.dll`

 * *Files identical despite different names*

### Comparing `toori-1.1.0/external/WinDivert-2.2.2-A/x64/WinDivert.lib` & `toori-1.1.1/external/WinDivert-2.2.2-A/x64/WinDivert.lib`

 * *Files identical despite different names*

### Comparing `toori-1.1.0/external/WinDivert-2.2.2-A/x64/WinDivert64.sys` & `toori-1.1.1/external/WinDivert-2.2.2-A/x64/WinDivert64.sys`

 * *Files identical despite different names*

### Comparing `toori-1.1.0/setup.py` & `toori-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 2e73 6574 7570 5f68 656c 7065 7273 2069  .setup_helpers i
 00000050: 6d70 6f72 7420 5079 6269 6e64 3131 4578  mport Pybind11Ex
 00000060: 7465 6e73 696f 6e2c 2062 7569 6c64 5f65  tension, build_e
 00000070: 7874 0d0a 6672 6f6d 2073 6574 7570 746f  xt..from setupto
 00000080: 6f6c 7320 696d 706f 7274 2073 6574 7570  ols import setup
 00000090: 0d0a 696d 706f 7274 2070 6174 686c 6962  ..import pathlib
 000000a0: 0d0a 0d0a 5f5f 7665 7273 696f 6e5f 5f20  ....__version__ 
-000000b0: 3d20 2231 2e31 2e30 220d 0a0d 0a23 2054  = "1.1.0"....# T
+000000b0: 3d20 2231 2e31 2e31 220d 0a0d 0a23 2054  = "1.1.1"....# T
 000000c0: 6865 206d 6169 6e20 696e 7465 7266 6163  he main interfac
 000000d0: 6520 6973 2074 6872 6f75 6768 2050 7962  e is through Pyb
 000000e0: 696e 6431 3145 7874 656e 7369 6f6e 2e0d  ind11Extension..
 000000f0: 0a23 202a 2059 6f75 2063 616e 2061 6464  .# * You can add
 00000100: 2063 7878 5f73 7464 3d31 312f 3134 2f31   cxx_std=11/14/1
 00000110: 372c 2061 6e64 2074 6865 6e20 6275 696c  7, and then buil
 00000120: 645f 6578 7420 6361 6e20 6265 2072 656d  d_ext can be rem
```

### Comparing `toori-1.1.0/toori/main.cpp` & `toori-1.1.1/toori/main.cpp`

 * *Files identical despite different names*

### Comparing `toori-1.1.0/toori/main.py` & `toori-1.1.1/toori/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,14 @@
 def start(address, filter_string=None, requested_ip=None, no_dns=False):
     base_filter = f"outbound && !loopback && ip.DstAddr != {resolve_address(address)}"
 
     if filter_string is None:
         filter_string = f"ip"
 
     if no_dns:
-        filter_string += f"&& (tcp || udp.DstPort != 53 || icmp)"
+        filter_string += f" && (tcp || udp.DstPort != 53 || icmp)"
 
     try:
         loop.run_until_complete(start_client(address, requested_ip, f"{base_filter} && {filter_string}"))
     except KeyboardInterrupt:
         _toori.stop()
         print("Exited, have a nice day :)")
```

### Comparing `toori-1.1.0/toori.egg-info/PKG-INFO` & `toori-1.1.1/toori.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toori
-Version: 1.1.0
+Version: 1.1.1
 Summary: A minimal layer 3 tunnel over http(s).
 Home-page: https://github.com/kokseen1/toori
 License: UNKNOWN
 Description: # ![icon](https://github.com/kokseen1/toori/blob/master/toori/icon.png?raw=true) toori 
         
         [![PyPI Release](https://github.com/kokseen1/toori/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/toori/actions/workflows/release.yml)
         [![PyPI Version](https://img.shields.io/pypi/v/toori.svg)](https://pypi.python.org/pypi/toori/)
```

