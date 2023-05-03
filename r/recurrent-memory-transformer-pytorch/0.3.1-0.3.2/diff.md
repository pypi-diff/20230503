# Comparing `tmp/recurrent-memory-transformer-pytorch-0.3.1.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.3.1.tar", last modified: Wed May  3 20:06:01 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.3.2.tar", last modified: Wed May  3 20:09:10 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.3.1.tar` & `recurrent-memory-transformer-pytorch-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:06:01.930699 recurrent-memory-transformer-pytorch-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 20:05:51.000000 recurrent-memory-transformer-pytorch-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 20:06:01.930699 recurrent-memory-transformer-pytorch-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-05-03 20:05:51.000000 recurrent-memory-transformer-pytorch-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:06:01.926699 recurrent-memory-transformer-pytorch-0.3.1/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 20:05:51.000000 recurrent-memory-transformer-pytorch-0.3.1/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-03 20:05:51.000000 recurrent-memory-transformer-pytorch-0.3.1/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    19165 2023-05-03 20:05:51.000000 recurrent-memory-transformer-pytorch-0.3.1/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:06:01.930699 recurrent-memory-transformer-pytorch-0.3.1/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 20:06:01.000000 recurrent-memory-transformer-pytorch-0.3.1/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-03 20:06:01.000000 recurrent-memory-transformer-pytorch-0.3.1/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:06:01.000000 recurrent-memory-transformer-pytorch-0.3.1/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 20:06:01.000000 recurrent-memory-transformer-pytorch-0.3.1/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 20:06:01.000000 recurrent-memory-transformer-pytorch-0.3.1/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:06:01.930699 recurrent-memory-transformer-pytorch-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-03 20:05:51.000000 recurrent-memory-transformer-pytorch-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:09:10.516166 recurrent-memory-transformer-pytorch-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 20:08:57.000000 recurrent-memory-transformer-pytorch-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 20:09:10.516166 recurrent-memory-transformer-pytorch-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-05-03 20:08:57.000000 recurrent-memory-transformer-pytorch-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:09:10.512166 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 20:08:57.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-03 20:08:57.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-05-03 20:08:57.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:09:10.516166 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 20:09:10.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-03 20:09:10.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:09:10.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 20:09:10.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 20:09:10.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:09:10.516166 recurrent-memory-transformer-pytorch-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-03 20:08:57.000000 recurrent-memory-transformer-pytorch-0.3.2/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.3.1/LICENSE` & `recurrent-memory-transformer-pytorch-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.3.1/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.3.1
+Version: 0.3.2
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.3.1/README.md` & `recurrent-memory-transformer-pytorch-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.3.1/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.3.1/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
         self.maybe_token_shift = token_shift_fn if token_shift else identity
 
         # memory related
 
         self.num_memory_tokens = num_memory_tokens
 
-        self.read_memory_emb = nn.Parameter(torch.zeros(dim))
+        self.read_memory_emb = nn.Parameter(torch.zeros(num_memory_tokens, dim))
         nn.init.normal_(self.read_memory_emb, std = 0.02)
 
         self.memory_tokens = nn.Parameter(torch.randn(num_memory_tokens, dim))
         nn.init.normal_(self.memory_tokens, std = 0.02)
 
         self.write_memories_norm = RMSNorm(dim) if norm_write_memories else None
```

### Comparing `recurrent-memory-transformer-pytorch-0.3.1/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.3.1
+Version: 0.3.2
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.3.1/setup.py` & `recurrent-memory-transformer-pytorch-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.1',
+  version = '0.3.2',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

