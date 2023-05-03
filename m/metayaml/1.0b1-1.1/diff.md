# Comparing `tmp/metayaml-1.0b1.tar.gz` & `tmp/metayaml-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metayaml-1.0b1.tar", last modified: Mon Nov  7 00:08:20 2022, max compression
+gzip compressed data, was "metayaml-1.1.tar", last modified: Wed May  3 20:27:37 2023, max compression
```

## Comparing `metayaml-1.0b1.tar` & `metayaml-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-11-07 00:08:20.819802 metayaml-1.0b1/
--rw-rw-rw-   0        0        0     8790 2022-11-07 00:08:20.818801 metayaml-1.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     8138 2022-11-05 22:55:55.000000 metayaml-1.0b1/README.rst
-drwxrwxrwx   0        0        0        0 2022-11-07 00:08:20.794820 metayaml-1.0b1/metayaml/
--rw-rw-rw-   0        0        0       72 2015-04-13 21:12:55.000000 metayaml-1.0b1/metayaml/__init__.py
--rw-rw-rw-   0        0        0      737 2022-11-07 00:03:37.000000 metayaml-1.0b1/metayaml/exception.py
--rw-rw-rw-   0        0        0     2485 2022-11-07 00:04:01.000000 metayaml-1.0b1/metayaml/jinja_eval.py
--rw-rw-rw-   0        0        0    11548 2022-11-07 00:03:50.000000 metayaml-1.0b1/metayaml/metayaml.py
-drwxrwxrwx   0        0        0        0 2022-11-07 00:08:20.816802 metayaml-1.0b1/metayaml.egg-info/
--rw-rw-rw-   0        0        0     8790 2022-11-07 00:08:20.000000 metayaml-1.0b1/metayaml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2022-11-07 00:08:20.000000 metayaml-1.0b1/metayaml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-07 00:08:20.000000 metayaml-1.0b1/metayaml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2022-11-07 00:08:20.000000 metayaml-1.0b1/metayaml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-11-07 00:08:20.000000 metayaml-1.0b1/metayaml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-07 00:08:20.819802 metayaml-1.0b1/setup.cfg
--rw-rw-rw-   0        0        0      802 2022-11-07 00:01:20.000000 metayaml-1.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 20:27:37.297443 metayaml-1.1/
+-rw-rw-rw-   0        0        0     8747 2023-05-03 20:27:37.282523 metayaml-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8138 2022-11-13 22:01:52.000000 metayaml-1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-03 20:27:37.217939 metayaml-1.1/metayaml/
+-rw-rw-rw-   0        0        0       72 2015-04-13 21:12:55.000000 metayaml-1.1/metayaml/__init__.py
+-rw-rw-rw-   0        0        0      737 2022-11-13 22:01:52.000000 metayaml-1.1/metayaml/exception.py
+-rw-rw-rw-   0        0        0     2485 2023-05-01 23:30:26.000000 metayaml-1.1/metayaml/jinja_eval.py
+-rw-rw-rw-   0        0        0    11828 2023-05-01 23:34:29.000000 metayaml-1.1/metayaml/metayaml.py
+drwxrwxrwx   0        0        0        0 2023-05-03 20:27:37.282523 metayaml-1.1/metayaml.egg-info/
+-rw-rw-rw-   0        0        0     8747 2023-05-03 20:27:36.000000 metayaml-1.1/metayaml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-03 20:27:37.000000 metayaml-1.1/metayaml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 20:27:36.000000 metayaml-1.1/metayaml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-03 20:27:36.000000 metayaml-1.1/metayaml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-03 20:27:36.000000 metayaml-1.1/metayaml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 20:27:37.297443 metayaml-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      822 2023-05-01 23:43:35.000000 metayaml-1.1/setup.py
```

### Comparing `metayaml-1.0b1/PKG-INFO` & `metayaml-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: metayaml
-Version: 1.0b1
+Version: 1.1
 Summary: Enhancements of yaml format to support include and python expression
 Home-page: https://bitbucket.org/atagunov/metayaml/
 Author: Anton Tagunov
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Other Environment
 Classifier: Operating System :: OS Independent
@@ -215,15 +213,15 @@
 
 **last.yaml**::
 
     extend:
       - base.yaml
     main:
       iso_3166:
-         ${__del__}: China  #  key 'China' will be removed from the result
+         China: ${__del__}  #  key 'China' will be removed from the result
          Liberia: LR  # add new key
 
       country_codes:
          - LR         # after merge country_codes contains only one element.
 
       country_codes_3:
         ${__extend__}:
@@ -320,9 +318,7 @@
     #    buz: 33
     #    foobar: 3
 
 
 License
 =======
 MetaYaml is released under a MIT license.
-
-
```

### Comparing `metayaml-1.0b1/README.rst` & `metayaml-1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 
 **last.yaml**::
 
     extend:
       - base.yaml
     main:
       iso_3166:
