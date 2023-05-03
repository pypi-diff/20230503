# Comparing `tmp/pygmtools-0.3.7.tar.gz` & `tmp/pygmtools-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtools-0.3.7.tar", last modified: Thu Apr 27 15:32:24 2023, max compression
+gzip compressed data, was "pygmtools-0.3.8.tar", last modified: Wed May  3 10:13:43 2023, max compression
```

## Comparing `pygmtools-0.3.7.tar` & `pygmtools-0.3.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:32:24.621053 pygmtools-0.3.7/
--rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-04-27 15:32:08.000000 pygmtools-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 15:32:08.000000 pygmtools-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-04-27 15:32:24.621053 pygmtools-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-04-27 15:32:08.000000 pygmtools-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:32:24.617053 pygmtools-0.3.7/pygmtools/
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26415 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    47379 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/classic_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    57869 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/dataset_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    57459 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/jittor_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/jittor_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    75786 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/linear_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/mindspore_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    43089 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/multi_graph_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    69204 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/neural_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    59271 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/numpy_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    56491 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/paddle_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/paddle_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    57454 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/pytorch_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    23046 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/tensorflow_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-04-27 15:32:08.000000 pygmtools-0.3.7/pygmtools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:32:24.617053 pygmtools-0.3.7/pygmtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-04-27 15:32:24.000000 pygmtools-0.3.7/pygmtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-27 15:32:24.000000 pygmtools-0.3.7/pygmtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:32:24.000000 pygmtools-0.3.7/pygmtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-27 15:32:24.000000 pygmtools-0.3.7/pygmtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 15:32:24.000000 pygmtools-0.3.7/pygmtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:32:24.621053 pygmtools-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-27 15:32:08.000000 pygmtools-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:32:24.621053 pygmtools-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-04-27 15:32:08.000000 pygmtools-0.3.7/tests/test_classic_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-27 15:32:08.000000 pygmtools-0.3.7/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-27 15:32:08.000000 pygmtools-0.3.7/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-27 15:32:08.000000 pygmtools-0.3.7/tests/test_multi_graph_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-27 15:32:08.000000 pygmtools-0.3.7/tests/test_neural_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-27 15:32:08.000000 pygmtools-0.3.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:43.109770 pygmtools-0.3.8/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-05-03 10:13:27.000000 pygmtools-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 10:13:27.000000 pygmtools-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-03 10:13:43.109770 pygmtools-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-03 10:13:27.000000 pygmtools-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:43.105770 pygmtools-0.3.8/pygmtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26415 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47379 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/classic_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57869 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/dataset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57459 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/jittor_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/jittor_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75786 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/linear_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/mindspore_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43089 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/multi_graph_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69204 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/neural_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59271 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/numpy_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56491 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/paddle_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/paddle_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57454 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/pytorch_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23046 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/tensorflow_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-05-03 10:13:28.000000 pygmtools-0.3.8/pygmtools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:43.109770 pygmtools-0.3.8/pygmtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-03 10:13:43.000000 pygmtools-0.3.8/pygmtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-03 10:13:43.000000 pygmtools-0.3.8/pygmtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:13:43.000000 pygmtools-0.3.8/pygmtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-03 10:13:43.000000 pygmtools-0.3.8/pygmtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 10:13:43.000000 pygmtools-0.3.8/pygmtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 10:13:43.109770 pygmtools-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-03 10:13:28.000000 pygmtools-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:13:43.109770 pygmtools-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-05-03 10:13:28.000000 pygmtools-0.3.8/tests/test_classic_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-03 10:13:28.000000 pygmtools-0.3.8/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-03 10:13:28.000000 pygmtools-0.3.8/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-03 10:13:28.000000 pygmtools-0.3.8/tests/test_multi_graph_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-05-03 10:13:28.000000 pygmtools-0.3.8/tests/test_neural_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-03 10:13:28.000000 pygmtools-0.3.8/tests/test_utils.py
```

### Comparing `pygmtools-0.3.7/PKG-INFO` & `pygmtools-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.7
+Version: 0.3.8
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
@@ -136,15 +136,15 @@
 
 <img src="https://pygmtools.readthedocs.io/en/latest/_images/paddle_logo.png" alt="paddle logo" width="200"/>
 
 * [Tensorflow](https://tensorflow.google.cn/) (GPU friendly, deep learning friendly)
 
 <img src="https://pygmtools.readthedocs.io/en/latest/_images/tensorflow_logo.png" alt="tensorflow logo" width="200"/>
 
-### Development status (0.3.7)
+### Development status (0.3.8)
 
 |                     | Numpy | PyTorch | Jittor | PaddlePaddle | Tensorflow | MindSpore |
 | ------------------- | ----- | ------- | ------ | ------------ | ---------- | --------- |
 | Linear Solvers      | ✔     | ✔       | ✔      | ✔            | ✔         | ✔        |
 | Classic Solvers     | ✔     | ✔       | ✔      | ✔            | ✔         | ✔        |
 | Multi-Graph Solvers | ✔    | ✔       | ✔      | ✔            | 📆         | 📆        |
 | Neural Solvers      | ✔    | ✔       | ✔      | ✔           | 📆         | 📆        |
```

### Comparing `pygmtools-0.3.7/README.md` & `pygmtools-0.3.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 <img src="https://pygmtools.readthedocs.io/en/latest/_images/paddle_logo.png" alt="paddle logo" width="200"/>
 
 * [Tensorflow](https://tensorflow.google.cn/) (GPU friendly, deep learning friendly)
 
 <img src="https://pygmtools.readthedocs.io/en/latest/_images/tensorflow_logo.png" alt="tensorflow logo" width="200"/>
 
-### Development status (0.3.7)
+### Development status (0.3.8)
 
 |                     | Numpy | PyTorch | Jittor | PaddlePaddle | Tensorflow | MindSpore |
 | ------------------- | ----- | ------- | ------ | ------------ | ---------- | --------- |
 | Linear Solvers      | ✔     | ✔       | ✔      | ✔            | ✔         | ✔        |
 | Classic Solvers     | ✔     | ✔       | ✔      | ✔            | ✔         | ✔        |
 | Multi-Graph Solvers | ✔    | ✔       | ✔      | ✔            | 📆         | 📆        |
 | Neural Solvers      | ✔    | ✔       | ✔      | ✔           | 📆         | 📆        |
```

### Comparing `pygmtools-0.3.7/pygmtools/__init__.py` & `pygmtools-0.3.8/pygmtools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .benchmark import Benchmark
 from .linear_solvers import sinkhorn, hungarian
 from .classic_solvers import rrwm, sm, ipfp
 from .multi_graph_solvers import cao, mgm_floyd, gamgm
 from .neural_solvers import pca_gm, ipca_gm, cie, ngm
 import pygmtools.utils as utils
 BACKEND = 'numpy'
-__version__ = '0.3.7'
+__version__ = '0.3.8'
 __author__ = 'ThinkLab at SJTU'
 
 
 def env_report():
     """
     Print environment report
     """
```

### Comparing `pygmtools-0.3.7/pygmtools/benchmark.py` & `pygmtools-0.3.8/pygmtools/benchmark.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/classic_solvers.py` & `pygmtools-0.3.8/pygmtools/classic_solvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
             >>> optim = nn.SGD(model.parameters(), lr=0.1)
             >>> X = model(K, n1, n2)
             >>> loss = X.sum()
             >>> optim.step(loss)
             >>> len(jt.nonzero(K.opt_grad(optim)))
             2560
 
-    .. dropdown:: mindspore Example
+    .. dropdown:: MindSpore Example
 
         ::
 
             >>> import mindspore
             >>> import pygmtools as pygm
             >>> pygm.BACKEND = 'mindspore'
             >>> _ = mindspore.set_seed(1)
@@ -609,15 +609,15 @@
             >>> optim = nn.SGD(model.parameters(), lr=0.1)
             >>> X = model(K, n1, n2, beta=100)
             >>> loss = X.sum()
             >>> optim.step(loss)
             >>> len(jt.nonzero(K.opt_grad(optim)))
             1536
 
-    .. dropdown:: mindspore Example
+    .. dropdown:: MindSpore Example
 
         ::
 
             >>> import mindspore
             >>> import pygmtools as pygm
             >>> pygm.BACKEND = 'mindspore'
             >>> _ = mindspore.set_seed(1)
@@ -933,15 +933,15 @@
                     [0. 0. 0. 1.]
                     [0. 1. 0. 0.]], dtype=float32)
 
             # Accuracy
             >>> (pygm.hungarian(X) * X_gt).sum() / X_gt.sum()
             jt.Var([1.], dtype=float32)
 
