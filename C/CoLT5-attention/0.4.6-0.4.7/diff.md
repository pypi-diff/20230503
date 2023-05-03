# Comparing `tmp/CoLT5-attention-0.4.6.tar.gz` & `tmp/CoLT5-attention-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.4.6.tar", last modified: Wed May  3 01:58:13 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.4.7.tar", last modified: Wed May  3 15:09:56 2023, max compression
```

## Comparing `CoLT5-attention-0.4.6.tar` & `CoLT5-attention-0.4.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:58:13.161205 CoLT5-attention-0.4.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:58:13.161205 CoLT5-attention-0.4.6/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 01:58:13.000000 CoLT5-attention-0.4.6/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 01:58:13.000000 CoLT5-attention-0.4.6/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 01:58:13.000000 CoLT5-attention-0.4.6/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 01:58:13.000000 CoLT5-attention-0.4.6/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 01:58:13.000000 CoLT5-attention-0.4.6/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 01:58:13.161205 CoLT5-attention-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:58:13.161205 CoLT5-attention-0.4.6/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    33640 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 01:58:13.161205 CoLT5-attention-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:09:56.151166 CoLT5-attention-0.4.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:09:56.151166 CoLT5-attention-0.4.7/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 15:09:56.000000 CoLT5-attention-0.4.7/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 15:09:56.000000 CoLT5-attention-0.4.7/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:09:56.000000 CoLT5-attention-0.4.7/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 15:09:56.000000 CoLT5-attention-0.4.7/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 15:09:56.000000 CoLT5-attention-0.4.7/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 15:09:56.151166 CoLT5-attention-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:09:56.151166 CoLT5-attention-0.4.7/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34147 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:09:56.151166 CoLT5-attention-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-03 15:09:44.000000 CoLT5-attention-0.4.7/setup.py
```

### Comparing `CoLT5-attention-0.4.6/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.4.7/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.6
+Version: 0.4.7
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.6/LICENSE` & `CoLT5-attention-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.6/PKG-INFO` & `CoLT5-attention-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.6
+Version: 0.4.7
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.6/README.md` & `CoLT5-attention-0.4.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -134,17 +134,18 @@
 - [ ] make flash attention compatible
 - [ ] fused coordinate descent kernel using triton
     - [x] forwards        
     - [x] backwards
     - [x] add some tests and benchmark for triton vs plain pytorch coor_descent - 10x faster for forward, 4x faster for backwards and memory saved is n_iters times
     - [x] fall back on plain coordinate descent for cpu
     - [x] handle edge case for when a row is completely masked out for triton, or simply enforce it never to be so
+    - [x] fix masking in coordinate descent
     - [ ] allow for saving intermediates every number of iterations - trading memory for recompute efficiency during backwards
-    - [ ] maximum block size in triton allowed is 131k, make sure at least quarter of million sequence length can be reached
-    - [ ] issue with intermittent gradient errors is because of masking - load the key padding mask into triton and mask out during each iteration
+    - [ ] issue with intermittent gradient errors occurs only during masking
+    - [ ] maximum block size in triton allowed is 131k, make sure at least quarter of million sequence length can be reached. to get around this initially, one can fold a million token sequence into ~9 131k and uniformly route. offer uniform routing scheme within router itself
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -61,22 +61,23 @@
 attention scenario, support for routing token that first queries the source
 tokens, before retrieving from memories - [ ] make flash attention compatible -
 [ ] fused coordinate descent kernel using triton - [x] forwards - [x] backwards
 - [x] add some tests and benchmark for triton vs plain pytorch coor_descent -
 10x faster for forward, 4x faster for backwards and memory saved is n_iters
 times - [x] fall back on plain coordinate descent for cpu - [x] handle edge
 case for when a row is completely masked out for triton, or simply enforce it
