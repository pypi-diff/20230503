# Comparing `tmp/py_fumen_util-0.0.2.tar.gz` & `tmp/py_fumen_util-0.1.0.tar.gz`

## Comparing `py_fumen_util-0.0.2.tar` & `py_fumen_util-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/glue_fumen.py.old
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/src/py_fumen_util/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/src/py_fumen_util/__main__.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/src/py_fumen_util/fumen_combiner.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/src/py_fumen_util/fumen_locker.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/src/py_fumen_util/fumen_splitter.py
--rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/src/py_fumen_util/glue_fumen.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/src/py_fumen_util/mirror_fumen.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/src/py_fumen_util/remove_comment.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/src/py_fumen_util/unglue_fumen.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/LICENSE
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/README.md
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 py_fumen_util-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/__init__.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/__main__.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/fumen_combiner.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/fumen_locker.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/fumen_splitter.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/glue_fumen.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/grayout_all.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/grayout_last.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/mirror_fumen.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/remove_comment.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/src/py_fumen_util/unglue_fumen.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/LICENSE
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/README.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 py_fumen_util-0.1.0/PKG-INFO
```

### Comparing `py_fumen_util-0.0.2/src/py_fumen_util/__main__.py` & `py_fumen_util-0.1.0/src/py_fumen_util/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,73 @@
 # -*- coding:utf-8 -*-
 
 import sys
 
-import py_fumen
+from py_fumen_py import *
 from .fumen_combiner import fumen_combiner
 from .fumen_locker import fumen_locker
 from .fumen_splitter import fumen_splitter
 from .glue_fumen import glue_fumen
+from .grayout_all import grayout_all_fumen
+from .grayout_last import grayout_fumen
 from .mirror_fumen import mirror_fumen
 from .remove_comment import remove_comment
 from .unglue_fumen import unglue_fumen
 
 def usage(dummy_arg=None):
     return [
         'Usage:',
         'python3 -m py_fumen_util command fumen_code [fumen_code...]',
         'Commands (case-insensitive):',
         '    Combine:   Combine multiple Fumens into one',
-        '               Alias: Concat',
+        '               Alias: Concat, Join',
         '    Split:     Split each page into a Fumen',
         '',
         '    Glue:      Glue each Fumen page into tetromino placements',
         '               Alias: Decompile',
         '    Unglue:    Unglue Fumen placements into one page',
         '               Alias: Compile',
         '',
+        '    Gray:      Gray out the last page of each fumen',
+        '               Alias: Grey'
+        '    Grayall:   Gray out all pages of each fumen',
+        '               Alias: Greyall',
+        '',
         '    Lock:      Lock the last page of each Fumen and append a new page',
         '    Mirror:    Mirror Fumen pages',
         '               Alias: Flip',
         '    Uncomment: Uncomment Fumen pages',
     ]
 
 if __name__ == '__main__':
     if len(sys.argv) > 2:
         command = sys.argv[1].casefold()
         fumen_codes = ' '.join(sys.argv[2:]).split()
 
         command_function = {
             'combine': fumen_combiner,
             'concat' : fumen_combiner,
+            'join': fumen_combiner,
             'split': fumen_splitter,
             'glue': glue_fumen,
             'decompile': glue_fumen,
             'unglue': unglue_fumen,
             'compile': unglue_fumen,
+            'gray': grayout_fumen,
+            'grey': grayout_fumen,
+            'grayall': grayout_all_fumen,
+            'greyall': grayout_all_fumen,
             'lock': fumen_locker,
             'mirror': mirror_fumen,
             'flip': mirror_fumen,
             'uncomment': remove_comment,
         }.get(command, usage)
     else:
         command_function = usage
         fumen_codes = None
 
     try:
         for line in command_function(fumen_codes):
             print(line)
-    except py_fumen.decoder.VersionException as e:
+    except Exception as e:
         print(e)
         usage()
```

### Comparing `py_fumen_util-0.0.2/src/py_fumen_util/fumen_locker.py` & `py_fumen_util-0.1.0/src/py_fumen_util/grayout_last.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # -*- coding: utf-8 -*-
 
 import sys
 