-         ${__del__}: China  #  key 'China' will be removed from the result
+         China: ${__del__}  #  key 'China' will be removed from the result
          Liberia: LR  # add new key
 
       country_codes:
          - LR         # after merge country_codes contains only one element.
 
       country_codes_3:
         ${__extend__}:
```

### Comparing `metayaml-1.0b1/metayaml/exception.py` & `metayaml-1.1/metayaml/exception.py`

 * *Files identical despite different names*

### Comparing `metayaml-1.0b1/metayaml/jinja_eval.py` & `metayaml-1.1/metayaml/jinja_eval.py`

 * *Files identical despite different names*

### Comparing `metayaml-1.0b1/metayaml/metayaml.py` & `metayaml-1.1/metayaml/metayaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
                 dest = {}
             elif not isinstance(dest, dict):
                 if isinstance(dest, list) and len(source) == 1 and self.EXTEND_MARKER in source:
                     added_values = source[self.EXTEND_MARKER]
                     if not isinstance(added_values, list):
                         raise MetaYamlExceptionPath(f"expected list, but have got {type(added_values)}",
                                                     path + (self.EXTEND_MARKER, ), added_values)
-                    added_values = self.eval_value(added_values, path, global_data, True)
+                    added_values, _ = self.eval_expression(added_values, global_data, path, True)
                     dest.extend(added_values)
                     return dest
                 else:
                     raise MetaYamlExceptionPath(f"dict can't be merged to {type(dest)}", path, source)
             return self._merge_dict(source, dest, global_data, path)
 
         if isinstance(source, list):
@@ -224,45 +224,49 @@
 
         brackets = self.eager_brackets if eager else self.lazy_brackets
         if brackets[0] not in val:
             return val
 
         return jinja_eval_value(self, val, path, global_data, eager, brackets)
 
-    def process_lazy(self, data, global_data, path: Path) -> tp.Tuple[tp.Any, bool]:
+    def eval_expression(self, data, global_data, path: Path, eager: bool) -> tp.Tuple[tp.Any, bool]:
         # the first item in result is evaluated value
         # the second item is true when value was substituted
         if isinstance(data, (float, int, bool)):
             return data, False
 
         if isinstance(data, str):
-            evaluated_value = self.eval_value(data, path, global_data, False)
+            evaluated_value = self.eval_value(data, path, global_data, eager)
             return evaluated_value, evaluated_value != data
 
         substituted = False
         if isinstance(data, dict):
             for key, value in list(data.items()):
                 evaluated_key = self.eval_value(key, _path(path, key), global_data, False)
-                evaluated_value, changed = self.process_lazy(value, global_data, _path(path, key))
+                evaluated_value, changed = self.eval_expression(value, global_data, _path(path, key), eager=eager)
                 substituted |= changed
                 if key != evaluated_key:
                     data.pop(key)
                     substituted = True
                 data[evaluated_key] = evaluated_value
             return data, substituted
 
         if isinstance(data, list):
             for index, value in enumerate(data):
-                evaluated_value, changed = self.process_lazy(value, global_data, _path(path, index, index=True))
+                evaluated_value, changed = self.eval_expression(value, global_data,
+                                                                _path(path, index, index=True), eager)
                 if changed:
-                    data[index] = changed
+                    data[index] = evaluated_value
                     substituted = True
             return data, substituted
         return data, False
 
+    def process_lazy(self, data, global_data, path: Path) -> tp.Tuple[tp.Any, bool]:
+        return self.eval_expression(data, global_data, path, False)
+
 
 def read(yaml_file, defaults=None, extend_key_word="extend", ignore_errors=False,
          ignore_not_existed_files=False):
     """
       Reads and process yaml config files
 
       :param yaml_file
```

### Comparing `metayaml-1.0b1/metayaml.egg-info/PKG-INFO` & `metayaml-1.1/metayaml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: metayaml
-Version: 1.0b1
+Version: 1.1
 Summary: Enhancements of yaml format to support include and python expression
 Home-page: https://bitbucket.org/atagunov/metayaml/
 Author: Anton Tagunov
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Other Environment
 Classifier: Operating System :: OS Independent
@@ -215,15 +213,15 @@
 
 **last.yaml**::
 
     extend:
       - base.yaml
     main:
       iso_3166:
-         ${__del__}: China  #  key 'China' will be removed from the result
+         China: ${__del__}  #  key 'China' will be removed from the result
          Liberia: LR  # add new key
 
       country_codes:
          - LR         # after merge country_codes contains only one element.
 
       country_codes_3:
         ${__extend__}:
@@ -320,9 +318,7 @@
     #    buz: 33
     #    foobar: 3
 
 
 License
 =======
 MetaYaml is released under a MIT license.
-
-
```

