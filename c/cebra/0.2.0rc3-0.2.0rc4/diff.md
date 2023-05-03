# Comparing `tmp/cebra-0.2.0rc3.tar.gz` & `tmp/cebra-0.2.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cebra-0.2.0rc3.tar", last modified: Mon May  1 23:42:05 2023, max compression
+gzip compressed data, was "cebra-0.2.0rc4.tar", last modified: Wed May  3 18:27:54 2023, max compression
```

## Comparing `cebra-0.2.0rc3.tar` & `cebra-0.2.0rc4.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.495751 cebra-0.2.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-01 23:42:05.495751 cebra-0.2.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.487751 cebra-0.2.0rc3/cebra/
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.487751 cebra-0.2.0rc3/cebra/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16008 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    25366 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/multi_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/data/single_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.487751 cebra-0.2.0rc3/cebra/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.491751 cebra-0.2.0rc3/cebra/datasets/allen/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/ca_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/ca_movie_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/combined.py
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/make_neuropixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/neuropixel_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/neuropixel_movie_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/allen/single_session_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/gaussian_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/generate_synthetic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/hippocampus.py
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/make_neuropixel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/monkey_reaching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/poisson.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/datasets/save_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.491751 cebra-0.2.0rc3/cebra/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9935 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/distributions/multisession.py
--rw-r--r--   0 runner    (1001) docker     (123)    21964 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.491751 cebra-0.2.0rc3/cebra/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/deeplabcut.py
--rw-r--r--   0 runner    (1001) docker     (123)    46689 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/matplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.491751 cebra-0.2.0rc3/cebra/integrations/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55181 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/cebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/integrations/sklearn/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.491751 cebra-0.2.0rc3/cebra/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/models/criterions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27878 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/models/multiobjective.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/models/projector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.495751 cebra-0.2.0rc3/cebra/solver/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/solver/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/solver/multi_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/solver/single_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/solver/supervised.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/cebra/solver/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.487751 cebra-0.2.0rc3/cebra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-01 23:42:05.000000 cebra-0.2.0rc3/cebra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-01 23:42:05.000000 cebra-0.2.0rc3/cebra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:42:05.000000 cebra-0.2.0rc3/cebra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-01 23:42:05.000000 cebra-0.2.0rc3/cebra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 23:42:05.000000 cebra-0.2.0rc3/cebra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15768 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-01 23:42:05.495751 cebra-0.2.0rc3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:42:05.495751 cebra-0.2.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_criterions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_data_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_dlc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_integration_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    23949 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    29031 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_sklearn_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-01 23:41:55.000000 cebra-0.2.0rc3/tests/test_usecases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:27:54.212710 cebra-0.2.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-03 18:27:54.212710 cebra-0.2.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:27:54.204710 cebra-0.2.0rc4/cebra/
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:27:54.204710 cebra-0.2.0rc4/cebra/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/data/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16008 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/data/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25366 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/data/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/data/multi_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/data/single_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:27:54.204710 cebra-0.2.0rc4/cebra/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:27:54.208711 cebra-0.2.0rc4/cebra/datasets/allen/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/allen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/allen/ca_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/allen/ca_movie_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/allen/combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/allen/make_neuropixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/allen/neuropixel_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/allen/neuropixel_movie_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/allen/single_session_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/gaussian_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/generate_synthetic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/hippocampus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/make_neuropixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/monkey_reaching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/datasets/save_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:27:54.208711 cebra-0.2.0rc4/cebra/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/distributions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/distributions/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/distributions/mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9935 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/distributions/multisession.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21964 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:27:54.208711 cebra-0.2.0rc4/cebra/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/integrations/deeplabcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46689 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/integrations/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:27:54.208711 cebra-0.2.0rc4/cebra/integrations/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/integrations/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55181 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/integrations/sklearn/cebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/integrations/sklearn/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/integrations/sklearn/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/integrations/sklearn/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/integrations/sklearn/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/integrations/sklearn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:27:54.208711 cebra-0.2.0rc4/cebra/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/models/criterions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28714 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/models/multiobjective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/models/projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:27:54.208711 cebra-0.2.0rc4/cebra/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/solver/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/solver/multi_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/solver/single_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/solver/supervised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/cebra/solver/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:27:54.204710 cebra-0.2.0rc4/cebra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-03 18:27:54.000000 cebra-0.2.0rc4/cebra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-03 18:27:54.000000 cebra-0.2.0rc4/cebra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:27:54.000000 cebra-0.2.0rc4/cebra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-03 18:27:54.000000 cebra-0.2.0rc4/cebra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 18:27:54.000000 cebra-0.2.0rc4/cebra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15768 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-03 18:27:54.212710 cebra-0.2.0rc4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:27:54.212710 cebra-0.2.0rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_criterions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_data_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_dlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_integration_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23949 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29031 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_sklearn_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-03 18:27:46.000000 cebra-0.2.0rc4/tests/test_usecases.py
```

### Comparing `cebra-0.2.0rc3/LICENSE.md` & `cebra-0.2.0rc4/LICENSE.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     Any IMPROVEMENTS must remain open source with a copy of this license. The terms "academic, non-commercial", as used
     in this Agreement, mean academic or other scholarly research which (a) is not undertaken for profit, or (b) is not 
     intended to produce works, services, or data for commercial use, or (c) is neither conducted, nor funded, by a person
     or an entity engaged in the commercial use, application or exploitation of works similar to the PROGRAM.
 
 5.	LICENSEE agrees that they shall credit the use of CEBRA with an appropriate citation: 
     Steffen Schneider, Jin H. Lee, Mackenzie Weygandt Mathis. Learnable latent embeddings for joint behavioral 
