# Comparing `tmp/meiga-1.8.2rc0.tar.gz` & `tmp/meiga-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meiga-1.8.2rc0.tar", last modified: Wed Feb 15 15:17:58 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `meiga-1.8.2rc0.tar` & `meiga-1.8.3.tar`

### file list

```diff
@@ -1,38 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:17:58.041073 meiga-1.8.2rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-02-15 15:17:58.041073 meiga-1.8.2rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:17:58.041073 meiga-1.8.2rc0/meiga/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-15 15:17:49.000000 meiga-1.8.2rc0/meiga/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/alias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:17:58.041073 meiga-1.8.2rc0/meiga/assertions/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/assertions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/assertions/assert_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/assertions/assert_success.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:17:58.041073 meiga-1.8.2rc0/meiga/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/decorators/early_return.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/decorators/to_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/decorators/unexpected_decoration_order_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/no_given_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/on_failure_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/public_api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/meiga/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:17:58.041073 meiga-1.8.2rc0/meiga.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-02-15 15:17:57.000000 meiga-1.8.2rc0/meiga.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-02-15 15:17:58.000000 meiga-1.8.2rc0/meiga.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 15:17:57.000000 meiga-1.8.2rc0/meiga.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 15:17:57.000000 meiga-1.8.2rc0/meiga.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-15 15:17:57.000000 meiga-1.8.2rc0/meiga.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-15 15:17:57.000000 meiga-1.8.2rc0/meiga.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:17:58.041073 meiga-1.8.2rc0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-15 15:17:58.041073 meiga-1.8.2rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-02-15 15:17:48.000000 meiga-1.8.2rc0/setup.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/VERSION
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/__init__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/alias.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/deprecation.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/error.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/handlers.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/misc.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/no_given_value.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/on_failure_exception.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/public_api.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/py.typed
+-rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/result.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/assertions/__init__.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/assertions/assert_failure.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/assertions/assert_success.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/decorators/__init__.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/decorators/early_return.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/decorators/to_result.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 meiga-1.8.3/meiga/decorators/unexpected_decoration_order_error.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 meiga-1.8.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 meiga-1.8.3/LICENSE
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 meiga-1.8.3/README.md
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 meiga-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 meiga-1.8.3/PKG-INFO
```

