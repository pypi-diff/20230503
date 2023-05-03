# Comparing `tmp/flattrs-23.1.0b7.tar.gz` & `tmp/flattrs-23.1.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flattrs-23.1.0b7.tar", last modified: Tue Mar 28 14:04:53 2023, max compression
+gzip compressed data, was "flattrs-23.1.0b8.tar", last modified: Wed May  3 10:59:42 2023, max compression
```

## Comparing `flattrs-23.1.0b7.tar` & `flattrs-23.1.0b8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-03-28 14:04:53.066082 flattrs-23.1.0b7/
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1074 2020-11-10 12:31:21.000000 flattrs-23.1.0b7/LICENSE
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      186 2023-03-28 14:04:53.066309 flattrs-23.1.0b7/PKG-INFO
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     2299 2023-03-28 14:03:50.000000 flattrs-23.1.0b7/README.rst
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      308 2023-02-23 10:21:14.000000 flattrs-23.1.0b7/pyproject.toml
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      136 2023-03-28 14:04:53.067166 flattrs-23.1.0b7/setup.cfg
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1118 2023-03-28 14:02:35.000000 flattrs-23.1.0b7/setup.py
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-03-28 14:04:53.047872 flattrs-23.1.0b7/src/
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-03-28 14:04:53.052932 flattrs-23.1.0b7/src/flattrs/
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      930 2023-02-28 15:21:53.000000 flattrs-23.1.0b7/src/flattrs/__init__.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)    11817 2023-03-15 13:05:01.000000 flattrs-23.1.0b7/src/flattrs/_analysis.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1686 2023-02-25 17:46:21.000000 flattrs-23.1.0b7/src/flattrs/_consts.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      489 2023-03-15 13:05:01.000000 flattrs-23.1.0b7/src/flattrs/_types.py
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-03-28 14:04:53.062891 flattrs-23.1.0b7/src/flattrs/cflattrs/
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)        0 2023-02-23 10:21:14.000000 flattrs-23.1.0b7/src/flattrs/cflattrs/__init__.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)   701668 2023-03-28 13:58:54.000000 flattrs-23.1.0b7/src/flattrs/cflattrs/builder.c
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)    28957 2023-02-23 10:21:14.000000 flattrs-23.1.0b7/src/flattrs/cflattrs/builder.pyx
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)   170967 2023-02-23 10:23:16.000000 flattrs-23.1.0b7/src/flattrs/cflattrs/encode.c
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1443 2023-02-23 10:21:14.000000 flattrs-23.1.0b7/src/flattrs/cflattrs/encode.pyx
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)   336629 2023-03-28 13:58:54.000000 flattrs-23.1.0b7/src/flattrs/cflattrs/number_types.c
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      351 2023-02-23 10:21:14.000000 flattrs-23.1.0b7/src/flattrs/cflattrs/number_types.pxd
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     2081 2023-02-23 10:21:14.000000 flattrs-23.1.0b7/src/flattrs/cflattrs/number_types.pyx
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)    20943 2023-03-08 16:56:01.000000 flattrs-23.1.0b7/src/flattrs/converters.py
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-03-28 14:04:53.064231 flattrs-23.1.0b7/src/flattrs/modgen/
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)        0 2023-02-23 10:21:14.000000 flattrs-23.1.0b7/src/flattrs/modgen/__init__.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      451 2023-03-15 13:05:01.000000 flattrs-23.1.0b7/src/flattrs/modgen/__main__.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1664 2023-03-15 13:05:01.000000 flattrs-23.1.0b7/src/flattrs/modgen/parser.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)    26288 2023-03-28 13:28:19.000000 flattrs-23.1.0b7/src/flattrs/modgen/renderer.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)        0 2023-02-23 10:21:14.000000 flattrs-23.1.0b7/src/flattrs/py.typed
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1413 2023-02-25 17:46:21.000000 flattrs-23.1.0b7/src/flattrs/types.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     2765 2023-03-15 13:05:01.000000 flattrs-23.1.0b7/src/flattrs/typing.py
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-03-28 14:04:53.056410 flattrs-23.1.0b7/src/flattrs.egg-info/
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      186 2023-03-28 14:04:53.000000 flattrs-23.1.0b7/src/flattrs.egg-info/PKG-INFO
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      915 2023-03-28 14:04:53.000000 flattrs-23.1.0b7/src/flattrs.egg-info/SOURCES.txt
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)        1 2023-03-28 14:04:53.000000 flattrs-23.1.0b7/src/flattrs.egg-info/dependency_links.txt
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)       57 2023-03-28 14:04:53.000000 flattrs-23.1.0b7/src/flattrs.egg-info/entry_points.txt
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)        1 2020-11-10 12:31:30.000000 flattrs-23.1.0b7/src/flattrs.egg-info/not-zip-safe
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)      142 2023-03-28 14:04:53.000000 flattrs-23.1.0b7/src/flattrs.egg-info/requires.txt
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)        8 2023-03-28 14:04:53.000000 flattrs-23.1.0b7/src/flattrs.egg-info/top_level.txt
-drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-03-28 14:04:53.065560 flattrs-23.1.0b7/tests/
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1070 2023-03-08 16:53:46.000000 flattrs-23.1.0b7/tests/test_misc.py
--rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1511 2023-03-15 13:05:01.000000 flattrs-23.1.0b7/tests/test_modgen.py
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.893114 flattrs-23.1.0b8/
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1074 2020-11-10 12:31:21.000000 flattrs-23.1.0b8/LICENSE
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      186 2023-05-03 10:59:42.893250 flattrs-23.1.0b8/PKG-INFO
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     2382 2023-05-03 10:51:46.000000 flattrs-23.1.0b8/README.rst
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      308 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/pyproject.toml
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      136 2023-05-03 10:59:42.893741 flattrs-23.1.0b8/setup.cfg
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1118 2023-05-03 10:57:32.000000 flattrs-23.1.0b8/setup.py
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.878152 flattrs-23.1.0b8/src/
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.882460 flattrs-23.1.0b8/src/flattrs/
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      930 2023-02-28 15:21:53.000000 flattrs-23.1.0b8/src/flattrs/__init__.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)    11817 2023-03-15 13:05:01.000000 flattrs-23.1.0b8/src/flattrs/_analysis.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1686 2023-02-25 17:46:21.000000 flattrs-23.1.0b8/src/flattrs/_consts.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      489 2023-03-15 13:05:01.000000 flattrs-23.1.0b8/src/flattrs/_types.py
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.890634 flattrs-23.1.0b8/src/flattrs/cflattrs/
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)        0 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/__init__.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)   701668 2023-05-02 23:55:06.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/builder.c
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)    28957 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/builder.pyx
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)   170967 2023-02-23 10:23:16.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/encode.c
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1443 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/encode.pyx
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)   336629 2023-05-02 23:55:06.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/number_types.c
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      351 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/number_types.pxd
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     2081 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/cflattrs/number_types.pyx
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)    20943 2023-03-08 16:56:01.000000 flattrs-23.1.0b8/src/flattrs/converters.py
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.891959 flattrs-23.1.0b8/src/flattrs/modgen/
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)        0 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/modgen/__init__.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      451 2023-03-15 13:05:01.000000 flattrs-23.1.0b8/src/flattrs/modgen/__main__.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1664 2023-03-15 13:05:01.000000 flattrs-23.1.0b8/src/flattrs/modgen/parser.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)    27816 2023-05-03 10:51:46.000000 flattrs-23.1.0b8/src/flattrs/modgen/renderer.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)        0 2023-02-23 10:21:14.000000 flattrs-23.1.0b8/src/flattrs/py.typed
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1413 2023-02-25 17:46:21.000000 flattrs-23.1.0b8/src/flattrs/types.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     2765 2023-03-15 13:05:01.000000 flattrs-23.1.0b8/src/flattrs/typing.py
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.884601 flattrs-23.1.0b8/src/flattrs.egg-info/
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      186 2023-05-03 10:59:42.000000 flattrs-23.1.0b8/src/flattrs.egg-info/PKG-INFO
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      915 2023-05-03 10:59:42.000000 flattrs-23.1.0b8/src/flattrs.egg-info/SOURCES.txt
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)        1 2023-05-03 10:59:42.000000 flattrs-23.1.0b8/src/flattrs.egg-info/dependency_links.txt
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)       57 2023-05-03 10:59:42.000000 flattrs-23.1.0b8/src/flattrs.egg-info/entry_points.txt
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)        1 2020-11-10 12:31:30.000000 flattrs-23.1.0b8/src/flattrs.egg-info/not-zip-safe
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)      142 2023-05-03 10:59:42.000000 flattrs-23.1.0b8/src/flattrs.egg-info/requires.txt
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)        8 2023-05-03 10:59:42.000000 flattrs-23.1.0b8/src/flattrs.egg-info/top_level.txt
+drwxr-xr-x   0 tintvrtkovic   (501) staff       (20)        0 2023-05-03 10:59:42.892795 flattrs-23.1.0b8/tests/
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1070 2023-03-08 16:53:46.000000 flattrs-23.1.0b8/tests/test_misc.py
+-rw-r--r--   0 tintvrtkovic   (501) staff       (20)     1511 2023-03-15 13:05:01.000000 flattrs-23.1.0b8/tests/test_modgen.py
```

### Comparing `flattrs-23.1.0b7/LICENSE` & `flattrs-23.1.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/README.rst` & `flattrs-23.1.0b8/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 .. image:: https://img.shields.io/github/license/pocketzworld/flattrs?style=flat-square
    :alt: MIT
 
 Changelog:
 ----------
 