-    and neural analysis. Nature 2023 doi: _pending_.
+    and neural analysis. Nature 2023 doi: https://doi.org/10.1038/s41586-023-06031-6.
 
 6.	Ownership of all rights, including copyright in the PROGRAM and in any material associated therewith, shall at all times
    remain with LICENSOR and LICENSEE agrees to preserve the same. LICENSEE agrees not to use any portion of the PROGRAM or 
    of any IMPROVEMENTS in any machine-readable form outside the PROGRAM, nor to make any copies except for its internal use, 
    without prior written consent of LICENSOR. LICENSEE agrees to maintain this license file with the source code and place the
    following copyright notice on any such copies:
```

### Comparing `cebra-0.2.0rc3/PKG-INFO` & `cebra-0.2.0rc4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cebra
-Version: 0.2.0rc3
+Version: 0.2.0rc4
 Summary: Consistent Embeddings of high-dimensional Recordings using Auxiliary variables
 Home-page: https://github.com/AdaptiveMotorControlLab/CEBRA
 Author: Steffen Schneider, Jin H Lee, Mackenzie W Mathis
 Author-email: stes@hey.com
 Project-URL: Bug Tracker, https://github.com/AdaptiveMotorControlLab/CEBRA/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -38,31 +38,35 @@
 [🪲 Reporting Issues](https://github.com/AdaptiveMotorControlLab/CEBRA) 
 
 
 [![Downloads](https://static.pepy.tech/badge/cebra)](https://pepy.tech/project/cebra)
 [![Downloads](https://static.pepy.tech/badge/cebra/month)](https://pepy.tech/project/cebra)
 [![PyPI version](https://badge.fury.io/py/cebra.svg)](https://badge.fury.io/py/cebra)
 ![License: Non-Commercial](https://img.shields.io/badge/License-Non--commercial-lightgrey)
-![Codecov](https://img.shields.io/codecov/c/github/AdaptiveMotorControlLab/CEBRA)
 [![Twitter Follow](https://img.shields.io/twitter/follow/CEBRAAI.svg?label=CEBRAai&style=social)](https://twitter.com/CEBRAAI)
 
 
 
 </div>
 
 # Welcome! 👋
 
-CEBRA is a library for estimating **C**onsistent **E**m**B**eddings of high-dimensional **R**ecordings using **A**uxiliary variables. It contains self-supervised learning algorithms implemented in PyTorch, and has support for a variety of different datasets common in biology and neuroscience.
+**CEBRA** is a library for estimating **C**onsistent **E**m**B**eddings of high-dimensional **R**ecordings using **A**uxiliary variables. It contains self-supervised learning algorithms implemented in PyTorch, and has support for a variety of different datasets common in biology and neuroscience.
 
 To receive updates on code releases, please 👀 watch or ⭐️ star this repository!
 
 ``cebra`` is a self-supervised method for non-linear clustering that allows for label-informed time series analysis. 
 It can jointly use behavioral and neural data in a hypothesis- or discovery-driven manner to produce consistent, high-performance latent spaces. While it is not specific to neural and behavioral data, this is the first domain we used the tool in. This application case is to obtain a consistent representation of latent variables driving activity and behavior, improving decoding accuracy of behavioral variables over standard supervised learning, and obtaining embeddings which are robust to domain shifts.
 
 
 # Reference 
-- 📄 **Preprint**:
+
+- 📄 **Publication May 2023**:
+  [Learnable latent embeddings for joint behavioural and neural analysis.](https://doi.org/10.1038/s41586-023-06031-6)
+  Steffen Schneider*, Jin Hwa Lee* and Mackenzie Weygandt Mathis. Nature 2023.
+  
+- 📄 **Preprint April 2022**:
   [Learnable latent embeddings for joint behavioral and neural analysis.](https://arxiv.org/abs/2204.00673)
   Steffen Schneider*, Jin Hwa Lee* and Mackenzie Weygandt Mathis
   
  # License
--  CEBRA is released for academic use only (please read the license file). If this license is not appropriate for your application, please contact Prof. Mackenzie W. Mathis (mackenzie@post.harvard.edu) and/or the TTO office at EPFL (tto@epfl.ch) for a commercial use license.
+-  CEBRA is released for academic use only (please read the license file). If this license is not appropriate for your application, please contact Prof. Mackenzie W. Mathis (mackenzie@post.harvard.edu) for a commercial use license.
```

### Comparing `cebra-0.2.0rc3/README.md` & `cebra-0.2.0rc4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,31 +14,35 @@
 [🪲 Reporting Issues](https://github.com/AdaptiveMotorControlLab/CEBRA) 
 
 
 [![Downloads](https://static.pepy.tech/badge/cebra)](https://pepy.tech/project/cebra)
 [![Downloads](https://static.pepy.tech/badge/cebra/month)](https://pepy.tech/project/cebra)
 [![PyPI version](https://badge.fury.io/py/cebra.svg)](https://badge.fury.io/py/cebra)
 ![License: Non-Commercial](https://img.shields.io/badge/License-Non--commercial-lightgrey)
-![Codecov](https://img.shields.io/codecov/c/github/AdaptiveMotorControlLab/CEBRA)
 [![Twitter Follow](https://img.shields.io/twitter/follow/CEBRAAI.svg?label=CEBRAai&style=social)](https://twitter.com/CEBRAAI)
 
 
 
 </div>
 
 # Welcome! 👋
 
-CEBRA is a library for estimating **C**onsistent **E**m**B**eddings of high-dimensional **R**ecordings using **A**uxiliary variables. It contains self-supervised learning algorithms implemented in PyTorch, and has support for a variety of different datasets common in biology and neuroscience.
+**CEBRA** is a library for estimating **C**onsistent **E**m**B**eddings of high-dimensional **R**ecordings using **A**uxiliary variables. It contains self-supervised learning algorithms implemented in PyTorch, and has support for a variety of different datasets common in biology and neuroscience.
 
 To receive updates on code releases, please 👀 watch or ⭐️ star this repository!
 
 ``cebra`` is a self-supervised method for non-linear clustering that allows for label-informed time series analysis. 
 It can jointly use behavioral and neural data in a hypothesis- or discovery-driven manner to produce consistent, high-performance latent spaces. While it is not specific to neural and behavioral data, this is the first domain we used the tool in. This application case is to obtain a consistent representation of latent variables driving activity and behavior, improving decoding accuracy of behavioral variables over standard supervised learning, and obtaining embeddings which are robust to domain shifts.
 
 
 # Reference 
-- 📄 **Preprint**:
+
+- 📄 **Publication May 2023**:
+  [Learnable latent embeddings for joint behavioural and neural analysis.](https://doi.org/10.1038/s41586-023-06031-6)
+  Steffen Schneider*, Jin Hwa Lee* and Mackenzie Weygandt Mathis. Nature 2023.
+  
+- 📄 **Preprint April 2022**:
   [Learnable latent embeddings for joint behavioral and neural analysis.](https://arxiv.org/abs/2204.00673)
   Steffen Schneider*, Jin Hwa Lee* and Mackenzie Weygandt Mathis
   
  # License
--  CEBRA is released for academic use only (please read the license file). If this license is not appropriate for your application, please contact Prof. Mackenzie W. Mathis (mackenzie@post.harvard.edu) and/or the TTO office at EPFL (tto@epfl.ch) for a commercial use license.
+-  CEBRA is released for academic use only (please read the license file). If this license is not appropriate for your application, please contact Prof. Mackenzie W. Mathis (mackenzie@post.harvard.edu) for a commercial use license.
```

### Comparing `cebra-0.2.0rc3/cebra/__init__.py` & `cebra-0.2.0rc4/cebra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     from cebra.integrations.deeplabcut import load_deeplabcut
     is_load_deeplabcut_available = True
 except (ImportError, NameError):
     pass
 
 import cebra.integrations.sklearn as sklearn
 
-__version__ = "0.2.0rc3"
+__version__ = "0.2.0rc4"
 __all__ = ["CEBRA"]
 __allow_lazy_imports = False
 __lazy_imports = {}
 
 
 def allow_lazy_imports():
     """Enables lazy imports of all submodules and packages of cebra.
```

### Comparing `cebra-0.2.0rc3/cebra/__main__.py` & `cebra-0.2.0rc4/cebra/__main__.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/config.py` & `cebra-0.2.0rc4/cebra/config.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/data/__init__.py` & `cebra-0.2.0rc4/cebra/data/__init__.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/data/base.py` & `cebra-0.2.0rc4/cebra/data/base.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/data/datasets.py` & `cebra-0.2.0rc4/cebra/data/datasets.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/data/datatypes.py` & `cebra-0.2.0rc4/cebra/data/datatypes.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/data/helper.py` & `cebra-0.2.0rc4/cebra/data/helper.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/data/load.py` & `cebra-0.2.0rc4/cebra/data/load.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/data/multi_session.py` & `cebra-0.2.0rc4/cebra/data/multi_session.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/data/single_session.py` & `cebra-0.2.0rc4/cebra/data/single_session.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/__init__.py` & `cebra-0.2.0rc4/cebra/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/allen/__init__.py` & `cebra-0.2.0rc4/cebra/datasets/allen/__init__.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/allen/ca_movie.py` & `cebra-0.2.0rc4/cebra/datasets/allen/ca_movie.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/allen/ca_movie_decoding.py` & `cebra-0.2.0rc4/cebra/datasets/allen/ca_movie_decoding.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/allen/combined.py` & `cebra-0.2.0rc4/cebra/datasets/allen/combined.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/allen/make_neuropixel.py` & `cebra-0.2.0rc4/cebra/datasets/allen/make_neuropixel.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/allen/neuropixel_movie.py` & `cebra-0.2.0rc4/cebra/datasets/allen/neuropixel_movie.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/allen/neuropixel_movie_decoding.py` & `cebra-0.2.0rc4/cebra/datasets/allen/neuropixel_movie_decoding.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/allen/single_session_ca.py` & `cebra-0.2.0rc4/cebra/datasets/allen/single_session_ca.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/demo.py` & `cebra-0.2.0rc4/cebra/datasets/demo.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/gaussian_mixture.py` & `cebra-0.2.0rc4/cebra/datasets/gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/generate_synthetic_data.py` & `cebra-0.2.0rc4/cebra/datasets/generate_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/hippocampus.py` & `cebra-0.2.0rc4/cebra/datasets/hippocampus.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/make_neuropixel.py` & `cebra-0.2.0rc4/cebra/datasets/make_neuropixel.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/monkey_reaching.py` & `cebra-0.2.0rc4/cebra/datasets/monkey_reaching.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/poisson.py` & `cebra-0.2.0rc4/cebra/datasets/poisson.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/datasets/save_dataset.py` & `cebra-0.2.0rc4/cebra/datasets/save_dataset.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/distributions/__init__.py` & `cebra-0.2.0rc4/cebra/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/distributions/base.py` & `cebra-0.2.0rc4/cebra/distributions/base.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/distributions/continuous.py` & `cebra-0.2.0rc4/cebra/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/distributions/discrete.py` & `cebra-0.2.0rc4/cebra/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/distributions/index.py` & `cebra-0.2.0rc4/cebra/distributions/index.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/distributions/mixed.py` & `cebra-0.2.0rc4/cebra/distributions/mixed.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/distributions/multisession.py` & `cebra-0.2.0rc4/cebra/distributions/multisession.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/grid_search.py` & `cebra-0.2.0rc4/cebra/grid_search.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/helper.py` & `cebra-0.2.0rc4/cebra/helper.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/integrations/__init__.py` & `cebra-0.2.0rc4/cebra/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/integrations/deeplabcut.py` & `cebra-0.2.0rc4/cebra/integrations/deeplabcut.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/integrations/matplotlib.py` & `cebra-0.2.0rc4/cebra/integrations/matplotlib.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/integrations/sklearn/__init__.py` & `cebra-0.2.0rc4/cebra/integrations/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/integrations/sklearn/cebra.py` & `cebra-0.2.0rc4/cebra/integrations/sklearn/cebra.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/integrations/sklearn/dataset.py` & `cebra-0.2.0rc4/cebra/integrations/sklearn/dataset.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/integrations/sklearn/decoder.py` & `cebra-0.2.0rc4/cebra/integrations/sklearn/decoder.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/integrations/sklearn/helpers.py` & `cebra-0.2.0rc4/cebra/integrations/sklearn/helpers.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/integrations/sklearn/metrics.py` & `cebra-0.2.0rc4/cebra/integrations/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/integrations/sklearn/utils.py` & `cebra-0.2.0rc4/cebra/integrations/sklearn/utils.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/io.py` & `cebra-0.2.0rc4/cebra/io.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/models/__init__.py` & `cebra-0.2.0rc4/cebra/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/models/criterions.py` & `cebra-0.2.0rc4/cebra/models/criterions.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/models/layers.py` & `cebra-0.2.0rc4/cebra/models/layers.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/models/model.py` & `cebra-0.2.0rc4/cebra/models/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,39 @@
 
 import cebra.data
 import cebra.data.datatypes
 import cebra.models.layers as cebra_layers
 from cebra.models import register
 
 
+def _check_torch_version(raise_error=False):
+    current_version = tuple(
+        [int(i) for i in torch.__version__.split(".")[:2] if len(i) > 0])
+    required_version = (1, 12)
+    if current_version < required_version:
+        if raise_error:
+            raise ImportError(
+                f"PyTorch < 1.12 is not supported for models using "
+                f"Dropout1D, but got PyTorch={torch.__version__}.")
+        else:
+            return False
+    return True
+
+
+def _register_conditionally(*args, **kwargs):
+    if _check_torch_version(raise_error=False):
+        return register(*args, **kwargs)
+    else:
+
+        def do_nothing(cls):
+            return cls
+
+        return do_nothing
+
+
 class Model(nn.Module):
     """Base model for CEBRA experiments.
 
     The model is a pytorch ``nn.Module``. Features can be computed by
     calling the ``forward()`` or ``__call__`` method. This class should not be
     directly instantiated, and instead used as the base class for CEBRA
     models.
@@ -665,17 +690,21 @@
         )
 
     def get_offset(self) -> cebra.data.datatypes.Offset:
         """See `:py:meth:Model.get_offset`"""
         return cebra.data.Offset(18, 18)
 
 
-@register("offset36-model-dropout")
+@_register_conditionally("offset36-model-dropout")
 class Offset36Dropout(_OffsetModel, ConvolutionalModelMixin):
-    """CEBRA model with a 10 sample receptive field."""
+    """CEBRA model with a 10 sample receptive field.
+    
+    Note:
+        Requires ``torch>=1.12``.
+    """
 
     def __init__(self, num_neurons, num_units, num_output, normalize=True):
         if num_units < 1:
             raise ValueError(
                 f"Hidden dimension needs to be at least 1, but got {num_units}."
             )
         super().__init__(
@@ -705,17 +734,21 @@
         )
 
     def get_offset(self) -> cebra.data.datatypes.Offset:
         """See `:py:meth:Model.get_offset`"""
         return cebra.data.Offset(18, 18)
 
 
-@register("offset36-model-more-dropout")
+@_register_conditionally("offset36-model-more-dropout")
 class Offset36Dropoutv2(_OffsetModel, ConvolutionalModelMixin):
-    """CEBRA model with a 10 sample receptive field."""
+    """CEBRA model with a 10 sample receptive field.
+    
+    Note:
+        Requires ``torch>=1.12``.
+    """
 
     def _make_layers(self, num_units, p, n):
         return [
             cebra_layers._Skip(torch.nn.Dropout1d(p=p),
                                nn.Conv1d(num_units, num_units, 3), nn.GELU())
             for _ in range(n)
         ]
```

### Comparing `cebra-0.2.0rc3/cebra/models/multiobjective.py` & `cebra-0.2.0rc4/cebra/models/multiobjective.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/models/projector.py` & `cebra-0.2.0rc4/cebra/models/projector.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/registry.py` & `cebra-0.2.0rc4/cebra/registry.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/solver/__init__.py` & `cebra-0.2.0rc4/cebra/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/solver/base.py` & `cebra-0.2.0rc4/cebra/solver/base.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/solver/multi_session.py` & `cebra-0.2.0rc4/cebra/solver/multi_session.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/solver/single_session.py` & `cebra-0.2.0rc4/cebra/solver/single_session.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/solver/supervised.py` & `cebra-0.2.0rc4/cebra/solver/supervised.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra/solver/util.py` & `cebra-0.2.0rc4/cebra/solver/util.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra.egg-info/PKG-INFO` & `cebra-0.2.0rc4/cebra.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cebra
-Version: 0.2.0rc3
+Version: 0.2.0rc4
 Summary: Consistent Embeddings of high-dimensional Recordings using Auxiliary variables
 Home-page: https://github.com/AdaptiveMotorControlLab/CEBRA
 Author: Steffen Schneider, Jin H Lee, Mackenzie W Mathis
 Author-email: stes@hey.com
 Project-URL: Bug Tracker, https://github.com/AdaptiveMotorControlLab/CEBRA/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -38,31 +38,35 @@
 [🪲 Reporting Issues](https://github.com/AdaptiveMotorControlLab/CEBRA) 
 
 
 [![Downloads](https://static.pepy.tech/badge/cebra)](https://pepy.tech/project/cebra)
 [![Downloads](https://static.pepy.tech/badge/cebra/month)](https://pepy.tech/project/cebra)
 [![PyPI version](https://badge.fury.io/py/cebra.svg)](https://badge.fury.io/py/cebra)
 ![License: Non-Commercial](https://img.shields.io/badge/License-Non--commercial-lightgrey)
-![Codecov](https://img.shields.io/codecov/c/github/AdaptiveMotorControlLab/CEBRA)
 [![Twitter Follow](https://img.shields.io/twitter/follow/CEBRAAI.svg?label=CEBRAai&style=social)](https://twitter.com/CEBRAAI)
 
 
 
 </div>
 
 # Welcome! 👋
 
-CEBRA is a library for estimating **C**onsistent **E**m**B**eddings of high-dimensional **R**ecordings using **A**uxiliary variables. It contains self-supervised learning algorithms implemented in PyTorch, and has support for a variety of different datasets common in biology and neuroscience.
+**CEBRA** is a library for estimating **C**onsistent **E**m**B**eddings of high-dimensional **R**ecordings using **A**uxiliary variables. It contains self-supervised learning algorithms implemented in PyTorch, and has support for a variety of different datasets common in biology and neuroscience.
 
 To receive updates on code releases, please 👀 watch or ⭐️ star this repository!
 
 ``cebra`` is a self-supervised method for non-linear clustering that allows for label-informed time series analysis. 
 It can jointly use behavioral and neural data in a hypothesis- or discovery-driven manner to produce consistent, high-performance latent spaces. While it is not specific to neural and behavioral data, this is the first domain we used the tool in. This application case is to obtain a consistent representation of latent variables driving activity and behavior, improving decoding accuracy of behavioral variables over standard supervised learning, and obtaining embeddings which are robust to domain shifts.
 
 
 # Reference 
-- 📄 **Preprint**:
+
+- 📄 **Publication May 2023**:
+  [Learnable latent embeddings for joint behavioural and neural analysis.](https://doi.org/10.1038/s41586-023-06031-6)
+  Steffen Schneider*, Jin Hwa Lee* and Mackenzie Weygandt Mathis. Nature 2023.
+  
+- 📄 **Preprint April 2022**:
   [Learnable latent embeddings for joint behavioral and neural analysis.](https://arxiv.org/abs/2204.00673)
   Steffen Schneider*, Jin Hwa Lee* and Mackenzie Weygandt Mathis
   
  # License
--  CEBRA is released for academic use only (please read the license file). If this license is not appropriate for your application, please contact Prof. Mackenzie W. Mathis (mackenzie@post.harvard.edu) and/or the TTO office at EPFL (tto@epfl.ch) for a commercial use license.
+-  CEBRA is released for academic use only (please read the license file). If this license is not appropriate for your application, please contact Prof. Mackenzie W. Mathis (mackenzie@post.harvard.edu) for a commercial use license.
```

### Comparing `cebra-0.2.0rc3/cebra.egg-info/SOURCES.txt` & `cebra-0.2.0rc4/cebra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/cebra.egg-info/requires.txt` & `cebra-0.2.0rc4/cebra.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 pytest-benchmark
 pytest-xdist
 pytest-timeout
 pytest-sphinx
 tables
 licenseheaders
 codespell
+cffconvert
 
 [docs]
 sphinx==5.3
 sphinx-gallery==0.10.1
 docutils
 pydata-sphinx-theme==0.9.0
 sphinx_autodoc_typehints==1.19
```

### Comparing `cebra-0.2.0rc3/pyproject.toml` & `cebra-0.2.0rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/setup.cfg` & `cebra-0.2.0rc4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 	pytest-benchmark
 	pytest-xdist
 	pytest-timeout
 	pytest-sphinx
 	tables
 	licenseheaders
 	codespell
+	cffconvert
 
 [bdist_wheel]
 universal = 1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `cebra-0.2.0rc3/tests/_util.py` & `cebra-0.2.0rc4/tests/_util.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_api.py` & `cebra-0.2.0rc4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_benchmark.py` & `cebra-0.2.0rc4/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_criterions.py` & `cebra-0.2.0rc4/tests/test_criterions.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_data_helper.py` & `cebra-0.2.0rc4/tests/test_data_helper.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_datasets.py` & `cebra-0.2.0rc4/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_demo.py` & `cebra-0.2.0rc4/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_distributions.py` & `cebra-0.2.0rc4/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_dlc.py` & `cebra-0.2.0rc4/tests/test_dlc.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_grid_search.py` & `cebra-0.2.0rc4/tests/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_integration_train.py` & `cebra-0.2.0rc4/tests/test_integration_train.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_io.py` & `cebra-0.2.0rc4/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_load.py` & `cebra-0.2.0rc4/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_loader.py` & `cebra-0.2.0rc4/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_models.py` & `cebra-0.2.0rc4/tests/test_models.py`

 * *Files 13% similar despite different names*

```diff
@@ -118,7 +118,36 @@
     assert second.shape == (5, 6)
     assert third.shape == (5, 10)
 
     first, second, third = multi_model_separate(x)
     assert first.shape == (5, 4)
     assert second.shape == (5, 2)
     assert third.shape == (5, 4)
+
+
+@pytest.mark.parametrize("version,raises", [
+    ["1.12", False],
+    ["2.", False],
+    ["2.0.0rc", False],
+    ["2.0", False],
+    ["2.5", False],
+    ["1.11.0rc1", True],
+    ["1.10", True],
+    ["1.2", True],
+    ["1.0", True],
+])
+def test_version_check(version, raises):
+
+    torch.__version__ = version
+    assert cebra.models.model._check_torch_version(
+        raise_error=False) == (not raises)
+    if raises:
+        with pytest.raises(ImportError):
+            cebra.models.model._check_torch_version(raise_error=True)
+
+
+def test_version_check():
+    raises = not cebra.models.model._check_torch_version(raise_error=False)
+    if raises:
+        assert len(cebra.models.get_options("*dropout*")) == 0
+    else:
+        assert len(cebra.models.get_options("*dropout*")) > 0
```

### Comparing `cebra-0.2.0rc3/tests/test_plot.py` & `cebra-0.2.0rc4/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_registry.py` & `cebra-0.2.0rc4/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_sklearn.py` & `cebra-0.2.0rc4/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_sklearn_decoder.py` & `cebra-0.2.0rc4/tests/test_sklearn_decoder.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_sklearn_metrics.py` & `cebra-0.2.0rc4/tests/test_sklearn_metrics.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_solver.py` & `cebra-0.2.0rc4/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `cebra-0.2.0rc3/tests/test_usecases.py` & `cebra-0.2.0rc4/tests/test_usecases.py`

 * *Files identical despite different names*

