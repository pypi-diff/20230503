# Comparing `tmp/flytekitplugins-awsbatch-1.6.0b0.tar.gz` & `tmp/flytekitplugins-awsbatch-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-awsbatch-1.6.0b0.tar", last modified: Wed Apr 19 20:54:26 2023, max compression
+gzip compressed data, was "flytekitplugins-awsbatch-1.6.0b1.tar", last modified: Wed May  3 04:48:03 2023, max compression
```

## Comparing `flytekitplugins-awsbatch-1.6.0b0.tar` & `flytekitplugins-awsbatch-1.6.0b1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:26.075022 flytekitplugins-awsbatch-1.6.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-19 20:54:26.075022 flytekitplugins-awsbatch-1.6.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-19 20:54:06.000000 flytekitplugins-awsbatch-1.6.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:26.075022 flytekitplugins-awsbatch-1.6.0b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:26.075022 flytekitplugins-awsbatch-1.6.0b0/flytekitplugins/awsbatch/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-19 20:54:06.000000 flytekitplugins-awsbatch-1.6.0b0/flytekitplugins/awsbatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-19 20:54:06.000000 flytekitplugins-awsbatch-1.6.0b0/flytekitplugins/awsbatch/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:26.075022 flytekitplugins-awsbatch-1.6.0b0/flytekitplugins_awsbatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-19 20:54:26.000000 flytekitplugins-awsbatch-1.6.0b0/flytekitplugins_awsbatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-19 20:54:26.000000 flytekitplugins-awsbatch-1.6.0b0/flytekitplugins_awsbatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:26.000000 flytekitplugins-awsbatch-1.6.0b0/flytekitplugins_awsbatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:26.000000 flytekitplugins-awsbatch-1.6.0b0/flytekitplugins_awsbatch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 20:54:26.000000 flytekitplugins-awsbatch-1.6.0b0/flytekitplugins_awsbatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:26.000000 flytekitplugins-awsbatch-1.6.0b0/flytekitplugins_awsbatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:54:26.075022 flytekitplugins-awsbatch-1.6.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-19 20:54:25.000000 flytekitplugins-awsbatch-1.6.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:03.728287 flytekitplugins-awsbatch-1.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-03 04:48:03.728287 flytekitplugins-awsbatch-1.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-03 04:47:44.000000 flytekitplugins-awsbatch-1.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:03.728287 flytekitplugins-awsbatch-1.6.0b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:03.728287 flytekitplugins-awsbatch-1.6.0b1/flytekitplugins/awsbatch/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 04:47:44.000000 flytekitplugins-awsbatch-1.6.0b1/flytekitplugins/awsbatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-03 04:47:44.000000 flytekitplugins-awsbatch-1.6.0b1/flytekitplugins/awsbatch/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:03.728287 flytekitplugins-awsbatch-1.6.0b1/flytekitplugins_awsbatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-03 04:48:03.000000 flytekitplugins-awsbatch-1.6.0b1/flytekitplugins_awsbatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 04:48:03.000000 flytekitplugins-awsbatch-1.6.0b1/flytekitplugins_awsbatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:48:03.000000 flytekitplugins-awsbatch-1.6.0b1/flytekitplugins_awsbatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:03.000000 flytekitplugins-awsbatch-1.6.0b1/flytekitplugins_awsbatch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 04:48:03.000000 flytekitplugins-awsbatch-1.6.0b1/flytekitplugins_awsbatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:03.000000 flytekitplugins-awsbatch-1.6.0b1/flytekitplugins_awsbatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 04:48:03.728287 flytekitplugins-awsbatch-1.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-03 04:48:03.000000 flytekitplugins-awsbatch-1.6.0b1/setup.py
```

### Comparing `flytekitplugins-awsbatch-1.6.0b0/PKG-INFO` & `flytekitplugins-awsbatch-1.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-awsbatch
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: This package holds the AWS Batch plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-awsbatch-1.6.0b0/flytekitplugins/awsbatch/task.py` & `flytekitplugins-awsbatch-1.6.0b1/flytekitplugins/awsbatch/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-awsbatch-1.6.0b0/flytekitplugins_awsbatch.egg-info/PKG-INFO` & `flytekitplugins-awsbatch-1.6.0b1/flytekitplugins_awsbatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-awsbatch
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: This package holds the AWS Batch plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-awsbatch-1.6.0b0/setup.py` & `flytekitplugins-awsbatch-1.6.0b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "awsbatch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0"]
 
-__version__ = "1.6.0b0"
+__version__ = "1.6.0b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the AWS Batch plugins for flytekit",
```

