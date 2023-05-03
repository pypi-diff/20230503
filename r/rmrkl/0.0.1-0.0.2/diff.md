# Comparing `tmp/rmrkl-0.0.1.tar.gz` & `tmp/rmrkl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmrkl-0.0.1.tar", last modified: Wed Apr 26 15:11:30 2023, max compression
+gzip compressed data, was "rmrkl-0.0.2.tar", last modified: Wed May  3 06:36:03 2023, max compression
```

## Comparing `rmrkl-0.0.1.tar` & `rmrkl-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:11:30.916170 rmrkl-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 15:10:42.000000 rmrkl-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-26 15:11:30.916170 rmrkl-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-26 15:10:42.000000 rmrkl-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:11:30.916170 rmrkl-0.0.1/rmrkl/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 15:10:42.000000 rmrkl-0.0.1/rmrkl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-26 15:10:42.000000 rmrkl-0.0.1/rmrkl/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-26 15:10:42.000000 rmrkl-0.0.1/rmrkl/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-26 15:10:42.000000 rmrkl-0.0.1/rmrkl/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 15:10:42.000000 rmrkl-0.0.1/rmrkl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:11:30.916170 rmrkl-0.0.1/rmrkl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-26 15:11:30.000000 rmrkl-0.0.1/rmrkl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-26 15:11:30.000000 rmrkl-0.0.1/rmrkl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:11:30.000000 rmrkl-0.0.1/rmrkl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 15:11:30.000000 rmrkl-0.0.1/rmrkl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 15:11:30.000000 rmrkl-0.0.1/rmrkl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:11:30.916170 rmrkl-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-26 15:10:42.000000 rmrkl-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:11:30.916170 rmrkl-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-26 15:10:42.000000 rmrkl-0.0.1/tests/test_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:36:03.724211 rmrkl-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 06:35:31.000000 rmrkl-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-03 06:36:03.724211 rmrkl-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-03 06:35:31.000000 rmrkl-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:36:03.720211 rmrkl-0.0.2/rmrkl/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 06:35:31.000000 rmrkl-0.0.2/rmrkl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-03 06:35:31.000000 rmrkl-0.0.2/rmrkl/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-03 06:35:31.000000 rmrkl-0.0.2/rmrkl/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-03 06:35:31.000000 rmrkl-0.0.2/rmrkl/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 06:35:31.000000 rmrkl-0.0.2/rmrkl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:36:03.724211 rmrkl-0.0.2/rmrkl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-03 06:36:03.000000 rmrkl-0.0.2/rmrkl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-03 06:36:03.000000 rmrkl-0.0.2/rmrkl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:36:03.000000 rmrkl-0.0.2/rmrkl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 06:36:03.000000 rmrkl-0.0.2/rmrkl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 06:36:03.000000 rmrkl-0.0.2/rmrkl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 06:36:03.724211 rmrkl-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-03 06:35:31.000000 rmrkl-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:36:03.724211 rmrkl-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-03 06:35:31.000000 rmrkl-0.0.2/tests/test_agent.py
```

### Comparing `rmrkl-0.0.1/LICENSE` & `rmrkl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rmrkl-0.0.1/PKG-INFO` & `rmrkl-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmrkl
-Version: 0.0.1
+Version: 0.0.2
 Summary: Robust Modular Reasoning, Knowledge and Language agent that uses tools and retries on failure
 Home-page: https://github.com/whitead/robust-mrkl
 Author: Andrew White
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rmrkl-0.0.1/rmrkl/agent.py` & `rmrkl-0.0.2/rmrkl/agent.py`

 * *Files identical despite different names*

### Comparing `rmrkl-0.0.1/rmrkl/prompts.py` & `rmrkl-0.0.2/rmrkl/prompts.py`

 * *Files identical despite different names*

### Comparing `rmrkl-0.0.1/rmrkl.egg-info/PKG-INFO` & `rmrkl-0.0.2/rmrkl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmrkl
-Version: 0.0.1
+Version: 0.0.2
 Summary: Robust Modular Reasoning, Knowledge and Language agent that uses tools and retries on failure
 Home-page: https://github.com/whitead/robust-mrkl
 Author: Andrew White
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rmrkl-0.0.1/setup.py` & `rmrkl-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     version=__version__,
     description="Robust Modular Reasoning, Knowledge and Language agent that uses tools and retries on failure",
     author="Andrew White",
     author_email="andrew.white@rochester.edu",
     url="https://github.com/whitead/robust-mrkl",
     license="MIT",
     packages=["rmrkl"],
-    install_requires=["langchain>=0.0.147"],
+    install_requires=["langchain>=0.0.157"],
     test_suite="tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ],
```

### Comparing `rmrkl-0.0.1/tests/test_agent.py` & `rmrkl-0.0.2/tests/test_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from rmrkl import ChatZeroShotAgent, RetryAgentExecutor
 from langchain.llms.fake import FakeListLLM
 from langchain.agents import load_tools
 
 
 def test_agent_init():
-    tools = load_tools(["python_repl"])
+    tools = load_tools(["terminal"])
     responses = [
         "I should use the REPL tool",
         "Action: Python REPL\nAction Input: print(2 + 2)",
         "Final Answer: 4",
     ]
     llm = FakeListLLM(responses=responses)
```

