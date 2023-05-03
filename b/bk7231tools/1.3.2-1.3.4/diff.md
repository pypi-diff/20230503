# Comparing `tmp/bk7231tools-1.3.2.tar.gz` & `tmp/bk7231tools-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk7231tools-1.3.2.tar", max compression
+gzip compressed data, was "bk7231tools-1.3.4.tar", max compression
```

## Comparing `bk7231tools-1.3.2.tar` & `bk7231tools-1.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1083 2023-03-28 19:37:53.549803 bk7231tools-1.3.2/LICENSE
--rwxr-xr-x   0        0        0       26 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/__init__.py
--rw-r--r--   0        0        0    19995 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/__main__.py
--rw-r--r--   0        0        0        0 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/analysis/__init__.py
--rw-r--r--   0        0        0      570 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/analysis/crc16.py
--rw-r--r--   0        0        0      707 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/analysis/flash.py
--rw-r--r--   0        0        0     6033 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/analysis/goto.py
--rw-r--r--   0        0        0     6209 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/analysis/rbl.py
--rw-r--r--   0        0        0    10535 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/analysis/storage.py
--rw-r--r--   0        0        0      257 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/analysis/utils.py
--rw-r--r--   0        0        0        0 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/crypto/__init__.py
--rw-r--r--   0        0        0     5803 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/crypto/code.py
--rw-r--r--   0        0        0      128 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/crypto/util.py
--rw-r--r--   0        0        0     5402 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/serial/__init__.py
--rw-r--r--   0        0        0     4946 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/serial/cmd_chip.py
--rw-r--r--   0        0        0     7063 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/serial/cmd_flash.py
--rw-r--r--   0        0        0     5942 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/serial/packets.py
--rw-r--r--   0        0        0     8106 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/serial/protocol.py
--rw-r--r--   0        0        0      140 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/bk7231tools/serial/utils.py
--rw-r--r--   0        0        0      604 2023-03-28 19:37:53.553803 bk7231tools-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 bk7231tools-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/LICENSE
+-rwxr-xr-x   0        0        0       26 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/__init__.py
+-rw-r--r--   0        0        0    20269 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/analysis/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/analysis/crc16.py
+-rw-r--r--   0        0        0      707 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/analysis/flash.py
+-rw-r--r--   0        0        0     6033 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/analysis/goto.py
+-rw-r--r--   0        0        0     6209 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/analysis/rbl.py
+-rw-r--r--   0        0        0    10697 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/analysis/storage.py
+-rw-r--r--   0        0        0      257 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/analysis/utils.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/crypto/__init__.py
+-rw-r--r--   0        0        0     5803 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/crypto/code.py
+-rw-r--r--   0        0        0      128 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/crypto/util.py
+-rw-r--r--   0        0        0     5402 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/serial/__init__.py
+-rw-r--r--   0        0        0     4946 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/serial/cmd_chip.py
+-rw-r--r--   0        0        0     7112 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/serial/cmd_flash.py
+-rw-r--r--   0        0        0     6068 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/serial/packets.py
+-rw-r--r--   0        0        0     8106 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/serial/protocol.py
+-rw-r--r--   0        0        0      140 2023-05-03 11:32:06.596855 bk7231tools-1.3.4/bk7231tools/serial/utils.py
+-rw-r--r--   0        0        0      604 2023-05-03 11:32:06.600855 bk7231tools-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 bk7231tools-1.3.4/PKG-INFO
```

### Comparing `bk7231tools-1.3.2/LICENSE` & `bk7231tools-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.2/bk7231tools/__main__.py` & `bk7231tools-1.3.4/bk7231tools/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,21 @@
             print("\t- failed to decrypt!")
             break
         keys = storage.find_all_keys()
         print(f"\t{pos:#06x}: {storage.length // 1024:d} KiB - {len(keys)} keys")
         print("\n".join(f"\t- '{key}'" for key in keys))
         if args.extract:
             storage.extract_all(output_directory, separate_keys=args.storage)
+            filepath = __generate_payload_output_file_path(
+                dumpfile=dumpfile,
+                payload_name="storage",
+                output_directory=output_directory,
+                extra_tag="decrypted",
+            )
+            storage.save(filepath)
         break
 
     if not args.extract:
         # no more work to do, upk can't be searched without app code
         return
 
     upk = None
```

### Comparing `bk7231tools-1.3.2/bk7231tools/analysis/crc16.py` & `bk7231tools-1.3.4/bk7231tools/analysis/crc16.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.2/bk7231tools/analysis/flash.py` & `bk7231tools-1.3.4/bk7231tools/analysis/flash.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.2/bk7231tools/analysis/goto.py` & `bk7231tools-1.3.4/bk7231tools/analysis/goto.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.2/bk7231tools/analysis/rbl.py` & `bk7231tools-1.3.4/bk7231tools/analysis/rbl.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.2/bk7231tools/analysis/storage.py` & `bk7231tools-1.3.4/bk7231tools/analysis/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,18 @@
     crc_calc = out & 0xFFFFFFFF
     if crc_read != crc_calc:
         print(f"\t- invalid CRC: read {crc_read:08x}, calculated {crc_calc:08x}")
         return False
     return True
 
 
-def check_magic(expected: int, found: int) -> bool:
-    if expected != found:
-        print(f"\t- invalid magic: expected {expected:08x}, found {found:08x}")
+def check_magic(found: int, *expected: int) -> bool:
+    if found not in expected:
+        expected = [f"{e:08x}" for e in expected]
+        print(f"\t- invalid magic: expected {expected}, found {found:08x}")
         return False
     return True
 
 
 class TuyaStorage:
     data: bytearray
     indexes: dict
