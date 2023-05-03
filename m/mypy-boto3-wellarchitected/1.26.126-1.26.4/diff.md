# Comparing `tmp/mypy-boto3-wellarchitected-1.26.126.tar.gz` & `tmp/mypy-boto3-wellarchitected-1.26.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wellarchitected-1.26.126.tar", last modified: Wed May  3 19:33:10 2023, max compression
+gzip compressed data, was "mypy-boto3-wellarchitected-1.26.4.tar", last modified: Mon Nov  7 20:50:37 2022, max compression
```

## Comparing `mypy-boto3-wellarchitected-1.26.126.tar` & `mypy-boto3-wellarchitected-1.26.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:33:10.508074 mypy-boto3-wellarchitected-1.26.126/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-03 19:32:58.000000 mypy-boto3-wellarchitected-1.26.126/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-05-03 19:33:10.508074 mypy-boto3-wellarchitected-1.26.126/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-05-03 19:32:58.000000 mypy-boto3-wellarchitected-1.26.126/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:33:10.500074 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-03 19:32:58.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-03 19:32:58.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-03 19:32:58.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30436 2023-05-03 19:32:58.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30387 2023-05-03 19:32:58.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-03 19:32:58.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-05-03 19:32:58.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:32:58.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42216 2023-05-03 19:32:59.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42169 2023-05-03 19:32:59.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 19:32:58.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:33:10.508074 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16869 2023-05-03 19:33:10.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-03 19:33:10.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:33:10.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:33:10.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 19:33:10.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-03 19:33:10.000000 mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:33:10.508074 mypy-boto3-wellarchitected-1.26.126/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-03 19:32:58.000000 mypy-boto3-wellarchitected-1.26.126/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:37.092346 mypy-boto3-wellarchitected-1.26.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    16502 2022-11-07 20:50:37.092346 mypy-boto3-wellarchitected-1.26.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    15035 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:37.072346 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29412 2022-11-07 20:50:23.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29364 2022-11-07 20:50:23.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     9629 2022-11-07 20:50:23.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/literals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9627 2022-11-07 20:50:23.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    39740 2022-11-07 20:50:24.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39695 2022-11-07 20:50:24.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 20:50:37.092346 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    16502 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      751 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-07 20:50:36.000000 mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 20:50:37.092346 mypy-boto3-wellarchitected-1.26.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-11-07 20:50:22.000000 mypy-boto3-wellarchitected-1.26.4/setup.py
```

### Comparing `mypy-boto3-wellarchitected-1.26.126/LICENSE` & `mypy-boto3-wellarchitected-1.26.4/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-wellarchitected-1.26.126/PKG-INFO` & `mypy-boto3-wellarchitected-1.26.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wellarchitected
-Version: 1.26.126
-Summary: Type annotations for boto3.WellArchitected 1.26.126 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.4
+Summary: Type annotations for boto3.WellArchitected 1.26.4 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wellarchitected?color=blue)](https://pypistats.org/packages/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.26.126](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -284,26 +283,22 @@
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckProviderType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
-    DefinitionTypeType,
     DifferenceStatusType,
-    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
-    MetricTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -327,15 +322,14 @@
 
 ```python
 from mypy_boto3_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
-    BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateLensVersionInputRequestTypeDef,
@@ -345,15 +339,14 @@
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
     ExportLensInputRequestTypeDef,
     GetAnswerInputRequestTypeDef,
-    GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
@@ -387,15 +380,14 @@
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
     AdditionalResourcesTypeDef,
-    QuestionMetricTypeDef,
     ImprovementSummaryTypeDef,
     UpdateAnswerInputRequestTypeDef,
     CreateLensShareOutputTypeDef,
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
@@ -419,76 +411,72 @@
     ListWorkloadSharesOutputTypeDef,
     ListWorkloadsOutputTypeDef,
     MilestoneSummaryTypeDef,
     PillarDifferenceTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     ChoiceTypeDef,
-    PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     GetWorkloadOutputTypeDef,
     MilestoneTypeDef,
     UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
     ListMilestonesOutputTypeDef,
     VersionDifferencesTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
-    LensMetricTypeDef,
     GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
-    ConsolidatedReportMetricTypeDef,
-    GetConsolidatedReportOutputTypeDef,
 )
 
 
 def get_structure() -> ChoiceContentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-wellarchitected-1.26.126/README.md` & `mypy-boto3-wellarchitected-1.26.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wellarchitected?color=blue)](https://pypistats.org/packages/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.26.126](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -252,26 +252,22 @@
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckProviderType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
-    DefinitionTypeType,
     DifferenceStatusType,
-    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
-    MetricTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -295,15 +291,14 @@
 
 ```python
 from mypy_boto3_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
-    BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateLensVersionInputRequestTypeDef,
@@ -313,15 +308,14 @@
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
     ExportLensInputRequestTypeDef,
     GetAnswerInputRequestTypeDef,
-    GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
@@ -355,15 +349,14 @@
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
     AdditionalResourcesTypeDef,
-    QuestionMetricTypeDef,
     ImprovementSummaryTypeDef,
     UpdateAnswerInputRequestTypeDef,
     CreateLensShareOutputTypeDef,
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
@@ -387,76 +380,72 @@
     ListWorkloadSharesOutputTypeDef,
     ListWorkloadsOutputTypeDef,
     MilestoneSummaryTypeDef,
     PillarDifferenceTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     ChoiceTypeDef,
-    PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     GetWorkloadOutputTypeDef,
     MilestoneTypeDef,
     UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
     ListMilestonesOutputTypeDef,
     VersionDifferencesTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
-    LensMetricTypeDef,
     GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
-    ConsolidatedReportMetricTypeDef,
-    GetConsolidatedReportOutputTypeDef,
 )
 
 
 def get_structure() -> ChoiceContentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/__main__.py` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WellArchitected 1.26.126\nVersion:         1.26.126\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.WellArchitected 1.26.4\nVersion:         1.26.4\nBuilder"
+        " version: 7.11.10\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.126")
+    print("1.26.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/client.py` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,18 @@
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AnswerReasonType,
-    DiscoveryIntegrationStatusType,
     LensStatusTypeType,
     LensTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ReportFormatType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
 )
 from .type_defs import (
@@ -37,15 +35,14 @@
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportLensOutputTypeDef,
     GetAnswerOutputTypeDef,
-    GetConsolidatedReportOutputTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetMilestoneOutputTypeDef,
     GetWorkloadOutputTypeDef,
     ImportLensOutputTypeDef,
@@ -291,29 +288,14 @@
         """
         Get the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_answer)
         """
 
-    def get_consolidated_report(
-        self,
-        *,
-        Format: ReportFormatType,
-        IncludeSharedResources: bool = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
-    ) -> GetConsolidatedReportOutputTypeDef:
-        """
-        Get a consolidated report of your workloads.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_consolidated_report)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_consolidated_report)
-        """
-
     def get_lens(self, *, LensAlias: str, LensVersion: str = ...) -> GetLensOutputTypeDef:
         """
         Get an existing lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_lens)
         """
@@ -369,15 +351,15 @@
         *,
         JSONString: str,
         ClientRequestToken: str,
         LensAlias: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> ImportLensOutputTypeDef:
         """
-        Import a new custom lens or update an existing custom lens.
+        Import a new lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.import_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#import_lens)
         """
 
     def list_answers(
         self,
@@ -386,15 +368,15 @@
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListAnswersOutputTypeDef:
         """
-        List of answers for a particular workload and lens.
+        List of answers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_answers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_answers)
         """
 
     def list_check_details(
         self,
@@ -455,15 +437,15 @@
         *,
         WorkloadId: str,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListLensReviewsOutputTypeDef:
         """
-        List lens reviews for a particular workload.
+        List lens reviews.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_reviews)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_reviews)
         """
 
     def list_lens_shares(
         self,
@@ -557,15 +539,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workload_shares)
         """
 
     def list_workloads(
         self, *, WorkloadNamePrefix: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListWorkloadsOutputTypeDef:
         """
-        Paginated list of workloads.
+        List workloads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workloads)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workloads)
         """
 
     def tag_resource(self, *, WorkloadArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
@@ -599,37 +581,34 @@
         Update the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_answer)
         """
 
     def update_global_settings(
-        self,
-        *,
-        OrganizationSharingStatus: OrganizationSharingStatusType = ...,
-        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...
+        self, *, OrganizationSharingStatus: OrganizationSharingStatusType = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates whether the Amazon Web Services account is opted into organization
-        sharing and discovery integration features.
+        sharing features.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_global_settings)
         """
 
     def update_lens_review(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         LensNotes: str = ...,
         PillarNotes: Mapping[str, str] = ...
     ) -> UpdateLensReviewOutputTypeDef:
         """
-        Update lens review for a particular workload.
+        Update lens review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_lens_review)
         """
 
     def update_share_invitation(
         self, *, ShareInvitationId: str, ShareInvitationAction: ShareInvitationActionType
@@ -679,12 +658,12 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_workload_share)
         """
 
     def upgrade_lens_review(
         self, *, WorkloadId: str, LensAlias: str, MilestoneName: str, ClientRequestToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Upgrade lens review for a particular workload.
+        Upgrade lens review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#upgrade_lens_review)
         """
```

### Comparing `mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/client.pyi` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,18 @@
 """
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     AnswerReasonType,
-    DiscoveryIntegrationStatusType,
     LensStatusTypeType,
     LensTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ReportFormatType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
 )
 from .type_defs import (
@@ -37,15 +35,14 @@
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportLensOutputTypeDef,
     GetAnswerOutputTypeDef,
-    GetConsolidatedReportOutputTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetMilestoneOutputTypeDef,
     GetWorkloadOutputTypeDef,
     ImportLensOutputTypeDef,
@@ -271,28 +268,14 @@
     ) -> GetAnswerOutputTypeDef:
         """
         Get the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_answer)
         """
