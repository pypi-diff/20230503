# Comparing `tmp/nepattern-0.5.5.tar.gz` & `tmp/nepattern-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepattern-0.5.5.tar", last modified: Fri Apr 28 07:35:36 2023, max compression
+gzip compressed data, was "nepattern-0.5.6.tar", last modified: Wed May  3 12:22:38 2023, max compression
```

## Comparing `nepattern-0.5.5.tar` & `nepattern-0.5.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 nepattern-0.5.5/LICENSE
--rw-r--r--   0        0        0      703 2023-04-17 06:05:25.529605 nepattern-0.5.5/nepattern/__init__.py
--rw-r--r--   0        0        0     8885 2023-04-24 13:27:27.344009 nepattern-0.5.5/nepattern/base.py
--rw-r--r--   0        0        0     4010 2023-03-31 19:06:53.737926 nepattern-0.5.5/nepattern/context.py
--rw-r--r--   0        0        0     1419 2023-04-17 06:19:02.570290 nepattern-0.5.5/nepattern/context.pyi
--rw-r--r--   0        0        0    15577 2023-04-28 07:29:56.289893 nepattern-0.5.5/nepattern/core.py
--rw-r--r--   0        0        0       63 2022-08-22 03:10:58.502097 nepattern-0.5.5/nepattern/exception.py
--rw-r--r--   0        0        0       26 2023-04-17 06:05:25.556543 nepattern-0.5.5/nepattern/i18n/.config.json
--rw-r--r--   0        0        0      381 2023-04-17 06:05:25.502608 nepattern-0.5.5/nepattern/i18n/en-US.json
--rw-r--r--   0        0        0      353 2023-04-17 06:05:25.567509 nepattern-0.5.5/nepattern/i18n/zh-CN.json
--rw-r--r--   0        0        0    10183 2023-04-17 06:15:54.768610 nepattern-0.5.5/nepattern/main.py
--rw-r--r--   0        0        0      695 2023-04-17 06:21:36.032925 nepattern-0.5.5/nepattern/util.py
--rw-r--r--   0        0        0     1738 2023-04-28 06:40:55.722197 nepattern-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      943 2023-02-25 11:05:27.501329 nepattern-0.5.5/README.md
--rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 nepattern-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 nepattern-0.5.6/LICENSE
+-rw-r--r--   0        0        0      703 2023-04-17 06:05:25.529605 nepattern-0.5.6/nepattern/__init__.py
+-rw-r--r--   0        0        0     8946 2023-05-03 08:23:13.426003 nepattern-0.5.6/nepattern/base.py
+-rw-r--r--   0        0        0     4010 2023-03-31 19:06:53.737926 nepattern-0.5.6/nepattern/context.py
+-rw-r--r--   0        0        0     1419 2023-04-17 06:19:02.570290 nepattern-0.5.6/nepattern/context.pyi
+-rw-r--r--   0        0        0    15857 2023-05-03 08:15:17.438046 nepattern-0.5.6/nepattern/core.py
+-rw-r--r--   0        0        0       63 2022-08-22 03:10:58.502097 nepattern-0.5.6/nepattern/exception.py
+-rw-r--r--   0        0        0       26 2023-04-17 06:05:25.556543 nepattern-0.5.6/nepattern/i18n/.config.json
+-rw-r--r--   0        0        0      381 2023-04-17 06:05:25.502608 nepattern-0.5.6/nepattern/i18n/en-US.json
+-rw-r--r--   0        0        0      353 2023-04-17 06:05:25.567509 nepattern-0.5.6/nepattern/i18n/zh-CN.json
+-rw-r--r--   0        0        0    10277 2023-05-03 08:25:00.521491 nepattern-0.5.6/nepattern/main.py
+-rw-r--r--   0        0        0      695 2023-04-17 06:21:36.032925 nepattern-0.5.6/nepattern/util.py
+-rw-r--r--   0        0        0     1738 2023-05-03 08:26:17.522535 nepattern-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      943 2023-02-25 11:05:27.501329 nepattern-0.5.6/README.md
+-rw-r--r--   0        0        0     1625 1970-01-01 00:00:00.000000 nepattern-0.5.6/PKG-INFO
```

### Comparing `nepattern-0.5.5/LICENSE` & `nepattern-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.5/nepattern/__init__.py` & `nepattern-0.5.6/nepattern/__init__.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.5/nepattern/base.py` & `nepattern-0.5.6/nepattern/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,23 +107,23 @@
     _mode: Literal["pre", "suf", "all"]
 
     def __init__(self, form: type[TSeq], base: BasePattern):
         self.base = base
         self._mode = "all"
         if form is list:
             super().__init__(
-                r"\[(.+?)\]", MatchMode.REGEX_MATCH, form, alias=f"list[{base}]"
+                r"\[(.+?)\]", MatchMode.REGEX_CONVERT, form, lambda _, x: x, f"list[{base}]"
             )
         elif form is tuple:
             super().__init__(
-                r"\((.+?)\)", MatchMode.REGEX_MATCH, form, alias=f"tuple[{base}]"
+                r"\((.+?)\)", MatchMode.REGEX_CONVERT, form, lambda _, x: x, f"tuple[{base}]"
             )
         elif form is set:
             super().__init__(
-                r"\{(.+?)\}", MatchMode.REGEX_MATCH, form, alias=f"set[{base}]"
+                r"\{(.+?)\}", MatchMode.REGEX_CONVERT, form, lambda _, x: x, f"set[{base}]"
             )
         else:
             raise ValueError(
                 lang.require("nepattern", "sequence_form_error").format(
                     target=str(form)
                 )
             )
