# Comparing `tmp/tailors-fast-0.1.1.tar.gz` & `tmp/tailors-fast-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailors-fast-0.1.1.tar", max compression
+gzip compressed data, was "tailors-fast-0.2.0.tar", last modified: Wed May  3 04:18:29 2023, max compression
```

## Comparing `tailors-fast-0.1.1.tar` & `tailors-fast-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0      758 2022-12-23 03:53:00.949336 tailors-fast-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      133 2022-12-16 02:42:48.189777 tailors-fast-0.1.1/tailors_fast/__init__.py
--rw-r--r--   0        0        0      577 2022-12-15 11:57:27.562240 tailors-fast-0.1.1/tailors_fast/dates.py
--rw-r--r--   0        0        0      522 2022-12-16 02:46:01.369366 tailors-fast-0.1.1/tailors_fast/locations.py
--rw-r--r--   0        0        0     1772 2022-12-22 10:42:01.486580 tailors-fast-0.1.1/tailors_fast/model.py
--rw-r--r--   0        0        0     2249 2022-12-16 02:46:21.688941 tailors-fast-0.1.1/tailors_fast/split.py
--rw-r--r--   0        0        0    13144 2022-12-21 11:12:42.471297 tailors-fast-0.1.1/tailors_fast/stopwords.py
--rw-r--r--   0        0        0     1708 2022-12-15 11:57:27.562240 tailors-fast-0.1.1/tailors_fast/texts.py
--rw-r--r--   0        0        0     4006 2022-12-23 06:04:16.249152 tailors-fast-0.1.1/tailors_fast/tokenizer.py
--rw-r--r--   0        0        0     6172 2022-12-23 02:15:02.968387 tailors-fast-0.1.1/tailors_fast/train.py
--rw-r--r--   0        0        0      806 2022-12-23 06:17:09.156570 tailors-fast-0.1.1/setup.py
--rw-r--r--   0        0        0      533 2022-12-23 06:17:09.156755 tailors-fast-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-04-06 10:13:50.081854 tailors-fast-0.2.0/LICENSE
+-rw-r--r--   0        0        0       18 2023-04-06 10:13:50.081854 tailors-fast-0.2.0/README.md
+-rw-r--r--   0        0        0     1104 2023-04-17 09:50:08.048606 tailors-fast-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-05-03 04:18:04.178689 tailors-fast-0.2.0/tailors_fast/__init__.py
+-rw-r--r--   0        0        0     9648 2023-04-25 09:45:12.879567 tailors-fast-0.2.0/tailors_fast/dataset_from_eb.py
+-rw-r--r--   0        0        0      577 2022-12-15 11:57:27.562240 tailors-fast-0.2.0/tailors_fast/dates.py
+-rw-r--r--   0        0        0      522 2022-12-16 02:46:01.369366 tailors-fast-0.2.0/tailors_fast/locations.py
+-rw-r--r--   0        0        0     1764 2023-04-24 08:06:04.775256 tailors-fast-0.2.0/tailors_fast/model.py
+-rw-r--r--   0        0        0     2254 2023-04-17 09:50:39.524417 tailors-fast-0.2.0/tailors_fast/split.py
+-rw-r--r--   0        0        0    13144 2022-12-21 11:12:42.471297 tailors-fast-0.2.0/tailors_fast/stopwords.py
+-rw-r--r--   0        0        0     1708 2022-12-15 11:57:27.562240 tailors-fast-0.2.0/tailors_fast/texts.py
+-rw-r--r--   0        0        0     4074 2023-04-07 08:49:44.708009 tailors-fast-0.2.0/tailors_fast/tokenizer.py
+-rw-r--r--   0        0        0     6702 2023-04-25 07:02:49.146151 tailors-fast-0.2.0/tailors_fast/train.py
+-rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 tailors-fast-0.2.0/PKG-INFO
```

### Comparing `tailors-fast-0.1.1/tailors_fast/dates.py` & `tailors-fast-0.2.0/tailors_fast/dates.py`

 * *Files identical despite different names*

### Comparing `tailors-fast-0.1.1/tailors_fast/locations.py` & `tailors-fast-0.2.0/tailors_fast/locations.py`

 * *Files identical despite different names*

### Comparing `tailors-fast-0.1.1/tailors_fast/model.py` & `tailors-fast-0.2.0/tailors_fast/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,13 +38,13 @@
         model = fasttext.load_model(model_path)
         LOGGER.info(f"[FastModel] loaded, took: {sw.took()}")
         return model
 
     def predict(self, text: str, k=1, threshold=0.0):
         text = hao.strings.strip_to_none(text)
         if text is None:
