# Comparing `tmp/staircase_kit-0.1.8.tar.gz` & `tmp/staircase_kit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staircase_kit-0.1.8.tar", max compression
+gzip compressed data, was "staircase_kit-0.1.9.tar", max compression
```

## Comparing `staircase_kit-0.1.8.tar` & `staircase_kit-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      685 2023-02-20 11:58:59.374866 staircase_kit-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1248 2023-02-20 06:39:56.176090 staircase_kit-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-02-08 15:44:20.252000 staircase_kit-0.1.8/staircase/__init__.py
--rw-r--r--   0        0        0      936 2023-02-20 11:58:50.123576 staircase_kit-0.1.8/staircase/cli.py
--rw-r--r--   0        0        0     2046 2023-02-19 19:54:51.666827 staircase_kit-0.1.8/staircase/command_providers.py
--rw-r--r--   0        0        0        0 2023-02-08 15:44:20.267000 staircase_kit-0.1.8/staircase/commands/__init__.py
--rw-r--r--   0        0        0     6998 2023-02-19 22:32:15.546384 staircase_kit-0.1.8/staircase/commands/ci.py
--rw-r--r--   0        0        0      188 2023-02-16 11:32:12.474599 staircase_kit-0.1.8/staircase/commands/config/__init__.py
--rw-r--r--   0        0        0      227 2023-02-19 20:16:03.712298 staircase_kit-0.1.8/staircase/commands/config/file_path.py
--rw-r--r--   0        0        0      674 2023-02-19 21:02:33.666346 staircase_kit-0.1.8/staircase/commands/config/setup.py
--rw-r--r--   0        0        0      300 2023-02-16 15:32:32.535779 staircase_kit-0.1.8/staircase/commands/envs/__init__.py
--rw-r--r--   0        0        0      566 2023-02-19 20:14:48.909933 staircase_kit-0.1.8/staircase/commands/envs/add.py
--rw-r--r--   0        0        0      461 2023-02-19 20:14:24.169096 staircase_kit-0.1.8/staircase/commands/envs/list.py
--rw-r--r--   0        0        0      678 2023-02-19 20:15:10.056144 staircase_kit-0.1.8/staircase/commands/envs/remove.py
--rw-r--r--   0        0        0      144 2023-02-08 15:44:20.305000 staircase_kit-0.1.8/staircase/commands/postman/__init__.py
--rw-r--r--   0        0        0      174 2023-02-08 15:44:20.310000 staircase_kit-0.1.8/staircase/commands/postman/import_/__init__.py
--rw-r--r--   0        0        0     4084 2023-02-19 20:13:14.734470 staircase_kit-0.1.8/staircase/commands/postman/import_/api.py
--rw-r--r--   0        0        0     2375 2023-02-19 20:13:58.496221 staircase_kit-0.1.8/staircase/commands/postman/import_/envs.py
--rw-r--r--   0        0        0     1024 2023-02-20 11:57:13.426801 staircase_kit-0.1.8/staircase/config.py
--rw-r--r--   0        0        0      616 2023-02-19 20:10:55.890068 staircase_kit-0.1.8/staircase/env_manager.py
--rw-r--r--   0        0        0     1651 2023-02-19 19:41:52.720775 staircase_kit-0.1.8/staircase/env_storage.py
--rw-r--r--   0        0        0        0 2023-02-08 15:44:20.333000 staircase_kit-0.1.8/staircase/lib/__init__.py
--rw-r--r--   0        0        0      193 2023-02-08 15:44:20.339000 staircase_kit-0.1.8/staircase/lib/click.py
--rw-r--r--   0        0        0     1277 2023-02-16 21:22:05.924245 staircase_kit-0.1.8/staircase/lib/fzf.py
--rw-r--r--   0        0        0      454 2023-02-08 15:44:20.346000 staircase_kit-0.1.8/staircase/lib/postman_http_client.py
--rw-r--r--   0        0        0       47 2023-02-16 11:24:08.065258 staircase_kit-0.1.8/staircase/lib/sdk/__init__.py
--rw-r--r--   0        0        0      138 2023-02-16 11:32:12.477106 staircase_kit-0.1.8/staircase/lib/sdk/ci/__init__.py
--rw-r--r--   0        0        0      755 2023-02-08 15:44:20.364000 staircase_kit-0.1.8/staircase/lib/sdk/ci/assess.py
--rw-r--r--   0        0        0      945 2023-02-16 11:32:12.478107 staircase_kit-0.1.8/staircase/lib/sdk/ci/build.py
--rw-r--r--   0        0        0     1155 2023-02-16 11:32:12.478107 staircase_kit-0.1.8/staircase/lib/sdk/ci/clone.py
--rw-r--r--   0        0        0     1637 2023-02-16 11:32:12.478107 staircase_kit-0.1.8/staircase/lib/sdk/ci/deploy.py
--rw-r--r--   0        0        0      511 2023-02-08 15:44:20.382000 staircase_kit-0.1.8/staircase/lib/sdk/ci/test.py
--rw-r--r--   0        0        0      362 2023-02-16 11:32:12.478107 staircase_kit-0.1.8/staircase/lib/sdk/staircase_env.py
--rw-r--r--   0        0        0     1664 2023-02-16 11:32:12.478107 staircase_kit-0.1.8/staircase/lib/sdk/staircase_http_client.py
--rw-r--r--   0        0        0      532 2023-02-08 15:44:20.406000 staircase_kit-0.1.8/staircase/lib/shutil.py
--rw-r--r--   0        0        0      338 2023-02-08 15:44:20.411000 staircase_kit-0.1.8/staircase/logger.py
--rw-r--r--   0        0        0       56 2023-02-08 15:44:20.415000 staircase_kit-0.1.8/staircase/main.py
--rw-r--r--   0        0        0     2122 2023-02-16 22:07:52.876752 staircase_kit-0.1.8/staircase/postman.py
--rw-r--r--   0        0        0     2957 2023-02-19 19:31:33.961770 staircase_kit-0.1.8/staircase/staircase.py
--rw-r--r--   0        0        0     1081 2023-02-16 22:07:52.883752 staircase_kit-0.1.8/staircase/user_prompts.py
--rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 staircase_kit-0.1.8/setup.py
--rw-r--r--   0        0        0     1979 1970-01-01 00:00:00.000000 staircase_kit-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      685 2023-02-20 12:02:03.241543 staircase_kit-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1248 2023-02-20 06:39:56.176090 staircase_kit-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-02-08 15:44:20.252000 staircase_kit-0.1.9/staircase/__init__.py
+-rw-r--r--   0        0        0      929 2023-02-20 12:01:58.742713 staircase_kit-0.1.9/staircase/cli.py
+-rw-r--r--   0        0        0     2046 2023-02-19 19:54:51.666827 staircase_kit-0.1.9/staircase/command_providers.py
+-rw-r--r--   0        0        0        0 2023-02-08 15:44:20.267000 staircase_kit-0.1.9/staircase/commands/__init__.py
+-rw-r--r--   0        0        0     6998 2023-02-19 22:32:15.546384 staircase_kit-0.1.9/staircase/commands/ci.py
+-rw-r--r--   0        0        0      188 2023-02-16 11:32:12.474599 staircase_kit-0.1.9/staircase/commands/config/__init__.py
+-rw-r--r--   0        0        0      227 2023-02-19 20:16:03.712298 staircase_kit-0.1.9/staircase/commands/config/file_path.py
+-rw-r--r--   0        0        0      674 2023-02-19 21:02:33.666346 staircase_kit-0.1.9/staircase/commands/config/setup.py
+-rw-r--r--   0        0        0      300 2023-02-16 15:32:32.535779 staircase_kit-0.1.9/staircase/commands/envs/__init__.py
+-rw-r--r--   0        0        0      566 2023-02-19 20:14:48.909933 staircase_kit-0.1.9/staircase/commands/envs/add.py
+-rw-r--r--   0        0        0      461 2023-02-19 20:14:24.169096 staircase_kit-0.1.9/staircase/commands/envs/list.py
+-rw-r--r--   0        0        0      678 2023-02-19 20:15:10.056144 staircase_kit-0.1.9/staircase/commands/envs/remove.py
+-rw-r--r--   0        0        0      144 2023-02-08 15:44:20.305000 staircase_kit-0.1.9/staircase/commands/postman/__init__.py
+-rw-r--r--   0        0        0      174 2023-02-08 15:44:20.310000 staircase_kit-0.1.9/staircase/commands/postman/import_/__init__.py
+-rw-r--r--   0        0        0     4084 2023-02-19 20:13:14.734470 staircase_kit-0.1.9/staircase/commands/postman/import_/api.py
+-rw-r--r--   0        0        0     2375 2023-02-19 20:13:58.496221 staircase_kit-0.1.9/staircase/commands/postman/import_/envs.py
+-rw-r--r--   0        0        0     1024 2023-02-20 11:57:13.426801 staircase_kit-0.1.9/staircase/config.py
+-rw-r--r--   0        0        0      616 2023-02-19 20:10:55.890068 staircase_kit-0.1.9/staircase/env_manager.py
+-rw-r--r--   0        0        0     1651 2023-02-19 19:41:52.720775 staircase_kit-0.1.9/staircase/env_storage.py
+-rw-r--r--   0        0        0        0 2023-02-08 15:44:20.333000 staircase_kit-0.1.9/staircase/lib/__init__.py
+-rw-r--r--   0        0        0      193 2023-02-08 15:44:20.339000 staircase_kit-0.1.9/staircase/lib/click.py
+-rw-r--r--   0        0        0     1277 2023-02-16 21:22:05.924245 staircase_kit-0.1.9/staircase/lib/fzf.py
+-rw-r--r--   0        0        0      454 2023-02-08 15:44:20.346000 staircase_kit-0.1.9/staircase/lib/postman_http_client.py
+-rw-r--r--   0        0        0       47 2023-02-16 11:24:08.065258 staircase_kit-0.1.9/staircase/lib/sdk/__init__.py
+-rw-r--r--   0        0        0      138 2023-02-16 11:32:12.477106 staircase_kit-0.1.9/staircase/lib/sdk/ci/__init__.py
+-rw-r--r--   0        0        0      755 2023-02-08 15:44:20.364000 staircase_kit-0.1.9/staircase/lib/sdk/ci/assess.py
+-rw-r--r--   0        0        0      945 2023-02-16 11:32:12.478107 staircase_kit-0.1.9/staircase/lib/sdk/ci/build.py
+-rw-r--r--   0        0        0     1155 2023-02-16 11:32:12.478107 staircase_kit-0.1.9/staircase/lib/sdk/ci/clone.py
+-rw-r--r--   0        0        0     1637 2023-02-16 11:32:12.478107 staircase_kit-0.1.9/staircase/lib/sdk/ci/deploy.py
+-rw-r--r--   0        0        0      511 2023-02-08 15:44:20.382000 staircase_kit-0.1.9/staircase/lib/sdk/ci/test.py
+-rw-r--r--   0        0        0      362 2023-02-16 11:32:12.478107 staircase_kit-0.1.9/staircase/lib/sdk/staircase_env.py
+-rw-r--r--   0        0        0     1664 2023-02-16 11:32:12.478107 staircase_kit-0.1.9/staircase/lib/sdk/staircase_http_client.py
+-rw-r--r--   0        0        0      532 2023-02-08 15:44:20.406000 staircase_kit-0.1.9/staircase/lib/shutil.py
+-rw-r--r--   0        0        0      338 2023-02-08 15:44:20.411000 staircase_kit-0.1.9/staircase/logger.py
+-rw-r--r--   0        0        0       56 2023-02-08 15:44:20.415000 staircase_kit-0.1.9/staircase/main.py
+-rw-r--r--   0        0        0     2122 2023-02-16 22:07:52.876752 staircase_kit-0.1.9/staircase/postman.py
+-rw-r--r--   0        0        0     2957 2023-02-19 19:31:33.961770 staircase_kit-0.1.9/staircase/staircase.py
+-rw-r--r--   0        0        0     1081 2023-02-16 22:07:52.883752 staircase_kit-0.1.9/staircase/user_prompts.py
+-rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 staircase_kit-0.1.9/setup.py
+-rw-r--r--   0        0        0     1979 1970-01-01 00:00:00.000000 staircase_kit-0.1.9/PKG-INFO
```

### Comparing `staircase_kit-0.1.8/pyproject.toml` & `staircase_kit-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "staircase_kit"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Zik <zikunov.vladislav@staircase.co>"]
 readme = "README.md"
 packages = [{include = "staircase"}]
