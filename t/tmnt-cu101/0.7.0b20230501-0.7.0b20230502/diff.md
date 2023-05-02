# Comparing `tmp/tmnt-cu101-0.7.0b20230501.tar.gz` & `tmp/tmnt-cu101-0.7.0b20230502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmnt-cu101-0.7.0b20230501.tar", last modified: Mon May  1 23:02:21 2023, max compression
+gzip compressed data, was "tmnt-cu101-0.7.0b20230502.tar", last modified: Tue May  2 23:02:18 2023, max compression
```

## Comparing `tmnt-cu101-0.7.0b20230501.tar` & `tmnt-cu101-0.7.0b20230502.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:02:21.559843 tmnt-cu101-0.7.0b20230501/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-01 23:02:21.559843 tmnt-cu101-0.7.0b20230501/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 23:02:21.559843 tmnt-cu101-0.7.0b20230501/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:02:21.555843 tmnt-cu101-0.7.0b20230501/tmnt/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24818 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/bert_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:02:21.559843 tmnt-cu101-0.7.0b20230501/tmnt/classifier/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/classifier/load_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/classifier/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/classifier/train_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/common_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/data_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:02:21.559843 tmnt-cu101-0.7.0b20230501/tmnt/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19028 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/embeddings/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/embeddings/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/embeddings/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/embeddings/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    88743 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/eval_npmi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    31889 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:02:21.559843 tmnt-cu101-0.7.0b20230501/tmnt/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/preprocess/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15894 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/preprocess/vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    25950 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:02:21.559843 tmnt-cu101-0.7.0b20230501/tmnt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/utils/csv2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/utils/mat_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/utils/ngram_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/utils/pubmed_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-01 23:02:03.000000 tmnt-cu101-0.7.0b20230501/tmnt/utils/recalibrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:02:21.559843 tmnt-cu101-0.7.0b20230501/tmnt_cu101.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-01 23:02:21.000000 tmnt-cu101-0.7.0b20230501/tmnt_cu101.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-01 23:02:21.000000 tmnt-cu101-0.7.0b20230501/tmnt_cu101.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:02:21.000000 tmnt-cu101-0.7.0b20230501/tmnt_cu101.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-01 23:02:21.000000 tmnt-cu101-0.7.0b20230501/tmnt_cu101.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 23:02:21.000000 tmnt-cu101-0.7.0b20230501/tmnt_cu101.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:02:18.295031 tmnt-cu101-0.7.0b20230502/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-02 23:02:18.295031 tmnt-cu101-0.7.0b20230502/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 23:02:18.295031 tmnt-cu101-0.7.0b20230502/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:02:18.295031 tmnt-cu101-0.7.0b20230502/tmnt/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24818 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/bert_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:02:18.295031 tmnt-cu101-0.7.0b20230502/tmnt/classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/classifier/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/classifier/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/classifier/train_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/common_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/data_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14181 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:02:18.295031 tmnt-cu101-0.7.0b20230502/tmnt/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19028 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/embeddings/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/embeddings/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/embeddings/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/embeddings/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88749 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/eval_npmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23674 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31889 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:02:18.295031 tmnt-cu101-0.7.0b20230502/tmnt/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/preprocess/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15894 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/preprocess/vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25950 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:02:18.295031 tmnt-cu101-0.7.0b20230502/tmnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/utils/csv2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/utils/mat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/utils/ngram_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/utils/pubmed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-02 23:02:00.000000 tmnt-cu101-0.7.0b20230502/tmnt/utils/recalibrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:02:18.295031 tmnt-cu101-0.7.0b20230502/tmnt_cu101.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-02 23:02:18.000000 tmnt-cu101-0.7.0b20230502/tmnt_cu101.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-02 23:02:18.000000 tmnt-cu101-0.7.0b20230502/tmnt_cu101.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 23:02:18.000000 tmnt-cu101-0.7.0b20230502/tmnt_cu101.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-02 23:02:18.000000 tmnt-cu101-0.7.0b20230502/tmnt_cu101.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 23:02:18.000000 tmnt-cu101-0.7.0b20230502/tmnt_cu101.egg-info/top_level.txt
```

### Comparing `tmnt-cu101-0.7.0b20230501/LICENSE` & `tmnt-cu101-0.7.0b20230502/LICENSE`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/setup.py` & `tmnt-cu101-0.7.0b20230502/setup.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/bert_handling.py` & `tmnt-cu101-0.7.0b20230502/tmnt/bert_handling.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/classifier/load_data.py` & `tmnt-cu101-0.7.0b20230502/tmnt/classifier/load_data.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/classifier/model.py` & `tmnt-cu101-0.7.0b20230502/tmnt/classifier/model.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/classifier/train_sparse.py` & `tmnt-cu101-0.7.0b20230502/tmnt/classifier/train_sparse.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/common_params.py` & `tmnt-cu101-0.7.0b20230502/tmnt/common_params.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/configuration.py` & `tmnt-cu101-0.7.0b20230502/tmnt/configuration.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/data_loading.py` & `tmnt-cu101-0.7.0b20230502/tmnt/data_loading.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/distribution.py` & `tmnt-cu101-0.7.0b20230502/tmnt/distribution.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/embeddings/data.py` & `tmnt-cu101-0.7.0b20230502/tmnt/embeddings/data.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/embeddings/executors.py` & `tmnt-cu101-0.7.0b20230502/tmnt/embeddings/executors.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/embeddings/model.py` & `tmnt-cu101-0.7.0b20230502/tmnt/embeddings/model.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/embeddings/train.py` & `tmnt-cu101-0.7.0b20230502/tmnt/embeddings/train.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/estimator.py` & `tmnt-cu101-0.7.0b20230502/tmnt/estimator.py`

 * *Files 0% similar despite different names*

