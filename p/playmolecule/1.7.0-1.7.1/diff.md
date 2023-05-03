# Comparing `tmp/playmolecule-1.7.0.tar.gz` & `tmp/playmolecule-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.7.0.tar", last modified: Tue Apr 18 14:05:07 2023, max compression
+gzip compressed data, was "playmolecule-1.7.1.tar", last modified: Wed May  3 15:55:00 2023, max compression
```

## Comparing `playmolecule-1.7.0.tar` & `playmolecule-1.7.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:05:07.676640 playmolecule-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-18 14:04:42.000000 playmolecule-1.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-18 14:04:42.000000 playmolecule-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-18 14:05:07.672640 playmolecule-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-18 14:04:42.000000 playmolecule-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:05:07.676640 playmolecule-1.7.0/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 14:05:07.676640 playmolecule-1.7.0/playmolecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/func2argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-18 14:04:42.000000 playmolecule-1.7.0/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:05:07.672640 playmolecule-1.7.0/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-18 14:05:07.000000 playmolecule-1.7.0/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-18 14:05:07.000000 playmolecule-1.7.0/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:05:07.000000 playmolecule-1.7.0/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:05:07.000000 playmolecule-1.7.0/playmolecule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 14:05:07.000000 playmolecule-1.7.0/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 14:05:07.000000 playmolecule-1.7.0/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-18 14:04:42.000000 playmolecule-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:05:07.676640 playmolecule-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-18 14:04:42.000000 playmolecule-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:05:07.672640 playmolecule-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-18 14:04:42.000000 playmolecule-1.7.0/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-04-18 14:04:42.000000 playmolecule-1.7.0/tests/test_app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 14:04:42.000000 playmolecule-1.7.0/tests/test_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-18 14:04:42.000000 playmolecule-1.7.0/tests/test_func_to_argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:55:00.081680 playmolecule-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-03 15:54:39.000000 playmolecule-1.7.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-03 15:54:39.000000 playmolecule-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-03 15:55:00.081680 playmolecule-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-03 15:54:39.000000 playmolecule-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:55:00.081680 playmolecule-1.7.1/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 15:55:00.081680 playmolecule-1.7.1/playmolecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33242 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/func2argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-03 15:54:39.000000 playmolecule-1.7.1/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:55:00.081680 playmolecule-1.7.1/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-03 15:55:00.000000 playmolecule-1.7.1/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-03 15:55:00.000000 playmolecule-1.7.1/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:55:00.000000 playmolecule-1.7.1/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:54:59.000000 playmolecule-1.7.1/playmolecule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 15:55:00.000000 playmolecule-1.7.1/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 15:55:00.000000 playmolecule-1.7.1/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-03 15:54:39.000000 playmolecule-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:55:00.081680 playmolecule-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 15:54:39.000000 playmolecule-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:55:00.081680 playmolecule-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-03 15:54:39.000000 playmolecule-1.7.1/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-03 15:54:39.000000 playmolecule-1.7.1/tests/test_app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-03 15:54:39.000000 playmolecule-1.7.1/tests/test_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-03 15:54:39.000000 playmolecule-1.7.1/tests/test_func_to_argparse.py
```

### Comparing `playmolecule-1.7.0/LICENSE.md` & `playmolecule-1.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/PKG-INFO` & `playmolecule-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.7.0
+Version: 1.7.1
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.7.0/playmolecule/__init__.py` & `playmolecule-1.7.1/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/playmolecule/_test_funcs.py` & `playmolecule-1.7.1/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/playmolecule/config.py` & `playmolecule-1.7.1/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/playmolecule/datacenter.py` & `playmolecule-1.7.1/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/playmolecule/devutils.py` & `playmolecule-1.7.1/playmolecule/devutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -551,50 +551,63 @@
         if len(newvals) == 1:
             newvals = newvals[0]
         input_args[name] = newvals
 
     return input_args
 
 
