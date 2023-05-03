# Comparing `tmp/jaco2-3.7-cp311-cp311-win_amd64.whl.zip` & `tmp/jaco2-3.8-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 499628 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   189952 b- defN 23-May-03 05:26 jaco2.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat   852480 b- defN 23-May-02 18:07 jaco2-3.7.data/data/dll_lib/CommandLayerEthernet.dll
--rw-rw-rw-  2.0 fat   964096 b- defN 23-May-02 18:07 jaco2-3.7.data/data/dll_lib/CommandLayerWindows.dll
--rw-rw-rw-  2.0 fat    18432 b- defN 23-May-02 18:07 jaco2-3.7.data/data/dll_lib/CommunicationLayerEthernet.dll
--rw-rw-rw-  2.0 fat    18432 b- defN 23-May-02 18:07 jaco2-3.7.data/data/dll_lib/CommunicationLayerWindows.dll
--rw-rw-rw-  2.0 fat      138 b- defN 23-May-03 05:26 jaco2-3.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-May-03 05:26 jaco2-3.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-03 05:26 jaco2-3.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      817 b- defN 23-May-03 05:26 jaco2-3.7.dist-info/RECORD
-9 files, 2044455 bytes uncompressed, 498212 bytes compressed:  75.6%
+Zip file size: 499894 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   190464 b- defN 23-May-03 05:42 jaco2.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   852480 b- defN 23-May-02 18:07 jaco2-3.8.data/data/dll_lib/CommandLayerEthernet.dll
+-rw-rw-rw-  2.0 fat   964096 b- defN 23-May-02 18:07 jaco2-3.8.data/data/dll_lib/CommandLayerWindows.dll
+-rw-rw-rw-  2.0 fat    18432 b- defN 23-May-02 18:07 jaco2-3.8.data/data/dll_lib/CommunicationLayerEthernet.dll
+-rw-rw-rw-  2.0 fat    18432 b- defN 23-May-02 18:07 jaco2-3.8.data/data/dll_lib/CommunicationLayerWindows.dll
+-rw-rw-rw-  2.0 fat      138 b- defN 23-May-03 05:42 jaco2-3.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-May-03 05:42 jaco2-3.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-03 05:42 jaco2-3.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      817 b- defN 23-May-03 05:42 jaco2-3.8.dist-info/RECORD
+9 files, 2044967 bytes uncompressed, 498478 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: jaco2.cp311-win_amd64.pyd
 Comment: 
 
-Filename: jaco2-3.7.data/data/dll_lib/CommandLayerEthernet.dll
+Filename: jaco2-3.8.data/data/dll_lib/CommandLayerEthernet.dll
 Comment: 
 
-Filename: jaco2-3.7.data/data/dll_lib/CommandLayerWindows.dll
+Filename: jaco2-3.8.data/data/dll_lib/CommandLayerWindows.dll
 Comment: 
 
-Filename: jaco2-3.7.data/data/dll_lib/CommunicationLayerEthernet.dll
+Filename: jaco2-3.8.data/data/dll_lib/CommunicationLayerEthernet.dll
 Comment: 
 
-Filename: jaco2-3.7.data/data/dll_lib/CommunicationLayerWindows.dll
+Filename: jaco2-3.8.data/data/dll_lib/CommunicationLayerWindows.dll
 Comment: 
 
-Filename: jaco2-3.7.dist-info/METADATA
+Filename: jaco2-3.8.dist-info/METADATA
 Comment: 
 
-Filename: jaco2-3.7.dist-info/WHEEL
+Filename: jaco2-3.8.dist-info/WHEEL
 Comment: 
 
-Filename: jaco2-3.7.dist-info/top_level.txt
+Filename: jaco2-3.8.dist-info/top_level.txt
 Comment: 
 
-Filename: jaco2-3.7.dist-info/RECORD
+Filename: jaco2-3.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `jaco2-3.7.data/data/dll_lib/CommandLayerEthernet.dll` & `jaco2-3.8.data/data/dll_lib/CommandLayerEthernet.dll`

 * *Files identical despite different names*

## Comparing `jaco2-3.7.data/data/dll_lib/CommandLayerWindows.dll` & `jaco2-3.8.data/data/dll_lib/CommandLayerWindows.dll`

 * *Files identical despite different names*

## Comparing `jaco2-3.7.data/data/dll_lib/CommunicationLayerEthernet.dll` & `jaco2-3.8.data/data/dll_lib/CommunicationLayerEthernet.dll`

 * *Files identical despite different names*

## Comparing `jaco2-3.7.data/data/dll_lib/CommunicationLayerWindows.dll` & `jaco2-3.8.data/data/dll_lib/CommunicationLayerWindows.dll`

 * *Files identical despite different names*

## Comparing `jaco2-3.7.dist-info/RECORD` & `jaco2-3.8.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-jaco2.cp311-win_amd64.pyd,sha256=ACZO9Zj-D8mwOkBq30YnONM_MYsuH6igrIcv8Gb6EBs,189952
-jaco2-3.7.data/data/dll_lib/CommandLayerEthernet.dll,sha256=lhQSk5BThZq08hlUqYpi502HkyqD2N2gWwFwFf9rfWo,852480
-jaco2-3.7.data/data/dll_lib/CommandLayerWindows.dll,sha256=S_aG-N5io4SLhQygL_ha61H0hyxBdDd70fbDBbP17Tg,964096
-jaco2-3.7.data/data/dll_lib/CommunicationLayerEthernet.dll,sha256=_ZpKgL-ckpUeo2bDYJcYz1YXdHM5WizbjCIF0Ee_fls,18432
-jaco2-3.7.data/data/dll_lib/CommunicationLayerWindows.dll,sha256=wuQHFK5ZUV45sd0G-q0NuIrhlGteCl6BVfZL6TIx2gE,18432
-jaco2-3.7.dist-info/METADATA,sha256=68BrUcHluB-IP4n1Ui9ivciNJghBjaIocDnvv3E4LA8,138
-jaco2-3.7.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
-jaco2-3.7.dist-info/top_level.txt,sha256=96aeDvzyMwwznUlytOi2AlCWWw2vNLUuaOddMOdt0AY,6
-jaco2-3.7.dist-info/RECORD,,
+jaco2.cp311-win_amd64.pyd,sha256=StiuL3TXC5-m6kudzd73TrZtVwPpvua-ta9TyU9s2Ls,190464
+jaco2-3.8.data/data/dll_lib/CommandLayerEthernet.dll,sha256=lhQSk5BThZq08hlUqYpi502HkyqD2N2gWwFwFf9rfWo,852480
+jaco2-3.8.data/data/dll_lib/CommandLayerWindows.dll,sha256=S_aG-N5io4SLhQygL_ha61H0hyxBdDd70fbDBbP17Tg,964096
+jaco2-3.8.data/data/dll_lib/CommunicationLayerEthernet.dll,sha256=_ZpKgL-ckpUeo2bDYJcYz1YXdHM5WizbjCIF0Ee_fls,18432
+jaco2-3.8.data/data/dll_lib/CommunicationLayerWindows.dll,sha256=wuQHFK5ZUV45sd0G-q0NuIrhlGteCl6BVfZL6TIx2gE,18432
+jaco2-3.8.dist-info/METADATA,sha256=7DT96HW5854qkaObs15GM93uG6Y466BOnqcIDYX9Bts,138
+jaco2-3.8.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
+jaco2-3.8.dist-info/top_level.txt,sha256=96aeDvzyMwwznUlytOi2AlCWWw2vNLUuaOddMOdt0AY,6
+jaco2-3.8.dist-info/RECORD,,
```

