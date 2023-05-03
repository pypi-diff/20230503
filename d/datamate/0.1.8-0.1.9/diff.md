# Comparing `tmp/datamate-0.1.8.tar.gz` & `tmp/datamate-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamate-0.1.8.tar", last modified: Tue May  2 12:56:34 2023, max compression
+gzip compressed data, was "datamate-0.1.9.tar", last modified: Wed May  3 21:39:26 2023, max compression
```

## Comparing `datamate-0.1.8.tar` & `datamate-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-02 12:56:34.334211 datamate-0.1.8/
--rw-r--r--   0 lappalainenj (1483866292) 1899195968     3829 2023-05-02 12:56:34.333460 datamate-0.1.8/PKG-INFO
--rw-r--r--   0 lappalainenj (1483866292) 1899195968     3642 2023-03-06 13:58:32.000000 datamate-0.1.8/README.md
-drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-02 12:56:34.329914 datamate-0.1.8/datamate/
--rw-r--r--   0 lappalainenj (1483866292) 1899195968      647 2023-05-01 19:25:54.000000 datamate-0.1.8/datamate/__init__.py
--rw-r--r--   0 lappalainenj (1483866292) 1899195968    57284 2023-05-02 12:04:55.000000 datamate-0.1.8/datamate/directory.py
--rw-r--r--   0 lappalainenj (1483866292) 1899195968    11921 2023-05-01 17:35:54.000000 datamate-0.1.8/datamate/namespaces.py
--rw-r--r--   0 lappalainenj (1483866292) 1899195968       20 2023-05-02 12:54:26.000000 datamate-0.1.8/datamate/version.py
-drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-02 12:56:34.332120 datamate-0.1.8/datamate.egg-info/
--rw-r--r--   0 lappalainenj (1483866292) 1899195968     3829 2023-05-02 12:56:34.000000 datamate-0.1.8/datamate.egg-info/PKG-INFO
--rw-r--r--   0 lappalainenj (1483866292) 1899195968      312 2023-05-02 12:56:34.000000 datamate-0.1.8/datamate.egg-info/SOURCES.txt
--rw-r--r--   0 lappalainenj (1483866292) 1899195968        1 2023-05-02 12:56:34.000000 datamate-0.1.8/datamate.egg-info/dependency_links.txt
--rw-r--r--   0 lappalainenj (1483866292) 1899195968      109 2023-05-02 12:56:34.000000 datamate-0.1.8/datamate.egg-info/requires.txt
--rw-r--r--   0 lappalainenj (1483866292) 1899195968        9 2023-05-02 12:56:34.000000 datamate-0.1.8/datamate.egg-info/top_level.txt
--rw-r--r--   0 lappalainenj (1483866292) 1899195968       38 2023-05-02 12:56:34.334360 datamate-0.1.8/setup.cfg
--rw-r--r--   0 lappalainenj (1483866292) 1899195968      926 2023-05-01 19:20:47.000000 datamate-0.1.8/setup.py
-drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-02 12:56:34.332949 datamate-0.1.8/tests/
--rwxr-xr-x   0 lappalainenj (1483866292) 1899195968    30336 2023-05-02 12:36:23.000000 datamate-0.1.8/tests/test_directory.py
--rw-r--r--   0 lappalainenj (1483866292) 1899195968     3747 2023-04-04 14:23:09.000000 datamate-0.1.8/tests/test_namespaces.py
+drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-03 21:39:26.627900 datamate-0.1.9/
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968     3829 2023-05-03 21:39:26.627236 datamate-0.1.9/PKG-INFO
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968     3642 2023-03-06 13:58:32.000000 datamate-0.1.9/README.md
+drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-03 21:39:26.622092 datamate-0.1.9/datamate/
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968      647 2023-05-03 21:21:07.000000 datamate-0.1.9/datamate/__init__.py
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968    58283 2023-05-03 21:30:55.000000 datamate-0.1.9/datamate/directory.py
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968    11921 2023-05-01 17:35:54.000000 datamate-0.1.9/datamate/namespaces.py
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968       22 2023-05-03 21:32:04.000000 datamate-0.1.9/datamate/version.py
+drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-03 21:39:26.625124 datamate-0.1.9/datamate.egg-info/
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968     3829 2023-05-03 21:39:26.000000 datamate-0.1.9/datamate.egg-info/PKG-INFO
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968      331 2023-05-03 21:39:26.000000 datamate-0.1.9/datamate.egg-info/SOURCES.txt
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968        1 2023-05-03 21:39:26.000000 datamate-0.1.9/datamate.egg-info/dependency_links.txt
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968      109 2023-05-03 21:39:26.000000 datamate-0.1.9/datamate.egg-info/requires.txt
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968        9 2023-05-03 21:39:26.000000 datamate-0.1.9/datamate.egg-info/top_level.txt
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968       38 2023-05-03 21:39:26.628046 datamate-0.1.9/setup.cfg
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968      926 2023-05-01 19:20:47.000000 datamate-0.1.9/setup.py
+drwxr-xr-x   0 lappalainenj (1483866292) 1899195968        0 2023-05-03 21:39:26.626639 datamate-0.1.9/tests/
+-rwxr-xr-x   0 lappalainenj (1483866292) 1899195968    30672 2023-05-03 21:20:18.000000 datamate-0.1.9/tests/test_directory.py
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968     3734 2023-05-03 21:20:00.000000 datamate-0.1.9/tests/test_namespaces.py
+-rw-r--r--   0 lappalainenj (1483866292) 1899195968     2299 2023-05-03 21:38:37.000000 datamate-0.1.9/tests/test_swmr.py
```

### Comparing `datamate-0.1.8/PKG-INFO` & `datamate-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamate
-Version: 0.1.8
+Version: 0.1.9
 Summary: A data organization and compilation system.
 Author: Janne Lappalainen & Mason McGill
 Description-Content-Type: text/markdown
 
 # Datamate
 
 Datamate is a lightweight data and configuration management framework for structuring data in machine learning projects on a hierarchical filesystem.
