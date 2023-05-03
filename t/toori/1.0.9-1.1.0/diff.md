# Comparing `tmp/toori-1.0.9.tar.gz` & `tmp/toori-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\toori-1.0.9.tar", last modified: Wed Jan 25 02:30:16 2023, max compression
+gzip compressed data, was "dist\toori-1.1.0.tar", last modified: Wed May  3 04:25:44 2023, max compression
```

## Comparing `toori-1.0.9.tar` & `toori-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 02:30:16.000000 toori-1.0.9/
--rw-rw-rw-   0        0        0     1150 2023-01-25 02:30:16.000000 toori-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-01-25 02:29:34.000000 toori-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-01-25 02:30:16.000000 toori-1.0.9/external/
-drwxrwxrwx   0        0        0        0 2023-01-25 02:30:16.000000 toori-1.0.9/external/WinDivert-2.2.2-A/
-drwxrwxrwx   0        0        0        0 2023-01-25 02:30:16.000000 toori-1.0.9/external/WinDivert-2.2.2-A/include/
--rw-rw-rw-   0        0        0    20671 2023-01-25 02:29:34.000000 toori-1.0.9/external/WinDivert-2.2.2-A/include/windivert.h
-drwxrwxrwx   0        0        0        0 2023-01-25 02:30:16.000000 toori-1.0.9/external/WinDivert-2.2.2-A/x64/
--rw-rw-rw-   0        0        0    47616 2023-01-25 02:29:34.000000 toori-1.0.9/external/WinDivert-2.2.2-A/x64/WinDivert.dll
--rw-rw-rw-   0        0        0    25422 2023-01-25 02:29:34.000000 toori-1.0.9/external/WinDivert-2.2.2-A/x64/WinDivert.lib
--rw-rw-rw-   0        0        0    94144 2023-01-25 02:29:34.000000 toori-1.0.9/external/WinDivert-2.2.2-A/x64/WinDivert64.sys
--rw-rw-rw-   0        0        0      120 2023-01-25 02:29:34.000000 toori-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-25 02:30:16.000000 toori-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2241 2023-01-25 02:29:34.000000 toori-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-25 02:30:16.000000 toori-1.0.9/toori/
--rw-rw-rw-   0        0        0      430 2023-01-25 02:29:34.000000 toori-1.0.9/toori/console.py
--rw-rw-rw-   0        0        0     3198 2023-01-25 02:29:34.000000 toori-1.0.9/toori/main.cpp
--rw-rw-rw-   0        0        0     1731 2023-01-25 02:29:34.000000 toori-1.0.9/toori/main.py
-drwxrwxrwx   0        0        0        0 2023-01-25 02:30:16.000000 toori-1.0.9/toori.egg-info/
--rw-rw-rw-   0        0        0     1150 2023-01-25 02:30:16.000000 toori-1.0.9/toori.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      467 2023-01-25 02:30:16.000000 toori-1.0.9/toori.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-25 02:30:16.000000 toori-1.0.9/toori.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-01-25 02:30:16.000000 toori-1.0.9/toori.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-01-25 02:30:16.000000 toori-1.0.9/toori.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       24 2023-01-25 02:30:16.000000 toori-1.0.9/toori.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-01-25 02:30:16.000000 toori-1.0.9/toori.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/
+-rw-rw-rw-   0        0        0     1442 2023-05-03 04:25:44.000000 toori-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2023-05-03 04:25:02.000000 toori-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/external/
+drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/external/WinDivert-2.2.2-A/
+drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/external/WinDivert-2.2.2-A/include/
+-rw-rw-rw-   0        0        0    20671 2023-05-03 04:25:02.000000 toori-1.1.0/external/WinDivert-2.2.2-A/include/windivert.h
+drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/external/WinDivert-2.2.2-A/x64/
+-rw-rw-rw-   0        0        0    47616 2023-05-03 04:25:02.000000 toori-1.1.0/external/WinDivert-2.2.2-A/x64/WinDivert.dll
+-rw-rw-rw-   0        0        0    25422 2023-05-03 04:25:02.000000 toori-1.1.0/external/WinDivert-2.2.2-A/x64/WinDivert.lib
+-rw-rw-rw-   0        0        0    94144 2023-05-03 04:25:02.000000 toori-1.1.0/external/WinDivert-2.2.2-A/x64/WinDivert64.sys
+-rw-rw-rw-   0        0        0      120 2023-05-03 04:25:02.000000 toori-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 04:25:44.000000 toori-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2241 2023-05-03 04:25:02.000000 toori-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/toori/
+-rw-rw-rw-   0        0        0      504 2023-05-03 04:25:02.000000 toori-1.1.0/toori/console.py
+-rw-rw-rw-   0        0        0     3578 2023-05-03 04:25:02.000000 toori-1.1.0/toori/main.cpp
+-rw-rw-rw-   0        0        0     2166 2023-05-03 04:25:02.000000 toori-1.1.0/toori/main.py
+drwxrwxrwx   0        0        0        0 2023-05-03 04:25:44.000000 toori-1.1.0/toori.egg-info/
+-rw-rw-rw-   0        0        0     1442 2023-05-03 04:25:43.000000 toori-1.1.0/toori.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2023-05-03 04:25:44.000000 toori-1.1.0/toori.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 04:25:43.000000 toori-1.1.0/toori.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-03 04:25:43.000000 toori-1.1.0/toori.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 04:25:43.000000 toori-1.1.0/toori.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2023-05-03 04:25:43.000000 toori-1.1.0/toori.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 04:25:43.000000 toori-1.1.0/toori.egg-info/top_level.txt
```

### Comparing `toori-1.0.9/README.md` & `toori-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# ![icon](https://github.com/kokseen1/Toori/blob/master/toori/icon.png?raw=true) Toori 
+# ![icon](https://github.com/kokseen1/toori/blob/master/toori/icon.png?raw=true) toori 
 