@@ -132,14 +133,18 @@
             return None
         self.data = filedata[pos: pos + self.flash_sz + self.swap_flash_sz]
         self.data = bytearray(self.data)
         if len(self.data) != self.flash_sz + self.swap_flash_sz:
             return None
         return pos
 
+    def save(self, file: str):
+        with open(file, "wb") as f:
+            f.write(self.data)
+
     def block(self, i: int, new: bytearray = None) -> bytearray:
         if new:
             self.data[i * self.block_sz: (i + 1) * self.block_sz] = new
             return new
         return self.data[i * self.block_sz: (i + 1) * self.block_sz]
 
     def page(self, ib: int, ip: int, size: int = 0) -> bytearray:
@@ -155,25 +160,25 @@
                 "PyCryptodomex dependency is required for storage decryption. "
                 "Install it with: pip install pycryptodomex"
             )
 
         aes = AES.new(KEY_MASTER, AES.MODE_ECB)
         master = self.block(0, aes.decrypt(self.block(0)))
         magic, crc, key = unpack("<II16s", master[0:24])
-        if not check_magic(0x13579753, magic):
+        if not check_magic(magic, 0x13579753):
             return False
         if not check_crc(crc, key):
             return False
 
         key = self.make_inner_key(key)
         aes = AES.new(key, AES.MODE_ECB)
         for i in range(self.block_nums):
             block = self.block(i + 1, aes.decrypt(self.block(i + 1)))
             magic, crc, _ = unpack("<IIH", block[0:10])
-            if not check_magic(0x98761234, magic):
+            if not check_magic(magic, 0x98761234, 0x135726AB):
                 return False
             if not check_crc(crc, block[8:]):
                 return False
         return True
 
     def find_all_keys(self) -> List[str]:
         # go through all elements, trying to find one that doesn't exist
```

### Comparing `bk7231tools-1.3.2/bk7231tools/crypto/code.py` & `bk7231tools-1.3.4/bk7231tools/crypto/code.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.2/bk7231tools/serial/__init__.py` & `bk7231tools-1.3.4/bk7231tools/serial/__init__.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.2/bk7231tools/serial/cmd_chip.py` & `bk7231tools-1.3.4/bk7231tools/serial/cmd_chip.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.2/bk7231tools/serial/cmd_flash.py` & `bk7231tools-1.3.4/bk7231tools/serial/cmd_flash.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,21 +158,21 @@
 
     def flash_read_sr(self, size: int = 1) -> int:
         sr = self.flash_read_reg8(0x05)
         if size == 2:
             sr |= self.flash_read_reg8(0x35) << 8
         return sr
 
-    def flash_write_sr(self, sr: int, size: int = 1):
+    def flash_write_sr(self, sr: int, size: int = 1, mask: int = 0xFFFF):
         if size == 1:
             self.flash_write_reg8(0x01, sr)
         else:
             self.flash_write_reg16(0x01, sr)
         sr_read = self.flash_read_sr(size)
-        if sr != sr_read:
+        if (sr & mask) != (sr_read & mask):
             raise RuntimeError(
                 f"Writing Status Register failed: wrote 0x{sr:04X}, got 0x{sr_read:04X}"
             )
 
     def flash_read_id(self, cmd: int = 0x9F) -> dict:
         self.flash_id = self.flash_id or bytes(self.flash_read_reg24(cmd))
         return dict(
@@ -196,15 +196,15 @@
     def flash_unprotect(self, mask: int = 0b01111100):
         flash_id: bytes = self.flash_read_id()["id"]
         if flash_id not in self.FLASH_SR_SIZE:
             raise ValueError(f"Flash ID not known: {flash_id.hex()}")
         sr_size = self.FLASH_SR_SIZE[flash_id]
         sr = self.flash_read_sr(size=sr_size)
         sr &= ~mask
-        self.flash_write_sr(sr, size=sr_size)
+        self.flash_write_sr(sr, size=sr_size, mask=mask)
 
     def flash_erase_block(
         self,
         start: int,
         size: EraseSize,
         dry_run: bool = False,
     ):
```

### Comparing `bk7231tools-1.3.2/bk7231tools/serial/packets.py` & `bk7231tools-1.3.4/bk7231tools/serial/packets.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,22 @@
 class BkLinkCheckResp(Packet):
     CODE = 0x01  # CMD_LinkCheck + 1
     FORMAT = "B"
     value: int
 
 
 @dataclass
+class BkWriteRegCmnd(Packet):
+    CODE = 0x01  # CMD_WriteReg
+    FORMAT = "<II"
+    address: int
+    value: int
+
+
+@dataclass
 class BkReadRegCmnd(Packet):
     CODE = 0x03  # CMD_ReadReg
     FORMAT = "<I"
     HAS_RESP_OTHER = True
     HAS_RESP_SAME = slice(0, 4)
     address: int
```

### Comparing `bk7231tools-1.3.2/bk7231tools/serial/protocol.py` & `bk7231tools-1.3.4/bk7231tools/serial/protocol.py`

 * *Files identical despite different names*

### Comparing `bk7231tools-1.3.2/pyproject.toml` & `bk7231tools-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bk7231tools"
-version = "1.3.2"
+version = "1.3.4"
 description = "Tools to interact with and analyze artifacts for BK7231 MCUs"
 authors = ["Khaled Nassar <kmhnassar@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pyserial = "^3.5"
```

### Comparing `bk7231tools-1.3.2/PKG-INFO` & `bk7231tools-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bk7231tools
-Version: 1.3.2
+Version: 1.3.4
 Summary: Tools to interact with and analyze artifacts for BK7231 MCUs
 License: MIT
 Author: Khaled Nassar
 Author-email: kmhnassar@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

