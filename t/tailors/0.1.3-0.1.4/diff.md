# Comparing `tmp/tailors-0.1.3.tar.gz` & `tmp/tailors-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailors-0.1.3.tar", max compression
+gzip compressed data, was "tailors-0.1.4.tar", last modified: Wed May  3 04:12:56 2023, max compression
```

## Comparing `tailors-0.1.3.tar` & `tailors-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,15 @@
--rw-r--r--   0        0        0       32 2022-06-05 07:04:12.137747 tailors-0.1.3/README.md
--rw-r--r--   0        0        0     1168 2022-09-14 10:36:43.549281 tailors-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2875 2022-09-09 03:51:08.837109 tailors-0.1.3/tailors/__init__.py
--rw-r--r--   0        0        0     3735 2022-09-07 06:06:55.756209 tailors-0.1.3/tailors/domains.py
--rw-r--r--   0        0        0     7407 2022-08-19 02:56:09.246403 tailors-0.1.3/tailors/embedders.py
--rw-r--r--   0        0        0      134 2022-08-18 15:03:41.251992 tailors-0.1.3/tailors/exceptions.py
--rw-r--r--   0        0        0        0 2022-06-04 03:01:18.854863 tailors-0.1.3/tailors/fast/__init__.py
--rw-r--r--   0        0        0      577 2022-06-04 04:11:44.405730 tailors-0.1.3/tailors/fast/dates.py
--rw-r--r--   0        0        0     1670 2022-08-18 15:34:53.162413 tailors-0.1.3/tailors/fast/model.py
--rw-r--r--   0        0        0    13143 2022-06-05 23:08:26.867233 tailors-0.1.3/tailors/fast/stopwords.py
--rw-r--r--   0        0        0     1708 2022-06-04 04:34:11.308616 tailors-0.1.3/tailors/fast/texts.py
--rw-r--r--   0        0        0     4014 2022-06-06 15:56:50.144738 tailors-0.1.3/tailors/fast/tokenizer.py
--rw-r--r--   0        0        0    11803 2022-09-08 11:47:53.279289 tailors-0.1.3/tailors/losses.py
--rw-r--r--   0        0        0     1395 2022-09-13 10:46:37.035009 tailors-0.1.3/tailors/metrics/__init__.py
--rw-r--r--   0        0        0      997 2022-09-11 15:40:41.002387 tailors-0.1.3/tailors/metrics/classification_metrics.py
--rw-r--r--   0        0        0      853 2022-09-11 23:57:23.036053 tailors-0.1.3/tailors/metrics/sequence_metrics.py
--rw-r--r--   0        0        0     9758 2022-09-15 10:10:52.362641 tailors-0.1.3/tailors/models.py
--rw-r--r--   0        0        0        0 2022-08-19 02:06:59.762239 tailors-0.1.3/tailors/utils/__init__.py
--rw-r--r--   0        0        0      522 2022-08-19 02:07:12.438057 tailors-0.1.3/tailors/utils/locations.py
--rw-r--r--   0        0        0      890 2022-09-15 16:30:09.706250 tailors-0.1.3/setup.py
--rw-r--r--   0        0        0     1068 2022-09-15 16:30:09.706499 tailors-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-21 14:36:35.493704 tailors-0.1.4/LICENSE
+-rw-r--r--   0        0        0       32 2022-06-05 07:04:12.137747 tailors-0.1.4/README.md
+-rw-r--r--   0        0        0      907 2023-05-03 04:11:54.630248 tailors-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3651 2023-04-23 08:41:07.683317 tailors-0.1.4/tailors/__init__.py
+-rw-r--r--   0        0        0     3818 2023-04-21 08:26:17.073814 tailors-0.1.4/tailors/domains.py
+-rw-r--r--   0        0        0      134 2022-08-18 15:03:41.251992 tailors-0.1.4/tailors/exceptions.py
+-rw-r--r--   0        0        0    12526 2023-04-14 03:44:14.091927 tailors-0.1.4/tailors/losses.py
+-rw-r--r--   0        0        0     1395 2022-09-13 10:46:37.035009 tailors-0.1.4/tailors/metrics/__init__.py
+-rw-r--r--   0        0        0      995 2023-04-21 08:46:46.279605 tailors-0.1.4/tailors/metrics/classification_metrics.py
+-rw-r--r--   0        0        0      853 2022-09-11 23:57:23.036053 tailors-0.1.4/tailors/metrics/sequence_metrics.py
+-rw-r--r--   0        0        0    10326 2023-04-25 10:32:29.107724 tailors-0.1.4/tailors/models.py
+-rw-r--r--   0        0        0     7462 2023-04-22 11:46:16.988917 tailors-0.1.4/tailors/plms.py
+-rw-r--r--   0        0        0        0 2022-08-19 02:06:59.762239 tailors-0.1.4/tailors/utils/__init__.py
+-rw-r--r--   0        0        0      522 2022-08-19 02:07:12.438057 tailors-0.1.4/tailors/utils/locations.py
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 tailors-0.1.4/PKG-INFO
```

### Comparing `tailors-0.1.3/tailors/__init__.py` & `tailors-0.1.4/tailors/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # -*- coding: utf-8 -*-
+__version__ = '0.1.4'
+
 import os
 import random
