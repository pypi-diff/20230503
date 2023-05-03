# Comparing `tmp/rewards_envs-0.1.2.tar.gz` & `tmp/rewards_envs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewards_envs-0.1.2.tar", max compression
+gzip compressed data, was "rewards_envs-0.1.3.tar", max compression
```

## Comparing `rewards_envs-0.1.2.tar` & `rewards_envs-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3938 2023-04-30 04:46:56.839050 rewards_envs-0.1.2/README.md
--rw-r--r--   0        0        0      494 2023-05-01 20:36:35.833047 rewards_envs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      339 2023-04-30 10:49:37.858452 rewards_envs-0.1.2/rewards_envs/__init__.py
--rw-r--r--   0        0        0     6699 2023-05-01 20:17:47.636843 rewards_envs-0.1.2/rewards_envs/core.py
--rw-r--r--   0        0        0        0 2023-04-17 00:19:10.993914 rewards_envs-0.1.2/rewards_envs/engines/pygame/__init__.py
--rw-r--r--   0        0        0      192 2023-04-17 00:21:43.549724 rewards_envs-0.1.2/rewards_envs/engines/pygame/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-04-16 21:50:07.050409 rewards_envs-0.1.2/rewards_envs/engines/pygame/car_race/__init__.py
--rw-r--r--   0        0        0    79384 2023-04-16 21:35:27.215637 rewards_envs-0.1.2/rewards_envs/engines/pygame/car_race/assets/car.png
--rw-r--r--   0        0        0    86212 2023-04-16 17:18:48.777957 rewards_envs-0.1.2/rewards_envs/engines/pygame/car_race/assets/evaluation/track-1.png
--rw-r--r--   0        0        0    60297 2023-04-16 17:19:04.354021 rewards_envs-0.1.2/rewards_envs/engines/pygame/car_race/assets/training/track-1.png
--rw-r--r--   0        0        0    42293 2023-04-16 17:19:04.362021 rewards_envs-0.1.2/rewards_envs/engines/pygame/car_race/assets/training/track-2.png
--rw-r--r--   0        0        0    49467 2023-04-16 17:19:04.374021 rewards_envs-0.1.2/rewards_envs/engines/pygame/car_race/assets/training/track-3.png
--rw-r--r--   0        0        0    15375 2023-05-01 20:10:18.083191 rewards_envs-0.1.2/rewards_envs/engines/pygame/car_race/car_race.py
--rw-r--r--   0        0        0        0 2023-04-17 00:20:23.669824 rewards_envs-0.1.2/rewards_envs/envs/__init__.py
--rw-r--r--   0        0        0      182 2023-04-26 10:13:49.307527 rewards_envs-0.1.2/rewards_envs/envs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2834 2023-04-26 10:16:20.204393 rewards_envs-0.1.2/rewards_envs/envs/__pycache__/car_race.cpython-310.pyc
--rw-r--r--   0        0        0     1803 2023-05-01 20:20:01.089333 rewards_envs-0.1.2/rewards_envs/envs/car_race.py
--rw-r--r--   0        0        0     4749 1970-01-01 00:00:00.000000 rewards_envs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3938 2023-04-30 04:46:56.839050 rewards_envs-0.1.3/README.md
+-rw-r--r--   0        0        0      455 2023-05-03 06:12:00.309002 rewards_envs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      339 2023-04-30 10:49:37.858452 rewards_envs-0.1.3/rewards_envs/__init__.py
+-rw-r--r--   0        0        0     6699 2023-05-01 20:17:47.636843 rewards_envs-0.1.3/rewards_envs/core.py
+-rw-r--r--   0        0        0        0 2023-04-17 00:19:10.993914 rewards_envs-0.1.3/rewards_envs/engines/pygame/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-17 00:21:43.549724 rewards_envs-0.1.3/rewards_envs/engines/pygame/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-04-16 21:50:07.050409 rewards_envs-0.1.3/rewards_envs/engines/pygame/car_race/__init__.py
+-rw-r--r--   0        0        0    79384 2023-04-16 21:35:27.215637 rewards_envs-0.1.3/rewards_envs/engines/pygame/car_race/assets/car.png
+-rw-r--r--   0        0        0    86212 2023-04-16 17:18:48.777957 rewards_envs-0.1.3/rewards_envs/engines/pygame/car_race/assets/evaluation/track-1.png
+-rw-r--r--   0        0        0    60297 2023-04-16 17:19:04.354021 rewards_envs-0.1.3/rewards_envs/engines/pygame/car_race/assets/training/track-1.png
+-rw-r--r--   0        0        0    42293 2023-04-16 17:19:04.362021 rewards_envs-0.1.3/rewards_envs/engines/pygame/car_race/assets/training/track-2.png
+-rw-r--r--   0        0        0    49467 2023-04-16 17:19:04.374021 rewards_envs-0.1.3/rewards_envs/engines/pygame/car_race/assets/training/track-3.png
+-rw-r--r--   0        0        0    15375 2023-05-01 20:10:18.083191 rewards_envs-0.1.3/rewards_envs/engines/pygame/car_race/car_race.py
+-rw-r--r--   0        0        0        0 2023-04-17 00:20:23.669824 rewards_envs-0.1.3/rewards_envs/envs/__init__.py
+-rw-r--r--   0        0        0      182 2023-04-26 10:13:49.307527 rewards_envs-0.1.3/rewards_envs/envs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2834 2023-04-26 10:16:20.204393 rewards_envs-0.1.3/rewards_envs/envs/__pycache__/car_race.cpython-310.pyc
+-rw-r--r--   0        0        0     1803 2023-05-01 20:20:01.089333 rewards_envs-0.1.3/rewards_envs/envs/car_race.py
+-rw-r--r--   0        0        0     4667 1970-01-01 00:00:00.000000 rewards_envs-0.1.3/PKG-INFO
```

### Comparing `rewards_envs-0.1.2/README.md` & `rewards_envs-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.1.2/rewards_envs/core.py` & `rewards_envs-0.1.3/rewards_envs/core.py`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.1.2/rewards_envs/engines/pygame/car_race/assets/car.png` & `rewards_envs-0.1.3/rewards_envs/engines/pygame/car_race/assets/car.png`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.1.2/rewards_envs/engines/pygame/car_race/assets/evaluation/track-1.png` & `rewards_envs-0.1.3/rewards_envs/engines/pygame/car_race/assets/evaluation/track-1.png`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.1.2/rewards_envs/engines/pygame/car_race/assets/training/track-1.png` & `rewards_envs-0.1.3/rewards_envs/engines/pygame/car_race/assets/training/track-1.png`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.1.2/rewards_envs/engines/pygame/car_race/assets/training/track-2.png` & `rewards_envs-0.1.3/rewards_envs/engines/pygame/car_race/assets/training/track-2.png`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.1.2/rewards_envs/engines/pygame/car_race/assets/training/track-3.png` & `rewards_envs-0.1.3/rewards_envs/engines/pygame/car_race/assets/training/track-3.png`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.1.2/rewards_envs/engines/pygame/car_race/car_race.py` & `rewards_envs-0.1.3/rewards_envs/engines/pygame/car_race/car_race.py`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.1.2/rewards_envs/envs/__pycache__/car_race.cpython-310.pyc` & `rewards_envs-0.1.3/rewards_envs/envs/__pycache__/car_race.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.1.2/rewards_envs/envs/car_race.py` & `rewards_envs-0.1.3/rewards_envs/envs/car_race.py`

 * *Files identical despite different names*

### Comparing `rewards_envs-0.1.2/PKG-INFO` & `rewards_envs-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: rewards-envs
-Version: 0.1.2
+Version: 0.1.3
 Summary: A custom environment creation engine for rewards.ai
 License: MIT
 Author: rewards.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Flask (>=2.2.3,<3.0.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
-Requires-Dist: gymnasium (>=0.28.1,<0.29.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pygame (>=2.3.0,<3.0.0)
-Requires-Dist: torch (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # rewards_envs
 
 rewards-envs is the official repository for environment store, custom environment developement and integration. When it comes to reinforcement learning, we face a hard time creating custom environment and wraping under `gymnasium`'s format. Hence introducing `rewards_envs`. With just few lines of code, Now you can create or convert your games (pygame) to cutsom environment for your agents.
 
 ### Installation and getting started.
```

