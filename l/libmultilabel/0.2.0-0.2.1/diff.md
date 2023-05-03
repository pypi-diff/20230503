# Comparing `tmp/libmultilabel-0.2.0.tar.gz` & `tmp/libmultilabel-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/LibMultiLabel/LibMultiLabel/dist/.tmp-mea1opt5/libmultilabel-0.2.0.tar", last modified: Fri Apr 14 13:27:40 2023, max compression
+gzip compressed data, was "/home/runner/work/LibMultiLabel/LibMultiLabel/dist/.tmp-uzg9r_cd/libmultilabel-0.2.1.tar", last modified: Wed May  3 09:22:23 2023, max compression
```

## Comparing `libmultilabel-0.2.0.tar` & `libmultilabel-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22422 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/linear/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/linear/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/linear/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/linear/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/linear/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel/nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/bert_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/caml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/kim_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/labelwise_attention_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/networks/xml_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/libmultilabel/nn/nn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/libmultilabel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 13:27:28.000000 libmultilabel-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-14 13:27:40.000000 libmultilabel-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23621 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/linear/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/linear/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/linear/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/linear/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/linear/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/bert_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/caml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/kim_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/labelwise_attention_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/networks/xml_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/libmultilabel/nn/nn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/libmultilabel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 09:22:08.000000 libmultilabel-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-03 09:22:23.000000 libmultilabel-0.2.1/setup.cfg
```

### Comparing `libmultilabel-0.2.0/LICENSE` & `libmultilabel-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/PKG-INFO` & `libmultilabel-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmultilabel
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library for multi-label text classification
 Home-page: https://github.com/ASUS-AICS/LibMultiLabel
 Author: LibMultiLabel Team
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ASUS-AICS/LibMultiLabel/issues
 Project-URL: Documentation, https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 Project-URL: Source Code, https://github.com/ASUS-AICS/LibMultiLabel/
```

### Comparing `libmultilabel-0.2.0/README.md` & `libmultilabel-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel/common_utils.py` & `libmultilabel-0.2.1/libmultilabel/common_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -85,14 +85,23 @@
     with open(log_path, 'w') as fp:
         json.dump(result, fp)
 
     logging.info(f'Finish writing log to {log_path}.')
 
 
 def argsort_top_k(vals, k, axis=-1):
+    """Get the indices of the top-k elements in a 2D array.
+
+    Args:
+        vals: Array to sort.
+        k: Consider only the top k elements for each query
+        axis: Axis along which to sort. The default is -1 (the last axis).
+
+    Returns: Array of indices that sort vals along the specified axis.
+    """
     unsorted_top_k_idx = np.argpartition(vals, -k, axis=axis)[:, -k:]
     unsorted_top_k_scores = np.take_along_axis(
         vals, unsorted_top_k_idx, axis=axis)
     sorted_order = np.argsort(-unsorted_top_k_scores, axis=axis)
     sorted_top_k_idx = np.take_along_axis(
         unsorted_top_k_idx, sorted_order, axis=axis)
     return sorted_top_k_idx
