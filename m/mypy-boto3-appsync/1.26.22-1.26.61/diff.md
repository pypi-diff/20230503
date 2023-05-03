# Comparing `tmp/mypy-boto3-appsync-1.26.22.tar.gz` & `tmp/mypy-boto3-appsync-1.26.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appsync-1.26.22.tar", last modified: Fri Dec  2 20:32:44 2022, max compression
+gzip compressed data, was "mypy-boto3-appsync-1.26.61.tar", last modified: Tue Jan 31 20:49:53 2023, max compression
```

## Comparing `mypy-boto3-appsync-1.26.22.tar` & `mypy-boto3-appsync-1.26.61.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 20:32:44.375240 mypy-boto3-appsync-1.26.22/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-12-02 20:32:05.000000 mypy-boto3-appsync-1.26.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    18801 2022-12-02 20:32:44.375240 mypy-boto3-appsync-1.26.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17364 2022-12-02 20:32:05.000000 mypy-boto3-appsync-1.26.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 20:32:44.375240 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/
--rw-r--r--   0 runner    (1001) docker     (122)     1758 2022-12-02 20:32:05.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1757 2022-12-02 20:32:05.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      908 2022-12-02 20:32:05.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36656 2022-12-02 20:32:05.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    36591 2022-12-02 20:32:05.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    10360 2022-12-02 20:32:06.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    10358 2022-12-02 20:32:06.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     8150 2022-12-02 20:32:05.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)     8141 2022-12-02 20:32:05.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-02 20:32:05.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    47751 2022-12-02 20:32:06.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    47678 2022-12-02 20:32:06.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-12-02 20:32:05.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-02 20:32:44.375240 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    18801 2022-12-02 20:32:44.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      680 2022-12-02 20:32:44.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-02 20:32:44.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-02 20:32:44.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-12-02 20:32:44.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2022-12-02 20:32:44.000000 mypy-boto3-appsync-1.26.22/mypy_boto3_appsync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-02 20:32:44.375240 mypy-boto3-appsync-1.26.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1964 2022-12-02 20:32:05.000000 mypy-boto3-appsync-1.26.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.626128 mypy-boto3-appsync-1.26.61/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-01-31 20:49:53.626128 mypy-boto3-appsync-1.26.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17403 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.614128 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36769 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-01-31 20:47:21.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-01-31 20:47:21.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-01-31 20:47:21.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48122 2023-01-31 20:47:22.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48049 2023-01-31 20:47:21.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.626128 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-01-31 20:49:53.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-31 20:49:53.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:53.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:53.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:53.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-31 20:49:53.000000 mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 20:49:53.626128 mypy-boto3-appsync-1.26.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-01-31 20:47:20.000000 mypy-boto3-appsync-1.26.61/setup.py
```

### Comparing `mypy-boto3-appsync-1.26.22/LICENSE` & `mypy-boto3-appsync-1.26.61/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.26.22/PKG-INFO` & `mypy-boto3-appsync-1.26.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appsync
-Version: 1.26.22
-Summary: Type annotations for boto3.AppSync 1.26.22 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.61
+Summary: Type annotations for boto3.AppSync 1.26.61 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appsync?color=blue)](https://pypistats.org/packages/mypy-boto3-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppSync 1.26.22](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[boto3.AppSync 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,14 +372,15 @@
     ResponseMetadataTypeDef,
     AwsIamConfigTypeDef,
     CachingConfigTypeDef,
     CodeErrorLocationTypeDef,
     CreateApiCacheRequestRequestTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
+    EventBridgeDataSourceConfigTypeDef,
     LambdaDataSourceConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
     CreateDomainNameRequestRequestTypeDef,
     DomainNameConfigTypeDef,
     LogConfigTypeDef,
     UserPoolConfigTypeDef,
     PipelineConfigTypeDef,
```

### Comparing `mypy-boto3-appsync-1.26.22/README.md` & `mypy-boto3-appsync-1.26.61/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appsync?color=blue)](https://pypistats.org/packages/mypy-boto3-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppSync 1.26.22](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[boto3.AppSync 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,14 +340,15 @@
     ResponseMetadataTypeDef,
     AwsIamConfigTypeDef,
     CachingConfigTypeDef,
     CodeErrorLocationTypeDef,
     CreateApiCacheRequestRequestTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
+    EventBridgeDataSourceConfigTypeDef,
     LambdaDataSourceConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
     CreateDomainNameRequestRequestTypeDef,
     DomainNameConfigTypeDef,
     LogConfigTypeDef,
     UserPoolConfigTypeDef,
     PipelineConfigTypeDef,
```

### Comparing `mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/__init__.py` & `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/__init__.pyi` & `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/__main__.py` & `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppSync 1.26.22\nVersion:         1.26.22\nBuilder version:"
-        " 7.11.11\nDocs:           "
+        "Type annotations for boto3.AppSync 1.26.61\nVersion:         1.26.61\nBuilder version:"
+        " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.22")
+    print("1.26.61")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/client.py` & `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     CreateGraphqlApiResponseTypeDef,
     CreateResolverResponseTypeDef,
     CreateTypeResponseTypeDef,
     DynamodbDataSourceConfigTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
     EvaluateCodeResponseTypeDef,
     EvaluateMappingTemplateResponseTypeDef,
