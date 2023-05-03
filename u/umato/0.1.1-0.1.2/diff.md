# Comparing `tmp/umato-0.1.1.tar.gz` & `tmp/umato-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/umato-0.1.1.tar", last modified: Mon Apr  3 17:45:33 2023, max compression
+gzip compressed data, was "dist/umato-0.1.2.tar", last modified: Wed May  3 15:28:28 2023, max compression
```

## Comparing `umato-0.1.1.tar` & `umato-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-03 17:45:33.049845 umato-0.1.1/
--rw-rw-r--   0 hj        (1010) hj        (1010)    14989 2023-04-03 17:45:33.049845 umato-0.1.1/PKG-INFO
--rw-rw-r--   0 hj        (1010) hj        (1010)    12032 2023-04-03 14:53:45.000000 umato-0.1.1/README.md
--rw-rw-r--   0 hj        (1010) hj        (1010)       38 2023-04-03 17:45:33.049845 umato-0.1.1/setup.cfg
--rw-rw-r--   0 hj        (1010) hj        (1010)      830 2023-04-03 17:44:39.000000 umato-0.1.1/setup.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-03 17:45:33.049845 umato-0.1.1/src/
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-03 17:45:33.049845 umato-0.1.1/src/evaluation/
--rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-03 09:16:23.000000 umato-0.1.1/src/evaluation/__init__.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     3728 2023-04-03 09:16:23.000000 umato-0.1.1/src/evaluation/comparison.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1316 2023-04-03 09:16:23.000000 umato-0.1.1/src/evaluation/comparison_all.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     2172 2023-04-03 09:16:23.000000 umato-0.1.1/src/evaluation/comparison_local.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     2267 2023-04-03 09:16:23.000000 umato-0.1.1/src/evaluation/convert_to_csv.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     2081 2023-04-03 09:16:23.000000 umato-0.1.1/src/evaluation/convert_to_fvecs.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      907 2023-04-03 09:16:23.000000 umato-0.1.1/src/evaluation/convert_to_txt.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1539 2023-04-03 09:16:23.000000 umato-0.1.1/src/evaluation/save_subset.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1071 2023-04-03 09:16:23.000000 umato-0.1.1/src/evaluation/stability.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1607 2023-04-03 09:16:23.000000 umato-0.1.1/src/evaluation/stability_over.py
--rw-rw-r--   0 hj        (1010) hj        (1010)    14143 2023-04-03 09:16:23.000000 umato-0.1.1/src/evaluation/utils.py
--rw-rw-r--   0 hj        (1010) hj        (1010)      650 2023-04-03 09:16:23.000000 umato-0.1.1/src/evaluation/visualization.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-03 17:45:33.049845 umato-0.1.1/src/umato/
--rw-rw-r--   0 hj        (1010) hj        (1010)      298 2023-04-03 09:16:23.000000 umato-0.1.1/src/umato/__init__.py
--rw-rw-r--   0 hj        (1010) hj        (1010)    33397 2023-04-03 09:16:23.000000 umato-0.1.1/src/umato/distances.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     6180 2023-04-03 09:16:23.000000 umato-0.1.1/src/umato/layouts.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     8909 2023-04-03 09:16:23.000000 umato-0.1.1/src/umato/nndescent.py
--rw-rw-r--   0 hj        (1010) hj        (1010)    27473 2023-04-03 09:16:23.000000 umato-0.1.1/src/umato/rp_tree.py
--rw-rw-r--   0 hj        (1010) hj        (1010)    15587 2023-04-03 09:16:23.000000 umato-0.1.1/src/umato/sparse.py
--rw-rw-r--   0 hj        (1010) hj        (1010)    12330 2023-04-03 09:16:23.000000 umato-0.1.1/src/umato/sparse_nndescent.py
--rw-rw-r--   0 hj        (1010) hj        (1010)    20628 2023-04-03 09:16:23.000000 umato-0.1.1/src/umato/umap_.py
--rw-rw-r--   0 hj        (1010) hj        (1010)    30117 2023-04-03 17:42:57.000000 umato-0.1.1/src/umato/umato_.py
--rw-rw-r--   0 hj        (1010) hj        (1010)    32109 2023-04-03 09:16:23.000000 umato-0.1.1/src/umato/umato_pva.py
--rw-rw-r--   0 hj        (1010) hj        (1010)    20526 2023-04-03 09:16:23.000000 umato-0.1.1/src/umato/utils.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-03 17:45:33.049845 umato-0.1.1/src/umato.egg-info/
--rw-rw-r--   0 hj        (1010) hj        (1010)    14989 2023-04-03 17:45:32.000000 umato-0.1.1/src/umato.egg-info/PKG-INFO
--rw-rw-r--   0 hj        (1010) hj        (1010)      795 2023-04-03 17:45:32.000000 umato-0.1.1/src/umato.egg-info/SOURCES.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-04-03 17:45:32.000000 umato-0.1.1/src/umato.egg-info/dependency_links.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)       66 2023-04-03 17:45:32.000000 umato-0.1.1/src/umato.egg-info/requires.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)       17 2023-04-03 17:45:32.000000 umato-0.1.1/src/umato.egg-info/top_level.txt
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-03 15:28:28.180115 umato-0.1.2/
+-rw-rw-r--   0 hj        (1010) hj        (1010)    14987 2023-05-03 15:28:28.180115 umato-0.1.2/PKG-INFO
+-rw-rw-r--   0 hj        (1010) hj        (1010)    12030 2023-05-03 14:53:22.000000 umato-0.1.2/README.md
+-rw-rw-r--   0 hj        (1010) hj        (1010)       38 2023-05-03 15:28:28.180115 umato-0.1.2/setup.cfg
+-rw-rw-r--   0 hj        (1010) hj        (1010)      830 2023-05-03 15:28:23.000000 umato-0.1.2/setup.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-03 15:28:28.176115 umato-0.1.2/src/
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-03 15:28:28.176115 umato-0.1.2/src/evaluation/
+-rw-rw-r--   0 hj        (1010) hj        (1010)        0 2023-04-03 09:16:23.000000 umato-0.1.2/src/evaluation/__init__.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     3728 2023-04-03 09:16:23.000000 umato-0.1.2/src/evaluation/comparison.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1316 2023-04-03 09:16:23.000000 umato-0.1.2/src/evaluation/comparison_all.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     2172 2023-04-03 09:16:23.000000 umato-0.1.2/src/evaluation/comparison_local.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     2267 2023-04-03 09:16:23.000000 umato-0.1.2/src/evaluation/convert_to_csv.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     2081 2023-04-03 09:16:23.000000 umato-0.1.2/src/evaluation/convert_to_fvecs.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      907 2023-04-03 09:16:23.000000 umato-0.1.2/src/evaluation/convert_to_txt.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1539 2023-04-03 09:16:23.000000 umato-0.1.2/src/evaluation/save_subset.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1071 2023-04-03 09:16:23.000000 umato-0.1.2/src/evaluation/stability.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1607 2023-04-03 09:16:23.000000 umato-0.1.2/src/evaluation/stability_over.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)    14143 2023-04-03 09:16:23.000000 umato-0.1.2/src/evaluation/utils.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)      650 2023-04-03 09:16:23.000000 umato-0.1.2/src/evaluation/visualization.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-03 15:28:28.176115 umato-0.1.2/src/umato/
+-rw-rw-r--   0 hj        (1010) hj        (1010)      298 2023-04-03 09:16:23.000000 umato-0.1.2/src/umato/__init__.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)    33397 2023-04-03 09:16:23.000000 umato-0.1.2/src/umato/distances.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     6196 2023-05-03 15:14:44.000000 umato-0.1.2/src/umato/layouts.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     8909 2023-04-03 09:16:23.000000 umato-0.1.2/src/umato/nndescent.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)    27473 2023-04-03 09:16:23.000000 umato-0.1.2/src/umato/rp_tree.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)    15587 2023-04-03 09:16:23.000000 umato-0.1.2/src/umato/sparse.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)    12330 2023-04-03 09:16:23.000000 umato-0.1.2/src/umato/sparse_nndescent.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)    20628 2023-04-03 09:16:23.000000 umato-0.1.2/src/umato/umap_.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)    30244 2023-05-03 15:25:51.000000 umato-0.1.2/src/umato/umato_.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)    32109 2023-04-03 09:16:23.000000 umato-0.1.2/src/umato/umato_pva.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)    20526 2023-04-03 09:16:23.000000 umato-0.1.2/src/umato/utils.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-05-03 15:28:28.176115 umato-0.1.2/src/umato.egg-info/
+-rw-rw-r--   0 hj        (1010) hj        (1010)    14987 2023-05-03 15:28:28.000000 umato-0.1.2/src/umato.egg-info/PKG-INFO
+-rw-rw-r--   0 hj        (1010) hj        (1010)      795 2023-05-03 15:28:28.000000 umato-0.1.2/src/umato.egg-info/SOURCES.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-05-03 15:28:28.000000 umato-0.1.2/src/umato.egg-info/dependency_links.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)       66 2023-05-03 15:28:28.000000 umato-0.1.2/src/umato.egg-info/requires.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)       17 2023-05-03 15:28:28.000000 umato-0.1.2/src/umato.egg-info/top_level.txt
```

### Comparing `umato-0.1.1/PKG-INFO` & `umato-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umato
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Implementation of UMATO (Uniform Manifold Approximation with Two-Phase Optimization)
 Home-page: https://github.com/hyungkwonko/umato
 Author: Hyeon Jeon
 Author-email: hj@hcil.snu.ac.kr
 License: UNKNOWN
 Description: <p align="center">
           <h2 align="center">UMATO</h2>