-    def get_consolidated_report(
-        self,
-        *,
-        Format: ReportFormatType,
-        IncludeSharedResources: bool = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
-    ) -> GetConsolidatedReportOutputTypeDef:
-        """
-        Get a consolidated report of your workloads.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_consolidated_report)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_consolidated_report)
-        """
     def get_lens(self, *, LensAlias: str, LensVersion: str = ...) -> GetLensOutputTypeDef:
         """
         Get an existing lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.get_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#get_lens)
         """
@@ -342,15 +325,15 @@
         *,
         JSONString: str,
         ClientRequestToken: str,
         LensAlias: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> ImportLensOutputTypeDef:
         """
-        Import a new custom lens or update an existing custom lens.
+        Import a new lens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.import_lens)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#import_lens)
         """
     def list_answers(
         self,
         *,
@@ -358,15 +341,15 @@
         LensAlias: str,
         PillarId: str = ...,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListAnswersOutputTypeDef:
         """
-        List of answers for a particular workload and lens.
+        List of answers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_answers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_answers)
         """
     def list_check_details(
         self,
         *,
@@ -423,15 +406,15 @@
         *,
         WorkloadId: str,
         MilestoneNumber: int = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListLensReviewsOutputTypeDef:
         """
-        List lens reviews for a particular workload.
+        List lens reviews.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_lens_reviews)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_lens_reviews)
         """
     def list_lens_shares(
         self,
         *,
@@ -517,15 +500,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workload_shares)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workload_shares)
         """
     def list_workloads(
         self, *, WorkloadNamePrefix: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListWorkloadsOutputTypeDef:
         """
-        Paginated list of workloads.
+        List workloads.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.list_workloads)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#list_workloads)
         """
     def tag_resource(self, *, WorkloadArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds one or more tags to the specified resource.
@@ -555,36 +538,33 @@
         """
         Update the answer to a specific question in a workload review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_answer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_answer)
         """
     def update_global_settings(
-        self,
-        *,
-        OrganizationSharingStatus: OrganizationSharingStatusType = ...,
-        DiscoveryIntegrationStatus: DiscoveryIntegrationStatusType = ...
+        self, *, OrganizationSharingStatus: OrganizationSharingStatusType = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates whether the Amazon Web Services account is opted into organization
-        sharing and discovery integration features.
+        sharing features.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_global_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_global_settings)
         """
     def update_lens_review(
         self,
         *,
         WorkloadId: str,
         LensAlias: str,
         LensNotes: str = ...,
         PillarNotes: Mapping[str, str] = ...
     ) -> UpdateLensReviewOutputTypeDef:
         """
-        Update lens review for a particular workload.
+        Update lens review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_lens_review)
         """
     def update_share_invitation(
         self, *, ShareInvitationId: str, ShareInvitationAction: ShareInvitationActionType
     ) -> UpdateShareInvitationOutputTypeDef:
