# Comparing `tmp/looqbox_components-1.3.1-py3-none-any.whl.zip` & `tmp/looqbox_components-1.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8682 bytes, number of entries: 14
--rw-r--r--  2.0 unx      167 b- defN 23-Apr-28 18:07 looqbox_components/__init__.py
+Zip file size: 8694 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      231 b- defN 23-May-03 16:35 looqbox_components/__init__.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Apr-28 18:07 looqbox_components/templates/__init__.py
 -rw-r--r--  2.0 unx     6858 b- defN 23-Apr-28 18:07 looqbox_components/templates/container.py
 -rw-r--r--  2.0 unx     2350 b- defN 23-Apr-28 18:07 looqbox_components/templates/simple_card.py
 -rw-r--r--  2.0 unx     5683 b- defN 23-Apr-28 18:07 looqbox_components/templates/tag.py
 -rw-r--r--  2.0 unx     2840 b- defN 23-Apr-28 18:07 looqbox_components/templates/toplist.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 18:07 looqbox_components/templates/tests/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 18:07 looqbox_components/tests/__init__.py
 -rw-r--r--  2.0 unx      233 b- defN 23-Apr-28 18:07 looqbox_components/tests/test_looqbox_components.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 18:07 looqbox_components/utils/__init__.py
--rw-r--r--  2.0 unx      989 b- defN 23-May-03 14:54 looqbox_components-1.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 14:54 looqbox_components-1.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-May-03 14:54 looqbox_components-1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1294 b- defN 23-May-03 14:54 looqbox_components-1.3.1.dist-info/RECORD
-14 files, 20526 bytes uncompressed, 6458 bytes compressed:  68.5%
+-rw-r--r--  2.0 unx      989 b- defN 23-May-03 16:36 looqbox_components-1.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 16:36 looqbox_components-1.3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-May-03 16:36 looqbox_components-1.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1294 b- defN 23-May-03 16:36 looqbox_components-1.3.2.dist-info/RECORD
+14 files, 20590 bytes uncompressed, 6470 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: looqbox_components/tests/test_looqbox_components.py
 Comment: 
 
 Filename: looqbox_components/utils/__init__.py
 Comment: 
 
-Filename: looqbox_components-1.3.1.dist-info/METADATA
+Filename: looqbox_components-1.3.2.dist-info/METADATA
 Comment: 
 
-Filename: looqbox_components-1.3.1.dist-info/WHEEL
+Filename: looqbox_components-1.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: looqbox_components-1.3.1.dist-info/top_level.txt
+Filename: looqbox_components-1.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: looqbox_components-1.3.1.dist-info/RECORD
+Filename: looqbox_components-1.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## looqbox_components/__init__.py

```diff
@@ -1,3 +1,4 @@
 from looqbox_components.templates.container import Container
 from looqbox_components.templates.tag import Tag
 from looqbox_components.templates.toplist import TopList
+from looqbox_components.templates.simple_card import SimpleCard
```

## Comparing `looqbox_components-1.3.1.dist-info/METADATA` & `looqbox_components-1.3.2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looqbox-components
-Version: 1.3.1
+Version: 1.3.2
 Summary: A looqbox package with most used visual components templates
 Home-page: https://github.com/looqbox/python-visual-components
 Author: Looqbox
 Author-email: admin@looqbox.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `looqbox_components-1.3.1.dist-info/RECORD` & `looqbox_components-1.3.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-looqbox_components/__init__.py,sha256=_ZlhoINy7zRHdLhYXYEZOokTG3S22R4VWo012qLiJww,167
+looqbox_components/__init__.py,sha256=t-xfKsHcJ7n8NfeWb6JLRJeBgdPD86Aqm_nQid_fZxw,231
 looqbox_components/templates/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 looqbox_components/templates/container.py,sha256=vsjreTp40yse1YmdrT3LCO_g2waadDY-dQ7m08HYLh4,6858
 looqbox_components/templates/simple_card.py,sha256=wfL-cG3hWQqDb4ETg_I9tl5PglDJE9hcBajKiqd8590,2350
 looqbox_components/templates/tag.py,sha256=EciZ3VRCIdloOUTC68hF7FHL-_9xtQ2TVi1K60oAKDw,5683
 looqbox_components/templates/toplist.py,sha256=mAlFkUBYXMMqSSIz5MogMascE1OfzVoT5sfGfFiuC5Y,2840
 looqbox_components/templates/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 looqbox_components/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 looqbox_components/tests/test_looqbox_components.py,sha256=8fVRfEvqcxlJDuNp6RlucKwH13JMCrXkeGgSmkdxonU,233
 looqbox_components/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-looqbox_components-1.3.1.dist-info/METADATA,sha256=THSbrVJZPfRgI3JiZFHiKswBCVwsDy9JYaPPPsKFQyo,989
-looqbox_components-1.3.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-looqbox_components-1.3.1.dist-info/top_level.txt,sha256=Zb_QlF8DlA-rP1wb-5-vbk_U_exlVnC4IXl1bBro5kQ,19
-looqbox_components-1.3.1.dist-info/RECORD,,
+looqbox_components-1.3.2.dist-info/METADATA,sha256=go2xZEdxyqwkaE9EfDqB2z_LBvmk-xxzix1LlpHtlkQ,989
+looqbox_components-1.3.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+looqbox_components-1.3.2.dist-info/top_level.txt,sha256=Zb_QlF8DlA-rP1wb-5-vbk_U_exlVnC4IXl1bBro5kQ,19
+looqbox_components-1.3.2.dist-info/RECORD,,
```

