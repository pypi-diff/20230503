# Comparing `tmp/recurrent-memory-transformer-pytorch-0.2.2.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.2.2.tar", last modified: Wed Apr 26 14:45:51 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.2.3.tar", last modified: Wed May  3 14:42:35 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.2.2.tar` & `recurrent-memory-transformer-pytorch-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:51.451192 recurrent-memory-transformer-pytorch-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 14:45:14.000000 recurrent-memory-transformer-pytorch-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 14:45:51.451192 recurrent-memory-transformer-pytorch-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-04-26 14:45:14.000000 recurrent-memory-transformer-pytorch-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:51.447193 recurrent-memory-transformer-pytorch-0.2.2/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-26 14:45:14.000000 recurrent-memory-transformer-pytorch-0.2.2/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-26 14:45:14.000000 recurrent-memory-transformer-pytorch-0.2.2/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-04-26 14:45:14.000000 recurrent-memory-transformer-pytorch-0.2.2/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:45:51.451192 recurrent-memory-transformer-pytorch-0.2.2/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 14:45:51.000000 recurrent-memory-transformer-pytorch-0.2.2/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 14:45:51.000000 recurrent-memory-transformer-pytorch-0.2.2/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:45:51.000000 recurrent-memory-transformer-pytorch-0.2.2/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 14:45:51.000000 recurrent-memory-transformer-pytorch-0.2.2/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 14:45:51.000000 recurrent-memory-transformer-pytorch-0.2.2/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 14:45:51.451192 recurrent-memory-transformer-pytorch-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-26 14:45:14.000000 recurrent-memory-transformer-pytorch-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:42:35.325415 recurrent-memory-transformer-pytorch-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 14:42:19.000000 recurrent-memory-transformer-pytorch-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 14:42:35.325415 recurrent-memory-transformer-pytorch-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-03 14:42:19.000000 recurrent-memory-transformer-pytorch-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:42:35.325415 recurrent-memory-transformer-pytorch-0.2.3/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 14:42:19.000000 recurrent-memory-transformer-pytorch-0.2.3/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-03 14:42:19.000000 recurrent-memory-transformer-pytorch-0.2.3/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-05-03 14:42:19.000000 recurrent-memory-transformer-pytorch-0.2.3/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:42:35.325415 recurrent-memory-transformer-pytorch-0.2.3/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 14:42:35.000000 recurrent-memory-transformer-pytorch-0.2.3/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-03 14:42:35.000000 recurrent-memory-transformer-pytorch-0.2.3/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:42:35.000000 recurrent-memory-transformer-pytorch-0.2.3/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 14:42:35.000000 recurrent-memory-transformer-pytorch-0.2.3/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 14:42:35.000000 recurrent-memory-transformer-pytorch-0.2.3/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:42:35.325415 recurrent-memory-transformer-pytorch-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-03 14:42:19.000000 recurrent-memory-transformer-pytorch-0.2.3/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.2/LICENSE` & `recurrent-memory-transformer-pytorch-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.2.2/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.2.2
+Version: 0.2.3
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.2/README.md` & `recurrent-memory-transformer-pytorch-0.2.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 <img src="./rmt.png" width="450px"></img>
 
 ## Recurrent Memory Transformer - Pytorch
 
 Implementation of <a href="https://arxiv.org/abs/2207.06881">Recurrent Memory Transformer</a> <a href="https://openreview.net/forum?id=Uynr3iPhksa">(openreview)</a> in Pytorch. They had <a href="https://arxiv.org/abs/2304.11062">a short follow up paper</a> recently that demonstrated it was able to copy information across 1 million tokens at the very least.
 
+There is no doubt in my mind that RMT would make a stronger RL agent than <a href="https://sites.google.com/view/adaptive-agent/">AdA</a>, which is just a Transformer-XL
+
+<a href="https://www.youtube.com/watch?v=4Cclp6yPDuw">Yannic Kilcher paper review</a>
+
 ## Appreciation
 
 - <a href="https://stability.ai/">Stability</a> and <a href="https://huggingface.co/">🤗 Huggingface</a> for their generous sponsorships to work on and open source cutting edge artificial intelligence research
 
 ## Install
 
 ```bash
@@ -38,14 +42,43 @@
 logits2, mem2, _ = model(x, mem1)  # (1, 1024, 20000), (1, 128, 512), None
 logits3, mem3, _ = model(x, mem2)  # (1, 1024, 20000), (1, 128, 512), None
 
 # and so on ...
 
 ```
 
