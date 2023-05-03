# Comparing `tmp/fabrique_nodes_core-0.9.7-py3-none-any.whl.zip` & `tmp/fabrique_nodes_core-0.9.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 21904 bytes, number of entries: 23
+Zip file size: 21915 bytes, number of entries: 23
 -rw-rw-r--  2.0 unx      359 b- defN 23-Mar-09 14:27 fabrique_nodes_core/__init__.py
--rw-rw-r--  2.0 unx     2845 b- defN 23-Jan-31 10:51 fabrique_nodes_core/configs_model.py
+-rw-rw-r--  2.0 unx     2867 b- defN 23-Mar-17 13:49 fabrique_nodes_core/configs_model.py
 -rw-rw-r--  2.0 unx     1285 b- defN 23-Jan-30 13:40 fabrique_nodes_core/convertors.py
 -rw-rw-r--  2.0 unx     2281 b- defN 23-Mar-09 13:12 fabrique_nodes_core/core.py
 -rw-rw-r--  2.0 unx     3035 b- defN 23-Jan-12 16:48 fabrique_nodes_core/jspath_parser.py
 -rw-rw-r--  2.0 unx     5396 b- defN 23-Mar-14 20:55 fabrique_nodes_core/model_generators.py
 -rw-rw-r--  2.0 unx      322 b- defN 23-Jan-10 14:04 fabrique_nodes_core/port_types.py
 -rw-rw-r--  2.0 unx     3942 b- defN 23-Mar-13 12:38 fabrique_nodes_core/ui_params.py
 -rw-rw-r--  2.0 unx     4834 b- defN 23-Jan-16 22:55 fabrique_nodes_core/validators.py
@@ -14,12 +14,12 @@
 -rw-rw-r--  2.0 unx      874 b- defN 22-Nov-15 17:09 tests/import_spoofer.py
 -rw-rw-r--  2.0 unx    12119 b- defN 23-Jan-17 14:39 tests/nodes_for_tests.py
 -rw-rw-r--  2.0 unx     1137 b- defN 23-Jan-30 12:06 tests/test_0_positive_core.py
 -rw-rw-r--  2.0 unx     2016 b- defN 23-Jan-16 23:22 tests/test_1_core_validators.py
 -rw-rw-r--  2.0 unx     7130 b- defN 23-Mar-14 21:05 tests/test_2_positive_convertors.py
 -rw-rw-r--  2.0 unx     2721 b- defN 23-Mar-09 13:36 tests/test_3_positive_config_model copy.py
 -rw-rw-r--  2.0 unx     1186 b- defN 23-Mar-09 14:11 tests/test_4_stateful.py
--rw-rw-r--  2.0 unx     3611 b- defN 23-Mar-14 21:06 fabrique_nodes_core-0.9.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-14 21:06 fabrique_nodes_core-0.9.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       26 b- defN 23-Mar-14 21:06 fabrique_nodes_core-0.9.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2023 b- defN 23-Mar-14 21:06 fabrique_nodes_core-0.9.7.dist-info/RECORD
-23 files, 61152 bytes uncompressed, 18578 bytes compressed:  69.6%
+-rw-rw-r--  2.0 unx     3611 b- defN 23-Mar-17 13:50 fabrique_nodes_core-0.9.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Mar-17 13:50 fabrique_nodes_core-0.9.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       26 b- defN 23-Mar-17 13:50 fabrique_nodes_core-0.9.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2023 b- defN 23-Mar-17 13:50 fabrique_nodes_core-0.9.8.dist-info/RECORD
+23 files, 61174 bytes uncompressed, 18589 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -51,20 +51,20 @@
 
 Filename: tests/test_3_positive_config_model copy.py
 Comment: 
 
 Filename: tests/test_4_stateful.py
 Comment: 
 
-Filename: fabrique_nodes_core-0.9.7.dist-info/METADATA
+Filename: fabrique_nodes_core-0.9.8.dist-info/METADATA
 Comment: 
 
-Filename: fabrique_nodes_core-0.9.7.dist-info/WHEEL
+Filename: fabrique_nodes_core-0.9.8.dist-info/WHEEL
 Comment: 
 
-Filename: fabrique_nodes_core-0.9.7.dist-info/top_level.txt
+Filename: fabrique_nodes_core-0.9.8.dist-info/top_level.txt
 Comment: 
 
-Filename: fabrique_nodes_core-0.9.7.dist-info/RECORD
+Filename: fabrique_nodes_core-0.9.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fabrique_nodes_core/configs_model.py

