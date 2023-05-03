# Comparing `tmp/mypy-boto3-iottwinmaker-1.26.26.tar.gz` & `tmp/mypy-boto3-iottwinmaker-1.26.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iottwinmaker-1.26.26.tar", last modified: Thu Dec  8 20:25:42 2022, max compression
+gzip compressed data, was "mypy-boto3-iottwinmaker-1.26.97.tar", last modified: Wed Mar 22 19:32:31 2023, max compression
```

## Comparing `mypy-boto3-iottwinmaker-1.26.26.tar` & `mypy-boto3-iottwinmaker-1.26.97.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:25:42.976790 mypy-boto3-iottwinmaker-1.26.26/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-08 20:25:31.000000 mypy-boto3-iottwinmaker-1.26.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16383 2022-12-08 20:25:42.976790 mypy-boto3-iottwinmaker-1.26.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2022-12-08 20:25:31.000000 mypy-boto3-iottwinmaker-1.26.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:25:42.976790 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2022-12-08 20:25:31.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2022-12-08 20:25:31.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2022-12-08 20:25:31.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24671 2022-12-08 20:25:31.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2022-12-08 20:25:31.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9087 2022-12-08 20:25:32.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2022-12-08 20:25:32.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 20:25:31.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43079 2022-12-08 20:25:33.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43006 2022-12-08 20:25:33.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-08 20:25:31.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:25:42.976790 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16383 2022-12-08 20:25:42.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2022-12-08 20:25:42.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 20:25:42.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 20:25:42.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-08 20:25:42.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-08 20:25:42.000000 mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 20:25:42.976790 mypy-boto3-iottwinmaker-1.26.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2022-12-08 20:25:31.000000 mypy-boto3-iottwinmaker-1.26.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.337776 mypy-boto3-iottwinmaker-1.26.97/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-03-22 19:32:31.337776 mypy-boto3-iottwinmaker-1.26.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.337776 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43258 2023-03-22 19:32:05.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43185 2023-03-22 19:32:04.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:32:31.337776 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-03-22 19:32:31.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-22 19:32:31.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:32:31.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-22 19:32:31.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-22 19:32:31.000000 mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 19:32:31.337776 mypy-boto3-iottwinmaker-1.26.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-22 19:32:03.000000 mypy-boto3-iottwinmaker-1.26.97/setup.py
```

### Comparing `mypy-boto3-iottwinmaker-1.26.26/LICENSE` & `mypy-boto3-iottwinmaker-1.26.97/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.26.26/PKG-INFO` & `mypy-boto3-iottwinmaker-1.26.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iottwinmaker
-Version: 1.26.26
-Summary: Type annotations for boto3.IoTTwinMaker 1.26.26 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.97
+Summary: Type annotations for boto3.IoTTwinMaker 1.26.97 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iottwinmaker?color=blue)](https://pypistats.org/packages/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.26.26](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iottwinmaker-1.26.26/README.md` & `mypy-boto3-iottwinmaker-1.26.97/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iottwinmaker?color=blue)](https://pypistats.org/packages/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.26.26](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/__main__.py` & `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTTwinMaker 1.26.26\nVersion:         1.26.26\nBuilder"
-        " version: 7.12.0\nDocs:           "
+        "Type annotations for boto3.IoTTwinMaker 1.26.97\nVersion:         1.26.97\nBuilder"
+        " version: 7.13.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.26")
+    print("1.26.97")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/client.py` & `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,16 @@
         self,
         *,
         workspaceId: str,
         sceneId: str,
         contentLocation: str,
         description: str = ...,
         capabilities: Sequence[str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
+        sceneMetadata: Mapping[str, str] = ...
     ) -> CreateSceneResponseTypeDef:
         """
         Creates a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_scene)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/client/#create_scene)
         """
@@ -533,15 +534,16 @@
     def update_scene(
         self,
         *,
         workspaceId: str,
         sceneId: str,
         contentLocation: str = ...,
         description: str = ...,
-        capabilities: Sequence[str] = ...
+        capabilities: Sequence[str] = ...,
+        sceneMetadata: Mapping[str, str] = ...
     ) -> UpdateSceneResponseTypeDef:
         """
         Updates a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_scene)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/client/#update_scene)
         """
```

### Comparing `mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/client.pyi` & `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,16 @@
         self,
         *,
         workspaceId: str,
         sceneId: str,
         contentLocation: str,
         description: str = ...,
         capabilities: Sequence[str] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
+        sceneMetadata: Mapping[str, str] = ...
     ) -> CreateSceneResponseTypeDef:
         """
         Creates a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_scene)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/client/#create_scene)
         """