+With XL memories
+
+```python
+import torch
+from recurrent_memory_transformer_pytorch import RecurrentMemoryTransformer
+
+model = RecurrentMemoryTransformer(
+    num_tokens = 20000,
+    num_memory_tokens = 128,
+    dim = 512,
+    depth = 6,
+    causal = True,
+    dim_head = 64,
+    heads = 8,
+    seq_len = 1024,
+    use_flash_attn = True,
+    use_xl_memories = True,    # set this to True
+    xl_mem_len = 512           # can be shorter than the seq len - i think just having a bit of the past will prevent much of the RMT memories  memorizing the immediate preceding text
+)
+
+x = torch.randint(0, 256, (1, 1024))
+
+logits1, mem1, xl_mem1 = model(x)                               # (1, 1024, 20000), (1, 128, 512), [(2, 1, 512, 512)]
+logits2, mem2, xl_mem2 = model(x, mem1, xl_memories = xl_mem1)  # (1, 1024, 20000), (1, 128, 512), [(2, 1, 512, 512)]
+logits3, mem3, xl_mem3 = model(x, mem2, xl_memories = xl_mem2)  # (1, 1024, 20000), (1, 128, 512), [(2, 1, 512, 512)]
+
+# and so on ...
+```
+
 Train on an absurdly long sequence
 
 ```python
 import torch
 from recurrent_memory_transformer_pytorch import (
     RecurrentMemoryTransformer,
     RecurrentMemoryTransformerWrapper
@@ -68,14 +101,15 @@
 loss = model(seq, memory_replay_backprop = True) # memory efficient training from memformer paper
 
 ```
 
 ## Todo
 
 - [ ] get rotary embeddings working properly with xl memories
+- [ ] test on long context genomics, do bidirectional RMT on reverse complement and concat
 
 - [x] add xl memories, detached
 - [x] offer a way to turn off rotary embeddings, absolute positional embeddings, and add token shift
 - [x] make memories being causally masked an option
 - [x] add the memory replay backprop technique from memformer paper
 - [x] relative positional encoding
```

#### html2text {}

```diff
@@ -1,76 +1,91 @@
 [./rmt.png] ## Recurrent Memory Transformer - Pytorch Implementation of
 Recurrent_Memory_Transformer (openreview) in Pytorch. They had a_short_follow
 up_paper recently that demonstrated it was able to copy information across 1
-million tokens at the very least. ## Appreciation - Stability and ð¤
-Huggingface for their generous sponsorships to work on and open source cutting
-edge artificial intelligence research ## Install ```bash $ pip install
-recurrent-memory-transformer-pytorch ``` ## Usage ```python import torch from
+million tokens at the very least. There is no doubt in my mind that RMT would
+make a stronger RL agent than AdA, which is just a Transformer-XL Yannic
+Kilcher_paper_review ## Appreciation - Stability and ð¤_Huggingface for their
+generous sponsorships to work on and open source cutting edge artificial
+intelligence research ## Install ```bash $ pip install recurrent-memory-
+transformer-pytorch ``` ## Usage ```python import torch from
 recurrent_memory_transformer_pytorch import RecurrentMemoryTransformer model =
 RecurrentMemoryTransformer( num_tokens = 20000, # number of tokens
 num_memory_tokens = 128, # number of memory tokens, this will determine the
 bottleneck for information being passed to the future dim = 512, # model
 dimensions depth = 6, # transformer depth causal = True, # autoregressive or
 not dim_head = 64, # dimension per head heads = 8, # heads seq_len = 1024, #
 sequence length of a segment use_flash_attn = True # whether to use flash
 attention ) x = torch.randint(0, 256, (1, 1024)) logits1, mem1, _ = model(x) #
 (1, 1024, 20000), (1, 128, 512), None logits2, mem2, _ = model(x, mem1) # (1,
 1024, 20000), (1, 128, 512), None logits3, mem3, _ = model(x, mem2) # (1, 1024,