```

### Comparing `staircase_kit-0.1.8/README.md` & `staircase_kit-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/cli.py` & `staircase_kit-0.1.9/staircase/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import click
 
 from .config import DATA_FOLDER, VAR_FOLDER, CONFIG_FILE_PATH, get_user_cfg, write_user_cfg
 
-from 
 from .commands.postman import postman_group
 from .commands.envs import envs_group
 from .commands import config as config_
 from .commands import ci
 
 
 def get_cli():
```

### Comparing `staircase_kit-0.1.8/staircase/command_providers.py` & `staircase_kit-0.1.9/staircase/command_providers.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/commands/ci.py` & `staircase_kit-0.1.9/staircase/commands/ci.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/commands/config/setup.py` & `staircase_kit-0.1.9/staircase/commands/config/setup.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/commands/envs/add.py` & `staircase_kit-0.1.9/staircase/commands/envs/add.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/commands/envs/remove.py` & `staircase_kit-0.1.9/staircase/commands/envs/remove.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/commands/postman/import_/api.py` & `staircase_kit-0.1.9/staircase/commands/postman/import_/api.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/commands/postman/import_/envs.py` & `staircase_kit-0.1.9/staircase/commands/postman/import_/envs.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/config.py` & `staircase_kit-0.1.9/staircase/config.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/env_manager.py` & `staircase_kit-0.1.9/staircase/env_manager.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/env_storage.py` & `staircase_kit-0.1.9/staircase/env_storage.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/lib/fzf.py` & `staircase_kit-0.1.9/staircase/lib/fzf.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/lib/sdk/ci/assess.py` & `staircase_kit-0.1.9/staircase/lib/sdk/ci/assess.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/lib/sdk/ci/build.py` & `staircase_kit-0.1.9/staircase/lib/sdk/ci/build.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/lib/sdk/ci/clone.py` & `staircase_kit-0.1.9/staircase/lib/sdk/ci/clone.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/lib/sdk/ci/deploy.py` & `staircase_kit-0.1.9/staircase/lib/sdk/ci/deploy.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/lib/sdk/staircase_http_client.py` & `staircase_kit-0.1.9/staircase/lib/sdk/staircase_http_client.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/lib/shutil.py` & `staircase_kit-0.1.9/staircase/lib/shutil.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/postman.py` & `staircase_kit-0.1.9/staircase/postman.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/staircase.py` & `staircase_kit-0.1.9/staircase/staircase.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/staircase/user_prompts.py` & `staircase_kit-0.1.9/staircase/user_prompts.py`

 * *Files identical despite different names*

### Comparing `staircase_kit-0.1.8/setup.py` & `staircase_kit-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 entry_points = \
 {'console_scripts': ['sc = staircase.cli:launch_cli',
                      'staircase = staircase.cli:launch_cli']}
 
 setup_kwargs = {
     'name': 'staircase-kit',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '**Table of contents**\n- [Installation](#installation)\n  - [Requirements](#requirements)\n    - [Git token](#git-token)\n    - [Hot get Postman API Key](#hot-get-postman-api-key)\n  - [Installing](#installing)\n  - [Configuring](#configuring)\n- [How to use](#how-to-use)\n\n\n# Installation\n## Requirements\n- [`fzf`]("https://github.com/junegunn/fzf#installation")\n- `git` + be setup with Staircase by ssh key\n- [`git` token](#git-token)\n- [Postman API Key](#hot-get-postman-api-key)\n- Marketplace API key\n- `pipenv` *optional*\n\n### Git token\nUsed for clone product.\nGitHub token. Go to GitHub.com/Settings/Developer settings/Personal access token/New/Enable SSO.\nAdd checks to enable repo access.\n\n### Hot get Postman API Key\nFollow steps via app or website:\n- Click on profile pic \n- Settings \n- API keys \n- Generate API key\n  Consider verify that expiration date is okay, you are going need to renew it after.\n\n## Installing \n- Open terminal.\n- `pip install staircase-kit`\n\n## Configuring\n- Open terminal.\n- Run command `staircase config setup` or edit file `staircase config file-path`.\n\n# How to use\n- Open terminal\n- Run command `staircase` or `sc`\n- You can run `--help` to any command to get extra info.\n',
     'author': 'Zik',
     'author_email': 'zikunov.vladislav@staircase.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `staircase_kit-0.1.8/PKG-INFO` & `staircase_kit-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staircase-kit
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Zik
 Author-email: zikunov.vladislav@staircase.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

