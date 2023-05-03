# Comparing `tmp/cortex-python-6.3.1a2.tar.gz` & `tmp/cortex-python-6.3.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex-python-6.3.1a2.tar", last modified: Wed Apr 26 11:35:37 2023, max compression
+gzip compressed data, was "cortex-python-6.3.1a3.tar", last modified: Wed May  3 15:18:28 2023, max compression
```

## Comparing `cortex-python-6.3.1a2.tar` & `cortex-python-6.3.1a3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/
--rw-r--r--   0 root         (0) root         (0)      533 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    11368 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4623 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3938 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/cortex/
--rw-r--r--   0 root         (0) root         (0)      877 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/__init__.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/__version__.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/auth.py
--rw-r--r--   0 root         (0) root         (0)     1989 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/camel.py
--rw-r--r--   0 root         (0) root         (0)    27147 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/client.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/connection.py
--rw-r--r--   0 root         (0) root         (0)      684 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/constant.py
--rw-r--r--   0 root         (0) root         (0)     9662 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/content.py
--rw-r--r--   0 root         (0) root         (0)     2532 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/env.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/cortex/experiment/
--rw-r--r--   0 root         (0) root         (0)      675 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/experiment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7794 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/experiment/local.py
--rw-r--r--   0 root         (0) root         (0)    10770 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/experiment/model.py
--rw-r--r--   0 root         (0) root         (0)    37404 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/experiment/remote.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/message.py
--rw-r--r--   0 root         (0) root         (0)     4387 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/model.py
--rw-r--r--   0 root         (0) root         (0)    10071 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/properties.py
--rw-r--r--   0 root         (0) root         (0)     2517 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/secrets.py
--rw-r--r--   0 root         (0) root         (0)    11705 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/serviceconnector.py
--rw-r--r--   0 root         (0) root         (0)     4460 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/session.py
--rw-r--r--   0 root         (0) root         (0)     8521 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/skill.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/timer.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/types.py
--rw-r--r--   0 root         (0) root         (0)     8411 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/utils.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/cortex/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/cortex_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4623 2023-04-26 11:35:37.000000 cortex-python-6.3.1a2/cortex_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-04-26 11:35:37.000000 cortex-python-6.3.1a2/cortex_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 11:35:37.000000 cortex-python-6.3.1a2/cortex_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-04-26 11:35:37.000000 cortex-python-6.3.1a2/cortex_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-26 11:35:37.000000 cortex-python-6.3.1a2/cortex_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2175 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/test/
--rw-r--r--   0 root         (0) root         (0)      590 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:35:37.189905 cortex-python-6.3.1a2/test/unit/
--rw-r--r--   0 root         (0) root         (0)      590 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2493 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/authenticationclient_test.py
--rw-r--r--   0 root         (0) root         (0)     4371 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/connectionclient_test.py
--rw-r--r--   0 root         (0) root         (0)     9014 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/cortex_test.py
--rw-r--r--   0 root         (0) root         (0)     5216 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/environment_config_test.py
--rw-r--r--   0 root         (0) root         (0)     6809 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/experiment_test.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/fixtures.py
--rw-r--r--   0 root         (0) root         (0)     8807 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/run_test.py
--rw-r--r--   0 root         (0) root         (0)     1736 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/serviceconnector_test.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-04-26 11:33:44.000000 cortex-python-6.3.1a2/test/unit/sessionclient_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/
+-rw-r--r--   0 root         (0) root         (0)      533 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    11368 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4623 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3938 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/cortex/
+-rw-r--r--   0 root         (0) root         (0)      877 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/auth.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/camel.py
+-rw-r--r--   0 root         (0) root         (0)    27147 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/client.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/connection.py
+-rw-r--r--   0 root         (0) root         (0)      684 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/constant.py
+-rw-r--r--   0 root         (0) root         (0)     9662 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/content.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/env.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/cortex/experiment/
+-rw-r--r--   0 root         (0) root         (0)      675 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/experiment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7794 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/experiment/local.py
+-rw-r--r--   0 root         (0) root         (0)    10770 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/experiment/model.py
+-rw-r--r--   0 root         (0) root         (0)    37404 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/experiment/remote.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/message.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/model.py
+-rw-r--r--   0 root         (0) root         (0)    10071 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/properties.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/secrets.py
+-rw-r--r--   0 root         (0) root         (0)    11705 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/serviceconnector.py
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/session.py
+-rw-r--r--   0 root         (0) root         (0)     8521 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/skill.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/timer.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/types.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/cortex/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/cortex_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4623 2023-05-03 15:18:28.000000 cortex-python-6.3.1a3/cortex_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-05-03 15:18:28.000000 cortex-python-6.3.1a3/cortex_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 15:18:28.000000 cortex-python-6.3.1a3/cortex_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-03 15:18:28.000000 cortex-python-6.3.1a3/cortex_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-03 15:18:28.000000 cortex-python-6.3.1a3/cortex_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/test/
+-rw-r--r--   0 root         (0) root         (0)      590 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:18:28.909790 cortex-python-6.3.1a3/test/unit/
+-rw-r--r--   0 root         (0) root         (0)      590 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/authenticationclient_test.py
+-rw-r--r--   0 root         (0) root         (0)     4371 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/connectionclient_test.py
+-rw-r--r--   0 root         (0) root         (0)     9014 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/cortex_test.py
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/environment_config_test.py
+-rw-r--r--   0 root         (0) root         (0)     6809 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/experiment_test.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     8807 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/run_test.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/serviceconnector_test.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-05-03 15:16:36.000000 cortex-python-6.3.1a3/test/unit/sessionclient_test.py
```

### Comparing `cortex-python-6.3.1a2/CHANGELOG.md` & `cortex-python-6.3.1a3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/LICENSE` & `cortex-python-6.3.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/PKG-INFO` & `cortex-python-6.3.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortex-python
-Version: 6.3.1a2
+Version: 6.3.1a3
 Summary: Python module for the CognitiveScale Cortex Cognitive Platform
 Home-page: https://github.com/CognitiveScale/cortex-python
 Author: CognitiveScale
 Author-email: support@cognitivescale.com
 License: Apache 2.0
 Project-URL: Documentation, https://cognitivescale.github.io/cortex-python/master/
 Project-URL: Source, https://github.com/CognitiveScale/cortex-python
