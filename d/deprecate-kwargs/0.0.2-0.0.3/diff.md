# Comparing `tmp/deprecate_kwargs-0.0.2.tar.gz` & `tmp/deprecate_kwargs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deprecate_kwargs-0.0.2.tar", last modified: Fri Jun  3 10:35:55 2022, max compression
+gzip compressed data, was "deprecate_kwargs-0.0.3.tar", last modified: Wed May  3 16:42:29 2023, max compression
```

## Comparing `deprecate_kwargs-0.0.2.tar` & `deprecate_kwargs-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-06-03 10:35:55.000000 deprecate_kwargs-0.0.2/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2876 2022-06-03 10:25:56.000000 deprecate_kwargs-0.0.2/README.md
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1479 2022-05-31 09:43:04.000000 deprecate_kwargs-0.0.2/setup.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       38 2022-06-03 10:35:55.000000 deprecate_kwargs-0.0.2/setup.cfg
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-06-03 10:35:55.000000 deprecate_kwargs-0.0.2/deprecate_kwargs.egg-info/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       17 2022-06-03 10:35:55.000000 deprecate_kwargs-0.0.2/deprecate_kwargs.egg-info/top_level.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      314 2022-06-03 10:35:55.000000 deprecate_kwargs-0.0.2/deprecate_kwargs.egg-info/SOURCES.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        1 2022-06-03 10:35:55.000000 deprecate_kwargs-0.0.2/deprecate_kwargs.egg-info/dependency_links.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4263 2022-06-03 10:35:55.000000 deprecate_kwargs-0.0.2/deprecate_kwargs.egg-info/PKG-INFO
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       97 2022-06-03 10:35:55.000000 deprecate_kwargs-0.0.2/deprecate_kwargs.egg-info/requires.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4263 2022-06-03 10:35:55.000000 deprecate_kwargs-0.0.2/PKG-INFO
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-06-03 10:35:55.000000 deprecate_kwargs-0.0.2/deprecate_kwargs/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      126 2022-05-29 07:29:48.000000 deprecate_kwargs-0.0.2/deprecate_kwargs/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2902 2022-06-03 10:27:50.000000 deprecate_kwargs-0.0.2/deprecate_kwargs/_dk.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       22 2022-06-03 10:34:31.000000 deprecate_kwargs-0.0.2/deprecate_kwargs/version.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-06-03 10:35:55.000000 deprecate_kwargs-0.0.2/test/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1557 2022-06-03 10:31:05.000000 deprecate_kwargs-0.0.2/test/test_dk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:42:29.839166 deprecate_kwargs-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 16:42:21.000000 deprecate_kwargs-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-03 16:42:29.835165 deprecate_kwargs-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-03 16:42:21.000000 deprecate_kwargs-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:42:29.835165 deprecate_kwargs-0.0.3/deprecate_kwargs/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 16:42:21.000000 deprecate_kwargs-0.0.3/deprecate_kwargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-03 16:42:21.000000 deprecate_kwargs-0.0.3/deprecate_kwargs/_dk.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 16:42:21.000000 deprecate_kwargs-0.0.3/deprecate_kwargs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:42:29.835165 deprecate_kwargs-0.0.3/deprecate_kwargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-03 16:42:29.000000 deprecate_kwargs-0.0.3/deprecate_kwargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-03 16:42:29.000000 deprecate_kwargs-0.0.3/deprecate_kwargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:42:29.000000 deprecate_kwargs-0.0.3/deprecate_kwargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 16:42:29.000000 deprecate_kwargs-0.0.3/deprecate_kwargs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 16:42:29.000000 deprecate_kwargs-0.0.3/deprecate_kwargs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:42:29.839166 deprecate_kwargs-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-03 16:42:21.000000 deprecate_kwargs-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:42:29.835165 deprecate_kwargs-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-03 16:42:21.000000 deprecate_kwargs-0.0.3/test/test_dk.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `deprecate_kwargs-0.0.2/README.md` & `deprecate_kwargs-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 # [deprecate-kwargs](https://github.com/DeepPSP/deprecate-kwargs/)
 
 ![formatting](https://github.com/DeepPSP/deprecate-kwargs/actions/workflows/check-formatting.yml/badge.svg)
 ![pytest](https://github.com/DeepPSP/deprecate-kwargs/actions/workflows/run-pytest.yml/badge.svg)
+[![codecov](https://codecov.io/gh/DeepPSP/deprecate-kwargs/branch/master/graph/badge.svg?token=6J4Q7SBF7M)](https://codecov.io/gh/DeepPSP/deprecate-kwargs)
 ![PyPI](https://img.shields.io/pypi/v/deprecate-kwargs?style=flat-square)
+![downloads](https://img.shields.io/pypi/dm/deprecate-kwargs?style=flat-square)
+![license](https://img.shields.io/github/license/DeepPSP/deprecate-kwargs?style=flat-square)
 
 A Tool for Deprecating (Keyword) Arguments for Backward Compatibility for Python Functions.
 
 A decorator is implemented to deprecate old kwargs in a function, with signature and docstring modified accordingly.
 Instead of replacing the old kwargs with new ones, this decorator makes old and new kwargs both available,
 with warnings raised when old kwargs are passed.
 
 <!-- toc -->
 
-- [Installation](#installation)
-- [Usage Example](#usage-example)
-- [Benefits](#benefits)
+- [deprecate-kwargs](#deprecate-kwargs)
+  - [Installation](#installation)
+  - [Usage Example](#usage-example)
+  - [Benefits](#benefits)
 
 <!-- tocstop -->
 
 ## Installation
+
 Run
+
 ```bash
 python -m pip install deprecate-kwargs
 ```
+
 or install the latest version in [GitHub](https://github.com/DeepPSP/deprecate-kwargs/) using
+
 ```bash
 python -m pip install git+https://github.com/DeepPSP/deprecate-kwargs.git
 ```
 
 ## Usage Example
+
 ```python
 >>> from deprecate_kwargs import deprecate_kwargs
 >>> @deprecate_kwargs([["new_arg_1", "old_arg_1"], ["new_arg_2", "old_arg_2"], ["new_kw", "old_kw"]])
 >>> def some_func(old_arg_1: int, old_arg_2: int, old_kw: int = 3):
 >>>     return (old_arg_1 + old_arg_2) * old_kw
 >>> some_func.__signature__
 <Signature (new_arg_1: int, new_arg_2: int, new_kw: int = 3)>
