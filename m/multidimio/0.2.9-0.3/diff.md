# Comparing `tmp/multidimio-0.2.9.tar.gz` & `tmp/multidimio-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidimio-0.2.9.tar", max compression
+gzip compressed data, was "multidimio-0.3.tar", max compression
```

## Comparing `multidimio-0.2.9.tar` & `multidimio-0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    10203 2023-03-10 15:18:05.939740 multidimio-0.2.9/LICENSE
--rw-r--r--   0        0        0     6043 2023-03-10 15:18:05.939740 multidimio-0.2.9/README.md
--rw-r--r--   0        0        0     2860 2023-03-10 15:18:19.051646 multidimio-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      474 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/__init__.py
--rw-r--r--   0        0        0     2697 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/__main__.py
--rw-r--r--   0        0        0      127 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/api/__init__.py
--rw-r--r--   0        0        0    24779 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/api/accessor.py
--rw-r--r--   0        0        0     2322 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/api/convenience.py
--rw-r--r--   0        0        0     4451 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/api/io_utils.py
--rw-r--r--   0        0        0      105 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/commands/__init__.py
--rw-r--r--   0        0        0    10623 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/commands/segy.py
--rw-r--r--   0        0        0      529 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/constants.py
--rw-r--r--   0        0        0      141 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/converters/__init__.py
--rw-r--r--   0        0        0      597 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/converters/exceptions.py
--rw-r--r--   0        0        0     6349 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/converters/mdio.py
--rw-r--r--   0        0        0    12386 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/converters/segy.py
--rw-r--r--   0        0        0      143 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/__init__.py
--rw-r--r--   0        0        0     3811 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/dimension.py
--rw-r--r--   0        0        0      268 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/exceptions.py
--rw-r--r--   0        0        0     3765 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/grid.py
--rw-r--r--   0        0        0     2917 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/indexing.py
--rw-r--r--   0        0        0     2727 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/serialization.py
--rw-r--r--   0        0        0      429 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/core/utils_write.py
--rw-r--r--   0        0        0     1646 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/py.typed
--rw-r--r--   0        0        0       44 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/__init__.py
--rw-r--r--   0        0        0      636 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/_standards_common.py
--rw-r--r--   0        0        0     9384 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/_standards_rev0.py
--rw-r--r--   0        0        0     8023 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/_workers.py
--rw-r--r--   0        0        0    11362 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/blocked_io.py
--rw-r--r--   0        0        0     1760 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/byte_utils.py
--rw-r--r--   0        0        0     9396 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/creation.py
--rw-r--r--   0        0        0     4856 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/ebcdic.py
--rw-r--r--   0        0        0      181 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/exceptions.py
--rw-r--r--   0        0        0     2748 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/headers.py
--rw-r--r--   0        0        0     3561 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/headers_text.py
--rw-r--r--   0        0        0     3232 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/helpers_segy.py
--rw-r--r--   0        0        0     5785 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/ibm_float.py
--rw-r--r--   0        0        0     4540 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/parsers.py
--rw-r--r--   0        0        0     6160 2023-03-10 15:18:05.955740 multidimio-0.2.9/src/mdio/segy/utilities.py
--rw-r--r--   0        0        0     7680 1970-01-01 00:00:00.000000 multidimio-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    10203 2023-05-02 22:26:43.331880 multidimio-0.3/LICENSE
+-rw-r--r--   0        0        0     6043 2023-05-02 22:26:43.331880 multidimio-0.3/README.md
+-rw-r--r--   0        0        0     2859 2023-05-02 22:27:06.088113 multidimio-0.3/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/__init__.py
+-rw-r--r--   0        0        0     2697 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/__main__.py
+-rw-r--r--   0        0        0      127 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/api/__init__.py
+-rw-r--r--   0        0        0    24779 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/api/accessor.py
+-rw-r--r--   0        0        0     2322 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/api/convenience.py
+-rw-r--r--   0        0        0     4451 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/api/io_utils.py
+-rw-r--r--   0        0        0      105 2023-05-02 22:26:43.351881 multidimio-0.3/src/mdio/commands/__init__.py
+-rw-r--r--   0        0        0    10623 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/commands/segy.py
+-rw-r--r--   0        0        0      529 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/constants.py
+-rw-r--r--   0        0        0      141 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/converters/__init__.py
+-rw-r--r--   0        0        0      597 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/converters/exceptions.py
+-rw-r--r--   0        0        0     6510 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/converters/mdio.py
+-rw-r--r--   0        0        0    12386 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/converters/segy.py
+-rw-r--r--   0        0        0      143 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/__init__.py
+-rw-r--r--   0        0        0     3811 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/dimension.py
+-rw-r--r--   0        0        0      268 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/exceptions.py
+-rw-r--r--   0        0        0     3765 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/grid.py
+-rw-r--r--   0        0        0     2917 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/indexing.py
+-rw-r--r--   0        0        0     2727 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/serialization.py
+-rw-r--r--   0        0        0      429 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/core/utils_write.py
+-rw-r--r--   0        0        0     1646 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/py.typed
+-rw-r--r--   0        0        0       44 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/__init__.py
+-rw-r--r--   0        0        0      636 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/_standards_common.py
+-rw-r--r--   0        0        0     9384 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/_standards_rev0.py
+-rw-r--r--   0        0        0     7560 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/_workers.py
+-rw-r--r--   0        0        0    11173 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/blocked_io.py
+-rw-r--r--   0        0        0     1760 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/byte_utils.py
+-rw-r--r--   0        0        0     9396 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/creation.py
+-rw-r--r--   0        0        0     4856 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/ebcdic.py
+-rw-r--r--   0        0        0      181 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/exceptions.py
+-rw-r--r--   0        0        0     2748 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/headers.py
+-rw-r--r--   0        0        0     3561 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/headers_text.py
+-rw-r--r--   0        0        0     3232 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/helpers_segy.py
+-rw-r--r--   0        0        0     5785 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/ibm_float.py
+-rw-r--r--   0        0        0     4393 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/parsers.py
+-rw-r--r--   0        0        0     6160 2023-05-02 22:26:43.355881 multidimio-0.3/src/mdio/segy/utilities.py
+-rw-r--r--   0        0        0     7673 1970-01-01 00:00:00.000000 multidimio-0.3/PKG-INFO
```

### Comparing `multidimio-0.2.9/LICENSE` & `multidimio-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/README.md` & `multidimio-0.3/README.md`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/pyproject.toml` & `multidimio-0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multidimio"
-version = "0.2.9"
+version = "0.3"
 description = "Cloud-native, scalable, and user-friendly multi dimensional energy data!"
 authors = ["TGS <sys-opensource@tgs.com>"]
 maintainers = [
     "Altay Sansal <altay.sansal@tgs.com>",
     "Sri Kainkaryam <sribharath.kainkaryam@tgs.com>",
 ]
 license = "Apache-2.0"
@@ -20,29 +20,29 @@
 ]
 keywords = ["mdio", "multidimio", "seismic", "wind", "data"]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/TGSAI/mdio-python/releases"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 click = "^8.1.3"
 click-params = "^0.3.0"
 zarr = "^2.12.0"
 dask = ">=2022.11.0"
 tqdm = "^4.64.0"
 segyio = "^1.9.3"
 numba = ">=0.55.2,<1.0.0"
 psutil = "^5.9.1"
 distributed = {version = ">=2022.11.0", optional = true}
 bokeh = {version = "^2.4.3", optional = true}
 s3fs = {version = ">=2022.7.0", optional = true}
 gcsfs = {version = ">=2022.7.0", optional = true}
 adlfs = {version = ">=2022.7.0", optional = true}
-zfpy = {version = "^1.0.0", optional = true}
+#zfpy = {version = "^1.0.0", optional = true}
 
 [tool.poetry.extras]
 distributed = ["distributed", "bokeh"]
 cloud = ["s3fs", "gcsfs", "adlfs"]
 lossy = ["zfpy"]
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `multidimio-0.2.9/src/mdio/__main__.py` & `multidimio-0.3/src/mdio/__main__.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/api/accessor.py` & `multidimio-0.3/src/mdio/api/accessor.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/api/convenience.py` & `multidimio-0.3/src/mdio/api/convenience.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/api/io_utils.py` & `multidimio-0.3/src/mdio/api/io_utils.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/commands/segy.py` & `multidimio-0.3/src/mdio/commands/segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/constants.py` & `multidimio-0.3/src/mdio/constants.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/converters/exceptions.py` & `multidimio-0.3/src/mdio/converters/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/converters/mdio.py` & `multidimio-0.3/src/mdio/converters/mdio.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,13 +174,17 @@
                 live_mask=live_mask,
                 out_dtype=out_dtype,
                 out_byteorder=out_byteorder,
                 file_root=tmp_dir.name,
                 axis=tuple(range(1, samples.ndim)),
             ).compute()
 