```

### Comparing `datamate-0.1.8/README.md` & `datamate-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `datamate-0.1.8/datamate/__init__.py` & `datamate-0.1.9/datamate/__init__.py`

 * *Files identical despite different names*

### Comparing `datamate-0.1.8/datamate/directory.py` & `datamate-0.1.9/datamate/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,34 @@
     Mapping,
     MutableMapping,
     Optional,
     Tuple,
     Dict,
     Union,
     cast,
-    get_origin
+    get_origin,
 )
 from typing_extensions import Protocol
 import datetime
 from traceback import format_tb
 
 
 from contextlib import contextmanager
 
 import h5py as h5
 import numpy as np
 from pandas import DataFrame
 
-from datamate.namespaces import Namespace, namespacify, is_disjoint, is_superset, to_dict
+from datamate.namespaces import (
+    Namespace,
+    namespacify,
+    is_disjoint,
+    is_superset,
+    to_dict,
+)
 
 __all__ = ["Directory", "ArrayFile"]
 
 # -- Custom Errors and Warnings ------------------------------------------------
 
 
 class ConfigWarning(Warning):
@@ -133,14 +139,15 @@
     Example:
         with set_root_context(new_dir):
             dir = MyDirectory(...)
     """
 
     def decorator(callable):
         if inspect.isfunction(callable):
+
             @functools.wraps(callable)
             def function(*args, **kwargs):
                 _root_dir = get_root_dir()
                 within_context = getattr(context, "within_root_context", False)
                 # case 1: root_dir provided
                 if root_dir is not None and not within_context:
                     set_root_dir(root_dir)
@@ -149,14 +156,15 @@
                 # case 4: root dir not provided and not within context
                 # case 5: root dir not provided and within context
                 else:
                     set_root_dir(_root_dir)
                 _return = callable(*args, **kwargs)
                 set_root_dir(_root_dir)
                 return _return
+
             return function
         elif inspect.isclass(callable):
             new = callable.__new__
 
             @functools.wraps(callable)
             def function(*args, **kwargs):
                 _root_dir = get_root_dir()
@@ -175,16 +183,18 @@
                 return _return
 
             callable.__new__ = function
 
             return callable
         else:
             raise ValueError
+
     return decorator
 
+
 @contextmanager
 def set_root_context(root_dir: Union[str, Path, NoneType] = None):
     """Set root directory within a context and revert after.
 
     Example:
         with set_root_context(dir):
             Directory(config)