@@ -45,23 +54,29 @@
 PendingDeprecationWarning: (keyword) argument "old_kw" is deprecated, use "new_kw" instead
 90
 ```
 
 ## Benefits
 
 `deprecate_kwargs` is quite useful when one wants to change the name of an argument (or keyword argument) of some function, while keeping old codes using this function still working, hence is beneficial for backward compatibility. For example, say in version 0.1 of some package, there's a function
+
 ```python
 def some_deep_learning_model_trainer(learning_rate, ...):
     ...
 ```
+
 And in version 0.2, someone wants to change `learning_rate` to `lr`. If it was replaced directly via
+
 ```python
 def some_deep_learning_model_trainer(lr, ...):
     ...
 ```
+
 then old codes using this function bycalling `some_deep_learning_model_trainer(learning_rate=1e-3, ...)` would break. However, if the replacement is done using
+
 ```python
 @deprecate_kwargs([["lr", "learning_rate"]])
 def some_deep_learning_model_trainer(learning_rate, ...):
     ...
 ```
+
 then one can call this function using `some_deep_learning_model_trainer(lr=1e-3)`, as well as `some_deep_learning_model_trainer(learning_rate=1e-3, ...)` only with a warning raised. In this way, old codes are rescued from breaking.
```

### Comparing `deprecate_kwargs-0.0.2/setup.py` & `deprecate_kwargs-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 extras = {}
 extras["test"] = [
     "black==22.3.0",
     "flake8",
     "pytest",
     "pytest-xdist",
+    "pytest-cov",
 ]
 extras["dev"] = extras["test"]
 
 
 setuptools.setup(
     name="deprecate_kwargs",
     version=__version__,
```

### Comparing `deprecate_kwargs-0.0.2/deprecate_kwargs/_dk.py` & `deprecate_kwargs-0.0.3/deprecate_kwargs/_dk.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,29 +12,34 @@
     "deprecate_kwargs",
 ]
 
 
 _WARNING_CATEGORY = PendingDeprecationWarning
 
 
-def deprecate_kwargs(l_kwargs: Sequence[Sequence[str]]) -> Callable:
-    """
-
-    Decorator to deprecate old kwargs in a function,
+def deprecate_kwargs(
+    l_kwargs: Sequence[Sequence[str]], update_docstring: bool = True
+) -> Callable:
+    """Decorator to deprecate old kwargs in a function,
     with signature and docstring modified accordingly.
+
     Instead of replacing the old kwargs with new ones,
     this decorator makes old and new kwargs both available,
     with warnings raised when old kwargs are passed.
 
     Parameters
     ----------