+    EventBridgeDataSourceConfigTypeDef,
     GetApiAssociationResponseTypeDef,
     GetApiCacheResponseTypeDef,
     GetDataSourceResponseTypeDef,
     GetDomainNameResponseTypeDef,
     GetFunctionResponseTypeDef,
     GetGraphqlApiResponseTypeDef,
     GetIntrospectionSchemaResponseTypeDef,
@@ -203,15 +204,16 @@
         description: str = ...,
         serviceRoleArn: str = ...,
         dynamodbConfig: DynamodbDataSourceConfigTypeDef = ...,
         lambdaConfig: LambdaDataSourceConfigTypeDef = ...,
         elasticsearchConfig: ElasticsearchDataSourceConfigTypeDef = ...,
         openSearchServiceConfig: OpenSearchServiceDataSourceConfigTypeDef = ...,
         httpConfig: HttpDataSourceConfigTypeDef = ...,
-        relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...
+        relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...,
+        eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a `DataSource` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#create_data_source)
         """
@@ -655,15 +657,16 @@
         description: str = ...,
         serviceRoleArn: str = ...,
         dynamodbConfig: DynamodbDataSourceConfigTypeDef = ...,
         lambdaConfig: LambdaDataSourceConfigTypeDef = ...,
         elasticsearchConfig: ElasticsearchDataSourceConfigTypeDef = ...,
         openSearchServiceConfig: OpenSearchServiceDataSourceConfigTypeDef = ...,
         httpConfig: HttpDataSourceConfigTypeDef = ...,
-        relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...
+        relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...,
+        eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Updates a `DataSource` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#update_data_source)
         """
```

### Comparing `mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/client.pyi` & `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     CreateGraphqlApiResponseTypeDef,
     CreateResolverResponseTypeDef,
     CreateTypeResponseTypeDef,
     DynamodbDataSourceConfigTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
     EvaluateCodeResponseTypeDef,
     EvaluateMappingTemplateResponseTypeDef,
+    EventBridgeDataSourceConfigTypeDef,
     GetApiAssociationResponseTypeDef,
     GetApiCacheResponseTypeDef,
     GetDataSourceResponseTypeDef,
     GetDomainNameResponseTypeDef,
     GetFunctionResponseTypeDef,
     GetGraphqlApiResponseTypeDef,
     GetIntrospectionSchemaResponseTypeDef,
@@ -193,15 +194,16 @@
         description: str = ...,
         serviceRoleArn: str = ...,
         dynamodbConfig: DynamodbDataSourceConfigTypeDef = ...,
         lambdaConfig: LambdaDataSourceConfigTypeDef = ...,
         elasticsearchConfig: ElasticsearchDataSourceConfigTypeDef = ...,
         openSearchServiceConfig: OpenSearchServiceDataSourceConfigTypeDef = ...,
         httpConfig: HttpDataSourceConfigTypeDef = ...,