@@ -209,14 +219,15 @@
 #     _in_memory = getattr(context, "in_memory", False)
 #     context.in_memory = True
 #     try:
 #         yield
 #     finally:
 #         context.in_memory = _in_memory
 
+
 def enforce_config_match(enforce: bool) -> None:
     """
     Enforce error if configs are not matching.
 
     Defaults to True.
 
     Configs are compared, when initializing a directory
@@ -311,29 +322,26 @@
         path Union[str, Path]: The path at which the Directory is, or should be,
             stored, can be relative to the current `root_dir`.
         config Dict[str, object]: The configuration of the Directory.
             When including a "type" field indicates the type of Directory to
             search for and construct in the scope. Note, the config can be
             unpacked into the constructor as keyword arguments.
 
-    Constructors:
-         - Directory(): creates auto-named Directory inside the current
-            `root_dir`.
-         - Directory(config: Dict[str, object]): creates auto-named Directory inside
-            the current `root_dir` with the given config. If __init__ is
-            implemented, it will be called with the config as keyword arguments.
-         - Directory(path: Union[str, Path]): creates named Directory inside the
-             current `root_dir`. `path` will be either relative to the current
-                `root_dir` or absolute.
-         - Directory(path: Union[str, Path], config: Dict[str, object]): creates
-            named Directory inside the
-             current `root_dir`. `path` will be either relative to the current
-                `root_dir` or absolute. If __init__ is
-            implemented, it will be called with the config as keyword arguments.
+    Valid constructors:
+            To auto-name Directorys relative to `root_dir`:
+            - Directory()
+            - Directory(config: Dict[str, object])
+
+            To name Directorys relative to `root_dir` or absolute:
+            - Directory(path: Union[str, Path])
+            - Directory(path: Union[str, Path], config: Dict[str, object])
+            Note, config can also be passed as keyword arguments after
+            `path`.
 
+    If __init__ is implemented, it will be called to build the Directory.
 
     If only `path` is provided, the corresponding Directory is
     returned. It will be empty if `path` points to an empty or nonexistent
     directory.
 
     If only `config` is provided, it will search the current `root_dir`
     for a matching directory, and return a Directory pointing there if it
@@ -996,19 +1004,22 @@
 
     # <invalid signature>
     else:
         raise TypeError(
             "Invalid argument types for the `Directory` constructor.\n"
             "Valid signatures:\n"
             "\n"
-            "    - Directory(conf: Mapping[str, object])\n"
-            "    - Directory(path: Path|str)\n"
-            "    - Directory(path: Path|str, conf: Mapping[str, object])\n"
+            "    - Directory()\n"
+            "    - Directory(config: Dict[str, object])\n"
+            "    - Directory(path: Path)\n"
+            "    - Directory(path: Path, config: Dict[str, object])\n"
             "    - Directory(name: str)\n"
-            "    - Directory(name: str, conf: Mapping[str, object])"
+            "    - Directory(name: str, config: Dict[str, object])"
+            "Note, config can also be passed as keyword arguments after "
+            "`path` or `name`. `name` is relative to the root directory."
         )
 
 
 def _implements_init(cls: Directory) -> bool:
     """True if the class implements `__init__`."""
     return inspect.getsource(cls.__init__).split("\n")[-2].replace(" ", "") != "pass"
 
@@ -1018,15 +1029,18 @@
     # check if Config only has annotations, no defaults
     annotations = get_annotations(cls)
 
     if _implements_init(cls) and not defaults and not annotations:
         with warnings.catch_warnings():
             warnings.simplefilter("always")
             warnings.warn(
-                (f"The Directory {type(cls)} implements __init__ but not Config."),
+                (
+                    f"The Directory {type(cls)} implements __init__ to write data"
+                    " but specifies no configuration."
+                ),
                 ImplementationWarning,
                 stacklevel=2,
             )
 
 
 def _directory(cls: type) -> Directory:
     """
@@ -1238,24 +1252,22 @@
         write_meta(config=config, status="done")
     except BaseException as e:
         write_meta(config=config, status="stopped")
         raise e
 
 
 def call_signature(cls):
