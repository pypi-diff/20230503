# Comparing `tmp/tailors-trainer-0.1.3.tar.gz` & `tmp/tailors-trainer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailors-trainer-0.1.3.tar", max compression
+gzip compressed data, was "tailors-trainer-0.1.4.tar", last modified: Wed May  3 04:15:06 2023, max compression
```

## Comparing `tailors-trainer-0.1.3.tar` & `tailors-trainer-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,27 @@
--rw-r--r--   0        0        0      901 2022-09-14 10:40:50.635021 tailors-trainer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-08-18 15:02:22.358678 tailors-trainer-0.1.3/tailors_trainer/__init__.py
--rw-r--r--   0        0        0     7877 2022-09-14 15:13:21.138013 tailors-trainer-0.1.3/tailors_trainer/callbacks.py
--rw-r--r--   0        0        0     8068 2022-08-25 08:52:48.857268 tailors-trainer-0.1.3/tailors_trainer/corpus_from_eb.py
--rw-r--r--   0        0        0     8564 2022-09-15 10:14:29.593816 tailors-trainer-0.1.3/tailors_trainer/data.py
--rw-r--r--   0        0        0     2572 2022-06-26 10:22:05.350445 tailors-trainer-0.1.3/tailors_trainer/domains.py
--rw-r--r--   0        0        0      289 2022-08-18 15:02:26.870761 tailors-trainer-0.1.3/tailors_trainer/exceptions.py
--rw-r--r--   0        0        0        0 2022-06-05 15:08:22.178172 tailors-trainer-0.1.3/tailors_trainer/fast/__init__.py
--rw-r--r--   0        0        0     2260 2022-06-06 15:43:20.948048 tailors-trainer-0.1.3/tailors_trainer/fast/split.py
--rw-r--r--   0        0        0     4695 2022-08-18 16:02:41.872118 tailors-trainer-0.1.3/tailors_trainer/fast/train.py
--rw-r--r--   0        0        0     2564 2022-08-18 15:36:31.835251 tailors-trainer-0.1.3/tailors_trainer/optimizers.py
--rw-r--r--   0        0        0    10048 2022-09-15 16:24:31.762326 tailors-trainer-0.1.3/tailors_trainer/schedulers.py
--rw-r--r--   0        0        0     1645 2022-09-14 10:19:21.219266 tailors-trainer-0.1.3/tailors_trainer/train.py
--rw-r--r--   0        0        0    19884 2022-09-15 11:59:25.242494 tailors-trainer-0.1.3/tailors_trainer/trainer.py
--rw-r--r--   0        0        0     1044 2022-09-15 16:30:49.643522 tailors-trainer-0.1.3/setup.py
--rw-r--r--   0        0        0      575 2022-09-15 16:30:49.643741 tailors-trainer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-21 14:36:38.869665 tailors-trainer-0.1.4/LICENSE
+-rw-r--r--   0        0        0      387 2022-08-14 09:45:16.330766 tailors-trainer-0.1.4/README.md
+-rw-r--r--   0        0        0     1403 2023-05-03 04:13:50.969066 tailors-trainer-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      408 2023-02-22 02:14:34.315256 tailors-trainer-0.1.4/tailors_trainer/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 06:26:37.738729 tailors-trainer-0.1.4/tailors_trainer/agent/__init__.py
+-rw-r--r--   0        0        0      455 2023-04-24 02:36:59.736502 tailors-trainer-0.1.4/tailors_trainer/agent/agent.py
+-rw-r--r--   0        0        0     8073 2023-04-25 07:05:52.900451 tailors-trainer-0.1.4/tailors_trainer/callbacks.py
+-rw-r--r--   0        0        0     9614 2023-04-23 12:15:14.248527 tailors-trainer-0.1.4/tailors_trainer/cartographer.py
+-rw-r--r--   0        0        0     8965 2023-04-25 10:19:11.655830 tailors-trainer-0.1.4/tailors_trainer/data.py
+-rw-r--r--   0        0        0    10502 2023-04-25 09:45:32.223303 tailors-trainer-0.1.4/tailors_trainer/dataset_from_eb.py
+-rw-r--r--   0        0        0     2572 2023-04-17 07:03:24.234644 tailors-trainer-0.1.4/tailors_trainer/domains.py
+-rw-r--r--   0        0        0      289 2022-08-18 15:02:26.870761 tailors-trainer-0.1.4/tailors_trainer/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-27 06:26:55.635737 tailors-trainer-0.1.4/tailors_trainer/manager/__init__.py
+-rw-r--r--   0        0        0     1028 2023-03-27 07:27:17.667097 tailors-trainer-0.1.4/tailors_trainer/manager/apis/__init__.py
+-rw-r--r--   0        0        0     2110 2023-03-27 06:55:01.655359 tailors-trainer-0.1.4/tailors_trainer/manager/apis/auths.py
+-rw-r--r--   0        0        0     1013 2023-03-27 07:27:00.455169 tailors-trainer-0.1.4/tailors_trainer/manager/apis/passport_api.py
+-rw-r--r--   0        0        0      380 2023-03-27 07:30:32.949347 tailors-trainer-0.1.4/tailors_trainer/manager/apis/unsecure.py
+-rw-r--r--   0        0        0      929 2023-03-27 06:52:20.922505 tailors-trainer-0.1.4/tailors_trainer/manager/domains.py
+-rw-r--r--   0        0        0      649 2023-03-27 06:40:16.199626 tailors-trainer-0.1.4/tailors_trainer/manager/exceptions.py
+-rw-r--r--   0        0        0     2269 2023-03-27 07:24:17.547888 tailors-trainer-0.1.4/tailors_trainer/manager/manager.py
+-rw-r--r--   0        0        0     2326 2023-03-27 06:46:51.624071 tailors-trainer-0.1.4/tailors_trainer/manager/permissions.py
+-rw-r--r--   0        0        0     2576 2023-04-17 09:47:38.841519 tailors-trainer-0.1.4/tailors_trainer/optimizers.py
+-rw-r--r--   0        0        0     3269 2023-04-22 11:56:24.378350 tailors-trainer-0.1.4/tailors_trainer/pefts.py
+-rw-r--r--   0        0        0    10061 2023-04-17 09:47:56.045412 tailors-trainer-0.1.4/tailors_trainer/schedulers.py
+-rw-r--r--   0        0        0     1800 2023-04-28 09:49:23.442875 tailors-trainer-0.1.4/tailors_trainer/train.py
+-rw-r--r--   0        0        0    22388 2023-04-25 07:13:09.700614 tailors-trainer-0.1.4/tailors_trainer/trainer.py
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 tailors-trainer-0.1.4/PKG-INFO
```

### Comparing `tailors-trainer-0.1.3/tailors_trainer/callbacks.py` & `tailors-trainer-0.1.4/tailors_trainer/callbacks.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 
 import hao
 from tailors.domains import Derivable
 
 import tailors_trainer
 from tailors_trainer.exceptions import StopTailorsTrainer
 
-LOGGER = hao.logs.get_logger(__name__)
+LOGGER = hao.logs.get_logger('trainer.callbacks')
 
 
 class Callback(abc.ABC, Derivable):
 
     def __init__(self,
                  train_conf: 'tailors_trainer.trainer.TrainConf',
                  trainer_conf: 'tailors_trainer.trainer.TrainerConf',
-                 state: 'tailors_trainer.trainer.TrainerState') -> None:
+                 state: 'tailors_trainer.trainer.TrainerState',
+                 exp_dir: str) -> None:
         super().__init__()
         self.train_conf = train_conf
         self.trainer_conf = trainer_conf
         self.state = state
+        self.exp_dir = exp_dir
 
     def on_fit_start(self):
         pass
 
     def on_fit_end(self):
         pass
 
