# Comparing `tmp/frinx_conductor_workers-1.1.8.tar.gz` & `tmp/frinx_conductor_workers-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frinx_conductor_workers-1.1.8.tar", last modified: Tue Apr  4 09:53:57 2023, max compression
+gzip compressed data, was "frinx_conductor_workers-1.1.9.tar", last modified: Tue Apr 11 10:56:43 2023, max compression
```

## Comparing `frinx_conductor_workers-1.1.8.tar` & `frinx_conductor_workers-1.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:53:57.760859 frinx_conductor_workers-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-04 09:53:57.760859 frinx_conductor_workers-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:53:57.756859 frinx_conductor_workers-1.1.8/frinx_conductor_workers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14282 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/cli_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/cli_worker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/common_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/connection_manager_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/frinx_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/http_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/import_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/logging_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/netconf_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/netconf_worker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    58899 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/resource_manager_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    32398 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/uniconfig_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26509 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/uniconfig_worker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:53:57.756859 frinx_conductor_workers-1.1.8/frinx_conductor_workers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-04 09:53:57.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-04 09:53:57.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 09:53:57.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-04 09:53:57.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:53:57.756859 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/Dynamic_fork.json
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/Mount_apply_template_unmount_cli.json
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/UC_TX_close.json
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/UC_TX_commit.json
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/UC_TX_rollback.json
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/UC_TX_start.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 09:53:57.760859 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Prefix_Resource.json
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Resource.json
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Prefix_Resource.json
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Resource.json
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Pool.json
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Prefix_Pool.json
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Pool.json
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Prefix_Pool.json
--rw-r--r--   0 runner    (1001) docker     (123)    17433 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Create_Subnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Deallocate_Resource.json
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv4.json
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv6.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 09:53:57.760859 frinx_conductor_workers-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-04 09:53:45.000000 frinx_conductor_workers-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:56:43.587787 frinx_conductor_workers-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-11 10:56:43.587787 frinx_conductor_workers-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:56:43.583787 frinx_conductor_workers-1.1.9/frinx_conductor_workers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14282 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/cli_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/cli_worker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/common_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/connection_manager_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/frinx_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/http_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/import_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/logging_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/netconf_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/netconf_worker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59280 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/resource_manager_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32398 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/uniconfig_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26509 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/uniconfig_worker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:56:43.583787 frinx_conductor_workers-1.1.9/frinx_conductor_workers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-11 10:56:43.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-11 10:56:43.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:56:43.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-11 10:56:43.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:56:43.583787 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/Dynamic_fork.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/Mount_apply_template_unmount_cli.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/UC_TX_close.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/UC_TX_commit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/UC_TX_rollback.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/UC_TX_start.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:56:43.587787 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Prefix_Resource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Resource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Prefix_Resource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Resource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Pool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Prefix_Pool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Pool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Prefix_Pool.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17433 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Create_Subnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Deallocate_Resource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv6.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:56:43.587787 frinx_conductor_workers-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-11 10:56:31.000000 frinx_conductor_workers-1.1.9/setup.py
```

### Comparing `frinx_conductor_workers-1.1.8/PKG-INFO` & `frinx_conductor_workers-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frinx_conductor_workers
-Version: 1.1.8
+Version: 1.1.9
 Summary: Conductor python client workers
 Home-page: https://github.com/FRINXio/fm-base-workers
 Author: Frinx
 Author-email: info@frinx.io
 License: Apache 2.0
 Keywords: conductor
 Description-Content-Type: text/markdown