-        relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...
+        relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...,
+        eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a `DataSource` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#create_data_source)
         """
@@ -602,15 +604,16 @@
         description: str = ...,
         serviceRoleArn: str = ...,
         dynamodbConfig: DynamodbDataSourceConfigTypeDef = ...,
         lambdaConfig: LambdaDataSourceConfigTypeDef = ...,
         elasticsearchConfig: ElasticsearchDataSourceConfigTypeDef = ...,
         openSearchServiceConfig: OpenSearchServiceDataSourceConfigTypeDef = ...,
         httpConfig: HttpDataSourceConfigTypeDef = ...,
-        relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...
+        relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...,
+        eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Updates a `DataSource` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_data_source)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/client/#update_data_source)
         """
```

### Comparing `mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/literals.py` & `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApiCacheStatusType",
     "ApiCacheTypeType",
     "ApiCachingBehaviorType",
     "AssociationStatusType",
     "AuthenticationTypeType",
     "AuthorizationTypeType",
@@ -47,15 +46,14 @@
     "AppSyncServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApiCacheStatusType = Literal["AVAILABLE", "CREATING", "DELETING", "FAILED", "MODIFYING"]
 ApiCacheTypeType = Literal[
     "LARGE",
     "LARGE_12X",
     "LARGE_2X",
     "LARGE_4X",
     "LARGE_8X",
@@ -77,14 +75,15 @@
 ]
 AuthorizationTypeType = Literal["AWS_IAM"]
 ConflictDetectionTypeType = Literal["NONE", "VERSION"]
 ConflictHandlerTypeType = Literal["AUTOMERGE", "LAMBDA", "NONE", "OPTIMISTIC_CONCURRENCY"]
 DataSourceTypeType = Literal[
     "AMAZON_DYNAMODB",
     "AMAZON_ELASTICSEARCH",
+    "AMAZON_EVENTBRIDGE",
     "AMAZON_OPENSEARCH_SERVICE",
     "AWS_LAMBDA",
     "HTTP",
     "NONE",
     "RELATIONAL_DATABASE",
 ]
 DefaultActionType = Literal["ALLOW", "DENY"]
@@ -144,24 +143,26 @@
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
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -269,30 +270,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
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
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -378,14 +382,15 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
```

### Comparing `mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/literals.pyi` & `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ApiCacheStatusType",
     "ApiCacheTypeType",
     "ApiCachingBehaviorType",
     "AssociationStatusType",
     "AuthenticationTypeType",
     "AuthorizationTypeType",
@@ -46,14 +47,15 @@
     "AppSyncServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ApiCacheStatusType = Literal["AVAILABLE", "CREATING", "DELETING", "FAILED", "MODIFYING"]
 ApiCacheTypeType = Literal[
     "LARGE",
     "LARGE_12X",
     "LARGE_2X",
     "LARGE_4X",
     "LARGE_8X",
@@ -75,14 +77,15 @@
 ]
 AuthorizationTypeType = Literal["AWS_IAM"]
 ConflictDetectionTypeType = Literal["NONE", "VERSION"]
 ConflictHandlerTypeType = Literal["AUTOMERGE", "LAMBDA", "NONE", "OPTIMISTIC_CONCURRENCY"]
 DataSourceTypeType = Literal[
     "AMAZON_DYNAMODB",
     "AMAZON_ELASTICSEARCH",
+    "AMAZON_EVENTBRIDGE",
     "AMAZON_OPENSEARCH_SERVICE",
     "AWS_LAMBDA",
     "HTTP",
     "NONE",
     "RELATIONAL_DATABASE",
 ]
 DefaultActionType = Literal["ALLOW", "DENY"]
@@ -142,24 +145,26 @@
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
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
@@ -267,30 +272,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
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
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -376,14 +384,15 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
```

### Comparing `mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/paginator.py` & `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/paginator.pyi` & `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/type_defs.py` & `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     "ResponseMetadataTypeDef",
     "AwsIamConfigTypeDef",
     "CachingConfigTypeDef",
     "CodeErrorLocationTypeDef",
     "CreateApiCacheRequestRequestTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "ElasticsearchDataSourceConfigTypeDef",
+    "EventBridgeDataSourceConfigTypeDef",
     "LambdaDataSourceConfigTypeDef",
     "OpenSearchServiceDataSourceConfigTypeDef",
     "CreateDomainNameRequestRequestTypeDef",
     "DomainNameConfigTypeDef",
     "LogConfigTypeDef",
     "UserPoolConfigTypeDef",
     "PipelineConfigTypeDef",
