# Comparing `tmp/pyzsf-0.1.2-cp36-abi3-win_amd64.whl.zip` & `tmp/pyzsf-0.1.3-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 21287 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      128 b- defN 21-Nov-09 14:46 pyzsf/__init__.py
--rw-rw-rw-  2.0 fat    34816 b- defN 21-Nov-09 14:52 pyzsf/_zsf_cffi.pyd
--rw-rw-rw-  2.0 fat     7910 b- defN 21-Nov-09 14:46 pyzsf/pyzsf.py
--rw-rw-rw-  2.0 fat     7817 b- defN 21-Nov-09 14:52 pyzsf-0.1.2.dist-info/COPYING.LESSER
--rw-rw-rw-  2.0 fat     1018 b- defN 21-Nov-09 14:52 pyzsf-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 21-Nov-09 14:52 pyzsf-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 21-Nov-09 14:52 pyzsf-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      604 b- defN 21-Nov-09 14:52 pyzsf-0.1.2.dist-info/RECORD
-8 files, 52399 bytes uncompressed, 20245 bytes compressed:  61.4%
+Zip file size: 21442 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      128 b- defN 23-May-03 13:00 pyzsf/__init__.py
+-rw-rw-rw-  2.0 fat    35328 b- defN 23-May-03 13:02 pyzsf/_zsf_cffi.pyd
+-rw-rw-rw-  2.0 fat     7910 b- defN 23-May-03 13:00 pyzsf/pyzsf.py
+-rw-rw-rw-  2.0 fat     7817 b- defN 23-May-03 13:02 pyzsf-0.1.3.dist-info/COPYING.LESSER
+-rw-rw-rw-  2.0 fat     1050 b- defN 23-May-03 13:02 pyzsf-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-03 13:02 pyzsf-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-03 13:02 pyzsf-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      604 b- defN 23-May-03 13:02 pyzsf-0.1.3.dist-info/RECORD
+8 files, 52943 bytes uncompressed, 20400 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: pyzsf/_zsf_cffi.pyd
 Comment: 
 
 Filename: pyzsf/pyzsf.py
 Comment: 
 
-Filename: pyzsf-0.1.2.dist-info/COPYING.LESSER
+Filename: pyzsf-0.1.3.dist-info/COPYING.LESSER
 Comment: 
 
-Filename: pyzsf-0.1.2.dist-info/METADATA
+Filename: pyzsf-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: pyzsf-0.1.2.dist-info/WHEEL
+Filename: pyzsf-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyzsf-0.1.2.dist-info/top_level.txt
+Filename: pyzsf-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyzsf-0.1.2.dist-info/RECORD
+Filename: pyzsf-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyzsf-0.1.2.dist-info/COPYING.LESSER` & `pyzsf-0.1.3.dist-info/COPYING.LESSER`

 * *Files identical despite different names*

## Comparing `pyzsf-0.1.2.dist-info/METADATA` & `pyzsf-0.1.3.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1
-Name: pyzsf
-Version: 0.1.2
-Summary: Model for salt intrusion through shipping locks.
-Home-page: https://www.deltares.nl
-Author: Jack Vreeken
-Author-email: jack@vreeken.me
-Maintainer: Jack Vreeken
-License: LGPLv3
-Keywords: zsf shipping locks salt intrusion
-Platform: Windows
-Platform: Linux
-Platform: Mac OS-X
-Platform: Unix
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Other
-Classifier: Topic :: Scientific/Engineering :: GIS
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.6
-Requires-Dist: cffi (>=1.0.0)
-
-UNKNOWN
-
-
+Metadata-Version: 2.1
+Name: pyzsf
+Version: 0.1.3
+Summary: Model for salt intrusion through shipping locks.
+Home-page: https://www.deltares.nl
+Author: Jack Vreeken
+Author-email: jack@vreeken.me
+Maintainer: Jack Vreeken
+License: LGPLv3
+Keywords: zsf shipping locks salt intrusion
+Platform: Windows
+Platform: Linux
+Platform: Mac OS-X
+Platform: Unix
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Other
+Classifier: Topic :: Scientific/Engineering :: GIS
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Requires-Python: >=3.6
+Requires-Dist: cffi (>=1.0.0)
+
+UNKNOWN
+
+
```

