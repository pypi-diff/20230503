# Comparing `tmp/bridgestan-1.0.2.tar.gz` & `tmp/bridgestan-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bridgestan-1.0.2.tar", last modified: Wed Mar 22 13:23:20 2023, max compression
+gzip compressed data, was "bridgestan-2.0.0.tar", last modified: Wed May  3 16:14:12 2023, max compression
```

## Comparing `bridgestan-1.0.2.tar` & `bridgestan-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:23:20.045055 bridgestan-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-22 13:23:20.045055 bridgestan-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-22 13:22:16.000000 bridgestan-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:23:20.041055 bridgestan-1.0.2/bridgestan/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-22 13:22:16.000000 bridgestan-1.0.2/bridgestan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-22 13:22:44.000000 bridgestan-1.0.2/bridgestan/__version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-03-22 13:22:16.000000 bridgestan-1.0.2/bridgestan/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-22 13:22:16.000000 bridgestan-1.0.2/bridgestan/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    21047 2023-03-22 13:22:16.000000 bridgestan-1.0.2/bridgestan/model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 13:22:16.000000 bridgestan-1.0.2/bridgestan/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-22 13:22:16.000000 bridgestan-1.0.2/bridgestan/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:23:20.045055 bridgestan-1.0.2/bridgestan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-22 13:23:20.000000 bridgestan-1.0.2/bridgestan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-22 13:23:20.000000 bridgestan-1.0.2/bridgestan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:23:20.000000 bridgestan-1.0.2/bridgestan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-22 13:23:20.000000 bridgestan-1.0.2/bridgestan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 13:23:20.000000 bridgestan-1.0.2/bridgestan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-22 13:22:16.000000 bridgestan-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-22 13:23:20.045055 bridgestan-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-22 13:22:16.000000 bridgestan-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:23:20.045055 bridgestan-1.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-22 13:22:16.000000 bridgestan-1.0.2/test/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-22 13:22:16.000000 bridgestan-1.0.2/test/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-03-22 13:22:16.000000 bridgestan-1.0.2/test/test_stanmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:12.305067 bridgestan-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-03 16:14:12.305067 bridgestan-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-03 16:13:14.000000 bridgestan-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:12.305067 bridgestan-2.0.0/bridgestan/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 16:13:14.000000 bridgestan-2.0.0/bridgestan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 16:13:39.000000 bridgestan-2.0.0/bridgestan/__version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-03 16:13:14.000000 bridgestan-2.0.0/bridgestan/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-03 16:13:14.000000 bridgestan-2.0.0/bridgestan/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25803 2023-05-03 16:13:14.000000 bridgestan-2.0.0/bridgestan/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 16:13:14.000000 bridgestan-2.0.0/bridgestan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-03 16:13:14.000000 bridgestan-2.0.0/bridgestan/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:12.305067 bridgestan-2.0.0/bridgestan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-03 16:14:12.000000 bridgestan-2.0.0/bridgestan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-03 16:14:12.000000 bridgestan-2.0.0/bridgestan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:14:12.000000 bridgestan-2.0.0/bridgestan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 16:14:12.000000 bridgestan-2.0.0/bridgestan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 16:14:12.000000 bridgestan-2.0.0/bridgestan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 16:13:14.000000 bridgestan-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-03 16:14:12.305067 bridgestan-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-03 16:13:14.000000 bridgestan-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:12.305067 bridgestan-2.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-03 16:13:14.000000 bridgestan-2.0.0/test/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-03 16:13:14.000000 bridgestan-2.0.0/test/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25460 2023-05-03 16:13:14.000000 bridgestan-2.0.0/test/test_stanmodel.py
```

### Comparing `bridgestan-1.0.2/PKG-INFO` & `bridgestan-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bridgestan
-Version: 1.0.2
+Version: 2.0.0
 Home-page: https://github.com/roualdes/bridgestan
 Author: Brian Ward, Edward Roualdes, Bob Carpenter
 License: BSD 3-Clause License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # bridgestan.py - The Python interface to BridgeStan
 
