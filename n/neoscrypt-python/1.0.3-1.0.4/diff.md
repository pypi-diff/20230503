# Comparing `tmp/neoscrypt_python-1.0.3.tar.gz` & `tmp/neoscrypt_python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/neoscrypt_python-1.0.3.tar", last modified: Sun Oct 27 12:24:00 2019, max compression
+gzip compressed data, was "neoscrypt_python-1.0.4.tar", last modified: Wed May  3 14:03:47 2023, max compression
```

## Comparing `neoscrypt_python-1.0.3.tar` & `neoscrypt_python-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2019-10-27 12:24:00.000000 neoscrypt_python-1.0.3/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       20 2019-10-27 12:21:51.000000 neoscrypt_python-1.0.3/MANIFEST.in
--rw-r--r--   0 daniel    (1000) daniel    (1000)      371 2019-10-27 12:24:00.000000 neoscrypt_python-1.0.3/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      167 2019-10-27 12:21:51.000000 neoscrypt_python-1.0.3/README.md
--rw-r--r--   0 daniel    (1000) daniel    (1000)    20499 2019-10-27 12:21:51.000000 neoscrypt_python-1.0.3/neoscrypt.c
--rw-r--r--   0 daniel    (1000) daniel    (1000)      942 2019-10-27 12:21:51.000000 neoscrypt_python-1.0.3/neoscrypt.h
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2019-10-27 12:24:00.000000 neoscrypt_python-1.0.3/neoscrypt_python.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      371 2019-10-27 12:24:00.000000 neoscrypt_python-1.0.3/neoscrypt_python.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      242 2019-10-27 12:24:00.000000 neoscrypt_python-1.0.3/neoscrypt_python.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2019-10-27 12:24:00.000000 neoscrypt_python-1.0.3/neoscrypt_python.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       10 2019-10-27 12:24:00.000000 neoscrypt_python-1.0.3/neoscrypt_python.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1518 2019-10-27 12:21:51.000000 neoscrypt_python-1.0.3/neoscryptmodule.c
--rw-r--r--   0 daniel    (1000) daniel    (1000)       79 2019-10-27 12:24:00.000000 neoscrypt_python-1.0.3/setup.cfg
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      896 2019-10-27 12:21:51.000000 neoscrypt_python-1.0.3/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-03 14:03:47.285238 neoscrypt_python-1.0.4/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1086 2019-10-27 12:21:51.000000 neoscrypt_python-1.0.4/COPYING
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1086 2019-10-27 12:21:51.000000 neoscrypt_python-1.0.4/LICENSE.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       20 2019-10-27 12:21:51.000000 neoscrypt_python-1.0.4/MANIFEST.in
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      380 2023-05-03 14:03:47.285238 neoscrypt_python-1.0.4/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      167 2019-10-27 12:21:51.000000 neoscrypt_python-1.0.4/README.md
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    86489 2023-04-19 09:05:31.000000 neoscrypt_python-1.0.4/neoscrypt.c
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2162 2023-04-19 09:06:44.000000 neoscrypt_python-1.0.4/neoscrypt.h
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-03 14:03:47.285238 neoscrypt_python-1.0.4/neoscrypt_python.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      380 2023-05-03 14:03:47.000000 neoscrypt_python-1.0.4/neoscrypt_python.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      262 2023-05-03 14:03:47.000000 neoscrypt_python-1.0.4/neoscrypt_python.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-03 14:03:47.000000 neoscrypt_python-1.0.4/neoscrypt_python.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       10 2023-05-03 14:03:47.000000 neoscrypt_python-1.0.4/neoscrypt_python.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1526 2023-04-19 09:09:33.000000 neoscrypt_python-1.0.4/neoscryptmodule.c
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       79 2023-05-03 14:03:47.285238 neoscrypt_python-1.0.4/setup.cfg
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      901 2023-04-19 09:09:44.000000 neoscrypt_python-1.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `neoscrypt_python-1.0.3/neoscryptmodule.c` & `neoscrypt_python-1.0.4/neoscryptmodule.c`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright (C) 2019 The Xaya developers
+// Copyright (C) 2019-2023 The Xaya developers
 // Distributed under the MIT software license, see the accompanying
 // file COPYING or http://www.opensource.org/licenses/mit-license.php.
 
 #include <Python.h>
 
 #include "neoscrypt.h"
 
@@ -17,15 +17,15 @@
 #endif
     if (!PyArg_ParseTuple(args, "S", &input))
         return NULL;
     Py_INCREF(input);
     output = PyMem_Malloc(32);
 
 #if PY_MAJOR_VERSION >= 3
-    neoscrypt((const unsigned char *)PyBytes_AsString((PyObject*) input), output);
+    neoscrypt((const unsigned char *)PyBytes_AsString((PyObject*) input), output, 0);
 #else
     neoscrypt((const unsigned char *)PyString_AsString((PyObject*) input), output);
 #endif
     Py_DECREF(input);
 #if PY_MAJOR_VERSION >= 3
     value = Py_BuildValue("y#", output, 32);
 #else
```

### Comparing `neoscrypt_python-1.0.3/setup.py` & `neoscrypt_python-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2019 The Xaya developers
+# Copyright (C) 2019-2023 The Xaya developers
 # Distributed under the MIT software license, see the accompanying
 # file COPYING or http://www.opensource.org/licenses/mit-license.php.
 
 from setuptools import setup, Extension
 
 neoscrypt_module = Extension('neoscrypt',
                                sources = ['neoscryptmodule.c',
                                           'neoscrypt.c'],
                                include_dirs=['.'])
 
 setup (name = 'neoscrypt_python',
-       version = '1.0.3',
+       version = '1.0.4',
        license = 'MIT',
        description = 'Bindings for the NeoScrypt proof-of-work algorithm',
        author = 'Autonomous Worlds Ltd',
        author_email = 'info@autonomousworlds.com',
        url = 'https://github.com/xaya/neoscrypt_python',
-       download_url = 'https://github.com/xaya/neoscrypt_python/archive/v1.0.2.tar.gz',
+       download_url = 'https://github.com/xaya/neoscrypt_python/archive/v1.0.4.tar.gz',
        ext_modules = [neoscrypt_module])
```