@@ -178,17 +178,18 @@
 
     def __init__(self, arg_key: BasePattern[TKey], arg_value: BasePattern[TVal]):
         self.key = arg_key
         self.value = arg_value
         self._mode = "all"
         super().__init__(
             r"\{(.+?)\}",
-            MatchMode.REGEX_MATCH,
+            MatchMode.REGEX_CONVERT,
             dict,
-            alias=f"dict[{self.key}, {self.value}]",
+            lambda _, x: x,
+            f"dict[{self.key}, {self.value}]",
         )
 
     def match(self, text: str | Any):
         _res = super().match(text)
         success: list[tuple[int, Any, Any]] = []
         fail: list[tuple[int, MatchFailed]] = []
         _max = 0
```

### Comparing `nepattern-0.5.5/nepattern/context.py` & `nepattern-0.5.6/nepattern/context.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.5/nepattern/context.pyi` & `nepattern-0.5.6/nepattern/context.pyi`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.5/nepattern/core.py` & `nepattern-0.5.6/nepattern/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,14 @@
 except ImportError:
     from typing_extensions import Annotated, Self, get_origin
 
 from .exception import MatchFailed
 from .util import TPattern
 
 
-def _accept(
-    input_: Any,
-    patterns: list[BasePattern] | None = None,
-    types: list[type] | None = None,
-):
-    res_p = any(map(lambda x: x.exec(input_).success, patterns)) if patterns else False
-    res_t = generic_isinstance(input_, tuple(types)) if types else False
-    return res_t or res_p
-
-
 class MatchMode(IntEnum):
     """参数表达式匹配模式"""
 
     REGEX_CONVERT = 3
     """正则匹配并转换"""
     TYPE_CONVERT = 2
     """传入值直接转换"""
@@ -150,16 +140,16 @@
     pattern: str
     mode: MatchMode
     converter: Callable[[BasePattern[TOrigin], str | Any], TOrigin | None]
     validators: list[Callable[[TOrigin], bool]]
 
     anti: bool
     origin: type[TOrigin]
-    pattern_accepts: list[BasePattern]
-    type_accepts: list[type]
+    pattern_accepts: tuple[BasePattern, ...]
+    type_accepts: tuple[type, ...]
     alias: str | None
     previous: BasePattern | None
 
     __slots__ = (
         "regex_pattern",
         "pattern",
         "mode",
@@ -167,14 +157,17 @@
         "anti",
         "origin",
         "pattern_accepts",
         "type_accepts",
         "alias",
         "previous",
         "validators",
+        "_hash",
+        "_repr",
+        "_accept"
     )
 
     def __init__(
         self,
         pattern: str = ".+",
         model: int | MatchMode = MatchMode.REGEX_MATCH,
         origin: type[TOrigin] = str,
@@ -197,29 +190,42 @@
         self.pattern = pattern
         self.regex_pattern = re.compile(f"^{pattern}$")
         self.mode = MatchMode(model)
         self.origin = origin
         self.alias = alias
         self.previous = previous
         accepts = accepts or []
-        self.pattern_accepts = list(
+        self.pattern_accepts = tuple(
             filter(lambda x: isinstance(x, BasePattern), accepts)  # type: ignore
         )
-        self.type_accepts = list(
+        self.type_accepts = tuple(
             filter(lambda x: not isinstance(x, BasePattern), accepts)  # type: ignore
         )
         self.converter = converter or (
             lambda _, x: (get_origin(origin) or origin)(x)
             if model == MatchMode.TYPE_CONVERT
             else eval(x)
         )
         self.validators = validators or []
         self.anti = anti
+        self._repr = self.__calc_repr__()
+        self._hash = hash(self._repr)
+        if not self.pattern_accepts and not self.type_accepts:
+            self._accept = lambda _: True
+        elif not self.pattern_accepts:
+            self._accept = lambda x: generic_isinstance(x, self.type_accepts)
+        elif not self.type_accepts:
+            self._accept = lambda x: any(map(lambda y: y.exec(x).flag == 'valid', self.pattern_accepts))
+        else:
+            self._accept = lambda x: (
+                generic_isinstance(x, self.type_accepts) or
+                any(map(lambda y: y.exec(x).flag == 'valid', self.pattern_accepts))
+            )
 
-    def __repr__(self):
+    def __calc_repr__(self):
         if self.mode == MatchMode.KEEP:
             if self.alias:
                 return self.alias
             return (
                 "Any"
                 if not self.type_accepts and not self.pattern_accepts
                 else "|".join(
@@ -247,22 +253,25 @@
         else:
             text = self.alias
         return (
             f"{f'{self.previous.__repr__()} -> ' if self.previous and id(self.previous) != id(self) else ''}"
             f"{'!' if self.anti else ''}{text}"
         )
 
+    def __repr__(self):
+        return self._repr
+
     def __str__(self):
-        return self.__repr__()
+        return self._repr
 
     def __hash__(self):
-        return hash(self.__repr__())
+        return self._hash
 
     def __eq__(self, other):
-        return isinstance(other, BasePattern) and self.__repr__() == other.__repr__()
+        return isinstance(other, BasePattern) and self._repr == other._repr
 
     @staticmethod
     def of(unit: type[TOrigin]) -> BasePattern[TOrigin]:
         """提供 Type[DataUnit] 类型的构造方法"""
         return BasePattern(
             "", MatchMode.KEEP, unit, alias=unit.__name__, accepts=[unit]
         )
@@ -285,14 +294,16 @@
 
         if isinstance(res := type_parser(content, "allow"), BasePattern):
             return res
 
     def reverse(self) -> Self:
         """改变 pattern 的 anti 值"""
         self.anti = not self.anti
+        self._repr = self.__calc_repr__()
+        self._hash = hash(self._repr)
         return self
 
     def prefixed(self):
         """让表达式能在某些场景下实现前缀匹配; 返回自身的拷贝"""
         cp_self = deepcopy(self)
         if self.mode in (MatchMode.REGEX_MATCH, MatchMode.REGEX_CONVERT):
             cp_self.regex_pattern = re.compile(f"^{self.pattern}")
@@ -306,27 +317,21 @@
         return cp_self
 
     def match(self, input_: str | Any) -> TOrigin:
         """
         对传入的参数进行匹配, 如果匹配成功, 则返回转换后的值, 否则返回None
         """
         if (
-            self.mode > 0
+            self.mode > 1
             and self.origin is not str and self.origin is not Any
             and generic_isinstance(input_, self.origin)
         ):
             return input_  # type: ignore
-        if (self.type_accepts or self.pattern_accepts) and not _accept(
-            input_, self.pattern_accepts, self.type_accepts
-        ):
-            if not self.previous or not _accept(
-                input_ := self.previous.match(input_),
-                self.pattern_accepts,
-                self.type_accepts,
-            ):  # pragma: no cover
+        if not self._accept(input_):
+            if not self.previous or not self._accept(input_ := self.previous.match(input_)):  # pragma: no cover
                 raise MatchFailed(
                     lang.require("nepattern", "type_error").format(
                         target=input_.__class__
                     )
                 )
         if self.mode == 0:
             return input_  # type: ignore
@@ -342,28 +347,26 @@
                     self.origin,
                 ):
                     raise MatchFailed(
                         lang.require("nepattern", "content_error").format(target=input_)
                     )
             return res
         if input_.__class__ is not str:
-            if not self.previous or not isinstance(
-                input_ := self.previous.match(input_), str
-            ):
+            if not self.previous or not isinstance(input_ := self.previous.match(input_), str):
                 raise MatchFailed(
                     lang.require("nepattern", "type_error").format(target=type(input_))
                 )
         if mat := self.regex_pattern.match(input_):
-            glen = len(mat.groups())
+            emp = not mat.groups()
             return (
-                self.converter(self, mat[1] if glen > 0 else mat[0])
+                self.converter(self, mat[0] if emp else mat[1])
                 if self.mode == 3
-                else mat[1]
-                if glen > 0
                 else mat[0]
+                if emp
+                else mat[1]
             )
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_)
         )
 
     @overload
     def validate(self, input_: Any) -> ValidateResult[TOrigin]:
```

### Comparing `nepattern-0.5.5/nepattern/main.py` & `nepattern-0.5.6/nepattern/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,14 +266,16 @@
             raise TypeError("Bind[...] second argument should be a callable or str.")
         pattern = deepcopy(pattern)
         pattern.alias = (
             al[0]
             if (al := [i for i in params[1:] if isinstance(i, str)])
             else pattern.alias
         )
+        pattern._repr = pattern.__calc_repr__()
+        pattern._hash = hash(pattern._repr)
         pattern.validators.extend(filter(callable, params[1:]))
         return pattern
 
 
 __all__ = [
     "Bind",
     "AnyString",
```

### Comparing `nepattern-0.5.5/nepattern/util.py` & `nepattern-0.5.6/nepattern/util.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.5/pyproject.toml` & `nepattern-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nepattern"
-version = "0.5.5"
+version = "0.5.6"
 description = "a complex pattern, support typing"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
     "tarina>=0.3.3",
```

### Comparing `nepattern-0.5.5/README.md` & `nepattern-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `nepattern-0.5.5/PKG-INFO` & `nepattern-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepattern
-Version: 0.5.5
+Version: 0.5.6
 Summary: a complex pattern, support typing
 License: MIT
 Keywords: typing,pattern,converter,validator
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