@@ -79,19 +81,24 @@
 
 
 class CallbackHandler:
 
     def __init__(self,
                  train_conf: 'tailors_trainer.trainer.TrainConf',
                  trainer_conf: 'tailors_trainer.trainer.TrainerConf',
-                 state: 'tailors_trainer.trainer.TrainerState') -> None:
+                 state: 'tailors_trainer.trainer.TrainerState',
+                 exp_dir: str) -> None:
         self.train_conf = train_conf
         self.trainer_conf = trainer_conf
         self.state = state
-        self.callbacks: List[Callback] = [clz(train_conf, trainer_conf, state) for clz in Callback.subclasses()]
+        self.exp_dir = exp_dir
+        self.callbacks: List[Callback] = [
+            clz(train_conf, trainer_conf, state, exp_dir)
+            for clz in Callback.subclasses()
+        ]
         LOGGER.info(f"callbacks: {[f'{c.__class__.__name__}' for c in self.callbacks]}")
 
     def _on_event(self, event: str, **kwargs):
         for callback in self.callbacks:
             fn = getattr(callback, event, None)
             if fn is None:
                 continue
@@ -152,42 +159,45 @@
         self._on_event('load_state_dict', state_dict)
 
 
 class TensorboardWriterCallback(Callback):
     def __init__(self,
                  train_conf: 'tailors_trainer.trainer.TrainConf',
                  trainer_conf: 'tailors_trainer.trainer.TrainerConf',
-                 state: 'tailors_trainer.trainer.TrainerState') -> None:
-        from torch.utils.tensorboard import SummaryWriter
-        super().__init__(train_conf, trainer_conf, state)
-        self.writer = SummaryWriter(hao.paths.get(f"data/logs/{train_conf.model}", train_conf.corpus, trainer_conf.exp, state.ts))
+                 state: 'tailors_trainer.trainer.TrainerState',
+                 exp_dir: str) -> None:
+        super().__init__(train_conf, trainer_conf, state, exp_dir)
+        self.path = hao.paths.get(exp_dir)
+        self.writer = None
 
     def write_scalar(self, k, v, step=None):
         if not isinstance(v, (int, float)):
             return
         if step is None:
-            step = self.epoch * self.steps_per_epoch_train
+            step = self.state.step
+        if self.writer is None:
+            from torch.utils.tensorboard import SummaryWriter
+            self.writer = SummaryWriter(self.path)
         self.writer.add_scalar(k, v, step)
 
     def on_train_batch_end(self):
-        step = self.state.current_steps()
-        self.write_scalar('loss/batch', self.state.metrics.get('loss/batch'), step)
+        self.write_scalar('loss/batch', self.state.metrics.get('loss/batch'))
 
     def on_epoch_end(self):
-        step = self.state.current_steps()
         for k, v in self.state.metrics.items():
-            self.write_scalar(k, v, step)
+            self.write_scalar(k, v)
 
 
 class EarlyStopCallback(Callback):
     def __init__(self,
                  train_conf: 'tailors_trainer.trainer.TrainConf',
                  trainer_conf: 'tailors_trainer.trainer.TrainerConf',
-                 state: 'tailors_trainer.trainer.TrainerState') -> None:
-        super().__init__(train_conf, trainer_conf, state)
+                 state: 'tailors_trainer.trainer.TrainerState',
+                 exp_dir: str) -> None:
+        super().__init__(train_conf, trainer_conf, state, exp_dir)
         self.consec_increases = 0
 
     def should_stop(self):
         if self.state.epoch < 1:
             return False
         if self.state.val_losses[-1] <= self.state.val_losses[-2]:
             self.consec_increases = 0
@@ -222,20 +232,21 @@
                 _, path = self.state._ckpts.top_n.pop()
                 to_deletes.append(path)
         if self.trainer_conf.save_last:
             if self.state._ckpts.last and all(self.state._ckpts.last != path for _, path in self.state._ckpts.top_n):
                 to_deletes.append(self.state._ckpts.last)
             self.state._ckpts.last = path_new
         for to_delete in to_deletes:
-            if os.path.isfile(to_delete):
-                os.remove(to_delete)
+            path = hao.paths.get(to_delete)
+            if os.path.isfile(path):
+                os.remove(path)
 
-        LOGGER.debug(self.top_n_msg())
+        LOGGER.info(self.top_n_msg())
         if self.trainer_conf.save_last:
-            LOGGER.debug(f"[checkpoint] last: {self.state._ckpts.last}")
+            LOGGER.info(f"[checkpoint] last: {self.state._ckpts.last}")
 
     def on_fit_end(self):
         LOGGER.info(self.top_n_msg())
         if self.trainer_conf.save_last:
             LOGGER.info(f"[checkpoint] last: {self.state._ckpts.last}")
 
     def top_n_msg(self):
```

### Comparing `tailors-trainer-0.1.3/tailors_trainer/corpus_from_eb.py` & `tailors-trainer-0.1.4/tailors_trainer/dataset_from_eb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,134 +1,191 @@
 # -*- coding: utf-8 -*-
 import itertools
 import json
 import logging
 import operator
 import os
 import random
-from collections import Counter
-from typing import List, Optional, Tuple
+from collections import defaultdict
+from typing import List, Tuple
 
 import hao
-from hao.mongo import Mongo
+import requests
 from hao.namespaces import attr, from_args
 from hao.stopwatch import Stopwatch
-from tqdm import tqdm
 
-LOGGER = hao.logs.get_logger(__name__)
+LOGGER = hao.logs.get_logger('trainer.dataset_from_eb')
 hao.logs.update_logger_levels({
     "__main__": logging.INFO,
 })
 
 
 @from_args
 class Conf(object):
-    task: str = attr(str, default='bidding')
-    reviewed_only: bool = attr(bool, action='store_true')
+    task: str = attr(str, required=True)
+    token: str = attr(str, help='task token or user token', required=True, secret=True)
+    format: str = attr(str, choices=['neat', 'raw'], default='raw')
+    selection: str = attr(str, choices=('annotated', 'reviewed', 'all'), default='annotated')
     cases: bool = attr(bool, default=True)
     cases_factor: int = attr(int, default=2, help='n duplicates of the cases')
     cases_starts: int = attr(int, help='No. from which are all cases')
-    size: int = attr(int)
+    ignore_by: str = attr(str, help='ignore items annotated by user')
     seed: int = attr(int, required=True, default=1000)
-    query: str = attr(str)
+    type: str = attr(str, choices=('SLC', 'MLC', 'NER', 'RE', 'T2T'), help='task types')
+    endpoint: str = attr(str, default=hao.config.get('eb.endpoint', 'http://bjb.bl-ai.com'))
 
 
 def process():
     LOGGER.info('process')
     sw = Stopwatch()
     conf = Conf()
     LOGGER.info(conf)
 
-    task_name = conf.task if conf.task.startswith("task-") else f"task-{conf.task}"
-    task_cases_name = f"{task_name}-cases"
-
-    mongo = Mongo()
-    task_exist, task_cases_exist = mongo.is_collection_exist(task_name), mongo.is_collection_exist(task_cases_name)
-    if not task_exist and not task_cases_exist:
-        LOGGER.info('tasks not exist')
-        return
+    labels = get_labels(conf)
+    items = get_items(conf)
+    items_cases = get_items(conf, is_cases=True) if conf.cases and not conf.task.endswith('cases') else []
+    items_train, items_val = group_split(conf, items, items_cases)
+
+    dataset = {'train': convert(items_train), 'val': convert(items_val)}
+    log_summary(conf, dataset, labels)
+    msgs = [save_to_file(conf.task, split, items) for split, items in dataset.items()]
+    LOGGER.info(f'done, took: {sw.took()}')
+    for msg in msgs:
+        LOGGER.info(msg)
 