```diff
@@ -49,19 +49,19 @@
     g_ports_in: Optional[List[List[Port]]] = [[]]
     g_ports_out: Optional[List[List[Port]]] = [[]]
     description: Optional[str] = ''
     schema_: Optional[str] = ''
     type_: Optional[str]
     group_type_: Optional[str]
     ui_config: Optional[dict]
-    category: Optional[Literal['StructOps', 'IO', 'Functional', 'Stateful', 'Misc', 'Conditional']]
+    category: Optional[Literal['StructOps', 'IO', 'Functional', 'Stateful', 'Misc', 'Conditional', 'Comment']]
 
 
 class PipelineNodeData(NodeData):
-    category: Optional[Literal['Actor', 'Bus']]
+    category: Optional[Literal['Actor', 'Bus', 'Comment']]
 
 
 class Node(BaseModel):
     id: str
     data: Optional[NodeData]
```

## Comparing `fabrique_nodes_core-0.9.7.dist-info/METADATA` & `fabrique_nodes_core-0.9.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrique-nodes-core
-Version: 0.9.7
+Version: 0.9.8
 Summary: Fabrique nodes SDK
 Home-page: http://www.fabrique.ai
 Author: Sergey Kuzmin
 Author-email: sergey.kuzmin@fabrique.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `fabrique_nodes_core-0.9.7.dist-info/RECORD` & `fabrique_nodes_core-0.9.8.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 fabrique_nodes_core/__init__.py,sha256=AZTRReMV7Xx8mMlysGPVqkhL4HF-55M25uAQXm_1Hp4,359
-fabrique_nodes_core/configs_model.py,sha256=LoKe4RkZEoEw6oQylK74JPFEwiXvL4Fcmc7dLsGR2ew,2845
+fabrique_nodes_core/configs_model.py,sha256=6ZjEfs9LhI-jJ1AXYa3o1ftJaZyH2fbEuFlTpxyVmjg,2867
 fabrique_nodes_core/convertors.py,sha256=4hRO-cp8AgiaE4VAluLOliVSwlmCdQn7sbgOGqx3Trk,1285
 fabrique_nodes_core/core.py,sha256=iwugvtoR4GmRe5jEUBL2BuPANHA39d_s0L1kMBb0qQs,2281
 fabrique_nodes_core/jspath_parser.py,sha256=Gu3JI12o3OMYlxjz6NitO74pXMunYf7ljTl14iAK4mk,3035
 fabrique_nodes_core/model_generators.py,sha256=svTih8g4k3H8gqYeswV4OLjOgO6AeSABJmuMWXyeM68,5396
 fabrique_nodes_core/port_types.py,sha256=5XKAgmPz0RxkhJbarpoXvIUK6FgJlWQkxWlcLtvCA_s,322
 fabrique_nodes_core/ui_params.py,sha256=2X5QgRfDRN4YK2ldRSYfNOjLkl8S-9hh3cQ-222IpK4,3942
 fabrique_nodes_core/validators.py,sha256=qO89Dhae_Bmkb_dy_ewts0KZAGRemtPrO5BP-mRsCjw,4834
@@ -13,11 +13,11 @@
 tests/import_spoofer.py,sha256=1eX6NAM-fs9ADO617KiLVX_D3Z3cnl9CuYKOsZPOW40,874
 tests/nodes_for_tests.py,sha256=iey2SNz3kbSk6t1_uj4sxgA1Pfa7hEYjZwS6_b-vFg8,12119
 tests/test_0_positive_core.py,sha256=MVXEALgcrjnxb12Bob1p6ho2Eg8tlwe-AkW4h_ZYQYc,1137
 tests/test_1_core_validators.py,sha256=2eUj94jh4dPe5KP9FF7aklodlBY9WoGvFmecAxolXyE,2016
 tests/test_2_positive_convertors.py,sha256=9ehJRScNBf_qwXaWMtFQW4SyXCNq6FHXEa_yqepPZTM,7130
 tests/test_3_positive_config_model copy.py,sha256=LtZdQTPILopb3fVD0dy2hYNkPN39UDfJFEgzorKx0ZA,2721
 tests/test_4_stateful.py,sha256=g4KiHOAOjZdZfhpLusvpAfDhYQ5aLYXWme3HA0ZWmMM,1186
-fabrique_nodes_core-0.9.7.dist-info/METADATA,sha256=Qv3E1eexy0qZkzMJkT2HecEedMXHMsNTT5RoL31H4cs,3611
-fabrique_nodes_core-0.9.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-fabrique_nodes_core-0.9.7.dist-info/top_level.txt,sha256=JjbMKYNcnQfJlxkUFTCI2M3nPS6aMLiVWHMV9-o91eM,26
-fabrique_nodes_core-0.9.7.dist-info/RECORD,,
+fabrique_nodes_core-0.9.8.dist-info/METADATA,sha256=NTlcGDRCAVyTR0Cz5BN-mSk5tS_tiDJa5p7sbbsmlE0,3611
+fabrique_nodes_core-0.9.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+fabrique_nodes_core-0.9.8.dist-info/top_level.txt,sha256=JjbMKYNcnQfJlxkUFTCI2M3nPS6aMLiVWHMV9-o91eM,26
+fabrique_nodes_core-0.9.8.dist-info/RECORD,,
```

