# Comparing `tmp/looqbox_components-1.2.5-py3-none-any.whl.zip` & `tmp/looqbox_components-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,16 @@
-Zip file size: 7430 bytes, number of entries: 13
--rw-r--r--  2.0 unx      167 b- defN 23-Feb-10 15:17 looqbox_components/__init__.py
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-13 21:05 looqbox_components/templates/__init__.py
--rw-r--r--  2.0 unx     6640 b- defN 23-Feb-01 19:20 looqbox_components/templates/container.py
--rw-r--r--  2.0 unx     5683 b- defN 23-Feb-15 11:47 looqbox_components/templates/tag.py
--rw-r--r--  2.0 unx     1711 b- defN 23-Feb-10 14:45 looqbox_components/templates/toplist.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-01 19:20 looqbox_components/templates/tests/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-01 19:20 looqbox_components/tests/__init__.py
--rw-r--r--  2.0 unx      233 b- defN 23-Feb-01 19:20 looqbox_components/tests/test_looqbox_components.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-13 21:05 looqbox_components/utils/__init__.py
--rw-r--r--  2.0 unx      989 b- defN 23-Feb-15 11:48 looqbox_components-1.2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-15 11:48 looqbox_components-1.2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Feb-15 11:48 looqbox_components-1.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1194 b- defN 23-Feb-15 11:48 looqbox_components-1.2.5.dist-info/RECORD
-13 files, 16729 bytes uncompressed, 5368 bytes compressed:  67.9%
+Zip file size: 8682 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      167 b- defN 23-Apr-28 18:07 looqbox_components/__init__.py
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-28 18:07 looqbox_components/templates/__init__.py
+-rw-r--r--  2.0 unx     6858 b- defN 23-Apr-28 18:07 looqbox_components/templates/container.py
+-rw-r--r--  2.0 unx     2350 b- defN 23-Apr-28 18:07 looqbox_components/templates/simple_card.py
+-rw-r--r--  2.0 unx     5683 b- defN 23-Apr-28 18:07 looqbox_components/templates/tag.py
+-rw-r--r--  2.0 unx     2840 b- defN 23-Apr-28 18:07 looqbox_components/templates/toplist.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 18:07 looqbox_components/templates/tests/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 18:07 looqbox_components/tests/__init__.py
+-rw-r--r--  2.0 unx      233 b- defN 23-Apr-28 18:07 looqbox_components/tests/test_looqbox_components.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 18:07 looqbox_components/utils/__init__.py
+-rw-r--r--  2.0 unx      989 b- defN 23-May-03 12:20 looqbox_components-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 12:20 looqbox_components-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-May-03 12:20 looqbox_components-1.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1294 b- defN 23-May-03 12:20 looqbox_components-1.3.0.dist-info/RECORD
+14 files, 20526 bytes uncompressed, 6458 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: looqbox_components/templates/__init__.py
 Comment: 
 
 Filename: looqbox_components/templates/container.py
 Comment: 
 
+Filename: looqbox_components/templates/simple_card.py
+Comment: 
+
 Filename: looqbox_components/templates/tag.py
 Comment: 
 
 Filename: looqbox_components/templates/toplist.py
 Comment: 
 
 Filename: looqbox_components/templates/tests/__init__.py
@@ -21,20 +24,20 @@
 
 Filename: looqbox_components/tests/test_looqbox_components.py
 Comment: 
 
 Filename: looqbox_components/utils/__init__.py
 Comment: 
 
-Filename: looqbox_components-1.2.5.dist-info/METADATA
+Filename: looqbox_components-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: looqbox_components-1.2.5.dist-info/WHEEL
+Filename: looqbox_components-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: looqbox_components-1.2.5.dist-info/top_level.txt
+Filename: looqbox_components-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: looqbox_components-1.2.5.dist-info/RECORD
+Filename: looqbox_components-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## looqbox_components/templates/container.py

```diff
@@ -13,14 +13,15 @@
 
     def __init__(self, *content, **properties):
         """
         :param sample_info:
         :param kwargs: all component variables and optional pre-sets for the container
 
             height: Height of the container, defaults to 50px
+            use_border: If it should have the side line, defaults to True
             line: If it should have the side line, defaults to True
             line_thickness: Thickness of the side line, defaults to 5px
             tooltip: Tooltip text, displayed if not empty, defaults to empty string
             title: Title of the container
             subtitle: Subtitle of the container
             line_color: Side line color, defaults to "#40db62"
             tooltip_spacing: Tooltip margin against container
@@ -30,14 +31,15 @@
         super().__init__()
 
         self.content = content
         self.properties = properties
 
         self.obj_container_args = [
             "height",
+            "use_border",
             "line",
             "line_thickness",
             "tooltip",
             "title",
             "subtitle",
             "line_color",
             "title_spacing",
@@ -103,20 +105,25 @@
             (_header if not _is_single_container and _header else []) + [children_container],
             css_options=self._children_style,
         )
 
         _line = self._get_line()
         _tooltip = self._get_container_tooltip()
 
-        return ObjRow(
+        container_row = ObjRow(
             _line,
             _current,
             _tooltip,
             css_options=self._container_style,
-        ).add_border.set_cross_alignment_center
+        ).set_cross_alignment_center
+
+        if self.properties.get("use_border", True):
+            container_row.add_border
+
+        return container_row
 
     def _insert_header_on_switch(self, _header):
         for idx in range(len(tmp_container := self.content[0].children)):
             tmp_container[idx] = ObjColumn(_header, tmp_container[idx], tab_label=tmp_container[idx].tab_label)
 
     def _get_header(self):
         _header = [
```

