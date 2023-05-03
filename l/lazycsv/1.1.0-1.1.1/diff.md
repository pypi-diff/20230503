# Comparing `tmp/lazycsv-1.1.0.tar.gz` & `tmp/lazycsv-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazycsv-1.1.0.tar", last modified: Tue May  2 03:26:44 2023, max compression
+gzip compressed data, was "lazycsv-1.1.1.tar", last modified: Wed May  3 00:55:57 2023, max compression
```

## Comparing `lazycsv-1.1.0.tar` & `lazycsv-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 03:26:44.032390 lazycsv-1.1.0/
--rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.1.0/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     8936 2023-05-02 03:26:44.032390 lazycsv-1.1.0/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     8255 2023-05-01 23:49:17.000000 lazycsv-1.1.0/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-02 03:26:44.032390 lazycsv-1.1.0/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     2034 2023-05-02 03:25:32.000000 lazycsv-1.1.0/setup.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 03:26:44.032390 lazycsv-1.1.0/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 03:26:44.032390 lazycsv-1.1.0/src/lazycsv/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.1.0/src/lazycsv/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    39297 2023-05-02 02:35:46.000000 lazycsv-1.1.0/src/lazycsv/lazycsv.c
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 03:26:44.032390 lazycsv-1.1.0/src/lazycsv.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     8936 2023-05-02 03:26:44.000000 lazycsv-1.1.0/src/lazycsv.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-05-02 03:26:44.000000 lazycsv-1.1.0/src/lazycsv.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-02 03:26:44.000000 lazycsv-1.1.0/src/lazycsv.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       67 2023-05-02 03:26:44.000000 lazycsv-1.1.0/src/lazycsv.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-02 03:26:44.000000 lazycsv-1.1.0/src/lazycsv.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 03:26:44.032390 lazycsv-1.1.0/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)    23362 2023-05-01 23:23:30.000000 lazycsv-1.1.0/tests/test_lazycsv.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-03 00:55:57.318527 lazycsv-1.1.1/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.1.1/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     9415 2023-05-03 00:55:57.318527 lazycsv-1.1.1/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     8364 2023-05-02 14:38:28.000000 lazycsv-1.1.1/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-03 00:55:57.318527 lazycsv-1.1.1/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     2400 2023-05-03 00:55:38.000000 lazycsv-1.1.1/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-03 00:55:57.318527 lazycsv-1.1.1/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-03 00:55:57.318527 lazycsv-1.1.1/src/lazycsv/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.1.1/src/lazycsv/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    39385 2023-05-02 14:43:37.000000 lazycsv-1.1.1/src/lazycsv/lazycsv.c
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-03 00:55:57.318527 lazycsv-1.1.1/src/lazycsv.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     9415 2023-05-03 00:55:57.000000 lazycsv-1.1.1/src/lazycsv.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-05-03 00:55:57.000000 lazycsv-1.1.1/src/lazycsv.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-03 00:55:57.000000 lazycsv-1.1.1/src/lazycsv.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       66 2023-05-03 00:55:57.000000 lazycsv-1.1.1/src/lazycsv.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-05-03 00:55:57.000000 lazycsv-1.1.1/src/lazycsv.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-03 00:55:57.318527 lazycsv-1.1.1/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)    23737 2023-05-02 15:32:03.000000 lazycsv-1.1.1/tests/test_lazycsv.py
```

### Comparing `lazycsv-1.1.0/LICENSE` & `lazycsv-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lazycsv-1.1.0/PKG-INFO` & `lazycsv-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
 Name: lazycsv
-Version: 1.1.0
-Summary: an OOM csv parser
+Version: 1.1.1
+Summary: an fast, memory efficient csv parser
 Author: Michael Green, Chris Perkins
 Author-email: dev@crunch.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Provides-Extra: test
-Provides-Extra: benchmarks
+Provides-Extra: benchmark
 License-File: LICENSE
 
 # lazycsv - a memory-efficient csv parser
 
 ###### Developers: Michael Green, Chris Perkins
 
 lazycsv is a C implementation of a csv parser for python. The aim of this
