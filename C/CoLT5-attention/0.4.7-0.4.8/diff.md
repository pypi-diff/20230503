# Comparing `tmp/CoLT5-attention-0.4.7.tar.gz` & `tmp/CoLT5-attention-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.4.7.tar", last modified: Wed May  3 15:09:56 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.4.8.tar", last modified: Wed May  3 16:32:22 2023, max compression
```

## Comparing `CoLT5-attention-0.4.7.tar` & `CoLT5-attention-0.4.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:09:56.151166 CoLT5-attention-0.4.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:09:56.151166 CoLT5-attention-0.4.7/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 15:09:56.000000 CoLT5-attention-0.4.7/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 15:09:56.000000 CoLT5-attention-0.4.7/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:09:56.000000 CoLT5-attention-0.4.7/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 15:09:56.000000 CoLT5-attention-0.4.7/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 15:09:56.000000 CoLT5-attention-0.4.7/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 15:09:56.151166 CoLT5-attention-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:09:56.151166 CoLT5-attention-0.4.7/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    34147 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:09:56.151166 CoLT5-attention-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:32:22.899337 CoLT5-attention-0.4.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:32:22.899337 CoLT5-attention-0.4.8/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 16:32:22.000000 CoLT5-attention-0.4.8/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 16:32:22.000000 CoLT5-attention-0.4.8/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:32:22.000000 CoLT5-attention-0.4.8/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 16:32:22.000000 CoLT5-attention-0.4.8/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 16:32:22.000000 CoLT5-attention-0.4.8/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 16:32:22.899337 CoLT5-attention-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:32:22.899337 CoLT5-attention-0.4.8/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/colt5_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34285 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:32:22.899337 CoLT5-attention-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-03 16:32:09.000000 CoLT5-attention-0.4.8/setup.py
```

### Comparing `CoLT5-attention-0.4.7/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.4.8/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.7
+Version: 0.4.8
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.7/LICENSE` & `CoLT5-attention-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.7/PKG-INFO` & `CoLT5-attention-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.7
+Version: 0.4.8
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.7/README.md` & `CoLT5-attention-0.4.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -157,7 +157,16 @@
 @article{Tillet2019TritonAI,
     title   = {Triton: an intermediate language and compiler for tiled neural network computations},
     author  = {Philippe Tillet and H. Kung and D. Cox},
     journal = {Proceedings of the 3rd ACM SIGPLAN International Workshop on Machine Learning and Programming Languages},
     year    = {2019}
 }
 ```
+
+```bibtex
+@inproceedings{dao2022flashattention,
+    title     = {Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-Awareness},
+    author    = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+    booktitle = {Advances in Neural Information Processing Systems},
+    year      = {2022}
+}
+```
```

#### html2text {}

```diff
@@ -76,8 +76,13 @@
 Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
 Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
 Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
 Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` ```bibtex @article
 {Tillet2019TritonAI, title = {Triton: an intermediate language and compiler for
 tiled neural network computations}, author = {Philippe Tillet and H. Kung and
 D. Cox}, journal = {Proceedings of the 3rd ACM SIGPLAN International Workshop
-on Machine Learning and Programming Languages}, year = {2019} } ```
+on Machine Learning and Programming Languages}, year = {2019} } ``` ```bibtex
+@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
+Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
+Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
+} ```
```

### Comparing `CoLT5-attention-0.4.7/colt5_attention/coor_descent.py` & `CoLT5-attention-0.4.8/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.7/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.4.8/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.7/colt5_attention/transformer_block.py` & `CoLT5-attention-0.4.8/colt5_attention/transformer_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
 from local_attention import LocalMHA
 from einops import rearrange, repeat, pack, unpack
 
+from colt5_attention.attend import Attend
+
 # helper functions
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
@@ -73,26 +75,29 @@
 
 class Attention(nn.Module):
     def __init__(
         self,
         dim,
         dim_head = 64,
         heads = 8,
-        multiply_keys_by_score = False
+        multiply_keys_by_score = False,
+        use_flash = False
     ):
         super().__init__()
         self.heads = heads
         self.scale = dim_head ** -0.5
         dim_hidden = dim_head * heads
 
         self.multiply_keys_by_score = multiply_keys_by_score
 
         self.norm = RMSNorm(dim)
         self.null_kv = nn.Parameter(torch.randn(2, heads, dim_head))
 
