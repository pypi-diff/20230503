# Comparing `tmp/synchronicity-0.4.3-py3-none-any.whl.zip` & `tmp/synchronicity-0.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 19758 bytes, number of entries: 12
+Zip file size: 19907 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       72 b- defN 22-Mar-21 08:08 synchronicity/__init__.py
--rw-rw-r--  2.0 unx     2547 b- defN 23-Apr-03 08:46 synchronicity/async_wrap.py
+-rw-rw-r--  2.0 unx     2547 b- defN 23-Apr-24 07:29 synchronicity/async_wrap.py
 -rw-rw-r--  2.0 unx     1485 b- defN 23-Mar-23 14:53 synchronicity/callback.py
 -rw-rw-r--  2.0 unx     1303 b- defN 23-Mar-20 08:05 synchronicity/exceptions.py
 -rw-rw-r--  2.0 unx      136 b- defN 23-Mar-29 14:29 synchronicity/interface.py
--rw-rw-r--  2.0 unx     1694 b- defN 23-Apr-03 08:46 synchronicity/overload_tracking.py
--rw-rw-r--  2.0 unx    25247 b- defN 23-Apr-05 06:55 synchronicity/synchronizer.py
--rw-rw-r--  2.0 unx    22482 b- defN 23-Apr-04 07:22 synchronicity/type_stubs.py
--rw-rw-r--  2.0 unx     7736 b- defN 23-Apr-06 13:08 synchronicity-0.4.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-06 13:08 synchronicity-0.4.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Apr-06 13:08 synchronicity-0.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      997 b- defN 23-Apr-06 13:08 synchronicity-0.4.3.dist-info/RECORD
-12 files, 63805 bytes uncompressed, 18080 bytes compressed:  71.7%
+-rw-rw-r--  2.0 unx     1694 b- defN 23-May-03 14:36 synchronicity/overload_tracking.py
+-rw-rw-r--  2.0 unx    25602 b- defN 23-May-03 19:40 synchronicity/synchronizer.py
+-rw-rw-r--  2.0 unx    22482 b- defN 23-Apr-24 07:29 synchronicity/type_stubs.py
+-rw-rw-r--  2.0 unx     7736 b- defN 23-May-03 19:47 synchronicity-0.4.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-03 19:47 synchronicity-0.4.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-May-03 19:47 synchronicity-0.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      997 b- defN 23-May-03 19:47 synchronicity-0.4.4.dist-info/RECORD
+12 files, 64160 bytes uncompressed, 18229 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: synchronicity/synchronizer.py
 Comment: 
 
 Filename: synchronicity/type_stubs.py
 Comment: 
 
-Filename: synchronicity-0.4.3.dist-info/METADATA
+Filename: synchronicity-0.4.4.dist-info/METADATA
 Comment: 
 
-Filename: synchronicity-0.4.3.dist-info/WHEEL
+Filename: synchronicity-0.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: synchronicity-0.4.3.dist-info/top_level.txt
+Filename: synchronicity-0.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: synchronicity-0.4.3.dist-info/RECORD
+Filename: synchronicity-0.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## synchronicity/synchronizer.py

