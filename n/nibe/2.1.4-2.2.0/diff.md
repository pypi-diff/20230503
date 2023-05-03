# Comparing `tmp/nibe-2.1.4.tar.gz` & `tmp/nibe-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nibe-2.1.4.tar", last modified: Tue Mar 14 18:30:22 2023, max compression
+gzip compressed data, was "nibe-2.2.0.tar", last modified: Wed May  3 19:17:51 2023, max compression
```

## Comparing `nibe-2.1.4.tar` & `nibe-2.2.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:30:22.385235 nibe-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-14 18:30:12.000000 nibe-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42024 2023-03-14 18:30:22.385235 nibe-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-03-14 18:30:12.000000 nibe-2.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:30:22.377235 nibe-2.1.4/nibe/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/coil.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/coil_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:30:22.381235 nibe-2.1.4/nibe/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/connection/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/connection/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/connection/modbus.py
--rw-r--r--   0 runner    (1001) docker     (123)    23788 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/connection/nibegw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:30:22.381235 nibe-2.1.4/nibe/console_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/console_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/console_scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/console_scripts/convert_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:30:22.385235 nibe-2.1.4/nibe/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)   349736 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/f1145_f1245.json
--rw-r--r--   0 runner    (1001) docker     (123)   235740 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/f1155_f1255.json
--rw-r--r--   0 runner    (1001) docker     (123)   363580 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/f1345.json
--rw-r--r--   0 runner    (1001) docker     (123)   370969 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/f1355.json
--rw-r--r--   0 runner    (1001) docker     (123)   112227 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/f370_f470.json
--rw-r--r--   0 runner    (1001) docker     (123)   132739 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/f730.json
--rw-r--r--   0 runner    (1001) docker     (123)   147755 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/f750.json
--rw-r--r--   0 runner    (1001) docker     (123)   233725 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/s1155_s1255.json
--rw-r--r--   0 runner    (1001) docker     (123)   152307 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/s2125.json
--rw-r--r--   0 runner    (1001) docker     (123)   151836 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/s320_s325.json
--rw-r--r--   0 runner    (1001) docker     (123)    81905 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/smo20.json
--rw-r--r--   0 runner    (1001) docker     (123)   302299 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/smo40.json
--rw-r--r--   0 runner    (1001) docker     (123)   223244 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/smos40.json
--rw-r--r--   0 runner    (1001) docker     (123)   210957 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/vvm225_vvm320_vvm325.json
--rw-r--r--   0 runner    (1001) docker     (123)   206217 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/data/vvm310_vvm500.json
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/event_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/heatpump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 18:30:12.000000 nibe-2.1.4/nibe/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:30:22.381235 nibe-2.1.4/nibe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42024 2023-03-14 18:30:22.000000 nibe-2.1.4/nibe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-14 18:30:22.000000 nibe-2.1.4/nibe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 18:30:22.000000 nibe-2.1.4/nibe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-14 18:30:22.000000 nibe-2.1.4/nibe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-14 18:30:22.000000 nibe-2.1.4/nibe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-14 18:30:22.000000 nibe-2.1.4/nibe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 18:30:22.000000 nibe-2.1.4/nibe.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-14 18:30:12.000000 nibe-2.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-14 18:30:22.385235 nibe-2.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:30:22.385235 nibe-2.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-03-14 18:30:12.000000 nibe-2.1.4/tests/test_coil.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-03-14 18:30:12.000000 nibe-2.1.4/tests/test_heatpump.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.245375 nibe-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 19:17:41.000000 nibe-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42067 2023-05-03 19:17:51.245375 nibe-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-05-03 19:17:41.000000 nibe-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.241375 nibe-2.2.0/nibe/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/coil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/coil_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.241375 nibe-2.2.0/nibe/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/connection/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/connection/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/connection/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23788 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/connection/nibegw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.241375 nibe-2.2.0/nibe/console_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/console_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/console_scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/console_scripts/convert_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.245375 nibe-2.2.0/nibe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)   349736 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f1145_f1245.json
+-rw-r--r--   0 runner    (1001) docker     (123)   235740 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f1155_f1255.json
+-rw-r--r--   0 runner    (1001) docker     (123)   363580 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f1345.json
+-rw-r--r--   0 runner    (1001) docker     (123)   370969 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f1355.json
+-rw-r--r--   0 runner    (1001) docker     (123)   112227 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f370_f470.json
+-rw-r--r--   0 runner    (1001) docker     (123)   132739 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f730.json
+-rw-r--r--   0 runner    (1001) docker     (123)   147755 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/f750.json
+-rw-r--r--   0 runner    (1001) docker     (123)   233725 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/s1155_s1255.json
+-rw-r--r--   0 runner    (1001) docker     (123)   152307 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/s2125.json
+-rw-r--r--   0 runner    (1001) docker     (123)   151836 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/s320_s325.json
+-rw-r--r--   0 runner    (1001) docker     (123)   183682 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/s735.json
+-rw-r--r--   0 runner    (1001) docker     (123)    81905 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/smo20.json
+-rw-r--r--   0 runner    (1001) docker     (123)   302299 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/smo40.json
+-rw-r--r--   0 runner    (1001) docker     (123)   230143 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/smos40.json
+-rw-r--r--   0 runner    (1001) docker     (123)   210957 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/vvm225_vvm320_vvm325.json
+-rw-r--r--   0 runner    (1001) docker     (123)   206217 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/data/vvm310_vvm500.json
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/event_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/heatpump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:41.000000 nibe-2.2.0/nibe/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.241375 nibe-2.2.0/nibe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42067 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:17:51.000000 nibe-2.2.0/nibe.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-03 19:17:41.000000 nibe-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-03 19:17:51.249375 nibe-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:17:51.245375 nibe-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-05-03 19:17:41.000000 nibe-2.2.0/tests/test_coil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-03 19:17:41.000000 nibe-2.2.0/tests/test_heatpump.py
```

### Comparing `nibe-2.1.4/LICENSE` & `nibe-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/PKG-INFO` & `nibe-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nibe
-Version: 2.1.4
+Version: 2.2.0
 Summary: Nibe heatpump communication library
 Home-page: https://github.com/yozik04/nibe
 Author: Jevgeni Kiski
 Author-email: yozik04@gmail.com
 License: LGPL 3
 Project-URL: Bug Tracker, https://github.com/yozik04/nibe/issues
 Keywords: nibe modbus library nibegw
