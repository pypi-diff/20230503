# Comparing `tmp/octis-1.8.3.tar.gz` & `tmp/octis-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/octis-1.8.3.tar", last modified: Mon Jul 26 12:51:01 2021, max compression
+gzip compressed data, was "dist/octis-1.9.0.tar", last modified: Mon Sep 27 13:34:48 2021, max compression
```

## Comparing `octis-1.8.3.tar` & `octis-1.9.0.tar`

### file list

```diff
@@ -1,125 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2021-07-26 12:33:00.000000 octis-1.8.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)      785 2021-07-26 12:33:00.000000 octis-1.8.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-07-26 12:33:00.000000 octis-1.8.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-07-26 12:51:01.000000 octis-1.8.3/octis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-26 12:51:01.000000 octis-1.8.3/octis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-26 12:51:01.000000 octis-1.8.3/octis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-07-26 12:51:01.000000 octis-1.8.3/octis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3317 2021-07-26 12:51:01.000000 octis-1.8.3/octis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    29151 2021-07-26 12:51:01.000000 octis-1.8.3/octis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-07-26 12:51:01.000000 octis-1.8.3/octis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-07-26 12:33:00.000000 octis-1.8.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-07-26 12:33:00.000000 octis-1.8.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2021-07-26 12:33:00.000000 octis-1.8.3/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)    16096 2021-07-26 12:33:00.000000 octis-1.8.3/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-07-26 12:33:00.000000 octis-1.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12638 2021-07-26 12:33:00.000000 octis-1.8.3/tests/test_octis.py
--rw-r--r--   0 runner    (1001) docker     (121)     5450 2021-07-26 12:33:00.000000 octis-1.8.3/tests/test_evaluation_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    24432 2021-07-26 12:33:00.000000 octis-1.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      331 2021-07-26 12:33:00.000000 octis-1.8.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-07-26 12:33:00.000000 octis-1.8.3/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)      767 2021-07-26 12:33:00.000000 octis-1.8.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     4290 2021-07-26 12:33:00.000000 octis-1.8.3/docs/dashboard.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5127 2021-07-26 12:33:00.000000 octis-1.8.3/docs/optimization.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-07-26 12:33:00.000000 octis-1.8.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-07-26 12:33:00.000000 octis-1.8.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-07-26 12:33:00.000000 octis-1.8.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4759 2021-07-26 12:33:00.000000 octis-1.8.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-07-26 12:33:00.000000 octis-1.8.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2021-07-26 12:33:00.000000 octis-1.8.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-07-26 12:33:00.000000 octis-1.8.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      606 2021-07-26 12:33:00.000000 octis-1.8.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     3487 2021-07-26 12:33:00.000000 octis-1.8.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      447 2021-07-26 12:51:01.000000 octis-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    29151 2021-07-26 12:51:01.000000 octis-1.8.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/dashboard/
--rw-r--r--   0 runner    (1001) docker     (121)    13305 2021-07-26 12:33:00.000000 octis-1.8.3/octis/dashboard/queueManager.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-07-26 12:33:00.000000 octis-1.8.3/octis/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2021-07-26 12:33:00.000000 octis-1.8.3/octis/dashboard/frameworkScanner.py
--rw-r--r--   0 runner    (1001) docker     (121)    15370 2021-07-26 12:33:00.000000 octis-1.8.3/octis/dashboard/experimentManager.py
--rw-r--r--   0 runner    (1001) docker     (121)    15067 2021-07-26 12:33:00.000000 octis-1.8.3/octis/dashboard/server.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2021-07-26 12:33:00.000000 octis-1.8.3/octis/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/models/
--rw-r--r--   0 runner    (1001) docker     (121)     3959 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    10425 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/LDA.py
--rw-r--r--   0 runner    (1001) docker     (121)     7995 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/LSI.py
--rw-r--r--   0 runner    (1001) docker     (121)     8341 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/NMF.py
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/NeuralLDA.py
--rw-r--r--   0 runner    (1001) docker     (121)     7772 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/HDP.py
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6309 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/NMF_scikit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/models/contextualized_topic_models/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/models/contextualized_topic_models/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/contextualized_topic_models/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18428 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/contextualized_topic_models/models/ctm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/models/contextualized_topic_models/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/contextualized_topic_models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6453 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/contextualized_topic_models/utils/data_preparation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/contextualized_topic_models/utils/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/contextualized_topic_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/models/contextualized_topic_models/networks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/contextualized_topic_models/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6194 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/contextualized_topic_models/networks/decoding_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     6253 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/contextualized_topic_models/networks/inference_network.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/models/contextualized_topic_models/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/contextualized_topic_models/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/contextualized_topic_models/datasets/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/contextualized_topic_models/contextualized_topic_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3343 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/LDA_tomopy.py
--rw-r--r--   0 runner    (1001) docker     (121)    18362 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/ETM.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/ProdLDA.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/models/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/early_stopping/pytorchtools.py
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/CTM.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/models/pytorchavitm/
--rw-r--r--   0 runner    (1001) docker     (121)    10143 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/pytorchavitm/AVITM.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/pytorchavitm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/models/pytorchavitm/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      660 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/pytorchavitm/datasets/bow.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/pytorchavitm/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/models/pytorchavitm/avitm/
--rw-r--r--   0 runner    (1001) docker     (121)     5766 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/pytorchavitm/avitm/decoder_network.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/pytorchavitm/avitm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17435 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/pytorchavitm/avitm/avitm_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3226 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/pytorchavitm/avitm/inference_network.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/models/ETM_model/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/ETM_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4491 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/ETM_model/etm.py
--rw-r--r--   0 runner    (1001) docker     (121)      775 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/ETM_model/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/ETM_model/skipgram.py
--rw-r--r--   0 runner    (1001) docker     (121)     2952 2021-07-26 12:33:00.000000 octis-1.8.3/octis/models/ETM_model/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2021-07-26 12:33:00.000000 octis-1.8.3/octis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)    28715 2021-07-26 12:33:00.000000 octis-1.8.3/octis/configuration/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-07-26 12:33:00.000000 octis-1.8.3/octis/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7405 2021-07-26 12:33:00.000000 octis-1.8.3/octis/configuration/citations.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-07-26 12:33:00.000000 octis-1.8.3/octis/octis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/optimization/
--rw-r--r--   0 runner    (1001) docker     (121)    10938 2021-07-26 12:33:00.000000 octis-1.8.3/octis/optimization/optimizer_tool.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-26 12:33:00.000000 octis-1.8.3/octis/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22126 2021-07-26 12:33:00.000000 octis-1.8.3/octis/optimization/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8085 2021-07-26 12:33:00.000000 octis-1.8.3/octis/optimization/optimizer_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-26 12:33:00.000000 octis-1.8.3/octis/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16876 2021-07-26 12:33:00.000000 octis-1.8.3/octis/preprocessing/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/evaluation_metrics/
--rw-r--r--   0 runner    (1001) docker     (121)     5050 2021-07-26 12:33:00.000000 octis-1.8.3/octis/evaluation_metrics/topic_significance_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     8087 2021-07-26 12:33:00.000000 octis-1.8.3/octis/evaluation_metrics/diversity_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     8910 2021-07-26 12:33:00.000000 octis-1.8.3/octis/evaluation_metrics/similarity_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     9203 2021-07-26 12:33:00.000000 octis-1.8.3/octis/evaluation_metrics/word_embeddings_rbo.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-26 12:33:00.000000 octis-1.8.3/octis/evaluation_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7765 2021-07-26 12:33:00.000000 octis-1.8.3/octis/evaluation_metrics/word_embeddings_rbo_centroid.py
--rw-r--r--   0 runner    (1001) docker     (121)     6247 2021-07-26 12:33:00.000000 octis-1.8.3/octis/evaluation_metrics/coherence_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)      692 2021-07-26 12:33:00.000000 octis-1.8.3/octis/evaluation_metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    10611 2021-07-26 12:33:00.000000 octis-1.8.3/octis/evaluation_metrics/rbo.py
--rw-r--r--   0 runner    (1001) docker     (121)     7747 2021-07-26 12:33:00.000000 octis-1.8.3/octis/evaluation_metrics/classification_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 12:51:01.000000 octis-1.8.3/octis/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)     4124 2021-07-26 12:33:00.000000 octis-1.8.3/octis/dataset/downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-26 12:33:00.000000 octis-1.8.3/octis/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14263 2021-07-26 12:33:00.000000 octis-1.8.3/octis/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2021-09-27 13:15:38.000000 octis-1.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3487 2021-09-27 13:15:38.000000 octis-1.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2133 2021-09-27 13:15:38.000000 octis-1.9.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-09-27 13:15:38.000000 octis-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2021-09-27 13:15:38.000000 octis-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    29151 2021-09-27 13:34:48.000000 octis-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    24432 2021-09-27 13:15:38.000000 octis-1.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2021-09-27 13:15:38.000000 octis-1.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-09-27 13:15:38.000000 octis-1.9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4759 2021-09-27 13:15:38.000000 octis-1.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-09-27 13:15:38.000000 octis-1.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4290 2021-09-27 13:15:38.000000 octis-1.9.0/docs/dashboard.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-09-27 13:15:38.000000 octis-1.9.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2021-09-27 13:15:38.000000 octis-1.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2021-09-27 13:15:38.000000 octis-1.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2021-09-27 13:15:38.000000 octis-1.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-09-27 13:15:38.000000 octis-1.9.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5127 2021-09-27 13:15:38.000000 octis-1.9.0/docs/optimization.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-09-27 13:15:38.000000 octis-1.9.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-09-27 13:15:38.000000 octis-1.9.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2021-09-27 13:15:38.000000 octis-1.9.0/octis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2021-09-27 13:15:38.000000 octis-1.9.0/octis/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/configuration/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-09-27 13:15:38.000000 octis-1.9.0/octis/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7405 2021-09-27 13:15:38.000000 octis-1.9.0/octis/configuration/citations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28715 2021-09-27 13:15:38.000000 octis-1.9.0/octis/configuration/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-09-27 13:15:38.000000 octis-1.9.0/octis/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15370 2021-09-27 13:15:38.000000 octis-1.9.0/octis/dashboard/experimentManager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2341 2021-09-27 13:15:38.000000 octis-1.9.0/octis/dashboard/frameworkScanner.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13305 2021-09-27 13:15:38.000000 octis-1.9.0/octis/dashboard/queueManager.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15067 2021-09-27 13:15:38.000000 octis-1.9.0/octis/dashboard/server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/dataset/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-27 13:15:38.000000 octis-1.9.0/octis/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14342 2021-09-27 13:15:38.000000 octis-1.9.0/octis/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4124 2021-09-27 13:15:38.000000 octis-1.9.0/octis/dataset/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/evaluation_metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-27 13:15:38.000000 octis-1.9.0/octis/evaluation_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7747 2021-09-27 13:15:38.000000 octis-1.9.0/octis/evaluation_metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6247 2021-09-27 13:15:38.000000 octis-1.9.0/octis/evaluation_metrics/coherence_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8094 2021-09-27 13:15:38.000000 octis-1.9.0/octis/evaluation_metrics/diversity_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2021-09-27 13:15:38.000000 octis-1.9.0/octis/evaluation_metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10611 2021-09-27 13:15:38.000000 octis-1.9.0/octis/evaluation_metrics/rbo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8910 2021-09-27 13:15:38.000000 octis-1.9.0/octis/evaluation_metrics/similarity_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5050 2021-09-27 13:15:38.000000 octis-1.9.0/octis/evaluation_metrics/topic_significance_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9203 2021-09-27 13:15:38.000000 octis-1.9.0/octis/evaluation_metrics/word_embeddings_rbo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7907 2021-09-27 13:15:38.000000 octis-1.9.0/octis/evaluation_metrics/word_embeddings_rbo_centroid.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/models/
+-rw-r--r--   0 runner    (1001) docker     (121)    11356 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/CTM.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8666 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/DETM.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/models/DETM_model/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/DETM_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6615 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/DETM_model/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8977 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/DETM_model/detm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14190 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/ETM.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/models/ETM_model/
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/ETM_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/ETM_model/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4491 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/ETM_model/etm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1932 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/ETM_model/skipgram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2952 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/ETM_model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7772 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/HDP.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10425 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/LDA.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3343 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/LDA_tomopy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7995 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/LSI.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8341 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/NMF.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6309 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/NMF_scikit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/NeuralLDA.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/ProdLDA.py
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4338 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/base_etm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/models/contextualized_topic_models/
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/contextualized_topic_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/contextualized_topic_models/contextualized_topic_models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/models/contextualized_topic_models/datasets/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/contextualized_topic_models/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1149 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/contextualized_topic_models/datasets/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/models/contextualized_topic_models/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/contextualized_topic_models/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18466 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/contextualized_topic_models/models/ctm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/models/contextualized_topic_models/networks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/contextualized_topic_models/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6253 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/contextualized_topic_models/networks/decoding_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6308 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/contextualized_topic_models/networks/inference_network.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/models/contextualized_topic_models/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/contextualized_topic_models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6453 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/contextualized_topic_models/utils/data_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2766 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/contextualized_topic_models/utils/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/models/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/early_stopping/pytorchtools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3959 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/models/pytorchavitm/
+-rw-r--r--   0 runner    (1001) docker     (121)    10143 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/pytorchavitm/AVITM.py
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/pytorchavitm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/models/pytorchavitm/avitm/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/pytorchavitm/avitm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17435 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/pytorchavitm/avitm/avitm_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5766 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/pytorchavitm/avitm/decoder_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3226 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/pytorchavitm/avitm/inference_network.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/models/pytorchavitm/datasets/
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/pytorchavitm/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2021-09-27 13:15:38.000000 octis-1.9.0/octis/models/pytorchavitm/datasets/bow.py
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-09-27 13:15:38.000000 octis-1.9.0/octis/octis.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/optimization/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-27 13:15:38.000000 octis-1.9.0/octis/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22126 2021-09-27 13:15:38.000000 octis-1.9.0/octis/optimization/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8085 2021-09-27 13:15:38.000000 octis-1.9.0/octis/optimization/optimizer_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10938 2021-09-27 13:15:38.000000 octis-1.9.0/octis/optimization/optimizer_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-27 13:15:38.000000 octis-1.9.0/octis/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16968 2021-09-27 13:15:38.000000 octis-1.9.0/octis/preprocessing/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/octis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    29151 2021-09-27 13:34:48.000000 octis-1.9.0/octis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3463 2021-09-27 13:34:48.000000 octis-1.9.0/octis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-27 13:34:48.000000 octis-1.9.0/octis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2021-09-27 13:34:48.000000 octis-1.9.0/octis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-27 13:34:48.000000 octis-1.9.0/octis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-09-27 13:34:48.000000 octis-1.9.0/octis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-27 13:34:48.000000 octis-1.9.0/octis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2021-09-27 13:34:48.000000 octis-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-09-27 13:15:38.000000 octis-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 13:34:48.000000 octis-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2021-09-27 13:15:38.000000 octis-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2775 2021-09-27 13:15:38.000000 octis-1.9.0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5450 2021-09-27 13:15:38.000000 octis-1.9.0/tests/test_evaluation_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12638 2021-09-27 13:15:38.000000 octis-1.9.0/tests/test_octis.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16096 2021-09-27 13:15:38.000000 octis-1.9.0/tests/test_optimization.py
```

### Comparing `octis-1.8.3/HISTORY.rst` & `octis-1.9.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =======
 History
 =======
 
