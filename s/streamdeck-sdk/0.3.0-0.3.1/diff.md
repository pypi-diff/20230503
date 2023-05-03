# Comparing `tmp/streamdeck_sdk-0.3.0.tar.gz` & `tmp/streamdeck_sdk-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamdeck_sdk-0.3.0.tar", last modified: Tue Apr 18 14:28:10 2023, max compression
+gzip compressed data, was "streamdeck_sdk-0.3.1.tar", last modified: Wed May  3 18:17:14 2023, max compression
```

## Comparing `streamdeck_sdk-0.3.0.tar` & `streamdeck_sdk-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-04-18 14:28:10.091638 streamdeck_sdk-0.3.0/
--rw-r--r--   0 grisha     (501) staff       (20)    11357 2023-03-09 11:40:53.000000 streamdeck_sdk-0.3.0/LICENSE
--rw-r--r--   0 grisha     (501) staff       (20)     2653 2023-04-18 14:28:10.091511 streamdeck_sdk-0.3.0/PKG-INFO
--rw-r--r--   0 grisha     (501) staff       (20)     1924 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/README.md
--rw-r--r--   0 grisha     (501) staff       (20)       38 2023-04-18 14:28:10.091677 streamdeck_sdk-0.3.0/setup.cfg
--rw-r--r--   0 grisha     (501) staff       (20)     1367 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/setup.py
-drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-04-18 14:28:10.087964 streamdeck_sdk-0.3.0/src/
-drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-04-18 14:28:10.089475 streamdeck_sdk-0.3.0/src/streamdeck_sdk/
--rw-r--r--   0 grisha     (501) staff       (20)      258 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/__init__.py
--rw-r--r--   0 grisha     (501) staff       (20)     1650 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/event_routings.py
--rw-r--r--   0 grisha     (501) staff       (20)     1531 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/logger.py
--rw-r--r--   0 grisha     (501) staff       (20)     6902 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/mixins.py
-drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-04-18 14:28:10.090604 streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/
--rw-r--r--   0 grisha     (501) staff       (20)       98 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/__init__.py
--rw-r--r--   0 grisha     (501) staff       (20)     5392 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/events_received_objs.py
--rw-r--r--   0 grisha     (501) staff       (20)     2245 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/events_sent_objs.py
--rw-r--r--   0 grisha     (501) staff       (20)      888 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/registration_objs.py
--rw-r--r--   0 grisha     (501) staff       (20)     7342 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/sdk.py
-drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-04-18 14:28:10.091288 streamdeck_sdk-0.3.0/src/streamdeck_sdk/utils/
--rw-r--r--   0 grisha     (501) staff       (20)      125 2023-03-15 00:54:43.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/utils/__init__.py
--rw-r--r--   0 grisha     (501) staff       (20)      620 2023-03-12 23:47:41.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/utils/image_converters.py
--rw-r--r--   0 grisha     (501) staff       (20)     1110 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk/utils/in_separate_thread.py
-drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-04-18 14:28:10.090060 streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/
--rw-r--r--   0 grisha     (501) staff       (20)     2653 2023-04-18 14:28:10.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/PKG-INFO
--rw-r--r--   0 grisha     (501) staff       (20)      701 2023-04-18 14:28:10.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 grisha     (501) staff       (20)        1 2023-04-18 14:28:10.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 grisha     (501) staff       (20)       83 2023-04-18 14:28:10.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/requires.txt
--rw-r--r--   0 grisha     (501) staff       (20)       15 2023-04-18 14:28:10.000000 streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-05-03 18:17:14.683524 streamdeck_sdk-0.3.1/
+-rw-r--r--   0 grisha     (501) staff       (20)    11357 2023-03-09 11:40:53.000000 streamdeck_sdk-0.3.1/LICENSE
+-rw-r--r--   0 grisha     (501) staff       (20)     2653 2023-05-03 18:17:14.683390 streamdeck_sdk-0.3.1/PKG-INFO
+-rw-r--r--   0 grisha     (501) staff       (20)     1924 2023-04-18 15:14:24.000000 streamdeck_sdk-0.3.1/README.md
+-rw-r--r--   0 grisha     (501) staff       (20)       38 2023-05-03 18:17:14.683567 streamdeck_sdk-0.3.1/setup.cfg
+-rw-r--r--   0 grisha     (501) staff       (20)     1367 2023-05-03 18:15:43.000000 streamdeck_sdk-0.3.1/setup.py
+drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-05-03 18:17:14.679272 streamdeck_sdk-0.3.1/src/
+drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-05-03 18:17:14.681056 streamdeck_sdk-0.3.1/src/streamdeck_sdk/
+-rw-r--r--   0 grisha     (501) staff       (20)      258 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk/__init__.py
+-rw-r--r--   0 grisha     (501) staff       (20)     1650 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk/event_routings.py
+-rw-r--r--   0 grisha     (501) staff       (20)     1531 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk/logger.py
+-rw-r--r--   0 grisha     (501) staff       (20)     6902 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk/mixins.py
+drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-05-03 18:17:14.682539 streamdeck_sdk-0.3.1/src/streamdeck_sdk/sd_objs/
+-rw-r--r--   0 grisha     (501) staff       (20)       98 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk/sd_objs/__init__.py
+-rw-r--r--   0 grisha     (501) staff       (20)     5394 2023-05-03 18:15:30.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk/sd_objs/events_received_objs.py
+-rw-r--r--   0 grisha     (501) staff       (20)     2245 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk/sd_objs/events_sent_objs.py
+-rw-r--r--   0 grisha     (501) staff       (20)      888 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk/sd_objs/registration_objs.py
+-rw-r--r--   0 grisha     (501) staff       (20)     7342 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk/sdk.py
+drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-05-03 18:17:14.683162 streamdeck_sdk-0.3.1/src/streamdeck_sdk/utils/
+-rw-r--r--   0 grisha     (501) staff       (20)      125 2023-03-15 00:54:43.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk/utils/__init__.py
+-rw-r--r--   0 grisha     (501) staff       (20)      620 2023-03-12 23:47:41.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk/utils/image_converters.py
+-rw-r--r--   0 grisha     (501) staff       (20)     1110 2023-04-18 14:25:35.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk/utils/in_separate_thread.py
+drwxr-xr-x   0 grisha     (501) staff       (20)        0 2023-05-03 18:17:14.681777 streamdeck_sdk-0.3.1/src/streamdeck_sdk.egg-info/
+-rw-r--r--   0 grisha     (501) staff       (20)     2653 2023-05-03 18:17:14.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 grisha     (501) staff       (20)      701 2023-05-03 18:17:14.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 grisha     (501) staff       (20)        1 2023-05-03 18:17:14.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 grisha     (501) staff       (20)       83 2023-05-03 18:17:14.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk.egg-info/requires.txt
+-rw-r--r--   0 grisha     (501) staff       (20)       15 2023-05-03 18:17:14.000000 streamdeck_sdk-0.3.1/src/streamdeck_sdk.egg-info/top_level.txt
```

### Comparing `streamdeck_sdk-0.3.0/LICENSE` & `streamdeck_sdk-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.3.0/PKG-INFO` & `streamdeck_sdk-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeck_sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library for creating Stream Deck plugins in Python.
 Home-page: https://github.com/gri-gus/streamdeck-python-sdk
 Author: Grigoriy Gusev
 Author-email: thegrigus@gmail.com
 License: Apache Software License
 Keywords: python,sdk,streamdeck,streamdeck-sdk,streamdeck_sdk,stream deck sdk,stream deck,elgato,elgato sdk,elgato stream deck,streamdeck-python-sdk,streamdeck_python_sdk,streamdeck python sdk
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamdeck_sdk Version: 0.3.0 Summary: Library for
+Metadata-Version: 2.1 Name: streamdeck_sdk Version: 0.3.1 Summary: Library for
 creating Stream Deck plugins in Python. Home-page: https://github.com/gri-gus/
 streamdeck-python-sdk Author: Grigoriy Gusev Author-email: thegrigus@gmail.com
 License: Apache Software License Keywords: python,sdk,streamdeck,streamdeck-
 sdk,streamdeck_sdk,stream deck sdk,stream deck,elgato,elgato sdk,elgato stream
 deck,streamdeck-python-sdk,streamdeck_python_sdk,streamdeck python sdk
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
```

### Comparing `streamdeck_sdk-0.3.0/README.md` & `streamdeck_sdk-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.3.0/setup.py` & `streamdeck_sdk-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = "0.3.0"
+VERSION = "0.3.1"
 PACKAGE_DIR = "src"
 REQUIREMENTS_FILE = PACKAGE_DIR + "/requirements.txt"
 README = "README.md"
 
 with open(REQUIREMENTS_FILE, "r") as f:
     requirements = f.read().splitlines()