@@ -630,12 +610,12 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#update_workload_share)
         """
     def upgrade_lens_review(
         self, *, WorkloadId: str, LensAlias: str, MilestoneName: str, ClientRequestToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Upgrade lens review for a particular workload.
+        Upgrade lens review.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.upgrade_lens_review)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/client/#upgrade_lens_review)
         """
```

### Comparing `mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/literals.py` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,26 +23,22 @@
     "AdditionalResourceTypeType",
     "AnswerReasonType",
     "CheckFailureReasonType",
     "CheckProviderType",
     "CheckStatusType",
     "ChoiceReasonType",
     "ChoiceStatusType",
-    "DefinitionTypeType",
     "DifferenceStatusType",
-    "DiscoveryIntegrationStatusType",
     "ImportLensStatusType",
     "LensStatusType",
     "LensStatusTypeType",
     "LensTypeType",
-    "MetricTypeType",
     "NotificationTypeType",
     "OrganizationSharingStatusType",
     "PermissionTypeType",
-    "ReportFormatType",
     "RiskType",
     "ShareInvitationActionType",
     "ShareResourceTypeType",
     "ShareStatusType",
     "TrustedAdvisorIntegrationStatusType",
     "WorkloadEnvironmentType",
     "WorkloadImprovementStatusType",
@@ -62,26 +58,22 @@
 ]
 CheckProviderType = Literal["TRUSTED_ADVISOR"]
 CheckStatusType = Literal["ERROR", "FETCH_FAILED", "NOT_AVAILABLE", "OKAY", "WARNING"]
 ChoiceReasonType = Literal[
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 ChoiceStatusType = Literal["NOT_APPLICABLE", "SELECTED", "UNSELECTED"]
-DefinitionTypeType = Literal["APP_REGISTRY", "WORKLOAD_METADATA"]
 DifferenceStatusType = Literal["DELETED", "NEW", "UPDATED"]
-DiscoveryIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 ImportLensStatusType = Literal["COMPLETE", "ERROR", "IN_PROGRESS"]
 LensStatusType = Literal["CURRENT", "DELETED", "DEPRECATED", "NOT_CURRENT", "UNSHARED"]
 LensStatusTypeType = Literal["ALL", "DRAFT", "PUBLISHED"]
 LensTypeType = Literal["AWS_OFFICIAL", "CUSTOM_SELF", "CUSTOM_SHARED"]
-MetricTypeType = Literal["WORKLOAD"]
 NotificationTypeType = Literal["LENS_VERSION_DEPRECATED", "LENS_VERSION_UPGRADED"]
 OrganizationSharingStatusType = Literal["DISABLED", "ENABLED"]
 PermissionTypeType = Literal["CONTRIBUTOR", "READONLY"]
-ReportFormatType = Literal["JSON", "PDF"]
 RiskType = Literal["HIGH", "MEDIUM", "NONE", "NOT_APPLICABLE", "UNANSWERED"]
 ShareInvitationActionType = Literal["ACCEPT", "REJECT"]
 ShareResourceTypeType = Literal["LENS", "WORKLOAD"]
 ShareStatusType = Literal[
     "ACCEPTED", "ASSOCIATED", "ASSOCIATING", "EXPIRED", "FAILED", "PENDING", "REJECTED", "REVOKED"
 ]
 TrustedAdvisorIntegrationStatusType = Literal["DISABLED", "ENABLED"]
@@ -110,15 +102,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -128,31 +119,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -181,15 +168,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -234,57 +220,51 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -316,33 +296,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -351,15 +326,14 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
-    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -370,63 +344,55 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
-    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/literals.pyi` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/literals.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -22,26 +22,22 @@
     "AdditionalResourceTypeType",
     "AnswerReasonType",
     "CheckFailureReasonType",
     "CheckProviderType",
     "CheckStatusType",
     "ChoiceReasonType",
     "ChoiceStatusType",