+        # If whole blocks are missing, remove them from the list.
+        missing_mask = flat_files == "missing"
+        flat_files = flat_files[~missing_mask]
+
         final_concat = [output_segy_path] + flat_files.tolist()
 
         if client is not None:
             _ = client.submit(concat_files, final_concat).result()
         else:
             concat_files(final_concat, progress=True)
```

### Comparing `multidimio-0.2.9/src/mdio/converters/segy.py` & `multidimio-0.3/src/mdio/converters/segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/core/dimension.py` & `multidimio-0.3/src/mdio/core/dimension.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/core/grid.py` & `multidimio-0.3/src/mdio/core/grid.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/core/indexing.py` & `multidimio-0.3/src/mdio/core/indexing.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/core/serialization.py` & `multidimio-0.3/src/mdio/core/serialization.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/exceptions.py` & `multidimio-0.3/src/mdio/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/segy/_standards_common.py` & `multidimio-0.3/src/mdio/segy/_standards_common.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/segy/_standards_rev0.py` & `multidimio-0.3/src/mdio/segy/_standards_rev0.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/segy/_workers.py` & `multidimio-0.3/src/mdio/segy/_workers.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,21 +204,7 @@
     tmp_data = tmp_data[nonzero_mask]
     chunk_sum = tmp_data.sum(dtype="float64")
     chunk_sum_squares = np.square(tmp_data, dtype="float64").sum()
     min_val = tmp_data.min()
     max_val = tmp_data.max()
 
     return count, chunk_sum, chunk_sum_squares, min_val, max_val
