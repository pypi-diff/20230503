# Comparing `tmp/enterprise-platform-compute-0.0.2.tar.gz` & `tmp/enterprise-platform-compute-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enterprise-platform-compute-0.0.2.tar", last modified: Thu Apr 20 03:34:57 2023, max compression
+gzip compressed data, was "enterprise-platform-compute-0.0.3.tar", last modified: Wed May  3 14:34:22 2023, max compression
```

## Comparing `enterprise-platform-compute-0.0.2.tar` & `enterprise-platform-compute-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:34:57.755314 enterprise-platform-compute-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-20 03:34:57.755314 enterprise-platform-compute-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:34:57.755314 enterprise-platform-compute-0.0.2/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-20 03:34:49.000000 enterprise-platform-compute-0.0.2/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 03:34:49.000000 enterprise-platform-compute-0.0.2/compute/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-20 03:34:49.000000 enterprise-platform-compute-0.0.2/compute/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-20 03:34:49.000000 enterprise-platform-compute-0.0.2/compute/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-20 03:34:49.000000 enterprise-platform-compute-0.0.2/compute/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-20 03:34:49.000000 enterprise-platform-compute-0.0.2/compute/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 03:34:49.000000 enterprise-platform-compute-0.0.2/compute/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-20 03:34:49.000000 enterprise-platform-compute-0.0.2/compute/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 03:34:57.755314 enterprise-platform-compute-0.0.2/enterprise_platform_compute.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-20 03:34:57.000000 enterprise-platform-compute-0.0.2/enterprise_platform_compute.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-20 03:34:57.000000 enterprise-platform-compute-0.0.2/enterprise_platform_compute.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 03:34:57.000000 enterprise-platform-compute-0.0.2/enterprise_platform_compute.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-20 03:34:57.000000 enterprise-platform-compute-0.0.2/enterprise_platform_compute.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 03:34:57.000000 enterprise-platform-compute-0.0.2/enterprise_platform_compute.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 03:34:57.755314 enterprise-platform-compute-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-20 03:34:49.000000 enterprise-platform-compute-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:34:22.576304 enterprise-platform-compute-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-03 14:34:22.576304 enterprise-platform-compute-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-03 14:34:12.000000 enterprise-platform-compute-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:34:22.576304 enterprise-platform-compute-0.0.3/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-03 14:34:12.000000 enterprise-platform-compute-0.0.3/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-03 14:34:12.000000 enterprise-platform-compute-0.0.3/compute/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-03 14:34:12.000000 enterprise-platform-compute-0.0.3/compute/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-05-03 14:34:12.000000 enterprise-platform-compute-0.0.3/compute/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-03 14:34:12.000000 enterprise-platform-compute-0.0.3/compute/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-03 14:34:12.000000 enterprise-platform-compute-0.0.3/compute/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-03 14:34:12.000000 enterprise-platform-compute-0.0.3/compute/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 14:34:12.000000 enterprise-platform-compute-0.0.3/compute/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-03 14:34:12.000000 enterprise-platform-compute-0.0.3/compute/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-03 14:34:12.000000 enterprise-platform-compute-0.0.3/compute/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:34:22.576304 enterprise-platform-compute-0.0.3/enterprise_platform_compute.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-03 14:34:22.000000 enterprise-platform-compute-0.0.3/enterprise_platform_compute.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 14:34:22.000000 enterprise-platform-compute-0.0.3/enterprise_platform_compute.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:34:22.000000 enterprise-platform-compute-0.0.3/enterprise_platform_compute.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-03 14:34:22.000000 enterprise-platform-compute-0.0.3/enterprise_platform_compute.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 14:34:22.000000 enterprise-platform-compute-0.0.3/enterprise_platform_compute.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:34:22.576304 enterprise-platform-compute-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-03 14:34:12.000000 enterprise-platform-compute-0.0.3/setup.py
```

### Comparing `enterprise-platform-compute-0.0.2/compute/client.py` & `enterprise-platform-compute-0.0.3/compute/client.py`

 * *Files identical despite different names*

### Comparing `enterprise-platform-compute-0.0.2/compute/graph.py` & `enterprise-platform-compute-0.0.3/compute/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import asyncio
 import base64
 import gzip
 import json
 from typing import Callable, Union
 from uuid import uuid4
 
 import networkx as nx
@@ -147,15 +148,15 @@
             return base64.b64encode(ret_compressed).decode("utf-8")
         return ret
 
     def evaluate(self, *, api_key: str, requirements: list[str] = None):
         self.graph.end()
         self.requirements = requirements or []
         execution = Execution.submit(self.json(compress=True), api_key=api_key)
-        execution.poll_for_completion()
+        asyncio.run(execution.join())
         return execution.get_results()
 
 
 class Edge:
     id: str
     source: Node
     target: Node
```

### Comparing `enterprise-platform-compute-0.0.2/compute/utils.py` & `enterprise-platform-compute-0.0.3/compute/utils.py`

 * *Files identical despite different names*