```

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/cli_worker.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/cli_worker.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/cli_worker_test.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/cli_worker_test.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/common_worker.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/common_worker.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/connection_manager_worker.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/connection_manager_worker.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/frinx_rest.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/frinx_rest.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/http_worker.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/http_worker.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/import_workflows.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/import_workflows.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/logging_helpers.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/logging_helpers.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/netconf_worker.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/netconf_worker.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/netconf_worker_test.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/netconf_worker_test.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/resource_manager_worker.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/resource_manager_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,15 +422,15 @@
 @logging_handler(log)
 def create_pool(task, logs):
     """
     Create pool id in Uniresource
 
          Args:
 
-             task (dict): dictionary with input data ["resource", "poolName", "poolProperties"]
+             task (dict): dictionary with input data ["resourceType", "poolName", "poolProperties"]
 
              logs: stream of log messages
 
         Returns:
             Response from uniresource. Worker output format::
             "result": {
               "data": {
@@ -458,26 +458,32 @@
     }
     pool_types_string, pool_string, pool_variables_string = "", "", ""
     if task["inputData"]["poolProperties"]:
         pool_properties = task["inputData"]["poolProperties"]
         for index, key in enumerate(pool_properties.keys()):
             variable_type = type(pool_properties[key])
             property_variable = ""
+            # if input from workflow send bool value as string, then it will be converted back to bool
+            if variable_type is str and (
+                pool_properties[key].lower() == "true" or pool_properties[key].lower() == "false"
+            ):
+                variable_type = type(True)
             if variable_type is str:
                 variable_type = "string"
                 property_variable = "String!"
             elif variable_type is dict:
                 variable_type = "map"
                 property_variable = "Map!"
             elif variable_type is int:
                 variable_type = "int"
                 property_variable = "ID!"
             elif variable_type is bool:
                 variable_type = "bool"
                 property_variable = "Boolean"
+                pool_properties[key] = bool(pool_properties[key])
             pool_types_string += key + ': "' + variable_type + '"'
             pool_variables_string += "$" + key + ": " + property_variable
             pool_string += key + ": $" + key
             if index < len(pool_properties.keys()) - 1:
                 pool_string += ",\n"
                 pool_types_string += ",\n"
                 pool_variables_string += ", "
@@ -504,15 +510,15 @@
 
 @logging_handler(log)
 def create_vlan_pool(task, logs):
     """
     Create vlan pool in Uniresource
     Args:
 
-         task (dict): dictionary with input data ["poolName", "from", "to", "parent_resource_id"]
+         task (dict): dictionary with input data ["poolName", "from", "to", "parentResourceId"]
 
          logs: stream of log messages
     """
     pool_name = task["inputData"]["poolName"]
     from_range = task["inputData"]["from"] if "from" in task["inputData"] else None
     to_range = task["inputData"]["to"] if "to" in task["inputData"] else None
     parent_resource_id = (
@@ -597,15 +603,15 @@
 
 @logging_handler(log)
 def create_unique_id_pool(task, logs):
     """
     Create vlan range pool in Uniresource
     Args:
 
-         task (dict): dictionary with input data ["poolName", "idFormat"]
+         task (dict): dictionary with input data ["poolName", "idFormat", "from", "to"]
 
          logs: stream of log messages
     """
     pool_name = task["inputData"]["poolName"]
     id_format = task["inputData"]["idFormat"]
     from_value = task["inputData"]["from"] if "from" in task["inputData"] else None
     if from_value == "":
@@ -655,15 +661,15 @@
 @logging_handler(log)
 def query_pool(task, logs):
     """
     Query pool id in Uniresource
 
          Args:
 
-             task (dict): dictionary with input data ["poolNames", "resourceTypeId"]
+             task (dict): dictionary with input data ["poolNames", "resource"]
 
              logs: stream of log messages
 
         Returns:
             Response from uniresource. Worker output format::
             "result":{
               "data": {
@@ -919,15 +925,15 @@
 @logging_handler(log)
 def calculate_available_prefixes_for_address_pool(task, logs):
     """
     Calculate available prefixes for address pool
 
          Args:
 
-             task (dict): dictionary with input data ["free_capacity", "resource_type"]
+             task (dict): dictionary with input data ["poolId", "resource_type"]
 
              logs: stream of log messages
         Returns:
             "result":{"data": "/24":"1","/25":"2","/26":"4","/27":"8","/28":"16","/29":"32","/30":"64","/31":"128","/32":"256"}}
     """
     pool_id = task["inputData"]["poolId"]
     resource_type = str(task["inputData"]["resourceType"])
@@ -1025,15 +1031,15 @@
 
 
 @logging_handler(log)
 def query_resource_by_alt_id(task, logs):
     """
     Query resource by alternative id in Uniresource
          Args:
-             task (dict): dictionary with input data ["alternativeId"] and optional data ["poolId", "first"]
+             task (dict): dictionary with input data ["alternativeId", "poolId", "first", "last", "after", "before"]
          Returns:
             Response from uniresource. Worker output format::
             "result": {
                 "data": {
                     "QueryResourcesByAltId": {
                         "edges": [
                         {
@@ -1085,15 +1091,15 @@
 @logging_handler(log)
 def deallocate_resource(task, logs):
     """
     Deallocate resource from pool
 
          Args:
 
-             task (dict): dictionary with input data ["poolId", "userInput", "alternativeId"]
+             task (dict): dictionary with input data ["poolId", "userInput"]
 
              logs: stream of log messages
 
         Returns:
             Response from Uniresource. Worker output format:
             "result": {
               "data": {
@@ -1161,15 +1167,15 @@
 @logging_handler(log)
 def calculate_host_and_broadcast_address(task, logs):
     """
     Calculate host and broadcast address from customer and provider ip address, if those ip addresses are not defined, it will calculate even these
 
          Args:
 
-             task (dict): dictionary with input data ["desired_size", "resource_type"] and optional ["customer_address", "provider_address"]
+             task (dict): dictionary with input data ["desiredSize", "resourceType", "customerAddress", "providerAddress", "networkAddress"]
 
              logs: stream of log messages
         Returns:
             "result":{
                 "data": {
                     "network_address": <network_address>
                     "broadcast_address": <broadcast_address>
@@ -1282,15 +1288,15 @@
 @logging_handler(log)
 def calculate_desired_size_from_prefix(task, logs):
     """
     Calculate desired size from prefix
 
          Args:
 
-             task (dict): dictionary with input data ["prefix", "resource_type"]
+             task (dict): dictionary with input data ["prefix", "resourceType", "subnet"]
 
              logs: stream of log messages
         Returns:
             "result": {
                 "data": <desired_size>
             }
     """
@@ -1359,15 +1365,15 @@
 
 
 @logging_handler(log)
 def query_recently_active_resources(task, logs):
     """
     Query resource by alternative id in Uniresource
          Args:
-             task (dict): dictionary with input data ["alternativeId"] and optional data ["poolId", "first"]
+             task (dict): dictionary with input data ["fromDatetime", "toDatetime", "first", "last", "before", "after"]
          Returns:
             Response from uniresource. Worker output format::
             "result": {
                 "data": {
                     "QueryRecentlyActiveResources": {
                         edges {
                             node {
```

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/uniconfig_worker.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/uniconfig_worker.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/uniconfig_worker_test.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/uniconfig_worker_test.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers/util.py` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers/util.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers.egg-info/PKG-INFO` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frinx-conductor-workers
-Version: 1.1.8
+Version: 1.1.9
 Summary: Conductor python client workers
 Home-page: https://github.com/FRINXio/fm-base-workers
 Author: Frinx
 Author-email: info@frinx.io
 License: Apache 2.0
 Keywords: conductor
 Description-Content-Type: text/markdown