+from collections import UserDict
+from typing import List
 
 import hao
 import torch
 from decorator import decorator
+from torch.nn import functional as F
 
 LOGGER = hao.logs.get_logger(__name__)
 
 
 def freeze(model):
     for param in model.parameters():
         param.requires_grad = False
@@ -56,18 +61,22 @@
     torch.backends.cudnn.deterministic = deterministic
     torch.backends.cudnn.benchmark = benchmark
 
 
 def move_to_device(data, device, non_blocking=True):
     if device is None:
         return
-    if isinstance(data, dict):
+    if isinstance(data, (dict, UserDict)):
         return {k: move_to_device(v, device, non_blocking) for k, v in data.items()}
     elif isinstance(data, tuple):
-        return tuple([move_to_device(v, device, non_blocking) for v in data])
+        if hasattr(data, '_asdict') and hasattr(data, '_fields'):
+            cls = type(data)
+            return cls(*[move_to_device(v, device, non_blocking) for v in data])
+        else:
+            return tuple([move_to_device(v, device, non_blocking) for v in data])
     elif isinstance(data, list):
         return [move_to_device(v, device, non_blocking) for v in data]
     elif isinstance(data, torch.Tensor):
         return data.to(device, non_blocking=non_blocking)
     return data
 
 
@@ -88,7 +97,23 @@
     elif isinstance(data, tuple):
         return tuple([off_tensor(v) for v in data])
     elif isinstance(data, list):
         return [off_tensor(v) for v in data]
     elif isinstance(data, torch.Tensor):
         return data.detach().cpu() if data.is_sparse else data.tolist()
     return data
+
+
+def append_batch(items, batch):
+    batch = off_tensor(batch)
+    if isinstance(batch, tuple):
+        hao.lists.add_tuple_to_list(items, batch)
+    elif isinstance(batch, torch.Tensor):
+        items.append(batch)
+    else:
+        items.extend(batch)
+
+
+def multi_hot(items: List[int], n_classes: int, dtype=torch.float32):
+    data = torch.LongTensor(items)
+    onehot = F.one_hot(data, num_classes=n_classes)
+    return onehot.sum(dim=0).to(dtype)
```

### Comparing `tailors-0.1.3/tailors/domains.py` & `tailors-0.1.4/tailors/domains.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # -*- coding: utf-8 -*-
 import itertools
+from collections import namedtuple
 from dataclasses import dataclass
 from typing import List, Optional, Union
 
 import hao
 
+Example = namedtuple('Example', ['idx', 'features', 'target'])
+
 
 class Derivable:
 
     @classmethod
     def subclasses(cls):
         all_subclasses = []
         for subclass in cls.__subclasses__():