-never to be so - [ ] allow for saving intermediates every number of iterations
-- trading memory for recompute efficiency during backwards - [ ] maximum block
-size in triton allowed is 131k, make sure at least quarter of million sequence
-length can be reached - [ ] issue with intermittent gradient errors is because
-of masking - load the key padding mask into triton and mask out during each
-iteration ## Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL, title =
-{CoLT5: Faster Long-Range Transformers with Conditional Computation}, author =
-{Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and
-Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James
-Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ```
-```bibtex @article{Tillet2019TritonAI, title = {Triton: an intermediate
-language and compiler for tiled neural network computations}, author =
-{Philippe Tillet and H. Kung and D. Cox}, journal = {Proceedings of the 3rd ACM
-SIGPLAN International Workshop on Machine Learning and Programming Languages},
-year = {2019} } ```
+never to be so - [x] fix masking in coordinate descent - [ ] allow for saving
+intermediates every number of iterations - trading memory for recompute
+efficiency during backwards - [ ] issue with intermittent gradient errors
+occurs only during masking - [ ] maximum block size in triton allowed is 131k,
+make sure at least quarter of million sequence length can be reached. to get
+around this initially, one can fold a million token sequence into ~9 131k and
+uniformly route. offer uniform routing scheme within router itself ## Citations
+```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
+Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
+Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
+Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
+Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` ```bibtex @article
+{Tillet2019TritonAI, title = {Triton: an intermediate language and compiler for
+tiled neural network computations}, author = {Philippe Tillet and H. Kung and
+D. Cox}, journal = {Proceedings of the 3rd ACM SIGPLAN International Workshop
+on Machine Learning and Programming Languages}, year = {2019} } ```
```

### Comparing `CoLT5-attention-0.4.6/colt5_attention/coor_descent.py` & `CoLT5-attention-0.4.7/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.6/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.4.7/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.6/colt5_attention/transformer_block.py` & `CoLT5-attention-0.4.7/colt5_attention/transformer_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,15 +553,16 @@
         heavy_dim_head = 64,
         heavy_heads = 8,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
         router_type = 'coor_descent',
         router_kwargs: dict = {},
         multiply_keys_by_score = False,
         multiply_queries_by_score = False,
-        use_triton = False
+        use_triton = False,
+        use_null_q_tokens = True
     ):
         super().__init__()
         assert router_type in ROUTERS.keys()
 
         self.router_type = router_type
 
         router_klass = ROUTERS.get(router_type)
@@ -582,14 +583,18 @@
             prenorm = True,
             causal = False,
             use_rotary_pos_emb = False,
             look_backward = 1,
             look_forward = 1
         )
 
+        self.null_q_token = None
+        if use_null_q_tokens:
+            self.null_q_token = nn.Parameter(torch.randn(dim)) # for the query tokens not selected by the router, give it a learned output embed
+
         self.q_router = router_klass(
             dim = dim,
             straight_through = router_straight_through,
             **router_kwargs
         )
 
         self.kv_router = router_klass(
@@ -652,15 +657,20 @@
             normalized_scores_q = normalized_scores_q if self.multiply_queries_by_score else None
         )
 
         routed_tokens_out = routed_tokens_out * rearrange(normalized_scores_q, '... -> ... 1')
 
         # scatter back the output of the heavy branch
 
-        heavy_out = torch.zeros_like(x)
+        if exists(self.null_q_token):
+            heavy_out = rearrange(self.null_q_token, 'd -> 1 1 d')
+            heavy_out = heavy_out.expand_as(x).clone()
+        else:
+            heavy_out = torch.zeros_like(x)
+
         heavy_out = self.q_router.route_back(heavy_out, routed_tokens_out, indices_q)
 
         # sum light and heavy branches
 
         return light_out + heavy_out
 
 # improvised conditionally routed autoregressive attention
@@ -999,15 +1009,16 @@
         light_ff_mult = 0.5,
         heavy_ff_mult = 4,
         router_straight_through = True,
         router_type = 'coor_descent',
         router_kwargs: dict = {},
         multiply_keys_by_score = False,
         multiply_queries_by_score = False,
-        use_triton = False
+        use_triton = False,
+        use_null_q_tokens = True
     ):
         super().__init__()
         self.conditional_ff = ConditionalRoutedFeedForward(
             dim,
             num_heavy_tokens = num_heavy_ff_tokens,
             light_ff_mult = light_ff_mult,
             heavy_ff_mult = heavy_ff_mult,
@@ -1028,15 +1039,16 @@
             num_heavy_tokens_kv = num_heavy_attn_tokens_kv,
             num_routed_kv = num_routed_kv,
             router_straight_through = router_straight_through,
             router_type = router_type,
             router_kwargs = router_kwargs,
             multiply_keys_by_score = multiply_keys_by_score,
             multiply_queries_by_score = multiply_queries_by_score,
-            use_triton = use_triton
+            use_triton = use_triton,
+            use_null_q_tokens = use_null_q_tokens
         )
 
     def forward(
         self,
         x,
         mask = None,
         num_heavy_attn_tokens_q = None,
```

### Comparing `CoLT5-attention-0.4.6/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.4.7/colt5_attention/triton_coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.6/setup.py` & `CoLT5-attention-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.4.6',
+  version = '0.4.7',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

