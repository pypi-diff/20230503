# Comparing `tmp/rewards_experimental-0.0.1.tar.gz` & `tmp/rewards_experimental-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewards_experimental-0.0.1.tar", max compression
+gzip compressed data, was "rewards_experimental-0.0.2.tar", max compression
```

## Comparing `rewards_experimental-0.0.1.tar` & `rewards_experimental-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     8386 2023-04-19 10:23:39.443037 rewards_experimental-0.0.1/README.md
--rw-r--r--   0        0        0      443 2023-04-19 10:22:44.614833 rewards_experimental-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      285 2023-04-19 10:23:14.322944 rewards_experimental-0.0.1/rewards_experimental/__init__.py
--rw-r--r--   0        0        0     4231 2023-04-18 19:29:41.358005 rewards_experimental-0.0.1/rewards_experimental/agent.py
--rw-r--r--   0        0        0      766 2023-04-19 06:55:50.823332 rewards_experimental-0.0.1/rewards_experimental/config.py
--rw-r--r--   0        0        0     5299 2023-04-18 17:29:27.678654 rewards_experimental-0.0.1/rewards_experimental/models.py
--rw-r--r--   0        0        0      825 2023-04-18 20:28:11.774543 rewards_experimental-0.0.1/rewards_experimental/multiagent.py
--rw-r--r--   0        0        0     5775 2023-04-18 19:30:33.521846 rewards_experimental-0.0.1/rewards_experimental/trainer.py
--rw-r--r--   0        0        0     7778 2023-04-19 00:45:55.077662 rewards_experimental-0.0.1/rewards_experimental/utils.py
--rw-r--r--   0        0        0     3518 2023-04-19 06:58:52.780207 rewards_experimental-0.0.1/rewards_experimental/workflow.py
--rw-r--r--   0        0        0     9192 1970-01-01 00:00:00.000000 rewards_experimental-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8386 2023-04-19 10:23:39.443037 rewards_experimental-0.0.2/README.md
+-rw-r--r--   0        0        0      426 2023-05-03 06:10:17.432892 rewards_experimental-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      285 2023-04-19 10:23:14.322944 rewards_experimental-0.0.2/rewards_experimental/__init__.py
+-rw-r--r--   0        0        0     4231 2023-04-18 19:29:41.358005 rewards_experimental-0.0.2/rewards_experimental/agent.py
+-rw-r--r--   0        0        0      766 2023-04-19 06:55:50.823332 rewards_experimental-0.0.2/rewards_experimental/config.py
+-rw-r--r--   0        0        0     5299 2023-04-18 17:29:27.678654 rewards_experimental-0.0.2/rewards_experimental/models.py
+-rw-r--r--   0        0        0      825 2023-04-18 20:28:11.774543 rewards_experimental-0.0.2/rewards_experimental/multiagent.py
+-rw-r--r--   0        0        0     5775 2023-04-18 19:30:33.521846 rewards_experimental-0.0.2/rewards_experimental/trainer.py
+-rw-r--r--   0        0        0     7778 2023-04-19 00:45:55.077662 rewards_experimental-0.0.2/rewards_experimental/utils.py
+-rw-r--r--   0        0        0     3518 2023-04-19 06:58:52.780207 rewards_experimental-0.0.2/rewards_experimental/workflow.py
+-rw-r--r--   0        0        0     9154 1970-01-01 00:00:00.000000 rewards_experimental-0.0.2/PKG-INFO
```

### Comparing `rewards_experimental-0.0.1/README.md` & `rewards_experimental-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rewards_experimental-0.0.1/rewards_experimental/agent.py` & `rewards_experimental-0.0.2/rewards_experimental/agent.py`

 * *Files identical despite different names*

### Comparing `rewards_experimental-0.0.1/rewards_experimental/config.py` & `rewards_experimental-0.0.2/rewards_experimental/config.py`

 * *Files identical despite different names*

### Comparing `rewards_experimental-0.0.1/rewards_experimental/models.py` & `rewards_experimental-0.0.2/rewards_experimental/models.py`

 * *Files identical despite different names*

### Comparing `rewards_experimental-0.0.1/rewards_experimental/multiagent.py` & `rewards_experimental-0.0.2/rewards_experimental/multiagent.py`

 * *Files identical despite different names*

### Comparing `rewards_experimental-0.0.1/rewards_experimental/trainer.py` & `rewards_experimental-0.0.2/rewards_experimental/trainer.py`

 * *Files identical despite different names*

### Comparing `rewards_experimental-0.0.1/rewards_experimental/utils.py` & `rewards_experimental-0.0.2/rewards_experimental/utils.py`

 * *Files identical despite different names*

### Comparing `rewards_experimental-0.0.1/rewards_experimental/workflow.py` & `rewards_experimental-0.0.2/rewards_experimental/workflow.py`

 * *Files identical despite different names*

### Comparing `rewards_experimental-0.0.1/PKG-INFO` & `rewards_experimental-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewards-experimental
-Version: 0.0.1
+Version: 0.0.2
 Summary: Start learning about RL and make model and envs in minutes in just few lines of code
 License: MIT
 Author: Anindya
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pygame (>=2.3.0,<3.0.0)
-Requires-Dist: torch (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # **rewards**
 
 #### Create custom environments and train custom agents in few lines of code.
 
 Getting started with RL is quite easy now a days. The workflow stays almost same. You create your environment. This environment is either used for from Open AI's `gym` or we make custom environment using `pygame` and `unity`. After environment creation we go for making deep RL agents, by creating our model using `tensorflow` or `pytorch` etc.
```