-    signature = (
-"""
+    signature = """
 
 Example call signature:
     {}
     {}
 Note, these use the `Directory(config: Dict[str, object])` constructor and are
 inferred from defaults and annotations, i.e. they are equivalent to constructing
 without arguments."""
-)
     defaults = to_dict(get_defaults(cls))
     string = ""
     for key, val in defaults.items():
         string += f"{key}={val}, "
     if string.endswith(", "):
         string = string[:-2]
     # variant 1: unpacking config kwargs
@@ -1270,37 +1282,38 @@
     if signature1 and signature2:
         return signature.format(signature1, signature2)
 
     return signature.format("(specify defaults for auto-doc of call signature)", "")
 
 
 def type_signature(cls):
-    signature = (
-    """
+    signature = """
 
     Types of config elements:
        {}
 
     """
-    )
     annotations = to_dict(get_annotations(cls))
+
     def qualname(annotation):
         origin = get_origin(annotation)
         if origin:
             return repr(annotation)
         return annotation.__qualname__
+
     signature1 = ""
     for key, val in annotations.items():
         signature1 += f"{key}: {qualname(val)}, "
     if signature1.endswith(", "):
         signature1 = signature1[:-2]
     if signature1:
         return signature.format(signature1)
     return signature.format("(annotate types for auto-doc of type signature)")
 
+
 def _auto_doc(cls: type, cls_doc=True, base_doc=False):
     docstring = "{}{}{}{}"
     if isinstance(cls, Directory):
         cls = type(cls)
     call_sig = call_signature(cls)
     type_sig = type_signature(cls)
 
@@ -1310,14 +1323,15 @@
 
     _base_doc = ""
     if base_doc and cls.__base__.__doc:
         _base_doc = cls.__base__.__doc__
 
     return docstring.format(_cls_doc, call_sig, type_sig, _base_doc)
 
+
 def _resolve_path(path: Path) -> Path:
     """
     Dereference ".", "..", "~", and "@".
     """
     if path.parts[0] == "@":
         path = get_root_dir() / "/".join(path.parts[1:])
     return path.expanduser().resolve()
@@ -1383,22 +1397,40 @@
     cls_override = config.pop("type", None)
     if isinstance(cls_override, type):
         cls = cls_override
     elif isinstance(cls_override, str):
         try:
             cls = get_scope()[cls_override]
         except KeyError as e:
-            raise KeyError(
-                f'"{cls_override}" can\'t be resolved because it is not found'
-                + f" inside the current scope of Directory subclasses."
-                + " If this happens unexpectedly with autoreload enabled in"
-                + " a notebook/IPython session, run `datamate.reset_scope(datamate.Directory)`"
-                + " as a workaround or restart the kernel"
-                + f" (background: https://github.com/ipython/ipython/issues/12399)."
-            ) from e
+            cls = type(cls_override, (Directory,), {})
+            with warnings.catch_warnings():
+                warnings.simplefilter("always")
+                warnings.warn(
+                    (
+                        "Casting to a new subclass of Directory because "
+                        f'"{cls_override}" can\'t be resolved as it is not found'
+                        + f" inside the current scope of Directory subclasses."
+                        + " This dynamically created subclass allows to view the data"
+                        + " without access to the original class definition and methods."
+                        + " If this happens unexpectedly with autoreload enabled in"
+                        + " a notebook/IPython session, run `datamate.reset_scope(datamate.Directory)`"
+                        + " as a workaround or restart the kernel"
+                        + f" (background: https://github.com/ipython/ipython/issues/12399)."
+                    ),
+                    ConfigWarning,
+                    stacklevel=2,
+                )
+            # raise KeyError(
+            #     f'"{cls_override}" can\'t be resolved because it is not found'
+            #     + f" inside the current scope of Directory subclasses."
+            #     + " If this happens unexpectedly with autoreload enabled in"
+            #     + " a notebook/IPython session, run `datamate.reset_scope(datamate.Directory)`"
+            #     + " as a workaround or restart the kernel"
+            #     + f" (background: https://github.com/ipython/ipython/issues/12399)."
+            # ) from e
 
     # Construct and return a Directory instance
     obj = object.__new__(cls)
     default_config = get_defaults(cls)
     default_config.update(config)
     config = Namespace(type=_identify(type(obj)), **default_config)
     object.__setattr__(obj, "_config", namespacify(config))
