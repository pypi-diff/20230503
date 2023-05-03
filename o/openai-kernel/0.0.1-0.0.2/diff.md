# Comparing `tmp/openai_kernel-0.0.1.tar.gz` & `tmp/openai_kernel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_kernel-0.0.1.tar", last modified: Wed May  3 17:12:53 2023, max compression
+gzip compressed data, was "openai_kernel-0.0.2.tar", last modified: Wed May  3 17:57:10 2023, max compression
```

## Comparing `openai_kernel-0.0.1.tar` & `openai_kernel-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 danielharrison   (501) staff       (20)        0 2023-05-03 17:12:53.147424 openai_kernel-0.0.1/
--rw-r--r--   0 danielharrison   (501) staff       (20)      627 2023-05-03 17:12:53.147153 openai_kernel-0.0.1/PKG-INFO
--rw-r--r--   0 danielharrison   (501) staff       (20)      278 2023-05-01 15:54:35.000000 openai_kernel-0.0.1/README.md
-drwxr-xr-x   0 danielharrison   (501) staff       (20)        0 2023-05-03 17:12:53.142781 openai_kernel-0.0.1/openai_kernel/
--rw-r--r--   0 danielharrison   (501) staff       (20)      157 2023-05-01 18:14:41.000000 openai_kernel-0.0.1/openai_kernel/__init__.py
--rw-r--r--   0 danielharrison   (501) staff       (20)      105 2023-04-28 21:23:08.000000 openai_kernel-0.0.1/openai_kernel/__main__.py
--rw-r--r--   0 danielharrison   (501) staff       (20)      180 2023-04-27 21:14:47.000000 openai_kernel-0.0.1/openai_kernel/kernel.json
--rw-r--r--   0 danielharrison   (501) staff       (20)     9138 2023-05-01 18:14:41.000000 openai_kernel-0.0.1/openai_kernel/kernel.py
-drwxr-xr-x   0 danielharrison   (501) staff       (20)        0 2023-05-03 17:12:53.146739 openai_kernel-0.0.1/openai_kernel/magics/
--rw-r--r--   0 danielharrison   (501) staff       (20)      202 2023-05-01 18:14:40.000000 openai_kernel-0.0.1/openai_kernel/magics/__init__.py
--rw-r--r--   0 danielharrison   (501) staff       (20)      285 2023-04-28 21:23:08.000000 openai_kernel-0.0.1/openai_kernel/magics/clear_history_magic.py
--rw-r--r--   0 danielharrison   (501) staff       (20)      777 2023-05-01 18:14:41.000000 openai_kernel-0.0.1/openai_kernel/magics/history_magic.py
--rw-r--r--   0 danielharrison   (501) staff       (20)      283 2023-04-28 21:41:52.000000 openai_kernel-0.0.1/openai_kernel/magics/mode_magic.py
--rw-r--r--   0 danielharrison   (501) staff       (20)      628 2023-04-28 21:23:08.000000 openai_kernel-0.0.1/openai_kernel/magics/openai_api_magic.py
--rw-r--r--   0 danielharrison   (501) staff       (20)      634 2023-04-28 21:23:08.000000 openai_kernel-0.0.1/openai_kernel/magics/set_magic.py
--rw-r--r--   0 danielharrison   (501) staff       (20)     2349 2023-05-01 18:14:11.000000 openai_kernel-0.0.1/openai_kernel/mock_kernel.py
--rw-r--r--   0 danielharrison   (501) staff       (20)      270 2023-04-28 21:23:08.000000 openai_kernel-0.0.1/openai_kernel/outputs.py
--rw-r--r--   0 danielharrison   (501) staff       (20)     1210 2023-04-28 21:23:08.000000 openai_kernel-0.0.1/openai_kernel/utils.py
--rw-r--r--   0 danielharrison   (501) staff       (20)       88 2023-04-21 15:50:26.000000 openai_kernel-0.0.1/openai_kernel/version.py
-drwxr-xr-x   0 danielharrison   (501) staff       (20)        0 2023-05-03 17:12:53.144141 openai_kernel-0.0.1/openai_kernel.egg-info/
--rw-r--r--   0 danielharrison   (501) staff       (20)      627 2023-05-03 17:12:53.000000 openai_kernel-0.0.1/openai_kernel.egg-info/PKG-INFO
--rw-r--r--   0 danielharrison   (501) staff       (20)      631 2023-05-03 17:12:53.000000 openai_kernel-0.0.1/openai_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 danielharrison   (501) staff       (20)        1 2023-05-03 17:12:53.000000 openai_kernel-0.0.1/openai_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 danielharrison   (501) staff       (20)       40 2023-05-03 17:12:53.000000 openai_kernel-0.0.1/openai_kernel.egg-info/requires.txt
--rw-r--r--   0 danielharrison   (501) staff       (20)       14 2023-05-03 17:12:53.000000 openai_kernel-0.0.1/openai_kernel.egg-info/top_level.txt
--rw-r--r--   0 danielharrison   (501) staff       (20)       38 2023-05-03 17:12:53.147506 openai_kernel-0.0.1/setup.cfg
--rw-r--r--   0 danielharrison   (501) staff       (20)      854 2023-04-28 21:23:08.000000 openai_kernel-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:57:10.721245 openai_kernel-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-03 17:57:10.721245 openai_kernel-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:57:10.721245 openai_kernel-0.0.2/openai_kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:57:10.721245 openai_kernel-0.0.2/openai_kernel/magics/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/magics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/magics/clear_history_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/magics/history_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/magics/mode_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/magics/openai_api_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/magics/set_magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/mock_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/openai_kernel/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:57:10.721245 openai_kernel-0.0.2/openai_kernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-03 17:57:10.000000 openai_kernel-0.0.2/openai_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-03 17:57:10.000000 openai_kernel-0.0.2/openai_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:57:10.000000 openai_kernel-0.0.2/openai_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 17:57:10.000000 openai_kernel-0.0.2/openai_kernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 17:57:10.000000 openai_kernel-0.0.2/openai_kernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:57:10.721245 openai_kernel-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-03 17:56:58.000000 openai_kernel-0.0.2/setup.py
```

### Comparing `openai_kernel-0.0.1/PKG-INFO` & `openai_kernel-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_kernel
-Version: 0.0.1
+Version: 0.0.2
 Summary: OpenAI jupyter kernel
 Author: Oak City Labs
 Author-email: team@oakcity.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
