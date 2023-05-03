# Comparing `tmp/serprog-0.2.1.tar.gz` & `tmp/serprog-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serprog-0.2.1.tar", last modified: Wed Mar 22 06:57:49 2023, max compression
+gzip compressed data, was "serprog-0.3.0.tar", last modified: Wed May  3 16:31:42 2023, max compression
```

## Comparing `serprog-0.2.1.tar` & `serprog-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 06:57:49.658104 serprog-0.2.1/
--rw-rw-rw-   0        0        0     1155 2023-03-13 05:04:07.000000 serprog-0.2.1/LICENSE
--rw-rw-rw-   0        0        0       89 2023-03-09 08:05:57.000000 serprog-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      740 2023-03-22 06:57:49.655104 serprog-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-03-09 08:22:17.000000 serprog-0.2.1/README.md
--rw-rw-rw-   0        0        0       36 2023-03-09 07:50:46.000000 serprog-0.2.1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-03-22 06:57:49.596262 serprog-0.2.1/serprog/
--rw-rw-rw-   0        0        0      133 2023-03-22 06:54:36.000000 serprog-0.2.1/serprog/__init__.py
--rw-rw-rw-   0        0        0      980 2023-03-13 09:19:30.000000 serprog-0.2.1/serprog/__main__.py
--rw-rw-rw-   0        0        0     3943 2023-03-08 08:49:02.000000 serprog-0.2.1/serprog/bootprotocol.py
--rw-rw-rw-   0        0        0     3553 2023-03-22 06:30:07.000000 serprog-0.2.1/serprog/business.py
--rw-rw-rw-   0        0        0     6454 2023-03-22 06:29:18.000000 serprog-0.2.1/serprog/cmdline.py
--rw-rw-rw-   0        0        0     1216 2023-03-22 03:15:41.000000 serprog-0.2.1/serprog/device.py
--rw-rw-rw-   0        0        0      887 2023-03-04 08:11:44.000000 serprog-0.2.1/serprog/exceptions.py
--rw-rw-rw-   0        0        0     5864 2023-03-13 09:12:07.000000 serprog-0.2.1/serprog/ihex.py
--rw-rw-rw-   0        0        0    21924 2023-03-22 06:49:49.000000 serprog-0.2.1/serprog/loader.py
-drwxrwxrwx   0        0        0        0 2023-03-22 06:57:49.646130 serprog-0.2.1/serprog.egg-info/
--rw-rw-rw-   0        0        0      740 2023-03-22 06:57:49.000000 serprog-0.2.1/serprog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-03-22 06:57:49.000000 serprog-0.2.1/serprog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 06:57:49.000000 serprog-0.2.1/serprog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-03-22 06:57:49.000000 serprog-0.2.1/serprog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-22 06:36:46.000000 serprog-0.2.1/serprog.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2023-03-22 06:57:49.000000 serprog-0.2.1/serprog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-22 06:57:49.000000 serprog-0.2.1/serprog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 06:57:49.659095 serprog-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      858 2023-03-09 08:18:44.000000 serprog-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 06:57:49.650133 serprog-0.2.1/test/
--rw-rw-rw-   0        0        0     5405 2023-03-13 09:02:42.000000 serprog-0.2.1/test/test_ihex.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:31:42.950154 serprog-0.3.0/
+-rw-rw-rw-   0        0        0     1155 2023-03-13 05:04:07.000000 serprog-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       89 2023-03-09 08:05:57.000000 serprog-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2378 2023-05-03 16:31:42.949158 serprog-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2081 2023-05-03 16:31:24.000000 serprog-0.3.0/README.md
+-rw-rw-rw-   0        0        0       36 2023-03-09 07:50:46.000000 serprog-0.3.0/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 16:31:42.913255 serprog-0.3.0/serprog/
+-rw-rw-rw-   0        0        0      133 2023-05-03 16:25:42.000000 serprog-0.3.0/serprog/__init__.py
+-rw-rw-rw-   0        0        0      980 2023-03-13 09:19:30.000000 serprog-0.3.0/serprog/__main__.py
+-rw-rw-rw-   0        0        0     3889 2023-04-04 12:44:15.000000 serprog-0.3.0/serprog/bootprotocol.py
+-rw-rw-rw-   0        0        0     3504 2023-04-04 12:25:17.000000 serprog-0.3.0/serprog/business.py
+-rw-rw-rw-   0        0        0     6454 2023-03-22 06:29:18.000000 serprog-0.3.0/serprog/cmdline.py
+-rw-rw-rw-   0        0        0     1168 2023-04-04 12:25:17.000000 serprog-0.3.0/serprog/device.py
+-rw-rw-rw-   0        0        0      887 2023-03-04 08:11:44.000000 serprog-0.3.0/serprog/exceptions.py
+-rw-rw-rw-   0        0        0     6218 2023-05-03 16:22:17.000000 serprog-0.3.0/serprog/ihex.py
+-rw-rw-rw-   0        0        0    21924 2023-03-22 14:10:07.000000 serprog-0.3.0/serprog/loader.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:31:42.947186 serprog-0.3.0/serprog.egg-info/
+-rw-rw-rw-   0        0        0     2378 2023-05-03 16:31:42.000000 serprog-0.3.0/serprog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-05-03 16:31:42.000000 serprog-0.3.0/serprog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 16:31:42.000000 serprog-0.3.0/serprog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-03 16:31:42.000000 serprog-0.3.0/serprog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-03-22 06:36:46.000000 serprog-0.3.0/serprog.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-05-03 16:31:42.000000 serprog-0.3.0/serprog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 16:31:42.000000 serprog-0.3.0/serprog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 16:31:42.950154 serprog-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      858 2023-03-09 08:18:44.000000 serprog-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:31:42.948160 serprog-0.3.0/test/
+-rw-rw-rw-   0        0        0     6135 2023-05-03 16:19:34.000000 serprog-0.3.0/test/test_ihex.py
```

### Comparing `serprog-0.2.1/LICENSE` & `serprog-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `serprog-0.2.1/serprog/__main__.py` & `serprog-0.3.0/serprog/__main__.py`

 * *Files identical despite different names*