@@ -1513,14 +1545,15 @@
             # workaround if dataset was first created as non-chunked
             # using __setitem__ and then extended using extend
             if "Only chunked datasets can be resized" in str(e):
                 _override_to_chunked(path, val)
             else:
                 raise e
 
+
 def _copy_file(dst: Path, src: Path) -> None:
     # shutil.rmtree(dst, ignore_errors=True)
     dst.parent.mkdir(parents=True, exist_ok=True)
     shutil.copy(src, dst)
 
 
 def _copy_dir(dst: Path, src: Path) -> None:
```

### Comparing `datamate-0.1.8/datamate/namespaces.py` & `datamate-0.1.9/datamate/namespaces.py`

 * *Files identical despite different names*

### Comparing `datamate-0.1.8/datamate.egg-info/PKG-INFO` & `datamate-0.1.9/datamate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamate
-Version: 0.1.8
+Version: 0.1.9
 Summary: A data organization and compilation system.
 Author: Janne Lappalainen & Mason McGill
 Description-Content-Type: text/markdown
 
 # Datamate
 
 Datamate is a lightweight data and configuration management framework for structuring data in machine learning projects on a hierarchical filesystem.
```

### Comparing `datamate-0.1.8/setup.py` & `datamate-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `datamate-0.1.8/tests/test_directory.py` & `datamate-0.1.9/tests/test_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import threading
+import time
 from pathlib import Path
 from typing import List
 
 import h5py as h5
 import numpy as np
 import pytest
 import shutil
@@ -16,15 +18,15 @@
 )
 from datamate.directory import (
     ModifiedError,
     ModifiedWarning,
     ConfigWarning,
     ImplementationWarning,
     ImplementationError,
-    _auto_doc
+    _auto_doc,
 )
 
 # -- Helper functions ----------------------------------------------------------
 
 
 def data_file(path: Path) -> Path:
     path.parent.mkdir(parents=True, exist_ok=True)
@@ -34,28 +36,32 @@
 
 def data_file_concat(path: Path, args: List[Path]) -> Path:
     path.parent.mkdir(parents=True, exist_ok=True)
     path.write_bytes(b"".join(a.read_bytes() for a in args))
     return path
 
 
-def assert_directory_equals(directory: Directory, target: dict) -> None:
+def assert_attributes_equal(directory: Directory, target: dict) -> None:
     if "__type__" in target:
         assert isinstance(directory, target.pop("__type__"))
     if "__path__" in target:
         assert directory.path == target.pop("__path__")
     if "__conf__" in target:
         assert directory._config == target.pop("__conf__")
     if "__meta__" in target:
         assert directory.meta == target.pop("__meta__")
     if "__doc__" in target:
         assert directory.__doc__ == target.pop("__doc__")
     if "__exists__" in target:
         assert directory.path.exists() == target.pop("__exists__")
 
+
+def assert_directory_equals(directory: Directory, target: dict) -> None:
+    assert_attributes_equal(directory, target)
+
     assert len(directory) == len(target)
     assert len(list(directory)) == len(target)
 
     for k, v in target.items():
         assert k in directory
         assert k in list(directory)
         assert hasattr(directory, k)
@@ -277,18 +283,18 @@
                 ),
                 "e": {"f": [0.1, 0.2, 0.3, 0.4, 0.5]},
             }
         },
     )
     b = Directory(tmp_path / "b")
     b.b = {
-            "c": np.empty((0, 2), dtype="uint16"),
-            "d.bin": data_file(tmp_path / "d0.bin"),
-            "e": {"f": [0.1, 0.2]},
-        }
+        "c": np.empty((0, 2), dtype="uint16"),
+        "d.bin": data_file(tmp_path / "d0.bin"),
+        "e": {"f": [0.1, 0.2]},
+    }
     b.extend(
         "b",
         {
             "c": np.uint16([[1, 2], [3, 4]]),
             "d.bin": data_file(tmp_path / "d1.bin"),
             "e": {"f": [0.3, 0.4, 0.5]},
         },
@@ -409,25 +415,28 @@
 
 def test_construction_from_nothing(tmp_path: Path) -> None:
     # Setup
     set_root_dir(tmp_path)
     AnotherDirectory.Config.n_calls = 0
 
     # Case 1: (not exists)
-    a0 = AnotherDirectory()
+    with pytest.warns(ImplementationWarning):
+        a0 = AnotherDirectory()
     assert AnotherDirectory.Config.n_calls == 0
 
     # Case 2: (exists, empty)
     path = a0.path
-    a1 = AnotherDirectory()
+    with pytest.warns(ImplementationWarning):
+        a1 = AnotherDirectory()
     assert path == a1.path
 
     # Case 3: (exists, non-empty)
     a0.__init__()
-    a1 = AnotherDirectory()
+    with pytest.warns(ImplementationWarning):
+        a1 = AnotherDirectory()
     assert AnotherDirectory.Config.n_calls == 1
 
     # Cleanup
     set_root_dir(Path("."))
 
 
 def test_construction_from_path(tmp_path: Path) -> None:
@@ -587,42 +596,42 @@
     RootedDirectory, rooted_dir_root_path = rooted_dir
 
     assert rooted_dir_root_path != tmp_path
 
     # case 1: root dir provided in decorator
     dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
     assert_directory_equals(
-            dir,
-            dict(
-                __type__=RootedDirectory,
-                __path__= rooted_dir_root_path / dir.path.name,
-                array=np.arange(0, 10, 1),
-            ),
-        )
+        dir,
+        dict(
+            __type__=RootedDirectory,
+            __path__=rooted_dir_root_path / dir.path.name,
+            array=np.arange(0, 10, 1),
+        ),
+    )
 
     # case 2: root dir provided and not within context
     set_root_dir(tmp_path)
     dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
     assert_directory_equals(
-            dir,
-            dict(
-                __type__=RootedDirectory,
-                __path__= rooted_dir_root_path / dir.path.name,
-                array=np.arange(0, 10, 1),
-            ),
-        )
+        dir,
+        dict(
+            __type__=RootedDirectory,
+            __path__=rooted_dir_root_path / dir.path.name,
+            array=np.arange(0, 10, 1),
+        ),
+    )
 
     # case 3: root_dir provided and within context
     with set_root_context(tmp_path):
         dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
         assert_directory_equals(
             dir,
             dict(
                 __type__=RootedDirectory,
-                __path__= tmp_path / dir.path.name,
+                __path__=tmp_path / dir.path.name,
                 array=np.arange(0, 10, 1),
             ),
         )
 
 
 @root()
 class RootedDirectory(Directory):
@@ -630,35 +639,38 @@
         self.array = np.arange(config.start, config.stop, config.step)
 
 
 def test_root_dir_not_provided(tmp_path):
     set_root_dir(tmp_path)
 
     # case 4: root dir not provided and not within context
-    dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
+    with pytest.warns(ImplementationWarning):
+        dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
     assert_directory_equals(
-            dir,
-            dict(
-                __type__=RootedDirectory,
-                __path__= tmp_path / dir.path.name,
-                array=np.arange(0, 10, 1),
-            ),
+        dir,
+        dict(
+            __type__=RootedDirectory,
+            __path__=tmp_path / dir.path.name,
+            array=np.arange(0, 10, 1),
+        ),
     )
     # case 5: root dir not provided and within context
     with set_root_context(tmp_path / "subdir"):
-        dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
+        with pytest.warns(ImplementationWarning):
+            dir = RootedDirectory(Namespace(start=0, stop=10, step=1))
         assert_directory_equals(
             dir,
             dict(
                 __type__=RootedDirectory,
-                __path__= tmp_path / "subdir" / dir.path.name,
+                __path__=tmp_path / "subdir" / dir.path.name,
                 array=np.arange(0, 10, 1),
             ),
         )
 
+
 # -- test default config
 
 
 class DefaultConfigDir(Directory):
     class Config:
         x: int = 2
 
@@ -780,15 +792,15 @@
                 __type__=BadImplementation,
                 __path__=tmp_path / dir.path.name,
                 __conf__=Namespace(type="BadImplementation", x=2),
                 __meta__={
                     "config": {"type": "BadImplementation", "x": 2},
                     "status": "done",
                 },
-                x=np.arange(2)
+                x=np.arange(2),
             ),
         )
 
     with pytest.warns(ImplementationWarning):
         dir = BadImplementation(tmp_path / "test10", dict(x=2))
         assert_directory_equals(
             dir,
@@ -796,15 +808,15 @@
                 __type__=BadImplementation,
                 __path__=tmp_path / "test10",
                 __conf__=Namespace(type="BadImplementation", x=2),
                 __meta__={
                     "config": {"type": "BadImplementation", "x": 2},
                     "status": "done",
                 },
-                x=np.arange(2)
+                x=np.arange(2),
             ),
         )
 
     # config has no default attributes but directory has init, with custom, wrong config
     with pytest.raises(AttributeError):
         with pytest.warns(ImplementationWarning):
             dir = BadImplementation(dict(y=2))
@@ -812,14 +824,15 @@
     with pytest.raises(AttributeError):
         with pytest.warns(ImplementationWarning):
             dir = BadImplementation(tmp_path / "test12", dict(y=2))
 
 
 # -- test auto docstring
 
+
 class AutoDocConfigDir(Directory):
     """Dir to test auto docstring based on config."""
 
     class Config:
         x: int = 2
         y: float = 2.0
         q = Namespace(a=1, b=2)
@@ -862,15 +875,17 @@
     """Dir to test auto docstring based on config."""
 
     pass
 
 
 def test_auto_doc(tmp_path):
     a = AutoDocConfigDir()
-    doc = "Dir to test auto docstring based on config.{}".format(_auto_doc(a, cls_doc=False))
+    doc = "Dir to test auto docstring based on config.{}".format(
+        _auto_doc(a, cls_doc=False)
+    )
     # breakpoint()
     assert_directory_equals(
         a,
         dict(
             __doc__=doc,
             __exists__=False,
         ),
@@ -901,15 +916,17 @@
         dict(
             __doc__=doc.replace("SoloConfigDocDir", "SoloInitDocDir"),
             __exists__=False,
         ),
     )
 
     c = EmptyConfigDocDir()
-    doc = "Dir to test auto docstring based on config.{}".format(_auto_doc(c, cls_doc=False))
+    doc = "Dir to test auto docstring based on config.{}".format(
+        _auto_doc(c, cls_doc=False)
+    )
     assert_directory_equals(
         c,
         dict(
             __doc__=doc,
             __exists__=False,
         ),
     )
@@ -920,15 +937,17 @@
         dict(
             __doc__=doc,
             __exists__=False,
         ),
     )
 
     d = NoConfigDocDir()
-    doc = "Dir to test auto docstring based on config.{}".format(_auto_doc(d, cls_doc=False))
+    doc = "Dir to test auto docstring based on config.{}".format(
+        _auto_doc(d, cls_doc=False)
+    )
     assert_directory_equals(
         d,
         dict(__doc__=doc, __exists__=False),
     )
 
 
 # --- test default config and init from init kwargs
@@ -940,47 +959,56 @@
         self.bar = bar
 
 
 def test_init_from_kwargs(tmp_path):
     set_root_dir(tmp_path)
     dir = SmartDir()
     assert_directory_equals(
-            dir,
-            dict(
-                __path__=tmp_path / dir.path.name,
-                __conf__=Namespace(type="SmartDir", foo=2, bar=3),
-                __meta__={"config": {"type": "SmartDir", "foo": 2, "bar": 3}, "status": "done"},
-                foo=2,
-                bar=3
-            ),
+        dir,
+        dict(
+            __path__=tmp_path / dir.path.name,
+            __conf__=Namespace(type="SmartDir", foo=2, bar=3),
+            __meta__={
+                "config": {"type": "SmartDir", "foo": 2, "bar": 3},
+                "status": "done",
+            },
+            foo=2,
+            bar=3,
+        ),
     )
 
     dir = SmartDir(foo=5, bar=1)
     assert_directory_equals(
-            dir,
-            dict(
-                __path__=tmp_path / dir.path.name,
-                __conf__=Namespace(type="SmartDir", foo=5, bar=1),
-                __meta__={"config": {"type": "SmartDir", "foo": 5, "bar": 1}, "status": "done"},
-                foo=5,
-                bar=1
-            ),
+        dir,
+        dict(
+            __path__=tmp_path / dir.path.name,
+            __conf__=Namespace(type="SmartDir", foo=5, bar=1),
+            __meta__={
+                "config": {"type": "SmartDir", "foo": 5, "bar": 1},
+                "status": "done",
+            },
+            foo=5,
+            bar=1,
+        ),
     )
     name = dir.path.name
 
     dir = SmartDir(name)
     assert_directory_equals(
-            dir,
-            dict(
-                __path__=tmp_path / name,
-                __conf__=Namespace(type="SmartDir", foo=5, bar=1),
-                __meta__={"config": {"type": "SmartDir", "foo": 5, "bar": 1}, "status": "done"},
-                foo=5,
-                bar=1
-            ),
+        dir,
+        dict(
+            __path__=tmp_path / name,
+            __conf__=Namespace(type="SmartDir", foo=5, bar=1),
+            __meta__={
+                "config": {"type": "SmartDir", "foo": 5, "bar": 1},
+                "status": "done",
+            },
+            foo=5,
+            bar=1,
+        ),
     )
 
     with pytest.raises(FileExistsError):
         dir = SmartDir(dir.path.name, foo=3, bar=2)
 
 
 # --- test directory with Config but without init
@@ -1001,29 +1029,29 @@
 
 
 def test_directory_with_config_without_init(tmp_path):
     set_root_dir(tmp_path)
 
     nnd = NetworkDir()
     assert_directory_equals(
-            nnd,
-            dict(
-                __conf__=Namespace(type="NetworkDir", tau=200.0, sigma=0.1),
-                __exists__=False,
-            ),
+        nnd,
+        dict(
+            __conf__=Namespace(type="NetworkDir", tau=200.0, sigma=0.1),
+            __exists__=False,
+        ),
     )
 
     nnd = NetworkDir(tmp_path / "test")
     assert_directory_equals(
-            nnd,
-            dict(
-                __path__=tmp_path / "test",
-                __conf__=Namespace(type="NetworkDir", tau=200.0, sigma=0.1),
-                __exists__=False,
-            ),
+        nnd,
+        dict(
+            __path__=tmp_path / "test",
+            __conf__=Namespace(type="NetworkDir", tau=200.0, sigma=0.1),
+            __exists__=False,
+        ),
     )
 
 
 # --- test merge of defaults
 
 
 class ConIni1(Directory):
@@ -1033,22 +1061,23 @@
     def __init__(self, tau=200):
         pass
 
 
 def test_cross_configs(tmp_path):
     dir = ConIni1()
     assert_directory_equals(
-            dir,
-            dict(
-                __conf__=Namespace(type="ConIni1", tau=200.0, sigma=0.1),
-                __exists__=False,
-            ),
+        dir,
+        dict(
+            __conf__=Namespace(type="ConIni1", tau=200.0, sigma=0.1),
+            __exists__=False,
+        ),
     )
 
     with pytest.raises(ValueError):
+
         class ConIni2(Directory):
             class Config:
                 tau: float = 200.0
                 sigma: float = 0.1
 
             def __init__(self, sigma=2):
                 pass
```

### Comparing `datamate-0.1.8/tests/test_namespaces.py` & `datamate-0.1.9/tests/test_namespaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,25 +105,25 @@
         "    str = 'The quick brown fox jumped over the lazy dog.'\n"
         "  )\n"
         ")"
     )
 
 
 def test_all():
-    x = Namespace(a = Namespace(b = [1, 2, 3]))
+    x = Namespace(a=Namespace(b=[1, 2, 3]))
     assert x.all()
 
-    x = Namespace(a = Namespace(b = [1, 2, 0]))
+    x = Namespace(a=Namespace(b=[1, 2, 0]))
     assert not x.all()
 
     y = x.deepcopy()
     y.a.b = [4, 2, 1]
     assert not y == x
     assert y.all()
 
-    x = Namespace(a = np.arange(3))
-    y = Namespace(a = np.arange(1, 5))
+    x = Namespace(a=np.arange(3))
+    y = Namespace(a=np.arange(1, 5))
     assert not x.all() and y.all()
     assert y != x
 
-    y = Namespace(a = np.arange(3))
-    assert y == x
+    y = Namespace(a=np.arange(3))
+    assert y == x
```

