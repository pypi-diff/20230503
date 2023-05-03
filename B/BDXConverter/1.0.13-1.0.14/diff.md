# Comparing `tmp/BDXConverter-1.0.13.tar.gz` & `tmp/BDXConverter-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDXConverter-1.0.13.tar", last modified: Wed May  3 07:22:36 2023, max compression
+gzip compressed data, was "BDXConverter-1.0.14.tar", last modified: Wed May  3 07:50:47 2023, max compression
```

## Comparing `BDXConverter-1.0.13.tar` & `BDXConverter-1.0.14.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:22:36.006907 BDXConverter-1.0.13/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:22:35.998906 BDXConverter-1.0.13/BDXConverter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:22:35.998906 BDXConverter-1.0.13/BDXConverter/Converter/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Converter/ConvertErrorDefine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Converter/Converter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:22:36.002907 BDXConverter-1.0.13/BDXConverter/General/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/General/GeneralClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/General/Pool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/General/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:22:36.006907 BDXConverter-1.0.13/BDXConverter/Operation/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddInt16XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddInt16YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddInt16ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddInt16ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddInt32XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddInt32YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddInt32ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddInt32ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddInt8XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddInt8YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddInt8ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AddZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/AssignDebugData.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/CreateConstantString.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/NOP.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlockWithBlockStates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlockWithNBTData.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/PlaceRuntimeBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/SetCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/SubtractXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/SubtractYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/SubtractZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/Terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/UseRuntimeIDPool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/Operation/structOfChest.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:22:36.006907 BDXConverter-1.0.13/BDXConverter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/utils/getByte.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/utils/getString.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/utils/marshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/utils/marshalNBT_OldVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/utils/unmarshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/BDXConverter/utils/unmarshalNBT_OldVersion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:22:35.998906 BDXConverter-1.0.13/BDXConverter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-03 07:22:35.000000 BDXConverter-1.0.13/BDXConverter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-03 07:22:35.000000 BDXConverter-1.0.13/BDXConverter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 07:22:35.000000 BDXConverter-1.0.13/BDXConverter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-03 07:22:35.000000 BDXConverter-1.0.13/BDXConverter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 07:22:35.000000 BDXConverter-1.0.13/BDXConverter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-03 07:22:36.006907 BDXConverter-1.0.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 07:22:36.006907 BDXConverter-1.0.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-03 07:22:22.000000 BDXConverter-1.0.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.862207 BDXConverter-1.0.14/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.846207 BDXConverter-1.0.14/BDXConverter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.846207 BDXConverter-1.0.14/BDXConverter/Converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Converter/ConvertErrorDefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Converter/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.846207 BDXConverter-1.0.14/BDXConverter/General/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/General/GeneralClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/General/Pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/General/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.858207 BDXConverter-1.0.14/BDXConverter/Operation/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt16XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt16YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt16ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt16ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt32XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt32YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt32ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt32ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt8XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt8YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddInt8ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AddZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/AssignDebugData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/CreateConstantString.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/NOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithBlockStates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithNBTData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/SetCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/SubtractXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/SubtractYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/SubtractZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/Terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/UseRuntimeIDPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/Operation/structOfChest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.862207 BDXConverter-1.0.14/BDXConverter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/getByte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/getString.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/marshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/marshalNBT_OldVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/unmarshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/BDXConverter/utils/unmarshalNBT_OldVersion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:50:47.846207 BDXConverter-1.0.14/BDXConverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-03 07:50:47.000000 BDXConverter-1.0.14/BDXConverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-03 07:50:47.000000 BDXConverter-1.0.14/BDXConverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 07:50:47.000000 BDXConverter-1.0.14/BDXConverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-03 07:50:47.000000 BDXConverter-1.0.14/BDXConverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 07:50:47.000000 BDXConverter-1.0.14/BDXConverter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-03 07:50:47.862207 BDXConverter-1.0.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 07:50:47.862207 BDXConverter-1.0.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-03 07:50:34.000000 BDXConverter-1.0.14/setup.py
```

### Comparing `BDXConverter-1.0.13/BDXConverter/Converter/ConvertErrorDefine.py` & `BDXConverter-1.0.14/BDXConverter/Converter/ConvertErrorDefine.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Converter/Converter.py` & `BDXConverter-1.0.14/BDXConverter/Converter/Converter.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/General/GeneralClass.py` & `BDXConverter-1.0.14/BDXConverter/General/GeneralClass.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/General/Pool.py` & `BDXConverter-1.0.14/BDXConverter/General/Pool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/AddInt16XValue.py` & `BDXConverter-1.0.14/BDXConverter/Operation/AddInt16XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/AddInt16YValue.py` & `BDXConverter-1.0.14/BDXConverter/Operation/AddInt16YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/AddInt16ZValue.py` & `BDXConverter-1.0.14/BDXConverter/Operation/AddInt16ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/AddInt16ZValue0.py` & `BDXConverter-1.0.14/BDXConverter/Operation/AddInt16ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/AddInt32XValue.py` & `BDXConverter-1.0.14/BDXConverter/Operation/AddInt32XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/AddInt32YValue.py` & `BDXConverter-1.0.14/BDXConverter/Operation/AddInt32YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/AddInt32ZValue.py` & `BDXConverter-1.0.14/BDXConverter/Operation/AddInt32ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/AddInt32ZValue0.py` & `BDXConverter-1.0.14/BDXConverter/Operation/AddInt32ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/AddInt8XValue.py` & `BDXConverter-1.0.14/BDXConverter/Operation/AddInt8XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/AddInt8YValue.py` & `BDXConverter-1.0.14/BDXConverter/Operation/AddInt8YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/AddInt8ZValue.py` & `BDXConverter-1.0.14/BDXConverter/Operation/AddInt8ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/AssignDebugData.py` & `BDXConverter-1.0.14/BDXConverter/Operation/AssignDebugData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/CreateConstantString.py` & `BDXConverter-1.0.14/BDXConverter/Operation/CreateConstantString.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlock.py` & `BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlockWithBlockStates.py` & `BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithBlockStates.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py` & `BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlockWithChestData.py` & `BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py` & `BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlockWithNBTData.py` & `BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithNBTData.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-import nbtlib, sys
+import nbtlib
+import sys
 from io import BytesIO
 from struct import pack, unpack
 from ..General.GeneralClass import GeneralClass
 from ..utils.getByte import getByte
 
 
