# Comparing `tmp/alibabacloud_vpc20160428-2.0.8.tar.gz` & `tmp/alibabacloud_vpc20160428-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_vpc20160428-2.0.8.tar", last modified: Wed Aug 31 13:47:34 2022, max compression
+gzip compressed data, was "dist/alibabacloud_vpc20160428-2.0.9.tar", last modified: Thu Sep  1 08:09:30 2022, max compression
```

## Comparing `alibabacloud_vpc20160428-2.0.8.tar` & `alibabacloud_vpc20160428-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/
--rw-r--r--   0 root         (0) root         (0)      564 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2346 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/alibabacloud_vpc20160428/
--rw-r--r--   0 root         (0) root         (0)       21 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/alibabacloud_vpc20160428/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1557912 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/alibabacloud_vpc20160428/client.py
--rw-r--r--   0 root         (0) root         (0)  2423992 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/alibabacloud_vpc20160428/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/alibabacloud_vpc20160428.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2346 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/alibabacloud_vpc20160428.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/alibabacloud_vpc20160428.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/alibabacloud_vpc20160428.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/alibabacloud_vpc20160428.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/alibabacloud_vpc20160428.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2628 2022-08-31 13:47:34.000000 alibabacloud_vpc20160428-2.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/
+-rw-r--r--   0 root         (0) root         (0)      635 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2346 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1557912 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428/client.py
+-rw-r--r--   0 root         (0) root         (0)  2424267 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2346 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-09-01 08:09:30.000000 alibabacloud_vpc20160428-2.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2628 2022-09-01 08:09:29.000000 alibabacloud_vpc20160428-2.0.9/setup.py
```

### Comparing `alibabacloud_vpc20160428-2.0.8/LICENSE` & `alibabacloud_vpc20160428-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_vpc20160428-2.0.8/PKG-INFO` & `alibabacloud_vpc20160428-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_vpc20160428
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud Virtual Private Cloud (20160428) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_vpc20160428-2.0.8/README-CN.md` & `alibabacloud_vpc20160428-2.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_vpc20160428-2.0.8/README.md` & `alibabacloud_vpc20160428-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_vpc20160428-2.0.8/alibabacloud_vpc20160428/client.py` & `alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_vpc20160428-2.0.8/alibabacloud_vpc20160428/models.py` & `alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -30946,14 +30946,15 @@
         self,
         auto_pay: bool = None,
         business_status: str = None,
         creation_time: str = None,
         deletion_protection: bool = None,
         description: str = None,
         ecs_metric_enabled: bool = None,
+        eip_bind_mode: str = None,
         expired_time: str = None,
         forward_table_ids: DescribeNatGatewaysResponseBodyNatGatewaysNatGatewayForwardTableIds = None,
         full_nat_table_ids: DescribeNatGatewaysResponseBodyNatGatewaysNatGatewayFullNatTableIds = None,
         icmp_reply_enabled: bool = None,
         instance_charge_type: str = None,
         internet_charge_type: str = None,
         ip_lists: DescribeNatGatewaysResponseBodyNatGatewaysNatGatewayIpLists = None,
@@ -30975,14 +30976,15 @@
     ):
         self.auto_pay = auto_pay
         self.business_status = business_status
         self.creation_time = creation_time
         self.deletion_protection = deletion_protection
         self.description = description
         self.ecs_metric_enabled = ecs_metric_enabled
+        self.eip_bind_mode = eip_bind_mode
         self.expired_time = expired_time
         self.forward_table_ids = forward_table_ids
         self.full_nat_table_ids = full_nat_table_ids
         self.icmp_reply_enabled = icmp_reply_enabled
         self.instance_charge_type = instance_charge_type
         self.internet_charge_type = internet_charge_type
         self.ip_lists = ip_lists
@@ -31030,14 +31032,16 @@
             result['CreationTime'] = self.creation_time
         if self.deletion_protection is not None:
             result['DeletionProtection'] = self.deletion_protection
         if self.description is not None:
             result['Description'] = self.description
         if self.ecs_metric_enabled is not None:
             result['EcsMetricEnabled'] = self.ecs_metric_enabled
+        if self.eip_bind_mode is not None:
+            result['EipBindMode'] = self.eip_bind_mode
         if self.expired_time is not None:
             result['ExpiredTime'] = self.expired_time
         if self.forward_table_ids is not None:
             result['ForwardTableIds'] = self.forward_table_ids.to_map()
         if self.full_nat_table_ids is not None:
             result['FullNatTableIds'] = self.full_nat_table_ids.to_map()
         if self.icmp_reply_enabled is not None:
@@ -31090,14 +31094,16 @@
             self.creation_time = m.get('CreationTime')
         if m.get('DeletionProtection') is not None:
             self.deletion_protection = m.get('DeletionProtection')
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('EcsMetricEnabled') is not None:
             self.ecs_metric_enabled = m.get('EcsMetricEnabled')
+        if m.get('EipBindMode') is not None:
+            self.eip_bind_mode = m.get('EipBindMode')
         if m.get('ExpiredTime') is not None:
             self.expired_time = m.get('ExpiredTime')
         if m.get('ForwardTableIds') is not None:
             temp_model = DescribeNatGatewaysResponseBodyNatGatewaysNatGatewayForwardTableIds()
             self.forward_table_ids = temp_model.from_map(m['ForwardTableIds'])
         if m.get('FullNatTableIds') is not None:
             temp_model = DescribeNatGatewaysResponseBodyNatGatewaysNatGatewayFullNatTableIds()
```

### Comparing `alibabacloud_vpc20160428-2.0.8/alibabacloud_vpc20160428.egg-info/PKG-INFO` & `alibabacloud_vpc20160428-2.0.9/alibabacloud_vpc20160428.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-vpc20160428
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud Virtual Private Cloud (20160428) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_vpc20160428-2.0.8/setup.py` & `alibabacloud_vpc20160428-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_vpc20160428.
 
-Created on 31/08/2022
+Created on 01/09/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_vpc20160428"
 NAME = "alibabacloud_vpc20160428" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Virtual Private Cloud (20160428) SDK Library for Python"
```

