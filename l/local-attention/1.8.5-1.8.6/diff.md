# Comparing `tmp/local-attention-1.8.5.tar.gz` & `tmp/local-attention-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-attention-1.8.5.tar", last modified: Wed Mar 22 19:09:07 2023, max compression
+gzip compressed data, was "local-attention-1.8.6.tar", last modified: Wed May  3 16:45:10 2023, max compression
```

## Comparing `local-attention-1.8.5.tar` & `local-attention-1.8.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:09:07.372283 local-attention-1.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-22 19:08:56.000000 local-attention-1.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-22 19:09:07.372283 local-attention-1.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-03-22 19:08:56.000000 local-attention-1.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:09:07.372283 local-attention-1.8.5/local_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-22 19:08:57.000000 local-attention-1.8.5/local_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-03-22 19:08:57.000000 local-attention-1.8.5/local_attention/local_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-22 19:08:57.000000 local-attention-1.8.5/local_attention/rotary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-03-22 19:08:57.000000 local-attention-1.8.5/local_attention/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 19:09:07.372283 local-attention-1.8.5/local_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-22 19:09:07.000000 local-attention-1.8.5/local_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-22 19:09:07.000000 local-attention-1.8.5/local_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 19:09:07.000000 local-attention-1.8.5/local_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-22 19:09:07.000000 local-attention-1.8.5/local_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-22 19:09:07.000000 local-attention-1.8.5/local_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 19:09:07.372283 local-attention-1.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-22 19:08:57.000000 local-attention-1.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:45:10.945933 local-attention-1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 16:45:01.000000 local-attention-1.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-03 16:45:10.945933 local-attention-1.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-03 16:45:01.000000 local-attention-1.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:45:10.941933 local-attention-1.8.6/local_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 16:45:01.000000 local-attention-1.8.6/local_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-05-03 16:45:01.000000 local-attention-1.8.6/local_attention/local_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-03 16:45:01.000000 local-attention-1.8.6/local_attention/rotary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-03 16:45:01.000000 local-attention-1.8.6/local_attention/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:45:10.941933 local-attention-1.8.6/local_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-03 16:45:10.000000 local-attention-1.8.6/local_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-03 16:45:10.000000 local-attention-1.8.6/local_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:45:10.000000 local-attention-1.8.6/local_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 16:45:10.000000 local-attention-1.8.6/local_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 16:45:10.000000 local-attention-1.8.6/local_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:45:10.945933 local-attention-1.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-03 16:45:01.000000 local-attention-1.8.6/setup.py
```

### Comparing `local-attention-1.8.5/LICENSE` & `local-attention-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `local-attention-1.8.5/PKG-INFO` & `local-attention-1.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local-attention
-Version: 1.8.5
+Version: 1.8.6
 Summary: Local attention, window with lookback, for language modeling
 Home-page: https://github.com/lucidrains/local-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: transformers,attention,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `local-attention-1.8.5/README.md` & `local-attention-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `local-attention-1.8.5/local_attention/local_attention.py` & `local-attention-1.8.6/local_attention/local_attention.py`

 * *Files identical despite different names*

### Comparing `local-attention-1.8.5/local_attention/rotary.py` & `local-attention-1.8.6/local_attention/rotary.py`

 * *Files identical despite different names*

### Comparing `local-attention-1.8.5/local_attention/transformer.py` & `local-attention-1.8.6/local_attention/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from local_attention.local_attention import LocalAttention
 
 # helper function
 
 def exists(val):
     return val is not None
 
+def default(val, d):
+    return val if exists(val) else d
+
 def l2norm(t):
     return F.normalize(t, dim = -1)
 
 def eval_decorator(fn):
     def inner(model, *args, **kwargs):
         was_training = model.training
         model.eval()
@@ -45,14 +48,15 @@
         dropout = 0.,
         causal = False,
         prenorm = False,
         qk_rmsnorm = False,
         qk_scale = 8,
         use_xpos = False,
         xpos_scale_base = None,
+        exact_windowsize = None,
         **kwargs
     ):
         super().__init__()        
         inner_dim = dim_head * heads
 
         self.norm = nn.LayerNorm(dim) if prenorm else None
 
@@ -67,15 +71,15 @@
 
         self.attn_fn = LocalAttention(
             dim = dim_head,
             window_size = window_size,
             causal = causal,
             autopad = True,
             scale = (qk_scale if qk_rmsnorm else None),
-            exact_windowsize = True,
+            exact_windowsize = default(exact_windowsize, True),
             use_xpos = use_xpos,
             xpos_scale_base = xpos_scale_base,
             **kwargs
         )
 
         self.to_out = nn.Linear(inner_dim, dim, bias = False)
```

### Comparing `local-attention-1.8.5/local_attention.egg-info/PKG-INFO` & `local-attention-1.8.6/local_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local-attention
-Version: 1.8.5
+Version: 1.8.6
 Summary: Local attention, window with lookback, for language modeling
 Home-page: https://github.com/lucidrains/local-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: transformers,attention,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `local-attention-1.8.5/setup.py` & `local-attention-1.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'local-attention',
   packages = find_packages(),
-  version = '1.8.5',
+  version = '1.8.6',
   license='MIT',
   description = 'Local attention, window with lookback, for language modeling',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/local-attention',
   keywords = [
```