-    l_kwargs: Sequence[Sequence[str]],
-        a list of kwargs to be deprecated,
-        each element is a sequence of length 2,
-        of the form (new_kwarg, old_kwarg)
+    l_kwargs : Sequence[Sequence[str]],
+        A list of kwargs to be deprecated.
+        Each element is a sequence of length 2,
+        of the form ``(new_kwarg, old_kwarg)``.
+    update_docstring : bool, default True
+        Whether to update the docstring of the decorated function.
+        The update is done by replacing all occurrences of old kwargs
+        with new kwargs in the docstring.
 
     Examples
     --------
     >>> from deprecate_kwargs import deprecate_kwargs
     >>> @deprecate_kwargs([["new_arg_1", "old_arg_1"], ["new_arg_2", "old_arg_2"], ["new_kw", "old_kw"]])
     >>> def some_func(old_arg_1: int, old_arg_2: int, *, old_kw: int = 3):
     >>>     return (old_arg_1 + old_arg_2) * old_kw
@@ -45,23 +50,28 @@
     >>> some_func(new_arg_1=10, new_arg_2=20, new_kw=3)
     90
     >>> some_func(10, old_arg_2=20, old_kw=3)
     PendingDeprecationWarning: (keyword) argument "old_arg_2" is deprecated, use "new_arg_2" instead
     PendingDeprecationWarning: (keyword) argument "old_kw" is deprecated, use "new_kw" instead
     90
 
+    Warning
+    -------
+    If the replaced (old) argument has a simple name, e.g. ``a``,
+    then `update_docstring` should better be set to ``False``,
+    and the new docstring should be updated manually, or using
+    finer-grained methods.
+
     """
     warnings.simplefilter("always")
 
     def decorator(func: Callable) -> Callable:
-        """ """
-
         @wraps(func)
         def wrapper(*args, **kwargs) -> Callable:
-            """ """
+
             input_kwargs = deepcopy(kwargs)
             for new_kw, old_kw in l_kwargs:
                 if new_kw in kwargs:
                     input_kwargs.pop(new_kw, None)
                     input_kwargs[old_kw] = kwargs[new_kw]
                 elif old_kw in kwargs:
                     warnings.warn(
@@ -72,15 +82,15 @@
 
         func_params = list(inspect.signature(func).parameters.values())
         func_param_names = list(inspect.signature(func).parameters.keys())
         wrapper.__doc__ = deepcopy(func.__doc__)
         for new_kw, old_kw in l_kwargs:
             idx = func_param_names.index(old_kw)
             func_params[idx] = func_params[idx].replace(name=new_kw)
-            if wrapper.__doc__ is not None:
+            if update_docstring and wrapper.__doc__ is not None:
                 wrapper.__doc__ = wrapper.__doc__.replace(old_kw, new_kw)
         wrapper.__signature__ = inspect.Signature(parameters=func_params)
         return wrapper
 
     warnings.simplefilter("default")
 
     return decorator
```

### Comparing `deprecate_kwargs-0.0.2/test/test_dk.py` & `deprecate_kwargs-0.0.3/test/test_dk.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 """
 """
 
 import sys
 
 import pytest
 
-try:
-    from deprecate_kwargs import deprecate_kwargs
-    from deprecate_kwargs._dk import _WARNING_CATEGORY
-except ModuleNotFoundError:
-    from pathlib import Path
-
-    sys.path.insert(0, str(Path(__file__).absolute().parents[1]))
-
-    from deprecate_kwargs import deprecate_kwargs
-    from deprecate_kwargs._dk import _WARNING_CATEGORY
+from deprecate_kwargs import deprecate_kwargs
+from deprecate_kwargs._dk import _WARNING_CATEGORY
 
 
 @deprecate_kwargs(
     [["new_arg_1", "old_arg_1"], ["new_arg_2", "old_arg_2"], ["new_kw", "old_kw"]]
 )
 def some_func(old_arg_1: int, old_arg_2: int, *, old_kw: int = 3):
     """
@@ -53,11 +45,7 @@
         "\n    Parameters\n    ----------"
         "\n    new_arg_1: int,\n        argument 1"
         "\n    new_arg_2: int,\n        argument 2"
         "\n    new_kw: int, default 3,\n        keyword argument\n\n    "
     )
 
     pytest.warns(_WARNING_CATEGORY, some_func, old_arg_1=10, old_arg_2=20, old_kw=3)
-
-
-if __name__ == "__main__":
-    test_dk()
```