@@ -33,23 +36,24 @@
 
     @staticmethod
     def build_mappings(tags: List[str],
                        supporting_tags: Optional[List[str]] = None,
                        trivial_tag: str = 'O',
                        is_bies = False):
         assert tags is not None and len(tags) > 0, 'expecting `tags` of list of str'
-        assert trivial_tag not in tags, '`tags` should not contain `trivial_tag`'
         if supporting_tags:
             assert all(tag not in tags for tag in supporting_tags), '`tags` should not contain any of `supporting_tags`'
 
         tags, supporting_tags = hao.lists.uniquify(tags), hao.lists.uniquify(supporting_tags)
         if is_bies:
             prefixes = ('B-', 'I-', 'E-', 'S-')
             tags = [f"{prefix}{tag}" for tag, prefix in itertools.product(tags, prefixes)]
-        tags_all = tags + (supporting_tags or []) + [trivial_tag]
+        tags_all = tags + (supporting_tags or [])
+        if trivial_tag not in tags_all:
+            tags_all.append(trivial_tag)
 
         tag2id = {tag: i for i, tag in enumerate(tags_all)}
         id2tag = {i: tag for i, tag in enumerate(tags_all)}
         return tag2id, id2tag, len(tags_all)
 
     def get_id_by_tag(self, tag: str, default=None, ignore_supporting=False):
         if ignore_supporting and tag in self.supporting_tag:
@@ -72,14 +76,15 @@
 
     def is_supporting_tag_id(self, _id):
         return _id in self.supporting_tag_ids
 
     def is_not_supporting_tag_id(self, _id):
         return not self.is_supporting_tag_id(_id)
 
+
 @dataclass
 class Factor:
     factor: float
     min_val: float = 1e-10
     max_val: float = 1e-1
 
     def apply(self, v: Union[int, float]):
```

### Comparing `tailors-0.1.3/tailors/embedders.py` & `tailors-0.1.4/tailors/plms.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 # -*- coding: utf-8 -*-
 import abc
 import tempfile
 
 import hao
-from transformers import (
-    BertModel,
-    BertTokenizerFast,
-    ElectraModel,
-    ElectraTokenizerFast,
-    PreTrainedModel,
-    PreTrainedTokenizerFast,
-    XLNetModel,
-    XLNetTokenizerFast,
-)
+from transformers import (BertModel, BertTokenizerFast, ElectraModel,
+                          ElectraTokenizerFast, PreTrainedModel,
+                          PreTrainedTokenizerFast, XLNetModel,
+                          XLNetTokenizerFast)
 
 from tailors import freeze
 from tailors.domains import Derivable
 
 
-class Embedder(abc.ABC, Derivable):
+class PLM(abc.ABC, Derivable):
     def __init__(self, model_conf) -> None:
         super().__init__(model_conf)
         self.model_conf = model_conf
         self.tokenizer = self.build_tokenizer()
-        self.embedding = self.build_embedding()
+        self.plm = self.build_plm()
+
+    @property
+    def config(self):
+        return self.plm.config
 
     def get_additional_tokens_for_tokenizer(self):
         return []
 
     @abc.abstractmethod
     def build_tokenizer(self) -> PreTrainedTokenizerFast:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def build_embedding(self) -> PreTrainedModel:
+    def build_plm(self) -> PreTrainedModel:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get_embedding_size(self):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def on_save_checkpoint(self, checkpoint) -> None:
         raise NotImplementedError()
 
     @staticmethod
     def get_pretrained_model_path(model: str):
         # hao.oss.init(f"pretrained.{model}", config='tailors.yml')