-    items = list(from_eb(mongo, task_name, conf.reviewed_only, conf.size, conf.query))
-    items_cases = []
 
-    items_train = [item for item in items if item.get('splits', {}).get(conf.seed) == 'train']
-    items_val = [item for item in items if item.get('splits', {}).get(conf.seed) == 'val']
+def get_labels(conf: Conf):
+    labels_path = hao.paths.get(f"data/raw/{conf.task}-labels.json")
+    if os.path.exists(labels_path):
+        return json.loads(open(labels_path).read())
+
+    headers = {'API-Token': conf.token}
+    url = f"{conf.endpoint}/api/task/{conf.task}/tags"
+    res = requests.get(url, headers=headers)
+    res.raise_for_status()
+
+    hao.paths.make_parent_dirs(labels_path)
+    LOGGER.info(f"[labels.json] saving to: {labels_path}")
+
+    data = res.json().get('data')
+    labels = {
+        label: {tag.get('name'): tag.get('description') for tag in tags.get('tags')}
+        for label, tags in data.items()
+    }
 
-    if len(items_train) > 0 and len(items_val) > 0:
-        items_cases = [item for item in items if item.get('split', {}).get(conf.seed) not in ('train', 'val')]
+    with open(labels_path, 'w') as f:
+        f.write(hao.jsons.prettify(labels))
+    return labels
+
+
+def get_items(conf: Conf, *, is_cases: bool = False):
+    def qualified(item):
+        if item.get('enabled') == False:
+            return False
+        if item.get('editor_timestamp') is None:
+            return False
+        if conf.ignore_by is not None and item.get('editor') == conf.ignore_by:
+            return False
+        return True
+
+    task = f"{conf.task}-cases" if is_cases else conf.task
+    dataset_raw_path = hao.paths.get(f"data/raw/{task}.jsonl")
+
+    if os.path.exists(dataset_raw_path):
+        items = open(dataset_raw_path).readlines()
+        items = [json.loads(item) for item in items]
 
     else:
-        LOGGER.info('no pre splits on seed')
-        if conf.cases and task_cases_exist:
-            items_cases = list(from_eb(mongo, task_cases_name, conf.reviewed_only, conf.size, conf.query))
-        elif conf.cases_starts and conf.cases_starts < len(items):
-            items_cases = items[conf.cases_starts:]
-            items = items[:conf.cases_starts]
-        random.seed(conf.seed)
-        random.shuffle(items)
-        i = int(0.8 * len(items))
-        items_train = items[:i]
-        items_val = items[i:]
-
-    corpus = {
-        'train': items_train + items_cases * conf.cases_factor,
-        'val': items_val
-    }
-    msgs = []
-    for split, items in corpus.items():
-        msg = save_to_file(conf.task, split, items)
-        log_summary(split, items)
-        msgs.append(msg)
+        headers = {'API-Token': conf.token}
+        url = f"{conf.endpoint}/api/task/export?name={task}&format={conf.format}&selection={conf.selection}&zip=false"
+        res = requests.get(url, headers=headers)
+        res.raise_for_status()
+
+        contents = res.text.splitlines()
+        if len(contents) == 1 and json.loads(contents[0]).get('message') is not None:
+            LOGGER.error(f"[{task}] {res.text}")
+            return []
+
+        hao.paths.make_parent_dirs(dataset_raw_path)
+        LOGGER.info(f"[raw.jsonl] saving to: {dataset_raw_path}")
+
+        with open(dataset_raw_path, 'w') as f:
+            f.write(res.text)
+        items = res.text.splitlines()
+        items = [json.loads(item) for item in items]
+
+    return list(filter(qualified, items))
+
+
+def group_split(conf: Conf, items_general: list, items_cases: list):
+    items_train = [item for item in items_general if item.get('splits', {}).get(conf.seed) == 'train']
+    items_val = [item for item in items_general if item.get('splits', {}).get(conf.seed) == 'val']
+    items_general = [item for item in items_general if item.get('splits', {}).get(conf.seed) not in ('train', 'val')]
+
+    if conf.cases_starts:
+        _items_cases = items_general[conf.cases_starts:]
+        items_cases.extend(_items_cases)
+        items_general = items_general[:conf.cases_starts]
 
-    LOGGER.info(f'done, took: {sw.took()}')
-    for msg in msgs:
-        LOGGER.info(msg)
+    if conf.type in ('T2T', 'NER', 'RE', None):
+        groups = {conf.type: items_general}
 
-
-def from_eb(mongo: Mongo, col_name: str, reviewed_only: bool = False, size: Optional[int] = None, query: Optional[str] = None):
-    LOGGER.info(f"[from eb] task: {col_name}, reviewed_only: {reviewed_only}, size: {size}, query: {query}")
-    _query = {'enabled': {'$ne': False}, 'editor_timestamp': {'$ne': None}, 'annotation': {'$exists': True}}
-    if query is not None:
-        query = {**_query, **json.loads(query)}
     else:
-        query = _query
-        if reviewed_only:
-            query['reviewer_timestamp'] = {'$ne': None}
-
-    total = mongo.count(col_name, query)
-    if size is not None:
-        total = min(size, total)
-
-    projection = {'uid': 1, 'es_id': 1, 'caption': 1, 'html': 1, 'text': 1, 'annotation': 1}
-    for item in tqdm(mongo.find(col_name, query, projection).limit(total), total=total, desc=f"[fetching] {col_name}"):
-        data = convert_annotations(item)
-        if data:
-            yield data
-
-
-def convert_annotations(item):
-    annotation = item.get('annotation')
-    if annotation is None or len(annotation) == 0:
-        return
+        groups = defaultdict(list)
 
-    entities, relations = get_entities_and_relations(annotation)
-    label, labels = get_classifications(annotation)
-    data = {
-        'uid': item.get('uid'),
-        'es_id': item.get('es_id'),
-        'caption': item.get('caption'),
-        'text': item.get('text'),
-        'html': item.get('html'),
-        'label': label,
-        'labels': labels,
-        'entities': entities,
-        'relations': relations,
-        'splits': item.get('splits')
-    }
-    return {k: v for k, v in data.items() if v is not None}
+        for item in items_general:
+            annotation = item.get('annotation', {})
+            annotations = annotation.get(conf.type)
+            if annotations is None:
+                continue
+
+            if conf.type == 'SLC':
+                label = annotations
+            elif conf.type == 'MLC':
+                random.seed(conf.seed)
+                label = random.choice(annotation)
+            else:
+                LOGGER.error(f"Unsupported type: {conf.type}")
+                continue
+
+            groups[label].append(item)
+
+    items_train, items_val = [], []
+    for items in groups.values():
+        random.seed(conf.seed)
+        random.shuffle(items)
+        i = len(items) * 8 // 10
+        items_train.extend(items[:i])
+        items_val.extend(items[i:])
+    items_train.extend(items_cases * conf.cases_factor)
+    return items_train, items_val
+
+
+def convert(items: list):
+    def transform(e):
+        annotation = e.get('annotation')
+        if annotation is None or len(annotation) == 0:
+            return
+
+        entities, relations = get_entities_and_relations(annotation)
+        label, labels = get_classifications(annotation)
+        data = {
+            'uid': e.get('uid'),
+            'es_id': e.get('es_id'),
+            'caption': e.get('caption'),
+            'text': e.get('text'),
+            'html': e.get('html'),
+            'label': label,
+            'labels': labels,
+            'entities': entities,
+            'relations': relations,
+            'splits': e.get('splits')
+        }
+        return {k: v for k, v in data.items() if v is not None}
+    return list(filter(None, [transform(item) for item in items]))
 
 
 def get_entities_and_relations(annotation: dict) -> Tuple[list, list]:
     annotations_ner, annotations_re = annotation.get("NER"), annotation.get("RE")
     if annotations_ner is None:
         return None, None
     if len(annotations_ner) == 0:
