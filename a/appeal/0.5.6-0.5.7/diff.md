# Comparing `tmp/appeal-0.5.6.tar.gz` & `tmp/appeal-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appeal-0.5.6.tar", last modified: Tue May  2 09:10:26 2023, max compression
+gzip compressed data, was "appeal-0.5.7.tar", last modified: Wed May  3 18:44:38 2023, max compression
```

## Comparing `appeal-0.5.6.tar` & `appeal-0.5.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       19 2022-01-26 11:06:53.000000 appeal-0.5.6/.gitignore
--rw-r--r--   0        0        0     1090 2023-04-27 05:54:38.102243 appeal-0.5.6/LICENSE
--rw-r--r--   0        0        0    66802 2023-05-02 09:09:34.290513 appeal-0.5.6/README.md
--rw-r--r--   0        0        0   171409 2023-05-02 09:08:54.290186 appeal-0.5.6/appeal/__init__.py
--rw-r--r--   0        0        0    23346 2023-04-27 05:54:38.106243 appeal-0.5.6/appeal/argument_grouping.py
--rw-r--r--   0        0        0     4637 2022-02-12 23:26:33.980913 appeal-0.5.6/appeal/cpp.py
--rw-r--r--   0        0        0    19692 2023-05-02 08:57:46.416604 appeal-0.5.6/appeal/text.py
--rw-r--r--   0        0        0      537 2023-05-02 08:57:46.416604 appeal-0.5.6/pyproject.toml
--rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.5.6/resources/images/appeal.logo.png
--rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.5.6/resources/images/give.your.program.appeal.png
--rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.5.6/resources/links.txt
--rw-r--r--   0        0        0    64835 2023-04-27 05:54:38.106243 appeal-0.5.6/tests/run_tests.py
--rw-r--r--   0        0        0    67296 1970-01-01 00:00:00.000000 appeal-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0       19 2022-01-26 11:06:53.000000 appeal-0.5.7/.gitignore
+-rw-r--r--   0        0        0     1090 2023-05-02 08:25:22.598769 appeal-0.5.7/LICENSE
+-rw-r--r--   0        0        0    67303 2023-05-03 18:37:18.618814 appeal-0.5.7/README.md
+-rw-r--r--   0        0        0   173042 2023-05-03 18:37:47.599733 appeal-0.5.7/appeal/__init__.py
+-rw-r--r--   0        0        0    23346 2023-05-02 08:25:22.602769 appeal-0.5.7/appeal/argument_grouping.py
+-rw-r--r--   0        0        0     4637 2022-02-12 23:26:33.980913 appeal-0.5.7/appeal/cpp.py
+-rw-r--r--   0        0        0    19692 2023-05-02 08:26:43.265271 appeal-0.5.7/appeal/text.py
+-rw-r--r--   0        0        0      537 2023-05-02 08:26:43.265271 appeal-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.5.7/resources/images/appeal.logo.png
+-rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.5.7/resources/images/give.your.program.appeal.png
+-rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.5.7/resources/links.txt
+-rw-r--r--   0        0        0    65199 2023-05-03 18:16:25.747049 appeal-0.5.7/tests/run_tests.py
+-rw-r--r--   0        0        0    67797 1970-01-01 00:00:00.000000 appeal-0.5.7/PKG-INFO
```

### Comparing `appeal-0.5.6/LICENSE` & `appeal-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `appeal-0.5.6/README.md` & `appeal-0.5.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,17 @@
 also intuitive, because it mirrors Python itself.
 If you understand how to write Python functions,
 you're already halfway to understanding Appeal!
 
 Appeal has only one dependency,
 [my **big** library.](https://github.com/larryhastings/big)
 
+Appeal is currently only supported for POSIX platforms
+(UNIX, Linux, BSD, OS X, etc).  It might work on Windows
+but this has not yet been tested.
 
 ### A New And Appealing Approach
 
 Appeal isn't like other command-line parsing libraries.
 In fact, you really shouldn't think of Appeal as a
 "command-line parsing library" per se. And, although you
 work with Appeal by passing in functions for Appeal to call,
@@ -1962,14 +1965,23 @@
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
 
 
 ## Changelog
 
+**0.5.7**
+
+* Rewrite the technology behind `accumulator[...]` and
+  `mapping[...]`.  It previously used `exec()`, which was
+  limiting; for example, you couldn't use your own types
+  or converters.  The new implementation should be much
+  more robust; it now manually defines an explicit signature
+  for the `option()` method of the subclass it creates.
+
 **0.5.6**
 
 * Fix formatting for usage when you have a
   global command *and* subcommands.
 
 **0.5.5**
```

