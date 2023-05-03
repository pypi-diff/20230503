# Comparing `tmp/ign-gpao-client-0.8.0.tar.gz` & `tmp/ign-gpao-client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ign-gpao-client-0.8.0.tar", last modified: Tue Dec  6 15:18:41 2022, max compression
+gzip compressed data, was "ign-gpao-client-0.9.0.tar", last modified: Thu Dec  8 07:51:51 2022, max compression
```

## Comparing `ign-gpao-client-0.8.0.tar` & `ign-gpao-client-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:18:41.922584 ign-gpao-client-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-06 15:18:41.922584 ign-gpao-client-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2022-12-06 15:17:49.000000 ign-gpao-client-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:18:41.918584 ign-gpao-client-0.8.0/client/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-06 15:17:51.000000 ign-gpao-client-0.8.0/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2022-12-06 15:17:49.000000 ign-gpao-client-0.8.0/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2022-12-06 15:17:49.000000 ign-gpao-client-0.8.0/client/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:18:41.918584 ign-gpao-client-0.8.0/ign_gpao_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-06 15:18:41.000000 ign-gpao-client-0.8.0/ign_gpao_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2022-12-06 15:18:41.000000 ign-gpao-client-0.8.0/ign_gpao_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 15:18:41.000000 ign-gpao-client-0.8.0/ign_gpao_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-06 15:18:41.000000 ign-gpao-client-0.8.0/ign_gpao_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 15:18:41.922584 ign-gpao-client-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      708 2022-12-06 15:17:49.000000 ign-gpao-client-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:18:41.918584 ign-gpao-client-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2022-12-06 15:17:49.000000 ign-gpao-client-0.8.0/test/test_print_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2022-12-06 15:17:49.000000 ign-gpao-client-0.8.0/test/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 07:51:51.060283 ign-gpao-client-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-08 07:51:51.060283 ign-gpao-client-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2022-12-08 07:51:03.000000 ign-gpao-client-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 07:51:51.060283 ign-gpao-client-0.9.0/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-08 07:51:05.000000 ign-gpao-client-0.9.0/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2022-12-08 07:51:03.000000 ign-gpao-client-0.9.0/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2022-12-08 07:51:03.000000 ign-gpao-client-0.9.0/client/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 07:51:51.060283 ign-gpao-client-0.9.0/ign_gpao_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-08 07:51:50.000000 ign-gpao-client-0.9.0/ign_gpao_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2022-12-08 07:51:50.000000 ign-gpao-client-0.9.0/ign_gpao_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 07:51:50.000000 ign-gpao-client-0.9.0/ign_gpao_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-08 07:51:50.000000 ign-gpao-client-0.9.0/ign_gpao_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 07:51:51.060283 ign-gpao-client-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2022-12-08 07:51:03.000000 ign-gpao-client-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 07:51:51.060283 ign-gpao-client-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2022-12-08 07:51:03.000000 ign-gpao-client-0.9.0/test/test_print_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2022-12-08 07:51:03.000000 ign-gpao-client-0.9.0/test/test_worker.py
```

### Comparing `ign-gpao-client-0.8.0/PKG-INFO` & `ign-gpao-client-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ign-gpao-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: Client GPAO
 Home-page: https://github.com/ign-gpao/client.git
 Author: IGN
 Author-email: arnaud.birk@ign.fr
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ign-gpao-client-0.8.0/README.md` & `ign-gpao-client-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ign-gpao-client-0.8.0/client/worker.py` & `ign-gpao-client-0.9.0/client/worker.py`

 * *Files identical despite different names*

### Comparing `ign-gpao-client-0.8.0/ign_gpao_client.egg-info/PKG-INFO` & `ign-gpao-client-0.9.0/ign_gpao_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ign-gpao-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: Client GPAO
 Home-page: https://github.com/ign-gpao/client.git
 Author: IGN
 Author-email: arnaud.birk@ign.fr
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ign-gpao-client-0.8.0/setup.py` & `ign-gpao-client-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ign-gpao-client-0.8.0/test/test_print_loop.py` & `ign-gpao-client-0.9.0/test/test_print_loop.py`

 * *Files identical despite different names*

### Comparing `ign-gpao-client-0.8.0/test/test_worker.py` & `ign-gpao-client-0.9.0/test/test_worker.py`

 * *Files identical despite different names*