-        return hao.config.get_path(f"pretrained.{model}.local", config='tailors.yml')
+        key = f"pretrained.{model}.local"
+        return hao.config.get_path(key) or hao.config.get_path(key, config='tailors.yml')
 
 
-class Bert(Embedder):
+class Bert(PLM):
 
     def build_tokenizer(self):
         if hasattr(self.model_conf, 'vocab'):
             with tempfile.NamedTemporaryFile() as f:
                 f.write(self.model_conf.vocab.encode())
                 tokenizer = BertTokenizerFast(vocab_file=f.name)
                 if hasattr(self.model_conf, 'additional_special_tokens'):
@@ -64,38 +63,38 @@
             pretrained_model_path = self.get_pretrained_model_path('bert')
             tokenizer = BertTokenizerFast.from_pretrained(pretrained_model_path)
             additional_special_tokens = self.get_additional_tokens_for_tokenizer()
             if additional_special_tokens is not None and len(additional_special_tokens) > 0:
                 tokenizer.add_special_tokens({'additional_special_tokens': additional_special_tokens})
             return tokenizer
 
-    def build_embedding(self):
+    def build_plm(self):
         if hasattr(self.model_conf, 'bert_config'):
             bert = BertModel(self.model_conf.bert_config)
         else:
             pretrained_model_path = self.get_pretrained_model_path('bert')
             bert = BertModel.from_pretrained(pretrained_model_path)
         if self.model_conf.freeze_embedding:
             freeze(bert)
         return bert
 
     def get_embedding_size(self):
-        return self.embedding.config.hidden_size
+        return self.plm.config.hidden_size
 
     def on_save_checkpoint(self) -> None:
         if not hasattr(self.model_conf, 'vocab'):
             pretrained_model_path = self.get_pretrained_model_path('bert')
             path_vocab_file = hao.paths.get_path(pretrained_model_path, 'vocab.txt')
             self.model_conf.vocab = open(path_vocab_file).read()
         if len(self.tokenizer.additional_special_tokens) > 0:
             self.model_conf.additional_special_tokens = self.tokenizer.additional_special_tokens
-        self.model_conf.bert_config = self.embedding.config
+        self.model_conf.bert_config = self.plm.config
 
 
-class XLNet(Embedder):
+class XLNet(PLM):
 
     def build_tokenizer(self):
         if hasattr(self.model_conf, 'vocab'):
             with tempfile.NamedTemporaryFile() as f:
                 f.write(self.model_conf.vocab)
                 tokenizer = XLNetTokenizerFast(vocab_file=f.name)
                 if hasattr(self.model_conf, 'additional_special_tokens'):
@@ -105,38 +104,38 @@
             pretrained_model_path = self.get_pretrained_model_path('xlnet')
             tokenizer = XLNetTokenizerFast.from_pretrained(pretrained_model_path)
             additional_special_tokens = self.get_additional_tokens_for_tokenizer()
             if additional_special_tokens is not None and len(additional_special_tokens) > 0:
                 tokenizer.add_special_tokens({'additional_special_tokens': additional_special_tokens})
             return tokenizer
 
-    def build_embedding(self):
+    def build_plm(self):
         if hasattr(self.model_conf, 'xlnet_config'):
             xlnet = XLNetModel(self.model_conf.xlnet_config)
         else:
             pretrained_model_path = self.get_pretrained_model_path('xlnet')
             xlnet = XLNetModel.from_pretrained(pretrained_model_path)
         if self.model_conf.freeze_embedding:
             freeze(xlnet)
         return xlnet
 
     def get_embedding_size(self):
-        return self.embedding.config.d_model
+        return self.plm.config.d_model
 
     def on_save_checkpoint(self) -> None:
         if not hasattr(self.model_conf, 'vocab'):
             pretrained_model_path = self.get_pretrained_model_path('xlnet')
             path_vocab_file = hao.paths.get_path(pretrained_model_path, 'spiece.model')
             self.model_conf.vocab = open(path_vocab_file, 'rb').read()
         if len(self.tokenizer.additional_special_tokens) > 0:
             self.model_conf.additional_special_tokens = self.tokenizer.additional_special_tokens