-def app_wrapper2(func, cli_arg_str=None, token=None, execid=None, dump_argparser=None):
+def app_wrapper2(
+    func,
+    cli_arg_str=None,
+    token=None,
+    execid=None,
+    dump_argparser=None,
+    input_json=None,
+):
     from contextlib import redirect_stdout, redirect_stderr
     from playmolecule.func2argparse import func_to_argparser
     import importlib
     import datetime
     import shutil
     from unittest import mock
     import json
     from pathlib import Path
     import yaml
     import traceback
+    import logging
 
     # Import the module/function of the app to call
     pieces = func.split(".")
     module = ".".join(pieces[:-1])
     func = getattr(importlib.import_module(module), pieces[-1])
     parser = func_to_argparser(func)
     if dump_argparser is not None:
         _write_argparser_json(dump_argparser, parser)
         return
 
     if token is None:
-        cli_arg = cli_arg_str.split()
-        print("Parsing arguments", cli_arg)
-        # The parser really likes to kill the app when failing to parse... This mock.patch prevents it
-        with mock.patch("sys.exit") as m:
-            appargs, unknownargs = parser.parse_known_args(cli_arg)
-            if len(unknownargs):
-                # Otherwise throw an error for unknown arguments
-                parser.print_help()
-                raise RuntimeError(
-                    f"Unrecognized arguments \"{' '.join(unknownargs)}\""
-                )
-            if m.call_count > 0:
-                raise RuntimeError("Failed parsing app arguments")
-        params = vars(appargs)
+        if input_json is not None:
+            with open(input_json, "r") as f:
+                params = json.load(f)
+        else:
+            cli_arg = cli_arg_str.split()
+            print("Parsing arguments", cli_arg)
+            # The parser really likes to kill the app when failing to parse... This mock.patch prevents it
+            with mock.patch("sys.exit") as m:
+                appargs, unknownargs = parser.parse_known_args(cli_arg)
+                if len(unknownargs):
+                    # Otherwise throw an error for unknown arguments
+                    parser.print_help()
+                    raise RuntimeError(
+                        f"Unrecognized arguments \"{' '.join(unknownargs)}\""
+                    )
+                if m.call_count > 0:
+                    raise RuntimeError("Failed parsing app arguments")
+            params = vars(appargs)
+
         # Convert empty strings to Nones and Paths to strings
         for arg, value in params.items():
             if value == "":
                 params[arg] = None
             if isinstance(value, Path):
                 params[arg] = str(value)
             if isinstance(value, list) or isinstance(value, tuple):
@@ -657,14 +670,15 @@
 
         errored = False
         msg = ""
         try:
             currtime = datetime.datetime.now().strftime("%Y-%m-%d %H:%M")
             # Change the cwd eventually to scratchdir
             with open(logfile, "a", buffering=1) as logf:
+                logging.getLogger().addHandler(logging.StreamHandler(logf))
                 logf.write(
                     f"\n#############\nExecuting {JOB._appid} {func} on {currtime}\nARGS:\n{yaml.dump(params)}#############\n"
                 )
                 logf.flush()
                 with redirect_stdout(logf), redirect_stderr(logf):
                     func(**sessionargs, **params)
         except Exception as e:
```

### Comparing `playmolecule-1.7.0/playmolecule/func2argparse.py` & `playmolecule-1.7.1/playmolecule/func2argparse.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/playmolecule/job.py` & `playmolecule-1.7.1/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/playmolecule/jsonlogger.py` & `playmolecule-1.7.1/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/playmolecule/local.py` & `playmolecule-1.7.1/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/playmolecule/playqueue.py` & `playmolecule-1.7.1/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/playmolecule/session.py` & `playmolecule-1.7.1/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/playmolecule/utils.py` & `playmolecule-1.7.1/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.7.1/playmolecule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.7.0
+Version: 1.7.1
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.7.0/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.7.1/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/pyproject.toml` & `playmolecule-1.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/tests/test.py` & `playmolecule-1.7.1/tests/test.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/tests/test_app_wrapper.py` & `playmolecule-1.7.1/tests/test_app_wrapper.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/tests/test_datacenter.py` & `playmolecule-1.7.1/tests/test_datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.7.0/tests/test_func_to_argparse.py` & `playmolecule-1.7.1/tests/test_func_to_argparse.py`

 * *Files identical despite different names*