+1.9.0 (2021-09-27)
+------------------
+* Bug fix preprocessing (#26)
+* Bug fix ctm (#28)
+* Bug fix weirbo_centroid (#31)
+* Added new Italian datasets
+* Minor fixes
+
 1.8.3 (2021-07-26)
 ------------------
 * Gensim migration from 3.8 to >=4.0.0
 
 1.8.2 (2021-07-25)
 ------------------
 * Fixed unwanted sorting of documents
```

### Comparing `octis-1.8.3/AUTHORS.rst` & `octis-1.9.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis.egg-info/SOURCES.txt` & `octis-1.9.0/octis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,25 +47,30 @@
 octis/evaluation_metrics/metrics.py
 octis/evaluation_metrics/rbo.py
 octis/evaluation_metrics/similarity_metrics.py
 octis/evaluation_metrics/topic_significance_metrics.py
 octis/evaluation_metrics/word_embeddings_rbo.py
 octis/evaluation_metrics/word_embeddings_rbo_centroid.py
 octis/models/CTM.py
+octis/models/DETM.py
 octis/models/ETM.py
 octis/models/HDP.py
 octis/models/LDA.py
 octis/models/LDA_tomopy.py
 octis/models/LSI.py
 octis/models/NMF.py
 octis/models/NMF_scikit.py
 octis/models/NeuralLDA.py
 octis/models/ProdLDA.py
 octis/models/__init__.py
+octis/models/base_etm.py
 octis/models/model.py
+octis/models/DETM_model/__init__.py
+octis/models/DETM_model/data.py
+octis/models/DETM_model/detm.py
 octis/models/ETM_model/__init__.py
 octis/models/ETM_model/data.py
 octis/models/ETM_model/etm.py
 octis/models/ETM_model/skipgram.py
 octis/models/ETM_model/utils.py
 octis/models/contextualized_topic_models/__init__.py
 octis/models/contextualized_topic_models/contextualized_topic_models.py
```

### Comparing `octis-1.8.3/octis.egg-info/PKG-INFO` & `octis-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: octis
-Version: 1.8.3
+Version: 1.9.0
 Summary: octis: a library for Optimizing and Comparing Topic Models.
 Home-page: https://github.com/MIND-LAB/OCTIS
 Author: Silvia Terragni
 Author-email: s.terragni4@campus.unimib.it
 License: MIT license
 Description: =========================================================
         OCTIS : Optimizing and Comparing Topic Models is Simple!
```

### Comparing `octis-1.8.3/setup.py` & `octis-1.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     keywords='octis',
     name='octis',
     packages=find_packages(include=['octis', 'octis.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/MIND-LAB/OCTIS',
-    version='1.8.3',
+    version='1.9.0',
     zip_safe=False,
 )
```

### Comparing `octis-1.8.3/LICENSE` & `octis-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/tests/test_datasets.py` & `octis-1.9.0/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/tests/test_optimization.py` & `octis-1.9.0/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/tests/test_octis.py` & `octis-1.9.0/tests/test_octis.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/tests/test_evaluation_metrics.py` & `octis-1.9.0/tests/test_evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/README.rst` & `octis-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/docs/modules.rst` & `octis-1.9.0/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/docs/make.bat` & `octis-1.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/docs/dashboard.rst` & `octis-1.9.0/docs/dashboard.rst`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/docs/optimization.rst` & `octis-1.9.0/docs/optimization.rst`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/docs/conf.py` & `octis-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/docs/installation.rst` & `octis-1.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/docs/Makefile` & `octis-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/CONTRIBUTING.rst` & `octis-1.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/PKG-INFO` & `octis-1.9.0/octis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: octis
-Version: 1.8.3
+Version: 1.9.0
 Summary: octis: a library for Optimizing and Comparing Topic Models.
 Home-page: https://github.com/MIND-LAB/OCTIS
 Author: Silvia Terragni
 Author-email: s.terragni4@campus.unimib.it
 License: MIT license
 Description: =========================================================
         OCTIS : Optimizing and Comparing Topic Models is Simple!
```

### Comparing `octis-1.8.3/octis/dashboard/queueManager.py` & `octis-1.9.0/octis/dashboard/queueManager.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/dashboard/frameworkScanner.py` & `octis-1.9.0/octis/dashboard/frameworkScanner.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/dashboard/experimentManager.py` & `octis-1.9.0/octis/dashboard/experimentManager.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/dashboard/server.py` & `octis-1.9.0/octis/dashboard/server.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/model.py` & `octis-1.9.0/octis/models/model.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/LDA.py` & `octis-1.9.0/octis/models/LDA.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/LSI.py` & `octis-1.9.0/octis/models/LSI.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/NMF.py` & `octis-1.9.0/octis/models/NMF.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/NeuralLDA.py` & `octis-1.9.0/octis/models/NeuralLDA.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/HDP.py` & `octis-1.9.0/octis/models/HDP.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/NMF_scikit.py` & `octis-1.9.0/octis/models/NMF_scikit.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/contextualized_topic_models/models/ctm.py` & `octis-1.9.0/octis/models/contextualized_topic_models/models/ctm.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         :param num_epochs: int, number of epochs to train for, (default 100)
         :param reduce_on_plateau: bool, reduce learning rate by 10x on plateau of 10 epochs (default False)
         :param num_data_loader_workers: int, number of data loader workers (default cpu_count). set it to 0 if you are using Windows
         """
 
         assert isinstance(input_size, int) and input_size > 0, \
             "input_size must by type int > 0."
-        assert isinstance(num_topics, int) and input_size > 0, \
+        assert (isinstance(num_topics, int) or isinstance(num_topics, np.int64)) and num_topics > 0, \
             "num_topics must by type int > 0."
         assert model_type in ['LDA', 'prodLDA'], \
             "model must be 'LDA' or 'prodLDA'."
         assert isinstance(hidden_sizes, tuple), \
             "hidden_sizes must be type tuple."
         assert activation in ['softplus', 'relu', 'sigmoid', 'swish', 'tanh', 'leakyrelu',
                               'rrelu', 'elu', 'selu'], \
```

### Comparing `octis-1.8.3/octis/models/contextualized_topic_models/utils/data_preparation.py` & `octis-1.9.0/octis/models/contextualized_topic_models/utils/data_preparation.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/contextualized_topic_models/utils/preprocessing.py` & `octis-1.9.0/octis/models/contextualized_topic_models/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/contextualized_topic_models/networks/decoding_network.py` & `octis-1.9.0/octis/models/contextualized_topic_models/networks/decoding_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """PyTorch class for feed foward AVITM network."""
 
 import torch
 from torch import nn
 from torch.nn import functional as F
+import numpy as np
 
 from octis.models.contextualized_topic_models.networks.inference_network import CombinedInferenceNetwork, ContextualInferenceNetwork
 
 
 class DecoderNetwork(nn.Module):
 
     """AVITM Network."""
@@ -25,15 +26,15 @@
             activation : string, 'softplus', 'relu', (default 'softplus')
             learn_priors : bool, make priors learnable parameter
             topic_prior_mean: double, mean parameter of the prior
             topic_prior_variance: double, variance parameter of the prior
         """
         super(DecoderNetwork, self).__init__()
         assert isinstance(input_size, int), "input_size must by type int."
-        assert isinstance(n_components, int) and n_components > 0, \
+        assert (isinstance(n_components, int) or isinstance(n_components, np.int64)) and n_components > 0, \
             "n_components must be type int > 0."
         assert model_type in ['prodLDA', 'LDA'], \
             "model type must be 'prodLDA' or 'LDA'"
         assert isinstance(hidden_sizes, tuple), \
             "hidden_sizes must be type tuple."
         assert activation in ['softplus', 'relu', 'sigmoid', 'tanh', 'leakyrelu',
                               'rrelu', 'elu', 'selu'], \
```

### Comparing `octis-1.8.3/octis/models/contextualized_topic_models/networks/inference_network.py` & `octis-1.9.0/octis/models/contextualized_topic_models/networks/inference_network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """PyTorch class for feed foward inference network."""
 
 from collections import OrderedDict
 from torch import nn
 import torch
-
+import numpy as np
 
 class ContextualInferenceNetwork(nn.Module):
 
     """Inference Network."""
 
     def __init__(self, input_size, bert_size, output_size, hidden_sizes,
                  activation='softplus', dropout=0.2):
@@ -78,16 +78,14 @@
         x = self.dropout_enc(x)
         mu = self.f_mu_batchnorm(self.f_mu(x))
         log_sigma = self.f_sigma_batchnorm(self.f_sigma(x))
 
         return mu, log_sigma
 
 
-
-
 class CombinedInferenceNetwork(nn.Module):
 
     """Inference Network."""
 
     def __init__(self, input_size, bert_size, output_size, hidden_sizes,
                  activation='softplus', dropout=0.2):
         """
@@ -98,15 +96,15 @@
             output_size : int, dimension of output
             hidden_sizes : tuple, length = n_layers
             activation : string, 'softplus' or 'relu', default 'softplus'
             dropout : float, default 0.2, default 0.2
         """
         super(CombinedInferenceNetwork, self).__init__()
         assert isinstance(input_size, int), "input_size must by type int."
-        assert isinstance(output_size, int), "output_size must be type int."
+        assert (isinstance(output_size, int) or isinstance(output_size, np.int64)), "output_size must be type int."
         assert isinstance(hidden_sizes, tuple), \
             "hidden_sizes must be type tuple."
         assert activation in ['softplus', 'relu', 'sigmoid', 'tanh', 'leakyrelu',
                               'rrelu', 'elu', 'selu'], \
             "activation must be 'softplus', 'relu', 'sigmoid', 'leakyrelu'," \
             " 'rrelu', 'elu', 'selu' or 'tanh'."
```

### Comparing `octis-1.8.3/octis/models/contextualized_topic_models/datasets/dataset.py` & `octis-1.9.0/octis/models/contextualized_topic_models/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/LDA_tomopy.py` & `octis-1.9.0/octis/models/LDA_tomopy.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/ETM.py` & `octis-1.9.0/octis/models/ETM.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from __future__ import print_function
 from octis.models.early_stopping.pytorchtools import EarlyStopping
-
 import torch
 import numpy as np
 from octis.models.ETM_model import data
 from sklearn.feature_extraction.text import CountVectorizer
 from torch import nn, optim
 from octis.models.ETM_model import etm
-from octis.models.model import AbstractModel
+from octis.models.base_etm import BaseETM
 import gensim
 import pickle as pkl
 
 
-class ETM(AbstractModel):
+class ETM(BaseETM):
 
     def __init__(self, num_topics=10, num_epochs=100, t_hidden_size=800, rho_size=300, embedding_size=300,
                  activation='relu', dropout=0.5, lr=0.005, optimizer='adam', batch_size=128, clip=0.0,
                  wdecay=1.2e-6, bow_norm=1, device='cpu', top_word=10, train_embeddings=True, embeddings_path=None,
                  use_partitions=True):
         super(ETM, self).__init__()
         self.hyperparameters = dict()
@@ -104,41 +103,14 @@
                              embeddings=self.embeddings,
                              train_embeddings=self.hyperparameters['train_embeddings'],
                              enc_drop=self.hyperparameters['dropout']).to(self.device)
         print('model: {}'.format(self.model))
 
         self.optimizer = self.set_optimizer()
 
-    def set_optimizer(self):
-        self.hyperparameters['lr'] = float(self.hyperparameters['lr'])
-        self.hyperparameters['wdecay'] = float(self.hyperparameters['wdecay'])
-        if self.hyperparameters['optimizer'] == 'adam':
-            optimizer = optim.Adam(self.model.parameters(), lr=self.hyperparameters['lr'],
-                                   weight_decay=self.hyperparameters['wdecay'])
-        elif self.hyperparameters['optimizer'] == 'adagrad':
-            optimizer = optim.Adagrad(self.model.parameters(), lr=self.hyperparameters['lr'],
-                                      weight_decay=self.hyperparameters['wdecay'])
-        elif self.hyperparameters['optimizer'] == 'adadelta':
-            optimizer = optim.Adadelta(self.model.parameters(), lr=self.hyperparameters['lr'],
-                                       weight_decay=self.hyperparameters['wdecay'])
-        elif self.hyperparameters['optimizer'] == 'rmsprop':
-            optimizer = optim.RMSprop(self.model.parameters(), lr=self.hyperparameters['lr'],
-                                      weight_decay=self.hyperparameters['wdecay'])
-        elif self.hyperparameters['optimizer'] == 'asgd':
-            optimizer = optim.ASGD(self.model.parameters(), lr=self.hyperparameters['lr'],
-                                   t0=0, lambd=0., weight_decay=self.hyperparameters['wdecay'])
-        elif self.hyperparameters['optimizer'] == 'sgd':
-            optimizer = optim.SGD(self.model.parameters(), lr=self.hyperparameters['lr'],
-                                  weight_decay=self.hyperparameters['wdecay'])
-        else:
-            print('Defaulting to vanilla SGD')
-            optimizer = optim.SGD(self.model.parameters(), lr=self.hyperparameters['lr'])
-
-        return optimizer
-
     def _train_epoch(self, epoch):
         self.data_list = []
         self.model.train()
         acc_loss = 0
         acc_kl_theta_loss = 0
         cnt = 0
         indices = torch.arange(0, len(self.train_tokens))
@@ -253,15 +225,14 @@
                     top_words = list(gammas[k].argsort()[-self.top_word:][::-1])
                 topic_words = [self.vocab[a] for a in top_words]
                 topic_w.append(topic_words)
 
         info['topic-word-matrix'] = gammas
         info['topic-document-matrix'] = theta.cpu().detach().numpy().T
         info['topics'] = topic_w
-        print(info['topics'])
         return info
 
     def inference(self):
         assert isinstance(self.use_partitions, bool) and self.use_partitions
         topic_d = []
         self.model.eval()
         indices = torch.arange(0, len(self.test_tokens))
@@ -294,20 +265,17 @@
         for k in hyperparameters.keys():
             if k in self.hyperparameters.keys():
                 self.hyperparameters[k] = hyperparameters.get(k, self.hyperparameters[k])
 
     def partitioning(self, use_partitions=False):
         self.use_partitions = use_partitions
 
+    
     @staticmethod
     def preprocess(vocab2id, train_corpus, test_corpus=None, validation_corpus=None):
-        # def split_bow(bow_in, n_docs):
-        #    indices = np.asarray([np.asarray([w for w in bow_in[doc, :].indices]) for doc in range(n_docs)])
-        #    counts = np.asarray([np.asarray([c for c in bow_in[doc, :].data]) for doc in range(n_docs)])
-        #    return np.expand_dims(indices, axis=0), np.expand_dims(counts, axis=0)
 
         def split_bow(bow_in, n_docs):
             indices = [[w for w in bow_in[doc, :].indices] for doc in range(n_docs)]
             counts = [[c for c in bow_in[doc, :].data] for doc in range(n_docs)]
             return indices, counts
 
         vec = CountVectorizer(
@@ -339,50 +307,7 @@
         else:
             if validation_corpus is not None:
                 x_validation = vec.transform(validation_corpus)
                 x_val_tokens, x_val_count = split_bow(x_validation, x_validation.shape[0])
                 return x_train_tokens, x_train_count, x_val_tokens, x_val_count
             else:
                 return x_train_tokens, x_train_count
-
-    def load_embeddings(self):
-        if not self.hyperparameters['train_embeddings']:
-            vectors = {}
-            embs = pkl.load(open(self.hyperparameters['embeddings_path'], 'rb'))
-            for l in embs:
-                line = l.split()
-                word = line[0]
-                if word in self.vocab.values():
-                    vect = np.array(line[1:]).astype(np.float)
-                    vectors[word] = vect
-            embeddings = np.zeros((len(self.vocab.keys()), self.hyperparameters['embedding_size']))
-            words_found = 0
-            for i, word in enumerate(self.vocab.values()):
-                try:
-                    embeddings[i] = vectors[word]
-                    words_found += 1
-                except KeyError:
-                    embeddings[i] = np.random.normal(scale=0.6, size=(self.hyperparameters['embedding_size'],))
-            self.embeddings = torch.from_numpy(embeddings).to(self.device)
-
-    def filter_pretrained_embeddings(self, pretrained_embeddings_path, save_embedding_path, vocab_path, binary=True):
-        """
-        Filter the embeddings from a set of word2vec-format pretrained embeddings based on the vocabulary
-        This should allow you to avoid to load the whole embedding space every time you do Bayesian Optimization
-        but just the embeddings that are in the vocabulary.
-        :param pretrained_embeddings_path:
-        :return:
-        """
-        vocab = []
-        with open(vocab_path, 'r') as fr:
-            for line in fr.readlines():
-                vocab.append(line.strip().split(" ")[0])
-
-        w2v_model = gensim.models.KeyedVectors.load_word2vec_format(pretrained_embeddings_path, binary=binary)
-        embeddings = []
-        for word in vocab:
-            if word in w2v_model.vocab:
-                line = word
-                for w in w2v_model[word].tolist():
-                    line = line + " " + str(w)
-                embeddings.append(line)
-        pkl.dump(embeddings, open(save_embedding_path, 'wb'))
```

### Comparing `octis-1.8.3/octis/models/ProdLDA.py` & `octis-1.9.0/octis/models/ProdLDA.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/early_stopping/pytorchtools.py` & `octis-1.9.0/octis/models/early_stopping/pytorchtools.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/CTM.py` & `octis-1.9.0/octis/models/CTM.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/pytorchavitm/AVITM.py` & `octis-1.9.0/octis/models/pytorchavitm/AVITM.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/pytorchavitm/datasets/bow.py` & `octis-1.9.0/octis/models/pytorchavitm/datasets/bow.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/pytorchavitm/avitm/decoder_network.py` & `octis-1.9.0/octis/models/pytorchavitm/avitm/decoder_network.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/pytorchavitm/avitm/avitm_model.py` & `octis-1.9.0/octis/models/pytorchavitm/avitm/avitm_model.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/pytorchavitm/avitm/inference_network.py` & `octis-1.9.0/octis/models/pytorchavitm/avitm/inference_network.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/ETM_model/etm.py` & `octis-1.9.0/octis/models/ETM_model/etm.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/ETM_model/data.py` & `octis-1.9.0/octis/models/ETM_model/data.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/ETM_model/skipgram.py` & `octis-1.9.0/octis/models/ETM_model/skipgram.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/models/ETM_model/utils.py` & `octis-1.9.0/octis/models/ETM_model/utils.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/configuration/defaults.py` & `octis-1.9.0/octis/configuration/defaults.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/configuration/citations.py` & `octis-1.9.0/octis/configuration/citations.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/optimization/optimizer_tool.py` & `octis-1.9.0/octis/optimization/optimizer_tool.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/optimization/optimizer.py` & `octis-1.9.0/octis/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/optimization/optimizer_evaluation.py` & `octis-1.9.0/octis/optimization/optimizer_evaluation.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/preprocessing/preprocessing.py` & `octis-1.9.0/octis/preprocessing/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         init Preprocessing
 
         :param lowercase: if true, words in documents are reduced to lowercase (default: true)
         :type lowercase: boolean
         :param vocabulary: the vocabulary of the corpus to preprocess (default: None)
         :type vocabulary: list
         :param max_features: maximum number of words that the vocabulary must contain. The less frequent
-        words will be removed (default: None)
+        words will be removed. If it's not None, then max_df and min_df are ignored (default: None)
         :type max_features: int
         :param min_df: words below this minumum document frequency will be removed (default: 0.0)
         :type min_df: float
         :param max_df: words above this maximum document frequency will be removed (default: 1.0)
         :type max_df: float
         :param remove_punctuation: if true, punctuation will be removed (default: true)
         :type remove_punctuation: bool
@@ -244,16 +244,17 @@
                                          lowercase=self.lowercase, stop_words=self.stopwords)
 
         elif self.max_features is not None:
             self.preprocessing_steps.append('filter vocabulary to ' + str(self.max_features) + ' terms')
             self.preprocessing_steps.append('filter words with document frequency lower than ' + str(self.min_df) +
                                             ' and higher than ' + str(self.max_df))
             self.preprocessing_steps.append('filter words with less than ' + str(self.min_chars) + " character")
-            vectorizer = TfidfVectorizer(df_max_freq=self.max_df, df_min_freq=self.min_df, lowercase=self.lowercase,
-                                         max_features=self.max_features, stop_words=self.stopwords,
+            # we ignore df_max_freq e df_min_freq because self.max_features is not None
+            vectorizer = TfidfVectorizer(lowercase=self.lowercase, max_features=self.max_features,
+                                         stop_words=self.stopwords,
                                          token_pattern=r"(?u)\b[\w|\-]{" + str(self.min_chars) + r",}\b")
 
         else:
 
             #string.punctuation
 
             self.preprocessing_steps.append('filter words with document frequency lower than ' + str(self.min_df) +
```

### Comparing `octis-1.8.3/octis/evaluation_metrics/topic_significance_metrics.py` & `octis-1.9.0/octis/evaluation_metrics/topic_significance_metrics.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/evaluation_metrics/diversity_metrics.py` & `octis-1.9.0/octis/evaluation_metrics/diversity_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
             for list1, list2 in itertools.combinations(topics, 2):
                 word2index = get_word2index(list1, list2)
                 index2word = {v: k for k, v in word2index.items()}
                 indexed_list1 = [word2index[word] for word in list1]
                 indexed_list2 = [word2index[word] for word in list2]
                 rbo_val = weirbo_centroid(
                     indexed_list1[:self.topk], indexed_list2[:self.topk], p=self.weight, index2word=index2word,
-                    word2vec=self.wv, norm=self.norm)[2]
+                    embedding_space=self.wv, norm=self.norm)[2]
 
                 collect.append(rbo_val)
             return 1 - np.mean(collect)
 
 
 class LogOddsRatio(AbstractMetric):
     def __init__(self):
```

### Comparing `octis-1.8.3/octis/evaluation_metrics/similarity_metrics.py` & `octis-1.9.0/octis/evaluation_metrics/similarity_metrics.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/evaluation_metrics/word_embeddings_rbo.py` & `octis-1.9.0/octis/evaluation_metrics/word_embeddings_rbo.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/evaluation_metrics/word_embeddings_rbo_centroid.py` & `octis-1.9.0/octis/evaluation_metrics/word_embeddings_rbo_centroid.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,122 +31,118 @@
         if isinstance(v, set):
             ans.update(v)
         else:
             ans.add(v)
     return ans
 
 
-def embeddings_overlap(list1, list2, depth, index2word, word2vec, norm=True):
+def embeddings_overlap(list1, list2, depth, index2word, embedding_space, norm=True):
     set1, set2 = set_at_depth(list1, depth), set_at_depth(list2, depth)
     word_list1 = [index2word[index] for index in list1]
     word_list2 = [index2word[index] for index in list2]
 
-    centroid_1 = np.mean([word2vec.wv[w] for w in word_list1[:depth]], axis=0)
-    centroid_2 = np.mean([word2vec.wv[w] for w in word_list2[:depth]], axis=0)
+    centroid_1 = np.mean([embedding_space[w] for w in word_list1[:depth] if w in embedding_space], axis=0)
+    centroid_2 = np.mean([embedding_space[w] for w in word_list2[:depth] if w in embedding_space], axis=0)
     cos_sim = 1 - distance.cosine(centroid_1, centroid_2)
     if cos_sim > 1:
         cos_sim = 1
     elif cos_sim < -1:
         cos_sim = -1
     if norm:
         e_ov = 1 - (math.acos(cos_sim) / math.pi)
     else:
         e_ov = cos_sim
     return e_ov, len(set1), len(set2)
 
 
-def overlap(list1, list2, depth, index2word, word2vec, norm):
+def overlap(list1, list2, depth, index2word, embedding_space, norm):
     # return agreement(list1, list2, depth) * min(depth, len(list1), len(list2))
     # NOTE: comment the preceding and uncomment the following line if you want
     # to stick to the algorithm as defined by the paper
-    ov = embeddings_overlap(list1, list2, depth, index2word, word2vec, norm=norm)[0]
+    ov = embeddings_overlap(list1, list2, depth, index2word, embedding_space, norm=norm)[0]
     # print("overlap", ov)
     return ov
 
 
-def agreement(list1, list2, depth, index2word, word2vec, norm):
+def agreement(list1, list2, depth, index2word, embedding_space, norm):
     """Proportion of shared values between two sorted lists at given depth."""
-    len_intersection, len_set1, len_set2 = embeddings_overlap(list1, list2, depth, index2word, word2vec, norm=norm)
+    len_intersection, len_set1, len_set2 = embeddings_overlap(list1, list2, depth, index2word, embedding_space=embedding_space, norm=norm)
     return 2 * len_intersection / (len_set1 + len_set2)
 
 
-def cumulative_agreement(list1, list2, depth, index2word, word2vec, norm):
-    return (agreement(list1, list2, d, index2word, word2vec, norm) for d in range(1, depth + 1))
+def cumulative_agreement(list1, list2, depth, index2word, embedding_space, norm):
+    return (agreement(list1, list2, d, index2word, embedding_space, norm) for d in range(1, depth + 1))
 
 
-def rbo_min(list1, list2, p, index2word, word2vec, norm=True, depth=None):
+def rbo_min(list1, list2, p, index2word, embedding_space, norm=True, depth=None):
     """Tight lower bound on RBO.
     See equation (11) in paper.
     """
     depth = min(len(list1), len(list2)) if depth is None else depth
-    x_k = overlap(list1, list2, depth, index2word, word2vec, norm)
+    x_k = overlap(list1, list2, depth, index2word, embedding_space, norm)
     log_term = x_k * math.log(1 - p)
     sum_term = sum(
-        p ** d / d * (overlap(list1, list2, d, index2word, word2vec=word2vec, norm=norm) - x_k) for d in range(1, depth + 1)
+        p ** d / d * (overlap(list1, list2, d, index2word, embedding_space=embedding_space, norm=norm) - x_k) for d in range(1, depth + 1)
     )
     return (1 - p) / p * (sum_term - log_term)
 
 
-def rbo_res(list1, list2, p, index2word, word2vec, norm=True):
+def rbo_res(list1, list2, p, index2word, embedding_space, norm=True):
     """Upper bound on residual overlap beyond evaluated depth.
     See equation (30) in paper.
     NOTE: The doctests weren't verified against manual computations but seem
     plausible. In particular, for identical lists, ``rbo_min()`` and
     ``rbo_res()`` should add up to 1, which is the case.
     """
     S, L = sorted((list1, list2), key=len)
     s, l = len(S), len(L)
-    x_l = overlap(list1, list2, l, index2word, word2vec, norm=norm)
+    x_l = overlap(list1, list2, l, index2word, embedding_space, norm=norm)
     # since overlap(...) can be fractional in the general case of ties and f
     # must be an integer --> math.ceil()
     f = int(math.ceil(l + s - x_l))
     # upper bound of range() is non-inclusive, therefore + 1 is needed
     term1 = s * sum(p ** d / d for d in range(s + 1, f + 1))
     term2 = l * sum(p ** d / d for d in range(l + 1, f + 1))
     term3 = x_l * (math.log(1 / (1 - p)) - sum(p ** d / d for d in range(1, f + 1)))
     return p ** s + p ** l - p ** f - (1 - p) / p * (term1 + term2 + term3)
 
 
-def rbo_ext(list1, list2, p, index2word, word2vec, norm=True):
+def rbo_ext(list1, list2, p, index2word, embedding_space, norm=True):
     """RBO point estimate based on extrapolating observed overlap.
     See equation (32) in paper.
     NOTE: The doctests weren't verified against manual computations but seem
     plausible.
-    >>> _round(rbo_ext("abcdefg", "abcdefg", .9))
-    1.0
-    >>> _round(rbo_ext("abcdefg", "bacdefg", .9))
-    0.9
     """
     S, L = sorted((list1, list2), key=len)
     s, l = len(S), len(L)
-    x_l = overlap(list1, list2, l, index2word, word2vec, norm=norm)
-    x_s = overlap(list1, list2, s, index2word, word2vec, norm=norm)
+    x_l = overlap(list1, list2, l, index2word, embedding_space=embedding_space, norm=norm)
+    x_s = overlap(list1, list2, s, index2word, embedding_space=embedding_space, norm=norm)
     # the paper says overlap(..., d) / d, but it should be replaced by
     # agreement(..., d) defined as per equation (28) so that ties are handled
     # properly (otherwise values > 1 will be returned)
     # sum1 = sum(p**d * overlap(list1, list2, d)[0] / d for d in range(1, l + 1))
-    sum1 = sum(p ** d * agreement(list1, list2, d, index2word=index2word, word2vec=word2vec, norm=norm)
+    sum1 = sum(p ** d * agreement(list1, list2, d, index2word=index2word, embedding_space=embedding_space, norm=norm)
                for d in range(1, l + 1))
     sum2 = sum(p ** d * x_s * (d - s) / s / d for d in range(s + 1, l + 1))
     term1 = (1 - p) / p * (sum1 + sum2)
     term2 = p ** l * ((x_l - x_s) / l + x_s / s)
     return term1 + term2
 
 
-def word_embeddings_rbo(list1, list2, p, index2word, word2vec, norm):
+def word_embeddings_rbo(list1, list2, p, index2word, embedding_space, norm):
     """Complete RBO analysis (lower bound, residual, point estimate).
     ``list`` arguments should be already correctly sorted iterables and each
     item should either be an atomic value or a set of values tied for that
     rank. ``p`` is the probability of looking for overlap at rank k + 1 after
     having examined rank k.
     RBO(min=0.489, res=0.477, ext=0.967)
     """
     if not 0 <= p <= 1:
         raise ValueError("The ``p`` parameter must be between 0 and 1.")
-    args = (list1, list2, p, index2word, word2vec, norm)
+    args = (list1, list2, p, index2word, embedding_space, norm)
 
     return RBO(rbo_min(*args), rbo_res(*args), rbo_ext(*args))
 
 
 def sort_dict(dct, *, ascending=False):
     """Sort keys in ``dct`` according to their corresponding values.
     Sorts in descending order by default, because the values are
@@ -179,21 +175,21 @@
                 items[i] = {existing_item, item}
         else:
             scores.insert(i, score)
             items.insert(i, item)
     return items
 
 
-def rbo_dict(dict1, dict2, p, index2word, word2vec, norm, *, sort_ascending=False):
+def rbo_dict(dict1, dict2, p, index2word, embedding_space, norm, *, sort_ascending=False):
     """Wrapper around ``rbo()`` for dict input.
     Each dict maps items to be sorted to the score according to which
     they should be sorted. The RBO analysis is then performed on the
     resulting sorted lists.
     The sort is descending by default, because scores are typically the
     higher the better, but this can be overridden by specifying
     ``sort_ascending=True``.
     """
     list1, list2 = (
         sort_dict(dict1, ascending=sort_ascending),
         sort_dict(dict2, ascending=sort_ascending),
     )
-    return word_embeddings_rbo(list1, list2, p, index2word, word2vec, norm)
+    return word_embeddings_rbo(list1, list2, p, index2word, embedding_space, norm)
```

### Comparing `octis-1.8.3/octis/evaluation_metrics/coherence_metrics.py` & `octis-1.9.0/octis/evaluation_metrics/coherence_metrics.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/evaluation_metrics/metrics.py` & `octis-1.9.0/octis/evaluation_metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/evaluation_metrics/rbo.py` & `octis-1.9.0/octis/evaluation_metrics/rbo.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/evaluation_metrics/classification_metrics.py` & `octis-1.9.0/octis/evaluation_metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/dataset/downloader.py` & `octis-1.9.0/octis/dataset/downloader.py`

 * *Files identical despite different names*

### Comparing `octis-1.8.3/octis/dataset/dataset.py` & `octis-1.9.0/octis/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import codecs
 import json
 import pickle
 from os.path import join, exists
 from pathlib import Path
 
 import pandas as pd
-from werkzeug.utils import header_property
 
 from octis.dataset.downloader import get_data_home, _pkl_filepath, download_dataset
 
 
 class Dataset:
     """
     Dataset handles a dataset and offers methods to access, save and edit the dataset data
@@ -212,15 +211,15 @@
         Parameters
         ----------
         file_name : name of the file to write
         -------
         """
         data = self.get_vocabulary()
         if data is not None:
-            with open(file_name, 'w') as outfile:
+            with open(file_name, 'w', encoding='utf8') as outfile:
                 for word in data:
                     outfile.write(word + "\n")
         else:
             raise Exception("error in saving vocabulary")
 
     def _save_document_indexes(self, file_name):
         """
@@ -265,20 +264,20 @@
             with open(file_name, 'r') as indexes_file:
                 for line in indexes_file:
                     document_indexes.append(line.strip())
             self.__original_indexes = document_indexes
         else:
             raise Exception("error in loading vocabulary")
 
-    def save(self, path):
+    def save(self, path, multilabel=False):
         """
         Saves all the dataset info in a folder
         Parameters
         ----------
-        path : path to the folder in wich files are saved.
+        path : path to the folder in which files are saved.
                If the folder doesn't exist it will be created
         """
         Path(path).mkdir(parents=True, exist_ok=True)
         try:
             partitions = self.get_partitioned_corpus()
             corpus, partition = [], []
             for i, p in enumerate(partitions):
@@ -292,15 +291,18 @@
                 for doc in p:
                     corpus.append(' '.join(doc))
                     partition.append(part)
 
             df = pd.DataFrame(data=corpus)
             df = pd.concat([df, pd.DataFrame(partition)], axis=1)
 
-            labs = [' '.join(lab) for lab in self.__labels]
+            if multilabel:
+                labs = [' '.join(lab) for lab in self.__labels]
+            else:
+                labs = self.__labels
             if self.__labels:
                 df = pd.concat([df, pd.DataFrame(labs)], axis=1)
             df.to_csv(path + '/corpus.tsv', sep='\t', index=False, header=False)
 
             self._save_vocabulary(path + "/vocabulary.txt")
             self._save_metadata(path + "/metadata.json")
             self._save_document_indexes(path + "/indexes.txt")
```