-            return None, None
+            return []
         text = texts.fix_text(text)
         tokenized = self.tokenizer.cut_and_join(text)
         predictions, scores = self.model.predict(tokenized, k=k, threshold=threshold)
         preds = [(p[9:], s) for p, s in zip(predictions, scores)]
         return preds[0] if k == 1 else preds
```

### Comparing `tailors-fast-0.1.1/tailors_fast/split.py` & `tailors-fast-0.2.0/tailors_fast/split.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
 
 def process():
     print('[process]')
     conf = Conf()
     LOGGER.info(conf)
 
-    corpus_path = hao.paths.get('data/corpus/raw.jsonl')
-    train_path = hao.paths.get('data/corpus/fast/train.txt')
-    val_path = hao.paths.get('data/corpus/fast/val.txt')
+    dataset_path = hao.paths.get('data/dataset/raw.jsonl')
+    train_path = hao.paths.get('data/dataset/fast/train.txt')
+    val_path = hao.paths.get('data/dataset/fast/val.txt')
 
-    lines = open(corpus_path).readlines()
+    lines = open(dataset_path).readlines()
     entries = [json.loads(line) for line in lines if len(line.strip()) > 0]
     entries_general = entries[:conf.cut]
     entries_extra = entries[conf.cut:]
 
     if conf.seed:
         random.seed(conf.seed)
         random.shuffle(entries_general)
```

### Comparing `tailors-fast-0.1.1/tailors_fast/stopwords.py` & `tailors-fast-0.2.0/tailors_fast/stopwords.py`

 * *Files identical despite different names*

### Comparing `tailors-fast-0.1.1/tailors_fast/texts.py` & `tailors-fast-0.2.0/tailors_fast/texts.py`

 * *Files identical despite different names*

### Comparing `tailors-fast-0.1.1/tailors_fast/tokenizer.py` & `tailors-fast-0.2.0/tailors_fast/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,17 @@
             if len(items) > 0 and word == ' ' == items[-1]:
                 continue
             if not self.is_valid_word(word):
                 continue
             items.append(word.replace("\r", "").replace("\n", ""))
         return items
 
-    def cut_and_join(self, text, sep=' '):
+    def cut_and_join(self, text, sep=' ', min_len=3):
+        if len(text) <= min_len:
+            return text
         return sep.join(self.cut(text))
 
     def is_valid_word(self, word):
         len_word = len(word)
         if self._min_size > 1 and len_word < self._min_size:
             return False
         if len_word == 1 and not hao.strings.is_char_chinese(word):
```

### Comparing `tailors-fast-0.1.1/tailors_fast/train.py` & `tailors-fast-0.2.0/tailors_fast/train.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 import datetime
 import itertools
-import json
 import os
-from typing import List
+from typing import List, Optional
 
 import fasttext
 import hao
 import numpy as np
 from hao.namespaces import attr, from_args
 from hao.stopwatch import Stopwatch
 from sklearn.metrics import classification_report
@@ -22,60 +21,64 @@
     'tune_size': 'autotuneModelSize',
     'pretrained_file': 'pretrainedVectors',
     'min_count': 'minCount',
     'ngram': 'wordNgrams',
 }
 FILE_SKIP_ATTR = ('pretrained_file', 'train_file', 'val_file', 'tune_time', 'tune_size')
 
-@from_args
+@from_args(config='tailors.yml')
 class TrainConf(object):
