# Comparing `tmp/mypy-boto3-opensearch-1.26.61.tar.gz` & `tmp/mypy-boto3-opensearch-1.26.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opensearch-1.26.61.tar", last modified: Tue Jan 31 20:49:57 2023, max compression
+gzip compressed data, was "mypy-boto3-opensearch-1.26.77.tar", last modified: Wed Feb 22 20:34:22 2023, max compression
```

## Comparing `mypy-boto3-opensearch-1.26.61.tar` & `mypy-boto3-opensearch-1.26.77.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:57.178170 mypy-boto3-opensearch-1.26.61/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-31 20:48:49.000000 mypy-boto3-opensearch-1.26.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19778 2023-01-31 20:49:57.166170 mypy-boto3-opensearch-1.26.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18272 2023-01-31 20:48:49.000000 mypy-boto3-opensearch-1.26.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:57.166170 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-01-31 20:48:49.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-01-31 20:48:49.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-31 20:48:49.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37529 2023-01-31 20:48:50.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37472 2023-01-31 20:48:49.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14025 2023-01-31 20:48:50.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-01-31 20:48:50.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:48:49.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60094 2023-01-31 20:48:52.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60045 2023-01-31 20:48:51.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-31 20:48:49.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:57.166170 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19778 2023-01-31 20:49:56.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-01-31 20:49:56.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:56.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:56.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:56.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-31 20:49:56.000000 mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 20:49:57.178170 mypy-boto3-opensearch-1.26.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-01-31 20:48:49.000000 mypy-boto3-opensearch-1.26.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.534112 mypy-boto3-opensearch-1.26.77/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20285 2023-02-22 20:34:22.534112 mypy-boto3-opensearch-1.26.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18779 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.530112 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39359 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39300 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-02-22 20:34:00.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14518 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64964 2023-02-22 20:34:01.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64907 2023-02-22 20:34:01.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:34:22.534112 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20285 2023-02-22 20:34:22.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-02-22 20:34:22.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:34:22.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-22 20:34:22.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 20:34:22.000000 mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 20:34:22.534112 mypy-boto3-opensearch-1.26.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-22 20:33:59.000000 mypy-boto3-opensearch-1.26.77/setup.py
```

### Comparing `mypy-boto3-opensearch-1.26.61/LICENSE` & `mypy-boto3-opensearch-1.26.77/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.26.61/PKG-INFO` & `mypy-boto3-opensearch-1.26.77/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.26.61
-Summary: Type annotations for boto3.OpenSearchService 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.77
+Summary: Type annotations for boto3.OpenSearchService 1.26.77 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearch?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -276,14 +276,17 @@
 ### Literals
 
 `mypy_boto3_opensearch.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_opensearch.literals import (
+    ActionSeverityType,
+    ActionStatusType,
+    ActionTypeType,
     AutoTuneDesiredStateType,
     AutoTuneStateType,
     AutoTuneTypeType,
     ConnectionModeType,
     DeploymentStatusType,
     DescribePackagesFilterNameType,
     DomainPackageStatusType,
@@ -297,31 +300,33 @@
     OutboundConnectionStatusCodeType,
     OverallChangeStatusType,
     PackageStatusType,
     PackageTypeType,
     PrincipalTypeType,
     ReservedInstancePaymentOptionType,
     RollbackOnDisableType,
+    ScheduleAtType,
     ScheduledAutoTuneActionTypeType,
     ScheduledAutoTuneSeverityTypeType,
+    ScheduledByType,
     TLSSecurityPolicyType,
     TimeUnitType,
     UpgradeStatusType,
     UpgradeStepType,
     VolumeTypeType,
     VpcEndpointErrorCodeType,
     VpcEndpointStatusType,
     OpenSearchServiceServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
-def check_value(value: AutoTuneDesiredStateType) -> bool:
+def check_value(value: ActionSeverityType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
@@ -355,14 +360,15 @@
     ConnectionPropertiesTypeDef,
     DomainEndpointOptionsTypeDef,
     EBSOptionsTypeDef,
     EncryptionAtRestOptionsTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
     SnapshotOptionsTypeDef,
+    SoftwareUpdateOptionsTypeDef,
     VPCOptionsTypeDef,
     OutboundConnectionStatusTypeDef,
     PackageSourceTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteInboundConnectionRequestRequestTypeDef,
     DeleteOutboundConnectionRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
@@ -395,27 +401,31 @@
     InboundConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     InstanceTypeDetailsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
+    ListScheduledActionsRequestRequestTypeDef,
+    ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVersionsRequestRequestTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
+    WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
+    UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
     DomainInformationContainerTypeDef,
     EmptyResponseMetadataTypeDef,
     GetUpgradeStatusResponseTypeDef,
     ListVersionsResponseTypeDef,
     PurchaseReservedInstanceOfferingResponseTypeDef,
@@ -437,14 +447,15 @@
     GetCompatibleVersionsResponseTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     EBSOptionsStatusTypeDef,
     EncryptionAtRestOptionsStatusTypeDef,
     LogPublishingOptionsStatusTypeDef,
     NodeToNodeEncryptionOptionsStatusTypeDef,
     SnapshotOptionsStatusTypeDef,
+    SoftwareUpdateOptionsStatusTypeDef,
     CreateVpcEndpointRequestRequestTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     CreatePackageRequestRequestTypeDef,
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
@@ -456,14 +467,17 @@
     PackageDetailsTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     DryRunProgressStatusTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
     InstanceLimitsTypeDef,
     ListInstanceTypeDetailsResponseTypeDef,
+    ListScheduledActionsResponseTypeDef,
+    UpdateScheduledActionResponseTypeDef,
+    OffPeakWindowTypeDef,
     ReservedInstanceOfferingTypeDef,
     ReservedInstanceTypeDef,
     SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     CreateOutboundConnectionRequestRequestTypeDef,
@@ -482,28 +496,30 @@
     CreatePackageResponseTypeDef,
     DeletePackageResponseTypeDef,
     DescribePackagesResponseTypeDef,
     UpdatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DescribeVpcEndpointsResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
+    OffPeakWindowOptionsTypeDef,
     DescribeReservedInstanceOfferingsResponseTypeDef,
     DescribeReservedInstancesResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AdvancedSecurityOptionsTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    OffPeakWindowOptionsStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DomainConfigTypeDef,
     CreateDomainResponseTypeDef,
```