-    .. dropdown:: mindspore Example
+    .. dropdown:: MindSpore Example
 
         ::
 
             >>> import mindspore
             >>> import pygmtools as pygm
             >>> pygm.BACKEND = 'mindspore'
             >>> _ = mindspore.set_seed(1)
```

### Comparing `pygmtools-0.3.7/pygmtools/dataset.py` & `pygmtools-0.3.8/pygmtools/dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/dataset_config.py` & `pygmtools-0.3.8/pygmtools/dataset_config.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/jittor_backend.py` & `pygmtools-0.3.8/pygmtools/jittor_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/jittor_modules.py` & `pygmtools-0.3.8/pygmtools/jittor_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/linear_solvers.py` & `pygmtools-0.3.8/pygmtools/linear_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/mindspore_backend.py` & `pygmtools-0.3.8/pygmtools/mindspore_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/multi_graph_solvers.py` & `pygmtools-0.3.8/pygmtools/multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/neural_solvers.py` & `pygmtools-0.3.8/pygmtools/neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/numpy_backend.py` & `pygmtools-0.3.8/pygmtools/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/numpy_modules.py` & `pygmtools-0.3.8/pygmtools/numpy_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/paddle_backend.py` & `pygmtools-0.3.8/pygmtools/paddle_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/paddle_modules.py` & `pygmtools-0.3.8/pygmtools/paddle_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/pytorch_backend.py` & `pygmtools-0.3.8/pygmtools/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/pytorch_modules.py` & `pygmtools-0.3.8/pygmtools/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/tensorflow_backend.py` & `pygmtools-0.3.8/pygmtools/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools/utils.py` & `pygmtools-0.3.8/pygmtools/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/pygmtools.egg-info/PKG-INFO` & `pygmtools-0.3.8/pygmtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.7
+Version: 0.3.8
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
@@ -136,15 +136,15 @@
 
 <img src="https://pygmtools.readthedocs.io/en/latest/_images/paddle_logo.png" alt="paddle logo" width="200"/>
 
 * [Tensorflow](https://tensorflow.google.cn/) (GPU friendly, deep learning friendly)
 
 <img src="https://pygmtools.readthedocs.io/en/latest/_images/tensorflow_logo.png" alt="tensorflow logo" width="200"/>
 
-### Development status (0.3.7)
+### Development status (0.3.8)
 
 |                     | Numpy | PyTorch | Jittor | PaddlePaddle | Tensorflow | MindSpore |
 | ------------------- | ----- | ------- | ------ | ------------ | ---------- | --------- |
 | Linear Solvers      | ✔     | ✔       | ✔      | ✔            | ✔         | ✔        |
 | Classic Solvers     | ✔     | ✔       | ✔      | ✔            | ✔         | ✔        |
 | Multi-Graph Solvers | ✔    | ✔       | ✔      | ✔            | 📆         | 📆        |
 | Neural Solvers      | ✔    | ✔       | ✔      | ✔           | 📆         | 📆        |
```

### Comparing `pygmtools-0.3.7/pygmtools.egg-info/SOURCES.txt` & `pygmtools-0.3.8/pygmtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/setup.py` & `pygmtools-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/tests/test_classic_solvers.py` & `pygmtools-0.3.8/tests/test_classic_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/tests/test_dataset.py` & `pygmtools-0.3.8/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/tests/test_misc.py` & `pygmtools-0.3.8/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/tests/test_multi_graph_solvers.py` & `pygmtools-0.3.8/tests/test_multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/tests/test_neural_solvers.py` & `pygmtools-0.3.8/tests/test_neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.7/tests/test_utils.py` & `pygmtools-0.3.8/tests/test_utils.py`

 * *Files identical despite different names*