-    exp: str = attr(str, required=True, help='experiment name')
-    file_train: str = attr(str, default='data/corpus/fast/train.txt', required=True)
-    file_val: str = attr(str, default='data/corpus/fast/val.txt', required=True)
-    file_labels: str = attr(str, default='data/corpus/fast/labels.json', required=False, help='json, key -> desc')
-    tune_time: int = attr(int, default=600, help='auto tune duration in seconds')
-    tune_size: str = attr(str, default="100M", help='auto tune model size')
-    lr: list = attr(List[float], default=[])
+    task: str = attr(str, help='task name in tailors.yml')
+    exp: str = attr(str, key='tasks.{task}.exp', required=True, help='experiment name')
+    dataset: str = attr(str, key='tasks.{task}.dataset', required=True, help='datasets.{dataset} in tailors.yml')
+    tune_time: int = attr(int, key='tasks.{task}.tune_time', default=600, help='auto tune duration in seconds')
+    tune_size: str = attr(str, key='tasks.{task}.tune_size', default="100M", help='auto tune model size')
+    lr: list = attr(List[float], key='tasks.{task}.lr', default=[])
     dim: list = attr(List[int], default=[50])
     ws: list = attr(List[int], default=[], help="window size")
-    epoch: list = attr(List[int], default=[])
-    neg: list = attr(List[int], default=[])
-    min_count: list = attr(List[int], default=[30])
-    ngram: list = attr(List[int], default=[3])
+    epoch: list = attr(List[int], key='tasks.{task}.epoch', default=[])
+    neg: list = attr(List[int], key='tasks.{task}.neg', default=[])
+    min_count: list = attr(List[int], key='tasks.{task}.min_count', default=[30])
+    ngram: list = attr(List[int], key='tasks.{task}.ngram', default=[3])
     minn: list = attr(List[int], default=[])
     maxn: list = attr(List[int], default=[])
-    loss: list = attr(List[str], choices=('ns', 'hs', 'softmax', 'ova'), default=[])
-    k: int = attr(int, default=1, help='top k')
-    threshold: float = attr(float, default=0.0, help='threshold for top k')
-    pretrained: str = attr(str)
+    loss: list = attr(List[str], key='tasks.{task}.loss', choices=('ns', 'hs', 'softmax', 'ova'), default=[])
+    k: int = attr(int, default=1, key='tasks.{task}.k', help='top k')
+    threshold: float = attr(float, key='tasks.{task}.threshold', default=0.0, help='threshold for top k')
+    pretrained: str = attr(str, key='tasks.{task}.pretrained')
 
 
-def train():
-    conf = TrainConf()
+def train(conf: Optional[TrainConf] = None):
+    conf = conf or TrainConf()
     LOGGER.info(conf)
-    train_file = hao.paths.get(conf.file_train)
-    val_file = hao.paths.get(conf.file_val)
-    labels_file = hao.paths.get(conf.file_labels)
+
+    dataset = hao.config.get(f"datasets.{conf.dataset}", config='tailors.yml')
+    datasets = dataset.get('datasets')
+    train_file = hao.paths.get(datasets.get('train'))
+    val_file = hao.paths.get(datasets.get('val'))
+    labels = dataset.get('meta', {}).get('labels')
+    if labels is None:
+        labels = get_labels_from_dataset([train_file, val_file])
+
     pretrained_file = hao.paths.get(conf.pretrained)
     k = conf.k
     threshold = conf.threshold
 
