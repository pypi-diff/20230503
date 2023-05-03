# Comparing `tmp/pyzsf-0.1.1-cp36-abi3-win_amd64.whl.zip` & `tmp/pyzsf-0.1.2-cp36-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 21227 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      128 b- defN 21-May-20 17:50 pyzsf/__init__.py
--rw-rw-rw-  2.0 fat    34816 b- defN 21-May-20 17:54 pyzsf/_zsf_cffi.pyd
--rw-rw-rw-  2.0 fat     7764 b- defN 21-May-20 17:50 pyzsf/pyzsf.py
--rw-rw-rw-  2.0 fat     7817 b- defN 21-May-20 17:54 pyzsf-0.1.1.dist-info/COPYING.LESSER
--rw-rw-rw-  2.0 fat     1018 b- defN 21-May-20 17:54 pyzsf-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 21-May-20 17:54 pyzsf-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 21-May-20 17:54 pyzsf-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      604 b- defN 21-May-20 17:54 pyzsf-0.1.1.dist-info/RECORD
-8 files, 52253 bytes uncompressed, 20185 bytes compressed:  61.4%
+Zip file size: 21287 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      128 b- defN 21-Nov-09 14:46 pyzsf/__init__.py
+-rw-rw-rw-  2.0 fat    34816 b- defN 21-Nov-09 14:52 pyzsf/_zsf_cffi.pyd
+-rw-rw-rw-  2.0 fat     7910 b- defN 21-Nov-09 14:46 pyzsf/pyzsf.py
+-rw-rw-rw-  2.0 fat     7817 b- defN 21-Nov-09 14:52 pyzsf-0.1.2.dist-info/COPYING.LESSER
+-rw-rw-rw-  2.0 fat     1018 b- defN 21-Nov-09 14:52 pyzsf-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 21-Nov-09 14:52 pyzsf-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 21-Nov-09 14:52 pyzsf-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      604 b- defN 21-Nov-09 14:52 pyzsf-0.1.2.dist-info/RECORD
+8 files, 52399 bytes uncompressed, 20245 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: pyzsf/_zsf_cffi.pyd
 Comment: 
 
 Filename: pyzsf/pyzsf.py
 Comment: 
 
-Filename: pyzsf-0.1.1.dist-info/COPYING.LESSER
+Filename: pyzsf-0.1.2.dist-info/COPYING.LESSER
 Comment: 
 
-Filename: pyzsf-0.1.1.dist-info/METADATA
+Filename: pyzsf-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: pyzsf-0.1.1.dist-info/WHEEL
+Filename: pyzsf-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyzsf-0.1.1.dist-info/top_level.txt
+Filename: pyzsf-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyzsf-0.1.1.dist-info/RECORD
+Filename: pyzsf-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyzsf/pyzsf.py

```diff
@@ -5,14 +5,17 @@
 
 def _struct_to_dict(struct):
     d = {}
 
     for k in dir(struct):
         d[k] = getattr(struct, k)
 
+        if not isinstance(d[k], (float, int, str)) and ffi.typeof(d[k]).cname.startswith("struct "):
+            d[k] = _struct_to_dict(d[k])
+
     return d
 
 
 def _zsf_error_message(code):
     return ffi.string(lib.zsf_error_msg(code)).decode("utf-8")
```

## Comparing `pyzsf-0.1.1.dist-info/COPYING.LESSER` & `pyzsf-0.1.2.dist-info/COPYING.LESSER`

 * *Files identical despite different names*

## Comparing `pyzsf-0.1.1.dist-info/METADATA` & `pyzsf-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzsf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Model for salt intrusion through shipping locks.
 Home-page: https://www.deltares.nl
 Author: Jack Vreeken
 Author-email: jack@vreeken.me
 Maintainer: Jack Vreeken
 License: LGPLv3
 Keywords: zsf shipping locks salt intrusion
```

