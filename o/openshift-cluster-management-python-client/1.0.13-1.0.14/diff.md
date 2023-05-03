# Comparing `tmp/openshift-cluster-management-python-client-1.0.13.tar.gz` & `tmp/openshift-cluster-management-python-client-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift-cluster-management-python-client-1.0.13.tar", last modified: Wed May  3 11:51:21 2023, max compression
+gzip compressed data, was "openshift-cluster-management-python-client-1.0.14.tar", last modified: Wed May  3 12:01:26 2023, max compression
```

## Comparing `openshift-cluster-management-python-client-1.0.13.tar` & `openshift-cluster-management-python-client-1.0.14.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 11:51:21.367592 openshift-cluster-management-python-client-1.0.13/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2147 2023-05-03 11:51:21.366592 openshift-cluster-management-python-client-1.0.13/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1270 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/README.md
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 11:51:21.366592 openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13785 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/cluster.py
--rw-r--r--   0 root         (0) root         (0)      554 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2786 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/ocm_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 11:51:21.366592 openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2147 2023-05-03 11:51:21.000000 openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2023-05-03 11:51:21.000000 openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 11:51:21.000000 openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-05-03 11:51:21.000000 openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-03 11:51:21.000000 openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1570 2023-05-03 11:51:19.000000 openshift-cluster-management-python-client-1.0.13/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 11:51:21.367592 openshift-cluster-management-python-client-1.0.13/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:01:26.773316 openshift-cluster-management-python-client-1.0.14/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-05-03 12:01:26.773316 openshift-cluster-management-python-client-1.0.14/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/README.md
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:01:26.773316 openshift-cluster-management-python-client-1.0.14/ocm_python_wrapper/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/ocm_python_wrapper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13785 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/ocm_python_wrapper/cluster.py
+-rw-r--r--   0 root         (0) root         (0)      554 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/ocm_python_wrapper/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/ocm_python_wrapper/ocm_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:01:26.773316 openshift-cluster-management-python-client-1.0.14/openshift_cluster_management_python_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-05-03 12:01:26.000000 openshift-cluster-management-python-client-1.0.14/openshift_cluster_management_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      496 2023-05-03 12:01:26.000000 openshift-cluster-management-python-client-1.0.14/openshift_cluster_management_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 12:01:26.000000 openshift-cluster-management-python-client-1.0.14/openshift_cluster_management_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-05-03 12:01:26.000000 openshift-cluster-management-python-client-1.0.14/openshift_cluster_management_python_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-03 12:01:26.000000 openshift-cluster-management-python-client-1.0.14/openshift_cluster_management_python_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 12:01:26.773316 openshift-cluster-management-python-client-1.0.14/setup.cfg
```

### Comparing `openshift-cluster-management-python-client-1.0.13/LICENSE` & `openshift-cluster-management-python-client-1.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.13/PKG-INFO` & `openshift-cluster-management-python-client-1.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-management-python-client
-Version: 1.0.13
+Version: 1.0.14
 Summary: Wrapper around https://github.com/openshift/openshift-cluster-management-python-client
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-cluster-management-python-client
 Project-URL: Download, https://pypi.org/project/openshift-cluster-management-python-client/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/oopenshift-cluster-management-python-client/issues
 Project-URL: Documentation, https://github.com/rnetser/openshift-cluster-management-python-wrapper/blob/main/README.md
 Keywords: Openshift,OCM
```

### Comparing `openshift-cluster-management-python-client-1.0.13/README.md` & `openshift-cluster-management-python-client-1.0.14/README.md`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/cluster.py` & `openshift-cluster-management-python-client-1.0.14/ocm_python_wrapper/cluster.py`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/exceptions.py` & `openshift-cluster-management-python-client-1.0.14/ocm_python_wrapper/exceptions.py`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.13/ocm_python_wrapper/ocm_client.py` & `openshift-cluster-management-python-client-1.0.14/ocm_python_wrapper/ocm_client.py`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.13/openshift_cluster_management_python_client.egg-info/PKG-INFO` & `openshift-cluster-management-python-client-1.0.14/openshift_cluster_management_python_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-management-python-client
-Version: 1.0.13
+Version: 1.0.14
 Summary: Wrapper around https://github.com/openshift/openshift-cluster-management-python-client
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-cluster-management-python-client
 Project-URL: Download, https://pypi.org/project/openshift-cluster-management-python-client/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/oopenshift-cluster-management-python-client/issues
 Project-URL: Documentation, https://github.com/rnetser/openshift-cluster-management-python-wrapper/blob/main/README.md
 Keywords: Openshift,OCM
```

### Comparing `openshift-cluster-management-python-client-1.0.13/pyproject.toml` & `openshift-cluster-management-python-client-1.0.14/pyproject.toml`

 * *Files identical despite different names*

