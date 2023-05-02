# Comparing `tmp/ksos-4.9.0-py3-none-any.whl.zip` & `tmp/ksos-4.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 3801 bytes, number of entries: 10
--rw-r--r--  2.0 unx      539 b- defN 23-Jan-18 16:06 ksos-4.9.0-py3.7-nspkg.pth
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-18 16:04 kelvin/ksos/__init__.py
--rw-r--r--  2.0 unx     2049 b- defN 23-Jan-18 16:04 kelvin/ksos/ksos.py
--rw-r--r--  2.0 unx     1252 b- defN 23-Jan-18 16:06 ksos-4.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-18 16:06 ksos-4.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jan-18 16:06 ksos-4.9.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-18 16:06 ksos-4.9.0.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-18 16:06 ksos-4.9.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jan-18 16:06 ksos-4.9.0.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      792 b- defN 23-Jan-18 16:06 ksos-4.9.0.dist-info/RECORD
-10 files, 4786 bytes uncompressed, 2433 bytes compressed:  49.2%
+Zip file size: 3800 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      539 b- defN 23-Jan-19 14:20 ksos-4.9.1-py3.7-nspkg.pth
+-rw-r--r--  2.0 unx        0 b- defN 23-Jan-19 14:18 kelvin/ksos/__init__.py
+-rw-r--r--  2.0 unx     2049 b- defN 23-Jan-19 14:18 kelvin/ksos/ksos.py
+-rw-r--r--  2.0 unx     1252 b- defN 23-Jan-19 14:20 ksos-4.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jan-19 14:20 ksos-4.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jan-19 14:20 ksos-4.9.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jan-19 14:20 ksos-4.9.1.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jan-19 14:20 ksos-4.9.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jan-19 14:20 ksos-4.9.1.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      792 b- defN 23-Jan-19 14:20 ksos-4.9.1.dist-info/RECORD
+10 files, 4786 bytes uncompressed, 2432 bytes compressed:  49.2%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
-Filename: ksos-4.9.0-py3.7-nspkg.pth
+Filename: ksos-4.9.1-py3.7-nspkg.pth
 Comment: 
 
 Filename: kelvin/ksos/__init__.py
 Comment: 
 
 Filename: kelvin/ksos/ksos.py
 Comment: 
 
-Filename: ksos-4.9.0.dist-info/METADATA
+Filename: ksos-4.9.1.dist-info/METADATA
 Comment: 
 
-Filename: ksos-4.9.0.dist-info/WHEEL
+Filename: ksos-4.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: ksos-4.9.0.dist-info/entry_points.txt
+Filename: ksos-4.9.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ksos-4.9.0.dist-info/namespace_packages.txt
+Filename: ksos-4.9.1.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: ksos-4.9.0.dist-info/top_level.txt
+Filename: ksos-4.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ksos-4.9.0.dist-info/zip-safe
+Filename: ksos-4.9.1.dist-info/zip-safe
 Comment: 
 
-Filename: ksos-4.9.0.dist-info/RECORD
+Filename: ksos-4.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ksos-4.9.0-py3.7-nspkg.pth` & `ksos-4.9.1-py3.7-nspkg.pth`

 * *Files identical despite different names*

## Comparing `ksos-4.9.0.dist-info/METADATA` & `ksos-4.9.1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ksos
-Version: 4.9.0
+Version: 4.9.1
 Summary: KSOS
 Home-page: https://kelvininc.com/
 Author: Kelvin Inc
 Author-email: engineering@kelvininc.com
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.7.0
 Description-Content-Type: text/markdown
 Requires-Dist: click (==8.0.*)
-Requires-Dist: kelvin-sdk (==7.8.0)
+Requires-Dist: kelvin-sdk (==7.8.1)
 
 # KSOS
 
 The Kelvin Sustainable Operations Software (KSOS) package provides tools that enable users to interact with the KSOS Platform through the command line interface.  KSOS is the AI software platform for building and managing control applications.  Control applications combine insights, events and actions into powerful automation workflows.   KSOS provides tools and interfaces to ease the effort of data science, app development, testing, validation, management, and finally orchestration and deployment.
 
 For additional information, visit https://docs.kelvininc.com or contact support@kelvininc.com.
```

## Comparing `ksos-4.9.0.dist-info/RECORD` & `ksos-4.9.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-ksos-4.9.0-py3.7-nspkg.pth,sha256=1fbcbyIee7ejR5PY4F-Y4WRcRImE9tlGFfrkB8u09Vs,539
+ksos-4.9.1-py3.7-nspkg.pth,sha256=1fbcbyIee7ejR5PY4F-Y4WRcRImE9tlGFfrkB8u09Vs,539
 kelvin/ksos/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kelvin/ksos/ksos.py,sha256=AUOjm5MXBcFzX4P7lYcNUmlsaTYMN4sDyx1iL4PJrQU,2049
-ksos-4.9.0.dist-info/METADATA,sha256=LzWjcHgIbf89_bIpL6ygkQwrEFQE5rWlRVtxzIxjn4E,1252
-ksos-4.9.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-ksos-4.9.0.dist-info/entry_points.txt,sha256=58hzWN1RTCZwQzSt44Eoymv1oMNMiknKvfG7h4gBRzM,47
-ksos-4.9.0.dist-info/namespace_packages.txt,sha256=_6yecVlTrSwEnjc4lO27C8g1RL1Rey_1FVZgL4PjUYY,7
-ksos-4.9.0.dist-info/top_level.txt,sha256=_6yecVlTrSwEnjc4lO27C8g1RL1Rey_1FVZgL4PjUYY,7
-ksos-4.9.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ksos-4.9.0.dist-info/RECORD,,
+ksos-4.9.1.dist-info/METADATA,sha256=0FAo--pBxotyGsJlenpfejbmCdwb1-P0tGEm6P4b7qE,1252
+ksos-4.9.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+ksos-4.9.1.dist-info/entry_points.txt,sha256=58hzWN1RTCZwQzSt44Eoymv1oMNMiknKvfG7h4gBRzM,47
+ksos-4.9.1.dist-info/namespace_packages.txt,sha256=_6yecVlTrSwEnjc4lO27C8g1RL1Rey_1FVZgL4PjUYY,7
+ksos-4.9.1.dist-info/top_level.txt,sha256=_6yecVlTrSwEnjc4lO27C8g1RL1Rey_1FVZgL4PjUYY,7
+ksos-4.9.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ksos-4.9.1.dist-info/RECORD,,
```