```diff
@@ -598,15 +598,14 @@
             elbo_losses = []
             lab_losses  = []
             for i, (data_batch, aux_batch) in enumerate(joint_loader):
                 with autograd.record():
                     elbo_ls, kl_loss, _, _, lab_loss, total_ls = self._get_losses(self.model, data_batch)
                     elbo_mean = elbo_ls.mean()
                 total_ls.backward()
-
                 if aux_batch is not None:
                     aux_data, = aux_batch
                     aux_data, _ = aux_data # ignore (null) label
                     aux_data = aux_data.as_in_context(self.ctx)
                     with autograd.record():
                         elbo_ls_a, kl_loss_a, _, _, total_ls_a = \
                             self._get_unlabeled_losses(self.model, aux_data)
@@ -1042,19 +1041,20 @@
             emb_size = len(self.vocabulary.embedding.idx_to_vec[0])
             for word in self.vocabulary.embedding._idx_to_token:
                 if (self.vocabulary.embedding[word] == mx.nd.zeros(emb_size)).sum() == emb_size:
                     self.vocabulary.embedding[word] = mx.nd.random.normal(0, 0.1, emb_size)
         else:
             emb_size = self.embedding_size
         model = \
-            CovariateBowVAEModel(n_covars=self.n_covars,
-                                 vocabulary=self.vocabulary, enc_dim=self.enc_hidden_dim, embedding_size=emb_size,
-                                 fixed_embedding=self.fixed_embedding, latent_distribution=self.latent_distribution,
+            CovariateBowVAEModel(enc_dim=self.enc_hidden_dim, embedding_size=emb_size, 
+                                 n_encoding_layers=self.n_encoding_layers, enc_dr=self.enc_dr, fixed_embedding=self.fixed_embedding,
+                                 n_covars=self.n_covars,
+                                 vocabulary=self.vocabulary, 
+                                 latent_distribution=self.latent_distribution,
                                  coherence_reg_penalty=self.coherence_reg_penalty, redundancy_reg_penalty=self.redundancy_reg_penalty,
-                                 batch_size=self.batch_size, n_encoding_layers=self.n_encoding_layers, enc_dr=self.enc_dr,
                                  ctx=self.ctx)
         return model
 
 
     def _get_losses(self, model, batch_data):
         # batch_data has form: ((data, covars),)
         (data,covars), = batch_data
```

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/eval_npmi.py` & `tmnt-cu101-0.7.0b20230502/tmnt/eval_npmi.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/inference.py` & `tmnt-cu101-0.7.0b20230502/tmnt/inference.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/modeling.py` & `tmnt-cu101-0.7.0b20230502/tmnt/modeling.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/preprocess/tokenizer.py` & `tmnt-cu101-0.7.0b20230502/tmnt/preprocess/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/preprocess/vectorizer.py` & `tmnt-cu101-0.7.0b20230502/tmnt/preprocess/vectorizer.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/selector.py` & `tmnt-cu101-0.7.0b20230502/tmnt/selector.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/trainer.py` & `tmnt-cu101-0.7.0b20230502/tmnt/trainer.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/utils/csv2json.py` & `tmnt-cu101-0.7.0b20230502/tmnt/utils/csv2json.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/utils/log_utils.py` & `tmnt-cu101-0.7.0b20230502/tmnt/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/utils/mat_utils.py` & `tmnt-cu101-0.7.0b20230502/tmnt/utils/mat_utils.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/utils/ngram_helpers.py` & `tmnt-cu101-0.7.0b20230502/tmnt/utils/ngram_helpers.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/utils/pubmed_utils.py` & `tmnt-cu101-0.7.0b20230502/tmnt/utils/pubmed_utils.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt/utils/recalibrate.py` & `tmnt-cu101-0.7.0b20230502/tmnt/utils/recalibrate.py`

 * *Files identical despite different names*

### Comparing `tmnt-cu101-0.7.0b20230501/tmnt_cu101.egg-info/SOURCES.txt` & `tmnt-cu101-0.7.0b20230502/tmnt_cu101.egg-info/SOURCES.txt`

 * *Files identical despite different names*