-
-
-# tqdm only works properly with pool.map
-# However, we need pool.starmap because we have more than one
-# argument to make pool.map work with multiple arguments, we
-# wrap the function and consolidate arguments to one
-def trace_worker_map(args):
-    """Wrapper for trace worker to use with tqdm."""
-    return trace_worker(*args)
-
-
-def header_scan_worker_map(args):
-    """Wrapper for header scan worker to use with tqdm."""
-    return header_scan_worker(*args)
```

### Comparing `multidimio-0.2.9/src/mdio/segy/blocked_io.py` & `multidimio-0.3/src/mdio/segy/blocked_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Functions for doing blocked I/O from SEG-Y."""
 
 
 from __future__ import annotations
 
 import multiprocessing as mp
+from concurrent.futures import ProcessPoolExecutor
 from itertools import repeat
 
 import numpy as np
 from dask.array import Array
 from dask.array import blockwise
 from dask.array.reductions import _tree_reduce
 from numpy.typing import NDArray
@@ -15,15 +16,15 @@
 from segyio.tracefield import keys as segy_hdr_keys
 from tqdm.auto import tqdm
 from zarr import Blosc
 from zarr import Group
 
 from mdio.core import Grid
 from mdio.core.indexing import ChunkIterator
-from mdio.segy._workers import trace_worker_map
+from mdio.segy._workers import trace_worker
 from mdio.segy.byte_utils import ByteOrder
 from mdio.segy.byte_utils import Dtype
 from mdio.segy.creation import concat_files
 from mdio.segy.creation import write_to_segy_stack
 
 
 try:
@@ -128,43 +129,35 @@
         dimension_separator="/",
     )
 
     # Initialize chunk iterator (returns next chunk slice indices each iteration)
     chunker = ChunkIterator(trace_array, chunk_samples=False)
     num_chunks = len(chunker)
 
-    # Setting all multiprocessing parameters.
-    parallel_inputs = zip(  # noqa: B905
-        repeat(segy_path),
-        repeat(trace_array),
-        repeat(header_array),
-        repeat(grid),
-        chunker,
-        repeat(segy_endian),
-    )
-
-    # This is for Unix async writes to s3fs/fsspec, when using
-    # multiprocessing. By default, Linux uses the 'fork' method.
-    # 'spawn' is a little slower to spool up processes, but 'fork'
-    # doesn't work. If you don't use this, processes get deadlocked
-    # on cloud stores. 'spawn' is default in Windows.
+    # For Unix async writes with s3fs/fsspec & multiprocessing,
+    # use 'spawn' instead of default 'fork' to avoid deadlocks
+    # on cloud stores. Slower but necessary. Default on Windows.
+    num_workers = min(num_chunks, NUM_CORES)
     context = mp.get_context("spawn")
+    executor = ProcessPoolExecutor(max_workers=num_workers, mp_context=context)
 
-    # This is the chunksize for multiprocessing. Not to be confused
-    # with Zarr chunksize.
-    num_workers = min(num_chunks, NUM_CORES)
+    # Chunksize here is for multiprocessing, not Zarr chunksize.
     pool_chunksize, extra = divmod(num_chunks, num_workers * 4)
     pool_chunksize += 1 if extra else pool_chunksize
 
     tqdm_kw = dict(unit="block", dynamic_ncols=True)
-    with context.Pool(num_workers) as pool:
-        # pool.imap is lazy
-        lazy_work = pool.imap(
-            func=trace_worker_map,
-            iterable=parallel_inputs,
+    with executor:
+        lazy_work = executor.map(
+            trace_worker,  # fn
+            repeat(segy_path),
+            repeat(trace_array),
+            repeat(header_array),
+            repeat(grid),
+            chunker,
+            repeat(segy_endian),
             chunksize=pool_chunksize,
         )
 
         lazy_work = tqdm(
             iterable=lazy_work,
             total=num_chunks,
             desc=f"Ingesting SEG-Y in {num_chunks} chunks",
```

### Comparing `multidimio-0.2.9/src/mdio/segy/byte_utils.py` & `multidimio-0.3/src/mdio/segy/byte_utils.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/segy/creation.py` & `multidimio-0.3/src/mdio/segy/creation.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/segy/ebcdic.py` & `multidimio-0.3/src/mdio/segy/ebcdic.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/segy/headers.py` & `multidimio-0.3/src/mdio/segy/headers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/segy/headers_text.py` & `multidimio-0.3/src/mdio/segy/headers_text.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/segy/helpers_segy.py` & `multidimio-0.3/src/mdio/segy/helpers_segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/segy/ibm_float.py` & `multidimio-0.3/src/mdio/segy/ibm_float.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/src/mdio/segy/parsers.py` & `multidimio-0.3/src/mdio/segy/parsers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Parsers for sections of SEG-Y files."""
 
 
 from __future__ import annotations
 
