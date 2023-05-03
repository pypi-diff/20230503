# Comparing `tmp/xia_scw_vpc-0.1.0-cp39-none-manylinux1_x86_64.whl.zip` & `tmp/xia_scw_vpc-0.1.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 242774 bytes, number of entries: 11
--rw-r--r--  2.0 unx       87 b- defN 23-May-02 18:47 xia_scw_vpc/__init__.py
--rw-r--r--  2.0 unx   760232 b- defN 23-May-02 18:50 xia_scw_vpc/vpc.cpython-39-x86_64-linux-gnu.so
+Zip file size: 111352 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       87 b- defN 23-May-03 21:13 xia_scw_vpc/__init__.py
+-rw-r--r--  2.0 unx   263168 b- defN 23-May-03 21:17 xia_scw_vpc/vpc.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 unx     1210 b- defN 23-May-02 08:44 xia_scw_vpc/templates/ScwVpc/main.tf
 -rw-rw-rw-  2.0 unx     1028 b- defN 23-May-02 18:47 xia_scw_vpc/templates/ScwVpc/output.tf
 -rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 13:39 xia_scw_vpc/templates/ScwVpc/provider.tf
 -rw-rw-rw-  2.0 unx     2295 b- defN 23-May-02 08:44 xia_scw_vpc/templates/ScwVpc/variables.tf
--rw-rw-rw-  2.0 unx      150 b- defN 23-May-02 18:50 xia_scw_vpc-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      672 b- defN 23-May-02 18:50 xia_scw_vpc-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      107 b- defN 23-May-02 18:50 xia_scw_vpc-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-02 18:50 xia_scw_vpc-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      974 b- defN 23-May-02 18:50 xia_scw_vpc-0.1.0.dist-info/RECORD
-11 files, 767110 bytes uncompressed, 241102 bytes compressed:  68.6%
+-rw-rw-rw-  2.0 unx      150 b- defN 23-May-03 21:17 xia_scw_vpc-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      672 b- defN 23-May-03 21:17 xia_scw_vpc-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-03 21:17 xia_scw_vpc-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-03 21:17 xia_scw_vpc-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      961 b- defN 23-May-03 21:17 xia_scw_vpc-0.1.1.dist-info/RECORD
+11 files, 270025 bytes uncompressed, 109704 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -1,34 +1,34 @@
 Filename: xia_scw_vpc/__init__.py
 Comment: 
 
-Filename: xia_scw_vpc/vpc.cpython-39-x86_64-linux-gnu.so
+Filename: xia_scw_vpc/vpc.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/main.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/output.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/provider.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/variables.tf
 Comment: 
 
-Filename: xia_scw_vpc-0.1.0.dist-info/LICENSE.txt
+Filename: xia_scw_vpc-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.1.0.dist-info/METADATA
+Filename: xia_scw_vpc-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_vpc-0.1.0.dist-info/WHEEL
+Filename: xia_scw_vpc-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_vpc-0.1.0.dist-info/top_level.txt
+Filename: xia_scw_vpc-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.1.0.dist-info/RECORD
+Filename: xia_scw_vpc-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_vpc/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_vpc.vpc import ScwVpc
 
 
 __all__ = [
     "ScwVpc"
 ]
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## Comparing `xia_scw_vpc-0.1.0.dist-info/METADATA` & `xia_scw_vpc-0.1.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-scw-vpc
-Version: 0.1.0
+Version: 0.1.1
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-vpc/0.1.0/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-vpc/0.1.1/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

