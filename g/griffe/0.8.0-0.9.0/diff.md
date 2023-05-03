# Comparing `tmp/griffe-0.8.0.tar.gz` & `tmp/griffe-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griffe-0.8.0.tar", last modified: Sun Jan  2 13:57:19 2022, max compression
+gzip compressed data, was "griffe-0.9.0.tar", last modified: Tue Jan  4 17:32:37 2022, max compression
```

## Comparing `griffe-0.8.0.tar` & `griffe-0.9.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0 pawamoy   (1000) users      (985)      754 2021-09-25 13:37:21.496997 griffe-0.8.0/LICENSE
--rw-r--r--   0 pawamoy   (1000) users      (985)     4592 2022-01-02 13:54:12.526392 griffe-0.8.0/README.md
--rw-r--r--   0 pawamoy   (1000) users      (985)     2983 2021-12-31 15:31:40.883103 griffe-0.8.0/pyproject.toml
--rw-r--r--   0 pawamoy   (1000) users      (985)      196 2021-12-31 15:23:38.810180 griffe-0.8.0/src/griffe/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      338 2021-11-16 11:29:47.822825 griffe-0.8.0/src/griffe/__main__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)       80 2021-11-26 18:46:47.020408 griffe-0.8.0/src/griffe/agents/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     1331 2021-11-25 23:43:02.327998 griffe-0.8.0/src/griffe/agents/base.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      280 2021-11-28 10:26:11.869311 griffe-0.8.0/src/griffe/agents/extensions/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     8535 2022-01-01 18:39:01.413506 griffe-0.8.0/src/griffe/agents/extensions/base.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     2686 2021-12-31 12:13:29.253201 griffe-0.8.0/src/griffe/agents/extensions/hybrid.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    12648 2022-01-01 17:02:32.530040 griffe-0.8.0/src/griffe/agents/inspector.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    33541 2021-12-31 17:32:47.783062 griffe-0.8.0/src/griffe/agents/nodes.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    18145 2022-01-01 18:40:49.671906 griffe-0.8.0/src/griffe/agents/visitor.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     7460 2022-01-02 11:30:35.898994 griffe-0.8.0/src/griffe/cli.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     1938 2021-12-20 20:50:58.389063 griffe-0.8.0/src/griffe/collections.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    34718 2022-01-01 16:14:11.422500 griffe-0.8.0/src/griffe/dataclasses.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      173 2021-11-20 21:50:56.698101 griffe-0.8.0/src/griffe/docstrings/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     5642 2021-11-22 21:55:51.562764 griffe-0.8.0/src/griffe/docstrings/dataclasses.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    23222 2021-12-20 12:41:45.657584 griffe-0.8.0/src/griffe/docstrings/google.py
--rw-r--r--   0 pawamoy   (1000) users      (985)       99 2021-09-25 13:37:21.496997 griffe-0.8.0/src/griffe/docstrings/markdown.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    17213 2021-11-22 22:20:29.447402 griffe-0.8.0/src/griffe/docstrings/numpy.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     1499 2021-11-22 22:01:38.507678 griffe-0.8.0/src/griffe/docstrings/parsers.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    16357 2022-01-02 13:54:36.489367 griffe-0.8.0/src/griffe/docstrings/rst.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     1152 2021-11-21 19:52:02.876063 griffe-0.8.0/src/griffe/docstrings/utils.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     3859 2021-11-21 20:50:23.963272 griffe-0.8.0/src/griffe/encoders.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     1424 2022-01-01 18:22:07.651154 griffe-0.8.0/src/griffe/exceptions.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     3911 2021-12-27 18:58:27.494283 griffe-0.8.0/src/griffe/expressions.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      586 2021-12-31 11:42:46.249192 griffe-0.8.0/src/griffe/importer.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    25499 2022-01-01 18:22:07.927817 griffe-0.8.0/src/griffe/loader.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     2097 2021-12-31 13:34:59.394873 griffe-0.8.0/src/griffe/logger.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     4517 2021-12-31 16:34:37.554495 griffe-0.8.0/src/griffe/mixins.py
--rw-r--r--   0 pawamoy   (1000) users      (985)        0 2021-09-25 13:37:21.496997 griffe-0.8.0/src/griffe/py.typed
--rw-r--r--   0 pawamoy   (1000) users      (985)       37 2021-12-31 17:34:59.204171 griffe-0.8.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0 pawamoy   (1000) users      (985)      194 2021-12-31 17:34:59.204171 griffe-0.8.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 pawamoy   (1000) users      (985)      295 2021-12-31 17:34:59.204171 griffe-0.8.0/tests/.pytest_cache/README.md
--rw-r--r--   0 pawamoy   (1000) users      (985)        2 2022-01-01 19:13:36.412554 griffe-0.8.0/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 pawamoy   (1000) users      (985)     8927 2022-01-02 13:56:03.778065 griffe-0.8.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 pawamoy   (1000) users      (985)        2 2022-01-02 13:56:03.778065 griffe-0.8.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 pawamoy   (1000) users      (985)       10 2022-01-02 13:56:02.784747 griffe-0.8.0/tests/.pytest_cache/v/randomly_seed
--rw-r--r--   0 pawamoy   (1000) users      (985)      159 2021-09-25 13:37:21.496997 griffe-0.8.0/tests/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)       47 2021-09-25 13:37:21.496997 griffe-0.8.0/tests/conftest.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      823 2021-11-03 19:10:40.226000 griffe-0.8.0/tests/fixtures/functions/parameters.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      428 2021-12-31 15:23:38.810180 griffe-0.8.0/tests/test_cli.py
--rw-r--r--   0 pawamoy   (1000) users      (985)       28 2021-09-29 20:04:50.003107 griffe-0.8.0/tests/test_docstrings/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     2737 2021-11-21 20:41:08.313361 griffe-0.8.0/tests/test_docstrings/helpers.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    18436 2021-11-26 18:35:15.082957 griffe-0.8.0/tests/test_docstrings/test_google.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     7909 2021-11-26 18:47:00.940168 griffe-0.8.0/tests/test_docstrings/test_numpy.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    23599 2022-01-01 19:12:53.319867 griffe-0.8.0/tests/test_docstrings/test_rst.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     6516 2021-12-20 18:46:46.715194 griffe-0.8.0/tests/test_functions.py
--rw-------   0 pawamoy   (1000) users      (985)     7237 2022-01-02 13:57:19.796931 griffe-0.8.0/PKG-INFO
+-rw-r--r--   0 pawamoy   (1000) users      (985)      754 2021-09-25 13:37:21.496997 griffe-0.9.0/LICENSE
+-rw-r--r--   0 pawamoy   (1000) users      (985)     4592 2022-01-02 13:54:12.526392 griffe-0.9.0/README.md
+-rw-r--r--   0 pawamoy   (1000) users      (985)     2983 2022-01-04 17:16:42.589013 griffe-0.9.0/pyproject.toml
+-rw-r--r--   0 pawamoy   (1000) users      (985)      196 2021-12-31 15:23:38.810180 griffe-0.9.0/src/griffe/__init__.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)      338 2021-11-16 11:29:47.822825 griffe-0.9.0/src/griffe/__main__.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)       80 2021-11-26 18:46:47.020408 griffe-0.9.0/src/griffe/agents/__init__.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     1119 2022-01-02 17:58:14.070449 griffe-0.9.0/src/griffe/agents/base.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)      424 2022-01-02 21:06:34.014075 griffe-0.9.0/src/griffe/agents/extensions/__init__.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     8535 2022-01-01 18:39:01.413506 griffe-0.9.0/src/griffe/agents/extensions/base.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     2686 2021-12-31 12:13:29.253201 griffe-0.9.0/src/griffe/agents/extensions/hybrid.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)    15143 2022-01-04 12:22:27.256380 griffe-0.9.0/src/griffe/agents/inspector.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)    34325 2022-01-04 13:02:04.703431 griffe-0.9.0/src/griffe/agents/nodes.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)    18505 2022-01-02 17:56:59.794837 griffe-0.9.0/src/griffe/agents/visitor.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     6525 2022-01-04 17:18:41.393875 griffe-0.9.0/src/griffe/cli.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     1938 2021-12-20 20:50:58.389063 griffe-0.9.0/src/griffe/collections.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)    35550 2022-01-04 17:02:07.859043 griffe-0.9.0/src/griffe/dataclasses.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)      173 2021-11-20 21:50:56.698101 griffe-0.9.0/src/griffe/docstrings/__init__.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     5642 2021-11-22 21:55:51.562764 griffe-0.9.0/src/griffe/docstrings/dataclasses.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)    23473 2022-01-02 22:28:25.415852 griffe-0.9.0/src/griffe/docstrings/google.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)       99 2021-09-25 13:37:21.496997 griffe-0.9.0/src/griffe/docstrings/markdown.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)    17213 2021-11-22 22:20:29.447402 griffe-0.9.0/src/griffe/docstrings/numpy.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     1499 2021-11-22 22:01:38.507678 griffe-0.9.0/src/griffe/docstrings/parsers.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)    16357 2022-01-02 13:54:36.489367 griffe-0.9.0/src/griffe/docstrings/rst.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     1152 2021-11-21 19:52:02.876063 griffe-0.9.0/src/griffe/docstrings/utils.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     3861 2022-01-02 22:22:34.857658 griffe-0.9.0/src/griffe/encoders.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     1873 2022-01-03 22:11:57.255776 griffe-0.9.0/src/griffe/exceptions.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     4068 2022-01-03 17:28:38.808468 griffe-0.9.0/src/griffe/expressions.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)      791 2022-01-02 17:56:33.225214 griffe-0.9.0/src/griffe/importer.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)    23438 2022-01-04 17:18:19.987534 griffe-0.9.0/src/griffe/loader.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     2094 2022-01-02 21:14:30.583849 griffe-0.9.0/src/griffe/logger.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     4517 2021-12-31 16:34:37.554495 griffe-0.9.0/src/griffe/mixins.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)        0 2021-09-25 13:37:21.496997 griffe-0.9.0/src/griffe/py.typed
+-rw-r--r--   0 pawamoy   (1000) users      (985)       37 2021-12-31 17:34:59.204171 griffe-0.9.0/tests/.pytest_cache/.gitignore
+-rw-r--r--   0 pawamoy   (1000) users      (985)      194 2021-12-31 17:34:59.204171 griffe-0.9.0/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 pawamoy   (1000) users      (985)      295 2021-12-31 17:34:59.204171 griffe-0.9.0/tests/.pytest_cache/README.md
+-rw-r--r--   0 pawamoy   (1000) users      (985)      317 2022-01-04 17:13:48.548326 griffe-0.9.0/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 pawamoy   (1000) users      (985)     9239 2022-01-04 17:31:29.942222 griffe-0.9.0/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 pawamoy   (1000) users      (985)        2 2022-01-04 17:31:29.942222 griffe-0.9.0/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 pawamoy   (1000) users      (985)       10 2022-01-04 17:31:28.985570 griffe-0.9.0/tests/.pytest_cache/v/randomly_seed
+-rw-r--r--   0 pawamoy   (1000) users      (985)      159 2021-09-25 13:37:21.496997 griffe-0.9.0/tests/__init__.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)       47 2022-01-03 17:32:45.588049 griffe-0.9.0/tests/conftest.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)      823 2021-11-03 19:10:40.226000 griffe-0.9.0/tests/fixtures/functions/parameters.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     1267 2022-01-03 18:40:58.735692 griffe-0.9.0/tests/helpers.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)      443 2022-01-04 17:13:02.149032 griffe-0.9.0/tests/test_cli.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)       28 2021-09-29 20:04:50.003107 griffe-0.9.0/tests/test_docstrings/__init__.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     2763 2022-01-03 18:39:26.737050 griffe-0.9.0/tests/test_docstrings/helpers.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)    19458 2022-01-02 22:30:52.450370 griffe-0.9.0/tests/test_docstrings/test_google.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     7909 2021-11-26 18:47:00.940168 griffe-0.9.0/tests/test_docstrings/test_numpy.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)    23599 2022-01-01 19:12:53.319867 griffe-0.9.0/tests/test_docstrings/test_rst.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)     6516 2021-12-20 18:46:46.715194 griffe-0.9.0/tests/test_functions.py
+-rw-r--r--   0 pawamoy   (1000) users      (985)      955 2022-01-03 18:22:57.754971 griffe-0.9.0/tests/test_inspector.py
+-rw-------   0 pawamoy   (1000) users      (985)     7237 2022-01-04 17:32:37.654529 griffe-0.9.0/PKG-INFO
```

### Comparing `griffe-0.8.0/LICENSE` & `griffe-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/README.md` & `griffe-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/pyproject.toml` & `griffe-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = "Signatures for entire Python programs. Extract the structure, the frame, the skeleton of your project, to generate API documentation or find breaking changes in your API."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = []
 dynamic = []
 classifiers = [ "Development Status :: 4 - Beta", "Intended Audience :: Developers", "License :: OSI Approved :: ISC License (ISCL)", "Programming Language :: Python", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3 :: Only", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3.10", "Programming Language :: Python :: 3.11", "Topic :: Documentation", "Topic :: Software Development", "Topic :: Software Development :: Documentation", "Topic :: Utilities", "Typing :: Typed",]
 dependencies = [ "cached_property; python_version < '3.8'",]