-from py_fumen import encoder, decoder
-from py_fumen.page import Page, Flags
+from py_fumen_py import *
 
-def fumen_locker(fumen_codes):
-    locked_fumen = []
+def grayout_fumen(fumen_codes):
+    grayed_fumen = []
     for code in fumen_codes:
-        input_pages = decoder.decode(code)
-        input_pages.append(Page(flags=Flags(lock=True)))
-        locked_fumen.append(encoder.encode(input_pages))
-    return locked_fumen
+        input_pages = decode(code)
+        if input_pages[-1].field:
+            for line in input_pages[-1].field[:]:
+                for i, mino in enumerate(line):
+                    if mino.is_colored():
+                        line[i] = Mino.X
+        grayed_fumen.append(encode(input_pages))
+    return grayed_fumen
 
 if __name__ == '__main__':
     if len(sys.argv) > 1:
-        for line in fumen_locker(' '.join(sys.argv[1:]).split()):
+        for line in grayout_fumen(' '.join(sys.argv[1:]).split()):
             print(line)
+
```

### Comparing `py_fumen_util-0.0.2/src/py_fumen_util/fumen_splitter.py` & `py_fumen_util-0.1.0/src/py_fumen_util/fumen_splitter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
 import sys
 
-from py_fumen import encoder, decoder
+from py_fumen_py import *
 
 def fumen_splitter(fumen_codes):
     split_fumen = []
     for code in fumen_codes:
-        input_pages = decoder.decode(code)
+        input_pages = decode(code)
         for page in input_pages:
             if input_pages[0].flags.colorize:
                 page.flags.colorize = True
-            split_fumen.append(encoder.encode([page]))
+            split_fumen.append(encode([page]))
     return split_fumen
 
 if __name__ == '__main__':
     if len(sys.argv) > 1:
         for line in fumen_splitter(' '.join(sys.argv[1:]).split()):
             print(line)
```

### Comparing `py_fumen_util-0.0.2/src/py_fumen_util/glue_fumen.py` & `py_fumen_util-0.1.0/src/py_fumen_util/glue_fumen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,73 @@
 # -*- coding: utf-8 -*-
 
-import re
 import sys
 
