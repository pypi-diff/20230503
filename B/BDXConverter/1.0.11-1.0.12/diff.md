# Comparing `tmp/BDXConverter-1.0.11.tar.gz` & `tmp/BDXConverter-1.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDXConverter-1.0.11.tar", last modified: Tue May  2 21:02:07 2023, max compression
+gzip compressed data, was "BDXConverter-1.0.12.tar", last modified: Wed May  3 07:16:59 2023, max compression
```

## Comparing `BDXConverter-1.0.11.tar` & `BDXConverter-1.0.12.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.500085 BDXConverter-1.0.11/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.484086 BDXConverter-1.0.11/BDXConverter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.484086 BDXConverter-1.0.11/BDXConverter/Converter/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Converter/ConvertErrorDefine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Converter/Converter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.488086 BDXConverter-1.0.11/BDXConverter/General/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/General/GeneralClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/General/Pool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/General/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.496086 BDXConverter-1.0.11/BDXConverter/Operation/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt16XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt16YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt16ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt16ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt32XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt32YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt32ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt32ZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt8XValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt8YValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddInt8ZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AddZValue0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/AssignDebugData.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/CreateConstantString.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/NOP.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithBlockStates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithNBTData.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/SetCommandBlockData.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/SubtractXValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/SubtractYValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/SubtractZValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/Terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/UseRuntimeIDPool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/Operation/structOfChest.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.500085 BDXConverter-1.0.11/BDXConverter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/utils/getByte.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/utils/getString.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/utils/marshalNBT.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/BDXConverter/utils/unmarshalNBT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:02:07.484086 BDXConverter-1.0.11/BDXConverter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-02 21:02:07.000000 BDXConverter-1.0.11/BDXConverter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-02 21:02:07.000000 BDXConverter-1.0.11/BDXConverter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:02:07.000000 BDXConverter-1.0.11/BDXConverter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 21:02:07.000000 BDXConverter-1.0.11/BDXConverter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 21:02:07.000000 BDXConverter-1.0.11/BDXConverter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-02 21:02:07.500085 BDXConverter-1.0.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:02:07.500085 BDXConverter-1.0.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-02 21:01:50.000000 BDXConverter-1.0.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:16:59.199852 BDXConverter-1.0.12/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:16:59.171852 BDXConverter-1.0.12/BDXConverter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:16:59.175852 BDXConverter-1.0.12/BDXConverter/Converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Converter/ConvertErrorDefine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Converter/Converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:16:59.175852 BDXConverter-1.0.12/BDXConverter/General/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/General/GeneralClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/General/Pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/General/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:16:59.195852 BDXConverter-1.0.12/BDXConverter/Operation/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddInt16XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddInt16YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddInt16ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddInt16ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddInt32XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddInt32YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddInt32ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddInt32ZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddInt8XValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddInt8YValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddInt8ZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AddZValue0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/AssignDebugData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/CreateConstantString.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/NOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlockWithBlockStates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlockWithNBTData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlockWithRuntimeId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/PlaceRuntimeBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/SetCommandBlockData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/SubtractXValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/SubtractYValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/SubtractZValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/Terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/UseRuntimeIDPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/Operation/structOfChest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:16:59.199852 BDXConverter-1.0.12/BDXConverter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/utils/getByte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/utils/getString.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/utils/marshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/utils/marshalNBT_OldVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/utils/unmarshalNBT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/BDXConverter/utils/unmarshalNBT_OldVersion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 07:16:59.171852 BDXConverter-1.0.12/BDXConverter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-03 07:16:59.000000 BDXConverter-1.0.12/BDXConverter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-03 07:16:59.000000 BDXConverter-1.0.12/BDXConverter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 07:16:59.000000 BDXConverter-1.0.12/BDXConverter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-03 07:16:59.000000 BDXConverter-1.0.12/BDXConverter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 07:16:59.000000 BDXConverter-1.0.12/BDXConverter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-03 07:16:59.199852 BDXConverter-1.0.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 07:16:59.199852 BDXConverter-1.0.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-03 07:16:38.000000 BDXConverter-1.0.12/setup.py
```

### Comparing `BDXConverter-1.0.11/BDXConverter/Converter/ConvertErrorDefine.py` & `BDXConverter-1.0.12/BDXConverter/Converter/ConvertErrorDefine.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Converter/Converter.py` & `BDXConverter-1.0.12/BDXConverter/Converter/Converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 def ReadBDXFile(path: str) -> tuple[list[GeneralClass], str]:
     """
     Convert BDX file into list[GeneralClass] and return the author's name
     """
     with open(path, "r+b") as file:
         fileContext: bytes = file.read()