-if sys.version_info.major>=3 and sys.version_info.minor>=10:
+if sys.version_info.major >= 3 and sys.version_info.minor >= 10:
     from ..utils.marshalNBT import MarshalPythonNBTObjectToWriter
     from ..utils.unmarshalNBT import UnMarshalBufferToPythonNBTObject
 else:
     from ..utils.marshalNBT_OldVersion import MarshalPythonNBTObjectToWriter
     from ..utils.unmarshalNBT_OldVersion import UnMarshalBufferToPythonNBTObject
 
 
 class PlaceBlockWithNBTData(GeneralClass):
     def __init__(self) -> None:
         self.operationName: str = 'PlaceBlockWithNBTData'
         self.operationNumber: int = 41
         self.blockConstantStringID: int = 0
         self.blockStatesConstantStringID: int = 0
-        self.blockNBT: nbtlib.tag.Compound = nbtlib.tag.Compound({})
+        self.blockNBT: nbtlib.tag.Compound = nbtlib.tag.Compound(
+            {})  # type: ignore
 
     def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>H', self.blockConstantStringID) + pack('>H',self.blockStatesConstantStringID) + pack('>H', self.blockStatesConstantStringID))
+        writer.write(pack('>H', self.blockConstantStringID) + pack('>H',
+                     self.blockStatesConstantStringID) + pack('>H', self.blockStatesConstantStringID))
         MarshalPythonNBTObjectToWriter(writer, self.blockNBT, '')
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
         self.blockStatesConstantStringID = unpack('>H', getByte(buffer, 2))[0]
         getByte(buffer, 2)  # do not delete this line because it is correct
         self.blockNBT, _ = UnMarshalBufferToPythonNBTObject(  # type: ignore
```

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/PlaceBlockWithRuntimeId.py` & `BDXConverter-1.0.14/BDXConverter/Operation/PlaceBlockWithRuntimeId.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py` & `BDXConverter-1.0.14/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/PlaceRuntimeBlock.py` & `BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py` & `BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py` & `BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py` & `BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py` & `BDXConverter-1.0.14/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/SetCommandBlockData.py` & `BDXConverter-1.0.14/BDXConverter/Operation/SetCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/UseRuntimeIDPool.py` & `BDXConverter-1.0.14/BDXConverter/Operation/UseRuntimeIDPool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/Operation/structOfChest.py` & `BDXConverter-1.0.14/BDXConverter/Operation/structOfChest.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/utils/marshalNBT.py` & `BDXConverter-1.0.14/BDXConverter/utils/marshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/utils/marshalNBT_OldVersion.py` & `BDXConverter-1.0.14/BDXConverter/utils/marshalNBT_OldVersion.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/utils/unmarshalNBT.py` & `BDXConverter-1.0.14/BDXConverter/utils/unmarshalNBT.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter/utils/unmarshalNBT_OldVersion.py` & `BDXConverter-1.0.14/BDXConverter/utils/unmarshalNBT_OldVersion.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/BDXConverter.egg-info/PKG-INFO` & `BDXConverter-1.0.14/BDXConverter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.0.13
+Version: 1.0.14
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,15 +49,15 @@
 - [其他](#其他)
 
 
 
 
 
 # `BDX Converter`
-`BDX Converter` 是一个轻量化的纯Python实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
+`BDX Converter` 是一个轻量化的纯 `Python` 实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 
 
 
 
 # 快速上手
 您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。
```

### Comparing `BDXConverter-1.0.13/BDXConverter.egg-info/SOURCES.txt` & `BDXConverter-1.0.14/BDXConverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/LICENSE` & `BDXConverter-1.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.13/PKG-INFO` & `BDXConverter-1.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.0.13
+Version: 1.0.14
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,15 +49,15 @@
 - [其他](#其他)
 
 
 
 
 
 # `BDX Converter`
-`BDX Converter` 是一个轻量化的纯Python实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
+`BDX Converter` 是一个轻量化的纯 `Python` 实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 
 
 
 
 # 快速上手
 您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。
```

### Comparing `BDXConverter-1.0.13/README.md` & `BDXConverter-1.0.14/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 - [其他](#其他)
 
 
 
 
 
 # `BDX Converter`
-`BDX Converter` 是一个轻量化的纯Python实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
+`BDX Converter` 是一个轻量化的纯 `Python` 实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
 
 
 
 
 
 # 快速上手
 您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。
```