-from py_fumen.constants import FieldConstants
-from py_fumen import encoder, decoder
-from py_fumen.field import Field, Operation
-from py_fumen.page import Page, Flags
-
-MINOS = 'TILJSZO'
-LINECLEAR = 'X' * FieldConstants.WIDTH
+from py_fumen_py import *
 
 PIECE_MAPPINGS = {
-    'T': [
-        [[0, -1], [0, 0], [-1, -1], [1, -1]],
-        [[0, -1], [0, 0], [-1, -1], [0, -2]],
-        [[1, 0], [0, 0], [2, 0], [1, -1]],
-        [[0, -1], [0, 0], [1, -1], [0, -2]],
-    ],
-    'I': [
+    Mino.I: [
         [[1, 0], [0, 0], [2, 0], [3, 0]],
         [[0, -2], [0, 0], [0, -1], [0, -3]],
     ],
-    'L': [
+    Mino.L: [
         [[-1, -1], [0, 0], [-2, -1], [0, -1]],
         [[1, -1], [0, 0], [1, 0], [1, -2]],
         [[1, 0], [0, 0], [2, 0], [0, -1]],
         [[0, -1], [0, 0], [0, -2], [1, -2]],
     ],
-    'J': [
+    Mino.O: [
+        [[0, -1], [0, 0], [1, 0], [1, -1]],
+    ],
+    Mino.Z: [
+        [[1, -1], [0, 0], [1, 0], [2, -1]],
+        [[0, -1], [0, 0], [-1, -1], [-1, -2]],
+    ],
+    Mino.T: [
+        [[0, -1], [0, 0], [-1, -1], [1, -1]],
+        [[0, -1], [0, 0], [-1, -1], [0, -2]],
+        [[1, 0], [0, 0], [2, 0], [1, -1]],
+        [[0, -1], [0, 0], [1, -1], [0, -2]],
+    ],
+    Mino.J: [
         [[1, -1], [0, 0], [0, -1], [2, -1]],
         [[0, -1], [0, 0], [-1, -2], [0, -2]],
         [[1, 0], [0, 0], [2, 0], [2, -1]],
         [[0, -1], [0, 0], [1, 0], [0, -2]],
     ],
-    'S': [
+    Mino.S: [
         [[0, -1], [0, 0], [1, 0], [-1, -1]],
         [[1, -1], [0, 0], [0, -1], [1, -2]],
     ],
-    'Z': [
-        [[1, -1], [0, 0], [1, 0], [2, -1]],
-        [[0, -1], [0, 0], [-1, -1], [-1, -2]],
-    ],
-    'O': [
-        [[0, -1], [0, 0], [1, 0], [1, -1]],
-    ],
-}
-
-ROTATION_DICT = {
-    0: 'spawn',
-    1: 'left',
-    2: 'reverse',
-    3: 'right',
 }
 
-def height(field):
-    return len(field.string().splitlines()[:-FieldConstants.GARBAGE_LINE])
-
 def is_inside(field, x, y):
-    return 0 <= x < FieldConstants.WIDTH and 0 <= y < height(field)
+    return 0 <= x < FieldConstants.WIDTH and 0 <= y < field.height()
 
 def place_piece(field, mino_positions):
-    new_field = field.copy()
     for x, y in mino_positions:
-        new_field.set(x, y, 'X')
-    return new_field
+        field.fill(x, y, Mino.X)
 
 def remove_line_clears(field):
     lines = []
     n_lineclear = 0
-    for line in field.string().splitlines()[:-FieldConstants.GARBAGE_LINE]:
-        if line == LINECLEAR:
+    for line in field:
+        if all(mino is Mino.X for mino in line):
             n_lineclear += 1
         else:
             lines.append(line)
-    return Field.create(
-        ''.join(lines),
-        field.string().splitlines()[-FieldConstants.GARBAGE_LINE:]
-    ), n_lineclear
+    return Field(field=lines, garbage=field[:0]), n_lineclear
 
 def find_remaining_pieces(field):
-    return [p for p in MINOS if p in ''.join(
-        field.string().splitlines()[:-FieldConstants.GARBAGE_LINE]
-    )]
+    remaining = set()
+    for line in field:
+        for mino in line:
+            if mino.is_colored():
+                remaining.add(mino)
+    return remaining
 
 def check_rotation(x, y, field, pieces_arr, all_pieces_arr):
     piece = field.at(x, y)
     found = False
     leftover_pieces = None
 
     for state, piece_shape in enumerate(PIECE_MAPPINGS[piece]):
@@ -96,23 +77,23 @@
             if not is_inside(field, px, py) or field.at(px, py) != piece:
                 break
         else:
             found_before = found
             found = True
             new_piece_arr = pieces_arr[:]
             new_piece_arr.append(
-                Operation(piece_type=piece, rotation=ROTATION_DICT[state],
+                Operation(mino=piece, rotation=Rotation(state).shifted(2),
                           x=mino_positions[0][0], y=mino_positions[0][1])
             )
 
-            new_field, n_lineclear = remove_line_clears(
-                    place_piece(field, mino_positions)
-            )
+            new_field = field.copy()
+            place_piece(new_field, mino_positions)
+            new_field, n_lineclear = remove_line_clears(new_field)
 
-            x0, y0 = (0, height(new_field)-1) if n_lineclear else (x, y)
+            x0, y0 = (0, new_field.height()-1) if n_lineclear else (x, y)
 
             old_len = len(all_pieces_arr)
             poss_piece_arr, leftover_pieces = scan_field(
                 x0, y0, new_field, new_piece_arr, all_pieces_arr
             )
 
             if leftover_pieces is None:
@@ -126,56 +107,54 @@
                 else:
                     found = found_before
     return found, leftover_pieces
 
 def scan_field(x0, y0, field, pieces_arr, all_pieces_arr):
     for y in range(y0, -1, -1):
         for x in range(x0 if y == y0 else 0, FieldConstants.WIDTH):
-            if field.at(x, y) != 'X' and field.at(x, y) != '_':
+            if field.at(x, y).is_colored():
                 rotation_worked, leftover = check_rotation(
                     x, y, field, pieces_arr, all_pieces_arr
                 )
                 if rotation_worked:
                     return None, leftover
     return pieces_arr, None
 
 def make_empty_field(field):
-    field_string = field.string()
-    for mino in MINOS:
-        if mino in field_string:
-            field_string = field_string.replace(mino, '_')
-    return Field.create(
-        ''.join(field_string.splitlines()[:-FieldConstants.GARBAGE_LINE]),
-        ''.join(field_string.splitlines()[-FieldConstants.GARBAGE_LINE:])
-    )
+    field = field.copy()
+    for line in field:
+        for i, mino in enumerate(line):
+            if mino.is_colored():
+                line[i] = Mino._
+    return field
 
 def glue_fumen(fumen_codes):
     all_pieces_arr = []
     all_fumens = []
     fumen_issues = 0
 
     for code in fumen_codes:
-        input_pages = decoder.decode(code)
+        input_pages = decode(code)
         this_glue_fumens = []
         for page in input_pages:
-            field, n_lineclear = remove_line_clears(page.get_field())
+            field, n_lineclear = remove_line_clears(page.field.copy())
             empty_field = make_empty_field(field)
             all_pieces_arr.clear()
 
-            scan_field(0, height(field) - 1, field, [], all_pieces_arr)
+            scan_field(0, field.height()-1, field, [], all_pieces_arr)
 
             if not all_pieces_arr:
                 print(code, "couldn't be glued")
                 fumen_issues += 1
 
             for pieces_arr in all_pieces_arr:
                 pages = [Page(field=empty_field, operation=pieces_arr[0])]
                 for operation in pieces_arr[1:]:
                     pages.append(Page(operation=operation))
-                this_glue_fumens.append(encoder.encode(pages))
+                this_glue_fumens.append(encode(pages))
 
             if len(all_pieces_arr) > 1:
                 all_fumens.append(
                     'Warning: {} led to {} outputs: {}'.format(
                         code, len(all_pieces_arr), ' '.join(this_glue_fumens)
                     )
                 )
```

### Comparing `py_fumen_util-0.0.2/src/py_fumen_util/remove_comment.py` & `py_fumen_util-0.1.0/src/py_fumen_util/grayout_all.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # -*- coding: utf-8 -*-
 
 import sys
 
-from py_fumen import encoder, decoder
+from py_fumen_py import *
 
-def remove_comment(fumen_codes):
-    output_codes = []
+def grayout_all_fumen(fumen_codes):
+    grayed_fumen = []
     for code in fumen_codes:
-        input_pages = decoder.decode(code)
+        input_pages = decode(code)
         for page in input_pages:
-            page.comment = ''
-            page.flags.quiz = False
-        output_codes.append(encoder.encode(input_pages))
-    return output_codes
+            if page.field:
+                for line in page.field[:]:
+                    for i, mino in enumerate(line):
+                        if mino.is_colored():
+                            line[i] = Mino.X
+        grayed_fumen.append(encode(input_pages))
+    return grayed_fumen
 
 if __name__ == '__main__':
     if len(sys.argv) > 1:
-        for line in remove_comment(' '.join(sys.argv[1:]).split()):
+        for line in grayout_all_fumen(' '.join(sys.argv[1:]).split()):
             print(line)
```

### Comparing `py_fumen_util-0.0.2/.gitignore` & `py_fumen_util-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `py_fumen_util-0.0.2/LICENSE` & `py_fumen_util-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_fumen_util-0.0.2/pyproject.toml` & `py_fumen_util-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py_fumen_util"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
 	{ name="Octupus Tea" },
 ]
 description = "Python implementation of the JavaScript package 'FumenUtil'"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
 	"Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependecies = [
-	"py-fumen >= 0.1.0",
+	"py-fumen-py >= 0.0.4",
 ]
 
 [project.urls]
 "Source" = "https://github.com/OctupusTea/py-fumen-util"
```