@@ -183,25 +190,28 @@
 
 Users pinned to an older version of numpy (<1.7) may wish to instead compile
 using a `LAZYCSV_INCLUDE_NUMPY_LEGACY=1` flag, which drops the API pin in the
 module while still compiling with numpy support.
 
 #### Benchmarks (CPU)
 
+CPU benchmarks are included below, benchmarked on a Ryzen 7 5800X inside a
+stock python3.9 docker container.
+
 ```
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 0.134gb
 cols=10000
 rows=10000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 0.4978358040098101
-parsing cols... time to parse: 1.8409163669857662
-total time: 2.3387521709955763
+indexing lazy... time to index: 0.4746863649925217
+parsing cols... time to parse: 1.5940959230065346
+total time: 2.0687822879990563
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 0.40828132900060154
 parsing cols... time to parse: 3.810204313998838
 total time: 4.21848564299944
 
@@ -215,17 +225,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 1.387gb
 cols=10000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 4.978727137990063
-parsing cols... time to parse: 23.64216143201338
-total time: 28.620888570003444
+indexing lazy... time to index: 4.287910053972155
+parsing cols... time to parse: 20.004111379006645
+total time: 24.2920214329788
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 2.4456441220027045
 parsing cols... time to parse: 37.424315700998704
 total time: 39.86995982300141
 
@@ -238,17 +248,17 @@
 ```
 filesize: 14.333gb
 cols=100000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 58.97352126000624
-parsing cols... time to parse: 508.8208989979903
-total time: 567.7944202579965
+indexing lazy... time to index: 61.56681043098797
+parsing cols... time to parse: 553.8464674730203
+total time: 615.4132779040083
 
 benchmarking datatable:
  58% |█████████████████████████████▍                    | Reading data Killed
 
 benchmarking polars (read):
 Killed
 ```
```

### Comparing `lazycsv-1.1.0/README.md` & `lazycsv-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -163,25 +163,28 @@
 
 Users pinned to an older version of numpy (<1.7) may wish to instead compile
 using a `LAZYCSV_INCLUDE_NUMPY_LEGACY=1` flag, which drops the API pin in the
 module while still compiling with numpy support.
 
 #### Benchmarks (CPU)
 
+CPU benchmarks are included below, benchmarked on a Ryzen 7 5800X inside a
+stock python3.9 docker container.
+
 ```
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 0.134gb
 cols=10000
 rows=10000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 0.4978358040098101
-parsing cols... time to parse: 1.8409163669857662
-total time: 2.3387521709955763
+indexing lazy... time to index: 0.4746863649925217
+parsing cols... time to parse: 1.5940959230065346
+total time: 2.0687822879990563
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 0.40828132900060154
 parsing cols... time to parse: 3.810204313998838
 total time: 4.21848564299944
 
@@ -195,17 +198,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 1.387gb
 cols=10000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 4.978727137990063
-parsing cols... time to parse: 23.64216143201338
-total time: 28.620888570003444
+indexing lazy... time to index: 4.287910053972155
+parsing cols... time to parse: 20.004111379006645
+total time: 24.2920214329788
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 2.4456441220027045
 parsing cols... time to parse: 37.424315700998704
 total time: 39.86995982300141
 
@@ -218,17 +221,17 @@
 ```
 filesize: 14.333gb
 cols=100000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 58.97352126000624
-parsing cols... time to parse: 508.8208989979903
-total time: 567.7944202579965
+indexing lazy... time to index: 61.56681043098797
+parsing cols... time to parse: 553.8464674730203
+total time: 615.4132779040083
 
 benchmarking datatable:
  58% |█████████████████████████████▍                    | Reading data Killed
 
 benchmarking polars (read):
 Killed
 ```
```

### Comparing `lazycsv-1.1.0/setup.py` & `lazycsv-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 
 from setuptools import Extension, find_packages, setup
 
-LAZYCSV_DEBUG = int(os.environ.get("LAZYCSV_DEBUG", 0))
+LAZYCSV_DEBUG = int("LAZYCSV_DEBUG" in os.environ)
 LAZYCSV_INDEX_DTYPE = os.environ.get("LAZYCSV_INDEX_DTYPE", "uint16_t")
 