-[View the Python interface documentation online](https://roualdes.github.io/bridgestan/languages/python.html)
+[View the Python interface documentation online](https://roualdes.github.io/bridgestan/latest/languages/python.html)
 
 ## Installation
 
 **From PyPI**:
 ```shell
 pip install bridgestan
 ```
```

### Comparing `bridgestan-1.0.2/bridgestan/compile.py` & `bridgestan-2.0.0/bridgestan/compile.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import platform
 import subprocess
 from pathlib import Path
 from typing import List
 
-from .util import validate_readable
 from .__version import __version__
 from .download import CURRENT_BRIDGESTAN, get_bridgestan_src
+from .util import validate_readable
 
 
 def verify_bridgestan_path(path: str) -> None:
     folder = Path(path).resolve()
     if not folder.exists():
         raise ValueError(
             f"BridgeStan folder '{folder}' does not exist!\n"
```

### Comparing `bridgestan-1.0.2/bridgestan/download.py` & `bridgestan-2.0.0/bridgestan/download.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from pathlib import Path
-import urllib.request
-import urllib.error
 import tarfile
+import urllib.error
+import urllib.request
+from pathlib import Path
 from time import sleep
 
 from .__version import __version__
 
 HOME_BRIDGESTAN = Path("~").expanduser() / ".bridgestan"
 CURRENT_BRIDGESTAN = HOME_BRIDGESTAN / f"bridgestan-{__version__}"
```

### Comparing `bridgestan-1.0.2/bridgestan/model.py` & `bridgestan-2.0.0/bridgestan/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,112 @@
 import ctypes
+import warnings
 from typing import List, Optional, Tuple
 
 import numpy as np
 import numpy.typing as npt
 from numpy.ctypeslib import ndpointer
 
+from .__version import __version_info__
 from .compile import compile_model
 from .util import validate_readable
 
 FloatArray = npt.NDArray[np.float64]
 double_array = ndpointer(dtype=ctypes.c_double, flags=("C_CONTIGUOUS"))
+star_star_char = ctypes.POINTER(ctypes.c_char_p)
+c_print_callback = ctypes.CFUNCTYPE(None, ctypes.POINTER(ctypes.c_char), ctypes.c_int)
+
+
+@c_print_callback
+def _print_callback(s, n):
+    print(ctypes.string_at(s, n).decode("utf-8"), end="")
 
 
 class StanModel:
     """
     A StanModel instance encapsulates a Stan model instantiated with data
     and provides methods to access parameter names, transforms, log
     densities, gradients, and Hessians.
-
-    The constructor method instantiates a Stan model and sets constant
-    return values.  The constructor arguments are
-
-    :param model_lib: A path to a compiled shared object.
-    :param model_data: Either a JSON string literal or a
-         path to a data file in JSON format ending in ``.json``.
-    :param seed: A pseudo random number generator seed.
-    :param chain_id: A unique identifier for concurrent chains of
-        pseudorandom numbers.
-    :raises FileNotFoundError or PermissionError: If ``model_lib`` is not readable or
-        ``model_data`` is specified and not a path to a readable file.
-    :raises RuntimeError: If there is an error instantiating the Stan model.
     """
 
     def __init__(
         self,
         model_lib: str,
         model_data: Optional[str] = None,
         *,
         seed: int = 1234,
-        chain_id: int = 0,
+        capture_stan_prints: bool = True,
     ) -> None:
         """
-        Construct a StanModel object for a Stan model and data given
+        Construct a StanModel object for a compiled Stan model and data given
         constructor arguments.
 
         :param model_lib: A system path to compiled shared object.
-        :param model_data: Either a JSON string literal or a
-            system path to a data file in JSON format ending in ``.json``.
-        :param seed: A pseudo random number generator seed.
-        :param chain_id: A unique identifier for concurrent chains of
-            pseudorandom numbers.
+        :param model_data: Either a JSON string literal, a
+            system path to a data file in JSON format ending in ``.json``,
+            or the empty string.
+        :param seed: A pseudo random number generator seed, used for RNG functions
+            in the ``transformed data`` block.
+        :param capture_stan_prints: If ``True``, capture all ``print`` statements
+            from the Stan model and print them from Python. This has no effect if
+            the model does not contain any ``print`` statements, but may have
+            a performance impact if it does. If ``False``, ``print`` statements
+            from the Stan model will be sent to ``cout`` and will not be seen in
+            Jupyter or capturable with :func:`contextlib.redirect_stdout`.
+
+            **Note:** If this is set for a model, any other models instantiated
+            from the *same shared library* will also have the callback set, even
+            if they were created *before* this model.
         :raises FileNotFoundError or PermissionError: If ``model_lib`` is not readable or
             ``model_data`` is specified and not a path to a readable file.
         :raises RuntimeError: If there is an error instantiating the
             model from C++.
         """
         validate_readable(model_lib)
-        if not model_data is None and model_data.endswith('.json'):
+        if  model_data is not None and model_data.endswith(".json"):
             validate_readable(model_data)
+            with open(model_data, "r") as f:
+                model_data = f.read()
+
         self.lib_path = model_lib
         self.stanlib = ctypes.CDLL(self.lib_path)
-        self.data_path = model_data or ""
+
+        self.data = model_data or ""
         self.seed = seed
-        self.chain_id = chain_id
 
-        self._construct = self.stanlib.bs_construct
+        self._construct = self.stanlib.bs_model_construct
         self._construct.restype = ctypes.c_void_p
-        self._construct.argtypes = [ctypes.c_char_p, ctypes.c_uint, ctypes.c_uint]
-
-        self.model_rng = self._construct(
-            str.encode(self.data_path), self.seed, self.chain_id
-        )
+        self._construct.argtypes = [
+            ctypes.c_char_p,
+            ctypes.c_uint,
+            star_star_char,
+        ]
 
-        if not self.model_rng:
-            raise RuntimeError("could not construct model RNG")
+        self._free_error = self.stanlib.bs_free_error_msg
+        self._free_error.restype = None
+        self._free_error.argtypes = [ctypes.c_char_p]
+
+        self._set_print_callback = self.stanlib.bs_set_print_callback
+        self._set_print_callback.restype = None
+        self._set_print_callback.argtypes = [c_print_callback, star_star_char]
+        if capture_stan_prints:
+            self._set_print_callback(_print_callback, None)
+
+        err = ctypes.pointer(ctypes.c_char_p())
+        self.model = self._construct(str.encode(self.data), self.seed, err)
+
+        if not self.model:
+            raise self._handle_error(err.contents, "bs_model_construct")
+
+        if self.model_version() != __version_info__:
+            warnings.warn(
+                "The version of the compiled model does not match the version of the "
+                "Python package. Consider recompiling the model.",
+                RuntimeWarning,
+            )
 
         self._name = self.stanlib.bs_name
         self._name.restype = ctypes.c_char_p
         self._name.argtypes = [ctypes.c_void_p]
 
         self._model_info = self.stanlib.bs_model_info
         self._model_info.restype = ctypes.c_char_p
@@ -107,393 +136,448 @@
         self._param_constrain.restype = ctypes.c_int
         self._param_constrain.argtypes = [
             ctypes.c_void_p,
             ctypes.c_int,
             ctypes.c_int,
             double_array,
             double_array,
+            ctypes.c_void_p,
+            star_star_char,
         ]
 
         self._param_unconstrain = self.stanlib.bs_param_unconstrain
         self._param_unconstrain.restype = ctypes.c_int
-        self._param_unconstrain.argtypes = [ctypes.c_void_p, double_array, double_array]
+        self._param_unconstrain.argtypes = [
+            ctypes.c_void_p,
+            double_array,
+            double_array,
+            star_star_char,
+        ]
 
         self._param_unconstrain_json = self.stanlib.bs_param_unconstrain_json
         self._param_unconstrain_json.restype = ctypes.c_int
         self._param_unconstrain_json.argtypes = [
             ctypes.c_void_p,
             ctypes.c_char_p,
             double_array,
+            star_star_char,
         ]
 
         self._log_density = self.stanlib.bs_log_density
         self._log_density.restype = ctypes.c_int
         self._log_density.argtypes = [
             ctypes.c_void_p,
             ctypes.c_int,
             ctypes.c_int,
             double_array,
             ctypes.POINTER(ctypes.c_double),
+            star_star_char,
         ]
 
         self._log_density_gradient = self.stanlib.bs_log_density_gradient
         self._log_density_gradient.restype = ctypes.c_int
         self._log_density_gradient.argtypes = [
             ctypes.c_void_p,
             ctypes.c_int,
             ctypes.c_int,
             double_array,
             ctypes.POINTER(ctypes.c_double),
             double_array,
+            star_star_char,
         ]
 
         self._log_density_hessian = self.stanlib.bs_log_density_hessian
         self._log_density_hessian.restype = ctypes.c_int
         self._log_density_hessian.argtypes = [
             ctypes.c_void_p,
             ctypes.c_int,
             ctypes.c_int,
             double_array,
             ctypes.POINTER(ctypes.c_double),
             double_array,
             double_array,
+            star_star_char,
         ]
 
-        self._destruct = self.stanlib.bs_destruct
-        self._destruct.restype = ctypes.c_int
+        self._destruct = self.stanlib.bs_model_destruct
+        self._destruct.restype = None
         self._destruct.argtypes = [ctypes.c_void_p]
 
     @classmethod
     def from_stan_file(
         cls,
         stan_file: str,
         model_data: Optional[str] = None,
         *,
         stanc_args: List[str] = [],
         make_args: List[str] = [],
         seed: int = 1234,
-        chain_id: int = 0,
+        capture_stan_prints: bool = True,
     ):
         """
         Construct a StanModel instance from a ``.stan`` file, compiling if necessary.
 
-        This is equivalent to calling :func:`bridgestan.compile_model` and then the
+        This is equivalent to calling :func:`bridgestan.compile_model`` and then the
         constructor of this class.
 
         :param stan_file: A path to a Stan model file.
         :param model_data: A path to data in JSON format.
         :param stanc_args: A list of arguments to pass to stanc3.
             For example, ``["--O1"]`` will enable compiler optimization level 1.
         :param make_args: A list of additional arguments to pass to Make.
             For example, ``["STAN_THREADS=True"]`` will enable
             threading for the compiled model. If the same flags are defined
             in ``make/local``, the versions passed here will take precedent.
-        :param seed: A pseudo random number generator seed.
-        :param chain_id: A unique identifier for concurrent chains of
-            pseudorandom numbers.
-        :raises FileNotFoundError or PermissionError: If `stan_file` does not exist
+        :param seed: A pseudo random number generator seed, used for RNG functions
+            in the ``transformed data`` block.
+        :param capture_stan_prints: If ``True``, capture all ``print`` statements
+            from the Stan model and print them from Python. This has no effect if
+            the model does not contain any ``print`` statements, but may have
+            a performance impact if it does. If ``False``, ``print`` statements
+            from the Stan model will be sent to ``cout`` and will not be seen in
+            Jupyter or capturable with ``contextlib.redirect_stdout``.
+        :raises FileNotFoundError or PermissionError: If ``stan_file`` does not exist
             or is not readable.
         :raises ValueError: If BridgeStan cannot be located.
         :raises RuntimeError: If compilation fails.
         """
         result = compile_model(stan_file, stanc_args=stanc_args, make_args=make_args)
-        return cls(str(result), model_data, seed=seed, chain_id=chain_id)
+        return cls(
+            str(result), model_data, seed=seed, capture_stan_prints=capture_stan_prints
+        )
 
     def __del__(self) -> None:
         """
         Destroy the Stan model and free memory.
         """
-        if hasattr(self, "model_rng") and hasattr(self, "_destruct"):
-            self._destruct(self.model_rng)
+        if hasattr(self, "model") and hasattr(self, "_destruct"):
+            self._destruct(self.model)
 
     def __repr__(self) -> str:
-        data = f"{self.data_path!r}, " if self.data_path else ""
-        return f"StanModel({self.lib_path!r}, {data}seed={self.seed}, chain_id={self.chain_id})"
+        data = f"{self.data!r}, " if self.data else ""
+        return f"StanModel({self.lib_path!r}, {data}, seed={self.seed})"
 
     def name(self) -> str:
         """
         Return the name of the Stan model.
 
         :return: The name of Stan model.
         """
-        return self._name(self.model_rng).decode("utf-8")
+        return self._name(self.model).decode("utf-8")
 
     def model_info(self) -> str:
         """
         Return compilation information about the model. For example,
         this includes the current Stan version and important
         compiler settings.
 
         :return: Information about the compiled Stan model.
         """
-        return self._model_info(self.model_rng).decode("utf-8")
+        return self._model_info(self.model).decode("utf-8")
+
+    def model_version(self) -> Tuple[int, int, int]:
+        """
+        Return the BridgeStan version of the compiled model.
+        """
+        return (
+            ctypes.c_int.in_dll(self.stanlib, "bs_major_version").value,
+            ctypes.c_int.in_dll(self.stanlib, "bs_minor_version").value,
+            ctypes.c_int.in_dll(self.stanlib, "bs_patch_version").value,
+        )
 
     def param_num(self, *, include_tp: bool = False, include_gq: bool = False) -> int:
         """
         Return the number of parameters, including transformed
         parameters and/or generated quantities as indicated.
 
-        :param include_tp: `True` to include the transformed parameters.
-        :param include_gq: `True` to include the generated quantities.
+        :param include_tp: ``True`` to include the transformed parameters.
+        :param include_gq: ``True`` to include the generated quantities.
         :return: The number of parameters.
         """
-        return self._param_num(self.model_rng, int(include_tp), int(include_gq))
+        return self._param_num(self.model, int(include_tp), int(include_gq))
 
     def param_unc_num(self) -> int:
         """
         Return the number of unconstrained parameters.
 
         :return: The number of unconstrained parameters.
         """
-        return self._param_unc_num(self.model_rng)
+        return self._param_unc_num(self.model)
 
     def param_names(
         self, *, include_tp: bool = False, include_gq: bool = False
     ) -> List[str]:
         """
         Return the indexed names of the parameters, including transformed
         parameters and/or generated quantities as indicated.  For
         containers, indexes are separated by periods (`.`).
-        For example, the scalar `a` has
-        indexed name `a`, the vector entry `a[1]` has indexed name `a.1`
-        and the matrix entry `a[2, 3]` has indexed name `a.2.3`.
+        For example, the scalar ``a`` has
+        indexed name ``a``, the vector entry ``a[1]`` has indexed name ``a.1``
+        and the matrix entry ``a[2, 3]`` has indexed name ``a.2.3``.
         Parameter order of the output is column major and more
         generally last-index major for containers.
 
-        :param include_tp: `True` to include transformed parameters.
-        :param include_gq: `True` to include generated quantities.
+        :param include_tp: ``True`` to include transformed parameters.
+        :param include_gq: ``True`` to include generated quantities.
         :return: The indexed names of the parameters.
         """
         return (
-            self._param_names(self.model_rng, int(include_tp), int(include_gq))
+            self._param_names(self.model, int(include_tp), int(include_gq))
             .decode("utf-8")
             .split(",")
         )
 
     def param_unc_names(self) -> List[str]:
         """
         Return the indexed names of the unconstrained parameters.
-        For example, a scalar unconstrained parameter `b` has indexed
-        name `b` and a vector entry `b[3]` has indexed name `b.3`.
+        For example, a scalar unconstrained parameter ``b`` has indexed
+        name ``b`` and a vector entry ``b[3]`` has indexed name ``b.3``.
 
         :return: The indexed names of the unconstrained parameters.
         """
-        return self._param_unc_names(self.model_rng).decode("utf-8").split(",")
+        return self._param_unc_names(self.model).decode("utf-8").split(",")
 
     def param_constrain(
         self,
         theta_unc: FloatArray,
         *,
         include_tp: bool = False,
         include_gq: bool = False,
         out: Optional[FloatArray] = None,
+        rng: Optional["StanRNG"] = None,
     ) -> FloatArray:
         """
         Return the constrained parameters derived from the specified
         unconstrained parameters as an array, optionally including the
         transformed parameters and/or generated quantitities as specified.
         Including generated quantities uses the PRNG and may update its state.
-        Setting `out` avoids allocation of a new array for the return value.
+        Setting ``out`` avoids allocation of a new array for the return value.
 
         :param theta_unc: Unconstrained parameter array.
-        :param include_tp: `True` to include transformed parameters.
-        :param include_gq: `True` to include generated quantities.
+        :param include_tp: ``True`` to include transformed parameters.
+        :param include_gq: ``True`` to include generated quantities.
         :param out: A location into which the result is stored.  If
-            provided, it must have shape `(D, )`, where `D` is the number of
-            constrained parameters.  If not provided or `None`, a freshly
+            provided, it must have shape ``(D, )``, where ``D`` is the number of
+            constrained parameters.  If not provided or ``None``, a freshly
             allocated array is returned.
+        :param rng: A ``StanRNG`` object to use for generating random
+            numbers, see :meth:`~StanModel.new_rng``. Must be specified
+            if ``include_gq`` is ``True``.
         :return: The constrained parameter array.
-        :raises ValueError: If `out` is specified and is not the same
+        :raises ValueError: If ``out`` is specified and is not the same
             shape as the return.
+        :raises ValueError: If ``rng`` is ``None`` and ``include_gq`` is ``True``.
         :raises RuntimeError: If the C++ Stan model throws an exception.
         """
+        if rng is None:
+            if include_gq:
+                raise ValueError(
+                    "Error: must specify rng when including generated quantities"
+                )
+            rng_ptr = None
+        else:
+            rng_ptr = rng.ptr
+
         dims = self.param_num(include_tp=include_tp, include_gq=include_gq)
         if out is None:
             out = np.zeros(dims)
         elif out.size != dims:
             raise ValueError(
                 "Error: out must be same size as number of constrained parameters"
             )
+
+        err = ctypes.pointer(ctypes.c_char_p())
+
         rc = self._param_constrain(
-            self.model_rng, int(include_tp), int(include_gq), theta_unc, out
+            self.model,
+            int(include_tp),
+            int(include_gq),
+            theta_unc,
+            out,
+            rng_ptr,
+            err,
         )
+
         if rc:
-            raise RuntimeError(
-                "param_constrain failed on C++ side; see stderr for messages"
-            )
+            raise self._handle_error(err.contents, "param_constrain")
         return out
 
+    def new_rng(self, seed) -> "StanRNG":
+        """
+        Return a new PRNG for use in :meth:`~StanModel.param_constrain``.
+
+        :param seed: A seed for the PRNG.
+        :return: A new PRNG wrapper.
+        """
+        return StanRNG(self.stanlib, seed)
+
     def param_unconstrain(
         self, theta: FloatArray, *, out: Optional[FloatArray] = None
     ) -> FloatArray:
         """
         Return the unconstrained parameters derived from the specified
-        constrained parameters.  Setting `out` avoids allocation of a
+        constrained parameters.  Setting ``out`` avoids allocation of a
         new array for the return value.
 
         :param theta: Constrained parameter array.
         :param out: A location into which the result is stored.  If
-            provided, it must have shape `(D, )`, where `D` is the number of
-            unconstrained parameters.  If not provided or `None`, a freshly
+            provided, it must have shape ``(D, )``, where ``D`` is the number of
+            unconstrained parameters.  If not provided or ``None``, a freshly
             allocated array is returned.
-        :raises ValueError: If `out` is specified and is not the same
+        :raises ValueError: If ``out`` is specified and is not the same
             shape as the return.
         :raises RuntimeError: If the C++ Stan model throws an exception.
         """
         dims = self.param_unc_num()
         if out is None:
             out = np.zeros(shape=dims)
         elif out.size != dims:
             raise ValueError(
                 f"out size = {out.size} != unconstrained params size = {dims}"
             )
-        rc = self._param_unconstrain(self.model_rng, theta, out)
+        err = ctypes.pointer(ctypes.c_char_p())
+        rc = self._param_unconstrain(self.model, theta, out, err)
         if rc:
-            raise RuntimeError(
-                "param_unconstrain failed on C++ side; see stderr for messages"
-            )
+            raise self._handle_error(err.contents, "param_unconstrain")
         return out
 
     def param_unconstrain_json(
         self, theta_json: str, *, out: Optional[FloatArray] = None
     ) -> FloatArray:
         """
         Return an array of the unconstrained parameters derived from the
         specified JSON formatted data.  See the *CmdStan Reference
         Manual* for the schema definition used.
 
         :param theta_json: The JSON encoded constrained parameters.
         :param out: A location into which the result is stored.  If
-            provided, it must have shape `(D, )`, where `D` is the number of
-            unconstrained parameters.  If not provided or `None`, a freshly
+            provided, it must have shape ``(D, )``, where ``D`` is the number of
+            unconstrained parameters.  If not provided or ``None``, a freshly
             allocated array is returned.
         :return: The unconstrained parameter array.
-        :raises ValueError: If `out` is specified and is not the same
+        :raises ValueError: If ``out`` is specified and is not the same
             shape as the return value.
         :raises RuntimeError: If the C++ Stan model throws an exception.
         """
         dims = self.param_unc_num()
         if out is None:
             out = np.zeros(shape=dims)
         elif out.size != dims:
             raise ValueError(
                 f"out size = {out.size} != unconstrained params size = {dims}"
             )
         chars = theta_json.encode("UTF-8")
-        rc = self._param_unconstrain_json(self.model_rng, chars, out)
+        err = ctypes.pointer(ctypes.c_char_p())
+        rc = self._param_unconstrain_json(self.model, chars, out, err)
         if rc:
-            raise RuntimeError(
-                "param_unconstrain_json failed on C++ side; see stderr for messages"
-            )
+            raise self._handle_error(err.contents, "param_unconstrain_json")
         return out
 
     def log_density(
         self,
         theta_unc: FloatArray,
         *,
         propto: bool = True,
         jacobian: bool = True,
     ) -> float:
         """
         Return the log density of the specified unconstrained
         parameters, dropping constant terms that do not depend on the
-        parameters if `propto` is `True` and including change of
-        variables terms for constrained parameters if `jacobian` is `True`.
+        parameters if ``propto`` is ``True`` and including change of
+        variables terms for constrained parameters if ``jacobian`` is ``True``.
 
         :param theta_unc: Unconstrained parameter array.
-        :param propto: `True` if constant terms should be dropped from the log density.
-        :param jacobian: `True` if change-of-variables terms for
+        :param propto: ``True`` if constant terms should be dropped from the log density.
+        :param jacobian: ``True`` if change-of-variables terms for
             constrained parameters should be included in the log density.
         :return: The log density.
         :raises RuntimeError: If the C++ Stan model throws an exception.
         """
         lp = ctypes.pointer(ctypes.c_double())
+        err = ctypes.pointer(ctypes.c_char_p())
         rc = self._log_density(
-            self.model_rng, int(propto), int(jacobian), theta_unc, lp
+            self.model, int(propto), int(jacobian), theta_unc, lp, err
         )
         if rc:
-            raise RuntimeError(
-                "C++ exception in log_density(); see stderr for messages"
-            )
+            raise self._handle_error(err.contents, "log_density")
         return lp.contents.value
 
     def log_density_gradient(
         self,
         theta_unc: FloatArray,
         *,
         propto: bool = True,
         jacobian: bool = True,
         out: Optional[FloatArray] = None,
     ) -> Tuple[float, FloatArray]:
         """
         Return a tuple of the log density and gradient of the specified
         unconstrained parameters, dropping constant terms that do not depend
-        on the parameters if `propto` is `True` and including change of
-        variables terms for constrained parameters if `jacobian`
-        is `True`.
+        on the parameters if ``propto`` is ``True`` and including change of
+        variables terms for constrained parameters if ``jacobian``
+        is ``True``.
 
         :param theta_unc: Unconstrained parameter array.
-        :param propto: `True` if constant terms should be dropped from the log density.
-        :param jacobian: `True` if change-of-variables terms for
+        :param propto: ``True`` if constant terms should be dropped from the log density.
+        :param jacobian: ``True`` if change-of-variables terms for
             constrained parameters should be included in the log density.
         :param out: A location into which the gradient is stored.  If
-            provided, it must have shape `(D, )` where `D` is the number
+            provided, it must have shape `(D, )` where ``D`` is the number
             of parameters.  If not provided, a freshly allocated array
             is returned.
         :return: A tuple consisting of log density and gradient.
-        :raises ValueError: If `out` is specified and is not the same
+        :raises ValueError: If ``out`` is specified and is not the same
             shape as the gradient.
         :raises RuntimeError: If the C++ Stan model throws an exception.
         """
         dims = self.param_unc_num()
         if out is None:
             out = np.zeros(shape=dims)
         elif out.size != dims:
             raise ValueError(f"out size = {out.size} != params size = {dims}")
         lp = ctypes.pointer(ctypes.c_double())
+        err = ctypes.pointer(ctypes.c_char_p())
         rc = self._log_density_gradient(
-            self.model_rng, int(propto), int(jacobian), theta_unc, lp, out
+            self.model, int(propto), int(jacobian), theta_unc, lp, out, err
         )
         if rc:
-            raise RuntimeError(
-                "C++ exception in log_density_gradient(); see stderr for messages"
-            )
+            raise self._handle_error(err.contents, "log_density_gradient")
         return lp.contents.value, out
 
     def log_density_hessian(
         self,
         theta_unc: FloatArray,
         *,
         propto: bool = True,
         jacobian: bool = True,
         out_grad: Optional[FloatArray] = None,
         out_hess: Optional[FloatArray] = None,
     ) -> Tuple[float, FloatArray, FloatArray]:
         """
         Return a tuple of the log density, gradient, and Hessian of the
         specified unconstrained parameters, dropping constant terms that do
-        not depend on the parameters if `propto` is `True` and including
+        not depend on the parameters if ``propto`` is ``True`` and including
         change of variables terms for constrained parameters if
-        `jacobian` is `True`.
+        ``jacobian`` is ``True``.
 
         :param theta_unc: Unconstrained parameter array.
-        :param propto: `True` if constant terms should be dropped from the log density.
-        :param jacobian: `True` if change-of-variables terms for
+        :param propto: ``True`` if constant terms should be dropped from the log density.
+        :param jacobian: ``True`` if change-of-variables terms for
             constrained parameters should be included in the log density.
         :param out_grad: A location into which the gradient is stored.  If
-            provided, it must have shape `(D, )` where `D` is the number
+            provided, it must have shape `(D, )` where ``D`` is the number
             of parameters.  If not provided, a freshly allocated array
             is returned.
         :param out_hess: A location into which the Hessian is stored. If
-            provided, it must have shape `(D, D)`, where `D` is the
+            provided, it must have shape `(D, D)`, where ``D`` is the
             number of parameters.  If not provided, a freshly allocated
             array is returned.
         :return: A tuple consisting of the log density, gradient, and Hessian.
-        :raises ValueError: If `out_grad` is specified and is not the
-            same shape as the gradient or if `out_hess` is specified and it
+        :raises ValueError: If ``out_grad`` is specified and is not the
+            same shape as the gradient or if ``out_hess`` is specified and it
             is not the same shape as the Hessian.
         :raises RuntimeError: If the C++ Stan model throws an exception.
         """
         dims = self.param_unc_num()
         if out_grad is None:
             out_grad = np.zeros(shape=dims)
         elif out_grad.shape != (dims,):
@@ -502,22 +586,67 @@
         if out_hess is None:
             out_hess = np.zeros(shape=hess_size)
         elif out_hess.shape != (dims, dims):
             raise ValueError(
                 f"out_hess size = {out_hess.size} != params size^2 = {hess_size}"
             )
         lp = ctypes.pointer(ctypes.c_double())
+        err = ctypes.pointer(ctypes.c_char_p())
         rc = self._log_density_hessian(
-            self.model_rng,
+            self.model,
             int(propto),
             int(jacobian),
             theta_unc,
             lp,
             out_grad,
             out_hess,
+            err,
         )
         if rc:
-            raise RuntimeError(
-                "C++ exception in log_density_hessian(); see stderr for messages"
-            )
+            raise self._handle_error(err.contents, "log_density_hessian")
         out_hess = out_hess.reshape(dims, dims)
         return lp.contents.value, out_grad, out_hess
+
+    def _handle_error(self, err: ctypes.c_char_p, method: str) -> Exception:
+        """
+        Creates an exception based on a string from C++,
+        frees the string, and returns the exception.
+
+        :param err: A C string containing an error message, or nullptr.
+        :param method: The name of the method that threw the error.
+        :return: An exception based on the.
+        """
+        if err:
+            string = ctypes.string_at(err).decode("utf-8")
+            self._free_error(err)
+            return RuntimeError(string)
+        else:
+            return RuntimeError(f"Unknown error in {method}. ")
+
+
+class StanRNG:
+    def __init__(self, lib: ctypes.CDLL, seed: int) -> None:
+        """
+        Construct a Stan random number generator.
+        This should not be called directly. Instead, use
+        :meth:`StanModel.new_rng`.
+        """
+        self.stanlib = lib
+
+        construct = self.stanlib.bs_rng_construct
+        construct.restype = ctypes.c_void_p
+        construct.argtypes = [ctypes.c_uint, star_star_char]
+        self.ptr = construct(seed, None)
+
+        if not self.ptr:
+            raise RuntimeError("Failed to construct RNG.")
+
+        self._destruct = self.stanlib.bs_rng_destruct
+        self._destruct.restype = None
+        self._destruct.argtypes = [ctypes.c_void_p]
+
+    def __del__(self) -> None:
+        """
+        Destroy the Stan model and free memory.
+        """
+        if hasattr(self, "ptr") and hasattr(self, "_destruct"):
+            self._destruct(self.ptr)
```

### Comparing `bridgestan-1.0.2/bridgestan.egg-info/PKG-INFO` & `bridgestan-2.0.0/bridgestan.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bridgestan
-Version: 1.0.2
+Version: 2.0.0
 Home-page: https://github.com/roualdes/bridgestan
 Author: Brian Ward, Edward Roualdes, Bob Carpenter
 License: BSD 3-Clause License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # bridgestan.py - The Python interface to BridgeStan
 
-[View the Python interface documentation online](https://roualdes.github.io/bridgestan/languages/python.html)
+[View the Python interface documentation online](https://roualdes.github.io/bridgestan/latest/languages/python.html)
 
 ## Installation
 
 **From PyPI**:
 ```shell
 pip install bridgestan
 ```
```

### Comparing `bridgestan-1.0.2/test/test_compile.py` & `bridgestan-2.0.0/test/test_compile.py`

 * *Files identical despite different names*

### Comparing `bridgestan-1.0.2/test/test_stanmodel.py` & `bridgestan-2.0.0/test/test_stanmodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,44 +26,40 @@
     bernoulli_data_string = (
         STAN_FOLDER / "bernoulli" / "bernoulli.data.json"
     ).read_text()
     b3 = bs.StanModel(bernoulli_so, bernoulli_data_string)
     np.testing.assert_allclose(bool(b3), True)
 
     # test missing so file
-    with np.testing.assert_raises(FileNotFoundError):
+    with pytest.raises(FileNotFoundError):
         bs.StanModel("nope, not going to find it")
 
     # test missing data file
-    with np.testing.assert_raises(FileNotFoundError):
+    with pytest.raises(FileNotFoundError):
         bs.StanModel(bernoulli_so, "nope, not going to find it.json")
 
     # test data load exception
     throw_data_so = str(STAN_FOLDER / "throw_data" / "throw_data_model.so")
-    print("construct() EXCEPTION MSG ON NEXT LINE IS NOT AN ERROR")
-    with np.testing.assert_raises(RuntimeError):
+    with pytest.raises(RuntimeError, match="find this text: datafails"):
         b4 = bs.StanModel(throw_data_so)
 
-    # TODO(carpenter): test get right error message on stderr
-
 
 def test_name():
     std_so = str(STAN_FOLDER / "stdnormal" / "stdnormal_model.so")
     b = bs.StanModel(std_so)
     np.testing.assert_equal("stdnormal_model", b.name())
 
 
 def test_model_info():
     std_so = str(STAN_FOLDER / "stdnormal" / "stdnormal_model.so")
     b = bs.StanModel(std_so)
     assert "STAN_OPENCL" in b.model_info()
     assert "BridgeStan version: 1." in b.model_info()
 
 
-
 def test_param_num():
     full_so = str(STAN_FOLDER / "full" / "full_model.so")
     b = bs.StanModel(full_so)
     np.testing.assert_equal(1, b.param_num())
     np.testing.assert_equal(1, b.param_num(include_tp=False))
     np.testing.assert_equal(1, b.param_num(include_gq=False))
     np.testing.assert_equal(1, b.param_num(include_tp=False, include_gq=False))
@@ -208,47 +204,58 @@
 
     b = bridge.param_constrain(a)
     B = b.reshape(D, D)
     np.testing.assert_allclose(B_expected, B)
 
     full_so = str(STAN_FOLDER / "full" / "full_model.so")
     bridge2 = bs.StanModel(full_so)
+    rng = bridge2.new_rng(seed=1234)
 
     np.testing.assert_equal(1, bridge2.param_constrain(a).size)
     np.testing.assert_equal(2, bridge2.param_constrain(a, include_tp=True).size)
-    np.testing.assert_equal(3, bridge2.param_constrain(a, include_gq=True).size)
     np.testing.assert_equal(
-        4, bridge2.param_constrain(a, include_tp=True, include_gq=True).size
+        3, bridge2.param_constrain(a, include_gq=True, rng=rng).size
+    )
+    np.testing.assert_equal(
+        4, bridge2.param_constrain(a, include_tp=True, include_gq=True, rng=rng).size
+    )
+
+    # reproducibility test
+    np.testing.assert_equal(
+        bridge2.param_constrain(a, include_gq=True, rng=bridge2.new_rng(seed=4567)),
+        bridge2.param_constrain(a, include_gq=True, rng=bridge2.new_rng(seed=4567)),
     )
 
+    # test error if neither seed or rng is provided
+    with pytest.raises(ValueError):
+        bridge2.param_constrain(a, include_gq=True)
+
     # out tests, matched and mismatched
     scratch = np.zeros(16)
     b = bridge.param_constrain(a, out=scratch)
     B = b.reshape(D, D)
     np.testing.assert_allclose(B_expected, B)
     scratch_wrong = np.zeros(10)
-    with np.testing.assert_raises(ValueError):
+    with pytest.raises(ValueError):
         bridge.param_constrain(a, out=scratch_wrong)
 
     # exception handling test in transformed parameters/model (compiled same way)
     throw_tp_so = str(STAN_FOLDER / "throw_tp" / "throw_tp_model.so")
     bridge2 = bs.StanModel(throw_tp_so)
 
     y = np.array(np.random.uniform(1))
     bridge2.param_constrain(y, include_tp=False)
-    print("param_constrain() EXCEPTION MSG ON NEXT LINE IS NOT AN ERROR")
-    with np.testing.assert_raises(RuntimeError):
+    with pytest.raises(RuntimeError, match="find this text: tpfails"):
         bridge2.param_constrain(y, include_tp=True)
 
     throw_gq_so = str(STAN_FOLDER / "throw_gq" / "throw_gq_model.so")
     bridge3 = bs.StanModel(throw_gq_so)
     bridge3.param_constrain(y, include_gq=False)
-    print("param_constrain() EXCEPTION MSG ON NEXT LINE IS NOT AN ERROR")
-    with np.testing.assert_raises(RuntimeError):
-        bridge3.param_constrain(y, include_gq=True)
+    with pytest.raises(RuntimeError, match="find this text: gqfails"):
+        bridge3.param_constrain(y, include_gq=True, rng=bridge3.new_rng(seed=1))
 
 
 def test_param_unconstrain():
     fr_gaussian_so = str(STAN_FOLDER / "fr_gaussian" / "fr_gaussian_model.so")
     fr_gaussian_data = str(STAN_FOLDER / "fr_gaussian" / "fr_gaussian.data.json")
     bridge = bs.StanModel(fr_gaussian_so, fr_gaussian_data)
 
@@ -258,15 +265,15 @@
     c = bridge.param_unconstrain(b)
     np.testing.assert_allclose(a, c)
 
     scratch = np.zeros(10)
     c2 = bridge.param_unconstrain(b, out=scratch)
     np.testing.assert_allclose(a, c2)
     scratch_wrong = np.zeros(16)
-    with np.testing.assert_raises(ValueError):
+    with pytest.raises(ValueError):
         bridge.param_unconstrain(b, out=scratch_wrong)
 
 
 def test_param_unconstrain_json():
     gaussian_so = str(STAN_FOLDER / "gaussian" / "gaussian_model.so")
     gaussian_data = str(STAN_FOLDER / "gaussian" / "gaussian.data.json")
     bridge = bs.StanModel(gaussian_so, gaussian_data)
@@ -278,15 +285,15 @@
     np.testing.assert_allclose(theta_unc, theta_unc_j_test)
 
     scratch = np.zeros(2)
     theta_unc_j_test2 = bridge.param_unconstrain_json(theta_json, out=scratch)
     np.testing.assert_allclose(theta_unc, theta_unc_j_test2)
 
     scratch_bad = np.zeros(10)
-    with np.testing.assert_raises(ValueError):
+    with pytest.raises(ValueError):
         bridge.param_unconstrain_json(theta_json, out=scratch_bad)
 
 
 def _log_jacobian(p):
     return np.log(p * (1 - p))
 
 
@@ -314,16 +321,16 @@
         np.testing.assert_allclose(lp3, _bernoulli_jacobian(y, x))
         lp4 = bridge.log_density(np.array([x_unc]), propto=True, jacobian=False)
         np.testing.assert_allclose(lp4, _bernoulli(y, x))
 
     throw_lp_so = str(STAN_FOLDER / "throw_lp" / "throw_lp_model.so")
     bridge2 = bs.StanModel(throw_lp_so)
     y2 = np.array(np.random.uniform(1))
-    print("log_density() EXCEPTION MSG ON NEXT LINE IS NOT AN ERROR")
-    with np.testing.assert_raises(RuntimeError):
+
+    with pytest.raises(RuntimeError, match="find this text: lpfails"):
         bridge2.log_density(y2)
 
 
 def test_log_density_gradient():
     def _logp(y_unc):
         y = np.exp(y_unc)
         return -0.5 * y**2
@@ -384,15 +391,15 @@
     logdensity, grad = bridge.log_density_gradient(
         y_unc_arr, propto=True, jacobian=True, out=scratch
     )
     np.testing.assert_allclose(_logp(y_unc) + _jacobian_true(y_unc), logdensity)
     np.testing.assert_allclose(_grad_logp(y_unc) + _grad_jacobian_true(y_unc), grad[0])
     #
     scratch_bad = np.zeros(bridge.param_unc_num() + 10)
-    with np.testing.assert_raises(ValueError):
+    with pytest.raises(ValueError):
         bridge.log_density_gradient(y_unc, out=scratch_bad)
 
 
 def test_log_density_hessian():
     def _logp(y_unc):
         y = np.exp(y_unc)
         return -0.5 * y**2
@@ -490,15 +497,15 @@
     logdensity, grad, hess = bridge.log_density_hessian(
         y_unc_arr, propto=True, jacobian=True, out_grad=scratch
     )
     np.testing.assert_allclose(_logp(y_unc) + _jacobian_true(y_unc), logdensity)
     np.testing.assert_allclose(_grad_logp(y_unc) + _grad_jacobian_true(y_unc), grad[0])
     #
     scratch_bad = np.zeros(bridge.param_unc_num() + 10)
-    with np.testing.assert_raises(ValueError):
+    with pytest.raises(ValueError):
         bridge.log_density_hessian(y_unc, out_grad=scratch_bad)
 
     # test with 5 x 5 Hessian
     simple_so = str(STAN_FOLDER / "simple" / "simple_model.so")
     simple_data = str(STAN_FOLDER / "simple" / "simple.data.json")
     bridge2 = bs.StanModel(simple_so, simple_data)
 
@@ -634,14 +641,70 @@
     names_unc = model.param_unc_names()
     pos = 0
     for n in range(1, 11):
         np.testing.assert_string_equal(names_unc[pos], f"Omega.{n}")
         pos += 1
 
 
+def test_stdout_capture():
+    import contextlib, io
+
+    theta = 0.1
+
+    m = bs.StanModel(
+        str(STAN_FOLDER / "print" / "print_model.so"), capture_stan_prints=False
+    )
+
+    with contextlib.redirect_stdout(io.StringIO()) as f:
+        print("Hello from Python!")
+        m.log_density(np.array([theta]))
+
+    captured = f.getvalue()
+    assert captured.splitlines()[0] == "Hello from Python!"
+    assert "Stan" not in captured
+
+    m2 = bs.StanModel(str(STAN_FOLDER / "print" / "print_model.so"))
+
+    with contextlib.redirect_stdout(io.StringIO()) as f:
+        print("Hello from Python!")
+        m2.log_density(np.array([theta]))
+
+    lines = f.getvalue().splitlines()
+    assert lines[0] == "Hello from Python!"
+    assert lines[1] == "Hi from Stan!"
+    assert lines[2] == f"theta = {theta}"
+
+    # test re-entrancy
+    import ctypes, threading
+
+    # define a new, sillier, callback which lets us test thread safety
+    x = 0
+
+    @ctypes.CFUNCTYPE(None, ctypes.POINTER(ctypes.c_char), ctypes.c_int)
+    def callback(s, n):
+        nonlocal x
+        x += 1
+
+    m2._set_print_callback(callback, None)
+
+    # call it many times from several threads
+    def f():
+        rng = m2.new_rng(1234)
+        for _ in range(25):
+            m2.param_constrain(np.array([theta]), include_gq=True, rng=rng)
+
+    threads = [threading.Thread(target=f) for _ in range(10)]
+    for t in threads:
+        t.start()
+    for t in threads:
+        t.join()
+
+    assert x == 500  # 2 calls per print, 10 threads, 25 iterations
+
+
 @pytest.fixture
 def recompile_simple():
     """Recompile simple_model with autodiff hessian enable, then clean-up/restore it after test"""
 
     stanfile = STAN_FOLDER / "simple" / "simple.stan"
     lib = bs.compile.generate_so_name(stanfile)
     lib.unlink(missing_ok=True)
```