-    file.close()
     # get the context of this bdx file
     if fileContext[0:3] != b'BD@':
         raise notAcorrectBDXFileError(path)
     buffer = BytesIO(decompress(fileContext[3:]))
     if getByte(buffer, 3) != b'BDX':
         raise notAcorrectBDXFileError(path)
     # check header and create new buffer
@@ -76,15 +75,14 @@
             length=1, byteorder='big', signed=False))
         i.Marshal(writer)
     # marshal python object into the writer
     result = b'BD@' + compress(writer.getvalue())
     # compress writer into bytes and set outside header which named "BD@"
     with open(outputPath, 'w+b') as file:
         file.write(result)
-    file.close()
     # write bytes into a bdx file
 
 
 def VisualStructs(structs: list[GeneralClass], outputPath: str) -> None:
     """
     Convert list[GeneralClass] into json data and write it into outputPath:str
     """
@@ -98,15 +96,14 @@
         indent=4,
         separators=(', ', ': '),
         ensure_ascii=False
     )
     # get string
     with open(outputPath, 'w+', encoding='utf-8') as file:
         file.write(result)
-    file.close()
     # write json datas
 
 
 def ConvertJSONFileIntoStructs(path: str) -> list[GeneralClass]:
     """
     Read json datas from path:str and convert it into list[GeneralClass]
     """
```

### Comparing `BDXConverter-1.0.11/BDXConverter/General/GeneralClass.py` & `BDXConverter-1.0.12/BDXConverter/General/GeneralClass.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/General/Pool.py` & `BDXConverter-1.0.12/BDXConverter/General/Pool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/AddInt16XValue.py` & `BDXConverter-1.0.12/BDXConverter/Operation/AddInt16XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/AddInt16YValue.py` & `BDXConverter-1.0.12/BDXConverter/Operation/AddInt16YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/AddInt16ZValue.py` & `BDXConverter-1.0.12/BDXConverter/Operation/AddInt16ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/AddInt16ZValue0.py` & `BDXConverter-1.0.12/BDXConverter/Operation/AddInt16ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/AddInt32XValue.py` & `BDXConverter-1.0.12/BDXConverter/Operation/AddInt32XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/AddInt32YValue.py` & `BDXConverter-1.0.12/BDXConverter/Operation/AddInt32YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/AddInt32ZValue.py` & `BDXConverter-1.0.12/BDXConverter/Operation/AddInt32ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/AddInt32ZValue0.py` & `BDXConverter-1.0.12/BDXConverter/Operation/AddInt32ZValue0.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/AddInt8XValue.py` & `BDXConverter-1.0.12/BDXConverter/Operation/AddInt8XValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/AddInt8YValue.py` & `BDXConverter-1.0.12/BDXConverter/Operation/AddInt8YValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/AddInt8ZValue.py` & `BDXConverter-1.0.12/BDXConverter/Operation/AddInt8ZValue.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/AssignDebugData.py` & `BDXConverter-1.0.12/BDXConverter/Operation/AssignDebugData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/CreateConstantString.py` & `BDXConverter-1.0.12/BDXConverter/Operation/CreateConstantString.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlock.py` & `BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithBlockStates.py` & `BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlockWithBlockStates.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py` & `BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlockWithBlockStatesDeprecated.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithChestData.py` & `BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py` & `BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithNBTData.py` & `BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlockWithNBTData.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-import nbtlib
+import nbtlib, sys
 from io import BytesIO
 from struct import pack, unpack
 from ..General.GeneralClass import GeneralClass
 from ..utils.getByte import getByte
