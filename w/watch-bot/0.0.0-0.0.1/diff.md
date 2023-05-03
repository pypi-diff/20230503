# Comparing `tmp/watch-bot-0.0.0.tar.gz` & `tmp/watch-bot-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watch-bot-0.0.0.tar", last modified: Wed May  3 16:37:18 2023, max compression
+gzip compressed data, was "watch-bot-0.0.1.tar", last modified: Wed May  3 16:42:33 2023, max compression
```

## Comparing `watch-bot-0.0.0.tar` & `watch-bot-0.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:37:18.960168 watch-bot-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:37:18.956168 watch-bot-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:37:18.956168 watch-bot-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-03 16:36:52.000000 watch-bot-0.0.0/.github/workflows/actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-03 16:36:52.000000 watch-bot-0.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-03 16:36:52.000000 watch-bot-0.0.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:37:18.956168 watch-bot-0.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-03 16:36:52.000000 watch-bot-0.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-03 16:36:52.000000 watch-bot-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:36:52.000000 watch-bot-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-03 16:37:18.960168 watch-bot-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-03 16:36:52.000000 watch-bot-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-03 16:36:52.000000 watch-bot-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 16:36:52.000000 watch-bot-0.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:37:18.960168 watch-bot-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:37:18.956168 watch-bot-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:37:18.956168 watch-bot-0.0.0/src/watch_bot/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 16:36:52.000000 watch-bot-0.0.0/src/watch_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-03 16:36:52.000000 watch-bot-0.0.0/src/watch_bot/_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-03 16:36:52.000000 watch-bot-0.0.0/src/watch_bot/_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-03 16:36:52.000000 watch-bot-0.0.0/src/watch_bot/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-03 16:36:52.000000 watch-bot-0.0.0/src/watch_bot/prompt.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:37:18.956168 watch-bot-0.0.0/src/watch_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-03 16:37:18.000000 watch-bot-0.0.0/src/watch_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-03 16:37:18.000000 watch-bot-0.0.0/src/watch_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:37:18.000000 watch-bot-0.0.0/src/watch_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 16:37:18.000000 watch-bot-0.0.0/src/watch_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 16:37:18.000000 watch-bot-0.0.0/src/watch_bot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:37:18.960168 watch-bot-0.0.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:37:18.960168 watch-bot-0.0.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-03 16:36:52.000000 watch-bot-0.0.0/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-03 16:36:52.000000 watch-bot-0.0.0/test/data/hack_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-03 16:36:52.000000 watch-bot-0.0.0/test/data/hack_prompt_answer.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-03 16:36:52.000000 watch-bot-0.0.0/test/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-03 16:36:52.000000 watch-bot-0.0.0/test/test_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-03 16:36:52.000000 watch-bot-0.0.0/test/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:42:33.533211 watch-bot-0.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:42:33.529211 watch-bot-0.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:42:33.529211 watch-bot-0.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-03 16:42:10.000000 watch-bot-0.0.1/.github/workflows/actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-03 16:42:10.000000 watch-bot-0.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-03 16:42:10.000000 watch-bot-0.0.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:42:33.529211 watch-bot-0.0.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-03 16:42:10.000000 watch-bot-0.0.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-03 16:42:10.000000 watch-bot-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:42:10.000000 watch-bot-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-03 16:42:33.533211 watch-bot-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-03 16:42:10.000000 watch-bot-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-03 16:42:10.000000 watch-bot-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 16:42:10.000000 watch-bot-0.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:42:33.533211 watch-bot-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:42:33.529211 watch-bot-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:42:33.533211 watch-bot-0.0.1/src/watch_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 16:42:10.000000 watch-bot-0.0.1/src/watch_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-03 16:42:10.000000 watch-bot-0.0.1/src/watch_bot/_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-03 16:42:10.000000 watch-bot-0.0.1/src/watch_bot/_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-03 16:42:10.000000 watch-bot-0.0.1/src/watch_bot/_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-03 16:42:10.000000 watch-bot-0.0.1/src/watch_bot/prompt.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:42:33.533211 watch-bot-0.0.1/src/watch_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-03 16:42:33.000000 watch-bot-0.0.1/src/watch_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-03 16:42:33.000000 watch-bot-0.0.1/src/watch_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:42:33.000000 watch-bot-0.0.1/src/watch_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 16:42:33.000000 watch-bot-0.0.1/src/watch_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 16:42:33.000000 watch-bot-0.0.1/src/watch_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:42:33.533211 watch-bot-0.0.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:42:33.533211 watch-bot-0.0.1/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-03 16:42:10.000000 watch-bot-0.0.1/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-03 16:42:10.000000 watch-bot-0.0.1/test/data/hack_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-03 16:42:10.000000 watch-bot-0.0.1/test/data/hack_prompt_answer.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-03 16:42:10.000000 watch-bot-0.0.1/test/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-03 16:42:10.000000 watch-bot-0.0.1/test/test_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-03 16:42:10.000000 watch-bot-0.0.1/test/test_response.py
```

### Comparing `watch-bot-0.0.0/.github/workflows/actions.yml` & `watch-bot-0.0.1/.github/workflows/actions.yml`

 * *Files 2% similar despite different names*

```diff
@@ -85,11 +85,9 @@
     - name: Prepare release 🙆‍♂️📦
       run: |
         python -m venv venv || . venv/bin/activate
         pip install -U pip wheel setuptools build twine
     - name: Build 🛠️📦
       run: |
         python -m build
