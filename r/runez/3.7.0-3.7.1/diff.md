# Comparing `tmp/runez-3.7.0.tar.gz` & `tmp/runez-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runez-3.7.0.tar", last modified: Fri Mar 31 04:39:00 2023, max compression
+gzip compressed data, was "runez-3.7.1.tar", last modified: Wed May  3 18:26:49 2023, max compression
```

## Comparing `runez-3.7.0.tar` & `runez-3.7.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 04:39:00.792476 runez-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-31 04:38:07.000000 runez-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-31 04:38:07.000000 runez-3.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-03-31 04:39:00.792476 runez-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-03-31 04:38:07.000000 runez-3.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-31 04:38:07.000000 runez-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 04:39:00.792476 runez-3.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-31 04:38:07.000000 runez-3.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 04:39:00.784476 runez-3.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 04:39:00.788476 runez-3.7.0/src/runez/
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/click.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 04:39:00.788476 runez-3.7.0/src/runez/colors/
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/colors/named.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/colors/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14267 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/date.py
--rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    39701 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    46357 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/logsetup.py
--rw-r--r--   0 runner    (1001) docker     (123)    24983 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)    43870 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/pyenv.py
--rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    11463 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    27665 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    81617 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-31 04:38:07.000000 runez-3.7.0/src/runez/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 04:39:00.788476 runez-3.7.0/src/runez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-03-31 04:39:00.000000 runez-3.7.0/src/runez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-31 04:39:00.000000 runez-3.7.0/src/runez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 04:39:00.000000 runez-3.7.0/src/runez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 04:39:00.000000 runez-3.7.0/src/runez.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 04:39:00.792476 runez-3.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    25749 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_logsetup.py
--rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)    33428 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_pyenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_slotted.py
--rw-r--r--   0 runner    (1001) docker     (123)    31192 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-31 04:38:07.000000 runez-3.7.0/tests/test_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:26:49.412461 runez-3.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 18:26:04.000000 runez-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-03 18:26:04.000000 runez-3.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-03 18:26:49.412461 runez-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-03 18:26:04.000000 runez-3.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 18:26:04.000000 runez-3.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 18:26:49.412461 runez-3.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-03 18:26:04.000000 runez-3.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:26:49.404461 runez-3.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:26:49.408461 runez-3.7.1/src/runez/
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15102 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/click.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:26:49.408461 runez-3.7.1/src/runez/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/colors/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/colors/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14267 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26799 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38953 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46357 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/logsetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24983 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43870 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/pyenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11463 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27665 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81617 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-03 18:26:04.000000 runez-3.7.1/src/runez/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:26:49.408461 runez-3.7.1/src/runez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-03 18:26:49.000000 runez-3.7.1/src/runez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-03 18:26:49.000000 runez-3.7.1/src/runez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:26:49.000000 runez-3.7.1/src/runez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 18:26:49.000000 runez-3.7.1/src/runez.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:26:49.412461 runez-3.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25749 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_logsetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33428 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_pyenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_slotted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31192 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-03 18:26:04.000000 runez-3.7.1/tests/test_thread.py
```

### Comparing `runez-3.7.0/LICENSE` & `runez-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/PKG-INFO` & `runez-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runez
-Version: 3.7.0
+Version: 3.7.1
 Summary: Friendly misc/utils/convenience library
 Home-page: https://github.com/codrsquad/runez
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/runez/wiki
 Project-URL: Release notes, https://github.com/codrsquad/runez/wiki/Release-notes
```

### Comparing `runez-3.7.0/README.rst` & `runez-3.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/setup.py` & `runez-3.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/__init__.py` & `runez-3.7.1/src/runez/__init__.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/__main__.py` & `runez-3.7.1/src/runez/__main__.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/ascii.py` & `runez-3.7.1/src/runez/ascii.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/click.py` & `runez-3.7.1/src/runez/click.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/colors/__init__.py` & `runez-3.7.1/src/runez/colors/__init__.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/colors/named.py` & `runez-3.7.1/src/runez/colors/named.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/colors/terminal.py` & `runez-3.7.1/src/runez/colors/terminal.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/config.py` & `runez-3.7.1/src/runez/config.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/conftest.py` & `runez-3.7.1/src/runez/conftest.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/convert.py` & `runez-3.7.1/src/runez/convert.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/date.py` & `runez-3.7.1/src/runez/date.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/file.py` & `runez-3.7.1/src/runez/file.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/heartbeat.py` & `runez-3.7.1/src/runez/heartbeat.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/http.py` & `runez-3.7.1/src/runez/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 import os
 import re
 import sys
 import urllib.parse
 from pathlib import Path
 
 from runez.file import checksum, decompress, delete, ensure_folder, TempFolder, to_path
-from runez.logsetup import LogManager
 from runez.system import _R, abort, DEV, find_caller, joined, short, stringified, SYS_INFO, UNSET
 
 
 def urljoin(base, url):
     """Join base + url, considering that `base` is intended to be the base url of a REST end point"""
     if not base:
         return url
@@ -576,18 +575,14 @@
             # We were invoked without arguments, form: @RestHandler.mock
             w = MockWrapper(cls, None, None)
             return w(base_url)
 
         return MockWrapper(cls, base_url, specs)
 
     @classmethod