@@ -169,60 +226,68 @@
 
 
 def get_classifications(annotation: dict):
     return annotation.get('SLC'), annotation.get('MLC')
 
 
 def save_to_file(task: str, split: str, items: List[dict]):
-    filepath = hao.paths.get(f"data/corpus/{task}/{split}.jsonl")
+    filepath = hao.paths.get(f"data/dataset/{task}/{split}.jsonl")
     hao.paths.make_parent_dirs(filepath)
     with open(filepath, "w") as f:
-        for item in tqdm(items, desc=f"[saving] {os.path.basename(filepath)}"):
+        for item in items:
             f.write(f"{hao.jsons.dumps(item)}\n")
     return f"saved to {filepath}, size: {len(items)}"
 
 
-def log_summary(split, items):
-    counter_tags, counter_relations, counter_labels, counter_seed = Counter(), Counter(), Counter(), Counter()
-    LOGGER.info(f" {split} ".center(60, '='))
-    for item in items:
-        entities, relations, label, labels = item.get('entities'), item.get('relations'), item.get('label'), item.get('labels')
-        for entries in entities:
-            counter_tags.update([entry.get('tag') for entry in entries])
-        counter_relations.update([relation.get('p') for relation in relations])
-        if label:
-            counter_labels.update((label,))
-        if labels:
-            counter_labels.update(labels)
-        counter_seed.update(list(item.get('splits', [])))
-
-    if len(counter_tags) > 0:
-        LOGGER.info(" entities ".center(35, '-'))
-        size = max([len(tag) for tag in counter_tags]) + 1
-        for seed, count in counter_tags.items():
-            LOGGER.info(f"\t{seed: <{size}}: {count}")
-
-    if len(counter_relations) > 0:
-        LOGGER.info(" relations ".center(35, '-'))
-        size = max([len(tag) for tag in counter_relations]) + 1
-        for seed, count in counter_relations.items():
-            LOGGER.info(f"\t{seed: <{size}}: {count}")
-
-    if len(counter_labels) > 0:
-        LOGGER.info(" labels ".center(35, '-'))
-        size = max([len(tag) for tag in counter_labels]) + 1
-        for seed, count in counter_labels.items():
-            LOGGER.info(f"\t{seed: <{size}}: {count}")
-
-    if len(counter_seed) > 0:
-        LOGGER.info(" seeds ".center(35, '-'))
-        size = max([len(str(seed)) for seed in counter_seed]) + 1
-        for seed, count in counter_seed.items():
-            LOGGER.info(f"\t{seed: <{size}}: {count}")
+def log_summary(conf: Conf, dataset: dict, mappings: dict):
+    if conf.type == 'T2T':
+        return
+    counters_ner = defaultdict(lambda: defaultdict(int))
+    counters_re = defaultdict(lambda: defaultdict(int))
+    counters_slc = defaultdict(lambda: defaultdict(int))
+    counters_mlc = defaultdict(lambda: defaultdict(int))
+    for split, items in dataset.items():
+        for item in items:
+            entities, relations, label, labels = item.get('entities'), item.get('relations'), item.get('label'), item.get('labels')
+            if entities:
+                for entries in entities:
+                    for entry in entries:
+                        counters_ner[entry.get('tag')][split] += 1
+            if relations:
+                for relation in relations:
+                    counters_re[relation.get('p')][split] += 1
+            if label:
+                counters_slc[label][split] += 1
+            if labels:
+                for label in labels:
+                    counters_mlc[label][split] += 1
+
+    _print_counter('NER', counters_ner, mappings.get('NER'))
+    _print_counter('RE', counters_re, mappings.get('RE'))
+    _print_counter('SLC', counters_slc, mappings.get('SLC'))
+    _print_counter('MLC', counters_mlc, mappings.get('MLC'))
+
 
+def _print_counter(name, counters: dict, labels: dict):
+    if len(counters) == 0:
+        return
+    lines = [f" {name} ".center(35, '-')]
+    size = max(10, max([len(label) for label in labels]) + 1)
+    lines.append(f"\t{' ': <{size}} {'train': <10} {'val': <10} {'ratio': <10} (description)")
+    for label, description in labels.items():
+        counter = counters.get(label)
+        if counter is None:
+            counts = f"{'-': <10} {'-': <10}"
+            ratio = '-'
+        else:
+            count_train, count_val = counter.get('train', 0), counter.get('val', 0)
+            counts = f"{count_train: <10} {count_val: <10}"
+            ratio = '0.0' if count_val == 0 else f"{count_train / count_val:0.1f}"
+        lines.append(f"\t{label: <{size}} {counts} {ratio: <10} ({description})")
+    LOGGER.info('\n'.join(lines))
 
 
 if __name__ == '__main__':
     try:
         process()
     except KeyboardInterrupt:
         print('[ctrl-c] stopped')
```

### Comparing `tailors-trainer-0.1.3/tailors_trainer/data.py` & `tailors-trainer-0.1.4/tailors_trainer/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 # -*- coding: utf-8 -*-
 import abc
 import os
 import pickle
 import shutil
-from typing import List, Optional
+from typing import Generator, List, Union
 
 import hao
 import lmdb
 import rocksdbpy
 from hao.namespaces import attr, from_args
 from hao.singleton import Singleton
-from tailors.domains import Derivable
+from tailors.domains import Derivable, Example
 from tailors.models import TailorsIO
 from torch.utils.data import Dataset
 from torch.utils.data.dataloader import DataLoader
 from torch.utils.data.distributed import DistributedSampler
 from tqdm import tqdm
 
 from tailors_trainer.exceptions import TailorsTrainerError
 
-LOGGER = hao.logs.get_logger(__name__)
+LOGGER = hao.logs.get_logger('trainer.data')
 
 
 class CacheStore(abc.ABC, Derivable):
 
     @staticmethod
     def get_instance(name, cache_dir, split) -> 'CacheStore':
         for clz in CacheStore.subclasses():
             if clz.name() == name:
                 return clz(cache_dir, split)
         raise TailorsTrainerError(f"Unsupported cache type: {name}")
 
     def __init__(self, cache_dir: str, split: str) -> None:
-        self.path = hao.paths.get(f"data/cache/{cache_dir}/{split}.{self.name()}")
-        hao.paths.make_parent_dirs(self.path)
-        self.db: Optional[lmdb.Environment] = None
+        self.cache_path = f"{cache_dir}/{split}.{self.name()}"
+        self.fullpath = hao.paths.get(self.cache_path)
+        hao.paths.make_parent_dirs(self.fullpath)
+        self.db = None
         self.length = -1
         self.keys = None
 
     @staticmethod
     @abc.abstractmethod
     def name():
         raise NotImplementedError()
@@ -94,25 +95,25 @@
 class LmdbCacheStore(CacheStore):
 
     @staticmethod
     def name():
         return 'lmdb'
 
     def load(self) -> bool:
-        if not os.path.exists(self.path):
+        if not os.path.exists(self.fullpath):
             return False
 
         try:
             self.db = self.open_db()
             with self.db.begin(write=False) as txn:
                 self.length = txn.stat()["entries"]
                 self.keys = [key for key, _ in txn.cursor()]
                 return self.length > 0
         except Exception:
-            hao.paths.delete(f"{self.path}*")
+            hao.paths.delete(f"{self.fullpath}*")
             return False
 
     def populate(self, items):
         with self.open_db(readonly=False) as db:
             txn = db.begin(write=True)
             for i, item in enumerate(items):
                 txn.put(f"{i}".encode("ascii"), self.serialize(item))