### Comparing `appeal-0.5.6/appeal/__init__.py` & `appeal-0.5.7/appeal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 "A powerful & Pythonic command-line parsing library.  Give your program Appeal!"
-__version__ = "0.5.6"
+__version__ = "0.5.7"
 
 
 # please leave this copyright notice in binary distributions.
 license = """
 appeal/__init__.py
 part of the Appeal software package
 Copyright 2021-2023 by Larry Hastings
@@ -2931,37 +2931,58 @@
 
     return Counter
 
 
 class AccumulatorMeta(ABCMeta):
     def __getitem__(cls, t):
         if not isinstance(t, (tuple, list)):
-            t = (t,)
+            return cls.__getitem_single__(t)
+        return cls.__getitem_iterable__(t)
+
+
+    def __getitem_single__(cls, t):
+        class accumulator(cls):
+            __name__ = f'{cls.__name__}[{t.__name__}]'
+
+            def option(self, arg:t):
+                self.values.append(arg)
+        return accumulator
+
+    def __getitem_iterable__(cls, t):
+        iterable_type = type(t)
         t_names = "_".join(ti.__name__ for ti in t)
-        name = f"{cls.__name__}_{t_names}"
-        parameters = ", ".join(f"p{i}:{ti.__name__}" for i, ti in enumerate(t))
-        if len(t) == 1:
-            arguments = "p0"
-        else:
-            arguments = "(" + ", ".join(f"p{i}" for i in range(len(t))) + ")"
-        types = "(" + ", ".join(ti.__name__ for ti in t) + ")"
-        text = f"""
-class {name}(cls):
-    __name__ = '{cls.__name__}[{t_names}]'
-
-    def option(self, {parameters}):
-        # print("accumulator meta got", {arguments})
-        self.values.append({arguments})
 
-    __types__ = {types}
-"""
-        globals = {'cls': cls, 't': t}
-        # print("TEXT", text)
-        exec(text, globals)
-        return globals[name]
+        class accumulator(cls):
+            __name__ = f'{cls.__name__}[{t_names}]'
+
+            def option(self, *args):
+                if type(args) != iterable_type:
+                    args = iterable_type(args)
+                self.values.append(args)
+
+        parameters = []
+        padding = math.ceil(math.log10(len(t)))
+        for i, value in enumerate(t):
+            p = inspect.Parameter(
+                name = f'arg{i:0{padding}}',
+                default = inspect.Parameter.empty,
+                annotation = value,
+                kind = inspect.Parameter.POSITIONAL_ONLY,
+                )
+            parameters.append(p)
+
+        signature = inspect.signature(accumulator.option)
+        updated_signature = signature.replace(
+            parameters=parameters,
+            return_annotation=inspect.Signature.empty,
+            )
+
+        accumulator.__signature__ = updated_signature
+
+        return accumulator
 
     def __repr__(cls):
         return f'<{cls.__name__}>'
 
 
 class accumulator(MultiOption, metaclass=AccumulatorMeta):
     def init(self, default):
@@ -2976,54 +2997,81 @@
         return self.values
 
 
 class MappingMeta(ABCMeta):
     def __getitem__(cls, t):
         if not ((isinstance(t, (tuple, list))) and (len(t) >= 2)):
             raise AppealConfigurationError("MappingMeta[] must have at least two types")
-        t_names = "_".join(ti.__name__ for ti in t)
-        name = f"{cls.__name__}_{t_names}"
-        key = "key"
-        parameters0 = f"key:{t[0].__name__}, "
         if len(t) == 2:
-            parameters = parameters0 + f"value:{t[1].__name__}"
-            value = "value"
-        else:
-            parameters = parameters0 + ", ".join(f"value{i}:{ti.__name__}" for i, ti in enumerate(t[1:], 1))
-            value = "(" + ", ".join(f"value{i}" for i in range(1, len(t))) + ")"
-        types = "(" + ", ".join(ti.__name__ for ti in t) + ")"
-        text = f"""
-class {name}(cls):
-    __name__ = '{cls.__name__}[{t_names}]'
-
-    def option(self, {parameters}):
-        # print("mapping meta got", {key}, "=", {value})
-        self.dict[{key}] = {value}
+            return cls.__getitem_key_single__(t[0], t[1])
+        return cls.__getitem_key_iterable__(t[0], t[1:])
 