```

### Comparing `openai_kernel-0.0.1/openai_kernel/kernel.py` & `openai_kernel-0.0.2/openai_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `openai_kernel-0.0.1/openai_kernel/magics/history_magic.py` & `openai_kernel-0.0.2/openai_kernel/magics/history_magic.py`

 * *Files identical despite different names*

### Comparing `openai_kernel-0.0.1/openai_kernel/magics/openai_api_magic.py` & `openai_kernel-0.0.2/openai_kernel/magics/openai_api_magic.py`

 * *Files identical despite different names*

### Comparing `openai_kernel-0.0.1/openai_kernel/magics/set_magic.py` & `openai_kernel-0.0.2/openai_kernel/magics/set_magic.py`

 * *Files identical despite different names*

### Comparing `openai_kernel-0.0.1/openai_kernel/mock_kernel.py` & `openai_kernel-0.0.2/openai_kernel/mock_kernel.py`

 * *Files identical despite different names*

### Comparing `openai_kernel-0.0.1/openai_kernel/utils.py` & `openai_kernel-0.0.2/openai_kernel/utils.py`

 * *Files identical despite different names*

### Comparing `openai_kernel-0.0.1/openai_kernel.egg-info/PKG-INFO` & `openai_kernel-0.0.2/openai_kernel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-kernel
-Version: 0.0.1
+Version: 0.0.2
 Summary: OpenAI jupyter kernel
 Author: Oak City Labs
 Author-email: team@oakcity.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
```

### Comparing `openai_kernel-0.0.1/openai_kernel.egg-info/SOURCES.txt` & `openai_kernel-0.0.2/openai_kernel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai_kernel-0.0.1/setup.py` & `openai_kernel-0.0.2/setup.py`

 * *Files identical despite different names*

