# Comparing `tmp/CalSciPy-0.2.3.tar.gz` & `tmp/CalSciPy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalSciPy-0.2.3.tar", last modified: Fri Apr 28 22:03:12 2023, max compression
+gzip compressed data, was "CalSciPy-0.2.4.tar", last modified: Wed May  3 20:02:40 2023, max compression
```

## Comparing `CalSciPy-0.2.3.tar` & `CalSciPy-0.2.4.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 22:03:12.598456 CalSciPy-0.2.3/
--rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     4998 2023-04-28 22:03:12.597450 CalSciPy-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.2.3/README.md
--rw-rw-rw-   0        0        0     2330 2023-04-28 22:02:45.000000 CalSciPy-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-28 22:03:12.598456 CalSciPy-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 22:03:12.549425 CalSciPy-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 22:03:12.570453 CalSciPy-0.2.3/src/CalSciPy/
--rw-rw-rw-   0        0        0      388 2023-04-03 13:04:29.000000 CalSciPy-0.2.3/src/CalSciPy/__init__.py
--rw-rw-rw-   0        0        0    11403 2023-04-05 15:38:36.000000 CalSciPy-0.2.3/src/CalSciPy/bruker.py
--rw-rw-rw-   0        0        0     3028 2023-04-07 16:45:41.000000 CalSciPy-0.2.3/src/CalSciPy/coloring.py
--rw-rw-rw-   0        0        0     2237 2023-04-03 13:04:29.000000 CalSciPy-0.2.3/src/CalSciPy/event_processing.py
--rw-rw-rw-   0        0        0     4621 2023-04-28 22:02:25.000000 CalSciPy-0.2.3/src/CalSciPy/image_processing.py
--rw-rw-rw-   0        0        0     9653 2023-04-26 15:19:07.000000 CalSciPy-0.2.3/src/CalSciPy/io_tools.py
--rw-rw-rw-   0        0        0     5917 2023-04-28 16:24:44.000000 CalSciPy-0.2.3/src/CalSciPy/misc.py
--rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.2.3/src/CalSciPy/reorganization.py
--rw-rw-rw-   0        0        0     4770 2023-03-29 21:13:37.000000 CalSciPy-0.2.3/src/CalSciPy/trace_processing.py
--rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.2.3/src/CalSciPy/version.py
-drwxrwxrwx   0        0        0        0 2023-04-28 22:03:12.579450 CalSciPy-0.2.3/src/CalSciPy.egg-info/
--rw-rw-rw-   0        0        0     4998 2023-04-28 22:03:12.000000 CalSciPy-0.2.3/src/CalSciPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      701 2023-04-28 22:03:12.000000 CalSciPy-0.2.3/src/CalSciPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 22:03:12.000000 CalSciPy-0.2.3/src/CalSciPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      365 2023-04-28 22:03:12.000000 CalSciPy-0.2.3/src/CalSciPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-28 22:03:12.000000 CalSciPy-0.2.3/src/CalSciPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.2.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 22:03:12.595449 CalSciPy-0.2.3/tests/
--rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.2.3/tests/test_a_install.py
--rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.2.3/tests/test_bruker.py
--rw-rw-rw-   0        0        0      887 2023-04-07 16:44:54.000000 CalSciPy-0.2.3/tests/test_coloring.py
--rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.2.3/tests/test_event_processing.py
--rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.2.3/tests/test_io_tools.py
--rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.2.3/tests/test_misc.py
--rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.2.3/tests/test_reorganization.py
--rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.2.3/tests/test_trace_processing.py
+drwxrwxrwx   0        0        0        0 2023-05-03 20:02:40.139025 CalSciPy-0.2.4/
+-rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     4998 2023-05-03 20:02:40.138025 CalSciPy-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.2.4/README.md
+-rw-rw-rw-   0        0        0     2330 2023-05-03 20:02:03.000000 CalSciPy-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 20:02:40.139025 CalSciPy-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 20:02:40.072024 CalSciPy-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 20:02:40.108025 CalSciPy-0.2.4/src/CalSciPy/
+-rw-rw-rw-   0        0        0      388 2023-04-03 13:04:29.000000 CalSciPy-0.2.4/src/CalSciPy/__init__.py
+-rw-rw-rw-   0        0        0    11403 2023-04-05 15:38:36.000000 CalSciPy-0.2.4/src/CalSciPy/bruker.py
+-rw-rw-rw-   0        0        0     3060 2023-05-03 19:59:44.000000 CalSciPy-0.2.4/src/CalSciPy/coloring.py
+-rw-rw-rw-   0        0        0     2237 2023-04-03 13:04:29.000000 CalSciPy-0.2.4/src/CalSciPy/event_processing.py
+-rw-rw-rw-   0        0        0     4621 2023-05-03 19:58:49.000000 CalSciPy-0.2.4/src/CalSciPy/image_processing.py
+-rw-rw-rw-   0        0        0     5914 2023-05-03 20:01:36.000000 CalSciPy-0.2.4/src/CalSciPy/interactive_visuals.py
+-rw-rw-rw-   0        0        0     9653 2023-04-26 15:19:07.000000 CalSciPy-0.2.4/src/CalSciPy/io_tools.py
+-rw-rw-rw-   0        0        0     7557 2023-05-03 19:58:49.000000 CalSciPy-0.2.4/src/CalSciPy/misc.py
+-rw-rw-rw-   0        0        0     3444 2023-03-29 17:06:08.000000 CalSciPy-0.2.4/src/CalSciPy/reorganization.py
+-rw-rw-rw-   0        0        0    10343 2023-05-03 20:01:23.000000 CalSciPy-0.2.4/src/CalSciPy/trace_processing.py
+-rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.2.4/src/CalSciPy/version.py
+drwxrwxrwx   0        0        0        0 2023-05-03 20:02:40.117025 CalSciPy-0.2.4/src/CalSciPy.egg-info/
+-rw-rw-rw-   0        0        0     4998 2023-05-03 20:02:40.000000 CalSciPy-0.2.4/src/CalSciPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-05-03 20:02:40.000000 CalSciPy-0.2.4/src/CalSciPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 20:02:40.000000 CalSciPy-0.2.4/src/CalSciPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      365 2023-05-03 20:02:40.000000 CalSciPy-0.2.4/src/CalSciPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-03 20:02:40.000000 CalSciPy-0.2.4/src/CalSciPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.2.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 20:02:40.136025 CalSciPy-0.2.4/tests/
+-rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.2.4/tests/test_a_install.py
+-rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.2.4/tests/test_bruker.py
+-rw-rw-rw-   0        0        0      887 2023-04-07 16:44:54.000000 CalSciPy-0.2.4/tests/test_coloring.py
+-rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.2.4/tests/test_event_processing.py
+-rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.2.4/tests/test_io_tools.py
+-rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.2.4/tests/test_misc.py
+-rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.2.4/tests/test_reorganization.py
+-rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.2.4/tests/test_trace_processing.py
```

### Comparing `CalSciPy-0.2.3/LICENSE` & `CalSciPy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/PKG-INFO` & `CalSciPy-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.2.3
+Version: 0.2.4
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.2.3/README.md` & `CalSciPy-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/pyproject.toml` & `CalSciPy-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CalSciPy"
-version = "0.2.3"
+version = "0.2.4"
 description = "A collection"
 readme = "README.md"
 requires-python = ">=3.7, <4"
 license = {file = "LICENSE"}
 keywords = ["CalSciPy", "Calcium Imaging"]
 authors = [
   {name = "Darik A. O'Neil"}
```

### Comparing `CalSciPy-0.2.3/src/CalSciPy/bruker.py` & `CalSciPy-0.2.4/src/CalSciPy/bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/src/CalSciPy/coloring.py` & `CalSciPy-0.2.4/src/CalSciPy/coloring.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 import numpy as np
 from functools import cached_property
 
 
+# TODO PASTE AND DOCUMENT ME
+
 class BackgroundImage:
     def __init__(self, images: np.ndarray, style: int = 0, cutoffs: Tuple[float, float] = (0.0, 100.0)):
         self.images = images
         self.style = style
         self.cutoffs = cutoffs
 
     @cached_property
```

### Comparing `CalSciPy-0.2.3/src/CalSciPy/event_processing.py` & `CalSciPy-0.2.4/src/CalSciPy/event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/src/CalSciPy/image_processing.py` & `CalSciPy-0.2.4/src/CalSciPy/image_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/src/CalSciPy/io_tools.py` & `CalSciPy-0.2.4/src/CalSciPy/io_tools.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/src/CalSciPy/misc.py` & `CalSciPy-0.2.4/src/CalSciPy/misc.py`

 * *Files 20% similar despite different names*

```diff
@@ -77,14 +77,54 @@
                 pass  # if all we have left is overlap then it is a perfect segmentation
             else:
                 yield tuple(block)[-idx:]  # if we don't have a full block, we must ensure the number of repeats is
                 # equal to block buffer
             raise StopIteration
 
 
+def generate_overlapping_blocks(sequence: Iterable, block_size: int, block_buffer: int) -> Iterator:
+    if block_size <= 1:
+        raise ValueError("Block size must be > 1")
+    if block_buffer >= block_size:
+        raise AssertionError("Block buffer must be smaller than the size of the block.")
+    if block_size >= len(sequence):
+        raise AssertionError("Block must be smaller than iterable sequence")
+
+    block_size = int(block_size)  # coerce in case float
+
+    block = deque(maxlen=block_size + 2 * block_buffer)
+    iterable = iter(sequence)
+
+    # make nil block
+    for _ in range(block_size + 2 * block_buffer):
+        block.append(0)
+
+    # make first block
+    for _ in range(block_size + block_buffer):
+        block.append(next(iterable))
+
+    while True:
+        try:
+            yield tuple(block)
+            for idx in range(block_size):  # noqa: B007
+                block.append(next(iterable))  # we subtract the block buffer to make space for overlap
+
+        except StopIteration:
+            # noinspection PyUnboundLocalVariable
+            idx += block_buffer  # make sure that we always have at least the overlap
+            if idx == 0:
+                pass  # if we managed a perfect segmentation, then pass to stop iteration
+            elif idx == block_buffer:
+                pass  # if all we have left is overlap then it is a perfect segmentation
+            else:
+                yield tuple(block)[-idx:]  # if we don't have a full block, we must ensure the number of repeats is
+                # equal to block buffer
+            raise StopIteration
+
+
 def generate_padded_filename(output_folder: Path, index: int, base: str = "images", digits: int = 2,
                              ext: str = ".tif") -> Path:
     """
     Generates a pathlib Path whose name is defined as '{base}_{index}{ext}' where index is zero-padded if it
     is not equal to the number of digits
 
     :param output_folder: folder that will contain file
```

### Comparing `CalSciPy-0.2.3/src/CalSciPy/reorganization.py` & `CalSciPy-0.2.4/src/CalSciPy/reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/src/CalSciPy.egg-info/PKG-INFO` & `CalSciPy-0.2.4/src/CalSciPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.2.3
+Version: 0.2.4
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
```

### Comparing `CalSciPy-0.2.3/src/CalSciPy.egg-info/SOURCES.txt` & `CalSciPy-0.2.4/src/CalSciPy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 src/__init__.py
 src/CalSciPy/__init__.py
 src/CalSciPy/bruker.py
 src/CalSciPy/coloring.py
 src/CalSciPy/event_processing.py
 src/CalSciPy/image_processing.py
+src/CalSciPy/interactive_visuals.py
 src/CalSciPy/io_tools.py
 src/CalSciPy/misc.py
 src/CalSciPy/reorganization.py
 src/CalSciPy/trace_processing.py
 src/CalSciPy/version.py
 src/CalSciPy.egg-info/PKG-INFO
 src/CalSciPy.egg-info/SOURCES.txt
```

### Comparing `CalSciPy-0.2.3/tests/test_a_install.py` & `CalSciPy-0.2.4/tests/test_a_install.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/tests/test_bruker.py` & `CalSciPy-0.2.4/tests/test_bruker.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/tests/test_coloring.py` & `CalSciPy-0.2.4/tests/test_coloring.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/tests/test_event_processing.py` & `CalSciPy-0.2.4/tests/test_event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/tests/test_io_tools.py` & `CalSciPy-0.2.4/tests/test_io_tools.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/tests/test_misc.py` & `CalSciPy-0.2.4/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/tests/test_reorganization.py` & `CalSciPy-0.2.4/tests/test_reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.2.3/tests/test_trace_processing.py` & `CalSciPy-0.2.4/tests/test_trace_processing.py`

 * *Files identical despite different names*