-        self.model_conf.xlnet_config = self.embedding.config
+        self.model_conf.xlnet_config = self.plm.config
 
 
-class Electra(Embedder):
+class Electra(PLM):
 
     def build_tokenizer(self):
         if hasattr(self.model_conf, 'vocab'):
             with tempfile.NamedTemporaryFile() as f:
                 f.write(self.model_conf.vocab.encode())
                 tokenizer = ElectraTokenizerFast(vocab_file=f.name)
                 if hasattr(self.model_conf, 'additional_special_tokens'):
@@ -146,32 +145,32 @@
             pretrained_model_path = self.get_pretrained_model_path('electra')
             tokenizer = ElectraTokenizerFast.from_pretrained(pretrained_model_path)
             additional_special_tokens = self.get_additional_tokens_for_tokenizer()
             if additional_special_tokens is not None and len(additional_special_tokens) > 0:
                 tokenizer.add_special_tokens({'additional_special_tokens': additional_special_tokens})
             return tokenizer
 
-    def build_embedding(self):
+    def build_plm(self):
         if hasattr(self.model_conf, 'electra_config'):
             electra = ElectraModel(self.model_conf.electra_config)
         else:
             pretrained_model_path = self.get_pretrained_model_path('electra')
             electra = ElectraModel.from_pretrained(pretrained_model_path)
         if self.model_conf.freeze_embedding:
             freeze(electra)
         return electra
 
     def get_embedding_size(self):
-        return self.embedding.config.hidden_size
+        return self.plm.config.hidden_size
 
     def on_save_checkpoint(self) -> None:
         if not hasattr(self.model_conf, 'vocab'):
             pretrained_model_path = self.get_pretrained_model_path('electra')
             path_vocab_file = hao.paths.get_path(pretrained_model_path, 'vocab.txt')
             self.model_conf.vocab = open(path_vocab_file).read()
         if len(self.tokenizer.additional_special_tokens) > 0:
             self.model_conf.additional_special_tokens = self.tokenizer.additional_special_tokens
-        self.model_conf.electra_config = self.embedding.config
+        self.model_conf.electra_config = self.plm.config
 
 
-def list_embedders():
-    return Embedder.subclasses()
+def list_plms():
+    return PLM.subclasses()
```

### Comparing `tailors-0.1.3/tailors/losses.py` & `tailors-0.1.4/tailors/losses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 from typing import Optional
 
 import torch
 import torch.nn as nn
-from tailors.exceptions import TailorsError
 from torch import Tensor
 from torch.autograd import Variable
-from torch.nn import functional
+from torch.nn import functional as F
+
+from tailors.exceptions import TailorsError
 
 
 class FocalLoss(nn.Module):
     def __init__(self, gamma=0, alpha=None, size_average=True):
         super(FocalLoss, self).__init__()
         self.gamma = gamma
         self.alpha = alpha
@@ -147,15 +148,15 @@
             loss = 1 - ((2 * intersection + self.smooth) /
                         (torch.sum(torch.square(flat_input, ), -1) + torch.sum(torch.square(flat_target), -1) + self.smooth))
 
         return loss
 
     def _multiple_class(self, logits, target, logits_size, mask=None):
         flat_input = logits
-        flat_target = functional.one_hot(target, num_classes=logits_size).float() if self.index_label_position else target.float()
+        flat_target = F.one_hot(target, num_classes=logits_size).float() if self.index_label_position else target.float()
         flat_input = torch.nn.Softmax(dim=1)(flat_input) if self.with_logits else flat_input
 
         if mask is not None:
             mask = mask.float()
             flat_input = flat_input * mask
             flat_target = flat_target * mask
         else:
@@ -243,15 +244,15 @@
     def __str__(self):
         return f"Dice Loss smooth:{self.smooth}, ohem: {self.ohem_ratio}, alpha: {self.alpha}"
 
     def __repr__(self):
         return str(self)
 
 
