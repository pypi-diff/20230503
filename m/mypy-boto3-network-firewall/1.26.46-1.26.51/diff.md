# Comparing `tmp/mypy-boto3-network-firewall-1.26.46.tar.gz` & `tmp/mypy-boto3-network-firewall-1.26.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-network-firewall-1.26.46.tar", last modified: Mon Jan  9 20:27:39 2023, max compression
+gzip compressed data, was "mypy-boto3-network-firewall-1.26.51.tar", last modified: Tue Jan 17 20:24:22 2023, max compression
```

## Comparing `mypy-boto3-network-firewall-1.26.46.tar` & `mypy-boto3-network-firewall-1.26.51.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.380431 mypy-boto3-network-firewall-1.26.46/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-09 20:27:26.000000 mypy-boto3-network-firewall-1.26.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-01-09 20:27:39.380431 mypy-boto3-network-firewall-1.26.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16715 2023-01-09 20:27:26.000000 mypy-boto3-network-firewall-1.26.46/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.372431 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-01-09 20:27:26.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-01-09 20:27:26.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-09 20:27:26.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27559 2023-01-09 20:27:26.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27517 2023-01-09 20:27:26.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-01-09 20:27:27.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10328 2023-01-09 20:27:26.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-01-09 20:27:26.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-01-09 20:27:26.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:26.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39435 2023-01-09 20:27:27.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39387 2023-01-09 20:27:27.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-09 20:27:26.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 20:27:39.380431 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-01-09 20:27:39.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-01-09 20:27:39.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 20:27:39.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-09 20:27:39.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-09 20:27:39.000000 mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 20:27:39.380431 mypy-boto3-network-firewall-1.26.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-01-09 20:27:26.000000 mypy-boto3-network-firewall-1.26.46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:22.383515 mypy-boto3-network-firewall-1.26.51/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18260 2023-01-17 20:24:22.383515 mypy-boto3-network-firewall-1.26.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16738 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:22.383515 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27559 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27517 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39734 2023-01-17 20:24:13.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39684 2023-01-17 20:24:12.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:22.383515 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18260 2023-01-17 20:24:22.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-01-17 20:24:22.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 20:24:22.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 20:24:22.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-17 20:24:22.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-17 20:24:22.000000 mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 20:24:22.383515 mypy-boto3-network-firewall-1.26.51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-01-17 20:24:11.000000 mypy-boto3-network-firewall-1.26.51/setup.py
```

### Comparing `mypy-boto3-network-firewall-1.26.46/LICENSE` & `mypy-boto3-network-firewall-1.26.51/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.26.46/PKG-INFO` & `mypy-boto3-network-firewall-1.26.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-network-firewall
-Version: 1.26.46
-Summary: Type annotations for boto3.NetworkFirewall 1.26.46 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.51
+Summary: Type annotations for boto3.NetworkFirewall 1.26.51 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-network-firewall?color=blue)](https://pypistats.org/packages/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.26.51](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
 
@@ -315,14 +315,15 @@
 ```python
 from mypy_boto3_network_firewall.literals import (
     AttachmentStatusType,
     ConfigurationSyncStateType,
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
+    IPAddressTypeType,
     ListFirewallPoliciesPaginatorName,
     ListFirewallsPaginatorName,
     ListRuleGroupsPaginatorName,
     ListTagsForResourcePaginatorName,
     LogDestinationTypeType,
     LogTypeType,
     OverrideActionType,
```

### Comparing `mypy-boto3-network-firewall-1.26.46/README.md` & `mypy-boto3-network-firewall-1.26.51/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-network-firewall?color=blue)](https://pypistats.org/packages/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.26.51](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,14 +283,15 @@
 ```python
 from mypy_boto3_network_firewall.literals import (
     AttachmentStatusType,
     ConfigurationSyncStateType,
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
+    IPAddressTypeType,
     ListFirewallPoliciesPaginatorName,
     ListFirewallsPaginatorName,
     ListRuleGroupsPaginatorName,
     ListTagsForResourcePaginatorName,
     LogDestinationTypeType,
     LogTypeType,
     OverrideActionType,
```

### Comparing `mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/__init__.py` & `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/__init__.pyi` & `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/__main__.py` & `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.NetworkFirewall 1.26.46\nVersion:         1.26.46\nBuilder"
-        " version: 7.12.2\nDocs:           "
+        "Type annotations for boto3.NetworkFirewall 1.26.51\nVersion:         1.26.51\nBuilder"
+        " version: 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.46")
+    print("1.26.51")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/client.py` & `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/client.pyi` & `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/literals.py` & `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 __all__ = (
     "AttachmentStatusType",
     "ConfigurationSyncStateType",
     "EncryptionTypeType",
     "FirewallStatusValueType",
     "GeneratedRulesTypeType",
+    "IPAddressTypeType",
     "ListFirewallPoliciesPaginatorName",
     "ListFirewallsPaginatorName",
     "ListRuleGroupsPaginatorName",
     "ListTagsForResourcePaginatorName",
     "LogDestinationTypeType",
     "LogTypeType",
     "OverrideActionType",
@@ -53,14 +54,15 @@
 
 
 AttachmentStatusType = Literal["CREATING", "DELETING", "READY", "SCALING"]
 ConfigurationSyncStateType = Literal["CAPACITY_CONSTRAINED", "IN_SYNC", "PENDING"]
 EncryptionTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_KMS"]
 FirewallStatusValueType = Literal["DELETING", "PROVISIONING", "READY"]
 GeneratedRulesTypeType = Literal["ALLOWLIST", "DENYLIST"]
+IPAddressTypeType = Literal["DUALSTACK", "IPV4"]
 ListFirewallPoliciesPaginatorName = Literal["list_firewall_policies"]
 ListFirewallsPaginatorName = Literal["list_firewalls"]
 ListRuleGroupsPaginatorName = Literal["list_rule_groups"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 LogDestinationTypeType = Literal["CloudWatchLogs", "KinesisDataFirehose", "S3"]
 LogTypeType = Literal["ALERT", "FLOW"]
 OverrideActionType = Literal["DROP_TO_ALERT"]
@@ -136,14 +138,15 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
```

### Comparing `mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/literals.pyi` & `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 __all__ = (
     "AttachmentStatusType",
     "ConfigurationSyncStateType",
     "EncryptionTypeType",
     "FirewallStatusValueType",
     "GeneratedRulesTypeType",
+    "IPAddressTypeType",
     "ListFirewallPoliciesPaginatorName",
     "ListFirewallsPaginatorName",
     "ListRuleGroupsPaginatorName",
     "ListTagsForResourcePaginatorName",
     "LogDestinationTypeType",
     "LogTypeType",
     "OverrideActionType",
@@ -51,14 +52,15 @@
 )
 
 AttachmentStatusType = Literal["CREATING", "DELETING", "READY", "SCALING"]
 ConfigurationSyncStateType = Literal["CAPACITY_CONSTRAINED", "IN_SYNC", "PENDING"]
 EncryptionTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_KMS"]
 FirewallStatusValueType = Literal["DELETING", "PROVISIONING", "READY"]
 GeneratedRulesTypeType = Literal["ALLOWLIST", "DENYLIST"]
+IPAddressTypeType = Literal["DUALSTACK", "IPV4"]
 ListFirewallPoliciesPaginatorName = Literal["list_firewall_policies"]
 ListFirewallsPaginatorName = Literal["list_firewalls"]
 ListRuleGroupsPaginatorName = Literal["list_rule_groups"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 LogDestinationTypeType = Literal["CloudWatchLogs", "KinesisDataFirehose", "S3"]
 LogTypeType = Literal["ALERT", "FLOW"]
 OverrideActionType = Literal["DROP_TO_ALERT"]
@@ -134,14 +136,15 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
```

### Comparing `mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/paginator.py` & `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/paginator.pyi` & `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/type_defs.py` & `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from .literals import (
     AttachmentStatusType,
     ConfigurationSyncStateType,
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
+    IPAddressTypeType,
     LogDestinationTypeType,
     LogTypeType,
     PerObjectSyncStatusType,
     ResourceManagedStatusType,
     ResourceManagedTypeType,
     ResourceStatusType,
     RuleGroupTypeType,
@@ -199,20 +200,32 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-SubnetMappingTypeDef = TypedDict(
-    "SubnetMappingTypeDef",
+_RequiredSubnetMappingTypeDef = TypedDict(
+    "_RequiredSubnetMappingTypeDef",
     {
         "SubnetId": str,
     },
 )
+_OptionalSubnetMappingTypeDef = TypedDict(
+    "_OptionalSubnetMappingTypeDef",
+    {
+        "IPAddressType": IPAddressTypeType,
+    },
+    total=False,
+)
+
+
+class SubnetMappingTypeDef(_RequiredSubnetMappingTypeDef, _OptionalSubnetMappingTypeDef):
+    pass
+
 
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "SubnetId": str,
         "EndpointId": str,
         "Status": AttachmentStatusType,
```

### Comparing `mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall/type_defs.pyi` & `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from .literals import (
     AttachmentStatusType,
     ConfigurationSyncStateType,
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
+    IPAddressTypeType,
     LogDestinationTypeType,
     LogTypeType,
     PerObjectSyncStatusType,
     ResourceManagedStatusType,
     ResourceManagedTypeType,
     ResourceStatusType,
     RuleGroupTypeType,
@@ -196,20 +197,30 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-SubnetMappingTypeDef = TypedDict(
-    "SubnetMappingTypeDef",
+_RequiredSubnetMappingTypeDef = TypedDict(
+    "_RequiredSubnetMappingTypeDef",
     {
         "SubnetId": str,
     },
 )
+_OptionalSubnetMappingTypeDef = TypedDict(
+    "_OptionalSubnetMappingTypeDef",
+    {
+        "IPAddressType": IPAddressTypeType,
+    },
+    total=False,
+)
+
+class SubnetMappingTypeDef(_RequiredSubnetMappingTypeDef, _OptionalSubnetMappingTypeDef):
+    pass
 
 AttachmentTypeDef = TypedDict(
     "AttachmentTypeDef",
     {
         "SubnetId": str,
         "EndpointId": str,
         "Status": AttachmentStatusType,
```

### Comparing `mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall.egg-info/PKG-INFO` & `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-network-firewall
-Version: 1.26.46
-Summary: Type annotations for boto3.NetworkFirewall 1.26.46 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.51
+Summary: Type annotations for boto3.NetworkFirewall 1.26.51 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-network-firewall.svg?color=blue)](https://pypi.org/project/mypy-boto3-network-firewall)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-network-firewall?color=blue)](https://pypistats.org/packages/mypy-boto3-network-firewall)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.NetworkFirewall 1.26.46](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
+[boto3.NetworkFirewall 1.26.51](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-network-firewall docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_network_firewall/).
 
 See how it helps to find and fix potential bugs:
 
@@ -315,14 +315,15 @@
 ```python
 from mypy_boto3_network_firewall.literals import (
     AttachmentStatusType,
     ConfigurationSyncStateType,
     EncryptionTypeType,
     FirewallStatusValueType,
     GeneratedRulesTypeType,
+    IPAddressTypeType,
     ListFirewallPoliciesPaginatorName,
     ListFirewallsPaginatorName,
     ListRuleGroupsPaginatorName,
     ListTagsForResourcePaginatorName,
     LogDestinationTypeType,
     LogTypeType,
     OverrideActionType,
```

### Comparing `mypy-boto3-network-firewall-1.26.46/mypy_boto3_network_firewall.egg-info/SOURCES.txt` & `mypy-boto3-network-firewall-1.26.51/mypy_boto3_network_firewall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-network-firewall-1.26.46/setup.py` & `mypy-boto3-network-firewall-1.26.51/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-network-firewall",
-    version="1.26.46",
+    version="1.26.51",
     packages=["mypy_boto3_network_firewall"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.NetworkFirewall 1.26.46 service generated with"
-        " mypy-boto3-builder 7.12.2"
+        "Type annotations for boto3.NetworkFirewall 1.26.51 service generated with"
+        " mypy-boto3-builder 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

