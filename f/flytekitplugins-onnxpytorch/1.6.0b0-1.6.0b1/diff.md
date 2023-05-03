# Comparing `tmp/flytekitplugins-onnxpytorch-1.6.0b0.tar.gz` & `tmp/flytekitplugins-onnxpytorch-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-onnxpytorch-1.6.0b0.tar", last modified: Wed Apr 19 20:54:32 2023, max compression
+gzip compressed data, was "flytekitplugins-onnxpytorch-1.6.0b1.tar", last modified: Wed May  3 04:48:10 2023, max compression
```

## Comparing `flytekitplugins-onnxpytorch-1.6.0b0.tar` & `flytekitplugins-onnxpytorch-1.6.0b1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:32.971124 flytekitplugins-onnxpytorch-1.6.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-19 20:54:32.971124 flytekitplugins-onnxpytorch-1.6.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-19 20:54:06.000000 flytekitplugins-onnxpytorch-1.6.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:32.967124 flytekitplugins-onnxpytorch-1.6.0b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:32.967124 flytekitplugins-onnxpytorch-1.6.0b0/flytekitplugins/onnxpytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 20:54:06.000000 flytekitplugins-onnxpytorch-1.6.0b0/flytekitplugins/onnxpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-19 20:54:06.000000 flytekitplugins-onnxpytorch-1.6.0b0/flytekitplugins/onnxpytorch/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:32.971124 flytekitplugins-onnxpytorch-1.6.0b0/flytekitplugins_onnxpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-19 20:54:32.000000 flytekitplugins-onnxpytorch-1.6.0b0/flytekitplugins_onnxpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-19 20:54:32.000000 flytekitplugins-onnxpytorch-1.6.0b0/flytekitplugins_onnxpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:32.000000 flytekitplugins-onnxpytorch-1.6.0b0/flytekitplugins_onnxpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:32.000000 flytekitplugins-onnxpytorch-1.6.0b0/flytekitplugins_onnxpytorch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 20:54:32.000000 flytekitplugins-onnxpytorch-1.6.0b0/flytekitplugins_onnxpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:32.000000 flytekitplugins-onnxpytorch-1.6.0b0/flytekitplugins_onnxpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:54:32.971124 flytekitplugins-onnxpytorch-1.6.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-19 20:54:25.000000 flytekitplugins-onnxpytorch-1.6.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:10.504315 flytekitplugins-onnxpytorch-1.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-03 04:48:10.504315 flytekitplugins-onnxpytorch-1.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-03 04:47:44.000000 flytekitplugins-onnxpytorch-1.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:10.504315 flytekitplugins-onnxpytorch-1.6.0b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:10.504315 flytekitplugins-onnxpytorch-1.6.0b1/flytekitplugins/onnxpytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-03 04:47:44.000000 flytekitplugins-onnxpytorch-1.6.0b1/flytekitplugins/onnxpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-03 04:47:44.000000 flytekitplugins-onnxpytorch-1.6.0b1/flytekitplugins/onnxpytorch/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:10.504315 flytekitplugins-onnxpytorch-1.6.0b1/flytekitplugins_onnxpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-03 04:48:10.000000 flytekitplugins-onnxpytorch-1.6.0b1/flytekitplugins_onnxpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 04:48:10.000000 flytekitplugins-onnxpytorch-1.6.0b1/flytekitplugins_onnxpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:48:10.000000 flytekitplugins-onnxpytorch-1.6.0b1/flytekitplugins_onnxpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:10.000000 flytekitplugins-onnxpytorch-1.6.0b1/flytekitplugins_onnxpytorch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 04:48:10.000000 flytekitplugins-onnxpytorch-1.6.0b1/flytekitplugins_onnxpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:10.000000 flytekitplugins-onnxpytorch-1.6.0b1/flytekitplugins_onnxpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 04:48:10.504315 flytekitplugins-onnxpytorch-1.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-03 04:48:03.000000 flytekitplugins-onnxpytorch-1.6.0b1/setup.py
```

### Comparing `flytekitplugins-onnxpytorch-1.6.0b0/PKG-INFO` & `flytekitplugins-onnxpytorch-1.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxpytorch
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: ONNX PyTorch Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxpytorch-1.6.0b0/flytekitplugins/onnxpytorch/schema.py` & `flytekitplugins-onnxpytorch-1.6.0b1/flytekitplugins/onnxpytorch/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-onnxpytorch-1.6.0b0/flytekitplugins_onnxpytorch.egg-info/PKG-INFO` & `flytekitplugins-onnxpytorch-1.6.0b1/flytekitplugins_onnxpytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxpytorch
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: ONNX PyTorch Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxpytorch-1.6.0b0/setup.py` & `flytekitplugins-onnxpytorch-1.6.0b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "onnxpytorch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "torch>=1.11.0"]
 
-__version__ = "1.6.0b0"
+__version__ = "1.6.0b1"
 
 setup(
     name=f"flytekitplugins-{PLUGIN_NAME}",
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="ONNX PyTorch Plugin for Flytekit",
```

