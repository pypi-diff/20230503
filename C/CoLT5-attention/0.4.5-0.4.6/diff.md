# Comparing `tmp/CoLT5-attention-0.4.5.tar.gz` & `tmp/CoLT5-attention-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.4.5.tar", last modified: Wed May  3 00:57:07 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.4.6.tar", last modified: Wed May  3 01:58:13 2023, max compression
```

## Comparing `CoLT5-attention-0.4.5.tar` & `CoLT5-attention-0.4.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:57:07.737730 CoLT5-attention-0.4.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:57:07.737730 CoLT5-attention-0.4.5/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 00:57:07.000000 CoLT5-attention-0.4.5/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 00:57:07.000000 CoLT5-attention-0.4.5/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:57:07.000000 CoLT5-attention-0.4.5/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 00:57:07.000000 CoLT5-attention-0.4.5/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 00:57:07.000000 CoLT5-attention-0.4.5/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 00:56:53.000000 CoLT5-attention-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 00:57:07.737730 CoLT5-attention-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-03 00:56:53.000000 CoLT5-attention-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:57:07.737730 CoLT5-attention-0.4.5/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 00:56:53.000000 CoLT5-attention-0.4.5/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-03 00:56:53.000000 CoLT5-attention-0.4.5/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-03 00:56:53.000000 CoLT5-attention-0.4.5/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    33238 2023-05-03 00:56:53.000000 CoLT5-attention-0.4.5/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-03 00:56:53.000000 CoLT5-attention-0.4.5/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 00:57:07.737730 CoLT5-attention-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-03 00:56:53.000000 CoLT5-attention-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:58:13.161205 CoLT5-attention-0.4.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:58:13.161205 CoLT5-attention-0.4.6/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 01:58:13.000000 CoLT5-attention-0.4.6/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 01:58:13.000000 CoLT5-attention-0.4.6/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 01:58:13.000000 CoLT5-attention-0.4.6/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 01:58:13.000000 CoLT5-attention-0.4.6/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 01:58:13.000000 CoLT5-attention-0.4.6/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 01:58:13.161205 CoLT5-attention-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:58:13.161205 CoLT5-attention-0.4.6/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33640 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 01:58:13.161205 CoLT5-attention-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-03 01:58:01.000000 CoLT5-attention-0.4.6/setup.py
```

### Comparing `CoLT5-attention-0.4.5/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.4.6/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.5
+Version: 0.4.6
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.5/LICENSE` & `CoLT5-attention-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.5/PKG-INFO` & `CoLT5-attention-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.5
+Version: 0.4.6
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.5/README.md` & `CoLT5-attention-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.5/colt5_attention/coor_descent.py` & `CoLT5-attention-0.4.6/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.5/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.4.6/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.5/colt5_attention/transformer_block.py` & `CoLT5-attention-0.4.6/colt5_attention/transformer_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -681,15 +681,15 @@
         heavy_heads = 8,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
         router_type = 'coor_descent',
         router_kwargs: dict = {},
         multiply_keys_by_score = False,
         multiply_queries_by_score = False,
         use_triton = False,
-        use_null_q_tokens = False
+        use_null_q_tokens = True
     ):
         super().__init__()
         assert router_type in ROUTERS.keys()
 
         self.router_type = router_type
 
         router_klass = ROUTERS.get(router_type)
@@ -862,29 +862,34 @@
         dim_head = 64,
         heads = 8,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
         router_type = 'coor_descent',
         router_kwargs: dict = {},
         kv_routing_tokens = 1,
         multiply_keys_by_score = False,
-        use_triton = False
+        use_triton = False,
+        use_null_q_tokens = True
     ):
         super().__init__()
         assert router_type in ROUTERS.keys()
 
         self.router_type = router_type
 
         router_klass = ROUTERS.get(router_type)
 
         if router_type == 'coor_descent' and use_triton:
             router_kwargs = {**router_kwargs, 'use_triton': True}
 
         self.num_tokens_q = num_tokens_q
         self.num_tokens_kv = num_tokens_kv
 
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
@@ -961,15 +966,19 @@
         # early return if queries did not undergo routing
 
         if not should_route_queries:
             return routed_tokens_out
 
         # otherwise, scatter back the query outputs
 
-        out = torch.zeros_like(x)
+        if exists(self.null_q_token):
+            out = rearrange(self.null_q_token, 'd -> 1 1 d')
+            out = out.expand_as(x).clone()
+        else:
+            out = torch.zeros_like(x)
 
         out = self.q_router.route_back(out, routed_tokens_out, indices_q)
 
         return out
 
 # block
```

### Comparing `CoLT5-attention-0.4.5/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.4.6/colt5_attention/triton_coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.5/setup.py` & `CoLT5-attention-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.4.5',
+  version = '0.4.6',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

