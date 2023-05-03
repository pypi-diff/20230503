# Comparing `tmp/flytekitplugins-kfpytorch-1.6.0b0.tar.gz` & `tmp/flytekitplugins-kfpytorch-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfpytorch-1.6.0b0.tar", last modified: Wed Apr 19 20:54:31 2023, max compression
+gzip compressed data, was "flytekitplugins-kfpytorch-1.6.0b1.tar", last modified: Wed May  3 04:48:09 2023, max compression
```

## Comparing `flytekitplugins-kfpytorch-1.6.0b0.tar` & `flytekitplugins-kfpytorch-1.6.0b1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:31.519102 flytekitplugins-kfpytorch-1.6.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-19 20:54:31.519102 flytekitplugins-kfpytorch-1.6.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-19 20:54:06.000000 flytekitplugins-kfpytorch-1.6.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:31.519102 flytekitplugins-kfpytorch-1.6.0b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:31.519102 flytekitplugins-kfpytorch-1.6.0b0/flytekitplugins/kfpytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-19 20:54:06.000000 flytekitplugins-kfpytorch-1.6.0b0/flytekitplugins/kfpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-19 20:54:06.000000 flytekitplugins-kfpytorch-1.6.0b0/flytekitplugins/kfpytorch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-19 20:54:06.000000 flytekitplugins-kfpytorch-1.6.0b0/flytekitplugins/kfpytorch/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:31.519102 flytekitplugins-kfpytorch-1.6.0b0/flytekitplugins_kfpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-19 20:54:31.000000 flytekitplugins-kfpytorch-1.6.0b0/flytekitplugins_kfpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-19 20:54:31.000000 flytekitplugins-kfpytorch-1.6.0b0/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:31.000000 flytekitplugins-kfpytorch-1.6.0b0/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:31.000000 flytekitplugins-kfpytorch-1.6.0b0/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-19 20:54:31.000000 flytekitplugins-kfpytorch-1.6.0b0/flytekitplugins_kfpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:31.000000 flytekitplugins-kfpytorch-1.6.0b0/flytekitplugins_kfpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:54:31.523102 flytekitplugins-kfpytorch-1.6.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-19 20:54:25.000000 flytekitplugins-kfpytorch-1.6.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:09.088308 flytekitplugins-kfpytorch-1.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-03 04:48:09.088308 flytekitplugins-kfpytorch-1.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-03 04:47:44.000000 flytekitplugins-kfpytorch-1.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:09.084308 flytekitplugins-kfpytorch-1.6.0b1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:09.088308 flytekitplugins-kfpytorch-1.6.0b1/flytekitplugins/kfpytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-03 04:47:44.000000 flytekitplugins-kfpytorch-1.6.0b1/flytekitplugins/kfpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-03 04:47:44.000000 flytekitplugins-kfpytorch-1.6.0b1/flytekitplugins/kfpytorch/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:09.088308 flytekitplugins-kfpytorch-1.6.0b1/flytekitplugins_kfpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-03 04:48:09.000000 flytekitplugins-kfpytorch-1.6.0b1/flytekitplugins_kfpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-03 04:48:09.000000 flytekitplugins-kfpytorch-1.6.0b1/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:48:09.000000 flytekitplugins-kfpytorch-1.6.0b1/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:09.000000 flytekitplugins-kfpytorch-1.6.0b1/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 04:48:09.000000 flytekitplugins-kfpytorch-1.6.0b1/flytekitplugins_kfpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:09.000000 flytekitplugins-kfpytorch-1.6.0b1/flytekitplugins_kfpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 04:48:09.088308 flytekitplugins-kfpytorch-1.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-03 04:48:03.000000 flytekitplugins-kfpytorch-1.6.0b1/setup.py
```

### Comparing `flytekitplugins-kfpytorch-1.6.0b0/PKG-INFO` & `flytekitplugins-kfpytorch-1.6.0b1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,7 +13,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
+Provides-Extra: elastic
```

### Comparing `flytekitplugins-kfpytorch-1.6.0b0/README.md` & `flytekitplugins-kfpytorch-1.6.0b1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Flytekit Kubeflow PyTorch Plugin
 
 This plugin uses the Kubeflow PyTorch Operator and provides an extremely simplified interface for executing distributed training using various PyTorch backends.
 
+This plugin can execute torch elastic training, which is equivalent to run `torchrun`. Elastic training can be executed
+in a single Pod (without requiring the PyTorch operator, see below) as well as in a distributed multi-node manner.
+
 To install the plugin, run the following command:
 
 ```bash
 pip install flytekitplugins-kfpytorch
 ```
 
 To set up PyTorch operator in the Flyte deployment's backend, follow the [PyTorch Operator Setup](https://docs.flyte.org/en/latest/deployment/plugin_setup/pytorch_operator.html) guide.
```

### Comparing `flytekitplugins-kfpytorch-1.6.0b0/flytekitplugins_kfpytorch.egg-info/PKG-INFO` & `flytekitplugins-kfpytorch-1.6.0b1/flytekitplugins_kfpytorch.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,7 +13,8 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
+Provides-Extra: elastic
```

### Comparing `flytekitplugins-kfpytorch-1.6.0b0/setup.py` & `flytekitplugins-kfpytorch-1.6.0b1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from setuptools import setup
 
 PLUGIN_NAME = "kfpytorch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
-plugin_requires = ["flytekit>=1.3.0b2,<2.0.0"]
+plugin_requires = ["cloudpickle", "flytekit>=1.3.0,<2.0.0", "flyteidl>=1.3.19"]
 
-__version__ = "1.6.0b0"
+__version__ = "1.6.0b1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Pytorch plugin for Flytekit",
     namespace_packages=["flytekitplugins"],
     packages=[f"flytekitplugins.{PLUGIN_NAME}"],
     install_requires=plugin_requires,
+    extras_require={
+        "elastic": ["torch>=1.9.0"],
+    },
     license="apache2",
     python_requires=">=3.8",
     classifiers=[
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
```