-class GPLoss(nn.Module):
+class GlobalPointerLoss(nn.Module):
     """https://kexue.fm/archives/7359"""
 
     def forward(self, y_pred, y_true):
         if y_true.is_sparse:
             y_true = y_true.to_dense()
         bz, n_heads = y_pred.shape[:2]
         y_true = y_true.reshape([bz * n_heads, -1])
@@ -265,22 +266,43 @@
         y_pred_neg = torch.cat([y_pred_neg, zeros], dim=-1)
         y_pred_pos = torch.cat([y_pred_pos, zeros], dim=-1)
         neg_loss = torch.logsumexp(y_pred_neg, dim=-1)
         pos_loss = torch.logsumexp(y_pred_pos, dim=-1)
         return (neg_loss + pos_loss).mean()
 
 
+class RDropLoss(nn.Module):
+    """https://github.com/dropreg/R-Drop"""
+
+    def __init__(self, alpha=4):
+        super().__init__()
+        self.alpha = alpha
+        self.ce = nn.CrossEntropyLoss(reduction='none')
+        self.kld = nn.KLDivLoss(reduction='none')
+
+    def forward(self, logits1, logits2, target):
+        ce_loss = (self.ce(logits1, target) + self.ce(logits2, target)) / 2
+
+        prob1 = F.log_softmax(logits1, dim=-1)
+        prob2 = F.log_softmax(logits2, dim=-1)
+        kl_loss1 = self.kld(prob1, prob2).sum(-1)
+        kl_loss2 = self.kld(prob2, prob1).sum(-1)
+        kl_loss = (kl_loss1 + kl_loss2) / 2
+        return ce_loss + kl_loss * self.alpha
+
+
 LOSSES = {
     'ce': nn.CrossEntropyLoss,
     'bce': nn.BCELoss,
     'bce-l': nn.BCEWithLogitsLoss,
     'l1': nn.L1Loss,
     'focal': FocalLoss,
     'dice': DiceLoss,
-    'gp': GPLoss,
+    'gp': GlobalPointerLoss,
+    'r-drop': RDropLoss,
 }
 
 
 def get(name: str):
     assert name is not None
     loss = LOSSES.get(name)
     if loss is None:
```

### Comparing `tailors-0.1.3/tailors/metrics/__init__.py` & `tailors-0.1.4/tailors/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tailors-0.1.3/tailors/metrics/classification_metrics.py` & `tailors-0.1.4/tailors/metrics/classification_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 precision_recall_fscore_support = functools.partial(metrics.precision_recall_fscore_support, average='micro', zero_division=0)
 classification_report = functools.partial(metrics.classification_report, digits=4, zero_division=0)
 
 
 def calculate(target, preds, labels: Optional[List[str]] = None):
     if isinstance(target, torch.Tensor):
         targets = target.tolist()
-    precision, recall, f1, _ = precision_recall_fscore_support(targets, targets, labels=labels)
+    precision, recall, f1, _ = precision_recall_fscore_support(targets, preds, labels=labels)
     report = classification_report(targets, preds, labels=labels)
     return {'precision': precision, 'recall': recall, 'f1': f1, 'report': report}
```

### Comparing `tailors-0.1.3/tailors/metrics/sequence_metrics.py` & `tailors-0.1.4/tailors/metrics/sequence_metrics.py`

 * *Files identical despite different names*

### Comparing `tailors-0.1.3/tailors/models.py` & `tailors-0.1.4/tailors/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 from typing import Dict, Iterator, List, Optional, Union
 
 import hao
 import torch
 import torch.nn as nn
 from hao.namespaces import attr, from_args
 from hao.stopwatch import Stopwatch
+from peft import get_peft_config, get_peft_model, set_peft_model_state_dict
 from torch.nn import DataParallel
 from torch.nn.parallel import DistributedDataParallel
 from torch.utils.data.dataloader import default_collate
 from transformers import PreTrainedModel, PreTrainedTokenizerFast
 
 import tailors