-LAZYCSV_INCLUDE_NUMPY = int(os.environ.get("LAZYCSV_INCLUDE_NUMPY", 0))
-LAZYCSV_INCLUDE_NUMPY_LEGACY = int(os.environ.get("LAZYCSV_INCLUDE_NUMPY_LEGACY", 0))
+LAZYCSV_INCLUDE_NUMPY = int("LAZYCSV_INCLUDE_NUMPY" in os.environ)
+LAZYCSV_INCLUDE_NUMPY_LEGACY = int("LAZYCSV_INCLUDE_NUMPY_LEGACY" in os.environ)
 
 include_dirs = (
     [__import__("numpy").get_include()]
     if (LAZYCSV_INCLUDE_NUMPY | LAZYCSV_INCLUDE_NUMPY_LEGACY)
     else []
 )
 
@@ -27,37 +27,44 @@
             ("INCLUDE_NUMPY", LAZYCSV_INCLUDE_NUMPY),
             ("INCLUDE_NUMPY_LEGACY", LAZYCSV_INCLUDE_NUMPY_LEGACY),
             ("DEBUG", LAZYCSV_DEBUG),
         ],
     )
 ]
 
-with open("README.md", "r") as f:
+with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="lazycsv",
-    version="1.1.0",
+    version="1.1.1",
     author="Michael Green, Chris Perkins",
     author_email="dev@crunch.io",
-    description="an OOM csv parser",
+    description="an fast, memory efficient csv parser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src"),
     extras_require={
         "test": ["pytest", "numpy"],
-        "benchmarks": ["datatable", "pandas", "pyarrow", "polars"],
+        "benchmark": ["datatable", "pandas", "pyarrow", "polars"],
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: POSIX",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Utilities",
     ],
     package_dir={"": "src"},
     ext_modules=extensions,
 )