### Comparing `mypy-boto3-opensearch-1.26.61/README.md` & `mypy-boto3-opensearch-1.26.77/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearch?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -244,14 +244,17 @@
 ### Literals
 
 `mypy_boto3_opensearch.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_opensearch.literals import (
+    ActionSeverityType,
+    ActionStatusType,
+    ActionTypeType,
     AutoTuneDesiredStateType,
     AutoTuneStateType,
     AutoTuneTypeType,
     ConnectionModeType,
     DeploymentStatusType,
     DescribePackagesFilterNameType,
     DomainPackageStatusType,
@@ -265,31 +268,33 @@
     OutboundConnectionStatusCodeType,
     OverallChangeStatusType,
     PackageStatusType,
     PackageTypeType,
     PrincipalTypeType,
     ReservedInstancePaymentOptionType,
     RollbackOnDisableType,
+    ScheduleAtType,
     ScheduledAutoTuneActionTypeType,
     ScheduledAutoTuneSeverityTypeType,
+    ScheduledByType,
     TLSSecurityPolicyType,
     TimeUnitType,
     UpgradeStatusType,
     UpgradeStepType,
     VolumeTypeType,
     VpcEndpointErrorCodeType,
     VpcEndpointStatusType,
     OpenSearchServiceServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
-def check_value(value: AutoTuneDesiredStateType) -> bool:
+def check_value(value: ActionSeverityType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
@@ -323,14 +328,15 @@
     ConnectionPropertiesTypeDef,
     DomainEndpointOptionsTypeDef,
     EBSOptionsTypeDef,
     EncryptionAtRestOptionsTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
     SnapshotOptionsTypeDef,
+    SoftwareUpdateOptionsTypeDef,
     VPCOptionsTypeDef,
     OutboundConnectionStatusTypeDef,
     PackageSourceTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteInboundConnectionRequestRequestTypeDef,
     DeleteOutboundConnectionRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
@@ -363,27 +369,31 @@
     InboundConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     InstanceTypeDetailsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
+    ListScheduledActionsRequestRequestTypeDef,
+    ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVersionsRequestRequestTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
+    WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
+    UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
     DomainInformationContainerTypeDef,
     EmptyResponseMetadataTypeDef,
     GetUpgradeStatusResponseTypeDef,
     ListVersionsResponseTypeDef,
     PurchaseReservedInstanceOfferingResponseTypeDef,
@@ -405,14 +415,15 @@
     GetCompatibleVersionsResponseTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     EBSOptionsStatusTypeDef,
     EncryptionAtRestOptionsStatusTypeDef,
     LogPublishingOptionsStatusTypeDef,
     NodeToNodeEncryptionOptionsStatusTypeDef,
     SnapshotOptionsStatusTypeDef,
+    SoftwareUpdateOptionsStatusTypeDef,
     CreateVpcEndpointRequestRequestTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     CreatePackageRequestRequestTypeDef,
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
@@ -424,14 +435,17 @@
     PackageDetailsTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     DryRunProgressStatusTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
     InstanceLimitsTypeDef,
     ListInstanceTypeDetailsResponseTypeDef,
+    ListScheduledActionsResponseTypeDef,
+    UpdateScheduledActionResponseTypeDef,
+    OffPeakWindowTypeDef,
     ReservedInstanceOfferingTypeDef,
     ReservedInstanceTypeDef,
     SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     CreateOutboundConnectionRequestRequestTypeDef,
@@ -450,28 +464,30 @@
     CreatePackageResponseTypeDef,
     DeletePackageResponseTypeDef,
     DescribePackagesResponseTypeDef,
     UpdatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DescribeVpcEndpointsResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
+    OffPeakWindowOptionsTypeDef,
     DescribeReservedInstanceOfferingsResponseTypeDef,
     DescribeReservedInstancesResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AdvancedSecurityOptionsTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    OffPeakWindowOptionsStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DomainConfigTypeDef,
     CreateDomainResponseTypeDef,
```

### Comparing `mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/__main__.py` & `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchService 1.26.61\nVersion:         1.26.61\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.OpenSearchService 1.26.77\nVersion:         1.26.77\nBuilder"
+        " version: 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.61")
+    print("1.26.77")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/client.py` & `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    ActionTypeType,
     ConnectionModeType,
     DryRunModeType,
     EngineTypeType,
     LogTypeType,
     OpenSearchPartitionInstanceTypeType,
+    ScheduleAtType,
 )
 from .type_defs import (
     AcceptInboundConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
@@ -69,29 +71,33 @@
     GetPackageVersionHistoryResponseTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     GetUpgradeStatusResponseTypeDef,
     ListDomainNamesResponseTypeDef,
     ListDomainsForPackageResponseTypeDef,
     ListInstanceTypeDetailsResponseTypeDef,
     ListPackagesForDomainResponseTypeDef,
+    ListScheduledActionsResponseTypeDef,
     ListTagsResponseTypeDef,
     ListVersionsResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
+    OffPeakWindowOptionsTypeDef,
     PackageSourceTypeDef,
     PurchaseReservedInstanceOfferingResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     SnapshotOptionsTypeDef,
+    SoftwareUpdateOptionsTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     TagTypeDef,
     UpdateDomainConfigResponseTypeDef,
     UpdatePackageResponseTypeDef,
+    UpdateScheduledActionResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     VPCOptionsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -118,14 +124,15 @@
     DisabledOperationException: Type[BotocoreClientError]
     InternalException: Type[BotocoreClientError]
     InvalidPaginationTokenException: Type[BotocoreClientError]
     InvalidTypeException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
+    SlotNotAvailableException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 
 class OpenSearchServiceClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/)
@@ -223,15 +230,17 @@
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedOptions: Mapping[str, str] = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         TagList: Sequence[TagTypeDef] = ...,
-        AutoTuneOptions: AutoTuneOptionsInputTypeDef = ...
+        AutoTuneOptions: AutoTuneOptionsInputTypeDef = ...,
+        OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
+        SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> CreateDomainResponseTypeDef:
         """
         Creates an Amazon OpenSearch Service domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#create_domain)
         """
@@ -574,14 +583,24 @@
         """
         Lists all packages associated with an Amazon OpenSearch Service domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_packages_for_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#list_packages_for_domain)
         """
 
+    def list_scheduled_actions(
+        self, *, DomainName: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListScheduledActionsResponseTypeDef:
+        """
+        Retrieves a list of configuration changes that are scheduled for a domain.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_scheduled_actions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#list_scheduled_actions)
+        """
+
     def list_tags(self, *, ARN: str) -> ListTagsResponseTypeDef:
         """
         Returns all resource tags for an Amazon OpenSearch Service domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#list_tags)
         """
@@ -664,15 +683,15 @@
         an interface VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.revoke_vpc_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#revoke_vpc_endpoint_access)
         """
 
     def start_service_software_update(
-        self, *, DomainName: str
+        self, *, DomainName: str, ScheduleAt: ScheduleAtType = ..., DesiredStartTime: int = ...
     ) -> StartServiceSoftwareUpdateResponseTypeDef:
         """
         Schedules a service software update for an Amazon OpenSearch Service domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.start_service_software_update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#start_service_software_update)
         """
@@ -691,15 +710,17 @@
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
         DryRun: bool = ...,
-        DryRunMode: DryRunModeType = ...
+        DryRunMode: DryRunModeType = ...,
+        OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
+        SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_domain_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#update_domain_config)
@@ -716,14 +737,30 @@
         """
         Updates a package for use with Amazon OpenSearch Service domains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_package)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#update_package)
         """
 
+    def update_scheduled_action(
+        self,
+        *,
+        DomainName: str,
+        ActionID: str,
+        ActionType: ActionTypeType,
+        ScheduleAt: ScheduleAtType,
+        DesiredStartTime: int = ...
+    ) -> UpdateScheduledActionResponseTypeDef:
+        """
+        Reschedules a planned domain configuration change for a later time.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_scheduled_action)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#update_scheduled_action)
+        """
+
     def update_vpc_endpoint(
         self, *, VpcEndpointId: str, VpcOptions: VPCOptionsTypeDef
     ) -> UpdateVpcEndpointResponseTypeDef:
         """
         Modifies an Amazon OpenSearch Service-managed interface VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_vpc_endpoint)