### Comparing `serprog-0.2.1/serprog/bootprotocol.py` & `serprog-0.3.0/serprog/bootprotocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,37 +101,31 @@
         return self._isDone
 
     def isError(self):
         return self._isError
 
     def getPacket(self):
         if self.isDone():
-            res = {
-                'command': self._command,
-                'data': self._data
-            }
+            res = {'command': self._command, 'data': self._data}
             self._isDone = False
         else:
-            res = {
-                'command': None,
-                'data': b''
-            }
+            res = {'command': None, 'data': b''}
         return res
 
 def encode(cmd: Union[int, CMD], data: bytes) -> bytes:
     """Encode command, data to a package.
     
     Args:
         cmd (Union[int, Command]): Command in the package.
         data (bytes): Data in the package.
     
     Returns:
         bytes: Package as bytes.
     """
 
-    res  = bytes()
-    res += HEADER
-    res += cmd.to_bytes(1, 'little')
-    res += len(data).to_bytes(2, 'big')
-    res += data
-    res += (sum(data) % 256).to_bytes(1, 'little')
-    return res
+    header   = HEADER
+    command  = cmd.to_bytes(1, 'little')
+    length   = len(data).to_bytes(2, 'big')
+    checksum = (sum(data) % 256).to_bytes(1, 'little')
+
+    payload = header + command + length + data + checksum
+    return payload
```

### Comparing `serprog-0.2.1/serprog/business.py` & `serprog-0.3.0/serprog/business.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,39 +10,37 @@
 import serial.tools.list_ports
 
 import progressbar
 import serial
 import sys
 
 def do_print_devices(args):
-    s  = "Available device list:\n"
-    s += "    device name   \t num \t note\n"
-    for dev in device.device_list:
-        s += "  - {0:11s}  \t {1:4s}\t {2}\n".format(
-            dev['name'], str(dev['dev_type']), dev['note'])
-
-    print(s)
+    print("Available device list:")
+    print("    device name   \t num \t note")
+    print("-" * 40)
+    devices = [f"  - {dev['name']:11s}  \t {dev['dev_type']:4}\t {dev['note']}" for dev in device.device_list]
+    print('\n'.join(devices))
 
 def do_print_ports(args):
     for (port, desc, hwid) in serial.tools.list_ports.comports():