```

### Comparing `lazycsv-1.1.0/src/lazycsv/lazycsv.c` & `lazycsv-1.1.1/src/lazycsv/lazycsv.c`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,14 @@
     PyObject_HEAD
     PyObject* lazy;
     size_t row;
     size_t col;
     size_t position;
     size_t stop;
     size_t step;
-    void (*fn)(struct lazycsv_iter*, size_t*, size_t*);
     char reversed;
 } LazyCSV_Iter;
 
 
 static inline void _BufferWrite(int fd, LazyCSV_Buffer *buffer, void *data,
                                 size_t size) {
 
@@ -328,74 +327,91 @@
 
 static PyObject* LazyCSV_IterNext(PyObject* self) {
     LazyCSV_Iter* iter = (LazyCSV_Iter*)self;
     LazyCSV *lazy = (LazyCSV *)iter->lazy;
 
     size_t offset = SIZE_MAX, len;
 
-    iter->fn(iter, &offset, &len);
+    if (iter->col != SIZE_MAX) {
+        LazyCSV_IterCol(iter, &offset, &len);
+    }
+
+    else if (iter->row != SIZE_MAX) {
+        LazyCSV_IterRow(iter, &offset, &len);
+    }
+
+    else {
+        PyErr_SetString(
+            PyExc_RuntimeError,
+            "could not determine axis for materialization"
+        );
+        return NULL;
+    }
 
     if (offset==SIZE_MAX) {
         PyErr_SetNone(PyExc_StopIteration);
         return NULL;
     }
 
     return PyBytes_FromOffsetAndLen(lazy, offset, len);
 }
 
 
 static PyObject* LazyCSV_IterAsList(PyObject* self) {
     LazyCSV_Iter* iter = (LazyCSV_Iter*)self;
     LazyCSV* lazy = (LazyCSV*)iter->lazy;
+    void (*fn)(LazyCSV_Iter*, size_t*, size_t*);
 
     size_t size;
 
     if (iter->col != SIZE_MAX) {
         size = lazy->rows - iter->position;
+        fn = LazyCSV_IterCol;
     }
     else if (iter->row != SIZE_MAX) {
         size = lazy->cols - iter->position;
+        fn = LazyCSV_IterRow;
     }
     else {
         PyErr_SetString(
             PyExc_RuntimeError,
             "could not determine axis for materialization"
         );
         return NULL;
     }
 
     PyObject* result = PyList_New(size);
     size_t offset, len;
 
     PyObject* item;
     for (size_t i = 0; i < size; i++) {
-        iter->fn(iter, &offset, &len);
+        fn(iter, &offset, &len);
         item = PyBytes_FromOffsetAndLen(lazy, offset, len);
         PyList_SET_ITEM(result, i, item);
     }
 
     return result;
 }
 
 
 #if INCLUDE_NUMPY
 static PyObject* LazyCSV_IterAsNumpy(PyObject* self) {
     LazyCSV_Iter* iter = (LazyCSV_Iter*)self;
     LazyCSV* lazy = (LazyCSV*)iter->lazy;
 
     size_t size;
-    void (*IterFn)(LazyCSV_Iter*, size_t*, size_t*);
+    void (*fn)(LazyCSV_Iter*, size_t*, size_t*);
 
     if (iter->col != SIZE_MAX) {
-        IterFn = LazyCSV_IterCol;
         size = lazy->rows - iter->position;
+        fn = LazyCSV_IterCol;
     }
     else if (iter->row != SIZE_MAX) {
-        IterFn = LazyCSV_IterRow;
         size = lazy->cols - iter->position;
+        fn = LazyCSV_IterRow;
     }
     else {
         PyErr_SetString(
             PyExc_RuntimeError,
             "could not determine axis for materialization"
         );
         return NULL;
@@ -405,15 +421,15 @@
     LazyCSV_Buffer buffer = {.data = malloc(buffer_capacity),
                              .size = 0,
                              .capacity = buffer_capacity};
 
     size_t offset, len=0, max_len=0;
     char* addr;
     for (size_t i=0; i < size; i++) {
-        IterFn(iter, &offset, &len);
+        fn(iter, &offset, &len);
         addr = lazy->_data->data + offset;
         _BufferCache(&buffer, &len, sizeof(size_t));
         _BufferCache(&buffer, addr, len);
         max_len = len > max_len ? len : max_len;
     }
 
     npy_intp const dimensions[1] = {size, };
@@ -1046,15 +1062,14 @@
 
 
 static PyObject *LazyCSV_Seq(PyObject *self, PyObject *args, PyObject *kwargs) {
 
     size_t row = SIZE_MAX;
     size_t col = SIZE_MAX;
     size_t stop;
-    void (*fn)(LazyCSV_Iter*, size_t*, size_t*);
     char reversed;
 
     static char *kwlist[] = {"row", "col", "reversed", NULL};
 
     char ok = PyArg_ParseTupleAndKeywords(
         args, kwargs, "|nnb", kwlist, &row, &col, &reversed
     );
@@ -1080,19 +1095,17 @@
             PyExc_ValueError,
             "cannot specify both row and col"
         );
         return NULL;
     }
 
     if (col != SIZE_MAX) {
-        fn = LazyCSV_IterCol;
         stop = ((LazyCSV*)self)->rows;
     }
     else if (row != SIZE_MAX) {
-        fn = LazyCSV_IterRow;
         stop = ((LazyCSV*)self)->cols;
     }
     else {
         PyErr_SetString(
             PyExc_RuntimeError,
             "could not determine axis for materialization"
         );
@@ -1113,15 +1126,14 @@
     iter->row = row;
     iter->col = col;
     iter->reversed = reversed;
     iter->position = 0;
     iter->step = 1;
     iter->stop = stop;
     iter->lazy = self;
-    iter->fn = fn;
 
     Py_INCREF(self);
 
     return (PyObject*)iter;
 }
 
 
@@ -1196,16 +1208,14 @@
         return LazyCSV_GetValue(self, row_obj, col_obj);
 
     int row_is_slice = PySlice_Check(row_obj);
     int col_is_slice = PySlice_Check(col_obj);
 
     LazyCSV* lazy = (LazyCSV*)self;
 
-    void (*fn)(LazyCSV_Iter*, size_t*, size_t*);
-
     if (row_is_slice && !col_is_slice) {
         PySliceObject* row_slice = (PySliceObject*)row_obj;
 
         Py_ssize_t _col = PyLong_AsSsize_t(col_obj);
         size_t col = _col < 0 ? lazy->cols + _col : (size_t)_col;
 
         int col_in_bounds = (
@@ -1250,15 +1260,14 @@
         iter->row = SIZE_MAX;
         iter->col = col;
         iter->reversed = reversed;
         iter->position = start;
         iter->step = step;
         iter->stop = stop;
         iter->lazy = self;
-        iter->fn = LazyCSV_IterCol;
         Py_INCREF(self);
 
         return (PyObject*)iter;
     }
 
     if (col_is_slice && !row_is_slice) {
         PySliceObject* col_slice = (PySliceObject*)col_obj;
@@ -1307,15 +1316,14 @@
 
         iter->row = row;
         iter->col = SIZE_MAX;
         iter->reversed = reversed;
         iter->position = start;
         iter->step = step;
         iter->stop = stop;
-        iter->fn = LazyCSV_IterRow;
         iter->lazy = self;
         Py_INCREF(self);
 
         return (PyObject*)iter;
     }
 
     goto schema_err;
```