@@ -123,15 +124,15 @@
 
     def get(self, index: int):
         with self.db.begin(write=False) as txn:
             return self.unserialize(txn.get(self.keys[index]))
 
     def open_db(self, readonly: bool = True) -> lmdb.Environment:
         return lmdb.open(
-            self.path,
+            self.fullpath,
             subdir=False,
             readonly=readonly,
             lock=not readonly,
             readahead=False,
             meminit=False,
             map_size=1099511627776 * 2,
             map_async=True
@@ -144,23 +145,23 @@
 class RocksdbCacheStore(CacheStore):
 
     @staticmethod
     def name():
         return 'rocksdb'
 
     def load(self) -> bool:
-        if not os.path.exists(self.path):
+        if not os.path.exists(self.fullpath):
             return False
 
         try:
             self.db = self.open_db()
             self.length = self.get('total')
             return self.length > 0
         except Exception:
-            hao.paths.delete(f"{self.path}*")
+            hao.paths.delete(f"{self.fullpath}*")
             return False
 
     def populate(self, items):
         db = self.open_db(readonly=False)
         try:
             total = 0
             for i, item in enumerate(items):
@@ -181,17 +182,17 @@
         option = rocksdbpy.Option()
         option.create_if_missing(True)
         option.set_max_open_files(100)
         option.set_use_fsync(False)
         option.set_bytes_per_sync(1024 * 1024)
         option.optimize_for_point_lookup(1024 * 1024)
         if readonly:
-            return rocksdbpy.open_for_readonly(self.path, option)
+            return rocksdbpy.open_for_readonly(self.fullpath, option)
         else:
-            return rocksdbpy.open(self.path, option)
+            return rocksdbpy.open(self.fullpath, option)
 
 
 def cache_names() -> tuple:
     return tuple(clz.name() for clz in CacheStore.subclasses())
 
 
 @from_args
@@ -209,51 +210,57 @@
         super().__init__()
         self.io = io
         self.name = name
         self.split = split
         self.files = files if isinstance(files, list) else [files]
         self.ddp = False  # todo
         self.dataset_conf = dataset_conf
-        self.cache = CacheStore.get_instance(dataset_conf.cache, f"{self.io.__module__}/{self.name}", self.split)
+        model_name = f"{self.io.__module__}.{self.io.__class__.__qualname__[:-2]}"
+        cache_dir = f"data/cache/{model_name}/{self.name}/"
+        self.cache = CacheStore.get_instance(dataset_conf.cache, cache_dir, self.split)
 
     def load(self):
         if not self.cache.load():
             try:
                 self.cache.populate(self.from_files())
             except KeyboardInterrupt:
-                shutil.rmtree(self.cache.path)
+                shutil.rmtree(self.cache.fullpath)
             if not self.cache.load():
                 raise TailorsTrainerError(f'Failed to load/populate cache: {self.dataset_conf.cache}')
-        LOGGER.info(f"[dataset] split: {self.split}, size: {self.cache.size()}, cache: {self.cache.path or 'n/a'}")
+        LOGGER.info(f"[dataset] split: {self.split}, size: {self.cache.size()}, cache: {self.cache.cache_path or 'n/a'}")
         return self
 
     def from_files(self):
         for file in self.files:
             yield from self.from_file(file)
 
-    def from_file(self, file):
+    def from_file(self, file) -> Generator[Example, None, None]:
         filepath = hao.paths.get(file)
         if not os.path.exists(filepath):
-            raise TailorsTrainerError(f"[dataset] file not found, corpus: {self.name}, split: {self.split}, file: {file}")
+            raise TailorsTrainerError(f"[dataset] file not found, dataset: {self.name}, split: {self.split}, file: {file}")
 
         tqdm_opts = {'desc': f"[dataset] {os.path.basename(filepath): <20}", 'ascii': '░▒▓', 'colour': 'cyan'}
         if (from_lines := getattr(self.io, 'from_lines', None)) is not None:
             for data in tqdm(from_lines(open(filepath, 'r').read()), **tqdm_opts):
                 yield data
 
         else:
             n_lines = hao.files.count_lines(filepath)
             with open(filepath, "r") as f:
                 for line in tqdm(f, total=n_lines, **tqdm_opts):
                     line = hao.strings.strip_to_none(line)
                     if line is None:
                         continue
-                    yield from self.from_line(line)
+                    data = self.from_line(line)
+                    if isinstance(data, list):
+                        yield from data
+                    else:
+                        yield data
 
-    def from_line(self, line: str):
+    def from_line(self, line: str) -> Union[Example, List[Example]]:
         return self.io.from_line(line)
 
     def __getitem__(self, index: int):
         return self.cache.get(index)
 
     def __len__(self) -> int:
         return self.cache.size()
```

### Comparing `tailors-trainer-0.1.3/tailors_trainer/domains.py` & `tailors-trainer-0.1.4/tailors_trainer/domains.py`

 * *Files identical despite different names*

### Comparing `tailors-trainer-0.1.3/tailors_trainer/optimizers.py` & `tailors-trainer-0.1.4/tailors_trainer/optimizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import hao
 from hao.namespaces import attr, from_args
 from tailors.exceptions import TailorsError
 from torch.optim import SGD, Adadelta
 from torch_optimizer import SGDW, Lamb, RAdam
 from transformers import AdamW
 
-LOGGER = hao.logs.get_logger(__name__)
+LOGGER = hao.logs.get_logger('trainer.optimizers')
 
 
 @from_args
 class AdadeltaConf:
     rho: float = attr(float)
     eps: float = attr(float, default=1e-8)
     lr: float = attr(float)
```

### Comparing `tailors-trainer-0.1.3/tailors_trainer/schedulers.py` & `tailors-trainer-0.1.4/tailors_trainer/schedulers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, List, Optional
 
 import hao
 from hao.namespaces import attr, from_args
 from tailors.exceptions import TailorsError
 from torch.optim.lr_scheduler import CosineAnnealingLR, CosineAnnealingWarmRestarts, OneCycleLR, ReduceLROnPlateau, _LRScheduler
 
-LOGGER = hao.logs.get_logger(__name__)
+LOGGER = hao.logs.get_logger('trainer.schedulers')
 
 
 @from_args(prefix='sched')
 class SchedulerConf:
     interval: str = attr(str, default='epoch', choices=('epoch', 'step'))
     monitor: str = attr(str, default='val_loss')
 
@@ -173,15 +173,15 @@
             min_lr=min_lr,
             eps=eps,
             verbose=verbose
         )
 
     def step(self, metrics: Any, epoch: Optional[int] = ...) -> None:
         self._step_count += 1
-        if self._step_count < self.warmup_steps:
+        if self._step_count <= self.warmup_steps:
             for i, group in enumerate(self.optimizer.param_groups):
                 group['lr'] = float(group['lr']) + self.warmup_delta
             self._last_lr = [group['lr'] for group in self.optimizer.param_groups]
         else:
             super().step(metrics, epoch)
 
     def get_last_lr(self):
```

### Comparing `tailors-trainer-0.1.3/tailors_trainer/train.py` & `tailors-trainer-0.1.4/tailors_trainer/train.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 import sys
 import warnings
+from typing import Optional
 
 import hao
 import regex
 from hao.namespaces import attr, from_args
 
 from tailors_trainer.exceptions import TailorsTrainerError
 from tailors_trainer.trainer import Trainer
 
 warnings.filterwarnings("ignore")
-LOGGER = hao.logs.get_logger(__name__)
+LOGGER = hao.logs.get_logger('train')
 
 
 @from_args
 class TaskConf:
     task: str = attr(str, help='using predefined values in `tasks.{task}` in tailors.yml')
 
 
@@ -29,30 +30,31 @@
     n_args = len(arguments)
 
     sep = ' ' if n_args <= 1 else ' \\\n\t'
     args = sep.join(arguments)
     LOGGER.info(f"\n{'━' * 50}\ntailors-train{sep}{args}\n{'━' * 50}")
 
 