-from ..utils.marshalNBT import MarshalPythonNBTObjectToWriter
-from ..utils.unmarshalNBT import UnMarshalBufferToPythonNBTObject
+
+
+if sys.version_info.major>=3 and sys.version_info.minor>=10:
+    from ..utils.marshalNBT import MarshalPythonNBTObjectToWriter
+    from ..utils.unmarshalNBT import UnMarshalBufferToPythonNBTObject
+else:
+    from ..utils.marshalNBT_OldVersion import MarshalPythonNBTObjectToWriter
+    from ..utils.unmarshalNBT_OldVersion import UnMarshalBufferToPythonNBTObject
 
 
 class PlaceBlockWithNBTData(GeneralClass):
     def __init__(self) -> None:
         self.operationName: str = 'PlaceBlockWithNBTData'
         self.operationNumber: int = 41
         self.blockConstantStringID: int = 0
         self.blockStatesConstantStringID: int = 0
         self.blockNBT: nbtlib.tag.Compound = nbtlib.tag.Compound({})
 
     def Marshal(self, writer: BytesIO) -> None:
-        writer.write(pack('>H', self.blockConstantStringID) + pack('>H',
-                     self.blockStatesConstantStringID) + pack('>H', self.blockStatesConstantStringID))
+        writer.write(pack('>H', self.blockConstantStringID) + pack('>H',self.blockStatesConstantStringID) + pack('>H', self.blockStatesConstantStringID))
         MarshalPythonNBTObjectToWriter(writer, self.blockNBT, '')
 
     def UnMarshal(self, buffer: BytesIO) -> None:
         self.blockConstantStringID = unpack('>H', getByte(buffer, 2))[0]
         self.blockStatesConstantStringID = unpack('>H', getByte(buffer, 2))[0]
         getByte(buffer, 2)  # do not delete this line because it is correct
         self.blockNBT, _ = UnMarshalBufferToPythonNBTObject(  # type: ignore
```

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/PlaceBlockWithRuntimeId.py` & `BDXConverter-1.0.12/BDXConverter/Operation/PlaceBlockWithRuntimeId.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py` & `BDXConverter-1.0.12/BDXConverter/Operation/PlaceCommandBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlock.py` & `BDXConverter-1.0.12/BDXConverter/Operation/PlaceRuntimeBlock.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py` & `BDXConverter-1.0.12/BDXConverter/Operation/PlaceRuntimeBlockWithChestData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py` & `BDXConverter-1.0.12/BDXConverter/Operation/PlaceRuntimeBlockWithChestDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py` & `BDXConverter-1.0.12/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py` & `BDXConverter-1.0.12/BDXConverter/Operation/PlaceRuntimeBlockWithCommandBlockDataAndUint32RuntimeID.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/SetCommandBlockData.py` & `BDXConverter-1.0.12/BDXConverter/Operation/SetCommandBlockData.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/UseRuntimeIDPool.py` & `BDXConverter-1.0.12/BDXConverter/Operation/UseRuntimeIDPool.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter/Operation/structOfChest.py` & `BDXConverter-1.0.12/BDXConverter/Operation/structOfChest.py`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/BDXConverter.egg-info/PKG-INFO` & `BDXConverter-1.0.12/BDXConverter.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,99 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.0.11
+Version: 1.0.12
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">BDX Converter</h1>
 <h3 align="center">一个免费开源的 BDX 文件解析器</h3>
 <br/>
 <p align="center">
 <img src="https://forthebadge.com/images/badges/built-with-love.svg">
 <p>
 
 [GitHub: Happy2018new]: https://img.shields.io/badge/GitHub-Happy2018new-00A1E7?style=for-the-badge
+[GitHub: Inotart]: https://img.shields.io/badge/GitHub-Inotart-00A1E7?style=for-the-badge
 [python]: https://img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge
 [release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/LICENSE-MIT-228B22?style=for-the-badge
 
 [![][GitHub: Happy2018new]](https://github.com/Happy2018new)<br/>
+[![][GitHub: Inotart]](https://github.com/Inotart)<br/>
 [![][python]](https://www.python.org/)<br/>
 [![][license]](LICENSE)<br/>
 
 
 
 
 
+
+
+# 目录
+- [目录](#目录)
+- [`BDX Converter`](#bdx-converter)
+- [快速上手](#快速上手)
+- [🐍 Pypi Packages](#-pypi-packages)
+- [第三方依赖](#第三方依赖)
+- [特性](#特性)
+- [什么是 `BDX` 文件](#什么是-bdx-文件)
+- [关于 `PhoenixBuilder`](#关于-phoenixbuilder)
+- [待办列表](#待办列表)
+- [其他](#其他)
+
+
+
+
+
 # `BDX Converter`
-`BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
+`BDX Converter` 是一个轻量化的纯Python实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
+
+
+
+
 
 # 快速上手
 您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
-使用下述命令快速安装吧
-```shell
-pip install BDXConverter
-```
-> 我们建议您在 Python 3.10及其以上版本使用他,3.7及其以下版本Python不再维护更新
 
-# 项目依赖
+
+
+
+
+# 🐍 Pypi Packages
+我们已将此存储库以 `BDXConverter` 的名字上载到 `Pypi` ，您可以通过 `pip install BDXConverter` 快速安装。
+
+访问 [🐍 BDXConverter on Pypi](https://pypi.org/project/BDXConverter) 以了解有关此库的更多信息。
+
+我们配置了自动化 `CD/CI 工作流` ，因此如果您是本项目的 `协作者` ，您可以通过更改 `version` 文件或通过手动触发的方式启动工作流，它会自动编译本项目并将将其上载到 `Pypi` 中。
+
+_[注：我们建议您在 `Python 3.10` 及以上的版本使用本项目，`3.7` 及以下的版本已不再受到 `Python` 的维护和更新]_
+
+
+
+# 第三方依赖
 本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
 
 ```
 pip install brotli
 pip install nbtlib
 ```
 
-# 项目特性
+
+
+
+
+# 特性
 您可以从 [`BDXConverter/General/Pool.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
 
 实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
 
 ```python
 class GeneralClass:
     """
@@ -92,15 +130,39 @@
 ```
 
 因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
 而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
 
 目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。 
 
+
+
+
+
+# 什么是 `BDX` 文件
+`PhoenixBuilder` 是一个用于 `网易我的世界中国版 · 基岩版租赁服` 的商业化快速建造器，而 `BDX` 文件则是此建造器用于存储 `Minecraft` 建筑结构的 `私有文件格式` 。
+
+如果您希望解析 `BDX` 文件，敬请参阅 [`bdump-cn.md`](https://github.com/LNSSPsd/PhoenixBuilder/blob/main/doc/bdump/bdump-cn.md) 。
+
+# 关于 `PhoenixBuilder`
+- 您可以通过此链接访问 `PhoenixBuilder` 的存储库
+   - [`PhoenixBuilder`](https://github.com/LNSSPsd/PhoenixBuilder/)
+- 您可以通过下述链接访问 `PhoenixBuilder` 的相关网站
+   - [`用户中心`](https://uc.fastbuilder.pro/)
+   - [`官方网站`](https://fastbuilder.pro/)
+
+
+
+
+
 # 待办列表
 - [ ] `API` 文档
 - [ ] 支持与 `签名` 有关的功能
 - [ ] 可以将得到的 `Python Class` 进一步解析为建筑结构
 - [ ] 可以自由地转换 `BDX` 和其他建筑文件格式
 
+
+
+
+
 # 其他
 本项目依照 [`MIT LICENSE`](./LICENSE) 许可证进行许可和授权。
```

### Comparing `BDXConverter-1.0.11/BDXConverter.egg-info/SOURCES.txt` & `BDXConverter-1.0.12/BDXConverter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -52,8 +52,10 @@
 BDXConverter/Operation/UseRuntimeIDPool.py
 BDXConverter/Operation/__init__.py
 BDXConverter/Operation/structOfChest.py
 BDXConverter/utils/__init__.py
 BDXConverter/utils/getByte.py
 BDXConverter/utils/getString.py
 BDXConverter/utils/marshalNBT.py
-BDXConverter/utils/unmarshalNBT.py
+BDXConverter/utils/marshalNBT_OldVersion.py
+BDXConverter/utils/unmarshalNBT.py
+BDXConverter/utils/unmarshalNBT_OldVersion.py
```

### Comparing `BDXConverter-1.0.11/LICENSE` & `BDXConverter-1.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `BDXConverter-1.0.11/PKG-INFO` & `BDXConverter-1.0.12/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,99 @@
 Metadata-Version: 2.1
 Name: BDXConverter
-Version: 1.0.11
+Version: 1.0.12
 Summary: A code library to marshal, unmarshal, visual and reverse visualization of BDX files
 Home-page: https://github.com/TriM-Organization/BDXConverter
 Author: Minecraft Muti-Media Organization
 Author-email: TriM-Organization@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">BDX Converter</h1>
 <h3 align="center">一个免费开源的 BDX 文件解析器</h3>
 <br/>
 <p align="center">
 <img src="https://forthebadge.com/images/badges/built-with-love.svg">
 <p>
 
 [GitHub: Happy2018new]: https://img.shields.io/badge/GitHub-Happy2018new-00A1E7?style=for-the-badge
+[GitHub: Inotart]: https://img.shields.io/badge/GitHub-Inotart-00A1E7?style=for-the-badge
 [python]: https://img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge
 [release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/LICENSE-MIT-228B22?style=for-the-badge
 
 [![][GitHub: Happy2018new]](https://github.com/Happy2018new)<br/>
+[![][GitHub: Inotart]](https://github.com/Inotart)<br/>
 [![][python]](https://www.python.org/)<br/>
 [![][license]](LICENSE)<br/>
 
 
 
 
 
+
+
+# 目录
+- [目录](#目录)
+- [`BDX Converter`](#bdx-converter)
+- [快速上手](#快速上手)
+- [🐍 Pypi Packages](#-pypi-packages)
+- [第三方依赖](#第三方依赖)
+- [特性](#特性)
+- [什么是 `BDX` 文件](#什么是-bdx-文件)
+- [关于 `PhoenixBuilder`](#关于-phoenixbuilder)
+- [待办列表](#待办列表)
+- [其他](#其他)
+
+
+
+
+
 # `BDX Converter`
-`BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
+`BDX Converter` 是一个轻量化的纯Python实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
+
+
+
+
 
 # 快速上手
 您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
-使用下述命令快速安装吧
-```shell
-pip install BDXConverter
-```
-> 我们建议您在 Python 3.10及其以上版本使用他,3.7及其以下版本Python不再维护更新
 
-# 项目依赖
+
+
+
+
+# 🐍 Pypi Packages
+我们已将此存储库以 `BDXConverter` 的名字上载到 `Pypi` ，您可以通过 `pip install BDXConverter` 快速安装。
+
+访问 [🐍 BDXConverter on Pypi](https://pypi.org/project/BDXConverter) 以了解有关此库的更多信息。
+
+我们配置了自动化 `CD/CI 工作流` ，因此如果您是本项目的 `协作者` ，您可以通过更改 `version` 文件或通过手动触发的方式启动工作流，它会自动编译本项目并将将其上载到 `Pypi` 中。
+
+_[注：我们建议您在 `Python 3.10` 及以上的版本使用本项目，`3.7` 及以下的版本已不再受到 `Python` 的维护和更新]_
+
+
+
+# 第三方依赖
 本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
 
 ```
 pip install brotli
 pip install nbtlib
 ```
 
-# 项目特性
+
+
+
+
+# 特性
 您可以从 [`BDXConverter/General/Pool.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
 
 实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
 
 ```python
 class GeneralClass:
     """
@@ -92,15 +130,39 @@
 ```
 
 因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
 而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
 
 目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。 
 
+
+
+
+
+# 什么是 `BDX` 文件
+`PhoenixBuilder` 是一个用于 `网易我的世界中国版 · 基岩版租赁服` 的商业化快速建造器，而 `BDX` 文件则是此建造器用于存储 `Minecraft` 建筑结构的 `私有文件格式` 。
+
+如果您希望解析 `BDX` 文件，敬请参阅 [`bdump-cn.md`](https://github.com/LNSSPsd/PhoenixBuilder/blob/main/doc/bdump/bdump-cn.md) 。
+
+# 关于 `PhoenixBuilder`
+- 您可以通过此链接访问 `PhoenixBuilder` 的存储库
+   - [`PhoenixBuilder`](https://github.com/LNSSPsd/PhoenixBuilder/)
+- 您可以通过下述链接访问 `PhoenixBuilder` 的相关网站
+   - [`用户中心`](https://uc.fastbuilder.pro/)
+   - [`官方网站`](https://fastbuilder.pro/)
+
+
+
+
+
 # 待办列表
 - [ ] `API` 文档
 - [ ] 支持与 `签名` 有关的功能
 - [ ] 可以将得到的 `Python Class` 进一步解析为建筑结构
 - [ ] 可以自由地转换 `BDX` 和其他建筑文件格式
 
+
+
+
+
 # 其他
 本项目依照 [`MIT LICENSE`](./LICENSE) 许可证进行许可和授权。
```

### Comparing `BDXConverter-1.0.11/README.md` & `BDXConverter-1.0.12/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,46 +2,84 @@
 <h3 align="center">一个免费开源的 BDX 文件解析器</h3>
 <br/>
 <p align="center">
 <img src="https://forthebadge.com/images/badges/built-with-love.svg">
 <p>
 
 [GitHub: Happy2018new]: https://img.shields.io/badge/GitHub-Happy2018new-00A1E7?style=for-the-badge
+[GitHub: Inotart]: https://img.shields.io/badge/GitHub-Inotart-00A1E7?style=for-the-badge
 [python]: https://img.shields.io/badge/python-3.8-AB70FF?style=for-the-badge
 [release]: https://img.shields.io/github/v/release/EillesWan/Musicreater?style=for-the-badge
 [license]: https://img.shields.io/badge/LICENSE-MIT-228B22?style=for-the-badge
 
 [![][GitHub: Happy2018new]](https://github.com/Happy2018new)<br/>
+[![][GitHub: Inotart]](https://github.com/Inotart)<br/>
 [![][python]](https://www.python.org/)<br/>
 [![][license]](LICENSE)<br/>
 
 
 
 
 
+
+
+# 目录
+- [目录](#目录)
+- [`BDX Converter`](#bdx-converter)
+- [快速上手](#快速上手)
+- [🐍 Pypi Packages](#-pypi-packages)
+- [第三方依赖](#第三方依赖)
+- [特性](#特性)
+- [什么是 `BDX` 文件](#什么是-bdx-文件)
+- [关于 `PhoenixBuilder`](#关于-phoenixbuilder)
+- [待办列表](#待办列表)
+- [其他](#其他)
+
+
+
+
+
 # `BDX Converter`
-`BDX Converter` 是一个轻量化的实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
+`BDX Converter` 是一个轻量化的纯Python实现，它提供了基本的 `BDX` 解析、反解析、`JSON` 可视化和反可视化功能。 
+
+
+
+
 
 # 快速上手
 您可以利用 [`BDXConverter/Converter/Converter.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/Converter/Converter.py) 中已提供的 `4` 个函数来完成 `BDX` 文件和 `JSON` 文件的相关操作。 
-使用下述命令快速安装吧
-```shell
-pip install BDXConverter
-```
-> 我们建议您在 Python 3.10及其以上版本使用他,3.7及其以下版本Python不再维护更新
 
-# 项目依赖
+
+
+
+
+# 🐍 Pypi Packages
+我们已将此存储库以 `BDXConverter` 的名字上载到 `Pypi` ，您可以通过 `pip install BDXConverter` 快速安装。
+
+访问 [🐍 BDXConverter on Pypi](https://pypi.org/project/BDXConverter) 以了解有关此库的更多信息。
+
+我们配置了自动化 `CD/CI 工作流` ，因此如果您是本项目的 `协作者` ，您可以通过更改 `version` 文件或通过手动触发的方式启动工作流，它会自动编译本项目并将将其上载到 `Pypi` 中。
+
+_[注：我们建议您在 `Python 3.10` 及以上的版本使用本项目，`3.7` 及以下的版本已不再受到 `Python` 的维护和更新]_
+
+
+
+# 第三方依赖
 本项目使用了 `brotli` 和 `nbtlib` 总计 `2` 个第三方库，您可以通过在 `终端` 逐一地执行以下命令以安装它们。
 
 ```
 pip install brotli
 pip install nbtlib
 ```
 
-# 项目特性
+
+
+
+
+# 特性
 您可以从 [`BDXConverter/General/Pool.py`](https://github.com/TriM-Organization/BDXConverter/blob/main/BDXConverter/General/Pool.py) 查看本项目已支持的全部 `BDX` 操作符。
 
 实际上，我们将每一个操作符都转换为了 `Python` 下已被实例化的类，并且每个类都有以下属性。 
 
 ```python
 class GeneralClass:
     """
@@ -78,15 +116,39 @@
 ```
 
 因此，通过 `Marshal` 和 `UnMarshal` 函数，`BDX Converter` 可以自由的将 `二进制数据` 转换为 `Python Class` ，亦或转换回去。 <br/>
 而 `Loads` 和 `Dumps` 分别支持了把只带有基本数据类型的字典转换为 `Python Class` 亦或转换回去的功能。 
 
 目前 `BDX Converter` 支持了所有的操作符(不含签名功能)，包括但不限于 `Operation 5, Operation 13, Operation 40` 和 `Operation 41` 。 
 
+
+
+
+
+# 什么是 `BDX` 文件
+`PhoenixBuilder` 是一个用于 `网易我的世界中国版 · 基岩版租赁服` 的商业化快速建造器，而 `BDX` 文件则是此建造器用于存储 `Minecraft` 建筑结构的 `私有文件格式` 。
+
+如果您希望解析 `BDX` 文件，敬请参阅 [`bdump-cn.md`](https://github.com/LNSSPsd/PhoenixBuilder/blob/main/doc/bdump/bdump-cn.md) 。
+
+# 关于 `PhoenixBuilder`
+- 您可以通过此链接访问 `PhoenixBuilder` 的存储库
+   - [`PhoenixBuilder`](https://github.com/LNSSPsd/PhoenixBuilder/)
+- 您可以通过下述链接访问 `PhoenixBuilder` 的相关网站
+   - [`用户中心`](https://uc.fastbuilder.pro/)
+   - [`官方网站`](https://fastbuilder.pro/)
+
+
+
+
+
 # 待办列表
 - [ ] `API` 文档
 - [ ] 支持与 `签名` 有关的功能
 - [ ] 可以将得到的 `Python Class` 进一步解析为建筑结构
 - [ ] 可以自由地转换 `BDX` 和其他建筑文件格式
 
+
+
+
+
 # 其他
 本项目依照 [`MIT LICENSE`](./LICENSE) 许可证进行许可和授权。
```

### Comparing `BDXConverter-1.0.11/setup.py` & `BDXConverter-1.0.12/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import setuptools
 
 with open("requirements.txt", "r+", encoding="utf-8") as file:
     dependences = file.read().strip().split("\n")
+
 with open("README.md", "r+", encoding='utf-8') as file:
     long_description = file.read()
+
 with open("version", "r+", encoding='utf-8') as file:
     version = file.read()
+
 setuptools.setup(
     name="BDXConverter",
     version=version,
     author="Minecraft Muti-Media Organization",
     author_email="TriM-Organization@hotmail.com",
     description="A code library to marshal, unmarshal, visual and reverse visualization of BDX files",
     long_description=long_description,
@@ -18,9 +21,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=dependences,
-    python_requires='>=3.8',
+    python_requires='>=3.9',
 )
```