@@ -35,15 +35,15 @@
         ```
         
         ```python
         import umato
         from sklearn.datasets import load_iris
         
         X, y = load_iris(return_X_y=True)
-        emb = umato.UMATO(hub_num=300).fit_transform(X)
+        emb = umato.UMATO(hub_num=50).fit_transform(X)
         ```
         
         ## API
         
         ### Default Class: UMATO
         
         Umato has only one class ```UMATO```. Note that UMATO shares a bunch of parameters with UMAP. For more details, please refer to [UMAP API](https://umap-learn.readthedocs.io/en/latest/api.html).
@@ -181,15 +181,15 @@
         
         Whether to utilize an angular random projection forest for initializing the approximate nearest neighbor search. This approach can offer improved speed, but it is primarily beneficial for metrics employing an angular-style distance, such as cosine, correlation, and others. For these metrics, angular forests will be automatically selected.
         
         ```python
         init = "pca"
         ```
         
-        The initialization method to use for the embedding. It must be a string or a numpy array. If a string is passed it must match one of the following: `init`, `randobm`, `spectral`.
+        The initialization method to use for the embedding. It must be a string or a numpy array. If a string is passed it must match one of the following: `init`, `random`, `spectral`.
         
         
         ```python
         verbose = False
         ```
         Whether to print information about the optimization process.
```