-def load_task():
-    task_conf = TaskConf()
+def load_task(task_conf: Optional[TaskConf] = None):
+    task_conf = task_conf or TaskConf()
     if task_conf.task is None:
         return
     task = hao.config.get(f"tasks.{task_conf.task}", config='tailors.yml')
     if task is None or len(task) == 0:
         return
     args = parse_args()
     arguments = [f"--{k}={v}" for k, v in task.items() if k not in args]
     sys.argv.extend(arguments)
 
 
-def train():
+def train(task_conf: Optional[TaskConf] = None):
     try:
-        log_cmdline()
-        load_task()
+        if task_conf is None:
+            log_cmdline()
+        load_task(task_conf)
         trainer = Trainer()
         trainer.fit()
     except KeyboardInterrupt:
         print("[ctrl-c] stopped")
     except TailorsTrainerError as err:
         LOGGER.error(err)
     except Exception as err:
```

### Comparing `tailors-trainer-0.1.3/tailors_trainer/trainer.py` & `tailors-trainer-0.1.4/tailors_trainer/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,78 @@
 # -*- coding: utf-8 -*-
 import collections
 import importlib
-import math
 import os
 from datetime import datetime
 from types import SimpleNamespace
 from typing import Optional
 
 import hao
+import pandas as pd
 import torch
 import torchinfo
 from hao.namespaces import attr, from_args
-from tailors import losses, move_to_device, off_tensor, set_seed
+from peft import PeftType, TaskType, get_peft_config, get_peft_model_state_dict, set_peft_model_state_dict
+from tailors import append_batch, losses, move_to_device, set_seed
 from tailors.exceptions import TailorsError
 from tailors.metrics import classification_metrics
 from tailors.models import Tailors
 from torch.nn.parallel import DistributedDataParallel
 from torch.utils.data.dataloader import DataLoader
 from tqdm import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 
-from tailors_trainer import callbacks, optimizers, schedulers
+from tailors_trainer import callbacks, model_size, optimizers, pefts, schedulers
 from tailors_trainer.data import DatasetConf, TailorDataset
 from tailors_trainer.exceptions import StopTailorsTrainer, TailorsTrainerError
 
-LOGGER = hao.logs.get_logger(__name__)
+LOGGER = hao.logs.get_logger('trainer')
 
 
 @from_args
 class TrainConf:
+    """Hyperparams"""
     model: str = attr(str, required=True)
-    corpus: str = attr(str, required=True)
+    dataset: str = attr(str, required=True)
     seed = attr(int, default=1000)
     max_epochs: int = attr(int, default=50)
     loss = attr(str, choices=tuple(losses.LOSSES))
     lr: float = attr(float, default=1e-4)
     optimizer = attr(str, choices=tuple(optimizers.OPTIMIZERS), default=list(optimizers.OPTIMIZERS)[0])
     weight_decay: float = attr(float, default=1e-2)
     scheduler: str = attr(str, choices=tuple(schedulers.SCHEDULERS), default=list(schedulers.SCHEDULERS)[0])
     clip_norm: float = attr(float, default=1.0, help='clip grad norm for NLP tasks, generally: 1.0')
     amp: bool = attr(bool, default=False)
     accumulation: int = attr(int, default=1)
+    peft: str = attr(str, choices=tuple(t.value.lower() for t in PeftType), default=None)
+    peft_task_type: str = attr(str, choices=tuple(t.value.lower() for t in TaskType))
 
 
 @from_args
 class TrainerConf:
+    """Non-hyperparams"""
     exp: str = attr(str, required=True)
     gpus: str = attr(str, help='gpu indices separated by comma, no spaces')
     logger: str = attr(str, default='tensorboard')
-    log_summary: bool = attr(bool, default=True)
+    log_model_summary: bool = attr(bool, default=True)
+    log_model_depth: int = attr(int, default=3)
     resume_from: str = attr(str)
     early_stop_patience: int = attr(int, default=5)
-    checkpoint_name: str = attr(str, default='{model}-{corpus}-{exp}-{ts}-epoch={epoch}-val_loss={loss_val}-f1={f1}.ckpt')
+    track_dynamics: bool = attr(bool, default=False)
+    checkpoint_name: str = attr(str, default='{model}-{dataset}-{exp}-{ts}-epoch={epoch}-val_loss={loss_val}-f1={f1}.ckpt')
     save_top_n: int = attr(int, default=1)
     save_last: bool = attr(bool, default=False)
 
 
 class TrainerState:
     def __init__(self) -> None:
         self.ts = datetime.now().strftime('%y%m%d-%H%M')
         self.bz = 0
         self.steps_per_epoch = {}
+        self.step = 0
         self.epoch = -1
         self.batch_id = -1
         self.val_losses = []
         self.metrics = {}
         self.reports = {}
         self._ckpts = SimpleNamespace(top_n=[], last=None, should_save=False, new_path=None)
         self._resume_state_dict = None
@@ -77,17 +85,14 @@
     def set_metrics(self, metrics: dict):
         for k, v in metrics.items():
             if 'report' in k.lower():
                 self.reports[k] = v
             else:
                 self.set_metric(k, v)
 
-    def current_steps(self):
-        return self.epoch * self.steps_per_epoch.get('train') + (self.batch_id + 1) * self.bz
-
     def state_dict(self):
         return {k: v for k, v in vars(self).items() if not k.startswith('_')}
 
     def load_state_dict(self, state_dict):
         for k, v in state_dict.items():
             setattr(self, k, v)
 
@@ -97,15 +102,16 @@
         super().__init__()
         self.trainer_conf = trainer_conf or TrainerConf()
         self.train_conf = train_conf or TrainConf()
         LOGGER.info(self.trainer_conf)
         LOGGER.info(self.train_conf)
         self.device, self.rank, self.world_size = self.check_devices()
         self.state = TrainerState()
-        self.callback_handler = callbacks.CallbackHandler(self.train_conf, self.trainer_conf, self.state)
+        self.exp_dir = f"data/exps/{self.train_conf.model}/{self.train_conf.dataset}/{self.trainer_conf.exp}-{self.state.ts}"
+        self.callback_handler = callbacks.CallbackHandler(self.train_conf, self.trainer_conf, self.state, self.exp_dir)
         self.load_resume_from_state_dict()
 
         set_seed(self.train_conf.seed)
         self.model: Tailors = self.get_model()
         self.dataloaders, self.state.steps_per_epoch = self.get_dataloaders()
 
         self.criteria = losses.get(self.train_conf.loss) if self.train_conf.loss else None
@@ -148,60 +154,66 @@
     def validate(self):
         if self.criteria is None and not hasattr(self.model, 'compute_loss'):
             raise TailorsTrainerError('Expecting either `--loss=xxx` or `compute_losss()` method')
 
     def go_thru_resume_from_state_dict(self):
         if self.state._resume_state_dict is None:
             return