-[![PyPI Release](https://github.com/kokseen1/Toori/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/Toori/actions/workflows/release.yml)
+[![PyPI Release](https://github.com/kokseen1/toori/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/toori/actions/workflows/release.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/toori.svg)](https://pypi.python.org/pypi/toori/)
 
 A minimal layer 3 tunnel over http(s).
 
 ## Prerequisites
 
 - [MSVC Build Tools](https://visualstudio.microsoft.com/downloads/)
@@ -19,11 +19,24 @@
 
 Run as Administrator:
 
 ```shell
 toori <server address>
 ```
 
-e.g.
-```
+### Examples
+
+```shell
 toori https://toori.server
 ```
+
+Don't tunnel DNS requests
+
+```shell
+toori https://toori.server -nd
+```
+
+Only tunnel SSH traffic
+
+```shell
+toori https://toori.server -f "tcp.DstPort == 22"
+```
```

### Comparing `toori-1.0.9/external/WinDivert-2.2.2-A/include/windivert.h` & `toori-1.1.0/external/WinDivert-2.2.2-A/include/windivert.h`

 * *Files identical despite different names*

### Comparing `toori-1.0.9/external/WinDivert-2.2.2-A/x64/WinDivert.dll` & `toori-1.1.0/external/WinDivert-2.2.2-A/x64/WinDivert.dll`

 * *Files identical despite different names*

### Comparing `toori-1.0.9/external/WinDivert-2.2.2-A/x64/WinDivert.lib` & `toori-1.1.0/external/WinDivert-2.2.2-A/x64/WinDivert.lib`

 * *Files identical despite different names*

### Comparing `toori-1.0.9/external/WinDivert-2.2.2-A/x64/WinDivert64.sys` & `toori-1.1.0/external/WinDivert-2.2.2-A/x64/WinDivert64.sys`

 * *Files identical despite different names*

### Comparing `toori-1.0.9/setup.py` & `toori-1.1.0/setup.py`

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
-000000b0: 3d20 2231 2e30 2e39 220d 0a0d 0a23 2054  = "1.0.9"....# T
+000000b0: 3d20 2231 2e31 2e30 220d 0a0d 0a23 2054  = "1.1.0"....# T
 000000c0: 6865 206d 6169 6e20 696e 7465 7266 6163  he main interfac
 000000d0: 6520 6973 2074 6872 6f75 6768 2050 7962  e is through Pyb
 000000e0: 696e 6431 3145 7874 656e 7369 6f6e 2e0d  ind11Extension..
 000000f0: 0a23 202a 2059 6f75 2063 616e 2061 6464  .# * You can add
 00000100: 2063 7878 5f73 7464 3d31 312f 3134 2f31   cxx_std=11/14/1
 00000110: 372c 2061 6e64 2074 6865 6e20 6275 696c  7, and then buil
 00000120: 645f 6578 7420 6361 6e20 6265 2072 656d  d_ext can be rem
@@ -60,15 +60,15 @@
 000003b0: 2057 696e 4469 7665 7274 2e6c 6962 0d0a   WinDivert.lib..
 000003c0: 2020 2020 292c 0d0a 5d0d 0a0d 0a73 6574      ),..]....set
 000003d0: 7570 280d 0a20 2020 206e 616d 653d 2274  up(..    name="t
 000003e0: 6f6f 7269 222c 0d0a 2020 2020 7665 7273  oori",..    vers
 000003f0: 696f 6e3d 5f5f 7665 7273 696f 6e5f 5f2c  ion=__version__,
 00000400: 0d0a 2020 2020 7572 6c3d 2268 7474 7073  ..    url="https
 00000410: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b6f  ://github.com/ko
-00000420: 6b73 6565 6e31 2f54 6f6f 7269 222c 0d0a  kseen1/Toori",..
+00000420: 6b73 6565 6e31 2f74 6f6f 7269 222c 0d0a  kseen1/toori",..
 00000430: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
 00000440: 2241 206d 696e 696d 616c 206c 6179 6572  "A minimal layer
 00000450: 2033 2074 756e 6e65 6c20 6f76 6572 2068   3 tunnel over h
 00000460: 7474 7028 7329 2e22 2c0d 0a20 2020 206c  ttp(s).",..    l
 00000470: 6f6e 675f 6465 7363 7269 7074 696f 6e3d  ong_description=
 00000480: 2870 6174 686c 6962 2e50 6174 6828 5f5f  (pathlib.Path(__
 00000490: 6669 6c65 5f5f 292e 7061 7265 6e74 202f  file__).parent /
```

### Comparing `toori-1.0.9/toori/main.cpp` & `toori-1.1.0/toori/main.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 UINT32 g_clientIpBuf[4];
 std::string g_filter;
 
 void init(std::string filter, std::string localIp)
 {
     g_filter = filter;
 
+    printf("Using filter \"%s\"\n", g_filter.c_str());
+
     handle = WinDivertOpen(g_filter.c_str(), WINDIVERT_LAYER_NETWORK, 0, 0);
     if (handle == INVALID_HANDLE_VALUE)
     {
         auto err = GetLastError();
         fprintf(stderr, "error: failed to open the WinDivert device (%d)\n", err);
         if (err == 5)
             fprintf(stderr, "The calling application does not have Administrator privileges.\n");
@@ -107,15 +109,30 @@
     // {
     //     std::cerr << "WinDivertHelperCalcChecksums failed" << std::endl;
     // }
 
     return py::bytes(packet, packet_len);
 }
 
+void stop()
+{
+    if (handle != INVALID_HANDLE_VALUE)
+    {
+        if (!WinDivertClose(handle))
+        {
+            fprintf(stderr, "error: failed to close the WinDivert device (%d)\n",
+                    GetLastError());
+        }
+    }
+    handle = INVALID_HANDLE_VALUE;
+}
+
 PYBIND11_MODULE(_toori, m)
 {
     m.def("init", &init);
 
     m.def("get", &get);
 
     m.def("inj", &inj);
+
+    m.def("stop", &stop);
 }
```

### Comparing `toori-1.0.9/toori/main.py` & `toori-1.1.0/toori/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,30 +21,39 @@
 def resolve_address(address):
     hostname = address.split("//")[-1:][0]
     ip = socket.gethostbyname(hostname)
 
     return ip
 
 
+@sio.on("message")
+async def print_message(msg):
+    print(msg)
+
+
 @sio.on("connect")
 async def on_connect():
-    print("connected to server")
-    await sio.emit(event="announce_ip", data=LOCAL_IP)
+    print("Connected to server")
 
 
 @sio.on("in")
 async def handle_incoming(data):
     # await loop.run_in_executor(_executor, _toori.inj, data)
     _toori.inj(data)
     # await asyncio.sleep(0.0)
 
 
-async def start_client(address, filter_string):
+async def start_client(address, requested_ip, filter_string):
+    headers = {"req_ip": requested_ip, "loc_ip": LOCAL_IP}
 
-    await sio.connect(f"{address}")
+    try:
+        await sio.connect(f"{address}", auth=headers)
+    except socketio.exceptions.ConnectionError:
+        print(f"Unable to connect to the address {address}")
+        exit()
 
     _toori.init(
         filter_string,
         LOCAL_IP,
     )
 
     while True:
@@ -55,15 +64,21 @@
                 await sio.emit(event="out", data=data)
             except Exception:
                 pass
 
         # await asyncio.sleep(0.0001)
 
 
-def start(address, filter_string=None, no_dns=False):
+def start(address, filter_string=None, requested_ip=None, no_dns=False):
+    base_filter = f"outbound && !loopback && ip.DstAddr != {resolve_address(address)}"
+
     if filter_string is None:
-        filter_string = f"outbound && !loopback && ip.DstAddr != {resolve_address(address)} && ip"
+        filter_string = f"ip"
 
     if no_dns:
-        filter_string = f"{filter_string} || udp.DstPort != 53"
+        filter_string += f"&& (tcp || udp.DstPort != 53 || icmp)"
 
-    loop.run_until_complete(start_client(address, filter_string))
+    try:
+        loop.run_until_complete(start_client(address, requested_ip, f"{base_filter} && {filter_string}"))
+    except KeyboardInterrupt:
+        _toori.stop()
+        print("Exited, have a nice day :)")
```

