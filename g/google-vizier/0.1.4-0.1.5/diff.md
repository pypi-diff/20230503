# Comparing `tmp/google-vizier-0.1.4.tar.gz` & `tmp/google-vizier-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-vizier-0.1.4.tar", last modified: Mon Mar 13 23:07:06 2023, max compression
+gzip compressed data, was "google-vizier-0.1.5.tar", last modified: Tue May  2 21:57:00 2023, max compression
```

## Comparing `google-vizier-0.1.4.tar` & `google-vizier-0.1.5.tar`

### file list

```diff
@@ -1,301 +1,329 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.261183 google-vizier-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-13 23:06:42.000000 google-vizier-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-03-13 23:07:06.261183 google-vizier-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-03-13 23:06:42.000000 google-vizier-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.217183 google-vizier-0.1.4/google_vizier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-03-13 23:07:06.000000 google-vizier-0.1.4/google_vizier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-03-13 23:07:06.000000 google-vizier-0.1.4/google_vizier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 23:07:06.000000 google-vizier-0.1.4/google_vizier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 23:07:06.000000 google-vizier-0.1.4/google_vizier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-13 23:07:06.000000 google-vizier-0.1.4/google_vizier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-13 23:07:06.000000 google-vizier-0.1.4/google_vizier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 23:07:06.261183 google-vizier-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-03-13 23:06:42.000000 google-vizier-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.221183 google-vizier-0.1.4/vizier/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.221183 google-vizier-0.1.4/vizier/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.221183 google-vizier-0.1.4/vizier/_src/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.221183 google-vizier-0.1.4/vizier/_src/algorithms/classification/
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/classification/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/classification/classifiers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.221183 google-vizier-0.1.4/vizier/_src/algorithms/core/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/core/abstractions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.225183 google-vizier-0.1.4/vizier/_src/algorithms/designers/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19486 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/bocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/bocs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/cmaes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/cmaes_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.225183 google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19573 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/emukit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/emukit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.229183 google-vizier-0.1.4/vizier/_src/algorithms/designers/gp/
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/gp/acquisitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/gp/acquisitions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16305 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/gp/output_warpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/gp/output_warpers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/gp/yjt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/gp_bandit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/gp_bandit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/grid_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/harmonica.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/harmonica_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/quasi_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/quasi_random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/scalarizing_designer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/designers/scalarizing_designer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.229183 google-vizier-0.1.4/vizier/_src/algorithms/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/evolution/numpy_populations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/evolution/numpy_populations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/evolution/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.229183 google-vizier-0.1.4/vizier/_src/algorithms/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/optimizers/designer_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/optimizers/designer_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/optimizers/eagle_param_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26084 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/optimizers/eagle_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14671 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/optimizers/eagle_strategy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11595 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/optimizers/vectorized_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/optimizers/vectorized_base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.233183 google-vizier-0.1.4/vizier/_src/algorithms/policies/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14343 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/policies/designer_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/policies/designer_policy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/policies/random_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/policies/random_policy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.233183 google-vizier-0.1.4/vizier/_src/algorithms/random/
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/random/random_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/random/random_sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.233183 google-vizier-0.1.4/vizier/_src/algorithms/regression/
--rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/regression/trial_regression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/regression/trial_regression_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.233183 google-vizier-0.1.4/vizier/_src/algorithms/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/testing/comparator_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/testing/comparator_runner_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/testing/optimizer_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/algorithms/testing/test_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.213183 google-vizier-0.1.4/vizier/_src/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.233183 google-vizier-0.1.4/vizier/_src/benchmarks/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/analyzers/convergence_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/analyzers/convergence_curve_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/analyzers/simple_regret_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.237183 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.241183 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/combo/
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/combo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/combo_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/experimenter_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.241183 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/hpob/
--rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/hpob/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    25640 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/hpob_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/noisy_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/numpy_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/shifting_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/sparse_experimenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.241183 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/synthetic/
--rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/synthetic/bbob.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.241183 google-vizier-0.1.4/vizier/_src/benchmarks/runners/
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/runners/benchmark_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/runners/benchmark_runner_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/runners/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/benchmarks/runners/benchmark_state_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.241183 google-vizier-0.1.4/vizier/_src/jax/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.241183 google-vizier-0.1.4/vizier/_src/jax/models/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/jax/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/jax/models/gaussian_process_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/jax/models/gaussian_process_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/jax/models/hebo_gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/jax/models/hebo_gp_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/jax/models/tuned_gp_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/jax/models/tuned_gp_models_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.241183 google-vizier-0.1.4/vizier/_src/jax/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/jax/optimizers/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/jax/optimizers/optimizers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21813 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/jax/stochastic_process_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/jax/stochastic_process_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/jax/xla_pareto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/jax/xla_pareto_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.245183 google-vizier-0.1.4/vizier/_src/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyglove/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyglove/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyglove/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyglove/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyglove/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyglove/converters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyglove/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyglove/oss_vizier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyglove/oss_vizier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyglove/performance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyglove/pythia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyglove/pythia_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyglove/vizier_test_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.245183 google-vizier-0.1.4/vizier/_src/pythia/
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pythia/local_policy_supporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pythia/local_policy_supporters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pythia/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pythia/policy_supporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pythia/pythia_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.217183 google-vizier-0.1.4/vizier/_src/pyvizier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.249183 google-vizier-0.1.4/vizier/_src/pyvizier/multimetric/
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/multimetric/hypervolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/multimetric/hypervolume_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/multimetric/pareto_optimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/multimetric/safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/multimetric/safety_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.249183 google-vizier-0.1.4/vizier/_src/pyvizier/oss/
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/oss/automated_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/oss/automated_stopping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/oss/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/oss/metadata_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/oss/metadata_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    32414 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/oss/proto_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/oss/proto_converters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/oss/study_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    36444 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/oss/study_config_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.249183 google-vizier-0.1.4/vizier/_src/pyvizier/pythia/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/pythia/study.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/_src/pyvizier/shared/
--rw-r--r--   0 runner    (1001) docker     (123)    13005 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/shared/base_study_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/shared/base_study_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23687 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/shared/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/shared/common_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/shared/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/shared/context_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    46946 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/shared/parameter_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    23074 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/shared/parameter_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/shared/parameter_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/shared/parameter_iterators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/shared/study.py
--rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/shared/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/_src/pyvizier/shared/trial_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/algorithms/designers/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/algorithms/designers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/algorithms/policies/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/algorithms/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/benchmarks/experimenters/
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/benchmarks/experimenters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/benchmarks/experimenters/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/benchmarks/experimenters/hpo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/benchmarks/experimenters/nas/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/benchmarks/experimenters/nas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/benchmarks/experimenters/rl/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/benchmarks/experimenters/rl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/client/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/client/client_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/client/client_abc_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/interfaces/serializable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/jax/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/jax/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/jax/optimizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyglove/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyglove/pyglove_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pythia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.253183 google-vizier-0.1.4/vizier/pyvizier/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyvizier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.257183 google-vizier-0.1.4/vizier/pyvizier/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyvizier/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44111 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyvizier/converters/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    41131 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyvizier/converters/core_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyvizier/converters/embedder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyvizier/converters/embedder_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyvizier/converters/feature_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyvizier/converters/feature_mapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20165 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyvizier/converters/spatio_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyvizier/converters/spatio_temporal_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.257183 google-vizier-0.1.4/vizier/pyvizier/multimetric/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyvizier/multimetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/pyvizier/multimetric/xla_pareto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.261183 google-vizier-0.1.4/vizier/service/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8178 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/clients_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/custom_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23165 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/datastore_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/datastore_test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/grpc_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/performance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/policy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/pythia_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/pythia_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.261183 google-vizier-0.1.4/vizier/service/pyvizier/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/pyvizier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/resources_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/service_policy_supporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/service_policy_supporter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22376 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/sql_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/sql_datastore_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/stubs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/stubs_util_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.261183 google-vizier-0.1.4/vizier/service/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/testing/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    18455 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/vizier_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/vizier_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/vizier_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    36014 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/vizier_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/service/vizier_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.261183 google-vizier-0.1.4/vizier/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/testing/test_studies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 23:07:06.261183 google-vizier-0.1.4/vizier/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/utils/attrs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/utils/attrs_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-13 23:06:42.000000 google-vizier-0.1.4/vizier/utils/json_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.202545 google-vizier-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 21:56:38.000000 google-vizier-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-05-02 21:57:00.202545 google-vizier-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-05-02 21:56:38.000000 google-vizier-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/google_vizier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-05-02 21:57:00.000000 google-vizier-0.1.5/google_vizier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-05-02 21:57:00.000000 google-vizier-0.1.5/google_vizier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:57:00.000000 google-vizier-0.1.5/google_vizier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:57:00.000000 google-vizier-0.1.5/google_vizier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-02 21:57:00.000000 google-vizier-0.1.5/google_vizier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 21:57:00.000000 google-vizier-0.1.5/google_vizier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:57:00.202545 google-vizier-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-02 21:56:38.000000 google-vizier-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/_src/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/_src/algorithms/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/classification/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/classification/classifiers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/_src/algorithms/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/core/abstractions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.178544 google-vizier-0.1.5/vizier/_src/algorithms/designers/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19486 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/bocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/bocs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/cmaes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/cmaes_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.178544 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19573 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/emukit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/emukit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.178544 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)    20728 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/acquisitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/acquisitions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24111 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/output_warpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15369 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/output_warpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/yjt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17842 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/gp_bandit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/grid_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/harmonica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/harmonica_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/quasi_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/quasi_random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/scalarizing_designer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/designers/scalarizing_designer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.178544 google-vizier-0.1.5/vizier/_src/algorithms/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13712 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/evolution/numpy_populations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/evolution/numpy_populations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/evolution/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.182544 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/designer_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/designer_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_param_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27583 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_strategy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11522 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/vectorized_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/optimizers/vectorized_base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.182544 google-vizier-0.1.5/vizier/_src/algorithms/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/policies/designer_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/policies/designer_policy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/policies/random_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/policies/random_policy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.182544 google-vizier-0.1.5/vizier/_src/algorithms/random/
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/random/random_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/random/random_sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.182544 google-vizier-0.1.5/vizier/_src/algorithms/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/regression/trial_regression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/regression/trial_regression_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.182544 google-vizier-0.1.5/vizier/_src/algorithms/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/testing/comparator_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/testing/comparator_runner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/testing/optimizer_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/algorithms/testing/test_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/_src/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.182544 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/convergence_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/convergence_curve_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/simple_regret_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/state_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/state_analyzer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo/
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/experimenter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob/
+-rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25640 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/noisy_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/numpy_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/shifting_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sparse_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/surrogate_experimenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/synthetic/bbob.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/benchmarks/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_runner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_state_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/jax/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/jax/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/gaussian_process_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/gaussian_process_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/hebo_gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/hebo_gp_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/tuned_gp_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/models/tuned_gp_models_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.186544 google-vizier-0.1.5/vizier/_src/jax/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/optimizers/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/optimizers/optimizers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25862 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/stochastic_process_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19460 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/stochastic_process_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/xla_pareto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/jax/xla_pareto_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.190544 google-vizier-0.1.5/vizier/_src/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/e2e_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/oss_vizier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/oss_vizier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/pythia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/pythia_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyglove/vizier_test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.190544 google-vizier-0.1.5/vizier/_src/pythia/
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pythia/local_policy_supporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pythia/local_policy_supporters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pythia/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pythia/policy_supporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pythia/pythia_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.174544 google-vizier-0.1.5/vizier/_src/pyvizier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.190544 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/hypervolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/hypervolume_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/pareto_optimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/safety_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.190544 google-vizier-0.1.5/vizier/_src/pyvizier/oss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/automated_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/automated_stopping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/metadata_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/metadata_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32429 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/proto_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/proto_converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/study_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36459 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/oss/study_config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.190544 google-vizier-0.1.5/vizier/_src/pyvizier/pythia/
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/pythia/study.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.194544 google-vizier-0.1.5/vizier/_src/pyvizier/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/base_study_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/base_study_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23687 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/context_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47569 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23926 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_iterators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/study.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/pyvizier/shared/trial_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.194544 google-vizier-0.1.5/vizier/_src/raytune/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/raytune/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/raytune/converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/raytune/run_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/raytune/run_tune_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.194544 google-vizier-0.1.5/vizier/_src/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/clients_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/custom_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/datastore_test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/grpc_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/policy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/pythia_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/pythia_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15795 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/ram_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/ram_datastore_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/resources_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/service_policy_supporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/service_policy_supporter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22481 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/sql_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/sql_datastore_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/stubs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/stubs_util_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/_src/service/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/testing/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17372 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/vizier_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12258 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/vizier_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/vizier_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36086 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/vizier_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/_src/service/vizier_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/algorithms/designers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/algorithms/designers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/algorithms/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/algorithms/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/benchmarks/experimenters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/benchmarks/experimenters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/benchmarks/experimenters/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/benchmarks/experimenters/hpo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/benchmarks/experimenters/nas/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/benchmarks/experimenters/nas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/benchmarks/experimenters/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/benchmarks/experimenters/rl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/client/client_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15643 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/client/client_abc_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/interfaces/serializable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/jax/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/jax/optimizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyglove/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pythia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/pyvizier/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/pyvizier/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44581 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44020 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/core_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/embedder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/embedder_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/feature_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/feature_mapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/input_warping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/input_warping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20165 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/spatio_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/converters/spatio_temporal_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/pyvizier/multimetric/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/multimetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/pyvizier/multimetric/xla_pareto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/raytune/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/raytune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/service/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/service/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/service/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/service/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/service/pyvizier/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/service/pyvizier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/service/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/service/servers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.198544 google-vizier-0.1.5/vizier/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/testing/test_studies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:57:00.202545 google-vizier-0.1.5/vizier/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/utils/attrs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/utils/attrs_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/utils/json_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-05-02 21:56:38.000000 google-vizier-0.1.5/vizier/utils/profiler_test.py
```

### Comparing `google-vizier-0.1.4/LICENSE` & `google-vizier-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/PKG-INFO` & `google-vizier-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-vizier
-Version: 0.1.4
+Version: 0.1.5
 Summary: Open Source Vizier: Distributed service framework for blackbox optimization and research.
 Home-page: https://github.com/google/vizier
 Author: Vizier Team
 Author-email: oss-vizier-dev@google.com
 License: Apache License 2.0
 Keywords: ai machine learning hyperparameter blackbox optimization framework
 Classifier: Development Status :: 3 - Alpha
@@ -38,15 +38,15 @@
 ![Continuous Integration (Benchmarks)](https://github.com/google/vizier/workflows/pytest_benchmarks/badge.svg)
 ![Continuous Integration (Docs)](https://github.com/google/vizier/workflows/docs/badge.svg)
 
   [**Google AI Blog**](https://ai.googleblog.com/2023/02/open-source-vizier-towards-reliable-and.html)
 | [**Getting Started**](#getting_started)
 | [**Documentation**](#documentation)
 | [**Installation**](#installation)
-| [**Citing Vizier**](#citing_vizier)
+| [**Citing and Highlights**](#citing_vizier)
 
 ## What is Open Source (OSS) Vizier?
 [OSS Vizier](https://arxiv.org/abs/2207.13676) is a Python-based service for black-box optimization and research, based on [Google Vizier](https://dl.acm.org/doi/10.1145/3097983.3098043), one of the first hyperparameter tuning services designed to work at scale.
 
 <figure>
 <p align="center" width=65%>
 <img src="docs/assets/oss_vizier_service.gif"/>
@@ -129,16 +129,20 @@
 * `requirements-tf.txt`: Tensorflow libraries used by benchmarks.
 * `requirements-algorithms.txt`: Additional repositories (e.g. EvoJAX) for algorithms.
 * `requirements-benchmarks.txt`: Additional repositories (e.g. NASBENCH-201) for benchmarks.
 * `requirements-test.txt`: Libraries needed for testing code.
 
 Check if all unit tests work by running `run_tests.sh` after a full installation. OSS Vizier requires Python 3.10+, while client-only packages require Python 3.7+.
 
-## Citing Vizier <a name="citing_vizier"></a>
-If you found this code useful, please consider citing the [OSS Vizier paper](https://arxiv.org/abs/2207.13676) as well as the [Google Vizier paper](https://dl.acm.org/doi/10.1145/3097983.3098043). Thanks!
+## Citing and Highlights <a name="citing_vizier"></a>
+<ins>**Citing Vizier:**</ins> If you found this code useful, please consider citing the [OSS Vizier paper](https://arxiv.org/abs/2207.13676) as well as the [Google Vizier paper](https://dl.acm.org/doi/10.1145/3097983.3098043).
+
+<ins>**Highlights:**</ins> We track [notable users](https://oss-vizier.readthedocs.io/en/latest/highlights/applications.html) and [media attention](https://oss-vizier.readthedocs.io/en/latest/highlights/media.html) - let us know if OSS Vizier was helpful for your work.
+
+Thanks!
 
 ```
 @inproceedings{oss_vizier,
   author    = {Xingyou Song and
                Sagi Perel and
                Chansoo Lee and
                Greg Kochanski and
```

### Comparing `google-vizier-0.1.4/README.md` & `google-vizier-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ![Continuous Integration (Benchmarks)](https://github.com/google/vizier/workflows/pytest_benchmarks/badge.svg)
 ![Continuous Integration (Docs)](https://github.com/google/vizier/workflows/docs/badge.svg)
 
   [**Google AI Blog**](https://ai.googleblog.com/2023/02/open-source-vizier-towards-reliable-and.html)
 | [**Getting Started**](#getting_started)
 | [**Documentation**](#documentation)
 | [**Installation**](#installation)
-| [**Citing Vizier**](#citing_vizier)
+| [**Citing and Highlights**](#citing_vizier)
 
 ## What is Open Source (OSS) Vizier?
 [OSS Vizier](https://arxiv.org/abs/2207.13676) is a Python-based service for black-box optimization and research, based on [Google Vizier](https://dl.acm.org/doi/10.1145/3097983.3098043), one of the first hyperparameter tuning services designed to work at scale.
 
 <figure>
 <p align="center" width=65%>
 <img src="docs/assets/oss_vizier_service.gif"/>
@@ -101,16 +101,20 @@
 * `requirements-tf.txt`: Tensorflow libraries used by benchmarks.
 * `requirements-algorithms.txt`: Additional repositories (e.g. EvoJAX) for algorithms.
 * `requirements-benchmarks.txt`: Additional repositories (e.g. NASBENCH-201) for benchmarks.
 * `requirements-test.txt`: Libraries needed for testing code.
 
 Check if all unit tests work by running `run_tests.sh` after a full installation. OSS Vizier requires Python 3.10+, while client-only packages require Python 3.7+.
 
-## Citing Vizier <a name="citing_vizier"></a>
-If you found this code useful, please consider citing the [OSS Vizier paper](https://arxiv.org/abs/2207.13676) as well as the [Google Vizier paper](https://dl.acm.org/doi/10.1145/3097983.3098043). Thanks!
+## Citing and Highlights <a name="citing_vizier"></a>
+<ins>**Citing Vizier:**</ins> If you found this code useful, please consider citing the [OSS Vizier paper](https://arxiv.org/abs/2207.13676) as well as the [Google Vizier paper](https://dl.acm.org/doi/10.1145/3097983.3098043).
+
+<ins>**Highlights:**</ins> We track [notable users](https://oss-vizier.readthedocs.io/en/latest/highlights/applications.html) and [media attention](https://oss-vizier.readthedocs.io/en/latest/highlights/media.html) - let us know if OSS Vizier was helpful for your work.
+
+Thanks!
 
 ```
 @inproceedings{oss_vizier,
   author    = {Xingyou Song and
                Sagi Perel and
                Chansoo Lee and
                Greg Kochanski and
```

### Comparing `google-vizier-0.1.4/google_vizier.egg-info/PKG-INFO` & `google-vizier-0.1.5/google_vizier.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-vizier
-Version: 0.1.4
+Version: 0.1.5
 Summary: Open Source Vizier: Distributed service framework for blackbox optimization and research.
 Home-page: https://github.com/google/vizier
 Author: Vizier Team
 Author-email: oss-vizier-dev@google.com
 License: Apache License 2.0
 Keywords: ai machine learning hyperparameter blackbox optimization framework
 Classifier: Development Status :: 3 - Alpha
@@ -38,15 +38,15 @@
 ![Continuous Integration (Benchmarks)](https://github.com/google/vizier/workflows/pytest_benchmarks/badge.svg)
 ![Continuous Integration (Docs)](https://github.com/google/vizier/workflows/docs/badge.svg)
 
   [**Google AI Blog**](https://ai.googleblog.com/2023/02/open-source-vizier-towards-reliable-and.html)
 | [**Getting Started**](#getting_started)
 | [**Documentation**](#documentation)
 | [**Installation**](#installation)
-| [**Citing Vizier**](#citing_vizier)
+| [**Citing and Highlights**](#citing_vizier)
 
 ## What is Open Source (OSS) Vizier?
 [OSS Vizier](https://arxiv.org/abs/2207.13676) is a Python-based service for black-box optimization and research, based on [Google Vizier](https://dl.acm.org/doi/10.1145/3097983.3098043), one of the first hyperparameter tuning services designed to work at scale.
 
 <figure>
 <p align="center" width=65%>
 <img src="docs/assets/oss_vizier_service.gif"/>
@@ -129,16 +129,20 @@
 * `requirements-tf.txt`: Tensorflow libraries used by benchmarks.
 * `requirements-algorithms.txt`: Additional repositories (e.g. EvoJAX) for algorithms.
 * `requirements-benchmarks.txt`: Additional repositories (e.g. NASBENCH-201) for benchmarks.
 * `requirements-test.txt`: Libraries needed for testing code.
 
 Check if all unit tests work by running `run_tests.sh` after a full installation. OSS Vizier requires Python 3.10+, while client-only packages require Python 3.7+.
 
-## Citing Vizier <a name="citing_vizier"></a>
-If you found this code useful, please consider citing the [OSS Vizier paper](https://arxiv.org/abs/2207.13676) as well as the [Google Vizier paper](https://dl.acm.org/doi/10.1145/3097983.3098043). Thanks!
+## Citing and Highlights <a name="citing_vizier"></a>
+<ins>**Citing Vizier:**</ins> If you found this code useful, please consider citing the [OSS Vizier paper](https://arxiv.org/abs/2207.13676) as well as the [Google Vizier paper](https://dl.acm.org/doi/10.1145/3097983.3098043).
+
+<ins>**Highlights:**</ins> We track [notable users](https://oss-vizier.readthedocs.io/en/latest/highlights/applications.html) and [media attention](https://oss-vizier.readthedocs.io/en/latest/highlights/media.html) - let us know if OSS Vizier was helpful for your work.
+
+Thanks!
 
 ```
 @inproceedings{oss_vizier,
   author    = {Xingyou Song and
                Sagi Perel and
                Chansoo Lee and
                Greg Kochanski and
```

### Comparing `google-vizier-0.1.4/google_vizier.egg-info/SOURCES.txt` & `google-vizier-0.1.5/google_vizier.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 vizier/_src/algorithms/optimizers/base.py
 vizier/_src/algorithms/optimizers/designer_optimizer.py
 vizier/_src/algorithms/optimizers/designer_optimizer_test.py
 vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py
 vizier/_src/algorithms/optimizers/eagle_param_handler.py
 vizier/_src/algorithms/optimizers/eagle_strategy.py
 vizier/_src/algorithms/optimizers/eagle_strategy_test.py
+vizier/_src/algorithms/optimizers/lbfgsb_optimizer.py
+vizier/_src/algorithms/optimizers/lbfgsb_optimizer_test.py
 vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py
 vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py
 vizier/_src/algorithms/optimizers/vectorized_base.py
 vizier/_src/algorithms/optimizers/vectorized_base_test.py
 vizier/_src/algorithms/policies/__init__.py
 vizier/_src/algorithms/policies/designer_policy.py
 vizier/_src/algorithms/policies/designer_policy_test.py
@@ -79,27 +81,31 @@
 vizier/_src/algorithms/testing/comparator_runner_test.py
 vizier/_src/algorithms/testing/optimizer_test_utils.py
 vizier/_src/algorithms/testing/test_runners.py
 vizier/_src/benchmarks/analyzers/convergence_curve.py
 vizier/_src/benchmarks/analyzers/convergence_curve_test.py
 vizier/_src/benchmarks/analyzers/simple_regret_score.py
 vizier/_src/benchmarks/analyzers/simple_regret_score_test.py
+vizier/_src/benchmarks/analyzers/state_analyzer.py
+vizier/_src/benchmarks/analyzers/state_analyzer_test.py
 vizier/_src/benchmarks/experimenters/atari100k_experimenter.py
 vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py
 vizier/_src/benchmarks/experimenters/combo_experimenter.py
 vizier/_src/benchmarks/experimenters/combo_experimenter_test.py
 vizier/_src/benchmarks/experimenters/discretizing_experimenter.py
 vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py
 vizier/_src/benchmarks/experimenters/experimenter.py
 vizier/_src/benchmarks/experimenters/experimenter_factory.py
 vizier/_src/benchmarks/experimenters/experimenter_factory_test.py
 vizier/_src/benchmarks/experimenters/hpob_experimenter.py
 vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py
 vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py
 vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py
+vizier/_src/benchmarks/experimenters/multiobjective_experimenter.py
+vizier/_src/benchmarks/experimenters/multiobjective_experimenter_test.py
 vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py
 vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py
 vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py
 vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py
 vizier/_src/benchmarks/experimenters/noisy_experimenter.py
 vizier/_src/benchmarks/experimenters/noisy_experimenter_test.py
 vizier/_src/benchmarks/experimenters/normalizing_experimenter.py
@@ -108,23 +114,26 @@
 vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py
 vizier/_src/benchmarks/experimenters/shifting_experimenter.py
 vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py
 vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py
 vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py
 vizier/_src/benchmarks/experimenters/sparse_experimenter.py
 vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py
+vizier/_src/benchmarks/experimenters/surrogate_experimenter.py
+vizier/_src/benchmarks/experimenters/surrogate_experimenter_test.py
 vizier/_src/benchmarks/experimenters/combo/common.py
 vizier/_src/benchmarks/experimenters/hpob/handler.py
 vizier/_src/benchmarks/experimenters/synthetic/bbob.py
 vizier/_src/benchmarks/runners/benchmark_runner.py
 vizier/_src/benchmarks/runners/benchmark_runner_test.py
 vizier/_src/benchmarks/runners/benchmark_state.py
 vizier/_src/benchmarks/runners/benchmark_state_test.py
 vizier/_src/jax/stochastic_process_model.py
 vizier/_src/jax/stochastic_process_model_test.py
+vizier/_src/jax/types.py
 vizier/_src/jax/xla_pareto.py
 vizier/_src/jax/xla_pareto_test.py
 vizier/_src/jax/models/__init__.py
 vizier/_src/jax/models/gaussian_process_model.py
 vizier/_src/jax/models/gaussian_process_model_test.py
 vizier/_src/jax/models/hebo_gp_model.py
 vizier/_src/jax/models/hebo_gp_model_test.py
@@ -135,14 +144,15 @@
 vizier/_src/pyglove/algorithms.py
 vizier/_src/pyglove/backend.py
 vizier/_src/pyglove/client.py
 vizier/_src/pyglove/constants.py
 vizier/_src/pyglove/converters.py
 vizier/_src/pyglove/converters_test.py
 vizier/_src/pyglove/core.py
+vizier/_src/pyglove/e2e_test.py
 vizier/_src/pyglove/oss_vizier.py
 vizier/_src/pyglove/oss_vizier_test.py
 vizier/_src/pyglove/performance_test.py
 vizier/_src/pyglove/pythia.py
 vizier/_src/pyglove/pythia_test.py
 vizier/_src/pyglove/vizier_test_lib.py
 vizier/_src/pythia/local_policy_supporters.py
@@ -175,14 +185,46 @@
 vizier/_src/pyvizier/shared/parameter_config.py
 vizier/_src/pyvizier/shared/parameter_config_test.py
 vizier/_src/pyvizier/shared/parameter_iterators.py
 vizier/_src/pyvizier/shared/parameter_iterators_test.py
 vizier/_src/pyvizier/shared/study.py
 vizier/_src/pyvizier/shared/trial.py
 vizier/_src/pyvizier/shared/trial_test.py
+vizier/_src/raytune/converters.py
+vizier/_src/raytune/converters_test.py
+vizier/_src/raytune/run_tune.py
+vizier/_src/raytune/run_tune_test.py
+vizier/_src/service/clients.py
+vizier/_src/service/clients_test.py
+vizier/_src/service/constants.py
+vizier/_src/service/custom_errors.py
+vizier/_src/service/datastore.py
+vizier/_src/service/datastore_test_lib.py
+vizier/_src/service/grpc_util.py
+vizier/_src/service/performance_test.py
+vizier/_src/service/policy_factory.py
+vizier/_src/service/pythia_service.py
+vizier/_src/service/pythia_util.py
+vizier/_src/service/ram_datastore.py
+vizier/_src/service/ram_datastore_test.py
+vizier/_src/service/resources.py
+vizier/_src/service/resources_test.py
+vizier/_src/service/service_policy_supporter.py
+vizier/_src/service/service_policy_supporter_test.py
+vizier/_src/service/sql_datastore.py
+vizier/_src/service/sql_datastore_test.py
+vizier/_src/service/stubs_util.py
+vizier/_src/service/stubs_util_test.py
+vizier/_src/service/types.py
+vizier/_src/service/vizier_client.py
+vizier/_src/service/vizier_client_test.py
+vizier/_src/service/vizier_server.py
+vizier/_src/service/vizier_service.py
+vizier/_src/service/vizier_service_test.py
+vizier/_src/service/testing/util.py
 vizier/algorithms/__init__.py
 vizier/algorithms/designers/__init__.py
 vizier/algorithms/policies/__init__.py
 vizier/benchmarks/__init__.py
 vizier/benchmarks/experimenters/__init__.py
 vizier/benchmarks/experimenters/hpo/__init__.py
 vizier/benchmarks/experimenters/nas/__init__.py
@@ -192,55 +234,35 @@
 vizier/client/client_abc_testing.py
 vizier/interfaces/__init__.py
 vizier/interfaces/serializable.py
 vizier/jax/__init__.py
 vizier/jax/models.py
 vizier/jax/optimizers.py
 vizier/pyglove/__init__.py
-vizier/pyglove/pyglove_test.py
 vizier/pyvizier/__init__.py
 vizier/pyvizier/converters/__init__.py
 vizier/pyvizier/converters/core.py
 vizier/pyvizier/converters/core_test.py
 vizier/pyvizier/converters/embedder.py
 vizier/pyvizier/converters/embedder_test.py
 vizier/pyvizier/converters/feature_mapper.py
 vizier/pyvizier/converters/feature_mapper_test.py
+vizier/pyvizier/converters/input_warping.py
+vizier/pyvizier/converters/input_warping_test.py
 vizier/pyvizier/converters/spatio_temporal.py
 vizier/pyvizier/converters/spatio_temporal_test.py
 vizier/pyvizier/multimetric/__init__.py
 vizier/pyvizier/multimetric/xla_pareto.py
+vizier/raytune/__init__.py
 vizier/service/__init__.py
-vizier/service/clients.py
-vizier/service/clients_test.py
-vizier/service/constants.py
-vizier/service/custom_errors.py
-vizier/service/datastore.py
-vizier/service/datastore_test.py
-vizier/service/datastore_test_lib.py
-vizier/service/grpc_util.py
-vizier/service/performance_test.py
-vizier/service/policy_factory.py
-vizier/service/pythia_service.py
-vizier/service/pythia_util.py
-vizier/service/resources.py
-vizier/service/resources_test.py
-vizier/service/service_policy_supporter.py
-vizier/service/service_policy_supporter_test.py
-vizier/service/sql_datastore.py
-vizier/service/sql_datastore_test.py
-vizier/service/stubs_util.py
-vizier/service/stubs_util_test.py
-vizier/service/types.py
-vizier/service/vizier_client.py
-vizier/service/vizier_client_test.py
-vizier/service/vizier_server.py
-vizier/service/vizier_service.py
-vizier/service/vizier_service_test.py
+vizier/service/clients/__init__.py
+vizier/service/protos/__init__.py
 vizier/service/pyvizier/__init__.py
-vizier/service/testing/util.py
+vizier/service/servers/__init__.py
 vizier/testing/__init__.py
 vizier/testing/test_studies.py
 vizier/utils/attrs_utils.py
 vizier/utils/attrs_utils_test.py
 vizier/utils/json_utils.py
-vizier/utils/json_utils_test.py
+vizier/utils/json_utils_test.py
+vizier/utils/profiler.py
+vizier/utils/profiler_test.py
```

### Comparing `google-vizier-0.1.4/google_vizier.egg-info/requires.txt` & `google-vizier-0.1.5/google_vizier.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 emukit==0.4.9
 scipy<1.8.0,>1.2.3
 cvxpy==1.2.1
 cvxopt==1.3.0
 scikit-learn==1.1.2
 evojax==0.2.15
 lightgbm==2.2.3
-pyglove>=0.2.1
 
 [benchmarks]
 ale-py
 dopamine-rl
 nats_bench
 xgboost==1.5.1
```

### Comparing `google-vizier-0.1.4/setup.py` & `google-vizier-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/__init__.py` & `google-vizier-0.1.5/vizier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 from __future__ import annotations
 
 """Init file."""
 import os
 import sys
 
 THIS_DIR = os.path.dirname(os.path.realpath(__file__))
-PROTO_ROOT = os.path.realpath(os.path.join(THIS_DIR, "service"))
+PROTO_ROOT = os.path.realpath(os.path.join(THIS_DIR, "_src", "service"))
 
 sys.path.append(PROTO_ROOT)
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

### Comparing `google-vizier-0.1.4/vizier/_src/__init__.py` & `google-vizier-0.1.5/vizier/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/__init__.py` & `google-vizier-0.1.5/vizier/_src/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/classification/classifiers.py` & `google-vizier-0.1.5/vizier/_src/algorithms/classification/classifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from __future__ import annotations
 
 """Binary classifiers for Bayesian Optimization."""
 
 from typing import Optional
 
 import attr
-import chex
 import numpy as np
 from sklearn.gaussian_process import GaussianProcessClassifier
 from sklearn.gaussian_process.kernels import ConstantKernel
 from sklearn.gaussian_process.kernels import RBF
 
 # TODO: Replace the sklearn GP classifier with TFP GP classifier
 # once implemented.
@@ -43,17 +42,17 @@
       and `decision` which estimates a non-probability based metric such as the
       margin from the classification boundary.
   """
   classifier: Optional[GaussianProcessClassifier] = attr.field(
       kw_only=True,
       default=GaussianProcessClassifier(
           kernel=ConstantKernel(1.) * RBF(length_scale=1.)))
-  features: chex.Array = attr.field(kw_only=True)
-  labels: chex.Array = attr.field(kw_only=True)
-  features_test: chex.Array = attr.field(kw_only=True)
+  features: np.ndarray = attr.field(kw_only=True)
+  labels: np.ndarray = attr.field(kw_only=True)
+  features_test: np.ndarray = attr.field(kw_only=True)
   eval_metric: str = attr.field(kw_only=True, default='probability')
 
   def _check_features_and_labels_shapes(self) -> None:
     """Checks the compatibility between features and labels shapes."""
     if np.ndim(self.features) != 2:
       raise ValueError(f'{self} expects 2d features.')
     if self.labels.shape[0] != self.features.shape[0]:
@@ -79,15 +78,15 @@
     if self.eval_metric not in ['probability', 'decision']:
       raise ValueError(f'{self} expects the evaluation metric to be'
                        f'`probability` or `decision ` but `{self.eval_metric}`'
                        'was given.')
 
   # TODO: separate the training and evaluation for extra speed up.
   # Currently, the classifiers we use are reasonably fast.
-  def __call__(self) -> chex.Array:
+  def __call__(self) -> np.ndarray:
     self._check_features_and_labels_shapes()
     self._check_labels_values()
     self._check_eval_metric()
     self.classifier.fit(np.asarray(self.features), np.asarray(self.labels))
     if self.eval_metric == 'probability':
       return self.classifier.predict_proba(np.asarray(self.features_test))[:, 1]
     else:
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/classification/classifiers_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/classification/classifiers_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/core/__init__.py` & `google-vizier-0.1.5/vizier/_src/algorithms/core/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/core/abstractions.py` & `google-vizier-0.1.5/vizier/_src/algorithms/core/abstractions.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 """Abstractions."""
 
 import abc
 from typing import Optional, Protocol, Sequence, TypeVar
 
 import attr
 import chex
+import jax
 from vizier import pyvizier as vz
 from vizier.interfaces import serializable
 
 _T = TypeVar('_T')
 
 
 @attr.define(frozen=True)
@@ -157,21 +158,39 @@
 
   def __attrs_post_init__(self):
     if self.mean.shape != self.stddev.shape:
       raise ValueError('The shape of mean and stddev needs to be the same.')
 
 
 class Predictor(abc.ABC):
-  """Mixin for algorithms to expose prediction API."""
+  """Predicts objective values, given suggestions.
+
+  For algorithms which involve the use of function regressors, this class also
+  acts as a mixin to expose their prediction API.
+  """
 
   @abc.abstractmethod
   def predict(
-      self, trials: Sequence[vz.TrialSuggestion], rng: chex.PRNGKey
+      self,
+      trials: Sequence[vz.TrialSuggestion],
+      rng: Optional[jax.random.KeyArray] = None,
+      num_samples: Optional[int] = None,
   ) -> Prediction:
-    """Predicts the mean and stddev for any given trials."""
+    """Returns the mean and stddev for any given suggestions.
+
+    Arguments:
+      trials: The suggestions where the predictions will be made. Can also be
+        completed trials for retrospective predictions.
+      rng: The sampling random key used for approximation (if applicable).
+      num_samples: The number of samples used for the approximation (if
+        applicable).
+
+    Returns:
+      The predictions for the given suggestions.
+    """
 
 
 class DesignerFactory(Protocol[_T]):
   """Protocol (PEP-544) for a designer factory."""
 
   def __call__(self, problem: vz.ProblemStatement, **kwargs) -> _T:
     pass
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/__init__.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/bocs.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/bocs.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/bocs_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/bocs_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/cmaes.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/cmaes.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/cmaes_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/cmaes_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_designer_convergence_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/eagle_strategy_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/serialization.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/serialization.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/serialization_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/eagle_strategy/testing.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/eagle_strategy/testing.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/emukit.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/emukit.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,16 +192,17 @@
       gpy_model = models.GPRegression(features, labels)
       emukit_model = model_wrappers.GPyModelWrapper(gpy_model)
       acquisition = acquisitions.ExpectedImprovement(model=emukit_model)
 
     elif self._version == Version.MATERN52_UCB:
       gpy_model = _create_constrained_gp(features, labels)
       emukit_model = model_wrappers.GPyModelWrapper(gpy_model, n_restarts=20)
-      acquisition = acquisitions.NegativeLowerConfidenceBound(
-          model=emukit_model, beta=np.float64(1.8))
+      acquisition = acquisitions.NegativeLowerConfidenceBound(  # pytype: disable=wrong-arg-types  # numpy-scalars
+          model=emukit_model, beta=np.float64(1.8)
+      )
 
     logging.info(
         'Emukit model: model=%s',
         # Values associated with length-1 keys are useless.
         {k: v for k, v in emukit_model.model.to_dict().items() if len(k) > 1})
 
     logging.info('Gpy model: model=%s', gpy_model)
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/emukit_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/emukit_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/gp/yjt.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/gp/yjt.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/grid.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/grid.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,35 +11,44 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Grid Search Designer which searches over a discretized grid of Trial parameter values."""
-
+import copy
 import random
-from typing import List, Optional, Sequence
+from typing import Dict, List, Optional, Sequence
+from absl import logging
 
 import numpy as np
 from vizier import algorithms
 from vizier import pyvizier
 from vizier.pyvizier import converters
 
+GridValues = Dict[str, List[pyvizier.ParameterValue]]
+
 
 class GridSearchDesigner(algorithms.PartiallySerializableDesigner):
   """Grid Search designer.
 
   This designer searches over a grid of hyper-parameter values.
 
   NOTE: The grid search index (i.e. which grid point to output) is based the
   number of suggestions created so far (regardless of completion or not). This
   means the class must be wrapped via `PartiallySerializableDesignerPolicy` for
   use in Pythia, thus requiring load/dump implementations.
   """
 
+  _unshuffled_grid_values: GridValues
+  _grid_values: GridValues
+  _current_index: int
+  _shuffle_seed: Optional[int]
+  _double_grid_resolution: int
+
   def __init__(
       self,
       search_space: pyvizier.SearchSpace,
       shuffle_seed: Optional[int] = None,
       *,
       double_grid_resolution: int = 10,
   ):
@@ -52,34 +61,29 @@
       double_grid_resolution: Number of grid points for DOUBLE parameters.
     """
     if search_space.is_conditional:
       raise ValueError(
           f'This designer {self} does not support conditional search.'
       )
     self._search_space = search_space
+    self._shuffle_seed = shuffle_seed
     self._double_grid_resolution = double_grid_resolution
     self._current_index = 0
 
-    # Makes the grid values for every parameter.
-    self._grid_values = {}
+    # Creates unshuffled grid values for every parameter. This is just a
+    # template for creating the potentially shuffled self._grid_values to be
+    # used in suggest().
+    self._unshuffled_grid_values = {}
     for parameter_config in self._search_space.parameters:
-      self._grid_values[parameter_config.name] = (
+      self._unshuffled_grid_values[parameter_config.name] = (
           self._grid_points_from_parameter_config(parameter_config)
       )
 
-    # Shuffle the grid if specified.
-    if shuffle_seed is not None:
-      rng = random.Random(shuffle_seed)
-      # Shuffle dict keys.
-      shuffled_items = list(self._grid_values.items())
-      rng.shuffle(shuffled_items)
-      self._grid_values = dict(shuffled_items)
-      # Shuffle dict value lists.
-      for param_name in self._grid_values:
-        rng.shuffle(self._grid_values[param_name])
+    # Set true grid values to be used during suggest calls.
+    self._grid_values = self._maybe_shuffled_grid_values(self._shuffle_seed)
 
   @classmethod
   def from_problem(
       cls,
       problem: pyvizier.ProblemStatement,
       seed: Optional[int] = None,
   ):
@@ -123,19 +127,27 @@
 
     self._current_index += len(parameter_dicts)
     return [pyvizier.TrialSuggestion(parameters=p) for p in parameter_dicts]
 
   def load(self, metadata: pyvizier.Metadata) -> None:
     """Load the current index."""
     self._current_index = int(metadata.ns('grid')['current_index'])
+    none_or_int = metadata.ns('grid')['shuffle_seed']
+    if none_or_int == 'None':
+      self._shuffle_seed = None
+    else:
+      logging.info('Using integer seed for shuffling: %d', none_or_int)
+      self._shuffle_seed = int(none_or_int)
+    self._grid_values = self._maybe_shuffled_grid_values(self._shuffle_seed)
 
   def dump(self) -> pyvizier.Metadata:
     """Dump the current index."""
     metadata = pyvizier.Metadata()
     metadata.ns('grid')['current_index'] = str(self._current_index)
+    metadata.ns('grid')['shuffle_seed'] = str(self._shuffle_seed)
     return metadata
 
   def _grid_points_from_parameter_config(
       self,
       parameter_config: pyvizier.ParameterConfig,
   ) -> List[pyvizier.ParameterValue]:
     """Produces grid points from a parameter_config."""
@@ -167,7 +179,25 @@
       ]
 
     else:
       raise ValueError(
           'ParameterConfig type is not one of the supported primitives for'
           f' ParameterConfig: {parameter_config}'
       )
+
+  def _maybe_shuffled_grid_values(
+      self, shuffle_seed: Optional[int]
+  ) -> GridValues:
+    grid_values = copy.deepcopy(self._unshuffled_grid_values)
+
+    # Shuffle the grid if specified.
+    if shuffle_seed is not None:
+      rng = random.Random(shuffle_seed)
+      # Shuffle dict keys.
+      shuffled_items = list(grid_values.items())
+      rng.shuffle(shuffled_items)
+      grid_values = dict(shuffled_items)
+      # Shuffle dict value lists.
+      for param_name in grid_values:
+        rng.shuffle(grid_values[param_name])
+
+    return grid_values
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/grid_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/grid_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for grid."""
+import functools
+
 from vizier import pythia
 from vizier import pyvizier
 from vizier._src.algorithms.designers import grid
 from vizier._src.algorithms.policies import designer_policy
 
 from absl.testing import absltest
 from absl.testing import parameterized
@@ -90,20 +92,24 @@
         [
             tuple(suggestion.parameters.as_dict().values())
             for suggestion in suggestions
         ]
     )
     self.assertLen(distinct_suggestions, self.search_space_size)
 
-  def test_policy_wrapping(self):
+  @parameterized.parameters((None,), (0,), (1,), (2,))
+  def test_policy_wrapping(self, shuffle_seed):
     problem = pyvizier.ProblemStatement()
     problem.search_space = self.search_space
     policy_supporter = pythia.InRamPolicySupporter(problem)
+    designer_factory = functools.partial(
+        grid.GridSearchDesigner.from_problem, seed=shuffle_seed
+    )
     policy = designer_policy.PartiallySerializableDesignerPolicy(
-        problem, policy_supporter, grid.GridSearchDesigner.from_problem
+        problem, policy_supporter, designer_factory
     )
 
     # Make sure we covered entire search space.
     all_suggestions = []
     for _ in range(self.search_space_size):
       request = pythia.SuggestRequest(
           study_descriptor=policy_supporter.study_descriptor(), count=1
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/harmonica.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/harmonica.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,154 +16,193 @@
 
 """Harmonica algorithm for boolean search spaces from 'Hyperparameter Optimization: A Spectral Approach' (https://arxiv.org/abs/1706.00764).
 
 This is a faithful re-implementation based off
 https://github.com/callowbird/Harmonica.
 """
 # pylint:disable=invalid-name
-import functools
+import abc
 import itertools
-from typing import Callable, Optional, Sequence, Set
+from typing import Optional, Sequence, Set
+import attrs
 import numpy as np
 from sklearn import linear_model
 from sklearn import preprocessing
 
 from vizier import algorithms as vza
 from vizier import pyvizier as vz
 from vizier._src.algorithms.designers import random
 
 
-def _binary_subset_enumeration(dim: int,
-                               indices: Sequence[int],
-                               default_value: float = 1.0) -> np.ndarray:
-  """Outputs all possible binary vectors from {-1, 1}^{dim} where only positions from `indices` are changed."""
-  output = default_value * np.ones(
-      shape=(2**len(indices), dim), dtype=np.float32)
-  for i, binary in enumerate(
-      itertools.product([-1.0, 1.0], repeat=len(indices))):
-    output[i, indices] = binary
-  return output
+class _Surrogate(abc.ABC):
+  """Utility class to organize code."""
+
+  @abc.abstractmethod
+  def reset(self) -> None:
+    """Resets internal state."""
+
+  @abc.abstractmethod
+  def regress(self, X: np.ndarray, Y: np.ndarray) -> None:
+    """Performs regression and modifies internal state."""
 
+  @abc.abstractmethod
+  def predict(self, x: np.ndarray) -> float:
+    """Performs prediction. Should NOT modify internal state."""
 
-# TODO: Implement __repr__ via `attr`.
-class PolynomialSparseRecovery:
+
+@attrs.define
+class PolynomialSparseRecovery(_Surrogate):
   """Performs LASSO regression over low (d) degree polynomial coefficients."""
 
-  def __init__(self,
-               d: int = 3,
-               num_top_monomials: int = 5,
-               alpha: float = 3.0):
-    """Init.
+  # Maximum degree of monomials to use during polynomial regression.
+  _d: int = attrs.field(
+      default=3, validator=attrs.validators.ge(1), kw_only=True
+  )
+  # Number of top monomial coefficients to use.
+  _num_top_monomials: int = attrs.field(
+      default=5, validator=attrs.validators.ge(1), kw_only=True
+  )
+
+  # LASSO regularization coefficient.
+  _alpha = attrs.field(
+      default=3.0, validator=attrs.validators.ge(0.0), kw_only=True
+  )
+
+  # Internal state after performing regression.
+  _poly_transformer: preprocessing.PolynomialFeatures = attrs.field(init=False)
+  _top_poly_indices: np.ndarray = attrs.field(init=False)
+  _top_poly_coefficients: np.ndarray = attrs.field(init=False)
 
-    Args:
-      d: Maximum degree of monomials to use during polynomial regression.
-      num_top_monomials: Number of top monomial coefficients to use.
-      alpha: LASSO regularization coefficient.
-    """
-    self._d = d
-    self._num_top_monomials = num_top_monomials
-    self._alpha = alpha
+  def __attrs_post_init__(self):
     self.reset()
 
-  def reset(self):
+  def reset(self) -> None:
     self._poly_transformer = preprocessing.PolynomialFeatures(
-        self._d, interaction_only=True)
-    self._top_poly_indices: Optional[np.ndarray] = None
-    self._top_poly_coefficients: Optional[np.ndarray] = None
+        self._d, interaction_only=True
+    )
+    self._top_poly_indices = np.empty(0)
+    self._top_poly_coefficients = np.empty(0)
 
   def regress(self, X: np.ndarray, Y: np.ndarray) -> None:
     """Performs LASSO regression to obtain top monomial coefficients."""
 
-    # Computes monomial values for every vector in X.
-    X_poly_features = []
-    for x_vector in X:
-      X_poly_features.append(
-          self._poly_transformer.fit_transform(
-              np.array(x_vector).reshape(1, -1))[0].tolist())
-    X_poly_features = np.array(X_poly_features)
+    # Computes monomial features for every vector in X.
+    X_poly_features = self._poly_transformer.fit_transform(X)
 
     # Find optimial coefficients on monomials to the data.
     lasso_solver = linear_model.Lasso(fit_intercept=True, alpha=self._alpha)
     lasso_solver.fit(X_poly_features, Y)
 
     # Sort and obtain top coefficients.
     lasso_coefficients = lasso_solver.coef_
     poly_indices = np.argsort(-np.abs(lasso_coefficients))
-    self._top_poly_indices = poly_indices[:self._num_top_monomials]
+    self._top_poly_indices = poly_indices[: self._num_top_monomials]
     self._top_poly_coefficients = lasso_coefficients[self._top_poly_indices]
 
-  def surrogate(self, x: np.ndarray) -> float:
-    """Surrogate/Predicted function after regress()."""
-    x_poly_features = self._poly_transformer.fit_transform(x.reshape(1, -1))
+  def predict(self, x: np.ndarray) -> float:
+    """Predicts using polynomial features."""
+    x_poly_features = self._poly_transformer.transform(x.reshape(1, -1))
+    x_poly_features = x_poly_features[0]
+
     top_x_poly_features = np.take_along_axis(
-        x_poly_features[0], self._top_poly_indices, axis=0)
+        x_poly_features, self._top_poly_indices, axis=0
+    )
     return np.dot(top_x_poly_features, self._top_poly_coefficients)
 
   def index_set(self) -> Set[int]:
     """Returns parameter index set J from top coefficients.
 
     For example, if our monomials corresponding to top cofficients were x0*x1,
     x3, x1*x2*x3, then the output would be Union({0, 1}, {3}, {1, 2, 3}).
     """
-    index_set = set()
+    indices = set()
     poly_feature_one_hots = self._poly_transformer.powers_
     for top_poly_index in self._top_poly_indices:
-      active_indices = np.nonzero(
-          poly_feature_one_hots[top_poly_index])[0].tolist()
-      index_set = index_set | set(active_indices)
-    return index_set
+      active_indices = np.nonzero(poly_feature_one_hots[top_poly_index])
+      active_indices = active_indices[0].tolist()
+      indices = indices | set(active_indices)
+    return indices
 
 
-def _restricted_surrogate(x: np.ndarray, X_restrictors: np.ndarray,
-                          replacement_indices: Sequence[int],
-                          psr: PolynomialSparseRecovery):
+@attrs.define
+class RestrictedSurrogate(_Surrogate):
   """New surrogate with input x's positions replaced from X_restrictor values."""
-  objectives = []
-  for x_restrictor in X_restrictors:
-    x_copy = np.copy(x)
-    x_copy[replacement_indices] = x_restrictor[replacement_indices]
-    objectives.append(psr.surrogate(x_copy))
-  return np.mean(objectives)
 
+  X_restrictors: np.ndarray = attrs.field(init=True, kw_only=True)
+  replacement_indices: Sequence[int] = attrs.field(init=True, kw_only=True)
+  psr: PolynomialSparseRecovery = attrs.field(
+      init=True, kw_only=True, factory=PolynomialSparseRecovery
+  )
+
+  def reset(self) -> None:
+    raise NotImplementedError('Should not be used.')
 
-# TODO: Implement __repr__ via `attr`.
-class HarmonicaQ:
+  def regress(self, X: np.ndarray, Y: np.ndarray) -> None:
+    raise NotImplementedError('Should not be used.')
+
+  def predict(self, x: np.ndarray) -> float:
+    objectives = []
+    for x_restrictor in self.X_restrictors:
+      x_copy = np.copy(x)
+      x_copy[self.replacement_indices] = x_restrictor[self.replacement_indices]
+      objectives.append(self.psr.predict(x_copy))
+    return np.mean(objectives)
+
+
+def _binary_subset_enumeration(
+    dim: int, indices: Sequence[int], default_value: float = 1.0
+) -> np.ndarray:
+  """Outputs all possible binary vectors from {-1, 1}^{dim} where only positions from `indices` are changed."""
+  output = default_value * np.ones(
+      shape=(2 ** len(indices), dim), dtype=np.float32
+  )
+  for i, binary in enumerate(
+      itertools.product([-1.0, 1.0], repeat=len(indices))
+  ):
+    output[i, indices] = binary
+  return output
+
+
+@attrs.define
+class HarmonicaQ(_Surrogate):
   """Q-stage Harmonica.
 
   At each stage:
   1. Invoke PSR on the previous data (X,Y).
   2. Obtain t maximizers of the surrogate of the PSR.
   3. Redefine a 'restricted surrogate' using the t maximizers.
   4. Produce a new (X', Y') dataset via random search on this 'restricted
   surrogate'.
   """
 
-  def __init__(self,
-               psr: Optional[PolynomialSparseRecovery] = None,
-               q: int = 10,
-               t: int = 1,
-               T: int = 300):
-    """Init.
+  # PolynomialSparseRecovery regressor.
+  _psr: PolynomialSparseRecovery = attrs.field(
+      init=True, kw_only=True, factory=PolynomialSparseRecovery
+  )
+  # Number of stages.
+  _q: int = attrs.field(
+      default=10, validator=attrs.validators.ge(0), kw_only=True
+  )
+
+  # Number of maximizers on the surrogate to use.
+  _t: int = attrs.field(
+      default=1, validator=attrs.validators.ge(1), kw_only=True
+  )
+  # Number of data samples to collect on the restricted surrogate.
+  _T: int = attrs.field(
+      default=300, validator=attrs.validators.ge(1), kw_only=True
+  )
 
-    Args:
-      psr: PolynomialSparseRecovery class. If None, will be constructed with
-        default arguments.
-      q: Number of stages.
-      t: Number of maximizers on the surrogate to use.
-      T: Number of data samples to collect on the restricted surrogate.
-    """
-    self._psr = psr
-    self._psr = psr or PolynomialSparseRecovery()
-    self._q = q
-    self._t = t
-    self._T = T
+  _restricted_surrogate: Optional[RestrictedSurrogate] = None
+
+  def __attrs_post_init__(self):
     self.reset()
 
-  def reset(self):
-    self._restricted_surrogate: Optional[Callable[[np.ndarray], float]] = None
+  def reset(self) -> None:
+    self._restricted_surrogate = None
     self._psr.reset()
 
   def regress(self, X: np.ndarray, Y: np.ndarray) -> None:
     """Performs q-stage Harmonica."""
     num_vars = X.shape[-1]
 
     X_temp = X
@@ -172,31 +211,31 @@
       # Invoke PSR on data.
       self._psr.reset()
       self._psr.regress(X_temp, Y_temp)
       J = self._psr.index_set()
 
       # Perform brute force maximization to optain top t optimizers.
       all_X_in_J = _binary_subset_enumeration(num_vars, list(J))
-      all_Y_in_J = np.array([self._psr.surrogate(x) for x in all_X_in_J])
-      maximizer_idxs = np.argsort(all_Y_in_J)[-self._t:]
+      all_Y_in_J = np.array([self._psr.predict(x) for x in all_X_in_J])
+      maximizer_idxs = np.argsort(all_Y_in_J)[-self._t :]
       X_maximizers = all_X_in_J[maximizer_idxs]
 
       # Define restricted surrogate and obtain data from it.
-      self._restricted_surrogate = functools.partial(
-          _restricted_surrogate,
+      self._restricted_surrogate = RestrictedSurrogate(
           X_restrictors=X_maximizers,
           replacement_indices=list(J),
-          psr=self._psr)
+          psr=self._psr,
+      )
       X_temp = np.random.choice([-1.0, 1.0], size=(self._T, num_vars))
-      Y_temp = np.array([self._restricted_surrogate(x) for x in X_temp])
+      Y_temp = np.array([self._restricted_surrogate.predict(x) for x in X_temp])
 
-  def surrogate(self, x: np.ndarray) -> float:
+  def predict(self, x: np.ndarray) -> float:
     if self._restricted_surrogate is None:
       raise ValueError('You must call regress() first.')
-    return self._restricted_surrogate(x)
+    return self._restricted_surrogate.predict(x)
 
 
 class HarmonicaDesigner(vza.Designer):
   """Harmonica Designer.
 
   The summary of the current implementation is as follows:
 
@@ -205,34 +244,37 @@
   based on filtering only the highest coefficients.
   3. Obtain the "J"-set (i.e. set of input indices that only affect the
   predictor function).
   4. Find the global optimizer over the J-set domain on the predictor function,
   and return it as a suggestion.
   """
 
-  def __init__(self,
-               problem_statement: vz.ProblemStatement,
-               harmonica_q: Optional[HarmonicaQ] = None,
-               acquisition_samples: int = 100,
-               num_init_samples: int = 10):
+  def __init__(
+      self,
+      problem_statement: vz.ProblemStatement,
+      harmonica_q: Optional[HarmonicaQ] = None,
+      acquisition_samples: int = 100,
+      num_init_samples: int = 10,
+  ):
     """Init.
 
     Args:
       problem_statement: Must use a boolean search space.
       harmonica_q: HarmonicaQ class. If None, will use default class with
         default kwargs.
       acquisition_samples: Number of trial samples to optimize final acquisition
         function.
       num_init_samples: Number of initial random suggestions for seeding the
         model.
     """
 
     if problem_statement.search_space.is_conditional:
       raise ValueError(
-          f'This designer {self} does not support conditional search.')
+          f'This designer {self} does not support conditional search.'
+      )
     for p_config in problem_statement.search_space.parameters:
       if p_config.external_type != vz.ExternalType.BOOLEAN:
         raise ValueError('Only boolean search spaces are supported.')
 
     self._problem_statement = problem_statement
     self._metric_name = self._problem_statement.metric_information.item().name
     self._search_space = problem_statement.search_space
@@ -245,16 +287,17 @@
     self._trials = []
 
   def update(
       self, completed: vza.CompletedTrials, all_active: vza.ActiveTrials
   ) -> None:
     self._trials += tuple(completed.trials)
 
-  def suggest(self,
-              count: Optional[int] = None) -> Sequence[vz.TrialSuggestion]:
+  def suggest(
+      self, count: Optional[int] = None
+  ) -> Sequence[vz.TrialSuggestion]:
     """Performs entire q-stage Harmonica using previous trials for regression data.
 
     Args:
       count: Makes best effort to generate this many suggestions. If None,
         suggests as many as the algorithm wants.
 
     Returns:
@@ -278,26 +321,29 @@
       ]
       single_y = t.final_measurement.metrics[self._metric_name].value
       X.append(single_x)
       Y.append(single_y)
     X = np.array(X)
     Y = np.array(Y)
 
-    if self._problem_statement.metric_information.item(
-    ).goal == vz.ObjectiveMetricGoal.MINIMIZE:
+    if (
+        self._problem_statement.metric_information.item().goal
+        == vz.ObjectiveMetricGoal.MINIMIZE
+    ):
       Y = -Y
 
     # Perform q-stage Harmonica.
     self._harmonica_q.reset()
     self._harmonica_q.regress(X, Y)
 
     # Optimize final acquisition function.
     # TODO: Allow any designer instead of just random search.
-    X_temp = np.random.choice([-1.0, 1.0],
-                              size=(self._acquisition_samples, self._num_vars))
-    Y_temp = np.array([self._harmonica_q.surrogate(x) for x in X_temp])
+    X_temp = np.random.choice(
+        [-1.0, 1.0], size=(self._acquisition_samples, self._num_vars)
+    )
+    Y_temp = np.array([self._harmonica_q.predict(x) for x in X_temp])
     x_new = X_temp[np.argmax(Y_temp)]
 
     parameters = vz.ParameterDict()
     for i, p in enumerate(self._search_space.parameters):
       parameters[p.name] = 'True' if x_new[i] == 1.0 else 'False'
     return [vz.TrialSuggestion(parameters=parameters)]
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/harmonica_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/harmonica_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/quasi_random.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/quasi_random.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 from __future__ import annotations
 
 """Quasi-random designer."""
 
 import collections
 import math
-import random
 import sys
+import time
 from typing import Iterable, List, Optional, Sequence
 
 import attr
 import numpy as np
 from vizier import algorithms as vza
 from vizier import pyvizier as vz
 from vizier.interfaces import serializable
@@ -94,23 +94,25 @@
           iterable_validator=attr.validators.instance_of(Iterable),
       ),
   )
 
   _scramble: bool = attr.field(
       default=True, validator=attr.validators.instance_of(bool), kw_only=True
   )
+  _seed: int = attr.field(default=0)
 
   def __init__(
       self,
       num_dimensions: int,
       *,
       skip_points: int,
       num_points_generated: int = 0,
       primes_override: Optional[List[int]] = None,
       scramble: bool = True,
+      seed: int = 0,
   ):
     """Create a Halton sequence generator.
 
     Args:
       num_dimensions: Number of dimensions for each point in the seqeunce. This
         corresponds to the number of parameters in the Vizier search space.
       skip_points: The number of initial points that should be skipped before
@@ -118,14 +120,15 @@
       num_points_generated: Number of points that have already been generated.
       primes_override: If supplied, use these primes to seed each dimension of
         the Halton sequence. This is useful for testing. NOTE: These values are
         not validated, so it is the responsibility of the user to supply
         legitimate primes.
       scramble: If True, will scramble the resulting Halton sequence. Set this
         to False for testing.
+      seed: random seed
 
     Returns:
       A HaltonSequence object.
     """
     if skip_points < 0:
       raise ValueError('skip_points must be non-negative: %s' % skip_points)
 
@@ -142,42 +145,45 @@
 
     self.__attrs_init__(
         num_dimensions=num_dimensions,
         skip_points=skip_points,
         num_points_generated=num_points_generated,
         primes=primes,
         scramble=scramble,
+        seed=seed,
     )
 
   def load(self, metadata: vz.Metadata) -> None:
     self._num_points_generated = int(
         metadata.ns('halton')['num_points_generated']
     )
+    self._seed = int(metadata.ns('halton')['permutation_seed'])
 
   def dump(self) -> vz.Metadata:
     metadata = vz.Metadata()
     metadata.ns('halton')['num_points_generated'] = str(
         self._num_points_generated
     )
+    metadata.ns('halton')['permutation_seed'] = str(self._seed)
     return metadata
 
   def _get_scrambled_halton_value(self, index: int, base: int) -> float:
     """Get a scrambled Halton value for a given `index` using `base`.
 
     For example, if `index` can be represented in `base` b as:
 
     `index = 5 * b^{2} + 2 * b^{1} + 3`
 
     then the Halton value will be:
 
     `Halton(index) = 5 * b^{-1} + 2 * b^{-2} + 3 * b^{-3}.`
 
     If we choose to scramble, then the coefficients (5,2,3) will be randomly
-    permuted (seeded by `base`), leading to a roughly uniform distribution of
-    Halton values over the interval [0,1].
+    permuted seeded by self._seed and base, leading to a
+    roughly uniform distribution of Halton values over the interval [0,1].
 
     Args:
       index: Index to be converted to `base`.
       base: Base used for conversion.
 
     Returns:
       (Possibly scrambled) Halton value.
@@ -188,17 +194,17 @@
     result = 0.0
     base_rec = 1.0 / base
     f = base_rec
     i = index + 1  # For index 0 we want 1/base returned, not 0.
 
     # Use a fixed seed to generate the permutation in a deterministic way.
     if self._scramble:
-      local_random = random.Random(base)
       permutation = list(range(1, base))
-      local_random.shuffle(permutation)
+      rng = np.random.RandomState((self._seed, base))
+      rng.shuffle(permutation)
       permutation = [0] + permutation
     while i > 0:
       i, mod = divmod(i, base)
       if self._scramble:
         result += f * permutation[mod]
       else:
         result += f * mod
@@ -245,22 +251,31 @@
   `halton(n) = c3 * p^{-1} + c2 * p^{-2} + c1 * p^{-3} + c0 * p^{-4}`
 
   To obtain a pseuo-uniform distribution, we permute the coefficients:
 
   `permuted_halton(n) = c2 * p^{-1} + c1 * p^{-2} + c0 * p^{-3} + c3 * p^{-4}`
   """
 
-  def __init__(self, search_space: vz.SearchSpace, *, skip_points: int = 1000):
+  def __init__(
+      self,
+      search_space: vz.SearchSpace,
+      *,
+      skip_points: int = 1000,
+      seed: Optional[int] = None,
+  ):
     """Init.
 
     Args:
       search_space: Must be a flat search space.
       skip_points: If positive, then these first points in the sequence are
         discarded in order to avoid unwanted correlations.
+      seed: Random seed.
     """
+    if seed is None:
+      seed = np.int32(time.time())
     if search_space.is_conditional:
       raise ValueError(
           f'This designer {self} does not support conditional search.'
       )
 
     def create_input_converter(pc):
       return converters.DefaultModelInputConverter(
@@ -287,25 +302,25 @@
         )
 
     self._halton_generator = _HaltonSequence(
         len(search_space.parameters),
         skip_points=skip_points,
         num_points_generated=0,
         scramble=True,
+        seed=seed,
     )
 
     self._output_specs = tuple(self._converter.output_specs.values())
 
   @classmethod
   def from_problem(
       cls, problem: vz.ProblemStatement, seed: Optional[int] = None
   ):
     """For wrapping via `PartiallySerializableDesignerPolicy`."""
-    del seed
-    return QuasiRandomDesigner(problem.search_space)
+    return QuasiRandomDesigner(problem.search_space, seed=seed)
 
   def load(self, metadata: vz.Metadata) -> None:
     self._halton_generator.load(metadata)
 
   def dump(self) -> vz.Metadata:
     return self._halton_generator.dump()
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/quasi_random_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/quasi_random_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import random
+
 import numpy as np
 from scipy import stats
-
+from vizier import pythia
 from vizier import pyvizier as vz
 from vizier._src.algorithms.designers import quasi_random
+from vizier._src.algorithms.policies import designer_policy
 from vizier._src.algorithms.testing import test_runners
 from vizier.testing import test_studies
 
 from absl.testing import absltest
 
 
 class HaltonTest(absltest.TestCase):
@@ -64,18 +66,26 @@
     generator_2 = quasi_random._HaltonSequence(
         num_dimensions=4, skip_points=100, primes_override=[3, 5, 7, 11]
     )
     self.assertEqual(
         [generator_1.get_next_list() for i in range(100)],
         [generator_2.get_next_list() for i in range(100)],
     )
+    self.assertEqual(
+        [generator_1.get_next_list() for i in range(100)],
+        [generator_2.get_next_list() for i in range(100)],
+    )
 
   def test_unscrambled_sequence(self):
     generator = quasi_random._HaltonSequence(
-        num_dimensions=1, skip_points=0, primes_override=[3], scramble=False
+        num_dimensions=1,
+        skip_points=0,
+        primes_override=[3],
+        scramble=False,
+        seed=0,
     )
     sequence = [generator.get_next_list()[0] for _ in range(7)]
 
     expected_sequence = [
         1 / 3,
         2 / 3,
         1 / 9,
@@ -131,10 +141,55 @@
     # p_value greater than 0.9 roughly means we're very certain it's uniform.
     # Unfortunately KS-test doesn't work for discrete/categorical distributions.
     _, float_p_value = stats.kstest(
         float_points, stats.uniform(loc=0.0, scale=1.0).cdf
     )
     self.assertGreater(float_p_value, 0.9)
 
+  def test_equal_seeds(self):
+    problem = vz.ProblemStatement()
+    problem.search_space.root.add_float_param('float', 0.0, 1.0)
+    designer_1 = quasi_random.QuasiRandomDesigner(problem.search_space, seed=1)
+    suggestions_1 = designer_1.suggest(10)
+    designer_2 = quasi_random.QuasiRandomDesigner(problem.search_space, seed=1)
+    suggestions_2 = designer_2.suggest(10)
+    self.assertEqual(suggestions_1, suggestions_2)
+
+  def test_distinct_seeds(self):
+    problem = vz.ProblemStatement()
+    problem.search_space.root.add_float_param('float', 0.0, 1.0)
+    designer_1 = quasi_random.QuasiRandomDesigner(problem.search_space, seed=0)
+    suggestions_1 = designer_1.suggest(10)
+    designer_2 = quasi_random.QuasiRandomDesigner(problem.search_space, seed=1)
+    suggestions_2 = designer_2.suggest(10)
+    self.assertNotEqual(suggestions_1, suggestions_2)
+
+  def test_policy_wrapping(self):
+    problem = vz.ProblemStatement()
+    problem.search_space.root.add_float_param('float', 0.0, 1.0)
+    policy_supporter = pythia.InRamPolicySupporter(problem)
+    policy = designer_policy.PartiallySerializableDesignerPolicy(
+        problem,
+        policy_supporter,
+        quasi_random.QuasiRandomDesigner.from_problem,
+    )
+
+    # Make sure outputs are distinct.
+    all_suggestions = []
+    for _ in range(1000):
+      request = pythia.SuggestRequest(
+          study_descriptor=policy_supporter.study_descriptor(), count=1
+      )
+      decisions = policy.suggest(request)
+      all_suggestions.extend(decisions.suggestions)
+
+    distinct_suggestions = set(
+        [
+            tuple(suggestion.parameters.as_dict().values())
+            for suggestion in all_suggestions
+        ]
+    )
+    self.assertLen(distinct_suggestions, 1000)
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/random.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/random.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/random_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/shared/study.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,38 +10,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-"""Tests for random."""
+"""Shared classes for representing studies."""
 
-from vizier import pyvizier as vz
-from vizier._src.algorithms.designers import random
-from vizier._src.algorithms.testing import test_runners
-from vizier.testing import test_studies
-
-from absl.testing import absltest
-
-
-class RandomTest(absltest.TestCase):
-
-  def test_on_flat_space(self):
-    config = vz.ProblemStatement(test_studies.flat_space_with_all_types())
-    designer = random.RandomDesigner(config.search_space, seed=None)
-    self.assertLen(
-        test_runners.run_with_random_metrics(
-            designer, config, iters=50, batch_size=1), 50)
-
-  def test_reproducible_random(self):
-    config = vz.ProblemStatement(test_studies.flat_space_with_all_types())
-    designer = random.RandomDesigner(config.search_space, seed=5)
-    t1 = designer.suggest(10)
-
-    designer = random.RandomDesigner(config.search_space, seed=5)
-    t2 = designer.suggest(10)
-    self.assertEqual(t1, t2)
-
-
-if __name__ == '__main__':
-  absltest.main()
+from typing import List
+import attr
+from vizier._src.pyvizier.shared import base_study_config
+from vizier._src.pyvizier.shared import trial
+
+
+@attr.define(frozen=True, init=True, slots=True, kw_only=False)
+class ProblemAndTrials:
+  """Container for problem statement and trials."""
+  problem: base_study_config.ProblemStatement = attr.ib(init=True)
+  trials: List[trial.Trial] = attr.ib(
+      init=True,
+      # TODO: Remove the pylint.
+      converter=lambda x: list(x),  # pylint: disable=unnecessary-lambda
+      default=attr.Factory(list))
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/scalarizing_designer.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/scalarizing_designer.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,47 +15,48 @@
 from __future__ import annotations
 
 """Scalarizing Designer for MOO via reducing to a scalarized objective."""
 import copy
 from typing import Optional, Protocol, Sequence
 
 import attr
-import chex
+import jax
 from jax import numpy as jnp
+from jax.typing import ArrayLike
 from vizier import algorithms as vza
 from vizier import pyvizier as vz
 
 
 # TODO Separate into another file/folder.
 class Scalarization(Protocol):
   """Reduces an array of objectives to a single float.
 
   Assumes all objectives are for MAXIMIZATION.
   """
 
-  def __call__(self, objectives: chex.Array) -> float:
+  def __call__(self, objectives: ArrayLike) -> jax.Array:
     pass
 
 
 @attr.define(init=True)
 class HyperVolumeScalarization(Scalarization):
   """HyperVolume Scalarization."""
 
-  weights: chex.Array = attr.ib()
+  weights: ArrayLike = attr.ib()
 
-  reference_point: Optional[chex.Array] = attr.ib(default=None, kw_only=True)
+  reference_point: Optional[ArrayLike] = attr.ib(default=None, kw_only=True)
 
   def __attrs_post_init__(self):
     if any(self.weights <= 0):
       raise ValueError(f'Non-positive weights {self.weights}')
 
-  def __call__(
+  def __call__(  # pytype: disable=signature-mismatch  # numpy-scalars
       self,
-      objectives: chex.Array,
-  ) -> chex.Array:
+      objectives: ArrayLike,
+  ) -> jax.Array:
     # Uses scalarizations in https://arxiv.org/abs/2006.04655 for
     # non-convex multiobjective optimization.
     if self.reference_point is not None:
       return jnp.min((objectives - self.reference_point) / self.weights)
     else:
       return jnp.min(objectives / self.weights)
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/designers/scalarizing_designer_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/designers/scalarizing_designer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/evolution/__init__.py` & `google-vizier-0.1.5/vizier/_src/algorithms/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/evolution/nsga2.py` & `google-vizier-0.1.5/vizier/_src/algorithms/evolution/nsga2.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,23 +234,22 @@
         generations.
       metadata_namespace: Metadata namespace to use.
       seed: Random seed.
 
     Returns:
       NSGA2 Designer.
     """
-    del seed
     super().__init__(
         numpy_populations.PopulationConverter(
             problem.search_space,
             problem.metric_information,
             metadata_ns=metadata_namespace,
         ),
-        numpy_populations.UniformRandomSampler(problem.search_space),
+        numpy_populations.UniformRandomSampler(problem.search_space, seed=seed),
         NSGA2Survival(
             population_size,
             ranking_fn=ranking_fn,
             eviction_limit=eviction_limit,
         ),
-        adaptation=numpy_populations.LinfMutation(),
+        adaptation=numpy_populations.LinfMutation(seed=seed),
         first_survival_after=first_survival_after,
     )
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/evolution/nsga2_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/evolution/nsga2_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
   ])
 
   algorithm = nsga2.NSGA2Designer(
       problem,
       population_size,
       first_survival_after=population_size,
       eviction_limit=eviction_limit,
+      seed=0,
   )
   return algorithm
 
 
 class Nsga2Test(absltest.TestCase):
 
   def test_survival_by_pareto_rank(self):
@@ -206,10 +207,38 @@
     ys = algorithm.population.ys
     pareto = algorithm.population[nsga2._pareto_rank(ys) == 0]
     logging.info('Pareto frontier %s %s', pareto.xs, pareto.ys)
 
     # Smoke test dump-load.
     algorithm.load(dumped)
 
+  def test_seeding(self):
+    algorithm_1 = nsga2_on_all_types(10)
+    algorithm_2 = nsga2_on_all_types(10)
+
+    self.assertEqual(algorithm_1.suggest(10), algorithm_2.suggest(10))
+
+    completed_trials = []
+
+    for tid in range(1, 11):
+      trial = vz.Trial(id=tid)
+
+      trial.complete(
+          vz.Measurement({
+              'm1': np.random.random(),
+              'm2': np.random.random(),
+              's1': np.random.random(),
+              's2': np.random.random(),
+          })
+      )
+
+      completed_trials.append(trial)
+
+    trials = vza.CompletedTrials(completed_trials)
+    algorithm_1.update(trials, vza.ActiveTrials())
+    algorithm_2.update(trials, vza.ActiveTrials())
+
+    self.assertEqual(algorithm_1.suggest(10), algorithm_2.suggest(10))
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/evolution/numpy_populations.py` & `google-vizier-0.1.5/vizier/_src/algorithms/evolution/numpy_populations.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,38 +28,41 @@
 from vizier.utils import json_utils
 
 
 # TODO: Use a byte encoding instead of JSON.
 
 
 def _filter_and_split(
-    metrics: Collection[vz.MetricInformation]
+    metrics: Collection[vz.MetricInformation],
 ) -> Tuple[List[vz.MetricInformation], List[vz.MetricInformation]]:
   """Choose objective and safety metrics and split.
 
   Args:
     metrics:
 
   Returns:
     Tuple of objective and safety metrics.
   """
   metrics_by_type = collections.defaultdict(list)
   for metric in metrics:
     metrics_by_type[metric.type].append(metric)
 
-  return (metrics_by_type[vz.MetricType.OBJECTIVE],
-          metrics_by_type[vz.MetricType.SAFETY])
+  return (
+      metrics_by_type[vz.MetricType.OBJECTIVE],
+      metrics_by_type[vz.MetricType.SAFETY],
+  )
 
 
 def _concat(a1: np.ndarray, a2: np.ndarray) -> np.ndarray:
   return np.concatenate([a1, a2], axis=0)
 
 
-def _shape_equals(instance_to_shape: Callable[[Any],
-                                              Collection[Optional[int]]]):
+def _shape_equals(
+    instance_to_shape: Callable[[Any], Collection[Optional[int]]]
+):
   """Creates a shape validator for attr.
 
   For example, _shape_equals(lambda s : [3, None]) validates that the shape has
   length 2 and its first element is 3.
 
   Args:
     instance_to_shape: Takes instance as input and returns the desired shape for
@@ -77,16 +80,18 @@
         return False
       for s1, s2 in zip(value.shape, shape):
         if (s2 is not None) and (s1 != s2):
           return False
       return True
 
     if not _validator_boolean():
-      raise ValueError(f'{attribute.name} has shape {value.shape} '
-                       f'which does not match the expected shape {shape}')
+      raise ValueError(
+          f'{attribute.name} has shape {value.shape} '
+          f'which does not match the expected shape {shape}'
+      )
 
   return validator
 
 
 @attr.define(frozen=True, init=False)
 class Offspring(serializable.Serializable):
   """Offspring which corresponds to trial suggestions.
@@ -96,32 +101,40 @@
     generations: The number of changes this gene went through.
     ids: Identifier for the gene. Can be used to track the "family tree" created
       from the execution of an evolutionary algorithm. For example, when a new
       offspring is sampled, it is assigned a new id and its successors all carry
       the same id.
   """
 
-  xs: np.ndarray = attr.field(validator=[
-      attr.validators.instance_of(np.ndarray),
-      _shape_equals(lambda s: [len(s), None])
-  ])
-  ids: np.ndarray = attr.field(validator=[
-      attr.validators.instance_of(np.ndarray),
-      _shape_equals(lambda s: [len(s)])
-  ])
-
-  generations: np.ndarray = attr.field(validator=[
-      attr.validators.instance_of(np.ndarray),
-      _shape_equals(lambda s: [len(s)])
-  ])
-
-  def __init__(self,
-               xs: np.ndarray,
-               ids: Optional[np.ndarray] = None,
-               generations: Optional[np.ndarray] = None):
+  xs: np.ndarray = attr.field(
+      validator=[
+          attr.validators.instance_of(np.ndarray),
+          _shape_equals(lambda s: [len(s), None]),
+      ]
+  )
+  ids: np.ndarray = attr.field(
+      validator=[
+          attr.validators.instance_of(np.ndarray),
+          _shape_equals(lambda s: [len(s)]),
+      ]
+  )
+
+  generations: np.ndarray = attr.field(
+      validator=[
+          attr.validators.instance_of(np.ndarray),
+          _shape_equals(lambda s: [len(s)]),
+      ]
+  )
+
+  def __init__(
+      self,
+      xs: np.ndarray,
+      ids: Optional[np.ndarray] = None,
+      generations: Optional[np.ndarray] = None,
+  ):
     if generations is None:
       generations = np.zeros([xs.shape[0]])
     if ids is None:
       ids = np.zeros([xs.shape[0]])
 
     self.__attrs_init__(xs, ids, generations)
 
@@ -129,16 +142,18 @@
     return self.generations.shape[0]
 
   def __getitem__(self, index: Any) -> 'Offspring':
     return Offspring(self.xs[index], self.ids[index], self.generations[index])
 
   def __add__(self, other: 'Offspring') -> 'Offspring':
     return Offspring(
-        _concat(self.xs, other.xs), _concat(self.ids, other.ids),
-        _concat(self.generations, other.generations))
+        _concat(self.xs, other.xs),
+        _concat(self.ids, other.ids),
+        _concat(self.generations, other.generations),
+    )
 
   @classmethod
   def load(cls: Type['Offspring'], metadata: vz.Metadata) -> 'Offspring':
     encoded = metadata.get('values', cls=str)
     try:
       decoded = json.loads(encoded, object_hook=json_utils.numpy_hook)
     except Exception as e:
@@ -165,59 +180,78 @@
       metrics. The values should be pre-processed such that the constraint is to
       get them greater than zero.
     ages: The number of selection phases that each entity survived for.
     generations: The number of ancestors of each entity.
     ids: Identifier for the gene aka "family name".
     trial_ids: Trial ids. For debugging and testing only.
   """
-  xs: np.ndarray = attr.field(validator=[
-      attr.validators.instance_of(np.ndarray),
-      _shape_equals(lambda s: [len(s), None])
-  ])
-  ys: np.ndarray = attr.field(validator=[
-      attr.validators.instance_of(np.ndarray),
-      _shape_equals(lambda s: [len(s), None])
-  ])
-  cs: np.ndarray = attr.field(validator=[
-      attr.validators.instance_of(np.ndarray),
-      _shape_equals(lambda s: [len(s), None])
-  ])
-  ages: np.ndarray = attr.field(validator=[
-      attr.validators.instance_of(np.ndarray),
-      _shape_equals(lambda s: [len(s)])
-  ])
-  generations: np.ndarray = attr.field(validator=[
-      attr.validators.instance_of(np.ndarray),
-      _shape_equals(lambda s: [len(s)])
-  ])
-  ids: np.ndarray = attr.field(validator=[
-      attr.validators.instance_of(np.ndarray),
-      _shape_equals(lambda s: [len(s)])
-  ])
-  trial_ids: np.ndarray = attr.field(validator=[
-      attr.validators.instance_of(np.ndarray),
-      _shape_equals(lambda s: [len(s)])
-  ])
+
+  xs: np.ndarray = attr.field(
+      validator=[
+          attr.validators.instance_of(np.ndarray),
+          _shape_equals(lambda s: [len(s), None]),
+      ]
+  )
+  ys: np.ndarray = attr.field(
+      validator=[
+          attr.validators.instance_of(np.ndarray),
+          _shape_equals(lambda s: [len(s), None]),
+      ]
+  )
+  cs: np.ndarray = attr.field(
+      validator=[
+          attr.validators.instance_of(np.ndarray),
+          _shape_equals(lambda s: [len(s), None]),
+      ]
+  )
+  ages: np.ndarray = attr.field(
+      validator=[
+          attr.validators.instance_of(np.ndarray),
+          _shape_equals(lambda s: [len(s)]),
+      ]
+  )
+  generations: np.ndarray = attr.field(
+      validator=[
+          attr.validators.instance_of(np.ndarray),
+          _shape_equals(lambda s: [len(s)]),
+      ]
+  )
+  ids: np.ndarray = attr.field(
+      validator=[
+          attr.validators.instance_of(np.ndarray),
+          _shape_equals(lambda s: [len(s)]),
+      ]
+  )
+  trial_ids: np.ndarray = attr.field(
+      validator=[
+          attr.validators.instance_of(np.ndarray),
+          _shape_equals(lambda s: [len(s)]),
+      ]
+  )
 
   def __len__(self) -> int:
     return self.ys.shape[0]
 
   def __getitem__(
       self,
       index: Any,
      
   ) -> 'Population':
     return Population(**{k: v[index] for k, v in attr.asdict(self).items()})
 
   def __add__(self, other: 'Population') -> 'Population':
     return Population(
-        _concat(self.xs, other.xs), _concat(self.ys, other.ys),
-        _concat(self.cs, other.cs), _concat(self.ages, other.ages),
+        _concat(self.xs, other.xs),
+        _concat(self.ys, other.ys),
+        _concat(self.cs, other.cs),
+        _concat(self.ages, other.ages),
         _concat(self.generations, other.generations),
-        _concat(self.ids, other.ids), _concat(self.trial_ids, other.trial_ids))
+        _concat(self.ids, other.ids),
+        _concat(self.trial_ids, other.trial_ids),
+    )
 
   @classmethod
   def recover(cls, metadata: vz.Metadata) -> 'Population':
     encoded = metadata.get('values', default='', cls=str)
     try:
       decoded = json.loads(encoded, object_hook=json_utils.numpy_hook)
     except json.JSONDecodeError as e:
@@ -227,126 +261,152 @@
   def dump(self) -> vz.Metadata:
     encoded = json.dumps(attr.asdict(self), cls=json_utils.NumpyEncoder)
     return vz.Metadata({'values': encoded})
 
   def empty_like(self) -> 'Population':
     """Creates an empty population that has the same shape as this."""
 
-    return Population(**{
-        k: np.zeros([0] + list(v.shape[1:]))
-        for k, v in attr.asdict(self).items()
-    })
+    return Population(
+        **{
+            k: np.zeros([0] + list(v.shape[1:]))
+            for k, v in attr.asdict(self).items()
+        }
+    )
 
 
 def _create_parameter_converters(
-    search_space: vz.SearchSpace
+    search_space: vz.SearchSpace,
 ) -> Collection[converters.DefaultModelInputConverter]:
   """Returns parameter converters."""
   if search_space.is_conditional:
     raise ValueError('Cannot handle conditional search space!')
 
   def create_input_converter(
-      pc: vz.ParameterConfig) -> converters.DefaultModelInputConverter:
+      pc: vz.ParameterConfig,
+  ) -> converters.DefaultModelInputConverter:
     return converters.DefaultModelInputConverter(
-        pc, scale=True, max_discrete_indices=0, onehot_embed=True)
+        pc, scale=True, max_discrete_indices=0, onehot_embed=True
+    )
 
   return [create_input_converter(pc) for pc in search_space.parameters]
 
 
 def _create_metric_converter(
-    mc: vz.MetricInformation) -> converters.DefaultModelOutputConverter:
+    mc: vz.MetricInformation,
+) -> converters.DefaultModelOutputConverter:
   # TODO: Do something other than raising an error
   return converters.DefaultModelOutputConverter(
       mc,
       flip_sign_for_minimization_metrics=True,
       shift_safe_metrics=True,
-      raise_errors_for_missing_metrics=True)
+      raise_errors_for_missing_metrics=True,
+  )
 
 
 class PopulationConverter(templates.PopulationConverter):
   """Population converter."""
 
-  def __init__(self,
-               search_space: vz.SearchSpace,
-               metrics: Collection[vz.MetricInformation],
-               *,
-               metadata_ns: str = 'population'):
+  def __init__(
+      self,
+      search_space: vz.SearchSpace,
+      metrics: Collection[vz.MetricInformation],
+      *,
+      metadata_ns: str = 'population',
+  ):
     self._objective_metrics, self._safe_metrics = _filter_and_split(metrics)
     self._num_objective_metrics = len(self._objective_metrics)
     self._num_safe_metrics = len(self._safe_metrics)
     self._metrics = self._objective_metrics + self._safe_metrics
     self._metadata_ns = metadata_ns
 
     self._trial_converter = converters.DefaultTrialConverter(
         _create_parameter_converters(search_space),
-        [_create_metric_converter(mc) for mc in self._metrics])
+        [_create_metric_converter(mc) for mc in self._metrics],
+    )
     self._empty_feature_dict = converters.DictOf2DArrays(
-        self._trial_converter.to_features([]))
+        self._trial_converter.to_features([])
+    )
 
   def to_suggestions(  # pytype: disable=signature-mismatch  # overriding-parameter-type-checks
-      self, offsprings: Offspring) -> Collection[vz.TrialSuggestion]:
+      self, offsprings: Offspring
+  ) -> Collection[vz.TrialSuggestion]:
     parameters_list = self._trial_converter.to_parameters(
-        self._empty_feature_dict.dict_like(offsprings.xs))
+        self._empty_feature_dict.dict_like(offsprings.xs)
+    )
     suggestions = [vz.TrialSuggestion(p) for p in parameters_list]
     for idx, t in enumerate(suggestions):
-      t.metadata.ns(self._metadata_ns).update(offsprings[idx:idx + 1].dump())
+      t.metadata.ns(self._metadata_ns).update(offsprings[idx : idx + 1].dump())
     return suggestions
 
   def _empty_offsprings(self) -> Offspring:
-    return Offspring(self._empty_feature_dict.asarray(), np.zeros([0]),
-                     np.zeros([0]))
+    return Offspring(
+        self._empty_feature_dict.asarray(), np.zeros([0]), np.zeros([0])
+    )
 
   def to_population(self, completed: Sequence[vz.CompletedTrial]) -> Population:
     """Converts trials into population. Accepts an empty list."""
     offsprings = self._empty_offsprings()  # create empty
     # Each Trial should contain its genes as metadata. (Note that
     # genes-to-trial mapping is many-to-one). We try to load the genes.
     for t in completed:
       metadata = t.metadata.ns(self._metadata_ns)
       try:
         offsprings += Offspring.load(metadata)
       except serializable.DecodeError:
         # Upon failure, arbitrarily choose one set of genes that map to the
         # current trial.
         offsprings += Offspring(
-            converters.DictOf2DArrays(self._trial_converter.to_features(
-                [t])).asarray(), np.zeros([1]), np.zeros([1]))
+            converters.DictOf2DArrays(
+                self._trial_converter.to_features([t])
+            ).asarray(),
+            np.zeros([1]),
+            np.zeros([1]),
+        )
 
     ys = self._trial_converter.to_labels_array(completed)
-    return Population(offsprings.xs, ys[:, :self._num_objective_metrics],
-                      ys[:, self._num_objective_metrics:],
-                      np.zeros([ys.shape[0]]), offsprings.generations,
-                      offsprings.ids,
-                      np.asarray([t.id for t in completed], dtype=np.int32))
+    return Population(
+        offsprings.xs,
+        ys[:, : self._num_objective_metrics],
+        ys[:, self._num_objective_metrics :],
+        np.zeros([ys.shape[0]]),
+        offsprings.generations,
+        offsprings.ids,
+        np.asarray([t.id for t in completed], dtype=np.int32),
+    )
 
 
 class UniformRandomSampler(templates.Sampler[Offspring]):
   """Generates uniformly random samples."""
 
-  def __init__(self, search_space: vz.SearchSpace):
+  def __init__(self, search_space: vz.SearchSpace, seed: Optional[int] = None):
     if search_space.is_conditional:
       raise ValueError(f'{type(self)} does not support conditional spaces.')
     self._trial_converter = converters.DefaultTrialConverter(
-        _create_parameter_converters(search_space))
+        _create_parameter_converters(search_space)
+    )
     self._dimension = sum(
-        v[-1] for v in self._trial_converter.features_shape.values())
+        v[-1] for v in self._trial_converter.features_shape.values()
+    )
     self._num_samples = 0
+    self._rng = np.random.RandomState(seed)
 
   def sample(self, count: int) -> Offspring:
     self._num_samples += count
     return Offspring(
-        np.random.random([count, self._dimension]),
-        ids=np.arange(self._num_samples - count, self._num_samples))
+        self._rng.random([count, self._dimension]),
+        ids=np.arange(self._num_samples - count, self._num_samples),
+    )
 
 
 class LinfMutation(templates.Mutation):
   """L-inf Mutations. Values are assumed to be in [0,1] range."""
 
-  def __init__(self, norm: float = .1):
+  def __init__(self, norm: float = 0.1, seed: Optional[int] = None):
     self._norm = norm
+    self._rng = np.random.RandomState(seed)
 
   def mutate(self, population: Population, count: int) -> Offspring:
     """Perturb by a uniform sample from l-inf ball.
 
     If the perturbation pushes a coordinate out of [0, 1] range, it "wraps
     around". This is likely suboptimal if optimum is at or near the boundary.
 
@@ -356,14 +416,14 @@
 
     Returns:
       Offsprings.
     """
     # Mutate and truncate to [-5, 1.5] range. Perturbations should generally
     # NOT generate values outside this range.
     arr = population.xs.copy()
-    arr += np.random.uniform(-self._norm, self._norm, arr.shape)
-    arr = np.maximum(np.minimum(arr, 1.5), -.5)
+    arr += self._rng.uniform(-self._norm, self._norm, arr.shape)
+    arr = np.maximum(np.minimum(arr, 1.5), -0.5)
 
     # When the value is outside [0, 1] range, wrap around the limits.
     # -0.2 becomes 0.8, 1.2 becomes 0.2, etc.
     arr = np.where(arr < 0, 1 + arr, np.where(arr > 1, arr - 1, arr))
     return Offspring(arr, population.ids, population.generations + 1)
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/evolution/numpy_populations_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/evolution/numpy_populations_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/evolution/templates.py` & `google-vizier-0.1.5/vizier/_src/algorithms/evolution/templates.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/optimizers/__init__.py` & `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/optimizers/base.py` & `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/optimizers/designer_optimizer.py` & `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/designer_optimizer.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/optimizers/designer_optimizer_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/designer_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_optimizer_convergence_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,39 +15,43 @@
 from __future__ import annotations
 
 """Tests for eagle_optimizer."""
 
 import logging
 from typing import Optional
 
+import jax
+from jax import numpy as jnp
 import numpy as np
 from vizier import pyvizier as vz
 from vizier._src.algorithms.optimizers import eagle_strategy
 from vizier._src.algorithms.optimizers import random_vectorized_optimizer as rvo
 from vizier._src.algorithms.optimizers import vectorized_base as vb
 from vizier._src.algorithms.testing import comparator_runner
+from vizier._src.jax import types
 from vizier.pyvizier import converters
 
 from absl.testing import absltest
 from absl.testing import parameterized
 
 
-def randomize_array(converter: converters.TrialToArrayConverter) -> np.ndarray:
+def randomize_array(converter: converters.TrialToArrayConverter) -> jax.Array:
   """Generate a random array of features to be used as score_fn shift."""
   features_arrays = []
   for spec in converter.output_specs:
     if spec.type == converters.NumpyArraySpecType.ONEHOT_EMBEDDING:
       dim = spec.num_dimensions - spec.num_oovs
       features_arrays.append(
-          np.eye(spec.num_dimensions)[np.random.randint(0, dim)])
+          jnp.eye(spec.num_dimensions)[np.random.randint(0, dim)]
+      )
     elif spec.type == converters.NumpyArraySpecType.CONTINUOUS:
       features_arrays.append(np.random.uniform(0.4, 0.6, size=(1,)))
     else:
       raise ValueError(f'The type {spec.type} is not supported!')
-  return np.hstack(features_arrays)
+  return jnp.hstack(features_arrays)
 
 
 def create_continuous_problem(
     n_features: int,
     problem: Optional[vz.ProblemStatement] = None) -> vz.ProblemStatement:
   if not problem:
     problem = vz.ProblemStatement()
@@ -73,22 +77,22 @@
 def create_mix_problem(n_features: int,
                        categorical_dim: int = 8) -> vz.ProblemStatement:
   problem = create_continuous_problem(n_features // 2)
   return create_categorical_problem(n_features // 2, categorical_dim, problem)
 
 
 # TODO: Change to bbob functions when they can support batching.
-def sphere(x: np.ndarray) -> np.ndarray:
-  return -np.sum(np.square(x), axis=-1)
+def sphere(x: types.Array) -> jax.Array:
+  return -jnp.sum(jnp.square(x), axis=-1)
 
 
-def rastrigin_d10(x: np.ndarray) -> np.ndarray:
-  return 10 * np.sum(
-      np.cos(2 * np.pi * x), axis=-1) - np.sum(
-          np.square(x), axis=-1)
+def rastrigin_d10(x: types.Array) -> jax.Array:
+  return 10 * jnp.sum(jnp.cos(2 * np.pi * x), axis=-1) - jnp.sum(
+      jnp.square(x), axis=-1
+  )
 
 
 class EagleOptimizerConvegenceTest(parameterized.TestCase):
   """Test optimizing an acquisition functions using vectorized Eagle Strategy.
   """
 
   @absltest.skip("Test takes too long externally.")
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/optimizers/eagle_param_handler.py` & `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_param_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from __future__ import annotations
 
 """Utils for vectorized eagle strategy."""
 
 from typing import Optional
 
 import attr
-import numpy as np
+import jax
+from jax import numpy as jnp
 from vizier.pyvizier import converters
 
 
 @attr.define(kw_only=True)
 class EagleParamHandler:
   """Vectorized eagle strategy utils.
 
@@ -32,16 +33,14 @@
 
   Attributes:
     converter: The converter used to convert the original search space. It's
       used to get metadata on the different parameters and attribute the feature
       indices to them.
     config: The eagle strategy configuration used to set the perturbation
       factors for CATEGORICAL features.
-    rng: A numpy random generator to generate parameter-aware features, and
-      sample categorical features.
     categorical_perturbation_factor: The perturbation factor for categorical
       features.
     pure_categorical_perturbation_factor: The perturbation factor when all
       features are categorical.
     n_features: The total number of feature indices.
     n_categorical: The number of CATEGORICAL associated indices.
     has_categorical: A flag indicating if at least one feature is categorical.
@@ -57,25 +56,24 @@
     _oov_mask: A 1D array (n_features,) with 1s in the non-oov indices. The
       array is used to generate random features with 0 value in the OOV indices.
     _epsilon: A small value used in tie-breaker
   """
   converter: converters.TrialToArrayConverter
   categorical_perturbation_factor: float
   pure_categorical_perturbation_factor: float
-  rng: np.random.Generator
   # Public variables created by the class
   n_features: int = attr.field(init=False)
   n_categorical: int = attr.field(init=False)
   has_categorical: bool = attr.field(init=False)
   all_features_categorical: bool = attr.field(init=False)
   # Internal variables
-  _categorical_params_mask: np.ndarray = attr.field(init=False)
-  _categorical_mask: np.ndarray = attr.field(init=False)
-  _tiebreak_array: np.ndarray = attr.field(init=False)
-  _oov_mask: Optional[np.ndarray] = attr.field(init=False, default=None)
+  _categorical_params_mask: jax.Array = attr.field(init=False)
+  _categorical_mask: jax.Array = attr.field(init=False)
+  _tiebreak_array: jax.Array = attr.field(init=False)
+  _oov_mask: Optional[jax.Array] = attr.field(init=False, default=None)
   _epsilon: float = attr.field(init=False, default=1e-5)
 
   def __attrs_post_init__(self):
     self._init_utils()
 
   def _init_utils(self):
     """Initialize the utility class and cache arrays for repeated use."""
@@ -99,41 +97,43 @@
     self.has_categorical = self.n_categorical > 0
     self.all_features_categorical = self.n_features == self.n_categorical
     if self.has_categorical:
       self._create_categorical_masks()
 
   def _create_categorical_masks(self):
     """Create the categorical masks."""
-    self._categorical_params_mask = np.zeros(
-        (self.n_categorical, self.n_features))
-    self._oov_mask = np.ones((self.n_features,))
+    categorical_params_mask = jnp.zeros((self.n_categorical, self.n_features))
+    oov_mask = jnp.ones((self.n_features,))
     row = 0
     col = 0
     # Create a flag to indicate if the converter uses OOV padding. If none of
     # the CATEGORICAL params use padding the 'oov_mask' is set to None.
     is_pad_oov = False
     for spec in self.converter.output_specs:
       if spec.type == converters.NumpyArraySpecType.ONEHOT_EMBEDDING:
         n_dim = spec.num_dimensions
-        self._categorical_params_mask[row, col:col + n_dim] = 1.0
+        categorical_params_mask = categorical_params_mask.at[
+            row, col : col + n_dim
+        ].set(1.0)
         if spec.num_oovs:
-          self._oov_mask[col + n_dim - 1] = 0.0
+          oov_mask = oov_mask.at[col + n_dim - 1].set(0.0)
           is_pad_oov = True
         row += 1
         col += n_dim
       else:
         col += 1
-    if not is_pad_oov:
-      self._oov_mask = None
 
-    self._tiebreak_array = np.array(
-        [-self._epsilon * (i + 1) for i in range(self.n_features)])
-    self._categorical_mask = np.sum(self._categorical_params_mask, axis=0)
-
-  def sample_categorical(self, features: np.ndarray) -> np.ndarray:
+    self._oov_mask = oov_mask if is_pad_oov else None
+    self._tiebreak_array = -self._epsilon * jnp.arange(1, self.n_features + 1)
+    self._categorical_mask = jnp.sum(categorical_params_mask, axis=0)
+    self._categorical_params_mask = categorical_params_mask
+
+  def sample_categorical(
+      self, features: jax.Array, seed: jax.random.KeyArray
+  ) -> jax.Array:
     """Sample categorical features.
 
     The categorical sampling is used before returning suggestion to ensure that
     only actual categorical values are suggested. Non categorical features are
     left unchanged.
 
     For example: If 'features' has one categorical parameter with 3 values and
@@ -150,73 +150,73 @@
     6. Find the minimum index that its CDF > uniform. See code around
     'sampled_categorical_params' below for more detail and for why we need to
     add the tie-breaking array values.
     7. Flatten each row sampled values and combine with original features.
 
     Arguments:
       features: (batch_size, n_features)
+      seed: Random seed.
 
     Returns:
       The features with sampled categorical parameters. (batch_size ,n_features)
     """
     if not self.has_categorical:
       return features
     batch_size = features.shape[0]
-    # Broadcast features to: (batch_size, n_categorical, n_features)
-    expanded_shape = (self.n_categorical,) + features.shape
-    expanded_features = np.swapaxes(
-        np.broadcast_to(features, expanded_shape), 1, 0)
     # Mask each row (which represents a categorical param) to remove values in
     # indices that aren't associated with the parameter indices.
-    param_features = expanded_features * self._categorical_params_mask
+    param_features = features[:, jnp.newaxis, :] * self._categorical_params_mask
     # Create probabilities from non-normalized parameter features values.
-    probs = param_features / np.sum(param_features, axis=-1, keepdims=True)
+    probs = param_features / jnp.sum(param_features, axis=-1, keepdims=True)
     # Generate random uniform values to use for sampling.
     # TODO: Pre-compute random values in batch to improve performance.
-    unifs = self.rng.uniform(0.0, 1.0, size=(batch_size, self.n_categorical))
+    unifs = jax.random.uniform(seed, shape=(batch_size, self.n_categorical, 1))
     # Find the locations of the indices that exceed random values.
-    locs = np.cumsum(probs, axis=-1) >= np.expand_dims(unifs, axis=-1)
+    locs = jnp.cumsum(probs, axis=-1) >= unifs
     # Multiply by 'categorical_mask' to mask off cumsum in non-categorical
     # indices, and add 'tiebreak_mask' to find the first index.
     masked_locs = locs * self._categorical_params_mask + self._tiebreak_array
     # Generate the samples so that each parameter features has a single 1 value.
-    sampled_categorical_params = np.float_(
-        np.int_(masked_locs / np.max(masked_locs, axis=-1, keepdims=True)))
+    sampled_categorical_params = jnp.trunc(
+        masked_locs / jnp.max(masked_locs, axis=-1, keepdims=True)
+    )
     # Flatten all the categories features to dimension (batch_size, n_features)
-    sampled_features = np.sum(sampled_categorical_params, axis=1)
+    sampled_features = jnp.sum(sampled_categorical_params, axis=1)
     # Mask categorical features and add the new sampled categorical values.
     return sampled_features + features * (1 - self._categorical_mask)
 
-  def random_features(self, batch_size: int, n_features: int) -> np.ndarray:
+  def random_features(
+      self, batch_size: int, seed: jax.random.KeyArray
+  ) -> jax.Array:
     """Create random features with uniform distribution.
 
     In case there are CATEGORICAL features with OOV we use the 'oov_mask' which
     is 1D numpy array (n_features,) with 0s in OOV indices and otherwise 1s.
     After multiplying (and broadcasting) the randomly generated features with
     the mask we're guaranteed that no features will be created in OOV indices.
     Therefore when mutating fireflies' features (index by index), the final
     suggested features will also have 0s in the OOV indices as desired.
 
     Arguments:
       batch_size:
-      n_features:
+      seed: Random seed.
 
     Returns:
       The random features with out of vocabulary indices zeroed out.
     """
-    size = (batch_size, n_features)
+    size = (batch_size, self.n_features)
     if self._oov_mask is not None:
       # Don't create random values for CATEGORICAL features OOV indices.
       # Broadcasting: (batch_size, n_features) x (n_features,)
-      return self.rng.uniform(0.0, 1.0, size=size) * self._oov_mask
+      return jax.random.uniform(seed, shape=size) * self._oov_mask
     else:
-      return self.rng.uniform(0.0, 1.0, size=size)
+      return jax.random.uniform(seed, shape=size)
 
   @property
-  def perturbation_factors(self) -> np.ndarray:
+  def perturbation_factors(self) -> jax.Array:
     """Create the perturbations factors.
 
     Returns:
       Array of perturbation factors (n_features,)
     """
     perturbation_factors = []
 
@@ -228,8 +228,8 @@
       for spec in self.converter.output_specs:
         if spec.type == converters.NumpyArraySpecType.ONEHOT_EMBEDDING:
           perturbation_factors.extend([self.categorical_perturbation_factor] *
                                       spec.num_dimensions)
 
         elif spec.type == converters.NumpyArraySpecType.CONTINUOUS:
           perturbation_factors.append(1.0)
-    return np.array(perturbation_factors)
+    return jnp.array(perturbation_factors)
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/optimizers/eagle_strategy.py` & `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_strategy.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 parameter types (categorical, discrete, integer), and treat them uniquely when
 computing distance, adding pertrubation, and mutating fireflies.
 
 For more details, see the linked paper.
 
 OSS Vizier Implementation Summary
 =================================
-The firefly are stored in three Numpy arrays: features, rewards, perturbations.
+The fireflies are stored in three JAX arrays: features, rewards, perturbations.
 Each iteration we mutate 'batch_size' fireflies to generate new features. The
 new features are evaluated on the objective function to obtain their associated
 rewards and update the pool where improvement was obtained, and decrease the
 perturbation factor otherwise.
 
 If the firefly's perturbation reaches the `perturbation_lower_bound` threshold
 it's removed and replaced with new random features.
@@ -62,31 +62,43 @@
 Example
 =======
 # Construct the optimizer with eagle strategy.
 optimizer = VectorizedOptimizer(
     VectorizedEagleStrategyFactory(),
 )
 # Run the optimization.
-optimizer.optimize(problem_statement, objective_function)
-
-# Access the best features and reward.
-best_reward, best_parameters = optimizer.best_results
+trials = optimizer.optimize(problem_statement, objective_function)
 """
+# pylint: disable=g-long-lambda
 
+import enum
 import logging
-from typing import Optional, Literal
+import math
+from typing import Optional, Tuple
 
 import attr
-import numpy as np
+import chex
+import jax
+from jax import numpy as jnp
 from vizier._src.algorithms.optimizers import eagle_param_handler
 from vizier._src.algorithms.optimizers import vectorized_base as vb
+from vizier._src.jax import types
 from vizier.pyvizier import converters
 
 
-@attr.define
+@enum.unique
+class MutateNormalizationType(enum.IntEnum):
+  """The force normalization mode. Use IntEnum for JIT compatibility."""
+
+  MEAN = 0
+  RANDOM = 1
+  UNNORMALIZED = 2
+
+
+@chex.dataclass(frozen=True)
 class EagleStrategyConfig:
   """Eagle Strategy optimizer config.
 
   Attributes:
     visibility: The sensetivity to distance between flies when computing pulls.
     gravity: The maximum amount of attraction pull.
     negative_gravity: The maximum amount of repulsion pull.
@@ -95,14 +107,15 @@
     pure_categorical_perturbation_factor: A factor on purely categorical space.
     perturbation_lower_bound: The threshold below flies are removed from pool.
     penalize_factor: The perturbation decrease for unsuccessful flies.
     pool_size_exponent: An exponent for computing pool size based on search
       space size.
     pool_size: An optional way to set the pool size. If not 0, this takes
       precedent over the programatic pool size computation.
+    max_pool_size: Ceiling on pool size.
     mutate_normalization_type: The type of force mutation normalizatoin used for
       damping down the force intensity to stay within reasonable bounds.
     normalization_scale: A mutation force scale-factor to control intensity.
     prior_trials_pool_pct: The percentage of the pool populated by prior trials.
   """
 
   # Visibility
@@ -116,16 +129,19 @@
   pure_categorical_perturbation_factor: float = 30
   # Penalty
   perturbation_lower_bound: float = 7e-5
   penalize_factor: float = 7e-1
   # Pool size
   pool_size_exponent: float = 1.2
   pool_size: int = 0
+  max_pool_size: int = 100
   # Force normalization mode
-  mutate_normalization_type: str = "mean"
+  mutate_normalization_type: MutateNormalizationType = (
+      MutateNormalizationType.MEAN
+  )
   # Multiplier factor when using normalized modes
   normalization_scale: float = 0.5
   # The percentage of the firefly pool to be populated with prior trials
   prior_trials_pool_pct: float = 0.96
 
 
 @attr.define(frozen=True)
@@ -133,486 +149,568 @@
   """Eagle strategy factory."""
 
   eagle_config: EagleStrategyConfig = attr.field(factory=EagleStrategyConfig)
 
   def __call__(
       self,
       converter: converters.TrialToArrayConverter,
-      suggestion_batch_size: int = 5,
-      seed: Optional[int] = None,
-      prior_features: Optional[np.ndarray] = None,
-      prior_rewards: Optional[np.ndarray] = None,
+      suggestion_batch_size: Optional[int] = None,
   ) -> "VectorizedEagleStrategy":
     """Create a new vectorized eagle strategy.
 
     In order to create the strategy a converter has to be passed, which the
     strategy will then store a pointer to. The strategy uses the converter to
     get information about the original Vizier Parameters and their relation to
     the array indices (which index belong to which Vizier Parameter). This is
     useful for example for sampling CATEGORICAL features.
 
     Arguments:
       converter: TrialToArrayConverter that matches the converter used in
         computing the objective / acuisition function.
       suggestion_batch_size: The batch_size of the returned suggestion array.
-      seed: The seed to input into the random generator.
-      prior_features: The prior features for populating the pool.
-        (n_prior_candidates, n_features)
-      prior_rewards:  The prior rewards for populating the pool.
-        (n_prior_candidates,)
 
     Returns:
       A new instance of VectorizedEagleStrategy.
     """
     return VectorizedEagleStrategy(
         converter=converter,
         config=self.eagle_config,
         batch_size=suggestion_batch_size,
-        seed=seed,
-        prior_features=prior_features,
-        prior_rewards=prior_rewards,
     )
 
 
-# TODO: Create jit-compatible JAX version.
+@chex.dataclass(frozen=True)
+class VectorizedEagleStrategyState:
+  """Container for Eagle strategy state."""
+
+  iterations: jax.Array  # Scalar integer.
+  features: jax.Array  # Shape (pool_size, n_features).
+  rewards: jax.Array  # Shape (pool_size,).
+  best_reward: jax.Array  # Scalar float.
+  perturbations: jax.Array  # Shape (pool_size,).
+
+
 @attr.define
 class VectorizedEagleStrategy(vb.VectorizedStrategy):
   """Eagle strategy implementation for maximization problem based on Numpy.
 
   Attributes:
     converter: The converter used for the optimization problem.
     config: The Eagle strategy configuration.
     n_features: The number of features.
     batch_size: The number of suggestions generated at each suggestion call.
-    prior_features: The prior features to be used for seeding the pool. When the
-      optimizer is used to optimize a designer's acquisition function, the prior
-      features are the previous designer suggestions provided in the ordered
-      they were suggested. Shape: (n_prior_trials, n_features).
-    prior_rewards: The associated prior rewards of the prior features.
-      Shape: (n_prior_trials,)
-    seed: The seed to generate random values.
     pool_size: The total number of flies in the pool.
-    _features: Array with dimensions (suggestion_count, feature_count) storing
-      the firefly features.
-    _rewards: Array with dimensions (suggestion_count,) that for each firefly
-      stores the current (best) associated objective function result.
-    _perturbations: Array with dimensions (suggestion_count,) storing the
-      firefly current perturbations.
-    _batch_id: The current batch index which is in [0, pool_size/batch_size - 1]
-    _batch_slice: The slice of the indices in the current batch.
-    _iterations: The total number of batches suggested.
-    _num_removed_flies: The total number of removed flies (for debugging).
-    _best_results: An Heap storing the best results across all flies.
-    _last_suggested_features: The last features the strategy has suggested.
   """
 
-  converter: converters.TrialToArrayConverter
+  converter: converters.TrialToArrayConverter = attr.field(
+      init=True, repr=False
+  )
   config: EagleStrategyConfig = attr.field(init=True, repr=False)
-  batch_size: int = attr.field(init=True)
-  seed: Optional[int] = attr.field(init=True)
+  batch_size: Optional[int] = attr.field(init=True, default=None)
   pool_size: int = attr.field(init=False)
-  prior_features: Optional[np.ndarray] = attr.field(init=True, default=None)
-  prior_rewards: Optional[np.ndarray] = attr.field(init=True, default=None)
-  # Attributes related to the strategy's state.
-  _features: np.ndarray = attr.field(init=False, repr=False)
-  _rewards: np.ndarray = attr.field(init=False, repr=False)
-  _perturbations: np.ndarray = attr.field(init=False, repr=False)
-  _batch_id: int = attr.field(init=False, repr=False)
-  _batch_slice: slice = attr.field(init=False, repr=False)
-  _iterations: int = attr.field(init=False)
-  _last_suggested_features: np.ndarray = attr.field(init=False, repr=False)
-  _best_reward: float = attr.field(init=False)
   # Attributes related to computations.
-  _num_removed_flies: int = attr.field(init=False, default=0)
   _n_features: int = attr.field(init=False)
-  _perturbation_factors: np.ndarray = attr.field(init=False, repr=False)
+  _perturbation_factors: jax.Array = attr.field(init=False, repr=False)
 
   def __attrs_post_init__(self):
     self._initialize()
     logging.info("Eagle class attributes:\n%s", self)
     logging.info("Eagle configuration:\n%s", self.config)
 
-  def _compute_pool_size(self):
-    """Compute the pool size, and ensures it's a multiply of the batch_size."""
-    raw_pool_size = 10 + int(
-        0.5 * self._n_features
-        + self._n_features**self.config.pool_size_exponent
-    )
-    return int(np.ceil(raw_pool_size / self.batch_size) * self.batch_size)
+  def __hash__(self):
+    # Make this class hashable so it can be a static arg to a JIT-ed function.
+    return hash(id(self))
+
+  def _compute_pool_size(self) -> int:
+    """Compute the pool size, and ensures it's a multiple of the batch_size."""
+    n_params = len(self.converter.output_specs)
+    pool_size = 10 + int(
+        0.5 * n_params + n_params**self.config.pool_size_exponent
+    )
+    pool_size = min(pool_size, self.config.max_pool_size)
+    if self.batch_size is not None:
+      # If the batch_size was set, ensure pool_size is multiply of batch_size.
+      return int(math.ceil(pool_size / self.batch_size) * self.batch_size)
+    else:
+      return pool_size
 
-  def _initialize(self):
+  def _initialize(self) -> None:
     """Initialize the designer state."""
-    self._rng = np.random.default_rng(self.seed)
     self._param_handler = eagle_param_handler.EagleParamHandler(
         converter=self.converter,
-        rng=self._rng,
         categorical_perturbation_factor=self.config.categorical_perturbation_factor,
         pure_categorical_perturbation_factor=self.config.pure_categorical_perturbation_factor,
     )
     self._n_features = self._param_handler.n_features
     if self.config.pool_size > 0:
       # This allow to override the pool size computation.
       self.pool_size = self.config.pool_size
     else:
       self.pool_size = self._compute_pool_size()
     logging.info("Pool size: %d", self.pool_size)
-    if self.batch_size == -1:
+    if self.batch_size is None:
       # This configuration updates all the fireflies in each iteration.
       self.batch_size = self.pool_size
-    self._batch_id = 0
-    self._iterations = 0
-    self._batch_slice = np.s_[0 : self.batch_size]
-    self._perturbations = (
-        np.ones(
-            self.pool_size,
-        )
-        * self.config.perturbation
-    )
-    self._last_suggested_features = None
     self._perturbation_factors = self._param_handler.perturbation_factors
     # Use priors to populate Eagle state
-    if self.prior_features is not None or self.prior_rewards is not None:
-      self._populate_pool_with_prior_trials()
-    else:
-      self._features = self._param_handler.random_features(
-          self.pool_size, self._n_features
+
+  def init_state(
+      self,
+      seed: chex.PRNGKey,
+      prior_features: Optional[chex.Array] = None,
+      prior_rewards: Optional[chex.Array] = None,
+  ) -> VectorizedEagleStrategyState:
+    """Initializes the state."""
+    if prior_features is not None or prior_rewards is not None:
+      init_features = self._populate_pool_with_prior_trials(
+          seed, prior_features, prior_rewards
       )
-    # Rewards are not populated from seed, as they were potentially generated
-    # from a different objective function. New rewards will be obtained.
-    self._rewards = np.ones(
-        self.pool_size,
-    ) * (-np.inf)
-    self._best_reward = -np.inf
-    # Ignore subtracting np.inf - np.inf. See '_compute_scaled_directions' for
-    # explanation on why we ignore warning in this case.
-    np.seterr(invalid="ignore")
+    else:
+      init_features = self._param_handler.random_features(self.pool_size, seed)
+    return VectorizedEagleStrategyState(
+        iterations=jnp.array(0),
+        features=init_features,
+        rewards=jnp.ones(self.pool_size) * -jnp.inf,
+        best_reward=-jnp.inf,
+        perturbations=jnp.ones(self.pool_size) * self.config.perturbation,
+    )
 
-  def _populate_pool_with_prior_trials(self) -> None:
+  def _populate_pool_with_prior_trials(
+      self,
+      seed: chex.PRNGKey,
+      prior_features: chex.Array,
+      prior_rewards: chex.Array,
+  ) -> jax.Array:
     """Populate the pool with prior trials.
 
+    Args:
+      seed: Random seed.
+      prior_features: (n_prior_features, features_count)
+      prior_rewards: (n_prior_features, )
+
+    Returns:
+      initial_features
+
     A portion of the pool is first populated with random features based on
     'prior_trials_pool_pct', then the rest of the flies are populated by
     sequentially iterate over the prior trials, finding the cloest firefly in
     the pool and replace it if the reward is better.
     """
-    if self.prior_features is None or self.prior_rewards is None:
+    if prior_features is None or prior_rewards is None:
       raise ValueError("One of prior features / prior rewards wasn't provided!")
-    if self.prior_features.shape[0] != self.prior_rewards.shape[0]:
+    if prior_features.shape[0] != prior_rewards.shape[0]:
       raise ValueError(
-          f"prior features shape ({self.prior_features.shape[0]}) doesn't match"
-          f" prior  rewards shape ({self.prior_rewards.shape[0]})!"
+          f"prior features shape ({prior_features.shape[0]}) doesn't match"
+          f" prior  rewards shape ({prior_rewards.shape[0]})!"
       )
-    if self.prior_features.shape[1] != self._n_features:
+    if prior_features.shape[1] != self._n_features:
       raise ValueError(
-          "prior features shape doesn't match n_features{self._n_features}!"
+          f"prior features shape ({prior_features.shape[1]}) doesn't match "
+          f"n_features ({self._n_features})!"
       )
-    if len(self.prior_rewards.shape) > 1:
+    if len(prior_rewards.shape) > 1:
       raise ValueError("prior rewards is expected to be 1D array!")
 
     # Reverse the order of prior trials to assign more weight to recent trials.
-    self.prior_features = np.flip(self.prior_features, axis=-1)
-    self.prior_rewards = np.flip(self.prior_rewards, axis=-1)
+    flipped_prior_features = jnp.flip(prior_features, axis=0)
+    flipped_prior_rewards = jnp.flip(prior_rewards, axis=0)
 
-    self._features = np.zeros((0, self._n_features))
     # Fill pool with random features.
     n_random_flies = int(
         self.pool_size * (1 - self.config.prior_trials_pool_pct)
     )
-    self._features = self._param_handler.random_features(
-        n_random_flies, self._n_features
-    )
+    seed1, seed2 = jax.random.split(seed)
+    init_features = self._param_handler.random_features(n_random_flies, seed1)
     pool_left_space = self.pool_size - n_random_flies
 
-    if self.prior_features.shape[0] < pool_left_space:
+    if prior_features.shape[0] < pool_left_space:
       # Less prior trials than left space. Take all prior trials for the pool.
-      self._features = np.concatenate([self._features, self.prior_features])
+      init_features = jnp.concatenate([init_features, flipped_prior_features])
       # Randomize the rest of the pool fireflies.
       random_features = self._param_handler.random_features(
-          self.pool_size - len(self._features), self._n_features
+          self.pool_size - len(init_features), seed2
       )
-      self._features = np.concatenate([self._features, random_features])
+      return jnp.concatenate([init_features, random_features])
     else:
       # More prior trials than left space. Iteratively populate the pool.
-      tmp_features = self.prior_features[:pool_left_space]
-      tmp_rewards = self.prior_rewards[:pool_left_space]
-      for i in range(pool_left_space, self.prior_features.shape[0]):
-        ind = np.argmin(
-            np.sum(np.square(self.prior_features[i] - tmp_features), axis=-1)
+      tmp_features = flipped_prior_features[:pool_left_space]
+      tmp_rewards = flipped_prior_rewards[:pool_left_space]
+
+      def _loop_body(i, args):
+        features, rewards = args
+        ind = jnp.argmin(
+            jnp.sum(jnp.square(flipped_prior_features[i] - features), axis=-1)
+        )
+        return jax.lax.cond(
+            rewards[ind] < flipped_prior_rewards[i],
+            lambda: (
+                features.at[ind].set(flipped_prior_features[i]),
+                rewards.at[ind].set(flipped_prior_rewards[i]),
+            ),
+            lambda: (features, rewards),
         )
-        if tmp_rewards[ind] < self.prior_rewards[i]:
-          # Only take the prior trials features. Rewards obtain during update.
-          tmp_features[ind] = self.prior_features[i]
-          tmp_rewards[ind] = self.prior_rewards[i]
-      self._features = np.concatenate([self._features, tmp_features])
+
+      # TODO: Use a vectorized method to populate the pool and avoid
+      # the for-loop.
+      tmp_features, _ = jax.lax.fori_loop(
+          lower=pool_left_space,
+          upper=prior_features.shape[0],
+          body_fun=_loop_body,
+          init_val=(tmp_features, tmp_rewards),
+      )
+      return jnp.concatenate([init_features, tmp_features])
 
   @property
   def suggestion_batch_size(self) -> int:
     """The number of suggestions returned at each call of 'suggest'."""
     return self.batch_size
 
-  def suggest(self) -> np.ndarray:
+  def suggest(
+      self, state: VectorizedEagleStrategyState, seed: chex.PRNGKey
+  ) -> jax.Array:
     """Suggest new mutated and perturbed features.
 
     After initializing, at each call `batch_size` fireflies are mutated to
     generate new features using pulls (attraction/repulsion) from all other
     fireflies in the pool.
 
-    Returns:
-      suggested batch features: (batch_size, n_features)
-    """
-    if self._iterations < self.pool_size // self.batch_size:
-      # The strategy is still initializing. Return the random/prior features.
-      new_features = self._features[self._batch_slice]
-    else:
-      mutated_features = self._create_features()
-      perturbations = self._create_perturbations()
-      new_features = mutated_features + perturbations
-
-    new_features = self._param_handler.sample_categorical(new_features)
-    suggested_features = np.clip(new_features, 0, 1)
-    # Save the suggested features to be used in update.
-    self._last_suggested_features = suggested_features
-    return suggested_features
-
-  def _increment_batch(self):
-    """Increment the batch of fireflies features are generate from."""
-    self._batch_id = (self._batch_id + 1) % (self.pool_size // self.batch_size)
-    start_batch = self._batch_id * self.batch_size
-    end_batch = (self._batch_id + 1) * self.batch_size
-    self._batch_slice = np.s_[start_batch:end_batch]
-
-  def _create_features(self) -> np.ndarray:
-    """Create new batch of mutated and perturbed features.
-
-    Returns:
-      batch features: (batch_size, n_features)
-    """
-    features_diffs, dists = self._compute_features_diffs_and_dists()
-    scaled_directions = self._compute_scaled_directions()
-    features_changes = self._compute_features_changes(
-        features_diffs, dists, scaled_directions
-    )
-    return self._features[self._batch_slice] + features_changes
-
-  def _compute_features_diffs_and_dists(self) -> tuple[np.ndarray, np.ndarray]:
-    """Compute the features difference and distances.
-
-    The computation is done between the 'batch_size' fireflies and all
-    other fireflies in the pool.
-
-    features_diff[i, j, :] := features[j, :] - features[i, :]
-    features_dist[i, j, :] := distance between fly 'j' and fly 'i'
-
-    Returns:
-      feature differences: (batch_size, pool_size, n_features)
-      features distances: (batch_size, pool_size)
-    """
-    shape = (self.batch_size,) + self._features.shape
-    features_diffs = np.broadcast_to(self._features, shape) - np.expand_dims(
-        self._features[self._batch_slice], 1
-    )
-    dists = np.sum(np.square(features_diffs), axis=-1)
-    return features_diffs, dists
-
-  def _compute_scaled_directions(self) -> np.ndarray:
-    """Compute the scaled direction for applying pull between two flies.
-
-    scaled_directions[i,j] := direction of force applied by fly 'j' on fly 'i'.
-
-    Note that to compute 'directions' we might perform subtract with removed
-    flies with having value of -np.inf. Moreover, we might even subtract between
-    two removed flies which will result in np.nan. Both cases are handled when
-    computing the actual feautre changes applying a relevant mask.
+    Args:
+      state: Current strategy state.
+      seed: Random seed.
 
     Returns:
-      scaled directions: (batch_size, pool_size)
+      suggested batch features: (batch_size, n_features)
     """
-    shape = (self.batch_size,) + self._rewards.shape
-    directions = np.broadcast_to(self._rewards, shape) - np.expand_dims(
-        self._rewards[self._batch_slice], -1
-    )
-
-    scaled_directions = np.where(
-        directions >= 0, self.config.gravity, -self.config.negative_gravity
-    )
-    return scaled_directions
+    batch_id = state.iterations % (self.pool_size // self.batch_size)
+    start = batch_id * self.batch_size
+    features_batch = jax.lax.dynamic_slice_in_dim(
+        state.features, start, self.batch_size
+    )
+    rewards_batch = jax.lax.dynamic_slice_in_dim(
+        state.rewards, start, self.batch_size
+    )
+    perturbations_batch = jax.lax.dynamic_slice_in_dim(
+        state.perturbations, start, self.batch_size
+    )
+    features_seed, perturbations_seed, cat_seed = jax.random.split(seed, num=3)
+
+    def _mutate_features(features_batch_):
+      mutated_features = self._create_features(
+          state.features,
+          state.rewards,
+          features_batch_,
+          rewards_batch,
+          features_seed,
+      )
+      perturbations = self._create_random_perturbations(
+          perturbations_batch, perturbations_seed
+      )
+      return mutated_features + perturbations
+
+    # If the strategy is still initializing, return the random/prior features.
+    new_features = jax.lax.cond(
+        state.iterations < self.pool_size // self.batch_size,
+        lambda x: x,
+        _mutate_features,
+        features_batch,
+    )
+
+    new_features = self._param_handler.sample_categorical(
+        new_features, cat_seed
+    )
+    # TODO: The range of features is not always [0, 1].
+    #   Specifically, for features that are single-point, it can be [0, 0]; we
+    #   also want this code to be aware of the feature's bounds to enable
+    #   contextual bandit operation.  Note that if a parameter's bound changes,
+    #   we might also want to change the firefly noise or normalizations.
+    return jnp.clip(new_features, 0.0, 1.0)
 
-  def _compute_features_changes(
+  def _create_features(
       self,
-      features_diffs: np.ndarray,
-      dists: np.ndarray,
-      scaled_directions: np.ndarray,
-  ) -> np.ndarray:
-    """Compute the firefly features changes due to mutation.
+      features: jax.Array,
+      rewards: jax.Array,
+      features_batch: jax.Array,
+      rewards_batch: jax.Array,
+      seed: chex.PRNGKey,
+  ) -> jax.Array:
+    """Create new batch of mutated and perturbed features.
 
     The pool fireflies forces (pull/push) are being normalized to ensure the
     combined force doesn't throw the firefly too far. Mathematically, the
     normalization guarantees that the combined normalized force is within the
     simplex constructed by the unnormalized forces and therefore within bounds.
 
-    Arguments:
-      features_diffs: (batch_size, pool_size, n_features)
-      dists: (batch_size, pool_size)
-      scaled_directions: (batch_size, pool_size)
+    Args:
+      features: (pool_size, n_features)
+      rewards: (pool_size,)
+      features_batch: (batch_size, n_features)
+      rewards_batch: (batch_size,)
+      seed: Random seed.
 
     Returns:
-      feature changes: (batch_size, feature_n)
+      batch features: (batch_size, n_features)
     """
+    # Compute the pairwise squared distances between the features batch and the
+    # pool. We use a less numerically precise squared distance formulation to
+    # avoid materializing a possibly large intermediate of shape
+    # (batch_size, pool_size, n_features).
+    dists = (
+        jnp.sum(features_batch**2, axis=-1, keepdims=True)
+        + jnp.sum(features**2, axis=-1)
+        - 2.0 * jnp.matmul(features_batch, features.T)
+    )  # shape (batch_size, pool_size)
+
+    # Compute the scaled direction for applying pull between two flies.
+    # scaled_directions[i,j] := direction of force applied by fly 'j' on fly
+    # 'i'. Note that to compute 'directions' we might perform subtract with
+    # removed flies with having value of -np.inf. Moreover, we might even
+    # subtract between two removed flies which will result in np.nan. Both cases
+    # are handled when computing the actual feautre changes applying a relevant
+    # mask.
+    directions = rewards - rewards_batch[:, jnp.newaxis]
+    scaled_directions = jnp.where(
+        directions >= 0.0, self.config.gravity, -self.config.negative_gravity
+    )  # shape (batch_size, pool_size)
+
     # Normalize the distance by the number of features.
-    force = np.exp(-self.config.visibility * dists / self._n_features * 10)
-    scaled_force = np.expand_dims(scaled_directions * force, -1)
+    force = jnp.exp(-self.config.visibility * dists / self._n_features * 10.0)
+    scaled_force = scaled_directions * force
     # Handle removed fireflies without updated rewards.
-    inf_indx = np.isinf(self._rewards)
-    if np.sum(inf_indx) == self.pool_size:
-      logging.warning(
-          (
-              "All firefly were recently removed. This Shouldn't happen."
-              "Pool Features:\n%sPool rewards:\n%s"
-          ),
-          self._features,
-          self._rewards,
-      )
-      return np.zeros((self.batch_size, self._n_features))
+    finite_ind = jnp.isfinite(rewards).astype(scaled_force.dtype)
 
     # Ignore fireflies that were removed from the pool.
-    features_diffs = features_diffs[:, ~inf_indx, :]
-    scaled_force = scaled_force[:, ~inf_indx, :]
+    scaled_force = scaled_force * finite_ind
 
     # Separate forces to pull and push so to normalize them separately.
-    scaled_pulls = np.where(scaled_force > 0, scaled_force, 0)
-    scaled_push = np.where(scaled_force < 0, scaled_force, 0)
+    scaled_pulls = jnp.maximum(scaled_force, 0.0)
+    scaled_push = jnp.minimum(scaled_force, 0.0)
 
-    if self.config.mutate_normalization_type == "mean":
+    if self.config.mutate_normalization_type == MutateNormalizationType.MEAN:
       # Divide the push and pull forces by the number of flies participating.
       # Also multiply by normalization_scale.
-      norm_scaled_pulls = self.config.normalization_scale * np.nan_to_num(
-          scaled_pulls / np.sum(scaled_pulls > 0, axis=1, keepdims=True), 0
+      norm_scaled_pulls = self.config.normalization_scale * jnp.nan_to_num(
+          scaled_pulls / jnp.sum(scaled_pulls > 0.0, axis=1, keepdims=True), 0
       )
-      norm_scaled_push = self.config.normalization_scale * np.nan_to_num(
-          scaled_push / np.sum(scaled_push < 0, axis=1, keepdims=True), 0
+      norm_scaled_push = self.config.normalization_scale * jnp.nan_to_num(
+          scaled_push / jnp.sum(scaled_push < 0.0, axis=1, keepdims=True), 0
       )
-    elif self.config.mutate_normalization_type == "random":
+    elif self.config.mutate_normalization_type == (
+        MutateNormalizationType.RANDOM
+    ):
       # Create random matrices and normalize each row, s.t. the sum is 1.
-      pull_rand_matrix = self._rng.uniform(
-          0, 1, size=scaled_pulls.shape
-      ) * np.int_(scaled_pulls > 0)
-      pull_weight_matrix = pull_rand_matrix / np.sum(
+      pull_seed, push_seed = jax.random.split(seed)
+      scaled_pulls_pos = scaled_pulls > 0
+      pull_rand_matrix = (
+          jax.random.uniform(pull_seed, shape=scaled_pulls.shape)
+          * scaled_pulls_pos
+      )
+      pull_weight_matrix = pull_rand_matrix / jnp.sum(
           pull_rand_matrix, axis=1, keepdims=True
       )
-      push_rand_matrix = self._rng.uniform(
-          0, 1, size=scaled_pulls.shape
-      ) * np.int_(scaled_pulls > 0)
-      push_weight_matrix = push_rand_matrix / np.sum(
+      push_rand_matrix = (
+          jax.random.uniform(push_seed, shape=scaled_pulls.shape)
+          * scaled_pulls_pos
+      )
+      push_weight_matrix = push_rand_matrix / jnp.sum(
           push_rand_matrix, axis=1, keepdims=True
       )
       # Normalize pulls/pulls by the weight matrices.
       # Also multiply by normalization_scale.
       norm_scaled_pulls = (
           self.config.normalization_scale * scaled_pulls * pull_weight_matrix
       )
       norm_scaled_push = (
           self.config.normalization_scale * scaled_push * push_weight_matrix
       )
-    elif self.config.mutate_normalization_type == "unnormalized":
+    elif self.config.mutate_normalization_type == (
+        MutateNormalizationType.UNNORMALIZED
+    ):
       # Doesn't normalize the forces. Use this option with caution.
       norm_scaled_pulls = scaled_pulls
       norm_scaled_push = scaled_push
 
-    # Sums normalized forces (pull/push) of all fireflies.
-    return np.sum(
-        features_diffs * (norm_scaled_pulls + norm_scaled_push), axis=1
-    )
-
-  def _create_perturbations(self) -> np.ndarray:
-    """Create random perturbations for the newly creatd batch.
+    # Sums normalized forces (pull/push) of all fireflies. This is equivalent to
+    # features_dist[i, j] := distance between fly 'j' and fly 'i'
+    # but avoids materializing the large pairwise distance matrix.
+    scale = norm_scaled_pulls + norm_scaled_push
+    features_changes = jnp.matmul(scale, features) - features_batch * jnp.sum(
+        scale, axis=-1, keepdims=True
+    )
+    return features_batch + features_changes
+
+  def _create_random_perturbations(
+      self, perturbations_batch: jax.Array, seed: chex.PRNGKey
+  ) -> jax.Array:
+    """Create random perturbations for the newly created batch.
+
+    Args:
+      perturbations_batch: (batch_size,)
+      seed: Random seed.
 
     Returns:
-      batched perturbations: (base_size, n_features)
+      perturbations: (batch_size, n_features)
     """
     # Generate normalized noise for each batch.
-    batch_noise = self._rng.laplace(size=(self.batch_size, self._n_features))
-    batch_noise /= np.max(np.abs(batch_noise), axis=1, keepdims=True)
-    # Scale the noise by the each fly current perturbation.
+    batch_noise = jax.random.laplace(
+        seed, shape=(self.batch_size, self._n_features)
+    )
+    batch_noise /= jnp.max(jnp.abs(batch_noise), axis=1, keepdims=True)
     return (
         batch_noise
-        * self._perturbations[self._batch_slice][:, np.newaxis]
+        * perturbations_batch[:, jnp.newaxis]
         * self._perturbation_factors
     )
 
-  def update(self, batch_rewards: np.ndarray) -> None:
+  def update(
+      self,
+      state: VectorizedEagleStrategyState,
+      batch_features: types.Array,
+      batch_rewards: types.Array,
+      seed: chex.PRNGKey,
+  ) -> VectorizedEagleStrategyState:
     """Update the firefly pool based on the new batch of results.
 
     Arguments:
+      state: Current state.
+      batch_features: (batch_size, n_features)
       batch_rewards: (batch_size, )
+      seed: Random seed.
+
+    Returns:
+      new_state: Updated state.
     """
-    self._update_best_reward(batch_rewards)
-    if self._iterations < self.pool_size // self.batch_size:
-      # The strategy is still initializing. Assign rewards.
-      self._features[self._batch_slice] = self._last_suggested_features
-      self._rewards[self._batch_slice] = batch_rewards
-    else:
+    new_best_reward = jnp.maximum(state.best_reward, jnp.max(batch_rewards))
+    batch_id = state.iterations % (self.pool_size // self.batch_size)
+    batch_start_ind = batch_id * self.batch_size
+    batch_perturbations = jax.lax.dynamic_slice_in_dim(
+        state.perturbations, batch_start_ind, self.batch_size
+    )
+
+    def _update(batch_features, batch_rewards, batch_perturbations):
       # Pass the new batch rewards and the associated last suggested features.
-      self._update_pool_features_and_rewards(batch_rewards)
-      self._trim_pool()
-    self._increment_batch()
-    self._iterations += 1
-
-  def _update_best_reward(self, batch_rewards: np.ndarray) -> None:
-    """Store the best result seen thus far to be used in pool trimming."""
-    self._best_reward = np.max([self._best_reward, np.max(batch_rewards)])
+      new_batch_features, new_batch_rewards, new_batch_perturbations = (
+          self._update_pool_features_and_rewards(
+              batch_features,
+              batch_rewards,
+              jax.lax.dynamic_slice_in_dim(
+                  state.features, batch_start_ind, self.batch_size
+              ),
+              jax.lax.dynamic_slice_in_dim(
+                  state.rewards, batch_start_ind, self.batch_size
+              ),
+              batch_perturbations,
+          )
+      )
+      return self._trim_pool(
+          new_batch_features,
+          new_batch_rewards,
+          new_batch_perturbations,
+          new_best_reward,
+          seed,
+      )
+
+    # If the strategy is still initializing, return the random/prior values.
+    (new_batch_features, new_batch_rewards, new_batch_perturbations) = (
+        jax.lax.cond(
+            state.iterations < self.pool_size // self.batch_size,
+            lambda *args: args,
+            _update,
+            batch_features,
+            batch_rewards,
+            batch_perturbations,
+        )
+    )
+
+    return VectorizedEagleStrategyState(
+        iterations=state.iterations + 1,
+        features=jax.lax.dynamic_update_slice_in_dim(
+            state.features, new_batch_features, batch_start_ind, axis=0
+        ),
+        rewards=jax.lax.dynamic_update_slice_in_dim(
+            state.rewards, new_batch_rewards, batch_start_ind, axis=0
+        ),
+        best_reward=new_best_reward,
+        perturbations=jax.lax.dynamic_update_slice_in_dim(
+            state.perturbations,
+            new_batch_perturbations,
+            batch_start_ind,
+            axis=0,
+        ),
+    )
 
   def _update_pool_features_and_rewards(
       self,
-      batch_rewards: np.ndarray,
-  ):
+      batch_features: jax.Array,
+      batch_rewards: jax.Array,
+      prev_batch_features: jax.Array,
+      prev_batch_rewards: jax.Array,
+      perturbations: jax.Array,
+  ) -> Tuple[jax.Array, jax.Array, jax.Array]:
     """Update the features and rewards for flies with improved rewards.
 
     Arguments:
-      batch_rewards: (batch_size, )
+      batch_features: (batch_size, n_features), new proposed features batch.
+      batch_rewards: (batch_size,), rewards for new proposed features batch.
+      prev_batch_features: (batch_size, n_features), previous features batch.
+      prev_batch_rewards: (batch_size,), rewards for previous features batch.
+      perturbations: (batch_size,)
+
+    Returns:
+      sliced features, sliced rewards, sliced perturbations
     """
-    sliced_features = self._features[self._batch_slice]
-    sliced_rewards = self._rewards[self._batch_slice]
-    sliced_perturbations = self._perturbations[self._batch_slice]
     # Find indices of flies that their generated features made an improvement.
-    improve_indx = batch_rewards > sliced_rewards
+    improve_indx = batch_rewards > prev_batch_rewards
     # Update successful flies' with the associated last features and rewards.
-    sliced_features[improve_indx] = self._last_suggested_features[improve_indx]
-    sliced_rewards[improve_indx] = batch_rewards[improve_indx]
+    new_batch_features = jnp.where(
+        improve_indx[..., jnp.newaxis], batch_features, prev_batch_features
+    )
+    new_batch_rewards = jnp.where(
+        improve_indx, batch_rewards, prev_batch_rewards
+    )
     # Penalize unsuccessful flies.
-    sliced_perturbations[~improve_indx] *= self.config.penalize_factor
+    new_batch_perturbations = jnp.where(
+        improve_indx, perturbations, perturbations * self.config.penalize_factor
+    )
+    return new_batch_features, new_batch_rewards, new_batch_perturbations
 
-  def _trim_pool(self) -> None:
+  def _trim_pool(
+      self,
+      batch_features: jax.Array,
+      batch_rewards: jax.Array,
+      batch_perturbations: jax.Array,
+      best_reward: jax.Array,
+      seed: chex.PRNGKey,
+  ) -> Tuple[jax.Array, jax.Array, jax.Array]:
     """Trim the pool by replacing unsuccessful fireflies with new random ones.
 
     A firefly is considered unsuccessful if its current perturbation is below
     'perturbation_lower_bound' and it's not the best fly seen thus far.
     Random features are created to replace the existing ones, and rewards
     are set to -np.inf to indicate that we don't have values for those feaures
     yet and we shouldn't use them during suggest.
+
+    Args:
+      batch_features: (batch_size, n_features)
+      batch_rewards: (batch_size,)
+      batch_perturbations: (batch_size,)
+      best_reward: Best reward seen so far.
+      seed: Random seed.
+
+    Returns:
+      updated feature, reward, and perturbation batches.
     """
-    sliced_perturbations = self._perturbations[self._batch_slice]
-    indx = sliced_perturbations < self.config.perturbation_lower_bound
-    n_remove = np.sum(indx)
-    if n_remove > 0:
-      sliced_features = self._features[self._batch_slice]
-      sliced_rewards = self._rewards[self._batch_slice]
-      # Ensure the best firefly is never removed. For optimization purposes,
-      # this logic is inside the if statement to be peformed only if needed.
-      indx = indx & (sliced_rewards != self._best_reward)
-      n_remove = np.sum(indx)
-      if n_remove == 0:
-        return
-      # Replace fireflies with random features and evaluate rewards.
-      sliced_features[indx] = self._param_handler.random_features(
-          n_remove, self._n_features
-      )
-      sliced_perturbations[indx] = (
-          np.ones(
-              n_remove,
-          )
-          * self.config.perturbation
-      )
-      # Setting rewards to -inf to filter out those fireflies during suggest.
-      sliced_rewards[indx] = np.ones(
-          n_remove,
-      ) * (-np.inf)
-      self._num_removed_flies += n_remove
+    indx = batch_perturbations < self.config.perturbation_lower_bound
+    # Ensure the best firefly is never removed. For optimization purposes,
+    # this logic is inside the if statement to be peformed only if needed.
+    indx = indx & (batch_rewards != best_reward)
+
+    # Replace fireflies with random features and evaluate rewards.
+    random_features = self._param_handler.random_features(self.batch_size, seed)
+    new_batch_features = jnp.where(
+        indx[..., jnp.newaxis], random_features, batch_features
+    )
+    new_batch_perturbations = jnp.where(
+        indx, self.config.perturbation, batch_perturbations
+    )
+    # Setting rewards to -inf to filter out those fireflies during suggest.
+    new_batch_rewards = jnp.where(indx, -jnp.inf, batch_rewards)
+    return new_batch_features, new_batch_rewards, new_batch_perturbations
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/optimizers/eagle_strategy_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/eagle_strategy_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,222 +13,233 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for eagle strategy."""
 
 from absl.testing import parameterized
+import jax
+from jax import numpy as jnp
 import numpy as np
 from vizier import pyvizier as vz
 from vizier._src.algorithms.optimizers import eagle_param_handler
 from vizier._src.algorithms.optimizers import eagle_strategy
 from vizier._src.algorithms.optimizers import vectorized_base as vb
 from vizier.pyvizier import converters
 
 from absl.testing import absltest
 
 
+def _create_features_simple(
+    features, rewards, features_batch, rewards_batch, config, n_features
+):
+  """A version of `_create_features` that materializes large intermediates."""
+  features_diffs = features - features_batch[:, jnp.newaxis, :]
+  dists = jnp.sum(jnp.square(features_diffs), axis=-1)
+  directions = rewards - rewards_batch[:, jnp.newaxis]
+  scaled_directions = jnp.where(
+      directions >= 0.0, config.gravity, -config.negative_gravity
+  )
+
+  # Normalize the distance by the number of features.
+  force = jnp.exp(-config.visibility * dists / n_features * 10.0)
+  scaled_force = scaled_directions * force
+  # Handle removed fireflies without updated rewards.
+  finite_ind = jnp.isfinite(rewards).astype(scaled_force.dtype)
+
+  # Ignore fireflies that were removed from the pool.
+  scaled_force = scaled_force * finite_ind
+
+  # Separate forces to pull and push so to normalize them separately.
+  scaled_pulls = jnp.maximum(scaled_force, 0.0)
+  scaled_push = jnp.minimum(scaled_force, 0.0)
+  features_changes = jnp.sum(
+      features_diffs * (scaled_pulls + scaled_push)[..., jnp.newaxis], axis=1
+  )
+  return features_batch + features_changes
+
+
 class VectorizedEagleStrategyContinuousTest(parameterized.TestCase):
 
   def setUp(self):
     super(VectorizedEagleStrategyContinuousTest, self).setUp()
     self.config = eagle_strategy.EagleStrategyConfig(
         visibility=1, gravity=1, pool_size=4
     )
     problem = vz.ProblemStatement()
     root = problem.search_space.select_root()
     root.add_float_param('x1', 0.0, 1.0)
     root.add_float_param('x2', 0.0, 1.0)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
     self.eagle = eagle_strategy.VectorizedEagleStrategy(
-        converter=converter, config=self.config, batch_size=2, seed=1
+        converter=converter, config=self.config, batch_size=2
     )
     self.eagle._iterations = 2
 
-  def test_compute_features_diffs_and_dists(self):
-    self.eagle._features = np.array([[1, 2], [3, 4], [7, 7], [8, 8]])
-    features_diffs, dists = self.eagle._compute_features_diffs_and_dists()
-    expected_features_diffs = np.array(
-        [[[0, 0], [2, 2], [6, 5], [7, 6]], [[-2, -2], [0, 0], [4, 3], [5, 4]]]
-    )
-    np.testing.assert_array_equal(
-        features_diffs,
-        expected_features_diffs,
-        err_msg='feature differences mismatch',
-    )
-
-    expected_dists = np.array([[0, 8, 61, 85], [8, 0, 25, 41]])
-    np.testing.assert_array_almost_equal(
-        dists, expected_dists, err_msg='feature distance mismatch'
-    )
-
-  def test_compute_scaled_directions(self):
-    self.eagle._rewards = np.array([2, 3, 4, 1])
-    g = self.config.gravity
-    ng = -self.config.negative_gravity
-    expected_scaled_directions = np.array([
-        [g, g, g, ng],
-        [ng, g, g, ng],
-    ])
-    scaled_directions = self.eagle._compute_scaled_directions()
-    np.testing.assert_array_equal(scaled_directions, expected_scaled_directions)
-
-  def test_compute_scaled_directions_with_removed_flies(self):
-    self.eagle._rewards = np.array([-np.inf, 3, -np.inf, 1])
-    g = self.config.gravity
-    ng = -self.config.negative_gravity
-    # Note that -np.inf - (-np.inf) is not >=0.
-    expected_scaled_directions = np.array([
-        [ng, g, ng, g],
-        [ng, g, ng, ng],
-    ])
-    scaled_directions = self.eagle._compute_scaled_directions()
-    np.testing.assert_array_equal(scaled_directions, expected_scaled_directions)
-
-  @parameterized.parameters('random', 'mean')
-  def test_compute_features_changes(self, norm_type):
-    self.eagle._rewards = np.array([-np.inf, 3, -np.inf, 1])
-    features_diffs = np.array(
-        [[[0, 0], [2, 2], [6, 5], [7, 6]], [[-2, -2], [0, 0], [4, 3], [5, 4]]]
-    )
-    dists = np.array([[0, 8, 61, 85], [8, 0, 25, 41]])
-    scaled_directions = np.array([
-        [-1, 1, -1, 1],
-        [-1, 1, -1, -1],
-    ])
-    if norm_type == 'mean':
-      features_changes = self.eagle._compute_features_changes(
-          features_diffs, dists, scaled_directions
-      )
-      # scaled_pulls array:
-      # [[-1.00000000e+000  4.24835426e-018 -3.46883002e-133  2.65977679e-185]
-      # [-4.24835426e-018  1.00000000e+000 -5.16642063e-055 -9.32462145e-090]
-      c0 = (
-          np.array([2, 2]) * 4.24835426e-018 / 2.0
-          + np.array([7, 6]) * 2.65977679e-185 / 2.0
-      )
-      c1 = np.array([5, 4]) * (-9.32462145e-090) / 1.0
-      expected_features_changes = np.vstack([c0, c1])
-      self.assertEqual(features_changes.shape, (2, 2))
-      np.testing.assert_array_almost_equal(
-          expected_features_changes, features_changes
-      )
-
-    if norm_type == 'random':
-      for _ in range(1000):
-        # Repeat the check multiple time to increase confidence.
-        features_changes = self.eagle._compute_features_changes(
-            features_diffs, dists, scaled_directions
-        )
-        # scaled_pulls:
-        # [[-1.00000000e+000  4.24835426e-018 -3.46883002e-133  2.65977679e-185]
-        # [-4.24835426e-018  1.00000000e+000 -5.16642063e-055 -9.32462145e-090]]
-        c0 = (
-            np.array([2, 2]) * 4.24835426e-018 / 2.0
-            + np.array([7, 6]) * 2.65977679e-185 / 2.0
-        )
-        c1 = np.array([5, 4]) * (-9.32462145e-090) / 1.0
-        self.assertEqual(features_changes.shape, (2, 2))
-
-        low_bound_00 = 7 * 2.65977679e-185
-        high_bound_00 = 2 * 4.24835426e-018
-        low_bound_01 = 6 * 2.65977679e-185
-        high_bound_01 = 2 * 4.24835426e-018
-
-        self.assertBetween(features_changes[0][0], low_bound_00, high_bound_00)
-        self.assertBetween(features_changes[0][1], low_bound_01, high_bound_01)
-        np.testing.assert_array_almost_equal(features_changes[1], c1)
-
-        expected_features_changes = np.vstack([c0, c1])
-
-        np.testing.assert_array_almost_equal(
-            expected_features_changes, features_changes
-        )
-
   def test_create_features(self):
-    self.assertEqual(self.eagle._create_features().shape, (2, 2))
-
-  def test_create_perturbations(self):
-    perturbations = self.eagle._create_perturbations()
+    features = jnp.array([[1, 2], [3, 4], [7, 7], [8, 8]])
+    rewards = jnp.array([2, 3, 4, 1])
+    seed = jax.random.PRNGKey(0)
+    features_batch = features[: self.eagle.batch_size]
+    rewards_batch = rewards[: self.eagle.batch_size]
+    self.assertEqual(
+        self.eagle._create_features(
+            features,
+            rewards,
+            features_batch,
+            rewards_batch,
+            seed=seed,
+        ).shape,
+        (2, 2),
+    )
+
+    expected = _create_features_simple(
+        features,
+        rewards,
+        features_batch,
+        rewards_batch,
+        self.config.replace(
+            mutate_normalization_type=(
+                eagle_strategy.MutateNormalizationType.UNNORMALIZED
+            )
+        ),
+        self.eagle._n_features,
+    )
+    actual = self.eagle._create_features(
+        features,
+        rewards,
+        features_batch,
+        rewards_batch,
+        seed=seed,
+    )
+    np.testing.assert_array_equal(expected, actual)
+
+  def test_create_random_perturbations(self):
+    seed = jax.random.PRNGKey(0)
+    perturbations_batch = jnp.ones(self.eagle.batch_size)
+    perturbations = self.eagle._create_random_perturbations(
+        perturbations_batch, seed=seed
+    )
     self.assertEqual(perturbations.shape, (2, 2))
 
   def test_update_pool_features_and_rewards(self):
-    self.eagle._features = np.array(
-        [[1, 2], [3, 4], [7, 7], [8, 8]], dtype=np.float64
-    )
-    self.eagle._rewards = np.array([2, 3, 4, 1], dtype=np.float64)
-    self.eagle._perturbations = np.array([1, 1, 1, 1], dtype=np.float64)
-
-    self.eagle._last_suggested_features = np.array(
-        [[9, 9], [10, 10]], dtype=np.float64
+    features = jnp.array([[1, 2], [3, 4], [7, 7], [8, 8]], dtype=jnp.float64)
+    rewards = jnp.array([2, 3, 4, 1], dtype=jnp.float64)
+    perturbations = jnp.array([1, 1, 1, 1], dtype=jnp.float64)
+
+    batch_features = jnp.array([[9, 9], [10, 10]], dtype=jnp.float64)
+    batch_rewards = jnp.array([5, 0.5], dtype=jnp.float64)
+
+    new_features, new_rewards, new_perturbations = (
+        self.eagle._update_pool_features_and_rewards(
+            batch_features,
+            batch_rewards,
+            features[: self.eagle.batch_size],
+            rewards[: self.eagle.batch_size],
+            perturbations[: self.eagle.batch_size],
+        )
     )
-    batch_rewards = np.array([5, 0.5], dtype=np.float64)
-
-    self.eagle._update_pool_features_and_rewards(batch_rewards)
     np.testing.assert_array_equal(
-        self.eagle._features,
-        np.array([[9, 9], [3, 4], [7, 7], [8, 8]], dtype=np.float64),
+        new_features,
+        np.array([[9, 9], [3, 4]], dtype=np.float64),
         err_msg='Features are not equal.',
     )
 
     np.testing.assert_array_equal(
-        self.eagle._rewards,
-        np.array([5, 3, 4, 1], dtype=np.float64),
+        new_rewards,
+        np.array([5, 3], dtype=np.float64),
         err_msg='rewards are not equal.',
     )
 
     pc = self.config.penalize_factor
-    np.testing.assert_array_equal(
-        self.eagle._perturbations,
-        np.array([1, pc, 1, 1], dtype=np.float64),
+    np.testing.assert_array_almost_equal(
+        new_perturbations,
+        np.array([1, pc], dtype=np.float64),
         err_msg='Perturbations are not equal.',
     )
 
   def test_update_best_reward(self):
     # Test replacing the best reward.
-    self.eagle._rewards = np.array([2, 3, 4, 1], dtype=np.float64)
-    batch_rewards = np.array([5, 0.5], dtype=np.float64)
-    self.eagle._update_best_reward(batch_rewards)
-    self.assertEqual(self.eagle._best_reward, 5.0)
+    features = jnp.array([[1, 2], [3, 4], [7, 7], [8, 8]], dtype=jnp.float64)
+    rewards = jnp.array([2, 3, 4, 1], dtype=jnp.float64)
+    state = eagle_strategy.VectorizedEagleStrategyState(
+        iterations=jnp.array(0),
+        features=features,
+        rewards=rewards,
+        best_reward=jnp.max(rewards),
+        perturbations=jnp.ones_like(rewards),
+    )
+    batch_features = jnp.array([[9, 9], [10, 10]], dtype=jnp.float64)
+    batch_rewards = jnp.array([5, 0.5], dtype=jnp.float64)
+    seed = jax.random.PRNGKey(0)
+    new_state = self.eagle.update(
+        state, batch_features, batch_rewards, seed=seed
+    )
+    self.assertEqual(new_state.best_reward, 5.0)
     # Test not replacing the best reward.
-    batch_rewards = np.array([2, 4], dtype=np.float64)
-    self.eagle._update_best_reward(batch_rewards)
-    self.assertEqual(self.eagle._best_reward, 5.0)
+    batch_rewards = jnp.array([2, 4], dtype=jnp.float64)
+    new_new_state = self.eagle.update(
+        new_state, batch_features, batch_rewards, seed=seed
+    )
+    self.assertEqual(new_new_state.best_reward, 5.0)
+
+  @parameterized.parameters(
+      {'batch_size': 5, 'expected_batch_size': 5, 'max_pool_size': 50},
+      {'batch_size': None, 'expected_batch_size': 50, 'max_pool_size': 50},
+      {'batch_size': 5, 'expected_batch_size': 5, 'max_pool_size': 10},
+      {'batch_size': None, 'expected_batch_size': 10, 'max_pool_size': 10},
+  )
+  def test_batch_size_and_pool_size(
+      self, batch_size, expected_batch_size, max_pool_size
+  ):
+    problem = vz.ProblemStatement()
+    root = problem.search_space.root
+    for i in range(100):
+      root.add_float_param(f'x{i}', 0.0, 1.0)
+    converter = converters.TrialToArrayConverter.from_study_config(problem)
+    config = eagle_strategy.EagleStrategyConfig(max_pool_size=max_pool_size)
+    eagle = eagle_strategy.VectorizedEagleStrategy(
+        converter=converter, config=config, batch_size=batch_size
+    )
+    self.assertEqual(eagle.pool_size, max_pool_size)
+    self.assertEqual(eagle.batch_size, expected_batch_size)
 
   def test_trim_pool(self):
     pc = self.config.perturbation
-    self.eagle._features = np.array(
-        [[1, 2], [3, 4], [7, 7], [8, 8]], dtype=np.float64
+    features_batch = jnp.array([[1, 2], [3, 4]], dtype=jnp.float64)
+    rewards_batch = jnp.array([2, 3], dtype=jnp.float64)
+    perturbations = jnp.array([pc, 0], dtype=jnp.float64)
+    seed = jax.random.PRNGKey(0)
+    new_features, new_rewards, new_perturbations = self.eagle._trim_pool(
+        features_batch,
+        rewards_batch,
+        perturbations,
+        best_reward=jnp.array(4.0),
+        seed=seed,
     )
-    self.eagle._rewards = np.array([2, 3, 4, 1], dtype=np.float64)
-    self.eagle._perturbations = np.array([pc, 0, 0, pc], dtype=np.float64)
-    self.eagle._best_results = [
-        vb.VectorizedStrategyResult(reward=4.0, features=np.array([1.0, 2.0]))
-    ]
-    self.eagle._trim_pool()
 
     np.testing.assert_array_almost_equal(
-        self.eagle._features[[0, 2, 3], :],
-        np.array([[1, 2], [7, 7], [8, 8]], dtype=np.float64),
+        new_features[0],
+        features_batch[0],
         err_msg='Features are not equal.',
     )
     self.assertTrue(
-        all(np.not_equal(self.eagle._features[1, :], np.array([3, 4]))),
+        all(np.not_equal(new_features[1], features_batch[1])),
         msg='Features are not equal.',
     )
 
     np.testing.assert_array_equal(
-        self.eagle._rewards,
-        np.array([2, -np.inf, 4, 1], dtype=np.float64),
+        new_rewards,
+        np.array([2, -np.inf], dtype=np.float64),
         err_msg='rewards are not equal.',
     )
     # The best firefly is never removed.
-    np.testing.assert_array_equal(
-        self.eagle._perturbations,
-        np.array([pc, pc, 0, pc], dtype=np.float64),
+    np.testing.assert_array_almost_equal(
+        new_perturbations,
+        np.array([pc, pc], dtype=np.float64),
         err_msg='Perturbations are not equal.',
     )
 
   def test_create_strategy_from_factory(self):
     problem = vz.ProblemStatement()
     root = problem.search_space.select_root()
     root.add_float_param('x1', 0.0, 1.0)
@@ -245,15 +256,15 @@
     root.add_float_param('x1', 0.0, 1.0)
     root.add_float_param('x2', 0.0, 1.0)
     root.add_float_param('x3', 0.0, 1.0)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
     eagle_factory = eagle_strategy.VectorizedEagleStrategyFactory()
     optimizer = vb.VectorizedOptimizer(strategy_factory=eagle_factory)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
-    optimizer.optimize(converter, score_fn=lambda x: -np.sum(x, 1), count=1)
+    optimizer.optimize(converter, score_fn=lambda x: -jnp.sum(x, 1), count=1)
 
 
 class EagleParamHandlerTest(parameterized.TestCase):
 
   def setUp(self):
     super(EagleParamHandlerTest, self).setUp()
     problem = vz.ProblemStatement()
@@ -264,15 +275,14 @@
     root.add_discrete_param('d1', [2.0, 3.0, 5.0, 11.0])
     converter = converters.TrialToArrayConverter.from_study_config(
         problem, max_discrete_indices=0, pad_oovs=True
     )
     self.config = eagle_strategy.EagleStrategyConfig()
     self.param_handler = eagle_param_handler.EagleParamHandler(
         converter=converter,
-        rng=np.random.default_rng(1),
         categorical_perturbation_factor=self.config.categorical_perturbation_factor,
         pure_categorical_perturbation_factor=self.config.pure_categorical_perturbation_factor,
     )
 
   def test_init(self):
     self.assertEqual(self.param_handler.n_features, 9)
     self.assertFalse(self.param_handler.all_features_categorical)
@@ -295,15 +305,15 @@
     )
 
   def test_tiebreak_mask(self):
     eps = self.param_handler._epsilon
     expected_tiebreak_mask = np.array(
         [-eps * (i + 1) for i in range(9)], dtype=float
     )
-    np.testing.assert_array_equal(
+    np.testing.assert_array_almost_equal(
         self.param_handler._tiebreak_array, expected_tiebreak_mask
     )
 
   def test_categorical_oov_mask(self):
     expected_oov_mask = np.array([1, 1, 0, 1, 1, 1, 1, 0, 1], dtype=float)
     np.testing.assert_array_equal(
         self.param_handler._oov_mask, expected_oov_mask
@@ -317,46 +327,50 @@
     np.testing.assert_array_equal(
         self.param_handler.perturbation_factors, expected_perturbation_factors
     )
 
   def test_sample_categorical_features(self):
     # features shouldn't have values in oov_mask, and have the structure of:
     # [c1,c1,c1,f1,c2,c2,c2,c2,d1]
-    features = np.array([
+    features = jnp.array([
         [2.0, 0.0, 0.0, 1.5, 0.0, 0.0, 0.1, 0.0, 9.0],
         [3.0, 0.0, 0.0, 3.5, 5.0, 0.0, 0.0, 0.0, 8.0],
     ])
     expected_sampled_features = np.array([
         [1.0, 0.0, 0.0, 1.5, 0.0, 0.0, 1.0, 0.0, 9.0],
         [1.0, 0.0, 0.0, 3.5, 1.0, 0.0, 0.0, 0.0, 8.0],
     ])
-    sampled_features = self.param_handler.sample_categorical(features)
+    sampled_features = self.param_handler.sample_categorical(
+        features, seed=jax.random.PRNGKey(0)
+    )
     np.testing.assert_array_equal(sampled_features, expected_sampled_features)
 
   def test_prior_trials(self):
     config = eagle_strategy.EagleStrategyConfig(
         visibility=1, gravity=1, pool_size=4, prior_trials_pool_pct=1.0
     )
     problem = vz.ProblemStatement()
     root = problem.search_space.select_root()
     root.add_float_param('x1', 0.0, 1.0)
     root.add_float_param('x2', 0.0, 1.0)
     converter = converters.TrialToArrayConverter.from_study_config(problem)
 
-    prior_features = np.array([[1, 1], [2, 2], [3, 3], [4, 4]])
-    prior_rewards = np.array([1, 2, 3, 4])
+    prior_features = jnp.array([[1, -1], [2, 1], [3, 2], [4, 5]])
+    prior_rewards = jnp.array([1, 2, 3, 4])
     eagle = eagle_strategy.VectorizedEagleStrategy(
         converter=converter,
         config=config,
         batch_size=2,
-        seed=1,
-        prior_features=prior_features,
-        prior_rewards=prior_rewards,
     )
-    np.testing.assert_equal(eagle.prior_features, prior_features)
+    init_state = eagle.init_state(
+        jax.random.PRNGKey(0), prior_features, prior_rewards
+    )
+    np.testing.assert_array_equal(
+        init_state.features, jnp.flip(prior_features, axis=0)
+    )
 
   @parameterized.parameters(2, 10)
   def test_prior_trials_with_too_few_or_many_trials(self, n_prior_trials):
     # Test proper populating of the pool in case the number of prior trials is
     # greater or lesser than the pool size.
     config = eagle_strategy.EagleStrategyConfig(
         visibility=1, gravity=1, pool_size=4, prior_trials_pool_pct=1.0
@@ -370,16 +384,16 @@
     prior_features = np.random.randn(n_prior_trials, 2)
     prior_rewards = np.random.randn(n_prior_trials)
 
     eagle = eagle_strategy.VectorizedEagleStrategy(
         converter=converter,
         config=config,
         batch_size=2,
-        seed=1,
-        prior_features=prior_features,
-        prior_rewards=prior_rewards,
     )
-    self.assertEqual(eagle.prior_features.shape, (n_prior_trials, 2))
+    init_state = eagle.init_state(
+        jax.random.PRNGKey(0), prior_features, prior_rewards
+    )
+    self.assertEqual(init_state.features.shape, (config.pool_size, 2))
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py` & `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/random_vectorized_optimizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,68 +14,74 @@
 
 from __future__ import annotations
 
 """Random vectorized optimizer to be used in convergence test."""
 
 from typing import Optional
 
-import numpy as np
+import jax
 from vizier._src.algorithms.optimizers import vectorized_base as vb
+from vizier._src.jax import types
 from vizier.pyvizier import converters
 
 
 class RandomVectorizedStrategy(vb.VectorizedStrategy):
   """Random vectorized strategy."""
 
   def __init__(
       self,
       converter: converters.TrialToArrayConverter,
       suggestion_batch_size: int,
-      seed: Optional[int] = None,
-      prior_features: Optional[np.ndarray] = None,
-      prior_rewards: Optional[np.ndarray] = None,
   ):
     self._converter = converter
     self._suggestion_batch_size = suggestion_batch_size
-    self._rng = np.random.default_rng(seed)
     self._n_features = sum(
         [spec.num_dimensions for spec in self._converter.output_specs]
     )
 
-  def suggest(self) -> vb.Array:
-    return self._rng.uniform(
-        low=0,
-        high=1,
-        size=(
+  def init_state(
+      self,
+      seed: jax.random.KeyArray,
+      prior_features: Optional[types.Array] = None,
+      prior_rewards: Optional[types.Array] = None,
+  ) -> None:
+    del seed
+    return
+
+  def suggest(self, state: None, seed: jax.random.KeyArray) -> jax.Array:
+    del state
+    return jax.random.uniform(
+        seed,
+        shape=(
             self._suggestion_batch_size,
             self._n_features,
         ),
     )
 
   def suggestion_batch_size(self) -> int:
     return self._suggestion_batch_size
 
-  def update(self, rewards: vb.Array) -> None:
-    pass
+  def update(
+      self,
+      state: None,
+      batch_features: types.Array,
+      batch_rewards: types.Array,
+      seed: jax.random.KeyArray,
+  ) -> None:
+    return
 
 
 def _random_strategy_factory(
     converter: converters.TrialToArrayConverter,
     suggestion_batch_size: int,
-    seed: Optional[int] = None,
-    prior_features: Optional[np.ndarray] = None,
-    prior_rewards: Optional[np.ndarray] = None,
 ) -> vb.VectorizedStrategy:
   """Creates a new vectorized strategy based on the Protocol."""
   return RandomVectorizedStrategy(
       converter=converter,
       suggestion_batch_size=suggestion_batch_size,
-      seed=seed,
-      prior_features=prior_features,
-      prior_rewards=prior_rewards,
   )
 
 
 def create_random_optimizer(
     max_evaluations: int, suggestion_batch_size: int
 ) -> vb.VectorizedOptimizer:
   """Creates a random optimizer."""
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/optimizers/random_vectorized_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/optimizers/vectorized_base_test.py` & `google-vizier-0.1.5/vizier/_src/pyglove/converters_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,262 +10,224 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-"""Tests for vectorized_base."""
+"""Tests for converters."""
 
-import datetime
-import time
-from typing import Optional
-
-import mock
-import numpy as np
+import pyglove as pg
 from vizier import pyvizier as vz
-from vizier._src.algorithms.optimizers import vectorized_base as vb
-from vizier.pyvizier import converters
-
+from vizier._src.pyglove import constants
+from vizier._src.pyglove import converters
 from absl.testing import absltest
 from absl.testing import parameterized
 
 
-class FakeIncrementVectorizedStrategy(vb.VectorizedStrategy):
-  """Fake vectorized strategy with incrementing suggestions."""
-
-  def __init__(self, *args, **kwargs):
-    self._iter = 0
-
-  def suggest(self) -> np.ndarray:
-    # The following structure allows to test the top K results.
-    suggestions = (
-        np.array([
-            [self._iter % 10, self._iter % 10],
-            [(self._iter + 1) % 10, (self._iter + 1) % 10],
-            [(self._iter + 2) % 10, (self._iter + 2) % 10],
-            [(self._iter + 3) % 10, (self._iter + 3) % 10],
-            [(self._iter + 4) % 10, (self._iter + 4) % 10],
-        ])
-        / 10
-    )
-    self._iter += 5
-    return suggestions
-
-  @property
-  def suggestion_batch_size(self) -> int:
-    return 5
-
-  def update(self, rewards: np.ndarray) -> None:
-    pass
-
-
-# pylint: disable=unused-argument
-def fake_increment_strategy_factory(
-    converter: converters.TrialToArrayConverter,
-    suggestion_batch_size: int,
-    seed: Optional[int] = None,
-    prior_features: Optional[np.ndarray] = None,
-    prior_rewards: Optional[np.ndarray] = None,
-) -> vb.VectorizedStrategy:
-  return FakeIncrementVectorizedStrategy()
-
-
-class FakePriorTrialsVectorizedStrategy(vb.VectorizedStrategy):
-  """Fake vectorized strategy to test prior trials."""
-
-  def __init__(self, prior_features: np.ndarray, prior_rewards: np.ndarray):
-    self.seed_features, self.seed_rewards = prior_features, prior_rewards
-    if len(self.seed_rewards.shape) != 1:
-      raise ValueError('Expected seed labels to have 1D dimension!')
-
-  def suggest(self) -> np.ndarray:
-    return self.seed_features[np.argmax(self.seed_rewards, axis=-1)].reshape(
-        1, -1
-    )
-
-  @property
-  def suggestion_batch_size(self) -> int:
-    return 1
-
-  def update(self, rewards: np.ndarray) -> None:
-    pass
-
-
-# pylint: disable=unused-argument
-def fake_prior_trials_strategy_factory(
-    converter: converters.TrialToArrayConverter,
-    suggestion_batch_size: int,
-    seed: Optional[int] = None,
-    prior_features: Optional[np.ndarray] = None,
-    prior_rewards: Optional[np.ndarray] = None,
-) -> vb.VectorizedStrategy:
-  return FakePriorTrialsVectorizedStrategy(prior_features, prior_rewards)
-
-
-class VectorizedBaseTest(parameterized.TestCase):
-
-  @parameterized.parameters(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
-  def test_optimize_candidates_len(self, count):
-    problem = vz.ProblemStatement()
-    problem.search_space.root.add_float_param('f1', 0.0, 10.0)
-    problem.search_space.root.add_float_param('f2', 0.0, 10.0)
-    converter = converters.TrialToArrayConverter.from_study_config(problem)
-    score_fn = lambda x: np.sum(x, axis=-1)
-    optimizer = vb.VectorizedOptimizer(
-        strategy_factory=fake_increment_strategy_factory,
-        max_evaluations=100,
-    )
-    res = optimizer.optimize(
-        converter=converter, score_fn=score_fn, count=count
-    )
-    self.assertLen(res, count)
+class VizierCreatedSearchSpaceTest(parameterized.TestCase):
+  """Tests for search space created from vz.SearchSpace."""
 
-  @parameterized.parameters([None, datetime.timedelta(minutes=10)])
-  def test_should_stop_max_evaluations(self, max_duration):
-    problem = vz.ProblemStatement()
-    problem.search_space.root.add_float_param('f1', 0.0, 10.0)
-    problem.search_space.root.add_float_param('f2', 0.0, 10.0)
-    converter = converters.TrialToArrayConverter.from_study_config(problem)
-    score_fn = mock.Mock()
-    score_fn.side_effect = lambda x: np.sum(x, axis=-1)
-    optimizer = vb.VectorizedOptimizer(
-        strategy_factory=fake_increment_strategy_factory,
-        max_evaluations=100,
-        max_duration=max_duration,
-    )
-    optimizer.optimize(converter=converter, score_fn=score_fn, count=3)
-    # The batch size is 5, so we expect 100/5 = 20 calls
-    self.assertEqual(score_fn.call_count, 20)
-
-  def test_best_candidates_count_is_1(self):
-    problem = vz.ProblemStatement()
-    problem.search_space.root.add_float_param('f1', 0.0, 1.0)
-    problem.search_space.root.add_float_param('f2', 0.0, 1.0)
-    converter = converters.TrialToArrayConverter.from_study_config(problem)
-    score_fn = lambda x: -np.max(np.square(x - 0.52), axis=-1)
-    strategy_factory = FakeIncrementVectorizedStrategy
-    optimizer = vb.VectorizedOptimizer(
-        strategy_factory=strategy_factory, max_evaluations=10
-    )
-    best_candidates = optimizer.optimize(
-        converter=converter, score_fn=score_fn, count=1
-    )
-    # check the best candidate
-    self.assertEqual(best_candidates[0].parameters['f1'].value, 0.5)
-    self.assertEqual(best_candidates[0].parameters['f2'].value, 0.5)
+  def _search_space(self) -> vz.SearchSpace:
+    ss = vz.SearchSpace()
+    root = ss.root
+    root.add_float_param('double', -1., 1.)
+    root.add_int_param('int', 2, 4)
+    root.add_discrete_param('discrete_int', (-2, 4, 7, 8))
+    root.add_discrete_param('discrete_double', (-2.1, 4.1, 7.1, 8.1))
+    root.add_categorical_param('categorical', ('a', 'b', 'c'))
+    return ss
+
+  def test_dna_spec(self):
+    vc = converters.VizierConverter.from_problem(
+        vz.ProblemStatement(self._search_space()))
+    self.assertLen(vc.dna_spec, 5)
+    self.assertNotEmpty(
+        vc.problem.metadata.ns(constants.METADATA_NAMESPACE)[
+            constants.STUDY_METADATA_KEY_DNA_SPEC])
+
+  def test_dna_to_trial(self):
+    vc = converters.VizierConverter.from_problem(
+        vz.ProblemStatement(self._search_space()))
+    self.assertDictEqual(
+        vc.to_trial(vc.dna_spec.first_dna(),
+                    fallback='raise_error').parameters.as_dict(), {
+                        'double': -1,
+                        'int': 2,
+                        'discrete_int': -2,
+                        'discrete_double': -2.1,
+                        'categorical': 'a'
+                    })
+
+  @parameterized.parameters((7,), (7.,))
+  def test_trial_to_dna(self, discrete_int_value):
+    vc = converters.VizierConverter.from_problem(
+        vz.ProblemStatement(search_space=self._search_space()))
+    trial = vz.Trial()
+    trial.parameters['double'] = -.5
+    trial.parameters['int'] = 3
+    trial.parameters['discrete_int'] = discrete_int_value
+    trial.parameters['discrete_double'] = 4.1
+    trial.parameters['categorical'] = 'a'
+    self.assertEqual(vc.to_dna(trial), pg.DNA([-.5, 1, 2, 1, 0]))
+
+
+class PyGloveCreatedSearchSpaceTest(parameterized.TestCase):
+  """Tests for PyGlove created search space."""
+
+  def _dna_spec(self) -> pg.DNASpec:
+
+    class CustomTypeDecision(pg.hyper.CustomHyper):
+
+      def custom_decode(self, dna):
+        return dna.value
+
+    search_space = pg.Dict(
+        a=CustomTypeDecision(),
+        x=pg.oneof([3, 3, 2, 2]),
+        y=pg.floatv(0.1, 2.0),
+        z=pg.oneof(['foo', 'bar']))
+    return pg.dna_spec(search_space)
+
+  def test_search_space(self):
+    vc = converters.VizierConverter.from_dna_spec(self._dna_spec())
+    # Custom-type decision point `a` is not part of the search space.
+    self.assertLen(vc.search_space.parameters, 3)
+    self.assertNotEmpty(
+        vc.problem.metadata.ns(constants.METADATA_NAMESPACE)[
+            constants.STUDY_METADATA_KEY_DNA_SPEC])
+
+  def test_dna_to_trial(self):
+    dna_spec = self._dna_spec()
+    vc = converters.VizierConverter.from_dna_spec(dna_spec)
+    dna = pg.DNA(['abc', 0, 0.5, 1], spec=dna_spec)
+    trial = vc.to_trial(dna, fallback='raise_error')
+    self.assertLen(trial.parameters, 3)
+    self.assertEqual(trial.parameters['x'], vz.ParameterValue(3))
+    self.assertEqual(trial.parameters['y'], vz.ParameterValue(0.5))
+    self.assertEqual(trial.parameters['z'], vz.ParameterValue('1/2 (\'bar\')'))
     self.assertEqual(
-        best_candidates[0].final_measurement.metrics['acquisition'].value,
-        -((0.5 - 0.52) ** 2),
-    )
-
-  def test_best_candidates_count_is_3(self):
-    problem = vz.ProblemStatement()
-    problem.search_space.root.add_float_param('f1', 0.0, 1.0)
-    problem.search_space.root.add_float_param('f2', 0.0, 1.0)
-    converter = converters.TrialToArrayConverter.from_study_config(problem)
-    score_fn = lambda x: -np.max(np.square(x - 0.52), axis=-1)
-    optimizer = vb.VectorizedOptimizer(
-        strategy_factory=fake_increment_strategy_factory, max_evaluations=10
-    )
-    best_candidates = optimizer.optimize(
-        converter=converter, score_fn=score_fn, count=3
-    )
-    # check 1st best candidate
-    self.assertEqual(best_candidates[0].parameters['f1'].value, 0.5)
-    self.assertEqual(best_candidates[0].parameters['f2'].value, 0.5)
-    self.assertEqual(
-        best_candidates[0].final_measurement.metrics['acquisition'].value,
-        -((0.5 - 0.52) ** 2),
-    )
-    # check 2nd best candidate
-    self.assertEqual(best_candidates[1].parameters['f1'].value, 0.6)
-    self.assertEqual(best_candidates[1].parameters['f2'].value, 0.6)
-    self.assertEqual(
-        best_candidates[1].final_measurement.metrics['acquisition'].value,
-        -((0.6 - 0.52) ** 2),
-    )
-    # check 3rd best candidate
-    self.assertEqual(best_candidates[2].parameters['f1'].value, 0.4)
-    self.assertEqual(best_candidates[2].parameters['f2'].value, 0.4)
+        pg.from_json_str(
+            trial.metadata.ns(constants.METADATA_NAMESPACE)
+            [constants.TRIAL_METADATA_KEY_CUSTOM_TYPE_DECISIONS]), {'a': 'abc'})
+
+  def test_trial_to_dna(self):
+    vc = converters.VizierConverter.from_dna_spec(self._dna_spec())
+    trial = vz.Trial()
+    trial.parameters['x'] = 2.0
+    trial.parameters['y'] = 0.5
+    trial.parameters['z'] = '1/2 (\'bar\')'
+    trial.metadata.ns(constants.METADATA_NAMESPACE)[
+        constants.TRIAL_METADATA_KEY_CUSTOM_TYPE_DECISIONS] = pg.to_json_str(
+            {'a': 'abc'})
+    self.assertEqual(vc.to_dna(trial), pg.DNA(['abc', 3, 0.5, 1]))
+
+
+class MakeParameterConfigTest(absltest.TestCase):
+  """Tests for make parameter configs from DNASpec."""
+
+  def testScale(self):
+    """Test scale type conversion."""
+    self.assertEqual(converters.get_scale_type(None), vz.ScaleType.LINEAR)
+    self.assertEqual(converters.get_scale_type('linear'), vz.ScaleType.LINEAR)
+    self.assertEqual(converters.get_scale_type('log'), vz.ScaleType.LOG)
     self.assertEqual(
-        best_candidates[2].final_measurement.metrics['acquisition'].value,
-        -((0.4 - 0.52) ** 2),
-    )
+        converters.get_scale_type('rlog'), vz.ScaleType.REVERSE_LOG)
+    with self.assertRaisesRegex(
+        ValueError, 'Unsupported scale type'):
+      converters.get_scale_type('unknown')
+
+  def testHyperValueAsRoot(self):
+    """Test using hyper value as search space root."""
+    search_space = pg.oneof([1, 2])
+    actual = converters.VizierConverter.from_dna_spec(
+        pg.dna_spec(search_space)).search_space
+    expected = vz.SearchSpace()
+    expected.root.add_discrete_param('$', [1, 2])
+    self.assertEqual(actual, expected)
+
+  def testFlatSearchSpace(self):
+    """Test flat search spaces."""
+
+    class CustomDecisionPoint(pg.geno.CustomDecisionPoint):
+
+      def custom_decode(self, dna):
+        return dna.value
+
+    search_space = pg.Dict(
+        # custom decision point 'a' will not be inserted as a part of
+        # parameter config.
+        a=CustomDecisionPoint(),
+        x=pg.oneof([2, 2, 1]),
+        y=[pg.floatv(1e-6, 1.0, scale='log')],
+        z=pg.Dict(p=pg.manyof(2, ['foo', 'bar'])))
+    actual = converters.VizierConverter.from_dna_spec(
+        pg.dna_spec(search_space)).search_space
+    expected = vz.SearchSpace()
+    root = expected.root
+    # Feasible points of discrete params are sorted.
+    root.add_discrete_param('x', [1, 2])
+    root.add_float_param('y[0]', 1e-6, 1.0, scale_type=vz.ScaleType.LOG)
+    root.add_categorical_param('z.p[0]', ['0/2 (\'foo\')', '1/2 (\'bar\')'])
+    root.add_categorical_param('z.p[1]', ['0/2 (\'foo\')', '1/2 (\'bar\')'])
+
+    self.assertEqual(actual, expected)
+
+  def testHierarchicalSearchSpace(self):
+    """Test hierarchical search space."""
+    search_space = pg.oneof([[pg.oneof([1, 2])],
+                             pg.Dict(x=pg.floatv(0.1, 0.5)),
+                             pg.manyof(2,
+                                       [pg.oneof(['foo', 'bar']), True, False])
+                            ])
+    actual = converters.VizierConverter.from_dna_spec(
+        pg.dna_spec(search_space)).search_space
+
+    expected = vz.SearchSpace()
+    root = expected.root
+    categories = [
+        '0/3 ([0: OneOf(candidates=[0: 1, 1: 2])])',
+        '1/3 ({x=Float(min_value=0.1, max_value=0.5)})',
+        ('2/3 (ManyOf(num_choices=2, candidates=[0: OneOf('
+         'candidates=[0: \'foo\', 1: \'bar\']), 1: True, 2: False]))')
+    ]
+    dollar = root.add_categorical_param('$', categories)
+    dollar.select_values([categories[0]]).add_discrete_param(
+        '[=0/3][0]',
+        [
+            1,
+            2,
+        ],
+    )
+    dollar.select_values([categories[1]]).add_float_param(
+        name='[=1/3].x',
+        min_value=0.1,
+        max_value=0.5,
+        scale_type=vz.ScaleType.LINEAR,
+    )
+
+    branch2 = dollar.select_values([categories[2]])
+
+    def _add_children(name):
+      branch2.add_categorical_param(
+          name,
+          [
+              '0/3 (OneOf(candidates=[0: \'foo\', 1: \'bar\']))', '1/3 (True)',
+              '2/3 (False)'
+          ],
+      ).select_values(['0/3 (OneOf(candidates=[0: \'foo\', 1: \'bar\']))'
+                      ]).add_categorical_param(
+                          f'{name}[=0/3]',
+                          [
+                              '0/2 (\'foo\')',
+                              '1/2 (\'bar\')',
+                          ],
+                      )
 
-  def test_should_stop_max_duration(self):
-    problem = vz.ProblemStatement()
-    problem.search_space.root.add_float_param('f1', 0.0, 10.0)
-    problem.search_space.root.add_float_param('f2', 0.0, 10.0)
-    converter = converters.TrialToArrayConverter.from_study_config(problem)
-    score_fn = mock.Mock()
-
-    def slow_score_fn(x):
-      time.sleep(1)
-      return np.sum(x, axis=-1)
-
-    score_fn.side_effect = slow_score_fn
-    optimizer = vb.VectorizedOptimizer(
-        strategy_factory=fake_increment_strategy_factory,
-        max_evaluations=100,
-        max_duration=datetime.timedelta(seconds=3),
-    )
-    optimizer.optimize(converter=converter, score_fn=score_fn)
-    # Test the optimization stopped after ~3 seconds based on function calls.
-    self.assertLess(score_fn.call_count, 4)
-
-  def test_vectorized_optimizer_factory(self):
-    optimizer_factory = vb.VectorizedOptimizerFactory(
-        strategy_factory=fake_increment_strategy_factory
-    )
-    optimizer = optimizer_factory(suggestion_batch_size=5, max_evaluations=1000)
-    self.assertEqual(optimizer.max_evaluations, 1000)
-    self.assertEqual(optimizer.suggestion_batch_size, 5)
-
-  def test_prior_trials(self):
-    """Test that the optimizer can correctly parsae and pass seed trials."""
-    optimizer_factory = vb.VectorizedOptimizerFactory(
-        strategy_factory=fake_prior_trials_strategy_factory
-    )
-    optimizer = optimizer_factory(suggestion_batch_size=5, max_evaluations=100)
-
-    study_config = vz.ProblemStatement(
-        metric_information=[
-            vz.MetricInformation(
-                name='obj', goal=vz.ObjectiveMetricGoal.MAXIMIZE
-            )
-        ]
-    )
-    root = study_config.search_space.root
-    root.add_float_param('x1', 0.0, 10.0)
-    root.add_float_param('x2', 0.0, 10.0)
-    converter = converters.TrialToArrayConverter.from_study_config(study_config)
-
-    trial1 = vz.Trial(parameters={'x1': 1, 'x2': 1})
-    measurement1 = vz.Measurement(metrics={'obj': vz.Metric(value=-10.33)})
-    trial1.complete(measurement1, inplace=True)
-
-    trial2 = vz.Trial(parameters={'x1': 2, 'x2': 2})
-    measurement2 = vz.Measurement(metrics={'obj': vz.Metric(value=5.0)})
-    trial2.complete(measurement2, inplace=True)
-
-    best_trial = optimizer.optimize(
-        converter,
-        lambda x: -np.max(np.square(x - 0.52), axis=-1),
-        count=1,
-        prior_trials=[trial1, trial2, trial1],
-    )
-    self.assertEqual(best_trial[0].parameters['x1'].value, 2)
-    self.assertEqual(best_trial[0].parameters['x2'].value, 2)
-
-    best_trial = optimizer.optimize(
-        converter,
-        lambda x: -np.max(np.square(x - 0.52), axis=-1),
-        count=1,
-        prior_trials=[trial1],
-    )
-    self.assertEqual(best_trial[0].parameters['x1'].value, 1)
-    self.assertEqual(best_trial[0].parameters['x2'].value, 1)
+    _add_children('[=2/3][0]')
+    _add_children('[=2/3][1]')
+    self.assertEqual(
+        expected, actual, msg=f'expected={expected}, actual={actual}')
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/policies/__init__.py` & `google-vizier-0.1.5/vizier/_src/algorithms/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/policies/designer_policy.py` & `google-vizier-0.1.5/vizier/_src/algorithms/policies/designer_policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,44 +50,80 @@
   future `suggest()` calls.
   """
 
   def __init__(
       self,
       supporter: pythia.PolicySupporter,
       designer_factory: vza.DesignerFactory[vza.Designer],
+      *,
+      policy_name: str = 'DesignerPolicy',
   ):
     """Init.
 
     Args:
       supporter:
       designer_factory:
+      policy_name: A user visible name.
     """
     self._supporter = supporter
     self._designer_factory = designer_factory
+    self._policy_name = policy_name
 
   def suggest(self, request: pythia.SuggestRequest) -> pythia.SuggestDecision:
+    logging.info(
+        'Processing request for study guid %s, with max trial id %s',
+        request.study_guid,
+        request.max_trial_id,
+    )
     designer = self._designer_factory(request.study_config)
+    logging.info(
+        'Study guid %s: Designer created. Getting trials from Vizier service.',
+        request.study_guid,
+    )
     completed = self._supporter.GetTrials(
         status_matches=vz.TrialStatus.COMPLETED
     )
+    logging.info(
+        'Study guid %s: got %s COMPLETED trials',
+        request.study_guid,
+        len(completed),
+    )
     active = self._supporter.GetTrials(status_matches=vz.TrialStatus.ACTIVE)
+    logging.info(
+        'Study guid %s: got %s ACTIVE trials', request.study_guid, len(active)
+    )
+    logging.info(
+        'Study guid %s: Updating designer with trials.', request.study_guid
+    )
     designer.update(vza.CompletedTrials(completed), vza.ActiveTrials(active))
     self._designer = designer  # saved for debugging purposes only.
+    logging.info(
+        'Study guid %s: Asking designer for %s suggestions.',
+        request.study_guid,
+        request.count,
+    )
     return pythia.SuggestDecision(
-        designer.suggest(request.count), metadata=vz.MetadataDelta())
+        designer.suggest(request.count), metadata=vz.MetadataDelta()
+    )
 
-  def early_stop(self,
-                 request: pythia.EarlyStopRequest) -> pythia.EarlyStopDecisions:
+  def early_stop(
+      self, request: pythia.EarlyStopRequest
+  ) -> pythia.EarlyStopDecisions:
     raise NotImplementedError(
-        'DesignerPolicy does not support the early_stop() method.')
+        'DesignerPolicy does not support the early_stop() method.'
+    )
+
+  @property
+  def name(self) -> str:
+    return self._policy_name
 
 
-class _SerializableDesignerPolicyBase(pythia.Policy,
-                                      serializable.PartiallySerializable,
-                                      Generic[_T], abc.ABC):
+class _SerializableDesignerPolicyBase(
+    pythia.Policy, serializable.PartiallySerializable, Generic[_T], abc.ABC
+):
   """Partially implemented class for wrapping a (Partially)SerializableDesigner.
 
   Inherited by (Partially)SerializableDesignerPolicy which is fully implemented.
 
   (Partially)SerializableDesignerPolicy maintains a synchronized state between
   the set of trial ids that were passed to Designer via `update()` call, and
   the Designer instance that was used for during last `suggest()` call.
@@ -115,34 +151,37 @@
       problem_statement: vz.ProblemStatement,
       supporter: pythia.PolicySupporter,
       designer_factory: vza.DesignerFactory[_T],
       *,
       ns_root: str = 'designer_policy_v0',
       verbose: int = 0,
       seed: Optional[int] = None,
+      policy_name: str = '_SerializableDesignerPolicyBase',
   ):
     """Init.
 
     Args:
       problem_statement:
       supporter:
       designer_factory: Factory function to create.
         (Partially)SerializableDesigner designers.
       ns_root: Root of the namespace where policy state is stored.
       verbose: Logging verbosity.
       seed: Random seed to be passed to the designer factory.
+      policy_name: A user visible name.
     """
     self._supporter = supporter
     self._designer_factory = designer_factory
     self._ns_root = ns_root
     self._incorporated_completed_trial_ids: set[int] = set()
     self._problem_statement = problem_statement
     self._verbose = verbose
     self._designer = None
     self._seed = seed
+    self._policy_name = policy_name
 
   def suggest(self, request: pythia.SuggestRequest) -> pythia.SuggestDecision:
     """Perform a suggest operation.
 
     The order of operations is:
     1. Initialize the designer and load its state from metadata.
     2. Update the designer with newly completed trials.
@@ -179,28 +218,33 @@
         len(active_trials),
         len(self._incorporated_completed_trial_ids),
     )
     metadata_delta = vz.MetadataDelta()
     # During the 'suggest' call the designer's state could be changed, therefore
     # the state is dumped and stored only after 'suggest' was called.
     suggestions = pythia.SuggestDecision(
-        self.designer.suggest(request.count), metadata=metadata_delta)
+        self.designer.suggest(request.count), metadata=metadata_delta
+    )
     metadata_delta.on_study.ns(self._ns_root).attach(self.dump())
     return suggestions
 
-  def early_stop(self,
-                 request: pythia.EarlyStopRequest) -> pythia.EarlyStopDecisions:
+  def early_stop(
+      self, request: pythia.EarlyStopRequest
+  ) -> pythia.EarlyStopDecisions:
     raise NotImplementedError(
-        'PartiallySerializableDesignerPolicy does not implement early_stop().')
+        'PartiallySerializableDesignerPolicy does not implement early_stop().'
+    )
 
   @property
   def designer(self) -> _T:
     if self._designer is None:
-      raise ValueError('`self._designer` has not been initialized!'
-                       'Use self._restore_designer(..) to initialize it.')
+      raise ValueError(
+          '`self._designer` has not been initialized!'
+          'Use self._restore_designer(..) to initialize it.'
+      )
     return self._designer
 
   @abc.abstractmethod
   def _restore_designer(self, designer_metadata: vz.Metadata) -> _T:
     """Creates a new Designer by restoring the state from `designer_metadata`.
 
     Args:
@@ -232,16 +276,17 @@
             'Successfully recovered the policy state, which incorporated %s '
             'completed trials.'
         ),
         len(self._incorporated_completed_trial_ids),
     )
     self._designer = self._restore_designer(md.ns(self._ns_designer))
 
-  def _initialize_designer(self,
-                           problem_statement: vz.ProblemStatement) -> None:
+  def _initialize_designer(
+      self, problem_statement: vz.ProblemStatement
+  ) -> None:
     """Guarantees that `self._designer` is populated.
 
     This method guarantees that after a successful call, `self.designer` does
     not raise an Exception.
     This method catches all DecodeErrors.
 
     Args:
@@ -253,33 +298,38 @@
     """
     if self._designer is not None:
       # When the same policy object is maintained in RAM, prefer keeping
       # the designer object over restoring the state from metadata.
       # TOCONSIDER: Adding a boolean knob to turn off this behavior.
       logging.log_if(
           logging.INFO,
-          ('Policy already has a designer. '
-           'It will not attempt to load from metadata.'),
+          (
+              'Policy already has a designer. '
+              'It will not attempt to load from metadata.'
+          ),
           self._verbose >= 2,
       )
       return
     elif self._problem_statement != problem_statement:
       raise ValueError(
           f'{type(self)} cannot be re-used for different study configs!'
           f'Policy: {self}, previous study: {self._problem_statement} '
-          f'new study: {problem_statement}')
+          f'new study: {problem_statement}'
+      )
 
     metadata = problem_statement.metadata.ns(self._ns_root)
     try:
       self.load(metadata)
-      logging.log_if(logging.INFO, 'Successfully decoded all states!',
-                     self._verbose >= 1)
+      logging.log_if(
+          logging.INFO, 'Successfully decoded all states!', self._verbose >= 1
+      )
     except serializable.DecodeError as e:
-      logging.log_if(logging.INFO, 'Failed to decode state. %s',
-                     self._verbose >= 1, e)
+      logging.log_if(
+          logging.INFO, 'Failed to decode state. %s', self._verbose >= 1, e
+      )
       # Restart the state of the policy.
       self._designer = self._designer_factory(
           problem_statement, seed=self._seed
       )
       self._incorporated_completed_trial_ids: set[int] = set()
 
   def dump(self) -> vz.Metadata:
@@ -331,14 +381,18 @@
         'Loaded %s %s trials. Max trial id is %s.',
         len(new_trials),
         status,
         max_trial_id,
     )
     return new_trials
 
+  @property
+  def name(self) -> str:
+    return self._policy_name
+
 
 # TODO: Rewrite base to separate incorporated trial logic from
 # serialization logic. For now, it simply disables the serialization.
 class InRamDesignerPolicy(_SerializableDesignerPolicyBase[vza.Designer]):
   """Wraps a Designer in RAM for efficient updates()."""
 
   # Override restore() to simply return the designer.
@@ -347,27 +401,29 @@
 
   # Override dump() since this is in ram.
   def dump(self) -> vz.Metadata:
     return vz.Metadata()
 
 
 class PartiallySerializableDesignerPolicy(
-    _SerializableDesignerPolicyBase[vza.PartiallySerializableDesigner]):
+    _SerializableDesignerPolicyBase[vza.PartiallySerializableDesigner]
+):
   """Wraps a PartiallySerializableDesigner."""
 
   def _restore_designer(
-      self,
-      designer_metadata: vz.Metadata) -> vza.PartiallySerializableDesigner:
+      self, designer_metadata: vz.Metadata
+  ) -> vza.PartiallySerializableDesigner:
     designer = self._designer_factory(self._problem_statement)
     designer.load(designer_metadata)
     return designer
 
 
 class SerializableDesignerPolicy(
-    _SerializableDesignerPolicyBase[vza.SerializableDesigner]):
+    _SerializableDesignerPolicyBase[vza.SerializableDesigner]
+):
   """Wraps a SerializableDesigner."""
 
   def __init__(
       self,
       problem_statement: vz.ProblemStatement,
       supporter: pythia.PolicySupporter,
       designer_factory: vza.DesignerFactory[vza.SerializableDesigner],
@@ -393,9 +449,10 @@
         designer_factory,
         ns_root=ns_root,
         verbose=verbose,
     )
     self._designer_cls = designer_cls
 
   def _restore_designer(
-      self, designer_metadata: vz.Metadata) -> vza.SerializableDesigner:
+      self, designer_metadata: vz.Metadata
+  ) -> vza.SerializableDesigner:
     return self._designer_cls.recover(designer_metadata)
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/policies/designer_policy_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/policies/designer_policy_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/policies/random_policy.py` & `google-vizier-0.1.5/vizier/_src/algorithms/policies/random_policy.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/policies/random_policy_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/policies/random_policy_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/random/random_sample.py` & `google-vizier-0.1.5/vizier/_src/algorithms/random/random_sample.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/random/random_sample_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/random/random_sample_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/regression/trial_regression_utils.py` & `google-vizier-0.1.5/vizier/_src/algorithms/regression/trial_regression_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/regression/trial_regression_utils_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/regression/trial_regression_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/testing/__init__.py` & `google-vizier-0.1.5/vizier/_src/algorithms/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/testing/comparator_runner.py` & `google-vizier-0.1.5/vizier/_src/algorithms/testing/comparator_runner.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/testing/comparator_runner_test.py` & `google-vizier-0.1.5/vizier/_src/algorithms/testing/comparator_runner_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,23 @@
 
 from __future__ import annotations
 
 """Tests for comparator_runner."""
 
 from typing import Optional, Sequence
 
+import jax
+from jax import numpy as jnp
 import numpy as np
 from vizier import algorithms as vza
 from vizier import benchmarks
 from vizier import pyvizier as vz
 from vizier._src.algorithms.optimizers import vectorized_base as vb
 from vizier._src.algorithms.testing import comparator_runner
+from vizier._src.jax import types
 from vizier.benchmarks import experimenters
 from vizier.pyvizier import converters
 
 from absl.testing import absltest
 from absl.testing import parameterized
 
 
@@ -43,28 +46,42 @@
   ):
     self.converter = converter
     self.good_value = good_value
     self.bad_value = bad_value
     self.num_trial_to_converge = num_trial_to_converge
     self.num_trials_so_far = 0
 
-  def suggest(self) -> np.ndarray:
+  def init_state(
+      self,
+      seed: jax.random.KeyArray,
+      prior_features: Optional[types.Array] = None,
+      prior_rewards: Optional[types.Array] = None,
+  ) -> None:
+    return
+
+  def suggest(self, state: None, seed: jax.random.KeyArray) -> jax.Array:
     output_len = sum(
         [spec.num_dimensions for spec in self.converter.output_specs]
     )
     if self.num_trials_so_far < self.num_trial_to_converge:
-      return np.ones((1, output_len)) * self.bad_value
+      return jnp.ones((1, output_len)) * self.bad_value
     else:
-      return np.ones((1, output_len)) * self.good_value
+      return jnp.ones((1, output_len)) * self.good_value
 
   @property
   def suggestion_batch_size(self) -> int:
     return 1
 
-  def update(self, rewards: np.ndarray) -> None:
+  def update(
+      self,
+      state: None,
+      batch_features: types.Array,
+      batch_rewards: types.Array,
+      seed: jax.random.KeyArray,
+  ) -> None:
     pass
 
 
 class FakeDesigner(vza.Designer):
   """Dummy designer to control convergence."""
 
   def __init__(
@@ -311,29 +328,25 @@
         baseline_num_repeats=5,
         candidate_num_repeats=5,
         alpha=0.05,
         goal=goal,
     )
 
     # pylint: disable=unused-argument
-    def _baseline_strategy_factory(
-        converter, suggestion_batch_size, seed, prior_features, prior_rewards
-    ):
+    def _baseline_strategy_factory(converter, suggestion_batch_size):
       return FakeVectorizedStrategy(
           converter=converter,
           good_value=1.0,
           bad_value=1.0,
           num_trial_to_converge=0,
       )
 
       # pylint: disable=unused-argument
 
-    def _candidate_strategy_factory(
-        converter, suggestion_batch_size, seed, prior_features, prior_rewards
-    ):
+    def _candidate_strategy_factory(converter, suggestion_batch_size):
       return FakeVectorizedStrategy(
           converter=converter,
           good_value=candidate_x_value,
           bad_value=0.0,
           num_trial_to_converge=0,
       )
```

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/testing/optimizer_test_utils.py` & `google-vizier-0.1.5/vizier/_src/algorithms/testing/optimizer_test_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/algorithms/testing/test_runners.py` & `google-vizier-0.1.5/vizier/_src/algorithms/testing/test_runners.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Test runners for algorithms."""
-from typing import Any, Callable, Collection, Optional, Sequence
+from typing import Any, Callable, List, Optional, Sequence
 
 
 from absl import logging
 import attr
 import numpy as np
 from vizier import algorithms as vza
 from vizier import benchmarks
@@ -69,54 +69,62 @@
     iters: Number of suggest-update iterations.
     batch_size: Number of suggestions to ask in each suggest() call.
     seed: Random seed for generating metrics.
     verbose: Increase the verbosity to see more logs.
     validate_parameters: If True, check if the suggested trials are valid in the
       search space.
   """
+
   problem: vz.ProblemStatement = attr.field()
   iters: int = attr.field(default=5)
   batch_size: Optional[int] = attr.field(default=1, kw_only=True)
   seed: Any = attr.field(default=None, kw_only=True)
   verbose: int = attr.field(default=0, kw_only=True)
   validate_parameters: bool = attr.field(default=False, kw_only=True)
 
-  def _run(self, algorithm: benchmarks.PolicySuggester) -> Collection[vz.Trial]:
+  def _run(self, algorithm: benchmarks.PolicySuggester) -> List[vz.Trial]:
     """Implementation of run methods."""
     rng = np.random.RandomState(self.seed)
     for it in range(self.iters):
       suggestions = algorithm.suggest(self.batch_size)
       if not suggestions:
         logging.info(
-            'Preemptively finished at iteration %s'
-            'because designer returned nothing.', it)
+            (
+                'Preemptively finished at iteration %s'
+                'because designer returned nothing.'
+            ),
+            it,
+        )
         break
       trials = []
       for suggestion in suggestions:
         if self.validate_parameters:
           self.problem.search_space.assert_contains(suggestion.parameters)
         measurement = vz.Measurement()
         for mi in self.problem.metric_information:
           measurement.metrics[mi.name] = rng.uniform(
-              mi.min_value_or(lambda: -10.), mi.max_value_or(lambda: 10.))
+              mi.min_value_or(lambda: -10.0), mi.max_value_or(lambda: 10.0)
+          )
         trials.append(suggestion.complete(measurement))
       if self.verbose:
-        logging.info('At iteration %s, trials suggested and evaluated:\n%s', it,
-                     trials)
+        logging.info(
+            'At iteration %s, trials suggested and evaluated:\n%s', it, trials
+        )
       algorithm.supporter.AddTrials(trials)
     return algorithm.supporter.GetTrials()
 
-  def run_policy(self, policy_factory: Callable[[pythia.PolicySupporter],
-                                                pythia.Policy]):
+  def run_policy(
+      self, policy_factory: Callable[[pythia.PolicySupporter], pythia.Policy]
+  ) -> List[vz.Trial]:
     """Run the policy generated by policy_factory."""
     runner = pythia.InRamPolicySupporter(self.problem)
     policy = policy_factory(runner)
     return self._run(benchmarks.PolicySuggester(policy, runner))
 
-  def run_designer(self, designer: vza.Designer):
+  def run_designer(self, designer: vza.Designer) -> List[vz.Trial]:
     """Run the specified $designer."""
     supporter = pythia.InRamPolicySupporter(self.problem)
     policy = InRamDesignerPolicy(
         problem_statement=self.problem,
         supporter=supporter,
         designer_factory=lambda _, **kwargs: designer,
     )
@@ -128,16 +136,18 @@
     problem: vz.ProblemStatement,
    
     iters: int = 5,
     *,
     batch_size: Optional[int] = 1,
     seed: Any = None,
     verbose: int = 0,
-    validate_parameters: bool = False) -> Sequence[vz.Trial]:
+    validate_parameters: bool = False,
+) -> Sequence[vz.Trial]:
   """DEPRECATED. Use RandomMetricsRunner.run_designer()."""
   return RandomMetricsRunner(
       problem,
       iters,
       batch_size=batch_size,
       seed=seed,
       verbose=verbose,
-      validate_parameters=validate_parameters).run_designer(designer)
+      validate_parameters=validate_parameters,
+  ).run_designer(designer)
```

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/analyzers/convergence_curve.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/convergence_curve.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,23 +12,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Converters and comparators for convergence curves."""
 
-import dataclasses
 import enum
 from typing import Callable, List, Optional, Sequence, Union
 
+import attr
 import numpy as np
 from vizier import pyvizier
+from vizier.pyvizier import converters
+from vizier.pyvizier import multimetric
+from vizier.pyvizier.multimetric import xla_pareto
 
 
-@dataclasses.dataclass
+@attr.s(auto_attribs=True)
 class ConvergenceCurve:
   """Represents a batch of convergence curves on the same task."""
   xs: np.ndarray  # [T] array. All curves share the x axis.
   ys: np.ndarray  # [N x T] array where N is the batch size.
   ylabel: str = ''  # Optional for plotting.
   xlabel: str = ''  # Optional for plotting.
   # Indicates ys should be increasing in t or decreasing.
@@ -38,14 +41,29 @@
     """Trend of ys across t."""
     UNKNOWN = 'unknown'
     INCREASING = 'increasing'
     DECREASING = 'decreasing'
 
   trend: YTrend = YTrend.UNKNOWN
 
+  def __attrs_post_init__(self):
+    if len(self.ys.shape) != 2:
+      raise ValueError(f'Shapes for ys should be batch size by time {self.ys}')
+    if len(self.xs) != self.ys.shape[1]:
+      raise ValueError(
+          f'Shape mismatch for time dim: {len(self.xs)} vs {self.ys.shape}'
+      )
+    if self.trend == ConvergenceCurve.YTrend.INCREASING:
+      if not np.all(np.nan_to_num(np.diff(self.ys, axis=-1)) >= 0):
+        raise ValueError(f'Increasing trend not found: {self.ys}')
+
+    if self.trend == ConvergenceCurve.YTrend.DECREASING:
+      if not np.all(np.nan_to_num(np.diff(self.ys, axis=-1)) <= 0):
+        raise ValueError(f'Decreasing trend not found: {self.ys}')
+
   @property
   def batch_size(self) -> int:
     return self.ys.shape[0]
 
   @classmethod
   def align_xs(cls,
                curves: Sequence['ConvergenceCurve'],
@@ -145,32 +163,33 @@
         ylabel=curve.ylabel,
         trend=curve.trend)
 
 
 class ConvergenceCurveConverter:
   """Converter for Trial sequence to ConvergenceCurve."""
 
-  def __init__(self,
-               metric_information: pyvizier.MetricInformation,
-               *,
-               flip_signs: bool = False,
-               cost_fn: Callable[[pyvizier.Trial], Union[float,
-                                                         int]] = lambda _: 1,
-               measurements_type: str = 'final'):
+  def __init__(
+      self,
+      metric_information: pyvizier.MetricInformation,
+      *,
+      flip_signs_for_min: bool = False,
+      cost_fn: Callable[[pyvizier.Trial], Union[float, int]] = lambda _: 1,
+      measurements_type: str = 'final',
+  ):
     """Init.
 
     Args:
       metric_information: Information of relevant metric.
-      flip_signs: If True, flips the signs of metric values to always
-      maximize. Useful when desiring all increasing curves.
+      flip_signs_for_min: If True, flips the signs of metric values to always
+        maximize. Useful when desiring all increasing curves.
       cost_fn: Cost of each Trial (to determine xs in ConvergenceCurve).
       measurements_type: ['final', 'intermediate', 'all']
     """
     self.metric_information = metric_information
-    self.flip_signs = flip_signs
+    self.flip_signs_for_min = flip_signs_for_min
     self.cost_fn = cost_fn
     self.measurements_type = measurements_type
 
   def convert(self, trials: Sequence[pyvizier.Trial]) -> ConvergenceCurve:
     """Returns ConvergenceCurve of batch size 1."""
     yvals = [np.nan]
     xvals = [0]
@@ -189,33 +208,98 @@
                 measurement.metrics[self.metric_information.name].value)
 
       yvalue = comparator(candidates)
       xvals.append(xvals[-1] + self.cost_fn(trial))
       yvals.append(comparator([yvalue, yvals[-1]]))
 
     yvals = np.asarray(yvals[1:])
-    trend = ConvergenceCurve.YTrend.DECREASING
-    if (self.metric_information.goal == pyvizier.ObjectiveMetricGoal.MAXIMIZE
-       ) or (self.metric_information.goal
-             == pyvizier.ObjectiveMetricGoal.MINIMIZE and self.flip_signs):
+    if self.metric_information.goal == pyvizier.ObjectiveMetricGoal.MAXIMIZE:
       trend = ConvergenceCurve.YTrend.INCREASING
+      flipped = False
+    elif self.flip_signs_for_min:
+      trend = ConvergenceCurve.YTrend.INCREASING
+      flipped = True
+    else:
+      trend = ConvergenceCurve.YTrend.DECREASING
+      flipped = False
     return ConvergenceCurve(
         xs=np.asarray(xvals[1:]),
-        ys=np.asarray(yvals).reshape([1, -1]) * (-1 if self.flip_signs else 1),
+        ys=np.asarray(yvals).reshape([1, -1]) * (-1 if flipped else 1),
         trend=trend,
-        ylabel=self.metric_information.name)
+        ylabel=self.metric_information.name,
+    )
 
   @property
   def comparator(self):
     """Comparator used for creating the convergence curve."""
     return np.nanmax if (
         self.metric_information.goal
         == pyvizier.ObjectiveMetricGoal.MAXIMIZE) else np.nanmin
 
 
+class HypervolumeCurveConverter:
+  """Converts Trials to cumulative hypervolume curve for multiobjective."""
+
+  def __init__(
+      self,
+      metric_informations: Sequence[pyvizier.MetricInformation],
+      *,
+      reference_value: float = 0.0,
+      num_vectors: int = 10000,
+  ):
+    """Init.
+
+    Args:
+      metric_informations:
+      reference_value: Reference point value from which hypervolume is computed.
+        Default uses the origin and the value is broadcasted for all dimensions.
+      num_vectors: Number of vectors from which hypervolume is computed.
+    """
+    if len(metric_informations) < 2:
+      raise ValueError(
+          'Should not use hypervolume curve with less than'
+          f'two metrics {metric_informations}'
+      )
+    self._metric_informations = metric_informations
+    self._num_vectors = num_vectors
+
+    def create_metric_converter(mc):
+      return converters.DefaultModelOutputConverter(
+          mc,
+          flip_sign_for_minimization_metrics=True,
+          raise_errors_for_missing_metrics=False,
+      )
+
+    self._converter = converters.DefaultTrialConverter(
+        parameter_converters=[],
+        metric_converters=[
+            create_metric_converter(mc) for mc in metric_informations
+        ],
+    )
+    self._origin_value = reference_value
+
+  def convert(self, trials: Sequence[pyvizier.Trial]) -> ConvergenceCurve:
+    """Returns ConvergenceCurve with a curve of shape 1 x len(trials)."""
+    # Returns a len(trials) x number of metrics np.ndarray.
+    metrics = self._converter.to_labels_array(trials)
+    front = multimetric.ParetoFrontier(
+        points=metrics,
+        origin=np.array([self._origin_value] * metrics.shape[1]),
+        num_vectors=self._num_vectors,
+        cum_hypervolume_base=xla_pareto.jax_cum_hypervolume_origin,
+    )
+    hv_curve = front.hypervolume(is_cumulative=True)
+    return ConvergenceCurve(
+        xs=np.asarray(range(1, len(hv_curve) + 1)),
+        ys=np.asarray(hv_curve).reshape([1, -1]),
+        trend=ConvergenceCurve.YTrend.INCREASING,
+        ylabel='hypervolume',
+    )
+
+
 class ConvergenceCurveComparator:
   """Comparator methods for ConvergenceCurves.
 
   Methods in this class generally return comparison metrics for a compared curve
   against a baseline curve. Only works for curves with INCREASING or DECREASING
   trend.
```

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/analyzers/convergence_curve_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/convergence_curve_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,16 +91,17 @@
     np.testing.assert_array_equal(
         extra_c1.ys,
         np.array([[2, 1.5, 1.0, 0.5, 0.0, -0.5], [1, 1, 1, 1, 1, 1]]))
 
   def test_align_xs_on_increasing_and_dicreasing_fails(self):
     c1 = convergence.ConvergenceCurve(
         xs=np.array([1, 3, 4]),
-        ys=np.array([[2, 1, 1]]),
-        trend=convergence.ConvergenceCurve.YTrend.INCREASING)
+        ys=np.array([[2, 3, 3]]),
+        trend=convergence.ConvergenceCurve.YTrend.INCREASING,
+    )
     c2 = convergence.ConvergenceCurve(
         xs=np.array([2]),
         ys=np.array([[3]]),
         trend=convergence.ConvergenceCurve.YTrend.DECREASING)
     with self.assertRaisesRegex(ValueError, 'increasing'):
       convergence.ConvergenceCurve.align_xs([c1, c2])
 
@@ -114,14 +115,60 @@
     trials = _gen_trials([2, 1, 3])
     generator = convergence.ConvergenceCurveConverter(
         pyvizier.MetricInformation(name='', goal=goal))
     curve = generator.convert(trials)
     np.testing.assert_array_equal(curve.xs, [1, 2, 3])
     np.testing.assert_array_equal(curve.ys, expected)
 
+  @parameterized.named_parameters(
+      ('maximize', pyvizier.ObjectiveMetricGoal.MAXIMIZE, [[2, 2, 3]]),
+      ('minimize', pyvizier.ObjectiveMetricGoal.MINIMIZE, [[-2, -1, -1]]),
+  )
+  def test_convert_flip_signs(self, goal, expected):
+    trials = _gen_trials([2, 1, 3])
+    generator = convergence.ConvergenceCurveConverter(
+        pyvizier.MetricInformation(name='', goal=goal), flip_signs_for_min=True
+    )
+    curve = generator.convert(trials)
+    np.testing.assert_array_equal(curve.xs, [1, 2, 3])
+    np.testing.assert_array_equal(curve.ys, expected)
+
+
+class HyperConvergenceCurveConverterTest(parameterized.TestCase):
+
+  def test_convert_basic(self):
+    generator = convergence.HypervolumeCurveConverter([
+        pyvizier.MetricInformation(
+            name='max', goal=pyvizier.ObjectiveMetricGoal.MAXIMIZE
+        ),
+        pyvizier.MetricInformation(
+            name='min', goal=pyvizier.ObjectiveMetricGoal.MINIMIZE
+        ),
+    ])
+    pytrials = []
+    pytrials.append(
+        pyvizier.Trial().complete(
+            pyvizier.Measurement(metrics={'max': 4.0, 'min': 2.0})
+        )
+    )
+    pytrials.append(
+        pyvizier.Trial().complete(
+            pyvizier.Measurement(metrics={'max': 3.0, 'min': -1.0})
+        )
+    )
+    pytrials.append(
+        pyvizier.Trial().complete(
+            pyvizier.Measurement(metrics={'max': 4.0, 'min': -2.0})
+        )
+    )
+
+    curve = generator.convert(pytrials)
+    np.testing.assert_array_equal(curve.xs, [1, 2, 3])
+    np.testing.assert_array_almost_equal(curve.ys, [[0.0, 3.0, 8.0]], decimal=1)
+
 
 class ConvergenceComparatorTest(absltest.TestCase):
 
   def setUp(self):
     super(ConvergenceComparatorTest, self).setUp()
     xs = np.array(range(0, 20))
     xs_t = xs.reshape(1, len(xs))
```

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/analyzers/simple_regret_score.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/simple_regret_score.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/analyzers/simple_regret_score_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/atari100k_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/atari100k_experimenter_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,25 +37,28 @@
         'Runner.max_steps_per_episode': 2,
         'JaxDQNAgent.min_replay_history': 2,
         'OutOfGraphPrioritizedReplayBuffer.replay_capacity': 1000,
     }
     experimenter = atari100k_experimenter.Atari100kExperimenter(
         game_name='Pong',
         agent_name=agent_name,
-        initial_gin_bindings=initial_gin_bindings)
+        initial_gin_bindings=initial_gin_bindings,
+    )
 
     designer = random.RandomDesigner(
-        experimenter.problem_statement().search_space, seed=None)
+        experimenter.problem_statement().search_space, seed=None
+    )
 
     suggestions = designer.suggest(2)
     trials = [suggestion.to_trial() for suggestion in suggestions]
     experimenter.evaluate(trials)
-    for evaluated_trial in trials:
-      self.assertEqual(evaluated_trial.status, pyvizier.TrialStatus.COMPLETED)
-      logging.info('Evaluated Trial: %s', evaluated_trial)
-      self.assertGreaterEqual(
-          evaluated_trial.final_measurement.metrics['eval_average_return']
-          .value, 0.0)
+    # Trials should be completed in place.
+    for trial in trials:
+      self.assertEqual(trial.status, pyvizier.TrialStatus.COMPLETED)
+      logging.info('Evaluated Trial: %s', trial)
+      if trial.final_measurement:
+        value = trial.final_measurement.metrics['eval_average_return'].value
+        self.assertGreaterEqual(value, 0.0)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/combo/common.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo/common.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/combo_experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/combo_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/discretizing_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/discretizing_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/experimenter_factory.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/experimenter_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,51 +12,78 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Experimenter factories."""
 
-from typing import Optional, Protocol
+import abc
+import json
+from typing import Optional
 
 import attr
 import numpy as np
+from vizier import pyvizier as vz
 from vizier._src.benchmarks.experimenters import discretizing_experimenter
 from vizier._src.benchmarks.experimenters import experimenter
 from vizier._src.benchmarks.experimenters import noisy_experimenter
 from vizier._src.benchmarks.experimenters import normalizing_experimenter
 from vizier._src.benchmarks.experimenters import numpy_experimenter
 from vizier._src.benchmarks.experimenters import shifting_experimenter
 from vizier._src.benchmarks.experimenters.synthetic import bbob
+from vizier.interfaces import serializable
+from vizier.utils import json_utils
 
+BBOB_FACTORY_KEY = 'bbob_factory'
+SINGLE_OBJECTIVE_FACTORY_KEY = 'single_objective_factory'
 
-class ExperimenterFactory(Protocol):
+
+class ExperimenterFactory(serializable.Serializable):
   """Abstraction for creating Experimenters."""
 
-  def __call__(self) -> experimenter.Experimenter:
+  @abc.abstractmethod
+  def __call__(
+      self, *, seed: Optional[int] = None
+  ) -> experimenter.Experimenter:
     """Creates the Experimenter."""
+    pass
 
 
 @attr.define
 class BBOBExperimenterFactory(ExperimenterFactory):
   """Factory for a BBOB function."""
 
   # Should be a BBOB function name in bbob.py (name should match exactly).
-  name: str = attr.field(validator=attr.validators.instance_of(str))
+  name: str = attr.field(default='', validator=attr.validators.instance_of(str))
   dim: int = attr.field(
-      validator=[attr.validators.instance_of(int),
-                 attr.validators.gt(0)])
-
-  def __call__(self) -> numpy_experimenter.NumpyExperimenter:
+      default=1,
+      validator=[attr.validators.instance_of(int), attr.validators.gt(0)],
+  )
+
+  def __call__(
+      self, seed: Optional[int] = None
+  ) -> numpy_experimenter.NumpyExperimenter:
+    del seed
     bbob_function = getattr(bbob, self.name, None)
     if bbob_function is None:
       raise ValueError(f'{self.name} is not a valid BBOB function in bbob.py')
     return numpy_experimenter.NumpyExperimenter(
         bbob_function, bbob.DefaultBBOBProblemStatement(self.dim))
 
+  def dump(self) -> vz.Metadata:
+    metadata = vz.Metadata()
+    metadata_dict = {'name': self.name, 'dim': self.dim}
+    metadata[BBOB_FACTORY_KEY] = json.dumps(metadata_dict)
+    return metadata
+
+  @classmethod
+  def recover(cls, metadata: vz.Metadata) -> 'BBOBExperimenterFactory':
+    metadata_dict = json.loads(metadata[BBOB_FACTORY_KEY])
+    return cls(**metadata_dict)
+
 
 @attr.define
 class SingleObjectiveExperimenterFactory(ExperimenterFactory):
   """Factory for a single objective Experimenter."""
 
   base_factory: ExperimenterFactory = attr.field()
   # An array of doubles that is broadcastable to dim of search space.
@@ -73,15 +100,15 @@
   # only continuous parameters.
   discrete_dict: dict[int, int] = attr.field(default=attr.Factory(dict))
   # Dictionary of parameter indices to categorize in a grid.
   # Key = index of parameter to be categorize and Value = Number of feasible
   # points to categorize to. See discrete_dict.
   categorical_dict: dict[int, int] = attr.field(default=attr.Factory(dict))
 
-  def __call__(self) -> experimenter.Experimenter:
+  def __call__(self, seed: Optional[int] = None) -> experimenter.Experimenter:
     """Creates the SingleObjective Experimenter."""
     exptr = self.base_factory()
     if self.shift is not None:
       exptr = shifting_experimenter.ShiftingExperimenter(
           exptr, shift=self.shift)
     if self.num_normalization_samples:
       exptr = normalizing_experimenter.NormalizingExperimenter(
@@ -112,11 +139,57 @@
       }
       exptr = (
           discretizing_experimenter.DiscretizingExperimenter.create_with_grid(
               exptr, categorization, convert_to_str=True
           )
       )
     if self.noise_type is not None:
-      exptr = noisy_experimenter.NoisyExperimenter(
-          exptr, noise_type=self.noise_type.upper())
+      exptr = noisy_experimenter.NoisyExperimenter.from_type(
+          exptr, noise_type=self.noise_type.upper(), seed=seed
+      )
 
     return exptr
+
+  def dump(self) -> vz.Metadata:
+    # The resulting metadata stores base factory metadata
+    # and metadata_dict with different keys.
+    metadata = self.base_factory.dump()
+    metadata_dict = {
+        'shift': self.shift,
+        'noise_type': self.noise_type,
+        'num_normalization_samples': self.num_normalization_samples,
+        'discrete_dict': self.discrete_dict,
+        'categorical_dict': self.categorical_dict,
+    }
+    metadata[SINGLE_OBJECTIVE_FACTORY_KEY] = json.dumps(
+        metadata_dict, cls=json_utils.NumpyEncoder
+    )
+    return metadata
+
+  @classmethod
+  def recover(
+      cls, metadata: vz.Metadata
+  ) -> 'SingleObjectiveExperimenterFactory':
+    if BBOB_FACTORY_KEY in metadata:
+      base_factory = BBOBExperimenterFactory.recover(metadata)
+    else:
+      raise serializable.DecodeError(
+          f'No valid base factory found in {metadata}'
+      )
+
+    metadata_dict = json.loads(
+        metadata[SINGLE_OBJECTIVE_FACTORY_KEY], cls=json_utils.NumpyDecoder
+    )
+
+    # Turn string keys back to int for discrete/categorical dicts.
+    int_discrete_dict = {
+        int(k): v for k, v in metadata_dict['discrete_dict'].items()
+    }
+    metadata_dict['discrete_dict'] = int_discrete_dict
+    int_categorical_dict = {
+        int(k): v for k, v in metadata_dict['categorical_dict'].items()
+    }
+    metadata_dict['categorical_dict'] = int_categorical_dict
+
+    return SingleObjectiveExperimenterFactory(
+        base_factory=base_factory, **metadata_dict
+    )
```

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/experimenter_factory_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -132,10 +132,40 @@
           shift=np.asarray(1.9),
           noise_type='moderate_gaussian',
           num_normalization_samples=10,
           discrete_dict={0: 3, 1: 5},
           categorical_dict={1: 4},
       )()
 
+  def testSingleObjectiveSerialization(self):
+    dim = 5
+    bbob_factory = experimenter_factory.BBOBExperimenterFactory(
+        name='Sphere', dim=dim
+    )
+    bbob_metadata = bbob_factory.dump()
+    recovered_bbob = experimenter_factory.BBOBExperimenterFactory.recover(
+        bbob_metadata
+    )
+    self.assertEqual(recovered_bbob.dim, dim)
+    self.assertEqual(recovered_bbob.name, 'Sphere')
+
+    exptr_factory = experimenter_factory.SingleObjectiveExperimenterFactory(
+        base_factory=bbob_factory,
+        shift=np.asarray(1.9),
+        noise_type='moderate_gaussian',
+        num_normalization_samples=10,
+        discrete_dict={0: 3, 1: 5},
+    )
+    factory_metadata = exptr_factory.dump()
+    recovered_factory = (
+        experimenter_factory.SingleObjectiveExperimenterFactory.recover(
+            factory_metadata
+        )
+    )
+    self.assertEqual(recovered_factory.noise_type, 'moderate_gaussian')
+    self.assertEqual(recovered_factory.num_normalization_samples, 10)
+    np.testing.assert_array_equal(recovered_factory.shift, np.asarray(1.9))
+    self.assertDictEqual(recovered_factory.discrete_dict, {0: 3, 1: 5})
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/hpob/handler.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob/handler.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/hpob_experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/hpob_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/l1_categorical_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench101_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench101_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench201_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/nasbench201_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/noisy_experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/noisy_experimenter.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Applies the noise function to each metric in final measurement."""
 
 import functools
-import logging
 from typing import Callable, Optional, Sequence
 
 import attr
 import numpy as np
 from vizier import pyvizier
 from vizier._src.benchmarks.experimenters import experimenter
 
@@ -31,23 +30,31 @@
   """NoisyExperimenter applies noise to all metric(s) in final measurement.
 
   It stores the unnoised metric as metric_name + '_before_noise'. The noise
   function is a callable that is applied to metrics.
   """
 
   exptr: experimenter.Experimenter = attr.field()
-  noise_fn: Optional[Callable[[float], float]] = attr.field(default=None)
-  noise_type: Optional[str] = attr.field(default=None)
+  noise_fn: Callable[[float], float] = attr.field()
 
-  def __attrs_post_init__(self):
-    """Updates noise_fn with noise given by noise_type."""
-    if self.noise_type is not None:
-      dim = len(self.exptr.problem_statement().search_space.parameters)
-      self.noise_fn = _create_noise_fn(self.noise_type, dimension=dim)
-      logging.info('Initializing %s', str(self))
+  @classmethod
+  def from_type(
+      cls,
+      exptr: experimenter.Experimenter,
+      noise_type: str,
+      seed: Optional[int] = None,
+  ) -> 'NoisyExperimenter':
+    """Initializes noise_fn with noise given by noise_type."""
+    dim = len(exptr.problem_statement().search_space.parameters)
+    noise_fn = _create_noise_fn(
+        noise_type,
+        dimension=dim,
+        seed=seed,
+    )
+    return cls(exptr, noise_fn)
 
   def problem_statement(self) -> pyvizier.ProblemStatement:
     return self.exptr.problem_statement()
 
   def evaluate(self, suggestions: Sequence[pyvizier.Trial]):
     self.exptr.evaluate(suggestions)
     for suggestion in suggestions:
@@ -57,21 +64,23 @@
       for name, metric in suggestion.final_measurement.metrics.items():
         metric_dict_with_noise[name] = pyvizier.Metric(
             value=self.noise_fn(metric.value))
         metric_dict_with_noise[name + '_before_noise'] = metric
       suggestion.final_measurement.metrics = metric_dict_with_noise
 
   def __repr__(self):
-    return f'NoisyExperimenter({self.noise_type}) on {str(self.exptr)}'
+    return f'NoisyExperimenter({self.noise_fn}) on {str(self.exptr)}'
 
 
-def _create_noise_fn(noise: str,
-                     dimension: int,
-                     target_value: float = 1e-8,
-                     seed: int = 0) -> Callable[[float], float]:
+def _create_noise_fn(
+    noise: str,
+    dimension: int,
+    target_value: float = 1e-8,
+    seed: Optional[int] = None,
+) -> Callable[[float], float]:
   """Creates a noise function via NumPy.
 
   See https://bee22.com/resources/bbob%20noisy%20functions.pdf
 
   Args:
     noise: Noise specification
     dimension: Dimensionality of bbob function that the noise is applied to.
@@ -80,96 +89,112 @@
 
   Returns:
     Callable that returns the noisy version of the input.
 
   Raises:
     ValueError: if noise is not supported.
   """
-  np.random.seed(seed)
+  rng = np.random.default_rng(seed or 0)
   if noise == 'MODERATE_GAUSSIAN':
-    noise_fn = lambda v: v * np.random.lognormal(0, 0.01)
+    noise_fn = lambda v: v * rng.lognormal(0, 0.01)
   elif noise == 'SEVERE_GAUSSIAN':
-    noise_fn = lambda v: v * np.random.lognormal(0, 0.1)
+    noise_fn = lambda v: v * rng.lognormal(0, 0.1)
   elif noise == 'MODERATE_UNIFORM':
     noise_fn = functools.partial(
         _uniform_noise,
+        rng=rng,
         amplifying_exponent=0.01 * (0.49 + 1.0 / dimension),
-        shrinking_exponent=0.01)
+        shrinking_exponent=0.01,
+    )
   elif noise == 'SEVERE_UNIFORM':
     noise_fn = functools.partial(
         _uniform_noise,
+        rng=rng,
         amplifying_exponent=0.1 * (0.49 + 1.0 / dimension),
-        shrinking_exponent=0.1)
+        shrinking_exponent=0.1,
+    )
   elif noise == 'MODERATE_SELDOM_CAUCHY':
     noise_fn = functools.partial(
-        _cauchy_noise, noise_strength=0.01, noise_frequency=0.05)
+        _cauchy_noise, rng=rng, noise_strength=0.01, noise_frequency=0.05
+    )
   elif noise == 'SEVERE_SELDOM_CAUCHY':
     noise_fn = functools.partial(
-        _cauchy_noise, noise_strength=0.1, noise_frequency=0.25)
+        _cauchy_noise, rng=rng, noise_strength=0.1, noise_frequency=0.25
+    )
   elif noise == 'LIGHT_ADDITIVE_GAUSSIAN':
-    return functools.partial(_additive_normal_noise, stddev=0.01)
+    return functools.partial(_additive_normal_noise, rng=rng, stddev=0.01)
   elif noise == 'MODERATE_ADDITIVE_GAUSSIAN':
-    return functools.partial(_additive_normal_noise, stddev=0.1)
+    return functools.partial(_additive_normal_noise, rng=rng, stddev=0.1)
   elif noise == 'SEVERE_ADDITIVE_GAUSSIAN':
-    return functools.partial(_additive_normal_noise, stddev=1.0)
+    return functools.partial(_additive_normal_noise, rng=rng, stddev=1.0)
   else:
     raise ValueError('Noise was not supported: {}'.format(noise))
   return lambda v: _stabilized_noise(v, noise_fn, target_value)
 
 
-def _uniform_noise(value: float,
-                   amplifying_exponent: float,
-                   shrinking_exponent: float,
-                   epsilon: float = 1e-99) -> float:
+def _uniform_noise(
+    value: float,
+    amplifying_exponent: float,
+    shrinking_exponent: float,
+    rng: np.random.Generator,
+    epsilon: float = 1e-99,
+) -> float:
   """Uniform noise model for bbob-noisy benchmark.
 
   The noise strength increases when value is small.
 
   Args:
     value: Function value to apply noise to.
     amplifying_exponent: "alpha" in the paper. The higher this number is, the
       more likely it is for the noisy value to be greater than the input value.
       0 or less means the noise never amplifies the function value.
     shrinking_exponent: "beta" in the paper. The higher this number is, the more
       likely it is for the noisy value to be less than the input value. 0 or
       less means the noise never shrinks the function value.
+    rng: Rng.
     epsilon: "epsilon" in the paper. Prevents division by zero.
 
   Returns:
     Noisy version of value.
   """
-  f1 = np.power(np.random.uniform(), np.max([0.0, shrinking_exponent]))
-  f2 = np.power(1e9 / (value + epsilon),
-                amplifying_exponent * np.random.uniform())
+  f1 = np.power(rng.uniform(), np.max([0.0, shrinking_exponent]))
+  f2 = np.power(1e9 / (value + epsilon), amplifying_exponent * rng.uniform())
   return value * f1 * np.max([1.0, f2])
 
 
-def _additive_normal_noise(value: float, stddev: float) -> float:
+def _additive_normal_noise(
+    value: float, stddev: float, rng: np.random.Generator
+) -> float:
   """Additive normal noise."""
-  return value + np.random.normal(0.0, stddev)
+  return value + rng.normal(0.0, stddev)
 
 
-def _cauchy_noise(value: float, noise_strength: float,
-                  noise_frequency: float) -> float:
+def _cauchy_noise(
+    value: float,
+    noise_strength: float,
+    noise_frequency: float,
+    rng: np.random.Generator,
+) -> float:
   """Cauchy noise model for bbob-noisy benchmark.
 
   The noise is infrequent and difficult to analyze due to large outliers.
 
   Args:
     value: Function value to apply noise to.
     noise_strength: "alpha" in the paper. Its absolute value determines the
       noise strength. The recommended setup as in the paper is to use a positive
       number.
     noise_frequency: "p" in the paper. Determines the probability of the noisy
       evaluation. Clipped (not explicitly but effectively) to [0, 1] range.
+    rng:
 
   Returns:
     Noisy version of value.
   """
-  noise = (np.random.uniform() < noise_frequency) * np.random.standard_cauchy()
+  noise = (rng.uniform() < noise_frequency) * rng.standard_cauchy()
   return value + noise_strength * np.max([0.0, 1000.0 + noise])
 
 
 def _stabilized_noise(value: float,
                       noisy_fn: Callable[[float], float],
                       target_value: float = 1e-8) -> float:
   """Post processing of noise for bbob-noisy benchmark.
```

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/normalizing_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/normalizing_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/numpy_experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/numpy_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/numpy_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/shifting_experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/shifting_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/shifting_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sign_flip_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sign_flip_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/sparse_experimenter.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sparse_experimenter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/sparse_experimenter_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/experimenters/synthetic/bbob.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/experimenters/synthetic/bbob.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/runners/benchmark_runner.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -116,14 +116,43 @@
               'because designer returned nothing.'
           ),
           self.batch_size,
       )
 
 
 @attr.define
+class FillActiveTrials(BenchmarkSubroutine):
+  """Generate a number of Suggestions up to a limit of Active Trials."""
+
+  # Upper limit of active Trials to be filled with new Suggestions.
+  num_active_trials_limit: int = attr.field(
+      default=1, validator=attr.validators.instance_of(int)
+  )
+
+  def run(self, state: benchmark_state.BenchmarkState) -> None:
+    active_trials = state.algorithm.supporter.GetTrials(
+        status_matches=vz.TrialStatus.ACTIVE
+    )
+    if (
+        num_suggestions := self.num_active_trials_limit - len(active_trials)
+    ) > 0:
+      suggestions = state.algorithm.suggest(num_suggestions)
+      if not suggestions:
+        logging.info(
+            (
+                'Suggestions did not generate %d suggestions'
+                'to fill active Trials to %d '
+                'because designer returned nothing.'
+            ),
+            num_suggestions,
+            self.num_active_trials_limit,
+        )
+
+
+@attr.define
 class EvaluateActiveTrials(BenchmarkSubroutine):
   """Evaluate a fixed number of Active Trials as Completed Trials."""
 
   # If None, this Evaluates all Active Trials.
   num_evaluations: Optional[int] = attr.field(default=None)
 
   def run(self, state: benchmark_state.BenchmarkState) -> None:
```

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/runners/benchmark_runner_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_runner_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from vizier._src.benchmarks.runners import benchmark_runner
 from vizier._src.benchmarks.runners import benchmark_state
 
 from absl.testing import absltest
 from absl.testing import parameterized
 
 
-def _get_benchmark_state_factory():
+def _get_designer_benchmark_state_factory():
   dim = 10
   experimenter = experimenter_factory.BBOBExperimenterFactory('Sphere', dim)()
 
   def _designer_factory(config: vz.ProblemStatement, seed: int):
     return random.RandomDesigner(config.search_space, seed=seed)
 
   benchmark_state_factory = benchmark_state.DesignerBenchmarkStateFactory(
@@ -40,49 +40,57 @@
   return benchmark_state_factory
 
 
 class BaseRunnerTest(parameterized.TestCase):
 
   @parameterized.parameters(
       {
-          'runner':
-              benchmark_runner.BenchmarkRunner(
-                  benchmark_subroutines=[
-                      benchmark_runner.GenerateSuggestions(),
-                      benchmark_runner.EvaluateActiveTrials()
-                  ],
-                  num_repeats=7),
-          'expected_trials':
-              7
-      }, {
-          'runner':
-              benchmark_runner.BenchmarkRunner(
-                  benchmark_subroutines=[
-                      benchmark_runner.GenerateAndEvaluate(10)
-                  ],
-                  num_repeats=5),
-          'expected_trials':
-              50
-      })
+          'runner': benchmark_runner.BenchmarkRunner(
+              benchmark_subroutines=[
+                  benchmark_runner.GenerateSuggestions(),
+                  benchmark_runner.EvaluateActiveTrials(),
+              ],
+              num_repeats=7,
+          ),
+          'expected_trials': 7,
+      },
+      {
+          'runner': benchmark_runner.BenchmarkRunner(
+              benchmark_subroutines=[benchmark_runner.GenerateAndEvaluate(10)],
+              num_repeats=5,
+          ),
+          'expected_trials': 50,
+      },
+      {
+          'runner': benchmark_runner.BenchmarkRunner(
+              benchmark_subroutines=[
+                  benchmark_runner.FillActiveTrials(10),
+                  benchmark_runner.EvaluateActiveTrials(),
+              ],
+              num_repeats=5,
+          ),
+          'expected_trials': 50,
+      },
+  )
   def test_benchmark_run(self, runner, expected_trials):
-    benchmark_state_factory = _get_benchmark_state_factory()
+    benchmark_state_factory = _get_designer_benchmark_state_factory()
     bench_state = benchmark_state_factory(seed=5)
     runner.run(bench_state)
     self.assertEmpty(
         bench_state.algorithm.supporter.GetTrials(
             status_matches=vz.TrialStatus.ACTIVE
         )
     )
     all_trials = bench_state.algorithm.supporter.GetTrials()
     self.assertLen(all_trials, expected_trials)
     for trial in all_trials:
       self.assertEqual(trial.status, vz.TrialStatus.COMPLETED)
 
   def test_active_trials(self):
-    benchmark_state_factory = _get_benchmark_state_factory()
+    benchmark_state_factory = _get_designer_benchmark_state_factory()
     bench_state = benchmark_state_factory(seed=5)
     runner = benchmark_runner.BenchmarkRunner(
         benchmark_subroutines=[
             benchmark_runner.GenerateSuggestions(10),
             benchmark_runner.EvaluateActiveTrials(6),
         ],
         num_repeats=3,
@@ -97,10 +105,67 @@
     self.assertLen(
         bench_state.algorithm.supporter.GetTrials(
             status_matches=vz.TrialStatus.COMPLETED
         ),
         6 * 3,
     )
 
+  def test_fill_active_trials(self):
+    benchmark_state_factory = _get_designer_benchmark_state_factory()
+    bench_state = benchmark_state_factory(seed=5)
+    runner = benchmark_runner.BenchmarkRunner(
+        benchmark_subroutines=[
+            benchmark_runner.FillActiveTrials(10),
+            benchmark_runner.EvaluateActiveTrials(6),  # 6 Completions
+            benchmark_runner.FillActiveTrials(3),  # No-op
+            benchmark_runner.EvaluateActiveTrials(6),  # 4 Completions
+            benchmark_runner.FillActiveTrials(10),
+            benchmark_runner.EvaluateActiveTrials(6),  # 6 completions
+        ]
+    )
+    runner.run(bench_state)
+    self.assertLen(
+        bench_state.algorithm.supporter.GetTrials(
+            status_matches=vz.TrialStatus.ACTIVE
+        ),
+        4,
+    )
+    self.assertLen(
+        bench_state.algorithm.supporter.GetTrials(
+            status_matches=vz.TrialStatus.COMPLETED
+        ),
+        16,
+    )
+
+  def test_benchmark_run_from_exptr_factory(self):
+    dim = 10
+    exptr_factory = experimenter_factory.BBOBExperimenterFactory('Sphere', dim)
+
+    def _designer_factory(config: vz.ProblemStatement, seed: int):
+      return random.RandomDesigner(config.search_space, seed=seed)
+
+    benchmark_state_factory = (
+        benchmark_state.ExperimenterDesignerBenchmarkStateFactory(
+            designer_factory=_designer_factory,
+            experimenter_factory=exptr_factory,
+        )
+    )
+    benchmark_state_factory = _get_designer_benchmark_state_factory()
+    bench_state = benchmark_state_factory(seed=5)
+    runner = benchmark_runner.BenchmarkRunner(
+        benchmark_subroutines=[benchmark_runner.GenerateAndEvaluate(10)],
+        num_repeats=5,
+    )
+    runner.run(bench_state)
+    self.assertEmpty(
+        bench_state.algorithm.supporter.GetTrials(
+            status_matches=vz.TrialStatus.ACTIVE
+        )
+    )
+    all_trials = bench_state.algorithm.supporter.GetTrials()
+    self.assertLen(all_trials, 50)
+    for trial in all_trials:
+      self.assertEqual(trial.status, vz.TrialStatus.COMPLETED)
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/runners/benchmark_state.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_state.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 import attr
 from vizier import algorithms as vza
 from vizier import pythia
 from vizier import pyvizier as vz
 from vizier._src.algorithms.policies.designer_policy import InRamDesignerPolicy
 from vizier._src.benchmarks.experimenters.experimenter import Experimenter
+from vizier._src.benchmarks.experimenters.experimenter_factory import ExperimenterFactory
 
 
 @attr.define
 class PolicySuggester:
   """Wraps a Policy and a datastore/supporter as an algorithm.
 
   NOTE: Updates to datastore should interface directly with supporter API. The
@@ -95,26 +96,41 @@
   algorithm: PolicySuggester
 
 
 @attr.define(frozen=True)
 class BenchmarkStateFactory(abc.ABC):
   """Factory class to generate new BenchmarkState."""
 
-  experimenter: Experimenter
-
   @abc.abstractmethod
   def __call__(self, seed: Optional[int] = None) -> BenchmarkState:
     """Creates a new instance of BenchmarkFactory."""
     pass
 
 
 @attr.define(frozen=True)
+class ExperimenterDesignerBenchmarkStateFactory(BenchmarkStateFactory):
+  """Generate new BenchmarkState from exptr/designer factory."""
+
+  experimenter_factory: ExperimenterFactory
+  designer_factory: vza.DesignerFactory[vza.Designer]
+
+  def __call__(self, seed: Optional[int] = None) -> BenchmarkState:
+    """Create a BenchmarkState from experimenter and designer factory."""
+    experimenter = self.experimenter_factory(seed=seed)
+    factory = DesignerBenchmarkStateFactory(
+        experimenter=experimenter, designer_factory=self.designer_factory
+    )
+    return factory(seed=seed)
+
+
+@attr.define(frozen=True)
 class DesignerBenchmarkStateFactory(BenchmarkStateFactory):
   """Factory class to generate new BenchmarkState from designer factory."""
 
+  experimenter: Experimenter
   designer_factory: vza.DesignerFactory[vza.Designer]
 
   def __call__(self, seed: Optional[int] = None) -> BenchmarkState:
     """Create a BenchmarkState from designer factory."""
     problem = self.experimenter.problem_statement()
 
     return BenchmarkState(
@@ -134,14 +150,15 @@
     ...
 
 
 @attr.define(frozen=True)
 class PolicyBenchmarkStateFactory(BenchmarkStateFactory):
   """Factory class to generate new BenchmarkState from policy factory."""
 
+  experimenter: Experimenter
   policy_factory: SeededPolicyFactory
 
   def __call__(self, seed: Optional[int] = None) -> BenchmarkState:
     """Create a BenchmarkState from policy factory."""
     problem = self.experimenter.problem_statement()
     return BenchmarkState(
         experimenter=self.experimenter,
```

### Comparing `google-vizier-0.1.4/vizier/_src/benchmarks/runners/benchmark_state_test.py` & `google-vizier-0.1.5/vizier/_src/benchmarks/runners/benchmark_state_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/jax/models/__init__.py` & `google-vizier-0.1.5/vizier/_src/jax/models/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/jax/models/gaussian_process_model.py` & `google-vizier-0.1.5/vizier/_src/jax/models/gaussian_process_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         constraint=sp_model.Constraint(bounds=(self.dtype(0.0), None)),
     )
     return tfd.GaussianProcess(
         kernel,
         index_points=inputs,
         observation_noise_variance=observation_noise_variance,
         validate_args=self._use_tfp_runtime_validation,
-        always_yield_multivariate_normal=True)
+    )
 
 
 class GaussianProcessARDWithCategorical(sp_model.ModelCoroutine):
   """Specifies an ARD Gaussian process model over continuous/categorical data.
 
   While `GaussianProcessARD` operates on a continuous domain,
   `GaussianProcessARDWithCategorical` operates on a domain that contains both
@@ -253,9 +253,8 @@
         constraint=sp_model.Constraint(bounds=(self.dtype(0.0), None)),
     )
     return tfd.GaussianProcess(
         kernel,
         index_points=inputs,
         observation_noise_variance=observation_noise_variance,
         validate_args=self._use_tfp_runtime_validation,
-        always_yield_multivariate_normal=True,
     )
```

### Comparing `google-vizier-0.1.4/vizier/_src/jax/models/gaussian_process_model_test.py` & `google-vizier-0.1.5/vizier/_src/jax/models/gaussian_process_model_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/jax/models/hebo_gp_model.py` & `google-vizier-0.1.5/vizier/_src/jax/models/hebo_gp_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,63 +18,62 @@
 
 
 Faithful reimplementation of HEBO model based off of:
 Paper: https://arxiv.org/abs/2012.03826
 Repo: https://github.com/huawei-noah/HEBO.
 """
 
-from typing import Generator
+from typing import Generator, Optional
 import attr
-import chex
 import jax
 from jax import numpy as jnp
 from jax.config import config
 from tensorflow_probability.substrates import jax as tfp
 from vizier._src.jax import stochastic_process_model as sp
+from vizier._src.jax import types
 from vizier._src.jax.optimizers import optimizers
 
 config.update('jax_enable_x64', True)
 
 tfd = tfp.distributions
 tfb = tfp.bijectors
 tfpk = tfp.math.psd_kernels
 
 
 @attr.define
-class VizierHeboGaussianProcess(sp.ModelCoroutine[chex.Array,
-                                                  tfd.GaussianProcess]):
+class VizierHeboGaussianProcess(
+    sp.ModelCoroutine[types.Array, tfd.GaussianProcess]
+):
   """Hebo Gaussian process model."""
 
   @classmethod
   def model_and_loss_fn(
       cls,
-      features: chex.Array,
-      labels: chex.Array,
+      features: types.Array,
+      labels: types.Array,
   ) -> tuple[sp.StochasticProcessModel, optimizers.LossFunction]:
     """Returns the model and loss function."""
     gp_coroutine = VizierHeboGaussianProcess()
     model = sp.StochasticProcessModel(gp_coroutine)
 
     # Define the ARD loss function.
     def loss_fn(params):
       gp, mutables = model.apply({'params': params},
                                  features,
                                  mutable=['losses', 'predictive'])
-      # Normalize so we can use the same learning rate regardless of
-      # how many examples we have.
-      loss = (-gp.log_prob(labels) + jax.tree_util.tree_reduce(
-          jax.numpy.add, mutables['losses'])) / features.shape[0]
+      loss = -gp.log_prob(labels) + jax.tree_util.tree_reduce(
+          jnp.add, mutables['losses']
+      )
       return loss, dict()
 
     return model, loss_fn
 
   def __call__(
-      self,
-      inputs: chex.Array = None
-  ) -> Generator[sp.ModelParameter, chex.Array, tfd.GaussianProcess]:
+      self, inputs: Optional[types.Array] = None
+  ) -> Generator[sp.ModelParameter, jax.Array, tfd.GaussianProcess]:
     """Creates a generator.
 
     Args:
       inputs: tuple of (train_features, train_labels) train_features - array of
         dimension (num_examples, _feature_dim) train_labels - array of dimension
         (num_examples,)
 
@@ -117,30 +116,34 @@
     # Kernel
     kernel = tfpk.MaternThreeHalves(
         amplitude=jnp.sqrt(signal_variance)) + tfpk.Linear()
 
     # Length scale
     length_scale = yield sp.ModelParameter.from_prior(
         tfd.LogNormal(
-            loc=jnp.float64(0.0), scale=jnp.float64(1.0), name='length_scale'),
-        constraint=sp.Constraint((0., None), bijector=tfb.Exp()))
+            loc=jnp.float64(0.0), scale=jnp.float64(1.0), name='length_scale'
+        ),
+        constraint=sp.Constraint((0.0, None), bijector=tfb.Exp()),
+    )
     kernel = tfpk.FeatureScaled(kernel, scale_diag=length_scale)
 
     # Kumaraswamy input warping
     kumar_log_normal = tfd.LogNormal(loc=jnp.float64(0.0), scale=0.75)
 
     concentration0 = yield sp.ModelParameter.from_prior(
         kumar_log_normal.copy(name='concentration0'),
-        constraint=sp.Constraint((0., 10.), bijector=sigmoid))
+        constraint=sp.Constraint((0.0, 10.0), bijector=sigmoid),
+    )
 
     concentration1 = yield sp.ModelParameter.from_prior(
         kumar_log_normal.copy(name='concentration1'),
-        constraint=sp.Constraint((0., 10.), bijector=sigmoid))
+        constraint=sp.Constraint((0.0, 10.0), bijector=sigmoid),
+    )
 
     kernel = tfpk.KumaraswamyTransformed(kernel, concentration1, concentration0)
 
     return tfd.GaussianProcess(
         kernel,
         index_points=inputs,
         observation_noise_variance=observation_noise_variance,
         cholesky_fn=None,
-        always_yield_multivariate_normal=True)
+    )
```

### Comparing `google-vizier-0.1.4/vizier/_src/jax/models/hebo_gp_model_test.py` & `google-vizier-0.1.5/vizier/_src/jax/models/hebo_gp_model_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         features=self.x_obs, labels=self.y_obs)
     setup = lambda rng: model.init(rng, self.x_obs)['params']
     key = jax.random.PRNGKey(2)
     init_params = setup(key)
     optimize = optimizers.OptaxTrainWithRandomRestarts(
         optax.adam(5e-3), epochs=500, verbose=True, random_restarts=20
     )
-    constraints = sp.get_constraints(model.coroutine)
+    constraints = sp.get_constraints(model)
     params, metrics = optimize(setup, loss_fn, key, constraints=constraints)
 
     init_gp = model.apply({'params': init_params}, self.x_obs)
     gp = model.apply({'params': params}, self.x_obs)
     self.assertGreater(gp.log_prob(self.y_obs), init_gp.log_prob(self.y_obs))
     losses_every_50 = metrics['loss'][::50]
     self.assertTrue((losses_every_50[1:] < losses_every_50[:-1]).all())
```

### Comparing `google-vizier-0.1.4/vizier/_src/jax/models/tuned_gp_models.py` & `google-vizier-0.1.5/vizier/_src/jax/models/tuned_gp_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,38 +15,39 @@
 from __future__ import annotations
 
 """Collection of well-tuned GP models."""
 
 # TODO: Add Ax/BoTorch GP.
 
 import functools
-from typing import Any, Generator
+from typing import Any, Generator, Optional, Union
 
 import attr
-import chex
 import jax
 from jax import numpy as jnp
 from jax.config import config
 import numpy as np
 from tensorflow_probability.substrates import jax as tfp
 from vizier._src.jax import stochastic_process_model as sp
+from vizier._src.jax import types
 from vizier._src.jax.optimizers import optimizers
 
 # Jax disables float64 computations by default and will silently convert
 # float64s to float32s. We must explicitly enable float64.
 config.update('jax_enable_x64', True)
 
 tfb = tfp.bijectors
 tfd = tfp.distributions
-Array = Any
 tfpk = tfp.math.psd_kernels
 
 
 @attr.define
-class VizierGaussianProcess(sp.ModelCoroutine[chex.Array, tfd.GaussianProcess]):
+class VizierGaussianProcess(
+    sp.ModelCoroutine[types.Array, tfd.GaussianProcess]
+):
   """Vizier's tuned GP.
 
   See __call__ method documentation.
 
   Attributes:
     _boundary_epsilon: We expand the constraints by this number so that the
       values exactly at the boundary can be mapped to unconstrained space. i.e.
@@ -57,41 +58,43 @@
   _feature_dim: int
   _use_retrying_cholesky: bool = attr.field(default=True, kw_only=True)
   _boundary_epsilon: float = attr.field(default=1e-12, kw_only=True)
 
   @classmethod
   def model_and_loss_fn(
       cls,
-      features: chex.Array,
-      labels: chex.Array,
+      features: types.Array,
+      labels: types.Array,
       *,
       use_retrying_cholesky: bool = True,
   ) -> tuple[sp.StochasticProcessModel, optimizers.LossFunction]:
     """Returns the model and loss function."""
     gp_coroutine = VizierGaussianProcess(
         features.shape[-1], use_retrying_cholesky=use_retrying_cholesky
     )
     model = sp.StochasticProcessModel(gp_coroutine)
 
     # Run ARD.
     def loss_fn(params):
       gp, mutables = model.apply({'params': params},
                                  features,
                                  mutable=['losses', 'predictive'])
-      # Normalize so we can use the same learning rate regardless of
-      # how many examples we have.
-      loss = (-gp.log_prob(labels) + jax.tree_util.tree_reduce(
-          jax.numpy.add, mutables['losses'])) / features.shape[0]
+      loss = -gp.log_prob(labels) + jax.tree_util.tree_reduce(
+          jax.numpy.add, mutables['losses']
+      )
       return loss, dict()
 
     return model, loss_fn
 
   def _log_uniform_init(
-      self, low: float, high: float, shape: tuple[int,
-                                                  ...] = tuple()) -> sp.InitFn:
+      self,
+      low: Union[float, np.floating],
+      high: Union[float, np.floating],
+      shape: tuple[int, ...] = tuple(),
+  ) -> sp.InitFn:
     r"""Take log-uniform sample in the constraint and map it back to \R.
 
     Args:
       low: Parameter lower bound.
       high: Parameter upper bound.
       shape: Returned array has this shape. Each entry in the returned array is
         an i.i.d sample.
@@ -103,17 +106,16 @@
     def sample(key: Any) -> jnp.ndarray:
       unif = jnp.array(jax.random.uniform(key, shape, dtype=jnp.float64))
       return jnp.exp(unif * jnp.log(high / low) + jnp.log(low))
 
     return sample
 
   def __call__(
-      self,
-      inputs: Array = None
-  ) -> Generator[sp.ModelParameter, Array, tfd.GaussianProcess]:
+      self, inputs: Optional[types.Array] = None
+  ) -> Generator[sp.ModelParameter, jax.Array, tfd.GaussianProcess]:
     """Creates a generator.
 
     Args:
       inputs: Floating array of dimension (num_examples, _feature_dim).
 
     Yields:
       GaussianProcess whose event shape is `num_examples`.
@@ -170,9 +172,8 @@
       cholesky_fn = lambda matrix: retrying_cholesky(matrix)[0]
 
     return tfd.GaussianProcess(
         kernel,
         index_points=inputs,
         observation_noise_variance=observation_noise_variance,
         cholesky_fn=cholesky_fn,
-        always_yield_multivariate_normal=True,
     )
```

### Comparing `google-vizier-0.1.4/vizier/_src/jax/models/tuned_gp_models_test.py` & `google-vizier-0.1.5/vizier/_src/jax/models/tuned_gp_models_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     target_loss = -0.2
     model, loss_fn = tuned_gp_models.VizierGaussianProcess.model_and_loss_fn(
         x_obs, y_obs
     )
     setup = lambda rng: model.init(rng, x_obs)['params']
 
     optimize = optimizers.JaxoptLbfgsB(random_restarts=50)
-    constraints = sp.get_constraints(model.coroutine)
+    constraints = sp.get_constraints(model)
     optimal_params, metrics = optimize(
         setup, loss_fn, jax.random.PRNGKey(2), constraints=constraints
     )
     logging.info('Optimal: %s', optimal_params)
     logging.info('Loss: %s', loss_fn(optimal_params)[0])
     self.assertLess(metrics['loss'].min(), target_loss)
```

### Comparing `google-vizier-0.1.4/vizier/_src/jax/optimizers/optimizers.py` & `google-vizier-0.1.5/vizier/_src/jax/optimizers/optimizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 """High-level wrappers for stochastic process hyperparameter optimizers."""
 
 # TODO: Add optimizers that are frequently used in the literature.
 
 import functools
 import time
-from typing import Optional, Protocol
+from typing import Generic, Optional, Protocol, TypeVar
 
 from absl import logging
 import attr
 import chex
 import jax
 from jax import numpy as jnp
 from jax import random
@@ -32,37 +32,35 @@
 import optax
 from tensorflow_probability.substrates import jax as tfp
 import tree
 from vizier._src.jax import stochastic_process_model as sp
 
 tfb = tfp.bijectors
 
-PRNGKey = chex.PRNGKey
-Params = chex.ArrayTree
+_Params = TypeVar('_Params', bound=chex.ArrayTree)
 OptState = chex.ArrayTree
-Array = chex.Array
 
 
-class Setup(Protocol):
+class Setup(Protocol, Generic[_Params]):
   """Set up the model parameters given RNG key."""
 
-  def __call__(self, rng: PRNGKey):
+  def __call__(self, rng: jax.random.KeyArray) -> _Params:
     """Set up the model parameters given RNG key."""
     pass
 
 
-class LossFunction(Protocol):
+class LossFunction(Protocol, Generic[_Params]):
   """Evaluates model params and returns (loss, dict of auxiliary metrics)."""
 
-  def __call__(self, params: Params) -> tuple[Array, dict[str, Array]]:
+  def __call__(self, params: _Params) -> tuple[jax.Array, chex.ArrayTree]:
     """Evaluates model params and returns (loss, dict of auxiliary metrics)."""
     pass
 
 
-class Optimizer(Protocol):
+class Optimizer(Protocol, Generic[_Params]):
   """Optimizes the LossFunction.
 
   Example:
 
   ```python
   setup: Setup = lambda rng: jax.random.uniform(rng, minval=-5, maxval=5)
 
@@ -74,20 +72,20 @@
       optax.adam(5e-3), epochs=500, verbose=True, random_restarts=50)
   optimal_params, metrics = optimize(setup, loss_fn, jax.random.PRNGKey(0))
   ```
   """
 
   def __call__(
       self,
-      setup: Setup,
-      loss_fn: LossFunction,
-      rng: PRNGKey,
+      setup: Setup[_Params],
+      loss_fn: LossFunction[_Params],
+      rng: jax.random.KeyArray,
       *,
       constraints: Optional[sp.Constraint] = None,
-  ) -> tuple[Params, dict[str, Array]]:
+  ) -> tuple[_Params, chex.ArrayTree]:
     """Optimizes a LossFunction expecting Params as input.
 
     When constraint bijectors are applied, note that the returned parameters are
     in the constrained space (the parameter domain), not the unconstrained space
     over which the optimization takes place.
 
     If the Optimizer uses lower and upper bounds, then it is responsible for
@@ -103,78 +101,92 @@
       Tuple containing optimal input in the constrained space and optimization
       metrics.
     """
     pass
 
 
 @attr.define
-class OptaxTrainWithRandomRestarts(Optimizer):
+class OptaxTrainWithRandomRestarts(Optimizer[_Params]):
   """Wraps an Optax optimizer.
 
+  It's recommended to use this optimizer with a loss function that normalizes by
+  the number of observations. The unnormalized loss function for parameters `p`
+  is typically of the form
+
+  ```None
+  -gp_likelihood(observations | p) + regularization(p)
+  ```
+
+  where regularization may be a negative prior log probability. The likelihood
+  term is approximately proportional to the number of observations. As the
+  number of observations changes over the course of a study, dividing the loss
+  by this number helps ensure that loss values are roughly of the same order of
+  magnitude, such that a constant learning rate may be used for gradient-based
+  optimizers. Vizier library models make this adjustment automatically.
+
   Attributes:
     optimizer: Optax optimizer such as `optax.adam(1e-2)`.
     epochs: Number of train epochs.
     verbose: If >=1, logs the train progress. If >=2, logs the gradients.
-    random_restarts: Must be a non-negative number. If positive, optimizes from
-      multiple random initializations and returns the best.
-    best_n: Return this many optimal points. Must be less than random_restarts.
-      Set it to None if you want to avoid getting extra dimensions in the
-      result.
+    random_restarts: Must be positive; number of random initializations for the
+      optimization.
+    best_n: Number of best values to return from the initializations; must be
+      less than or equal to `random_restarts`.
   """
 
   optimizer: optax.GradientTransformation = attr.field()
   epochs: int = attr.field(kw_only=True)
   verbose: int = attr.field(kw_only=True, default=0, converter=int)
-  random_restarts: int = attr.field(kw_only=True, default=0)
-  best_n: Optional[int] = attr.field(kw_only=True, default=None)
+  random_restarts: int = attr.field(kw_only=True, default=32)
+  best_n: int = attr.field(kw_only=True, default=1)
 
   def __attrs_post_init__(self):
-    if self.random_restarts < (self.best_n or 0):
+    if self.random_restarts < self.best_n:
       raise ValueError(
           f'Cannot generate {self.best_n} results from'
           f' {self.random_restarts} restarts'
       )
 
   def __call__(
       self,
-      setup: Setup,
-      loss_fn: LossFunction,
-      rng: PRNGKey,
+      setup: Setup[_Params],
+      loss_fn: LossFunction[_Params],
+      rng: jax.random.KeyArray,
       *,
       constraints: Optional[sp.Constraint] = None,
-  ) -> tuple[Params, dict[str, Array]]:
+  ) -> tuple[_Params, chex.ArrayTree]:
     if constraints is None or constraints.bijector is None:
       bijector = None
       unconstrained_loss_fn = loss_fn
     else:
       bijector = constraints.bijector
       unconstrained_loss_fn = lambda x: loss_fn(bijector(x))
 
     grad_fn = jax.value_and_grad(unconstrained_loss_fn, has_aux=True)
 
-    def _setup_all(rng: chex.PRNGKey) -> tuple[Params, OptState]:
+    def _setup_all(rng: jax.random.KeyArray) -> tuple[_Params, OptState]:
       """Sets up both model params and optimizer state."""
       params = setup(rng)
       if bijector is not None:
         params = bijector.inverse(params)
       opt_state = self.optimizer.init(params)
       return params, opt_state
 
     def _train_step(
-        params: Params, opt_state: OptState
-    ) -> tuple[Params, OptState, dict[str, Array]]:
+        params: _Params, opt_state: OptState
+    ) -> tuple[_Params, OptState, chex.ArrayTree]:
       """One train step."""
       (loss, metrics), grads = grad_fn(params)
       logging.log_if(logging.INFO, 'gradients: %s', self.verbose >= 2, grads)
       updates, opt_state = self.optimizer.update(grads, opt_state, params)
       params = optax.apply_updates(params, updates)
       metrics['loss'] = loss
       return params, opt_state, metrics
 
-    if self.random_restarts:
+    if self.random_restarts > 1:
       # Random restarts are implemented via jax.vmap.
       # Note that both setup_all and train_step are vmapped.
       rngs = random.split(rng, self.random_restarts)
       params, opt_state = jax.vmap(_setup_all)(rngs)
       train_step = jax.vmap(_train_step)
     else:
       params, opt_state = _setup_all(rng)
@@ -206,57 +218,63 @@
         jnp.array,
         transposed_metrics,
         is_leaf=lambda x: jax.tree_util.tree_structure(x) == outer_treedef,
     )
 
     final_losses = metrics['loss'][-1]
     logging.info('Final loss: %s', final_losses)
-    if self.random_restarts:
-      best_n = self.best_n or 1
-      # Extract the best only.
-      argsorted = jnp.argsort(final_losses)
-      logging.info('Best loss(es): %s', final_losses[argsorted[:best_n]])
-      params = jax.tree_map(lambda x: x[argsorted[:best_n]], params)
-      if self.best_n is None:
-        params = jax.tree_map(functools.partial(jnp.squeeze, axis=0), params)
+    # Extract the best only.
+    argsorted = jnp.argsort(final_losses)
+    logging.info('Best loss(es): %s', final_losses[argsorted[: self.best_n]])
+    params = jax.tree_map(lambda x: x[argsorted[: self.best_n]], params)
+    if self.best_n == 1:
+      params = jax.tree_map(functools.partial(jnp.squeeze, axis=0), params)
     if bijector is not None:
       params = bijector(params)
     return params, metrics
 
 
 @attr.define
-class JaxoptLbfgsB(Optimizer):
+class JaxoptLbfgsB(Optimizer[_Params]):
   """Jaxopt's L-BFGS-B optimizer.
 
   Jaxopt calls Scipy's L-BFGS-B, which wraps a Fortran implementation.
   L-BFGS-B is a version of L-BFGS that incorporates box constraints on
   parameters.
   https://digital.library.unt.edu/ark:/67531/metadc666315/m2/1/high_res_d/204262.pdf
 
   Attributes:
     num_line_search_steps: Maximum number of line search steps.
-    random_restarts: Must be a non-negative number. If positive, optimizes from
-      multiple random initializations and returns the best.
-    best_n: Number of top values to return.
+    random_restarts: Must be positive; number of random initializations for the
+      optimization.
+    best_n: Number of best values to return from the initializations; must be
+      less than or equal to `random_restarts`.
     _speed_test: If True, return speed test results.
   """
 
   num_line_search_steps: int = attr.field(kw_only=True, default=20)
-  random_restarts: int = attr.field(kw_only=True, default=64)
-  best_n: Optional[int] = attr.field(kw_only=True, default=None)
+  random_restarts: int = attr.field(kw_only=True, default=4)
+  best_n: int = attr.field(kw_only=True, default=1)
   _speed_test: bool = attr.field(kw_only=True, default=False)
 
+  def __attrs_post_init__(self):
+    if self.random_restarts < self.best_n:
+      raise ValueError(
+          f'Cannot generate {self.best_n} results from'
+          f' {self.random_restarts} restarts'
+      )
+
   def __call__(
       self,
-      setup: Setup,
-      loss_fn: LossFunction,
-      rng: chex.PRNGKey,
+      setup: Setup[_Params],
+      loss_fn: LossFunction[_Params],
+      rng: jax.random.KeyArray,
       *,
       constraints: Optional[sp.Constraint] = None,
-  ) -> tuple[Params, dict[str, Array]]:
+  ) -> tuple[_Params, chex.ArrayTree]:
     # L-BFGS-B may be used on unconstrained problems (in which case it is
     # slightly different from L-BFGS, in that it uses the Cauchy point/subspace
     # minimization to choose the line search direction). Bounds must be None or
     # a tuple of size 2. The tuple must contain lower/upper bounds, which may be
     # None or a pytree with the same structure as the model parameters returned
     # by setup (otherwise Jaxopt will raise an error).
     p = setup(jax.random.PRNGKey(0))
@@ -309,23 +327,21 @@
         losses.append(opt_state.fun_val)
         params.append(position)
         logging.info('Loss: %s', opt_state.fun_val)
         logging.info('Last step time: %s', train_times[-1])
 
     all_params = jax.tree_util.tree_map(lambda *x: jnp.stack(x), *params)
     losses = jnp.array(losses)
-    if self.random_restarts:
-      best_n = self.best_n or 1
-      argsorted = jnp.argsort(losses)
-      logging.info('Best loss(es): %s', losses[argsorted[:best_n]])
-      optimal_params = jax.tree_util.tree_map(lambda p: p[argsorted[:best_n]],
-                                              all_params)
-      if self.best_n is None:
-        optimal_params = jax.tree_map(
-            functools.partial(jnp.squeeze, axis=0), optimal_params)
-    else:
-      optimal_params = all_params
+    argsorted = jnp.argsort(losses)
+    logging.info('Best loss(es): %s', losses[argsorted[: self.best_n]])
+    optimal_params = jax.tree_util.tree_map(
+        lambda p: p[argsorted[: self.best_n]], all_params
+    )
+    if self.best_n == 1:
+      optimal_params = jax.tree_map(
+          functools.partial(jnp.squeeze, axis=0), optimal_params
+      )
 
     metrics['loss'] = losses
     if self._speed_test:
       metrics['train_time'] = train_times
     return optimal_params, metrics
```

### Comparing `google-vizier-0.1.4/vizier/_src/jax/optimizers/optimizers_test.py` & `google-vizier-0.1.5/vizier/_src/jax/optimizers/optimizers_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/jax/stochastic_process_model.py` & `google-vizier-0.1.5/vizier/_src/jax/stochastic_process_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,49 +13,42 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Flax module for a trainable stochastic process."""
 
 import abc
-from typing import Any, Callable, Generator, Generic, Iterable, Mapping, Optional, Protocol, TypeVar, Union
+from typing import Any, Callable, Generator, Generic, Optional, Protocol, TypeVar
 
+from absl import logging
 import attr
-import chex
+from flax import config as flax_config
 from flax import linen as nn
 import jax
 from jax import numpy as jnp
 from jax import tree_util
+from jax.typing import ArrayLike
 from tensorflow_probability.substrates import jax as tfp
 import tree
+from vizier._src.jax import types
 
-Array = chex.Array
-ArrayTree = chex.ArrayTree
-PRNGKey = chex.PRNGKey
-
-# An ArrayTree that allows None values.
-ArrayTreeOptional = Union[
-    Array,
-    Iterable[Optional['ArrayTreeOptional']],
-    Mapping[Any, Optional['ArrayTreeOptional']],
-]
+flax_config.update('flax_return_frozendict', False)
 
 tfd = tfp.distributions
 tfb = tfp.bijectors
-tfpk = tfp.math.psd_kernels
 
+_In = TypeVar('_In', bound=types.ArrayTree)
 _D = TypeVar('_D', bound=tfd.Distribution)
-_In = TypeVar('_In', bound=ArrayTree)
 
 
 class InitFn(Protocol):
   """Protocol for Flax parameter initialization functions."""
 
   @abc.abstractmethod
-  def __call__(self, rng: PRNGKey) -> Array:
+  def __call__(self, rng: jax.random.KeyArray) -> jax.Array:
     pass
 
 
 @attr.frozen
 class Constraint:
   """Class specifying parameter constraints.
 
@@ -77,23 +70,30 @@
     bijector: A TFP bijector-like constraint function mapping the parameter (or
       structure of parameters) from an unconstrained space to the parameter
       domain. A value of `None` is equivalent to the identity function. A
       bijector that maps structures of parameters will typically be an instance
       of `tfb.JointMap`.
   """
 
-  bounds: Optional[tuple[Optional[ArrayTreeOptional],
-                         Optional[ArrayTreeOptional]]] = None
+  bounds: Optional[
+      tuple[
+          Optional[types.ArrayTreeOptional], Optional[types.ArrayTreeOptional]
+      ]
+  ] = None
   bijector: Optional[tfb.Bijector] = None
 
   @classmethod
   def create(
       cls,
-      bounds: tuple[Optional[ArrayTreeOptional], Optional[ArrayTreeOptional]],
-      bijector_fn: Callable[[Optional[Array], Optional[Array]], tfb.Bijector],
+      bounds: tuple[
+          Optional[types.ArrayTreeOptional], Optional[types.ArrayTreeOptional]
+      ],
+      bijector_fn: Callable[
+          [Optional[ArrayLike], Optional[ArrayLike]], tfb.Bijector
+      ],
   ) -> 'Constraint':
     """Factory that builds a `Constraint` from bounds and a bijector fn.
 
     The constraint's bijector is created by mapping `bijector_fn` over the tree
     structure of the lower/upper bounds. The bijector will operate on the same
     nested structure as the bounds.
 
@@ -152,16 +152,17 @@
     constraint: Parameter constraint.
     regularizer: Regularizes the parameter.
   """
 
   name: str = attr.field()
   init_fn: InitFn = attr.field()
   constraint: Optional[Constraint] = attr.field(default=None)
-  regularizer: Callable[[Array], Array] = attr.field(
-      kw_only=True, default=lambda x: jnp.zeros([], dtype=x.dtype))
+  regularizer: Callable[[ArrayLike], jax.Array] = attr.field(
+      kw_only=True, default=lambda x: jnp.zeros([], dtype=x.dtype)
+  )
 
   @classmethod
   def from_prior(cls,
                  prior: tfd.Distribution,
                  constraint: Optional[Constraint] = None) -> 'ModelParameter':
     """Builds a `ModelParameter` from a `tfd.Distribution`.
 
@@ -190,19 +191,21 @@
     init_fn = sample
     if bounds is not None:
       init_fn = lambda s: jnp.clip(sample(s), *bounds)
     return ModelParameter(
         init_fn=init_fn,
         name=prior.name,
         constraint=Constraint(bounds=bounds, bijector=bijector),
-        regularizer=lambda x: -prior.log_prob(x),
+        # TODO: `jnp.copy` is used to bypass TFP bijector caching;
+        # otherwise JAX tracers are leaked from JIT-ted code.
+        regularizer=lambda x: -prior.log_prob(jnp.copy(x)),
     )
 
 
-ModelParameterGenerator = Generator[ModelParameter, Array, _D]
+ModelParameterGenerator = Generator[ModelParameter, jax.Array, _D]
 
 
 class ModelCoroutine(Protocol, Generic[_In, _D]):
   """`Protocol` to avoid inheritance.
 
   The coroutine pattern allows the `ModelParameter` objects, and the assembly of
   parameters into the kernel and stochastic process, to be specified
@@ -331,25 +334,25 @@
       x_observed,
       y_observed,
       method=gp_model.posterior_predictive)
   ```
   """
 
   coroutine: ModelCoroutine
-  mean_fn: Optional[Callable[[_In], Array]] = None  # `None` implies zero-mean.
+  mean_fn: Optional[Callable[[_In], jax.Array]] = None  # `None` is zero-mean.
 
   def setup(self):
     """Builds module parameters."""
     generator = self.coroutine()
     try:
       p: ModelParameter = next(generator)
       while True:
         # Declare a Flax variable with the name and initialization function from
         # the `ModelParameter`.
-        param: Array = self.param(p.name, p.init_fn)
+        param: jax.Array = self.param(p.name, p.init_fn)
         p: ModelParameter = generator.send(param)
     except StopIteration:
       # Ignore the return value from the generator since this method only builds
       # the Flax parameters.
       pass
 
   def __call__(self, x: _In) -> _D:
@@ -369,33 +372,35 @@
       # If mean_fn is a module, call it so its parameters are initialized.
       _ = self.mean_fn(x)  # pylint: disable=not-callable
     try:
       p: ModelParameter = next(gen)
       while True:
         # "params" is the name that `nn.Module` gives to the collection of read-
         # only variables.
-        param: Array = self.get_variable('params', p.name)
+        param: jax.Array = self.get_variable('params', p.name)
         if p.regularizer:
           self.sow(  # `sow` stores a value in a collection.
               'losses',
               f'{p.name}_regularization',
               p.regularizer(param),
               reduce_fn=lambda _, b: b,
           )
         p = gen.send(param)
     except StopIteration as e:
       # After the generator is exhausted, it raises a `StopIteration` error. The
       # `StopIteration` object has a property `value` of type `_D`.
       gp = e.value
       return gp.copy(mean_fn=self.mean_fn)
 
-  def precompute_predictive(self, x_observed: _In, y_observed: Array) -> None:
+  def precompute_predictive(
+      self, x_observed: _In, y_observed: ArrayLike
+  ) -> None:
     """Builds a stochastic process regression model conditioned on observations.
 
-    The mutable variable returned by this method as auxillary output should be
+    The mutable variable returned by this method as auxiliary output should be
     passed as state to `posterior_predictive`. This avoids repeated, expensive
     operations (often Cholesky decompositions) when computing the posterior
     predictive.
 
     Args:
       x_observed: Index points on which to condition the posterior predictive.
       y_observed: Observations on which to condition the posterior predictive.
@@ -421,15 +426,15 @@
         'predictive',
         'precomputed_cholesky',
         cached_predictive_intermediates,
         reduce_fn=lambda _, b: b,
     )
 
   def posterior_predictive(
-      self, x_predictive: _In, x_observed: _In, y_observed: Array
+      self, x_predictive: _In, x_observed: _In, y_observed: ArrayLike
   ) -> _D:
     """Returns a posterior predictive stochastic process.
 
     The posterior predictive distribution over the function values at
     `x_predictive`, typically a `tfd.GaussianProcessRegressionModel` or
     `tfd.StudentTProcessRegressionModel`, is built using the mutable variable in
     `predictive/precomputed_cholesky`. This avoids repeated, expensive
@@ -479,15 +484,17 @@
   params = {'a': [4.0, 3.0], 'b': -2.0, 'c': [[6.0]]}
   bij = VectorToArrayTree(params)
   bij.inverse(params)  #  => [4.0, 3.0, -2.0, 6.0]
   bij([0.0, 1.0, 2.0, 3.0])  # => {'a': [0.0, 1.0], 'b': 2.0, 'c': [[3.0]]}
   ```
   """
 
-  def __init__(self, arraytree: ArrayTree, *, validate_args: bool = False):
+  def __init__(
+      self, arraytree: types.ParameterDict, *, validate_args: bool = False
+  ):
     """Init.
 
     Args:
       arraytree: A nested structure of Arrays.
       validate_args: If True, does runtime validation. It may be slow.
     """
     parameters = dict(locals())
@@ -502,23 +509,33 @@
     super().__init__(
         [restructure, reshape, split],
         parameters=parameters,
         name='VectorToArrayTree',
         validate_args=validate_args,
     )
 
-  def to_params(self, vector: Array) -> ArrayTree:
+  def to_params(self, vector: ArrayLike) -> types.ParameterDict:
     return self.forward(vector)
 
-  def to_vector(self, params: ArrayTree) -> Array:
+  def to_vector(self, params: types.ParameterDict) -> jax.Array:
     return self.inverse(params)
 
 
-def get_constraints(coroutine: ModelCoroutine) -> Constraint:
-  """Gets the parameter constraints from a ModelCoroutine.
+def get_constraints(
+    model: StochasticProcessModel, x: Optional[Any] = None
+) -> Constraint:
+  """Gets the parameter constraints from a StochasticProcessModel.
+
+  If the model contains trainable Flax variables besides those defined by the
+  coroutine (for example, if `mean_fn` is a Flax module), the non-coroutine
+  variables are assumed to be unconstrained (the bijector passes them through
+  unmodified, and their lower/upper bounds are `None`). In this case `x` must be
+  passed, so that the structure of the non-coroutine parameters dict(s) can be
+  generated. `Constraint` objects for models with constrained parameters aside
+  from those defined in the coroutine must be built manually.
 
   This method runs the coroutine, collects the parameter constraints, and
   returns a new Constraint object in which the lower/upper bounds are dicts
   (corresponding to the parameters dict) and the bijector operates on dicts. The
   object may be passed to a Vizier Optimizer to constrain the parameters for
   optimization.
 
@@ -540,32 +557,41 @@
         regularizer=lambda x: 1e-3 * x**2,
         constraint=length_scale_constraint,
         name='length_scale')
     kernel = tfpk.ExponentiatedQuadratic(
         amplitude=amplitude, length_scale=length_scale)
     return tfd.GaussianProcess(kernel, index_points=inputs)
 
-  constraint = GetConstraints(model_coroutine)
+  model = StochasticProcessModel(model_coroutine)
+  constraint = GetConstraints(model)
   constraint.bijector
   # => tfb.JointMap({'amplitude': tfb.Exp(),
                     'length_scale': tfb.Sigmoid(0.0, 10.0)})
 
   constraint.bounds
   # => ({'amplitude': jnp.array(0.1), 'length_scale': jnp.array(0.0)},
   #     {'amplitude': None, 'length_scale': jnp.array(10.0)})
   ```
 
   Args:
-    coroutine: A generator function that follows the `ModelCoroutine` protocol.
+    model: A `StochasticProcessModel` instance.
+    x: An input that can be passed to `model.lazy_init`. `x` must be of the same
+      structure as the model inputs and may contain arrays or `ShapeDtypeStruct`
+      instances (see flax.linen.Module.lazy_init docs). If `model` contains Flax
+      variables aside from those defined by `model.coroutine` (e.g. in a
+      trainable `mean_fn`) then this arg is required.
 
   Returns:
     constraint: A `Constraint` instance expressing constraints on the parameters
       specified by `coroutine`.
   """
-  gen = coroutine()
+
+  # Run the coroutine to extract constraints for the model parameters defined in
+  # the coroutine.
+  gen = model.coroutine()
   k = jax.random.PRNGKey(0)
   lower = {}
   upper = {}
   bijectors = {}
   try:
     p = next(gen)
     while True:
@@ -579,8 +605,75 @@
       if p.constraint is None or p.constraint.bijector is None:
         bijectors[p.name] = tfb.Identity()
       else:
         bijectors[p.name] = p.constraint.bijector
       p = gen.send(v)
   except StopIteration:
     pass
-  return Constraint((lower, upper), bijector=tfb.JointMap(bijectors=bijectors))
+
+  # `tfb.JointMap` applies a structure of bijectors to a parallel structure of
+  # inputs. Define a `JointMap` bijector that maps an unconstrained parameters
+  # dict to a constrained parameters dict with a dict of bijectors (all dicts
+  # are keyed by parameter names).
+  bijector = tfb.JointMap(bijectors=bijectors)
+  if x is not None:
+    # Get the parameters dict keys, if any, that do not come from the coroutine
+    # (e.g. `mean_fn` parameters).
+    params = model.lazy_init(jax.random.PRNGKey(0), x)['params']
+    non_coroutine_keys = set(params.keys()) - set(bijectors.keys())
+
+    # Define a bijector that ignores (applies an identity transformation to)
+    # non-coroutine parameters.
+    if non_coroutine_keys:
+      logging.info(
+          (
+              'Defining a constraint object that ignores the following'
+              'non-coroutine parameters: %s'
+          ),
+          non_coroutine_keys,
+      )
+
+      def _wrap_bijector_method_to_ignore_non_coro(f):
+        """Wrap bijector methods to pass non-coroutine params through."""
+
+        def _f(p):
+          p_ = p.copy()
+          non_coroutine_params = {k: p_.pop(k) for k in non_coroutine_keys}
+          y = f(p_)
+          y.update(non_coroutine_params)
+          return y
+
+        return _f
+
+      def _bijector_fldj_with_non_coro(p):
+        """Non-coroutine params do not affect the FLDJ."""
+        p_ = {k: v for k, v in p.items() if k not in non_coroutine_keys}
+        return bijector.forward_log_det_jacobian(p_)
+
+      bijector_forward_min_event_ndims = bijector.forward_min_event_ndims.copy()
+      # Populate `lower` and `upper` bounds dicts with `None` values for entries
+      # corresponding to non-coroutine params.
+      for k in non_coroutine_keys:
+        lower[k] = tree.map_structure(lambda _: None, params[k])
+        upper[k] = tree.map_structure(lambda _: None, params[k])
+        bijector_forward_min_event_ndims[k] = tree.map_structure(
+            lambda _: 0, params[k]
+        )
+      bijector = tfb.Inline(
+          forward_fn=_wrap_bijector_method_to_ignore_non_coro(bijector.forward),
+          inverse_fn=_wrap_bijector_method_to_ignore_non_coro(bijector.inverse),
+          forward_log_det_jacobian_fn=_bijector_fldj_with_non_coro,
+          forward_min_event_ndims=bijector_forward_min_event_ndims,
+      )
+    else:
+      # If the model doesn't have params aside from those defined by the
+      # coroutine, its params should have the same structure as `bijectors`
+      # (this assertion failing indicates a bug).
+      try:
+        tree.assert_same_structure(params, bijectors)
+      except ValueError as exc:
+        raise ValueError(
+            '`params` and `bijectors` should have the same nested structure.'
+            f'Saw: `params={params}` and `bijectors={bijectors}`'
+        ) from exc
+
+  return Constraint((lower, upper), bijector=bijector)
```

### Comparing `google-vizier-0.1.4/vizier/_src/jax/stochastic_process_model_test.py` & `google-vizier-0.1.5/vizier/_src/jax/stochastic_process_model_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
   if num_tasks == 1:
     return tfd.StudentTProcess(
         df=dtype(5.0),
         kernel=kernel,
         index_points=inputs,
         observation_noise_variance=np.ones([], dtype=dtype),
         validate_args=True,
+        always_yield_multivariate_student_t=True,
     )
 
   multi_task_kernel = tfpke.Independent(num_tasks=num_tasks, base_kernel=kernel)
   return tfde.MultiTaskGaussianProcess(
       kernel=multi_task_kernel,
       index_points=inputs,
       observation_noise_variance=np.ones([], dtype=dtype),
@@ -153,18 +154,26 @@
   )
   x_predictive = tfpke.ContinuousAndCategoricalValues(
       x_predictive_cont, x_predictive_cat
   )
   return x_observed, y_observed, x_predictive
 
 
+class MeanFn(nn.Module):
+
+  @nn.compact
+  def __call__(self, x):
+    x = nn.relu(nn.Dense(3)(x))
+    x = nn.Dense(1)(x)
+    return jnp.squeeze(x, axis=-1)
+
+
 class StochasticProcessModelTest(parameterized.TestCase):
 
   @parameterized.named_parameters(
-      # TODO: Add a test case with categorical data.
       # TODO: Fix support for f32.
       {
           'testcase_name': 'continuous_only',
           'kernel_coroutine': _continuous_kernel_coroutine,
           'test_data_fn': _make_inputs,
           'num_tasks': 1,
           'dtype': np.float64,
@@ -245,33 +254,36 @@
     )
     pp_log_prob = pp_dist.log_prob(pp_dist.sample(seed=sample_key))
     self.assertTrue(np.isfinite(pp_log_prob).all())
     self.assertEqual(pp_log_prob.dtype, dtype)
 
   @parameterized.named_parameters(
       {
-          'testcase_name': 'continuous_only',
+          'testcase_name': 'continuous_with_mean_fn',
           'num_tasks': 1,
           'kernel_coroutine': _continuous_kernel_coroutine,
           'test_data_fn': _make_inputs,
+          'use_mean_fn': True,
       },
       {
           'testcase_name': 'multitask_continuous',
           'num_tasks': 3,
           'kernel_coroutine': _continuous_kernel_coroutine,
           'test_data_fn': _make_inputs,
       },
       {
           'testcase_name': 'multitask_continuous_categorical',
           'num_tasks': 3,
           'kernel_coroutine': _categorical_kernel_coroutine,
           'test_data_fn': _make_inputs_with_categorical,
       },
   )
-  def test_jax_transformations(self, num_tasks, kernel_coroutine, test_data_fn):
+  def test_jax_transformations(
+      self, num_tasks, kernel_coroutine, test_data_fn, use_mean_fn=False
+  ):
     init_key, data_key, prior_key, post_key = jax.random.split(
         random.PRNGKey(0), num=4
     )
     num_observed = 20
     x_observed, y_observed, x_predictive = test_data_fn(
         data_key,
         num_tasks=num_tasks,
@@ -280,15 +292,16 @@
     )
     model = sp_model.StochasticProcessModel(
         coroutine=functools.partial(
             _test_coroutine,
             kernel_coroutine=kernel_coroutine,
             num_tasks=num_tasks,
             dtype=np.float32,
-        )
+        ),
+        mean_fn=MeanFn() if use_mean_fn else None,
     )
 
     batch_size = 10
     keys = jax.random.split(init_key, num=batch_size)
     init_state = jax.vmap(lambda k: model.init(k, x_observed))(keys)
     s = jax.jit(
         jax.vmap(
@@ -331,15 +344,15 @@
       sample = dist.sample(seed=post_key)
       return dist.log_prob(sample)
 
     pp_log_prob = _posterior_sample_and_log_prob(state)
     log_prob_grad = jax.grad(
         lambda s: jnp.sum(_posterior_sample_and_log_prob(s))
     )(state)
-    for g in log_prob_grad['params'].values():
+    for g in tree.flatten(log_prob_grad['params']):
       self.assertTrue(np.isfinite(g).all())
     self.assertTrue(np.isfinite(pp_log_prob).all())
     self.assertEqual(pp_log_prob.shape, (batch_size,))
 
   def test_cholesky_not_recomputed(self):
     # Need num_observed == num_predictive so the mock Cholesky works for both
     # observed and predictive.
@@ -532,25 +545,33 @@
     for y_, b_ in zip(tree.flatten(y), tree.flatten(lower)):
       if b_ is not None:
         self.assertTrue((y_ > b_).all())
     for y_, b_ in zip(tree.flatten(y), tree.flatten(upper)):
       if b_ is not None:
         self.assertTrue((y_ < b_).all())
 
-  def test_get_constraints(self):
-    constraint = sp_model.get_constraints(_test_coroutine)
-    x_part = np.linspace(-5.0, 5.0, 10)
-    x = {'amplitude': x_part, 'inverse_length_scale': x_part}
-    y = constraint.bijector(x)
+  @parameterized.parameters((None,), (MeanFn,))
+  def test_get_constraints(self, mean_fn):
+    if mean_fn:
+      mean_fn = mean_fn()
+
+    x = jnp.ones([5, 3])
+    model = sp_model.StochasticProcessModel(
+        coroutine=_test_coroutine, mean_fn=mean_fn
+    )
+
+    constraint = sp_model.get_constraints(model, x=x)
+    unconstrained_p = model.lazy_init(jax.random.PRNGKey(0), x)['params']
+    p = constraint.bijector(unconstrained_p)
     lower, upper = constraint.bounds
 
-    self.assertSameElements(list(x.keys()), list(y.keys()))
-    for y_, b_ in zip(tree.flatten(y), tree.flatten(lower)):
+    tree.assert_same_structure(p, unconstrained_p)
+    for y_, b_ in zip(tree.flatten(p), tree.flatten(lower)):
       if b_ is not None:
-        self.assertTrue((y_ > b_).all())
-    for y_, b_ in zip(tree.flatten(y), tree.flatten(upper)):
+        self.assertTrue((y_ >= b_).all())
+    for y_, b_ in zip(tree.flatten(p), tree.flatten(upper)):
       if b_ is not None:
-        self.assertTrue((y_ < b_).all())
+        self.assertTrue((y_ <= b_).all())
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.4/vizier/_src/jax/xla_pareto.py` & `google-vizier-0.1.5/vizier/_src/jax/xla_pareto.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/jax/xla_pareto_test.py` & `google-vizier-0.1.5/vizier/_src/jax/xla_pareto_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyglove/algorithms.py` & `google-vizier-0.1.5/vizier/_src/pyglove/algorithms.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyglove/backend.py` & `google-vizier-0.1.5/vizier/_src/pyglove/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-# Copyright 2019 The PyGlove Authors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
 """Cross-Platform Backend."""
 import enum
 import getpass
 import time
 
 from typing import Any, Dict, Optional, Sequence, Type, Union
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyglove/client.py` & `google-vizier-0.1.5/vizier/_src/pyglove/client.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyglove/constants.py` & `google-vizier-0.1.5/vizier/_src/pyglove/constants.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyglove/converters.py` & `google-vizier-0.1.5/vizier/_src/pyglove/converters.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyglove/core.py` & `google-vizier-0.1.5/vizier/_src/pyglove/core.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyglove/oss_vizier.py` & `google-vizier-0.1.5/vizier/_src/pyglove/oss_vizier.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-# Copyright 2022 The PyGlove Authors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
 """Tuner implementation based on Open Source Vizier."""
 
 from concurrent import futures
 import os
 import threading
 from typing import Optional, Union
 
@@ -41,26 +28,26 @@
 import pyglove as pg
 from vizier import pythia
 from vizier import pyvizier as vz
 from vizier._src.pyglove import algorithms
 from vizier._src.pyglove import backend
 from vizier._src.pyglove import client
 from vizier._src.pyglove import converters
+from vizier._src.service import clients as pyvizier_clients
+from vizier._src.service import constants
+from vizier._src.service import policy_factory as policy_factory_lib
+from vizier._src.service import pythia_service
+from vizier._src.service import pythia_service_pb2_grpc
+from vizier._src.service import resources
+from vizier._src.service import service_policy_supporter
+from vizier._src.service import stubs_util
+from vizier._src.service import types as vizier_types
+from vizier._src.service import vizier_client
 from vizier.client import client_abc
-from vizier.service import clients as pyvizier_clients
-from vizier.service import constants
-from vizier.service import policy_factory as policy_factory_lib
-from vizier.service import pythia_service
-from vizier.service import pythia_service_pb2_grpc
 from vizier.service import pyvizier as svz
-from vizier.service import resources
-from vizier.service import service_policy_supporter
-from vizier.service import stubs_util
-from vizier.service import types as vizier_types
-from vizier.service import vizier_client
 
 from google.protobuf import empty_pb2
 
 BuiltinAlgorithm = algorithms.BuiltinAlgorithm
 ExpandedStudyName = client.ExpandedStudyName
 PolicyCache = client.PolicyCache
 StudyKey = client.StudyKey
@@ -129,17 +116,15 @@
     self._vizier_endpoint = endpoint
     if self._vizier_service is not None:
       return
     if endpoint != constants.NO_ENDPOINT:
       pyvizier_clients.environment_variables.server_endpoint = (
           self._vizier_endpoint
       )
-    self._vizier_service = vizier_client.create_vizier_servicer_or_stub(
-        self._vizier_endpoint
-    )
+    self._vizier_service = vizier_client.create_vizier_servicer_or_stub()
 
   @property
   def vizier_service(self) -> vizier_types.VizierService:
     """Returns current vizier service."""
     assert self._vizier_service, 'call `use_vizier_service` first.'
     return self._vizier_service
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyglove/oss_vizier_test.py` & `google-vizier-0.1.5/vizier/_src/pyglove/oss_vizier_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,44 +10,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-# Copyright 2019 The PyGlove Authors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
 """Tests for pyglove.tuner.vizier2.oss_vizier_test."""
 import os
 from absl import logging
 
 from vizier._src.pyglove import oss_vizier as vizier
 from vizier._src.pyglove import vizier_test_lib
-from vizier.service import vizier_server
+from vizier._src.service import constants
+from vizier._src.service import vizier_server
 
 from absl.testing import absltest
 
 
 class OSSVizierSampleTest(vizier_test_lib.SampleTest):
 
   @classmethod
   def setUpClass(cls):
     super().setUpClass()
-    server = vizier_server.DefaultVizierServer(host=os.uname()[1])
+    server = vizier_server.DefaultVizierServer(
+        host=os.uname()[1], database_url=constants.SQL_MEMORY_URL
+    )
     logging.info(server.endpoint)
     vizier._services.reset_for_testing()
     vizier.init(vizier_endpoint=server.endpoint)
     cls.server = server
     logging.info('Vizier service has been set up!')
 
   def __init__(self, *args, **kwargs):
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyglove/performance_test.py` & `google-vizier-0.1.5/vizier/_src/pyglove/performance_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,30 +19,33 @@
 import os
 import random
 import time
 from absl import logging
 import pyglove as pg
 
 from vizier._src.pyglove import oss_vizier as vizier
-from vizier.service import vizier_server
+from vizier._src.service import constants
+from vizier._src.service import vizier_server
 
 from absl.testing import absltest
 from absl.testing import parameterized
 
 
 NUM_TRIALS_PER_WORKER = 10
 NUM_WORKERS = 10
 
 
 class PerformanceTest(parameterized.TestCase):
 
   @classmethod
   def setUpClass(cls):
     super().setUpClass()
-    server = vizier_server.DefaultVizierServer(host=os.uname()[1])
+    server = vizier_server.DefaultVizierServer(
+        host=os.uname()[1], database_url=constants.SQL_MEMORY_URL
+    )
     logging.info(server.endpoint)
     vizier._services.reset_for_testing()
     vizier.init(vizier_endpoint=server.endpoint)
     cls.server = server
     logging.info('Vizier service is set up!')
 
   @parameterized.parameters(
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyglove/pythia.py` & `google-vizier-0.1.5/vizier/_src/pyglove/pythia.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyglove/pythia_test.py` & `google-vizier-0.1.5/vizier/_src/pyglove/pythia_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class DummyAlgorithm(pg.DNAGenerator):
   """Dummy algorithm for testing."""
 
   def __init__(self):
     super().__init__()
-    self._random = pg.generators.Random(seed=1)
+    self._random = pg.geno.Random(seed=1)
 
   def setup(self, dna_spec: pg.DNASpec):
     super().setup(dna_spec)
     self._random.setup(dna_spec)
 
   def _propose(self) -> pg.DNA:
     return self._random.propose()
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyglove/vizier_test_lib.py` & `google-vizier-0.1.5/vizier/_src/pyglove/vizier_test_lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,27 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-# Copyright 2019 The PyGlove Authors
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
 """Libraries for testing different Tuners on the shared backend."""
 # pylint:disable=protected-access
 import inspect
 from typing import Type
 from absl import flags
 from absl import logging
 import pyglove as pg
@@ -42,15 +29,15 @@
 
 
 class DummyAlgorithm(pg.DNAGenerator):
   """Dummy algorithm for testing."""
 
   def setup(self, dna_spec: pg.DNASpec):
     super().setup(dna_spec)
-    self._random = pg.generators.Random(seed=1)
+    self._random = pg.geno.Random(seed=1)
     self._random.setup(dna_spec)
 
   def _propose(self) -> pg.DNA:
     return self._random.propose()
 
 
 class VizierTest(absltest.TestCase):
@@ -123,15 +110,15 @@
 
     logging.info('Check that constant space raises an error.')
     # Non-deterministic value.
     with self.assertRaisesRegex(ValueError, "'space' is a constant value"):
       next(
           pg.sample(
               pg.Dict(x=1),  # a fixed value.
-              algorithm=pg.generators.Random(seed=1),
+              algorithm=pg.geno.Random(seed=1),
               name='c',
           )
       )
 
   def testSampleWithRaceCondition(self):
     """Test `pg.sample` with race condition among co-workers."""
     self._backend_class.use_study_prefix('coworkers-with-race-conditions')
@@ -156,15 +143,15 @@
 
     algorithm = pg.evolution.Evolution(
         (
             pg.evolution.Identity()[-1]
             >> pg.evolution.mutators.Uniform()
             >> write_metadata
         ),
-        population_init=(pg.generators.Random(), 5),
+        population_init=(pg.geno.Random(), 5),
     )
 
     for i, (x, fx) in enumerate(
         pg.sample(
             pg.oneof(range(100)),
             algorithm=algorithm,
             num_examples=10,
@@ -220,15 +207,15 @@
 
     algorithm = pg.evolution.Evolution(
         (
             pg.evolution.Identity()[-1]
             >> pg.evolution.mutators.Uniform()
             >> controller_side_evaluate
         ),
-        population_init=(pg.generators.Sweeping(), 5),
+        population_init=(pg.geno.Sweeping(), 5),
     )
 
     client_side_evaluated = []
     for x, fx in pg.sample(
         pg.oneof(range(100)), algorithm=algorithm, num_examples=10
     ):
       client_side_evaluated.append(x)
@@ -314,15 +301,15 @@
 
   def testSampleWithCustomTermination(self):
     """Test `pg.sample` with custom termination."""
     self._backend_class.use_study_prefix(None)
     hyper_value = pg.Dict(x=pg.oneof([1, 2, 3]))
     for x, f in pg.sample(
         hyper_value,
-        algorithm=pg.generators.Random(seed=1),
+        algorithm=pg.geno.Random(seed=1),
         name='custom_termination',
     ):
       # Always invoke the feedback function in order to advance
       # to the next trial.
       if f.id == 1:
         f.skip()
       else:
@@ -446,34 +433,34 @@
     self._backend_class.use_study_prefix(None)
 
     hyper_value = pg.Dict(x=pg.oneof([1, 2, 3]))
 
     # Create a new study for sample using Random.
     sample1 = pg.sample(
         hyper_value,
-        algorithm=pg.generators.Random(seed=1),
+        algorithm=pg.geno.Random(seed=1),
         name='distributed_sampling2',
         group=0,
     )
 
     # `sample2` works on the same sampling queue with `sample1`
     # but with different trials by having the same `name` with
     # a different `group`.
     sample2 = pg.sample(
         hyper_value,
-        algorithm=pg.generators.Random(seed=1),
+        algorithm=pg.geno.Random(seed=1),
         name='distributed_sampling2',
         group=1,
     )
 
     # `sample3` works on the same sampling queue and the same trials
     # with `sample1` by having the same `name` and `group`.
     sample3 = pg.sample(
         hyper_value,
-        algorithm=pg.generators.Random(seed=1),
+        algorithm=pg.geno.Random(seed=1),
         name='distributed_sampling2',
         group=0,
     )
 
     # Make sure sampling with different worker IDs get different trial IDs.
     _, f1 = next(sample1)
     self.assertEqual(f1.id, 1)
```

### Comparing `google-vizier-0.1.4/vizier/_src/pythia/local_policy_supporters.py` & `google-vizier-0.1.5/vizier/_src/pythia/local_policy_supporters.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pythia/local_policy_supporters_test.py` & `google-vizier-0.1.5/vizier/_src/pythia/local_policy_supporters_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pythia/policy.py` & `google-vizier-0.1.5/vizier/_src/pythia/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,14 +243,20 @@
         support MakeEarlyEarlyStopDecisions().
       CachedPolicyIsStaleError: Causes the computation to be restarted with a
         freshly constructed Policy instance.  It is incorrect to raise
         this on the first use of a Policy; the Study will be inactivated.
     """
 
   @property
+  def name(self) -> str:
+    """Returns the policy name."""
+    # Derived classes should override this implementation.
+    return __class__.__name__
+
+  @property
   def should_be_cached(self) -> bool:
     """Returns True if it's safe & worthwhile to cache this Policy in RAM.
 
     This is called after MakeEarlyEarlyStopDecisions() and/or MakeSuggestions().
     If True, the policy may be stored in RAM (at least for a while), and state
     may be preserved for the next time that Study makes it to that Pythia
     server.
```

### Comparing `google-vizier-0.1.4/vizier/_src/pythia/policy_supporter.py` & `google-vizier-0.1.5/vizier/_src/pythia/policy_supporter.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pythia/pythia_errors.py` & `google-vizier-0.1.5/vizier/_src/pythia/pythia_errors.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/multimetric/hypervolume.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/hypervolume.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/multimetric/hypervolume_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/hypervolume_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/multimetric/pareto_optimal.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/pareto_optimal.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/pareto_optimal_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/multimetric/safety.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/safety.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/multimetric/safety_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/multimetric/safety_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/oss/automated_stopping.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/oss/automated_stopping.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from __future__ import annotations
 
 """Convenience classes for configuring Vizier Early-Stopping Configs."""
 import copy
 
 import attr
-from vizier.service import study_pb2
+from vizier._src.service import study_pb2
 
 # When new early stopping config protos are added, include them below
 # with a Union[]
 AutomatedStoppingConfigProto = study_pb2.StudySpec.DefaultEarlyStoppingSpec
 
 
 @attr.s(frozen=True, init=True, slots=True, kw_only=True)
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/oss/automated_stopping_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/oss/automated_stopping_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for automated_stopping."""
 
 from vizier._src.pyvizier.oss import automated_stopping
-from vizier.service import study_pb2
+from vizier._src.service import study_pb2
 from vizier._src.pyvizier.oss import compare
 from absl.testing import absltest
 
 
 class AutomatedStoppingTest(absltest.TestCase):
 
   def testDefaultStoppingConfig(self):
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/oss/compare.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/oss/compare.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/oss/metadata_util.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/oss/metadata_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,29 +12,31 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Utility functions for handling vizier metadata."""
 
-from typing import Iterable, Optional, Tuple, Type, TypeVar, Union
+from typing import Dict, Iterable, Optional, Tuple, Type, TypeVar, Union
+from absl import logging
 
 from vizier._src.pyvizier.shared import common
 from vizier._src.pyvizier.shared import trial
-from vizier.service import key_value_pb2
-from vizier.service import study_pb2
-from vizier.service import vizier_service_pb2
+from vizier._src.service import key_value_pb2
+from vizier._src.service import study_pb2
+from vizier._src.service import vizier_service_pb2
 from google.protobuf import any_pb2
 from google.protobuf.message import Message
 
 T = TypeVar('T')
 
 
-def _assign_value(metadatum: key_value_pb2.KeyValue,
-                  value: Union[str, any_pb2.Any, Message]) -> None:
+def _assign_value(
+    metadatum: key_value_pb2.KeyValue, value: Union[str, any_pb2.Any, Message]
+) -> None:
   """Assigns value to $metadatum."""
   if isinstance(value, str):
     metadatum.ClearField('proto')
     metadatum.value = value
   elif isinstance(value, any_pb2.Any):
     metadatum.ClearField('value')
     metadatum.proto.CopyFrom(value)
@@ -45,15 +47,15 @@
 
 def assign(
     container: Union[study_pb2.StudySpec, study_pb2.Trial],
     *,
     key: str,
     ns: str,
     value: Union[str, any_pb2.Any, Message],
-    mode: str = 'insert'
+    mode: str = 'insert',
 ) -> Tuple[key_value_pb2.KeyValue, bool]:
   """Insert and/or assign (key, value) to container.metadata.
 
   Args:
     container: container.metadata must be repeated KeyValue (protobuf) field.
     key:
     ns: A namespace for the key (defaults to '', which is the user's namespace).
@@ -75,28 +77,30 @@
   # Find existing metadatum, unless in `insert` mode.
   existing_metadatum = None
   if mode in ('insert_or_assign', 'insert_or_error'):
     for metadatum in container.metadata:
       if metadatum.key == key and metadatum.ns == ns:
         inserted = False
         if mode == 'insert_or_error':
-          raise ValueError(f'Duplicate (ns, key) pair: '
-                           f'({metadatum.ns}, {metadatum.key})')
+          raise ValueError(
+              f'Duplicate (ns, key) pair: ({metadatum.ns}, {metadatum.key})'
+          )
         existing_metadatum = metadatum
         break
 
   # If the metadatum does not exist, then add the (ns, key) pair.
   metadatum = existing_metadatum or container.metadata.add(key=key, ns=ns)
   _assign_value(metadatum, value)
 
   return metadatum, inserted
 
 
-def get(container: Union[study_pb2.StudySpec, study_pb2.Trial], *, key: str,
-        ns: str) -> Optional[str]:
+def get(
+    container: Union[study_pb2.StudySpec, study_pb2.Trial], *, key: str, ns: str
+) -> Optional[str]:
   """Returns the metadata value associated with key, or None.
 
   Args:
     container: A Trial of a StudySpec in protobuf form.
     key: The key of a KeyValue protobuf.
     ns: A namespace for the key (defaults to '', which is the user's namespace).
   """
@@ -104,16 +108,21 @@
   for kv in container.metadata:
     if kv.key == key and kv.ns == ns:
       if not kv.HasField('proto'):
         return kv.value
   return None
 
 
-def get_proto(container: Union[study_pb2.StudySpec, study_pb2.Trial], *,
-              key: str, ns: str, cls: Type[T]) -> Optional[T]:
+def get_proto(
+    container: Union[study_pb2.StudySpec, study_pb2.Trial],
+    *,
+    key: str,
+    ns: str,
+    cls: Type[T],
+) -> Optional[T]:
   """Unpacks the proto metadata into message.
 
   Args:
     container: (const) StudySpec or Trial to search the metadata from.
     key: (const) Lookup key of the metadata.
     ns: A namespace for the key (defaults to '', which is the user's namespace).
     cls: Pass in a proto ***class***, not a proto object.
@@ -128,31 +137,34 @@
         message = cls()
         success = kv.proto.Unpack(message)
         return message if success else None
   return None
 
 
 def make_key_value_list(
-    metadata: common.Metadata) -> list[key_value_pb2.KeyValue]:
+    metadata: common.Metadata,
+) -> list[key_value_pb2.KeyValue]:
   """Convert $metadata to a list of KeyValue protobufs."""
   result = []
   for ns, k, v in metadata.all_items():
     item = key_value_pb2.KeyValue(key=k, ns=ns.encode())
     _assign_value(item, v)
     result.append(item)
   return result
 
 
 def from_key_value_list(
-    kv_s: Iterable[key_value_pb2.KeyValue]) -> common.Metadata:
+    kv_s: Iterable[key_value_pb2.KeyValue],
+) -> common.Metadata:
   """Converts a list of KeyValue protos into a Metadata object."""
   metadata = common.Metadata()
   for kv in kv_s:
     metadata.abs_ns(common.Namespace.decode(kv.ns))[kv.key] = (
-        kv.proto if kv.HasField('proto') else kv.value)
+        kv.proto if kv.HasField('proto') else kv.value
+    )
   return metadata
 
 
 def trial_metadata_to_update_list(
     trial_metadata: dict[int, common.Metadata]
 ) -> list[vizier_service_pb2.UnitMetadataUpdate]:
   """Convert a dictionary of Trial.id:Metadata to a list of UnitMetadataUpdate.
@@ -167,45 +179,94 @@
   for trial_id, md in trial_metadata.items():
     for kv in make_key_value_list(md):
       # TODO: Verify this implementation.
       # Should str(trial_id) below be "resources.StudyResource.from_name(
       # study_resource_name).trial_resource(trial_id=str(trial_id)).name"?
       result.append(
           vizier_service_pb2.UnitMetadataUpdate(
-              trial_id=str(trial_id), metadatum=kv))
+              trial_id=str(trial_id), metadatum=kv
+          )
+      )
   return result
 
 
 def study_metadata_to_update_list(
-    study_metadata: common.Metadata
+    study_metadata: common.Metadata,
 ) -> list[vizier_service_pb2.UnitMetadataUpdate]:
   """Convert `on_study` metadata to list of metadata update protos."""
   unit_metadata_updates = []
   for ns, k, v in study_metadata.all_items():
     unit_metadata_update = vizier_service_pb2.UnitMetadataUpdate()
     metadatum = unit_metadata_update.metadatum
     metadatum.key = k
     metadatum.ns = ns.encode()
     _assign_value(metadatum, v)
     unit_metadata_updates.append(unit_metadata_update)
   return unit_metadata_updates
 
 
 def to_request_proto(
-    study_resource_name: str,
-    delta: trial.MetadataDelta) -> vizier_service_pb2.UpdateMetadataRequest:
+    study_resource_name: str, delta: trial.MetadataDelta
+) -> vizier_service_pb2.UpdateMetadataRequest:
   """Create an UpdateMetadataRequest proto.
 
   Args:
     study_resource_name:
     delta:
 
   Returns:
-
   """
   request = vizier_service_pb2.UpdateMetadataRequest(name=study_resource_name)
 
   # Study Metadata
   request.delta.extend(study_metadata_to_update_list(delta.on_study))
   # Trial metadata
   request.delta.extend(trial_metadata_to_update_list(delta.on_trials))
   return request
+
+
+def merge_study_metadata(
+    study_spec: study_pb2.StudySpec,
+    new_metadata: Iterable[key_value_pb2.KeyValue],
+) -> None:
+  """Merges $new_metadata into a Study's existing metadata."""
+  metadata_dict: Dict[Tuple[str, str], key_value_pb2.KeyValue] = {}
+  for kv in study_spec.metadata:
+    metadata_dict[(kv.ns, kv.key)] = kv
+  for kv in new_metadata:
+    metadata_dict[(kv.ns, kv.key)] = kv
+  study_spec.ClearField('metadata')
+  study_spec.metadata.extend(
+      sorted(metadata_dict.values(), key=lambda kv: (kv.ns, kv.key))
+  )
+
+
+def merge_trial_metadata(
+    trial_proto: study_pb2.Trial,
+    new_metadata: Iterable[vizier_service_pb2.UnitMetadataUpdate],
+) -> None:
+  """Merges $new_metadata into a Trial's existing metadata.
+
+  Args:
+    trial_proto: A representation of a Trial; this will be modified.
+    new_metadata: Metadata that will add or update metadata in the Trial.
+  NOTE: the metadata updates in $new_metadata should have the same ID as
+    $trial_proto.
+  """
+  metadata_dict: Dict[Tuple[str, str], key_value_pb2.KeyValue] = {}
+  for kv in trial_proto.metadata:
+    metadata_dict[(kv.ns, kv.key)] = kv
+  for md_update in new_metadata:
+    if md_update.trial_id == trial_proto.id:
+      metadata_dict[(md_update.metadatum.ns, md_update.metadatum.key)] = (
+          md_update.metadatum
+      )
+    else:
+      logging.warning(
+          'Metadata associated with wrong trial: %s instead of %s',
+          md_update.trial_id,
+          trial_proto.id,
+      )
+  trial_proto.ClearField('metadata')
+  trial_proto.metadata.extend(
+      sorted(metadata_dict.values(), key=lambda kv: (kv.ns, kv.key))
+  )
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/oss/metadata_util_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/oss/metadata_util_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for vizier.pyvizier.oss.metadata_util."""
 
 from vizier._src.pyvizier.oss import metadata_util
-from vizier.service import study_pb2
+from vizier._src.service import study_pb2
 
 from absl.testing import absltest
 
 
 class MetadataUtilTest(absltest.TestCase):
 
   def test_get(self):
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/oss/proto_converters.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/oss/proto_converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 from typing import Iterable, List, Optional, Sequence, Tuple, Union
 
 from absl import logging
 from vizier import pyvizier as vz
 from vizier._src.pythia import policy
 from vizier._src.pyvizier.oss import metadata_util
 from vizier._src.pyvizier.pythia import study
-from vizier.service import pythia_service_pb2
-from vizier.service import study_pb2
-from vizier.service import vizier_service_pb2
+from vizier._src.service import pythia_service_pb2
+from vizier._src.service import study_pb2
+from vizier._src.service import vizier_service_pb2
 
 ScaleType = vz.ScaleType
 _ScaleTypePb2 = study_pb2.StudySpec.ParameterSpec.ScaleType
 ParameterType = vz.ParameterType
 MonotypeParameterSequence = vz.MonotypeParameterSequence
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/oss/proto_converters_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/oss/proto_converters_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import attr
 
 from vizier._src.pyvizier.oss import proto_converters
 from vizier._src.pyvizier.pythia import study
 from vizier._src.pyvizier.shared import parameter_config as pc
 from vizier._src.pyvizier.shared import trial
-from vizier.service import study_pb2
+from vizier._src.service import study_pb2
 
 from google.protobuf import struct_pb2
 from google.protobuf import wrappers_pb2
 from vizier._src.pyvizier.oss import compare
 from absl.testing import absltest
 from absl.testing import parameterized
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/oss/study_config.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/oss/study_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import attr
 from vizier import pyvizier as vz
 from vizier._src.pyvizier.oss import automated_stopping
 from vizier._src.pyvizier.oss import metadata_util
 from vizier._src.pyvizier.oss import proto_converters
-from vizier.service import constants
-from vizier.service import study_pb2
+from vizier._src.service import constants
+from vizier._src.service import study_pb2
 
 ################### PyTypes ###################
 # Possible types for trial parameter values after cast to external types.
 # TODO: Define this in _src/shared/
 ParameterValueSequence = Union[vz.ParameterValueTypes, Sequence[int],
                                Sequence[float], Sequence[str], Sequence[bool]]
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/oss/study_config_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/oss/study_config_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for vizier.pyvizier.oss.study_config."""
 import datetime
 
-from vizier.service import constants
-from vizier.service import key_value_pb2
+from vizier._src.service import constants
+from vizier._src.service import key_value_pb2
+from vizier._src.service import study_pb2
 from vizier.service import pyvizier as vz
-from vizier.service import study_pb2
 
 from google.protobuf import struct_pb2
 from vizier._src.pyvizier.oss import compare
 from absl.testing import absltest
 from absl.testing import parameterized
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/pythia/study.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/pythia/study.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/shared/base_study_config.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/shared/base_study_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,26 +36,29 @@
 _T = TypeVar('_T')
 
 
 ################### Helper Classes ###################
 def _min_leq_max(instance: 'MetricInformation', _, value: float):
   if value > instance.max_value:
     raise ValueError(
-        f'min_value={value} cannot exceed max_value={instance.max_value}.')
+        f'min_value={value} cannot exceed max_value={instance.max_value}.'
+    )
 
 
 def _max_geq_min(instance: 'MetricInformation', _, value: float):
   if value < instance.min_value:
     raise ValueError(
-        f'min_value={instance.min_value} cannot exceed max_value={value}.')
+        f'min_value={instance.min_value} cannot exceed max_value={value}.'
+    )
 
 
 # Values should NEVER be removed from ObjectiveMetricGoal, only added.
 class ObjectiveMetricGoal(enum.IntEnum):
   """Valid Values for MetricInformation.Goal."""
+
   MAXIMIZE = 1
   MINIMIZE = 2
 
   # pylint: disable=comparison-with-callable
   @property
   def is_maximize(self) -> bool:
     return self == self.MAXIMIZE
@@ -67,14 +70,15 @@
 
 class MetricType(enum.Enum):
   """Type of the metric.
 
   OBJECTIVE: Objective to be maximized / minimized.
   SAFETY: Objective to be kept above / below a certain threshold.
   """
+
   OBJECTIVE = 'OBJECTIVE'
   SAFETY = 'SAFETY'  # Soft constraint
 
   # pylint: disable=comparison-with-callable
   @property
   def is_safety(self) -> bool:
     return self == MetricType.SAFETY
@@ -87,75 +91,82 @@
 @attr.define(frozen=False, init=True, slots=True)
 class MetricInformation:
   """MetricInformation provides optimization metrics configuration."""
 
   # The name of this metric. An empty string is allowed for single-metric
   # optimizations.
   name: str = attr.field(
-      init=True, default='', validator=attr.validators.instance_of(str))
+      init=True, default='', validator=attr.validators.instance_of(str)
+  )
 
   goal: ObjectiveMetricGoal = attr.field(
       init=True,
       # pylint: disable=g-long-lambda
       converter=ObjectiveMetricGoal,
       validator=attr.validators.instance_of(ObjectiveMetricGoal),
       on_setattr=[attr.setters.convert, attr.setters.validate],
-      kw_only=True)
+      kw_only=True,
+  )
 
   # The following should be used to configure this as a safety metric.
   # safety_threshold must always be set to a float (default 0.0), for safety
   # metrics.
   safety_threshold: Optional[float] = attr.field(
       init=True,
       default=None,
       validator=attr.validators.optional(attr.validators.instance_of(float)),
-      kw_only=True)
+      kw_only=True,
+  )
   # Safety_std_threshold is DEPRECATED and is here for backward compatibility.
   # To configure how cautious the optimization should be, please defer to
   # desired_min_safe_trials_fraction. This corresponds to the allowed
   # probability threshold (as a function of the z-score) of
   # violating the safety_threshold.
   safety_std_threshold: Optional[float] = attr.field(
       init=True,
       default=None,
       validator=attr.validators.optional(attr.validators.instance_of(float)),
-      kw_only=True)
+      kw_only=True,
+  )
   # Desired minimum fraction of safe trials (over total number of trials)
   # that should be targeted by the algorithm during the entire duration of the
   # study (best effort). A value of 0.0 is the same as None. If unset, or set
   # to 0.0, then Vizier has no constraint on the number/fraction of unsafe
   # trials it can suggest.
   desired_min_safe_trials_fraction: Optional[float] = attr.field(
       init=True,
       default=None,
       validator=[
           attr.validators.optional(attr.validators.instance_of(float)),
           attr.validators.optional(attr.validators.le(1.0)),
-          attr.validators.optional(attr.validators.ge(0.0))
+          attr.validators.optional(attr.validators.ge(0.0)),
       ],
-      kw_only=True)
+      kw_only=True,
+  )
 
   # Minimum value of this metric can be optionally specified.
   min_value: float = attr.field(
       init=True,
       default=None,
       # FYI: Converter is applied before validator.
       converter=lambda x: float(x) if x is not None else -np.inf,
       validator=[attr.validators.instance_of(float), _min_leq_max],
-      kw_only=True)
+      kw_only=True,
+  )
 
   # Maximum value of this metric can be optionally specified.
   max_value: float = attr.field(
       init=True,
       default=None,
       # FYI: Converter is applied before validator.
       converter=lambda x: float(x) if x is not None else np.inf,
       validator=[attr.validators.instance_of(float), _max_geq_min],
       on_setattr=attr.setters.validate,
-      kw_only=True)
+      kw_only=True,
+  )
 
   def min_value_or(self, default_value_fn: Callable[[], float]) -> float:
     """Returns the minimum value if finite, or default_value_fn().
 
     Avoids the common pitfalls of using
       `metric.min_value or default_value`
     which would incorrectly use the default_value when min_value == 0, and
@@ -208,26 +219,32 @@
 
 @attr.define(frozen=False, init=True, slots=True)
 class MetricsConfig(Collection[MetricInformation]):
   """Container for metrics.
 
   Metric names should be unique.
   """
+
   _metrics: List[MetricInformation] = attr.ib(
       init=True,
       factory=list,
       converter=list,
       validator=attr.validators.deep_iterable(
           member_validator=attr.validators.instance_of(MetricInformation),
-          iterable_validator=attr.validators.instance_of(Iterable)))
+          iterable_validator=attr.validators.instance_of(Iterable),
+      ),
+  )
 
   def item(self) -> MetricInformation:
     if len(self._metrics) != 1:
-      raise ValueError('item() may only be called when there is exactly one '
-                       'metric (there are %d).' % len(self._metrics))
+      raise ValueError(
+          'item() may only be called when there is exactly one '
+          'metric (there are %d).'
+          % len(self._metrics)
+      )
     return self._metrics[0]
 
   def _assert_names_are_unique(self) -> None:
     counts = collections.Counter(metric.name for metric in self._metrics)
     if len(counts) != len(self._metrics):
       for name, count in counts.items():
         if count > 1:
@@ -245,16 +262,16 @@
   def __len__(self) -> int:
     return len(self._metrics)
 
   def __add__(self, metrics: Iterable[MetricInformation]) -> 'MetricsConfig':
     return MetricsConfig(self._metrics + list(metrics))
 
   def of_type(
-      self, include: Union[MetricType,
-                           Iterable[MetricType]]) -> 'MetricsConfig':
+      self, include: Union[MetricType, Iterable[MetricType]]
+  ) -> 'MetricsConfig':
     """Filters the Metrics by type."""
     if isinstance(include, MetricType):
       include = (include,)
     return MetricsConfig(m for m in self._metrics if m.type in include)
 
   def exclude_type(
       self, exclude: Union[MetricType, Iterable[MetricType]]
@@ -298,28 +315,34 @@
   Pythia `Policy` interface uses `ProblemStatement` as opposed to `StudyConfig`
   so that the same algorithm code can be used across platforms.
   """
 
   search_space: parameter_config.SearchSpace = attr.ib(
       init=True,
       factory=parameter_config.SearchSpace,
-      validator=attr.validators.instance_of(parameter_config.SearchSpace))
+      validator=attr.validators.instance_of(parameter_config.SearchSpace),
+      on_setattr=[attr.setters.convert, attr.setters.validate],
+  )
 
   metric_information: MetricsConfig = attr.ib(
       init=True,
       factory=MetricsConfig,
       converter=MetricsConfig,
       validator=attr.validators.instance_of(MetricsConfig),
-      kw_only=True)
+      on_setattr=[attr.setters.convert, attr.setters.validate],
+      kw_only=True,
+  )
 
   metadata: common.Metadata = attr.field(
       init=True,
       kw_only=True,
       factory=common.Metadata,
-      validator=attr.validators.instance_of(common.Metadata))
+      validator=attr.validators.instance_of(common.Metadata),
+      on_setattr=[attr.setters.convert, attr.setters.validate],
+  )
 
   @property
   def debug_info(self) -> str:
     return ''
 
   @classmethod
   def from_problem(cls: Type[_T], problem: 'ProblemStatement') -> _T:
@@ -335,30 +358,32 @@
     Returns:
       A subclass instance filled with shallow copies of `ProblemStatement`
       fields.
     """
     return cls(
         search_space=problem.search_space,
         metric_information=problem.metric_information,
-        metadata=problem.metadata)
+        metadata=problem.metadata,
+    )
 
   def to_problem(self) -> 'ProblemStatement':
     """Converts to a ProblemStatement which is the parent class of `self`.
 
     Note that this method is useful in subclasses but not so much in
     `ProblemStatement` itself. `ProblemStatement.to_problem` simply generates
     a (shallow) copy of `problem`.
 
     Returns:
       `ProblemStatement` filled with shallow copies of `self.
     """
     return ProblemStatement(
         search_space=self.search_space,
         metric_information=self.metric_information,
-        metadata=self.metadata)
+        metadata=self.metadata,
+    )
 
   @property
   def is_single_objective(self) -> bool:
     """Returns True if only one objective metric is configured."""
     return self.metric_information.is_single_objective
 
   @property
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/shared/base_study_config_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/shared/base_study_config_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/shared/common.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/shared/common.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/shared/common_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/shared/common_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/shared/context.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/shared/context.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/shared/context_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/shared/context_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/shared/parameter_config.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 ExternalType = trial.ExternalType
 ParameterType = trial.ParameterType
 
 
 class ScaleType(enum.Enum):
   """Valid Values for ParameterConfig.scale_type."""
+
   LINEAR = 'LINEAR'
   LOG = 'LOG'
   REVERSE_LOG = 'REVERSE_LOG'
   UNIFORM_DISCRETE = 'UNIFORM_DISCRETE'
 
   def is_nonlinear(self) -> bool:
     return self in [self.LOG, self.REVERSE_LOG]
@@ -49,70 +50,77 @@
 MonotypeParameterSequence = Union[Sequence[Union[int, float]], Sequence[str]]
 MonotypeParameterList = Union[List[Union[int, float]], List[str]]
 
 
 def _validate_bounds(bounds: Union[Tuple[int, int], Tuple[float, float]]):
   """Validates the bounds."""
   if len(bounds) != 2:
-    raise ValueError('Bounds must have length 2. Given: {}'.format(bounds))
+    raise ValueError(f'Bounds must have length 2. Given: {bounds}')
   lower = bounds[0]
   upper = bounds[1]
   if not all([math.isfinite(v) for v in (lower, upper)]):
     raise ValueError(
-        'Both "lower" and "upper" must be finite. Given: (%f, %f)' %
-        (lower, upper))
+        f'Both "lower" and "upper" must be finite. Given: ({lower}, {upper})'
+    )
   if lower > upper:
     raise ValueError(
-        'Lower cannot be greater than upper: given lower={} upper={}'.format(
-            lower, upper))
+        f'Lower cannot be greater than upper: given lower={lower} upper={upper}'
+    )
 
 
 def _get_feasible_points_and_bounds(
-    feasible_values: Sequence[float]
+    feasible_values: Sequence[float],
 ) -> Tuple[List[float], Union[Tuple[int, int], Tuple[float, float]]]:
   """Validates and converts feasible values to floats."""
   if not all([math.isfinite(p) for p in feasible_values]):
-    raise ValueError('Feasible values must all be finite. Given: {}' %
-                     feasible_values)
+    raise ValueError(
+        f'Feasible values must all be finite. Given: {feasible_values}'
+    )
 
   feasible_points = list(sorted(feasible_values))
   bounds = (feasible_points[0], feasible_points[-1])
   return feasible_points, bounds
 
 
 def _get_categories(categories: Sequence[str]) -> List[str]:
   """Returns the categories."""
   return sorted(list(categories))
 
 
 def _get_default_value(
-    param_type: ParameterType,
-    default_value: Union[float, int, str]) -> Union[float, int, str]:
+    param_type: ParameterType, default_value: Union[float, int, str]
+) -> Union[float, int, str]:
   """Validates and converts the default_value to the right type."""
-  if (param_type in (ParameterType.DOUBLE, ParameterType.DISCRETE) and
-      (isinstance(default_value, float) or isinstance(default_value, int))):
+  if param_type in (ParameterType.DOUBLE, ParameterType.DISCRETE) and (
+      isinstance(default_value, float) or isinstance(default_value, int)
+  ):
     return float(default_value)
-  elif (param_type == ParameterType.INTEGER and
-        (isinstance(default_value, float) or isinstance(default_value, int))):
+  elif param_type == ParameterType.INTEGER and (
+      isinstance(default_value, float) or isinstance(default_value, int)
+  ):
     if isinstance(default_value, int):
       return default_value
     else:
       # Check if the float rounds nicely.
       default_int_value = round(default_value)
       if not math.isclose(default_value, default_int_value):
-        raise ValueError('default_value for an INTEGER parameter should be an '
-                         'integer, got float: [{}]'.format(default_value))
+        raise ValueError(
+            'default_value for an INTEGER parameter should be an '
+            f'integer, got float: [{default_value}]'
+        )
       return default_int_value
-  elif (param_type == ParameterType.CATEGORICAL and
-        isinstance(default_value, str)):
+  elif param_type == ParameterType.CATEGORICAL and isinstance(
+      default_value, str
+  ):
     return default_value
   raise ValueError(
-      'default_value has an incorrect type. ParameterType has type {}, '
-      'but default_value has type {}'.format(param_type.name,
-                                             type(default_value)))
+      'default_value has an incorrect type. '
+      f'ParameterType has type {param_type.name}, '
+      f'but default_value has type {type(default_value)}'
+  )
 
 
 #######################
 # Experimental features
 #######################
 class FidelityMode(enum.Enum):
   """Decides how the fidelity config should be interpreated.
@@ -130,90 +138,109 @@
     A high fideltiy Trial's measurements contain lower fidelity evaluations.
     When this is enabled, suggestion models do not use
     Trials' final_measurement. Instead, it reads the measurements whose
     "steps" exactly match one of the fidelities, and treats them as if they
     were separate Trials. Example: Fidelity is the number of total epochs
     to train on.
   """
+
   SEQUENTIAL = 'SEQUENTIAL'
   NOT_SEQUENTIAL = 'NOT_SEQUENTIAL'
   STEPS = 'STEPS'
 
 
 @attr.define
 class FidelityConfig:
   mode: FidelityMode = attr.field(converter=FidelityMode)
   cost_ratio: Sequence[float] = attr.field(
-      converter=tuple, default=tuple(), kw_only=True)
+      converter=tuple, default=tuple(), kw_only=True
+  )
 
 
 ########################
 # Experimental features end here
 ########################
 
 
 @attr.s(auto_attribs=True, frozen=False, init=True, slots=True, eq=True)
 class ParameterConfig:
   """A Vizier ParameterConfig.
 
   Please use ParameterConfig.factory() to create an instance instead of calling
   the constructor directly.
   """
+
   _name: str = attr.ib(
-      init=True, validator=attr.validators.instance_of(str), kw_only=True)
+      init=True, validator=attr.validators.instance_of(str), kw_only=True
+  )
   _type: ParameterType = attr.ib(
       init=True,
       validator=attr.validators.instance_of(ParameterType),
       repr=lambda v: v.name if v is not None else 'None',
-      kw_only=True)
+      kw_only=True,
+  )
   # Only one of _feasible_values, _bounds will be set at any given time.
   _bounds: Optional[Union[Tuple[int, int], Tuple[float, float]]] = attr.ib(
       init=True,
       validator=attr.validators.optional(
           attr.validators.deep_iterable(
               member_validator=attr.validators.instance_of((int, float)),
-              iterable_validator=attr.validators.instance_of(tuple))),
-      kw_only=True)
+              iterable_validator=attr.validators.instance_of(tuple),
+          )
+      ),
+      kw_only=True,
+  )
   _feasible_values: Optional[MonotypeParameterList] = attr.ib(
       init=True,
       validator=attr.validators.optional(
           attr.validators.deep_iterable(
               member_validator=attr.validators.instance_of((int, float, str)),
-              iterable_validator=attr.validators.instance_of((list, tuple)))),
-      kw_only=True)
+              iterable_validator=attr.validators.instance_of((list, tuple)),
+          )
+      ),
+      kw_only=True,
+  )
   _scale_type: Optional[ScaleType] = attr.ib(
       init=True,
       validator=attr.validators.optional(
-          attr.validators.instance_of(ScaleType)),
+          attr.validators.instance_of(ScaleType)
+      ),
       repr=lambda v: v.name if v is not None else 'None',
-      kw_only=True)
+      kw_only=True,
+  )
   _default_value: Optional[Union[float, int, str]] = attr.ib(
       init=True,
       validator=attr.validators.optional(
-          attr.validators.instance_of((float, int, str))),
-      kw_only=True)
+          attr.validators.instance_of((float, int, str))
+      ),
+      kw_only=True,
+  )
   _external_type: ExternalType = attr.ib(
       init=True,
       converter=lambda v: v or ExternalType.INTERNAL,
       validator=attr.validators.optional(
-          attr.validators.instance_of(ExternalType)),
+          attr.validators.instance_of(ExternalType)
+      ),
       repr=lambda v: v.name if v is not None else 'None',
-      kw_only=True)
+      kw_only=True,
+  )
 
   # TODO: Make this a defaultdict and public.
   _children: dict[Union[float, int, str, bool], 'SearchSpace'] = attr.ib(
       init=True,
       factory=dict,
       # For equality checks, drop any empty search spaces.
       eq=lambda d: {k: v for k, v in d.items() if v.parameters},
-      repr=lambda d: json.dumps(d, indent=2, default=repr))
+      repr=lambda d: json.dumps(d, indent=2, default=repr),
+  )
 
   # TODO: Deprecate this field.
   _matching_parent_values: MonotypeParameterSequence = attr.ib(
-      init=True, default=tuple(), kw_only=True, eq=False)
+      init=True, default=tuple(), kw_only=True, eq=False
+  )
 
   # Experimental feature.
   fidelity_config: Optional[FidelityConfig] = attr.ib(
       init=True,
       default=None,
       kw_only=True,
   )
@@ -224,20 +251,21 @@
   @classmethod
   def factory(
       cls,
       name: str,
       *,
       bounds: Optional[Union[Tuple[int, int], Tuple[float, float]]] = None,
       feasible_values: Optional[MonotypeParameterSequence] = None,
-      children: Optional[Sequence[Tuple[MonotypeParameterSequence,
-                                        'ParameterConfig']]] = None,
+      children: Optional[
+          Sequence[Tuple[MonotypeParameterSequence, 'ParameterConfig']]
+      ] = None,
       fidelity_config: Optional[FidelityConfig] = None,
       scale_type: Optional[ScaleType] = None,
       default_value: Optional[Union[float, int, str]] = None,
-      external_type: Optional[ExternalType] = ExternalType.INTERNAL
+      external_type: Optional[ExternalType] = ExternalType.INTERNAL,
   ) -> 'ParameterConfig':
     """Factory method.
 
     Args:
       name: The parameter's name. Cannot be empty.
       bounds: REQUIRED for INTEGER or DOUBLE type. Specifies (min, max). The
         type of (min, max) determines the created ParameterConfig's type.
@@ -267,56 +295,64 @@
     if not name:
       raise ValueError('Parameter name cannot be empty.')
 
     if bool(feasible_values) == bool(bounds):
       raise ValueError(
           'While creating Parameter with name={}: exactly one of '
           '"feasible_values" or "bounds" must be provided, but given '
-          'feasible_values={} and bounds={}.'.format(name, feasible_values,
-                                                     bounds))
+          'feasible_values={} and bounds={}.'.format(
+              name, feasible_values, bounds
+          )
+      )
     if feasible_values:
       if len(set(feasible_values)) != len(feasible_values):
         counter = collections.Counter(feasible_values)
         duplicate_dict = {k: v for k, v in counter.items() if v > 1}
         raise ValueError(
-            'Feasible values cannot have duplicates: {}'.format(duplicate_dict))
+            'Feasible values cannot have duplicates: {}'.format(duplicate_dict)
+        )
       if all(isinstance(v, (float, int)) for v in feasible_values):
         inferred_type = ParameterType.DISCRETE
         feasible_values, bounds = _get_feasible_points_and_bounds(
-            feasible_values)
+            feasible_values
+        )
       elif all(isinstance(v, str) for v in feasible_values):
         inferred_type = ParameterType.CATEGORICAL
         feasible_values = _get_categories(feasible_values)
       else:
         raise ValueError(
             'Feasible values must all be numeric or strings. Given {}'.format(
-                feasible_values))
+                feasible_values
+            )
+        )
     else:  # bounds were specified.
       if isinstance(bounds[0], int) and isinstance(bounds[1], int):
         inferred_type = ParameterType.INTEGER
         _validate_bounds(bounds)
       elif isinstance(bounds[0], float) and isinstance(bounds[1], float):
         inferred_type = ParameterType.DOUBLE
         _validate_bounds(bounds)
       else:
         raise ValueError(
-            'Bounds must both be integers or doubles. Given: {}'.format(bounds))
+            'Bounds must both be integers or doubles. Given: {}'.format(bounds)
+        )
 
     if default_value is not None:
       default_value = _get_default_value(inferred_type, default_value)
 
     pc = cls(
         name=name,
         type=inferred_type,
         bounds=bounds,
         feasible_values=feasible_values,
         scale_type=scale_type,
         default_value=default_value,
         fidelity_config=fidelity_config,
-        external_type=external_type)
+        external_type=external_type,
+    )
     if children:
       pc = pc._add_children(children)
     return pc
 
   @property
   def name(self) -> str:
     return self._name
@@ -333,16 +369,19 @@
   def scale_type(self) -> Optional[ScaleType]:
     return self._scale_type
 
   @property
   def bounds(self) -> Union[Tuple[float, float], Tuple[int, int]]:
     """Returns the bounds, if set, or raises a ValueError."""
     if self.type == ParameterType.CATEGORICAL:
-      raise ValueError('Accessing bounds of a categorical parameter: %s' %
-                       self.name)
+      raise ValueError(
+          'Accessing bounds of a categorical parameter: %s' % self.name
+      )
+    if self._bounds is None:
+      raise ValueError(f'Accessing bounds when not set for {self.name}')
     return self._bounds
 
   @property
   def _child_parameter_configs(self) -> Iterator['ParameterConfig']:
     for subspace in self._children.values():
       for param in subspace.parameters:
         yield param
@@ -391,18 +430,35 @@
     raise ValueError('feasible_values is invalid for type: %s' % self.type)
 
   @property
   def default_value(self) -> Optional[Union[int, float, str]]:
     """Returns the default value, or None if not set."""
     return self._default_value
 
+  @property
+  def deterministic_value(self) -> Optional[Union[int, float, str]]:
+    """Returns the value if ParameterConfig only allows one value."""
+    if self.type in [ParameterType.DOUBLE, ParameterType.INTEGER]:
+      min_val, max_val = self.bounds
+      if min_val == max_val:
+        return trial.ParameterValue(min_val).cast_as_internal(self.type)
+    else:
+      feasible_values = self.feasible_values
+      if len(feasible_values) == 1:
+        return trial.ParameterValue(self.feasible_values[0]).cast_as_internal(
+            self.type
+        )
+    return None
+
   # TODO: TO BE DEPRECATED. Used by factory() only.
   def _add_children(
-      self, new_children: Sequence[Tuple[MonotypeParameterSequence,
-                                         'ParameterConfig']]
+      self,
+      new_children: Sequence[
+          Tuple[MonotypeParameterSequence, 'ParameterConfig']
+      ],
   ) -> 'ParameterConfig':
     """Clones the ParameterConfig and adds new children to it.
 
     Args:
       new_children: A sequence of tuples formatted as: (matching_parent_values,
         ParameterConfig). If the child ParameterConfig have pre-existing parent
         values, they will be overridden.
@@ -416,56 +472,67 @@
     """
     parent = copy.deepcopy(self)
     if not new_children:
       return parent
 
     for child_pair in new_children:
       if len(child_pair) != 2:
-        raise ValueError('Each element in new_children must be a tuple of '
-                         '(Sequence of valid parent values,  ParameterConfig),'
-                         ' given: {}'.format(child_pair))
+        raise ValueError(
+            'Each element in new_children must be a tuple of '
+            '(Sequence of valid parent values,  ParameterConfig),'
+            ' given: {}'.format(child_pair)
+        )
 
     logging.debug('_add_children: new_children=%s', new_children)
     for unsorted_parent_values, child in new_children:
       parent_values = sorted(unsorted_parent_values)
       for parent_value in parent_values:
         parent.subspace(parent_value).add(copy.deepcopy(child))
     return parent
 
   def continuify(self) -> 'ParameterConfig':
     """Returns a newly created DOUBLE parameter with the same range."""
     if self.type == ParameterType.DOUBLE:
       return copy.deepcopy(self)
     elif not self.type.is_numeric():
       raise ValueError(
-          'Cannot convert a non-numeric parameter to DOUBLE: {}'.format(self))
+          'Cannot convert a non-numeric parameter to DOUBLE: {}'.format(self)
+      )
     elif list(self._child_parameter_configs):
       raise ValueError(
-          'Cannot convert a parent parameter to DOUBLE: {}'.format(self))
+          'Cannot convert a parent parameter to DOUBLE: {}'.format(self)
+      )
 
     scale_type = self.scale_type
     if scale_type == ScaleType.UNIFORM_DISCRETE:
       logging.log_every_n(
           logging.WARNING,
-          'Converting a UNIFORM_DISCRETE scaled discrete parameter '
-          'to DOUBLE: %s', 10, self)
+          (
+              'Converting a UNIFORM_DISCRETE scaled discrete parameter '
+              'to DOUBLE: %s'
+          ),
+          10,
+          self,
+      )
       scale_type = None
 
     default_value = self.default_value
     if default_value is not None:
       default_value = float(default_value)
     return ParameterConfig.factory(
         self.name,
         bounds=(float(self.bounds[0]), float(self.bounds[1])),
         scale_type=scale_type,
-        default_value=default_value)
+        default_value=default_value,
+    )
 
   @classmethod
-  def merge(cls, one: 'ParameterConfig',
-            other: 'ParameterConfig') -> 'ParameterConfig':
+  def merge(
+      cls, one: 'ParameterConfig', other: 'ParameterConfig'
+  ) -> 'ParameterConfig':
     """Merge two ParameterConfigs.
 
     Args:
       one: ParameterConfig with no child parameters.
       other: Must have the same type as one, and may not have child parameters.
 
     Returns:
@@ -476,42 +543,54 @@
 
     Raises:
       ValueError: If any of the input configs has child parameters, or if
         the two parameters have different types.
     """
     if one.child_parameter_configs or other.child_parameter_configs:
       raise ValueError(
-          'Cannot merge parameters with child_parameter_configs: %s and %s' %
-          one, other)
+          'Cannot merge parameters with child_parameter_configs: %s and %s'
+          % one,
+          other,
+      )
     if one.type != other.type:
-      raise ValueError('Type conflicts between {} and {}'.format(
-          one.type.name, other.type.name))
+      raise ValueError(
+          'Type conflicts between {} and {}'.format(
+              one.type.name, other.type.name
+          )
+      )
     if one.scale_type != other.scale_type:
-      logging.warning('Scale type conflicts while merging %s and %s', one,
-                      other)
+      logging.warning(
+          'Scale type conflicts while merging %s and %s', one, other
+      )
 
     if one.type in (ParameterType.CATEGORICAL, ParameterType.DISCRETE):
       new_feasible_values = list(
-          set(one.feasible_values + other.feasible_values))
+          set(one.feasible_values + other.feasible_values)
+      )
       return ParameterConfig.factory(
           name=one.name,
           feasible_values=new_feasible_values,
-          scale_type=one.scale_type)
+          scale_type=one.scale_type,
+      )
     elif one.type in (ParameterType.INTEGER, ParameterType.DOUBLE):
       original_min, original_max = one.bounds
       other_min, other_max = other.bounds
       new_bounds = (min(original_min, other_min), max(original_max, other_max))
       return ParameterConfig.factory(
-          name=one.name, bounds=new_bounds, scale_type=one.scale_type)
-    raise ValueError('Unknown type {}. This is currently'
-                     'an unreachable code.'.format(one.type))
+          name=one.name, bounds=new_bounds, scale_type=one.scale_type
+      )
+    raise ValueError(
+        'Unknown type {}. This is currentlyan unreachable code.'.format(
+            one.type
+        )
+    )
 
   def traverse(
-      self,
-      show_children: bool = False) -> Generator['ParameterConfig', None, None]:
+      self, show_children: bool = False
+  ) -> Generator['ParameterConfig', None, None]:
     """DFS Generator for parameter configs.
 
     Args:
       show_children: If True, every generated ParameterConfig has
         child_parameter_configs. For example, if 'foo' has two child configs
         'bar1' and 'bar2', then traversing 'foo' with show_children=True
         generates (foo, with bar1,bar2 as children), (bar1), and (bar2). If
@@ -526,16 +605,16 @@
     else:
       yield self.clone_without_children
     for child in self.child_parameter_configs:
       yield from child.traverse(show_children)
 
   # TODO: Rename to `validate_value or is_feasible`
   def contains(
-      self, value: Union[trial.ParameterValueTypes,
-                         trial.ParameterValue]) -> bool:
+      self, value: Union[trial.ParameterValueTypes, trial.ParameterValue]
+  ) -> bool:
     """Check if the `value` is a valid value for this parameter config."""
     if isinstance(value, trial.ParameterValue):
       # TODO: Extract the raw value.
       value = value.value
     try:
       self._assert_feasible(value)
     except (TypeError, ValueError):
@@ -549,23 +628,27 @@
     elif self.type == ParameterType.INTEGER:
       return self.bounds[1] - self.bounds[0] + 1
     else:
       return len(self.feasible_values)
 
   def _assert_bounds(self, value: trial.ParameterValueTypes) -> None:
     if not self.bounds[0] <= value <= self.bounds[1]:
-      raise ValueError(f'Parameter {self.name} has bounds: {self.bounds}. '
-                       f'Given: {value}')
+      raise ValueError(
+          f'Parameter {self.name} has bounds: {self.bounds}. Given: {value}'
+      )
 
-  def _assert_in_feasible_values(self,
-                                 value: trial.ParameterValueTypes) -> None:
+  def _assert_in_feasible_values(
+      self, value: trial.ParameterValueTypes
+  ) -> None:
     if value not in self._feasible_values:
-      raise ValueError(f'Parameter {self.name} has feasible values: '
-                       f'{self.feasible_values}. '
-                       f'Given: {value}')
+      raise ValueError(
+          f'Parameter {self.name} has feasible values: '
+          f'{self.feasible_values}. '
+          f'Given: {value}'
+      )
 
   def _assert_feasible(self, value: trial.ParameterValueTypes) -> None:
     """Asserts that the value is feasible for this parameter config.
 
     Args:
       value:
 
@@ -574,30 +657,32 @@
       ValueError: Value is not feasible.
       RuntimeError: Other errors.
     """
     try:
       self.type.assert_correct_type(value)
     except TypeError as e:
       raise TypeError(
-          f'Parameter {self.name} is not compatible with value: {value}') from e
+          f'Parameter {self.name} is not compatible with value: {value}'
+      ) from e
 
     # TODO: We should be able to directly use "value" without
     # casting to the internal type.
     value = trial.ParameterValue(value)
     if self.type == ParameterType.DOUBLE:
       self._assert_bounds(value.as_float)
     elif self.type == ParameterType.INTEGER:
       self._assert_bounds(value.as_int)
     elif self.type == ParameterType.DISCRETE:
       self._assert_in_feasible_values(value.as_float)
     elif self.type == ParameterType.CATEGORICAL:
       self._assert_in_feasible_values(value.as_str)
     else:
       raise RuntimeError(
-          f'Parameter {self.name} has unknown parameter type: {self.type}')
+          f'Parameter {self.name} has unknown parameter type: {self.type}'
+      )
 
   def get_subspace_deepcopy(self, value: ParameterValueTypes) -> 'SearchSpace':
     """Get a deep copy of the subspace.
 
     Validates the feasibility of value.
 
     Args:
@@ -642,16 +727,17 @@
 
   def __init__(self, selected: ParameterConfigOrConfigs):
     if isinstance(selected, Collection):
       self.__attrs_init__(tuple(selected))
     else:
       self.__attrs_init__(tuple([selected]))
 
-  def select_values(self,
-                    values: MonotypeParameterSequence) -> 'SearchSpaceSelector':
+  def select_values(
+      self, values: MonotypeParameterSequence
+  ) -> 'SearchSpaceSelector':
     """Select values."""
     values = tuple(values)
 
     for value in values:
       for config in self._selected:
         if not config.contains(value):
           # Validate first so we don't create a lot of unnecessary empty
@@ -687,22 +773,24 @@
 
   def __init__(self, selected: SearchSpaceOrSpaces):
     if isinstance(selected, Collection):
       self.__attrs_init__(tuple(selected))
     else:
       self.__attrs_init__(tuple([selected]))
 
-  def add_float_param(self,
-                      name: str,
-                      min_value: float,
-                      max_value: float,
-                      *,
-                      default_value: Optional[float] = None,
-                      scale_type: Optional[ScaleType] = ScaleType.LINEAR,
-                      index: Optional[int] = None) -> 'ParameterConfigSelector':
+  def add_float_param(
+      self,
+      name: str,
+      min_value: float,
+      max_value: float,
+      *,
+      default_value: Optional[float] = None,
+      scale_type: Optional[ScaleType] = None,
+      index: Optional[int] = None,
+  ) -> 'ParameterConfigSelector':
     """Adds floating point parameter config(s) to the selected search space(s).
 
     Args:
       name: The parameter's name. Cannot be empty.
       min_value: Inclusive lower bound for the parameter.
       max_value: Inclusive upper bound for the parameter.
       default_value: A default value for the Parameter.
@@ -715,24 +803,27 @@
       SearchSpaceSelector(s) for the newly added parameter(s):
       One SearchSpaceSelector if one parameter was added, or a list of
       SearchSpaceSelector if multiple parameters were added.
 
     Raises:
       ValueError: If `index` is invalid (e.g. negative).
     """
+    if scale_type is None:
+      scale_type = ScaleType.LINEAR
     bounds = (float(min_value), float(max_value))
     param_names = self._get_parameter_names_to_create(name=name, index=index)
 
     new_params = []
     for param_name in param_names:
       new_pc = ParameterConfig.factory(
           name=param_name,
           bounds=bounds,
           scale_type=scale_type,
-          default_value=default_value)
+          default_value=default_value,
+      )
       new_params.append(new_pc)
     return self._add_parameters(new_params)
 
   def add_int_param(
       self,
       name: str,
       min_value: int,
@@ -761,32 +852,37 @@
 
     Raises:
       ValueError: If min_value or max_value are not integers.
       ValueError: If `index` is invalid (e.g. negative).
     """
     int_min_value = int(min_value)
     if not math.isclose(min_value, int_min_value):
-      raise ValueError('min_value for an INTEGER parameter should be an integer'
-                       ', got: [{}]'.format(min_value))
+      raise ValueError(
+          'min_value for an INTEGER parameter should be an integer'
+          ', got: [{}]'.format(min_value)
+      )
     int_max_value = int(max_value)
     if not math.isclose(max_value, int_max_value):
-      raise ValueError('max_value for an INTEGER parameter should be an integer'
-                       ', got: [{}]'.format(min_value))
+      raise ValueError(
+          'max_value for an INTEGER parameter should be an integer'
+          ', got: [{}]'.format(min_value)
+      )
     bounds = (int_min_value, int_max_value)
 
     param_names = self._get_parameter_names_to_create(name=name, index=index)
 
     new_params = []
     for param_name in param_names:
       new_pc = ParameterConfig.factory(
           name=param_name,
           bounds=bounds,
           scale_type=scale_type,
           fidelity_config=experimental_fidelity_config,
-          default_value=default_value)
+          default_value=default_value,
+      )
       new_params.append(new_pc)
     return self._add_parameters(new_params)
 
   def add_discrete_param(
       self,
       name: str,
       feasible_values: Union[Sequence[float], Sequence[int]],
@@ -838,26 +934,28 @@
     for param_name in param_names:
       new_pc = ParameterConfig.factory(
           name=param_name,
           feasible_values=sorted(feasible_values),
           scale_type=scale_type,
           fidelity_config=experimental_fidelity_config,
           default_value=default_value,
-          external_type=external_type)
+          external_type=external_type,
+      )
       new_params.append(new_pc)
     return self._add_parameters(new_params)
 
   def add_categorical_param(
       self,
       name: str,
       feasible_values: Sequence[str],
       *,
       default_value: Optional[str] = None,
       scale_type: Optional[ScaleType] = None,
-      index: Optional[int] = None) -> 'ParameterConfigSelector':
+      index: Optional[int] = None,
+  ) -> 'ParameterConfigSelector':
     """Adds string-valued parameter config(s) to the selected search space(s).
 
     IMPORTANT: If a parameter is categorical, its values are assumed to be
     unordered. If the `feasible_values` have ordering, use add_discrete_param()
     above, since it will improve Vizier's model quality.
 
     Args:
@@ -879,25 +977,28 @@
 
     new_params = []
     for param_name in param_names:
       new_pc = ParameterConfig.factory(
           name=param_name,
           feasible_values=sorted(feasible_values),
           scale_type=scale_type,
-          default_value=default_value)
+          default_value=default_value,
+      )
       new_params.append(new_pc)
     return self._add_parameters(new_params)
 
-  def add_bool_param(self,
-                     name: str,
-                     feasible_values: Optional[Sequence[bool]] = None,
-                     *,
-                     default_value: Optional[bool] = None,
-                     scale_type: Optional[ScaleType] = None,
-                     index: Optional[int] = None) -> 'ParameterConfigSelector':
+  def add_bool_param(
+      self,
+      name: str,
+      feasible_values: Optional[Sequence[bool]] = None,
+      *,
+      default_value: Optional[bool] = None,
+      scale_type: Optional[ScaleType] = None,
+      index: Optional[int] = None,
+  ) -> 'ParameterConfigSelector':
     """Adds boolean-valued parameter config(s) to the selected search space(s).
 
     Args:
       name: The parameter's name. Cannot be empty.
       feasible_values: An optional list of feasible boolean values, i.e. one of
         the following: [True], [False], [True, False], [False, True].
       default_value: A default value for the Parameter.
@@ -910,18 +1011,22 @@
       ParameterConfigSelector for the newly added parameter(s).
 
     Raises:
       ValueError: If `feasible_values` has invalid values.
       ValueError: If `index` is invalid (e.g. negative).
     """
     allowed_values = (None, (True, False), (False, True), (True,), (False,))
-    if feasible_values is not None and tuple(
-        feasible_values) not in allowed_values:
-      raise ValueError('feasible_values must be one of %s; got: %s.' %
-                       (allowed_values, feasible_values))
+    if (
+        feasible_values is not None
+        and tuple(feasible_values) not in allowed_values
+    ):
+      raise ValueError(
+          'feasible_values must be one of %s; got: %s.'
+          % (allowed_values, feasible_values)
+      )
     # Boolean parameters are represented as categorical parameters internally.
     bool_to_string = lambda x: trial.TRUE_VALUE if x else trial.FALSE_VALUE
     if feasible_values is None:
       categories = (trial.TRUE_VALUE, trial.FALSE_VALUE)
     else:
       categories = [bool_to_string(x) for x in feasible_values]
     feasible_values = sorted(categories, reverse=True)
@@ -934,35 +1039,38 @@
     new_params = []
     for param_name in param_names:
       new_pc = ParameterConfig.factory(
           name=param_name,
           feasible_values=sorted(feasible_values),
           scale_type=scale_type,
           default_value=default_value,
-          external_type=ExternalType.BOOLEAN)
+          external_type=ExternalType.BOOLEAN,
+      )
       new_params.append(new_pc)
     return self._add_parameters(new_params)
 
   @overload
   def select(
       self,
       parameter_name: str,
       parameter_values: None,
   ) -> ParameterConfigSelector:
     ...
 
   @overload
   def select(
-      self, parameter_name: str,
-      parameter_values: MonotypeParameterSequence) -> 'SearchSpaceSelector':
+      self, parameter_name: str, parameter_values: MonotypeParameterSequence
+  ) -> 'SearchSpaceSelector':
     ...
 
-  def select(self,
-             parameter_name,
-             parameter_values: Optional[MonotypeParameterSequence] = None):
+  def select(
+      self,
+      parameter_name,
+      parameter_values: Optional[MonotypeParameterSequence] = None,
+  ):
     """Selects a parameter config or its subspace.
 
     This method is for constructing a _conditional_ search space.
 
     EXAMPLE: Suppose we have a selector to the root of the search space with one
     categorical parameter.
     root = pyvizier.SearchSpace().root
@@ -1008,19 +1116,21 @@
       for space in self._selected:
         selected_parameter = space.get(parameter_name)
         for value in parameter_values:
           selected_spaces.append(selected_parameter.subspace(value))
       return SearchSpaceSelector(selected_spaces)
 
   @classmethod
-  def _get_parameter_names_to_create(cls,
-                                     *,
-                                     name: str,
-                                     length: Optional[int] = None,
-                                     index: Optional[int] = None) -> List[str]:
+  def _get_parameter_names_to_create(
+      cls,
+      *,
+      name: str,
+      length: Optional[int] = None,
+      index: Optional[int] = None,
+  ) -> List[str]:
     """Returns the names of all parameters which should be created.
 
     Args:
       name: The base parameter name.
       length: Specifies the length of a multi-dimensional parameters. If larger
         than 1, then multiple ParameterConfigs are added. E.g. if name='rate'
         and length=2, then two ParameterConfigs with names 'rate[0]', 'rate[1]'
@@ -1032,16 +1142,18 @@
     Returns:
       List of parameter names to create.
 
     Raises:
       ValueError: If `length` or `index` are invalid.
     """
     if length is not None and index is not None:
-      raise ValueError('Only one of `length` and `index` can be specified. Got'
-                       ' length={}, index={}'.format(length, index))
+      raise ValueError(
+          'Only one of `length` and `index` can be specified. Got'
+          ' length={}, index={}'.format(length, index)
+      )
     if length is not None and length < 1:
       raise ValueError('length must be >= 1. Got length={}'.format(length))
     if index is not None and index < 0:
       raise ValueError('index must be >= 0. Got index={}'.format(index))
 
     param_names = []
     if length is None and index is None:
@@ -1061,15 +1173,16 @@
   @classmethod
   def _multi_dimensional_parameter_name(cls, name: str, index: int) -> str:
     """Returns the indexed parameter name."""
     return '{}[{}]'.format(name, index)
 
   @classmethod
   def parse_multi_dimensional_parameter_name(
-      cls, name: str) -> Optional[Tuple[str, int]]:
+      cls, name: str
+  ) -> Optional[Tuple[str, int]]:
     """Returns the base name for a multi-dimensional parameter name.
 
     Args:
       name: A parameter name.
 
     Returns:
       (base_name, index): if name='hidden_units[10]', base_name='hidden_units'
@@ -1081,25 +1194,29 @@
     matches = pattern.match(name)
     if matches is None:
       return None
     return (matches.groupdict()['name'], int(matches.groupdict()['index']))
 
   # TODO: Add def extend(space: SearchSpace)
   def _add_parameters(
-      self, parameters: List[ParameterConfig]) -> ParameterConfigSelector:
+      self, parameters: List[ParameterConfig]
+  ) -> ParameterConfigSelector:
     """Adds deepcopy of the ParameterConfigs.
 
     Args:
       parameters: The parameters to add to the search space.
 
     Returns:
       A list of SearchSpaceSelectors, one for each parameters added.
     """
-    logging.info('Adding child parameters %s to %s subspaces ',
-                 set(p.name for p in parameters), len(self._selected))
+    logging.info(
+        'Adding child parameters %s to %s subspaces ',
+        set(p.name for p in parameters),
+        len(self._selected),
+    )
     added = []
     for parameter in parameters:
       for selected in self._selected:
         # Adds a deepcopy so that every ParameterConfig object is unique.
         added.append(selected.add(copy.deepcopy(parameter)))
 
     return ParameterConfigSelector(added)
@@ -1111,38 +1228,39 @@
 
   Vizier search space can be *conditional*.
   Parameter names are guaranteed to be unique in any subspace.
 
   Attribute:
     _parameter_configs: Maps parameter names to configs.
   """
+
   _parameter_configs: dict[str, ParameterConfig] = attr.field(
-      init=False, factory=dict)
+      init=False, factory=dict
+  )
 
   # TODO: To be deprecated.
   _parent_values: MonotypeParameterSequence = attr.field(
-      default=tuple(), converter=tuple, kw_only=True)
+      default=tuple(), converter=tuple, kw_only=True
+  )
 
   @property
   def parameter_names(self) -> AbstractSet[str]:
     return self._parameter_configs.keys()
 
   def get(self, name: str) -> ParameterConfig:
     if name not in self._parameter_configs:
       raise KeyError(f'{name} is not in the search space.')
     return self._parameter_configs[name]
 
   def pop(self, name: str) -> ParameterConfig:
     return self._parameter_configs.pop(name)
 
-  def add(self,
-          parameter_config: ParameterConfig,
-         
-          *,
-          replace: bool = False) -> ParameterConfig:
+  def add(
+      self, parameter_config: ParameterConfig, *, replace: bool = False
+  ) -> ParameterConfig:
     """Adds the ParameterConfig.
 
     For advanced users only. Takes a reference to Parameterconfig.
     Future edits will change the search space.
 
     Args:
       parameter_config:
@@ -1155,15 +1273,16 @@
     """
     name = parameter_config.name
     parameter_config._matching_parent_values = tuple(self._parent_values)  # pylint: disable=protected-access
     if (name in self._parameter_configs) and (not replace):
       raise ValueError(
           f'Duplicate name: {parameter_config.name} already exists.\n'
           f'Existing config: {parameter_config}\n'
-          f'New config:{parameter_config}')
+          f'New config:{parameter_config}'
+      )
 
     self._parameter_configs[name] = parameter_config
     return parameter_config
 
   # TODO: Change the return type to Iterator.
   @property
   def parameters(self) -> list[ParameterConfig]:
@@ -1220,15 +1339,16 @@
           f' {set2 - set1}. Missing in parameters: {set1 - set2}.'
       )
     for pc in self._parameter_configs.values():
       if pc.name not in parameters:
         raise InvalidParameterError(f'{pc.name} is missing in {parameters}.')
       elif not pc.contains(parameters[pc.name]):
         raise InvalidParameterError(
-            f'{parameters[pc.name]} is not feasible in {pc}')
+            f'{parameters[pc.name]} is not feasible in {pc}'
+        )
     return True
 
   def num_parameters(self, param_type: Optional[ParameterType] = None) -> int:
     """Counts number of parameters with the param_type (if given)."""
     if param_type is None:
       return len(self.parameters)
     return [pc.type for pc in self.parameters].count(param_type)
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/shared/parameter_config_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_config_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,14 +273,39 @@
   @parameterized.parameters((True, True), ('a', False), (0, False))
   def testBoolean(self, value: Any, expected: bool):
     config = pc.ParameterConfig.factory(
         'pc1', feasible_values=[trial.TRUE_VALUE, trial.FALSE_VALUE])
     self.assertEqual(config.contains(value), expected)
 
 
+class ParameterConfigPropertyTest(parameterized.TestCase):
+
+  @parameterized.parameters(
+      ((-1.0, 1.0), None), ((-1, 1), None), ((-2.0, -2.0), -2.0), ((-2, -2), -2)
+  )
+  def testFloatandInt(self, bounds: Any, expected: Any):
+    config = pc.ParameterConfig.factory('pc1', bounds=bounds)
+    value = config.deterministic_value
+    if expected is None:
+      self.assertIsNone(value)
+    else:
+      self.assertEqual(value, expected)
+
+  @parameterized.parameters(
+      ([-1.0, 2.0], None), ([-1.0], -1.0), (['a', 'b'], None), (['a'], 'a')
+  )
+  def testDiscreteandCategorical(self, feasible_values: Any, expected: Any):
+    config = pc.ParameterConfig.factory('pc1', feasible_values=feasible_values)
+    value = config.deterministic_value
+    if expected is None:
+      self.assertIsNone(value)
+    else:
+      self.assertEqual(value, expected)
+
+
 class TraverseTest(parameterized.TestCase):
 
   @parameterized.named_parameters(('ShowChildrenTrue', True),
                                   ('ShowChildrenFalse', False))
   def testTraverse(self, show_children):
     grandchild1 = pc.ParameterConfig.factory('grandchild1', bounds=(-1.0, 1.0))
     grandchildren = [(['a'], grandchild1), (['b'], grandchild1)]
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/shared/parameter_iterators.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_iterators.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/shared/parameter_iterators_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/shared/parameter_iterators_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/shared/trial.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/shared/trial.py`

 * *Files 3% similar despite different names*

```diff
@@ -265,15 +265,35 @@
       self.data.__setitem__(key, value)
     else:
       self.data.__setitem__(key, Metric(value=value))
 
 
 @attr.s(auto_attribs=True, frozen=False, init=True, slots=True)
 class Measurement:
-  """Collection of metrics with a timestamp."""
+  """A collection of metrics with a timestamp & checkpoint.
+
+  metrics: Named, floating-point metrics.  A typical example would be the
+    accuracy of a machine-learning model.  Typically, all the metrics mentioned
+    in the MetricInformation class would be listed here; other metrics may be
+    listed but would not normally be used by Vizier.
+
+  elapsed_secs: (optional) The length of time it took to evaluate the Trial to
+    reach this Measurement, in seconds.  This may be used by some Vizier
+    algorithms.
+
+  steps: (optional)  A positive integer roughly proportional to the amount of
+    work spent.  When training a ML system, often this is a count of training
+    steps/epochs.  When supplied, $steps should be consistent with the order of
+    Measurements, but they need not be consecutive values.
+
+  checkpoint_path: (optional) A slash-separated pathname.  Typically used when
+    training a ML model; it would normally be a pathname for the checkpoint that
+    produced the Measurement.  Implementations may limit the length of this
+    string, but at least 2048 bytes will be allowed.
+  """
 
   def _value_is_finite(self, _, value):
     if not (np.isfinite(value) and value >= 0):
       raise ValueError('Must be finite and non-negative.')
 
   # Should be used as a regular Dict.
   metrics: _MetricDict = attr.ib(
@@ -296,14 +316,21 @@
       converter=int,
       init=True,
       default=0,
       validator=[attr.validators.instance_of(int), _value_is_finite],
       on_setattr=[attr.setters.convert, attr.setters.validate],
       kw_only=True)
 
+  checkpoint_path: str = attr.ib(
+      init=True,
+      default='',
+      validator=[attr.validators.instance_of(str)],
+      kw_only=True,
+  )
+
 
 def _to_local_time(
     dt: Optional[datetime.datetime]) -> Optional[datetime.datetime]:
   """Converter for initializing timestamps in Trial class."""
   return dt.astimezone() if dt else None
 
 
@@ -472,20 +499,21 @@
       validator=attr.validators.deep_iterable(
           member_validator=attr.validators.instance_of(Measurement),
           iterable_validator=attr.validators.instance_of(list)),
   )
 
   creation_time: Optional[datetime.datetime] = attr.ib(
       init=True,
-      default=datetime.datetime.now(),
+      factory=datetime.datetime.now,
       converter=_to_local_time,
       kw_only=True,
       repr=lambda v: v.strftime('%x %X') if v is not None else 'None',
       validator=attr.validators.optional(
-          attr.validators.instance_of(datetime.datetime)),
+          attr.validators.instance_of(datetime.datetime)
+      ),
   )
 
   completion_time: Optional[datetime.datetime] = attr.ib(
       init=True,
       kw_only=True,
       default=None,
       repr=lambda v: v.strftime('%x %X') if v is not None else 'None',
```

### Comparing `google-vizier-0.1.4/vizier/_src/pyvizier/shared/trial_test.py` & `google-vizier-0.1.5/vizier/_src/pyvizier/shared/trial_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,19 @@
   def testDefaultsNotShared(self):
     """Make sure default parameters are not shared between instances."""
     trial1 = trial.Trial()
     trial2 = trial.Trial()
     trial1.parameters['x1'] = trial.ParameterValue(5)
     self.assertEmpty(trial2.parameters)
 
+  def testCreationTime(self):
+    trial1 = trial.Trial()
+    trial2 = trial.Trial()
+    self.assertGreater(trial2.creation_time, trial1.creation_time)
+
 
 class ParameterDictTest(parameterized.TestCase):
 
   @parameterized.parameters((True,), (3,), (1.,), ('aa',))
   def testAssignRawValue(self, v):
     d = trial.ParameterDict()
     d['p1'] = v
```

### Comparing `google-vizier-0.1.4/vizier/algorithms/__init__.py` & `google-vizier-0.1.5/vizier/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/algorithms/designers/__init__.py` & `google-vizier-0.1.5/vizier/algorithms/designers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/algorithms/policies/__init__.py` & `google-vizier-0.1.5/vizier/algorithms/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/benchmarks/__init__.py` & `google-vizier-0.1.5/vizier/benchmarks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,22 @@
 
 from __future__ import annotations
 
 """Benchmarking utilities."""
 from vizier._src.benchmarks.analyzers.convergence_curve import ConvergenceCurve
 from vizier._src.benchmarks.analyzers.convergence_curve import ConvergenceCurveComparator
 from vizier._src.benchmarks.analyzers.convergence_curve import ConvergenceCurveConverter
+from vizier._src.benchmarks.analyzers.convergence_curve import HypervolumeCurveConverter
+from vizier._src.benchmarks.analyzers.state_analyzer import BenchmarkStateAnalyzer
 from vizier._src.benchmarks.runners.benchmark_runner import BenchmarkRunner
 from vizier._src.benchmarks.runners.benchmark_runner import BenchmarkSubroutine
 from vizier._src.benchmarks.runners.benchmark_runner import EvaluateActiveTrials
+from vizier._src.benchmarks.runners.benchmark_runner import FillActiveTrials
 from vizier._src.benchmarks.runners.benchmark_runner import GenerateAndEvaluate
 from vizier._src.benchmarks.runners.benchmark_runner import GenerateSuggestions
 from vizier._src.benchmarks.runners.benchmark_state import BenchmarkState
 from vizier._src.benchmarks.runners.benchmark_state import BenchmarkStateFactory
 from vizier._src.benchmarks.runners.benchmark_state import DesignerBenchmarkStateFactory
+from vizier._src.benchmarks.runners.benchmark_state import ExperimenterDesignerBenchmarkStateFactory
 from vizier._src.benchmarks.runners.benchmark_state import PolicyBenchmarkStateFactory
 from vizier._src.benchmarks.runners.benchmark_state import PolicySuggester
 from vizier._src.benchmarks.runners.benchmark_state import SeededPolicyFactory
```

### Comparing `google-vizier-0.1.4/vizier/benchmarks/experimenters/__init__.py` & `google-vizier-0.1.5/vizier/benchmarks/experimenters/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,24 +11,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Lightweight experimenters."""
+
 from vizier._src.benchmarks.experimenters.combo_experimenter import CentroidExperimenter
 from vizier._src.benchmarks.experimenters.combo_experimenter import ContaminationExperimenter
 from vizier._src.benchmarks.experimenters.combo_experimenter import IsingExperimenter
 from vizier._src.benchmarks.experimenters.combo_experimenter import MAXSATExperimenter
 from vizier._src.benchmarks.experimenters.combo_experimenter import PestControlExperimenter
 from vizier._src.benchmarks.experimenters.discretizing_experimenter import DiscretizingExperimenter
 from vizier._src.benchmarks.experimenters.experimenter import Experimenter
 from vizier._src.benchmarks.experimenters.experimenter_factory import BBOBExperimenterFactory
+from vizier._src.benchmarks.experimenters.experimenter_factory import ExperimenterFactory
 from vizier._src.benchmarks.experimenters.experimenter_factory import SingleObjectiveExperimenterFactory
 from vizier._src.benchmarks.experimenters.l1_categorical_experimenter import L1CategorialExperimenter
+from vizier._src.benchmarks.experimenters.multiobjective_experimenter import MultiObjectiveExperimenter
 from vizier._src.benchmarks.experimenters.noisy_experimenter import NoisyExperimenter
 from vizier._src.benchmarks.experimenters.normalizing_experimenter import NormalizingExperimenter
 from vizier._src.benchmarks.experimenters.numpy_experimenter import NumpyExperimenter
 from vizier._src.benchmarks.experimenters.shifting_experimenter import ShiftingExperimenter
 from vizier._src.benchmarks.experimenters.sign_flip_experimenter import SignFlipExperimenter
 from vizier._src.benchmarks.experimenters.sparse_experimenter import SparseExperimenter
+from vizier._src.benchmarks.experimenters.surrogate_experimenter import PredictorExperimenter
 from vizier._src.benchmarks.experimenters.synthetic import bbob
```

### Comparing `google-vizier-0.1.4/vizier/benchmarks/experimenters/hpo/__init__.py` & `google-vizier-0.1.5/vizier/benchmarks/experimenters/hpo/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/benchmarks/experimenters/nas/__init__.py` & `google-vizier-0.1.5/vizier/benchmarks/experimenters/nas/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/benchmarks/experimenters/rl/__init__.py` & `google-vizier-0.1.5/vizier/benchmarks/experimenters/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/client/__init__.py` & `google-vizier-0.1.5/vizier/client/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/client/client_abc.py` & `google-vizier-0.1.5/vizier/client/client_abc.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/client/client_abc_testing.py` & `google-vizier-0.1.5/vizier/client/client_abc_testing.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/interfaces/__init__.py` & `google-vizier-0.1.5/vizier/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/interfaces/serializable.py` & `google-vizier-0.1.5/vizier/interfaces/serializable.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/jax/__init__.py` & `google-vizier-0.1.5/vizier/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/jax/models.py` & `google-vizier-0.1.5/vizier/jax/models.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/jax/optimizers.py` & `google-vizier-0.1.5/vizier/jax/optimizers.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/pyglove/__init__.py` & `google-vizier-0.1.5/vizier/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/pyglove/pyglove_test.py` & `google-vizier-0.1.5/vizier/_src/pyglove/e2e_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,26 +10,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-"""Tests for Vizier backend for PyGlove."""
+"""End-to-end tests for Vizier backend for PyGlove."""
 
 import pyglove as pg
-from vizier import pyglove as pg_vizier
+from vizier._src.pyglove import oss_vizier
+from vizier._src.service import clients as pyvizier_clients
 from absl.testing import absltest
 
 
+pyvizier_clients.environment_variables.servicer_use_sql_ram()
+
+
 class PygloveTest(absltest.TestCase):
   """Tests for using Vizier as PyGlove backend."""
 
   def test_sample(self):
-    pg_vizier.init('my_study')
+    oss_vizier.init('my_study')
 
     examples = []
     for x, f in pg.sample(
         pg.oneof([1, 2, 3]), pg.geno.Random(seed=1), num_examples=3
     ):
       f(x)
       examples.append(x)
```

### Comparing `google-vizier-0.1.4/vizier/pythia.py` & `google-vizier-0.1.5/vizier/pythia.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/pyvizier/__init__.py` & `google-vizier-0.1.5/vizier/pyvizier/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/pyvizier/converters/__init__.py` & `google-vizier-0.1.5/vizier/pyvizier/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/pyvizier/converters/core.py` & `google-vizier-0.1.5/vizier/pyvizier/converters/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,29 +90,30 @@
   extra information specific to vizier.
 
   If `type` is `DOUBLE`, then `dtype` is a floating type, and bounds are
   floating numbers. num_dimensions is always 1, and num_oovs is zero.
 
   If 'type' is `DISCRETE`, then `dtype` is an integer type, and bounds are
   integers. num_dimensions is always 1. Suppose `bounds=(x,y)`. Then integers
-  x to (y-num_oovs) correspond to valid parameter values. The rest represent
-  out-of-vocabulary values. For example, an integer parameter in range (1,3)
-  can be represented by a DISCRETE NumpyArraySpec with bounds=(1,4) and oov=1.
+  x to-and-including (y-num_oovs) correspond to valid parameter values. The rest
+  represent out-of-vocabulary values. For example, an integer parameter in
+  the range 1 <= x <= 3 can be represented by a DISCRETE NumpyArraySpec with
+  bounds=(1,4) and oov=1.
 
   If 'type' is `ONEHOT_EMBEDDING`, then `dtype` is a floating type, and bounds
-  are floating numbers. Suppose num_dimensions is X.
+  are floating numbers. In this case, the output array can have multiple
+  columns.
 
   Attributes:
     type: Underlying type of the Vizier parameter corresponding to the array.
-    dtype: Numpy array's type.
+    dtype: The numpy array's type.
     bounds: Always inclusive in both directions.
     num_dimensions: Corresponds to shape[-1] of the numpy array. When `type` is
       `ONEHOT_EMBEDDING`, the first X dimensions correspond to valid parameter
       values. The other dimensions correspond to out-of-vocabulary values.
-      Otherwise, it is simply 1.
     name: Parameter name.
     num_oovs: Number of out-of-vocabulary items, for non-continuous type.
     scale: Scaling of the values.
   """
 
   type: NumpyArraySpecType
   dtype: np.dtype
@@ -130,16 +131,16 @@
   @classmethod
   def from_parameter_config(
       cls,
       pc: pyvizier.ParameterConfig,
       type_factory: Callable[
           [pyvizier.ParameterConfig], NumpyArraySpecType
       ] = NumpyArraySpecType.default_factory,
-      floating_dtype: np.dtype = np.float32,
-      int_dtype: np.dtype = np.int32,
+      floating_dtype: Union[np.dtype, Type[np.floating]] = np.float32,
+      int_dtype: Union[np.dtype, Type[np.integer]] = np.int32,
       *,
       pad_oovs: bool = True,
   ) -> 'NumpyArraySpec':
     """Factory function.
 
     Args:
       pc:
@@ -154,34 +155,34 @@
     Returns:
       NumpyArraySpec.
     """
     the_type = type_factory(pc)
     if the_type == NumpyArraySpecType.CONTINUOUS:
       return NumpyArraySpec(
           the_type,
-          floating_dtype,
+          np.dtype(floating_dtype),
           bounds=pc.bounds,
           num_dimensions=1,
           scale=pc.scale_type,
           name=pc.name,
           num_oovs=0,
       )
     elif the_type == NumpyArraySpecType.DISCRETE:
       return NumpyArraySpec(
           the_type,
-          int_dtype,
+          np.dtype(int_dtype),
           bounds=(0, len(pc.feasible_values)),
           num_dimensions=1,
           name=pc.name,
           num_oovs=1 if pad_oovs else 0,
       )
     elif the_type == NumpyArraySpecType.ONEHOT_EMBEDDING:
       return NumpyArraySpec(
           the_type,
-          floating_dtype,
+          np.dtype(floating_dtype),
           bounds=(0.0, 1.0),
           num_dimensions=len(pc.feasible_values) + 1,
           name=pc.name,
           num_oovs=1 if pad_oovs else 0,
       )
     raise ValueError(f'Unknown type {type}')
 
@@ -351,63 +352,74 @@
       trials:
 
     Returns:
       Returns an array of shape (number of trials, feature dimension).
       Subclasses must use a fixed feature dimension. In particular, it should
       be a constant function of the input trials.
     """
-    pass
 
   @property
   @abc.abstractmethod
   def output_spec(self) -> NumpyArraySpec:
     """Provides specification of the output from this converter."""
-    pass
 
   @property
   @abc.abstractmethod
   def parameter_config(self):
     """Original ParameterConfig that this converter acts on."""
-    pass
 
   @abc.abstractmethod
   def to_parameter_values(
       self, array: np.ndarray
   ) -> List[Optional[pyvizier.ParameterValue]]:
-    """Convert to parameter values."""
-    pass
+    """Convert and clip to the nearest feasible parameter values.
+
+    NOTE: value is automatically truncated to lie inside the search space.
+      This method should only be called to convert suggestions.
+
+    Args:
+      array: has shape (number of trials, feature dimension)
+
+    Returns:
+      List of (ParameterValue or None).  A list entry is None when this
+      converter's parameter doesn't exist in the Trial.  (This is common
+      when parameters are conditional.)
+    """
 
 
 @dataclasses.dataclass
 class ModelInputArrayBijector:
   """Transformations on the numpy arrays generated by ModelInputConverter."""
 
   forward_fn: Callable[[np.ndarray], np.ndarray]
   backward_fn: Callable[[np.ndarray], np.ndarray]
   output_spec: NumpyArraySpec  # Spec after forward_fn is applied.
 
   @classmethod
-  def identity(cls, spec) -> 'ModelInputArrayBijector':
+  def identity(cls, spec: NumpyArraySpec) -> 'ModelInputArrayBijector':
     return cls(lambda x: x, lambda x: x, spec)
 
   @classmethod
   def scaler_from_spec(cls, spec: NumpyArraySpec) -> 'ModelInputArrayBijector':
     """For continuous specs, linearize and scale it to (0, 1) range."""
     low, high = spec.bounds
     if spec.type != NumpyArraySpecType.CONTINUOUS:
       return cls.identity(attr.evolve(spec, scale=None))
     if low == high:
 
       def backward_fn(y):
-        return np.where(np.isfinite(y), np.zeros_like(y) + low, y)
+        return np.where(np.isfinite(y), y + low - 0.5, y)
+
+      def forward_fn(y):
+        return np.where(np.isfinite(y), y - low + 0.5, y)
 
       return cls(
-          lambda x: np.where(np.isfinite(x), np.zeros_like(x), x),
+          forward_fn,
           backward_fn,
-          attr.evolve(spec, bounds=(0.0, 1.0), scale=None),
+          attr.evolve(spec, bounds=(0.5, 0.5), scale=None),
       )
 
     if spec.scale == pyvizier.ScaleType.LOG:
       low, high = np.log(low), np.log(high)
       denom = (high - low) or 1.0
       if denom < 1e-6:
         logging.warning('Unusually small range detected for %s', spec)
@@ -507,15 +519,15 @@
   """
 
   def __init__(
       self,
       parameter_config: pyvizier.ParameterConfig,
       getter: Optional[Callable[[pyvizier.TrialSuggestion], Any]] = None,
       *,
-      float_dtype: np.dtype = np.float32,
+      float_dtype: Union[np.dtype, Type[np.floating]] = np.float32,
       max_discrete_indices: int = 10,
       scale: bool = False,
       onehot_embed: bool = False,
       converts_to_parameter: bool = True,
       pad_oovs: bool = True,
   ):
     """Init.
@@ -607,24 +619,15 @@
     values = [value_converter(t) for t in trials]
     array = np.asarray(values, dtype=self._getter_spec.dtype).reshape([-1, 1])
     return self.onehot_encoder.forward_fn(self.scaler.forward_fn(array))
 
   def _to_parameter_value(
       self, value: Union['np.float', float, int]
   ) -> Optional[pyvizier.ParameterValue]:
-    """Converts to a single parameter value.
-
-    Be aware that the value is automatically truncated.
-
-    Args:
-      value:
-
-    Returns:
-      ParameterValue.
-    """
+    """Converts to a single parameter value; see to_parameter_values()."""
     # TODO: NaNs and out-of-vocab values should return None instead
     # of raising an error.
     if not self._converts_to_parameter:
       return None
     if self.parameter_config.type == pyvizier.ParameterType.DOUBLE:
       # Input parameter was DOUBLE. Output is also DOUBLE.
       return pyvizier.ParameterValue(
@@ -744,15 +747,17 @@
 
   def __init__(
       self,
       metric_information: pyvizier.MetricInformation,
       *,
       flip_sign_for_minimization_metrics: bool = False,
       shift_safe_metrics: bool = True,
-      dtype: Union[Type[float], Type[int], np.dtype] = np.float32,
+      dtype: Union[
+          Type[float], Type[int], Type[np.generic], np.dtype
+      ] = np.float32,
       raise_errors_for_missing_metrics: bool = False,
   ):
     """Init.
 
     Args:
       metric_information:
       flip_sign_for_minimization_metrics: Flips the sign if the metric is to
@@ -1214,15 +1219,14 @@
     return dict_to_array(self._impl.to_labels(trials))
 
   def to_xy(self, trials) -> Tuple[np.ndarray, np.ndarray]:
     return self.to_features(trials), self.to_labels(trials)
 
   def to_parameters(self, arr: np.ndarray) -> Sequence[pyvizier.ParameterDict]:
     """Convert to nearest feasible parameter value. NaNs are preserved."""
-    # TODO: Add a boolean flag to disable automatic clipping.
     arrformat = DictOf2DArrays(self._impl.to_features([]))
     return self._impl.to_parameters(arrformat.dict_like(arr))
 
   @classmethod
   def from_study_config(
       cls,
       study_config: pyvizier.ProblemStatement,
```

### Comparing `google-vizier-0.1.4/vizier/pyvizier/converters/core_test.py` & `google-vizier-0.1.5/vizier/pyvizier/converters/core_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for core."""
 
+from absl import logging
 import numpy as np
 from vizier import pyvizier
 from vizier._src.algorithms.designers import random
 from vizier._src.algorithms.testing import test_runners
 from vizier.pyvizier.converters import core
 from vizier.testing import test_studies
 
@@ -335,26 +336,30 @@
             parameters={
                 'x1': pyvizier.ParameterValue(1.0),
                 'x2': pyvizier.ParameterValue(2.0),
             },
             final_measurement=pyvizier.Measurement(
                 steps=1, metrics={'y1': 10.0, 'y2': 20.0}
             ),
+            creation_time=None,
         ),
         pyvizier.Trial(
             parameters={
                 'x1': pyvizier.ParameterValue(3.0),
                 'x2': pyvizier.ParameterValue(4.0),
             },
             final_measurement=pyvizier.Measurement(
                 steps=1, metrics={'y1': 40.0, 'y2': 50.0, 'y3': 60.0}
             ),
+            creation_time=None,
         ),
     ]
     trials = converter.to_trials(actual_features, actual_labels)
+    for t in trials:
+      t.creation_time = None
     self.assertEqual(
         actual_trials,
         trials,
         msg='conversion from features and labels to trials failed.',
     )
     features, labels = converter.to_xy(actual_trials)
     np.testing.assert_equal(
@@ -555,15 +560,15 @@
     self.assertEqual(
         converter.metric_information,
         pyvizier.MetricInformation(
             name='metric2', goal=pyvizier.ObjectiveMetricGoal.MINIMIZE
         ),
     )
 
-  def test_shift_threshould(self):
+  def test_shift_threshold(self):
     converter = core.DefaultModelOutputConverter(
         pyvizier.MetricInformation(
             name='metric2',
             goal=pyvizier.ObjectiveMetricGoal.MINIMIZE,
             safety_threshold=5.0,
         ),
         flip_sign_for_minimization_metrics=False,
@@ -863,17 +868,19 @@
     )
 
     scaled = np.asarray([[0.0], [0.5], [1.0]], dtype)
     # Pytype still thinks `actual` entries might be None, hence we specify type.
     actual: list[pyvizier.ParameterValue] = converter.to_parameter_values(  # pytype:disable=annotation-type-mismatch
         scaled
     )
+    self.assertAlmostEqual(actual[0].value, 1e-4, delta=1e-6)
     self.assertGreaterEqual(actual[0].value, 1e-4)
-    self.assertLessEqual(actual[1].value, 0.5)
-    self.assertLessEqual(actual[1].value, 1e2)
+    self.assertAlmostEqual(actual[1].value, 0.1, delta=1e-5)
+    self.assertAlmostEqual(actual[2].value, 100.0, delta=1e-2)
+    self.assertLessEqual(actual[2].value, 100.0)
 
   @parameterized.parameters([
       dict(dtype=np.float32),
       dict(dtype=np.float64),
       dict(dtype='float32'),
       dict(dtype='float64'),
   ])
@@ -936,15 +943,15 @@
     )
     actual = converter.convert([
         Trial(parameters={'x1': pyvizier.ParameterValue(0.9)}),
         Trial(parameters={'x1': pyvizier.ParameterValue(1.0)}),
         Trial(parameters={'x1': pyvizier.ParameterValue('a')}),
         Trial(),
     ])
-    expected = np.asarray([[0.0], [0.0], [np.NaN], [np.NaN]], dtype)
+    expected = np.asarray([[0.5], [0.6], [np.NaN], [np.NaN]], dtype)
     np.testing.assert_equal(expected, actual)
 
   @parameterized.parameters([
       dict(dtype=np.float32),
       dict(dtype=np.float64),
       dict(dtype='float32'),
       dict(dtype='float64'),
@@ -962,16 +969,19 @@
     )
     actual = converter.convert([
         Trial(parameters={'x1': pyvizier.ParameterValue(np.exp(0.9))}),
         Trial(parameters={'x1': pyvizier.ParameterValue(np.exp(1.2))}),
         Trial(parameters={'x1': pyvizier.ParameterValue('a')}),
         Trial(),
     ])
-    expected = np.asarray([[0.0], [0.0], [np.NaN], [np.NaN]], dtype=dtype)
-    np.testing.assert_equal(expected, actual)
+    expected = np.asarray(
+        [[0.5], [0.5 + np.exp(1.2) - np.exp(0.9)], [np.NaN], [np.NaN]],
+        dtype=dtype,
+    )
+    np.testing.assert_almost_equal(expected, actual)
 
   @parameterized.parameters([
       dict(dtype=np.float32),
       dict(dtype=np.float64),
       dict(dtype='float32'),
       dict(dtype='float64'),
   ])
@@ -988,16 +998,19 @@
     )
     actual = converter.convert([
         Trial(parameters={'x1': pyvizier.ParameterValue(np.exp(0.9))}),
         Trial(parameters={'x1': pyvizier.ParameterValue(np.exp(1.2))}),
         Trial(parameters={'x1': pyvizier.ParameterValue('a')}),
         Trial(),
     ])
-    expected = np.asarray([[0.0], [0.0], [np.NaN], [np.NaN]], dtype=dtype)
-    np.testing.assert_equal(expected, actual)
+    expected = np.asarray(
+        [[0.5], [0.5 + np.exp(1.2) - np.exp(0.9)], [np.NaN], [np.NaN]],
+        dtype=dtype,
+    )
+    np.testing.assert_almost_equal(expected, actual)
 
   @parameterized.parameters([
       dict(dtype=np.float32),
       dict(dtype=np.float64),
       dict(dtype='float32'),
       dict(dtype='float64'),
   ])
@@ -1094,15 +1107,15 @@
     )
     np.testing.assert_allclose(expected, actual)
     self.assertEqual(expected.dtype, actual.dtype)
     self.assertEqual(
         converter.output_spec,
         core.NumpyArraySpec(
             core.NumpyArraySpecType.ONEHOT_EMBEDDING,
-            np.float32,
+            np.dtype(np.float32),
             (0, 1),
             4,
             'x1',
             1,
         ),
         msg=repr(converter.output_spec),
     )
@@ -1202,9 +1215,78 @@
         onehot_embed=False,
         float_dtype=dtype,
     )
     self.assertEqual(input_converter.output_spec.bounds[0], 0.0)
     self.assertEqual(input_converter.output_spec.bounds[1], 1.0)
 
 
+class ModelInputArrayBijectorTest(absltest.TestCase):
+
+  def testIdentityBijector(self):
+    parameter_config = pyvizier.ParameterConfig.factory('p', bounds=(0.0, 1.0))
+    spec = core.NumpyArraySpec(
+        name='p',
+        type=core.NumpyArraySpecType.default_factory(parameter_config),
+        dtype=np.dtype(np.float32),
+        bounds=(0.0, 1.0),
+        num_dimensions=1,
+        num_oovs=0,
+    )
+    bijector = core.ModelInputArrayBijector.identity(spec)
+    for x in [0.0, 0.25, 0.5, 0.625, 1.0]:
+      x = np.array(x)
+      self.assertLessEqual(
+          bijector.forward_fn(x), bijector.output_spec.bounds[1]
+      )
+      self.assertGreaterEqual(
+          bijector.forward_fn(x), bijector.output_spec.bounds[0]
+      )
+      self.assertEqual(bijector.backward_fn(bijector.forward_fn(x)), x)
+
+  def testScalarFromSpec(self):
+    parameter_config = pyvizier.ParameterConfig.factory('p', bounds=(1.0, 3.0))
+    spec = core.NumpyArraySpec(
+        name='p',
+        type=core.NumpyArraySpecType.default_factory(parameter_config),
+        dtype=np.dtype(np.float32),
+        bounds=(1.0, 3.0),
+        num_dimensions=1,
+        num_oovs=0,
+    )
+    bijector = core.ModelInputArrayBijector.scaler_from_spec(spec)
+    for x in [1.0, 1.25, 1.5, 2.625, 3.0]:
+      x = np.array(x)
+      self.assertLessEqual(
+          bijector.forward_fn(x), bijector.output_spec.bounds[1]
+      )
+      self.assertGreaterEqual(
+          bijector.forward_fn(x), bijector.output_spec.bounds[0]
+      )
+      self.assertEqual(bijector.backward_fn(bijector.forward_fn(x)), x)
+
+  def testScalarFromSinglePointSpec(self):
+    parameter_config = pyvizier.ParameterConfig.factory('p', bounds=(1.0, 1.0))
+    spec = core.NumpyArraySpec(
+        name='p',
+        type=core.NumpyArraySpecType.default_factory(parameter_config),
+        dtype=np.dtype(np.float32),
+        bounds=(1.0, 1.0),
+        num_dimensions=1,
+        num_oovs=0,
+    )
+    bijector = core.ModelInputArrayBijector.scaler_from_spec(spec)
+    x = np.array(1.0)
+    logging.info(
+        'fwd(x)=%s output_spec.bounds=%s',
+        bijector.forward_fn(x),
+        bijector.output_spec.bounds,
+    )
+    self.assertLessEqual(bijector.forward_fn(x), bijector.output_spec.bounds[1])
+    self.assertGreaterEqual(
+        bijector.forward_fn(x), bijector.output_spec.bounds[0]
+    )
+    self.assertLessEqual(bijector.forward_fn(x), bijector.output_spec.bounds[1])
+    self.assertEqual(bijector.backward_fn(bijector.forward_fn(x)), x)
+
+
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.4/vizier/pyvizier/converters/embedder.py` & `google-vizier-0.1.5/vizier/pyvizier/converters/embedder.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/pyvizier/converters/embedder_test.py` & `google-vizier-0.1.5/vizier/pyvizier/converters/embedder_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/pyvizier/converters/feature_mapper.py` & `google-vizier-0.1.5/vizier/pyvizier/converters/feature_mapper.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/pyvizier/converters/feature_mapper_test.py` & `google-vizier-0.1.5/vizier/pyvizier/converters/feature_mapper_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/pyvizier/converters/spatio_temporal.py` & `google-vizier-0.1.5/vizier/pyvizier/converters/spatio_temporal.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/pyvizier/converters/spatio_temporal_test.py` & `google-vizier-0.1.5/vizier/pyvizier/converters/spatio_temporal_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/pyvizier/multimetric/__init__.py` & `google-vizier-0.1.5/vizier/pyvizier/multimetric/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/pyvizier/multimetric/xla_pareto.py` & `google-vizier-0.1.5/vizier/pyvizier/multimetric/xla_pareto.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/service/__init__.py` & `google-vizier-0.1.5/vizier/service/servers/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,8 +10,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-# TODO: Fill this in w/ necessary service imports.
+"""Different servers for the user."""
+from vizier._src.service.vizier_server import DefaultVizierServer
+from vizier._src.service.vizier_server import DistributedPythiaVizierServer
```

### Comparing `google-vizier-0.1.4/vizier/service/clients.py` & `google-vizier-0.1.5/vizier/_src/service/clients.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,34 +17,25 @@
 """OSS Vizier client."""
 
 # TODO: Raise vizier-specific exceptions.
 
 from typing import Any, Callable, Iterable, Iterator, List, Mapping, Optional, Type
 import attr
 
+from vizier._src.service import constants
+from vizier._src.service import resources
+from vizier._src.service import vizier_client
 from vizier.client import client_abc
-from vizier.service import constants
 from vizier.service import pyvizier as vz
-from vizier.service import resources
-from vizier.service import vizier_client
 
 # Redeclared so users do not have to also import client_abc and clients.py.
 ResourceNotFoundError = client_abc.ResourceNotFoundError
 
-
-# TODO: Consider if user should set a one-line flag explicitly to
-# denote local NO_ENDPOINT server will be used.
-@attr.define
-class _EnvironmentVariables:
-  server_endpoint: str = attr.field(
-      default=constants.NO_ENDPOINT, validator=attr.validators.instance_of(str)
-  )
-
-
-environment_variables = _EnvironmentVariables()
+# Redeclared since clients.py is the user-facing client API.
+environment_variables = vizier_client.environment_variables
 
 
 @attr.define
 class Trial(client_abc.TrialInterface):
   """Trial class.
 
   This class owns a Vizier client of the Study that contains the Trial that
@@ -208,17 +199,14 @@
 
   def materialize_state(self) -> vz.StudyState:
     return self._client.get_study_state()
 
   @classmethod
   def from_resource_name(cls: Type['Study'], name: str) -> 'Study':
     client = vizier_client.VizierClient(
-        vizier_client.create_vizier_servicer_or_stub(
-            environment_variables.server_endpoint
-        ),
         name,
         constants.UNUSED_CLIENT_ID,
     )
     try:
       _ = client.get_study_config()  # Make sure study exists.
     except Exception as err:
       raise KeyError(f'Study {name} does not exist.') from err
@@ -260,14 +248,13 @@
       study_id: Unique identifier within the same owner.
 
     Returns:
       Study.
     """
     return Study(
         vizier_client.create_or_load_study(
-            environment_variables.server_endpoint,
             owner_id=owner,
             client_id=constants.UNUSED_CLIENT_ID,
             study_id=study_id,
             study_config=config,
         )
     )
```

### Comparing `google-vizier-0.1.4/vizier/service/clients_test.py` & `google-vizier-0.1.5/vizier/_src/service/clients_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for clients."""
 from absl import logging
+from vizier._src.service import clients
+from vizier._src.service import constants
+from vizier._src.service import vizier_server
 from vizier.client import client_abc_testing
-from vizier.service import clients
-from vizier.service import constants
 from vizier.service import pyvizier as vz
-from vizier.service import vizier_server
 
 from absl.testing import absltest
 
+# Affects local Vizier servicer tests only.
+clients.environment_variables.servicer_use_sql_ram()
+
 
 class VizierClientTest(client_abc_testing.TestCase):
   _owner: str
 
   def create_study(
       self, problem: vz.ProblemStatement, study_id: str
   ) -> clients.Study:
@@ -63,15 +66,17 @@
 class VizierClientTestOnDefaultServer(VizierClientTest):
   _server: vizier_server.DefaultVizierServer
 
   @classmethod
   def setUpClass(cls):
     logging.info('Test setup started.')
     super().setUpClass()
-    cls._server = vizier_server.DefaultVizierServer()
+    cls._server = vizier_server.DefaultVizierServer(
+        database_url=constants.SQL_MEMORY_URL
+    )
     clients.environment_variables.server_endpoint = cls._server.endpoint
     logging.info('Test setup finished.')
 
   @classmethod
   def tearDownClass(cls):
     cls._server._server.stop(None)
     super().tearDownClass()
@@ -80,15 +85,17 @@
 class VizierClientTestOnDistributedPythiaServer(VizierClientTest):
   _server: vizier_server.DistributedPythiaVizierServer
 
   @classmethod
   def setUpClass(cls):
     logging.info('Test setup started.')
     super().setUpClass()
-    cls._server = vizier_server.DistributedPythiaVizierServer()
+    cls._server = vizier_server.DistributedPythiaVizierServer(
+        database_url=constants.SQL_MEMORY_URL
+    )
     clients.environment_variables.server_endpoint = cls._server.endpoint
     logging.info('Test setup finished.')
 
   @classmethod
   def tearDownClass(cls):
     cls._server._server.stop(None)
     cls._server._pythia_server.stop(None)
```

### Comparing `google-vizier-0.1.4/vizier/service/constants.py` & `google-vizier-0.1.5/vizier/_src/service/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Hard coded constants used in /service/ folder."""
+import os
 
 # The metadata namespace under which the Pythia endpoint is stored.
 PYTHIA_ENDPOINT_NAMESPACE = 'service'
 
 # The Study.metadata key where a Pythia endpoint can be stored.
 PYTHIA_ENDPOINT_KEY = 'PYTHIA_ENDPOINT'
 
@@ -29,7 +30,12 @@
 UNUSED_CLIENT_ID = 'unused_client_id'
 
 # Max int32 value.
 MAX_STUDY_ID = 2147483647
 
 # Will use RAM for SQL memory.
 SQL_MEMORY_URL = 'sqlite:///:memory:'
+
+# Will use local file path for HDD storage.
+SERVICE_DIR = os.path.dirname(os.path.realpath(__file__))
+VIZIER_DB_PATH = os.path.join(SERVICE_DIR, 'vizier.db')
+SQL_LOCAL_URL = f'sqlite:///{VIZIER_DB_PATH}'
```

### Comparing `google-vizier-0.1.4/vizier/service/custom_errors.py` & `google-vizier-0.1.5/vizier/_src/service/custom_errors.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/service/datastore_test.py` & `google-vizier-0.1.5/vizier/_src/service/ram_datastore_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,32 +10,31 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-"""Tests for vizier.service.datastore."""
-from vizier.service import datastore
-from vizier.service import datastore_test_lib
-from vizier.service import vizier_service_pb2
-from vizier.service.testing import util as test_util
+from vizier._src.service import datastore_test_lib
+from vizier._src.service import ram_datastore
+from vizier._src.service import vizier_service_pb2
+from vizier._src.service.testing import util as test_util
 
 from absl.testing import absltest
 
 UnitMetadataUpdate = vizier_service_pb2.UnitMetadataUpdate
 
 
 class NestedDictRAMDataStoreTest(datastore_test_lib.DataStoreTestCase):
 
   def setUp(self):
     self.owner_id = 'my_username'
     self.study_id = '123123123'
     self.client_id = 'client_0'
-    self.datastore = datastore.NestedDictRAMDataStore()
+    self.datastore = ram_datastore.NestedDictRAMDataStore()
     self.example_study = test_util.generate_study(self.owner_id, self.study_id)
     self.example_trials = test_util.generate_trials(
         [1, 2], owner_id=self.owner_id, study_id=self.study_id
     )
     self.example_suggestion_operations = (
         test_util.generate_suggestion_operations(
             [1, 2, 3, 4], self.owner_id, self.study_id, self.client_id
```

### Comparing `google-vizier-0.1.4/vizier/service/datastore_test_lib.py` & `google-vizier-0.1.5/vizier/_src/service/datastore_test_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 
 """Library functions for testing databases."""
 import copy
 import random
 import string
 from typing import List
 
-from vizier.service import custom_errors
-from vizier.service import datastore
-from vizier.service import key_value_pb2
-from vizier.service import resources
-from vizier.service import study_pb2
-from vizier.service import vizier_oss_pb2
-from vizier.service import vizier_service_pb2
+from vizier._src.service import custom_errors
+from vizier._src.service import datastore
+from vizier._src.service import key_value_pb2
+from vizier._src.service import resources
+from vizier._src.service import study_pb2
+from vizier._src.service import vizier_oss_pb2
+from vizier._src.service import vizier_service_pb2
 
 from google.longrunning import operations_pb2
 from absl.testing import parameterized
 
 UnitMetadataUpdate = vizier_service_pb2.UnitMetadataUpdate
```

### Comparing `google-vizier-0.1.4/vizier/service/grpc_util.py` & `google-vizier-0.1.5/vizier/_src/service/grpc_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from __future__ import annotations
 
 """Utilities for handling GRPC API."""
 
 from typing import Optional
 import grpc
-from vizier.service import custom_errors
+from vizier._src.service import custom_errors
 
 
 # TODO: Create a type Union[_InactiveRpcError, LocalRpcError]
 class LocalRpcError(grpc.RpcError):
   """Class for imitating both a `grpc.ServiceContext` and a `grpc.RpcError`."""
 
   _code: grpc.StatusCode = grpc.StatusCode.UNKNOWN
```

### Comparing `google-vizier-0.1.4/vizier/service/performance_test.py` & `google-vizier-0.1.5/vizier/_src/service/performance_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,30 +16,34 @@
 
 """Large-scale stress tests (multiple clients, mulithreading, etc.) for Vizier Service."""
 
 import multiprocessing.pool
 import time
 from absl import logging
 
+from vizier._src.service import constants
+from vizier._src.service import vizier_client
+from vizier._src.service import vizier_server
 from vizier.benchmarks import experimenters
 from vizier.service import pyvizier
-from vizier.service import vizier_client
-from vizier.service import vizier_server
 
 from absl.testing import absltest
 from absl.testing import parameterized
 
 
 class PerformanceTest(parameterized.TestCase):
   server: vizier_server.DefaultVizierServer
 
   @classmethod
   def setUpClass(cls):
     super().setUpClass()
-    cls.server = vizier_server.DefaultVizierServer()
+    cls.server = vizier_server.DefaultVizierServer(
+        database_url=constants.SQL_MEMORY_URL
+    )
+    vizier_client.environment_variables.server_endpoint = cls.server.endpoint
 
   @parameterized.parameters(
       (1, 10, 2),
       (2, 10, 2),
       (10, 10, 2),
       (50, 5, 2),
       (100, 5, 2),
@@ -52,15 +56,14 @@
           'Sphere', dimension
       )()
       problem_statement = experimenter.problem_statement()
       study_config = pyvizier.StudyConfig.from_problem(problem_statement)
       study_config.algorithm = pyvizier.Algorithm.NSGA2
 
       client = vizier_client.create_or_load_study(
-          server_endpoint=self.server.endpoint,
           owner_id='my_username',
           study_id=self.id(),  # Use the testcase name.
           study_config=study_config,
           client_id=str(client_id),
       )
 
       for _ in range(num_trials_per_client):
```

### Comparing `google-vizier-0.1.4/vizier/service/policy_factory.py` & `google-vizier-0.1.5/vizier/_src/service/policy_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Policy Factory API."""
 # pylint:disable=g-import-not-at-top
 import functools
-import random
+import time
 from typing import Protocol
 
 from vizier import pythia
 from vizier._src.algorithms.policies import designer_policy as dp
 from vizier.service import pyvizier as vz
 
 
@@ -76,15 +76,15 @@
           problem_statement,
           policy_supporter,
           grid.GridSearchDesigner.from_problem,
       )
     elif algorithm == 'SHUFFLED_GRID_SEARCH':
       from vizier._src.algorithms.designers import grid
 
-      shuffle_seed = random.randint(0, 2147483647)
+      shuffle_seed = int(time.time())
       grid_factory = functools.partial(
           grid.GridSearchDesigner.from_problem, shuffle_seed=shuffle_seed
       )
       return dp.PartiallySerializableDesignerPolicy(
           problem_statement,
           policy_supporter,
           grid_factory,
```

### Comparing `google-vizier-0.1.4/vizier/service/pythia_service.py` & `google-vizier-0.1.5/vizier/_src/service/pythia_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 
 """Separate Pythia service for handling algorithmic logic."""
 from typing import Optional
 from absl import logging
 import attr
 import grpc
 
-from vizier.service import policy_factory as policy_factory_lib
-from vizier.service import pythia_service_pb2
-from vizier.service import pythia_service_pb2_grpc
+from vizier._src.service import policy_factory as policy_factory_lib
+from vizier._src.service import pythia_service_pb2
+from vizier._src.service import pythia_service_pb2_grpc
+from vizier._src.service import service_policy_supporter
+from vizier._src.service import stubs_util
+from vizier._src.service import types
 from vizier.service import pyvizier as vz
-from vizier.service import service_policy_supporter
-from vizier.service import stubs_util
-from vizier.service import types
 
 from google.protobuf import empty_pb2
 
 
 @attr.define
 class PythiaServicer(pythia_service_pb2_grpc.PythiaServiceServicer):
   """Implements the GRPC functions outlined in pythia_service.proto."""
```

### Comparing `google-vizier-0.1.4/vizier/service/pythia_util.py` & `google-vizier-0.1.5/vizier/_src/service/pythia_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,34 +14,39 @@
 
 from __future__ import annotations
 
 """Utility functions for the Pythia protocol code."""
 
 import logging
 import threading
-from typing import Generic, Optional, TypeVar
+from typing import Generic, Optional, Protocol, TypeVar
 from vizier import pythia
 
-_TT = TypeVar('_TT')
 
+class _HasErrorDetails(Protocol):
+  error_details: str
 
-class ResponseWaiter(Generic[_TT]):
+
+_T = TypeVar('_T', bound=_HasErrorDetails)
+
+
+class ResponseWaiter(Generic[_T]):
   """A stored message with a Wait() mechanism.
 
   This is a bridge between two threads; it stores a message, and
   the reader thread waits until the writer thread calls Report(..., done=True).
   Once Report() is called, it unblocks WaitForRespose().
   """
 
   def __init__(self):
     self._lock = threading.Lock()
-    self._response: Optional[_TT] = None
+    self._response: Optional[_T] = None
     self._wait = threading.Event()
 
-  def Report(self, update: _TT):
+  def Report(self, update: _T) -> None:
     """Called by the gRPC thread with a message from Vizier.
 
     When called, this unblocks WaitForResponse().
 
     Args:
       update:
 
@@ -52,28 +57,28 @@
     with self._lock:
       if self._wait.is_set():
         raise pythia.PythiaProtocolError(
             'ResponseWaiter.Report() called after wait is set')
       self._response = update
       self._wait.set()
 
-  def WaitForResponse(self) -> _TT:
+  def WaitForResponse(self) -> _T:
     """Returns the result or raises an error.
 
     Raises:
       PythiaProtocolError: Due to a failure of the Pythia protocol.
       VizierDatabaseError: Vizier was unable to service the request.
     """
     self._wait.wait()
     logging.info('About to take _lock in ResponseWaiter.WaitForResponse()')
     with self._lock:
-      if not self._response:
+      if self._response is None:
         logging.info('Raise')
         raise pythia.PythiaProtocolError('No response.')
-      if self._response.error_details:
+      elif self._response.error_details:
         raise pythia.VizierDatabaseError(self._response.error_details)
       logging.info('No raise -- WaitForResponse done')
       return self._response
 
   def CancelWait(self) -> None:
     """Cancel the wait."""
     logging.info('About to CancelWait()')
```

### Comparing `google-vizier-0.1.4/vizier/service/pyvizier/__init__.py` & `google-vizier-0.1.5/vizier/service/pyvizier/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/service/resources.py` & `google-vizier-0.1.5/vizier/_src/service/resources.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/service/resources_test.py` & `google-vizier-0.1.5/vizier/_src/service/resources_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for vizier.service.resources."""
 
-from vizier.service import resources
-from vizier.service import study_pb2
-from vizier.service.testing import util as test_util
+from vizier._src.service import resources
+from vizier._src.service import study_pb2
+from vizier._src.service.testing import util as test_util
 
 from absl.testing import absltest
 from absl.testing import parameterized
 
 
 class UtilTest(parameterized.TestCase):
```

### Comparing `google-vizier-0.1.4/vizier/service/service_policy_supporter.py` & `google-vizier-0.1.5/vizier/_src/service/service_policy_supporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 The Policy can use these methods to communicate with Vizier.
 """
 import datetime
 from typing import Iterable, List, Optional
 
 from vizier import pythia
 from vizier import pyvizier as vz
+from vizier._src.service import types
+from vizier._src.service import vizier_service_pb2
 from vizier.service import pyvizier
-from vizier.service import types
-from vizier.service import vizier_service_pb2
 
 
 # TODO: Consider replacing protos with Pyvizier clients.py.
 class ServicePolicySupporter(pythia.PolicySupporter):
   """Service version of the PolicySupporter."""
 
   def __init__(self, study_guid: str, vizier_service: types.VizierService):
```

### Comparing `google-vizier-0.1.4/vizier/service/service_policy_supporter_test.py` & `google-vizier-0.1.5/vizier/_src/service/service_policy_supporter_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,34 +10,36 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-"""Tests for vizier.service.service_policy_supporter."""
+from vizier._src.service import constants
+from vizier._src.service import resources
+from vizier._src.service import service_policy_supporter
+from vizier._src.service import study_pb2
+from vizier._src.service import vizier_service
+from vizier._src.service.testing import util as test_util
 from vizier.service import pyvizier
-from vizier.service import resources
-from vizier.service import service_policy_supporter
-from vizier.service import study_pb2
-from vizier.service import vizier_service
-from vizier.service.testing import util as test_util
 
 from absl.testing import absltest
 
 
 class PythiaSupporterTest(absltest.TestCase):
 
   def setUp(self):
     self.owner_id = 'my_username'
     self.study_id = '1231223'
     self.study_name = resources.StudyResource(
         owner_id=self.owner_id, study_id=self.study_id
     ).name
-    self.vs = vizier_service.VizierServicer()
+    self.vs = vizier_service.VizierServicer(
+        database_url=constants.SQL_MEMORY_URL
+    )
     self.example_study = test_util.generate_study(self.owner_id, self.study_id)
     self.vs.datastore.create_study(self.example_study)
 
     self.active_trials = test_util.generate_trials(
         range(1, 7), self.owner_id, self.study_id
     )
     self.succeeded_trial = test_util.generate_trials(
```

### Comparing `google-vizier-0.1.4/vizier/service/sql_datastore.py` & `google-vizier-0.1.5/vizier/_src/service/sql_datastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 import collections
 import threading
 from typing import Callable, DefaultDict, Iterable, List, Optional
 from absl import logging
 
 import sqlalchemy as sqla
 
-from vizier.service import custom_errors
-from vizier.service import datastore
-from vizier.service import key_value_pb2
-from vizier.service import resources
-from vizier.service import study_pb2
-from vizier.service import vizier_oss_pb2
+from vizier._src.service import custom_errors
+from vizier._src.service import datastore
+from vizier._src.service import key_value_pb2
+from vizier._src.service import resources
+from vizier._src.service import study_pb2
+from vizier._src.service import vizier_oss_pb2
+from vizier.service import pyvizier as vz
+
 from google.longrunning import operations_pb2
 
 
 # TODO: Consider using ORM API (when fixed) to reduce code length.
 class SQLDataStore(datastore.DataStore):
   """SQL Datastore."""
 
@@ -583,15 +585,17 @@
       study_result = self._connection.execute(get_study_query)
       row = study_result.fetchone()
       if not row:
         raise custom_errors.NotFoundError('No such study:', s_resource.name)
       original_study = study_pb2.Study.FromString(row['serialized_study'])
 
       # Store Study-related metadata into the database.
-      datastore.merge_study_metadata(original_study.study_spec, study_metadata)
+      vz.metadata_util.merge_study_metadata(
+          original_study.study_spec, study_metadata
+      )
       update_study_query = (
           sqla.update(self._studies_table)
           .where(self._studies_table.c.study_name == study_name)
           .values(serialized_study=original_study.SerializeToString())
       )
       self._connection.execute(update_study_query)
 
@@ -614,14 +618,14 @@
         trial_result = self._connection.execute(original_trial_query)
         row = trial_result.fetchone()
         if not row:
           raise custom_errors.NotFoundError('No such trial:', trial_name)
         original_trial = study_pb2.Trial.FromString(row['serialized_trial'])
 
         # Update Trial.
-        datastore.merge_trial_metadata(original_trial, md_list)
+        vz.metadata_util.merge_trial_metadata(original_trial, md_list)
         update_trial_query = (
             sqla.update(self._trials_table)
             .where(self._trials_table.c.trial_name == trial_name)
             .values(serialized_trial=original_trial.SerializeToString())
         )
         self._connection.execute(update_trial_query)
```

### Comparing `google-vizier-0.1.4/vizier/service/sql_datastore_test.py` & `google-vizier-0.1.5/vizier/_src/service/sql_datastore_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for sql_datastore."""
+import os
 import sqlalchemy as sqla
 
-from vizier.service import datastore_test_lib
-from vizier.service import sql_datastore
-from vizier.service.testing import util as test_util
+from vizier._src.service import constants
+from vizier._src.service import datastore_test_lib
+from vizier._src.service import sql_datastore
+from vizier._src.service.testing import util as test_util
 from absl.testing import absltest
 
 
 class SQLDataStoreTest(datastore_test_lib.DataStoreTestCase):
 
   def setUp(self):
     self.owner_id = 'my_username'
@@ -40,15 +42,15 @@
     )
     self.example_early_stopping_operations = (
         test_util.generate_early_stopping_operations(
             [1, 2], self.owner_id, self.study_id
         )
     )
 
-    engine = sqla.create_engine('sqlite:///:memory:', echo=True)
+    engine = sqla.create_engine(constants.SQL_MEMORY_URL, echo=True)
     self.datastore = sql_datastore.SQLDataStore(engine)
     super().setUp()
 
   def test_study_api(self):
     self.assertStudyAPI(self.datastore, self.example_study)
 
   def test_trial(self):
@@ -72,9 +74,35 @@
 
   def test_update_metadata(self):
     self.assertUpdateMetadataAPI(
         self.datastore, self.example_study, self.example_trials
     )
 
 
+class SQLDataStoreAdditionalTest(absltest.TestCase):
+  """For additional tests outside of regular database functionality."""
+
+  def setUp(self):
+    super().setUp()
+    self.owner_id = 'my_username'
+    self.study_id = '123123123'
+    self.example_study = test_util.generate_study(self.owner_id, self.study_id)
+
+  @absltest.skip("Github workflow tests don't allow using directories.")
+  def test_local_hdd_persistence(self):
+    db_path = os.path.join(absltest.get_default_test_tmpdir(), 'local.db')
+    sql_url = f'sqlite:///{db_path}'
+
+    engine = sqla.create_engine(sql_url, echo=True)
+    datastore = sql_datastore.SQLDataStore(engine)
+    datastore.create_study(self.example_study)
+    del datastore
+
+    engine2 = sqla.create_engine(sql_url, echo=True)
+    datastore2 = sql_datastore.SQLDataStore(engine2)
+    study = datastore2.load_study(self.example_study.name)
+
+    self.assertEqual(self.example_study, study)
+
+
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.4/vizier/service/stubs_util.py` & `google-vizier-0.1.5/vizier/_src/service/stubs_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 """Utility functions for creating GRPC stubs."""
 
 import functools
 from typing import Optional
 from absl import logging
 import grpc
 
-from vizier.service import pythia_service_pb2_grpc
-from vizier.service import vizier_service_pb2_grpc
+from vizier._src.service import pythia_service_pb2_grpc
+from vizier._src.service import vizier_service_pb2_grpc
 
 
 def _create_channel(
     endpoint: str, timeout: Optional[float] = None
 ) -> grpc.Channel:
   """Creates GRPC channel."""
   logging.info('Securing channel to %s.', endpoint)
```

### Comparing `google-vizier-0.1.4/vizier/service/stubs_util_test.py` & `google-vizier-0.1.5/vizier/_src/service/stubs_util_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Tests for vizier.service.stubs_util."""
 
 import grpc
-from vizier.service import stubs_util
+from vizier._src.service import stubs_util
 from absl.testing import absltest
 from absl.testing import parameterized
 
 
 class StubsUtilTest(parameterized.TestCase):
 
   @parameterized.parameters(
```

### Comparing `google-vizier-0.1.4/vizier/service/testing/util.py` & `google-vizier-0.1.5/vizier/_src/service/testing/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Below contain utilities for writing tests to reduce code duplication."""
 from typing import List, Sequence
 
-from vizier.service import resources
-from vizier.service import study_pb2
-from vizier.service import vizier_oss_pb2
+from vizier._src.service import resources
+from vizier._src.service import study_pb2
+from vizier._src.service import vizier_oss_pb2
 
 from google.longrunning import operations_pb2
 
 
 def generate_study(owner_id: str = 'my_username',
                    study_id: str = '1234',
                    display_name: str = 'cifar10',
@@ -108,16 +108,19 @@
       parameter_id='learning_rate', double_value_spec=double_value_spec)
 
   integer_value_spec = study_pb2.StudySpec.ParameterSpec.IntegerValueSpec(
       min_value=1, max_value=10)
   integer_parameter_spec = study_pb2.StudySpec.ParameterSpec(
       parameter_id='num_layers', integer_value_spec=integer_value_spec)
 
-  categorical_value_spec = study_pb2.StudySpec.ParameterSpec.CategoricalValueSpec(
-      values=['relu', 'sigmoid'])
+  categorical_value_spec = (
+      study_pb2.StudySpec.ParameterSpec.CategoricalValueSpec(
+          values=['relu', 'sigmoid']
+      )
+  )
   categorical_parameter_spec = study_pb2.StudySpec.ParameterSpec(
       parameter_id='nonlinearity',
       categorical_value_spec=categorical_value_spec)
 
   discrete_value_spec = study_pb2.StudySpec.ParameterSpec.DiscreteValueSpec(
       values=[1.0, 1.5, 3.0, 4.5])
   discrete_parameter_spec = study_pb2.StudySpec.ParameterSpec(
```

### Comparing `google-vizier-0.1.4/vizier/service/types.py` & `google-vizier-0.1.5/vizier/_src/service/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 """Convenient types library for the /service/ folder."""
 from typing import Union
 
-from vizier.service import pythia_service_pb2_grpc
-from vizier.service import vizier_service_pb2_grpc
+from vizier._src.service import pythia_service_pb2_grpc
+from vizier._src.service import vizier_service_pb2_grpc
 
 # PythiaService and VizierService aliases allow us to use either a gRPC stub or
 # the actual gRPC servicer implementation (for local setup) interchangeably.
 PythiaService = Union[
     pythia_service_pb2_grpc.PythiaServiceStub,
     pythia_service_pb2_grpc.PythiaServiceServicer,
 ]
```

### Comparing `google-vizier-0.1.4/vizier/service/vizier_client.py` & `google-vizier-0.1.5/vizier/_src/service/vizier_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 from typing import Any, Dict, List, Mapping, Optional, Union
 
 from absl import flags
 from absl import logging
 import attr
 import grpc
 
-from vizier.service import constants
+from vizier._src.service import constants
+from vizier._src.service import resources
+from vizier._src.service import stubs_util
+from vizier._src.service import study_pb2
+from vizier._src.service import types
+from vizier._src.service import vizier_service_pb2
+from vizier._src.service import vizier_service_pb2_grpc
 from vizier.service import pyvizier
-from vizier.service import resources
-from vizier.service import stubs_util
-from vizier.service import study_pb2
-from vizier.service import types
-from vizier.service import vizier_service_pb2
-from vizier.service import vizier_service_pb2_grpc
 from vizier.utils import attrs_utils
 
 from google.longrunning import operations_pb2
 from google.protobuf import duration_pb2
 from google.protobuf import json_format
 
 flags.DEFINE_integer(
@@ -52,86 +52,69 @@
         'are needed. (You may use zero for interactive demos, but it is only '
         'appropriate for very small Studies.)'
     ),
 )
 FLAGS = flags.FLAGS
 
 
+@attr.define
+class _EnvironmentVariables:
+  server_endpoint: str = attr.field(
+      default=constants.NO_ENDPOINT, validator=attr.validators.instance_of(str)
+  )
+  servicer_kwargs: Dict[str, Any] = attr.field(factory=dict)
+
+  def servicer_use_sql_ram(self) -> None:
+    """Should be used in tests to avoid filepath issues."""
+    self.servicer_kwargs['database_url'] = constants.SQL_MEMORY_URL
+
+
+environment_variables = _EnvironmentVariables()
+
+
 @functools.lru_cache(maxsize=None)
 def _create_local_vizier_servicer() -> (
     vizier_service_pb2_grpc.VizierServiceServicer
 ):
-  from vizier.service import vizier_service  # pylint:disable=g-import-not-at-top
+  from vizier._src.service import vizier_service  # pylint:disable=g-import-not-at-top
 
-  return vizier_service.VizierServicer()
+  return vizier_service.VizierServicer(**environment_variables.servicer_kwargs)
 
 
-def create_vizier_servicer_or_stub(endpoint: str) -> types.VizierService:
+def create_vizier_servicer_or_stub() -> types.VizierService:
+  endpoint = environment_variables.server_endpoint
   if endpoint == constants.NO_ENDPOINT:
     logging.info('No endpoint given; using cached local VizierServicer.')
     logging.warning('Python 3.8+ is required in this case.')
     return _create_local_vizier_servicer()
   return stubs_util.create_vizier_server_stub(endpoint)
 
 
 @attr.frozen(init=True)
 class VizierClient:
-  """Client for communicating with the Vizer Service via GRPC.
+  """Client for communicating with the Vizier Service via GRPC.
 
   It can be initialized directly with a VizierService, or
   created from endpoint. See also `create_server_stub`.
   """
 
-  # Note that if we use a literal VizierServicer class, only one client should
-  # interact with the server to prevent deadlocks.
-  _service: types.VizierService = attr.field(repr=False)
   _study_resource_name: str = attr.field(
       validator=attr.validators.instance_of(str)
   )
   _client_id: str = attr.field(
       validator=[attr.validators.instance_of(str), attrs_utils.assert_not_empty]
   )
+  _service: types.VizierService = attr.field(
+      repr=False, factory=create_vizier_servicer_or_stub
+  )
 
   @property
   def _study_resource(self) -> resources.StudyResource:
     return resources.StudyResource.from_name(self._study_resource_name)
 
-  @classmethod
-  def from_endpoint(
-      cls, server_endpoint: str, study_resource_name: str, client_id: str
-  ) -> 'VizierClient':
-    """Create a VizierClient object.
-
-    Use this constructor when you know the study_resource_name, and when the
-    Study already exists. Otherwise, you'll probably want to use
-    create_or_load_study() instead of constructing the
-    VizierClient class directly.
-
-    Args:
-      server_endpoint: Address of Vizier Server for creation of gRPC stub, e.g.
-        'localhost:8998'. If equal to UNSET_ENDPOINT, creates a local
-        VizierServicer inside the client.
-      study_resource_name: An identifier of the study. The full study name will
-        be `owners/{owner_id}/studies/{study_id}`.
-      client_id: An ID that identifies the worker requesting a `Trial`. Workers
-        that should run the same trial (for instance, when running a
-        multi-worker model) should have the same ID. If multiple
-        suggestTrialsRequests have the same client_id, the service will return
-        the identical suggested trial if the trial is PENDING, and provide a new
-        trial if the last suggest trial was completed.
-
-    Returns:
-      Vizier client.
-    """
-    return cls(
-        create_vizier_servicer_or_stub(server_endpoint),
-        study_resource_name,
-        client_id,
-    )
-
   @property
   def _owner_id(self) -> str:
     return self._study_resource.owner_id
 
   @property
   def _study_id(self) -> str:
     return self._study_resource.study_id
@@ -427,15 +410,14 @@
     response = self._service.UpdateMetadata(request)
 
     if response.error_details:
       raise RuntimeError(response.error_details)
 
 
 def create_or_load_study(
-    server_endpoint: str,
     owner_id: str,
     client_id: str,
     study_id: str,
     study_config: pyvizier.StudyConfig,
 ) -> VizierClient:
   """Factory method for creating or loading a VizierClient.
 
@@ -447,17 +429,14 @@
 
   This function is designed for use in a distributed system, where many jobs
   initially call create_or_load_study() nearly simultaneously with the same
   `study_config`. In that situation, all clients will end up pointing nicely
   to the same study.
 
   Args:
-      server_endpoint: Address of VizierService for creation of gRPC stub, e.g.
-        'localhost:8998'. If equal to UNSET_ENDPOINT, creates a local
-        VizierServicer inside the client.
       owner_id: An owner id.
       client_id: ID for the VizierClient. See class for notes.
       study_id: Each study is uniquely identified by the tuple (owner_id,
         study_id).
       study_config: Study configuration for Vizier service. If not supplied, it
         will be assumed that the study with the given study_id already exists,
         and will try to retrieve that study.
@@ -468,25 +447,25 @@
   Raises:
       RuntimeError: Indicates that study_config is supplied but CreateStudy
           failed and GetStudy did not succeed after
           constants.MAX_NUM_TRIES_FOR_STUDIES tries.
       ValueError: Indicates that study_config is not supplied and the study
           with the given study_id does not exist.
   """
-  vizier_stub = create_vizier_servicer_or_stub(server_endpoint)
+  vizier_stub = create_vizier_servicer_or_stub()
   study = study_pb2.Study(
       display_name=study_id, study_spec=study_config.to_proto()
   )
   request = vizier_service_pb2.CreateStudyRequest(
       parent=resources.OwnerResource(owner_id).name, study=study
   )
   # The response study contains a service assigned `name`, and may have been
   # created by this RPC or a previous RPC from another client.
   study = vizier_stub.CreateStudy(request)
-  return VizierClient(vizier_stub, study.name, client_id)
+  return VizierClient(study.name, client_id, vizier_stub)
 
 
 def PollingDelay(num_attempts: int, time_scale: float) -> datetime.timedelta:  # pylint:disable=invalid-name
   """Computes a delay to the next attempt to poll the Vizier service.
 
   This does bounded exponential backoff, starting with $time_scale.
   If $time_scale == 0, it starts with a small time interval, less than
```

### Comparing `google-vizier-0.1.4/vizier/service/vizier_client_test.py` & `google-vizier-0.1.5/vizier/_src/service/vizier_client_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,45 +20,48 @@
 # into the datastore.
 # TODO: Cover delete_trial, delete_study, get_study_config, and
 # add_trial, OR turn it into a private module
 
 from typing import List
 from absl import logging
 
-from vizier.service import constants
+from vizier._src.service import constants
+from vizier._src.service import resources
+from vizier._src.service import study_pb2
+from vizier._src.service import vizier_client
+from vizier._src.service import vizier_server
+from vizier._src.service import vizier_service_pb2_grpc
 from vizier.service import pyvizier
-from vizier.service import resources
-from vizier.service import study_pb2
-from vizier.service import vizier_client
-from vizier.service import vizier_server
-from vizier.service import vizier_service_pb2_grpc
 
 from absl.testing import absltest
 from absl.testing import parameterized
 
 
 class VizierClientTest(parameterized.TestCase):
 
   def setUp(self):
     super().setUp()
 
     # Setup Vizier Server and some pre-stored data.
-    self.local_server = vizier_server.DefaultVizierServer()
+    self.local_server = vizier_server.DefaultVizierServer(
+        database_url=constants.SQL_MEMORY_URL
+    )
     self.servicer = self.local_server._servicer
     self.owner_id = 'my_username'
     self.study_id = '1231232'
     self.study_resource_name = resources.StudyResource(
         self.owner_id, self.study_id
     ).name
 
     # Setup connection to server.
-    self.client = vizier_client.VizierClient.from_endpoint(
-        server_endpoint=self.local_server.endpoint,
-        study_resource_name=self.study_resource_name,
-        client_id='my_client',
+    vizier_client.environment_variables.server_endpoint = (
+        self.local_server.endpoint
+    )
+    self.client = vizier_client.VizierClient(
+        study_resource_name=self.study_resource_name, client_id='my_client'
     )
 
     # Store initial data in the vizier service.
     double_value_spec = study_pb2.StudySpec.ParameterSpec.DoubleValueSpec(
         min_value=-1.0, max_value=1.0
     )
     double_parameter_spec = study_pb2.StudySpec.ParameterSpec(
@@ -85,26 +88,24 @@
     self.servicer.datastore.create_trial(self.active_trial)
 
   def test_create_or_load_study(self):
     study_config = pyvizier.StudyConfig()
     study_id = 'example_display_name'
 
     client = vizier_client.create_or_load_study(
-        server_endpoint=self.local_server.endpoint,
         owner_id=self.owner_id,
         client_id='a_client',
         study_id=study_id,
         study_config=study_config,
     )
     study = self.servicer.datastore.load_study(client.study_resource_name)
     self.assertEqual(study.study_spec, study_config.to_proto())
     self.assertIsNotNone(study.name)
 
     another_client = vizier_client.create_or_load_study(
-        server_endpoint=self.local_server.endpoint,
         owner_id=self.owner_id,
         client_id='another_client',
         study_id=study_id,
         study_config=study_config,
     )
     self.assertEqual(
         client.study_resource_name, another_client.study_resource_name
@@ -252,15 +253,14 @@
           pyvizier.MetricInformation(
               name='latency', goal=pyvizier.ObjectiveMetricGoal.MINIMIZE
           )
       )
     study_config.algorithm = algorithm
 
     cifar10_client = vizier_client.create_or_load_study(
-        server_endpoint=self.local_server.endpoint,
         owner_id=self.owner_id,
         study_id='cifar10',
         study_config=study_config,
         client_id='cifar10_client',
     )
 
     for _ in range(num_iterations):
@@ -307,40 +307,37 @@
     self.client.update_metadata(metadata_delta)
 
   def test_unset_endpoint_client(self):
     study_id = 'dummy_study'
     study_config = pyvizier.StudyConfig()
     study_resource_name = resources.StudyResource(self.owner_id, study_id).name
 
-    # Check if server is stored in client.
+    vizier_client.environment_variables.server_endpoint = constants.NO_ENDPOINT
+    vizier_client.environment_variables.servicer_use_sql_ram()
+    # Check if servicer is stored in client.
     local_client1 = vizier_client.create_or_load_study(
-        server_endpoint=constants.NO_ENDPOINT,
         owner_id=self.owner_id,
         client_id='local_client1',
         study_id=study_id,
         study_config=study_config,
     )
     self.assertIsInstance(
         local_client1._service, vizier_service_pb2_grpc.VizierServiceServicer
     )
 
     # Check if the local server is shared.
-    local_client2 = vizier_client.VizierClient.from_endpoint(
-        server_endpoint=constants.NO_ENDPOINT,
-        study_resource_name=study_resource_name,
-        client_id='local_client2',
+    local_client2 = vizier_client.VizierClient(
+        study_resource_name=study_resource_name, client_id='local_client2'
     )
     self.assertEqual(local_client1._service, local_client2._service)
 
     # Same server still exists globally in cache after clients are deleted.
     del local_client1
     del local_client2
-    local_client3 = vizier_client.VizierClient.from_endpoint(
-        server_endpoint=constants.NO_ENDPOINT,
-        study_resource_name=study_resource_name,
-        client_id='local_client3',
+    local_client3 = vizier_client.VizierClient(
+        study_resource_name=study_resource_name, client_id='local_client3'
     )
     self.assertLen(local_client3.list_studies(), 1)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `google-vizier-0.1.4/vizier/service/vizier_server.py` & `google-vizier-0.1.5/vizier/_src/service/vizier_server.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,40 +22,44 @@
 from concurrent import futures
 import datetime
 import time
 
 import attr
 import grpc
 import portpicker
-from vizier.service import constants
-from vizier.service import datastore
-from vizier.service import policy_factory as policy_factory_lib
-from vizier.service import pythia_service
-from vizier.service import pythia_service_pb2_grpc
-from vizier.service import stubs_util
-from vizier.service import vizier_service
-from vizier.service import vizier_service_pb2_grpc
+
+from vizier._src.service import constants
+from vizier._src.service import datastore
+from vizier._src.service import policy_factory as policy_factory_lib
+from vizier._src.service import pythia_service
+from vizier._src.service import pythia_service_pb2_grpc
+from vizier._src.service import stubs_util
+from vizier._src.service import vizier_service
+from vizier._src.service import vizier_service_pb2_grpc
 
 
 @attr.define
 class DefaultVizierServer:
   """Vizier Server which runs Pythia and Vizier Servicers in the same process.
 
   Both servicers have access to the others' literal class instances.
+
+  NOTE: When using this in a test, the database_url should be in-memory
+  (SQL_MEMORY_URL) since tests don't easily allow arbitrarily filepaths.
   """
 
   _host: str = attr.field(init=True, default='localhost')
   _database_url: str = attr.field(
-      init=True, default=constants.SQL_MEMORY_URL, kw_only=True
+      init=True, default=constants.SQL_LOCAL_URL, kw_only=True
   )
   _policy_factory: policy_factory_lib.PolicyFactory = attr.field(
       init=True, factory=policy_factory_lib.DefaultPolicyFactory, kw_only=True
   )
   _early_stop_recycle_period: datetime.timedelta = attr.field(
-      init=False, default=datetime.timedelta(seconds=0.1)
+      init=True, default=datetime.timedelta(seconds=0.1), kw_only=True
   )
   _port: int = attr.field(init=False, factory=portpicker.pick_unused_port)
   _servicer: vizier_service.VizierServicer = attr.field(init=False)
   _server: grpc.Server = attr.field(init=False)
   stub: vizier_service_pb2_grpc.VizierServiceStub = attr.field(init=False)
 
   @property
@@ -88,15 +92,20 @@
 
   def wait_for_early_stop_recycle_period(self) -> None:
     time.sleep(self._early_stop_recycle_period.total_seconds())
 
 
 @attr.define
 class DistributedPythiaVizierServer(DefaultVizierServer):
-  """Separates Pythia from Vizier via over-the-wire distributed communication."""
+  """Separates Pythia from Vizier via over-the-wire distributed communication.
+
+  This is for testing / demonstration purposes only, as in normal use-cases, the
+  Pythia server should actually be created in a separate process from the Vizier
+  server.
+  """
 
   _pythia_port: int = attr.field(
       init=False, factory=portpicker.pick_unused_port
   )
   _pythia_servicer: pythia_service.PythiaServicer = attr.field(init=False)
   _pythia_server: grpc.Server = attr.field(init=False)
   pythia_stub: pythia_service_pb2_grpc.PythiaServiceStub = attr.field(
```

### Comparing `google-vizier-0.1.4/vizier/service/vizier_service.py` & `google-vizier-0.1.5/vizier/_src/service/vizier_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,28 +23,28 @@
 from absl import logging
 import grpc
 import numpy as np
 import sqlalchemy as sqla
 
 from vizier import pythia
 from vizier import pyvizier as vz
-from vizier.service import constants
-from vizier.service import custom_errors
-from vizier.service import datastore
-from vizier.service import grpc_util
-from vizier.service import pythia_service
+from vizier._src.service import constants
+from vizier._src.service import custom_errors
+from vizier._src.service import grpc_util
+from vizier._src.service import pythia_service
+from vizier._src.service import ram_datastore
+from vizier._src.service import resources
+from vizier._src.service import sql_datastore
+from vizier._src.service import stubs_util
+from vizier._src.service import study_pb2
+from vizier._src.service import types
+from vizier._src.service import vizier_oss_pb2
+from vizier._src.service import vizier_service_pb2
+from vizier._src.service import vizier_service_pb2_grpc
 from vizier.service import pyvizier as svz
-from vizier.service import resources
-from vizier.service import sql_datastore
-from vizier.service import stubs_util
-from vizier.service import study_pb2
-from vizier.service import types
-from vizier.service import vizier_oss_pb2
-from vizier.service import vizier_service_pb2
-from vizier.service import vizier_service_pb2_grpc
 
 from google.longrunning import operations_pb2
 from google.protobuf import empty_pb2
 from google.protobuf import timestamp_pb2
 from google.rpc import code_pb2
 from google.rpc import status_pb2
 
@@ -64,15 +64,15 @@
   _TRIAL_MUTABLE_STATES = (
       study_pb2.Trial.State.ACTIVE,
       study_pb2.Trial.State.STOPPING,
   )
 
   def __init__(
       self,
-      database_url: Optional[str] = constants.SQL_MEMORY_URL,
+      database_url: Optional[str] = constants.SQL_LOCAL_URL,
       early_stop_recycle_period: datetime.timedelta = datetime.timedelta(
           seconds=60
       ),
       default_pythia_service: Optional[types.PythiaService] = None,
   ):
     """Initializes the service.
 
@@ -92,15 +92,15 @@
     # By default, uses a local PythiaServicer instance.
     self.default_pythia_service: types.PythiaService = (
         default_pythia_service
         or pythia_service.PythiaServicer(vizier_service=self)
     )
 
     if database_url is None:
-      self.datastore = datastore.NestedDictRAMDataStore()
+      self.datastore = ram_datastore.NestedDictRAMDataStore()
     else:
       engine = sqla.create_engine(
           database_url,
           echo=False,  # Set True to log transactions for debugging.
           connect_args={'check_same_thread': False},
           poolclass=sqla.pool.StaticPool,
       )
```

### Comparing `google-vizier-0.1.4/vizier/service/vizier_service_test.py` & `google-vizier-0.1.5/vizier/_src/service/vizier_service_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 
 """Tests for vizier.service.vizier_server."""
 # TODO: Change the test to create a vizier stub and call its
 # methods, instead of directly calling VizierService methods.
 import datetime
 import time
 import grpc
-from vizier.service import key_value_pb2
-from vizier.service import resources
-from vizier.service import study_pb2
-from vizier.service import vizier_service
-from vizier.service import vizier_service_pb2
-from vizier.service.testing import util as test_util
+
+from vizier._src.service import constants
+from vizier._src.service import key_value_pb2
+from vizier._src.service import resources
+from vizier._src.service import study_pb2
+from vizier._src.service import vizier_service
+from vizier._src.service import vizier_service_pb2
+from vizier._src.service.testing import util as test_util
 
 from google.longrunning import operations_pb2
 
 from absl.testing import absltest
 from absl.testing import parameterized
 
 UnitMetadataUpdate = vizier_service_pb2.UnitMetadataUpdate
@@ -37,15 +39,16 @@
 
 class VizierServicerTest(parameterized.TestCase):
 
   def setUp(self):
     # TODO: Find a way to cleanly test both datastores.
     self.early_stop_recycle_period = datetime.timedelta(seconds=0.1)
     self.vs = vizier_service.VizierServicer(
-        early_stop_recycle_period=self.early_stop_recycle_period
+        database_url=constants.SQL_MEMORY_URL,
+        early_stop_recycle_period=self.early_stop_recycle_period,
     )
     self.owner_id = 'my_username'
     self.study_id = '0123123'
     self.client_id = 'client_0'
     super().setUp()
 
   @parameterized.named_parameters(
```

### Comparing `google-vizier-0.1.4/vizier/testing/__init__.py` & `google-vizier-0.1.5/vizier/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/testing/test_studies.py` & `google-vizier-0.1.5/vizier/testing/test_studies.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 """Test study generator."""
 
-from typing import Collection
+from typing import List
 from vizier import pyvizier as vz
 
 
 def flat_continuous_space_with_scaling() -> vz.SearchSpace:
   """Search space with all parameter types."""
 
   space = vz.SearchSpace()
@@ -44,40 +44,40 @@
   root.add_discrete_param(
       'discrete_logdouble', [1e-5, 1e-2, 1e-1], scale_type=vz.ScaleType.LOG)
   root.add_discrete_param('discrete_int', [-1, 1, 2])
 
   return space
 
 
-def metrics_objective_goals() -> Collection[vz.MetricInformation]:
+def metrics_objective_goals() -> List[vz.MetricInformation]:
   return [
       vz.MetricInformation('gain', goal=vz.ObjectiveMetricGoal.MAXIMIZE),
       vz.MetricInformation('loss', goal=vz.ObjectiveMetricGoal.MINIMIZE),
       vz.MetricInformation(
           'auc',
           goal=vz.ObjectiveMetricGoal.MAXIMIZE,
           min_value=0.0,
           max_value=1.0),
       vz.MetricInformation(
           'crossentropy', goal=vz.ObjectiveMetricGoal.MINIMIZE, min_value=0.0),
   ]
 
 
-def metrics_all_unconstrained() -> Collection[vz.MetricInformation]:
+def metrics_all_unconstrained() -> List[vz.MetricInformation]:
   return [
       vz.MetricInformation('gain', goal=vz.ObjectiveMetricGoal.MAXIMIZE),
       vz.MetricInformation('loss', goal=vz.ObjectiveMetricGoal.MINIMIZE),
       vz.MetricInformation(
           'gt2', goal=vz.ObjectiveMetricGoal.MAXIMIZE, safety_threshold=2.0),
       vz.MetricInformation(
           'lt2', goal=vz.ObjectiveMetricGoal.MINIMIZE, safety_threshold=2.0),
   ]
 
 
-def metrics_all_constrained() -> Collection[vz.MetricInformation]:
+def metrics_all_constrained() -> List[vz.MetricInformation]:
   return [
       vz.MetricInformation(
           'auc',
           goal=vz.ObjectiveMetricGoal.MAXIMIZE,
           min_value=0.0,
           max_value=1.0),
       vz.MetricInformation(
```

### Comparing `google-vizier-0.1.4/vizier/utils/attrs_utils.py` & `google-vizier-0.1.5/vizier/utils/attrs_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/utils/attrs_utils_test.py` & `google-vizier-0.1.5/vizier/utils/attrs_utils_test.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/utils/json_utils.py` & `google-vizier-0.1.5/vizier/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `google-vizier-0.1.4/vizier/utils/json_utils_test.py` & `google-vizier-0.1.5/vizier/utils/json_utils_test.py`

 * *Files identical despite different names*