-from tailors.domains import Factor, Tags
+from tailors.domains import Example, Factor, Tags
 from tailors.exceptions import TailorsError
 
 LOGGER = hao.logs.get_logger(__name__)
 
 
 @from_args
 class TailorsConf:
@@ -55,14 +56,15 @@
     @staticmethod
     def encode(text_or_tokens: Union[str, List[str]],
                tokenizer: PreTrainedTokenizerFast,
                seq_len: int,
                add_special_tokens=True,
                padding: Union[bool, str] = 'max_length',
                truncation: Union[bool, str] = True,
+               return_offsets_mapping: bool = True,
                return_tensors: Optional[str] = 'pt'):
         is_text = isinstance(text_or_tokens, str)
         if is_text:
             encoder = tokenizer.encode_plus
         else:
             encoder = tokenizer.prepare_for_model
             if text_or_tokens and isinstance(text_or_tokens[0], str):
@@ -71,35 +73,35 @@
             text_or_tokens,
             add_special_tokens=add_special_tokens,
             max_length=seq_len,
             padding=padding,
             truncation=truncation,
             return_attention_mask=True,
             return_token_type_ids=True,
-            return_offsets_mapping=True,
+            return_offsets_mapping=return_offsets_mapping,
             return_tensors=return_tensors,
         )
         input_ids = encoded.get("input_ids")
         attention_mask = encoded.get("attention_mask")
         token_type_ids = encoded.get("token_type_ids")
 
         if return_tensors:
             input_ids = input_ids.squeeze()
             attention_mask = attention_mask.squeeze()
             token_type_ids = token_type_ids.squeeze()
 
-        if is_text:
+        if is_text and return_offsets_mapping:
             offset_mapping = encoded.get("offset_mapping")
             if return_tensors:
                 offset_mapping = offset_mapping[0].tolist() if offset_mapping is not None else None
             return input_ids, attention_mask, token_type_ids, offset_mapping
         else:
             return input_ids, attention_mask, token_type_ids
 
-    def from_line(self, line: str):
+    def from_line(self, line: str) -> Union[Example, List[Example]]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def for_inference(self, lines: List[str], bz: int = 32, *args, **kwargs):
         raise NotImplementedError()
 
     @abc.abstractmethod
@@ -123,15 +125,15 @@
     def __init__(self, model_conf: TailorsConf):
         super().__init__()
         self.device = None
         assert model_conf.meta is not None, '`meta` must be populated manually'
         self.model_conf = model_conf
 
         self.io: TailorsIO = self.get_io()
-        self.embedding = self.build_embedding()
+        self.plm = self.build_plm()
 
     def freeze(self):
         tailors.freeze(self)
         self.eval()
 
     def unfreeze(self) -> None:
         tailors.unfreeze(self)
@@ -144,15 +146,15 @@
         return self
 
     @abc.abstractmethod
     def build_tokenizer(self) -> PreTrainedTokenizerFast:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def build_embedding(self) -> PreTrainedModel:
+    def build_plm(self) -> PreTrainedModel:
         raise NotImplementedError()
 
     def on_save_checkpoint(self):
         pass
 
     def get_io(self):
         class_name = f"{self.__class__.__name__}IO"
@@ -171,45 +173,53 @@
     def forward(self, *args, **kwargs):
         features, = args
         logits, mask = self.encode(features)
         return self.decode(logits, mask)
 
     @abc.abstractmethod
     def encode(self, *args, **kwargs):
+        """Make sure always return logits as the only/first value"""
         raise NotImplementedError()
 
     @abc.abstractmethod
     def decode(self, *args, **kwargs):
         raise NotImplementedError()
 
     def lr_factors(self) -> Dict[str, Factor]:
         return {
             'embedding': Factor(factor=0.1, max_val=1e-4),
             'crf': Factor(factor=1000, max_val=5e-2),
         }
 
     @classmethod