```

### Comparing `streamdeck_sdk-0.3.0/src/streamdeck_sdk/event_routings.py` & `streamdeck_sdk-0.3.1/src/streamdeck_sdk/event_routings.py`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.3.0/src/streamdeck_sdk/logger.py` & `streamdeck_sdk-0.3.1/src/streamdeck_sdk/logger.py`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.3.0/src/streamdeck_sdk/mixins.py` & `streamdeck_sdk-0.3.1/src/streamdeck_sdk/mixins.py`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/events_received_objs.py` & `streamdeck_sdk-0.3.1/src/streamdeck_sdk/sd_objs/events_received_objs.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,21 +113,21 @@
     coordinates: KeyCoordinates
     tapPos: list
     hold: bool
 
 
 class DialDownPayload(BaseModel):
     controller: str
-    settings: str
+    settings: dict
     coordinates: KeyCoordinates
 
 
 class DialUpPayload(BaseModel):
     controller: str
-    settings: str
+    settings: dict
     coordinates: KeyCoordinates
 
 
 # endregion NestedModels
 
 # region Models
 class DidReceiveSettings(BaseModel):
```

### Comparing `streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/events_sent_objs.py` & `streamdeck_sdk-0.3.1/src/streamdeck_sdk/sd_objs/events_sent_objs.py`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.3.0/src/streamdeck_sdk/sd_objs/registration_objs.py` & `streamdeck_sdk-0.3.1/src/streamdeck_sdk/sd_objs/registration_objs.py`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.3.0/src/streamdeck_sdk/sdk.py` & `streamdeck_sdk-0.3.1/src/streamdeck_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.3.0/src/streamdeck_sdk/utils/image_converters.py` & `streamdeck_sdk-0.3.1/src/streamdeck_sdk/utils/image_converters.py`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.3.0/src/streamdeck_sdk/utils/in_separate_thread.py` & `streamdeck_sdk-0.3.1/src/streamdeck_sdk/utils/in_separate_thread.py`

 * *Files identical despite different names*