```diff
@@ -17,14 +17,18 @@
 _BUILTIN_ASYNC_METHODS = {
     "__aiter__": "__iter__",
     "__aenter__": "__enter__",
     "__aexit__": "__exit__",
     "__anext__": "__next__",
 }
 
+IGNORED_ATTRIBUTES = (
+    "__provides__",  # the "zope" lib monkey patches in some non-introspectable stuff on stdlib abc.ABC. Ignoring __provides__ fixes an incompatibility with `channels[daphne]`, where Synchronizer creation fails when wrapping contextlib._AsyncGeneratorContextManager
+)
+
 _RETURN_FUTURE_KWARG = "_future"
 
 # Default names for classes
 _CLASS_PREFIXES = {
     Interface.BLOCKING: "Blocking",
     Interface.ASYNC: "Async",
 }
@@ -506,14 +510,16 @@
                     new_dict[k] = self._wrap_proxy_method(
                         v, interface, allow_futures=False
                     )
             elif k in ("__new__", "__init__"):
                 # Skip custom constructor in the wrapped class
                 # Instead, delegate to the base class constructor and wrap it
                 pass
+            elif k in IGNORED_ATTRIBUTES:
+                pass
             elif isinstance(v, staticmethod):
                 # TODO(erikbern): this feels pretty hacky
                 new_dict[k] = self._wrap_proxy_staticmethod(v, interface)
             elif isinstance(v, classmethod):
                 new_dict[k] = self._wrap_proxy_classmethod(v, interface)
             elif isinstance(v, property):
                 new_dict[k] = self._wrap_proxy_property(v, interface)
```

## Comparing `synchronicity-0.4.3.dist-info/METADATA` & `synchronicity-0.4.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synchronicity
-Version: 0.4.3
+Version: 0.4.4
 Summary: Export blocking and async library versions from a single async implementation
 Requires-Python: >=3.7.9
 Description-Content-Type: text/markdown
 Requires-Dist: sigtools (==4.0.1)
 
 ![CI/CD badge](https://github.com/erikbern/synchronicity/actions/workflows/ci.yml/badge.svg)
 [![pypi badge](https://img.shields.io/pypi/v/synchronicity.svg?style=flat)](https://pypi.python.org/pypi/synchronicity)
```

## Comparing `synchronicity-0.4.3.dist-info/RECORD` & `synchronicity-0.4.4.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 synchronicity/__init__.py,sha256=Q3dvKSQ-AUXnBfRe-utqSWh6mE9wV1kDoizoVtg_gxI,72
 synchronicity/async_wrap.py,sha256=ejbLikhxeGhL3-0pvCCJ145HU8GhN2UpUMOAbja4wAY,2547
 synchronicity/callback.py,sha256=ZPCfzrZkaepalwEmvxdfYewHEc059hDKFz_7oXIdIoY,1485
 synchronicity/exceptions.py,sha256=pJw_RhOvRSr-sMhSRLmCzNb1M5W36W4EFfeE0FD27OA,1303
 synchronicity/interface.py,sha256=9SVPl_zRhQs030LfDQ4_d_emsNkmlM-A7DL45P7JzAU,136
 synchronicity/overload_tracking.py,sha256=cfdar8Mc8gRYMY0HPInIIAW2FyH_-d_vCbM8h-x6_90,1694
-synchronicity/synchronizer.py,sha256=QLPUE6M6U6PXKJjkAMyeTs_yK-Jua74I7ywW9pygJ4U,25247
+synchronicity/synchronizer.py,sha256=TvZ0zUGDHVp6SKAb4ZyYqc1IV7v29Bce1u69RSEfR_4,25602
 synchronicity/type_stubs.py,sha256=hGE23W4ov1bBLB0mH8tZnQsIMd7mDLaHd5z-ZezSjss,22482
-synchronicity-0.4.3.dist-info/METADATA,sha256=UhDGh9GopCQk9KYsu_Wm2J1PPSTsc_5cXNm2HI9-_-Y,7736
-synchronicity-0.4.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-synchronicity-0.4.3.dist-info/top_level.txt,sha256=pqAkRTgp1bdeADR7z1vhyQijkZNYCCsezJKpOwFizoE,14
-synchronicity-0.4.3.dist-info/RECORD,,
+synchronicity-0.4.4.dist-info/METADATA,sha256=c_J9aHdAx8L8jGGxpeSaGc6zBnCrrl-KcNSFfLwLzyQ,7736
+synchronicity-0.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+synchronicity-0.4.4.dist-info/top_level.txt,sha256=pqAkRTgp1bdeADR7z1vhyQijkZNYCCsezJKpOwFizoE,14
+synchronicity-0.4.4.dist-info/RECORD,,
```

