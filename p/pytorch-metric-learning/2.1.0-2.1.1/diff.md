# Comparing `tmp/pytorch-metric-learning-2.1.0.tar.gz` & `tmp/pytorch-metric-learning-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-metric-learning-2.1.0.tar", last modified: Wed Apr  5 23:16:54 2023, max compression
+gzip compressed data, was "pytorch-metric-learning-2.1.1.tar", last modified: Wed May  3 11:53:00 2023, max compression
```

## Comparing `pytorch-metric-learning-2.1.0.tar` & `pytorch-metric-learning-2.1.1.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-04-05 23:16:54.958317 pytorch-metric-learning-2.1.0/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1090 2019-10-24 20:18:14.000000 pytorch-metric-learning-2.1.0/LICENSE
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    16202 2023-04-05 23:16:54.958317 pytorch-metric-learning-2.1.0/PKG-INFO
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15547 2023-04-05 22:59:33.000000 pytorch-metric-learning-2.1.0/README.md
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       38 2023-04-05 23:16:54.958317 pytorch-metric-learning-2.1.0/setup.cfg
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1507 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.0/setup.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-04-05 23:16:54.742314 pytorch-metric-learning-2.1.0/src/
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-04-05 23:16:54.770315 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       22 2023-04-05 22:59:33.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/__init__.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-04-05 23:16:54.790315 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/distances/
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      265 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/distances/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3469 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/distances/base_distance.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      755 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/distances/batched_distance.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      274 2021-02-11 13:46:54.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/distances/cosine_similarity.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      424 2021-02-11 13:46:54.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/distances/dot_product_similarity.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1042 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/distances/lp_distance.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      714 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/distances/snr_distance.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-04-05 23:16:54.850315 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1617 2023-04-05 22:50:01.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/__init__.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3061 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/angular_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1386 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/arcface_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      391 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/base_loss_wrapper.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2456 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/base_metric_loss_function.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2832 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/circle_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2005 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/contrastive_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      939 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/cosface_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5333 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/cross_batch_memory.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2833 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/fast_ap_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1492 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/generic_pair_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1689 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/instance_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2047 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5674 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3034 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/lifted_structure_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3288 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/margin_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2863 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/mixins.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1558 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/multi_similarity_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2351 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/multiple_losses.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1463 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/n_pairs_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1957 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/nca_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2173 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/normalized_softmax_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1778 2021-05-08 22:57:02.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/ntxent_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3506 2023-04-05 22:50:12.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/pnp_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3469 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/proxy_anchor_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1376 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/proxy_losses.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2021 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/self_supervised_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      373 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/signal_to_noise_ratio_losses.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3230 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/soft_triple_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      360 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/sphereface_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2600 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1715 2021-05-08 22:57:02.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/supcon_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2290 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/triplet_margin_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2049 2022-06-29 19:51:55.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/tuplet_margin_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3374 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/vicreg_loss.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-04-05 23:16:54.874316 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      569 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2874 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/angular_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2201 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/base_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     8131 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      404 2021-02-11 13:46:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/batch_hard_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2066 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/distance_weighted_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      493 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/embeddings_already_packaged_as_triplets.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2192 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/hdc_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2315 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/multi_similarity_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1742 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/pair_margin_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2403 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/triplet_margin_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2303 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/uniform_histogram_miner.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-04-05 23:16:54.890316 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      459 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      169 2021-02-11 13:46:59.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/avg_non_zero_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3816 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/base_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1130 2021-02-11 14:13:23.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/class_weighted_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1551 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/divisor_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      156 2021-02-11 13:47:00.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/do_nothing_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      473 2021-02-11 13:47:00.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/mean_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1214 2021-02-11 14:13:01.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/multiple_reducers.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2149 2021-05-08 22:57:04.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/per_anchor_reducer.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      182 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/sum_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2211 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/threshold_reducer.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-04-05 23:16:54.906316 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/regularizers/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      338 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/regularizers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      499 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/regularizers/base_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      871 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      723 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/regularizers/lp_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1229 2021-02-11 14:20:16.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2697 2021-05-08 22:57:05.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      432 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/regularizers/zero_mean_regularizer.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-04-05 23:16:54.914316 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/samplers/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      220 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/samplers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2132 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3856 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/samplers/hierarchical_sampler.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2555 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/samplers/m_per_class_sampler.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1696 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-04-05 23:16:54.922316 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/testers/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      243 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/testers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    12495 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/testers/base_tester.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1371 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/testers/global_embedding_space.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2820 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2791 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/testers/with_same_parent_label.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-04-05 23:16:54.934316 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      321 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    11599 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/base_trainer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3002 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/cascaded_embeddings.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     6807 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      625 2021-02-11 13:47:02.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/metric_loss_only.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1224 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/train_with_classifier.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2295 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/twostream_metric_loss.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-04-05 23:16:54.954317 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2020-05-18 23:01:59.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    18488 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/accuracy_calculator.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15447 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/common_functions.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     6399 2023-01-29 22:17:17.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/distributed.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    11776 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/inference.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1801 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/key_checker.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15836 2023-02-21 17:27:25.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/logging_presets.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     9444 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/loss_and_miner_utils.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1078 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/loss_tracker.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      661 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/module_with_records.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1624 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-04-05 23:16:54.778315 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning.egg-info/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    16202 2023-04-05 23:16:53.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning.egg-info/PKG-INFO
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5985 2023-04-05 23:16:53.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning.egg-info/SOURCES.txt
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)        1 2023-04-05 23:16:53.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning.egg-info/dependency_links.txt
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      226 2023-04-05 23:16:53.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning.egg-info/requires.txt
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       24 2023-04-05 23:16:53.000000 pytorch-metric-learning-2.1.0/src/pytorch_metric_learning.egg-info/top_level.txt
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.114436 pytorch-metric-learning-2.1.1/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1090 2019-10-24 20:18:14.000000 pytorch-metric-learning-2.1.1/LICENSE
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    16202 2023-05-03 11:53:00.114436 pytorch-metric-learning-2.1.1/PKG-INFO
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15547 2023-04-05 22:59:33.000000 pytorch-metric-learning-2.1.1/README.md
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       38 2023-05-03 11:53:00.114436 pytorch-metric-learning-2.1.1/setup.cfg
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1507 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.1/setup.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:52:59.926434 pytorch-metric-learning-2.1.1/src/
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:52:59.946434 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       22 2023-05-03 11:30:04.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/__init__.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:52:59.966434 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      265 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3508 2023-05-03 11:30:19.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/base_distance.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      755 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/batched_distance.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      274 2021-02-11 13:46:54.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/cosine_similarity.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      424 2021-02-11 13:46:54.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/dot_product_similarity.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1042 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/lp_distance.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      714 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/snr_distance.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.022435 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1617 2023-04-05 22:50:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/__init__.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3061 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/angular_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1386 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/arcface_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      391 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/base_loss_wrapper.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2456 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/base_metric_loss_function.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2832 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/circle_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2005 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/contrastive_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      939 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/cosface_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5333 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/cross_batch_memory.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2833 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/fast_ap_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1492 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/generic_pair_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1689 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/instance_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2047 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5674 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3034 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/lifted_structure_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3288 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/margin_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2863 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/mixins.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1558 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/multi_similarity_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2351 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/multiple_losses.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1463 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/n_pairs_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1957 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/nca_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2173 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/normalized_softmax_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1778 2021-05-08 22:57:02.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/ntxent_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3506 2023-04-05 22:50:12.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/pnp_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3469 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/proxy_anchor_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1376 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/proxy_losses.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2021 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/self_supervised_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      373 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/signal_to_noise_ratio_losses.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3230 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/soft_triple_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      360 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/sphereface_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2600 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1715 2021-05-08 22:57:02.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/supcon_loss.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2290 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/triplet_margin_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2049 2022-06-29 19:51:55.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/tuplet_margin_loss.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3374 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/vicreg_loss.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.038435 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      569 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2874 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/angular_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2201 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/base_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     8131 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      404 2021-02-11 13:46:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/batch_hard_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2066 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/distance_weighted_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      493 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/embeddings_already_packaged_as_triplets.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2192 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/hdc_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2315 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/multi_similarity_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1742 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/pair_margin_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2403 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/triplet_margin_miner.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2303 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/uniform_histogram_miner.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.058436 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      459 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      169 2021-02-11 13:46:59.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/avg_non_zero_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3816 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/base_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1130 2021-02-11 14:13:23.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/class_weighted_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1551 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/divisor_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      156 2021-02-11 13:47:00.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/do_nothing_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      473 2021-02-11 13:47:00.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/mean_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1214 2021-02-11 14:13:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/multiple_reducers.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2149 2021-05-08 22:57:04.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/per_anchor_reducer.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      182 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/sum_reducer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2211 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/threshold_reducer.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.066436 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      338 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      499 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/base_regularizer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      871 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      723 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/lp_regularizer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1229 2021-02-11 14:20:16.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2697 2021-05-08 22:57:05.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      432 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/zero_mean_regularizer.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.074436 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      220 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2132 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3856 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/hierarchical_sampler.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2555 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/m_per_class_sampler.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1696 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.082436 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      243 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    12495 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/base_tester.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1371 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/global_embedding_space.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2820 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2791 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/with_same_parent_label.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.094436 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      321 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    11599 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/base_trainer.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3002 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/cascaded_embeddings.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     6807 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      625 2021-02-11 13:47:02.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/metric_loss_only.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1224 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/train_with_classifier.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2295 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/twostream_metric_loss.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:53:00.114436 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2020-05-18 23:01:59.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/__init__.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    18488 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/accuracy_calculator.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15447 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/common_functions.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     6399 2023-01-29 22:17:17.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/distributed.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    11776 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/inference.py
+-rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1801 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/key_checker.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15836 2023-02-21 17:27:25.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/logging_presets.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     9444 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/loss_and_miner_utils.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1078 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/loss_tracker.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      661 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/module_with_records.py
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1624 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py
+drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-03 11:52:59.954434 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    16202 2023-05-03 11:52:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/PKG-INFO
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5985 2023-05-03 11:52:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/SOURCES.txt
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)        1 2023-05-03 11:52:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/dependency_links.txt
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      226 2023-05-03 11:52:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/requires.txt
+-rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       24 2023-05-03 11:52:58.000000 pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/top_level.txt
```

### Comparing `pytorch-metric-learning-2.1.0/LICENSE` & `pytorch-metric-learning-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/PKG-INFO` & `pytorch-metric-learning-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-metric-learning
-Version: 2.1.0
+Version: 2.1.1
 Summary: The easiest way to use deep metric learning in your application. Modular, flexible, and extensible. Written in PyTorch.
 Home-page: https://github.com/KevinMusgrave/pytorch-metric-learning
 Author: Kevin Musgrave
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.1.0 Summary: The
+Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.1.1 Summary: The
 easiest way to use deep metric learning in your application. Modular, flexible,
 and extensible. Written in PyTorch. Home-page: https://github.com/
 KevinMusgrave/pytorch-metric-learning Author: Kevin Musgrave License: UNKNOWN
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.0 Description-Content-Type: text/markdown
 Provides-Extra: with-hooks Provides-Extra: with-hooks-cpu Provides-Extra: docs