-    "DefinitionTypeType",
     "DifferenceStatusType",
-    "DiscoveryIntegrationStatusType",
     "ImportLensStatusType",
     "LensStatusType",
     "LensStatusTypeType",
     "LensTypeType",
-    "MetricTypeType",
     "NotificationTypeType",
     "OrganizationSharingStatusType",
     "PermissionTypeType",
-    "ReportFormatType",
     "RiskType",
     "ShareInvitationActionType",
     "ShareResourceTypeType",
     "ShareStatusType",
     "TrustedAdvisorIntegrationStatusType",
     "WorkloadEnvironmentType",
     "WorkloadImprovementStatusType",
@@ -60,26 +56,22 @@
 ]
 CheckProviderType = Literal["TRUSTED_ADVISOR"]
 CheckStatusType = Literal["ERROR", "FETCH_FAILED", "NOT_AVAILABLE", "OKAY", "WARNING"]
 ChoiceReasonType = Literal[
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 ChoiceStatusType = Literal["NOT_APPLICABLE", "SELECTED", "UNSELECTED"]
-DefinitionTypeType = Literal["APP_REGISTRY", "WORKLOAD_METADATA"]
 DifferenceStatusType = Literal["DELETED", "NEW", "UPDATED"]
-DiscoveryIntegrationStatusType = Literal["DISABLED", "ENABLED"]
 ImportLensStatusType = Literal["COMPLETE", "ERROR", "IN_PROGRESS"]
 LensStatusType = Literal["CURRENT", "DELETED", "DEPRECATED", "NOT_CURRENT", "UNSHARED"]
 LensStatusTypeType = Literal["ALL", "DRAFT", "PUBLISHED"]
 LensTypeType = Literal["AWS_OFFICIAL", "CUSTOM_SELF", "CUSTOM_SHARED"]
-MetricTypeType = Literal["WORKLOAD"]
 NotificationTypeType = Literal["LENS_VERSION_DEPRECATED", "LENS_VERSION_UPGRADED"]
 OrganizationSharingStatusType = Literal["DISABLED", "ENABLED"]
 PermissionTypeType = Literal["CONTRIBUTOR", "READONLY"]
-ReportFormatType = Literal["JSON", "PDF"]
 RiskType = Literal["HIGH", "MEDIUM", "NONE", "NOT_APPLICABLE", "UNANSWERED"]
 ShareInvitationActionType = Literal["ACCEPT", "REJECT"]
 ShareResourceTypeType = Literal["LENS", "WORKLOAD"]
 ShareStatusType = Literal[
     "ACCEPTED", "ASSOCIATED", "ASSOCIATING", "EXPIRED", "FAILED", "PENDING", "REJECTED", "REVOKED"
 ]
 TrustedAdvisorIntegrationStatusType = Literal["DISABLED", "ENABLED"]
@@ -108,15 +100,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -126,31 +117,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -179,15 +166,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -232,57 +218,51 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -314,33 +294,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -349,15 +324,14 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
-    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -368,63 +342,55 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
-    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/type_defs.py` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,25 +18,22 @@
 from .literals import (
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
-    DefinitionTypeType,
     DifferenceStatusType,
-    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -53,15 +50,14 @@
 
 
 __all__ = (
     "ChoiceContentTypeDef",
     "ChoiceAnswerSummaryTypeDef",
     "ChoiceAnswerTypeDef",
     "AssociateLensesInputRequestTypeDef",
-    "BestPracticeTypeDef",
     "CheckDetailTypeDef",
     "CheckSummaryTypeDef",
     "ChoiceImprovementPlanTypeDef",
     "ChoiceUpdateTypeDef",
     "CreateLensShareInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateLensVersionInputRequestTypeDef",
@@ -71,15 +67,14 @@
     "DeleteLensInputRequestTypeDef",
     "DeleteLensShareInputRequestTypeDef",
     "DeleteWorkloadInputRequestTypeDef",
     "DeleteWorkloadShareInputRequestTypeDef",
     "DisassociateLensesInputRequestTypeDef",
     "ExportLensInputRequestTypeDef",
     "GetAnswerInputRequestTypeDef",
-    "GetConsolidatedReportInputRequestTypeDef",
     "GetLensInputRequestTypeDef",
     "LensTypeDef",
     "GetLensReviewInputRequestTypeDef",
     "GetLensReviewReportInputRequestTypeDef",
     "LensReviewReportTypeDef",
     "GetLensVersionDifferenceInputRequestTypeDef",
     "GetMilestoneInputRequestTypeDef",
@@ -113,15 +108,14 @@
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
     "AdditionalResourcesTypeDef",
-    "QuestionMetricTypeDef",
     "ImprovementSummaryTypeDef",
     "UpdateAnswerInputRequestTypeDef",
     "CreateLensShareOutputTypeDef",
     "CreateLensVersionOutputTypeDef",
     "CreateMilestoneOutputTypeDef",
     "CreateWorkloadOutputTypeDef",
     "CreateWorkloadShareOutputTypeDef",
@@ -145,34 +139,30 @@
     "ListWorkloadSharesOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
     "MilestoneSummaryTypeDef",
     "PillarDifferenceTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
     "ChoiceTypeDef",
-    "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
     "GetWorkloadOutputTypeDef",
     "MilestoneTypeDef",
     "UpdateWorkloadOutputTypeDef",
     "GetLensReviewOutputTypeDef",
     "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
     "ListMilestonesOutputTypeDef",
     "VersionDifferencesTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
-    "LensMetricTypeDef",
     "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
-    "ConsolidatedReportMetricTypeDef",
-    "GetConsolidatedReportOutputTypeDef",
 )
 
 ChoiceContentTypeDef = TypedDict(
     "ChoiceContentTypeDef",
     {
         "DisplayText": str,
         "Url": str,
@@ -205,23 +195,14 @@
     "AssociateLensesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAliases": Sequence[str],
     },
 )
 
-BestPracticeTypeDef = TypedDict(
-    "BestPracticeTypeDef",
-    {
-        "ChoiceId": str,
-        "ChoiceTitle": str,
-    },
-    total=False,
-)
-
 CheckDetailTypeDef = TypedDict(
     "CheckDetailTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "Provider": Literal["TRUSTED_ADVISOR"],
@@ -338,15 +319,14 @@
     },
 )
 
 WorkloadDiscoveryConfigTypeDef = TypedDict(
     "WorkloadDiscoveryConfigTypeDef",
     {
         "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
-        "WorkloadResourceDefinition": Sequence[DefinitionTypeType],
     },
     total=False,
 )
 
 CreateWorkloadShareInputRequestTypeDef = TypedDict(
     "CreateWorkloadShareInputRequestTypeDef",
     {
@@ -440,38 +420,14 @@
 
 class GetAnswerInputRequestTypeDef(
     _RequiredGetAnswerInputRequestTypeDef, _OptionalGetAnswerInputRequestTypeDef
 ):
     pass
 
 
-_RequiredGetConsolidatedReportInputRequestTypeDef = TypedDict(
-    "_RequiredGetConsolidatedReportInputRequestTypeDef",
-    {
-        "Format": ReportFormatType,
-    },
-)
-_OptionalGetConsolidatedReportInputRequestTypeDef = TypedDict(
-    "_OptionalGetConsolidatedReportInputRequestTypeDef",
-    {
-        "IncludeSharedResources": bool,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class GetConsolidatedReportInputRequestTypeDef(
-    _RequiredGetConsolidatedReportInputRequestTypeDef,
-    _OptionalGetConsolidatedReportInputRequestTypeDef,
-):
-    pass
-
-
 _RequiredGetLensInputRequestTypeDef = TypedDict(
     "_RequiredGetLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalGetLensInputRequestTypeDef = TypedDict(
@@ -1012,15 +968,14 @@
     },
 )
 
 UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsInputRequestTypeDef",
     {
         "OrganizationSharingStatus": OrganizationSharingStatusType,
-        "DiscoveryIntegrationStatus": DiscoveryIntegrationStatusType,
     },
     total=False,
 )
 
 _RequiredUpdateLensReviewInputRequestTypeDef = TypedDict(
     "_RequiredUpdateLensReviewInputRequestTypeDef",
     {
@@ -1103,24 +1058,14 @@
     {
         "Type": AdditionalResourceTypeType,
         "Content": List[ChoiceContentTypeDef],
     },
     total=False,
 )
 
-QuestionMetricTypeDef = TypedDict(
-    "QuestionMetricTypeDef",
-    {
-        "QuestionId": str,
-        "Risk": RiskType,
-        "BestPractices": List[BestPracticeTypeDef],
-    },
-    total=False,
-)
-
 ImprovementSummaryTypeDef = TypedDict(
     "ImprovementSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Risk": RiskType,
@@ -1504,24 +1449,14 @@
         "HelpfulResource": ChoiceContentTypeDef,
         "ImprovementPlan": ChoiceContentTypeDef,
         "AdditionalResources": List[AdditionalResourcesTypeDef],
     },
     total=False,
 )
 
-PillarMetricTypeDef = TypedDict(
-    "PillarMetricTypeDef",
-    {
-        "PillarId": str,
-        "RiskCounts": Dict[RiskType, int],
-        "Questions": List[QuestionMetricTypeDef],
-    },
-    total=False,
-)
-
 ListLensReviewImprovementsOutputTypeDef = TypedDict(
     "ListLensReviewImprovementsOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
@@ -1637,24 +1572,14 @@
         "Risk": RiskType,
         "Notes": str,
         "Reason": AnswerReasonType,
     },
     total=False,
 )
 
-LensMetricTypeDef = TypedDict(
-    "LensMetricTypeDef",
-    {
-        "LensArn": str,
-        "Pillars": List[PillarMetricTypeDef],
-        "RiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
 GetMilestoneOutputTypeDef = TypedDict(
     "GetMilestoneOutputTypeDef",
     {
         "WorkloadId": str,
         "Milestone": MilestoneTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1704,32 +1629,7 @@
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-ConsolidatedReportMetricTypeDef = TypedDict(
-    "ConsolidatedReportMetricTypeDef",
-    {
-        "MetricType": Literal["WORKLOAD"],
-        "RiskCounts": Dict[RiskType, int],
-        "WorkloadId": str,
-        "WorkloadName": str,
-        "WorkloadArn": str,
-        "UpdatedAt": datetime,
-        "Lenses": List[LensMetricTypeDef],
-        "LensesAppliedCount": int,
-    },
-    total=False,
-)
-
-GetConsolidatedReportOutputTypeDef = TypedDict(
-    "GetConsolidatedReportOutputTypeDef",
-    {
-        "Metrics": List[ConsolidatedReportMetricTypeDef],
-        "NextToken": str,
-        "Base64String": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected/type_defs.pyi` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -18,25 +18,22 @@
 from .literals import (
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
-    DefinitionTypeType,
     DifferenceStatusType,
-    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -52,15 +49,14 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ChoiceContentTypeDef",
     "ChoiceAnswerSummaryTypeDef",
     "ChoiceAnswerTypeDef",
     "AssociateLensesInputRequestTypeDef",
-    "BestPracticeTypeDef",
     "CheckDetailTypeDef",
     "CheckSummaryTypeDef",
     "ChoiceImprovementPlanTypeDef",
     "ChoiceUpdateTypeDef",
     "CreateLensShareInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateLensVersionInputRequestTypeDef",
@@ -70,15 +66,14 @@
     "DeleteLensInputRequestTypeDef",
     "DeleteLensShareInputRequestTypeDef",
     "DeleteWorkloadInputRequestTypeDef",
     "DeleteWorkloadShareInputRequestTypeDef",
     "DisassociateLensesInputRequestTypeDef",
     "ExportLensInputRequestTypeDef",
     "GetAnswerInputRequestTypeDef",
-    "GetConsolidatedReportInputRequestTypeDef",
     "GetLensInputRequestTypeDef",
     "LensTypeDef",
     "GetLensReviewInputRequestTypeDef",
     "GetLensReviewReportInputRequestTypeDef",
     "LensReviewReportTypeDef",
     "GetLensVersionDifferenceInputRequestTypeDef",
     "GetMilestoneInputRequestTypeDef",
@@ -112,15 +107,14 @@
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
     "AdditionalResourcesTypeDef",
-    "QuestionMetricTypeDef",
     "ImprovementSummaryTypeDef",
     "UpdateAnswerInputRequestTypeDef",
     "CreateLensShareOutputTypeDef",
     "CreateLensVersionOutputTypeDef",
     "CreateMilestoneOutputTypeDef",
     "CreateWorkloadOutputTypeDef",
     "CreateWorkloadShareOutputTypeDef",
@@ -144,34 +138,30 @@
     "ListWorkloadSharesOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
     "MilestoneSummaryTypeDef",
     "PillarDifferenceTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
     "ChoiceTypeDef",
-    "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
     "GetWorkloadOutputTypeDef",
     "MilestoneTypeDef",
     "UpdateWorkloadOutputTypeDef",
     "GetLensReviewOutputTypeDef",
     "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
     "ListMilestonesOutputTypeDef",
     "VersionDifferencesTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
-    "LensMetricTypeDef",
     "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
-    "ConsolidatedReportMetricTypeDef",
-    "GetConsolidatedReportOutputTypeDef",
 )
 
 ChoiceContentTypeDef = TypedDict(
     "ChoiceContentTypeDef",
     {
         "DisplayText": str,
         "Url": str,
@@ -204,23 +194,14 @@
     "AssociateLensesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAliases": Sequence[str],
     },
 )
 
-BestPracticeTypeDef = TypedDict(
-    "BestPracticeTypeDef",
-    {
-        "ChoiceId": str,
-        "ChoiceTitle": str,
-    },
-    total=False,
-)
-
 CheckDetailTypeDef = TypedDict(
     "CheckDetailTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "Provider": Literal["TRUSTED_ADVISOR"],
@@ -333,15 +314,14 @@
     },
 )
 
 WorkloadDiscoveryConfigTypeDef = TypedDict(
     "WorkloadDiscoveryConfigTypeDef",
     {
         "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
-        "WorkloadResourceDefinition": Sequence[DefinitionTypeType],
     },
     total=False,
 )
 
 CreateWorkloadShareInputRequestTypeDef = TypedDict(
     "CreateWorkloadShareInputRequestTypeDef",
     {
@@ -431,36 +411,14 @@
 )
 
 class GetAnswerInputRequestTypeDef(
     _RequiredGetAnswerInputRequestTypeDef, _OptionalGetAnswerInputRequestTypeDef
 ):
     pass
 
-_RequiredGetConsolidatedReportInputRequestTypeDef = TypedDict(
-    "_RequiredGetConsolidatedReportInputRequestTypeDef",
-    {
-        "Format": ReportFormatType,
-    },
-)
-_OptionalGetConsolidatedReportInputRequestTypeDef = TypedDict(
-    "_OptionalGetConsolidatedReportInputRequestTypeDef",
-    {
-        "IncludeSharedResources": bool,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class GetConsolidatedReportInputRequestTypeDef(
-    _RequiredGetConsolidatedReportInputRequestTypeDef,
-    _OptionalGetConsolidatedReportInputRequestTypeDef,
-):
-    pass
-
 _RequiredGetLensInputRequestTypeDef = TypedDict(
     "_RequiredGetLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalGetLensInputRequestTypeDef = TypedDict(
@@ -975,15 +933,14 @@
     },
 )
 
 UpdateGlobalSettingsInputRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsInputRequestTypeDef",
     {
         "OrganizationSharingStatus": OrganizationSharingStatusType,
-        "DiscoveryIntegrationStatus": DiscoveryIntegrationStatusType,
     },
     total=False,
 )
 
 _RequiredUpdateLensReviewInputRequestTypeDef = TypedDict(
     "_RequiredUpdateLensReviewInputRequestTypeDef",
     {
@@ -1062,24 +1019,14 @@
     {
         "Type": AdditionalResourceTypeType,
         "Content": List[ChoiceContentTypeDef],
     },
     total=False,
 )
 
-QuestionMetricTypeDef = TypedDict(
-    "QuestionMetricTypeDef",
-    {
-        "QuestionId": str,
-        "Risk": RiskType,
-        "BestPractices": List[BestPracticeTypeDef],
-    },
-    total=False,
-)
-
 ImprovementSummaryTypeDef = TypedDict(
     "ImprovementSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Risk": RiskType,
@@ -1457,24 +1404,14 @@
         "HelpfulResource": ChoiceContentTypeDef,
         "ImprovementPlan": ChoiceContentTypeDef,
         "AdditionalResources": List[AdditionalResourcesTypeDef],
     },
     total=False,
 )
 
-PillarMetricTypeDef = TypedDict(
-    "PillarMetricTypeDef",
-    {
-        "PillarId": str,
-        "RiskCounts": Dict[RiskType, int],
-        "Questions": List[QuestionMetricTypeDef],
-    },
-    total=False,
-)
-
 ListLensReviewImprovementsOutputTypeDef = TypedDict(
     "ListLensReviewImprovementsOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
@@ -1590,24 +1527,14 @@
         "Risk": RiskType,
         "Notes": str,
         "Reason": AnswerReasonType,
     },
     total=False,
 )
 
