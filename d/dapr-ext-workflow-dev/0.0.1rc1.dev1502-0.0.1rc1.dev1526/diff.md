# Comparing `tmp/dapr-ext-workflow-dev-0.0.1rc1.dev1502.tar.gz` & `tmp/dapr-ext-workflow-dev-0.0.1rc1.dev1526.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-ext-workflow-dev-0.0.1rc1.dev1502.tar", last modified: Thu Apr 27 19:57:52 2023, max compression
+gzip compressed data, was "dist/dapr-ext-workflow-dev-0.0.1rc1.dev1526.tar", last modified: Wed May  3 19:50:17 2023, max compression
```

## Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1502.tar` & `dapr-ext-workflow-dev-0.0.1rc1.dev1526.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:52.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-27 19:57:28.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-27 19:57:52.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-27 19:57:28.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:52.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:52.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:52.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr/ext/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-27 19:57:28.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr/ext/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 19:57:28.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr/ext/workflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:57:52.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr_ext_workflow_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-27 19:57:52.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr_ext_workflow_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 19:57:52.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr_ext_workflow_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:57:52.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr_ext_workflow_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 19:57:52.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr_ext_workflow_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 19:57:52.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr_ext_workflow_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-27 19:57:52.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-27 19:57:28.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1502/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:50:17.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-03 19:50:01.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-03 19:50:17.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-03 19:50:01.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:50:17.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:50:17.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:50:17.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr/ext/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-03 19:50:01.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr/ext/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-03 19:50:01.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr/ext/workflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:50:17.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr_ext_workflow_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-03 19:50:17.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr_ext_workflow_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-03 19:50:17.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr_ext_workflow_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:50:17.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr_ext_workflow_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 19:50:17.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr_ext_workflow_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 19:50:17.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr_ext_workflow_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-03 19:50:17.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-03 19:50:01.000000 dapr-ext-workflow-dev-0.0.1rc1.dev1526/setup.py
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1502/LICENSE` & `dapr-ext-workflow-dev-0.0.1rc1.dev1526/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1502/PKG-INFO` & `dapr-ext-workflow-dev-0.0.1rc1.dev1526/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow-dev
-Version: 0.0.1rc1.dev1502
+Version: 0.0.1rc1.dev1526
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr/ext/workflow/__init__.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr/ext/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr/ext/workflow/version.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr/ext/workflow/version.py`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1502/dapr_ext_workflow_dev.egg-info/PKG-INFO` & `dapr-ext-workflow-dev-0.0.1rc1.dev1526/dapr_ext_workflow_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-ext-workflow-dev
-Version: 0.0.1rc1.dev1502
+Version: 0.0.1rc1.dev1526
 Summary: The developmental release for Dapr Workflow Authoring.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1502/setup.cfg` & `dapr-ext-workflow-dev-0.0.1rc1.dev1526/setup.cfg`

 * *Files identical despite different names*

### Comparing `dapr-ext-workflow-dev-0.0.1rc1.dev1502/setup.py` & `dapr-ext-workflow-dev-0.0.1rc1.dev1526/setup.py`

 * *Files identical despite different names*