```

### Comparing `mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/client.pyi` & `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,21 @@
 """
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
+    ActionTypeType,
     ConnectionModeType,
     DryRunModeType,
     EngineTypeType,
     LogTypeType,
     OpenSearchPartitionInstanceTypeType,
+    ScheduleAtType,
 )
 from .type_defs import (
     AcceptInboundConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
@@ -69,29 +71,33 @@
     GetPackageVersionHistoryResponseTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     GetUpgradeStatusResponseTypeDef,
     ListDomainNamesResponseTypeDef,
     ListDomainsForPackageResponseTypeDef,
     ListInstanceTypeDetailsResponseTypeDef,
     ListPackagesForDomainResponseTypeDef,
+    ListScheduledActionsResponseTypeDef,
     ListTagsResponseTypeDef,
     ListVersionsResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
+    OffPeakWindowOptionsTypeDef,
     PackageSourceTypeDef,
     PurchaseReservedInstanceOfferingResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     SnapshotOptionsTypeDef,
+    SoftwareUpdateOptionsTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     TagTypeDef,
     UpdateDomainConfigResponseTypeDef,
     UpdatePackageResponseTypeDef,
+    UpdateScheduledActionResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     VPCOptionsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -115,14 +121,15 @@
     DisabledOperationException: Type[BotocoreClientError]
     InternalException: Type[BotocoreClientError]
     InvalidPaginationTokenException: Type[BotocoreClientError]
     InvalidTypeException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
+    SlotNotAvailableException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
 class OpenSearchServiceClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/)
     """
@@ -211,15 +218,17 @@
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedOptions: Mapping[str, str] = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         TagList: Sequence[TagTypeDef] = ...,
-        AutoTuneOptions: AutoTuneOptionsInputTypeDef = ...
+        AutoTuneOptions: AutoTuneOptionsInputTypeDef = ...,
+        OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
+        SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> CreateDomainResponseTypeDef:
         """
         Creates an Amazon OpenSearch Service domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#create_domain)
         """
@@ -530,14 +539,23 @@
     ) -> ListPackagesForDomainResponseTypeDef:
         """
         Lists all packages associated with an Amazon OpenSearch Service domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_packages_for_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#list_packages_for_domain)
         """
+    def list_scheduled_actions(
+        self, *, DomainName: str, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListScheduledActionsResponseTypeDef:
+        """
+        Retrieves a list of configuration changes that are scheduled for a domain.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_scheduled_actions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#list_scheduled_actions)
+        """
     def list_tags(self, *, ARN: str) -> ListTagsResponseTypeDef:
         """
         Returns all resource tags for an Amazon OpenSearch Service domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#list_tags)
         """
@@ -611,15 +629,15 @@
         Revokes access to an Amazon OpenSearch Service domain that was provided through
         an interface VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.revoke_vpc_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#revoke_vpc_endpoint_access)
         """
     def start_service_software_update(
-        self, *, DomainName: str
+        self, *, DomainName: str, ScheduleAt: ScheduleAtType = ..., DesiredStartTime: int = ...
     ) -> StartServiceSoftwareUpdateResponseTypeDef:
         """
         Schedules a service software update for an Amazon OpenSearch Service domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.start_service_software_update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#start_service_software_update)
         """
@@ -637,15 +655,17 @@
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
         DryRun: bool = ...,
-        DryRunMode: DryRunModeType = ...
+        DryRunMode: DryRunModeType = ...,
+        OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
+        SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
         domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_domain_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#update_domain_config)
@@ -660,14 +680,29 @@
     ) -> UpdatePackageResponseTypeDef:
         """
         Updates a package for use with Amazon OpenSearch Service domains.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_package)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#update_package)
         """
+    def update_scheduled_action(
+        self,
+        *,
+        DomainName: str,
+        ActionID: str,
+        ActionType: ActionTypeType,
+        ScheduleAt: ScheduleAtType,
+        DesiredStartTime: int = ...
+    ) -> UpdateScheduledActionResponseTypeDef:
+        """
+        Reschedules a planned domain configuration change for a later time.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_scheduled_action)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/client/#update_scheduled_action)
+        """
     def update_vpc_endpoint(
         self, *, VpcEndpointId: str, VpcOptions: VPCOptionsTypeDef
     ) -> UpdateVpcEndpointResponseTypeDef:
         """
         Modifies an Amazon OpenSearch Service-managed interface VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_vpc_endpoint)
```

### Comparing `mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/literals.py` & `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 Type annotations for opensearch service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_opensearch.literals import AutoTuneDesiredStateType
+    from mypy_boto3_opensearch.literals import ActionSeverityType
 
-    data: AutoTuneDesiredStateType = "DISABLED"
+    data: ActionSeverityType = "HIGH"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
+    "ActionSeverityType",
+    "ActionStatusType",
+    "ActionTypeType",
     "AutoTuneDesiredStateType",
     "AutoTuneStateType",
     "AutoTuneTypeType",
     "ConnectionModeType",
     "DeploymentStatusType",
     "DescribePackagesFilterNameType",
     "DomainPackageStatusType",
@@ -37,30 +39,36 @@
     "OutboundConnectionStatusCodeType",
     "OverallChangeStatusType",
     "PackageStatusType",
     "PackageTypeType",
     "PrincipalTypeType",
     "ReservedInstancePaymentOptionType",
     "RollbackOnDisableType",
+    "ScheduleAtType",
     "ScheduledAutoTuneActionTypeType",
     "ScheduledAutoTuneSeverityTypeType",
+    "ScheduledByType",
     "TLSSecurityPolicyType",
     "TimeUnitType",
     "UpgradeStatusType",
     "UpgradeStepType",
     "VolumeTypeType",
     "VpcEndpointErrorCodeType",
     "VpcEndpointStatusType",
     "OpenSearchServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
+ActionSeverityType = Literal["HIGH", "LOW", "MEDIUM"]
+ActionStatusType = Literal[
+    "COMPLETED", "ELIGIBLE", "FAILED", "IN_PROGRESS", "NOT_ELIGIBLE", "PENDING_UPDATE"
+]
+ActionTypeType = Literal["JVM_HEAP_SIZE_TUNING", "JVM_YOUNG_GEN_TUNING", "SERVICE_SOFTWARE_UPDATE"]
 AutoTuneDesiredStateType = Literal["DISABLED", "ENABLED"]
 AutoTuneStateType = Literal[
     "DISABLED",
     "DISABLED_AND_ROLLBACK_COMPLETE",
     "DISABLED_AND_ROLLBACK_ERROR",
     "DISABLED_AND_ROLLBACK_IN_PROGRESS",
     "DISABLED_AND_ROLLBACK_SCHEDULED",
@@ -215,16 +223,18 @@
     "VALIDATING",
     "VALIDATION_FAILED",
 ]
 PackageTypeType = Literal["TXT-DICTIONARY"]
 PrincipalTypeType = Literal["AWS_ACCOUNT", "AWS_SERVICE"]
 ReservedInstancePaymentOptionType = Literal["ALL_UPFRONT", "NO_UPFRONT", "PARTIAL_UPFRONT"]
 RollbackOnDisableType = Literal["DEFAULT_ROLLBACK", "NO_ROLLBACK"]
+ScheduleAtType = Literal["NOW", "OFF_PEAK_WINDOW", "TIMESTAMP"]
 ScheduledAutoTuneActionTypeType = Literal["JVM_HEAP_SIZE_TUNING", "JVM_YOUNG_GEN_TUNING"]
 ScheduledAutoTuneSeverityTypeType = Literal["HIGH", "LOW", "MEDIUM"]