## looqbox_components/templates/toplist.py

```diff
@@ -12,40 +12,55 @@
     :param data: A pandas DataFrame or looqbox Objtable with the data to be displayed in the TopList.
 
     :return: A JSON string.
 
     """
 
     @overload
-    def __init__(self, data: DataFrame):
+    def __init__(self, data: DataFrame, thickness: int = 1, line_color: str = "#D5DFE9", alignment: str = "center"):
         """
         Receives a pandas dataframe and render it as a list.
         :param data: pd.DataFrame or lq.ObjTable
+        :param thickness: int - Thickness of the line between rows. Default is 1.
+        :param line_color: str - Color of the line between rows. Default is #D5DFE9.
+        :param alignment: str - Text-alignment of the list. Default is center. Can be left, right or center.
         """
         super().__init__()
         self.list_content = ObjTable(data)
+        self.alignment = alignment
+        self.thickness = thickness
+        self.line_color = line_color
 
     @overload
-    def __init__(self, data: ObjTable):
+    def __init__(self, data: ObjTable, thickness: int = 1, line_color: str = "#D5DFE9", alignment: str = "center"):
         """
         Receives a looqbox ObjTable and render it as a list.
         :param data: pd.DataFrame or lq.ObjTable
+        :param thickness: int - Thickness of the line between rows. Default is 1.
+        :param line_color: str - Color of the line between rows. Default is #D5DFE9.
+        :param alignment: str - Text-alignment of the list. Default is center. Can be left, right or center.
         """
         super().__init__()
         self.list_content = data
+        self.alignment = alignment
+        self.thickness = thickness
+        self.line_color = line_color
 
     def _set_list_style(self) -> None:
 
         for row in range(self.list_content.data.shape[0]):
             self.list_content.row_style[row] = {"background": "white",
-                                                "border-bottom": "1px solid #D5DFE9"}
+                                                "border-bottom": f"{self.thickness}px solid {self.line_color}"}
 
         self.list_content.show_head = False
         self.list_content.show_option_bar = False
         self.list_content.show_footer = False
+        self.list_content.col_style = dict(
+            zip(self.list_content.data.columns,
+                [{'text-alignment': self.alignment}] * len(self.list_content.data.columns)))
 
     def _data_frame_is_empty(self) -> bool:
         return self.list_content.data is None or self.list_content.data.empty
 
     def to_json_structure(self, visitor: BaseRender):
 
         if self._data_frame_is_empty():
```

## Comparing `looqbox_components-1.2.5.dist-info/METADATA` & `looqbox_components-1.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looqbox-components
-Version: 1.2.5
+Version: 1.3.0
 Summary: A looqbox package with most used visual components templates
 Home-page: https://github.com/looqbox/python-visual-components
 Author: Looqbox
 Author-email: admin@looqbox.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `looqbox_components-1.2.5.dist-info/RECORD` & `looqbox_components-1.3.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 looqbox_components/__init__.py,sha256=_ZlhoINy7zRHdLhYXYEZOokTG3S22R4VWo012qLiJww,167
 looqbox_components/templates/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-looqbox_components/templates/container.py,sha256=iaJdQKnyWB592MSKIscL0uR_HOwjjGDUtdKkdeggCHk,6640
+looqbox_components/templates/container.py,sha256=vsjreTp40yse1YmdrT3LCO_g2waadDY-dQ7m08HYLh4,6858
+looqbox_components/templates/simple_card.py,sha256=wfL-cG3hWQqDb4ETg_I9tl5PglDJE9hcBajKiqd8590,2350
 looqbox_components/templates/tag.py,sha256=EciZ3VRCIdloOUTC68hF7FHL-_9xtQ2TVi1K60oAKDw,5683
-looqbox_components/templates/toplist.py,sha256=0gpb-crDbDwXQ2wYxIqcAMXHfJzHblq27h8OVIQFpNM,1711
+looqbox_components/templates/toplist.py,sha256=mAlFkUBYXMMqSSIz5MogMascE1OfzVoT5sfGfFiuC5Y,2840
 looqbox_components/templates/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 looqbox_components/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 looqbox_components/tests/test_looqbox_components.py,sha256=8fVRfEvqcxlJDuNp6RlucKwH13JMCrXkeGgSmkdxonU,233
 looqbox_components/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-looqbox_components-1.2.5.dist-info/METADATA,sha256=OaBKZKHVH3Uk-2_Kc7SmaRTDHvCPjP9LXdZP8gp0J5I,989
-looqbox_components-1.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-looqbox_components-1.2.5.dist-info/top_level.txt,sha256=Zb_QlF8DlA-rP1wb-5-vbk_U_exlVnC4IXl1bBro5kQ,19
-looqbox_components-1.2.5.dist-info/RECORD,,
+looqbox_components-1.3.0.dist-info/METADATA,sha256=ZcZHoTXY___mSf0fT4p7XbHx--FvIheC-8aLPBvSR78,989
+looqbox_components-1.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+looqbox_components-1.3.0.dist-info/top_level.txt,sha256=Zb_QlF8DlA-rP1wb-5-vbk_U_exlVnC4IXl1bBro5kQ,19
+looqbox_components-1.3.0.dist-info/RECORD,,
```