-        for key, attr in (
+        for key, attri in (
             ('state', 'state'),
             ('state_dict', 'model'),
             ('scaler_state_dict', 'scaler'),
             ('optimizer_state_dict', 'optimizer'),
             ('scheduler_state_dict', 'scheduler'),
         ):
-            if (m := getattr(self, attr)) is None or (state_dict := self.state._resume_state_dict.get(key)) is None:
+            if (m := getattr(self, attri, None)) is None or (state_dict := self.state._resume_state_dict.get(key)) is None:
                 continue
             m.load_state_dict(state_dict)
 
+        state_dict = state_dict.get('state_dict')
+        if (peft_config := self.state._resume_state_dict.get('peft_config')) is None:
+            self.model.load_state_dict(state_dict)
+        else:
+            self.model.peft_config = get_peft_config(peft_config)
+            set_peft_model_state_dict(self.model, state_dict)
         self.state._resume_state_dict = None
 
     def get_model(self) -> Tailors:
         model_fqn = self.train_conf.model
         module_name, _, model_class_name = model_fqn.rpartition('.')
         module = importlib.import_module(module_name)
         model_class = getattr(module, model_class_name)
 
         if self.state._resume_state_dict is not None:
             model_conf = self.state._resume_state_dict.get('model_conf')
         else:
             model_conf_class = getattr(module, f"{model_class_name}Conf")
-            meta = hao.config.get(f"corpora.{self.train_conf.corpus}", config='tailors.yml').get('meta')
+            meta = hao.config.get(f"datasets.{self.train_conf.dataset}", config='tailors.yml').get('meta')
             if meta is None or not isinstance(meta, dict) or len(meta) == 0:
-                raise TailorsError(f"expecting `meta` dict in corpora.{self.train_conf.corpus}, in `tailors.yml`")
+                raise TailorsError(f"expecting `meta` dict in corpora.{self.train_conf.dataset}, in `tailors.yml`")
             model_conf = model_conf_class(meta=meta)
         LOGGER.info(model_conf)
-        model = model_class(model_conf).use_device(self.device)
+        model = model_class(model_conf)
+        model = pefts.peftify(model, self.train_conf.peft, self.train_conf.peft_task_type)
+        model.use_device(self.device)
+
         if self.world_size > 1:
             model = DistributedDataParallel(model, device_ids=[self.rank], output_device=self.rank)
         return model
 
     def get_dataloaders(self):
-        datasets = hao.config.get(f"corpora.{self.train_conf.corpus}", config='tailors.yml').get('datasets')
+        datasets = hao.config.get(f"datasets.{self.train_conf.dataset}", config='tailors.yml').get('datasets')
         dataset_conf = DatasetConf()
         LOGGER.info(dataset_conf)
         self.state.bz = dataset_conf.bz
         dataloaders = {
-            split: TailorDataset(self.model.io, self.train_conf.corpus, split, files, dataset_conf).dataloader()
+            split: TailorDataset(self.model.io, self.train_conf.dataset, split, files, dataset_conf).dataloader()
             for split, files in datasets.items()
         }
-        steps_per_epochs = {
-            split: math.ceil(len(dataloader) / dataloader.batch_size)
-            for split, dataloader in dataloaders.items()
-        }
+        steps_per_epochs = {split: len(dataloader) for split, dataloader in dataloaders.items()}
         return dataloaders, steps_per_epochs
 
     def get_scaler(self):
         return torch.cuda.amp.GradScaler() if self.train_conf.amp else None
 
     def get_optimizer(self):
         def get_bucket(name):
@@ -235,17 +247,25 @@
             grouped_parameters.append({'params': params, **group_meta.get(key)})
         return optimizers.get(self.train_conf.optimizer, grouped_parameters)
 
     def get_scheduler(self):
         return schedulers.get(self.train_conf.scheduler, self.optimizer, steps_per_epoch=self.state.steps_per_epoch.get('train'))
 
     def log_model_summary(self):
-        if self.trainer_conf.log_summary:
-            summary = torchinfo.summary(self.model, col_names=('num_params', 'trainable'), mode='train', row_settings=('ascii_only',), verbose=0)
+        if self.trainer_conf.log_model_summary:
+            summary = torchinfo.summary(
+                self.model,
+                col_names=('num_params', 'trainable'),
+                mode='train',
+                row_settings=('ascii_only',),
+                depth=self.trainer_conf.log_model_depth,
+                verbose=0,
+            )
             LOGGER.info(f"[summary] {self.train_conf.model}\n{summary}")
+            LOGGER.info(f"estimated size: {model_size(self.model)}")
 
     def get_lr(self):
         if hasattr(self.scheduler, 'get_lr'):
             return self.scheduler.get_lr()
         return self.get_lrs()[0]
 
     def get_lrs(self):
@@ -284,114 +304,120 @@
 
         # RuntimeError: unable to open shared memory object
         torch.multiprocessing.set_sharing_strategy('file_system')
 
     def train_epoch(self, epoch: int, dataloader: DataLoader):
         self.model.train()
         self.callback_handler.on_train_epoch_start()
-        losses = []
-        acc = max(1, self.train_conf.accumulation)
+        losses, dynamics = [], collections.defaultdict(list)
+        acmu = max(1, self.train_conf.accumulation)
         with logging_redirect_tqdm():
             batches = tqdm(dataloader, desc=f"[epoch {epoch}] training  ", ascii=' ━', colour='blue')
-            for batch_id, (data, target) in enumerate(batches):
+            for batch_id, batch in enumerate(batches):
                 self.state.batch_id = batch_id
+                self.state.step += acmu
                 self.callback_handler.on_train_batch_start()
 
-                data, target = move_to_device(data, self.model.device), move_to_device(target, self.model.device)
-                is_optimizer_step = acc == 1 or ((batch_id + 1) % acc == 0) or (batch_id + 1 == self.state.steps_per_epoch.get('train'))
+                batch = move_to_device(batch, self.model.device)
+                is_optimizer_step = acmu == 1 or self.state.step % acmu == 0
 
                 if self.scaler:
                     with torch.cuda.amp.autocast(True):
-                        encoded = self.model.encode(data)
+                        encoded = self.model.encode(batch.features)
                         decoded = self.model.decode(encoded)
-                        loss = self.compute_loss(encoded, decoded, target)
-                        loss = loss / acc
+                        loss = self.compute_loss(encoded, decoded, batch.target)
+                        loss = loss / acmu
+
                     self.scaler.scale(loss).backward()
                     loss = loss.item()
                     losses.append(loss)
                     if self.train_conf.clip_norm > 0:
                         self.scaler.unscale_(self.optimizer)
                         torch.nn.utils.clip_grad_norm_(self.model.parameters(), self.train_conf.clip_norm)
                     if is_optimizer_step:
                         self.scaler.step(self.optimizer)
                         self.scaler.update()
                         self.optimizer.zero_grad(set_to_none=True)
                         batches.set_postfix({'loss': f"{loss:.4f}", 'ts': self.state.ts})
 
                 else:
-                    encoded = self.model.encode(data)
+                    encoded = self.model.encode(batch.features)
                     decoded = self.model.decode(encoded)
-                    loss = self.compute_loss(encoded, decoded, target)
-                    loss = loss / acc
+                    loss = self.compute_loss(encoded, decoded, batch.target)
+                    loss = loss / acmu
                     loss.backward()
                     loss = loss.item()
                     losses.append(loss)
+
                     if self.train_conf.clip_norm > 0:
                         torch.nn.utils.clip_grad_norm_(self.model.parameters(), self.train_conf.clip_norm)
                     if is_optimizer_step:
                         self.optimizer.step()
                         self.optimizer.zero_grad(set_to_none=True)
                         batches.set_postfix({'loss': f"{loss:.4f}", 'ts': self.state.ts})
                 self.state.set_metric('loss/batch', loss)
 
+                if self.trainer_conf.track_dynamics is True:
+                    logits = encoded[0] if isinstance(encoded, tuple) else encoded
+                    logits = logits.detach().cpu().tolist()
+                    target = batch.target.detach().cpu().tolist()
+                    for guid, logits, gold in zip(batch.idx, logits, target):
+                        dynamics['epoch'].append(epoch)
+                        dynamics['guid'].append(guid)
+                        dynamics['logits'].append(logits)
+                        dynamics['gold'].append(gold)
+
                 self.callback_handler.on_train_batch_end()
 
         self.state.set_metric('loss/train', sum(losses) / len(losses))
+        self.save_dynamics(epoch, dynamics)
         self.callback_handler.on_train_epoch_end()
 
     def val_epoch(self, epoch: int, dataloader: DataLoader):
-        def append_batch_result(items, batch):
-            batch = off_tensor(batch)
-            if isinstance(batch, tuple):
-                hao.lists.add_tuple_to_list(items, batch)
-            elif isinstance(batch, torch.Tensor):
-                items.append(batch)
-            else:
-                items.extend(batch)
-
         self.model.eval()
         self.callback_handler.on_val_epoch_start()
-        losses, preds, targets = [], [], []
+        losses, encodeds, decodeds, targets = [], [], [], []
         with logging_redirect_tqdm(), torch.no_grad():
             batches = tqdm(dataloader, desc=f"[epoch {epoch}] validating", ascii=' ━', colour='green')
-            for batch_id, (data, target) in enumerate(batches):
+            for batch_id, batch in enumerate(batches):
                 self.state.batch_id = batch_id
                 self.callback_handler.on_eval_batch_start()
 
-                data, target = move_to_device(data, self.model.device), move_to_device(target, self.model.device)
-                encoded = self.model.encode(data)
+                batch = move_to_device(batch, self.model.device)
+                encoded = self.model.encode(batch.features)
                 decoded = self.model.decode(encoded)
-                loss = self.compute_loss(encoded, decoded, target)
+                loss = self.compute_loss(encoded, decoded, batch.target)
                 loss = loss.item()
                 losses.append(loss)
-                append_batch_result(preds, decoded)
-                append_batch_result(targets, target)
+                append_batch(encodeds, encoded)
+                append_batch(decodeds, decoded)
+                append_batch(targets, batch.target)
                 batches.set_postfix({'loss': f"{loss:.4f}", 'ts': self.state.ts})
 
                 if (on_eval_batch_end := getattr(self.model, 'on_eval_batch_end', None)) is not None:
-                    on_eval_batch_end(encoded, decoded, target)
+                    on_eval_batch_end(encoded, decoded, batch.target)
 
                 self.callback_handler.on_eval_batch_end()
 
         self.state.set_metric('loss/val', sum(losses) / len(losses))
-        self.compute_metrics(preds, targets)
+        self.compute_metrics(encodeds, decodeds, targets)
         self.callback_handler.on_val_epoch_end()
 
     def compute_loss(self, encoded, decoded, target):
         if (criteria := getattr(self.model, 'compute_loss', None)) is not None:
             return criteria(encoded, decoded, target)
         y_pred = encoded[0] if isinstance(encoded, tuple) else encoded
         y_true = target[0] if isinstance(target, tuple) else target
         return self.criteria(y_pred, y_true)
 
-    def compute_metrics(self, preds, targets):
+    def compute_metrics(self, encodeds, decodeds, targets):
         if (metrics_fn := getattr(self.model, 'compute_metrics', None)) is not None:
-            metrics = metrics_fn(preds, targets)
+            metrics = metrics_fn(encodeds, decodeds, targets)
         else:
-            metrics = classification_metrics.calculate(preds[0], targets[0])
+            metrics = classification_metrics.calculate(targets[0], decodeds[0], self.model.io.tags.id2tag)
         self.state.set_metrics(metrics)
 
     def lr_scheduler_step(self):
         scheduler_args = {'metrics': self.state.metrics.get('loss/val'), 'epoch': self.state.epoch}
         hao.invoker.invoke(self.scheduler.step, **scheduler_args)
 
         # get the new lrs
@@ -401,51 +427,74 @@
     def log_metrics(self):
         width = max(len(k) for k, _ in self.state.metrics.items()) + 1
         metrics = '\n'.join([f"\t{k: <{width}}: {v}" for k, v in self.state.metrics.items()])
         LOGGER.info(f"{' metrics '.center(50, '━')}\n{metrics}")
         for k, v in self.state.reports.items():
             LOGGER.info(f"{f' {k} '.center(50, '━')}\n{v}")
 
+    def save_dynamics(self, epoch: int, dynamics: dict):
+        if len(dynamics) == 0:
+            return
+        path = f"{self.exp_dir}/dynamics-{epoch:0>2}.pkl"
+        hao.paths.make_parent_dirs(hao.paths.get(path))
+        df = pd.DataFrame(dynamics)
+        df.to_pickle(path)
+
     def save_if_should(self):
         if self.state._ckpts.should_save:
-            self.model.on_save_checkpoint()
             self.state._ckpts.path_new = self.save()
             self.callback_handler.on_save_checkpoint()
             self.state._ckpts.should_save = False
 
     def save(self, name: Optional[str] = None):
-        state_dict = {
+        state_dicts = {
             'train_conf': self.train_conf,
             'model_conf': self.model.model_conf,
-            'state': self.state.state_dict(),
-            'state_dict': self.model.state_dict(),
             'optimizer_state_dict': self.optimizer.state_dict(),
             'scheduler_state_dict': self.scheduler.state_dict(),
         }
+        if (peft_config := getattr(self.model, 'peft_config', None)) is None:
+            self.model.on_save_checkpoint()
+            state_dicts['state_dict'] = self.model.state_dict()
+        else:
+            state_dicts['state_dict'] = get_peft_model_state_dict(self.model)
+            state_dicts['peft_config'] = {**peft_config.__dict__ , 'inference_mode': True}
+
         if self.scaler:
-            state_dict['scaler_state_dict'] = self.scaler.state_dict()
+            state_dicts['scaler_state_dict'] = self.scaler.state_dict()
         params = {
-            'model': self.model.__class__.__name__,
-            'corpus': self.train_conf.corpus,
+            'model': self.train_conf.model,
+            'dataset': self.train_conf.dataset,
             'exp': self.trainer_conf.exp or 'na',
             'epoch': self.state.epoch,
             'ts': self.state.ts,
             **{k.replace('/', '_'): f"{v:.4f}" for k, v in self.state.metrics.items() if isinstance(v, (str, int, float, bool))},
         }
         checkpoint_name = name or self.trainer_conf.checkpoint_name
         filename = checkpoint_name.format(**params)
-        path = hao.paths.get('data/checkpoints/', filename)
-        hao.paths.make_parent_dirs(path)
-        torch.save(state_dict, path)
-        LOGGER.debug(f"saved checkpoint: {path}")
-        return path
+        filepath = f"data/checkpoints/{filename}"
+        fullpath = hao.paths.get(filepath)
+        hao.paths.make_parent_dirs(fullpath)
+        torch.save(state_dicts, fullpath)
+        LOGGER.debug(f"saved checkpoint: {filepath}")
+        return filepath
 
     def save_model(self):
         if self.state.epoch <= 0 or len(self.state._ckpts.top_n) == 0:
             return
         checkpoint_path = self.state._ckpts.top_n[0][1]
         if not os.path.isfile(checkpoint_path):
             return
-        path_base, _ = os.path.splitext(os.path.basename(checkpoint_path))
-        model_path = hao.paths.get_path('data', 'model', f"{path_base}.bin")
-        self.model.export_to_model(model_path)
-        LOGGER.info(f"saved model: {model_path}")
+        filebase, _ = os.path.splitext(os.path.basename(checkpoint_path))
+        filepath = f"data/model/{filebase}.bin"
+        fullpath = hao.paths.get(filepath)
+        if (peft_config := getattr(self.model, 'peft_config', None)) is None:
+            self.model.export_to_model(fullpath)
+        else:
+            state_dicts = {
+                'model_conf': self.model.model_conf,
+                'state_dict': get_peft_model_state_dict(self.model),
+                'peft_config': {**peft_config.__dict__ , 'inference_mode': True},
+            }
+            hao.paths.make_parent_dirs(fullpath)
+            torch.save(state_dicts, fullpath)
+        LOGGER.info(f"saved model: {filepath}")
```

