# Comparing `tmp/jaco2-4.4-cp311-cp311-win_amd64.whl.zip` & `tmp/jaco2-4.5-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 499637 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   189952 b- defN 23-May-03 07:00 jaco2.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat   852480 b- defN 23-May-02 18:07 jaco2-4.4.data/data/dll_lib/CommandLayerEthernet.dll
--rw-rw-rw-  2.0 fat   964096 b- defN 23-May-02 18:07 jaco2-4.4.data/data/dll_lib/CommandLayerWindows.dll
--rw-rw-rw-  2.0 fat    18432 b- defN 23-May-02 18:07 jaco2-4.4.data/data/dll_lib/CommunicationLayerEthernet.dll
--rw-rw-rw-  2.0 fat    18432 b- defN 23-May-02 18:07 jaco2-4.4.data/data/dll_lib/CommunicationLayerWindows.dll
--rw-rw-rw-  2.0 fat      138 b- defN 23-May-03 07:00 jaco2-4.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-May-03 07:00 jaco2-4.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-03 07:00 jaco2-4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      817 b- defN 23-May-03 07:00 jaco2-4.4.dist-info/RECORD
-9 files, 2044455 bytes uncompressed, 498221 bytes compressed:  75.6%
+Zip file size: 499636 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   189952 b- defN 23-May-03 07:05 jaco2.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   852480 b- defN 23-May-02 18:07 jaco2-4.5.data/data/dll_lib/CommandLayerEthernet.dll
+-rw-rw-rw-  2.0 fat   964096 b- defN 23-May-02 18:07 jaco2-4.5.data/data/dll_lib/CommandLayerWindows.dll
+-rw-rw-rw-  2.0 fat    18432 b- defN 23-May-02 18:07 jaco2-4.5.data/data/dll_lib/CommunicationLayerEthernet.dll
+-rw-rw-rw-  2.0 fat    18432 b- defN 23-May-02 18:07 jaco2-4.5.data/data/dll_lib/CommunicationLayerWindows.dll
+-rw-rw-rw-  2.0 fat      138 b- defN 23-May-03 07:05 jaco2-4.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-May-03 07:05 jaco2-4.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-03 07:05 jaco2-4.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      817 b- defN 23-May-03 07:05 jaco2-4.5.dist-info/RECORD
+9 files, 2044455 bytes uncompressed, 498220 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: jaco2.cp311-win_amd64.pyd
 Comment: 
 
-Filename: jaco2-4.4.data/data/dll_lib/CommandLayerEthernet.dll
+Filename: jaco2-4.5.data/data/dll_lib/CommandLayerEthernet.dll
 Comment: 
 
-Filename: jaco2-4.4.data/data/dll_lib/CommandLayerWindows.dll
+Filename: jaco2-4.5.data/data/dll_lib/CommandLayerWindows.dll
 Comment: 
 
-Filename: jaco2-4.4.data/data/dll_lib/CommunicationLayerEthernet.dll
+Filename: jaco2-4.5.data/data/dll_lib/CommunicationLayerEthernet.dll
 Comment: 
 
-Filename: jaco2-4.4.data/data/dll_lib/CommunicationLayerWindows.dll
+Filename: jaco2-4.5.data/data/dll_lib/CommunicationLayerWindows.dll
 Comment: 
 
-Filename: jaco2-4.4.dist-info/METADATA
+Filename: jaco2-4.5.dist-info/METADATA
 Comment: 
 
-Filename: jaco2-4.4.dist-info/WHEEL
+Filename: jaco2-4.5.dist-info/WHEEL
 Comment: 
 
-Filename: jaco2-4.4.dist-info/top_level.txt
+Filename: jaco2-4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: jaco2-4.4.dist-info/RECORD
+Filename: jaco2-4.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `jaco2-4.4.data/data/dll_lib/CommandLayerEthernet.dll` & `jaco2-4.5.data/data/dll_lib/CommandLayerEthernet.dll`

 * *Files identical despite different names*

## Comparing `jaco2-4.4.data/data/dll_lib/CommandLayerWindows.dll` & `jaco2-4.5.data/data/dll_lib/CommandLayerWindows.dll`

 * *Files identical despite different names*

## Comparing `jaco2-4.4.data/data/dll_lib/CommunicationLayerEthernet.dll` & `jaco2-4.5.data/data/dll_lib/CommunicationLayerEthernet.dll`

 * *Files identical despite different names*

## Comparing `jaco2-4.4.data/data/dll_lib/CommunicationLayerWindows.dll` & `jaco2-4.5.data/data/dll_lib/CommunicationLayerWindows.dll`

 * *Files identical despite different names*

## Comparing `jaco2-4.4.dist-info/RECORD` & `jaco2-4.5.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-jaco2.cp311-win_amd64.pyd,sha256=HhwcWhwChvRNhDRsHODDzkABVmLrp6GLm35Gh7FJC_I,189952
-jaco2-4.4.data/data/dll_lib/CommandLayerEthernet.dll,sha256=lhQSk5BThZq08hlUqYpi502HkyqD2N2gWwFwFf9rfWo,852480
-jaco2-4.4.data/data/dll_lib/CommandLayerWindows.dll,sha256=S_aG-N5io4SLhQygL_ha61H0hyxBdDd70fbDBbP17Tg,964096
-jaco2-4.4.data/data/dll_lib/CommunicationLayerEthernet.dll,sha256=_ZpKgL-ckpUeo2bDYJcYz1YXdHM5WizbjCIF0Ee_fls,18432
-jaco2-4.4.data/data/dll_lib/CommunicationLayerWindows.dll,sha256=wuQHFK5ZUV45sd0G-q0NuIrhlGteCl6BVfZL6TIx2gE,18432
-jaco2-4.4.dist-info/METADATA,sha256=g-EwXZXwaERrqIId9jHbEt1caB_TX3czFKzmVmJ9IqQ,138
-jaco2-4.4.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
-jaco2-4.4.dist-info/top_level.txt,sha256=96aeDvzyMwwznUlytOi2AlCWWw2vNLUuaOddMOdt0AY,6
-jaco2-4.4.dist-info/RECORD,,
+jaco2.cp311-win_amd64.pyd,sha256=GRhOSxtWwse8kUBUHtQlNa6hP0CqK1BbMJ5QEbdZZZc,189952
+jaco2-4.5.data/data/dll_lib/CommandLayerEthernet.dll,sha256=lhQSk5BThZq08hlUqYpi502HkyqD2N2gWwFwFf9rfWo,852480
+jaco2-4.5.data/data/dll_lib/CommandLayerWindows.dll,sha256=S_aG-N5io4SLhQygL_ha61H0hyxBdDd70fbDBbP17Tg,964096
+jaco2-4.5.data/data/dll_lib/CommunicationLayerEthernet.dll,sha256=_ZpKgL-ckpUeo2bDYJcYz1YXdHM5WizbjCIF0Ee_fls,18432
+jaco2-4.5.data/data/dll_lib/CommunicationLayerWindows.dll,sha256=wuQHFK5ZUV45sd0G-q0NuIrhlGteCl6BVfZL6TIx2gE,18432
+jaco2-4.5.dist-info/METADATA,sha256=uXOJwf-e6Hz5-MtTOkNQ9m15VDi06h0X7iUkOGmoYfw,138
+jaco2-4.5.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
+jaco2-4.5.dist-info/top_level.txt,sha256=96aeDvzyMwwznUlytOi2AlCWWw2vNLUuaOddMOdt0AY,6
+jaco2-4.5.dist-info/RECORD,,
```