-        print("{:20}".format(port))
-        print("    desc: {}".format(desc))
-        print("    hwid: {}".format(hwid))
+        print(f"{port:20}")
+        print(f"    desc: {desc}")
+        print(f"    hwid: {hwid}")
 
 def do_prog(args):
 
     # Create Serial object
     ser = serial.Serial()
     ser.port = args.port
     ser.baudrate = 115200
     ser.timeout = 1
     try:
         ser.open()
     except:
-        print('ERROR: {0} has been opened by another application.'.format(args.port))
+        print(f"ERROR: {args.port} has been opened by another application.")
         sys.exit(1)
 
     is_prog_flash     = bool(args.flash_file)
     is_ext_flash      = bool(args.ext_flash_file)
     is_prog_eeprom    = bool(args.eeprom_file)
     is_ext_flash_boot = bool(args.ext_flash_boot)
 
@@ -67,28 +65,31 @@
         sys.exit(1)
     except exceptions.CheckDeviceError as e:
         print("ERROR: Device is not match.")
         print("       Assigned device is '{0:s}'".format(device.device_list[e.in_dev]['name']))
         print("       Detected device is '{0:s}'".format(device.device_list[e.real_dev]['name']))
         sys.exit(1)
 
-    print("Device is '{0:s}'".format(device.device_list[l.device_type]['name']))
-    print('Flash hex size is {0:0.2f} KB ({1} bytes)'.format(l.flash_size/1024, l.flash_size))
-    print('Externel Flash hex size is {0:0.2f} KB ({1} bytes)'.format(l.ext_flash_size/1024, l.ext_flash_size))
-    print('EEPROM hex size is {0} bytes.'.format(l.eeprom_size))
-    print('Estimated time  is {0:0.2f} s.'.format(l.prog_time))
+    print(f"Device is '{device.device_list[l.device_type]['name']}'")
+    print(f"Flash hex size is {l.flash_size/1024:.2f} KB ({l.flash_size} bytes)")
+    print(f"Externel Flash hex size is {l.ext_flash_size/1024:.2f} KB ({l.ext_flash_size} bytes)")
+    print(f"EEPROM hex size is {l.eeprom_size} bytes.")
+    print(f"Estimated time  is {l.prog_time:.2f} s.")
 
+    # Progress bar
     widgets = [
         ' [', progressbar.Timer('Elapsed Time: %(seconds)0.2fs', ), '] ',
         progressbar.Bar(),
         progressbar.Counter(format='%(percentage)0.2f%%'),
     ]
 
     bar = progressbar.ProgressBar(max_value=l.total_steps, widgets=widgets)
     bar.update(0)
+
+    # Program device
     for i in range(l.total_steps):
         try:
             l.do_step()
             bar.update(i)
         except exceptions.ComuError:
             print("ERROR: Can't communicate with the device.")
             print("Please check the comport is correct.")
