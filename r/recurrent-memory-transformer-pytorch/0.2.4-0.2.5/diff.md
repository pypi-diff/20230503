# Comparing `tmp/recurrent-memory-transformer-pytorch-0.2.4.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.2.4.tar", last modified: Wed May  3 15:57:01 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.2.5.tar", last modified: Wed May  3 17:15:48 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.2.4.tar` & `recurrent-memory-transformer-pytorch-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:57:01.078559 recurrent-memory-transformer-pytorch-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 15:56:47.000000 recurrent-memory-transformer-pytorch-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 15:57:01.078559 recurrent-memory-transformer-pytorch-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-03 15:56:47.000000 recurrent-memory-transformer-pytorch-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:57:01.074559 recurrent-memory-transformer-pytorch-0.2.4/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 15:56:47.000000 recurrent-memory-transformer-pytorch-0.2.4/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-03 15:56:47.000000 recurrent-memory-transformer-pytorch-0.2.4/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17944 2023-05-03 15:56:47.000000 recurrent-memory-transformer-pytorch-0.2.4/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:57:01.074559 recurrent-memory-transformer-pytorch-0.2.4/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 15:57:01.000000 recurrent-memory-transformer-pytorch-0.2.4/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-03 15:57:01.000000 recurrent-memory-transformer-pytorch-0.2.4/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:57:01.000000 recurrent-memory-transformer-pytorch-0.2.4/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 15:57:01.000000 recurrent-memory-transformer-pytorch-0.2.4/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 15:57:01.000000 recurrent-memory-transformer-pytorch-0.2.4/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:57:01.078559 recurrent-memory-transformer-pytorch-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-03 15:56:47.000000 recurrent-memory-transformer-pytorch-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:15:48.543178 recurrent-memory-transformer-pytorch-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 17:15:31.000000 recurrent-memory-transformer-pytorch-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 17:15:48.543178 recurrent-memory-transformer-pytorch-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-03 17:15:31.000000 recurrent-memory-transformer-pytorch-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:15:48.543178 recurrent-memory-transformer-pytorch-0.2.5/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 17:15:31.000000 recurrent-memory-transformer-pytorch-0.2.5/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-03 17:15:31.000000 recurrent-memory-transformer-pytorch-0.2.5/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18225 2023-05-03 17:15:31.000000 recurrent-memory-transformer-pytorch-0.2.5/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:15:48.543178 recurrent-memory-transformer-pytorch-0.2.5/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 17:15:48.000000 recurrent-memory-transformer-pytorch-0.2.5/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-03 17:15:48.000000 recurrent-memory-transformer-pytorch-0.2.5/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:15:48.000000 recurrent-memory-transformer-pytorch-0.2.5/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 17:15:48.000000 recurrent-memory-transformer-pytorch-0.2.5/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 17:15:48.000000 recurrent-memory-transformer-pytorch-0.2.5/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 17:15:48.543178 recurrent-memory-transformer-pytorch-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-03 17:15:31.000000 recurrent-memory-transformer-pytorch-0.2.5/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.4/LICENSE` & `recurrent-memory-transformer-pytorch-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.2.4/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.2.4
+Version: 0.2.5
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.4/README.md` & `recurrent-memory-transformer-pytorch-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.2.4/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.2.5/recurrent_memory_transformer_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.2.4/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.2.5/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,14 +208,15 @@
         rotary_pos_emb = False,
         token_shift = True,
         use_xl_memories = False,
         xl_mem_len = None,
         enhanced_xl_recurrence = False,     # add simple method for enhancing receptive field of xl memories, from ernie-doc paper
         emb_gradient_frac = 0.1,            # trick from cogview paper that leads to a bit more stability
         memory_not_causal = True,           # flash attention behaves a bit more optimally if causal mask is not explicitly passed in - but if the memories perform better without a causal mask, it is necessary to have this turned on
+        norm_write_memories = False,
     ):
         super().__init__()
         self.causal = causal
         self.seq_len = seq_len
 
         self.emb_gradient_frac = emb_gradient_frac
 
@@ -239,14 +240,16 @@
 
         self.read_memory_emb = nn.Parameter(torch.zeros(dim))
         nn.init.normal_(self.read_memory_emb, std = 0.02)
 
         self.memory_tokens = nn.Parameter(torch.randn(num_memory_tokens, dim))
         nn.init.normal_(self.memory_tokens, std = 0.02)
 
+        self.write_memories_norm = RMSNorm(dim) if norm_write_memories else None
+
         # xl memories
 
         xl_mem_len = default(xl_mem_len, seq_len)
         assert xl_mem_len <= seq_len
         self.xl_mem_len = xl_mem_len
 
         self.use_xl_memories = use_xl_memories
@@ -380,14 +383,19 @@
         if self.use_xl_memories:
             next_xl_memories = list(map(lambda t: torch.detach(t[..., -self.xl_mem_len:, :]), new_xl_memories))
 
         # split out memories using unpack
 
         read_memories, x, write_memories = unpack(x, ps, 'b * d')
 
+        # whether to norm the write memories
+
+        if exists(self.write_memories_norm):
+            write_memories = self.write_memories_norm(write_memories)
+
         # to logits
 
         logits = self.to_logits(x)
 
         if not return_loss:
             return logits, write_memories, next_xl_memories
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.4/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.2.5/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.2.4
+Version: 0.2.5
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.2.4/setup.py` & `recurrent-memory-transformer-pytorch-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.4',
+  version = '0.2.5',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