+23.1.0b8 (2023-05-03)
+~~~~~~~~~~~~~~~~~~~~~
+* Greatly improve namespace handling.
+
 23.1.0b7 (2023-03-28)
 ~~~~~~~~~~~~~~~~~~~~~
 * Implement reordering of unions in the generated code where required.
 * Internal refactor for more immutability.
 
 23.1.0b6 (2023-03-15)
 ~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `flattrs-23.1.0b7/setup.py` & `flattrs-23.1.0b8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 else:
     ext_modules = []
 
 setup(
     name="flattrs",
     long_description="Flatbuffers support for Python",
     long_description_content_type="text/x-rst",
-    version="23.1.0.b7",
+    version="23.1.0.b8",
     install_requires=[
         "attrs",
         "flatbuffers==23.1.4",
         "click",
         "lark >= 1.1.5",
         "immutables",
     ],
```

### Comparing `flattrs-23.1.0b7/src/flattrs/__init__.py` & `flattrs-23.1.0b8/src/flattrs/__init__.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/src/flattrs/_analysis.py` & `flattrs-23.1.0b8/src/flattrs/_analysis.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/src/flattrs/_consts.py` & `flattrs-23.1.0b8/src/flattrs/_consts.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/src/flattrs/cflattrs/builder.c` & `flattrs-23.1.0b8/src/flattrs/cflattrs/builder.c`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/src/flattrs/cflattrs/builder.pyx` & `flattrs-23.1.0b8/src/flattrs/cflattrs/builder.pyx`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/src/flattrs/cflattrs/encode.c` & `flattrs-23.1.0b8/src/flattrs/cflattrs/encode.c`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/src/flattrs/cflattrs/encode.pyx` & `flattrs-23.1.0b8/src/flattrs/cflattrs/encode.pyx`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/src/flattrs/cflattrs/number_types.c` & `flattrs-23.1.0b8/src/flattrs/cflattrs/number_types.c`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/src/flattrs/cflattrs/number_types.pyx` & `flattrs-23.1.0b8/src/flattrs/cflattrs/number_types.pyx`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/src/flattrs/converters.py` & `flattrs-23.1.0b8/src/flattrs/converters.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/src/flattrs/modgen/parser.py` & `flattrs-23.1.0b8/src/flattrs/modgen/parser.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/src/flattrs/modgen/renderer.py` & `flattrs-23.1.0b8/src/flattrs/modgen/renderer.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 from immutables import Map
 from lark import ParseTree, Token, Tree
 from lark.visitors import Interpreter
 
 from .._types import FieldName, Optionality
 from .parser import parser
 
