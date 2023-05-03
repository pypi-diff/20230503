# Comparing `tmp/babylog-0.0.2.tar.gz` & `tmp/babylog-1.0.2.tar.gz`

## Comparing `babylog-0.0.2.tar` & `babylog-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 babylog-0.0.2/dev-requirements.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 babylog-0.0.2/requirements.txt
--rw-r--r--   0        0        0     8983 2020-02-02 00:00:00.000000 babylog-0.0.2/examples/babylog_yolov8.ipynb
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 babylog-0.0.2/examples/sample_usage.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 babylog-0.0.2/examples/sample_viewing.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 babylog-0.0.2/resources/babylog.config.yaml
--rw-r--r--   0        0        0   124814 2020-02-02 00:00:00.000000 babylog-0.0.2/resources/panda.jpg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 babylog-0.0.2/src/babylog/__init__.py
--rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 babylog-0.0.2/src/babylog/babylog.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 babylog-0.0.2/src/babylog/config.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 babylog-0.0.2/src/babylog/data_utils.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 babylog-0.0.2/src/babylog/deserialize.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 babylog-0.0.2/src/babylog/logger.py
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 babylog-0.0.2/src/babylog/pubsub.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 babylog-0.0.2/src/babylog/utils.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 babylog-0.0.2/src/babylog/protobuf/__init__.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 babylog-0.0.2/src/babylog/protobuf/babylog_stream_pb2.py
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 babylog-0.0.2/src/babylog/protobuf/babylog_stream_pb2.pyi
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 babylog-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 babylog-0.0.2/tests/test_deserialize.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 babylog-0.0.2/.gitignore
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 babylog-0.0.2/README.md
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 babylog-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 babylog-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 babylog-1.0.2/dev-requirements.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 babylog-1.0.2/requirements.txt
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 babylog-1.0.2/examples/sample_usage.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 babylog-1.0.2/examples/sample_viewing.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 babylog-1.0.2/resources/config.yaml
+-rw-r--r--   0        0        0   124814 2020-02-02 00:00:00.000000 babylog-1.0.2/resources/panda.jpg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 babylog-1.0.2/src/babylog/__init__.py
+-rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 babylog-1.0.2/src/babylog/babylog.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 babylog-1.0.2/src/babylog/config.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 babylog-1.0.2/src/babylog/data_utils.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 babylog-1.0.2/src/babylog/deserialize.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 babylog-1.0.2/src/babylog/logger.py
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 babylog-1.0.2/src/babylog/pubsub.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 babylog-1.0.2/src/babylog/utils.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 babylog-1.0.2/src/babylog/protobuf/__init__.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 babylog-1.0.2/src/babylog/protobuf/babylog_stream_pb2.py
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 babylog-1.0.2/src/babylog/protobuf/babylog_stream_pb2.pyi
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 babylog-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 babylog-1.0.2/tests/test_deserialize.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 babylog-1.0.2/.gitignore
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 babylog-1.0.2/README.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 babylog-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 babylog-1.0.2/PKG-INFO
```

### Comparing `babylog-0.0.2/examples/sample_usage.py` & `babylog-1.0.2/examples/sample_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import cv2
 from tqdm import tqdm
 import numpy as np
 
 from babylog import Babylog, VisionModelType, InferenceDevice
 
 