### Comparing `lazycsv-1.1.0/src/lazycsv.egg-info/PKG-INFO` & `lazycsv-1.1.1/src/lazycsv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
 Name: lazycsv
-Version: 1.1.0
-Summary: an OOM csv parser
+Version: 1.1.1
+Summary: an fast, memory efficient csv parser
 Author: Michael Green, Chris Perkins
 Author-email: dev@crunch.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Provides-Extra: test
-Provides-Extra: benchmarks
+Provides-Extra: benchmark
 License-File: LICENSE
 
 # lazycsv - a memory-efficient csv parser
 
 ###### Developers: Michael Green, Chris Perkins
 
 lazycsv is a C implementation of a csv parser for python. The aim of this
@@ -183,25 +190,28 @@
 
 Users pinned to an older version of numpy (<1.7) may wish to instead compile
 using a `LAZYCSV_INCLUDE_NUMPY_LEGACY=1` flag, which drops the API pin in the
 module while still compiling with numpy support.
 
 #### Benchmarks (CPU)
 
+CPU benchmarks are included below, benchmarked on a Ryzen 7 5800X inside a
+stock python3.9 docker container.
+
 ```
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 0.134gb
 cols=10000
 rows=10000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 0.4978358040098101
-parsing cols... time to parse: 1.8409163669857662
-total time: 2.3387521709955763
+indexing lazy... time to index: 0.4746863649925217
+parsing cols... time to parse: 1.5940959230065346
+total time: 2.0687822879990563
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 0.40828132900060154
 parsing cols... time to parse: 3.810204313998838
 total time: 4.21848564299944
 
@@ -215,17 +225,17 @@
 root@aa9d7c7ffb59:/code# python tests/benchmark_lazy.py
 filesize: 1.387gb
 cols=10000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 4.978727137990063
-parsing cols... time to parse: 23.64216143201338
-total time: 28.620888570003444
+indexing lazy... time to index: 4.287910053972155
+parsing cols... time to parse: 20.004111379006645
+total time: 24.2920214329788
 
 benchmarking datatable:
 100% |██████████████████████████████████████████████████| Reading data [done]
 creating datatables frame... time to object: 2.4456441220027045
 parsing cols... time to parse: 37.424315700998704
 total time: 39.86995982300141
 
@@ -238,17 +248,17 @@
 ```
 filesize: 14.333gb
 cols=100000
 rows=100000
 sparsity=0.95
 
 benchmarking lazycsv:
-indexing lazy... time to index: 58.97352126000624
-parsing cols... time to parse: 508.8208989979903
-total time: 567.7944202579965
+indexing lazy... time to index: 61.56681043098797
+parsing cols... time to parse: 553.8464674730203
+total time: 615.4132779040083
 
 benchmarking datatable:
  58% |█████████████████████████████▍                    | Reading data Killed
 
 benchmarking polars (read):
 Killed
 ```
```

### Comparing `lazycsv-1.1.0/tests/test_lazycsv.py` & `lazycsv-1.1.1/tests/test_lazycsv.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
     yield lazy
 
 
 @pytest.fixture
 def file_1000r_1000c():
     tempf = tempfile.NamedTemporaryFile()
     cols, rows = 1000, 1000