@@ -397,14 +398,21 @@
     "ElasticsearchDataSourceConfigTypeDef",
     {
         "endpoint": str,
         "awsRegion": str,
     },
 )
 
+EventBridgeDataSourceConfigTypeDef = TypedDict(
+    "EventBridgeDataSourceConfigTypeDef",
+    {
+        "eventBusArn": str,
+    },
+)
+
 LambdaDataSourceConfigTypeDef = TypedDict(
     "LambdaDataSourceConfigTypeDef",
     {
         "lambdaFunctionArn": str,
     },
 )
 
@@ -1737,14 +1745,15 @@
         "serviceRoleArn": str,
         "dynamodbConfig": DynamodbDataSourceConfigTypeDef,
         "lambdaConfig": LambdaDataSourceConfigTypeDef,
         "elasticsearchConfig": ElasticsearchDataSourceConfigTypeDef,
         "openSearchServiceConfig": OpenSearchServiceDataSourceConfigTypeDef,
         "httpConfig": HttpDataSourceConfigTypeDef,
         "relationalDatabaseConfig": RelationalDatabaseDataSourceConfigTypeDef,
+        "eventBridgeConfig": EventBridgeDataSourceConfigTypeDef,
     },
     total=False,
 )
 
 
 class CreateDataSourceRequestRequestTypeDef(
     _RequiredCreateDataSourceRequestRequestTypeDef, _OptionalCreateDataSourceRequestRequestTypeDef
@@ -1762,14 +1771,15 @@
         "serviceRoleArn": str,
         "dynamodbConfig": DynamodbDataSourceConfigTypeDef,
         "lambdaConfig": LambdaDataSourceConfigTypeDef,
         "elasticsearchConfig": ElasticsearchDataSourceConfigTypeDef,
         "openSearchServiceConfig": OpenSearchServiceDataSourceConfigTypeDef,
         "httpConfig": HttpDataSourceConfigTypeDef,
         "relationalDatabaseConfig": RelationalDatabaseDataSourceConfigTypeDef,
+        "eventBridgeConfig": EventBridgeDataSourceConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataSourceRequestRequestTypeDef",
     {
@@ -1785,14 +1795,15 @@
         "serviceRoleArn": str,
         "dynamodbConfig": DynamodbDataSourceConfigTypeDef,
         "lambdaConfig": LambdaDataSourceConfigTypeDef,
         "elasticsearchConfig": ElasticsearchDataSourceConfigTypeDef,
         "openSearchServiceConfig": OpenSearchServiceDataSourceConfigTypeDef,
         "httpConfig": HttpDataSourceConfigTypeDef,
         "relationalDatabaseConfig": RelationalDatabaseDataSourceConfigTypeDef,
+        "eventBridgeConfig": EventBridgeDataSourceConfigTypeDef,
     },
     total=False,
 )
 
 
 class UpdateDataSourceRequestRequestTypeDef(
     _RequiredUpdateDataSourceRequestRequestTypeDef, _OptionalUpdateDataSourceRequestRequestTypeDef
```

### Comparing `mypy-boto3-appsync-1.26.22/mypy_boto3_appsync/type_defs.pyi` & `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     "ResponseMetadataTypeDef",
     "AwsIamConfigTypeDef",
     "CachingConfigTypeDef",
     "CodeErrorLocationTypeDef",
     "CreateApiCacheRequestRequestTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "ElasticsearchDataSourceConfigTypeDef",
+    "EventBridgeDataSourceConfigTypeDef",
     "LambdaDataSourceConfigTypeDef",
     "OpenSearchServiceDataSourceConfigTypeDef",
     "CreateDomainNameRequestRequestTypeDef",
     "DomainNameConfigTypeDef",
     "LogConfigTypeDef",
     "UserPoolConfigTypeDef",
     "PipelineConfigTypeDef",
@@ -384,14 +385,21 @@
     "ElasticsearchDataSourceConfigTypeDef",
     {
         "endpoint": str,
         "awsRegion": str,
     },
 )
 
+EventBridgeDataSourceConfigTypeDef = TypedDict(
+    "EventBridgeDataSourceConfigTypeDef",
+    {
+        "eventBusArn": str,
+    },
+)
+
 LambdaDataSourceConfigTypeDef = TypedDict(
     "LambdaDataSourceConfigTypeDef",
     {
         "lambdaFunctionArn": str,
     },
 )
 