```

### Comparing `pytorch-metric-learning-2.1.0/README.md` & `pytorch-metric-learning-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/setup.py` & `pytorch-metric-learning-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/distances/base_distance.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/base_distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,17 @@
         return torch.norm(embeddings, p=self.p, dim=dim, **kwargs)
 
     def set_default_stats(
         self, query_emb, ref_emb, query_emb_normalized, ref_emb_normalized
     ):
         if self.collect_stats:
             with torch.no_grad():
-                self.initial_avg_query_norm: torch.mean(self.get_norm(query_emb)).item()
+                self.initial_avg_query_norm = torch.mean(
+                    self.get_norm(query_emb)
+                ).item()
                 self.initial_avg_ref_norm = torch.mean(self.get_norm(ref_emb)).item()
                 self.final_avg_query_norm = torch.mean(
                     self.get_norm(query_emb_normalized)
                 ).item()
                 self.final_avg_ref_norm = torch.mean(
                     self.get_norm(ref_emb_normalized)
                 ).item()
```

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/distances/batched_distance.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/batched_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/distances/lp_distance.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/lp_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/distances/snr_distance.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/distances/snr_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/__init__.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/angular_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/angular_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/arcface_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/arcface_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/base_metric_loss_function.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/base_metric_loss_function.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/circle_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/circle_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/contrastive_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/cosface_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/cosface_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/cross_batch_memory.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/cross_batch_memory.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/fast_ap_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/fast_ap_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/generic_pair_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/generic_pair_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/instance_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/instance_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/lifted_structure_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/lifted_structure_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/margin_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/margin_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/mixins.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/mixins.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/multi_similarity_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/multi_similarity_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/multiple_losses.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/multiple_losses.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/n_pairs_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/n_pairs_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/nca_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/nca_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/normalized_softmax_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/normalized_softmax_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/ntxent_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/ntxent_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/pnp_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/pnp_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/proxy_anchor_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/proxy_anchor_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/proxy_losses.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/proxy_losses.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/self_supervised_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/self_supervised_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/soft_triple_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/soft_triple_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/supcon_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/supcon_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/triplet_margin_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/triplet_margin_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/tuplet_margin_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/tuplet_margin_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/losses/vicreg_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/losses/vicreg_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/__init__.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/angular_miner.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/angular_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/base_miner.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/base_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/distance_weighted_miner.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/distance_weighted_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/hdc_miner.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/hdc_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/multi_similarity_miner.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/multi_similarity_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/pair_margin_miner.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/pair_margin_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/triplet_margin_miner.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/triplet_margin_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/miners/uniform_histogram_miner.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/miners/uniform_histogram_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/base_reducer.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/base_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/class_weighted_reducer.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/class_weighted_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/divisor_reducer.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/divisor_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/multiple_reducers.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/multiple_reducers.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/per_anchor_reducer.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/per_anchor_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/reducers/threshold_reducer.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/reducers/threshold_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/regularizers/lp_regularizer.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/lp_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/samplers/hierarchical_sampler.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/hierarchical_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/samplers/m_per_class_sampler.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/m_per_class_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/testers/base_tester.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/base_tester.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/testers/global_embedding_space.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/global_embedding_space.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/testers/with_same_parent_label.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/testers/with_same_parent_label.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/base_trainer.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/base_trainer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/cascaded_embeddings.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/cascaded_embeddings.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/metric_loss_only.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/metric_loss_only.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/train_with_classifier.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/train_with_classifier.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/trainers/twostream_metric_loss.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/trainers/twostream_metric_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/accuracy_calculator.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/accuracy_calculator.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/common_functions.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/common_functions.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/distributed.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/inference.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/inference.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/key_checker.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/key_checker.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/logging_presets.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/logging_presets.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/loss_and_miner_utils.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/loss_and_miner_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/loss_tracker.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/loss_tracker.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/module_with_records.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/module_with_records.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning.egg-info/PKG-INFO` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-metric-learning
-Version: 2.1.0
+Version: 2.1.1
 Summary: The easiest way to use deep metric learning in your application. Modular, flexible, and extensible. Written in PyTorch.
 Home-page: https://github.com/KevinMusgrave/pytorch-metric-learning
 Author: Kevin Musgrave
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.1.0 Summary: The
+Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.1.1 Summary: The
 easiest way to use deep metric learning in your application. Modular, flexible,
 and extensible. Written in PyTorch. Home-page: https://github.com/
 KevinMusgrave/pytorch-metric-learning Author: Kevin Musgrave License: UNKNOWN
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.0 Description-Content-Type: text/markdown
 Provides-Extra: with-hooks Provides-Extra: with-hooks-cpu Provides-Extra: docs
```

### Comparing `pytorch-metric-learning-2.1.0/src/pytorch_metric_learning.egg-info/SOURCES.txt` & `pytorch-metric-learning-2.1.1/src/pytorch_metric_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