-    labels_all = get_all_labels(labels_file, [train_file, val_file])
-
+    results = []
     for lr, dim, epoch, ws, neg, min_count, ngram, minn, maxn, loss in itertools.product(
-            conf.lr or [None],
-            conf.dim or [None],
-            conf.epoch or [None],
-            conf.ws or [None],
-            conf.neg or [None],
-            conf.min_count or [None],
-            conf.ngram or [None],
-            conf.minn or [None],
-            conf.maxn or [None],
-            conf.loss or [None]
+        _params(conf, 'lr'),
+        _params(conf, 'dim'),
+        _params(conf, 'epoch'),
+        _params(conf, 'ws'),
+        _params(conf, 'neg'),
+        _params(conf, 'min_count'),
+        _params(conf, 'ngram'),
+        _params(conf, 'minn'),
+        _params(conf, 'maxn'),
+        _params(conf, 'loss'),
     ):
         params = {
             'pretrained_file': pretrained_file,
             'train_file': train_file,
             'val_file': val_file,
             'tune_time': conf.tune_time,
             'tune_size': conf.tune_size,
@@ -86,23 +89,28 @@
             'neg': neg,
             'min_count': min_count,
             'ngram': ngram,
             'minn': minn,
             'maxn': maxn,
             'loss': loss,
         }
-        train_and_val(conf.exp, k, threshold, labels_all, **params)
+        model_name, f1 = train_and_val(conf.exp, k, threshold, labels, **params)
+        results.append((model_name, f1))
+    return results
 
 
-def get_all_labels(labels_file: str, files: list):
-    assert labels_file is not None or len(files) > 0
-    if labels_file:
-        labels_mapping = json.loads(open(labels_file).read())
-        return list(labels_mapping.keys())
+def _params(conf: TrainConf, field: str) -> list:
+    v = getattr(conf, field)
+    if v is None or isinstance(v, list):
+        return v or [None]
+    return [v]
 
+
+def get_labels_from_dataset(files: list):
+    assert len(files) > 0
     labels = set()
     for file in files:
         with open(file) as f:
             for line in f:
                 splits = line.split('__label__')
                 for s in splits[1:]:
                     labels.add(s.strip())
@@ -124,43 +132,44 @@
     f1 = 2 * precision * recall / (precision + recall)
     LOGGER.info(f"val size: {n}, precision: {precision:.4}, recall: {recall:.4}, f1: {f1:.4}")
 
     model_params = '-'.join([
         f'{k}={v}' for k, v in kwargs.items()
         if k not in FILE_SKIP_ATTR and v is not None
     ])
-    model_name = f'{exp}-{date}-{model_params}-f1={f1:.4}.bin'
-    model_path = hao.paths.get('data/model', model_name)
+    model_file = f'data/model/{exp}-{date}-{model_params}-f1={f1:.4}.bin'
+    model_path = hao.paths.get(model_file)
     hao.paths.make_parent_dirs(model_path)
     model.save_model(model_path)
 
-    size = round(os.path.getsize(model_path) / (1024*1024), 2)
-    LOGGER.info(f'model saved to: {model_path}, size: {size}')
     for att in ('lr', 'dim', 'epoch', 'ws', 'neg', 'minCount', 'wordNgrams', 'minn', 'maxn'):
         LOGGER.info(f'{att: >25}: {getattr(model, att)}')
 
     lines = open(file_val).readlines()
     splits = [line.split('__label__') for line in lines]
     text, labels = list(zip(*[(s[0].strip(), [l.strip() for l in s[1:]]) for s in splits]))
     preds = [[p[9:] for p in prediction] for prediction in model.predict(list(text), k=k, threshold=threshold)[0]]
     indices_true = to_indices(labels, labels_all)
     indices_pred = to_indices(preds, labels_all)
     report = classification_report(indices_true, indices_pred, target_names=labels_all, digits=4, zero_division=0)
     LOGGER.info(f"\n{' classification report '.center(60, '=')}\n{report}")
+    size = round(os.path.getsize(model_path) / (1024*1024), 2)
+    LOGGER.info(f'model saved to: {model_file}, size: {size}')
 
     LOGGER.info(f'took: {sw.took()}')
-    return model_name, f1
+    return model_file, f1
 
 
 def to_indices(entries: List[list], labels):
     indices_labels = []
     for items in entries:
         indices = [0 for _ in labels]
         for label in items:
-            indices[labels.index(label)] = 1
+            if label in labels:
+                indices[labels.index(label)] = 1
         indices_labels.append(indices)
     return np.array(indices_labels)
 
 
 if __name__ == '__main__':
     try:
         train()
```

