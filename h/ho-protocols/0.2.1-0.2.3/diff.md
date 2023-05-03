# Comparing `tmp/ho-protocols-0.2.1.tar.gz` & `tmp/ho-protocols-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ho-protocols-0.2.1.tar", last modified: Tue May  2 12:05:25 2023, max compression
+gzip compressed data, was "ho-protocols-0.2.3.tar", last modified: Wed May  3 14:59:27 2023, max compression
```

## Comparing `ho-protocols-0.2.1.tar` & `ho-protocols-0.2.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1072 2021-12-17 10:20:38.000000 ho-protocols-0.2.1/LICENCE
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/PKG-INFO
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      959 2022-01-14 07:08:59.000000 ho-protocols-0.2.1/README.md
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       38 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/setup.cfg
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1084 2023-04-25 09:43:50.000000 ho-protocols-0.2.1/setup.py
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.581644 ho-protocols-0.2.1/src/
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.593644 ho-protocols-0.2.1/src/ho_protocols/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-17 08:26:26.000000 ho-protocols-0.2.1/src/ho_protocols/__init__.py
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.593644 ho-protocols-0.2.1/src/ho_protocols/alert/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2022-01-12 08:33:24.000000 ho-protocols-0.2.1/src/ho_protocols/alert/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1662 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/alert/alert_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1687 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/alert/alert_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1538 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/alert/bees_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2159 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/alert/bees_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2171 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/alert/system_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3868 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/alert/system_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.593644 ho-protocols-0.2.1/src/ho_protocols/cmd/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-22 12:31:53.000000 ho-protocols-0.2.1/src/ho_protocols/cmd/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3279 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/cmd/cmd_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6358 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/cmd/cmd_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1509 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/common_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1826 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/common_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5246 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/data_in_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    15289 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/data_in_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1563 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/example_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2146 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/example_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/src/ho_protocols/live/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-16 11:50:20.000000 ho-protocols-0.2.1/src/ho_protocols/live/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3207 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/actuators_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6961 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/actuators_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2402 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/live_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2906 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/live_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2573 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/models_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5335 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/models_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2575 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/sensors_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5829 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/sensors_pb2.pyi
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1275 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/system_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1273 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/live/system_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/src/ho_protocols/map/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 09:09:45.000000 ho-protocols-0.2.1/src/ho_protocols/map/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     4556 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/map/map_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    10813 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/map/map_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/src/ho_protocols/query/
--rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-28 10:24:29.000000 ho-protocols-0.2.1/src/ho_protocols/query/__init__.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5090 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/query/query_pb2.py
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    13000 2023-05-02 12:04:57.000000 ho-protocols-0.2.1/src/ho_protocols/query/query_pb2.pyi
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.593644 ho-protocols-0.2.1/src/ho_protocols.egg-info/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-02 12:05:25.000000 ho-protocols-0.2.1/src/ho_protocols.egg-info/PKG-INFO
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1421 2023-05-02 12:05:25.000000 ho-protocols-0.2.1/src/ho_protocols.egg-info/SOURCES.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        1 2023-05-02 12:05:25.000000 ho-protocols-0.2.1/src/ho_protocols.egg-info/dependency_links.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       17 2023-05-02 12:05:25.000000 ho-protocols-0.2.1/src/ho_protocols.egg-info/requires.txt
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       13 2023-05-02 12:05:25.000000 ho-protocols-0.2.1/src/ho_protocols.egg-info/top_level.txt
-drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-02 12:05:25.597644 ho-protocols-0.2.1/test/
--rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      625 2021-12-17 12:38:28.000000 ho-protocols-0.2.1/test/test.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-03 14:59:27.241622 ho-protocols-0.2.3/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1072 2021-12-17 10:20:38.000000 ho-protocols-0.2.3/LICENCE
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-03 14:59:27.241622 ho-protocols-0.2.3/PKG-INFO
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      959 2022-01-14 07:08:59.000000 ho-protocols-0.2.3/README.md
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       38 2023-05-03 14:59:27.241622 ho-protocols-0.2.3/setup.cfg
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1084 2023-04-25 09:43:50.000000 ho-protocols-0.2.3/setup.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-03 14:59:27.229622 ho-protocols-0.2.3/src/
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-03 14:59:27.233622 ho-protocols-0.2.3/src/ho_protocols/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-17 08:26:26.000000 ho-protocols-0.2.3/src/ho_protocols/__init__.py
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-03 14:59:27.233622 ho-protocols-0.2.3/src/ho_protocols/alert/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2022-01-12 08:33:24.000000 ho-protocols-0.2.3/src/ho_protocols/alert/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1662 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/alert/alert_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1687 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/alert/alert_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1538 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/alert/bees_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2159 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/alert/bees_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2171 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/alert/system_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3868 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/alert/system_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-03 14:59:27.233622 ho-protocols-0.2.3/src/ho_protocols/cmd/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-22 12:31:53.000000 ho-protocols-0.2.3/src/ho_protocols/cmd/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3279 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/cmd/cmd_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6358 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/cmd/cmd_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1509 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/common_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1826 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/common_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5246 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/data_in_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    15289 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/data_in_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1563 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/example_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2146 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/example_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-03 14:59:27.237622 ho-protocols-0.2.3/src/ho_protocols/live/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-16 11:50:20.000000 ho-protocols-0.2.3/src/ho_protocols/live/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     3207 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/live/actuators_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     6961 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/live/actuators_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2402 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/live/live_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2906 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/live/live_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2573 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/live/models_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5335 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/live/models_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     2346 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/live/sensors_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     4852 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/live/sensors_pb2.pyi
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1483 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/live/system_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1972 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/live/system_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-03 14:59:27.237622 ho-protocols-0.2.3/src/ho_protocols/map/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        0 2023-02-02 09:09:45.000000 ho-protocols-0.2.3/src/ho_protocols/map/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     4556 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/map/map_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    10813 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/map/map_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-03 14:59:27.241622 ho-protocols-0.2.3/src/ho_protocols/query/
+-rw-r--r--   0 vitaljok  (1000) vitaljok  (1000)        0 2021-12-28 10:24:29.000000 ho-protocols-0.2.3/src/ho_protocols/query/__init__.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     5090 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/query/query_pb2.py
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)    13000 2023-05-03 14:55:41.000000 ho-protocols-0.2.3/src/ho_protocols/query/query_pb2.pyi
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-03 14:59:27.233622 ho-protocols-0.2.3/src/ho_protocols.egg-info/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1351 2023-05-03 14:59:27.000000 ho-protocols-0.2.3/src/ho_protocols.egg-info/PKG-INFO
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)     1421 2023-05-03 14:59:27.000000 ho-protocols-0.2.3/src/ho_protocols.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)        1 2023-05-03 14:59:27.000000 ho-protocols-0.2.3/src/ho_protocols.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       17 2023-05-03 14:59:27.000000 ho-protocols-0.2.3/src/ho_protocols.egg-info/requires.txt
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)       13 2023-05-03 14:59:27.000000 ho-protocols-0.2.3/src/ho_protocols.egg-info/top_level.txt
+drwxrwxr-x   0 vitaljok  (1000) vitaljok  (1000)        0 2023-05-03 14:59:27.241622 ho-protocols-0.2.3/test/
+-rw-rw-r--   0 vitaljok  (1000) vitaljok  (1000)      625 2021-12-17 12:38:28.000000 ho-protocols-0.2.3/test/test.py
```

### Comparing `ho-protocols-0.2.1/LICENCE` & `ho-protocols-0.2.3/LICENCE`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/PKG-INFO` & `ho-protocols-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ho-protocols
-Version: 0.2.1
+Version: 0.2.3
 Summary: ProtoBuf definitions for HO components
 Home-page: https://github.com/hiveopolis/ho-protocols
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ho-protocols-0.2.1/README.md` & `ho-protocols-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/setup.py` & `ho-protocols-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/alert/alert_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/alert/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/alert/alert_pb2.pyi` & `ho-protocols-0.2.3/src/ho_protocols/alert/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/alert/bees_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/alert/bees_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/alert/bees_pb2.pyi` & `ho-protocols-0.2.3/src/ho_protocols/alert/bees_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/alert/system_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/alert/system_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/alert/system_pb2.pyi` & `ho-protocols-0.2.3/src/ho_protocols/alert/system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/cmd/cmd_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/cmd/cmd_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/cmd/cmd_pb2.pyi` & `ho-protocols-0.2.3/src/ho_protocols/cmd/cmd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/common_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/common_pb2.pyi` & `ho-protocols-0.2.3/src/ho_protocols/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/data_in_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/data_in_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/data_in_pb2.pyi` & `ho-protocols-0.2.3/src/ho_protocols/data_in_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/example_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/example_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/example_pb2.pyi` & `ho-protocols-0.2.3/src/ho_protocols/example_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/live/actuators_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/live/actuators_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/live/actuators_pb2.pyi` & `ho-protocols-0.2.3/src/ho_protocols/live/actuators_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/live/live_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/live/live_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/live/live_pb2.pyi` & `ho-protocols-0.2.3/src/ho_protocols/live/live_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/live/models_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/live/models_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/live/models_pb2.pyi` & `ho-protocols-0.2.3/src/ho_protocols/live/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/live/sensors_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/live/sensors_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,29 +9,27 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fho_protocols/live/sensors.proto\x12\x0fho.live.sensors\"\xe9\x01\n\x0eSensorLiveItem\x12/\n\tbroodnest\x18\x01 \x01(\x0b\x32\x1a.ho.live.sensors.BroodnestH\x00\x12\x34\n\x0ctraffic_flow\x18\x02 \x01(\x0b\x32\x1c.ho.live.sensors.TrafficFlowH\x00\x12/\n\tharvester\x18\x03 \x01(\x0b\x32\x1a.ho.live.sensors.HarvesterH\x00\x12\x34\n\x0cpower_supply\x18\x04 \x01(\x0b\x32\x1c.ho.live.sensors.PowerSupplyH\x00\x42\t\n\x07sensors\"2\n\tBroodnest\x12\x0c\n\x04temp\x18\x01 \x03(\x02\x12\n\n\x02rh\x18\x02 \x03(\x02\x12\x0b\n\x03\x63o2\x18\x03 \x01(\x02\"0\n\x0bTrafficFlow\x12\x0f\n\x07\x62\x65\x65s_in\x18\x01 \x03(\x02\x12\x10\n\x08\x62\x65\x65s_out\x18\x02 \x03(\x02\"\x1b\n\tHarvester\x12\x0e\n\x06weight\x18\x01 \x01(\x02\"\xb2\x01\n\x0bPowerSupply\x12\x0f\n\x07voltage\x18\x01 \x01(\x02\x12\x14\n\x0c\x63urrent_draw\x18\x02 \x01(\x02\x12\x14\n\x0c\x63urrent_rate\x18\x03 \x01(\x02\x12\x31\n\x05level\x18\x04 \x01(\x0e\x32\".ho.live.sensors.PowerSupply.Level\"3\n\x05Level\x12\x0b\n\x07Unknown\x10\x00\x12\x07\n\x03Low\x10\x01\x12\n\n\x06Medium\x10\x02\x12\x08\n\x04High\x10\x03\x42\x02H\x03\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fho_protocols/live/sensors.proto\x12\x0fho.live.sensors\"\xfb\x01\n\x0eSensorLiveItem\x12\x36\n\rbroodnest_tmp\x18\x01 \x01(\x0b\x32\x1d.ho.live.sensors.BroodnestTmpH\x00\x12\x36\n\rbroodnest_pwr\x18\x02 \x01(\x0b\x32\x1d.ho.live.sensors.BroodnestPwrH\x00\x12\x36\n\rbroodnest_rht\x18\x03 \x01(\x0b\x32\x1d.ho.live.sensors.BroodnestRhtH\x00\x12\x36\n\rbroodnest_co2\x18\x04 \x01(\x0b\x32\x1d.ho.live.sensors.BroodnestCO2H\x00\x42\t\n\x07sensors\"\x1c\n\x0c\x42roodnestTmp\x12\x0c\n\x04temp\x18\x01 \x03(\x02\"V\n\x0c\x42roodnestPwr\x12\x0f\n\x07\x63urrent\x18\x01 \x01(\x02\x12\r\n\x05power\x18\x02 \x01(\x02\x12\x15\n\rshunt_voltage\x18\x03 \x01(\x02\x12\x0f\n\x07voltage\x18\x04 \x01(\x02\"6\n\x0c\x42roodnestRht\x12\x11\n\trel_humid\x18\x01 \x01(\x02\x12\x13\n\x0btemperature\x18\x02 \x01(\x02\"C\n\x0c\x42roodnestCO2\x12\x0b\n\x03\x63o2\x18\x01 \x01(\x02\x12\x11\n\trel_humid\x18\x02 \x01(\x02\x12\x13\n\x0btemperature\x18\x03 \x01(\x02\x42\x02H\x03\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ho_protocols.live.sensors_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'H\003'
   _globals['_SENSORLIVEITEM']._serialized_start=53
-  _globals['_SENSORLIVEITEM']._serialized_end=286
-  _globals['_BROODNEST']._serialized_start=288
-  _globals['_BROODNEST']._serialized_end=338
-  _globals['_TRAFFICFLOW']._serialized_start=340
-  _globals['_TRAFFICFLOW']._serialized_end=388
-  _globals['_HARVESTER']._serialized_start=390
-  _globals['_HARVESTER']._serialized_end=417
-  _globals['_POWERSUPPLY']._serialized_start=420
-  _globals['_POWERSUPPLY']._serialized_end=598
-  _globals['_POWERSUPPLY_LEVEL']._serialized_start=547
-  _globals['_POWERSUPPLY_LEVEL']._serialized_end=598
+  _globals['_SENSORLIVEITEM']._serialized_end=304
+  _globals['_BROODNESTTMP']._serialized_start=306
+  _globals['_BROODNESTTMP']._serialized_end=334
+  _globals['_BROODNESTPWR']._serialized_start=336
+  _globals['_BROODNESTPWR']._serialized_end=422
+  _globals['_BROODNESTRHT']._serialized_start=424
+  _globals['_BROODNESTRHT']._serialized_end=478
+  _globals['_BROODNESTCO2']._serialized_start=480
+  _globals['_BROODNESTCO2']._serialized_end=547
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ho-protocols-0.2.1/src/ho_protocols/live/sensors_pb2.pyi` & `ho-protocols-0.2.3/src/ho_protocols/live/sensors_pb2.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -2,147 +2,129 @@
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
-import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import sys
-import typing
 
-if sys.version_info >= (3, 10):
+if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
 class SensorLiveItem(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    BROODNEST_FIELD_NUMBER: builtins.int
-    TRAFFIC_FLOW_FIELD_NUMBER: builtins.int
-    HARVESTER_FIELD_NUMBER: builtins.int
-    POWER_SUPPLY_FIELD_NUMBER: builtins.int
-    @property
-    def broodnest(self) -> global___Broodnest: ...
-    @property
-    def traffic_flow(self) -> global___TrafficFlow: ...
-    @property
-    def harvester(self) -> global___Harvester: ...
-    @property
-    def power_supply(self) -> global___PowerSupply: ...
+    BROODNEST_TMP_FIELD_NUMBER: builtins.int
+    BROODNEST_PWR_FIELD_NUMBER: builtins.int
+    BROODNEST_RHT_FIELD_NUMBER: builtins.int
+    BROODNEST_CO2_FIELD_NUMBER: builtins.int
+    @property
+    def broodnest_tmp(self) -> global___BroodnestTmp: ...
+    @property
+    def broodnest_pwr(self) -> global___BroodnestPwr: ...
+    @property
+    def broodnest_rht(self) -> global___BroodnestRht: ...
+    @property
+    def broodnest_co2(self) -> global___BroodnestCO2:
+        """TrafficFlow traffic_flow = 2;
+        Harvester harvester = 3;
+        PowerSupply power_supply = 4;
+        """
     def __init__(
         self,
         *,
-        broodnest: global___Broodnest | None = ...,
-        traffic_flow: global___TrafficFlow | None = ...,
-        harvester: global___Harvester | None = ...,
-        power_supply: global___PowerSupply | None = ...,
+        broodnest_tmp: global___BroodnestTmp | None = ...,
+        broodnest_pwr: global___BroodnestPwr | None = ...,
+        broodnest_rht: global___BroodnestRht | None = ...,
+        broodnest_co2: global___BroodnestCO2 | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["broodnest", b"broodnest", "harvester", b"harvester", "power_supply", b"power_supply", "sensors", b"sensors", "traffic_flow", b"traffic_flow"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["broodnest", b"broodnest", "harvester", b"harvester", "power_supply", b"power_supply", "sensors", b"sensors", "traffic_flow", b"traffic_flow"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["sensors", b"sensors"]) -> typing_extensions.Literal["broodnest", "traffic_flow", "harvester", "power_supply"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["broodnest_co2", b"broodnest_co2", "broodnest_pwr", b"broodnest_pwr", "broodnest_rht", b"broodnest_rht", "broodnest_tmp", b"broodnest_tmp", "sensors", b"sensors"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["broodnest_co2", b"broodnest_co2", "broodnest_pwr", b"broodnest_pwr", "broodnest_rht", b"broodnest_rht", "broodnest_tmp", b"broodnest_tmp", "sensors", b"sensors"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["sensors", b"sensors"]) -> typing_extensions.Literal["broodnest_tmp", "broodnest_pwr", "broodnest_rht", "broodnest_co2"] | None: ...
 
 global___SensorLiveItem = SensorLiveItem
 
 @typing_extensions.final
-class Broodnest(google.protobuf.message.Message):
+class BroodnestTmp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TEMP_FIELD_NUMBER: builtins.int
-    RH_FIELD_NUMBER: builtins.int
-    CO2_FIELD_NUMBER: builtins.int
     @property
     def temp(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
-    @property
-    def rh(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
-    co2: builtins.float
     def __init__(
         self,
         *,
         temp: collections.abc.Iterable[builtins.float] | None = ...,
-        rh: collections.abc.Iterable[builtins.float] | None = ...,
-        co2: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["co2", b"co2", "rh", b"rh", "temp", b"temp"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["temp", b"temp"]) -> None: ...
 
-global___Broodnest = Broodnest
+global___BroodnestTmp = BroodnestTmp
 
 @typing_extensions.final
-class TrafficFlow(google.protobuf.message.Message):
+class BroodnestPwr(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    BEES_IN_FIELD_NUMBER: builtins.int
-    BEES_OUT_FIELD_NUMBER: builtins.int
-    @property
-    def bees_in(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
-    @property
-    def bees_out(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
+    CURRENT_FIELD_NUMBER: builtins.int
+    POWER_FIELD_NUMBER: builtins.int
+    SHUNT_VOLTAGE_FIELD_NUMBER: builtins.int
+    VOLTAGE_FIELD_NUMBER: builtins.int
+    current: builtins.float
+    power: builtins.float
+    shunt_voltage: builtins.float
+    voltage: builtins.float
     def __init__(
         self,
         *,
-        bees_in: collections.abc.Iterable[builtins.float] | None = ...,
-        bees_out: collections.abc.Iterable[builtins.float] | None = ...,
+        current: builtins.float = ...,
+        power: builtins.float = ...,
+        shunt_voltage: builtins.float = ...,
+        voltage: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bees_in", b"bees_in", "bees_out", b"bees_out"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["current", b"current", "power", b"power", "shunt_voltage", b"shunt_voltage", "voltage", b"voltage"]) -> None: ...
 
-global___TrafficFlow = TrafficFlow
+global___BroodnestPwr = BroodnestPwr
 
 @typing_extensions.final
-class Harvester(google.protobuf.message.Message):
+class BroodnestRht(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    WEIGHT_FIELD_NUMBER: builtins.int
-    weight: builtins.float
+    REL_HUMID_FIELD_NUMBER: builtins.int
+    TEMPERATURE_FIELD_NUMBER: builtins.int
+    rel_humid: builtins.float
+    temperature: builtins.float
     def __init__(
         self,
         *,
-        weight: builtins.float = ...,
+        rel_humid: builtins.float = ...,
+        temperature: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["weight", b"weight"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["rel_humid", b"rel_humid", "temperature", b"temperature"]) -> None: ...
 
-global___Harvester = Harvester
+global___BroodnestRht = BroodnestRht
 
 @typing_extensions.final
-class PowerSupply(google.protobuf.message.Message):
+class BroodnestCO2(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    class _Level:
-        ValueType = typing.NewType("ValueType", builtins.int)
-        V: typing_extensions.TypeAlias = ValueType
-
-    class _LevelEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[PowerSupply._Level.ValueType], builtins.type):  # noqa: F821
-        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
-        Unknown: PowerSupply._Level.ValueType  # 0
-        Low: PowerSupply._Level.ValueType  # 1
-        Medium: PowerSupply._Level.ValueType  # 2
-        High: PowerSupply._Level.ValueType  # 3
-
-    class Level(_Level, metaclass=_LevelEnumTypeWrapper): ...
-    Unknown: PowerSupply.Level.ValueType  # 0
-    Low: PowerSupply.Level.ValueType  # 1
-    Medium: PowerSupply.Level.ValueType  # 2
-    High: PowerSupply.Level.ValueType  # 3
-
-    VOLTAGE_FIELD_NUMBER: builtins.int
-    CURRENT_DRAW_FIELD_NUMBER: builtins.int
-    CURRENT_RATE_FIELD_NUMBER: builtins.int
-    LEVEL_FIELD_NUMBER: builtins.int
-    voltage: builtins.float
-    current_draw: builtins.float
-    current_rate: builtins.float
-    level: global___PowerSupply.Level.ValueType
+    CO2_FIELD_NUMBER: builtins.int
+    REL_HUMID_FIELD_NUMBER: builtins.int
+    TEMPERATURE_FIELD_NUMBER: builtins.int
+    co2: builtins.float
+    rel_humid: builtins.float
+    temperature: builtins.float
     def __init__(
         self,
         *,
-        voltage: builtins.float = ...,
-        current_draw: builtins.float = ...,
-        current_rate: builtins.float = ...,
-        level: global___PowerSupply.Level.ValueType = ...,
+        co2: builtins.float = ...,
+        rel_humid: builtins.float = ...,
+        temperature: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["current_draw", b"current_draw", "current_rate", b"current_rate", "level", b"level", "voltage", b"voltage"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["co2", b"co2", "rel_humid", b"rel_humid", "temperature", b"temperature"]) -> None: ...
 
-global___PowerSupply = PowerSupply
+global___BroodnestCO2 = BroodnestCO2
```

