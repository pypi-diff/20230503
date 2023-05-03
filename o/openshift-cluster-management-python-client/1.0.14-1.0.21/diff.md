# Comparing `tmp/openshift-cluster-management-python-client-1.0.14.tar.gz` & `tmp/openshift-cluster-management-python-client-1.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift-cluster-management-python-client-1.0.14.tar", last modified: Wed May  3 12:01:26 2023, max compression
+gzip compressed data, was "openshift-cluster-management-python-client-1.0.21.tar", last modified: Wed May  3 12:36:18 2023, max compression
```

## Comparing `openshift-cluster-management-python-client-1.0.14.tar` & `openshift-cluster-management-python-client-1.0.21.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:01:26.773316 openshift-cluster-management-python-client-1.0.14/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2147 2023-05-03 12:01:26.773316 openshift-cluster-management-python-client-1.0.14/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1270 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/README.md
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:01:26.773316 openshift-cluster-management-python-client-1.0.14/ocm_python_wrapper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/ocm_python_wrapper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13785 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/ocm_python_wrapper/cluster.py
--rw-r--r--   0 root         (0) root         (0)      554 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/ocm_python_wrapper/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2786 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/ocm_python_wrapper/ocm_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:01:26.773316 openshift-cluster-management-python-client-1.0.14/openshift_cluster_management_python_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2147 2023-05-03 12:01:26.000000 openshift-cluster-management-python-client-1.0.14/openshift_cluster_management_python_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2023-05-03 12:01:26.000000 openshift-cluster-management-python-client-1.0.14/openshift_cluster_management_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 12:01:26.000000 openshift-cluster-management-python-client-1.0.14/openshift_cluster_management_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-05-03 12:01:26.000000 openshift-cluster-management-python-client-1.0.14/openshift_cluster_management_python_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-03 12:01:26.000000 openshift-cluster-management-python-client-1.0.14/openshift_cluster_management_python_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1570 2023-05-03 12:01:24.000000 openshift-cluster-management-python-client-1.0.14/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 12:01:26.773316 openshift-cluster-management-python-client-1.0.14/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:36:18.034265 openshift-cluster-management-python-client-1.0.21/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    58148 2023-05-03 12:36:18.034265 openshift-cluster-management-python-client-1.0.21/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    57407 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/README.md
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:36:18.033265 openshift-cluster-management-python-client-1.0.21/ocm_python_client/
+-rw-r--r--   0 root         (0) root         (0)      830 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/ocm_python_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39265 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/ocm_python_client/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16702 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/ocm_python_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/ocm_python_client/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    82559 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/ocm_python_client/model_utils.py
+-rw-r--r--   0 root         (0) root         (0)    14345 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/ocm_python_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:36:18.034265 openshift-cluster-management-python-client-1.0.21/openshift_cluster_management_python_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    58148 2023-05-03 12:36:18.000000 openshift-cluster-management-python-client-1.0.21/openshift_cluster_management_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      557 2023-05-03 12:36:18.000000 openshift-cluster-management-python-client-1.0.21/openshift_cluster_management_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 12:36:18.000000 openshift-cluster-management-python-client-1.0.21/openshift_cluster_management_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-05-03 12:36:18.000000 openshift-cluster-management-python-client-1.0.21/openshift_cluster_management_python_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-03 12:36:18.000000 openshift-cluster-management-python-client-1.0.21/openshift_cluster_management_python_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 12:36:18.034265 openshift-cluster-management-python-client-1.0.21/setup.cfg
```

### Comparing `openshift-cluster-management-python-client-1.0.14/LICENSE` & `openshift-cluster-management-python-client-1.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.14/pyproject.toml` & `openshift-cluster-management-python-client-1.0.21/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -23,42 +23,37 @@
 
 [project]
 name = "openshift-cluster-management-python-client"
 authors = [
     {name = "Meni Yakove", email = "myakove@gmail.com"},
     {name = "Ruth Netser", email = "rnetser@gmail.com"}
 ]
-description = "Wrapper around https://github.com/openshift/openshift-cluster-management-python-client"
+description = "A python client for https://api.openshift.com/api/ APIs"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.8"
 keywords = ["Openshift", "OCM"]
 dependencies = [
-    "colorlog",
-    "ocm-python-client",
-    "openshift-python-wrapper",
-    "requests",
-    "pyyaml",
-    "openshift-python-utilities",
+    "urllib3 >= 1.25.3",
+    "python-dateutil",
 ]
 dynamic = ["version"]
 # ...
 [tool.setuptools.dynamic]
 version = {file = "VERSION"}
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://github.com/RedHatQE/openshift-cluster-management-python-client"
 Download = "https://pypi.org/project/openshift-cluster-management-python-client/"
-"Bug Tracker" = "https://github.com/RedHatQE/oopenshift-cluster-management-python-client/issues"
-Documentation = "https://github.com/rnetser/openshift-cluster-management-python-wrapper/blob/main/README.md"
+Documentation = "https://github.com/RedHatQE/openshift-cluster-management-python-client/blob/main/README.md"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
-include = ["ocm_python_wrapper"]
+include = ["ocm_python_client"]
```