```

### Comparing `cortex-python-6.3.1a2/README.md` & `cortex-python-6.3.1a3/README.md`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/__init__.py` & `cortex-python-6.3.1a3/cortex/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/auth.py` & `cortex-python-6.3.1a3/cortex/auth.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/camel.py` & `cortex-python-6.3.1a3/cortex/camel.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/client.py` & `cortex-python-6.3.1a3/cortex/client.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/connection.py` & `cortex-python-6.3.1a3/cortex/connection.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/constant.py` & `cortex-python-6.3.1a3/cortex/constant.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/content.py` & `cortex-python-6.3.1a3/cortex/content.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/env.py` & `cortex-python-6.3.1a3/cortex/env.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/exceptions.py` & `cortex-python-6.3.1a3/cortex/exceptions.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/experiment/__init__.py` & `cortex-python-6.3.1a3/cortex/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/experiment/local.py` & `cortex-python-6.3.1a3/cortex/experiment/local.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/experiment/model.py` & `cortex-python-6.3.1a3/cortex/experiment/model.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/experiment/remote.py` & `cortex-python-6.3.1a3/cortex/experiment/remote.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/message.py` & `cortex-python-6.3.1a3/cortex/message.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/model.py` & `cortex-python-6.3.1a3/cortex/model.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/properties.py` & `cortex-python-6.3.1a3/cortex/properties.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/secrets.py` & `cortex-python-6.3.1a3/cortex/secrets.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/serviceconnector.py` & `cortex-python-6.3.1a3/cortex/serviceconnector.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/session.py` & `cortex-python-6.3.1a3/cortex/session.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/skill.py` & `cortex-python-6.3.1a3/cortex/skill.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/timer.py` & `cortex-python-6.3.1a3/cortex/timer.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/types.py` & `cortex-python-6.3.1a3/cortex/types.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/utils.py` & `cortex-python-6.3.1a3/cortex/utils.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex/viz.py` & `cortex-python-6.3.1a3/cortex/viz.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/cortex_python.egg-info/PKG-INFO` & `cortex-python-6.3.1a3/cortex_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortex-python
-Version: 6.3.1a2
+Version: 6.3.1a3
 Summary: Python module for the CognitiveScale Cortex Cognitive Platform
 Home-page: https://github.com/CognitiveScale/cortex-python
 Author: CognitiveScale
 Author-email: support@cognitivescale.com
 License: Apache 2.0
 Project-URL: Documentation, https://cognitivescale.github.io/cortex-python/master/
 Project-URL: Source, https://github.com/CognitiveScale/cortex-python
```

### Comparing `cortex-python-6.3.1a2/cortex_python.egg-info/SOURCES.txt` & `cortex-python-6.3.1a3/cortex_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/setup.py` & `cortex-python-6.3.1a3/setup.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/test/__init__.py` & `cortex-python-6.3.1a3/test/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/test/unit/__init__.py` & `cortex-python-6.3.1a3/test/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/test/unit/authenticationclient_test.py` & `cortex-python-6.3.1a3/test/unit/authenticationclient_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/test/unit/connectionclient_test.py` & `cortex-python-6.3.1a3/test/unit/connectionclient_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/test/unit/cortex_test.py` & `cortex-python-6.3.1a3/test/unit/cortex_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/test/unit/environment_config_test.py` & `cortex-python-6.3.1a3/test/unit/environment_config_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/test/unit/experiment_test.py` & `cortex-python-6.3.1a3/test/unit/experiment_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/test/unit/fixtures.py` & `cortex-python-6.3.1a3/test/unit/fixtures.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/test/unit/run_test.py` & `cortex-python-6.3.1a3/test/unit/run_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/test/unit/serviceconnector_test.py` & `cortex-python-6.3.1a3/test/unit/serviceconnector_test.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.3.1a2/test/unit/sessionclient_test.py` & `cortex-python-6.3.1a3/test/unit/sessionclient_test.py`

 * *Files identical despite different names*

