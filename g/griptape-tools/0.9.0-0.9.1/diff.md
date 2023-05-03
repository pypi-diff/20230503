# Comparing `tmp/griptape_tools-0.9.0.tar.gz` & `tmp/griptape_tools-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_tools-0.9.0.tar", max compression
+gzip compressed data, was "griptape_tools-0.9.1.tar", max compression
```

## Comparing `griptape_tools-0.9.0.tar` & `griptape_tools-0.9.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.9.0/LICENSE
--rw-r--r--   0        0        0     1151 2023-04-24 20:05:55.932841 griptape_tools-0.9.0/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.9.0/griptape/__init__.py
--rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.9.0/griptape/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.9.0/griptape/tools/aws_cli/__init__.py
--rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.9.0/griptape/tools/aws_cli/manifest.yml
--rw-r--r--   0        0        0       73 2023-04-30 21:00:51.923653 griptape_tools-0.9.0/griptape/tools/aws_cli/requirements.txt
--rw-r--r--   0        0        0     1745 2023-04-30 21:02:58.677825 griptape_tools-0.9.0/griptape/tools/aws_cli/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.9.0/griptape/tools/calculator/__init__.py
--rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.9.0/griptape/tools/calculator/manifest.yml
--rw-r--r--   0        0        0       16 2023-04-30 21:00:51.922811 griptape_tools-0.9.0/griptape/tools/calculator/requirements.txt
--rw-r--r--   0        0        0      816 2023-04-30 19:49:57.299564 griptape_tools-0.9.0/griptape/tools/calculator/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.9.0/griptape/tools/email_client/__init__.py
--rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.9.0/griptape/tools/email_client/manifest.yml
--rw-r--r--   0        0        0       16 2023-04-30 21:00:51.918672 griptape_tools-0.9.0/griptape/tools/email_client/requirements.txt
--rw-r--r--   0        0        0     6041 2023-04-30 19:49:57.293290 griptape_tools-0.9.0/griptape/tools/email_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.9.0/griptape/tools/sql_client/__init__.py
--rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.9.0/griptape/tools/sql_client/manifest.yml
--rw-r--r--   0        0        0       28 2023-04-30 21:00:51.919938 griptape_tools-0.9.0/griptape/tools/sql_client/requirements.txt
--rw-r--r--   0        0        0     1413 2023-04-30 19:49:57.297074 griptape_tools-0.9.0/griptape/tools/sql_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.9.0/griptape/tools/web_scraper/__init__.py
--rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.9.0/griptape/tools/web_scraper/manifest.yml
--rw-r--r--   0        0        0       28 2023-04-30 21:00:51.920950 griptape_tools-0.9.0/griptape/tools/web_scraper/requirements.txt
--rw-r--r--   0        0        0     2890 2023-04-30 19:49:57.304804 griptape_tools-0.9.0/griptape/tools/web_scraper/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.9.0/griptape/tools/web_search/__init__.py
--rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.9.0/griptape/tools/web_search/manifest.yml
--rw-r--r--   0        0        0       24 2023-04-30 21:00:51.921786 griptape_tools-0.9.0/griptape/tools/web_search/requirements.txt
--rw-r--r--   0        0        0     2323 2023-04-30 19:49:57.307290 griptape_tools-0.9.0/griptape/tools/web_search/tool.py
--rw-r--r--   0        0        0      520 2023-04-30 21:07:32.928296 griptape_tools-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 griptape_tools-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1151 2023-04-24 20:05:55.932841 griptape_tools-0.9.1/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.9.1/griptape/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.9.1/griptape/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.9.1/griptape/tools/aws_cli/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.9.1/griptape/tools/aws_cli/manifest.yml
+-rw-r--r--   0        0        0       73 2023-05-03 17:35:47.045678 griptape_tools-0.9.1/griptape/tools/aws_cli/requirements.txt
+-rw-r--r--   0        0        0     1780 2023-05-03 17:18:05.788226 griptape_tools-0.9.1/griptape/tools/aws_cli/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.9.1/griptape/tools/calculator/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.9.1/griptape/tools/calculator/manifest.yml
+-rw-r--r--   0        0        0       16 2023-05-03 17:35:47.047062 griptape_tools-0.9.1/griptape/tools/calculator/requirements.txt
+-rw-r--r--   0        0        0      816 2023-04-30 19:49:57.299564 griptape_tools-0.9.1/griptape/tools/calculator/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.9.1/griptape/tools/email_client/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.9.1/griptape/tools/email_client/manifest.yml
+-rw-r--r--   0        0        0       16 2023-05-03 17:35:47.048425 griptape_tools-0.9.1/griptape/tools/email_client/requirements.txt
+-rw-r--r--   0        0        0     6041 2023-04-30 19:49:57.293290 griptape_tools-0.9.1/griptape/tools/email_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.9.1/griptape/tools/sql_client/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.9.1/griptape/tools/sql_client/manifest.yml
+-rw-r--r--   0        0        0       28 2023-05-03 17:35:47.036400 griptape_tools-0.9.1/griptape/tools/sql_client/requirements.txt
+-rw-r--r--   0        0        0     1413 2023-04-30 19:49:57.297074 griptape_tools-0.9.1/griptape/tools/sql_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.9.1/griptape/tools/web_scraper/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.9.1/griptape/tools/web_scraper/manifest.yml
+-rw-r--r--   0        0        0       28 2023-05-03 17:35:47.038379 griptape_tools-0.9.1/griptape/tools/web_scraper/requirements.txt
+-rw-r--r--   0        0        0     2890 2023-04-30 19:49:57.304804 griptape_tools-0.9.1/griptape/tools/web_scraper/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.9.1/griptape/tools/web_search/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.9.1/griptape/tools/web_search/manifest.yml
+-rw-r--r--   0        0        0       24 2023-05-03 17:35:47.049925 griptape_tools-0.9.1/griptape/tools/web_search/requirements.txt
+-rw-r--r--   0        0        0     2323 2023-04-30 19:49:57.307290 griptape_tools-0.9.1/griptape/tools/web_search/tool.py
+-rw-r--r--   0        0        0      520 2023-05-03 17:37:10.633859 griptape_tools-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 griptape_tools-0.9.1/PKG-INFO
```

### Comparing `griptape_tools-0.9.0/LICENSE` & `griptape_tools-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.9.0/README.md` & `griptape_tools-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.9.0/griptape/tools/aws_cli/tool.py` & `griptape_tools-0.9.1/griptape/tools/aws_cli/tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-import json
 from typing import Optional
 from griptape.artifacts import BaseArtifact, TextArtifact, ErrorArtifact
 from schema import Schema
 from griptape.core import BaseTool
 from griptape.core.decorators import activity
 from griptape import utils
 from attr import define, field
 
 
 @define
 class AwsCli(BaseTool):
     aws_access_key_id: Optional[str] = field(default=None, kw_only=True, metadata={"env": "AWS_ACCESS_KEY_ID"})
     aws_secret_access_key: Optional[str] = field(default=None, kw_only=True, metadata={"env": "AWS_SECRET_ACCESS_KEY"})
     aws_default_region: str = field(default="us-east-1", kw_only=True, metadata={"env": "AWS_DEFAULT_REGION"})
