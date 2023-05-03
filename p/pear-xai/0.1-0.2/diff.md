# Comparing `tmp/pear-xai-0.1.tar.gz` & `tmp/pear-xai-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pear-xai-0.1.tar", last modified: Wed May  3 18:37:16 2023, max compression
+gzip compressed data, was "pear-xai-0.2.tar", last modified: Wed May  3 19:11:39 2023, max compression
```

## Comparing `pear-xai-0.1.tar` & `pear-xai-0.2.tar`

### file list

```diff
@@ -1,12 +1,165 @@
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 18:37:16.171897 pear-xai-0.1/
--rw-r--r--   0 avi        (501) staff       (20)     1504 2023-05-03 17:47:51.000000 pear-xai-0.1/LICENSE
--rw-r--r--   0 avi        (501) staff       (20)     2001 2023-05-03 18:37:16.171781 pear-xai-0.1/PKG-INFO
--rw-r--r--   0 avi        (501) staff       (20)     1724 2023-05-03 17:47:10.000000 pear-xai-0.1/README.md
-drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 18:37:16.171638 pear-xai-0.1/pear_xai.egg-info/
--rw-r--r--   0 avi        (501) staff       (20)     2001 2023-05-03 18:37:16.000000 pear-xai-0.1/pear_xai.egg-info/PKG-INFO
--rw-r--r--   0 avi        (501) staff       (20)      185 2023-05-03 18:37:16.000000 pear-xai-0.1/pear_xai.egg-info/SOURCES.txt
--rw-r--r--   0 avi        (501) staff       (20)        1 2023-05-03 18:37:16.000000 pear-xai-0.1/pear_xai.egg-info/dependency_links.txt
--rw-r--r--   0 avi        (501) staff       (20)      204 2023-05-03 18:37:16.000000 pear-xai-0.1/pear_xai.egg-info/requires.txt
--rw-r--r--   0 avi        (501) staff       (20)        5 2023-05-03 18:37:16.000000 pear-xai-0.1/pear_xai.egg-info/top_level.txt
--rw-r--r--   0 avi        (501) staff       (20)       38 2023-05-03 18:37:16.171935 pear-xai-0.1/setup.cfg
--rw-r--r--   0 avi        (501) staff       (20)     1292 2023-05-03 18:37:05.000000 pear-xai-0.1/setup.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.843679 pear-xai-0.2/
+-rw-r--r--   0 avi        (501) staff       (20)     1504 2023-05-03 17:47:51.000000 pear-xai-0.2/LICENSE
+-rw-r--r--   0 avi        (501) staff       (20)     2002 2023-05-03 19:11:39.843519 pear-xai-0.2/PKG-INFO
+-rw-r--r--   0 avi        (501) staff       (20)     1724 2023-05-03 17:47:10.000000 pear-xai-0.2/README.md
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.803829 pear-xai-0.2/captum/
+-rw-rw-r--   0 avi        (501) staff       (20)      281 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.804756 pear-xai-0.2/captum/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    20521 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/_utils/av.py
+-rw-rw-r--   0 avi        (501) staff       (20)    23939 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/_utils/common.py
+-rw-rw-r--   0 avi        (501) staff       (20)    35875 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/_utils/gradient.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.805002 pear-xai-0.2/captum/_utils/models/
+-rw-rw-r--   0 avi        (501) staff       (20)      499 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/_utils/models/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.805364 pear-xai-0.2/captum/_utils/models/linear_model/
+-rw-rw-r--   0 avi        (501) staff       (20)      447 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/_utils/models/linear_model/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    12218 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/_utils/models/linear_model/model.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11959 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/_utils/models/linear_model/train.py
+-rw-rw-r--   0 avi        (501) staff       (20)     2039 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/_utils/models/model.py
+-rw-rw-r--   0 avi        (501) staff       (20)     5137 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/_utils/progress.py
+-rw-rw-r--   0 avi        (501) staff       (20)     7142 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/_utils/sample_gradient.py
+-rw-rw-r--   0 avi        (501) staff       (20)     1176 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/_utils/typing.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.805478 pear-xai-0.2/captum/attr/
+-rw-rw-r--   0 avi        (501) staff       (20)     4660 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.807680 pear-xai-0.2/captum/attr/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    44110 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/deep_lift.py
+-rw-rw-r--   0 avi        (501) staff       (20)    29716 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/feature_ablation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    15634 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/feature_permutation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18688 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/gradient_shap.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14436 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/guided_backprop_deconvnet.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11370 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/guided_grad_cam.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6049 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/input_x_gradient.py
+-rw-rw-r--   0 avi        (501) staff       (20)    17859 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/integrated_gradients.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18691 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/kernel_shap.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.809211 pear-xai-0.2/captum/attr/_core/layer/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/layer/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11497 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/layer/grad_cam.py
+-rw-rw-r--   0 avi        (501) staff       (20)    15299 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/layer/internal_influence.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6759 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/layer/layer_activation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18776 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/layer/layer_conductance.py
+-rw-rw-r--   0 avi        (501) staff       (20)    33565 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/layer/layer_deep_lift.py
+-rw-rw-r--   0 avi        (501) staff       (20)    15136 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/layer/layer_feature_ablation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    22549 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/layer/layer_gradient_shap.py
+-rw-rw-r--   0 avi        (501) staff       (20)     9988 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/layer/layer_gradient_x_activation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    24591 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/layer/layer_integrated_gradients.py
+-rw-rw-r--   0 avi        (501) staff       (20)    13021 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/layer/layer_lrp.py
+-rw-rw-r--   0 avi        (501) staff       (20)    59483 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/lime.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18349 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/lrp.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.810267 pear-xai-0.2/captum/attr/_core/neuron/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/neuron/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    20769 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/neuron/neuron_conductance.py
+-rw-rw-r--   0 avi        (501) staff       (20)    25904 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/neuron/neuron_deep_lift.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14914 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/neuron/neuron_feature_ablation.py
+-rw-rw-r--   0 avi        (501) staff       (20)     9480 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/neuron/neuron_gradient.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14226 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/neuron/neuron_gradient_shap.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18506 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/neuron/neuron_guided_backprop_deconvnet.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14044 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/neuron/neuron_integrated_gradients.py
+-rw-rw-r--   0 avi        (501) staff       (20)    19799 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/noise_tunnel.py
+-rw-rw-r--   0 avi        (501) staff       (20)    19499 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/occlusion.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6516 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/saliency.py
+-rw-rw-r--   0 avi        (501) staff       (20)    39141 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_core/shapley_value.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.810654 pear-xai-0.2/captum/attr/_models/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_models/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11379 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_models/base.py
+-rw-rw-r--   0 avi        (501) staff       (20)    10280 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_models/pytext.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.812149 pear-xai-0.2/captum/attr/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     4781 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_utils/approximation_methods.py
+-rw-rw-r--   0 avi        (501) staff       (20)    21131 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_utils/attribution.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8032 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_utils/batching.py
+-rw-rw-r--   0 avi        (501) staff       (20)     3307 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_utils/class_summarizer.py
+-rw-rw-r--   0 avi        (501) staff       (20)    13033 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_utils/common.py
+-rw-rw-r--   0 avi        (501) staff       (20)      394 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_utils/custom_modules.py
+-rw-rw-r--   0 avi        (501) staff       (20)     2848 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_utils/input_layer_wrapper.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6309 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_utils/lrp_rules.py
+-rw-rw-r--   0 avi        (501) staff       (20)     7452 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_utils/stat.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8021 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_utils/summarizer.py
+-rw-rw-r--   0 avi        (501) staff       (20)    35661 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/attr/_utils/visualization.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.812302 pear-xai-0.2/captum/concept/
+-rw-rw-r--   0 avi        (501) staff       (20)      283 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/concept/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.812779 pear-xai-0.2/captum/concept/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/concept/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     7169 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/concept/_core/cav.py
+-rw-rw-r--   0 avi        (501) staff       (20)     3206 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/concept/_core/concept.py
+-rw-rw-r--   0 avi        (501) staff       (20)    33484 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/concept/_core/tcav.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.813259 pear-xai-0.2/captum/concept/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/concept/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8960 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/concept/_utils/classifier.py
+-rw-rw-r--   0 avi        (501) staff       (20)      726 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/concept/_utils/common.py
+-rw-rw-r--   0 avi        (501) staff       (20)     1919 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/concept/_utils/data_iterator.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.813375 pear-xai-0.2/captum/influence/
+-rw-rw-r--   0 avi        (501) staff       (20)      512 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/influence/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.813977 pear-xai-0.2/captum/influence/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/influence/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     1768 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/influence/_core/influence.py
+-rw-rw-r--   0 avi        (501) staff       (20)    14113 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/influence/_core/similarity_influence.py
+-rw-rw-r--   0 avi        (501) staff       (20)    71547 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/influence/_core/tracincp.py
+-rw-rw-r--   0 avi        (501) staff       (20)    85758 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/influence/_core/tracincp_fast_rand_proj.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.814391 pear-xai-0.2/captum/influence/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/influence/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    23003 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/influence/_utils/common.py
+-rw-rw-r--   0 avi        (501) staff       (20)    10067 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/influence/_utils/nearest_neighbors.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.814617 pear-xai-0.2/captum/insights/
+-rw-rw-r--   0 avi        (501) staff       (20)       84 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.832393 pear-xai-0.2/captum/insights/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/_utils/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.838230 pear-xai-0.2/captum/insights/attr_vis/
+-rw-rw-r--   0 avi        (501) staff       (20)       78 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/attr_vis/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.838492 pear-xai-0.2/captum/insights/attr_vis/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/attr_vis/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)      303 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/attr_vis/_utils/transforms.py
+-rw-rw-r--   0 avi        (501) staff       (20)    19467 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/attr_vis/app.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6733 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/attr_vis/attribution_calculation.py
+-rw-rw-r--   0 avi        (501) staff       (20)     2308 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/attr_vis/config.py
+-rw-rw-r--   0 avi        (501) staff       (20)     2584 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/attr_vis/example.py
+-rw-rw-r--   0 avi        (501) staff       (20)    11895 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/attr_vis/features.py
+-rw-rw-r--   0 avi        (501) staff       (20)     3331 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/attr_vis/server.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.838893 pear-xai-0.2/captum/insights/attr_vis/widget/
+-rw-rw-r--   0 avi        (501) staff       (20)      394 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/attr_vis/widget/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)      312 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/attr_vis/widget/_version.py
+-rw-rw-r--   0 avi        (501) staff       (20)     2057 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/attr_vis/widget/widget.py
+-rw-rw-r--   0 avi        (501) staff       (20)      208 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/insights/example.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.839021 pear-xai-0.2/captum/log/
+-rw-rw-r--   0 avi        (501) staff       (20)     1193 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/log/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.839331 pear-xai-0.2/captum/metrics/
+-rw-rw-r--   0 avi        (501) staff       (20)      204 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/metrics/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.839845 pear-xai-0.2/captum/metrics/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)       23 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/metrics/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    26077 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/metrics/_core/infidelity.py
+-rw-rw-r--   0 avi        (501) staff       (20)    13251 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/metrics/_core/sensitivity.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.840260 pear-xai-0.2/captum/metrics/_utils/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/metrics/_utils/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     3261 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/metrics/_utils/batching.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.840788 pear-xai-0.2/captum/module/
+-rw-rw-r--   0 avi        (501) staff       (20)      266 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/module/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    10241 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/module/binary_concrete_stochastic_gates.py
+-rw-rw-r--   0 avi        (501) staff       (20)     6914 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/module/gaussian_stochastic_gates.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8721 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/module/stochastic_gates_base.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.840918 pear-xai-0.2/captum/robust/
+-rw-rw-r--   0 avi        (501) staff       (20)      372 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/robust/__init__.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.841416 pear-xai-0.2/captum/robust/_core/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/robust/_core/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)     8725 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/robust/_core/fgsm.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.841787 pear-xai-0.2/captum/robust/_core/metrics/
+-rw-rw-r--   0 avi        (501) staff       (20)        0 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/robust/_core/metrics/__init__.py
+-rw-rw-r--   0 avi        (501) staff       (20)    19665 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/robust/_core/metrics/attack_comparator.py
+-rw-rw-r--   0 avi        (501) staff       (20)    18858 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/robust/_core/metrics/min_param_perturbation.py
+-rw-rw-r--   0 avi        (501) staff       (20)     1435 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/robust/_core/perturbation.py
+-rw-rw-r--   0 avi        (501) staff       (20)    10165 2023-02-27 18:57:42.000000 pear-xai-0.2/captum/robust/_core/pgd.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.842716 pear-xai-0.2/pear/
+-rw-r--r--   0 avi        (501) staff       (20)      757 2023-05-03 18:30:29.000000 pear-xai-0.2/pear/__init__.py
+-rw-r--r--   0 avi        (501) staff       (20)     2870 2023-03-02 01:56:26.000000 pear-xai-0.2/pear/disagreement_loss.py
+-rw-r--r--   0 avi        (501) staff       (20)    11118 2023-03-02 01:56:26.000000 pear-xai-0.2/pear/disagreement_metrics.py
+-rw-r--r--   0 avi        (501) staff       (20)     5573 2023-03-02 01:56:26.000000 pear-xai-0.2/pear/example.py
+-rw-r--r--   0 avi        (501) staff       (20)     7939 2023-05-03 18:30:45.000000 pear-xai-0.2/pear/explainers.py
+-rw-r--r--   0 avi        (501) staff       (20)     9559 2023-03-02 01:56:26.000000 pear-xai-0.2/pear/models.py
+-rw-r--r--   0 avi        (501) staff       (20)     4577 2023-03-02 01:56:26.000000 pear-xai-0.2/pear/tools.py
+drwxr-xr-x   0 avi        (501) staff       (20)        0 2023-05-03 19:11:39.843343 pear-xai-0.2/pear_xai.egg-info/
+-rw-r--r--   0 avi        (501) staff       (20)     2002 2023-05-03 19:11:39.000000 pear-xai-0.2/pear_xai.egg-info/PKG-INFO
+-rw-r--r--   0 avi        (501) staff       (20)     4563 2023-05-03 19:11:39.000000 pear-xai-0.2/pear_xai.egg-info/SOURCES.txt
+-rw-r--r--   0 avi        (501) staff       (20)        1 2023-05-03 19:11:39.000000 pear-xai-0.2/pear_xai.egg-info/dependency_links.txt
+-rw-r--r--   0 avi        (501) staff       (20)      204 2023-05-03 19:11:39.000000 pear-xai-0.2/pear_xai.egg-info/requires.txt
+-rw-r--r--   0 avi        (501) staff       (20)       12 2023-05-03 19:11:39.000000 pear-xai-0.2/pear_xai.egg-info/top_level.txt
+-rw-r--r--   0 avi        (501) staff       (20)       38 2023-05-03 19:11:39.843744 pear-xai-0.2/setup.cfg
+-rw-r--r--   0 avi        (501) staff       (20)     1342 2023-05-03 19:11:29.000000 pear-xai-0.2/setup.py
```

### Comparing `pear-xai-0.1/LICENSE` & `pear-xai-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pear-xai-0.1/PKG-INFO` & `pear-xai-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pear-xai
-Version: 0.1
+Version: 0.2
 Summary: PEAR: Post-hoc Explainer Agreement Regularization
 Home-page: https://arthur.ai
