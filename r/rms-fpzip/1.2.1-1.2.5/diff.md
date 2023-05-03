# Comparing `tmp/rms_fpzip-1.2.1-cp39-cp39-win_amd64.whl.zip` & `tmp/rms_fpzip-1.2.5-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 98741 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat   299008 b- defN 23-May-02 03:40 fpzip.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      148 b- defN 23-May-02 03:40 rms_fpzip-1.2.1.dist-info/AUTHORS
--rw-rw-rw-  2.0 fat     1556 b- defN 23-May-02 03:40 rms_fpzip-1.2.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3439 b- defN 23-May-02 03:40 rms_fpzip-1.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-02 03:40 rms_fpzip-1.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-02 03:40 rms_fpzip-1.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      568 b- defN 23-May-02 03:40 rms_fpzip-1.2.1.dist-info/RECORD
-7 files, 304825 bytes uncompressed, 97735 bytes compressed:  67.9%
+Zip file size: 98751 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat   299008 b- defN 23-May-03 01:13 fpzip.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      148 b- defN 23-May-03 01:13 rms_fpzip-1.2.5.dist-info/AUTHORS
+-rw-rw-rw-  2.0 fat     1556 b- defN 23-May-03 01:13 rms_fpzip-1.2.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3446 b- defN 23-May-03 01:13 rms_fpzip-1.2.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-03 01:13 rms_fpzip-1.2.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-03 01:13 rms_fpzip-1.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      568 b- defN 23-May-03 01:13 rms_fpzip-1.2.5.dist-info/RECORD
+7 files, 304832 bytes uncompressed, 97745 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: fpzip.cp39-win_amd64.pyd
 Comment: 
 
-Filename: rms_fpzip-1.2.1.dist-info/AUTHORS
+Filename: rms_fpzip-1.2.5.dist-info/AUTHORS
 Comment: 
 
-Filename: rms_fpzip-1.2.1.dist-info/LICENSE
+Filename: rms_fpzip-1.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: rms_fpzip-1.2.1.dist-info/METADATA
+Filename: rms_fpzip-1.2.5.dist-info/METADATA
 Comment: 
 
-Filename: rms_fpzip-1.2.1.dist-info/WHEEL
+Filename: rms_fpzip-1.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: rms_fpzip-1.2.1.dist-info/top_level.txt
+Filename: rms_fpzip-1.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: rms_fpzip-1.2.1.dist-info/RECORD
+Filename: rms_fpzip-1.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rms_fpzip-1.2.1.dist-info/LICENSE` & `rms_fpzip-1.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rms_fpzip-1.2.1.dist-info/METADATA` & `rms_fpzip-1.2.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rms-fpzip
-Version: 1.2.1
+Version: 1.2.5
 Summary: Numpy wrapper for fpzip algorithm (P. Lindstrom & M. Isenburg, 2006) RMS Fork
-Home-page: https://github.com/seung-lab/fpzip/
+Home-page: https://github.com/SETI/pds-fpzip/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 Maintainer: Robert French
 Maintainer-email: rfrench@seti.org
 License: None
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
@@ -49,26 +49,26 @@
 ```
 
 ## Installation
 
 #### `pip` Binary Installation
 
 ```bash
-pip install fpzip
+pip install rms-fpzip
 ```
 
 If we have a precompiled binary available the above command should just work. However, if you have to compile from source, it's unfortunately necessary to install numpy first because of a quirk in the Python installation procedure that won't easily recognize when a numpy installation completes in the same process. There are some hacks, but I haven't gotten them to work.
 
 #### `pip` Source Installation
 
 *Requires C++ compiler.*
 
 ```bash
 pip install numpy
-pip install fpzip
+pip install rms-fpzip
 ```
 
 #### Direct Installation
 
 *Requires C++ compiler.*
 
 ```bash
```

## Comparing `rms_fpzip-1.2.1.dist-info/RECORD` & `rms_fpzip-1.2.5.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-fpzip.cp39-win_amd64.pyd,sha256=LrbvKPJo4IFZ-xUS22iqvae6fB3WHKrjjG6H8sUjhPA,299008
-rms_fpzip-1.2.1.dist-info/AUTHORS,sha256=DWcBA-LLUE0rjzUE8xVO4sA1KzwxWIja0Iu7M1XhvGo,148
-rms_fpzip-1.2.1.dist-info/LICENSE,sha256=8BpZRbaM_5v8SwQlwhblgue4osr-URIVpjiJ7R-Iec8,1556
-rms_fpzip-1.2.1.dist-info/METADATA,sha256=uIxx5qUZHq3FCYBpMlxXbygQ0SQOJ6gv4Wj1a7hJ41Q,3439
-rms_fpzip-1.2.1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-rms_fpzip-1.2.1.dist-info/top_level.txt,sha256=FTQGjjMLAGhaiyzBJhAZTrMW7rzMdVpM-moiFbFZMVk,6
-rms_fpzip-1.2.1.dist-info/RECORD,,
+fpzip.cp39-win_amd64.pyd,sha256=ZjOF4SUlYCP5hABbx4kaeivTanUIRBSt2q_TaX3HxlQ,299008
+rms_fpzip-1.2.5.dist-info/AUTHORS,sha256=DWcBA-LLUE0rjzUE8xVO4sA1KzwxWIja0Iu7M1XhvGo,148
+rms_fpzip-1.2.5.dist-info/LICENSE,sha256=8BpZRbaM_5v8SwQlwhblgue4osr-URIVpjiJ7R-Iec8,1556
+rms_fpzip-1.2.5.dist-info/METADATA,sha256=yAUeWmsARpOiFy2pPFAhj_ky7EGN7qBWbEv3yfTjWAU,3446
+rms_fpzip-1.2.5.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+rms_fpzip-1.2.5.dist-info/top_level.txt,sha256=FTQGjjMLAGhaiyzBJhAZTrMW7rzMdVpM-moiFbFZMVk,6
+rms_fpzip-1.2.5.dist-info/RECORD,,
```