-version = "0.8.0"
+version = "0.9.0"
 [[project.authors]]
 name = "Timothée Mazzucotelli"
 email = "pawamoy@pm.me"
 
 [project.license]
 file = "LICENSE"
```

### Comparing `griffe-0.8.0/src/griffe/agents/extensions/base.py` & `griffe-0.9.0/src/griffe/agents/extensions/base.py`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/src/griffe/agents/extensions/hybrid.py` & `griffe-0.9.0/src/griffe/agents/extensions/hybrid.py`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/src/griffe/agents/inspector.py` & `griffe-0.9.0/src/griffe/agents/inspector.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,26 +18,38 @@
 The inspection agent works similarly to the regular "node visitor" agent,
 in that it maintains a state with the current object being handled,
 and recursively handle its members.
 """
 
 from __future__ import annotations
 
+import ast
+import sys
 from inspect import Parameter as SignatureParameter
-from inspect import Signature, getdoc
+from inspect import Signature, getdoc, getmodule
 from inspect import signature as getsignature
 from pathlib import Path
 from tokenize import TokenError
 from typing import Any
 
 from griffe.agents.base import BaseInspector
 from griffe.agents.extensions import Extensions
 from griffe.agents.nodes import ObjectKind, ObjectNode, get_annotation
 from griffe.collections import LinesCollection
-from griffe.dataclasses import Attribute, Class, Docstring, Function, Module, Parameter, ParameterKind, Parameters
+from griffe.dataclasses import (
+    Alias,
+    Attribute,
+    Class,
+    Docstring,
+    Function,
+    Module,
+    Parameter,
+    ParameterKind,
+    Parameters,
+)
 from griffe.docstrings.parsers import Parser
 from griffe.expressions import Expression, Name
 from griffe.importer import dynamic_import
 
 empty = Signature.empty
 
 
@@ -72,14 +84,28 @@
         parent,
         docstring_parser=docstring_parser,
         docstring_options=docstring_options,
         lines_collection=lines_collection,
     ).get_module()
 
 
+def _force_inspect(parent_module, child_module):
+    # Special case for builtin modules, example:
+    # - `ast` does `from _ast import *`
+    # - so we go and inspect `_ast`
+    # - when iterating on its child, as usual, we check each child's real module
+    #   thanks to `inspect.getmodule`
+    # - but in that case, `inspect.getmodule` returns `ast` for the children
+    # - it puts us in a cycle
+    # - so we break the cycle by ignoring inspect's result and inspecting the private module
+    if parent_module.startswith("_"):
+        return parent_module[1:] == child_module and parent_module in sys.builtin_module_names
+    return False
+
+
 class Inspector(BaseInspector):  # noqa: WPS338
     """This class is used to instantiate an inspector.
 
     Inspectors iterate on objects members to extract data from them.
     """
 
     def __init__(
@@ -155,15 +181,34 @@
         """Extend the base generic inspection with extensions.
 
         Parameters:
             node: The node to inspect.
         """
         for before_inspector in self.extensions.before_children_inspection:
             before_inspector.inspect(node)
-        super().generic_inspect(node)
+
+        for child in node.children:
+            child_module = getmodule(child.obj)
+            child_module_path = getattr(child_module, "__name__", None)
+
+            use_alias = (
+                child_module_path
+                and child_module_path != self.current.module.path
+                and not _force_inspect(node.name, child_module_path)
+            )
+            if use_alias:
+                if child_module is child.obj:
+                    target_path: str = child_module_path  # type: ignore[assignment]
+                else:
+                    child_name = getattr(child.obj, "__name__", child.name)
+                    target_path = f"{child_module_path}.{child_name}"
+                self.current[child.name] = Alias(child.name, target_path)
+            else:
+                self.inspect(child)
+
         for after_inspector in self.extensions.after_children_inspection:
             after_inspector.inspect(node)
 
     def inspect_module(self, node: ObjectNode) -> None:
         """Inspect a module.
 
         Parameters:
