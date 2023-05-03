# Comparing `tmp/semterm-0.2.0.tar.gz` & `tmp/semterm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semterm-0.2.0.tar", last modified: Tue May  2 05:58:02 2023, max compression
+gzip compressed data, was "semterm-0.2.1.tar", last modified: Wed May  3 03:11:23 2023, max compression
```

## Comparing `semterm-0.2.0.tar` & `semterm-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.837864 semterm-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 05:57:42.000000 semterm-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 05:57:42.000000 semterm-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 05:58:02.837864 semterm-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-02 05:57:42.000000 semterm-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-02 05:57:42.000000 semterm-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.833863 semterm-0.2.0/semterm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.833863 semterm-0.2.0/semterm/UI/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/UI/UserInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/UI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.837864 semterm-0.2.0/semterm/agent/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/agent/MrklAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/agent/TerminalAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/agent/TerminalAgentExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/agent/TerminalAgentPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.837864 semterm-0.2.0/semterm/config/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/config/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.837864 semterm-0.2.0/semterm/langchain_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/langchain_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/langchain_extensions/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/langchain_extensions/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.837864 semterm-0.2.0/semterm/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/terminal/SemanticTerminalManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/terminal/SemanticTerminalProcess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/terminal/TerminalOutputParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/terminal/TerminalTool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:57:42.000000 semterm-0.2.0/semterm/terminal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:58:02.833863 semterm-0.2.0/semterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 05:58:02.000000 semterm-0.2.0/semterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 05:58:02.000000 semterm-0.2.0/semterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:58:02.000000 semterm-0.2.0/semterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 05:58:02.000000 semterm-0.2.0/semterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 05:58:02.000000 semterm-0.2.0/semterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 05:58:02.000000 semterm-0.2.0/semterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:58:02.837864 semterm-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-02 05:57:42.000000 semterm-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.883560 semterm-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-03 03:10:59.000000 semterm-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-03 03:10:59.000000 semterm-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 03:11:23.883560 semterm-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-03 03:10:59.000000 semterm-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-03 03:10:59.000000 semterm-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.879560 semterm-0.2.1/semterm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.879560 semterm-0.2.1/semterm/UI/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/UI/UserInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/UI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.879560 semterm-0.2.1/semterm/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/agent/MrklAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/agent/TerminalAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/agent/TerminalAgentExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/agent/TerminalAgentPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.879560 semterm-0.2.1/semterm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/config/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.883560 semterm-0.2.1/semterm/langchain_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/langchain_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/langchain_extensions/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/langchain_extensions/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.883560 semterm-0.2.1/semterm/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/terminal/SemanticTerminalManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/terminal/SemanticTerminalProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/terminal/TerminalOutputParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/terminal/TerminalTool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:10:59.000000 semterm-0.2.1/semterm/terminal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:11:23.879560 semterm-0.2.1/semterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 03:11:23.000000 semterm-0.2.1/semterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-03 03:11:23.000000 semterm-0.2.1/semterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 03:11:23.000000 semterm-0.2.1/semterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 03:11:23.000000 semterm-0.2.1/semterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 03:11:23.000000 semterm-0.2.1/semterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 03:11:23.000000 semterm-0.2.1/semterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 03:11:23.883560 semterm-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-03 03:10:59.000000 semterm-0.2.1/setup.py
```

### Comparing `semterm-0.2.0/LICENSE` & `semterm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `semterm-0.2.0/README.md` & `semterm-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # SemTerm: The Semantic Terminal 🚀
 
-SemTerm is a revolutionary Semantic Terminal that leverages the power of Large Language Models to perform complex tasks with a simple, human speech-like command. With SemTerm, you can spin up Django projects, run servers, and much more, all with a simple, intuitive instruction. SemTerm offers a futuristic command-line experience currently available only for Linux and MacOS users.
+SemTerm is a groundbreaking command-line tool that harnesses the capabilities of Large Language Models to execute complex tasks using natural, conversational input.
+With SemTerm, you can run complex bash commands with a simple, intuitive instruction. 
+
+SemTerm offers a futuristic command-line experience currently available only for Linux and MacOS users.
 
 You can ask it things like
 ```bash
 You > How large is this directory?
 semterm > du -sh
 146M    .
 semterm >  The size of the current directory is 146M.
 ```
 
 And pretty much anything else you can think of. You are only limited by your imagination. 💭
 
+Join our [Discord](https://discord.gg/TQSbWnck) to discuss SemTerm and help out with development!
+
 ## Table of Contents 📚
 
 1. [Features](#features)
 2. [Requirements](#requirements)
 3. [Installation](#installation)
 4. [Usage](#usage)
 5. [Ideas for Future Development](#ideas-for-future-development)
```

### Comparing `semterm-0.2.0/semterm/agent/MrklAgent.py` & `semterm-0.2.1/semterm/agent/MrklAgent.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.0/semterm/agent/TerminalAgent.py` & `semterm-0.2.1/semterm/agent/TerminalAgent.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.0/semterm/agent/TerminalAgentExecutor.py` & `semterm-0.2.1/semterm/agent/TerminalAgentExecutor.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.0/semterm/agent/TerminalAgentPrompt.py` & `semterm-0.2.1/semterm/agent/TerminalAgentPrompt.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.0/semterm/langchain_extensions/tools.py` & `semterm-0.2.1/semterm/langchain_extensions/tools.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.0/semterm/terminal/SemanticTerminalManager.py` & `semterm-0.2.1/semterm/terminal/SemanticTerminalManager.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.0/semterm/terminal/SemanticTerminalProcess.py` & `semterm-0.2.1/semterm/terminal/SemanticTerminalProcess.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.0/semterm/terminal/TerminalOutputParser.py` & `semterm-0.2.1/semterm/terminal/TerminalOutputParser.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.0/semterm/terminal/TerminalTool.py` & `semterm-0.2.1/semterm/terminal/TerminalTool.py`

 * *Files identical despite different names*

### Comparing `semterm-0.2.0/semterm.egg-info/SOURCES.txt` & `semterm-0.2.1/semterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `semterm-0.2.0/setup.py` & `semterm-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="semterm",
-    version="0.2.0",
+    version="0.2.1",
     description="The Semantic Terminal",
     long_description="The Semantic Terminal",
     author="Lambrou",
     author_email="alexanderlambrou0602@gmail.com",
     packages=find_packages(),
     include_package_data=True,
     entry_points={
```