+        self.attend = Attend(use_flash = use_flash)
+
         self.to_q = nn.Linear(dim, dim_hidden, bias = False)
         self.to_kv = nn.Linear(dim, dim_hidden * 2, bias = False)
         self.to_out = nn.Linear(dim_hidden, dim, bias = False)
 
     def forward(
         self,
         x,
@@ -163,38 +168,27 @@
         # null key values
 
         nk, nv = map(lambda t: repeat(t, 'h d -> b h 1 d', b = batch), self.null_kv)
 
         k = torch.cat((nk, k), dim = -2)
         v = torch.cat((nv, v), dim = -2)
 
-        # scale and get similarity
-
-        q = q * self.scale
-        sim = einsum('b h i d, b h j d -> b h i j', q, k)
-
         # masking
 
         if exists(mask):
             if mask.ndim == 3:
                 mask = repeat(mask, 'b r j -> b (r h) 1 j', h = heads_per_route)
             else:
                 mask = rearrange(mask, 'b j -> b 1 1 j')
 
             mask = F.pad(mask, (1, 0), value = True)
 
-            sim = sim.masked_fill(~mask, -torch.finfo(sim.dtype).max)
-
         # attention
 
-        attn = sim.softmax(dim = -1)
-
-        # aggregate
-
-        out = einsum('b h i j, b h j d -> b h i d', attn, v)
+        out = self.attend(q, k, v)
 
         # merge heads
 
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
 # routing related logic
@@ -554,15 +548,16 @@
         heavy_heads = 8,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
         router_type = 'coor_descent',
         router_kwargs: dict = {},
         multiply_keys_by_score = False,
         multiply_queries_by_score = False,
         use_triton = False,
-        use_null_q_tokens = True
+        use_null_q_tokens = True,
+        use_flash_attn = False
     ):
         super().__init__()
         assert router_type in ROUTERS.keys()
 
         self.router_type = router_type
 
         router_klass = ROUTERS.get(router_type)
@@ -604,15 +599,16 @@
             **router_kwargs
         )
 
         self.heavy_attn = Attention(
             dim = dim,
             dim_head = heavy_dim_head,
             heads = heavy_heads,
-            multiply_keys_by_score = multiply_keys_by_score
+            multiply_keys_by_score = multiply_keys_by_score,
+            use_flash = use_flash_attn
         )
 
     def forward(
         self,
         x,
         *,
         num_heavy_tokens_q = None,
@@ -691,15 +687,16 @@
         heavy_heads = 8,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
         router_type = 'coor_descent',
         router_kwargs: dict = {},
         multiply_keys_by_score = False,
         multiply_queries_by_score = False,
         use_triton = False,
-        use_null_q_tokens = True
+        use_null_q_tokens = True,
+        use_flash_attn = False
     ):
         super().__init__()
         assert router_type in ROUTERS.keys()
 
         self.router_type = router_type
 
         router_klass = ROUTERS.get(router_type)
@@ -741,15 +738,16 @@
             **router_kwargs
         )
 
         self.heavy_attn = Attention(
             dim = dim,
             dim_head = heavy_dim_head,
             heads = heavy_heads,
-            multiply_keys_by_score = multiply_keys_by_score
+            multiply_keys_by_score = multiply_keys_by_score,
+            use_flash = use_flash_attn
         )
 
     def forward(
         self,
         x,
         *,
         num_heavy_tokens_q = None,
@@ -873,15 +871,16 @@
         heads = 8,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
         router_type = 'coor_descent',
         router_kwargs: dict = {},
         kv_routing_tokens = 1,
         multiply_keys_by_score = False,
         use_triton = False,
-        use_null_q_tokens = True
+        use_null_q_tokens = True,
+        use_flash_attn = False
     ):
         super().__init__()
         assert router_type in ROUTERS.keys()
 
         self.router_type = router_type
 
         router_klass = ROUTERS.get(router_type)
@@ -909,15 +908,16 @@
             **router_kwargs
         )
 
         self.heavy_attn = Attention(
             dim = dim,
             dim_head = dim_head,
             heads = heads,
-            multiply_keys_by_score = multiply_keys_by_score
+            multiply_keys_by_score = multiply_keys_by_score,
+            use_flash = use_flash_attn
         )
 
     def forward(
         self,
         x,
         context,
         *,
@@ -1010,15 +1010,16 @@
         heavy_ff_mult = 4,
         router_straight_through = True,
         router_type = 'coor_descent',
         router_kwargs: dict = {},
         multiply_keys_by_score = False,
         multiply_queries_by_score = False,
         use_triton = False,
-        use_null_q_tokens = True
+        use_null_q_tokens = True,
+        use_flash_attn = False
     ):
         super().__init__()
         self.conditional_ff = ConditionalRoutedFeedForward(
             dim,
             num_heavy_tokens = num_heavy_ff_tokens,
             light_ff_mult = light_ff_mult,
             heavy_ff_mult = heavy_ff_mult,
@@ -1040,15 +1041,16 @@
             num_routed_kv = num_routed_kv,
             router_straight_through = router_straight_through,
             router_type = router_type,
             router_kwargs = router_kwargs,
             multiply_keys_by_score = multiply_keys_by_score,
             multiply_queries_by_score = multiply_queries_by_score,
             use_triton = use_triton,
-            use_null_q_tokens = use_null_q_tokens
+            use_null_q_tokens = use_null_q_tokens,
+            use_flash_attn = use_flash_attn
         )
 
     def forward(
         self,
         x,
         mask = None,
         num_heavy_attn_tokens_q = None,
```

### Comparing `CoLT5-attention-0.4.7/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.4.8/colt5_attention/triton_coor_descent.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,16 +237,15 @@
 
             dsa = db * tl.where(sa >= 0, -1., 0.)
             ds += dsa
 
             da = tl.sum(dsa, axis = 0) + last_da
             da *= -eps
 
-            dsb = da * softmax
-            dsb *= inv_eps
+            dsb = da * softmax * inv_eps
 
             ds += dsb
             db = dsb
 
             last_da = 0.
 
     ds += -db
```

### Comparing `CoLT5-attention-0.4.7/setup.py` & `CoLT5-attention-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.4.7',
+  version = '0.4.8',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