### Comparing `umato-0.1.1/README.md` & `umato-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ```
 
 ```python
 import umato
 from sklearn.datasets import load_iris
 
 X, y = load_iris(return_X_y=True)
-emb = umato.UMATO(hub_num=300).fit_transform(X)
+emb = umato.UMATO(hub_num=50).fit_transform(X)
 ```
 
 ## API
 
 ### Default Class: UMATO
 
 Umato has only one class ```UMATO```. Note that UMATO shares a bunch of parameters with UMAP. For more details, please refer to [UMAP API](https://umap-learn.readthedocs.io/en/latest/api.html).
@@ -173,15 +173,15 @@
 
 Whether to utilize an angular random projection forest for initializing the approximate nearest neighbor search. This approach can offer improved speed, but it is primarily beneficial for metrics employing an angular-style distance, such as cosine, correlation, and others. For these metrics, angular forests will be automatically selected.
 
 ```python
 init = "pca"
 ```
 
-The initialization method to use for the embedding. It must be a string or a numpy array. If a string is passed it must match one of the following: `init`, `randobm`, `spectral`.
+The initialization method to use for the embedding. It must be a string or a numpy array. If a string is passed it must match one of the following: `init`, `random`, `spectral`.
 
 
 ```python
 verbose = False
 ```
 Whether to print information about the optimization process.
```

### Comparing `umato-0.1.1/setup.py` & `umato-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="umato",
-	version="0.1.1",
+	version="0.1.2",
 	author="Hyeon Jeon",
 	author_email="hj@hcil.snu.ac.kr",
 	description="Python Implementation of UMATO (Uniform Manifold Approximation with Two-Phase Optimization)", 
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/hyungkwonko/umato",
 	classifiers=[
```

### Comparing `umato-0.1.1/src/evaluation/comparison.py` & `umato-0.1.2/src/evaluation/comparison.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/evaluation/comparison_all.py` & `umato-0.1.2/src/evaluation/comparison_all.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/evaluation/comparison_local.py` & `umato-0.1.2/src/evaluation/comparison_local.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/evaluation/convert_to_csv.py` & `umato-0.1.2/src/evaluation/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/evaluation/convert_to_fvecs.py` & `umato-0.1.2/src/evaluation/convert_to_fvecs.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/evaluation/convert_to_txt.py` & `umato-0.1.2/src/evaluation/convert_to_txt.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/evaluation/save_subset.py` & `umato-0.1.2/src/evaluation/save_subset.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/evaluation/stability.py` & `umato-0.1.2/src/evaluation/stability.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/evaluation/stability_over.py` & `umato-0.1.2/src/evaluation/stability_over.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/evaluation/utils.py` & `umato-0.1.2/src/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/evaluation/visualization.py` & `umato-0.1.2/src/evaluation/visualization.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/umato/distances.py` & `umato-0.1.2/src/umato/distances.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/umato/layouts.py` & `umato-0.1.2/src/umato/layouts.py`

 * *Files 13% similar despite different names*

```diff
@@ -64,18 +64,18 @@
             cost = get_CE(P, tmpZ, d_squared, a, b)
             # cost = get_DTM(P, tmpZ, sigma=0.1)
             costs.append(cost)
             print(
                 f"[INFO] Current loss: {cost:.6f}, @ iteration: {i+1}/{n_epochs}"
             )
 
-        if savefig:
-            if i < 10 or i == 30:
-                from umato.umato_ import plot_tmptmp
-                plot_tmptmp(data=Z, label=label, name=f"pic1_global{i}")
+        # if savefig:
+        #     if i < 10 or i == 30:
+        #         from umato.umato_ import plot_tmptmp
+        #         plot_tmptmp(data=Z, label=label, name=f"pic1_global{i}")
 
     return Z
 
 
 def nn_layout_optimize(
     head_embedding,
     tail_embedding,
@@ -128,19 +128,19 @@
             epoch_of_next_negative_sample,
             epoch_of_next_sample,
             n,
         )
 
         alpha = learning_rate * (1.0 - (float(n) / float(n_epochs)))
 
-        if verbose and n % 10 == 0:
-            from umato.umato_ import plot_tmptmp
+        # if verbose and n % 10 == 0:
+        #     from umato.umato_ import plot_tmptmp
 
-            plot_tmptmp(data=head_embedding, label=label, name=f"pic3_{k}_local{n}")
-            print("\tcompleted ", n, " / ", n_epochs, "epochs")
+        #     plot_tmptmp(data=head_embedding, label=label, name=f"pic3_{k}_local{n}")
+        #     print("\tcompleted ", n, " / ", n_epochs, "epochs")
 
     return head_embedding
 
 
 def _nn_layout_optimize_single_epoch(
     head_embedding,
     tail_embedding,
```

### Comparing `umato-0.1.1/src/umato/nndescent.py` & `umato-0.1.2/src/umato/nndescent.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/umato/rp_tree.py` & `umato-0.1.2/src/umato/rp_tree.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/umato/sparse.py` & `umato-0.1.2/src/umato/sparse.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/umato/sparse_nndescent.py` & `umato-0.1.2/src/umato/sparse_nndescent.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/umato/umap_.py` & `umato-0.1.2/src/umato/umap_.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/umato/umato_.py` & `umato-0.1.2/src/umato/umato_.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             raise AssertionError("Logic should not reach this block.")
 
         # get distance for each element
         targets = sorted_index[sorted_index_c != -1]
         distances_squared = calculate_distances(data, source, targets)
 
         # append other elements
-        sorted_distance_indexes = targets[np.argsort(distances_squared)[:leaf_num - 1]].astype('int64')
+        sorted_distance_indexes = targets[np.argsort(distances_squared)[:leaf_num - 1]].astype(np.int64)
 
         # create KNN
         disjoint = [source] + list(sorted_distance_indexes)
 
         # mark indexes as used
         sorted_index_c[index_map[sorted_distance_indexes]] = -1
 
@@ -152,15 +152,15 @@
 
         # get distance for each element
         targets = sorted_index[sorted_index_c != -1]
         distances_squared = calculate_distances(data, source, targets)
 
         # append other elements
         real_elements = leaf_num - padding_point_count
-        sorted_distance_indexes = targets[np.argsort(distances_squared)[:real_elements - 1]].astype('int64')
+        sorted_distance_indexes = targets[np.argsort(distances_squared)[:real_elements - 1]].astype(np.int64)
 
         # create KNN
         disjoint = [source] + list(sorted_distance_indexes) + [-1] * padding_point_count
 
         # mark indexes as used
         sorted_index_c[index_map[sorted_distance_indexes]] = -1
 
@@ -235,15 +235,15 @@
             Z=Z,
             a=a,
             b=b,
             alpha=alpha,
             n_epochs=n_epochs,
             verbose=verbose,
             savefig=verbose,
-            label=label[hubs],
+            label=label[hubs] if label is not None else None,
         )
     else:
         result = optimize_global_layout(
             P, Z, a, b, alpha=alpha, n_epochs=n_epochs
         )  # (TODO) how to optimize n_epochs & alpha?
 
     return result
@@ -262,15 +262,15 @@
             data=data, hubs=hubs, knn_indices=knn_indices, nn_consider=nn_consider,
         )
 
         if val == len(hubs):
             if len(init) > len(hubs) and verbose:
                 print(f"len(hubs) {len(hubs)} is smaller than len(init) {len(init)}")
             break
-
+		
     # generate random normal distribution
     random_normal = random_state.normal(
         loc=0.0, scale=0.05, size=list(init.shape)
     ).astype(np.float32)
 
     hub_nn = set(hubs) - set(original_hubs)
     hub_nn = np.array(list(hub_nn))
@@ -278,25 +278,25 @@
     # initialize other nodes' position using only hub information
     init = nn_initialize(
         data=data,
         init=init,
         original_hubs=original_hubs,
         hub_nn=hub_nn,
         random=random_normal,
-        nn_consider=10, # number of hubs to consider
+        nn_consider=10 if len(original_hubs) >= 10 else len(original_hubs), # number of hubs to consider
     )
 
     # np.array of hub information (hubs = 2, hub_nn = 1, outliers = 0)
     hub_info = np.zeros(data.shape[0])
     hub_info[hub_nn] = 1
     hub_info[original_hubs] = 2
 
     # save figure2
-    if verbose:
-        plot_tmptmp(data=init[hubs], label=label[hubs], name=f"pic2")
+    # if verbose:
+    #     plot_tmptmp(data=init[hubs], label=label[hubs] if label is not None else None, name=f"pic2")
 
     return init, hub_info, hubs
 
 
 def embed_outliers(
     data, init, hubs, disjoints, random_state, label, verbose=False,
 ):
@@ -312,16 +312,16 @@
 
     if len(init) != len(nodes_number):
         raise ValueError(
             f"total data # ({len(init)}) != total embedded # ({len(nodes_number)})!"
         )
 
     # save figure3
-    if verbose:
-        plot_tmptmp(data=init, label=label, name="pic4_disjoint")
+    # if verbose:
+    #     plot_tmptmp(data=init, label=label, name="pic4_disjoint")
 
     return init
 
 
 @numba.njit()
 def disjoint_initialize(
     data, init, hubs, disjoints, random, nn_consider=1.0,
@@ -401,14 +401,15 @@
     data, init, original_hubs, hub_nn, random, nn_consider=10,
 ):
 
     num_log = np.zeros(data.shape[0], dtype=np.float32)
     num_log[original_hubs] = -1
     num_log[hub_nn] = -1
 
+
     for i in numba.prange(len(hub_nn)):
         # find nearest hub nodes
         dists = np.zeros(len(original_hubs), dtype=np.float32)
         for j in numba.prange(len(original_hubs)):
             dist = 0.0
             for d in numba.prange(data.shape[1]):
                 e = original_hubs[j]
```

### Comparing `umato-0.1.1/src/umato/umato_pva.py` & `umato-0.1.2/src/umato/umato_pva.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/umato/utils.py` & `umato-0.1.2/src/umato/utils.py`

 * *Files identical despite different names*

### Comparing `umato-0.1.1/src/umato.egg-info/PKG-INFO` & `umato-0.1.2/src/umato.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umato
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Implementation of UMATO (Uniform Manifold Approximation with Two-Phase Optimization)
 Home-page: https://github.com/hyungkwonko/umato
 Author: Hyeon Jeon
 Author-email: hj@hcil.snu.ac.kr
 License: UNKNOWN
 Description: <p align="center">
           <h2 align="center">UMATO</h2>
@@ -35,15 +35,15 @@
         ```
         
         ```python
         import umato
         from sklearn.datasets import load_iris
         
         X, y = load_iris(return_X_y=True)
-        emb = umato.UMATO(hub_num=300).fit_transform(X)
+        emb = umato.UMATO(hub_num=50).fit_transform(X)
         ```
         
         ## API
         
         ### Default Class: UMATO
         
         Umato has only one class ```UMATO```. Note that UMATO shares a bunch of parameters with UMAP. For more details, please refer to [UMAP API](https://umap-learn.readthedocs.io/en/latest/api.html).
@@ -181,15 +181,15 @@
         
         Whether to utilize an angular random projection forest for initializing the approximate nearest neighbor search. This approach can offer improved speed, but it is primarily beneficial for metrics employing an angular-style distance, such as cosine, correlation, and others. For these metrics, angular forests will be automatically selected.
         
         ```python
         init = "pca"
         ```
         
-        The initialization method to use for the embedding. It must be a string or a numpy array. If a string is passed it must match one of the following: `init`, `randobm`, `spectral`.
+        The initialization method to use for the embedding. It must be a string or a numpy array. If a string is passed it must match one of the following: `init`, `random`, `spectral`.
         
         
         ```python
         verbose = False
         ```
         Whether to print information about the optimization process.
```

### Comparing `umato-0.1.1/src/umato.egg-info/SOURCES.txt` & `umato-0.1.2/src/umato.egg-info/SOURCES.txt`

 * *Files identical despite different names*