### Comparing `streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/PKG-INFO` & `streamdeck_sdk-0.3.1/src/streamdeck_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamdeck-sdk
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library for creating Stream Deck plugins in Python.
 Home-page: https://github.com/gri-gus/streamdeck-python-sdk
 Author: Grigoriy Gusev
 Author-email: thegrigus@gmail.com
 License: Apache Software License
 Keywords: python,sdk,streamdeck,streamdeck-sdk,streamdeck_sdk,stream deck sdk,stream deck,elgato,elgato sdk,elgato stream deck,streamdeck-python-sdk,streamdeck_python_sdk,streamdeck python sdk
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamdeck-sdk Version: 0.3.0 Summary: Library for
+Metadata-Version: 2.1 Name: streamdeck-sdk Version: 0.3.1 Summary: Library for
 creating Stream Deck plugins in Python. Home-page: https://github.com/gri-gus/
 streamdeck-python-sdk Author: Grigoriy Gusev Author-email: thegrigus@gmail.com
 License: Apache Software License Keywords: python,sdk,streamdeck,streamdeck-
 sdk,streamdeck_sdk,stream deck sdk,stream deck,elgato,elgato sdk,elgato stream
 deck,streamdeck-python-sdk,streamdeck_python_sdk,streamdeck python sdk
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
```

### Comparing `streamdeck_sdk-0.3.0/src/streamdeck_sdk.egg-info/SOURCES.txt` & `streamdeck_sdk-0.3.1/src/streamdeck_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