-20000), (1, 128, 512), None # and so on ... ``` Train on an absurdly long
-sequence ```python import torch from recurrent_memory_transformer_pytorch
-import ( RecurrentMemoryTransformer, RecurrentMemoryTransformerWrapper ) model
-= RecurrentMemoryTransformer( num_tokens = 256, num_memory_tokens = 128, dim =
+20000), (1, 128, 512), None # and so on ... ``` With XL memories ```python
+import torch from recurrent_memory_transformer_pytorch import
+RecurrentMemoryTransformer model = RecurrentMemoryTransformer( num_tokens =
+20000, num_memory_tokens = 128, dim = 512, depth = 6, causal = True, dim_head =
+64, heads = 8, seq_len = 1024, use_flash_attn = True, use_xl_memories = True, #
+set this to True xl_mem_len = 512 # can be shorter than the seq len - i think
+just having a bit of the past will prevent much of the RMT memories memorizing
+the immediate preceding text ) x = torch.randint(0, 256, (1, 1024)) logits1,
+mem1, xl_mem1 = model(x) # (1, 1024, 20000), (1, 128, 512), [(2, 1, 512, 512)]
+logits2, mem2, xl_mem2 = model(x, mem1, xl_memories = xl_mem1) # (1, 1024,
+20000), (1, 128, 512), [(2, 1, 512, 512)] logits3, mem3, xl_mem3 = model(x,
+mem2, xl_memories = xl_mem2) # (1, 1024, 20000), (1, 128, 512), [(2, 1, 512,
+512)] # and so on ... ``` Train on an absurdly long sequence ```python import
+torch from recurrent_memory_transformer_pytorch import
+( RecurrentMemoryTransformer, RecurrentMemoryTransformerWrapper ) model =
+RecurrentMemoryTransformer( num_tokens = 256, num_memory_tokens = 128, dim =
 512, depth = 6, seq_len = 1024, use_flash_attn = True, causal = True ) model =
 RecurrentMemoryTransformerWrapper(model).cuda() seq = torch.randint(0, 256, (4,
 65536)).cuda() # absurdly long sequence, in reality, they curriculum learned
 this starting with 1 segment to about 7-8 segments loss = model(seq,
 memory_replay_backprop = True) # memory efficient training from memformer paper
-``` ## Todo - [ ] get rotary embeddings working properly with xl memories - [x]
-add xl memories, detached - [x] offer a way to turn off rotary embeddings,
-absolute positional embeddings, and add token shift - [x] make memories being
-causally masked an option - [x] add the memory replay backprop technique from
-memformer paper - [x] relative positional encoding ## Alternatives - Block
-Recurrent_Transformer - Memformer ## Citations ```bibtex @inproceedings
-{bulatov2022recurrent, title = {Recurrent Memory Transformer}, author = {Aydar
-Bulatov and Yuri Kuratov and Mikhail Burtsev}, booktitle = {Advances in Neural
-Information Processing Systems}, editor = {Alice H. Oh and Alekh Agarwal and
-Danielle Belgrave and Kyunghyun Cho}, year = {2022}, url = {https://
-openreview.net/forum?id=Uynr3iPhksa} } ``` ```bibtex @misc{bulatov2023scaling,
-title = {Scaling Transformer to 1M tokens and beyond with RMT}, author = {Aydar
-Bulatov and Yuri Kuratov and Mikhail S. Burtsev}, year = {2023}, eprint =
-{2304.11062}, archivePrefix = {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex
-@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
-Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
-Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
-booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
-} ``` ```bibtex @misc{shazeer2020glu, title = {GLU Variants Improve
-Transformer}, author = {Noam Shazeer}, year = {2020}, url = {https://arxiv.org/
-abs/2002.05202} } ``` ```bibtex @misc{su2021roformer, title = {RoFormer:
-Enhanced Transformer with Rotary Position Embedding}, author = {Jianlin Su and
-Yu Lu and Shengfeng Pan and Bo Wen and Yunfeng Liu}, year = {2021}, eprint =
-{2104.09864}, archivePrefix = {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex
-@inproceedings{Wu2020MemformerAM, title = {Memformer: A Memory-Augmented
-Transformer for Sequence Modeling}, author = {Qingyang Wu and Zhenzhong Lan and
-Kun Qian and Jing Gu and Alborz Geramifard and Zhou Yu}, booktitle = {AACL/
-IJCNLP}, year = {2020} } ``` ```bibtex @software{peng_bo_2021_5196578, author =
-{PENG Bo}, title = {BlinkDL/RWKV-LM: 0.01}, month = {aug}, year = {2021},
-publisher = {Zenodo}, version = {0.01}, doi = {10.5281/zenodo.5196578}, url =
-{https://doi.org/10.5281/zenodo.5196578} } ``` ```bibtex @misc{ding2021cogview,
-title = {CogView: Mastering Text-to-Image Generation via Transformers}, author
-= {Ming Ding and Zhuoyi Yang and Wenyi Hong and Wendi Zheng and Chang Zhou and
-Da Yin and Junyang Lin and Xu Zou and Zhou Shao and Hongxia Yang and Jie Tang},
-year = {2021}, eprint = {2105.13290}, archivePrefix = {arXiv}, primaryClass =
-{cs.CV} } ``` ```bibtex @software{Dayma_DALLE_Mini_2021, author = {Dayma, Boris
-and Patil, Suraj and Cuenca, Pedro and Saifullah, Khalid and Abraham, Tanishq
-and LÃª Kháº¯c, PhÃºc and Melas, Luke and Ghosh, Ritobrata}, doi = {10.5281/
-zenodo.5146400}, license = {Apache-2.0}, month = {jul}, title = {{DALLÂ·E
-Mini}}, url = {https://github.com/borisdayma/dalle-mini}, version = {v0.1-
-alpha}, year = {2021}} ``` ```bibtex @inproceedings{anonymous2022normformer,
-title = {NormFormer: Improved Transformer Pretraining with Extra
-Normalization}, author = {Anonymous}, booktitle = {Submitted to The Tenth
-International Conference on Learning Representations }, year = {2022}, url =
-{https://openreview.net/forum?id=GMYWzWztDx5}, note = {under review} } ```
-```bibtex @misc{ding2021erniedoc, title = {ERNIE-Doc: A Retrospective Long-
-Document Modeling Transformer}, author = {Siyu Ding and Junyuan Shang and
-Shuohuan Wang and Yu Sun and Hao Tian and Hua Wu and Haifeng Wang}, year =
-{2021}, eprint = {2012.15688}, archivePrefix = {arXiv}, primaryClass = {cs.CL}
-} ```
+``` ## Todo - [ ] get rotary embeddings working properly with xl memories - [ ]
+test on long context genomics, do bidirectional RMT on reverse complement and
+concat - [x] add xl memories, detached - [x] offer a way to turn off rotary
+embeddings, absolute positional embeddings, and add token shift - [x] make
+memories being causally masked an option - [x] add the memory replay backprop
+technique from memformer paper - [x] relative positional encoding ##
+Alternatives - Block_Recurrent_Transformer - Memformer ## Citations ```bibtex
+@inproceedings{bulatov2022recurrent, title = {Recurrent Memory Transformer},
+author = {Aydar Bulatov and Yuri Kuratov and Mikhail Burtsev}, booktitle =
+{Advances in Neural Information Processing Systems}, editor = {Alice H. Oh and
+Alekh Agarwal and Danielle Belgrave and Kyunghyun Cho}, year = {2022}, url =
+{https://openreview.net/forum?id=Uynr3iPhksa} } ``` ```bibtex @misc
+{bulatov2023scaling, title = {Scaling Transformer to 1M tokens and beyond with
+RMT}, author = {Aydar Bulatov and Yuri Kuratov and Mikhail S. Burtsev}, year =
+{2023}, eprint = {2304.11062}, archivePrefix = {arXiv}, primaryClass = {cs.CL}
+} ``` ```bibtex @inproceedings{dao2022flashattention, title = {Flash
+{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-Awareness},
+author = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R
+{\'e}, Christopher}, booktitle = {Advances in Neural Information Processing
+Systems}, year = {2022} } ``` ```bibtex @misc{shazeer2020glu, title = {GLU
+Variants Improve Transformer}, author = {Noam Shazeer}, year = {2020}, url =
+{https://arxiv.org/abs/2002.05202} } ``` ```bibtex @misc{su2021roformer, title
+= {RoFormer: Enhanced Transformer with Rotary Position Embedding}, author =
+{Jianlin Su and Yu Lu and Shengfeng Pan and Bo Wen and Yunfeng Liu}, year =
+{2021}, eprint = {2104.09864}, archivePrefix = {arXiv}, primaryClass = {cs.CL}
+} ``` ```bibtex @inproceedings{Wu2020MemformerAM, title = {Memformer: A Memory-
+Augmented Transformer for Sequence Modeling}, author = {Qingyang Wu and
+Zhenzhong Lan and Kun Qian and Jing Gu and Alborz Geramifard and Zhou Yu},
+booktitle = {AACL/IJCNLP}, year = {2020} } ``` ```bibtex @software
+{peng_bo_2021_5196578, author = {PENG Bo}, title = {BlinkDL/RWKV-LM: 0.01},
+month = {aug}, year = {2021}, publisher = {Zenodo}, version = {0.01}, doi =
+{10.5281/zenodo.5196578}, url = {https://doi.org/10.5281/zenodo.5196578} } ```
+```bibtex @misc{ding2021cogview, title = {CogView: Mastering Text-to-Image
+Generation via Transformers}, author = {Ming Ding and Zhuoyi Yang and Wenyi
+Hong and Wendi Zheng and Chang Zhou and Da Yin and Junyang Lin and Xu Zou and
+Zhou Shao and Hongxia Yang and Jie Tang}, year = {2021}, eprint = {2105.13290},
+archivePrefix = {arXiv}, primaryClass = {cs.CV} } ``` ```bibtex @software
+{Dayma_DALLE_Mini_2021, author = {Dayma, Boris and Patil, Suraj and Cuenca,
+Pedro and Saifullah, Khalid and Abraham, Tanishq and LÃª Kháº¯c, PhÃºc and
+Melas, Luke and Ghosh, Ritobrata}, doi = {10.5281/zenodo.5146400}, license =
+{Apache-2.0}, month = {jul}, title = {{DALLÂ·E Mini}}, url = {https://
+github.com/borisdayma/dalle-mini}, version = {v0.1-alpha}, year = {2021}} ```
+```bibtex @inproceedings{anonymous2022normformer, title = {NormFormer: Improved
+Transformer Pretraining with Extra Normalization}, author = {Anonymous},
+booktitle = {Submitted to The Tenth International Conference on Learning
+Representations }, year = {2022}, url = {https://openreview.net/
+forum?id=GMYWzWztDx5}, note = {under review} } ``` ```bibtex @misc
+{ding2021erniedoc, title = {ERNIE-Doc: A Retrospective Long-Document Modeling
+Transformer}, author = {Siyu Ding and Junyuan Shang and Shuohuan Wang and Yu
+Sun and Hao Tian and Hua Wu and Haifeng Wang}, year = {2021}, eprint =
+{2012.15688}, archivePrefix = {arXiv}, primaryClass = {cs.CL} } ```
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.2/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.2.3/recurrent_memory_transformer_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.2.2/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.2.3/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,31 +400,33 @@
         return loss, write_memories, next_xl_memories
 
 # wrapper to manage many segments
 
 class RecurrentMemoryTransformerWrapper(nn.Module):
     def __init__(
         self,
-        transformer: RecurrentMemoryTransformer
+        transformer: RecurrentMemoryTransformer,
+        truncate_at_step = None  # number of steps before detaching memories (truncated bptt). with memory replay checkpointing, there should be no memory issues, but in case of instability, as reported in initial paper
     ):
         super().__init__()
         self.transformer = transformer
         self.seq_len = transformer.seq_len
+        self.truncate_at_step = truncate_at_step
 
     @torch.no_grad()
     @eval_decorator
     def generate(
         self,
         prime,
         *,
         length,
         memories = None,
         xl_memories: Optional[List[torch.Tensor]] = None,
         temperature = 1.,
-        filter_thres = 0.9,
+        filter_thres = 0.9
     ):
         assert self.transformer.causal, 'only autoregressive transformers can generate'
 
         start_len, seq_len = prime.shape[-1], self.seq_len
 
         assert length >= start_len
 
@@ -471,18 +473,19 @@
         x,
         memories = None,
         *,
         mask = None,
         xl_memories: Optional[List[torch.Tensor]] = None,
         return_loss = False,
         labels = None,
+        truncate_at_step = None,         # if set, this would override the truncate_at_step at init
         memory_replay_backprop = False,  # whether to have the class do the backwards pass memory efficiently
         mrbp_loss_weight = 1.            # if using memory replay backprop with gradient accumulation, scale loss by this factor ex. (1. / <num grad accum steps>)
     ):
-        seq_len = self.seq_len
+        seq_len, truncate_at_step = self.seq_len, default(truncate_at_step, self.truncate_at_step)
 
         labels = None
         if (return_loss or memory_replay_backprop) and not exists(labels):
             x, labels = x[:, :-1], x[:, 1:]
 
         # segment input
 
@@ -518,19 +521,22 @@
         forward_context = nullcontext if not memory_replay_backprop else torch.no_grad
 
         # forward and get all outputs (can be either loss or logits)
 
         logits = []
         losses = []
 
-        for segment, mask_segment, label_segment, loss_weight in zip_longest(segments, mask_segments, label_segments, segment_length_frac):
+        for step, (segment, mask_segment, label_segment, loss_weight) in enumerate(zip_longest(segments, mask_segments, label_segments, segment_length_frac)):
 
             with forward_context():
                 output, memories, xl_memories = self.transformer(segment, memories, mask = mask_segment, labels = label_segment)
 
+            if exists(truncate_at_step) and divisible_by(step + 1, truncate_at_step):
+                memories = memories.detach()
+
             replay_buffer.append(memories)
 
             xl_segments.append(xl_memories)
 
             if return_loss:
                 losses.append(output * loss_weight)
             else:
@@ -552,16 +558,16 @@
                 mask_segments,
                 label_segments,
                 segment_length_frac,
             ]))
 
             total_loss = 0.
 
-            for i, segment, segment_memories, segment_xl_memories, mask_segment, label_segment, loss_weight in reversed_inputs:
-                is_first = i == 0
+            for step, segment, segment_memories, segment_xl_memories, mask_segment, label_segment, loss_weight in reversed_inputs:
+                is_first = step == 0
 
                 if exists(segment_memories):
                     segment_memories.requires_grad_()
 
                 loss, next_segment_memories, _ = self.transformer(segment, segment_memories, mask = mask_segment, xl_memories = segment_xl_memories, labels = label_segment)
 
                 weighted_loss = loss * loss_weight * mrbp_loss_weight
@@ -571,15 +577,18 @@
                 next_segment_memories.backward(memories_grad)
 
                 total_loss += weighted_loss
 
                 if is_first:
                     continue
 
-                memories_grad.copy_(segment_memories.grad.data)
+                if exists(truncate_at_step) and divisible_by(step + 1, truncate_at_step):
+                    memories_grad.zero_()
+                else:
+                    memories_grad.copy_(segment_memories.grad.data)
 
             return total_loss
 
         # return logits if needed
 
         if not return_loss:
             logits = torch.cat(logits, dim = -2)
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.2/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.2.3/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.2.2
+Version: 0.2.3
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.2/setup.py` & `recurrent-memory-transformer-pytorch-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.2',
+  version = '0.2.3',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

