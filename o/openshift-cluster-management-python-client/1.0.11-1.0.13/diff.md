# Comparing `tmp/openshift-cluster-management-python-client-1.0.11.tar.gz` & `tmp/openshift-cluster-management-python-client-1.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift-cluster-management-python-client-1.0.11.tar", last modified: Mon Apr 24 08:49:19 2023, max compression
+gzip compressed data, was "openshift-cluster-management-python-client-1.0.13.tar", last modified: Wed May  3 11:51:21 2023, max compression
```

## Comparing `openshift-cluster-management-python-client-1.0.11.tar` & `openshift-cluster-management-python-client-1.0.13.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:49:19.615628 openshift-cluster-management-python-client-1.0.11/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2147 2023-04-24 08:49:19.615628 openshift-cluster-management-python-client-1.0.11/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1270 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/README.md
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:49:19.615628 openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13664 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/cluster.py
--rw-r--r--   0 root         (0) root         (0)      554 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2432 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/logger.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/ocm_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:49:19.615628 openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2147 2023-04-24 08:49:19.000000 openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      525 2023-04-24 08:49:19.000000 openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 08:49:19.000000 openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-04-24 08:49:19.000000 openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-24 08:49:19.000000 openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1570 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 08:49:19.615628 openshift-cluster-management-python-client-1.0.11/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 11:51:21.367592 openshift-cluster-management-python-client-1.0.13/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-05-03 11:51:21.366592 openshift-cluster-management-python-client-1.0.13/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/README.md
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 11:51:21.366592 openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13785 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/cluster.py
+-rw-r--r--   0 root         (0) root         (0)      554 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/ocm_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 11:51:21.366592 openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-05-03 11:51:21.000000 openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2023-05-03 11:51:21.000000 openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 11:51:21.000000 openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-05-03 11:51:21.000000 openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-03 11:51:21.000000 openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 11:51:21.367592 openshift-cluster-management-python-client-1.0.13/setup.cfg
```

### Comparing `openshift-cluster-management-python-client-1.0.11/LICENSE` & `openshift-cluster-management-python-client-1.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.11/PKG-INFO` & `openshift-cluster-management-python-client-1.0.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-management-python-client
-Version: 1.0.11
+Version: 1.0.13
 Summary: Wrapper around https://github.com/openshift/openshift-cluster-management-python-client
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-cluster-management-python-client
 Project-URL: Download, https://pypi.org/project/openshift-cluster-management-python-client/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/oopenshift-cluster-management-python-client/issues
 Project-URL: Documentation, https://github.com/rnetser/openshift-cluster-management-python-wrapper/blob/main/README.md
 Keywords: Openshift,OCM
```

### Comparing `openshift-cluster-management-python-client-1.0.11/README.md` & `openshift-cluster-management-python-client-1.0.13/README.md`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/cluster.py` & `openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 )
 from ocm_python_client.model.upgrade_policy import UpgradePolicy
 from ocp_resources.constants import NOT_FOUND_ERROR_EXCEPTION_DICT
 from ocp_resources.resource import ResourceEditor
 from ocp_resources.rhmi import RHMI
 from ocp_resources.utils import TimeoutExpiredError, TimeoutSampler
 from ocp_utilities.infra import get_client
+from simple_logger.logger import get_logger
 
 from ocm_python_wrapper.exceptions import MissingResourceError
-from ocm_python_wrapper.logger import get_logger
 
 LOGGER = get_logger(__name__)
 TIMEOUT_10MIN = 10 * 60
 TIMEOUT_30MIN = 30 * 60
 SLEEP_1SEC = 1
 
 
@@ -368,20 +368,23 @@
                     return True
         LOGGER.info(f"{self.addon_name} was successfully removed")
         return res
 
     @staticmethod
     def update_rhoam_cluster_storage_config():
         def _wait_for_rhmi_resource():
-            for sample in TimeoutSampler(
+            for rhmi_sample in TimeoutSampler(
                 wait_timeout=TIMEOUT_30MIN,
                 sleep=SLEEP_1SEC,
                 func=lambda: RHMI(name="rhoam", namespace="redhat-rhoam-operator"),
-                exceptions_dict=NOT_FOUND_ERROR_EXCEPTION_DICT,
+                exceptions_dict={
+                    NotImplementedError: [],
+                    **NOT_FOUND_ERROR_EXCEPTION_DICT,
+                },
             ):
-                if sample:
-                    return sample
+                if rhmi_sample and rhmi_sample.exists:
+                    return rhmi_sample
 
         rhmi = _wait_for_rhmi_resource()
         ResourceEditor(
             patches={rhmi: {"spec": {"useClusterStorage": "false"}}}
         ).update()
```

### Comparing `openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/exceptions.py` & `openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/exceptions.py`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/ocm_client.py` & `openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/ocm_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/bin/python
 
 import requests
 from ocm_python_client.api.default_api import DefaultApi
 from ocm_python_client.api_client import ApiClient
 from ocm_python_client.configuration import Configuration
 from ocm_python_client.exceptions import UnauthorizedException
+from simple_logger.logger import get_logger
 
 from ocm_python_wrapper.exceptions import AuthenticationError, EndpointAccessError
-from ocm_python_wrapper.logger import get_logger
 
 LOGGER = get_logger(__name__)
 
 
 class OCMPythonClient(ApiClient):
     def __init__(
         self,
```

### Comparing `openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/PKG-INFO` & `openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-management-python-client
-Version: 1.0.11
+Version: 1.0.13
 Summary: Wrapper around https://github.com/openshift/openshift-cluster-management-python-client
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-cluster-management-python-client
 Project-URL: Download, https://pypi.org/project/openshift-cluster-management-python-client/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/oopenshift-cluster-management-python-client/issues
 Project-URL: Documentation, https://github.com/rnetser/openshift-cluster-management-python-wrapper/blob/main/README.md
 Keywords: Openshift,OCM
```

### Comparing `openshift-cluster-management-python-client-1.0.11/pyproject.toml` & `openshift-cluster-management-python-client-1.0.13/pyproject.toml`

 * *Files identical despite different names*