-LensMetricTypeDef = TypedDict(
-    "LensMetricTypeDef",
-    {
-        "LensArn": str,
-        "Pillars": List[PillarMetricTypeDef],
-        "RiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
 GetMilestoneOutputTypeDef = TypedDict(
     "GetMilestoneOutputTypeDef",
     {
         "WorkloadId": str,
         "Milestone": MilestoneTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1657,32 +1584,7 @@
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-ConsolidatedReportMetricTypeDef = TypedDict(
-    "ConsolidatedReportMetricTypeDef",
-    {
-        "MetricType": Literal["WORKLOAD"],
-        "RiskCounts": Dict[RiskType, int],
-        "WorkloadId": str,
-        "WorkloadName": str,
-        "WorkloadArn": str,
-        "UpdatedAt": datetime,
-        "Lenses": List[LensMetricTypeDef],
-        "LensesAppliedCount": int,
-    },
-    total=False,
-)
-
-GetConsolidatedReportOutputTypeDef = TypedDict(
-    "GetConsolidatedReportOutputTypeDef",
-    {
-        "Metrics": List[ConsolidatedReportMetricTypeDef],
-        "NextToken": str,
-        "Base64String": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected.egg-info/PKG-INFO` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wellarchitected
-Version: 1.26.126
-Summary: Type annotations for boto3.WellArchitected 1.26.126 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.4
+Summary: Type annotations for boto3.WellArchitected 1.26.4 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wellarchitected?color=blue)](https://pypistats.org/packages/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.26.126](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.26.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -284,26 +283,22 @@
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckProviderType,
     CheckStatusType,
     ChoiceReasonType,
     ChoiceStatusType,
-    DefinitionTypeType,
     DifferenceStatusType,
-    DiscoveryIntegrationStatusType,
     ImportLensStatusType,
     LensStatusType,
     LensStatusTypeType,
     LensTypeType,
-    MetricTypeType,
     NotificationTypeType,
     OrganizationSharingStatusType,
     PermissionTypeType,
-    ReportFormatType,
     RiskType,
     ShareInvitationActionType,
     ShareResourceTypeType,
     ShareStatusType,
     TrustedAdvisorIntegrationStatusType,
     WorkloadEnvironmentType,
     WorkloadImprovementStatusType,
@@ -327,15 +322,14 @@
 
 ```python
 from mypy_boto3_wellarchitected.type_defs import (
     ChoiceContentTypeDef,
     ChoiceAnswerSummaryTypeDef,
     ChoiceAnswerTypeDef,
     AssociateLensesInputRequestTypeDef,
-    BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
     ResponseMetadataTypeDef,
     CreateLensVersionInputRequestTypeDef,
@@ -345,15 +339,14 @@
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
     ExportLensInputRequestTypeDef,
     GetAnswerInputRequestTypeDef,
-    GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
@@ -387,15 +380,14 @@
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
     AdditionalResourcesTypeDef,
-    QuestionMetricTypeDef,
     ImprovementSummaryTypeDef,
     UpdateAnswerInputRequestTypeDef,
     CreateLensShareOutputTypeDef,
     CreateLensVersionOutputTypeDef,
     CreateMilestoneOutputTypeDef,
     CreateWorkloadOutputTypeDef,
     CreateWorkloadShareOutputTypeDef,
@@ -419,76 +411,72 @@
     ListWorkloadSharesOutputTypeDef,
     ListWorkloadsOutputTypeDef,
     MilestoneSummaryTypeDef,
     PillarDifferenceTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
     ChoiceTypeDef,
-    PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     GetWorkloadOutputTypeDef,
     MilestoneTypeDef,
     UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
     ListMilestonesOutputTypeDef,
     VersionDifferencesTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
-    LensMetricTypeDef,
     GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
-    ConsolidatedReportMetricTypeDef,
-    GetConsolidatedReportOutputTypeDef,
 )
 
 
 def get_structure() -> ChoiceContentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-wellarchitected-1.26.126/mypy_boto3_wellarchitected.egg-info/SOURCES.txt` & `mypy-boto3-wellarchitected-1.26.4/mypy_boto3_wellarchitected.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wellarchitected-1.26.126/setup.py` & `mypy-boto3-wellarchitected-1.26.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 """
 Setup script for mypy-boto3-wellarchitected.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-wellarchitected",
-    version="1.26.126",
+    version="1.26.4",
     packages=["mypy_boto3_wellarchitected"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WellArchitected 1.26.126 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.WellArchitected 1.26.4 service generated with"
+        " mypy-boto3-builder 7.11.10"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 wellarchitected type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_wellarchitected": ["py.typed", "*.pyi"]},
+    package_data={"": ["LICENSE"], "mypy_boto3_wellarchitected": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