@@ -281,24 +326,26 @@
 
         Parameters:
             node: The node to inspect.
             labels: Labels to add to the data object.
         """
         try:
             signature = getsignature(node.obj)
-        except (ValueError, TokenError, TypeError):
+        except (AttributeError, ValueError, TokenError, TypeError):
             parameters = None
             returns = None
         else:
-            parameters = Parameters(*[_convert_parameter(parameter) for parameter in signature.parameters.values()])
+            parameters = Parameters(
+                *[_convert_parameter(parameter, parent=self.current) for parameter in signature.parameters.values()]
+            )
             return_annotation = signature.return_annotation
             if return_annotation is empty:
                 returns = None
             else:
-                returns = return_annotation and get_annotation(return_annotation, parent=self.current)
+                returns = _convert_object_to_annotation(return_annotation, parent=self.current)
 
         function = Function(
             name=node.name,
             parameters=parameters,
             returns=returns,
             docstring=self._get_docstring(node),
         )
@@ -331,15 +378,18 @@
             labels.add("class")
         elif parent.kind is ObjectKind.FUNCTION:
             if parent.name != "__init__":
                 return
             parent = parent.parent
             labels.add("instance")
 
-        value = repr(node.obj)
+        try:
+            value = repr(node.obj)
+        except Exception:  # could trigger anything
+            value = None
         docstring = self._get_docstring(node)
 
         attribute = Attribute(
             name=node.name,
             value=value,
             annotation=annotation,
             # lineno=node.lineno,
@@ -358,19 +408,39 @@
     SignatureParameter.POSITIONAL_OR_KEYWORD: ParameterKind.positional_or_keyword,
     SignatureParameter.VAR_POSITIONAL: ParameterKind.var_positional,
     SignatureParameter.KEYWORD_ONLY: ParameterKind.keyword_only,
     SignatureParameter.VAR_KEYWORD: ParameterKind.var_keyword,
 }
 
 
-def _convert_parameter(parameter):
+def _convert_parameter(parameter, parent):
     name = parameter.name
     if parameter.annotation is empty:
         annotation = None
     else:
-        annotation = parameter.annotation
+        annotation = _convert_object_to_annotation(parameter.annotation, parent=parent)
     kind = _kind_map[parameter.kind]
     if parameter.default is empty:
         default = None
     else:
-        default = parameter.default
+        default = repr(parameter.default)
     return Parameter(name, annotation=annotation, kind=kind, default=default)
+
+
+def _convert_object_to_annotation(obj, parent):
+    # even when *we* import future annotations,
+    # the object from which we get a signature
+    # can come from modules which did *not* import them,
+    # so inspect.signature returns actual Python objects
+    # that we must deal with
+    if not isinstance(obj, str):
+        if hasattr(obj, "__name__"):
+            # simple types like int, str, custom classes, etc.
+            obj = obj.__name__
+        else:
+            # other, more complex types: hope for the best
+            obj = repr(obj)
+    try:
+        annotation_node = compile(obj, mode="eval", filename="<>", flags=ast.PyCF_ONLY_AST, optimize=2)
+    except SyntaxError:
+        return obj
+    return get_annotation(annotation_node.body, parent=parent)
```

### Comparing `griffe-0.8.0/src/griffe/agents/nodes.py` & `griffe-0.9.0/src/griffe/agents/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This module contains utilities for extracting information from AST nodes."""
+"""This module contains utilities for extracting information from nodes."""
 
 from __future__ import annotations
 
 import enum
 import inspect
 import sys
 from ast import AST
@@ -59,14 +59,15 @@
 from ast import Str as NodeStr
 from ast import Sub as NodeSub
 from ast import Subscript as NodeSubscript
 from ast import Tuple as NodeTuple
 from ast import UAdd as NodeUAdd
 from ast import UnaryOp as NodeUnaryOp
 from ast import USub as NodeUSub
+from ast import Yield as NodeYield
 from ast import arguments as NodeArguments
 from ast import comprehension as NodeComprehension
 from ast import keyword as NodeKeyword
 from functools import partial
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Sequence, Type
 
@@ -270,14 +271,17 @@
 
     Attributes:
         obj: The actual Python object.
         name: The Python object's name.
         parent: The parent node.
     """
 
+    # low level stuff known to cause issues when resolving aliases
+    exclude_specials = {"__builtins__", "__loader__", "__spec__"}
+
     def __init__(self, obj: Any, name: str, parent: ObjectNode | None = None) -> None:
         """
         Initialize the object.
 
         Arguments:
             obj: A Python object.
             name: The object's name.
@@ -337,15 +341,15 @@
         """Build and return the children of this node.
 
         Returns:
             A list of children.
         """
         children = []
         for name, member in inspect.getmembers(self.obj):
-            if self._pick_member(member):
+            if self._pick_member(name, member):
                 children.append(ObjectNode(member, name, parent=self))
         return children
 
     @cached_property
     def is_module(self) -> bool:
         """
         Tell if this node's object is a module.
@@ -463,15 +467,15 @@
     def is_staticmethod(self) -> bool:
         """
         Tell if this node's object is a staticmethod.
 
         Returns:
             If this node's object is a staticmethod.
         """
-        if not self.parent:
+        if self.parent is None:
             return False
         try:
             self_from_parent = self.parent.obj.__dict__.get(self.name, None)  # noqa: WPS609
         except AttributeError:
             return False
         return self.parent_is_class and isinstance(self_from_parent, staticmethod)
 
@@ -479,30 +483,35 @@
     def is_classmethod(self) -> bool:
         """
         Tell if this node's object is a classmethod.
 
         Returns:
             If this node's object is a classmethod.
         """
-        if not self.parent:
+        if self.parent is None:
             return False
         try:
             self_from_parent = self.parent.obj.__dict__.get(self.name, None)  # noqa: WPS609
         except AttributeError:
             return False
         return self.parent_is_class and isinstance(self_from_parent, classmethod)
 
     @cached_property
     def _ids(self) -> set[int]:
         if self.parent is None:
-            return {id(self)}
-        return {id(self)} | self.parent._ids  # noqa: WPS437
+            return {id(self.obj)}
+        return {id(self.obj)} | self.parent._ids  # noqa: WPS437
 
-    def _pick_member(self, member: Any) -> bool:
-        return member is not type and member is not object and id(member) not in self._ids
+    def _pick_member(self, name: str, member: Any) -> bool:
+        return (
+            name not in self.exclude_specials
+            and member is not type
+            and member is not object
+            and id(member) not in self._ids
+        )
 
 
 def _join(sequence, item):
     if not sequence:
         return []
     new_sequence = [sequence[0]]
     for element in sequence[1:]:
@@ -771,14 +780,18 @@
     return value
 
 
 def _get_constant_value(node: NodeConstant) -> str:
     return repr(node.value)
 
 
+def _get_constant_value_no_repr(node: NodeConstant) -> str:
+    return node.value
+
+
 def _get_dict_value(node: NodeDict) -> str:
     pairs = zip(node.keys, node.values)
     gen = (f"{'None' if key is None else get_value(key)}: {get_value(value)}" for key, value in pairs)  # noqa: WPS509
     return "{" + ", ".join(gen) + "}"
 
 
 def _get_dictcomp_value(node: NodeDictComp) -> str:
@@ -839,15 +852,18 @@
 
 
 def _get_isnot_value(node: NodeIsNot) -> str:
     return "is not"
 
 
 def _get_joinedstr_value(node: NodeJoinedStr) -> str:
-    return "".join(get_value(value) for value in node.values)
+    _node_value_map[NodeConstant] = _get_constant_value_no_repr
+    result = repr("".join(get_value(value) for value in node.values))
+    _node_value_map[NodeConstant] = _get_constant_value
+    return result
 
 
 def _get_keyword_value(node: NodeKeyword) -> str:
     return f"{node.arg}={get_value(node.value)}"
 
 
 def _get_lambda_value(node: NodeLambda) -> str:
@@ -934,15 +950,18 @@
 
 
 def _get_sub_value(node: NodeSub) -> str:
     return "-"
 
 
 def _get_subscript_value(node: NodeSubscript) -> str:
-    return f"{get_value(node.value)}[{get_value(node.slice).strip('()')}]"
+    subscript = get_value(node.slice)
+    if isinstance(subscript, str):
+        subscript = subscript.strip("()")
+    return f"{get_value(node.value)}[{subscript}]"
 
 
 def _get_tuple_value(node: NodeTuple) -> str:
     return "(" + ", ".join(get_value(el) for el in node.elts) + ")"
 
 
 def _get_uadd_value(node: NodeUAdd) -> str:
@@ -953,14 +972,20 @@
     return f"{get_value(node.op)}{get_value(node.operand)}"
 
 
 def _get_usub_value(node: NodeUSub) -> str:
     return "-"
 
 
+def _get_yield_value(node: NodeYield) -> str:
+    if node.value is None:
+        return repr(None)
+    return get_value(node.value)
+
+
 _node_value_map: dict[Type, Callable[[Any], str]] = {
     type(None): lambda _: repr(None),
     NodeAdd: _get_add_value,
     NodeAnd: _get_and_value,
     NodeArguments: _get_arguments_value,
     NodeAttribute: _get_attribute_value,
     NodeBinOp: _get_binop_value,
@@ -1010,14 +1035,15 @@
     NodeStarred: _get_starred_value,
     NodeSub: _get_sub_value,
     NodeSubscript: _get_subscript_value,
     NodeTuple: _get_tuple_value,
     NodeUAdd: _get_uadd_value,
     NodeUnaryOp: _get_unaryop_value,
     NodeUSub: _get_usub_value,
+    NodeYield: _get_yield_value,
 }
 
 # TODO: remove once Python 3.8 support is dropped
 if sys.version_info < (3, 9):
 
     def _get_index_value(node: NodeIndex) -> str:
         return get_value(node.value)
```

### Comparing `griffe-0.8.0/src/griffe/agents/visitor.py` & `griffe-0.9.0/src/griffe/agents/visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,16 @@
         """Extend the base generic visit with extensions.
 
         Parameters:
             node: The node to visit.
         """
         for before_visitor in self.extensions.before_children_visit:
             before_visitor.visit(node)
-        super().generic_visit(node)
+        for child in node.children:  # type: ignore[attr-defined]  # noqa: WPS437
+            self.visit(child)
         for after_visitor in self.extensions.after_children_visit:
             after_visitor.visit(node)
 
     def visit_module(self, node: ast.Module) -> None:
         """Visit a module node.
 
         Parameters:
