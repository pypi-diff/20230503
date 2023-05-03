# Comparing `tmp/cdk-eks-blueprint-0.0.7.tar.gz` & `tmp/cdk-eks-blueprint-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-eks-blueprint-0.0.7.tar", last modified: Tue May  2 01:41:41 2023, max compression
+gzip compressed data, was "cdk-eks-blueprint-0.0.8.tar", last modified: Wed May  3 14:51:53 2023, max compression
```

## Comparing `cdk-eks-blueprint-0.0.7.tar` & `cdk-eks-blueprint-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:41:41.810035 cdk-eks-blueprint-0.0.7/
--rw-r--r--   0 yuriliang  (1000) users      (100)      135 2023-05-02 01:41:41.810035 cdk-eks-blueprint-0.0.7/PKG-INFO
--rw-r--r--   0 yuriliang  (1000) users      (100)       14 2023-04-29 11:18:46.000000 cdk-eks-blueprint-0.0.7/README.md
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:41:41.806037 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/
--rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-05-02 01:38:40.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/__init__.py
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:41:41.810035 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/addons/
--rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-04-30 10:36:01.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/addons/__init__.py
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:41:41.810035 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/
--rw-r--r--   0 yuriliang  (1000) users      (100)       22 2023-05-02 01:38:52.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/__init__.py
--rw-r--r--   0 yuriliang  (1000) users      (100)      625 2023-04-25 10:05:59.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/_params_validation.py
--rw-r--r--   0 yuriliang  (1000) users      (100)     5933 2023-05-02 01:39:23.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/controller_plane.py
--rw-r--r--   0 yuriliang  (1000) users      (100)     5633 2023-05-02 01:39:57.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/eks_cluster.py
--rw-r--r--   0 yuriliang  (1000) users      (100)     3171 2023-05-02 01:40:03.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/managed_node_group.py
--rw-r--r--   0 yuriliang  (1000) users      (100)     2952 2023-05-02 01:40:09.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/self_manage_node_group.py
-drwxr-xr-x   0 yuriliang  (1000) users      (100)        0 2023-05-02 01:41:41.810035 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/
--rw-r--r--   0 yuriliang  (1000) users      (100)      135 2023-05-02 01:41:41.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/PKG-INFO
--rw-r--r--   0 yuriliang  (1000) users      (100)      562 2023-05-02 01:41:41.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/SOURCES.txt
--rw-r--r--   0 yuriliang  (1000) users      (100)        1 2023-05-02 01:41:41.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/dependency_links.txt
--rw-r--r--   0 yuriliang  (1000) users      (100)       93 2023-05-02 01:41:41.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/requires.txt
--rw-r--r--   0 yuriliang  (1000) users      (100)       18 2023-05-02 01:41:41.000000 cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/top_level.txt
--rw-r--r--   0 yuriliang  (1000) users      (100)       38 2023-05-02 01:41:41.810035 cdk-eks-blueprint-0.0.7/setup.cfg
--r--r--r--   0 yuriliang  (1000) users      (100)      504 2023-05-02 01:41:37.000000 cdk-eks-blueprint-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:51:53.074474 cdk-eks-blueprint-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 14:51:53.074474 cdk-eks-blueprint-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-03 14:51:14.000000 cdk-eks-blueprint-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:51:53.074474 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 14:51:14.000000 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:51:53.074474 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/addons/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 14:51:14.000000 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/addons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:51:53.074474 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:51:14.000000 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-03 14:51:14.000000 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/cluster/_params_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-05-03 14:51:14.000000 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/cluster/controller_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-03 14:51:14.000000 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/cluster/eks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-03 14:51:14.000000 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/cluster/managed_node_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-03 14:51:14.000000 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/cluster/self_manage_node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:51:53.074474 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 14:51:53.000000 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-03 14:51:53.000000 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:51:53.000000 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-03 14:51:53.000000 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 14:51:53.000000 cdk-eks-blueprint-0.0.8/cdk_eks_blueprint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:51:53.074474 cdk-eks-blueprint-0.0.8/setup.cfg
+-r--r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 14:51:20.000000 cdk-eks-blueprint-0.0.8/setup.py
```

### Comparing `cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/_params_validation.py` & `cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/cluster/_params_validation.py`

 * *Files identical despite different names*

### Comparing `cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/controller_plane.py` & `cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/cluster/controller_plane.py`

 * *Files identical despite different names*

### Comparing `cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/eks_cluster.py` & `cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/cluster/eks_cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pyright: reportUndefinedVariable=false, reportGeneralTypeIssues=false
 from typing import List
 from aws_cdk import aws_eks as eks
 from constructs import Construct
 from .controller_plane import ControllerPlane
 from .managed_node_group import EKSManagedNodeGroup
 from .self_manage_node_group import SelfManagedNodeGroup
 
@@ -11,15 +10,15 @@
     def __init__(
         self,
         scope: Construct,
         id: str,
         *,
         controller_plane: ControllerPlane,
         eks_managed_node_groups: List[EKSManagedNodeGroup] = [],
-        self_managed_node_group: List[SelfManagedNodeGroup] = [],
+        self_managed_node_groups: List[SelfManagedNodeGroup] = [],
         **kwargs,
     ):
         super().__init__(scope, id, **kwargs)
         cluster = eks.Cluster(
             self,
             f"{controller_plane.cluster_name}",
             cluster_name=controller_plane.cluster_name,
@@ -80,16 +79,15 @@
                 notifications=node_group.notifications,
                 signals=node_group.signals,
                 spot_price=node_group.spot_price,
                 termination_policies=node_group.termination_policies,
                 update_policy=node_group.update_policy,
                 vpc_subnets=node_group.vpc_subnets,
             )
-        # Create a launch Template first
-        for node_group in self_managed_node_group:
+        for node_group in self_managed_node_groups:
             cluster.add_nodegroup_capacity(
                 f"SELFEKSASG{node_group.nodegroup_name}",
                 nodegroup_name=node_group.nodegroup_name,
                 ami_type=node_group.ami_type,
                 capacity_type=node_group.capacity_type,
                 desired_size=node_group.desired_size,
                 disk_size=node_group.disk_size,
```

### Comparing `cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/managed_node_group.py` & `cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/cluster/managed_node_group.py`

 * *Files identical despite different names*

### Comparing `cdk-eks-blueprint-0.0.7/cdk_eks_blueprint/cluster/self_manage_node_group.py` & `cdk-eks-blueprint-0.0.8/cdk_eks_blueprint/cluster/self_manage_node_group.py`

 * *Files identical despite different names*

### Comparing `cdk-eks-blueprint-0.0.7/cdk_eks_blueprint.egg-info/SOURCES.txt` & `cdk-eks-blueprint-0.0.8/cdk_eks_blueprint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

