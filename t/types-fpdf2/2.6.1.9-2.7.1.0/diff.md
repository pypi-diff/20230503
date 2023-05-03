# Comparing `tmp/types-fpdf2-2.6.1.9.tar.gz` & `tmp/types-fpdf2-2.7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-fpdf2-2.6.1.9.tar", last modified: Wed Feb 22 09:18:19 2023, max compression
+gzip compressed data, was "types-fpdf2-2.7.1.0.tar", last modified: Wed May  3 15:15:20 2023, max compression
```

## Comparing `types-fpdf2-2.6.1.9.tar` & `types-fpdf2-2.7.1.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:18:19.778704 types-fpdf2-2.6.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-02-22 09:18:19.000000 types-fpdf2-2.6.1.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-22 09:18:19.000000 types-fpdf2-2.6.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-02-22 09:18:19.778704 types-fpdf2-2.6.1.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:18:19.774704 types-fpdf2-2.6.1.9/fpdf-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-22 09:18:19.000000 types-fpdf2-2.6.1.9/fpdf-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/_fonttools_shims.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/actions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/annotations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/deprecation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/encryption.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/fonts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18182 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/fpdf.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/graphics_state.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/image_parsing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/line_break.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/linearization.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/outline.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/output.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/prefs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/recorder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/sign.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/structure_tree.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/svg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/syntax.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/template.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/transitions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-22 09:17:01.000000 types-fpdf2-2.6.1.9/fpdf-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 09:18:19.778704 types-fpdf2-2.6.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-02-22 09:18:19.000000 types-fpdf2-2.6.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:18:19.778704 types-fpdf2-2.6.1.9/types_fpdf2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-02-22 09:18:19.000000 types-fpdf2-2.6.1.9/types_fpdf2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-22 09:18:19.000000 types-fpdf2-2.6.1.9/types_fpdf2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 09:18:19.000000 types-fpdf2-2.6.1.9/types_fpdf2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-22 09:18:19.000000 types-fpdf2-2.6.1.9/types_fpdf2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 09:18:19.000000 types-fpdf2-2.6.1.9/types_fpdf2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:20.337569 types-fpdf2-2.7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-03 15:15:19.000000 types-fpdf2-2.7.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 15:15:19.000000 types-fpdf2-2.7.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-03 15:15:20.337569 types-fpdf2-2.7.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:20.337569 types-fpdf2-2.7.1.0/fpdf-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 15:15:19.000000 types-fpdf2-2.7.1.0/fpdf-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/_fonttools_shims.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/actions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/annotations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/deprecation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14700 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/encryption.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/fonts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20182 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/fpdf.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/graphics_state.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/image_parsing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/line_break.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/linearization.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/outline.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/output.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/prefs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/recorder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/sign.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/structure_tree.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/svg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/syntax.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/template.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/transitions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-03 15:15:02.000000 types-fpdf2-2.7.1.0/fpdf-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:15:20.337569 types-fpdf2-2.7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-03 15:15:19.000000 types-fpdf2-2.7.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:20.337569 types-fpdf2-2.7.1.0/types_fpdf2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-03 15:15:20.000000 types-fpdf2-2.7.1.0/types_fpdf2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-03 15:15:20.000000 types-fpdf2-2.7.1.0/types_fpdf2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:15:20.000000 types-fpdf2-2.7.1.0/types_fpdf2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 15:15:20.000000 types-fpdf2-2.7.1.0/types_fpdf2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 15:15:20.000000 types-fpdf2-2.7.1.0/types_fpdf2.egg-info/top_level.txt
```

### Comparing `types-fpdf2-2.6.1.9/CHANGELOG.md` & `types-fpdf2-2.7.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 2.7.1.0 (2023-05-03)
+
+[fpdf2] Update to 2.7.1 (#9978)
+
+## 2.6.1.10 (2023-03-27)
+
+Add defaults for third-party stubs E-H (#9954)
+
 ## 2.6.1.9 (2023-02-22)
 
 Update `Unused` parameters in `stubs/` (#9704)
 
 * Update _Unused TypeAlias
 
 * Update `object | None` params
```

### Comparing `types-fpdf2-2.6.1.9/PKG-INFO` & `types-fpdf2-2.7.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-fpdf2
-Version: 2.6.1.9
+Version: 2.7.1.0
 Summary: Typing stubs for fpdf2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/fpdf2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `fpdf2`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/fpdf2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `078c6a095892e12c94462889fa43c2c2dc8280ad`.
+This package was generated from typeshed commit `ec1130adcc12431ba85415a6533da68c3692b2cb`.
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/__init__.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from pathlib import Path
 
-from .enums import Align as Align, XPos as XPos, YPos as YPos
-from .fpdf import FPDF as FPDF, TitleStyle as TitleStyle
+from .enums import Align as Align, TextMode as TextMode, XPos as XPos, YPos as YPos
+from .fpdf import FPDF as FPDF, FPDFException as FPDFException, TitleStyle as TitleStyle
 from .html import HTML2FPDF as HTML2FPDF, HTMLMixin as HTMLMixin
 from .prefs import ViewerPreferences as ViewerPreferences
 from .template import FlexTemplate as FlexTemplate, Template as Template
 
 __license__: str
 __version__: str
 FPDF_VERSION: str
 FPDF_FONT_DIR: Path
 
 __all__ = [
     "__version__",
     "__license__",
     "FPDF",
+    "FPDFException",
     "Align",
     "XPos",
     "YPos",
     "Template",
     "FlexTemplate",
     "TitleStyle",
     "ViewerPreferences",
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/_fonttools_shims.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/_fonttools_shims.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/actions.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/actions.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from _typeshed import Incomplete
 from abc import ABC, abstractmethod
 
 from .syntax import PDFObject
 
 class Action(ABC):
     next: PDFObject | str | None
-    def __init__(self, next_action: PDFObject | str | None = ...) -> None: ...
+    def __init__(self, next_action: PDFObject | str | None = None) -> None: ...
     @abstractmethod
     def serialize(self) -> str: ...
 
 class URIAction(Action):
     uri: str
-    def __init__(self, uri: str, next_action: PDFObject | str | None = ...) -> None: ...
+    def __init__(self, uri: str, next_action: PDFObject | str | None = None) -> None: ...
     def serialize(self) -> str: ...
 
 class NamedAction(Action):
     action_name: str
-    def __init__(self, action_name: str, next_action: PDFObject | str | None = ...) -> None: ...
+    def __init__(self, action_name: str, next_action: PDFObject | str | None = None) -> None: ...
     def serialize(self) -> str: ...
 
 class GoToAction(Action):
     dest: Incomplete
-    def __init__(self, dest, next_action: PDFObject | str | None = ...) -> None: ...
+    def __init__(self, dest, next_action: PDFObject | str | None = None) -> None: ...
     def serialize(self) -> str: ...
 
 class GoToRemoteAction(Action):
     file: str
     dest: Incomplete
-    def __init__(self, file: str, dest, next_action: PDFObject | str | None = ...) -> None: ...
+    def __init__(self, file: str, dest, next_action: PDFObject | str | None = None) -> None: ...
     def serialize(self) -> str: ...
 
 class LaunchAction(Action):
     file: str
-    def __init__(self, file: str, next_action: PDFObject | str | None = ...) -> None: ...
+    def __init__(self, file: str, next_action: PDFObject | str | None = None) -> None: ...
     def serialize(self) -> str: ...
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/annotations.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/annotations.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -31,46 +31,46 @@
         self,
         subtype: str,
         x: int,
         y: int,
         width: int,
         height: int,
         flags: tuple[AnnotationFlag, ...] = ...,
-        contents: str | None = ...,
-        dest: Destination | None = ...,
-        action: Action | None = ...,
-        color: tuple[int, int, int] | None = ...,
-        modification_time: datetime | None = ...,
-        title: str | None = ...,
-        quad_points: tuple[float, ...] | None = ...,  # multiple of 8 floats
-        border_width: int = ...,
-        name: AnnotationName | FileAttachmentAnnotationName | None = ...,
-        ink_list: tuple[int, ...] = ...,
-        file_spec: str | None = ...,
-        field_type: str | None = ...,
-        value: Incomplete | None = ...,
+        contents: str | None = None,
+        dest: Destination | None = None,
+        action: Action | None = None,
+        color: tuple[int, int, int] | None = None,
+        modification_time: datetime | None = None,
+        title: str | None = None,
+        quad_points: tuple[float, ...] | None = None,  # multiple of 8 floats
+        border_width: int = 0,
+        name: AnnotationName | FileAttachmentAnnotationName | None = None,
+        ink_list: tuple[int, ...] = (),
+        file_spec: str | None = None,
+        field_type: str | None = None,
+        value: Incomplete | None = None,
     ) -> None: ...
 
 class PDFAnnotation(AnnotationMixin, PDFObject): ...
 
 class AnnotationDict(AnnotationMixin):
     def serialize(self) -> str: ...
 
 class PDFEmbeddedFile(PDFContentStream):
     type: Name
     params: str
     def __init__(
         self,
         basename: str,
         contents: bytes,
-        desc: str = ...,
-        creation_date: datetime | None = ...,
-        modification_date: datetime | None = ...,
-        compress: bool = ...,
-        checksum: bool = ...,
+        desc: str = "",
+        creation_date: datetime | None = None,
+        modification_date: datetime | None = None,
+        compress: bool = False,
+        checksum: bool = False,
     ) -> None: ...
     def globally_enclosed(self) -> bool: ...
     def set_globally_enclosed(self, value: bool) -> None: ...
     def basename(self) -> str: ...
     def file_spec(self) -> FileSpec: ...
 
 class FileSpec(NamedTuple):
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/drawing.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/drawing.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -34,47 +34,47 @@
     r: Number
     g: Number
     b: Number
     a: Number | None
 
 class DeviceRGB(_DeviceRGBBase):
     OPERATOR: ClassVar[str]
-    def __new__(cls, r: Number, g: Number, b: Number, a: Number | None = ...) -> Self: ...
+    def __new__(cls, r: Number, g: Number, b: Number, a: Number | None = None) -> Self: ...
     @property
     def colors(self) -> tuple[Number, Number, Number]: ...
     def serialize(self) -> str: ...
 
 class _DeviceGrayBase(NamedTuple):
     g: Number
     a: Number | None
 
 class DeviceGray(_DeviceGrayBase):
     OPERATOR: ClassVar[str]
-    def __new__(cls, g: Number, a: Number | None = ...) -> Self: ...
+    def __new__(cls, g: Number, a: Number | None = None) -> Self: ...
     @property
     def colors(self) -> tuple[Number]: ...
     def serialize(self) -> str: ...
 
 class _DeviceCMYKBase(NamedTuple):
     c: Number
     m: Number
     y: Number
     k: Number
     a: Number | None
 
 class DeviceCMYK(_DeviceCMYKBase):
     OPERATOR: ClassVar[str]
-    def __new__(cls, c: Number, m: Number, y: Number, k: Number, a: Number | None = ...) -> Self: ...
+    def __new__(cls, c: Number, m: Number, y: Number, k: Number, a: Number | None = None) -> Self: ...
     @property
     def colors(self) -> tuple[Number, Number, Number, Number]: ...
     def serialize(self) -> str: ...
 
-def rgb8(r, g, b, a: Incomplete | None = ...) -> DeviceRGB: ...
-def gray8(g, a: Incomplete | None = ...) -> DeviceGray: ...
-def cmyk8(c, m, y, k, a: Incomplete | None = ...) -> DeviceCMYK: ...
+def rgb8(r, g, b, a: Incomplete | None = None) -> DeviceRGB: ...
+def gray8(g, a: Incomplete | None = None) -> DeviceGray: ...
+def cmyk8(c, m, y, k, a: Incomplete | None = None) -> DeviceCMYK: ...
 def color_from_hex_string(hexstr) -> DeviceRGB: ...
 def color_from_rgb_string(rgbstr) -> DeviceRGB: ...
 
 class Point(NamedTuple):
     x: Number
     y: Number
     def render(self): ...
@@ -98,26 +98,26 @@
     e: Number
     f: Number
     @classmethod
     def identity(cls): ...
     @classmethod
     def translation(cls, x, y): ...
     @classmethod
-    def scaling(cls, x, y: Incomplete | None = ...): ...
+    def scaling(cls, x, y: Incomplete | None = None): ...
     @classmethod
     def rotation(cls, theta): ...
     @classmethod
     def rotation_d(cls, theta_d): ...
     @classmethod
-    def shearing(cls, x, y: Incomplete | None = ...): ...
+    def shearing(cls, x, y: Incomplete | None = None): ...
     def translate(self, x, y): ...
-    def scale(self, x, y: Incomplete | None = ...): ...
+    def scale(self, x, y: Incomplete | None = None): ...
     def rotate(self, theta): ...
     def rotate_d(self, theta_d): ...
-    def shear(self, x, y: Incomplete | None = ...): ...
+    def shear(self, x, y: Incomplete | None = None): ...
     def about(self, x, y): ...
     def __mul__(self, other): ...
     def __rmul__(self, other): ...
     def __matmul__(self, other): ...
     def render(self, last_item): ...
 
 class GraphicsStyle:
@@ -312,20 +312,20 @@
 
 class Close(NamedTuple):
     def render(self, gsd_registry, style, last_item, initial_point): ...
     def render_debug(self, gsd_registry, style, last_item, initial_point, debug_stream, pfx): ...
 
 class DrawingContext:
     def __init__(self) -> None: ...
-    def add_item(self, item, _copy: bool = ...) -> None: ...
+    def add_item(self, item, _copy: bool = True) -> None: ...
     def render(self, gsd_registry, first_point, scale, height, starting_style): ...
     def render_debug(self, gsd_registry, first_point, scale, height, starting_style, debug_stream): ...
 
 class PaintedPath:
-    def __init__(self, x: int = ..., y: int = ...) -> None: ...
+    def __init__(self, x: int = 0, y: int = 0) -> None: ...
     def __deepcopy__(self, memo) -> Self: ...
     @property
     def style(self): ...
     @property
     def transform(self): ...
     @transform.setter
     def transform(self, tf) -> None: ...
@@ -339,17 +339,17 @@
     def paint_rule(self, style) -> None: ...
     @property
     def clipping_path(self): ...
     @clipping_path.setter
     def clipping_path(self, new_clipath) -> None: ...
     @contextmanager
     def transform_group(self, transform) -> Iterator[Self]: ...
-    def add_path_element(self, item, _copy: bool = ...) -> None: ...
+    def add_path_element(self, item, _copy: bool = True) -> None: ...
     def remove_last_path_element(self) -> None: ...
-    def rectangle(self, x, y, w, h, rx: int = ..., ry: int = ...) -> Self: ...
+    def rectangle(self, x, y, w, h, rx: int = 0, ry: int = 0) -> Self: ...
     def circle(self, cx, cy, r) -> Self: ...
     def ellipse(self, cx, cy, rx, ry) -> Self: ...
     def move_to(self, x, y) -> Self: ...
     def move_relative(self, x, y) -> Self: ...
     def line_to(self, x, y) -> Self: ...
     def line_relative(self, dx, dy) -> Self: ...
     def horizontal_line_to(self, x) -> Self: ...
@@ -360,23 +360,23 @@
     def curve_relative(self, dx1, dy1, dx2, dy2, dx3, dy3) -> Self: ...
     def quadratic_curve_to(self, x1, y1, x2, y2) -> Self: ...
     def quadratic_curve_relative(self, dx1, dy1, dx2, dy2) -> Self: ...
     def arc_to(self, rx, ry, rotation, large_arc, positive_sweep, x, y) -> Self: ...
     def arc_relative(self, rx, ry, rotation, large_arc, positive_sweep, dx, dy) -> Self: ...
     def close(self) -> None: ...
     def render(
-        self, gsd_registry, style, last_item, initial_point, debug_stream: Incomplete | None = ..., pfx: Incomplete | None = ...
+        self, gsd_registry, style, last_item, initial_point, debug_stream: Incomplete | None = None, pfx: Incomplete | None = None
     ): ...
     def render_debug(self, gsd_registry, style, last_item, initial_point, debug_stream, pfx): ...
 
 class ClippingPath(PaintedPath):
     paint_rule: Incomplete
-    def __init__(self, x: int = ..., y: int = ...) -> None: ...
+    def __init__(self, x: int = 0, y: int = 0) -> None: ...
     def render(
-        self, gsd_registry, style, last_item, initial_point, debug_stream: Incomplete | None = ..., pfx: Incomplete | None = ...
+        self, gsd_registry, style, last_item, initial_point, debug_stream: Incomplete | None = None, pfx: Incomplete | None = None
     ): ...
     def render_debug(self, gsd_registry, style, last_item, initial_point, debug_stream, pfx): ...
 
 class GraphicsContext:
     style: GraphicsStyle
     path_items: list[Incomplete]
     def __init__(self) -> None: ...
@@ -385,33 +385,33 @@
     def transform(self) -> Transform | None: ...
     @transform.setter
     def transform(self, tf) -> None: ...
     @property
     def clipping_path(self) -> ClippingPath | None: ...
     @clipping_path.setter
     def clipping_path(self, new_clipath) -> None: ...
-    def add_item(self, item, _copy: bool = ...) -> None: ...
+    def add_item(self, item, _copy: bool = True) -> None: ...
     def remove_last_item(self) -> None: ...
     def merge(self, other_context) -> None: ...
     def build_render_list(
         self,
         gsd_registry,
         style,
         last_item,
         initial_point,
-        debug_stream: Incomplete | None = ...,
-        pfx: Incomplete | None = ...,
-        _push_stack: bool = ...,
+        debug_stream: Incomplete | None = None,
+        pfx: Incomplete | None = None,
+        _push_stack: bool = True,
     ): ...
     def render(
         self,
         gsd_registry,
         style: DrawingContext,
         last_item,
         initial_point,
-        debug_stream: Incomplete | None = ...,
-        pfx: Incomplete | None = ...,
-        _push_stack: bool = ...,
+        debug_stream: Incomplete | None = None,
+        pfx: Incomplete | None = None,
+        _push_stack: bool = True,
     ): ...
     def render_debug(
-        self, gsd_registry, style: DrawingContext, last_item, initial_point, debug_stream, pfx, _push_stack: bool = ...
+        self, gsd_registry, style: DrawingContext, last_item, initial_point, debug_stream, pfx, _push_stack: bool = True
     ): ...
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/encryption.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/encryption.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from _typeshed import Incomplete, SupportsLenAndGetItem
 from collections.abc import Generator, Iterable
+from logging import Logger
 from typing import ClassVar, Protocol, TypeVar
 from typing_extensions import TypeAlias
 
 from .enums import EncryptionMethod
 from .fpdf import FPDF
 from .syntax import Name, PDFObject
 
 _Key: TypeAlias = SupportsLenAndGetItem[int]
 _T_co = TypeVar("_T_co", covariant=True)
 
+LOGGER: Logger
+
 import_error: ImportError | None
 
 class _SupportsGetItem(Protocol[_T_co]):
     def __getitem__(self, __k: int) -> _T_co: ...
 
 class ARC4:
     MOD: ClassVar[int]
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/enums.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/enums.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,59 @@
     @classmethod
     def coerce(cls, value: Self | str) -> Self: ...
 
 class CoerciveIntEnum(IntEnum):
     @classmethod
     def coerce(cls, value: Self | str | int) -> Self: ...
 
+class CoerciveIntFlag(IntFlag):
+    @classmethod
+    def coerce(cls, value: Self | str | int) -> Self: ...
+
+class WrapMode(CoerciveEnum):
+    WORD: str
+    CHAR: str
+
 class CharVPos(CoerciveEnum):
     SUP: str
     SUB: str
     NOM: str
     DENOM: str
     LINE: str
 
 class Align(CoerciveEnum):
     C: str
     X: str
     L: str
     R: str
     J: str
 
+class TextEmphasis(CoerciveIntFlag):
+    B: int
+    I: int
+    U: int
+
+    @property
+    def style(self) -> str: ...
+
+class TableBordersLayout(CoerciveEnum):
+    ALL: str
+    NONE: str
+    INTERNAL: str
+    MINIMAL: str
+    HORIZONTAL_LINES: str
+    NO_HORIZONTAL_LINES: str
+    SINGLE_TOP_LINE: str
+
+class TableCellFillMode(CoerciveEnum):
+    NONE: str
+    ALL: str
+    ROWS: str
+    COLUMNS: str
+
 class RenderStyle(CoerciveEnum):
     D: str
     F: str
     DF: str
     @property
     def operator(self) -> str: ...
     @property
@@ -196,9 +227,7 @@
     @classmethod
     def none(cls) -> Literal[0]: ...
 
 class EncryptionMethod(Enum):
     NO_ENCRYPTION: int
     RC4: int
     AES_128: int
-
-__pdoc__: dict[str, bool]
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/fpdf.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/fpdf.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,104 @@
 import datetime
-from _typeshed import Incomplete, StrPath
+from _typeshed import Incomplete, StrPath, Unused
 from collections.abc import Callable, Iterable, Sequence
 from contextlib import _GeneratorContextManager
 from io import BytesIO
 from pathlib import PurePath
 from re import Pattern
 from typing import Any, ClassVar, NamedTuple, overload
 from typing_extensions import Literal, TypeAlias
 
 from fpdf import ViewerPreferences
 from PIL import Image
 
 from .annotations import AnnotationDict, PDFEmbeddedFile
-from .drawing import DrawingContext, PaintedPath
+from .drawing import DeviceGray, DeviceRGB, DrawingContext, PaintedPath
 from .enums import (
     Align,
     AnnotationFlag,
     AnnotationName,
     Corner,
     FileAttachmentAnnotationName,
     PageLayout,
     PathPaintRule,
     RenderStyle,
+    TableBordersLayout,
+    TableCellFillMode,
     TextMarkupType,
     TextMode as TextMode,
+    WrapMode as WrapMode,
     XPos as XPos,
     YPos as YPos,
 )
+from .errors import FPDFException as FPDFException
+from .fonts import FontFace
+from .graphics_state import GraphicsStateMixin
 from .html import HTML2FPDF
-from .output import PDFPage
+from .output import OutputProducer, PDFPage
 from .recorder import FPDFRecorder
 from .structure_tree import StructureTreeBuilder
 from .syntax import DestinationXYZ
+from .table import Table
 from .util import _Unit
 
-__all__ = ["FPDF", "XPos", "YPos", "get_page_format", "TextMode", "TitleStyle", "PAGE_FORMATS"]
+__all__ = ["FPDF", "XPos", "YPos", "get_page_format", "ImageInfo", "TextMode", "TitleStyle", "PAGE_FORMATS"]
 
 _Orientation: TypeAlias = Literal["", "portrait", "p", "P", "landscape", "l", "L"]
 _Format: TypeAlias = Literal["", "a3", "A3", "a4", "A4", "a5", "A5", "letter", "Letter", "legal", "Legal"]
 _FontStyle: TypeAlias = Literal["", "B", "I"]
 _FontStyles: TypeAlias = Literal["", "B", "I", "U", "BU", "UB", "BI", "IB", "IU", "UI", "BIU", "BUI", "IBU", "IUB", "UBI", "UIB"]
 PAGE_FORMATS: dict[_Format, tuple[float, float]]
 
-class TitleStyle(NamedTuple):
-    font_family: str | None = ...
-    font_style: str | None = ...
-    font_size_pt: int | None = ...
-    color: int | tuple[int, int, int] | None = ...
-    underline: bool = ...
-    t_margin: int | None = ...
-    l_margin: int | None = ...
-    b_margin: int | None = ...
+class ImageInfo(dict[str, Any]):
+    @property
+    def width(self) -> int: ...
+    @property
+    def height(self) -> int: ...
+    @property
+    def rendered_width(self) -> int: ...
+    @property
+    def rendered_height(self) -> int: ...
+
+class TitleStyle(FontFace):
+    t_margin: int | None
+    l_margin: int | None
+    b_margin: int | None
+
+    def __init__(
+        self,
+        font_family: str | None = None,
+        font_style: str | None = None,
+        font_size_pt: int | None = None,
+        color: int | tuple[int, int, int] | None = None,
+        underline: bool = False,
+        t_margin: int | None = None,
+        l_margin: int | None = None,
+        b_margin: int | None = None,
+    ) -> None: ...
 
 class ToCPlaceholder(NamedTuple):
     render_function: Callable[[FPDF, Any], object]
     start_page: int
     y: int
     pages: int = ...
 
 class SubsetMap:
     def __init__(self, identities: Iterable[int]) -> None: ...
     def __len__(self) -> int: ...
     def pick(self, unicode: int) -> int: ...
     def dict(self) -> dict[int, int]: ...
 
-def get_page_format(format: _Format | tuple[float, float], k: float | None = ...) -> tuple[float, float]: ...
+def get_page_format(format: _Format | tuple[float, float], k: float | None = None) -> tuple[float, float]: ...
 
 # TODO: TypedDicts
 _Font: TypeAlias = dict[str, Any]
 _Image: TypeAlias = dict[str, Any]
 
-class FPDF:
+class FPDF(GraphicsStateMixin):
     MARKDOWN_BOLD_MARKER: ClassVar[str]
     MARKDOWN_ITALICS_MARKER: ClassVar[str]
     MARKDOWN_UNDERLINE_MARKER: ClassVar[str]
     MARKDOWN_LINK_REGEX: ClassVar[Pattern[str]]
     MARKDOWN_LINK_COLOR: ClassVar[Incomplete | None]
 
     HTML2FPDF_CLASS: ClassVar[type[HTML2FPDF]]
@@ -100,28 +124,15 @@
     section_title_styles: dict[int, Incomplete]
 
     core_fonts: dict[str, str]
     core_fonts_encoding: str
     font_aliases: dict[str, str]
     k: float
 
-    font_family: str
-    font_style: str
-    font_size_pt: float
-    font_stretching: float
-    char_spacing: float
-    underline: bool
-    current_font: _Font
-    draw_color: str
-    fill_color: str
-    text_color: str
     page_background: Incomplete | None
-    dash_pattern: dict[str, int]  # TODO: TypedDict
-    line_width: float
-    text_mode: TextMode
 
     dw_pt: float
     dh_pt: float
     def_orientation: Literal["P", "L"]
     x: float
     y: float
     l_margin: float
@@ -139,59 +150,58 @@
     w_pt: float
     h_pt: float
     w: float
     h: float
 
     def __init__(
         self,
-        orientation: _Orientation = ...,
-        unit: _Unit | float = ...,
-        format: _Format | tuple[float, float] = ...,
-        font_cache_dir: Literal["DEPRECATED"] = ...,
+        orientation: _Orientation = "portrait",
+        unit: _Unit | float = "mm",
+        format: _Format | tuple[float, float] = "A4",
+        font_cache_dir: Literal["DEPRECATED"] = "DEPRECATED",
     ) -> None: ...
-    # The following definition crashes stubtest 0.991, but seems to be fixed
-    # in later versions.
+    # The following definition crashes stubtest 1.1.1.
     # def set_encryption(
-    #    self,
-    #    owner_password: str,
-    #    user_password: str | None = None,
-    #    encryption_method: EncryptionMethod | str = ...,
-    #    permissions: AccessPermission = ...,
-    #    encrypt_metadata: bool = False,
+    #     self,
+    #     owner_password: str,
+    #     user_password: str | None = None,
+    #     encryption_method: EncryptionMethod | str = ...,
+    #     permissions: AccessPermission = ...,
+    #     encrypt_metadata: bool = False,
     # ) -> None: ...
     # args and kwargs are passed to HTML2FPDF_CLASS constructor.
     def write_html(self, text: str, *args: Any, **kwargs: Any) -> None: ...
     @property
     def is_ttf_font(self) -> bool: ...
     @property
     def page_mode(self): ...
     @property
     def epw(self) -> float: ...
     @property
     def eph(self) -> float: ...
     @property
     def pages_count(self) -> int: ...
     def set_margin(self, margin: float) -> None: ...
-    def set_margins(self, left: float, top: float, right: float = ...) -> None: ...
+    def set_margins(self, left: float, top: float, right: float = -1) -> None: ...
     def set_left_margin(self, margin: float) -> None: ...
     def set_top_margin(self, margin: float) -> None: ...
     r_margin: float
     def set_right_margin(self, margin: float) -> None: ...
     auto_page_break: bool
     b_margin: float
     page_break_trigger: float
-    def set_auto_page_break(self, auto: bool, margin: float = ...) -> None: ...
+    def set_auto_page_break(self, auto: bool, margin: float = 0) -> None: ...
     @property
     def default_page_dimensions(self) -> tuple[float, float]: ...
     zoom_mode: Literal["fullpage", "fullwidth", "real", "default"] | float
     page_layout: PageLayout | None
     def set_display_mode(
         self,
         zoom: Literal["fullpage", "fullwidth", "real", "default"] | float,
-        layout: Literal["single", "continuous", "two", "default"] = ...,
+        layout: Literal["single", "continuous", "two", "default"] = "continuous",
     ) -> None: ...
     def set_compression(self, compress: bool) -> None: ...
     title: str
     def set_title(self, title: str) -> None: ...
     lang: str
     def set_lang(self, lang: str) -> None: ...
     subject: str
@@ -204,137 +214,144 @@
     def set_creator(self, creator: str) -> None: ...
     producer: str
     def set_producer(self, producer: str) -> None: ...
     def set_creation_date(self, date: datetime.datetime) -> None: ...
     def set_xmp_metadata(self, xmp_metadata: str) -> None: ...
     def set_doc_option(self, opt: str, value: str) -> None: ...
     def set_image_filter(self, image_filter: str) -> None: ...
-    def alias_nb_pages(self, alias: str = ...) -> None: ...
+    def alias_nb_pages(self, alias: str = "{nb}") -> None: ...
     def add_page(
         self,
-        orientation: _Orientation = ...,
-        format: _Format | tuple[float, float] = ...,
-        same: bool = ...,
-        duration: int = ...,
-        transition: Incomplete | None = ...,
+        orientation: _Orientation = "",
+        format: _Format | tuple[float, float] = "",
+        same: bool = False,
+        duration: int = 0,
+        transition: Incomplete | None = None,
     ) -> None: ...
     def header(self) -> None: ...
     def footer(self) -> None: ...
     def page_no(self) -> int: ...
-    def set_draw_color(self, r: int, g: int = ..., b: int = ...) -> None: ...
-    def set_fill_color(self, r: int, g: int = ..., b: int = ...) -> None: ...
-    def set_text_color(self, r: int, g: int = ..., b: int = ...) -> None: ...
-    def get_string_width(self, s: str, normalized: bool = ..., markdown: bool = ...) -> float: ...
+    def set_draw_color(self, r: int, g: int = -1, b: int = -1) -> None: ...
+    def set_fill_color(self, r: int, g: int = -1, b: int = -1) -> None: ...
+    def set_text_color(self, r: int, g: int = -1, b: int = -1) -> None: ...
+    def get_string_width(self, s: str, normalized: bool = False, markdown: bool = False) -> float: ...
     def set_line_width(self, width: float) -> None: ...
     def set_page_background(self, background) -> None: ...
-    def drawing_context(self, debug_stream: Incomplete | None = ...) -> _GeneratorContextManager[DrawingContext]: ...
+    def drawing_context(self, debug_stream: Incomplete | None = None) -> _GeneratorContextManager[DrawingContext]: ...
     def new_path(
-        self, x: float = ..., y: float = ..., paint_rule: PathPaintRule = ..., debug_stream: Incomplete | None = ...
+        self, x: float = 0, y: float = 0, paint_rule: PathPaintRule = ..., debug_stream: Incomplete | None = None
     ) -> _GeneratorContextManager[PaintedPath]: ...
-    def draw_path(self, path: PaintedPath, debug_stream: Incomplete | None = ...) -> None: ...
-    def set_dash_pattern(self, dash: float = ..., gap: float = ..., phase: float = ...) -> None: ...
+    def draw_path(self, path: PaintedPath, debug_stream: Incomplete | None = None) -> None: ...
+    def set_dash_pattern(self, dash: float = 0, gap: float = 0, phase: float = 0) -> None: ...
     def line(self, x1: float, y1: float, x2: float, y2: float) -> None: ...
     def polyline(
-        self, point_list: list[tuple[float, float]], fill: bool = ..., polygon: bool = ..., style: RenderStyle | str | None = ...
+        self,
+        point_list: list[tuple[float, float]],
+        fill: bool = False,
+        polygon: bool = False,
+        style: RenderStyle | str | None = None,
+    ) -> None: ...
+    def polygon(
+        self, point_list: list[tuple[float, float]], fill: bool = False, style: RenderStyle | str | None = None
     ) -> None: ...
-    def polygon(self, point_list: list[tuple[float, float]], fill: bool = ..., style: RenderStyle | str | None = ...) -> None: ...
-    def dashed_line(self, x1, y1, x2, y2, dash_length: int = ..., space_length: int = ...) -> None: ...
+    def dashed_line(self, x1, y1, x2, y2, dash_length: int = 1, space_length: int = 1) -> None: ...
     def rect(
         self,
         x: float,
         y: float,
         w: float,
         h: float,
-        style: RenderStyle | str | None = ...,
-        round_corners: tuple[str, ...] | tuple[Corner, ...] | bool = ...,
-        corner_radius: float = ...,
+        style: RenderStyle | str | None = None,
+        round_corners: tuple[str, ...] | tuple[Corner, ...] | bool = False,
+        corner_radius: float = 0,
     ) -> None: ...
-    def ellipse(self, x: float, y: float, w: float, h: float, style: RenderStyle | str | None = ...) -> None: ...
-    def circle(self, x: float, y: float, r, style: RenderStyle | str | None = ...) -> None: ...
+    def ellipse(self, x: float, y: float, w: float, h: float, style: RenderStyle | str | None = None) -> None: ...
+    def circle(self, x: float, y: float, r, style: RenderStyle | str | None = None) -> None: ...
     def regular_polygon(
         self,
         x: float,
         y: float,
         numSides: int,
         polyWidth: float,
-        rotateDegrees: float = ...,
-        style: RenderStyle | str | None = ...,
+        rotateDegrees: float = 0,
+        style: RenderStyle | str | None = None,
     ): ...
     def star(
         self,
         x: float,
         y: float,
         r_in: float,
         r_out: float,
         corners: int,
-        rotate_degrees: float = ...,
-        style: RenderStyle | str | None = ...,
+        rotate_degrees: float = 0,
+        style: RenderStyle | str | None = None,
     ): ...
     def arc(
         self,
         x: float,
         y: float,
         a: float,
         start_angle: float,
         end_angle: float,
-        b: float | None = ...,
-        inclination: float = ...,
-        clockwise: bool = ...,
-        start_from_center: bool = ...,
-        end_at_center: bool = ...,
-        style: RenderStyle | str | None = ...,
+        b: float | None = None,
+        inclination: float = 0,
+        clockwise: bool = False,
+        start_from_center: bool = False,
+        end_at_center: bool = False,
+        style: RenderStyle | str | None = None,
     ) -> None: ...
     def solid_arc(
         self,
         x: float,
         y: float,
         a: float,
         start_angle: float,
         end_angle: float,
-        b: float | None = ...,
-        inclination: float = ...,
-        clockwise: bool = ...,
-        style: RenderStyle | str | None = ...,
+        b: float | None = None,
+        inclination: float = 0,
+        clockwise: bool = False,
+        style: RenderStyle | str | None = None,
     ) -> None: ...
     def add_font(
         self,
         family: str | None = None,
         style: _FontStyle = "",
         fname: str | PurePath | None = None,
         uni: bool | Literal["DEPRECATED"] = "DEPRECATED",
     ) -> None: ...
-    def set_font(self, family: str | None = ..., style: _FontStyles = ..., size: int = ...) -> None: ...
+    def set_font(self, family: str | None = None, style: _FontStyles = "", size: int = 0) -> None: ...
     def set_font_size(self, size: float) -> None: ...
     def set_char_spacing(self, spacing: float) -> None: ...
     def set_stretching(self, stretching: float) -> None: ...
+    def set_fallback_fonts(self, fallback_fonts: Iterable[str], exact_match: bool = True) -> None: ...
     def add_link(self, y: float = 0, x: float = 0, page: int = -1, zoom: float | Literal["null"] = "null") -> int: ...
     def set_link(self, link, y: float = 0, x: float = 0, page: int = -1, zoom: float | Literal["null"] = "null") -> None: ...
     def link(
-        self, x: float, y: float, w: float, h: float, link: str | int, alt_text: str | None = ..., border_width: int = ...
+        self, x: float, y: float, w: float, h: float, link: str | int, alt_text: str | None = None, border_width: int = 0
     ) -> AnnotationDict: ...
     def embed_file(
         self,
-        file_path: StrPath | None = ...,
-        bytes: bytes | None = ...,
-        basename: str | None = ...,
-        modification_date: datetime.datetime | None = ...,
+        file_path: StrPath | None = None,
+        bytes: bytes | None = None,
+        basename: str | None = None,
+        modification_date: datetime.datetime | None = None,
         *,
         creation_date: datetime.datetime | None = ...,
         desc: str = ...,
         compress: bool = ...,
         checksum: bool = ...,
     ) -> str: ...
     def file_attachment_annotation(
         self,
         file_path: StrPath,
         x: float,
         y: float,
-        w: float = ...,
-        h: float = ...,
-        name: FileAttachmentAnnotationName | str | None = ...,
+        w: float = 1,
+        h: float = 1,
+        name: FileAttachmentAnnotationName | str | None = None,
         flags: Iterable[AnnotationFlag | str] = ...,
         *,
         bytes: bytes | None = ...,
         basename: str | None = ...,
         creation_date: datetime.datetime | None = ...,
         modification_date: datetime.datetime | None = ...,
         desc: str = ...,
@@ -342,161 +359,194 @@
         checksum: bool = ...,
     ) -> AnnotationDict: ...
     def text_annotation(
         self,
         x: float,
         y: float,
         text: str,
-        w: float = ...,
-        h: float = ...,
-        name: AnnotationName | str | None = ...,
+        w: float = 1,
+        h: float = 1,
+        name: AnnotationName | str | None = None,
         flags: tuple[AnnotationFlag, ...] | tuple[str, ...] = ...,
     ) -> None: ...
     def add_action(self, action, x: float, y: float, w: float, h: float) -> None: ...
     def highlight(
         self,
         text: str,
-        title: str = ...,
-        type: TextMarkupType | str = ...,
-        color: tuple[float, float, float] = ...,
-        modification_time: datetime.datetime | None = ...,
+        title: str = "",
+        type: TextMarkupType | str = "Highlight",
+        color: tuple[float, float, float] = (1, 1, 0),
+        modification_time: datetime.datetime | None = None,
     ) -> _GeneratorContextManager[None]: ...
     add_highlight = highlight
     def add_text_markup_annotation(
         self,
         type: str,
         text: str,
         quad_points: Sequence[int],
-        title: str = ...,
-        color: tuple[float, float, float] = ...,
-        modification_time: datetime.datetime | None = ...,
-        page: int | None = ...,
+        title: str = "",
+        color: tuple[float, float, float] = (1, 1, 0),
+        modification_time: datetime.datetime | None = None,
+        page: int | None = None,
     ) -> AnnotationDict: ...
     def ink_annotation(
         self,
         coords: Iterable[Incomplete],
-        contents: str = ...,
-        title: str = ...,
-        color: Sequence[float] = ...,
-        border_width: int = ...,
+        contents: str = "",
+        title: str = "",
+        color: Sequence[float] = (1, 1, 0),
+        border_width: int = 1,
     ) -> AnnotationDict: ...
-    def text(self, x: float, y: float, txt: str = ...) -> None: ...
-    def rotate(self, angle: float, x: float | None = ..., y: float | None = ...) -> None: ...
-    def rotation(self, angle: float, x: float | None = ..., y: float | None = ...) -> _GeneratorContextManager[None]: ...
+    def text(self, x: float, y: float, txt: str = "") -> None: ...
+    def rotate(self, angle: float, x: float | None = None, y: float | None = None) -> None: ...
+    def rotation(self, angle: float, x: float | None = None, y: float | None = None) -> _GeneratorContextManager[None]: ...
     def skew(
         self, ax: float = 0, ay: float = 0, x: float | None = None, y: float | None = None
     ) -> _GeneratorContextManager[None]: ...
     def local_context(
         self,
-        font_family: Incomplete | None = ...,
-        font_style: Incomplete | None = ...,
-        font_size: Incomplete | None = ...,
-        line_width: Incomplete | None = ...,
-        draw_color: Incomplete | None = ...,
-        fill_color: Incomplete | None = ...,
-        text_color: Incomplete | None = ...,
-        dash_pattern: Incomplete | None = ...,
+        font_family: Incomplete | None = None,
+        font_style: Incomplete | None = None,
+        font_size: Incomplete | None = None,
+        line_width: Incomplete | None = None,
+        draw_color: Incomplete | None = None,
+        fill_color: Incomplete | None = None,
+        text_color: Incomplete | None = None,
+        dash_pattern: Incomplete | None = None,
         **kwargs,
     ) -> _GeneratorContextManager[None]: ...
     @property
     def accept_page_break(self) -> bool: ...
     def cell(
         self,
-        w: float | None = ...,
-        h: float | None = ...,
-        txt: str = ...,
-        border: bool | Literal[0, 1] | str = ...,
-        ln: int | Literal["DEPRECATED"] = ...,
+        w: float | None = None,
+        h: float | None = None,
+        txt: str = "",
+        border: bool | Literal[0, 1] | str = 0,
+        ln: int | Literal["DEPRECATED"] = "DEPRECATED",
         align: str | Align = ...,
-        fill: bool = ...,
-        link: str = ...,
-        center: bool | Literal["DEPRECATED"] = ...,
-        markdown: bool = ...,
+        fill: bool = False,
+        link: str = "",
+        center: bool | Literal["DEPRECATED"] = "DEPRECATED",
+        markdown: bool = False,
         new_x: XPos | str = ...,
         new_y: YPos | str = ...,
     ) -> bool: ...
+    def get_fallback_font(self, char: str, style: str = "") -> str | None: ...
     def will_page_break(self, height: float) -> bool: ...
     def multi_cell(
         self,
         w: float,
-        h: float | None = ...,
-        txt: str = ...,
-        border: bool | Literal[0, 1] | str = ...,
+        h: float | None = None,
+        txt: str = "",
+        border: bool | Literal[0, 1] | str = 0,
         align: str | Align = ...,
-        fill: bool = ...,
-        split_only: bool = ...,
-        link: str | int = ...,
-        ln: int | Literal["DEPRECATED"] = ...,
-        max_line_height: float | None = ...,
-        markdown: bool = ...,
-        print_sh: bool = ...,
+        fill: bool = False,
+        split_only: bool = False,
+        link: str | int = "",
+        ln: int | Literal["DEPRECATED"] = "DEPRECATED",
+        max_line_height: float | None = None,
+        markdown: bool = False,
+        print_sh: bool = False,
         new_x: XPos | str = ...,
         new_y: YPos | str = ...,
+        wrapmode: WrapMode = ...,
     ): ...
-    def write(self, h: float | None = ..., txt: str = ..., link: str = ..., print_sh: bool = ...) -> None: ...
+    def write(
+        self, h: float | None = None, txt: str = "", link: str = "", print_sh: bool = False, wrapmode: WrapMode = ...
+    ) -> bool: ...
     def image(
         self,
         name: str | Image.Image | BytesIO | StrPath,
         x: float | Align | None = None,
         y: float | None = None,
         w: float = 0,
         h: float = 0,
         type: str = "",
         link: str = "",
         title: str | None = None,
         alt_text: str | None = None,
         dims: tuple[float, float] | None = None,
+        keep_aspect_ratio: bool = False,
     ) -> _Image: ...
-    def ln(self, h: float | None = ...) -> None: ...
+    def preload_image(
+        self, name: str | Image.Image | BytesIO, dims: tuple[float, float] | None = None
+    ) -> tuple[str, Any, ImageInfo]: ...
+    def ln(self, h: float | None = None) -> None: ...
     def get_x(self) -> float: ...
     def set_x(self, x: float) -> None: ...
     def get_y(self) -> float: ...
     def set_y(self, y: float) -> None: ...
     def set_xy(self, x: float, y: float) -> None: ...
-    @overload
-    def output(self, name: Literal[""] = ...) -> bytearray: ...  # type: ignore[misc]
-    @overload
-    def output(self, name: str) -> None: ...
     def normalize_text(self, txt: str) -> str: ...
     def sign_pkcs12(
         self,
         pkcs_filepath: str,
-        password: bytes | None = ...,
-        hashalgo: str = ...,
-        contact_info: str | None = ...,
-        location: str | None = ...,
-        signing_time: datetime.datetime | None = ...,
-        reason: str | None = ...,
+        password: bytes | None = None,
+        hashalgo: str = "sha256",
+        contact_info: str | None = None,
+        location: str | None = None,
+        signing_time: datetime.datetime | None = None,
+        reason: str | None = None,
         flags: tuple[AnnotationFlag, ...] = ...,
     ) -> None: ...
     def sign(
         self,
         key,
         cert,
-        extra_certs: Sequence[Incomplete] = ...,
-        hashalgo: str = ...,
-        contact_info: str | None = ...,
-        location: str | None = ...,
-        signing_time: datetime.datetime | None = ...,
-        reason: str | None = ...,
+        extra_certs: Sequence[Incomplete] = (),
+        hashalgo: str = "sha256",
+        contact_info: str | None = None,
+        location: str | None = None,
+        signing_time: datetime.datetime | None = None,
+        reason: str | None = None,
         flags: tuple[AnnotationFlag, ...] = ...,
     ) -> None: ...
     def file_id(self) -> str: ...
-    def interleaved2of5(self, txt, x: float, y: float, w: float = ..., h: float = ...) -> None: ...
-    def code39(self, txt, x: float, y: float, w: float = ..., h: float = ...) -> None: ...
+    def interleaved2of5(self, txt, x: float, y: float, w: float = 1, h: float = 10) -> None: ...
+    def code39(self, txt, x: float, y: float, w: float = 1.5, h: float = 5) -> None: ...
     def rect_clip(self, x: float, y: float, w: float, h: float) -> _GeneratorContextManager[None]: ...
     def elliptic_clip(self, x: float, y: float, w: float, h: float) -> _GeneratorContextManager[None]: ...
     def round_clip(self, x: float, y: float, r: float) -> _GeneratorContextManager[None]: ...
     def unbreakable(self) -> _GeneratorContextManager[FPDFRecorder]: ...
     def offset_rendering(self) -> _GeneratorContextManager[FPDFRecorder]: ...
-    def insert_toc_placeholder(self, render_toc_function, pages: int = ...) -> None: ...
+    def insert_toc_placeholder(self, render_toc_function, pages: int = 1) -> None: ...
     def set_section_title_styles(
         self,
         level0: TitleStyle,
-        level1: TitleStyle | None = ...,
-        level2: TitleStyle | None = ...,
-        level3: TitleStyle | None = ...,
-        level4: TitleStyle | None = ...,
-        level5: TitleStyle | None = ...,
-        level6: TitleStyle | None = ...,
+        level1: TitleStyle | None = None,
+        level2: TitleStyle | None = None,
+        level3: TitleStyle | None = None,
+        level4: TitleStyle | None = None,
+        level5: TitleStyle | None = None,
+        level6: TitleStyle | None = None,
     ) -> None: ...
     def start_section(self, name: str, level: int = 0, strict: bool = True) -> None: ...
+    def use_font_face(self, font_face: FontFace) -> _GeneratorContextManager[None]: ...
+    def table(
+        self,
+        rows: Iterable[Incomplete] = (),
+        *,
+        align: str | Align = "CENTER",
+        borders_layout: str | TableBordersLayout = ...,
+        cell_fill_color: int | tuple[Incomplete, ...] | DeviceGray | DeviceRGB | None = None,
+        cell_fill_mode: str | TableCellFillMode = ...,
+        col_widths: int | tuple[int, ...] | None = None,
+        first_row_as_headings: bool = True,
+        headings_style: FontFace = ...,
+        line_height: int | None = None,
+        markdown: bool = False,
+        text_align: str | Align = "JUSTIFY",
+        width: int | None = None,
+    ) -> _GeneratorContextManager[Table]: ...
+    @overload
+    def output(  # type: ignore[misc]
+        self,
+        name: Literal[""] | None = "",
+        dest: Unused = "",
+        linearize: bool = False,
+        output_producer_class: Callable[[FPDF], OutputProducer] = ...,
+    ) -> None: ...
+    @overload
+    def output(
+        self, name: str, dest: Unused = "", linearize: bool = False, output_producer_class: Callable[[FPDF], OutputProducer] = ...
+    ) -> bytearray: ...
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/graphics_state.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/graphics_state.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any, ClassVar
 
+from fpdf.fonts import FontFace
+
 from .drawing import DeviceGray, DeviceRGB
 from .enums import TextMode
 
 class GraphicsStateMixin:
     DEFAULT_DRAW_COLOR: ClassVar[DeviceGray]
     DEFAULT_FILL_COLOR: ClassVar[DeviceGray]
     DEFAULT_TEXT_COLOR: ClassVar[DeviceGray]
@@ -96,7 +98,8 @@
     def nom_lift(self): ...
     @nom_lift.setter
     def nom_lift(self, v) -> None: ...
     @property
     def denom_lift(self): ...
     @denom_lift.setter
     def denom_lift(self, v) -> None: ...
+    def font_face(self) -> FontFace: ...
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/html.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/html.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 LEADING_SPACE: Pattern[str]
 WHITESPACE: Pattern[str]
 TRAILING_SPACE: Pattern[str]
 
 COLOR_DICT: Final[dict[str, str]]
 
 def px2mm(px: float) -> float: ...
-def color_as_decimal(color: str | None = ...) -> tuple[int, int, int] | None: ...
+def color_as_decimal(color: str | None = "#000000") -> tuple[int, int, int] | None: ...
 
 class HTML2FPDF(HTMLParser):
     HTML_UNCLOSED_TAGS: ClassVar[tuple[str, ...]]
+
     pdf: Incomplete
     image_map: Incomplete
     li_tag_indent: Incomplete
     table_line_separators: Incomplete
     ul_bullet_char: Incomplete
     style: Incomplete
     href: str
@@ -54,42 +55,37 @@
     theader_out: bool
     table_row_height: int
     heading_level: Incomplete
     heading_sizes: Incomplete
     heading_above: float
     heading_below: float
     warn_on_tags_not_matching: bool
+
+    # Not initialized in __init__:
+    font_face: Incomplete
+    h: float
+
     def __init__(
         self,
         pdf: FPDF,
         image_map: Callable[[str], str] | None = None,
         li_tag_indent: int = 5,
         dd_tag_indent: int = 10,
         table_line_separators: bool = False,
-        ul_bullet_char: str = ...,
+        ul_bullet_char: str = "\x95",
         heading_sizes: Incomplete | None = None,
         warn_on_tags_not_matching: bool = True,
         **_: Unused,
     ): ...
-    def width2unit(self, length): ...
     def handle_data(self, data) -> None: ...
-    def box_shadow(self, w, h, bgcolor) -> None: ...
-    def output_table_header(self) -> None: ...
-    tfooter_out: bool
-    def output_table_footer(self) -> None: ...
-    def output_table_sep(self) -> None: ...
-    font_face: Incomplete
-    table_offset: Incomplete
     def handle_starttag(self, tag, attrs) -> None: ...
-    tbody: Incomplete
     def handle_endtag(self, tag) -> None: ...
-    h: Incomplete
-    def set_font(self, face: Incomplete | None = ..., size: Incomplete | None = ...) -> None: ...
-    def set_style(self, tag: Incomplete | None = ..., enable: bool = ...) -> None: ...
-    def set_text_color(self, r: Incomplete | None = ..., g: int = ..., b: int = ...) -> None: ...
+    def set_font(self, face: Incomplete | None = None, size: Incomplete | None = None) -> None: ...
+    def set_style(self, tag: Incomplete | None = None, enable: bool = False) -> None: ...
+    def set_text_color(self, r: Incomplete | None = None, g: int = 0, b: int = 0) -> None: ...
     def put_link(self, txt) -> None: ...
     def render_toc(self, pdf, outline) -> None: ...
     def error(self, message: str) -> None: ...
 
 def leading_whitespace_repl(matchobj: Match[str]) -> str: ...
 def whitespace_repl(matchobj: Match[str]) -> str: ...
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/line_break.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/line_break.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from _typeshed import Incomplete
 from collections.abc import Sequence
 from typing import NamedTuple
 
+from .enums import WrapMode
+
 SOFT_HYPHEN: str
 HYPHEN: str
 SPACE: str
 NEWLINE: str
 
 class Fragment:
     characters: list[str]
@@ -49,16 +51,16 @@
     def char_vpos(self): ...
     @property
     def lift(self): ...
     @property
     def string(self): ...
     def trim(self, index: int): ...
     def __eq__(self, other: Fragment) -> bool: ...  # type: ignore[override]
-    def get_width(self, start: int = ..., end: int | None = ..., chars: str | None = ..., initial_cs: bool = ...): ...
-    def get_character_width(self, character: str, print_sh: bool = ..., initial_cs: bool = ...): ...
+    def get_width(self, start: int = 0, end: int | None = None, chars: str | None = None, initial_cs: bool = True): ...
+    def get_character_width(self, character: str, print_sh: bool = False, initial_cs: bool = True): ...
 
 class TextLine(NamedTuple):
     fragments: tuple[Incomplete, ...]
     text_width: float
     number_of_spaces: int
     justify: bool
     trailing_nl: bool = ...
@@ -86,31 +88,35 @@
 class CurrentLine:
     print_sh: Incomplete
     fragments: Incomplete
     width: int
     number_of_spaces: int
     space_break_hint: Incomplete
     hyphen_break_hint: Incomplete
-    def __init__(self, print_sh: bool = ...) -> None: ...
+    def __init__(self, print_sh: bool = False) -> None: ...
     def add_character(
         self,
         character: str,
         character_width: float,
         graphics_state: dict[str, Incomplete],
         k: float,
         original_fragment_index: int,
         original_character_index: int,
         url: str | None = None,
     ): ...
-    def manual_break(self, justify: bool = ..., trailing_nl: bool = ...): ...
+    def trim_trailing_spaces(self) -> None: ...
+    def manual_break(self, justify: bool = False, trailing_nl: bool = False): ...
     def automatic_break_possible(self): ...
     def automatic_break(self, justify: bool): ...
 
 class MultiLineBreak:
-    styled_text_fragments: Incomplete
-    justify: Incomplete
-    print_sh: Incomplete
+    styled_text_fragments: Sequence[Fragment]
+    justify: bool
+    print_sh: bool
+    wrap_mode: WrapMode
     fragment_index: int
     character_index: int
-    idx_last_forced_break: Incomplete
-    def __init__(self, styled_text_fragments: Sequence[Fragment], justify: bool = ..., print_sh: bool = ...) -> None: ...
-    def get_line_of_given_width(self, maximum_width: float, wordsplit: bool = ...): ...
+    idx_last_forced_break: int | None
+    def __init__(
+        self, styled_text_fragments: Sequence[Fragment], justify: bool = False, print_sh: bool = False, wrapmode: WrapMode = ...
+    ) -> None: ...
+    def get_line_of_given_width(self, maximum_width: float, wordsplit: bool = True): ...
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/linearization.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/linearization.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/outline.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/outline.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     prev: Incomplete | None
     next: Incomplete | None
     first: Incomplete | None
     last: Incomplete | None
     count: int
     dest: Destination | None
     struct_elem: StructElem | None
-    def __init__(self, title: str, dest: Destination | None = ..., struct_elem: StructElem | None = ...) -> None: ...
+    def __init__(self, title: str, dest: Destination | None = None, struct_elem: StructElem | None = None) -> None: ...
 
 class OutlineDictionary(PDFObject):
     type: str
     first: Incomplete | None
     last: Incomplete | None
     count: int
     def __init__(self) -> None: ...
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/output.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/output.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from _typeshed import Incomplete, Unused
 from collections import defaultdict
 from logging import Logger
 from typing_extensions import Final
 
 from .annotations import AnnotationDict
 from .encryption import StandardSecurityHandler
-from .syntax import Name, PDFArray, PDFContentStream, PDFObject
+from .syntax import Name, PDFArray, PDFContentStream, PDFObject, PDFString
 
 LOGGER: Logger
 ZOOM_CONFIGS: Final[dict[str, tuple[str, ...]]]
 
 class ContentWithoutID:
     def serialize(self, _security_handler: StandardSecurityHandler | None = None) -> str | None: ...
 
@@ -27,15 +27,20 @@
     w: Incomplete | None
     descendant_fonts: Incomplete | None
     to_unicode: Incomplete | None
     c_i_d_system_info: Incomplete | None
     font_descriptor: Incomplete | None
     c_i_d_to_g_i_d_map: Incomplete | None
     def __init__(
-        self, subtype: str, base_font: str, encoding: str | None = ..., d_w: Incomplete | None = ..., w: Incomplete | None = ...
+        self,
+        subtype: str,
+        base_font: str,
+        encoding: str | None = None,
+        d_w: Incomplete | None = None,
+        w: Incomplete | None = None,
     ) -> None: ...
 
 class PDFFontDescriptor(PDFObject):
     type: Name
     ascent: Incomplete
     descent: Incomplete
     cap_height: Incomplete
@@ -44,18 +49,17 @@
     italic_angle: Incomplete
     stem_v: Incomplete
     missing_width: Incomplete
     font_name: Incomplete | None
     def __init__(self, ascent, descent, cap_height, flags, font_b_box, italic_angle, stem_v, missing_width) -> None: ...
 
 class CIDSystemInfo(PDFObject):
-    registry: str
-    ordering: str
-    supplement: Incomplete
-    def __init__(self, registry: str | None, ordering: str | None, supplement) -> None: ...
+    registry: PDFString
+    ordering: PDFString
+    supplement: int
 
 class PDFInfo(PDFObject):
     title: str | None
     subject: str | None
     author: str | None
     keywords: str | None
     creator: str | None
@@ -90,18 +94,18 @@
     mark_info: Incomplete | None
     metadata: Incomplete | None
     names: Incomplete | None
     outlines: Incomplete | None
     struct_tree_root: Incomplete | None
     def __init__(
         self,
-        lang: str | None = ...,
-        page_layout: Incomplete | None = ...,
-        page_mode: Incomplete | None = ...,
-        viewer_preferences: Incomplete | None = ...,
+        lang: str | None = None,
+        page_layout: Incomplete | None = None,
+        page_mode: Incomplete | None = None,
+        viewer_preferences: Incomplete | None = None,
     ) -> None: ...
 
 class PDFResources(PDFObject):
     proc_set: Incomplete
     font: Incomplete
     x_object: Incomplete
     ext_g_state: Incomplete
@@ -131,19 +135,24 @@
         self,
         contents,
         subtype: str,
         width,
         height,
         color_space,
         bits_per_component,
-        img_filter: str | None = ...,
-        decode: Incomplete | None = ...,
-        decode_parms: Incomplete | None = ...,
+        img_filter: str | None = None,
+        decode: Incomplete | None = None,
+        decode_parms: Incomplete | None = None,
     ) -> None: ...
 
+class PDFICCPObject(PDFContentStream):
+    n: Incomplete
+    alternate: Name
+    def __init__(self, contents: bytes, n, alternate: str) -> None: ...
+
 class PDFPage(PDFObject):
     type: Name
     contents: Incomplete
     dur: Incomplete | None
     trans: Incomplete
     annots: PDFArray[AnnotationDict]
     group: Incomplete | None
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/structure_tree.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/structure_tree.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -25,24 +25,24 @@
     alt: PDFString | None
     pg: Incomplete | None
     def __init__(
         self,
         struct_type: str,
         parent: PDFObject,
         kids: Iterable[int] | Iterable[StructElem],
-        page_number: int | None = ...,
-        title: str | None = ...,
-        alt: str | None = ...,
+        page_number: int | None = None,
+        title: str | None = None,
+        alt: str | None = None,
     ) -> None: ...
     def page_number(self) -> int | None: ...
 
 class StructureTreeBuilder:
     struct_tree_root: Incomplete
     doc_struct_elem: Incomplete
     struct_elem_per_mc: Incomplete
     def __init__(self) -> None: ...
     def add_marked_content(
-        self, page_number: int, struct_type: str, mcid: int | None = ..., title: str | None = ..., alt_text: str | None = ...
+        self, page_number: int, struct_type: str, mcid: int | None = None, title: str | None = None, alt_text: str | None = None
     ) -> tuple[Incomplete, Incomplete]: ...
     def next_mcid_for_page(self, page_number: int) -> int: ...
     def empty(self) -> bool: ...
     def __iter__(self) -> Generator[Incomplete, None, None]: ...
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/svg.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/svg.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 class Percent(float): ...
 
 unit_splitter: Pattern[str]
 relative_length_units: set[str]
 absolute_length_units: dict[str, int]
 angle_units: dict[str, float]
 
-def resolve_length(length_str, default_unit: str = ...): ...
-def resolve_angle(angle_str, default_unit: str = ...): ...
+def resolve_length(length_str, default_unit: str = "pt"): ...
+def resolve_angle(angle_str, default_unit: str = "deg"): ...
 def xmlns(space, name): ...
 def xmlns_lookup(space, *names): ...
 
 shape_tags: Incomplete
 
 def svgcolor(colorstr): ...
 def convert_stroke_width(incoming): ...
@@ -64,26 +64,28 @@
     def __init__(self, pdf_path: PaintedPath, glyphSet: _TTGlyphSet | None = ...): ...
     def arcTo(self, rx, ry, rotation, arc, sweep, end) -> None: ...
 
 def svg_path_converter(pdf_path: PaintedPath, svg_path: str) -> None: ...
 
 class SVGObject:
     @classmethod
-    def from_file(cls, filename, *args, encoding: str = ..., **kwargs): ...
+    def from_file(cls, filename, *args, encoding: str = "utf-8", **kwargs): ...
     cross_references: Incomplete
     def __init__(self, svg_text) -> None: ...
     preserve_ar: Incomplete
     width: Incomplete
     height: Incomplete
     viewbox: Incomplete
     def extract_shape_info(self, root_tag) -> None: ...
     base_group: Incomplete
     def convert_graphics(self, root_tag) -> None: ...
-    def transform_to_page_viewport(self, pdf, align_viewbox: bool = ...): ...
-    def transform_to_rect_viewport(self, scale, width, height, align_viewbox: bool = ..., ignore_svg_top_attrs: bool = ...): ...
+    def transform_to_page_viewport(self, pdf, align_viewbox: bool = True): ...
+    def transform_to_rect_viewport(
+        self, scale, width, height, align_viewbox: bool = True, ignore_svg_top_attrs: bool = False
+    ): ...
     def draw_to_page(
-        self, pdf, x: Incomplete | None = ..., y: Incomplete | None = ..., debug_stream: Incomplete | None = ...
+        self, pdf, x: Incomplete | None = None, y: Incomplete | None = None, debug_stream: Incomplete | None = None
     ) -> None: ...
     def handle_defs(self, defs) -> None: ...
     def build_xref(self, xref): ...
-    def build_group(self, group, pdf_group: Incomplete | None = ...): ...
+    def build_group(self, group, pdf_group: Incomplete | None = None): ...
     def build_path(self, path): ...
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/syntax.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/syntax.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,69 @@
+import datetime
 from _typeshed import Incomplete, SupportsItems
 from abc import ABC, abstractmethod
 from re import Pattern
 from typing import ClassVar, Generic, TypeVar
-from typing_extensions import Literal
+from typing_extensions import Literal, Self
 
 from .encryption import StandardSecurityHandler
 
 _T = TypeVar("_T")
 
 def clear_empty_fields(d): ...
 def create_dictionary_string(
     dict_,
-    open_dict: str = ...,
-    close_dict: str = ...,
-    field_join: str = ...,
-    key_value_join: str = ...,
-    has_empty_fields: bool = ...,
-): ...
+    open_dict: str = "<<",
+    close_dict: str = ">>",
+    field_join: str = "\n",
+    key_value_join: str = " ",
+    has_empty_fields: bool = False,
+) -> str: ...
 def create_list_string(list_): ...
 def iobj_ref(n): ...
 def create_stream(
     stream: str | bytes | bytearray, encryption_handler: StandardSecurityHandler | None = None, obj_id: Incomplete | None = None
 ): ...
 
 class Raw(str): ...
 
 class Name(str):
     NAME_ESC: ClassVar[Pattern[bytes]]
     def serialize(self) -> str: ...
 
 class PDFObject:
-    def __init__(self) -> None: ...
     @property
     def id(self) -> int: ...
     @id.setter
     def id(self, n: int) -> None: ...
     @property
     def ref(self) -> str: ...
-    def serialize(self, obj_dict: Incomplete | None = ..., _security_handler: StandardSecurityHandler | None = None) -> str: ...
+    def serialize(self, obj_dict: Incomplete | None = None, _security_handler: StandardSecurityHandler | None = None) -> str: ...
     def content_stream(self) -> bytes: ...
 
 class PDFContentStream(PDFObject):
     filter: Name | None
     length: int
-    def __init__(self, contents: bytes, compress: bool = ...) -> None: ...
-    def encrypt(self, security_handler: StandardSecurityHandler) -> None: ...
+    def __init__(self, contents: bytes, compress: bool = False) -> None: ...
 
 def build_obj_dict(key_values: SupportsItems[str, Incomplete]) -> dict[str, str]: ...
 def camel_case(snake_case: str) -> str: ...
 
 class PDFString(str):
     USE_HEX_ENCODING: ClassVar[bool]
+    encrypt: bool
+    def __new__(cls, content: str, encrypt: bool = False) -> Self: ...
+    def serialize(self) -> str: ...
+
+class PDFDate:
+    date: datetime.datetime
+    with_tz: bool
+    encrypt: bool
+
+    def __init__(self, date: datetime.datetime, with_tz: bool = False, encrypt: bool = False) -> None: ...
     def serialize(self) -> str: ...
 
 class PDFArray(list[_T], Generic[_T]):
     def serialize(self) -> str: ...
 
 class Destination(ABC):
     @abstractmethod
@@ -62,9 +71,9 @@
 
 class DestinationXYZ(Destination):
     page_number: int
     top: float
     left: float
     zoom: float | Literal["null"]
     page_ref: Incomplete | None
-    def __init__(self, page: int, top: float, left: float = ..., zoom: float | Literal["null"] = ...) -> None: ...
+    def __init__(self, page: int, top: float, left: float = 0, zoom: float | Literal["null"] = "null") -> None: ...
     def serialize(self) -> str: ...
```

### Comparing `types-fpdf2-2.6.1.9/fpdf-stubs/transitions.pyi` & `types-fpdf2-2.7.1.0/fpdf-stubs/transitions.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     direction: Literal[0, 270, 315]
     def __init__(self, direction: Literal[0, 270, 315]) -> None: ...
     def serialize(self) -> str: ...
 
 class FlyTransition(Transition):
     dimension: Literal["H", "V"]
     direction: Literal[0, 270] | None
-    def __init__(self, dimension: Literal["H", "V"], direction: Literal[0, 270] | None = ...) -> None: ...
+    def __init__(self, dimension: Literal["H", "V"], direction: Literal[0, 270] | None = None) -> None: ...
     def serialize(self) -> str: ...
 
 class PushTransition(Transition):
     direction: Literal[0, 270]
     def __init__(self, direction: Literal[0, 270]) -> None: ...
     def serialize(self) -> str: ...
```

### Comparing `types-fpdf2-2.6.1.9/setup.py` & `types-fpdf2-2.7.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `fpdf2`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/fpdf2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `078c6a095892e12c94462889fa43c2c2dc8280ad`.
+This package was generated from typeshed commit `ec1130adcc12431ba85415a6533da68c3692b2cb`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.6.1.9",
+      version="2.7.1.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/fpdf2.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-Pillow>=9.2.0'],
       packages=['fpdf-stubs'],
-      package_data={'fpdf-stubs': ['__init__.pyi', '_fonttools_shims.pyi', 'actions.pyi', 'annotations.pyi', 'deprecation.pyi', 'drawing.pyi', 'encryption.pyi', 'enums.pyi', 'errors.pyi', 'fonts.pyi', 'fpdf.pyi', 'graphics_state.pyi', 'html.pyi', 'image_parsing.pyi', 'line_break.pyi', 'linearization.pyi', 'outline.pyi', 'output.pyi', 'prefs.pyi', 'recorder.pyi', 'sign.pyi', 'structure_tree.pyi', 'svg.pyi', 'syntax.pyi', 'template.pyi', 'transitions.pyi', 'util.pyi', 'METADATA.toml']},
+      package_data={'fpdf-stubs': ['__init__.pyi', '_fonttools_shims.pyi', 'actions.pyi', 'annotations.pyi', 'deprecation.pyi', 'drawing.pyi', 'encryption.pyi', 'enums.pyi', 'errors.pyi', 'fonts.pyi', 'fpdf.pyi', 'graphics_state.pyi', 'html.pyi', 'image_parsing.pyi', 'line_break.pyi', 'linearization.pyi', 'outline.pyi', 'output.pyi', 'prefs.pyi', 'recorder.pyi', 'sign.pyi', 'structure_tree.pyi', 'svg.pyi', 'syntax.pyi', 'table.pyi', 'template.pyi', 'transitions.pyi', 'util.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-fpdf2-2.6.1.9/types_fpdf2.egg-info/PKG-INFO` & `types-fpdf2-2.7.1.0/types_fpdf2.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-fpdf2
-Version: 2.6.1.9
+Version: 2.7.1.0
 Summary: Typing stubs for fpdf2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/fpdf2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `fpdf2`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/fpdf2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `078c6a095892e12c94462889fa43c2c2dc8280ad`.
+This package was generated from typeshed commit `ec1130adcc12431ba85415a6533da68c3692b2cb`.
```

### Comparing `types-fpdf2-2.6.1.9/types_fpdf2.egg-info/SOURCES.txt` & `types-fpdf2-2.7.1.0/types_fpdf2.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 fpdf-stubs/output.pyi
 fpdf-stubs/prefs.pyi
 fpdf-stubs/recorder.pyi
 fpdf-stubs/sign.pyi
 fpdf-stubs/structure_tree.pyi
 fpdf-stubs/svg.pyi
 fpdf-stubs/syntax.pyi
+fpdf-stubs/table.pyi
 fpdf-stubs/template.pyi
 fpdf-stubs/transitions.pyi
 fpdf-stubs/util.pyi
 types_fpdf2.egg-info/PKG-INFO
 types_fpdf2.egg-info/SOURCES.txt
 types_fpdf2.egg-info/dependency_links.txt
 types_fpdf2.egg-info/requires.txt
```