-    __types__ = {types}
-"""
-        globals = {'cls': cls, 't': t}
-        # print("TEXT", text)
-        exec(text, globals)
-        return globals[name]
+    def __getitem_key_single__(cls, k, v):
+        class accumulator(cls):
+            __name__ = f'{cls.__name__}[{k.__name__}_{v.__name__}]'
+
+            def option(self, key:k, value:v):
+                if key in self.dict:
+                    raise AppealUsageError("defined {key} more than once")
+                self.dict[key] = value
+        return accumulator
+
+    def __getitem_key_iterable__(cls, key, values):
+        iterable_type = type(values)
+        values_names = "_".join(ti.__name__ for ti in values)
+
+        class accumulator(cls):
+            __name__ = f'{cls.__name__}[{key.__name__}_{values_names}]'
+
+            def option(self, key, *values):
+                if key in self.dict:
+                    raise AppealUsageError("defined {key} more than once")
+                if type(values) != iterable_type:
+                    values = iterable_type(values)
+                self.dict[key] = values
+
+        parameters = [
+            inspect.Parameter(
+                name = 'key',
+                default = inspect.Parameter.empty,
+                annotation = key,
+                kind = inspect.Parameter.POSITIONAL_ONLY,
+                )]
+
+        padding = math.ceil(math.log10(len(values)))
+        for i, value in enumerate(values):
+            p = inspect.Parameter(
+                name = f'value{i:0{padding}}',
+                default = inspect.Parameter.empty,
+                annotation = value,
+                kind = inspect.Parameter.POSITIONAL_ONLY,
+                )
+            parameters.append(p)
 
-    def __repr__(cls):
-        return f'<{cls.__name__}>'
+        signature = inspect.signature(accumulator.option)
+        updated_signature = signature.replace(
+            parameters=parameters,
+            return_annotation=inspect.Signature.empty,
+            )
+
+        accumulator.__signature__ = updated_signature
+
+        return accumulator
 
 
 class mapping(MultiOption, metaclass=MappingMeta):
     def init(self, default):
         self.dict = {}
         if default is not empty:
             self.dict.update(dict(default))
 
-    def option(self, k:str, v:str):
-        if k in self.dict:
-            raise AppealUsageError("defined {k} more than once")
-        self.dict[k] = v
+    def option(self, key:str, value:str):
+        if key in self.dict:
+            raise AppealUsageError("defined {key} more than once")
+        self.dict[key] = value
 
     def render(self):
         return self.dict
 
 
 @must_be_instance
 def split(*separators, strip=False):
```

### Comparing `appeal-0.5.6/appeal/argument_grouping.py` & `appeal-0.5.7/appeal/argument_grouping.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.6/appeal/cpp.py` & `appeal-0.5.7/appeal/cpp.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.6/appeal/text.py` & `appeal-0.5.7/appeal/text.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.6/pyproject.toml` & `appeal-0.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `appeal-0.5.6/resources/images/appeal.logo.png` & `appeal-0.5.7/resources/images/appeal.logo.png`

 * *Files identical despite different names*

### Comparing `appeal-0.5.6/resources/images/give.your.program.appeal.png` & `appeal-0.5.7/resources/images/give.your.program.appeal.png`

 * *Files identical despite different names*

### Comparing `appeal-0.5.6/tests/run_tests.py` & `appeal-0.5.7/tests/run_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,17 @@
 
 def pool(s, *, define:appeal.mapping={}):
     return (pool, s, define)
 
 def snooker(s, *, define:appeal.mapping[int,str]={}):
     return (snooker, s, define)
 
+def skittles(s, *, define:appeal.mapping[int,str,float]={}):
+    return (skittles, s, define)
+
 def go(direction:appeal.validate("north", "south", "east", "west")):
     return (go, f"go {direction} young man!")
 
 def north(): return 'north'
 def south(): return 'south'
 def east(): return 'east'
 def west(): return 'west'
@@ -516,14 +519,22 @@
         command(snooker)
         self.assert_process(
             'snooker -d 1 e -d 2 f "part of the body" -d 3 g',
             (snooker, "part of the body", {1: 'e', 2: 'f', 3: 'g'}),
             )
 
 
+    def test_skittles_1(self):
+        command(skittles)
+        self.assert_process(
+            'skittles -d 1 e 3.3 -d 2 f 4.4 "part of the body" -d 3 g 5.5',
+            (skittles, "part of the body", {1: ('e', 3.3), 2: ('f', 4.4), 3: ('g', 5.5)}),
+            )
+
+
     def test_go_1(self):
         command(go)
         self.assert_process(
             'go north',
             (go, "go north young man!"),
             )
```

### Comparing `appeal-0.5.6/PKG-INFO` & `appeal-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appeal
-Version: 0.5.6
+Version: 0.5.7
 Summary: A powerful & Pythonic command-line parsing library.  Give your program Appeal!
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -89,14 +89,17 @@
 also intuitive, because it mirrors Python itself.
 If you understand how to write Python functions,
 you're already halfway to understanding Appeal!
 
 Appeal has only one dependency,
 [my **big** library.](https://github.com/larryhastings/big)
 
+Appeal is currently only supported for POSIX platforms
+(UNIX, Linux, BSD, OS X, etc).  It might work on Windows
+but this has not yet been tested.
 
 ### A New And Appealing Approach
 
 Appeal isn't like other command-line parsing libraries.
 In fact, you really shouldn't think of Appeal as a
 "command-line parsing library" per se. And, although you
 work with Appeal by passing in functions for Appeal to call,
@@ -1975,14 +1978,23 @@
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
 
 
 ## Changelog
 
+**0.5.7**
+
+* Rewrite the technology behind `accumulator[...]` and
+  `mapping[...]`.  It previously used `exec()`, which was
+  limiting; for example, you couldn't use your own types
+  or converters.  The new implementation should be much
+  more robust; it now manually defines an explicit signature
+  for the `option()` method of the subclass it creates.
+
 **0.5.6**
 
 * Fix formatting for usage when you have a
   global command *and* subcommands.
 
 **0.5.5**
```