-    def is_usable(cls):
-        """Is this handler currently usable"""
-
-    @classmethod
     def new_session(cls, **session_spec):
         """New session for 'session_spec'"""
 
     @classmethod
     def raw_response(cls, session, method, url, **passed_through):
         """
         Args:
@@ -621,32 +616,14 @@
         """Default user agent to use"""
         return "%s/%s (%s)" % (SYS_INFO.program_name, SYS_INFO.program_version, SYS_INFO.platform_info)
 
 
 class RequestsHandler(RestHandler):
     """Using requests (client is to bring in the dependency)"""
 
-    _is_usable = None
-
-    @classmethod
-    def is_usable(cls):
-        if cls._is_usable is None:
-            try:
-                import requests
-                import urllib3
-
-                # Silence logs, we use runez' more sophisticated logging setup
-                LogManager.silence(requests, urllib3)
-                cls._is_usable = True
-
-            except ImportError:  # pragma: no cover
-                cls._is_usable = False
-
-        return cls._is_usable
-
     @classmethod
     def default_retry(cls):
         import urllib3
 
         return urllib3.Retry(backoff_factor=1, status_forcelist={413, 429, 500, 502, 503, 504})
 
     @classmethod
@@ -734,17 +711,14 @@
         self.base_url = base_url
         self.headers = dict(headers) if headers else {}
         self.timeout = timeout
         self.cache_wrapper = cache
         if handler:
             self.handler = handler
 
-        if not self.handler or not self.handler.is_usable():
-            raise Exception("RestClient handler '%s' is not usable" % self.handler)
-
         self.user_agent = user_agent or self.handler.user_agent()
         self.session = session or self.handler.new_session(**session_spec)
         if self.user_agent:
             self.headers["User-Agent"] = self.user_agent
 
     def __repr__(self):
         return stringified(self.base_url or self.session)
```

### Comparing `runez-3.7.0/src/runez/inspector.py` & `runez-3.7.1/src/runez/inspector.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/logsetup.py` & `runez-3.7.1/src/runez/logsetup.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/program.py` & `runez-3.7.1/src/runez/program.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/prompt.py` & `runez-3.7.1/src/runez/prompt.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/pyenv.py` & `runez-3.7.1/src/runez/pyenv.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/render.py` & `runez-3.7.1/src/runez/render.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/schema.py` & `runez-3.7.1/src/runez/schema.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/serialize.py` & `runez-3.7.1/src/runez/serialize.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/system.py` & `runez-3.7.1/src/runez/system.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez/thread.py` & `runez-3.7.1/src/runez/thread.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/src/runez.egg-info/PKG-INFO` & `runez-3.7.1/src/runez.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runez
-Version: 3.7.0
+Version: 3.7.1
 Summary: Friendly misc/utils/convenience library
 Home-page: https://github.com/codrsquad/runez
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/runez/wiki
 Project-URL: Release notes, https://github.com/codrsquad/runez/wiki/Release-notes
```

### Comparing `runez-3.7.0/src/runez.egg-info/SOURCES.txt` & `runez-3.7.1/src/runez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_cached_property.py` & `runez-3.7.1/tests/test_cached_property.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_click.py` & `runez-3.7.1/tests/test_click.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_colors.py` & `runez-3.7.1/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_config.py` & `runez-3.7.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_convert.py` & `runez-3.7.1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_date.py` & `runez-3.7.1/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_file.py` & `runez-3.7.1/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_heartbeat.py` & `runez-3.7.1/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_http.py` & `runez-3.7.1/tests/test_http.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections import namedtuple
 from pathlib import Path
 from unittest.mock import MagicMock, patch
 
 import pytest
 
 import runez
-from runez.http import ForbiddenHttpError, GlobalHttpCalls, MockResponse, RestClient, RestHandler, RestResponse, urljoin
+from runez.http import ForbiddenHttpError, GlobalHttpCalls, MockResponse, RestClient, RestResponse, urljoin
 
 
 EXAMPLE = RestClient("https://example.com")
 CacheState = namedtuple("CacheState", "cached hits misses updates")
 
 
 class MockBackend:
@@ -169,18 +169,14 @@
     assert urljoin("a#fragment", "b") == "a#fragment/b"
     assert urljoin("http://example.net/a", "b") == "http://example.net/a/b"
     assert urljoin("http://example.net/a", "https://example.com/b") == "https://example.com/b"
     assert urljoin("http://example.net/a/#/b", "https://example.com/b") == "https://example.com/b"
     assert urljoin("http://example.net/a/#/b", "c") == 'http://example.net/a/#/b/c'
     assert urljoin("http://example.net/a#b", "c") == 'http://example.net/a#b/c'
 
-    with pytest.raises(Exception) as exc:
-        RestClient(handler=RestHandler)
-    assert "is not usable" in str(exc)
-
 
 @EXAMPLE.mock({})
 @RestClient.handler.mock
 @EXAMPLE.mock
 @RestClient.handler.mock({})
 def test_files(temp_folder):
     """yolo"""
```

### Comparing `runez-3.7.0/tests/test_inspector.py` & `runez-3.7.1/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_logsetup.py` & `runez-3.7.1/tests/test_logsetup.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_program.py` & `runez-3.7.1/tests/test_program.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_prompt.py` & `runez-3.7.1/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_pyenv.py` & `runez-3.7.1/tests/test_pyenv.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_render.py` & `runez-3.7.1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_schema.py` & `runez-3.7.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_serialize.py` & `runez-3.7.1/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_slotted.py` & `runez-3.7.1/tests/test_slotted.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_system.py` & `runez-3.7.1/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_testing.py` & `runez-3.7.1/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `runez-3.7.0/tests/test_thread.py` & `runez-3.7.1/tests/test_thread.py`

 * *Files identical despite different names*