```

### Comparing `serprog-0.2.1/serprog/cmdline.py` & `serprog-0.3.0/serprog/cmdline.py`

 * *Files identical despite different names*

### Comparing `serprog-0.2.1/serprog/device.py` & `serprog-0.3.0/serprog/device.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,16 +35,14 @@
 
     Args:
         s (str): String. Device name, device number are accepted.
 
     Returns:
         int: Device number. If returned -1, it failed. (wrong format s)
     """
-    if s.isdigit():
-        for d in device_list:
+    for d in device_list:
+        if s.isdigit():
             if int(s) == d['dev_type']:
                 return d['dev_type']
-    else:
-        for d in device_list:
-            if s == d['name']:
-                return d['dev_type']
+        elif s == d['name']:
+            return d['dev_type']
     return -1
```

### Comparing `serprog-0.2.1/serprog/exceptions.py` & `serprog-0.3.0/serprog/exceptions.py`

 * *Files identical despite different names*

### Comparing `serprog-0.2.1/serprog/ihex.py` & `serprog-0.3.0/serprog/ihex.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,15 +35,17 @@
     START_SEG_ADDR_RECORD = 3
     EXT_LINEAR_ADDR_RECORD = 4
     START_LINEAR_ADDR_RECORD = 5
 
     with open(filename, 'r') as hexfile:
         sections = []
         section_index = 0
-        extended_address = 0
+        extend_address = 0
+        extend_seg_address = 0
+        extend_lin_address = 0
         eof_flag = False
 
         for line in hexfile.readlines():
             # line is end up with '\n'
             if len(line) < 12:
                 # less than minimum length of General Record Format
                 raise exceptions.IhexFormatError(filename)
@@ -65,52 +67,59 @@
                 else:
                     data = bytearray.fromhex(line[9 : 9 + record_length*2])
             else:
                 data = b''
 
             if record_type == DATA_RECORD:
                 # Data record
+                # 32-bit extended address
+                if extend_seg_address != 0:
+                    extend_address = extend_seg_address << 4
+                elif extend_lin_address != 0:
+                    extend_address = extend_lin_address << 16
+
                 if section_index == 0:
                     # First section
                     sections.append({
-                        'address': (extended_address << 16) + address,
+                        'address': extend_address + address,
                         'data': data
                     })
                     section_index += 1
 
-                elif (extended_address << 16) + address == sections[section_index-1]['address'] + len(sections[section_index-1]['data']):
+                elif extend_address + address == sections[section_index-1]['address'] + len(sections[section_index-1]['data']):
                     # Add data to previous section
                     sections[section_index-1]['data'] += data
 
                 else:
                     # Start new section
                     sections.append({
-                        'address': (extended_address << 16) + address,
+                        'address': extend_address + address,
                         'data': data
                     })
                     section_index += 1
 
             elif record_type == EOF_RECORD:
                 # End of file record
                 if address == 0:
                     eof_flag = True
                 else:
                     raise exceptions.IhexFormatError(filename)
 
             elif record_type == EXT_SEG_ADDR_RECORD:
                 # Extended Segment Address
+                extend_seg_address = int(line[9:13], 16)
                 pass
 
             elif record_type == START_SEG_ADDR_RECORD:
                 # Start Segment Address
                 pass
 
             elif record_type == EXT_LINEAR_ADDR_RECORD:
                 # Extended Linear Address
-                extended_address = int(line[9:13], 16)
+                extend_lin_address = int(line[9:13], 16)
                 pass
 
             elif record_type == START_LINEAR_ADDR_RECORD:
                 # Start Linear Address
                 pass
 
         if not eof_flag:
```

### Comparing `serprog-0.2.1/serprog/loader.py` & `serprog-0.3.0/serprog/loader.py`

 * *Files identical despite different names*

### Comparing `serprog-0.2.1/setup.py` & `serprog-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `serprog-0.2.1/test/test_ihex.py` & `serprog-0.3.0/test/test_ihex.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     # test_ihex_file = datadir.join('ihex2.hex')
     real = ihex.parse('test/ihex2.hex')
     # print(real)
     assert(real == predict)
 
 
 def test_ihex_parse_3():
-    """測試分析有擴展位址ihex檔案
+    """測試分析有擴展位址ihex檔案 (Extended Linear Address, record type '04')
     第一段無擴展，高2位元組為0x0000
     第二段有擴展，高2位元組為0xABCD
     """
     predict = [
         {
             'address': 0x00000000,
             'data': b'\x00\x01\x02\x03\x04\x05\x06\x07\x08\x09\x0A\x0B\x0C\x0D\x0E\x0F'
@@ -77,14 +77,35 @@
     ]
 
     # test_ihex_file = datadir.join('ihex3.hex')
     real = ihex.parse('test/ihex3.hex')
     # print(real)
     assert(real == predict)
 
+def test_ihex_parse_4():
+    """測試分析有擴展位址ihex檔案 (Extended Segment Address, record type '02')
+    第一段無擴展，高2位元組為0x0000
+    第二段有擴展，高2位元組為0xABCD
+    """
+    predict = [
+        {
+            'address': 0x00000000,
+            'data': b'\x00\x01\x02\x03\x04\x05\x06\x07\x08\x09\x0A\x0B\x0C\x0D\x0E\x0F'
+        },
+        {
+            'address': 0x000ABDD0,
+            'data': b'\x00\x01\x02\x03\x04\x05\x06\x07\x08\x09\x0A\x0B\x0C\x0D\x0E\x0F'
+        }
+    ]
+
+    # test_ihex_file = datadir.join('ihex4.hex')
+    real = ihex.parse('test/ihex4.hex')
+    # print(real)
+    assert(real == predict)
+
 
 def test_ihex_padding_1():
     """測試補其空白函式，補其單頁
     """
     input = [
         {
             'address': 0,
```