```

### Comparing `libmultilabel-0.2.0/libmultilabel/linear/linear.py` & `libmultilabel-0.2.1/libmultilabel/linear/linear.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 __all__ = ['train_1vsrest',
            'train_thresholding',
            'train_cost_sensitive',
            'train_cost_sensitive_micro',
            'train_binary_and_multiclass',
            'predict_values',
-           'get_topk_labels']
+           'get_topk_labels',
+           'get_positive_labels']
 
 
 class FlatModel:
     def __init__(self, name: str,
                  weights: np.matrix,
                  bias: float,
                  thresholds: float | np.ndarray,
@@ -324,14 +325,17 @@
         y (np.ndarray): A +1/-1 array with dimensions number of instances * 1.
         x (sparse.csr_matrix): A matrix with dimensions number of instances * number of features.
         options (str): The option string passed to liblinear.
 
     Returns:
         np.matrix: the weights.
     """
+    if y.shape[0] == 0:
+        return np.matrix(np.zeros((x.shape[1], 1)))
+
     with silent_stderr():
         model = train(y, x, options)
 
     w = np.ctypeslib.as_array(model.w, (x.shape[1], 1))
     w = np.asmatrix(w)
     # Liblinear flips +1/-1 labels so +1 is always the first label,
     # but not if all labels are -1.
@@ -614,23 +618,46 @@
 
     Returns:
         np.ndarray: A matrix with dimension number of instances * number of classes.
     """
     return model.predict_values(x)
 
 
-def get_topk_labels(label_mapping: np.ndarray,
-                    preds: np.ndarray,
+def get_topk_labels(preds: np.ndarray,
+                    label_mapping: np.ndarray,
                     top_k: int = 5
-                    ) -> list[list[str]]:
-    """Get top k predictions from decision values.
+                    ) -> tuple[np.ndarray, np.ndarray]:
+    """Get labels and scores of top k predictions from decision values.
 
     Args:
+        preds (np.ndarray): A matrix of decision values with dimension (number of instances * number of classes).
         label_mapping (np.ndarray): A ndarray of class labels that maps each index (from 0 to ``num_class-1``) to its label.
-        preds (np.ndarray): A matrix of decision values with dimension number of instances * number of classes.
         top_k (int): Determine how many classes per instance should be predicted.
 
     Returns:
-        list of lists which contain top k labels.
+        Two 2d ndarray with first one containing predicted labels and the other containing corresponding scores.
+        Both have dimension (num_instances * top_k). 
+    """
+    idx = np.argpartition(preds, -top_k)[:, :-top_k-1:-1]
+    row_idx = np.arange(preds.shape[0])[:, None]
+    sorted_idx = idx[row_idx, np.argsort(-preds[row_idx, idx])]
+    scores = preds[row_idx, sorted_idx]
+    return label_mapping[sorted_idx], scores
+
+
+def get_positive_labels(preds: np.ndarray, label_mapping: np.ndarray) -> tuple[list[list[str]], list[list[float]]]:
+    """Get all labels and scores with positive decision value.
+
+    Args:
+        preds (np.ndarray): A matrix of decision values with dimension number of instances * number of classes.
+        label_mapping (np.ndarray): A ndarray of class labels that maps each index (from 0 to ``num_class-1``) to its label.
+
+    Returns:
+        Two 2d lists with first one containing predicted labels and the other containing corresponding scores.
     """
-    top_k_ind = np.argpartition(preds, -top_k)[:, :-top_k-1:-1]
-    return label_mapping[top_k_ind].tolist()
+    labels = []
+    scores = []
+    for ipred in preds:
+        pos_idx = np.where(ipred > 0)
+        labels.append(label_mapping[pos_idx[0]].tolist())
+        scores.append(ipred[pos_idx].tolist())
+    return labels, scores
```

### Comparing `libmultilabel-0.2.0/libmultilabel/linear/metrics.py` & `libmultilabel-0.2.1/libmultilabel/nn/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,221 +1,236 @@
-from __future__ import annotations
-
-import re
+from abc import abstractmethod
 
 import numpy as np
+import pytorch_lightning as pl
+import torch
+import torch.nn.functional as F
+import torch.optim as optim
 
-__all__ = ['get_metrics',
-           'compute_metrics',
-           'tabulate_metrics',
-           'MetricCollection']
-
-
-class RPrecision:
-    def __init__(self, top_k: int):
-        self.top_k = top_k
-        self.score = 0
-        self.num_sample = 0
-
-    def update(self, preds: np.ndarray, target: np.ndarray):
-        assert preds.shape == target.shape  # (batch_size, num_classes)
-        top_k_ind = np.argpartition(preds, -self.top_k)[:, -self.top_k:]
-        num_relevant = np.take_along_axis(
-            target, top_k_ind, axis=-1).sum(axis=-1)  # (batch_size, top_k)
-        self.score += np.nan_to_num(
-            num_relevant / np.minimum(self.top_k, target.sum(axis=-1)),
-            posinf=0.
-        ).sum()
-        self.num_sample += preds.shape[0]
-
-    def compute(self) -> float:
-        return self.score / self.num_sample
-
-    def reset(self):
-        self.score = 0
-        self.num_sample = 0
-
-
-class Precision:
-    def __init__(self, num_classes: int, average: str, top_k: int):
-        if average != 'samples':
-            raise ValueError('unsupported average')
-
-        self.top_k = top_k
-        self.score = 0
-        self.num_sample = 0
-
-    def update(self, preds: np.ndarray, target: np.ndarray):
-        assert preds.shape == target.shape  # (batch_size, num_classes)
-        top_k_ind = np.argpartition(preds, -self.top_k)[:, -self.top_k:]
-        num_relevant = np.take_along_axis(target, top_k_ind, -1).sum()
-        self.score += num_relevant / self.top_k
-        self.num_sample += preds.shape[0]
-
-    def compute(self) -> float:
-        return self.score / self.num_sample
-
-    def reset(self):
-        self.score = 0
-        self.num_sample = 0
-
-
-class F1:
-    def __init__(self, num_classes: int, average: str, multiclass=False):
-        self.num_classes = num_classes
-        if average not in {'macro', 'micro', 'another-macro'}:
-            raise ValueError('unsupported average')
-        self.average = average
-        self.multiclass = multiclass
-        self.tp = self.fp = self.fn = 0
+from ..common_utils import dump_log, argsort_top_k
+from ..nn.metrics import get_metrics, tabulate_metrics
 
-    def update(self, preds: np.ndarray, target: np.ndarray):
-        assert preds.shape == target.shape  # (batch_size, num_classes)
-        if self.multiclass:
-            max_idx = np.argmax(preds, axis=1).reshape(-1, 1)
-            preds = np.zeros(preds.shape)
-            np.put_along_axis(preds, max_idx, 1, axis=1)
-        else:
-            preds = preds > 0
-        self.tp += np.logical_and(target == 1, preds == 1).sum(axis=0)
-        self.fn += np.logical_and(target == 1, preds == 0).sum(axis=0)
-        self.fp += np.logical_and(target == 0, preds == 1).sum(axis=0)
-
-    def compute(self) -> float:
-        prev_settings = np.seterr('ignore')
-
-        if self.average == 'macro':
-            score = np.nansum(
-                2*self.tp / (2*self.tp + self.fp + self.fn)) / self.num_classes
-        elif self.average == 'micro':
-            score = np.nan_to_num(2*np.sum(self.tp) /
-                                  np.sum(2*self.tp + self.fp + self.fn))
-        elif self.average == 'another-macro':
-            macro_prec = np.nansum(
-                self.tp / (self.tp + self.fp)) / self.num_classes
-            macro_recall = np.nansum(
-                self.tp / (self.tp + self.fn)) / self.num_classes
-            score = np.nan_to_num(
-                2 * macro_prec * macro_recall / (macro_prec + macro_recall))
-
-        np.seterr(**prev_settings)
-        return score
-
-    def reset(self):
-        self.tp = self.fp = self.fn = 0
-
-
-class MetricCollection(dict):
-    """A collection of metrics created by get_metrics.
-    MetricCollection computes metric values in two steps. First, batches of
-    decision values and labels are added with update(). After all instances have been
-    added, compute() computes the metric values from the accumulated batches.
+
+class MultiLabelModel(pl.LightningModule):
+    """Abstract class handling Pytorch Lightning training flow
+
+    Args:
+        num_classes (int): Total number of classes.
+        learning_rate (float, optional): Learning rate for optimizer. Defaults to 0.0001.
+        optimizer (str, optional): Optimizer name (i.e., sgd, adam, or adamw). Defaults to 'adam'.
+        momentum (float, optional): Momentum factor for SGD only. Defaults to 0.9.
+        weight_decay (int, optional): Weight decay factor. Defaults to 0.
+        metric_threshold (float, optional): The decision value threshold over which a label is predicted as positive. Defaults to 0.5.
+        monitor_metrics (list, optional): Metrics to monitor while validating. Defaults to None.
+        log_path (str): Path to a directory holding the log files and models.
+        multiclass (bool, optional): Enable multiclass mode. Defaults to False.
+        silent (bool, optional): Enable silent mode. Defaults to False.
+        save_k_predictions (int, optional): Save top k predictions on test set. Defaults to 0.
     """
 
-    def __init__(self, metrics):
-        self.metrics = metrics
+    def __init__(
+        self,
+        num_classes,
+        learning_rate=0.0001,
+        optimizer='adam',
+        momentum=0.9,
+        weight_decay=0,
+        metric_threshold=0.5,
+        monitor_metrics=None,
+        log_path=None,
+        multiclass=False,
+        silent=False,
+        save_k_predictions=0,
+        **kwargs
+    ):
+        super().__init__()
+
+        # optimizer
+        self.learning_rate = learning_rate
+        self.optimizer = optimizer
+        self.momentum = momentum
+        self.weight_decay = weight_decay
+
+        # dump log
+        self.log_path = log_path
+        self.silent = silent
+        self.save_k_predictions = save_k_predictions
 
-    def update(self, preds: np.ndarray, target: np.ndarray):
-        """Adds a batch of decision values and labels.
+        # metrics for evaluation
+        self.multiclass = multiclass
+        top_k = 1 if self.multiclass else None
+        self.eval_metric = get_metrics(
+            metric_threshold, monitor_metrics, num_classes, top_k=top_k)
+
+    @abstractmethod
+    def shared_step(self, batch):
+        """Return loss and predicted logits"""
+        return NotImplemented
 
-        Args:
-            preds (np.ndarray): A matrix of decision values with dimensions number of instances * number of classes.
-            target (np.ndarray): A 0/1 matrix of labels with dimensions number of instances * number of classes.
+    def configure_optimizers(self):
+        """Initialize an optimizer for the free parameters of the network.
         """
-        assert preds.shape == target.shape  # (batch_size, num_classes)
-        for metric in self.metrics.values():
-            metric.update(preds, target)
+        parameters = [p for p in self.parameters() if p.requires_grad]
+        optimizer_name = self.optimizer
+        if optimizer_name == 'sgd':
+            optimizer = optim.SGD(parameters, self.learning_rate,
+                                  momentum=self.momentum,
+                                  weight_decay=self.weight_decay)
+        elif optimizer_name == 'adam':
+            optimizer = optim.Adam(parameters,
+                                   weight_decay=self.weight_decay,
+                                   lr=self.learning_rate)
+        elif optimizer_name == 'adamw':
+            optimizer = optim.AdamW(parameters,
+                                    weight_decay=self.weight_decay,
+                                    lr=self.learning_rate)
+        elif optimizer_name == 'adamax':
+            optimizer = optim.Adamax(parameters,
+                                     weight_decay=self.weight_decay,
+                                     lr=self.learning_rate)
+        else:
+            raise RuntimeError(
+                'Unsupported optimizer: {self.optimizer}')
 
-    def compute(self) -> dict[str, float]:
-        """Computes the metrics from the accumulated batches of decision values and labels.
+        torch.nn.utils.clip_grad_value_(parameters, 0.5)
 
-        Returns:
-            dict[str, float]: A dictionary of metric values.
-        """
-        ret = {}
-        for name, metric in self.metrics.items():
-            ret[name] = metric.compute()
-        return ret
+        return optimizer
 
-    def reset(self):
-        """Clears the accumulated batches of decision values and labels.
-        """
-        for metric in self.metrics.values():
-            metric.reset()
+    def training_step(self, batch, batch_idx):
+        loss, _ = self.shared_step(batch)
+        return loss
 
+    def validation_step(self, batch, batch_idx):
+        return self._shared_eval_step(batch, batch_idx)
 
-def get_metrics(monitor_metrics: list[str],
-                num_classes: int,
-                multiclass: bool = False
-                ) -> MetricCollection:
-    """Get a collection of metrics by their names.
-    See MetricCollection for more details.
+    def validation_step_end(self, batch_parts):
+        return self._shared_eval_step_end(batch_parts)
 
-    Args:
-        monitor_metrics (list[str]): A list of metric names.
-        num_classes (int): The number of classes.
-        multiclass (bool, optional): Enable multiclass mode. Defaults to False.
+    def validation_epoch_end(self, step_outputs):
+        return self._shared_eval_epoch_end(step_outputs, 'val')
 
-    Returns:
-        MetricCollection: A metric collection of the list of metrics.
-    """
-    if monitor_metrics is None:
-        monitor_metrics = []
-    metrics = {}
-    for metric in monitor_metrics:
-        if re.match('P@\d+', metric):
-            metrics[metric] = Precision(
-                num_classes, average='samples', top_k=int(metric[2:]))
-        elif re.match('RP@\d+', metric):
-            metrics[metric] = RPrecision(top_k=int(metric[3:]))
-        elif metric in {'Another-Macro-F1', 'Macro-F1', 'Micro-F1'}:
-            metrics[metric] = F1(num_classes,
-                                 average=metric[:-3].lower(),
-                                 multiclass=multiclass)
-        else:
-            raise ValueError(f'invalid metric: {metric}')
+    def test_step(self, batch, batch_idx):
+        return self._shared_eval_step(batch, batch_idx)
 
-    return MetricCollection(metrics)
+    def test_step_end(self, batch_parts):
+        return self._shared_eval_step_end(batch_parts)
 
+    def test_epoch_end(self, step_outputs):
+        return self._shared_eval_epoch_end(step_outputs, 'test')
 
-def compute_metrics(preds: np.ndarray,
-                    target: np.ndarray,
-                    monitor_metrics: list[str],
-                    multiclass: bool = False
-                    ) -> dict[str, float]:
-    """Compute metrics with decision values and labels.
-    See get_metrics and MetricCollection if decision values and labels are too
-    large to hold in memory.
+    def _shared_eval_step(self, batch, batch_idx):
+        loss, pred_logits = self.shared_step(batch)
+        return {'batch_idx': batch_idx,
+                'loss': loss,
+                'pred_scores': torch.sigmoid(pred_logits),
+                'target': batch['label']}
 
+    def _shared_eval_step_end(self, batch_parts):
+        return self.eval_metric.update(
+            preds=batch_parts['pred_scores'],
+            target=batch_parts['target'],
+            loss=batch_parts['loss']
+        )
 
-    Args:
-        preds (np.ndarray): A matrix of decision values with dimensions number of instances * number of classes.
-        target (np.ndarray): A 0/1 matrix of labels with dimensions number of instances * number of classes.
-        monitor_metrics (list[str]): A list of metric names.
-        multiclass (bool, optional): Enable multiclass mode. Defaults to False.
+    def _shared_eval_epoch_end(self, step_outputs, split):
+        """Get scores such as `Micro-F1`, `Macro-F1`, and monitor metrics defined
+        in the configuration file in the end of an epoch.
 
-    Returns:
-        dict[str, float]: A dictionary of metric values.
-    """
-    assert preds.shape == target.shape
+        Args:
+            step_outputs (list): List of the return values from the val or test step end.
+            split (str): One of the `val` or `test`.
 
-    metric = get_metrics(monitor_metrics, preds.shape[1], multiclass)
-    metric.update(preds, target)
-    return metric.compute()
+        Returns:
+            metric_dict (dict): Scores for all metrics in the dictionary format.
+        """
+        metric_dict = self.eval_metric.compute()
+        self.log_dict(metric_dict)
+        for k, v in metric_dict.items():
+            metric_dict[k] = v.item()
+        if self.log_path:
+            dump_log(metrics=metric_dict, split=split, log_path=self.log_path)
+        self.print(tabulate_metrics(metric_dict, split))
+        self.eval_metric.reset()
+        return metric_dict
+
+    def predict_step(self, batch, batch_idx):
+        """`predict_step` is triggered when calling `trainer.predict()`.
+        This function is used to get the top-k labels and their prediction scores.
 
+        Args:
+            batch (dict): A batch of text and label.
+            batch_idx (int): Index of current batch.
 
-def tabulate_metrics(metric_dict: dict[str, float], split: str) -> str:
-    """Convert a dictionary of metric values into a pretty formatted string for printing.
+        Returns:
+            dict: Top k label indexes and the prediction scores.
+        """
+        _, pred_logits = self.shared_step(batch)
+        pred_scores = pred_logits.detach().cpu().numpy()
+        k = self.save_k_predictions
+        top_k_idx = argsort_top_k(pred_scores, k, axis=1)
+        top_k_scores = np.take_along_axis(pred_scores, top_k_idx, axis=1)
+
+        return {'top_k_pred': top_k_idx,
+                'top_k_pred_scores': top_k_scores}
+
+    def print(self, *args, **kwargs):
+        """Prints only from process 0 and not in silent mode. Use this in any
+        distributed mode to log only once."""
+
+        if not self.silent:
+            # print() in LightningModule to print only from process 0
+            super().print(*args, **kwargs)
 
-    Args:
-        metric_dict (dict[str, float]): A dictionary of metric values.
-        split (str): Name of the data split.
 
-    Returns:
-        str: Pretty formatted string.
+class Model(MultiLabelModel):
+    """A class that implements `MultiLabelModel` for initializing and training a neural network.
+
+    Args:
+        classes (list): List of class names.
+        word_dict (torchtext.vocab.Vocab): A vocab object which maps tokens to indices.
+        embed_vecs (torch.Tensor): The pre-trained word vectors of shape (vocab_size, embed_dim).
+        network (nn.Module): Network (i.e., CAML, KimCNN, or XMLCNN).
+        loss_function (str, optional): Loss function name (i.e., binary_cross_entropy_with_logits,
+            cross_entropy). Defaults to 'binary_cross_entropy_with_logits'.
+        log_path (str): Path to a directory holding the log files and models.
     """
-    msg = f'====== {split} dataset evaluation result =======\n'
-    header = '|'.join([f'{k:^18}' for k in metric_dict.keys()])
-    values = '|'.join([f'{x:^18.4f}' if isinstance(x, (np.floating,
-                      float)) else f'{x:^18}' for x in metric_dict.values()])
-    msg += f"|{header}|\n|{'-----------------:|' * len(metric_dict)}\n|{values}|\n"
-    return msg
+
+    def __init__(
+        self,
+        classes,
+        word_dict,
+        embed_vecs,
+        network,
+        loss_function='binary_cross_entropy_with_logits',
+        log_path=None,
+        **kwargs
+    ):
+        super().__init__(num_classes=len(classes), log_path=log_path, **kwargs)
+        self.save_hyperparameters()
+        self.word_dict = word_dict
+        self.embed_vecs = embed_vecs
+        self.classes = classes
+        self.network = network
+        self.configure_loss_function(loss_function)
+
+    def configure_loss_function(self, loss_function):
+        assert hasattr(F, loss_function), """
+            Invalid `loss_function`. Make sure the loss function is defined here:
+            https://pytorch.org/docs/stable/nn.functional.html#loss-functions"""
+        self.loss_function = getattr(F, loss_function)
+
+    def shared_step(self, batch):
+        """Return loss and predicted logits of the network.
+
+        Args:
+            batch (dict): A batch of text and label.
+
+        Returns:
+            loss (torch.Tensor): Loss between target and predict logits.
+            pred_logits (torch.Tensor): The predict logits (batch_size, num_classes).
+        """
+        target_labels = batch['label']
+        outputs = self.network(batch)
+        pred_logits = outputs['logits']
+        loss = self.loss_function(pred_logits, target_labels.float())
+
+        return loss, pred_logits
```

### Comparing `libmultilabel-0.2.0/libmultilabel/linear/preprocessor.py` & `libmultilabel-0.2.1/libmultilabel/linear/preprocessor.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel/linear/tree.py` & `libmultilabel-0.2.1/libmultilabel/linear/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             pred = instance_preds[slice]
             scores[node.label_map] = np.exp(score - np.maximum(0, 1 - pred)**2)
         return scores
 
 
 def train_tree(y: sparse.csr_matrix,
                x: sparse.csr_matrix,
-               options: str,
+               options: str = '',
                K=100, dmax=10,
                verbose: bool = True,
                ) -> TreeModel:
     """Trains a linear model for multiabel data using a divide-and-conquer strategy.
     The algorithm used is based on https://github.com/xmc-aalto/bonsai.
 
     Args:
@@ -171,15 +171,15 @@
     """
     if d >= dmax or label_representation.shape[0] <= K:
         return Node(label_map=label_map,
                     children=[])
 
     metalabels = sklearn.cluster.KMeans(
         K,
-        random_state=np.random.randint(2**32),
+        random_state=np.random.randint(2**31 - 1),
         n_init=1,
         max_iter=300,
         tol=0.0001,
         algorithm='elkan',
     ).fit(label_representation).labels_
 
     children = []
```

### Comparing `libmultilabel-0.2.0/libmultilabel/linear/utils.py` & `libmultilabel-0.2.1/libmultilabel/linear/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,20 +105,32 @@
         preds = self.predict(X)
         metrics.update(preds, y.toarray())
         metric_dict = metrics.compute()
         return metric_dict[self.scoring_metric]
 
 
 class GridSearchCV(sklearn.model_selection.GridSearchCV):
+    """A customized `sklearn.model_selection.GridSearchCV`` class for Liblinear.
+    The usage is similar to sklearn's, except that the parameter ``scoring`` is unavailable. Instead, specify ``scoring_metric`` in ``MultiLabelEstimator`` in the Pipeline.
+
+    Args:
+        pipeline (sklearn.pipeline.Pipeline): A sklearn Pipeline for grid search.
+        param_grid (dict): Search space for a grid search containing a dictionary of
+            parameters and their corresponding list of candidate values.
+        n_jobs (int, optional): Number of CPU cores run in parallel. Defaults to None.
+    """
     _required_parameters = ['pipeline', 'param_grid']
 
     def __init__(self, pipeline: sklearn.pipeline.Pipeline, param_grid: dict, n_jobs=None, **kwargs):
         assert isinstance(pipeline, sklearn.pipeline.Pipeline)
         if n_jobs is not None and n_jobs > 1:
             param_grid = self._set_singlecore_options(pipeline, param_grid)
+        if 'scoring' in kwargs.keys():
+            raise ValueError(
+                'Please specify the validation metric with `MultiLabelEstimator.scoring_metric` in the Pipeline instead of using the parameter `scoring`.')
 
         super().__init__(
             estimator=pipeline,
             n_jobs=n_jobs,
             param_grid=param_grid,
             **kwargs
         )
```

### Comparing `libmultilabel-0.2.0/libmultilabel/logging.py` & `libmultilabel-0.2.1/libmultilabel/logging.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel/nn/data_utils.py` & `libmultilabel-0.2.1/libmultilabel/nn/data_utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel/nn/metrics.py` & `libmultilabel-0.2.1/libmultilabel/nn/metrics.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel/nn/networks/__init__.py` & `libmultilabel-0.2.1/libmultilabel/nn/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel/nn/networks/bert.py` & `libmultilabel-0.2.1/libmultilabel/nn/networks/bert.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel/nn/networks/bert_attention.py` & `libmultilabel-0.2.1/libmultilabel/nn/networks/bert_attention.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel/nn/networks/caml.py` & `libmultilabel-0.2.1/libmultilabel/nn/networks/caml.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel/nn/networks/kim_cnn.py` & `libmultilabel-0.2.1/libmultilabel/nn/networks/kim_cnn.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel/nn/networks/labelwise_attention_networks.py` & `libmultilabel-0.2.1/libmultilabel/nn/networks/labelwise_attention_networks.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel/nn/networks/modules.py` & `libmultilabel-0.2.1/libmultilabel/nn/networks/modules.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel/nn/networks/xml_cnn.py` & `libmultilabel-0.2.1/libmultilabel/nn/networks/xml_cnn.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel/nn/nn_utils.py` & `libmultilabel-0.2.1/libmultilabel/nn/nn_utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/libmultilabel.egg-info/PKG-INFO` & `libmultilabel-0.2.1/libmultilabel.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmultilabel
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library for multi-label text classification
 Home-page: https://github.com/ASUS-AICS/LibMultiLabel
 Author: LibMultiLabel Team
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ASUS-AICS/LibMultiLabel/issues
 Project-URL: Documentation, https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 Project-URL: Source Code, https://github.com/ASUS-AICS/LibMultiLabel/
```

### Comparing `libmultilabel-0.2.0/libmultilabel.egg-info/SOURCES.txt` & `libmultilabel-0.2.1/libmultilabel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.2.0/setup.cfg` & `libmultilabel-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libmultilabel
-version = 0.2.0
+version = 0.2.1
 author = LibMultiLabel Team
 license = MIT License
 license_file = LICENSE
 description = A library for multi-label text classification
 long_description = See documentation here: https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 url = https://github.com/ASUS-AICS/LibMultiLabel
 project_urls =
```