### Comparing `ho-protocols-0.2.1/src/ho_protocols/live/system_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/live/system_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,21 +9,19 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eho_protocols/live/system.proto\x12\x0eho.live.system\"@\n\x0eSystemLiveItem\x12$\n\x04\x64isk\x18\x01 \x01(\x0b\x32\x14.ho.live.system.DiskH\x00\x42\x08\n\x06system\"\x06\n\x04\x44iskB\x02H\x03\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eho_protocols/live/system.proto\x12\x0eho.live.system\"\xc6\x01\n\x0eSystemLiveItem\x12\x12\n\ndisk_total\x18\x01 \x01(\x03\x12\x11\n\tdisk_used\x18\x02 \x01(\x03\x12\x11\n\tdisk_free\x18\x03 \x01(\x03\x12\x0f\n\x07load_1m\x18\x04 \x01(\x02\x12\x0f\n\x07load_5m\x18\x05 \x01(\x02\x12\x10\n\x08load_15m\x18\x06 \x01(\x02\x12\x11\n\tmem_total\x18\x07 \x01(\x03\x12\x10\n\x08mem_used\x18\x08 \x01(\x03\x12\x11\n\tmem_avail\x18\t \x01(\x03\x12\x0e\n\x06uptime\x18\n \x01(\x02\x42\x02H\x03\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ho_protocols.live.system_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'H\003'
-  _globals['_SYSTEMLIVEITEM']._serialized_start=50
-  _globals['_SYSTEMLIVEITEM']._serialized_end=114
-  _globals['_DISK']._serialized_start=116
-  _globals['_DISK']._serialized_end=122
+  _globals['_SYSTEMLIVEITEM']._serialized_start=51
+  _globals['_SYSTEMLIVEITEM']._serialized_end=249
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ho-protocols-0.2.1/src/ho_protocols/map/map_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/map/map_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/map/map_pb2.pyi` & `ho-protocols-0.2.3/src/ho_protocols/map/map_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/query/query_pb2.py` & `ho-protocols-0.2.3/src/ho_protocols/query/query_pb2.py`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols/query/query_pb2.pyi` & `ho-protocols-0.2.3/src/ho_protocols/query/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/src/ho_protocols.egg-info/PKG-INFO` & `ho-protocols-0.2.3/src/ho_protocols.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ho-protocols
-Version: 0.2.1
+Version: 0.2.3
 Summary: ProtoBuf definitions for HO components
 Home-page: https://github.com/hiveopolis/ho-protocols
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ho-protocols-0.2.1/src/ho_protocols.egg-info/SOURCES.txt` & `ho-protocols-0.2.3/src/ho_protocols.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ho-protocols-0.2.1/test/test.py` & `ho-protocols-0.2.3/test/test.py`

 * *Files identical despite different names*