-License: MIT
+License: BSD3
 Keywords: pytorch,XAI,machine learning
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # :pear: PEAR: Post-hoc Explainer Agreement Regularization
```

### Comparing `pear-xai-0.1/README.md` & `pear-xai-0.2/README.md`

 * *Files identical despite different names*

### Comparing `pear-xai-0.1/pear_xai.egg-info/PKG-INFO` & `pear-xai-0.2/pear_xai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pear-xai
-Version: 0.1
+Version: 0.2
 Summary: PEAR: Post-hoc Explainer Agreement Regularization
 Home-page: https://arthur.ai
-License: MIT
+License: BSD3
 Keywords: pytorch,XAI,machine learning
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # :pear: PEAR: Post-hoc Explainer Agreement Regularization
```

### Comparing `pear-xai-0.1/setup.py` & `pear-xai-0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import os
 import sys
 from io import open
 
-from setuptools import setup
+from setuptools import setup, find_packages
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 sys.path.insert(0, os.path.join(here, "pear"))
 
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 # Manually install torch since the torchsort setup script requires this
 # the torch package is also listed in install_requires as this seems to be needed too
 os.system("pip install torch==1.11.0")
 
 setup(name="pear-xai",
-      version="v0.1",
+      version="v0.2",
       description="PEAR: Post-hoc Explainer Agreement Regularization",
       url="https://arthur.ai",
       keywords=["pytorch", "XAI", "machine learning"],
       long_description=long_description,
       long_description_content_type="text/markdown",
+      packages = find_packages(),
       py_modules=["pear"],
       python_requires=">=3.9",
       install_requires=[
           "jupyter==1.0.0",
           "lime==0.2.0.1",
           "matplotlib==3.5.2",
           "numpy==1.23.2",
@@ -35,9 +36,9 @@
           "shap==0.41.0",
           "sklearn==0.0",
           "tabulate==0.8.10",
           "torch==1.11.0",
           "torchvision==0.12.0",
           "tqdm==4.64.0",
           "torchsort==0.1.9"],
-      license="MIT")
+      license="BSD3")
```