-bl = Babylog("../resources/babylog.config.yaml", save_cloud=False, stream=False)
+bl = Babylog("../resources/config.yaml", save_cloud=False, stream=False)
 img = cv2.imread("../resources/panda.jpg")
 
 
 for i in tqdm(range(100)):
     bl.log(
         image=img,
         prediction=img,
```

### Comparing `babylog-0.0.2/resources/panda.jpg` & `babylog-1.0.2/resources/panda.jpg`

 * *Files identical despite different names*

### Comparing `babylog-0.0.2/src/babylog/babylog.py` & `babylog-1.0.2/src/babylog/babylog.py`

 * *Files identical despite different names*

### Comparing `babylog-0.0.2/src/babylog/config.py` & `babylog-1.0.2/src/babylog/config.py`

 * *Files identical despite different names*

### Comparing `babylog-0.0.2/src/babylog/deserialize.py` & `babylog-1.0.2/src/babylog/deserialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     @property
     def prediction(self) -> np.ndarray:
         return bytes_to_image(self._prediction.prediction.image_bytes)
 
     @property
     def timestamp(self) -> int:
-        return self._prediction.timestamp
+        return self.prediction.timestamp
 
     @classmethod
     def from_path(cls, filepath: str):
         with open(filepath, "rb") as f:
             binary_ = f.read()
         return cls(binary_)
```

### Comparing `babylog-0.0.2/src/babylog/logger.py` & `babylog-1.0.2/src/babylog/logger.py`

 * *Files identical despite different names*

### Comparing `babylog-0.0.2/src/babylog/pubsub.py` & `babylog-1.0.2/src/babylog/pubsub.py`

 * *Files identical despite different names*

### Comparing `babylog-0.0.2/src/babylog/protobuf/babylog_stream_pb2.py` & `babylog-1.0.2/src/babylog/protobuf/babylog_stream_pb2.py`

 * *Files identical despite different names*

### Comparing `babylog-0.0.2/src/babylog/protobuf/babylog_stream_pb2.pyi` & `babylog-1.0.2/src/babylog/protobuf/babylog_stream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `babylog-0.0.2/tests/test_deserialize.py` & `babylog-1.0.2/tests/test_deserialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 def teardown_module(module):
     """Clean up the logs"""
     shutil.rmtree("./babylog/")
 
 
 class TestDeserialize:
     def setup_class(self):
-        self.bl = Babylog("./python/resources/babylog.config.yaml")
+        self.bl = Babylog("./python/resources/config.yaml")
         self.img = cv2.imread("./python/resources/panda.jpg")
 
     @freeze_time("2023-01-29 03:21:34", tz_offset=0)
     def test_serialized_image(self):
         """Test to see that an object gets serialized at the right time"""
         self.bl.log(
             image=self.img,
```

### Comparing `babylog-0.0.2/.gitignore` & `babylog-1.0.2/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -158,10 +158,7 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/*
 
 # VSCode
 .vscode
-
-# logs
-*.bin
```

### Comparing `babylog-0.0.2/README.md` & `babylog-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `babylog-0.0.2/pyproject.toml` & `babylog-1.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "babylog"
-version = "0.0.2"
+version = "1.0.2"
 authors = [
   { name="BabylonAI, Inc.", email="support@babylonai.dev" },
   { name="Ahmad Roumie", email="ahmad@babylonai.dev"},
   { name="Rangel Milushev", email="rangel@babylonai.dev" },
 ]
 description = "A lightweight library for logging image and prediction data for your ML and computer vision models in production."
 readme = "README.md"
@@ -16,18 +16,17 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Development Status :: 4 - Beta",
     "Operating System :: OS Independent",
 ]
 dependencies=[
-    "numpy>=1.24.1",
-    "PyYAML>=6.0",
-    "opencv-python>=4.7.0.68",
+    "numpy==1.24.1",
+    "PyYAML==6.0",
+    "opencv-python==4.7.0.68",
     "boto3==1.15.3",
-    "protobuf>=4.21.12",
+    "protobuf==4.21.12",
     "zmq==0.0.0",
-    "tqdm"
 ]
 [project.urls]
 "Homepage" = "https://github.com/thebabylonai/babylog"
 "Bug Tracker" = "https://github.com/thebabylonai/babylog/issues"
```

### Comparing `babylog-0.0.2/PKG-INFO` & `babylog-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: babylog
-Version: 0.0.2
+Version: 1.0.2
 Summary: A lightweight library for logging image and prediction data for your ML and computer vision models in production.
 Project-URL: Homepage, https://github.com/thebabylonai/babylog
 Project-URL: Bug Tracker, https://github.com/thebabylonai/babylog/issues
 Author-email: "BabylonAI, Inc." <support@babylonai.dev>, Ahmad Roumie <ahmad@babylonai.dev>, Rangel Milushev <rangel@babylonai.dev>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: boto3==1.15.3
-Requires-Dist: numpy>=1.24.1
-Requires-Dist: opencv-python>=4.7.0.68
-Requires-Dist: protobuf>=4.21.12
-Requires-Dist: pyyaml>=6.0
-Requires-Dist: tqdm
+Requires-Dist: numpy==1.24.1
+Requires-Dist: opencv-python==4.7.0.68
+Requires-Dist: protobuf==4.21.12
+Requires-Dist: pyyaml==6.0
 Requires-Dist: zmq==0.0.0
 Description-Content-Type: text/markdown
 
 # babylog
 ## Supported python versions
 The babylog Python library is compatible with **Python version 3.8 and above**. It is recommended to use the latest version of Python for best performance and stability. If you are using an older version of Python, you may need to upgrade your Python installation in order to use babylog. You can check your Python version by running the command `python --version` in your command prompt or terminal.
```