@@ -494,15 +495,16 @@
     def update_scene(
         self,
         *,
         workspaceId: str,
         sceneId: str,
         contentLocation: str = ...,
         description: str = ...,
-        capabilities: Sequence[str] = ...
+        capabilities: Sequence[str] = ...,
+        sceneMetadata: Mapping[str, str] = ...
     ) -> UpdateSceneResponseTypeDef:
         """
         Updates a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_scene)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/client/#update_scene)
         """
```

### Comparing `mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/literals.py` & `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,24 +113,26 @@
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
@@ -216,14 +218,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -238,30 +241,33 @@
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
@@ -347,14 +353,15 @@
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
@@ -388,14 +395,15 @@
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

### Comparing `mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/literals.pyi` & `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -111,24 +111,26 @@
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
@@ -214,14 +216,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -236,30 +239,33 @@
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
@@ -345,14 +351,15 @@
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
@@ -386,14 +393,15 @@
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

### Comparing `mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/type_defs.py` & `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,15 @@
 )
 _OptionalCreateSceneRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSceneRequestRequestTypeDef",
     {
         "description": str,
         "capabilities": Sequence[str],
         "tags": Mapping[str, str],
+        "sceneMetadata": Mapping[str, str],
     },
     total=False,
 )
 
 
 class CreateSceneRequestRequestTypeDef(
     _RequiredCreateSceneRequestRequestTypeDef, _OptionalCreateSceneRequestRequestTypeDef
@@ -825,14 +826,15 @@
 )
 _OptionalUpdateSceneRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSceneRequestRequestTypeDef",
     {
         "contentLocation": str,
         "description": str,
         "capabilities": Sequence[str],
+        "sceneMetadata": Mapping[str, str],
     },
     total=False,
 )
 
 
 class UpdateSceneRequestRequestTypeDef(
     _RequiredUpdateSceneRequestRequestTypeDef, _OptionalUpdateSceneRequestRequestTypeDef
@@ -942,14 +944,16 @@
         "sceneId": str,
         "contentLocation": str,
         "arn": str,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "description": str,
         "capabilities": List[str],
+        "sceneMetadata": Dict[str, str],
+        "generatedSceneMetadata": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkspaceResponseTypeDef = TypedDict(
     "GetWorkspaceResponseTypeDef",
     {
```

### Comparing `mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker/type_defs.pyi` & `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -251,14 +251,15 @@
 )
 _OptionalCreateSceneRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSceneRequestRequestTypeDef",
     {
         "description": str,
         "capabilities": Sequence[str],
         "tags": Mapping[str, str],
+        "sceneMetadata": Mapping[str, str],
     },
     total=False,
 )
 
 class CreateSceneRequestRequestTypeDef(
     _RequiredCreateSceneRequestRequestTypeDef, _OptionalCreateSceneRequestRequestTypeDef
 ):
@@ -788,14 +789,15 @@
 )
 _OptionalUpdateSceneRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSceneRequestRequestTypeDef",
     {
         "contentLocation": str,
         "description": str,
         "capabilities": Sequence[str],
+        "sceneMetadata": Mapping[str, str],
     },
     total=False,
 )
 
 class UpdateSceneRequestRequestTypeDef(
     _RequiredUpdateSceneRequestRequestTypeDef, _OptionalUpdateSceneRequestRequestTypeDef
 ):
@@ -901,14 +903,16 @@
         "sceneId": str,
         "contentLocation": str,
         "arn": str,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "description": str,
         "capabilities": List[str],
+        "sceneMetadata": Dict[str, str],
+        "generatedSceneMetadata": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkspaceResponseTypeDef = TypedDict(
     "GetWorkspaceResponseTypeDef",
     {
```

### Comparing `mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker.egg-info/PKG-INFO` & `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iottwinmaker
-Version: 1.26.26
-Summary: Type annotations for boto3.IoTTwinMaker 1.26.26 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.97
+Summary: Type annotations for boto3.IoTTwinMaker 1.26.97 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iottwinmaker?color=blue)](https://pypistats.org/packages/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.26.26](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.26.97](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iottwinmaker-1.26.26/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt` & `mypy-boto3-iottwinmaker-1.26.97/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.26.26/setup.py` & `mypy-boto3-iottwinmaker-1.26.97/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-iottwinmaker",
-    version="1.26.26",
+    version="1.26.97",
     packages=["mypy_boto3_iottwinmaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTTwinMaker 1.26.26 service generated with mypy-boto3-builder"
-        " 7.12.0"
+        "Type annotations for boto3.IoTTwinMaker 1.26.97 service generated with mypy-boto3-builder"
+        " 7.13.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