-        ls
-        ls dist/
     - name: Release 📦🚀
       uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `watch-bot-0.0.0/.pre-commit-config.yaml` & `watch-bot-0.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `watch-bot-0.0.0/LICENSE` & `watch-bot-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `watch-bot-0.0.0/PKG-INFO` & `watch-bot-0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watch-bot
-Version: 0.0.0
+Version: 0.0.1
 Summary: Implementation of the watchbot, to control the behaviour of a LLM-based chatbot
 Author-email: Francesco Calcavecchia <francesco086@gmail.com>
 Maintainer-email: Francesco Calcavecchia <francesco086@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 This python projects implements the idea of a watchbot introduced in [this medium article](https://medium.com/@francesco.calcavecchia/control-the-behaviour-of-gpt-friends-a-novel-and-promising-approach-based-on-a-watchbot-5cd6f63c47e8).
 
 ## Quickstart
 
 ### Installation
 
 ```sh
-pip install git+https://github.com/francesco086/watchbot
+pip install watch-bot
 ```
 
 ### Usage
 
 Currently the watchbot is built on OpenAI's GPT. You therefore need a valid OpenAI API key (Azure OpenAI works too).
 Setup the credentials:
 ```py
```

### Comparing `watch-bot-0.0.0/README.md` & `watch-bot-0.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This python projects implements the idea of a watchbot introduced in [this medium article](https://medium.com/@francesco.calcavecchia/control-the-behaviour-of-gpt-friends-a-novel-and-promising-approach-based-on-a-watchbot-5cd6f63c47e8).
 
 ## Quickstart
 
 ### Installation
 
 ```sh
-pip install git+https://github.com/francesco086/watchbot
+pip install watch-bot
 ```
 
 ### Usage
 
 Currently the watchbot is built on OpenAI's GPT. You therefore need a valid OpenAI API key (Azure OpenAI works too).
 Setup the credentials:
 ```py
```

### Comparing `watch-bot-0.0.0/pyproject.toml` & `watch-bot-0.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `watch-bot-0.0.0/src/watch_bot/_bot.py` & `watch-bot-0.0.1/src/watch_bot/_bot.py`

 * *Files identical despite different names*

### Comparing `watch-bot-0.0.0/src/watch_bot/_dialog.py` & `watch-bot-0.0.1/src/watch_bot/_dialog.py`

 * *Files identical despite different names*

### Comparing `watch-bot-0.0.0/src/watch_bot/prompt.template` & `watch-bot-0.0.1/src/watch_bot/prompt.template`

 * *Files identical despite different names*

### Comparing `watch-bot-0.0.0/src/watch_bot.egg-info/PKG-INFO` & `watch-bot-0.0.1/src/watch_bot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watch-bot
-Version: 0.0.0
+Version: 0.0.1
 Summary: Implementation of the watchbot, to control the behaviour of a LLM-based chatbot
 Author-email: Francesco Calcavecchia <francesco086@gmail.com>
 Maintainer-email: Francesco Calcavecchia <francesco086@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 This python projects implements the idea of a watchbot introduced in [this medium article](https://medium.com/@francesco.calcavecchia/control-the-behaviour-of-gpt-friends-a-novel-and-promising-approach-based-on-a-watchbot-5cd6f63c47e8).
 
 ## Quickstart
 
 ### Installation
 
 ```sh
-pip install git+https://github.com/francesco086/watchbot
+pip install watch-bot
 ```
 
 ### Usage
 
 Currently the watchbot is built on OpenAI's GPT. You therefore need a valid OpenAI API key (Azure OpenAI works too).
 Setup the credentials:
 ```py
```

### Comparing `watch-bot-0.0.0/src/watch_bot.egg-info/SOURCES.txt` & `watch-bot-0.0.1/src/watch_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `watch-bot-0.0.0/test/data/hack_prompt.txt` & `watch-bot-0.0.1/test/data/hack_prompt.txt`

 * *Files identical despite different names*

### Comparing `watch-bot-0.0.0/test/test_bot.py` & `watch-bot-0.0.1/test/test_bot.py`

 * *Files identical despite different names*

### Comparing `watch-bot-0.0.0/test/test_dialog.py` & `watch-bot-0.0.1/test/test_dialog.py`

 * *Files identical despite different names*

