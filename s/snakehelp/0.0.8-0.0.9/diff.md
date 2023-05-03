# Comparing `tmp/snakehelp-0.0.8.tar.gz` & `tmp/snakehelp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakehelp-0.0.8.tar", last modified: Tue Apr 11 12:16:44 2023, max compression
+gzip compressed data, was "snakehelp-0.0.9.tar", last modified: Wed Apr 12 14:25:56 2023, max compression
```

## Comparing `snakehelp-0.0.8.tar` & `snakehelp-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:16:44.508580 snakehelp-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-11 12:16:10.000000 snakehelp-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-11 12:16:10.000000 snakehelp-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 12:16:44.512581 snakehelp-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-11 12:16:44.512581 snakehelp-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-11 12:16:10.000000 snakehelp-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:16:44.508580 snakehelp-0.0.8/snakehelp/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/parameter_combinations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/snakehelp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-11 12:16:10.000000 snakehelp-0.0.8/snakehelp/test_parameter_combinations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:16:44.508580 snakehelp-0.0.8/snakehelp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-11 12:16:44.000000 snakehelp-0.0.8/snakehelp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-11 12:16:44.000000 snakehelp-0.0.8/snakehelp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:16:44.000000 snakehelp-0.0.8/snakehelp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:16:44.000000 snakehelp-0.0.8/snakehelp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-11 12:16:44.000000 snakehelp-0.0.8/snakehelp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 12:16:44.000000 snakehelp-0.0.8/snakehelp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:16:44.508580 snakehelp-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 12:16:10.000000 snakehelp-0.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:16:44.508580 snakehelp-0.0.8/tests/property_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 12:16:10.000000 snakehelp-0.0.8/tests/property_tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-11 12:16:10.000000 snakehelp-0.0.8/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-11 12:16:10.000000 snakehelp-0.0.8/tests/test_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:25:56.249740 snakehelp-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 14:25:34.000000 snakehelp-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-12 14:25:34.000000 snakehelp-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-12 14:25:56.249740 snakehelp-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-12 14:25:56.249740 snakehelp-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-12 14:25:34.000000 snakehelp-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:25:56.249740 snakehelp-0.0.9/snakehelp/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-12 14:25:34.000000 snakehelp-0.0.9/snakehelp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-12 14:25:34.000000 snakehelp-0.0.9/snakehelp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 14:25:34.000000 snakehelp-0.0.9/snakehelp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-12 14:25:34.000000 snakehelp-0.0.9/snakehelp/parameter_combinations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-04-12 14:25:34.000000 snakehelp-0.0.9/snakehelp/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-12 14:25:34.000000 snakehelp-0.0.9/snakehelp/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-12 14:25:34.000000 snakehelp-0.0.9/snakehelp/snakehelp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-12 14:25:34.000000 snakehelp-0.0.9/snakehelp/test_parameter_combinations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:25:56.249740 snakehelp-0.0.9/snakehelp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-12 14:25:56.000000 snakehelp-0.0.9/snakehelp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-12 14:25:56.000000 snakehelp-0.0.9/snakehelp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:25:56.000000 snakehelp-0.0.9/snakehelp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:25:56.000000 snakehelp-0.0.9/snakehelp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 14:25:56.000000 snakehelp-0.0.9/snakehelp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 14:25:56.000000 snakehelp-0.0.9/snakehelp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:25:56.249740 snakehelp-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 14:25:34.000000 snakehelp-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:25:56.249740 snakehelp-0.0.9/tests/property_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 14:25:34.000000 snakehelp-0.0.9/tests/property_tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-12 14:25:34.000000 snakehelp-0.0.9/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-12 14:25:34.000000 snakehelp-0.0.9/tests/test_plotting.py
```

### Comparing `snakehelp-0.0.8/LICENSE` & `snakehelp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.8/PKG-INFO` & `snakehelp-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakehelp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Snakehelp: Making snakemake easier to use.
 Home-page: https://github.com/ivargr/snakehelp
 Author: Ivar Grytten
 Author-email: ivar.grytten@gmail.com
 License: MIT license
 Keywords: snakehelp
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `snakehelp-0.0.8/setup.py` & `snakehelp-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,10 +26,10 @@
     include_package_data=True,
     keywords='snakehelp',
     name='snakehelp',
     packages=find_packages(include=['snakehelp', 'snakehelp.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ivargr/snakehelp',
-    version='0.0.8',
+    version='0.0.9',
     zip_safe=False,
 )
```

### Comparing `snakehelp-0.0.8/snakehelp/parameter_combinations.py` & `snakehelp-0.0.9/snakehelp/parameter_combinations.py`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.8/snakehelp/parameters.py` & `snakehelp-0.0.9/snakehelp/parameters.py`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.8/snakehelp/plotting.py` & `snakehelp-0.0.9/snakehelp/plotting.py`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.8/snakehelp/snakehelp.py` & `snakehelp-0.0.9/snakehelp/snakehelp.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     if type == int:
         return "\\d+"
     if type == float:
         return "[+-]?([0-9]*[.])?[0-9]+"
     if type == str:
         return "\\w+"
     if get_origin(type) == Literal:
-        return "|".join([re.escape(arg) for arg in get_args(type)])
+        return "|".join([re.escape(str(arg)) for arg in get_args(type)])
     elif get_origin(type) in (Union, UnionType):
         if all(is_base_type(t) for t in get_args(type)):
             # all types are base type, we can give a regex for each
             return "|".join([type_to_regex(t) for t in get_args(type)])
         else:
             # There is one or more objects, we can have anything
             return ".*"
```

### Comparing `snakehelp-0.0.8/snakehelp/test_parameter_combinations.py` & `snakehelp-0.0.9/snakehelp/test_parameter_combinations.py`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.8/snakehelp.egg-info/PKG-INFO` & `snakehelp-0.0.9/snakehelp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakehelp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Snakehelp: Making snakemake easier to use.
 Home-page: https://github.com/ivargr/snakehelp
 Author: Ivar Grytten
 Author-email: ivar.grytten@gmail.com
 License: MIT license
 Keywords: snakehelp
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `snakehelp-0.0.8/snakehelp.egg-info/SOURCES.txt` & `snakehelp-0.0.9/snakehelp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.8/tests/test_parameters.py` & `snakehelp-0.0.9/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `snakehelp-0.0.8/tests/test_plotting.py` & `snakehelp-0.0.9/tests/test_plotting.py`

 * *Files identical despite different names*