-    aws_cli_policy: Optional[str] = field(default=None, kw_only=True, metadata={"env": "AWS_CLI_POLICY"})
+    aws_cli_policy: str = field(
+        default="""{"Version":"2012-10-17","Statement":[{"Effect":"Allow","Action":"*","Resource":"*"}]}""",
+        kw_only=True
+    )
 
     @property
     def schema_template_args(self) -> dict:
         return {
-            "policy": json.dumps(utils.minify_json(self.env_value("AWS_CLI_POLICY"))).strip('"')
+            "policy": utils.minify_json(self.aws_cli_policy)
         }
 
     @activity(config={
         "name": "execute",
         "description": "Can be used to execute AWS CLI v2 commands limited by this policy: {{ policy }}",
         "schema": Schema(
             str,
-            description="AWS CLI v2 command"
+            description="AWS CLI v2 command starting with 'aws'"
         )
     })
     def execute(self, value: str) -> BaseArtifact:
         result = utils.CommandRunner().run(f"AWS_PAGER='' {value} --output json")
 
         if isinstance(result, ErrorArtifact):
             return result
```

### Comparing `griptape_tools-0.9.0/griptape/tools/calculator/tool.py` & `griptape_tools-0.9.1/griptape/tools/calculator/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.9.0/griptape/tools/email_client/tool.py` & `griptape_tools-0.9.1/griptape/tools/email_client/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.9.0/griptape/tools/sql_client/tool.py` & `griptape_tools-0.9.1/griptape/tools/sql_client/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.9.0/griptape/tools/web_scraper/tool.py` & `griptape_tools-0.9.1/griptape/tools/web_scraper/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.9.0/griptape/tools/web_search/tool.py` & `griptape_tools-0.9.1/griptape/tools/web_search/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.9.0/pyproject.toml` & `griptape_tools-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "griptape-tools"
-version = "0.9.0"
+version = "0.9.1"
 description = "Tools for the griptape-core package."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-tools"
 
 packages = [
     {include = "griptape"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-griptape = ">=0.7.1"
+griptape = ">=0.7.2"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-mock = "*"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `griptape_tools-0.9.0/PKG-INFO` & `griptape_tools-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: griptape-tools
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tools for the griptape-core package.
 Home-page: https://github.com/griptape-ai/griptape-tools
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: griptape (>=0.7.1)
+Requires-Dist: griptape (>=0.7.2)
 Project-URL: Repository, https://github.com/griptape-ai/griptape-tools
 Description-Content-Type: text/markdown
 
 # griptape-tools
 
 [![PyPI Version](https://img.shields.io/pypi/v/griptape-tools.svg)](https://pypi.python.org/pypi/griptape-tools)
 [![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
```