### Comparing `meiga-1.8.2rc0/LICENSE` & `meiga-1.8.3/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021+ Alice Biometrics
+Copyright (c) 2023+ Alice Biometrics
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `meiga-1.8.2rc0/PKG-INFO` & `meiga-1.8.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: meiga
-Version: 1.8.2rc0
-Summary: A simple, typed and monad-based Result type for Python
-Home-page: https://github.com/alice-biometrics/meiga
-Author: Alice Biometrics
-Author-email: support@alicebiometrics.com
-License: MIT
-Keywords: Result,Monad,Typed,Typing
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # meiga 🧙 
 
 [![version](https://img.shields.io/github/release/alice-biometrics/meiga/all.svg)](https://github.com/alice-biometrics/meiga/releases) 
 [![ci](https://github.com/alice-biometrics/meiga/workflows/ci/badge.svg)](https://github.com/alice-biometrics/meiga/actions) 
 [![pypi](https://img.shields.io/pypi/dm/meiga)](https://pypi.org/project/meiga/) 
 [![codecov](https://codecov.io/gh/alice-biometrics/meiga/branch/main/graph/badge.svg?token=BX1IZJZLJQ)](https://codecov.io/gh/alice-biometrics/meiga)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

#### html2text {}

```diff
@@ -1,37 +1,27 @@
-Metadata-Version: 2.1 Name: meiga Version: 1.8.2rc0 Summary: A simple, typed
-and monad-based Result type for Python Home-page: https://github.com/alice-
-biometrics/meiga Author: Alice Biometrics Author-email:
-support@alicebiometrics.com License: MIT Keywords: Result,Monad,Typed,Typing
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-
-Content-Type: text/markdown License-File: LICENSE # meiga ð§ [![version]
-(https://img.shields.io/github/release/alice-biometrics/meiga/all.svg)](https:/
-/github.com/alice-biometrics/meiga/releases) [![ci](https://github.com/alice-
-biometrics/meiga/workflows/ci/badge.svg)](https://github.com/alice-biometrics/
-meiga/actions) [![pypi](https://img.shields.io/pypi/dm/meiga)](https://
-pypi.org/project/meiga/) [![codecov](https://codecov.io/gh/alice-biometrics/
-meiga/branch/main/graph/badge.svg?token=BX1IZJZLJQ)](https://codecov.io/gh/
-alice-biometrics/meiga) [![Code style: black](https://img.shields.io/badge/
-code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports:
-isort](https://img.shields.io/badge/%20imports-isort-
-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [!
-[license](https://img.shields.io/github/license/alice-biometrics/meiga.svg)]
-(https://github.com/alice-biometrics/meiga/blob/main/LICENSE) [![versions]
-(https://img.shields.io/pypi/pyversions/meiga.svg)](https://github.com/alice-
-biometrics/meiga) [https://github.com/alice-biometrics/custom-emojis/blob/
-master/images/alice_header.png?raw=true] --- **Documentation**: https://alice-
-biometrics.github.io/meiga/ **Source Code**: https://github.com/alice-
-biometrics/meiga --- ## What is meiga ð§? `meiga ð§` is a Python
-Âµframework that provides a simple, fully typed, monad-based result type â¡ï¸
-`Result[Value, Error]`. ## How could meiga ð§ help me? `meiga ð§` provides
-a simple and clear way of handling errors in Python without using `Exceptions`.
-This package improves the Dev Experience as it allows to know all possible
-typed responses. With Meiga ð§ your IDE will help you much more. ##
-Installation ð» ```console pip install meiga ``` ## Contribute We'd love you
-to contribute to *meiga* ð¥³ð¥³ð¥³ð¥³ð¥³ð¥³ï¸ï¸! For more information,
-check our [documentation](https://alice-biometrics.github.io/meiga/
-contributing/) ## Contact ð¬ support@alicebiometrics.com
+# meiga ð§ [![version](https://img.shields.io/github/release/alice-
+biometrics/meiga/all.svg)](https://github.com/alice-biometrics/meiga/releases)
+[![ci](https://github.com/alice-biometrics/meiga/workflows/ci/badge.svg)]
+(https://github.com/alice-biometrics/meiga/actions) [![pypi](https://
+img.shields.io/pypi/dm/meiga)](https://pypi.org/project/meiga/) [![codecov]
+(https://codecov.io/gh/alice-biometrics/meiga/branch/main/graph/
+badge.svg?token=BX1IZJZLJQ)](https://codecov.io/gh/alice-biometrics/meiga) [!
+[Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg)](https://github.com/psf/black) [![Imports: isort](https://
+img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)]
+(https://pycqa.github.io/isort/) [![license](https://img.shields.io/github/
+license/alice-biometrics/meiga.svg)](https://github.com/alice-biometrics/meiga/
+blob/main/LICENSE) [![versions](https://img.shields.io/pypi/pyversions/
+meiga.svg)](https://github.com/alice-biometrics/meiga) [https://github.com/
+alice-biometrics/custom-emojis/blob/master/images/alice_header.png?raw=true] --
+- **Documentation**: https://alice-biometrics.github.io/meiga/ **Source Code**:
+https://github.com/alice-biometrics/meiga --- ## What is meiga ð§? `meiga
+ð§` is a Python Âµframework that provides a simple, fully typed, monad-based
+result type â¡ï¸ `Result[Value, Error]`. ## How could meiga ð§ help me?
+`meiga ð§` provides a simple and clear way of handling errors in Python
+without using `Exceptions`. This package improves the Dev Experience as it
+allows to know all possible typed responses. With Meiga ð§ your IDE will help
+you much more. ## Installation ð» ```console pip install meiga ``` ##
+Contribute We'd love you to contribute to *meiga*
+ð¥³ð¥³ð¥³ð¥³ð¥³ð¥³ï¸ï¸! For more information, check our [documentation]
+(https://alice-biometrics.github.io/meiga/contributing/) ## Contact ð¬
+support@alicebiometrics.com
```

### Comparing `meiga-1.8.2rc0/meiga/alias.py` & `meiga-1.8.3/meiga/alias.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     __match_args__ = ("_value_success",)
 
     def __init__(self, value: TS = cast(TS, True)) -> None:
         super().__init__(success=value)
 
 
 class Failure(Generic[TF], Result[Any, TF]):
-
     __match_args__ = ("_value_failure",)
 
     def __init__(self, error: TF = cast(TF, Error())) -> None:
         super().__init__(failure=error)
 
 
 isSuccess: Result = Success()
```

### Comparing `meiga-1.8.2rc0/meiga/assertions/assert_failure.py` & `meiga-1.8.3/meiga/assertions/assert_failure.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import TYPE_CHECKING, Any, Type
+from typing import TYPE_CHECKING, Any, Optional, Type
 
 if TYPE_CHECKING:  # pragma: no cover
     from meiga.result import Result
 
 
 def assert_failure(
-    result: "Result", value_is_instance_of: Type = None, value_is_equal_to: Any = None
+    result: "Result",
+    value_is_instance_of: Optional[Type] = None,
+    value_is_equal_to: Optional[Any] = None,
 ) -> None:
     assert (
         result.is_failure
     ), f"result is not failure as expected. Given failure value is {result.value}"
     if value_is_instance_of:
         assert isinstance(result.value, value_is_instance_of), (
             f"Value is not instance of {value_is_instance_of}. "
```

### Comparing `meiga-1.8.2rc0/meiga/assertions/assert_success.py` & `meiga-1.8.3/meiga/assertions/assert_success.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import TYPE_CHECKING, Any, Type
+from typing import TYPE_CHECKING, Any, Optional, Type
 
 if TYPE_CHECKING:  # pragma: no cover
     from meiga.result import Result
 
 
 def assert_success(
-    result: "Result", value_is_instance_of: Type = None, value_is_equal_to: Any = None
+    result: "Result",
+    value_is_instance_of: Optional[Type] = None,
+    value_is_equal_to: Optional[Any] = None,
 ) -> None:
     assert (
         result.is_success
     ), f"result is not success as expected. Given failure value is {result.value}"
     if value_is_instance_of:
         assert isinstance(result.value, value_is_instance_of), (
             f"Value is not instance of {value_is_instance_of}. "
```

### Comparing `meiga-1.8.2rc0/meiga/decorators/early_return.py` & `meiga-1.8.3/meiga/decorators/early_return.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             if isinstance(func, staticmethod):
                 return Failure(UnexpectedDecorationOrderError())
             elif isinstance(func, classmethod):
                 return Failure(UnexpectedDecorationOrderError())
             else:
                 return func(*args, **kwargs)
         except OnFailureException as exc:
-            return exc.result
+            return cast(R, exc.result)
         except Error as error:
             return cast(R, Failure(error))
 
     return _early_return
 
 
 meiga = early_return  # To keep compatibility (Now this is deprecated)
```

### Comparing `meiga-1.8.2rc0/meiga/decorators/to_result.py` & `meiga-1.8.3/meiga/decorators/to_result.py`

 * *Files identical despite different names*

### Comparing `meiga-1.8.2rc0/meiga/deprecation.py` & `meiga-1.8.3/meiga/deprecation.py`

 * *Files identical despite different names*

### Comparing `meiga-1.8.2rc0/meiga/error.py` & `meiga-1.8.3/meiga/error.py`

 * *Files identical despite different names*

### Comparing `meiga-1.8.2rc0/meiga/handlers.py` & `meiga-1.8.3/meiga/handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Callable, Iterable
+from typing import Callable, Iterable, Optional
 
 from meiga.misc import get_args_list
 
 
 class Handler:
-    def __init__(self, func: Callable[..., None], args: Iterable = None):
+    def __init__(self, func: Callable[..., None], args: Optional[Iterable] = None):
         self.func = func
         self.args = args
 
     def execute(self, result) -> None:
         if self.args is not None:
             failure_args = get_args_list(self.args)
             if result.__id__ in failure_args:
```

### Comparing `meiga-1.8.2rc0/meiga/public_api.py` & `meiga-1.8.3/meiga/public_api.py`

 * *Files identical despite different names*

### Comparing `meiga-1.8.2rc0/meiga/result.py` & `meiga-1.8.3/meiga/result.py`

 * *Files 7% similar despite different names*

```diff
@@ -90,14 +90,18 @@
         return self._is_success
 
     @property
     def is_failure(self) -> bool:
         return not self._is_success
 
     def throw(self) -> None:
+        return self.reraise()
+
+    # cannot use raise as it is a reserved word
+    def reraise(self) -> None:
         if not self._is_success:
             raise self.value
         return None
 
     def unwrap(self) -> Union[TS, None]:
         if not self._is_success:
             return None
@@ -113,21 +117,26 @@
             return_value = (
                 self if return_value_on_failure is None else return_value_on_failure
             )
             raise OnFailureException(return_value)
         return cast(TS, self.value)
 
     def unwrap_or_throw(self) -> TS:
+        return self.unwrap_or_raise()
+
+    def unwrap_or_raise(self) -> TS:
         if not self._is_success:
-            self.throw()
+            self.reraise()
         return cast(TS, self.value)
 
     def unwrap_or_else(
         self,
-        on_failure_handler: OnFailureHandler = None,  # Default has to be None to be compatible with deprecated signature
+        on_failure_handler: Optional[
+            OnFailureHandler
+        ] = None,  # Default has to be None to be compatible with deprecated signature
         failure_value: Optional[TEF] = None,
         **kwargs,  # Deprecated parameter [on_failure, failure_args]
     ) -> Union[TS, TEF]:
         if not self._is_success:
             if on_failure_handler:
                 on_failure_handler.execute(self)
             else:  # Deal with deprecated parameters
@@ -135,31 +144,33 @@
                 if on_failure_handler:
                     on_failure_handler.execute(self)
             return cast(TEF, failure_value)
         return cast(TS, self.value)
 
     def unwrap_and(
         self,
-        on_success_handler: OnSuccessHandler = None,  # Default has to be None to be compatible with deprecated signature
+        on_success_handler: Optional[
+            OnSuccessHandler
+        ] = None,  # Default has to be None to be compatible with deprecated signature
         **kwargs,  # Deprecated parameter [on_success, success_args]
     ) -> Union[TS, None]:
         if self._is_success:
             if on_success_handler:
                 on_success_handler.execute(self)
             else:  # Deal with deprecated parameters
                 on_success_handler = get_on_success_handler_from_deprecated_args(kwargs)
                 if on_success_handler:
                     on_success_handler.execute(self)
             return self.value
         return None
 
     def handle(
         self,
-        on_success_handler: OnSuccessHandler = None,
-        on_failure_handler: OnFailureHandler = None,
+        on_success_handler: Optional[OnSuccessHandler] = None,
+        on_failure_handler: Optional[OnFailureHandler] = None,
         **kwargs,  # Deprecated parameter [on_success, on_failure, success_args, failure_args]
     ) -> "Result":
         if on_failure_handler:
             self.unwrap_or_else(on_failure_handler)
         else:  # Deal with deprecated parameters
             on_failure_handler = get_on_failure_handler_from_deprecated_args(kwargs)
             if on_failure_handler:
@@ -175,24 +186,28 @@
         return self
 
     def map(self, transform: Callable) -> None:
         new_value = transform(self.value)
         self.set_value(new_value)
 
     def assert_success(
-        self, value_is_instance_of: Type = None, value_is_equal_to: Any = None
+        self,
+        value_is_instance_of: Optional[Type] = None,
+        value_is_equal_to: Optional[Any] = None,
     ) -> None:
         assert_success(
             result=self,
             value_is_instance_of=value_is_instance_of,
             value_is_equal_to=value_is_equal_to,
         )
 
     def assert_failure(
-        self, value_is_instance_of: Type = None, value_is_equal_to: Any = None
+        self,
+        value_is_instance_of: Optional[Type] = None,
+        value_is_equal_to: Optional[Any] = None,
     ) -> None:
         assert_failure(
             result=self,
             value_is_instance_of=value_is_instance_of,
             value_is_equal_to=value_is_equal_to,
         )
```