+from concurrent.futures import ProcessPoolExecutor
 from itertools import repeat
 from math import ceil
-from multiprocessing import Pool
 from typing import Any
 from typing import Sequence
 
 import numpy as np
 import segyio
 from psutil import cpu_count
 from tqdm.auto import tqdm
 
 from mdio.core import Dimension
-from mdio.segy._workers import header_scan_worker_map
+from mdio.segy._workers import header_scan_worker
 
 
 NUM_CORES = cpu_count(logical=False)
 
 
 def get_trace_count(segy_path, segy_endian):
     """Get trace count from SEG-Y file (size)."""
@@ -100,32 +100,26 @@
     for idx in range(n_blocks):
         start, stop = idx * block_size, (idx + 1) * block_size
         if stop > trace_count:
             stop = trace_count
 
         trace_ranges.append((start, stop))
 
-    # Note: Make sure the order of this is exactly
-    # the same as the function call.
-    parallel_inputs = zip(  # noqa: B905 or strict=False >= py3.10
-        repeat(segy_path),
-        trace_ranges,
-        repeat(byte_locs),
-        repeat(byte_lengths),
-        repeat(segy_endian),
-    )
-
     num_workers = min(n_blocks, NUM_CORES)
 
     tqdm_kw = dict(unit="block", dynamic_ncols=True)
-    with Pool(num_workers) as pool:
+    with ProcessPoolExecutor(num_workers) as executor:
         # pool.imap is lazy
-        lazy_work = pool.imap(
-            func=header_scan_worker_map,
-            iterable=parallel_inputs,
+        lazy_work = executor.map(
+            header_scan_worker,  # fn
+            repeat(segy_path),
+            trace_ranges,
+            repeat(byte_locs),
+            repeat(byte_lengths),
+            repeat(segy_endian),
             chunksize=2,  # Not array chunks. This is for `multiprocessing`
         )
 
         if progress_bar is True:
             lazy_work = tqdm(
                 iterable=lazy_work,
                 total=n_blocks,
```

### Comparing `multidimio-0.2.9/src/mdio/segy/utilities.py` & `multidimio-0.3/src/mdio/segy/utilities.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.2.9/PKG-INFO` & `multidimio-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: multidimio
-Version: 0.2.9
+Version: 0.3
 Summary: Cloud-native, scalable, and user-friendly multi dimensional energy data!
 Home-page: https://mdio.dev
 License: Apache-2.0
 Keywords: mdio,multidimio,seismic,wind,data
 Author: TGS
 Author-email: sys-opensource@tgs.com
 Maintainer: Altay Sansal
 Maintainer-email: altay.sansal@tgs.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cloud
 Provides-Extra: distributed
 Provides-Extra: lossy
 Requires-Dist: adlfs (>=2022.7.0) ; extra == "cloud"
 Requires-Dist: bokeh (>=2.4.3,<3.0.0) ; extra == "distributed"
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-params (>=0.3.0,<0.4.0)
@@ -28,15 +29,14 @@
 Requires-Dist: gcsfs (>=2022.7.0) ; extra == "cloud"
 Requires-Dist: numba (>=0.55.2,<1.0.0)
 Requires-Dist: psutil (>=5.9.1,<6.0.0)
 Requires-Dist: s3fs (>=2022.7.0) ; extra == "cloud"
 Requires-Dist: segyio (>=1.9.3,<2.0.0)
 Requires-Dist: tqdm (>=4.64.0,<5.0.0)
 Requires-Dist: zarr (>=2.12.0,<3.0.0)
-Requires-Dist: zfpy (>=1.0.0,<2.0.0) ; extra == "lossy"
 Project-URL: Changelog, https://github.com/TGSAI/mdio-python/releases
 Project-URL: Documentation, https://mdio-python.readthedocs.io
 Project-URL: Repository, https://github.com/TGSAI/mdio-python
 Description-Content-Type: text/markdown
 
 <div>
   <img
```