-    headers = ",".join(f"col_{i}" for i in range(cols)) + "\n"
+    headers = ",".join("col_{i}".format_map(dict(i=i)) for i in range(cols)) + "\n"
     tempf.write(headers.encode("utf8"))
     for _ in range(rows):
-        row = ",".join(f"{j}" for j in range(cols)) + "\n"
+        row = ",".join("{j}".format_map(dict(j=j)) for j in range(cols)) + "\n"
         tempf.write(row.encode("utf8"))
     tempf.flush()
     yield tempf
     tempf.close()
 
 
 @contextlib.contextmanager
@@ -230,25 +230,30 @@
             with pytest.raises(ValueError) as err:
                 lazy[3, 3]
             assert ("provided value not in bounds of index",) == err.value.args
 
 
 class TestLazyCSVIter:
     def test_to_list(self, lazy):
-        _iter = lazy.sequence(col=0)
-        assert _iter.to_list() == [b"0", b"1"]
+        assert lazy.sequence(col=0).to_list() == [b"0", b"1"]
+        assert lazy.sequence(row=1).to_list() == [b'1', b'a1', b'b1']
 
     def test_to_numpy(self):
         actual = b"INDEX,ATTR\n0,a\n10,b\n100,c\n1000,d\n"
         with prepped_file(actual) as tempf:
             lazy = lazycsv.LazyCSV(tempf.name)
             _iter = lazy.sequence(col=0)
             if hasattr(_iter, "to_numpy"):
                 arr = _iter.to_numpy()
                 assert arr.tolist() == [b"0", b"10", b"100", b"1000"]
+                assert (lazy
+                    .sequence(row=1)
+                    .to_numpy()
+                    .tolist()
+                ) == [b'10', b'b']
             else:
                 raise RuntimeError(
                     "test suite did not test numpy, recompile while setting"
                     " LAZYCSV_INCLUDE_NUMPY=1 as an env variable to compile"
                     " extension with numpy support."
                 )
 
@@ -371,19 +376,19 @@
         lazy = lazycsv.LazyCSV(file_1000r_1000c.name, buffer_size=10**7)
         actual = list(lazy.sequence(col=0))
         assert len(actual) == 1000
 
     def test_big_sparse(self):
         tempf = tempfile.NamedTemporaryFile()
         cols, rows = 200, 200
-        headers = ",".join(f"col_{i}" for i in range(cols)) + "\n"
+        headers = ",".join("col_{i}".format_map(dict(i=i)) for i in range(cols)) + "\n"
         tempf.write(headers.encode("utf8"))
         targets = {249, 499, 749, 999}
         for _ in range(rows):
-            row = ",".join(f"{j}" if j in targets else "" for j in range(cols)) + "\n"
+            row = ",".join("{j}".format_map(dict(j=j)) if j in targets else "" for j in range(cols)) + "\n"
             tempf.write(row.encode("utf8"))
         tempf.flush()
 
         lazy = lazycsv.LazyCSV(tempf.name)
         with open(tempf.name) as f:
             reader = csv.reader(f)
             headers = tuple(x.encode() for x in next(reader))
@@ -429,27 +434,27 @@
 
 
 class TestEdgecases:
     def test_many_files_separators(self):
         for sep in ("\n", "\r", "\r\n"):
             for i in range(250, 265):
                 header = "A" * i
-                data = f"{header}{sep}1{sep}2"
+                data = "{header}{sep}1{sep}2".format_map(dict(header=header, sep=sep))
                 with prepped_file(data.encode()) as tempf:
                     lazy = lazycsv.LazyCSV(tempf.name)
                     actual = list(lazy.sequence(col=0))
                     headers = lazy.headers
                 assert actual == [b"1", b"2"]
                 assert headers == (header.encode(),)
 
     def test_many_empty_files_separators(self):
         for sep in ("\n", "\r", "\r\n"):
             for i in range(250, 261):
                 header = "A" * i
-                data = f"{header}{sep}{sep}"
+                data = "{header}{sep}{sep}".format_map(dict(header=header, sep=sep))
                 with prepped_file(data.encode()) as tempf:
                     lazy = lazycsv.LazyCSV(tempf.name)
                     actual = list(lazy.sequence(col=0))
                     headers = lazy.headers
                 assert actual == [b""]
                 assert headers == (header.encode(),)
```