+ScheduledByType = Literal["CUSTOMER", "SYSTEM"]
 TLSSecurityPolicyType = Literal["Policy-Min-TLS-1-0-2019-07", "Policy-Min-TLS-1-2-2019-07"]
 TimeUnitType = Literal["HOURS"]
 UpgradeStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED", "SUCCEEDED_WITH_ISSUES"]
 UpgradeStepType = Literal["PRE_UPGRADE_CHECK", "SNAPSHOT", "UPGRADE"]
 VolumeTypeType = Literal["gp2", "gp3", "io1", "standard"]
 VpcEndpointErrorCodeType = Literal["ENDPOINT_NOT_FOUND", "SERVER_ERROR"]
 VpcEndpointStatusType = Literal[
@@ -551,14 +561,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/literals.pyi` & `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 Type annotations for opensearch service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_opensearch.literals import AutoTuneDesiredStateType
+    from mypy_boto3_opensearch.literals import ActionSeverityType
 
-    data: AutoTuneDesiredStateType = "DISABLED"
+    data: ActionSeverityType = "HIGH"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
+    "ActionSeverityType",
+    "ActionStatusType",
+    "ActionTypeType",
     "AutoTuneDesiredStateType",
     "AutoTuneStateType",
     "AutoTuneTypeType",
     "ConnectionModeType",
     "DeploymentStatusType",
     "DescribePackagesFilterNameType",
     "DomainPackageStatusType",
@@ -36,29 +40,37 @@
     "OutboundConnectionStatusCodeType",
     "OverallChangeStatusType",
     "PackageStatusType",
     "PackageTypeType",
     "PrincipalTypeType",
     "ReservedInstancePaymentOptionType",
     "RollbackOnDisableType",
+    "ScheduleAtType",
     "ScheduledAutoTuneActionTypeType",
     "ScheduledAutoTuneSeverityTypeType",
+    "ScheduledByType",
     "TLSSecurityPolicyType",
     "TimeUnitType",
     "UpgradeStatusType",
     "UpgradeStepType",
     "VolumeTypeType",
     "VpcEndpointErrorCodeType",
     "VpcEndpointStatusType",
     "OpenSearchServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
+ActionSeverityType = Literal["HIGH", "LOW", "MEDIUM"]
+ActionStatusType = Literal[
+    "COMPLETED", "ELIGIBLE", "FAILED", "IN_PROGRESS", "NOT_ELIGIBLE", "PENDING_UPDATE"
+]
+ActionTypeType = Literal["JVM_HEAP_SIZE_TUNING", "JVM_YOUNG_GEN_TUNING", "SERVICE_SOFTWARE_UPDATE"]
 AutoTuneDesiredStateType = Literal["DISABLED", "ENABLED"]
 AutoTuneStateType = Literal[
     "DISABLED",
     "DISABLED_AND_ROLLBACK_COMPLETE",
     "DISABLED_AND_ROLLBACK_ERROR",
     "DISABLED_AND_ROLLBACK_IN_PROGRESS",
     "DISABLED_AND_ROLLBACK_SCHEDULED",
@@ -213,16 +225,18 @@
     "VALIDATING",
     "VALIDATION_FAILED",
 ]
 PackageTypeType = Literal["TXT-DICTIONARY"]
 PrincipalTypeType = Literal["AWS_ACCOUNT", "AWS_SERVICE"]
 ReservedInstancePaymentOptionType = Literal["ALL_UPFRONT", "NO_UPFRONT", "PARTIAL_UPFRONT"]
 RollbackOnDisableType = Literal["DEFAULT_ROLLBACK", "NO_ROLLBACK"]
+ScheduleAtType = Literal["NOW", "OFF_PEAK_WINDOW", "TIMESTAMP"]
 ScheduledAutoTuneActionTypeType = Literal["JVM_HEAP_SIZE_TUNING", "JVM_YOUNG_GEN_TUNING"]
 ScheduledAutoTuneSeverityTypeType = Literal["HIGH", "LOW", "MEDIUM"]
+ScheduledByType = Literal["CUSTOMER", "SYSTEM"]
 TLSSecurityPolicyType = Literal["Policy-Min-TLS-1-0-2019-07", "Policy-Min-TLS-1-2-2019-07"]
 TimeUnitType = Literal["HOURS"]
 UpgradeStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED", "SUCCEEDED_WITH_ISSUES"]
 UpgradeStepType = Literal["PRE_UPGRADE_CHECK", "SNAPSHOT", "UPGRADE"]
 VolumeTypeType = Literal["gp2", "gp3", "io1", "standard"]
 VpcEndpointErrorCodeType = Literal["ENDPOINT_NOT_FOUND", "SERVER_ERROR"]
 VpcEndpointStatusType = Literal[
@@ -549,14 +563,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/type_defs.py` & `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,17 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    ActionSeverityType,
+    ActionStatusType,
+    ActionTypeType,
     AutoTuneDesiredStateType,
     AutoTuneStateType,
     ConnectionModeType,
     DeploymentStatusType,
     DescribePackagesFilterNameType,
     DomainPackageStatusType,
     DryRunModeType,
@@ -31,16 +34,18 @@
     OptionStateType,
     OutboundConnectionStatusCodeType,
     OverallChangeStatusType,
     PackageStatusType,
     PrincipalTypeType,
     ReservedInstancePaymentOptionType,
     RollbackOnDisableType,
+    ScheduleAtType,
     ScheduledAutoTuneActionTypeType,
     ScheduledAutoTuneSeverityTypeType,
+    ScheduledByType,
     TLSSecurityPolicyType,
     UpgradeStatusType,
     UpgradeStepType,
     VolumeTypeType,
     VpcEndpointErrorCodeType,
     VpcEndpointStatusType,
 )
@@ -81,14 +86,15 @@
     "ConnectionPropertiesTypeDef",
     "DomainEndpointOptionsTypeDef",
     "EBSOptionsTypeDef",
     "EncryptionAtRestOptionsTypeDef",
     "LogPublishingOptionTypeDef",
     "NodeToNodeEncryptionOptionsTypeDef",
     "SnapshotOptionsTypeDef",
+    "SoftwareUpdateOptionsTypeDef",
     "VPCOptionsTypeDef",
     "OutboundConnectionStatusTypeDef",
     "PackageSourceTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteInboundConnectionRequestRequestTypeDef",
     "DeleteOutboundConnectionRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
@@ -121,27 +127,31 @@
     "InboundConnectionStatusTypeDef",
     "InstanceCountLimitsTypeDef",
     "InstanceTypeDetailsTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
     "ListInstanceTypeDetailsRequestRequestTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
+    "ListScheduledActionsRequestRequestTypeDef",
+    "ScheduledActionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListVersionsRequestRequestTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
+    "WindowStartTimeTypeDef",
     "PurchaseReservedInstanceOfferingRequestRequestTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     "SAMLIdpTypeDef",
     "StartServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
+    "UpdateScheduledActionRequestRequestTypeDef",
     "UpgradeDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
     "DomainInformationContainerTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetUpgradeStatusResponseTypeDef",
     "ListVersionsResponseTypeDef",
     "PurchaseReservedInstanceOfferingResponseTypeDef",
@@ -163,14 +173,15 @@
     "GetCompatibleVersionsResponseTypeDef",
     "DomainEndpointOptionsStatusTypeDef",
     "EBSOptionsStatusTypeDef",
     "EncryptionAtRestOptionsStatusTypeDef",
     "LogPublishingOptionsStatusTypeDef",
     "NodeToNodeEncryptionOptionsStatusTypeDef",
     "SnapshotOptionsStatusTypeDef",
+    "SoftwareUpdateOptionsStatusTypeDef",
     "CreateVpcEndpointRequestRequestTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "ListVpcEndpointsForDomainResponseTypeDef",
     "ListVpcEndpointsResponseTypeDef",
@@ -182,14 +193,17 @@
     "PackageDetailsTypeDef",
     "VPCDerivedInfoStatusTypeDef",
     "VpcEndpointTypeDef",
     "DryRunProgressStatusTypeDef",
     "GetPackageVersionHistoryResponseTypeDef",
     "InstanceLimitsTypeDef",
     "ListInstanceTypeDetailsResponseTypeDef",
+    "ListScheduledActionsResponseTypeDef",
+    "UpdateScheduledActionResponseTypeDef",
+    "OffPeakWindowTypeDef",
     "ReservedInstanceOfferingTypeDef",
     "ReservedInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "CreateOutboundConnectionRequestRequestTypeDef",
@@ -208,28 +222,30 @@
     "CreatePackageResponseTypeDef",
     "DeletePackageResponseTypeDef",
     "DescribePackagesResponseTypeDef",
     "UpdatePackageResponseTypeDef",
     "CreateVpcEndpointResponseTypeDef",
     "DescribeVpcEndpointsResponseTypeDef",
     "UpdateVpcEndpointResponseTypeDef",
+    "OffPeakWindowOptionsTypeDef",
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     "DescribeReservedInstancesResponseTypeDef",
     "AdvancedSecurityOptionsInputTypeDef",
     "AdvancedSecurityOptionsTypeDef",
     "LimitsTypeDef",
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
+    "OffPeakWindowOptionsStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "DomainStatusTypeDef",
     "DescribeInstanceTypeLimitsResponseTypeDef",
     "DomainConfigTypeDef",
     "CreateDomainResponseTypeDef",
@@ -376,14 +392,15 @@
 )
 
 AutoTuneOptionsOutputTypeDef = TypedDict(
     "AutoTuneOptionsOutputTypeDef",
     {
         "State": AutoTuneStateType,
         "ErrorMessage": str,
+        "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
 _RequiredAutoTuneStatusTypeDef = TypedDict(
     "_RequiredAutoTuneStatusTypeDef",
     {
@@ -546,14 +563,22 @@
     "SnapshotOptionsTypeDef",
     {
         "AutomatedSnapshotStartHour": int,
     },
     total=False,
 )
 
+SoftwareUpdateOptionsTypeDef = TypedDict(
+    "SoftwareUpdateOptionsTypeDef",
+    {
+        "AutoSoftwareUpdateEnabled": bool,
+    },
+    total=False,
+)
+
 VPCOptionsTypeDef = TypedDict(
     "VPCOptionsTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
@@ -1021,14 +1046,63 @@
 class ListPackagesForDomainRequestRequestTypeDef(
     _RequiredListPackagesForDomainRequestRequestTypeDef,
     _OptionalListPackagesForDomainRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListScheduledActionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListScheduledActionsRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListScheduledActionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListScheduledActionsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListScheduledActionsRequestRequestTypeDef(
+    _RequiredListScheduledActionsRequestRequestTypeDef,
+    _OptionalListScheduledActionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredScheduledActionTypeDef = TypedDict(
+    "_RequiredScheduledActionTypeDef",
+    {
+        "Id": str,
+        "Type": ActionTypeType,
+        "Severity": ActionSeverityType,
+        "ScheduledTime": int,
+    },
+)
+_OptionalScheduledActionTypeDef = TypedDict(
+    "_OptionalScheduledActionTypeDef",
+    {
+        "Description": str,
+        "ScheduledBy": ScheduledByType,
+        "Status": ActionStatusType,
+        "Mandatory": bool,
+        "Cancellable": bool,
+    },
+    total=False,
+)
+
+
+class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
+    pass
+
+
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ARN": str,
     },
 )
 
@@ -1089,14 +1163,22 @@
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+WindowStartTimeTypeDef = TypedDict(
+    "WindowStartTimeTypeDef",
+    {
+        "Hours": int,
+        "Minutes": int,
+    },
+)
+
 _RequiredPurchaseReservedInstanceOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedInstanceOfferingRequestRequestTypeDef",
     {
         "ReservedInstanceOfferingId": str,
         "ReservationName": str,
     },
 )
@@ -1152,30 +1234,71 @@
     "SAMLIdpTypeDef",
     {
         "MetadataContent": str,
         "EntityId": str,
     },
 )
 
-StartServiceSoftwareUpdateRequestRequestTypeDef = TypedDict(
-    "StartServiceSoftwareUpdateRequestRequestTypeDef",
+_RequiredStartServiceSoftwareUpdateRequestRequestTypeDef = TypedDict(
+    "_RequiredStartServiceSoftwareUpdateRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
+_OptionalStartServiceSoftwareUpdateRequestRequestTypeDef = TypedDict(
+    "_OptionalStartServiceSoftwareUpdateRequestRequestTypeDef",
+    {
+        "ScheduleAt": ScheduleAtType,
+        "DesiredStartTime": int,
+    },
+    total=False,
+)
+
+
+class StartServiceSoftwareUpdateRequestRequestTypeDef(
+    _RequiredStartServiceSoftwareUpdateRequestRequestTypeDef,
+    _OptionalStartServiceSoftwareUpdateRequestRequestTypeDef,
+):
+    pass
+
 
 StorageTypeLimitTypeDef = TypedDict(
     "StorageTypeLimitTypeDef",
     {
         "LimitName": str,
         "LimitValues": List[str],
     },
     total=False,
 )
 
+_RequiredUpdateScheduledActionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateScheduledActionRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "ActionID": str,
+        "ActionType": ActionTypeType,
+        "ScheduleAt": ScheduleAtType,
+    },
+)
+_OptionalUpdateScheduledActionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateScheduledActionRequestRequestTypeDef",
+    {
+        "DesiredStartTime": int,
+    },
+    total=False,
+)
+
+
+class UpdateScheduledActionRequestRequestTypeDef(
+    _RequiredUpdateScheduledActionRequestRequestTypeDef,
+    _OptionalUpdateScheduledActionRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpgradeDomainRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradeDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "TargetVersion": str,
     },
 )
