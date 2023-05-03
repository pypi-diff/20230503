# Comparing `tmp/rewards_api-0.1.3.tar.gz` & `tmp/rewards_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewards_api-0.1.3.tar", last modified: Tue May  2 16:05:58 2023, max compression
+gzip compressed data, was "rewards_api-0.1.4.tar", last modified: Wed May  3 06:17:08 2023, max compression
```

## Comparing `rewards_api-0.1.3.tar` & `rewards_api-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-05-02 16:05:58.661028 rewards_api-0.1.3/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-05-02 16:05:58.661028 rewards_api-0.1.3/PKG-INFO
--rw-r--r--   0 anindya   (1000) anindya   (1000)     5582 2023-04-21 05:26:09.000000 rewards_api-0.1.3/README.md
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      623 2023-04-21 14:36:16.000000 rewards_api-0.1.3/pyproject.toml
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-05-02 16:05:58.661028 rewards_api-0.1.3/rewards_api/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      214 2023-04-22 15:13:14.000000 rewards_api-0.1.3/rewards_api/__init__.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      239 2023-04-22 15:14:35.000000 rewards_api-0.1.3/rewards_api/cli.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      565 2023-04-22 00:31:16.000000 rewards_api-0.1.3/rewards_api/cli_args.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     1058 2023-04-22 15:12:26.000000 rewards_api-0.1.3/rewards_api/config.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)    10767 2023-05-02 15:51:28.000000 rewards_api-0.1.3/rewards_api/main.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)    11132 2023-04-22 15:11:49.000000 rewards_api-0.1.3/rewards_api/streamer.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)    12496 2023-04-22 04:08:17.000000 rewards_api-0.1.3/rewards_api/utils.py
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-05-02 16:05:58.661028 rewards_api-0.1.3/rewards_api.egg-info/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-05-02 16:05:58.000000 rewards_api-0.1.3/rewards_api.egg-info/PKG-INFO
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      399 2023-05-02 16:05:58.000000 rewards_api-0.1.3/rewards_api.egg-info/SOURCES.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)        1 2023-05-02 16:05:58.000000 rewards_api-0.1.3/rewards_api.egg-info/dependency_links.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       63 2023-05-02 16:05:58.000000 rewards_api-0.1.3/rewards_api.egg-info/entry_points.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       97 2023-05-02 16:05:58.000000 rewards_api-0.1.3/rewards_api.egg-info/requires.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       12 2023-05-02 16:05:58.000000 rewards_api-0.1.3/rewards_api.egg-info/top_level.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       38 2023-05-02 16:05:58.661028 rewards_api-0.1.3/setup.cfg
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     1049 2023-05-02 16:05:34.000000 rewards_api-0.1.3/setup.py
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-05-03 06:17:08.013271 rewards_api-0.1.4/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     6041 2023-05-03 06:17:08.009271 rewards_api-0.1.4/PKG-INFO
+-rw-r--r--   0 anindya   (1000) anindya   (1000)     5582 2023-04-21 05:26:09.000000 rewards_api-0.1.4/README.md
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      623 2023-04-21 14:36:16.000000 rewards_api-0.1.4/pyproject.toml
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-05-03 06:17:08.009271 rewards_api-0.1.4/rewards_api/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      214 2023-04-22 15:13:14.000000 rewards_api-0.1.4/rewards_api/__init__.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      239 2023-04-22 15:14:35.000000 rewards_api-0.1.4/rewards_api/cli.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      565 2023-04-22 00:31:16.000000 rewards_api-0.1.4/rewards_api/cli_args.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     1058 2023-04-22 15:12:26.000000 rewards_api-0.1.4/rewards_api/config.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)    10767 2023-05-02 15:51:28.000000 rewards_api-0.1.4/rewards_api/main.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)    11132 2023-04-22 15:11:49.000000 rewards_api-0.1.4/rewards_api/streamer.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)    12496 2023-04-22 04:08:17.000000 rewards_api-0.1.4/rewards_api/utils.py
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-05-03 06:17:08.009271 rewards_api-0.1.4/rewards_api.egg-info/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     6041 2023-05-03 06:17:07.000000 rewards_api-0.1.4/rewards_api.egg-info/PKG-INFO
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      399 2023-05-03 06:17:07.000000 rewards_api-0.1.4/rewards_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)        1 2023-05-03 06:17:07.000000 rewards_api-0.1.4/rewards_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       62 2023-05-03 06:17:07.000000 rewards_api-0.1.4/rewards_api.egg-info/entry_points.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       57 2023-05-03 06:17:07.000000 rewards_api-0.1.4/rewards_api.egg-info/requires.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       12 2023-05-03 06:17:07.000000 rewards_api-0.1.4/rewards_api.egg-info/top_level.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       38 2023-05-03 06:17:08.013271 rewards_api-0.1.4/setup.cfg
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      982 2023-05-03 06:15:20.000000 rewards_api-0.1.4/setup.py
```

### Comparing `rewards_api-0.1.3/PKG-INFO` & `rewards_api-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: rewards_api
-Version: 0.1.3
+Version: 0.1.4
 Summary: rewards api cli package for starting the local rewards server
 Home-page: https://github.com/rewards-ai/rewards-api/tree/latest
 Author: rewards.ai
 Author-email: proanindyadeep@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## **Rewards API:latest**
@@ -226,9 +224,7 @@
 - [ ] Leaderboard 
 
 - [ ] Documentation support (optional)
 
 - [ ] Change the `temp.json` path to the `training_metrics.json`. The path will also be given when the session is created. So there will be no issue for react to create that inside assets. 
 
 - [x] Authentication
-
-
```

### Comparing `rewards_api-0.1.3/README.md` & `rewards_api-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.3/pyproject.toml` & `rewards_api-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.3/rewards_api/cli_args.py` & `rewards_api-0.1.4/rewards_api/cli_args.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.3/rewards_api/config.py` & `rewards_api-0.1.4/rewards_api/config.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.3/rewards_api/main.py` & `rewards_api-0.1.4/rewards_api/main.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.3/rewards_api/streamer.py` & `rewards_api-0.1.4/rewards_api/streamer.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.3/rewards_api/utils.py` & `rewards_api-0.1.4/rewards_api/utils.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.3/rewards_api.egg-info/PKG-INFO` & `rewards_api-0.1.4/rewards_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: rewards-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: rewards api cli package for starting the local rewards server
 Home-page: https://github.com/rewards-ai/rewards-api/tree/latest
 Author: rewards.ai
 Author-email: proanindyadeep@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## **Rewards API:latest**
@@ -226,9 +224,7 @@
 - [ ] Leaderboard 
 
 - [ ] Documentation support (optional)
 
 - [ ] Change the `temp.json` path to the `training_metrics.json`. The path will also be given when the session is created. So there will be no issue for react to create that inside assets. 
 
 - [x] Authentication
-
-
```

### Comparing `rewards_api-0.1.3/setup.py` & `rewards_api-0.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fhand:
     long_description = fhand.read()
 
 setuptools.setup(
     name="rewards_api",
-    version="0.1.3",
+    version="0.1.4",
     author="rewards.ai",
     author_email="proanindyadeep@gmail.com",
     description="rewards api cli package for starting the local rewards server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rewards-ai/rewards-api/tree/latest",
     
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        "rewards-envs", 
-        "rewards-experimental", 
-        "torch", "opencv-python", 
+        "opencv-python", 
         "flask==2.2.3", "flask_cors", 
         "boto3", "Flask[async]"
         ],
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     entry_points={
         "console_scripts": [
```