@@ -1668,14 +1676,15 @@
         "serviceRoleArn": str,
         "dynamodbConfig": DynamodbDataSourceConfigTypeDef,
         "lambdaConfig": LambdaDataSourceConfigTypeDef,
         "elasticsearchConfig": ElasticsearchDataSourceConfigTypeDef,
         "openSearchServiceConfig": OpenSearchServiceDataSourceConfigTypeDef,
         "httpConfig": HttpDataSourceConfigTypeDef,
         "relationalDatabaseConfig": RelationalDatabaseDataSourceConfigTypeDef,
+        "eventBridgeConfig": EventBridgeDataSourceConfigTypeDef,
     },
     total=False,
 )
 
 class CreateDataSourceRequestRequestTypeDef(
     _RequiredCreateDataSourceRequestRequestTypeDef, _OptionalCreateDataSourceRequestRequestTypeDef
 ):
@@ -1691,14 +1700,15 @@
         "serviceRoleArn": str,
         "dynamodbConfig": DynamodbDataSourceConfigTypeDef,
         "lambdaConfig": LambdaDataSourceConfigTypeDef,
         "elasticsearchConfig": ElasticsearchDataSourceConfigTypeDef,
         "openSearchServiceConfig": OpenSearchServiceDataSourceConfigTypeDef,
         "httpConfig": HttpDataSourceConfigTypeDef,
         "relationalDatabaseConfig": RelationalDatabaseDataSourceConfigTypeDef,
+        "eventBridgeConfig": EventBridgeDataSourceConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDataSourceRequestRequestTypeDef",
     {
@@ -1714,14 +1724,15 @@
         "serviceRoleArn": str,
         "dynamodbConfig": DynamodbDataSourceConfigTypeDef,
         "lambdaConfig": LambdaDataSourceConfigTypeDef,
         "elasticsearchConfig": ElasticsearchDataSourceConfigTypeDef,
         "openSearchServiceConfig": OpenSearchServiceDataSourceConfigTypeDef,
         "httpConfig": HttpDataSourceConfigTypeDef,
         "relationalDatabaseConfig": RelationalDatabaseDataSourceConfigTypeDef,
+        "eventBridgeConfig": EventBridgeDataSourceConfigTypeDef,
     },
     total=False,
 )
 
 class UpdateDataSourceRequestRequestTypeDef(
     _RequiredUpdateDataSourceRequestRequestTypeDef, _OptionalUpdateDataSourceRequestRequestTypeDef
 ):
```

### Comparing `mypy-boto3-appsync-1.26.22/mypy_boto3_appsync.egg-info/PKG-INFO` & `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appsync
-Version: 1.26.22
-Summary: Type annotations for boto3.AppSync 1.26.22 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.61
+Summary: Type annotations for boto3.AppSync 1.26.61 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appsync.svg?color=blue)](https://pypi.org/project/mypy-boto3-appsync)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appsync?color=blue)](https://pypistats.org/packages/mypy-boto3-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppSync 1.26.22](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[boto3.AppSync 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-appsync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,14 +372,15 @@
     ResponseMetadataTypeDef,
     AwsIamConfigTypeDef,
     CachingConfigTypeDef,
     CodeErrorLocationTypeDef,
     CreateApiCacheRequestRequestTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
+    EventBridgeDataSourceConfigTypeDef,
     LambdaDataSourceConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
     CreateDomainNameRequestRequestTypeDef,
     DomainNameConfigTypeDef,
     LogConfigTypeDef,
     UserPoolConfigTypeDef,
     PipelineConfigTypeDef,
```

### Comparing `mypy-boto3-appsync-1.26.22/mypy_boto3_appsync.egg-info/SOURCES.txt` & `mypy-boto3-appsync-1.26.61/mypy_boto3_appsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appsync-1.26.22/setup.py` & `mypy-boto3-appsync-1.26.61/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-appsync",
-    version="1.26.22",
+    version="1.26.61",
     packages=["mypy_boto3_appsync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppSync 1.26.22 service generated with mypy-boto3-builder"
-        " 7.11.11"
+        "Type annotations for boto3.AppSync 1.26.61 service generated with mypy-boto3-builder"
+        " 7.12.3"
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
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 appsync type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_appsync": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_appsync": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appsync/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

