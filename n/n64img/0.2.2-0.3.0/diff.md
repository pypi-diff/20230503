# Comparing `tmp/n64img-0.2.2.tar.gz` & `tmp/n64img-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "n64img-0.2.2.tar", last modified: Tue Mar 28 04:47:26 2023, max compression
+gzip compressed data, was "n64img-0.3.0.tar", last modified: Wed May  3 15:13:17 2023, max compression
```

## Comparing `n64img-0.2.2.tar` & `n64img-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 04:47:26.348798 n64img-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-28 04:47:18.000000 n64img-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-28 04:47:26.348798 n64img-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-28 04:47:18.000000 n64img-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 04:47:26.344798 n64img-0.2.2/n64img/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 04:47:18.000000 n64img-0.2.2/n64img/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-03-28 04:47:18.000000 n64img-0.2.2/n64img/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-28 04:47:18.000000 n64img-0.2.2/n64img/iter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 04:47:26.348798 n64img-0.2.2/n64img.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-28 04:47:26.000000 n64img-0.2.2/n64img.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-28 04:47:26.000000 n64img-0.2.2/n64img.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 04:47:26.000000 n64img-0.2.2/n64img.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-28 04:47:26.000000 n64img-0.2.2/n64img.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-28 04:47:26.000000 n64img-0.2.2/n64img.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-28 04:47:18.000000 n64img-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-28 04:47:26.348798 n64img-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 04:47:26.348798 n64img-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 04:47:18.000000 n64img-0.2.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-28 04:47:18.000000 n64img-0.2.2/test/test_endian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-03-28 04:47:18.000000 n64img-0.2.2/test/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:13:17.391980 n64img-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-03 15:13:10.000000 n64img-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 15:13:17.391980 n64img-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-03 15:13:10.000000 n64img-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:13:17.391980 n64img-0.3.0/n64img/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:13:10.000000 n64img-0.3.0/n64img/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-05-03 15:13:10.000000 n64img-0.3.0/n64img/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-03 15:13:10.000000 n64img-0.3.0/n64img/iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:13:17.391980 n64img-0.3.0/n64img.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 15:13:17.000000 n64img-0.3.0/n64img.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-03 15:13:17.000000 n64img-0.3.0/n64img.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:13:17.000000 n64img-0.3.0/n64img.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 15:13:17.000000 n64img-0.3.0/n64img.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 15:13:17.000000 n64img-0.3.0/n64img.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 15:13:10.000000 n64img-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-03 15:13:17.391980 n64img-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:13:17.391980 n64img-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:13:10.000000 n64img-0.3.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-03 15:13:10.000000 n64img-0.3.0/test/test_endian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-03 15:13:10.000000 n64img-0.3.0/test/test_image.py
```

### Comparing `n64img-0.2.2/LICENSE` & `n64img-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `n64img-0.2.2/n64img/image.py` & `n64img-0.3.0/n64img/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,65 @@
 from math import ceil
 from pathlib import Path
-from typing import List, Optional, Tuple
+from typing import List, Literal, Optional, Tuple
 
 import png
 
 from n64img import iter
 
 Palette = List[Tuple[int, int, int, int]]
 
 
 class Image:
     def __init__(self, data: bytes, width: int, height: int):
         self.data: bytes = data
         self.width: int = width
         self.height: int = height
-        self.depth: int = 1
+        self.depth: float = 1
         self.greyscale: bool = False
         self.alpha: bool = False
         self.flip_h: bool = False
         self.flip_v: bool = False
         self.little_endian: bool = False
         self.palette: Optional[Palette] = None
 
     def __str__(self):
         return "Image(width={}, height={}, data={})".format(
             self.width, self.height, self.data
         )
 
+    def set_palette(
+        self, palette_bytes: bytes, endian: Literal["little", "big"] = "big"
+    ) -> None:
+        def unpack_color(data):
+            s = int.from_bytes(data[0:2], endian)
+
+            r = (s >> 11) & 0x1F
+            g = (s >> 6) & 0x1F
+            b = (s >> 1) & 0x1F
+            a = (s & 1) * 0xFF
+
+            r = ceil(0xFF * (r / 31))
+            g = ceil(0xFF * (g / 31))
+            b = ceil(0xFF * (b / 31))
+
+            return r, g, b, a
+
+        palette = []
+
+        for a, b in iter.iter_in_groups(palette_bytes, 2):
+            palette.append(unpack_color([a, b]))
+
+        self.palette = palette
+
     def get_writer(self) -> png.Writer:
         return png.Writer(
             self.width,
             self.height,
-            greyscale=self.greyscale,  # type: ignore
+            greyscale=self.greyscale,
             alpha=self.alpha,
             palette=self.palette,
         )
 
     def parse(self) -> bytes:
         if not self.flip_h and not self.flip_v:
             return self.data
@@ -59,15 +83,15 @@
         width = self.width
         while width > 0:
             # NOTE: rows must be padded to 8-byte boundary
             row = height = width
             remainder = ceil(width * self.depth) % 8
             if remainder != 0:
                 row += ceil((8 - remainder) / self.depth)
-            size += row * height * self.depth
+            size += int(row * height * self.depth)
             width >>= 1
         return size
 
     def size(self) -> int:
         return ceil(self.width * self.height * self.depth)
 
 
@@ -250,27 +274,27 @@
 
     def parse(self) -> bytes:
         img = bytearray()
 
         for x, y, i in iter.iter_image_indexes(
             self.width, self.height, self.depth, self.flip_h, self.flip_v
         ):
-            s = int.from_bytes(self.data[i:i+2], byteorder='big')
+            s = int.from_bytes(self.data[i : i + 2], byteorder="big")
 
             r = (s >> 11) & 0x1F
-            g = (s >>  6) & 0x1F
-            b = (s >>  1) & 0x1F
+            g = (s >> 6) & 0x1F
+            b = (s >> 1) & 0x1F
 
             r = (r << 3) | (r >> 2)
             g = (g << 3) | (g >> 2)
             b = (b << 3) | (b >> 2)
 
             a = 255 * (s & 1)
 
-            img += bytes((r,g,b,a))
+            img += bytes((r, g, b, a))
 
         return bytes(img)
 
 
 class RGBA32(Image):
     def __init__(self, data, width, height):
         super().__init__(data, width, height)
```

### Comparing `n64img-0.2.2/n64img/iter.py` & `n64img-0.3.0/n64img/iter.py`

 * *Files identical despite different names*

### Comparing `n64img-0.2.2/test/test_endian.py` & `n64img-0.3.0/test/test_endian.py`

 * *Files identical despite different names*

### Comparing `n64img-0.2.2/test/test_image.py` & `n64img-0.3.0/test/test_image.py`

 * *Files identical despite different names*