@@ -1446,14 +1569,23 @@
     "SnapshotOptionsStatusTypeDef",
     {
         "Options": SnapshotOptionsTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
+SoftwareUpdateOptionsStatusTypeDef = TypedDict(
+    "SoftwareUpdateOptionsStatusTypeDef",
+    {
+        "Options": SoftwareUpdateOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateVpcEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcEndpointRequestRequestTypeDef",
     {
         "DomainArn": str,
         "VpcOptions": VPCOptionsTypeDef,
     },
 )
@@ -1690,14 +1822,39 @@
     {
         "InstanceTypeDetails": List[InstanceTypeDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListScheduledActionsResponseTypeDef = TypedDict(
+    "ListScheduledActionsResponseTypeDef",
+    {
+        "ScheduledActions": List[ScheduledActionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateScheduledActionResponseTypeDef = TypedDict(
+    "UpdateScheduledActionResponseTypeDef",
+    {
+        "ScheduledAction": ScheduledActionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OffPeakWindowTypeDef = TypedDict(
+    "OffPeakWindowTypeDef",
+    {
+        "WindowStartTime": WindowStartTimeTypeDef,
+    },
+    total=False,
+)
+
 ReservedInstanceOfferingTypeDef = TypedDict(
     "ReservedInstanceOfferingTypeDef",
     {
         "ReservedInstanceOfferingId": str,
         "InstanceType": OpenSearchPartitionInstanceTypeType,
         "Duration": int,
         "FixedPrice": float,
@@ -1851,24 +2008,26 @@
 )
 
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
+        "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "RollbackOnDisable": RollbackOnDisableType,
         "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
+        "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
@@ -1973,14 +2132,23 @@
     "UpdateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OffPeakWindowOptionsTypeDef = TypedDict(
+    "OffPeakWindowOptionsTypeDef",
+    {
+        "Enabled": bool,
+        "OffPeakWindow": OffPeakWindowTypeDef,
+    },
+    total=False,
+)
+
 DescribeReservedInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstanceOfferings": List[ReservedInstanceOfferingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2102,14 +2270,23 @@
     {
         "Options": AutoTuneOptionsTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
+OffPeakWindowOptionsStatusTypeDef = TypedDict(
+    "OffPeakWindowOptionsStatusTypeDef",
+    {
+        "Options": OffPeakWindowOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateDomainRequestRequestTypeDef = TypedDict(
@@ -2126,14 +2303,16 @@
         "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsTypeDef,
         "AdvancedOptions": Mapping[str, str],
         "LogPublishingOptions": Mapping[LogTypeType, LogPublishingOptionTypeDef],
         "DomainEndpointOptions": DomainEndpointOptionsTypeDef,
         "AdvancedSecurityOptions": AdvancedSecurityOptionsInputTypeDef,
         "TagList": Sequence[TagTypeDef],
         "AutoTuneOptions": AutoTuneOptionsInputTypeDef,
+        "OffPeakWindowOptions": OffPeakWindowOptionsTypeDef,
+        "SoftwareUpdateOptions": SoftwareUpdateOptionsTypeDef,
     },
     total=False,
 )
 
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
@@ -2161,14 +2340,16 @@
         "EncryptionAtRestOptions": EncryptionAtRestOptionsTypeDef,
         "DomainEndpointOptions": DomainEndpointOptionsTypeDef,
         "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsTypeDef,
         "AdvancedSecurityOptions": AdvancedSecurityOptionsInputTypeDef,
         "AutoTuneOptions": AutoTuneOptionsTypeDef,
         "DryRun": bool,
         "DryRunMode": DryRunModeType,
+        "OffPeakWindowOptions": OffPeakWindowOptionsTypeDef,
+        "SoftwareUpdateOptions": SoftwareUpdateOptionsTypeDef,
     },
     total=False,
 )
 
 
 class UpdateDomainConfigRequestRequestTypeDef(
     _RequiredUpdateDomainConfigRequestRequestTypeDef,
@@ -2214,14 +2395,16 @@
         "AdvancedOptions": Dict[str, str],
         "LogPublishingOptions": Dict[LogTypeType, LogPublishingOptionTypeDef],
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
         "DomainEndpointOptions": DomainEndpointOptionsTypeDef,
         "AdvancedSecurityOptions": AdvancedSecurityOptionsTypeDef,
         "AutoTuneOptions": AutoTuneOptionsOutputTypeDef,
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
+        "OffPeakWindowOptions": OffPeakWindowOptionsTypeDef,
+        "SoftwareUpdateOptions": SoftwareUpdateOptionsTypeDef,
     },
     total=False,
 )
 
 
 class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
     pass
@@ -2249,14 +2432,16 @@
         "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsStatusTypeDef,
         "AdvancedOptions": AdvancedOptionsStatusTypeDef,
         "LogPublishingOptions": LogPublishingOptionsStatusTypeDef,
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
         "AdvancedSecurityOptions": AdvancedSecurityOptionsStatusTypeDef,
         "AutoTuneOptions": AutoTuneOptionsStatusTypeDef,
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
+        "OffPeakWindowOptions": OffPeakWindowOptionsStatusTypeDef,
+        "SoftwareUpdateOptions": SoftwareUpdateOptionsStatusTypeDef,
     },
     total=False,
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
```

### Comparing `mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch/type_defs.pyi` & `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,17 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
+    ActionSeverityType,
+    ActionStatusType,
+    ActionTypeType,
     AutoTuneDesiredStateType,
     AutoTuneStateType,
     ConnectionModeType,
     DeploymentStatusType,
     DescribePackagesFilterNameType,
     DomainPackageStatusType,
     DryRunModeType,
@@ -31,16 +34,18 @@
     OptionStateType,
     OutboundConnectionStatusCodeType,
     OverallChangeStatusType,
     PackageStatusType,
     PrincipalTypeType,
     ReservedInstancePaymentOptionType,
     RollbackOnDisableType,
+    ScheduleAtType,
     ScheduledAutoTuneActionTypeType,
     ScheduledAutoTuneSeverityTypeType,
+    ScheduledByType,
     TLSSecurityPolicyType,
     UpgradeStatusType,
     UpgradeStepType,
     VolumeTypeType,
     VpcEndpointErrorCodeType,
     VpcEndpointStatusType,
 )
@@ -80,14 +85,15 @@
     "ConnectionPropertiesTypeDef",
     "DomainEndpointOptionsTypeDef",
     "EBSOptionsTypeDef",
     "EncryptionAtRestOptionsTypeDef",
     "LogPublishingOptionTypeDef",
     "NodeToNodeEncryptionOptionsTypeDef",
     "SnapshotOptionsTypeDef",
+    "SoftwareUpdateOptionsTypeDef",
     "VPCOptionsTypeDef",
     "OutboundConnectionStatusTypeDef",
     "PackageSourceTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteInboundConnectionRequestRequestTypeDef",
     "DeleteOutboundConnectionRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
@@ -120,27 +126,31 @@
     "InboundConnectionStatusTypeDef",
     "InstanceCountLimitsTypeDef",
     "InstanceTypeDetailsTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
     "ListInstanceTypeDetailsRequestRequestTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
+    "ListScheduledActionsRequestRequestTypeDef",
+    "ScheduledActionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListVersionsRequestRequestTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
+    "WindowStartTimeTypeDef",
     "PurchaseReservedInstanceOfferingRequestRequestTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     "SAMLIdpTypeDef",
     "StartServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
+    "UpdateScheduledActionRequestRequestTypeDef",
     "UpgradeDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
     "DomainInformationContainerTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetUpgradeStatusResponseTypeDef",
     "ListVersionsResponseTypeDef",
     "PurchaseReservedInstanceOfferingResponseTypeDef",
@@ -162,14 +172,15 @@
     "GetCompatibleVersionsResponseTypeDef",
     "DomainEndpointOptionsStatusTypeDef",
     "EBSOptionsStatusTypeDef",
     "EncryptionAtRestOptionsStatusTypeDef",
     "LogPublishingOptionsStatusTypeDef",
     "NodeToNodeEncryptionOptionsStatusTypeDef",
     "SnapshotOptionsStatusTypeDef",
+    "SoftwareUpdateOptionsStatusTypeDef",
     "CreateVpcEndpointRequestRequestTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "ListVpcEndpointsForDomainResponseTypeDef",
     "ListVpcEndpointsResponseTypeDef",
@@ -181,14 +192,17 @@
     "PackageDetailsTypeDef",
     "VPCDerivedInfoStatusTypeDef",
     "VpcEndpointTypeDef",
     "DryRunProgressStatusTypeDef",
     "GetPackageVersionHistoryResponseTypeDef",
     "InstanceLimitsTypeDef",
     "ListInstanceTypeDetailsResponseTypeDef",
+    "ListScheduledActionsResponseTypeDef",
+    "UpdateScheduledActionResponseTypeDef",
+    "OffPeakWindowTypeDef",
     "ReservedInstanceOfferingTypeDef",
     "ReservedInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "CreateOutboundConnectionRequestRequestTypeDef",
@@ -207,28 +221,30 @@
     "CreatePackageResponseTypeDef",
     "DeletePackageResponseTypeDef",
     "DescribePackagesResponseTypeDef",
     "UpdatePackageResponseTypeDef",
     "CreateVpcEndpointResponseTypeDef",
     "DescribeVpcEndpointsResponseTypeDef",
     "UpdateVpcEndpointResponseTypeDef",
+    "OffPeakWindowOptionsTypeDef",
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     "DescribeReservedInstancesResponseTypeDef",
     "AdvancedSecurityOptionsInputTypeDef",
     "AdvancedSecurityOptionsTypeDef",
     "LimitsTypeDef",
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
+    "OffPeakWindowOptionsStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "DomainStatusTypeDef",
     "DescribeInstanceTypeLimitsResponseTypeDef",
     "DomainConfigTypeDef",
     "CreateDomainResponseTypeDef",
@@ -371,14 +387,15 @@
 )
 
 AutoTuneOptionsOutputTypeDef = TypedDict(
     "AutoTuneOptionsOutputTypeDef",
     {
         "State": AutoTuneStateType,
         "ErrorMessage": str,
+        "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
 _RequiredAutoTuneStatusTypeDef = TypedDict(
     "_RequiredAutoTuneStatusTypeDef",
     {
@@ -539,14 +556,22 @@
     "SnapshotOptionsTypeDef",
     {
         "AutomatedSnapshotStartHour": int,
     },
     total=False,
 )
 
+SoftwareUpdateOptionsTypeDef = TypedDict(
+    "SoftwareUpdateOptionsTypeDef",
+    {
+        "AutoSoftwareUpdateEnabled": bool,
+    },
+    total=False,
+)
+
 VPCOptionsTypeDef = TypedDict(
     "VPCOptionsTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
@@ -996,14 +1021,59 @@
 
 class ListPackagesForDomainRequestRequestTypeDef(
     _RequiredListPackagesForDomainRequestRequestTypeDef,
     _OptionalListPackagesForDomainRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListScheduledActionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListScheduledActionsRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalListScheduledActionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListScheduledActionsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListScheduledActionsRequestRequestTypeDef(
+    _RequiredListScheduledActionsRequestRequestTypeDef,
+    _OptionalListScheduledActionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredScheduledActionTypeDef = TypedDict(
+    "_RequiredScheduledActionTypeDef",
+    {
+        "Id": str,
+        "Type": ActionTypeType,
+        "Severity": ActionSeverityType,
+        "ScheduledTime": int,
+    },
+)
+_OptionalScheduledActionTypeDef = TypedDict(
+    "_OptionalScheduledActionTypeDef",
+    {
+        "Description": str,
+        "ScheduledBy": ScheduledByType,
+        "Status": ActionStatusType,
+        "Mandatory": bool,
+        "Cancellable": bool,
+    },
+    total=False,
+)
+
+class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
+    pass
+
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ARN": str,
     },
 )
 
@@ -1060,14 +1130,22 @@
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+WindowStartTimeTypeDef = TypedDict(
+    "WindowStartTimeTypeDef",
+    {
+        "Hours": int,
+        "Minutes": int,
+    },
+)
+
 _RequiredPurchaseReservedInstanceOfferingRequestRequestTypeDef = TypedDict(
     "_RequiredPurchaseReservedInstanceOfferingRequestRequestTypeDef",
     {
         "ReservedInstanceOfferingId": str,
         "ReservationName": str,
     },
 )
@@ -1121,30 +1199,67 @@
     "SAMLIdpTypeDef",
     {
         "MetadataContent": str,
         "EntityId": str,
     },
 )
 
-StartServiceSoftwareUpdateRequestRequestTypeDef = TypedDict(
-    "StartServiceSoftwareUpdateRequestRequestTypeDef",
+_RequiredStartServiceSoftwareUpdateRequestRequestTypeDef = TypedDict(
+    "_RequiredStartServiceSoftwareUpdateRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
+_OptionalStartServiceSoftwareUpdateRequestRequestTypeDef = TypedDict(
+    "_OptionalStartServiceSoftwareUpdateRequestRequestTypeDef",
+    {
+        "ScheduleAt": ScheduleAtType,
+        "DesiredStartTime": int,
+    },
+    total=False,
+)
+
+class StartServiceSoftwareUpdateRequestRequestTypeDef(
+    _RequiredStartServiceSoftwareUpdateRequestRequestTypeDef,
+    _OptionalStartServiceSoftwareUpdateRequestRequestTypeDef,
+):
+    pass
 
 StorageTypeLimitTypeDef = TypedDict(
     "StorageTypeLimitTypeDef",
     {
         "LimitName": str,
         "LimitValues": List[str],
     },
     total=False,
 )
 
+_RequiredUpdateScheduledActionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateScheduledActionRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "ActionID": str,
+        "ActionType": ActionTypeType,
+        "ScheduleAt": ScheduleAtType,
+    },
+)
+_OptionalUpdateScheduledActionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateScheduledActionRequestRequestTypeDef",
+    {
+        "DesiredStartTime": int,
+    },
+    total=False,
+)
+
+class UpdateScheduledActionRequestRequestTypeDef(
+    _RequiredUpdateScheduledActionRequestRequestTypeDef,
+    _OptionalUpdateScheduledActionRequestRequestTypeDef,
+):
+    pass
+
 _RequiredUpgradeDomainRequestRequestTypeDef = TypedDict(
     "_RequiredUpgradeDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "TargetVersion": str,
     },
 )
@@ -1413,14 +1528,23 @@
     "SnapshotOptionsStatusTypeDef",
     {
         "Options": SnapshotOptionsTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
+SoftwareUpdateOptionsStatusTypeDef = TypedDict(
+    "SoftwareUpdateOptionsStatusTypeDef",
+    {
+        "Options": SoftwareUpdateOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateVpcEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcEndpointRequestRequestTypeDef",
     {
         "DomainArn": str,
         "VpcOptions": VPCOptionsTypeDef,
     },
 )
@@ -1649,14 +1773,39 @@
     {
         "InstanceTypeDetails": List[InstanceTypeDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListScheduledActionsResponseTypeDef = TypedDict(
+    "ListScheduledActionsResponseTypeDef",
+    {
+        "ScheduledActions": List[ScheduledActionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateScheduledActionResponseTypeDef = TypedDict(
+    "UpdateScheduledActionResponseTypeDef",
+    {
+        "ScheduledAction": ScheduledActionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OffPeakWindowTypeDef = TypedDict(
+    "OffPeakWindowTypeDef",
+    {
+        "WindowStartTime": WindowStartTimeTypeDef,
+    },
+    total=False,
+)
+
 ReservedInstanceOfferingTypeDef = TypedDict(
     "ReservedInstanceOfferingTypeDef",
     {
         "ReservedInstanceOfferingId": str,
         "InstanceType": OpenSearchPartitionInstanceTypeType,
         "Duration": int,
         "FixedPrice": float,
@@ -1808,24 +1957,26 @@
 )
 
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
+        "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "RollbackOnDisable": RollbackOnDisableType,
         "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
+        "UseOffPeakWindow": bool,
     },
     total=False,
 )
 
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
@@ -1930,14 +2081,23 @@
     "UpdateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OffPeakWindowOptionsTypeDef = TypedDict(
+    "OffPeakWindowOptionsTypeDef",
+    {
+        "Enabled": bool,
+        "OffPeakWindow": OffPeakWindowTypeDef,
+    },
+    total=False,
+)
+
 DescribeReservedInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     {
         "NextToken": str,
         "ReservedInstanceOfferings": List[ReservedInstanceOfferingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2059,14 +2219,23 @@
     {
         "Options": AutoTuneOptionsTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
+OffPeakWindowOptionsStatusTypeDef = TypedDict(
+    "OffPeakWindowOptionsStatusTypeDef",
+    {
+        "Options": OffPeakWindowOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateDomainRequestRequestTypeDef = TypedDict(
@@ -2083,14 +2252,16 @@
         "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsTypeDef,
         "AdvancedOptions": Mapping[str, str],
         "LogPublishingOptions": Mapping[LogTypeType, LogPublishingOptionTypeDef],
         "DomainEndpointOptions": DomainEndpointOptionsTypeDef,
         "AdvancedSecurityOptions": AdvancedSecurityOptionsInputTypeDef,
         "TagList": Sequence[TagTypeDef],
         "AutoTuneOptions": AutoTuneOptionsInputTypeDef,
+        "OffPeakWindowOptions": OffPeakWindowOptionsTypeDef,
+        "SoftwareUpdateOptions": SoftwareUpdateOptionsTypeDef,
     },
     total=False,
 )
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
@@ -2116,14 +2287,16 @@
         "EncryptionAtRestOptions": EncryptionAtRestOptionsTypeDef,
         "DomainEndpointOptions": DomainEndpointOptionsTypeDef,
         "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsTypeDef,
         "AdvancedSecurityOptions": AdvancedSecurityOptionsInputTypeDef,
         "AutoTuneOptions": AutoTuneOptionsTypeDef,
         "DryRun": bool,
         "DryRunMode": DryRunModeType,
+        "OffPeakWindowOptions": OffPeakWindowOptionsTypeDef,
+        "SoftwareUpdateOptions": SoftwareUpdateOptionsTypeDef,
     },
     total=False,
 )
 
 class UpdateDomainConfigRequestRequestTypeDef(
     _RequiredUpdateDomainConfigRequestRequestTypeDef,
     _OptionalUpdateDomainConfigRequestRequestTypeDef,
@@ -2167,14 +2340,16 @@
         "AdvancedOptions": Dict[str, str],
         "LogPublishingOptions": Dict[LogTypeType, LogPublishingOptionTypeDef],
         "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
         "DomainEndpointOptions": DomainEndpointOptionsTypeDef,
         "AdvancedSecurityOptions": AdvancedSecurityOptionsTypeDef,
         "AutoTuneOptions": AutoTuneOptionsOutputTypeDef,
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
+        "OffPeakWindowOptions": OffPeakWindowOptionsTypeDef,
+        "SoftwareUpdateOptions": SoftwareUpdateOptionsTypeDef,
     },
     total=False,
 )
 
 class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
     pass
 
@@ -2200,14 +2375,16 @@
         "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsStatusTypeDef,
         "AdvancedOptions": AdvancedOptionsStatusTypeDef,
         "LogPublishingOptions": LogPublishingOptionsStatusTypeDef,
         "DomainEndpointOptions": DomainEndpointOptionsStatusTypeDef,
         "AdvancedSecurityOptions": AdvancedSecurityOptionsStatusTypeDef,
         "AutoTuneOptions": AutoTuneOptionsStatusTypeDef,
         "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
+        "OffPeakWindowOptions": OffPeakWindowOptionsStatusTypeDef,
+        "SoftwareUpdateOptions": SoftwareUpdateOptionsStatusTypeDef,
     },
     total=False,
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
```

### Comparing `mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch.egg-info/PKG-INFO` & `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.26.61
-Summary: Type annotations for boto3.OpenSearchService 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.77
+Summary: Type annotations for boto3.OpenSearchService 1.26.77 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-opensearch?color=blue)](https://pypistats.org/packages/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.26.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -276,14 +276,17 @@
 ### Literals
 
 `mypy_boto3_opensearch.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_opensearch.literals import (
+    ActionSeverityType,
+    ActionStatusType,
+    ActionTypeType,
     AutoTuneDesiredStateType,
     AutoTuneStateType,
     AutoTuneTypeType,
     ConnectionModeType,
     DeploymentStatusType,
     DescribePackagesFilterNameType,
     DomainPackageStatusType,
@@ -297,31 +300,33 @@
     OutboundConnectionStatusCodeType,
     OverallChangeStatusType,
     PackageStatusType,
     PackageTypeType,
     PrincipalTypeType,
     ReservedInstancePaymentOptionType,
     RollbackOnDisableType,
+    ScheduleAtType,
     ScheduledAutoTuneActionTypeType,
     ScheduledAutoTuneSeverityTypeType,
+    ScheduledByType,
     TLSSecurityPolicyType,
     TimeUnitType,
     UpgradeStatusType,
     UpgradeStepType,
     VolumeTypeType,
     VpcEndpointErrorCodeType,
     VpcEndpointStatusType,
     OpenSearchServiceServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
-def check_value(value: AutoTuneDesiredStateType) -> bool:
+def check_value(value: ActionSeverityType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
@@ -355,14 +360,15 @@
     ConnectionPropertiesTypeDef,
     DomainEndpointOptionsTypeDef,
     EBSOptionsTypeDef,
     EncryptionAtRestOptionsTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
     SnapshotOptionsTypeDef,
+    SoftwareUpdateOptionsTypeDef,
     VPCOptionsTypeDef,
     OutboundConnectionStatusTypeDef,
     PackageSourceTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteInboundConnectionRequestRequestTypeDef,
     DeleteOutboundConnectionRequestRequestTypeDef,
     DeletePackageRequestRequestTypeDef,
@@ -395,27 +401,31 @@
     InboundConnectionStatusTypeDef,
     InstanceCountLimitsTypeDef,
     InstanceTypeDetailsTypeDef,
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
+    ListScheduledActionsRequestRequestTypeDef,
+    ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
     ListVersionsRequestRequestTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
+    WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
+    UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
     DomainInformationContainerTypeDef,
     EmptyResponseMetadataTypeDef,
     GetUpgradeStatusResponseTypeDef,
     ListVersionsResponseTypeDef,
     PurchaseReservedInstanceOfferingResponseTypeDef,
@@ -437,14 +447,15 @@
     GetCompatibleVersionsResponseTypeDef,
     DomainEndpointOptionsStatusTypeDef,
     EBSOptionsStatusTypeDef,
     EncryptionAtRestOptionsStatusTypeDef,
     LogPublishingOptionsStatusTypeDef,
     NodeToNodeEncryptionOptionsStatusTypeDef,
     SnapshotOptionsStatusTypeDef,
+    SoftwareUpdateOptionsStatusTypeDef,
     CreateVpcEndpointRequestRequestTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     CreatePackageRequestRequestTypeDef,
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
@@ -456,14 +467,17 @@
     PackageDetailsTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     DryRunProgressStatusTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
     InstanceLimitsTypeDef,
     ListInstanceTypeDetailsResponseTypeDef,
+    ListScheduledActionsResponseTypeDef,
+    UpdateScheduledActionResponseTypeDef,
+    OffPeakWindowTypeDef,
     ReservedInstanceOfferingTypeDef,
     ReservedInstanceTypeDef,
     SAMLOptionsInputTypeDef,
     SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     CreateOutboundConnectionRequestRequestTypeDef,
@@ -482,28 +496,30 @@
     CreatePackageResponseTypeDef,
     DeletePackageResponseTypeDef,
     DescribePackagesResponseTypeDef,
     UpdatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DescribeVpcEndpointsResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
+    OffPeakWindowOptionsTypeDef,
     DescribeReservedInstanceOfferingsResponseTypeDef,
     DescribeReservedInstancesResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AdvancedSecurityOptionsTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
+    OffPeakWindowOptionsStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
     AdvancedSecurityOptionsStatusTypeDef,
     DomainStatusTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DomainConfigTypeDef,
     CreateDomainResponseTypeDef,
```

### Comparing `mypy-boto3-opensearch-1.26.61/mypy_boto3_opensearch.egg-info/SOURCES.txt` & `mypy-boto3-opensearch-1.26.77/mypy_boto3_opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.26.61/setup.py` & `mypy-boto3-opensearch-1.26.77/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-opensearch",
-    version="1.26.61",
+    version="1.26.77",
     packages=["mypy_boto3_opensearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpenSearchService 1.26.61 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.OpenSearchService 1.26.77 service generated with"
+        " mypy-boto3-builder 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