@@ -376,30 +377,37 @@
                 alias_name,
                 alias_path,
                 lineno=node.lineno,
                 endlineno=node.end_lineno,  # type: ignore[attr-defined]
             )
         self.generic_visit(node)
 
-    def visit_importfrom(self, node: ast.ImportFrom) -> None:
+    def visit_importfrom(self, node: ast.ImportFrom) -> None:  # noqa: WPS231
         """Visit an "import from" node.
 
         Parameters:
             node: The node to visit.
         """
         for name in node.names:
             alias_name = name.asname or name.name
             level = node.level
             module_path = node.module
             if level > 0:
+                if module_path is None:
+                    level -= 1
                 parent: Module = self.current.module
+                if parent.is_package or parent.is_subpackage:
+                    level -= 1
                 while level > 0:
                     parent = parent.parent  # type: ignore[assignment]
                     level -= 1
-                module_path = f"{parent.path}.{module_path}"
+                if module_path:
+                    module_path = f"{parent.path}.{module_path}"
+                else:
+                    module_path = parent.path
             if alias_name == "*":
                 alias_name = module_path.replace(".", "/") + "/*"  # type: ignore[union-attr]
                 alias_path = module_path
             else:
                 alias_path = f"{module_path}.{name.name}"
                 self.current.imports[alias_name] = alias_path
             self.current[alias_name] = Alias(
```

### Comparing `griffe-0.8.0/src/griffe/cli.py` & `griffe-0.9.0/src/griffe/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,97 +10,70 @@
 #   there's no `griffe.__main__` in `sys.modules`.
 
 """Module that contains the command line application."""
 
 from __future__ import annotations
 
 import argparse
-import asyncio
 import json
 import logging
 import os
 import sys
 from pathlib import Path
 from typing import Any, Sequence
 
 from griffe.agents.extensions import Extensions
 from griffe.agents.extensions.base import load_extensions
 from griffe.docstrings.parsers import Parser
 from griffe.encoders import Encoder
 from griffe.exceptions import ExtensionError
-from griffe.loader import AsyncGriffeLoader, GriffeLoader
+from griffe.loader import GriffeLoader
 from griffe.logger import get_logger
 
 logger = get_logger(__name__)
 
 
-def _print_data(data, output_file):
+def _print_data(data: str, output_file: str):
     if output_file is sys.stdout:
         print(data)
     else:
         with open(output_file, "w") as fd:
             print(data, file=fd)
 
 
-async def _load_packages_async(
-    packages: Sequence[str],
-    extensions: Extensions | None,
-    search_paths: Sequence[str],
-    docstring_parser: Parser | None,
-    docstring_options: dict[str, Any],
-):
-    loader = AsyncGriffeLoader(
-        extensions=extensions,
-        docstring_parser=docstring_parser,
-        docstring_options=docstring_options,
-    )
-    loaded = {}
-    for package in packages:
-        logger.info(f"Loading package {package}")
-        try:
-            module = await loader.load_module(package, search_paths=search_paths)
-        except ModuleNotFoundError:
-            logger.error(f"Could not find package {package}")
-        except ImportError:
-            logger.error(f"Tried but could not import package {package}")
-        else:
-            loaded[module.name] = module
-    for obj in loaded.values():
-        if not await loader.follow_aliases(obj):
-            logger.info("Not all aliases were resolved")
-    return loaded
-
-
 def _load_packages(
     packages: Sequence[str],
     extensions: Extensions | None,
     search_paths: Sequence[str],
     docstring_parser: Parser | None,
     docstring_options: dict[str, Any],
+    resolve_aliases: bool = True,
+    only_exported: bool = True,
+    only_known_modules: bool = True,
 ):
     loader = GriffeLoader(
         extensions=extensions,
         docstring_parser=docstring_parser,
         docstring_options=docstring_options,
     )
-    loaded = {}
     for package in packages:
         logger.info(f"Loading package {package}")
         try:
-            module = loader.load_module(package, search_paths=search_paths)
-        except ModuleNotFoundError:
-            logger.error(f"Could not find package {package}")
-        except ImportError:
-            logger.error(f"Tried but could not import package {package}")
+            loader.load_module(package, search_paths=search_paths)
+        except ModuleNotFoundError as error:
+            logger.error(f"Could not find package {package}: {error}")
+        except ImportError as error:
+            logger.error(f"Tried but could not import package {package}: {error}")
+    if resolve_aliases:
+        unresolved, iterations = loader.resolve_aliases(only_exported, only_known_modules)
+        if unresolved:
+            logger.info(f"{len(unresolved)} aliases were still unresolved after {iterations} iterations")
         else:
-            loaded[module.name] = module
-    for obj in loaded.values():
-        if not loader.follow_aliases(obj):
-            logger.info("Not all aliases were resolved")
-    return loaded
+            logger.info(f"All aliases were resolved after {iterations} iterations")
+    return loader.modules_collection.members
 
 
 _level_choices = ("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL")
 
 
 def get_parser() -> argparse.ArgumentParser:
     """Return the program argument parser.
@@ -222,20 +195,15 @@
 
     try:
         extensions = load_extensions(opts.extensions)
     except ExtensionError as error:
         print(f"griffe: error: {error}", file=sys.stderr)
         return 1
 
-    if opts.async_loader:
-        loop = asyncio.get_event_loop()
-        coroutine = _load_packages_async(opts.packages, extensions, search, opts.docstyle, opts.docopts)
-        packages = loop.run_until_complete(coroutine)
-    else:
-        packages = _load_packages(opts.packages, extensions, search, opts.docstyle, opts.docopts)
+    packages = _load_packages(opts.packages, extensions, search, opts.docstyle, opts.docopts)
 
     if per_package_output:
         for package_name, data in packages.items():
             serialized = json.dumps(data, cls=Encoder, indent=2, full=opts.full)
             _print_data(serialized, output.format(package=package_name))
     else:
         serialized = json.dumps(packages, cls=Encoder, indent=2, full=opts.full)
```

### Comparing `griffe-0.8.0/src/griffe/collections.py` & `griffe-0.9.0/src/griffe/collections.py`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/src/griffe/dataclasses.py` & `griffe-0.9.0/src/griffe/dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pathlib import Path
 from textwrap import dedent
 from typing import Any, Callable, cast
 
 from griffe.collections import LinesCollection, ModulesCollection
 from griffe.docstrings.dataclasses import DocstringSection
 from griffe.docstrings.parsers import Parser, parse  # noqa: WPS347
-from griffe.exceptions import AliasResolutionError, BuiltinModuleError, NameResolutionError
+from griffe.exceptions import AliasResolutionError, BuiltinModuleError, CyclicAliasError, NameResolutionError
 from griffe.expressions import Expression, Name
 from griffe.mixins import GetMembersMixin, ObjectAliasMixin, SetMembersMixin
 
 # TODO: remove once Python 3.7 support is dropped
 if sys.version_info < (3, 8):
     from cached_property import cached_property
 else:
@@ -335,16 +335,23 @@
         # attach the docstring to this object
         if docstring:
             docstring.parent = self
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}({self.name!r}, {self.lineno!r}, {self.endlineno!r})>"
 
-    def __bool__(self):
-        return bool(self.docstring) or any(self.members.values())
+    @property
+    def has_docstring(self) -> bool:
+        """Tell if this object has a non-empty docstring."""
+        return bool(self.docstring)  # noqa: DAR201
+
+    @property
+    def has_docstrings(self) -> bool:
+        """Tell if this object or any of its members has a non-empty docstring."""
+        return self.has_docstring or any(member.has_docstrings for member in self.members.values())  # noqa: DAR201
 
     def member_is_exported(self, member: Object | Alias, explicitely: bool = True) -> bool:
         """Tell if a member of this object is "exported".
 
         By exported, we mean that the object is included in the `__all__` attribute
         of its parent module or class. When `_all__` is not defined,
         we consider the member to be *implicitely* exported.
@@ -511,15 +518,15 @@
         """Return the full dotted path of this object.
 
         The canonical path is the path where the object was defined (not imported).
 
         Returns:
             A dotted path.
         """
-        if not self.parent:
+        if self.parent is None:
             return self.name
         return ".".join((self.parent.path, self.name))
 
     @cached_property
     def modules_collection(self) -> ModulesCollection:
         """Return the modules collection attached to this object or its parents.
 
@@ -699,23 +706,34 @@
         self.name: str = name
         if isinstance(target, str):
             self._target: Object | Alias | None = None
             self._target_path: str = target
         else:
             self._target = target
             self._target_path = target.path
-            if self.parent is not None:
-                target.aliases[self.path] = self
+            if parent is not None:
+                with suppress(AliasResolutionError):
+                    target.aliases[self.path] = self
         self.lineno: int | None = lineno
         self.endlineno: int | None = endlineno
         self._parent: Module | Class | None = parent
+        self._passed_through: bool = False
 
     def __getattr__(self, name: str) -> Any:
         # forward everything to the target
-        return getattr(self.target, name)
+        if self._passed_through:
+            raise CyclicAliasError([self._target_path])
+        self._passed_through = True
+        try:
+            attr = getattr(self.target, name)
+        except CyclicAliasError as error:
+            raise CyclicAliasError([self._target_path] + error.chain)
+        finally:
+            self._passed_through = False
+        return attr
 
     def __getitem__(self, key):
         # not handled by __getattr__
         return self.target[key]
 
     def __setitem__(self, key, value):
         # not handled by __getattr__
@@ -743,15 +761,16 @@
         """
         return self._parent
 
     @parent.setter
     def parent(self, value: Module | Class) -> None:
         self._parent = value
         if self.resolved:
-            self._target.aliases[self.path] = self  # type: ignore[union-attr]  # we just checked the target is not None
+            with suppress(AliasResolutionError):
+                self._target.aliases[self.path] = self  # type: ignore[union-attr]  # we just checked the target is not None
 
     @cached_property
     def path(self) -> str:
         """Return the dotted path / import path of this object.
 
         Returns:
             A dotted path.
@@ -922,15 +941,15 @@
     def is_namespace_package(self) -> bool:
         """Tell if this module is a namespace package (top folder, no `__init__.py`).
 
         Returns:
             True or False.
         """
         try:
-            return not self.parent and self.filepath.is_dir()
+            return self.parent is None and self.filepath.is_dir()
         except BuiltinModuleError:
             return False
 
     @cached_property
     def is_namespace_subpackage(self) -> bool:
         """Tell if this module is a namespace subpackage.
```

### Comparing `griffe-0.8.0/src/griffe/docstrings/dataclasses.py` & `griffe-0.9.0/src/griffe/docstrings/dataclasses.py`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/src/griffe/docstrings/google.py` & `griffe-0.9.0/src/griffe/docstrings/google.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     "attributes": DocstringSectionKind.attributes,
 }
 
 BlockItem = Tuple[int, List[str]]
 BlockItems = List[BlockItem]
 ItemsBlock = Tuple[BlockItems, int]
 
-_RE_ADMONITION: Pattern = re.compile(r"^(?P<type>[\w][\s\w-]*):(\s+(?P<title>.+))?$", re.I)
+_RE_ADMONITION: Pattern = re.compile(r"^(?P<type>[\w][\s\w-]*):(\s+(?P<title>[^\s].*))?$", re.I)
 """Regular expression to match admonitions, of the form `TYPE: [TITLE]`."""
 
 _RE_NAME_ANNOTATION_DESCRIPTION: Pattern = re.compile(r"^(?:(?P<name>\w+)?\s*(?:\((?P<type>.+)\))?:\s*)?(?P<desc>.*)$")
 """Regular expression to match `name (type): Description` in docstrings sections items."""
 
 
 def _read_block_items(docstring: Docstring, offset: int) -> ItemsBlock:  # noqa: WPS231
@@ -546,42 +546,47 @@
             current_section.append(lines[offset])
 
         else:
             # TODO: once Python 3.7 is dropped, use walrus operator
             match = _RE_ADMONITION.match(lines[offset])
             if match:
                 groups = match.groupdict()
-                admonition_type = groups["type"].lower()
-                if admonition_type in _section_kind:
+                title = groups["title"]
+                admonition_type = groups["type"]
+                if admonition_type.lower() in _section_kind:
                     if current_section:
                         if any(current_section):
                             sections.append(
                                 DocstringSection(
                                     DocstringSectionKind.text,
                                     "\n".join(current_section).rstrip("\n"),
                                 )
                             )
                         current_section = []
-                    reader = _section_reader[_section_kind[admonition_type]]
+                    reader = _section_reader[_section_kind[admonition_type.lower()]]
                     section, offset = reader(docstring, offset + 1)
                     if section:
-                        section.title = groups["title"]
+                        section.title = title
                         sections.append(section)
 
                 else:
                     contents, offset = _read_block(docstring, offset + 1)
                     if contents:
+                        if title is None and " " in admonition_type:
+                            title = admonition_type
+                            admonition_type = "note"
                         sections.append(
                             DocstringSection(
                                 kind=DocstringSectionKind.admonition,
-                                value=DocstringAdmonition(kind=admonition_type, contents=contents),
-                                title=groups["title"],
+                                value=DocstringAdmonition(kind=admonition_type.lower(), contents=contents),
+                                title=title,
                             )
                         )
                     else:
+                        offset -= 1
                         with suppress(IndexError):
                             current_section.append(lines[offset])
             else:
                 current_section.append(lines[offset])
 
         offset += 1
```

### Comparing `griffe-0.8.0/src/griffe/docstrings/numpy.py` & `griffe-0.9.0/src/griffe/docstrings/numpy.py`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/src/griffe/docstrings/parsers.py` & `griffe-0.9.0/src/griffe/docstrings/parsers.py`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/src/griffe/docstrings/rst.py` & `griffe-0.9.0/src/griffe/docstrings/rst.py`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/src/griffe/docstrings/utils.py` & `griffe-0.9.0/src/griffe/docstrings/utils.py`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/src/griffe/encoders.py` & `griffe-0.9.0/src/griffe/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """This module contains data encoders/serializers and decoders/deserializers.
 
 The available formats are:
 
-- JSON: see the [encoder][griffe.encoders.Encoder] and [decoder][griffe.encoders.decoder].
+- `JSON`: see the [encoder][griffe.encoders.Encoder] and [decoder][griffe.encoders.decoder].
 """
 
 from __future__ import annotations
 
 import json
 from pathlib import Path, PosixPath
 from typing import Any, Callable, Type
```

### Comparing `griffe-0.8.0/src/griffe/exceptions.py` & `griffe-0.9.0/src/griffe/exceptions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """This module contains all the exceptions specific to Griffe."""
 
+from __future__ import annotations
+
 
 class GriffeError(Exception):
     """The base exception for all Griffe errors."""
 
 
 class NameResolutionError(GriffeError):
     """Exception for names that cannot be resolved in a object scope."""
@@ -23,15 +25,28 @@
     def __init__(self, target_path: str) -> None:
         """Initialize the exception.
 
         Parameters:
             target_path: The problematic target path.
         """
         self.target_path: str = target_path
-        super().__init__(f"could not resolve {self.target_path}")
+        super().__init__(f"Could not resolve {self.target_path}")
+
+
+class CyclicAliasError(GriffeError):
+    """Exception raised when a cycle is detected in aliases."""
+
+    def __init__(self, chain: list[str]) -> None:
+        """Initialize the exception.
+
+        Parameters:
+            chain: The cyclic chain of items (such as target path).
+        """
+        self.chain: list[str] = chain
+        super().__init__("Cyclic aliases detected:\n  " + "\n  ".join(self.chain))
 
 
 class LastNodeError(GriffeError):
     """Exception raised when trying to access a next or previous node."""
 
 
 class RootNodeError(GriffeError):
```

### Comparing `griffe-0.8.0/src/griffe/expressions.py` & `griffe-0.9.0/src/griffe/expressions.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,17 @@
         if isinstance(full, str):
             self._full: str = full
             self._resolver: Callable = lambda: None
         else:
             self._full = ""
             self._resolver = full
 
+    def __eq__(self, other: Name) -> bool:  # type: ignore[override]
+        return self.source == other.source and self.full == other.full  # noqa: WPS437
+
     def __repr__(self) -> str:
         return f"Name(source={self.source!r}, full={self.full!r})"
 
     def __str__(self) -> str:
         return self.source
 
     @property
```

### Comparing `griffe-0.8.0/src/griffe/importer.py` & `griffe-0.9.0/src/griffe/importer.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,16 +8,22 @@
 
     It can be a module, class, method, function, attribute,
     nested arbitrarily.
 
     Parameters:
         import_path: The path of the object to import.
 
+    Raises:
+        ImportError: When there was an error during import.
+
     Returns:
         The imported object.
     """
-    module = __import__(import_path, level=0)
+    try:
+        module = __import__(import_path, level=0)
+    except Exception as error:
+        raise ImportError(f"Error while importing '{import_path}': {error}") from error
     attr_parts = import_path.split(".")[1:]
     value = module
     for part in attr_parts:
         value = getattr(value, part)
     return value
```

### Comparing `griffe-0.8.0/src/griffe/loader.py` & `griffe-0.9.0/src/griffe/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,29 @@
 griffe = GriffeLoader()
 fastapi = griffe.load_module("fastapi")
 ```
 """
 
 from __future__ import annotations
 
-import asyncio
 import os
 import sys
 import traceback
 from contextlib import suppress
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Iterator, Sequence, Tuple
 
 from griffe.agents.extensions import Extensions
 from griffe.agents.inspector import inspect
 from griffe.agents.visitor import patch_ast, visit
 from griffe.collections import LinesCollection, ModulesCollection
 from griffe.dataclasses import Alias, Kind, Module, Object
 from griffe.docstrings.parsers import Parser
-from griffe.exceptions import AliasResolutionError, UnhandledPthFileError, UnimportableModuleError
+from griffe.exceptions import AliasResolutionError, CyclicAliasError, UnhandledPthFileError, UnimportableModuleError
 from griffe.logger import get_logger
 
 NamePartsType = Tuple[str, ...]
 NamePartsAndPathType = Tuple[NamePartsType, Path]
 
 logger = get_logger(__name__)
 
@@ -65,15 +64,17 @@
 
     return _read_async
 
 
 _builtin_modules: set[str] = set(sys.builtin_module_names)
 
 
-class _BaseGriffeLoader:
+class GriffeLoader:
+    """The Griffe loader, allowing to load data from modules."""
+
     def __init__(
         self,
         extensions: Extensions | None = None,
         docstring_parser: Parser | None = None,
         docstring_options: dict[str, Any] | None = None,
         lines_collection: LinesCollection | None = None,
         modules_collection: ModulesCollection | None = None,
@@ -90,76 +91,14 @@
         self.extensions: Extensions = extensions or Extensions()
         self.docstring_parser: Parser | None = docstring_parser
         self.docstring_options: dict[str, Any] = docstring_options or {}
         self.lines_collection: LinesCollection = lines_collection or LinesCollection()
         self.modules_collection: ModulesCollection = modules_collection or ModulesCollection()
         patch_ast()
 
-    def _create_module(self, module_name: str, module_path: Path) -> Module:
-        return Module(
-            module_name,
-            filepath=module_path,
-            lines_collection=self.lines_collection,
-            modules_collection=self.modules_collection,
-        )
-
-    def _visit_module(self, code: str, module_name: str, module_path: Path, parent: Module | None = None) -> Module:
-        self.lines_collection[module_path] = code.splitlines(keepends=False)
-        return visit(
-            module_name,
-            filepath=module_path,
-            code=code,
-            extensions=self.extensions,
-            parent=parent,
-            docstring_parser=self.docstring_parser,
-            docstring_options=self.docstring_options,
-            lines_collection=self.lines_collection,
-            modules_collection=self.modules_collection,
-        )
-
-    def _inspect_module(self, module_name: str, filepath: Path | None = None, parent: Module | None = None) -> Module:
-        return inspect(
-            module_name,
-            filepath=filepath,
-            extensions=self.extensions,
-            parent=parent,
-            docstring_parser=self.docstring_parser,
-            docstring_options=self.docstring_options,
-            lines_collection=self.lines_collection,
-        )
-
-    def _member_parent(self, module: Module, subparts: NamePartsType, subpath: Path) -> Module:
-        parent_parts = subparts[:-1]
-        try:
-            return module[parent_parts]
-        except KeyError:
-            if module.is_namespace_package or module.is_namespace_subpackage:
-                member_parent = Module(
-                    subparts[0],
-                    filepath=subpath.parent,
-                    lines_collection=self.lines_collection,
-                    modules_collection=self.modules_collection,
-                )
-                module[parent_parts] = member_parent
-                return member_parent
-        raise UnimportableModuleError(f"{subpath} is not importable")
-
-    def _expand_wildcard(self, wildcard_obj: Alias) -> dict[str, Object | Alias]:
-        module = self.modules_collection[wildcard_obj.wildcard]  # type: ignore[index]  # we know it's a wildcard
-        explicitely = "__all__" in module.members
-        return {
-            name: imported_member
-            for name, imported_member in module.members.items()
-            if imported_member.is_exported(explicitely=explicitely)
-        }
-
-
-class GriffeLoader(_BaseGriffeLoader):
-    """The Griffe loader, allowing to load data from modules."""
-
     def load_module(
         self,
         module: str | Path,
         submodules: bool = True,
         search_paths: Sequence[str | Path] | None = None,
         try_relative_path: bool = True,
     ) -> Module:
@@ -189,65 +128,132 @@
                 top_module = self._inspect_module(module)  # type: ignore[arg-type]
             else:
                 logger.debug(f"Found {module}: visiting")
                 top_module = self._load_module_path(top_module_name, top_module_path, submodules=submodules)
         self.modules_collection[top_module.path] = top_module
         return self.modules_collection[module_name]  # type: ignore[index]
 
-    def follow_aliases(self, obj: Object, only_exported: bool = True) -> bool:  # noqa: WPS231
+    def resolve_aliases(  # noqa: WPS231
+        self,
+        only_exported: bool = True,
+        only_known_modules: bool = True,
+        max_iterations: int | None = None,
+    ) -> tuple[set[str], int]:
+        """Resolve aliases.
+
+        Parameters:
+            only_exported: When true, only try to resolve an alias if it is explicitely exported.
+            only_known_modules: When true, don't try to load unspecified modules to resolve aliases.
+            max_iterations: Maximum number of iterations on the loader modules collection.
+
+        Returns:
+            The unresolved aliases and the number of iterations done.
+        """
+        if max_iterations is None:
+            max_iterations = float("inf")  # type: ignore[assignment]
+        prev_unresolved: set[str] = set()
+        unresolved: set[str] = set("0")  # init to enter loop
+        iterations = 0
+        collection = self.modules_collection.members
+        while unresolved and unresolved != prev_unresolved and iterations < max_iterations:  # type: ignore[operator]
+            prev_unresolved = unresolved
+            unresolved = set()
+            iterations += 1
+            for module_name in list(collection.keys()):
+                module = collection[module_name]
+                unresolved |= self.resolve_module_aliases(module, only_exported, only_known_modules)
+            logger.debug(f"Iteration {iterations}")
+            logger.debug(f"prev: {len(prev_unresolved)}; current: {len(unresolved)}")
+            logger.debug("\n- " + "\n- ".join(sorted(unresolved & prev_unresolved)))
+        return unresolved, iterations
+
+    def resolve_module_aliases(  # noqa: WPS231
+        self,
+        obj: Object,
+        only_exported: bool = True,
+        only_known_modules: bool = True,
+        seen: set | None = None,
+    ) -> set[str]:
         """Follow aliases: try to recursively resolve all found aliases.
 
         Parameters:
             obj: The object and its members to recurse on.
-            only_exported: Only try to resolve an alias if it is explicitely exported.
+            only_exported: When true, only try to resolve an alias if it is explicitely exported.
+            only_known_modules: When true, don't try to load unspecified modules to resolve aliases.
+            seen: Used to avoid infinite recursion.
 
         Returns:
             True if everything was resolved, False otherwise.
         """
-        success = True
+        unresolved = set()
         expanded = {}
         to_remove = []
+        seen = seen or set()
+        seen.add(obj.path)
 
         # iterate a first time to expand wildcards
         for member in obj.members.values():
             if member.is_alias and member.wildcard:  # type: ignore[union-attr]  # we know it's an alias
                 package = member.wildcard.split(".", 1)[0]  # type: ignore[union-attr]
                 if obj.package.path != package and package not in self.modules_collection:
                     try:
                         self.load_module(package, try_relative_path=False)
                     except ImportError as error:
-                        logger.warning(f"Could not expand wildcard import {member.name} in {obj.path}: {error}")
+                        logger.debug(f"Could not expand wildcard import {member.name} in {obj.path}: {error}")
                     else:
                         expanded.update(self._expand_wildcard(member))  # type: ignore[arg-type]
                         to_remove.append(member.name)
 
         for name in to_remove:
             del obj[name]  # noqa: WPS420
         for new_member in expanded.values():
-            obj[new_member.name] = Alias(new_member.name, new_member)
+            if new_member.is_alias and not new_member.wildcard:  # type: ignore[union-attr]
+                try:
+                    alias = Alias(new_member.name, new_member.target)  # type: ignore[union-attr]
+                except AliasResolutionError:
+                    alias = Alias(new_member.name, new_member._target_path)  # type: ignore[union-attr]  # noqa: WPS437
+                except CyclicAliasError as error:  # noqa: WPS440
+                    logger.debug(str(error))
+            else:
+                alias = Alias(new_member.name, new_member)
+            obj[new_member.name] = alias
 
         # iterate a second time to resolve aliases and recurse
         for member in obj.members.values():  # noqa: WPS440
-            if member.is_alias and not member.wildcard:  # type: ignore[union-attr]
+            if member.is_alias:
+                if member.wildcard or member.resolved:  # type: ignore[union-attr]
+                    continue
                 if only_exported and not member.is_explicitely_exported:
                     continue
                 try:
                     member.resolve_target()  # type: ignore[union-attr]
                 except AliasResolutionError as error:  # noqa: WPS440
-                    success = False
-                    package = error.target_path.split(".", 1)[0]
-                    if obj.package.path != package and package not in self.modules_collection:
+                    path = member.path
+                    target = error.target_path  # type: ignore[union-attr]  # noqa: WPS437
+                    logger.debug(f"Alias resolution error for {path} -> {target}")
+                    unresolved.add(path)
+                    package = target.split(".", 1)[0]
+                    load_module = (
+                        not only_known_modules
+                        and obj.package.path != package
+                        and package not in self.modules_collection
+                    )
+                    if load_module:
                         try:  # noqa: WPS505
                             self.load_module(package, try_relative_path=False)
                         except ImportError as error:  # noqa: WPS440
-                            logger.warning(f"Could not follow alias {member.path}: {error}")
-            elif member.kind in {Kind.MODULE, Kind.CLASS}:
-                success &= self.follow_aliases(member)  # type: ignore[arg-type]  # we know it's an object
+                            logger.debug(f"Could not follow alias {member.path}: {error}")
+                except CyclicAliasError as error:
+                    logger.debug(str(error))
+                else:
+                    logger.debug(f"Alias {member.path} was resolved to {member.target.path}")  # type: ignore[union-attr]
+            elif member.kind in {Kind.MODULE, Kind.CLASS} and member.path not in seen:
+                unresolved |= self.resolve_module_aliases(member, only_exported, only_known_modules, seen)  # type: ignore[arg-type]
 
-        return success
+        return unresolved
 
     def _load_module_path(
         self,
         module_name: str,
         module_path: Path,
         submodules: bool = True,
         parent: Module | None = None,
@@ -268,153 +274,90 @@
         for subparts, subpath in sorted(iter_submodules(module.filepath), key=_module_depth):
             self._load_submodule(module, subparts, subpath)
 
     def _load_submodule(self, module: Module, subparts: NamePartsType, subpath: Path) -> None:
         try:
             member_parent = self._member_parent(module, subparts, subpath)
         except UnimportableModuleError as error:
-            logger.warning(f"{error}. Missing __init__ module?")
+            logger.debug(f"{error}. Missing __init__ module?")
             return
-        try:
+        try:  # noqa: WPS225
             member_parent[subparts[-1]] = self._load_module_path(
                 subparts[-1], subpath, submodules=False, parent=member_parent
             )
         except SyntaxError:
             message = traceback.format_exc(limit=0).replace("SyntaxError: invalid syntax", "").strip()
             logger.error(f"Syntax error: {message}")
+        except ImportError as error:  # noqa: WPS440
+            logger.error(f"Import error: {error}")
+        except UnicodeDecodeError as error:  # noqa: WPS440
+            logger.error(f"UnicodeDecodeError when loading {subpath}: {error}")
+        except OSError as error:  # noqa: WPS440
+            logger.error(f"OSError when loading {subpath}: {error}")
 
+    def _create_module(self, module_name: str, module_path: Path) -> Module:
+        return Module(
+            module_name,
+            filepath=module_path,
+            lines_collection=self.lines_collection,
+            modules_collection=self.modules_collection,
+        )
 
-class AsyncGriffeLoader(_BaseGriffeLoader):
-    """The asynchronous Griffe loader, allowing to load data from modules."""
-
-    async def load_module(
-        self,
-        module: str | Path,
-        submodules: bool = True,
-        search_paths: Sequence[str | Path] | None = None,
-        try_relative_path: bool = True,
-    ) -> Module:
-        """Load a module.
-
-        Parameters:
-            module: The module name or path.
-            submodules: Whether to recurse on the submodules.
-            search_paths: The paths to search into.
-            try_relative_path: Whether to try finding the module as a relative path.
-
-        Returns:
-            A module.
-        """
-        if module in _builtin_modules:
-            logger.debug(f"{module} is a builtin module: inspecting")
-            module_name = module
-            top_module = self._inspect_module(module)  # type: ignore[arg-type]
-        else:
-            try:
-                module_name, top_module_name, top_module_path = _top_name_and_path(
-                    module, search_paths, try_relative_path
-                )
-            except ModuleNotFoundError:
-                logger.debug(f"Could not find {module}: trying inspection")
-                module_name = module
-                top_module = self._inspect_module(module)  # type: ignore[arg-type]
-            else:
-                logger.debug(f"Found {module}: visiting")
-                top_module = await self._load_module_path(top_module_name, top_module_path, submodules=submodules)
-        self.modules_collection[top_module.path] = top_module
-        return self.modules_collection[module_name]  # type: ignore[index]
-
-    async def follow_aliases(self, obj: Object, only_exported: bool = True) -> bool:  # noqa: WPS231
-        """Follow aliases: try to recursively resolve all found aliases.
-
-        Parameters:
-            obj: The object and its members to recurse on.
-            only_exported: Only try to resolve an alias if it is explicitely exported.
-
-        Returns:
-            True if everything was resolved, False otherwise.
-        """
-        success = True
-        expanded = {}
-        to_remove = []
-
-        # iterate a first time to expand wildcards
-        for member in obj.members.values():
-            if member.is_alias and member.wildcard:  # type: ignore[union-attr]  # we know it's an alias
-                package = member.wildcard.split(".", 1)[0]  # type: ignore[union-attr]
-                if obj.package.path != package and package not in self.modules_collection:
-                    try:
-                        await self.load_module(package, try_relative_path=False)
-                    except ImportError as error:
-                        logger.warning(f"Could not expand wildcard import {member.name} in {obj.path}: {error}")
-                    else:
-                        expanded.update(self._expand_wildcard(member))  # type: ignore[arg-type]
-                        to_remove.append(member.name)
-
-        for name in to_remove:
-            del obj[name]  # noqa: WPS420
-        for new_member in expanded.values():
-            obj[new_member.name] = Alias(new_member.name, new_member)
-
-        # iterate a second time to resolve aliases and recurse
-        for member in obj.members.values():  # noqa: WPS440
-            if member.is_alias and not member.wildcard:  # type: ignore[union-attr]
-                if only_exported and not member.is_explicitely_exported:
-                    continue
-                try:
-                    member.resolve_target()  # type: ignore[union-attr]
-                except AliasResolutionError as error:  # noqa: WPS440
-                    success = False
-                    package = error.target_path.split(".", 1)[0]
-                    if obj.package.path != package and package not in self.modules_collection:
-                        try:  # noqa: WPS505
-                            await self.load_module(package, try_relative_path=False)
-                        except ImportError as error:  # noqa: WPS440
-                            logger.warning(f"Could not follow alias {member.path}: {error}")
-            elif member.kind in {Kind.MODULE, Kind.CLASS}:
-                success &= await self.follow_aliases(member)  # type: ignore[arg-type]  # we know it's an object
-
-        return success
-
-    async def _load_module_path(
-        self,
-        module_name: str,
-        module_path: Path,
-        submodules: bool = True,
-        parent: Module | None = None,
-    ) -> Module:
-        logger.debug(f"Loading path {module_path}")
-        if module_path.is_dir():
-            module = self._create_module(module_name, module_path)
-        elif module_path.suffix == ".py":
-            code = await _get_async_reader()(module_path)
-            module = self._visit_module(code, module_name, module_path, parent)
-        else:
-            module = self._inspect_module(module_name, module_path, parent)
-        if submodules:
-            await self._load_submodules(module)
-        return module
-
-    async def _load_submodules(self, module: Module) -> None:
-        await asyncio.gather(
-            *[
-                self._load_submodule(module, subparts, subpath)
-                for subparts, subpath in sorted(iter_submodules(module.filepath), key=_module_depth)
-            ]
+    def _visit_module(self, code: str, module_name: str, module_path: Path, parent: Module | None = None) -> Module:
+        self.lines_collection[module_path] = code.splitlines(keepends=False)
+        return visit(
+            module_name,
+            filepath=module_path,
+            code=code,
+            extensions=self.extensions,
+            parent=parent,
+            docstring_parser=self.docstring_parser,
+            docstring_options=self.docstring_options,
+            lines_collection=self.lines_collection,
+            modules_collection=self.modules_collection,
         )
 
-    async def _load_submodule(self, module: Module, subparts: NamePartsType, subpath: Path) -> None:
+    def _inspect_module(self, module_name: str, filepath: Path | None = None, parent: Module | None = None) -> Module:
         try:
-            member_parent = self._member_parent(module, subparts, subpath)
-        except UnimportableModuleError as error:
-            logger.debug(str(error))
-        else:
-            member_parent[subparts[-1]] = await self._load_module_path(
-                subparts[-1], subpath, submodules=False, parent=member_parent
+            return inspect(
+                module_name,
+                filepath=filepath,
+                extensions=self.extensions,
+                parent=parent,
+                docstring_parser=self.docstring_parser,
+                docstring_options=self.docstring_options,
+                lines_collection=self.lines_collection,
             )
+        except SystemExit as error:
+            raise ImportError(f"Importing '{module_name}' raised a system exit") from error
+
+    def _member_parent(self, module: Module, subparts: NamePartsType, subpath: Path) -> Module:
+        parent_parts = subparts[:-1]
+        try:
+            return module[parent_parts]
+        except KeyError:
+            if module.is_namespace_package or module.is_namespace_subpackage:
+                member_parent = Module(
+                    subparts[0],
+                    filepath=subpath.parent,
+                    lines_collection=self.lines_collection,
+                    modules_collection=self.modules_collection,
+                )
+                module[parent_parts] = member_parent
+                return member_parent
+        raise UnimportableModuleError(f"{subpath} is not importable")
+
+    def _expand_wildcard(self, wildcard_obj: Alias) -> dict[str, Object | Alias]:
+        module = self.modules_collection[wildcard_obj.wildcard]  # type: ignore[index]  # we know it's a wildcard
+        explicitely = "__all__" in module.members
+        return {
+            name: imported_member
+            for name, imported_member in module.members.items()
+            if imported_member.is_exported(explicitely=explicitely)
+        }
 
 
 def _top_name_and_path(
     module: str | Path,
     search_paths: Sequence[str | Path] | None = None,
     try_relative_path: bool = True,
 ) -> tuple[str, str, Path]:
```

### Comparing `griffe-0.8.0/src/griffe/logger.py` & `griffe-0.9.0/src/griffe/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 function so dependant libraries can patch loggers as they see fit.
 
 For example, to fit in the MkDocs logging configuration
 and prefix each log message with the module name:
 
 ```python
 import logging
-from griffe import logger as patch_loggers
+from griffe.logger import patch_loggers
 
 
 class LoggerAdapter(logging.LoggerAdapter):
     def __init__(self, prefix, logger):
         super().__init__(logger, {})
         self.prefix = prefix
```

### Comparing `griffe-0.8.0/src/griffe/mixins.py` & `griffe-0.9.0/src/griffe/mixins.py`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/tests/.pytest_cache/v/cache/nodeids` & `griffe-0.9.0/tests/.pytest_cache/v/cache/nodeids`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9541284403669725%*

 * *Differences: {'insert': "[(7, 'test_docstrings/test_google.py::test_multi_single_line_sections'), (18, "*

 * *           "'test_docstrings/test_google.py::test_parse_partially_indented_lines'), (27, "*

 * *           "'test_docstrings/test_google.py::test_unknown_matching_admonitions'), (107, "*

 * *           "'test_inspector.py::test_annotations_from_actual_python_objects'), (108, "*

 * *           "'test_inspector.py::test_s')]"}*

```diff
@@ -2,32 +2,35 @@
     "test_cli.py::test_main",
     "test_cli.py::test_show_help",
     "test_docstrings/test_google.py::test_close_sections",
     "test_docstrings/test_google.py::test_code_blocks",
     "test_docstrings/test_google.py::test_different_indentation",
     "test_docstrings/test_google.py::test_indented_code_block",
     "test_docstrings/test_google.py::test_invalid_sections",
+    "test_docstrings/test_google.py::test_multi_single_line_sections",
     "test_docstrings/test_google.py::test_multiline_docstring",
     "test_docstrings/test_google.py::test_multiple_lines_in_sections_items",
     "test_docstrings/test_google.py::test_parameter_line_without_colon",
     "test_docstrings/test_google.py::test_parameter_line_without_colon_keyword_only",
     "test_docstrings/test_google.py::test_parse_admonitions",
     "test_docstrings/test_google.py::test_parse_args_and_kwargs",
     "test_docstrings/test_google.py::test_parse_args_kwargs_keyword_only",
     "test_docstrings/test_google.py::test_parse_attributes_section",
     "test_docstrings/test_google.py::test_parse_examples_sections",
     "test_docstrings/test_google.py::test_parse_optional_type_in_docstring",
+    "test_docstrings/test_google.py::test_parse_partially_indented_lines",
     "test_docstrings/test_google.py::test_parse_types_in_docstring",
     "test_docstrings/test_google.py::test_parse_with_annotations",
     "test_docstrings/test_google.py::test_parse_without_annotations",
     "test_docstrings/test_google.py::test_parse_without_parent",
     "test_docstrings/test_google.py::test_parse_yields_section",
     "test_docstrings/test_google.py::test_parse_yields_section_with_return_annotation",
     "test_docstrings/test_google.py::test_prefer_docstring_types_over_annotations",
     "test_docstrings/test_google.py::test_simple_docstring",
+    "test_docstrings/test_google.py::test_unknown_matching_admonitions",
     "test_docstrings/test_numpy.py::test_attributes_section",
     "test_docstrings/test_numpy.py::test_code_blocks",
     "test_docstrings/test_numpy.py::test_deprecated_section",
     "test_docstrings/test_numpy.py::test_examples_section",
     "test_docstrings/test_numpy.py::test_indented_code_block",
     "test_docstrings/test_numpy.py::test_multiline_docstring",
     "test_docstrings/test_numpy.py::test_other_parameters_section",
@@ -98,9 +101,11 @@
     "test_docstrings/test_rst.py::test_parse__return_directive_annotation__prefer_return_directive",
     "test_docstrings/test_rst.py::test_parse__return_directive_annotation__return_section_with_type",
     "test_docstrings/test_rst.py::test_parse__return_directive_rtype__return_section_with_type",
     "test_docstrings/test_rst.py::test_parse__return_directive_rtype_first__return_section_with_type",
     "test_docstrings/test_rst.py::test_parse__return_invalid__error",
     "test_docstrings/test_rst.py::test_parse__rtype_invalid__error",
     "test_docstrings/test_rst.py::test_parse_module_attributes_section__expected_attributes_section",
-    "test_functions.py::test_loading_functions_parameters"
+    "test_functions.py::test_loading_functions_parameters",
+    "test_inspector.py::test_annotations_from_actual_python_objects",
+    "test_inspector.py::test_s"
 ]
```

### Comparing `griffe-0.8.0/tests/fixtures/functions/parameters.py` & `griffe-0.9.0/tests/fixtures/functions/parameters.py`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/tests/test_docstrings/helpers.py` & `griffe-0.9.0/tests/test_docstrings/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,9 +71,9 @@
 def assert_element_equal(actual: DocstringElement, expected: DocstringElement) -> None:
     """Help assert docstring elements are equal.
 
     Parameters:
         actual: The actual element.
         expected: The expected element.
     """
-    assert actual.annotation == expected.annotation
+    assert actual.annotation == expected.annotation  # type: ignore[operator]
     assert actual.description == expected.description
```

### Comparing `griffe-0.8.0/tests/test_docstrings/test_google.py` & `griffe-0.9.0/tests/test_docstrings/test_google.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,49 @@
         Blablablabla.
         """
     )
     assert len(sections) == 1
     assert not warnings
 
 
+def test_unknown_matching_admonitions():
+    """Properly handle offset when matching an unknown admonition (line ending with `:`)."""
+    docstring = """
+        First line.
+
+        Matching but unknown admonition type:
+
+        - Some list items
+
+        Ending line.
+    """
+    sections, warnings = parse(docstring)
+    assert len(sections) == 1
+    assert sections[0].kind is DocstringSectionKind.text
+    # -2 because docstring is stripped
+    assert len(sections[0].value.splitlines()) == len(docstring.splitlines()) - 2
+    assert not warnings
+
+
+def test_parse_partially_indented_lines():
+    """Properly handle partially indented lines."""
+    docstring = """
+        The available formats are:
+           - JSON
+
+        The unavailable formats are:  
+           - YAML
+    """  # noqa: W291
+    sections, warnings = parse(docstring)
+    assert len(sections) == 2
+    assert sections[0].kind is DocstringSectionKind.admonition
+    assert sections[1].kind is DocstringSectionKind.text
+    assert not warnings
+
+
 def test_multiple_lines_in_sections_items():
     """Parse multi-line item description."""
     docstring = """
         Parameters:
             p (int): This parameter
                has a description
               spawning on multiple lines.
@@ -652,16 +687,16 @@
         Something:
             Something.
     """
 
     sections, warnings = parse(docstring)
     assert len(sections) == 3
     assert not warnings
-    assert sections[0].title is None
-    assert sections[0].value.kind == "important note"
+    assert sections[0].title == "Important note"
+    assert sections[0].value.kind == "note"
     assert sections[0].value.contents == "Hello."
     assert sections[1].title == "With title."
     assert sections[1].value.kind == "note"
     assert sections[1].value.contents == "Hello again."
     assert sections[2].title is None
     assert sections[2].value.kind == "something"
     assert sections[2].value.contents == "Something."
```

### Comparing `griffe-0.8.0/tests/test_docstrings/test_numpy.py` & `griffe-0.9.0/tests/test_docstrings/test_numpy.py`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/tests/test_docstrings/test_rst.py` & `griffe-0.9.0/tests/test_docstrings/test_rst.py`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/tests/test_functions.py` & `griffe-0.9.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `griffe-0.8.0/PKG-INFO` & `griffe-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffe
-Version: 0.8.0
+Version: 0.9.0
 Summary: Signatures for entire Python programs. Extract the structure, the frame, the skeleton of your project, to generate API documentation or find breaking changes in your API.
 License: UNKNOWN
 Author-email: Timothée Mazzucotelli <pawamoy@pm.me>
 Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: griffe Version: 0.8.0 Summary: Signatures for
+Metadata-Version: 2.1 Name: griffe Version: 0.9.0 Summary: Signatures for
 entire Python programs. Extract the structure, the frame, the skeleton of your
 project, to generate API documentation or find breaking changes in your API.
 License: UNKNOWN Author-email: TimothÃ©e Mazzucotelli
 pm.me> Requires-Python: >=3.7 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: ISC License (ISCL) Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