+ImportableName: TypeAlias = str
+NamespacePrefix: TypeAlias = str
 Imports: TypeAlias = Mapping[str, Set[str]]
+UnresolvedImports: TypeAlias = Set[tuple[NamespacePrefix, ImportableName]]
 Script: TypeAlias = list[str]
-ImportableName: TypeAlias = str
 MISSING: Final = "$MISSING"
 
 
 @frozen
 class Attribute:
     name: str
     value: str | None = None
@@ -41,14 +43,15 @@
         namespace_prefix: str | None = None
         attrs: Sequence[Attribute] = field(factory=tuple, converter=tuple)
 
     name: ImportableName
     field_defs: Sequence[Field] = field(converter=tuple)
     imports: Imports = field(converter=Map)
     attrs: Sequence[Attribute] = field(converter=tuple)
+    unresolved_imports: UnresolvedImports = field(converter=frozenset)
 
     def adjust_enums(self, enums: set[str]) -> "Table":
         """
         Table fields that are enums must not be optional.
 
         Also, we adjust the default values for enums, if present.
 
@@ -187,42 +190,40 @@
 @frozen
 class Union:
     name: str
     members: Sequence[tuple[str, int | None]] = field(converter=tuple)
 
     def render(self) -> Script:
         member_names = []
-        to_resolve = set()
         if len(self.members) == 1:
             # Special case when there is only one union member.
             member_name, union_val = self.members[0]
-            to_resolve.add(member_name)
             if union_val is not None:
                 # This has a union tag attached.
                 member_name = f"Annotated[{member_name}, UnionVal({union_val})]"
             else:
                 member_name = f"Annotated[{member_name}, UnionVal(1)]"
             member_names.append(member_name)
         else:
             for member_name, union_val in self.members:
-                to_resolve.add(member_name)
                 if union_val is not None:
                     # This has a union tag attached.
                     member_name = f"Annotated[{member_name}, UnionVal({union_val})]"
                 member_names.append(member_name)
         member_string = " | ".join(member_names)
         return [f"{self.name} = {member_string}"]
 
 
 @define
 class Module:
     namespace: str | None
     path: Path
     imports: Imports
     importables: list[tuple[ImportableName, Union | Table | Enum | Attribute]]
+    unresolved_imports: UnresolvedImports
 
     def render(self) -> str:
         body = ""
         # We potentially need to reorder since unions must refer to existing
         # names.
         tables_to_indices = {}
         for ix, item in enumerate(self.importables):
@@ -281,55 +282,65 @@
             )
             + "\n"
             + body
         )
         return script
 
 
-class FlatbufferRenderer(Interpreter):
+class FlatbufferInterpreter(Interpreter):
     """Transform FlatBuffer code into Python code.
 
     The rendering needs to be done in several phases, since imports
     need to be resolved after the initial parsing pass and types
     may need to be adjusted based on the actual types.
     """
 
     def module(self, tree: ParseTree, filename: Path) -> Module:
         namespace = None
         for t in tree.find_data("namespace"):
             namespace = str(t.children[0])
         importables: list[
-            tuple[ImportableName, Script | Table | Enum | Attribute, Imports]
+            tuple[ImportableName, Union | Table | Enum | Attribute, Imports]
         ] = [
             self.visit(t)
             for t in tree.find_pred(
                 lambda t: t.data in ("table", "enum", "union", "attribute")
             )
         ]
         imports = {}
+        unresolved_imports = frozenset()
         res = []
 
         local_names = {i[0] for i in importables}
 
-        for name, script_or_table, imps in importables:
-            if isinstance(script_or_table, Attribute):
-                script_or_table = evolve(script_or_table, namespace=namespace)
-            res.append((name, script_or_table))
+        for name, importable, imps in importables:
+            if isinstance(importable, Attribute):
+                importable = evolve(importable, namespace=namespace)
+            res.append((name, importable))
             for k, v in imps.items():
-                if k == MISSING:
-                    for val in v:
-                        if val in local_names:
-                            continue
-                        imports.setdefault(k, set()).add(val)
-                else:
+                if k != MISSING:
                     if k not in imports:
                         imports[k] = set()
-                    imports[k] |= v
-
-        return Module(namespace, filename, imports, res)
+                    imports[k] |= v - local_names
+            if isinstance(importable, Union):
+                for k, v in imps.items():
+                    if k == MISSING:
+                        for val in v:
+                            if val in local_names:
+                                continue
+                            parts = val.rsplit(".", 1)
+                            if len(parts) == 1:
+                                unresolved_imports |= {("", val)}
+                            else:
+                                unresolved_imports |= {tuple(parts)}
+            if isinstance(importable, Table):
+                unresolved_imports |= {
+                    i for i in importable.unresolved_imports if i[1] not in local_names
+                }
+        return Module(namespace, filename, imports, res, unresolved_imports)
 
     def namespace(self, _: ParseTree) -> tuple[list[str], Imports]:
         return [], {}
 
     def attribute(self, tree: ParseTree) -> tuple[ImportableName, Attribute, Imports]:
         name = str(tree.children[0])
         return (name, Attribute(name), {})
@@ -339,27 +350,30 @@
         member_names = []
         to_resolve = set()
         imports = {}
         members = tree.children[1:]
         if len(members) == 1:
             # Special case when there is only one union member.
             member = members[0]
-            member_name = str(member.children[0]).split(".")[-1]
+            member_name = str(member.children[0])
             to_resolve.add(member_name)
+            member_name = member_name.split(".")[-1]
+
             imports["typing"] = {"Annotated"}
             imports["flattrs"] = {"UnionVal"}
             if len(member.children) > 1:
                 # This has a union tag attached.
                 member_names.append((member_name, int(member.children[1])))
             else:
                 member_names.append((member_name, None))
         else:
             for member in tree.children[1:]:
-                member_name = str(member.children[0]).split(".")[-1]
+                member_name = str(member.children[0])
                 to_resolve.add(member_name)
+                member_name = member_name.split(".")[-1]
                 if len(member.children) > 1:
                     # This has a union tag attached.
                     imports["typing"] = {"Annotated"}
                     imports["flattrs"] = {"UnionVal"}
                     member_names.append((member_name, int(member.children[1])))
                 else:
                     member_names.append((member_name, None))
@@ -401,46 +415,44 @@
             if isinstance(child, Tree) and child.data == "attributes":
                 table_attributes.extend(
                     Attribute(c, namespace=None if c in BUILTIN_ATTRS else MISSING)
                     for c in child.children
                 )
         field_defs = [self.table_field(c) for c in tree.find_data("table_field")]
         imports = Map()
-        for _, _, _, _, field_imports, _ in field_defs:
+        urs = set()
+        for _, _, _, _, field_imports, unresolved_imports, _ in field_defs:
             imports = merge_imports(imports, field_imports)
+            urs |= unresolved_imports
         fields = []
         for f in field_defs:
             is_optional = Attribute("required", namespace=None) not in f[3]
             fields.append(
                 Table.Field(
                     f[0],
                     f[1],
                     f[2],
                     is_optional,
-                    f[5] or None,
+                    f[6] or None,
                     f[3],
                 )
             )
 
-        table = Table(
-            name,
-            fields,
-            imports,
-            table_attributes,
-        )
+        table = Table(name, fields, imports, table_attributes, urs)
         return (
             name,
             table,
             imports,
         )
 
     def table_field(
         self, tree: ParseTree
-    ) -> tuple[FieldName, str, str, list[Attribute], Imports, str]:
+    ) -> tuple[FieldName, str, str, list[Attribute], Imports, UnresolvedImports, str]:
         imports = {}
+        unresolved_imports = set()
         name = str(tree.children[0])
         full_type = tree.children[1]
         attributes = []
         for attr_tree in tree.find_data("attributes"):
             for c in attr_tree.children:
                 attr_name = str(c)
                 if attr_name in BUILTIN_ATTRS:
@@ -455,15 +467,15 @@
             default = ""
         elif isinstance(full_type, Token):
             # This is a name, so probably a table field.
             default = ""
             namespace_prefix, type = (
                 full_type.rsplit(".", 1) if "." in full_type else ("", full_type)
             )
-            imports[MISSING] = imports.get(MISSING, frozenset()) | {str(type)}
+            unresolved_imports.add((namespace_prefix, type))
             for def_child in tree.find_data("table_field_default"):
                 default = str(def_child.children[0])
         else:
             if full_type.data == "vector_type":
                 inner_type = full_type.children[0]
                 if inner_type.lower() in ("uint8", "ubyte"):
                     type = "bytes"
@@ -474,17 +486,15 @@
                             imports["flattrs"] = {inner_type}
                     else:
                         namespace_prefix, inner_type = (
                             inner_type.rsplit(".", 1)
                             if "." in inner_type
                             else ("", inner_type)
                         )
-                        imports[MISSING] = imports.get(MISSING, frozenset()) | {
-                            str(inner_type)
-                        }
+                        unresolved_imports.add((namespace_prefix, str(inner_type)))
                     type = f"list[{inner_type}]"
                 default = ""
             elif full_type.data == "string":
                 pass
             else:
                 # A scalar.
                 attributes.append(Attribute("required", namespace=None))
@@ -501,49 +511,58 @@
                     if type == "bool":
                         def_val = def_val.capitalize()
                     elif not is_scalar:
                         # This has to be an enum
                         def_val = f"{type}.{def_val}"
                     default = def_val
 
-        return name, type, default, attributes, imports, namespace_prefix
+        return (
+            name,
+            type,
+            default,
+            attributes,
+            imports,
+            unresolved_imports,
+            namespace_prefix,
+        )
 
     def table_field_default(self):
         pass
 
 
 def parse_module(module_tree: Tree, file: Path) -> Module:
-    r = FlatbufferRenderer()
+    r = FlatbufferInterpreter()
     parsed_module = r.module(module_tree, file)
     return parsed_module
 
 
 def render_directory(
     input: Path, output: Path, gen_namespace_imports: bool = False
 ) -> None:
     """
     Render a directory of Flatbuffers into a directory of Python.
 
     """
     # First we parse, then we resolve imports, then we write.
     per_namespace: dict[str | None, list[Module]] = {}
-    importables_to_module: dict[str, Module] = {}
+    importables_to_module: dict[str, list[Module]] = {}
     namespace_to_attributes: dict[str, set[str]] = {}
     enums = set()
     modules: list[Module] = []
     for file in input.rglob("*.fbs"):
         rel_path = file.relative_to(input).with_suffix(".py")
         try:
             pm = parse_module(parser.parse(file.read_text()), rel_path)
         except Exception as exc:
             print(f"While parsing {file}: {exc}")
             print_exception(exc)
         modules.append(pm)
+        # Gather importables so we can resolve them later.
         for name, importable in pm.importables:
-            importables_to_module[name] = pm
+            importables_to_module.setdefault(name, []).append(pm)
             if isinstance(importable, Enum):
                 enums.add(importable.name)
             elif isinstance(importable, Attribute):
                 namespace_to_attributes.setdefault(pm.namespace or "", set()).add(
                     importable.name
                 )
         per_namespace.setdefault(pm.namespace, []).append(pm)
@@ -570,17 +589,29 @@
 
     # Now we write the modules to disk.
     output.mkdir(exist_ok=True, parents=True)
     (output / "__init__.py").write_text("")
     for pm_list in per_namespace.values():
         for pm in pm_list:
             pm_path = pm.path
-            missing_imports = pm.imports.pop(MISSING, set())
-            for importable in missing_imports:
-                module = importables_to_module[importable]
+            for ns, importable in pm.unresolved_imports:
+                for module in importables_to_module[importable]:
+                    if pm.namespace == module.namespace:
+                        # Referencing a symbol in the same namespace.
+                        break
+                    if not ns:
+                        if not module.namespace:
+                            break
+                    else:
+                        # A namespace is referenced.
+                        if module.namespace is not None:
+                            if module.namespace.endswith(ns):
+                                break
+                else:
+                    raise Exception(f"Cannot resolve {ns}.{importable} in {pm_path}")
 
                 if module.path.parent == pm_path.parent:
                     rel_path = f".{module.path.stem}"
                 else:
                     pm_parents = set(pm_path.parents)
                     target_parents = set(module.path.parents)
                     common_parent = sorted(
```

### Comparing `flattrs-23.1.0b7/src/flattrs/types.py` & `flattrs-23.1.0b8/src/flattrs/types.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/src/flattrs/typing.py` & `flattrs-23.1.0b8/src/flattrs/typing.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/src/flattrs.egg-info/SOURCES.txt` & `flattrs-23.1.0b8/src/flattrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/tests/test_misc.py` & `flattrs-23.1.0b8/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `flattrs-23.1.0b7/tests/test_modgen.py` & `flattrs-23.1.0b8/tests/test_modgen.py`

 * *Files identical despite different names*