```

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workers.egg-info/SOURCES.txt` & `frinx_conductor_workers-1.1.9/frinx_conductor_workers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/Dynamic_fork.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/Dynamic_fork.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/Mount_apply_template_unmount_cli.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/Mount_apply_template_unmount_cli.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/UC_TX_close.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/UC_TX_close.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/UC_TX_commit.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/UC_TX_commit.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/UC_TX_rollback.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/UC_TX_rollback.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/UC_TX_start.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/UC_TX_start.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Prefix_Resource.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Prefix_Resource.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Resource.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Resource.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Prefix_Resource.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Prefix_Resource.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Resource.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Resource.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Pool.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Pool.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Prefix_Pool.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Prefix_Pool.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Pool.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Pool.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Prefix_Pool.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Prefix_Pool.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Create_Subnet.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Create_Subnet.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Deallocate_Resource.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Deallocate_Resource.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv4.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv4.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv6.json` & `frinx_conductor_workers-1.1.9/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv6.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-1.1.8/setup.py` & `frinx_conductor_workers-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def __read__(file_name):
     return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 
 setup(
     name="frinx_conductor_workers",
     packages=["frinx_conductor_workers", "frinx_conductor_workflows"],
-    version="1.1.8",
+    version="1.1.9",
     description="Conductor python client workers",
     author="Frinx",
     author_email="info@frinx.io",
     url="https://github.com/FRINXio/fm-base-workers",
     keywords=["conductor"],
     license="Apache 2.0",
     include_package_data=True,
```