@@ -40,16 +40,21 @@
  - F1255
  - F1345
  - F1355
  - F370
  - F470
  - F730
  - F750
+ - S320
+ - S325
+ - S735
+ - S2125
  - SMO20
  - SMO40
+ - SMOS40
  - VVM225
  - VVM310
  - VVM320
  - VVM325
  - VVM500
 
 ## Connection methods
```

### Comparing `nibe-2.1.4/README.md` & `nibe-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,21 @@
  - F1255
  - F1345
  - F1355
  - F370
  - F470
  - F730
  - F750
+ - S320
+ - S325
+ - S735
+ - S2125
  - SMO20
  - SMO40
+ - SMOS40
  - VVM225
  - VVM310
  - VVM320
  - VVM325
  - VVM500
 
 ## Connection methods
```

### Comparing `nibe-2.1.4/nibe/coil.py` & `nibe-2.2.0/nibe/coil.py`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/coil_groups.py` & `nibe-2.2.0/nibe/coil_groups.py`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/connection/__init__.py` & `nibe-2.2.0/nibe/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/connection/encoders.py` & `nibe-2.2.0/nibe/connection/encoders.py`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/connection/mixins.py` & `nibe-2.2.0/nibe/connection/mixins.py`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/connection/modbus.py` & `nibe-2.2.0/nibe/connection/modbus.py`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/connection/nibegw.py` & `nibe-2.2.0/nibe/connection/nibegw.py`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/console_scripts/cli.py` & `nibe-2.2.0/nibe/console_scripts/cli.py`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/console_scripts/convert_csv.py` & `nibe-2.2.0/nibe/console_scripts/convert_csv.py`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/extensions.json` & `nibe-2.2.0/nibe/data/extensions.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/f1145_f1245.json` & `nibe-2.2.0/nibe/data/f1145_f1245.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/f1155_f1255.json` & `nibe-2.2.0/nibe/data/f1155_f1255.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/f1345.json` & `nibe-2.2.0/nibe/data/f1345.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/f1355.json` & `nibe-2.2.0/nibe/data/f1355.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/f370_f470.json` & `nibe-2.2.0/nibe/data/f370_f470.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/f730.json` & `nibe-2.2.0/nibe/data/f730.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/f750.json` & `nibe-2.2.0/nibe/data/f750.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/s1155_s1255.json` & `nibe-2.2.0/nibe/data/s1155_s1255.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/s2125.json` & `nibe-2.2.0/nibe/data/s2125.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/s320_s325.json` & `nibe-2.2.0/nibe/data/s320_s325.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/smo20.json` & `nibe-2.2.0/nibe/data/smo20.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/smo40.json` & `nibe-2.2.0/nibe/data/smo40.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/smos40.json` & `nibe-2.2.0/nibe/data/smos40.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9691808596918086%*

 * *Differences: {"'31007'": "OrderedDict([('title', 'Has one phase (EB102)'), ('factor', 1), ('size', 'u8'), "*

 * *            "('name', 'has-one-phase-eb102-31007')])",*

 * * "'31008'": "OrderedDict([('title', 'Serial index (EB102)'), ('factor', 1), ('size', 'u8'), "*

 * *            "('name', 'serial-index-eb102-31008')])",*

 * * "'31407'": "OrderedDict([('title', 'Version (EB102)'), ('factor', 1), ('size', 'u16'), ('name', "*

 * *            "'version-eb102-31407')])",*

 * * "'31408'": "OrderedDict([('title', 'Heat pump type (EB102)'), ('factor', 1 […]*

```diff
@@ -3235,14 +3235,26 @@
     },
     "30994": {
         "factor": 1,
         "name": "outd-air-heat-pump-inverter-speed-reducing-30994",
         "size": "u8",
         "title": "Outd. air heat pump, inverter, speed reducing"
     },
+    "31007": {
+        "factor": 1,
+        "name": "has-one-phase-eb102-31007",
+        "size": "u8",
+        "title": "Has one phase (EB102)"
+    },
+    "31008": {
+        "factor": 1,
+        "name": "serial-index-eb102-31008",
+        "size": "u8",
+        "title": "Serial index (EB102)"
+    },
     "31009": {
         "factor": 1,
         "name": "has-one-phase-eb101-31009",
         "size": "u8",
         "title": "Has one phase (EB101)"
     },
     "31010": {
@@ -3525,14 +3537,121 @@
     },
     "31136": {
         "factor": 1,
         "name": "docked-compressors-pool-2-31136",
         "size": "u8",
         "title": "Docked compressors pool 2"
     },
+    "31407": {
+        "factor": 1,
+        "name": "version-eb102-31407",
+        "size": "u16",
+        "title": "Version (EB102)"
+    },
+    "31408": {
+        "factor": 1,
+        "name": "heat-pump-type-eb102-31408",
+        "size": "u8",
+        "title": "Heat pump type (EB102)"
+    },
+    "31409": {
+        "factor": 1,
+        "name": "compressor-size-eb102-31409",
+        "size": "u8",
+        "title": "Compressor size (EB102)"
+    },
+    "31431": {
+        "factor": 10,
+        "name": "return-line-eb102-bt3-31431",
+        "size": "s16",
+        "title": "Return line (EB102-BT3)",
+        "unit": "\u00b0C"
+    },
+    "31434": {
+        "factor": 10,
+        "name": "supply-line-eb102-bt12-31434",
+        "size": "s16",
+        "title": "Supply line (EB102-BT12)",
+        "unit": "\u00b0C"
+    },
+    "31435": {
+        "factor": 10,
+        "name": "discharge-eb102-bt14-31435",
+        "size": "s16",
+        "title": "Discharge (EB102-BT14)",
+        "unit": "\u00b0C"
+    },
+    "31436": {
+        "factor": 10,
+        "name": "liquid-line-eb102-bt15-31436",
+        "size": "s16",
+        "title": "Liquid line (EB102-BT15)",
+        "unit": "\u00b0C"
+    },
+    "31437": {
+        "factor": 10,
+        "name": "suction-gas-eb102-bt17-31437",
+        "size": "s16",
+        "title": "Suction gas (EB102-BT17)",
+        "unit": "\u00b0C"
+    },
+    "31440": {
+        "factor": 1,
+        "name": "compressor-status-eb102-31440",
+        "size": "u8",
+        "title": "Compressor status (EB102)"
+    },
+    "31441": {
+        "factor": 1,
+        "name": "compressor-time-to-start-eb102-ep14-31441",
+        "size": "u8",
+        "title": "Compressor, time to start (EB102-EP14)",
+        "unit": "min"
+    },
+    "31442": {
+        "factor": 1,
+        "name": "relay-status-eb102-ep14-31442",
+        "size": "u16",
+        "title": "Relay status (EB102-EP14)"
+    },
+    "31445": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-number-of-starts-eb102-ep14-31445",
+        "size": "u32",
+        "title": "Compressor, number of starts (EB102-EP14)"
+    },
+    "31447": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-oper-time-total-eb102-ep14-31447",
+        "size": "u32",
+        "title": "Compressor, oper. time, total (EB102-EP14)",
+        "unit": "h"
+    },
+    "31449": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 2147483647.0,
+        "min": -2147483648.0,
+        "name": "compressor-oper-time-hot-water-eb102-ep14-31449",
+        "size": "u32",
+        "title": "Compressor, oper. time, hot water (EB102-EP14)",
+        "unit": "h"
+    },
+    "31451": {
+        "factor": 1,
+        "name": "alarm-number-eb102-ep14-31451",
+        "size": "u16",
+        "title": "Alarm number (EB102-EP14)"
+    },
     "31452": {
         "factor": 1,
         "name": "version-eb101-31452",
         "size": "u16",
         "title": "Version (EB101)"
     },
     "31453": {
@@ -3932,14 +4051,28 @@
     "31590": {
         "factor": 1,
         "name": "speed-gp12-31590",
         "size": "u8",
         "title": "Speed (GP12)",
         "unit": "%"
     },
+    "31618": {
+        "factor": 10,
+        "name": "outdoor-temperature-eb102-bt28-31618",
+        "size": "s16",
+        "title": "Outdoor temperature (EB102-BT28)",
+        "unit": "\u00b0C"
+    },
+    "31619": {
+        "factor": 10,
+        "name": "evaporator-eb102-bt16-31619",
+        "size": "s16",
+        "title": "Evaporator (EB102-BT16)",
+        "unit": "\u00b0C"
+    },
     "31622": {
         "factor": 10,
         "name": "outdoor-temperature-eb101-bt28-31622",
         "size": "s16",
         "title": "Outdoor temperature (EB101-BT28)",
         "unit": "\u00b0C"
     },
@@ -3974,14 +4107,21 @@
     "31627": {
         "factor": 10,
         "name": "eb100-ep14-bt16-31627",
         "size": "s16",
         "title": "(EB100-EP14-BT16)",
         "unit": "\u00b0C"
     },
+    "31636": {
+        "factor": 1,
+        "name": "charge-pump-speed-eb102-gp12-31636",
+        "size": "u8",
+        "title": "Charge pump speed (EB102-GP12)",
+        "unit": "%"
+    },
     "31637": {
         "factor": 1,
         "name": "heating-medium-pump-speed-gp1-31637",
         "size": "u8",
         "title": "Heating medium pump speed (GP1)",
         "unit": "%"
     },
@@ -4311,14 +4451,41 @@
     },
     "31787": {
         "factor": 1,
         "name": "bp4-unprocessed-eb102-ep14-31787",
         "size": "s16",
         "title": "BP4, unprocessed (EB102-EP14)"
     },
+    "31788": {
+        "factor": 10,
+        "name": "pressure-condenser-eb102-bp4-31788",
+        "size": "s16",
+        "title": "Pressure, condenser (EB102-BP4)",
+        "unit": "bar"
+    },
+    "31789": {
+        "factor": 10,
+        "name": "low-pressure-eb102-bp8-31789",
+        "size": "s16",
+        "title": "Low pressure (EB102-BP8)",
+        "unit": "bar"
+    },
+    "31790": {
+        "factor": 10,
+        "name": "current-compressor-frequency-eb102-31790",
+        "size": "s16",
+        "title": "Current compressor frequency (EB102)",
+        "unit": "Hz"
+    },
+    "31791": {
+        "factor": 1,
+        "name": "protection-mode-eb102-31791",
+        "size": "u16",
+        "title": "Protection mode (EB102)"
+    },
     "31792": {
         "factor": 1,
         "name": "defrosting-eb102-31792",
         "size": "u8",
         "title": "Defrosting (EB102)"
     },
     "31793": {
@@ -4362,14 +4529,21 @@
     },
     "31801": {
         "factor": 1,
         "name": "bp4-unprocessed-eb101-ep14-31801",
         "size": "s16",
         "title": "BP4, unprocessed (EB101-EP14)"
     },
+    "31802": {
+        "factor": 10,
+        "name": "pressure-sensor-condenser-eb101-bp4-31802",
+        "size": "s16",
+        "title": "Pressure sensor, condenser (EB101-BP4)",
+        "unit": "bar"
+    },
     "31803": {
         "factor": 10,
         "name": "low-pressure-eb101-bp8-31803",
         "size": "s16",
         "title": "Low pressure (EB101-BP8)",
         "unit": "bar"
     },
@@ -4582,14 +4756,21 @@
     "31852": {
         "factor": 1,
         "name": "requested-compressor-frequency-eb102-ep15-31852",
         "size": "u8",
         "title": "Requested compressor frequency (EB102-EP15)",
         "unit": "Hz"
     },
+    "31853": {
+        "factor": 1,
+        "name": "requested-compressor-frequency-eb102-31853",
+        "size": "u8",
+        "title": "Requested compressor frequency (EB102)",
+        "unit": "Hz"
+    },
     "31854": {
         "factor": 1,
         "name": "requested-compressor-frequency-eb101-ep15-31854",
         "size": "u8",
         "title": "Requested compressor frequency (EB101-EP15)",
         "unit": "Hz"
     },
@@ -4610,14 +4791,27 @@
     "31857": {
         "factor": 1,
         "name": "requested-compressor-frequency-31857",
         "size": "u8",
         "title": "Requested compressor frequency",
         "unit": "Hz"
     },
+    "31897": {
+        "factor": 1,
+        "name": "low-press-sensor-unprocessed-eb102-ep14-31897",
+        "size": "s16",
+        "title": "Low press. sensor, unprocessed (EB102-EP14)"
+    },
+    "31898": {
+        "factor": 10,
+        "name": "current-sensor-eb102-ep14-31898",
+        "size": "s16",
+        "title": "Current sensor (EB102-EP14)",
+        "unit": "A"
+    },
     "31903": {
         "factor": 1,
         "name": "low-press-sensor-unprocessed-eb101-ep14-31903",
         "size": "s16",
         "title": "Low press. sensor, unprocessed (EB101-EP14)"
     },
     "31904": {
@@ -4697,14 +4891,34 @@
     },
     "31919": {
         "factor": 1,
         "name": "operating-mode-smart-price-adaption-31919",
         "size": "u8",
         "title": "Operating mode (Smart Price Adaption)"
     },
+    "31961": {
+        "factor": 10,
+        "name": "evaporator-2-eb102-ep14-bt16-31961",
+        "size": "s16",
+        "title": "Evaporator 2 (EB102-EP14-BT16)",
+        "unit": "\u00b0C"
+    },
+    "31962": {
+        "factor": 10,
+        "name": "temperature-inverter-eb102-ep14-31962",
+        "size": "s16",
+        "title": "Temperature, inverter (EB102-EP14)",
+        "unit": "\u00b0C"
+    },
+    "31963": {
+        "factor": 1,
+        "name": "fan-speed-eb102-ep14-31963",
+        "size": "u8",
+        "title": "fan speed (EB102-EP14)"
+    },
     "31967": {
         "factor": 10,
         "name": "evaporator-2-eb101-ep14-bt16-31967",
         "size": "s16",
         "title": "Evaporator 2 (EB101-EP14-BT16)",
         "unit": "\u00b0C"
     },
@@ -6285,14 +6499,24 @@
         "max": 1.0,
         "min": 0.0,
         "name": "acs-40732",
         "size": "u8",
         "title": "ACS",
         "write": true
     },
+    "40748": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "operating-mode-charge-pump-climate-system-2-40748",
+        "size": "u8",
+        "title": "Operating mode charge pump climate system 2",
+        "write": true
+    },
     "40749": {
         "default": 0.0,
         "factor": 1,
         "max": 1.0,
         "min": 0.0,
         "name": "operating-mode-charge-pump-climate-system-1-40749",
         "size": "u8",
@@ -6345,14 +6569,24 @@
         "max": 59.0,
         "min": 0.0,
         "name": "input-aux5-40768",
         "size": "u8",
         "title": "Input AUX5",
         "write": true
     },
+    "40783": {
+        "default": 1.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "operating-mode-circulation-pump-heating-heat-pump-2-40783",
+        "size": "u8",
+        "title": "Operating mode circulation pump heating heat pump 2",
+        "write": true
+    },
     "40784": {
         "default": 1.0,
         "factor": 1,
         "max": 1.0,
         "min": 0.0,
         "name": "operating-mode-circulation-pump-heating-heat-pump-1-40784",
         "size": "u8",
@@ -6435,14 +6669,25 @@
         "max": 1.0,
         "min": 0.0,
         "name": "operating-mode-circulation-pump-hot-water-heat-pump-1-40800",
         "size": "u8",
         "title": "Operating mode circulation pump hot water heat pump 1",
         "write": true
     },
+    "40841": {
+        "default": 30.0,
+        "factor": 1,
+        "max": 100.0,
+        "min": 1.0,
+        "name": "speed-circulation-pump-waiting-mode-heat-pump-2-40841",
+        "size": "u8",
+        "title": "Speed circulation pump waiting mode heat pump 2",
+        "unit": "%",
+        "write": true
+    },
     "40842": {
         "default": 30.0,
         "factor": 1,
         "max": 100.0,
         "min": 1.0,
         "name": "speed-circulation-pump-waiting-mode-heat-pump-1-40842",
         "size": "u8",
@@ -6497,14 +6742,25 @@
         "max": 1.0,
         "min": 0.0,
         "name": "internal-shunt-controlled-additional-heat-40858",
         "size": "u8",
         "title": "Internal shunt controlled additional heat",
         "write": true
     },
+    "40867": {
+        "default": 100.0,
+        "factor": 1,
+        "max": 100.0,
+        "min": 80.0,
+        "name": "max-speed-controlled-charge-pump-eb102-40867",
+        "size": "u8",
+        "title": "Max. speed controlled charge pump (EB102)",
+        "unit": "%",
+        "write": true
+    },
     "40868": {
         "default": 100.0,
         "factor": 1,
         "max": 100.0,
         "min": 80.0,
         "name": "max-speed-controlled-charge-pump-eb101-40868",
         "size": "u8",
@@ -9219,25 +9475,47 @@
         "min": -50.0,
         "name": "bt12-offset-heat-pump-1-43235",
         "size": "s8",
         "title": "BT12 offset, heat pump 1",
         "unit": "\u00b0C",
         "write": true
     },
+    "43236": {
+        "default": 0.0,
+        "factor": 10,
+        "max": 50.0,
+        "min": -50.0,
+        "name": "bt12-offset-heat-pump-2-43236",
+        "size": "s8",
+        "title": "BT12 offset, heat pump 2",
+        "unit": "\u00b0C",
+        "write": true
+    },
     "43244": {
         "default": 1.0,
         "factor": 1,
         "max": 50.0,
         "min": 1.0,
         "name": "minimum-permitted-speed-eb101-gp12-43244",
         "size": "u8",
         "title": "Minimum permitted speed (EB101 GP12)",
         "unit": "%",
         "write": true
     },
+    "43245": {
+        "default": 1.0,
+        "factor": 1,
+        "max": 50.0,
+        "min": 1.0,
+        "name": "minimum-permitted-speed-eb102-gp12-43245",
+        "size": "u8",
+        "title": "Minimum permitted speed (EB102 GP12)",
+        "unit": "%",
+        "write": true
+    },
     "43252": {
         "default": 0.0,
         "factor": 1,
         "max": 1.0,
         "min": 0.0,
         "name": "start-fan-de-icing-eb101-43252",
         "size": "s8",
@@ -9499,14 +9777,24 @@
         "min": 50.0,
         "name": "external-adjustment-with-room-sensor-cooling-climate-system-1-44154",
         "size": "s16",
         "title": "External adjustment with room sensor, cooling climate system 1",
         "unit": "\u00b0C",
         "write": true
     },
+    "44158": {
+        "default": 0.0,
+        "factor": 1,
+        "max": 1.0,
+        "min": 0.0,
+        "name": "blockfreq-2-eb102-44158",
+        "size": "u8",
+        "title": "BlockFreq 2 (EB102)",
+        "write": true
+    },
     "44165": {
         "default": 0.0,
         "factor": 1,
         "max": 1.0,
         "min": 0.0,
         "name": "blockfreq-1-eb102-44165",
         "size": "u8",
```

### Comparing `nibe-2.1.4/nibe/data/vvm225_vvm320_vvm325.json` & `nibe-2.2.0/nibe/data/vvm225_vvm320_vvm325.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/data/vvm310_vvm500.json` & `nibe-2.2.0/nibe/data/vvm310_vvm500.json`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/event_server.py` & `nibe-2.2.0/nibe/event_server.py`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/exceptions.py` & `nibe-2.2.0/nibe/exceptions.py`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe/heatpump.py` & `nibe-2.2.0/nibe/heatpump.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 
     F370 = "f370_f470", Series.F
     F470 = "f370_f470", Series.F
 
     S320 = "s320_s325", Series.S
     S325 = "s320_s325", Series.S
 
+    S735 = "s735", Series.S
+
     S2125 = "s2125", Series.S
 
     SMO20 = "smo20", Series.F
     SMO40 = "smo40", Series.F
 
     SMOS40 = "smos40", Series.S
```

### Comparing `nibe-2.1.4/nibe/parsers.py` & `nibe-2.2.0/nibe/parsers.py`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/nibe.egg-info/PKG-INFO` & `nibe-2.2.0/nibe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nibe
-Version: 2.1.4
+Version: 2.2.0
 Summary: Nibe heatpump communication library
 Home-page: https://github.com/yozik04/nibe
 Author: Jevgeni Kiski
 Author-email: yozik04@gmail.com
 License: LGPL 3
 Project-URL: Bug Tracker, https://github.com/yozik04/nibe/issues
 Keywords: nibe modbus library nibegw
@@ -40,16 +40,21 @@
  - F1255
  - F1345
  - F1355
  - F370
  - F470
  - F730
  - F750
+ - S320
+ - S325
+ - S735
+ - S2125
  - SMO20
  - SMO40
+ - SMOS40
  - VVM225
  - VVM310
  - VVM320
  - VVM325
  - VVM500
 
 ## Connection methods
```

### Comparing `nibe-2.1.4/nibe.egg-info/SOURCES.txt` & `nibe-2.2.0/nibe.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 nibe/data/f1355.json
 nibe/data/f370_f470.json
 nibe/data/f730.json
 nibe/data/f750.json
 nibe/data/s1155_s1255.json
 nibe/data/s2125.json
 nibe/data/s320_s325.json
+nibe/data/s735.json
 nibe/data/smo20.json
 nibe/data/smo40.json
 nibe/data/smos40.json
 nibe/data/vvm225_vvm320_vvm325.json
 nibe/data/vvm310_vvm500.json
 tests/test_coil.py
 tests/test_heatpump.py
```

### Comparing `nibe-2.1.4/setup.cfg` & `nibe-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/tests/test_coil.py` & `nibe-2.2.0/tests/test_coil.py`

 * *Files identical despite different names*

### Comparing `nibe-2.1.4/tests/test_heatpump.py` & `nibe-2.2.0/tests/test_heatpump.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         (Model.VVM320, Series.F),
         (Model.VVM325, Series.F),
         (Model.VVM310, Series.F),
         (Model.VVM500, Series.F),
         (Model.SMOS40, Series.S),
         (Model.S320, Series.S),
         (Model.S325, Series.S),
+        (Model.S735, Series.S),
         (Model.S1155, Series.S),
         (Model.S1255, Series.S),
     ],
 )
 def test_series(model: Model, series: Series):
     heat_pump = HeatPump(model)
     assert heat_pump.series == series
```