-    def load(cls, path_or_key: str, use_gpu = True):
+    def from_pretrained(cls, path_or_key: str, use_gpu = True):
         if inspect.isabstract(cls):
             raise TailorsError(f"Not supported call from abstract class: {cls.__name__}")
 
         if ".local" in path_or_key:  # do not use SEQUE_CONFIG, since it's not called in this lib project
             hao.oss.init(path_or_key[: path_or_key.rfind(".")])
-            model_path = hao.config.get_path(path_or_key)
+            model_path = hao.config.get(path_or_key)
         else:
-            model_path = hao.paths.get_path(path_or_key)
+            model_path = path_or_key
+        fullpath = hao.paths.get(model_path)
 
-        if model_path is None or not os.path.isfile(model_path):
+        if model_path is None or not os.path.isfile(fullpath):
             raise TailorsError(f"model not found: {model_path}")
 
         LOGGER.info(f"[{cls.__name__}] loading from: {model_path}")
         sw = Stopwatch()
-        state_dict = torch.load(model_path)
-        model = cls(state_dict.get('model_conf'))
-        model.load_state_dict(state_dict.get('state_dict'))
+        state_dicts = torch.load(fullpath)
+        state_dict = state_dicts.get('state_dict')
+        model = cls(state_dicts.get('model_conf'))
+        if (peft_config := state_dicts.get('peft_config')) is None:
+            model.load_state_dict(state_dict)
+        else:
+            model = get_peft_model(model, get_peft_config(peft_config))
+            set_peft_model_state_dict(model, state_dict)
+
         model.freeze()
         LOGGER.info(f"[{cls.__name__}] loaded, took: {sw.took()}")
 
         if use_gpu:
             device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
             model.use_device(device)
         return model
@@ -219,17 +229,17 @@
         raise NotImplementedError()
 
     def export_to_model(self, output_path):
         is_dp_module = isinstance(self, (DistributedDataParallel, DataParallel))
         model = self.module if is_dp_module else self
 
         model.on_save_checkpoint()
-        checkpoint = {'state_dict': model.state_dict(), 'model_conf': model.model_conf}
+        state_dicts = {'state_dict': model.state_dict(), 'model_conf': model.model_conf}
         hao.paths.make_parent_dirs(output_path)
-        torch.save(checkpoint, output_path)
+        torch.save(state_dicts, output_path)
 
     def export_to_onnx(self, output_path):
         torch.onnx.export(
             self,
             self.io.empty_input,
             output_path,
             verbose=False,
@@ -252,15 +262,15 @@
     def to_model(cls, model_path, output_path=None):
         if model_path is None:
             raise TailorsError('empty output_path')
         model_path = hao.paths.get_path(model_path)
         if not os.path.exists(model_path):
             raise TailorsError(f'model_path not exist: {model_path}')
 
-        model = cls.load(model_path)
+        model = cls.from_pretrained(model_path)
         if output_path is None:
             path_base, _ = os.path.splitext(os.path.basename(model_path))
             output_path = hao.paths.get_path('data', 'model', f"{path_base}.bin")
         hao.paths.make_parent_dirs(output_path)
         model.export_to_model(output_path)
         return output_path
 
@@ -268,14 +278,14 @@
     def to_onnx(cls, model_path, output_path=None):
         if model_path is None:
             raise TailorsError('empty output_path')
         model_path = hao.paths.get_path(model_path)
         if not os.path.exists(model_path):
             raise TailorsError(f'model_path not exist: {model_path}')
 
-        model = cls.load(model_path)
+        model = cls.from_pretrained(model_path)
         if output_path is None:
             path_base, _ = os.path.splitext(os.path.basename(model_path))
             output_path = hao.paths.get_path('data', 'model', f"{path_base}.onnx")
         hao.paths.make_parent_dirs(output_path)
         model.export_to_onnx(output_path)
         return output_path
```

### Comparing `tailors-0.1.3/tailors/utils/locations.py` & `tailors-0.1.4/tailors/utils/locations.py`

 * *Files identical despite different names*

