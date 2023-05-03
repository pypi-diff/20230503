# Comparing `tmp/iam_actions-1.2.20230502.tar.gz` & `tmp/iam_actions-1.2.20230503.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230502.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230503.tar", max compression
```

## Comparing `iam_actions-1.2.20230502.tar` & `iam_actions-1.2.20230503.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/README.md
--rw-r--r--   0        0        0      228 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/__init__.py
--rw-r--r--   0        0        0  4242733 2023-05-02 02:27:51.362925 iam_actions-1.2.20230502/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-02 02:26:20.809970 iam_actions-1.2.20230502/iam_actions/generate/services.py
--rw-r--r--   0        0        0   545585 2023-05-02 02:27:51.362925 iam_actions-1.2.20230502/iam_actions/policies.json
--rw-r--r--   0        0        0   193567 2023-05-02 02:27:51.362925 iam_actions-1.2.20230502/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   529122 2023-05-02 02:27:51.362925 iam_actions-1.2.20230502/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-02 02:27:52.106933 iam_actions-1.2.20230502/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230502/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230502/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/README.md
+-rw-r--r--   0        0        0      228 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4244063 2023-05-03 02:26:59.365832 iam_actions-1.2.20230503/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-03 02:24:41.002322 iam_actions-1.2.20230503/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   545650 2023-05-03 02:26:59.365832 iam_actions-1.2.20230503/iam_actions/policies.json
+-rw-r--r--   0        0        0   193569 2023-05-03 02:26:59.365832 iam_actions-1.2.20230503/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   529184 2023-05-03 02:26:59.365832 iam_actions-1.2.20230503/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-03 02:27:00.281881 iam_actions-1.2.20230503/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230503/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230503/PKG-INFO
```

### Comparing `iam_actions-1.2.20230502/LICENSE` & `iam_actions-1.2.20230503/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230502/README.md` & `iam_actions-1.2.20230503/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230502/iam_actions/actions.json` & `iam_actions-1.2.20230503/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998155259621542%*

 * *Differences: {"'amplifybackend'": "{'CreateBackendConfig': {'resources': ['config']}, 'RemoveBackendConfig': "*

 * *                     "{'resources': ['config']}, 'UpdateBackendConfig': {'resources': ['config']}}",*

 * * "'cassandra'": "{'TagMultiRegionResource': {'access_level': 'Tagging', 'condition_keys': "*

 * *                "['aws:RequestTag/${TagKey}', 'aws:TagKeys'], 'description': 'Grants permission to "*

 * *                "tag a multiregion keyspace or table', 'resources': ['keyspace', 'table']}, "*

 * *                "'RestoreM […]*

```diff
@@ -2433,15 +2433,15 @@
         "CreateBackendConfig": {
             "access_level": "Write",
             "action": "CreateBackendConfig",
             "condition_keys": [],
             "description": "Grants permission to create a new Amplify Admin backend config by Amplify appId",
             "orphan": false,
             "resources": [
-                "backend"
+                "config"
             ]
         },
         "CreateBackendStorage": {
             "access_level": "Write",
             "action": "CreateBackendStorage",
             "condition_keys": [],
             "description": "Grants permission to create a backend storage resource",
@@ -2666,15 +2666,15 @@
         "RemoveBackendConfig": {
             "access_level": "Write",
             "action": "RemoveBackendConfig",
             "condition_keys": [],
             "description": "Grants permission to delete an Amplify Admin backend config by Amplify appId",
             "orphan": false,
             "resources": [
-                "backend"
+                "config"
             ]
         },
         "UpdateBackendAPI": {
             "access_level": "Write",
             "action": "UpdateBackendAPI",
             "condition_keys": [],
             "description": "Grants permission to update an API of an existing Amplify Admin backend environment by appId and backendEnvironmentName",
@@ -2700,15 +2700,15 @@
         "UpdateBackendConfig": {
             "access_level": "Write",
             "action": "UpdateBackendConfig",
             "condition_keys": [],
             "description": "Grants permission to update an Amplify Admin backend config by Amplify appId",
             "orphan": false,
             "resources": [
-                "backend"
+                "config"
             ]
         },
         "UpdateBackendJob": {
             "access_level": "Write",
             "action": "UpdateBackendJob",
             "condition_keys": [],
             "description": "Grants permission to update a job of an existing Amplify Admin backend environment by appId and backendEnvironmentName",
@@ -13262,20 +13262,26 @@
             "orphan": false,
             "resources": [
                 "keyspace",
                 "table"
             ]
         },
         "AlterMultiRegionResource": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AlterMultiRegionResource",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to alter a multiregion keyspace or table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "keyspace",
+                "table"
+            ]
         },
         "Create": {
             "access_level": "Write",
             "action": "Create",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -13284,57 +13290,68 @@
             "orphan": false,
             "resources": [
                 "keyspace",
                 "table"
             ]
         },
         "CreateMultiRegionResource": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateMultiRegionResource",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a multiregion keyspace or table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "keyspace",
+                "table"
+            ]
         },
         "Drop": {
             "access_level": "Write",
             "action": "Drop",
             "condition_keys": [],
             "description": "Grants permission to drop a keyspace or table",
             "orphan": false,
             "resources": [
                 "keyspace",
                 "table"
             ]
         },
         "DropMultiRegionResource": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DropMultiRegionResource",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to drop a multiregion keyspace or table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "keyspace",
+                "table"
+            ]
         },
         "Modify": {
             "access_level": "Write",
             "action": "Modify",
             "condition_keys": [],
             "description": "Grants permission to INSERT, UPDATE or DELETE data in a table",
             "orphan": false,
             "resources": [
                 "table"
             ]
         },
         "ModifyMultiRegionResource": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ModifyMultiRegionResource",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to INSERT, UPDATE or DELETE data in a multiregion table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "table"
+            ]
         },
         "Restore": {
             "access_level": "Write",
             "action": "Restore",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -13342,46 +13359,59 @@
             "description": "Grants permission to restore table from a backup",
             "orphan": false,
             "resources": [
                 "table"
             ]
         },
         "RestoreMultiRegionTable": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RestoreMultiRegionTable",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to restore multiregion table from a backup",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "table"
+            ]
         },
         "Select": {
             "access_level": "Read",
             "action": "Select",
             "condition_keys": [],
             "description": "Grants permission to SELECT data from a table",
             "orphan": false,
             "resources": [
                 "table"
             ]
         },
         "SelectMultiRegionResource": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "SelectMultiRegionResource",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to SELECT data from a multiregion table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "table"
+            ]
         },
         "TagMultiRegionResource": {
-            "access_level": "Undocumented",
+            "access_level": "Tagging",
             "action": "TagMultiRegionResource",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to tag a multiregion keyspace or table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "keyspace",
+                "table"
+            ]
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -13390,20 +13420,26 @@
             "orphan": false,
             "resources": [
                 "keyspace",
                 "table"
             ]
         },
         "UnTagMultiRegionResource": {
-            "access_level": "Undocumented",
+            "access_level": "Tagging",
             "action": "UnTagMultiRegionResource",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to untag a multiregion keyspace or table",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "keyspace",
+                "table"
+            ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
@@ -146936,14 +146972,22 @@
             "access_level": "Read",
             "action": "CheckCapacity",
             "condition_keys": [],
             "description": "Grants permission to calculate web ACL capacity unit (WCU) requirements for a specified scope and set of rules",
             "orphan": false,
             "resources": []
         },
+        "CreateAPIKey": {
+            "access_level": "Undocumented",
+            "action": "CreateAPIKey",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateIPSet": {
             "access_level": "Write",
             "action": "CreateIPSet",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -147104,14 +147148,22 @@
             "access_level": "Read",
             "action": "GenerateMobileSdkReleaseUrl",
             "condition_keys": [],
             "description": "Grants permission to generate a presigned download URL for the specified release of the mobile SDK",
             "orphan": false,
             "resources": []
         },
+        "GetDecryptedAPIKey": {
+            "access_level": "Undocumented",
+            "action": "GetDecryptedAPIKey",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetIPSet": {
             "access_level": "Read",
             "action": "GetIPSet",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to retrieve details about an IPSet",
@@ -147228,14 +147280,22 @@
                 "apigateway",
                 "apprunner",
                 "appsync",
                 "loadbalancer/app/",
                 "userpool"
             ]
         },
+        "ListAPIKeys": {
+            "access_level": "Undocumented",
+            "action": "ListAPIKeys",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListAvailableManagedRuleGroupVersions": {
             "access_level": "List",
             "action": "ListAvailableManagedRuleGroupVersions",
             "condition_keys": [],
             "description": "Grants permission to retrieve an array of managed rule group versions that are available for you to use",
             "orphan": false,
             "resources": []
```

### Comparing `iam_actions-1.2.20230502/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230503/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230502/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230503/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230502/iam_actions/generate/generate.py` & `iam_actions-1.2.20230503/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230502/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230503/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230502/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230503/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230502/iam_actions/generate/services.py` & `iam_actions-1.2.20230503/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230502/iam_actions/policies.json` & `iam_actions-1.2.20230503/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999993693875492%*

 * *Differences: {"'serviceMap'": "{'AWS WAF V2': {'Actions': {insert: [(2, 'CreateAPIKey'), (18, "*

 * *                 "'GetDecryptedAPIKey'), (30, 'ListAPIKeys')]}}}"}*

```diff
@@ -9187,14 +9187,15 @@
         },
         "AWS WAF V2": {
             "ARNFormat": "arn:aws:wafv2:${Region}:${Account}:${Scope}/${ResourceType}/${ResourceName}/${ResourceId}",
             "ARNRegex": "^arn:aws:wafv2:.+:.+:.+/.+/.+/.+",
             "Actions": [
                 "AssociateWebACL",
                 "CheckCapacity",
+                "CreateAPIKey",
                 "CreateIPSet",
                 "CreateRegexPatternSet",
                 "CreateRuleGroup",
                 "CreateWebACL",
                 "DeleteFirewallManagerRuleGroups",
                 "DeleteIPSet",
                 "DeleteLoggingConfiguration",
@@ -9202,25 +9203,27 @@
                 "DeleteRegexPatternSet",
                 "DeleteRuleGroup",
                 "DeleteWebACL",
                 "DescribeManagedRuleGroup",
                 "DisassociateFirewallManager",
                 "DisassociateWebACL",
                 "GenerateMobileSdkReleaseUrl",
+                "GetDecryptedAPIKey",
                 "GetIPSet",
                 "GetLoggingConfiguration",
                 "GetManagedRuleSet",
                 "GetMobileSdkRelease",
                 "GetPermissionPolicy",
                 "GetRateBasedStatementManagedKeys",
                 "GetRegexPatternSet",
                 "GetRuleGroup",
                 "GetSampledRequests",
                 "GetWebACL",
                 "GetWebACLForResource",
+                "ListAPIKeys",
                 "ListAvailableManagedRuleGroupVersions",
                 "ListAvailableManagedRuleGroups",
                 "ListIPSets",
                 "ListLoggingConfigurations",
                 "ListManagedRuleSets",
                 "ListMobileSdkReleases",
                 "ListRegexPatternSets",
```

### Comparing `iam_actions-1.2.20230502/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230503/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999781162464986%*

 * *Differences: {"'amplifybackend'": "{'config': {'arn_pattern': 'arn:*:amplifybackend:*:*:backend/*/config/*'}}"}*

```diff
@@ -125,15 +125,15 @@
             "condition_keys": null
         },
         "backend": {
             "arn_pattern": "arn:*:amplifybackend:*:*:backend/*",
             "condition_keys": null
         },
         "config": {
-            "arn_pattern": "arn:*:amplifybackend:*:*:backend/*/config",
+            "arn_pattern": "arn:*:amplifybackend:*:*:backend/*/config/*",
             "condition_keys": null
         },
         "environment": {
             "arn_pattern": "arn:*:amplifybackend:*:*:backend/*/environments",
             "condition_keys": null
         },
         "job": {
```

### Comparing `iam_actions-1.2.20230502/iam_actions/services.json` & `iam_actions-1.2.20230503/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999933935838486%*

 * *Differences: {"'wafv2'": "{'Actions': {insert: [(2, 'CreateAPIKey'), (18, 'GetDecryptedAPIKey'), (30, "*

 * *            "'ListAPIKeys')]}}"}*

```diff
@@ -20671,14 +20671,15 @@
         ],
         "ARNRegexes": [
             "^arn:aws:wafv2:.+:.+:.+/.+/.+/.+"
         ],
         "Actions": [
             "AssociateWebACL",
             "CheckCapacity",
+            "CreateAPIKey",
             "CreateIPSet",
             "CreateRegexPatternSet",
             "CreateRuleGroup",
             "CreateWebACL",
             "DeleteFirewallManagerRuleGroups",
             "DeleteIPSet",
             "DeleteLoggingConfiguration",
@@ -20686,25 +20687,27 @@
             "DeleteRegexPatternSet",
             "DeleteRuleGroup",
             "DeleteWebACL",
             "DescribeManagedRuleGroup",
             "DisassociateFirewallManager",
             "DisassociateWebACL",
             "GenerateMobileSdkReleaseUrl",
+            "GetDecryptedAPIKey",
             "GetIPSet",
             "GetLoggingConfiguration",
             "GetManagedRuleSet",
             "GetMobileSdkRelease",
             "GetPermissionPolicy",
             "GetRateBasedStatementManagedKeys",
             "GetRegexPatternSet",
             "GetRuleGroup",
             "GetSampledRequests",
             "GetWebACL",
             "GetWebACLForResource",
+            "ListAPIKeys",
             "ListAvailableManagedRuleGroupVersions",
             "ListAvailableManagedRuleGroups",
             "ListIPSets",
             "ListLoggingConfigurations",
             "ListManagedRuleSets",
             "ListMobileSdkReleases",
             "ListRegexPatternSets",
```

### Comparing `iam_actions-1.2.20230502/pyproject.toml` & `iam_actions-1.2.20230503/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230502"
+version = "1.2.20230503"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230502/setup.py` & `iam_actions-1.2.20230503/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230502',
+    'version': '1.2.20230503',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230502/PKG-INFO` & `iam_actions-1.2.20230503/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230502
+Version: 1.2.20230503
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

