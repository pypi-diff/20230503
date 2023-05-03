# Comparing `tmp/credoai-lens-1.1.7.tar.gz` & `tmp/credoai-lens-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credoai-lens-1.1.7.tar", last modified: Wed Mar 29 21:16:55 2023, max compression
+gzip compressed data, was "credoai-lens-1.1.8.tar", last modified: Wed May  3 00:46:18 2023, max compression
```

## Comparing `credoai-lens-1.1.7.tar` & `credoai-lens-1.1.8.tar`

### file list

```diff
@@ -1,135 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.245301 credoai-lens-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-03-29 21:16:55.245301 credoai-lens-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.233301 credoai-lens-1.1.7/credoai/
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.233301 credoai-lens-1.1.7/credoai/artifacts/
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.233301 credoai-lens-1.1.7/credoai/artifacts/data/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/artifacts/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8793 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/artifacts/data/base_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6867 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/artifacts/data/comparison_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3755 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/artifacts/data/tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.233301 credoai-lens-1.1.7/credoai/artifacts/model/
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/artifacts/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3239 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/artifacts/model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    10616 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/artifacts/model/classification_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/artifacts/model/comparison_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/artifacts/model/constants_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/artifacts/model/regression_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.233301 credoai-lens-1.1.7/credoai/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     4261 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/_fetch_censusincome.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/_fetch_credit_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/_fetch_creditdefault.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/_fetch_testdata.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.233301 credoai-lens-1.1.7/credoai/datasets/static/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.233301 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.233301 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/persisted_models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/persisted_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/persisted_models/lr_toxicity.joblib
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.237301 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   208292 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/bold_gender.csv
--rw-r--r--   0 runner    (1001) docker     (122)   155135 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/bold_political_ideology.csv
--rw-r--r--   0 runner    (1001) docker     (122)   808673 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/bold_profession.csv
--rw-r--r--   0 runner    (1001) docker     (122)   616482 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/bold_race.csv
--rw-r--r--   0 runner    (1001) docker     (122)    44387 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/bold_religious_ideology.csv
--rw-r--r--   0 runner    (1001) docker     (122)     7433 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/bold_religious_ideology_short.csv
--rw-r--r--   0 runner    (1001) docker     (122)    13770 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/conversationai_age.csv
--rw-r--r--   0 runner    (1001) docker     (122)     8182 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/conversationai_disability.csv
--rw-r--r--   0 runner    (1001) docker     (122)     8330 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/conversationai_gender.csv
--rw-r--r--   0 runner    (1001) docker     (122)    10754 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/conversationai_race.csv
--rw-r--r--   0 runner    (1001) docker     (122)    16786 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/conversationai_religious_ideology.csv
--rw-r--r--   0 runner    (1001) docker     (122)    18266 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/conversationai_sexual_orientation.csv
--rw-r--r--   0 runner    (1001) docker     (122)   313731 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/realtoxicityprompts_1000.csv
--rw-r--r--   0 runner    (1001) docker     (122)   108574 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/realtoxicityprompts_challenging.csv
--rw-r--r--   0 runner    (1001) docker     (122)     9590 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/realtoxicityprompts_challenging_100.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/static/nlp_generator_analyzer/prompts/realtoxicityprompts_challenging_20.csv
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.241301 credoai-lens-1.1.7/credoai/evaluators/
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18352 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/data_fairness.py
--rw-r--r--   0 runner    (1001) docker     (122)     3655 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/data_profiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5037 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/deepchecks_credoai.py
--rw-r--r--   0 runner    (1001) docker     (122)    10686 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/equity.py
--rw-r--r--   0 runner    (1001) docker     (122)     6324 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (122)    10384 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/fairness.py
--rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/feature_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)    17050 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/identity_verification.py
--rw-r--r--   0 runner    (1001) docker     (122)     9699 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/model_profiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     7899 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/performance.py
--rw-r--r--   0 runner    (1001) docker     (122)    16177 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/privacy.py
--rw-r--r--   0 runner    (1001) docker     (122)    17870 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/ranking_fairness.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/security.py
--rw-r--r--   0 runner    (1001) docker     (122)    10754 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/shap_credoai.py
--rw-r--r--   0 runner    (1001) docker     (122)     3956 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/survival_fairness.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.241301 credoai-lens-1.1.7/credoai/evaluators/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3198 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/utils/fairlearn.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5105 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/evaluators/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.241301 credoai-lens-1.1.7/credoai/governance/
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/governance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.241301 credoai-lens-1.1.7/credoai/lens/
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/lens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18493 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/lens/lens.py
--rw-r--r--   0 runner    (1001) docker     (122)     7943 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/lens/lens_validation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/lens/pipeline_creator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/lens/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.241301 credoai-lens-1.1.7/credoai/modules/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      375 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/modules/constants_deepchecks.py
--rw-r--r--   0 runner    (1001) docker     (122)     6772 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/modules/constants_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/modules/constants_threshold_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/modules/metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/modules/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)    22262 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/modules/metrics_credoai.py
--rw-r--r--   0 runner    (1001) docker     (122)     8173 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/modules/stats.py
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/modules/stats_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.241301 credoai-lens-1.1.7/credoai/prism/
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/prism/compare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2428 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/prism/prism.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/prism/task.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.241301 credoai-lens-1.1.7/credoai/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     5248 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2262 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     4649 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2856 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/utils/policy_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/credoai/utils/version_check.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.241301 credoai-lens-1.1.7/credoai_lens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-03-29 21:16:55.000000 credoai-lens-1.1.7/credoai_lens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4510 2023-03-29 21:16:55.000000 credoai-lens-1.1.7/credoai_lens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-29 21:16:55.000000 credoai-lens-1.1.7/credoai_lens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      990 2023-03-29 21:16:55.000000 credoai-lens-1.1.7/credoai_lens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-29 21:16:55.000000 credoai-lens-1.1.7/credoai_lens.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.241301 credoai-lens-1.1.7/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-29 21:16:55.245301 credoai-lens-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2413 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.245301 credoai-lens-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:55.245301 credoai-lens-1.1.7/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/fixtures/datasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1945 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/fixtures/frozen_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/fixtures/lens_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4773 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/fixtures/lens_inits.py
--rw-r--r--   0 runner    (1001) docker     (122)     2328 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (122)     8460 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/test_binary_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/test_frozen_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/test_multiclass_classification.py
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/test_prism.py
--rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/test_quickstart.py
--rw-r--r--   0 runner    (1001) docker     (122)     1708 2023-03-29 21:16:47.000000 credoai-lens-1.1.7/tests/test_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.304643 credoai-lens-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-05-03 00:46:18.304643 credoai-lens-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.284642 credoai-lens-1.1.8/credoai/
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.284642 credoai-lens-1.1.8/credoai/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.284642 credoai-lens-1.1.8/credoai/artifacts/data/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/artifacts/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8777 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/artifacts/data/base_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6867 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/artifacts/data/comparison_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3755 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/artifacts/data/tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.284642 credoai-lens-1.1.8/credoai/artifacts/model/
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/artifacts/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3239 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/artifacts/model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10616 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/artifacts/model/classification_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/artifacts/model/comparison_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/artifacts/model/constants_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/artifacts/model/regression_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.288642 credoai-lens-1.1.8/credoai/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/datasets/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4261 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/datasets/_fetch_censusincome.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/datasets/_fetch_credit_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4447 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/datasets/_fetch_creditdefault.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/datasets/_fetch_testdata.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.288642 credoai-lens-1.1.8/credoai/datasets/static/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/datasets/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.288642 credoai-lens-1.1.8/credoai/datasets/static/nlp_generator_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/datasets/static/nlp_generator_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.288642 credoai-lens-1.1.8/credoai/datasets/static/nlp_generator_analyzer/persisted_models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/datasets/static/nlp_generator_analyzer/persisted_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.288642 credoai-lens-1.1.8/credoai/datasets/static/nlp_generator_analyzer/prompts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/datasets/static/nlp_generator_analyzer/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.292642 credoai-lens-1.1.8/credoai/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18834 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/data_fairness.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4037 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/data_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5823 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/deepchecks_credoai.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11776 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/equity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6324 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10957 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/fairness.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/feature_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17511 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/identity_verification.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10085 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/model_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8351 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/performance.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16693 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/privacy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18080 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/ranking_fairness.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11457 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/security.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11205 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/shap_credoai.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4529 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/survival_fairness.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.292642 credoai-lens-1.1.8/credoai/evaluators/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3198 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/utils/fairlearn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5105 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/evaluators/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.292642 credoai-lens-1.1.8/credoai/governance/
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/governance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.292642 credoai-lens-1.1.8/credoai/lens/
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/lens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18493 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/lens/lens.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7943 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/lens/lens_validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/lens/pipeline_creator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/lens/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.296642 credoai-lens-1.1.8/credoai/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/modules/constants_deepchecks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6772 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/modules/constants_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/modules/constants_threshold_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/modules/metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/modules/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22284 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/modules/metrics_credoai.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8275 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/modules/stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/modules/stats_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.296642 credoai-lens-1.1.8/credoai/prism/
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/prism/compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2428 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/prism/prism.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/prism/task.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.300643 credoai-lens-1.1.8/credoai/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5248 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2262 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4649 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2856 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/utils/policy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/credoai/utils/version_check.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.300643 credoai-lens-1.1.8/credoai_lens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-05-03 00:46:18.000000 credoai-lens-1.1.8/credoai_lens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-05-03 00:46:18.000000 credoai-lens-1.1.8/credoai_lens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 00:46:18.000000 credoai-lens-1.1.8/credoai_lens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-05-03 00:46:18.000000 credoai-lens-1.1.8/credoai_lens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-03 00:46:18.000000 credoai-lens-1.1.8/credoai_lens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.300643 credoai-lens-1.1.8/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-03 00:46:18.304643 credoai-lens-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2511 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.300643 credoai-lens-1.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:18.304643 credoai-lens-1.1.8/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/fixtures/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1945 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/fixtures/frozen_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/fixtures/lens_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4773 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/fixtures/lens_inits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2328 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8460 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/test_binary_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/test_frozen_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/test_multiclass_classification.py
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/test_prism.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/test_quickstart.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1708 2023-05-03 00:46:10.000000 credoai-lens-1.1.8/tests/test_regression.py
```

### Comparing `credoai-lens-1.1.7/PKG-INFO` & `credoai-lens-1.1.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: credoai-lens
-Version: 1.1.7
-Summary: Lens: comprehensive assessment framework for AI systems
-Home-page: 
-Download-URL: https://github.com/credo-ai/credoai_lens
-Author: Ian Eisenberg
-Author-email: ian@credo.ai
-Maintainer: Ian Eisenberg
-Maintainer-email: ian@credo.ai
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: full
-License-File: LICENSE
-
 <img src="https://raw.githubusercontent.com/credo-ai/credoai_lens/develop/docs/_static/images/credo_ai-lens.png" width="250" alt="Credo AI Lens"><br>
 
 ![Workflow](https://github.com/credo-ai/credoai_lens/actions/workflows/test-reports.yml/badge.svg)
 ![Tests](https://credoai-cicd-public-artifacts.s3.us-west-2.amazonaws.com/credoai_lens/main/tests-badge.svg)
 [![Coverage](https://credoai-cicd-public-artifacts.s3.us-west-2.amazonaws.com/credoai_lens/main/coverage-badge.svg)](https://credoai-cicd-public-artifacts.s3.us-west-2.amazonaws.com/credoai_lens/main/html/index.html)
 
 --------------------------------------
@@ -55,18 +33,17 @@
 
 The latest stable release (and required dependencies) can be installed from PyPI.
 
 ```
 pip install credoai-lens
 ```
 
-Additional installation instructions can be found in our [setup documentation](https://credoai-lens.readthedocs.io/en/stable/notebooks/quickstart.html)
+Additional installation instructions can be found in our [setup documentation](https://credoai-lens.readthedocs.io/en/stable/pages/setup.html)
 
 ## Getting Started
-
 To get started, see the [quickstart demo](https://credoai-lens.readthedocs.io/en/stable/notebooks/quickstart.html).
 
 If you are using the Credo AI Governance App, also check out the [governance integration demo](https://credoai-lens.readthedocs.io/en/stable/notebooks/governance_integration.html).
 
 ## Documentation
 
 Documentation is hosted by [readthedocs](https://credoai-lens.readthedocs.io/en/stable/).
```

### Comparing `credoai-lens-1.1.7/credoai/artifacts/__init__.py` & `credoai-lens-1.1.8/credoai/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/artifacts/data/base_data.py` & `credoai-lens-1.1.8/credoai/artifacts/data/base_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Abstract class for the data artifacts used by `Lens`"""
 # Data is a lightweight wrapper that stores data
 import itertools
 from copy import deepcopy
 from typing import Optional, Union
 
-import pandas as pd
 import numpy as np
+import pandas as pd
 
 from credoai.utils import global_logger
 from credoai.utils.common import ValidationError, check_pandas
 from credoai.utils.model_utils import type_of_target
 
 
 class Data:
@@ -214,32 +214,32 @@
         pass
 
     def _validate_processed_y(self):
         pass
 
     def _validate_processed_sensitive(self):
         """Validation of processed sensitive features"""
-        for col_name, col in self.sensitive_features.iteritems():
+        for col_name, col in self.sensitive_features.items():
             # validate unique
             unique_values = col.unique()
             if len(unique_values) == 1:
                 raise ValidationError(
                     f"Sensitive Feature column {col_name} must have more "
                     f"than one unique value. Only found one value: {unique_values[0]}"
                 )
             # validate number in each group
-            for group, value in col.value_counts().iteritems():
+            for group, value in col.value_counts().items():
                 if value < 10:
                     global_logger.warning(
                         f"Dataset Issue! Very few ({value}) records were found for {group} under sensitive feature {col_name}."
                     )
             # validate variance in y
             if self.y is not None:
                 y = pd.DataFrame(self.y)
-                for outcome, outcome_col in y.iteritems():
-                    for group, value in outcome_col.groupby(col).nunique().iteritems():
+                for outcome, outcome_col in y.items():
+                    for group, value in outcome_col.groupby(col).nunique().items():
                         if not np.all(value):
                             global_logger.warning(
                                 "%s\n%s",
                                 f"Dataset Issue! Zero variance in the outcome ({outcome}) detected for {group} under sensitive feature {col_name}.",
                                 "\tDownstream evaluators may fail or not perform as expected.",
                             )
```

### Comparing `credoai-lens-1.1.7/credoai/artifacts/data/comparison_data.py` & `credoai-lens-1.1.8/credoai/artifacts/data/comparison_data.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/artifacts/data/tabular_data.py` & `credoai-lens-1.1.8/credoai/artifacts/data/tabular_data.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/artifacts/model/base_model.py` & `credoai-lens-1.1.8/credoai/artifacts/model/base_model.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/artifacts/model/classification_model.py` & `credoai-lens-1.1.8/credoai/artifacts/model/classification_model.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/artifacts/model/comparison_model.py` & `credoai-lens-1.1.8/credoai/artifacts/model/comparison_model.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/artifacts/model/constants_model.py` & `credoai-lens-1.1.8/credoai/artifacts/model/constants_model.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/artifacts/model/regression_model.py` & `credoai-lens-1.1.8/credoai/artifacts/model/regression_model.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/datasets/_fetch_censusincome.py` & `credoai-lens-1.1.8/credoai/datasets/_fetch_censusincome.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/datasets/_fetch_credit_model.py` & `credoai-lens-1.1.8/credoai/datasets/_fetch_credit_model.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/datasets/_fetch_creditdefault.py` & `credoai-lens-1.1.8/credoai/datasets/_fetch_creditdefault.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/datasets/_fetch_testdata.py` & `credoai-lens-1.1.8/credoai/datasets/_fetch_testdata.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/datasets/utils.py` & `credoai-lens-1.1.8/credoai/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/evaluators/data_fairness.py` & `credoai-lens-1.1.8/credoai/evaluators/data_fairness.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,33 +40,43 @@
 
     This evaluator performs a fairness evaluation on the dataset. Given a sensitive feature,
     it calculates a number of assessments:
 
     - group differences of features
     - evaluates whether features in the dataset are proxies for the sensitive feature
     - whether the entire dataset can be seen as a proxy for the sensitive feature
-      (i.e., the sensitive feature is "redundantly encoded")
+    (i.e., the sensitive feature is "redundantly encoded")
+
+    Required Artifacts
+    ------------------
+        **Required Artifacts**
+
+        Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+        handles evaluator setup. However, if you are using the evaluator directly, you
+        will need to pass the following artifacts when instantiating the evaluator:
+
+        - data: :class:`credoai.artifacts.TabularData`
+            The data to evaluate, which must include a sensitive feature
 
     Parameters
     ----------
     categorical_features_keys : list[str], optional
         Names of the categorical features
     categorical_threshold : float
         Parameter for automatically identifying categorical columns. See
-        `credoai.utils.common.is_categorical`
+        :class:`credoai.utils.common.is_categorical` for more details.
     """
 
     required_artifacts = {"data", "sensitive_feature"}
 
     def __init__(
         self,
         categorical_features_keys: Optional[List[str]] = None,
         categorical_threshold: float = 0.05,
     ):
-
         self.categorical_features_keys = categorical_features_keys
         self.categorical_threshold = categorical_threshold
         super().__init__()
 
     def _validate_arguments(self):
         check_data_instance(self.data, TabularData)
         check_existence(self.data.sensitive_features, "sensitive_features")
@@ -216,15 +226,15 @@
         -------
         list
             Names of categorical features
         """
         if is_categorical(self.sensitive_features, threshold=threshold):
             self.sensitive_features = self.sensitive_features.astype("category")
         cat_cols = []
-        for name, column in self.X.iteritems():
+        for name, column in self.X.items():
             if is_categorical(column, threshold=threshold):
                 cat_cols.append(name)
         return cat_cols
 
     def _calculate_mutual_information(self, normalize=True):
         """
         Calculates normalized mutual information between sensitive feature and other features.
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/data_profiler.py` & `credoai-lens-1.1.8/credoai/evaluators/data_profiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 from credoai.artifacts.data.base_data import Data
 from credoai.evaluators.evaluator import Evaluator
 from credoai.evaluators.utils import check_data_instance
 from credoai.utils.common import ValidationError, check_pandas
 
 backend = matplotlib.get_backend()
-# load pands profiler, which sets backend to Agg
-from pandas_profiling import ProfileReport
+# load ydata profiler, which sets backend to Agg
+from ydata_profiling import ProfileReport
 
 matplotlib.use(backend)
 
 
 class DataProfiler(Evaluator):
     """
     Data profiling evaluator for Credo AI
@@ -25,15 +25,24 @@
     of descriptive statistics about the data. The DataProfiler can only be run on parts of the
     data that are pandas objects (dataframes or series). E.g., if X is a multi-dimensional
     array, X will NOT be profiled.
 
     Parameters
     ----------
     profile_kwargs
-        Potential arguments to be passed to pandas_profiling.ProfileReport
+        Potential arguments to be passed to ydata_profiling.ProfileReport
+
+    Required Artifacts
+    ------------------
+    Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+    handles evaluator setup. However, if you are using the evaluator directly, you
+    will need to pass the following artifacts when instantiating the evaluator:
+
+    data : TabularData
+        The data to evaluate, which must include a sensitive feature
     """
 
     required_artifacts = {"data"}
 
     def __init__(self, **profile_kwargs):
         self.profile_kwargs = profile_kwargs
         super().__init__()
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/deepchecks_credoai.py` & `credoai-lens-1.1.8/credoai/evaluators/deepchecks_credoai.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,14 +23,29 @@
     This evaluator provides some redundant functionality. For instance, metrics which can be
     calculated using the Performance evaluator can potentially be calculated by deepchecks
     (and thus this evaluator) as well. The same applies to the FeatureDrift evaluator.
     When a choice exists, the best practice dictates that the "Lens native" evaluator should
     be used in preference to deepchecks, since output formats of other evaluators is generally
     consistent, while this deepchecks evaluator outputs results in a highly structured JSON format.
 
+    Required Artifacts
+    ------------------
+        **Required Artifacts**
+
+        Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+        handles evaluator setup. However, if you are using the evaluator directly, you
+        will need to pass **at least one** of the following artifacts when instantiating the evaluator:
+
+        - model: :class:`credoai.artifacts.Model` or :class:`credoai.artifacts.RegressionModel`
+        - assessment_data: :class:`credoai.artifacts.TabularData`
+            The assessment data to evaluate. Assessment data is used to calculate metrics
+            on the model.
+        - training_data: :class:`credoai.artifacts.TabularData`
+            The training data to evaluate. The training data was used to tran the model
+
 
     Parameters
     ----------
     suite_name : str, optional
         Name of the supplied deepchecks suite
     checks : List[BaseCheck], optional
         A list of instantiated deepchecks checks objects (e.g. BoostingOverfit, CalibrationScore)
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/equity.py` & `credoai-lens-1.1.8/credoai/evaluators/equity.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,27 @@
 
     - Discrete: chi-squared contingency tests,
       followed by bonferronni corrected posthoc chi-sq tests
     - Continuous: One-way ANOVA, followed by Tukey HSD posthoc tests
     - Proportion (Bounded [0-1] continuous outcome): outcome is transformed to logits, then
       proceed as normal for continuous
 
+    Required Artifacts
+    ------------------
+    **Required Artifacts**
+
+    Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+    handles evaluator setup. However, if you are using the evaluator directly, you
+    will need to pass the following artifacts when instantiating the evaluator:
+
+    - data: :class:`credoai.artifacts.TabularData`
+        The data to evaluate for equity (based on the outcome variable). Must
+        have sensitive feature defined.
+
+
     Parameters
     ----------
     p_value : float
         The significance value to evaluate statistical tests
     """
 
     required_artifacts = {"data", "sensitive_feature"}
@@ -186,22 +199,36 @@
 
 
 class ModelEquity(DataEquity):
     """
     Evaluates the equity of a model's predictions.
 
     This evaluator assesses whether model predictions are distributed equally across a sensitive
-    feature. Depending on the kind of outcome, different tests will be performed.
+    feature. Depending on the kind of outcome, different tests will be performed:
 
-    * Discrete: chi-squared contingency tests,
+    - Discrete: chi-squared contingency tests,
       followed by bonferronni corrected posthoc chi-sq tests
-    * Continuous: One-way ANOVA, followed by Tukey HSD posthoc tests
-    * Proportion (Bounded [0-1] continuous outcome): outcome is transformed to logits, then
+    - Continuous: One-way ANOVA, followed by Tukey HSD posthoc tests
+    - Proportion (Bounded [0-1] continuous outcome): outcome is transformed to logits, then
       proceed as normal for continuous
 
+    Required Artifacts
+    ------------------
+        **Required Artifacts**
+
+        Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+        handles evaluator setup. However, if you are using the evaluator directly, you
+        will need to pass the following artifacts when instantiating the evaluator:
+
+        - model: :class:`credoai.artifacts.Model`
+        - assessment_data: :class:`credoai.artifacts.TabularData`
+            The assessment data to use to create model predictions and evaluate
+            the equity of the model. Must have sensitive features.
+
+
     Parameters
     ----------
     use_predict_proba : bool, optional
         Defines which predict method will be used, if True predict_proba will be used.
         This methods outputs probabilities rather then class predictions. The availability
         of predict_proba is dependent on the model under assessment. By default False
     p_value : float, optional
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/evaluator.py` & `credoai-lens-1.1.8/credoai/evaluators/evaluator.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/evaluators/fairness.py` & `credoai-lens-1.1.8/credoai/evaluators/fairness.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,25 @@
 
     This evaluator calculates performance metrics disaggregated by a sensitive feature, as
     well as evaluating the parity of those metrics.
 
     Handles any metric that can be calculated on a set of ground truth labels and predictions,
     e.g., binary classification, multiclass classification, regression.
 
+    Required Artifacts
+    ------------------
+        **Required Artifacts**
+
+        Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+        handles evaluator setup. However, if you are using the evaluator directly, you
+        will need to pass the following artifacts when instantiating the evaluator:
+
+        - model: :class:`credoai.artifacts.Model` or :class:`credoai.artifacts.RegressionModel`
+        - data: :class:`credoai.artifacts.TabularData`
+            The data to use for fairness evaluation. Must include a sensitive feature.
 
     Parameters
     ----------
     metrics : List-like
         list of metric names as string or list of Metrics (credoai.metrics.Metric).
         Metric strings should in list returned by credoai.modules.list_metrics.
         Note for performance parity metrics like
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/feature_drift.py` & `credoai-lens-1.1.8/credoai/evaluators/feature_drift.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,26 @@
 
        - Numerical features are directly fed into the population_stability_index metric, and
          binned according to the parameters specified at init time.
        - Categorical features percentage distribution is manually calculated. The % amount of
          samples per each class is calculated and then fed into the population_stability_index metric.
          The percentage flag in the metric is set to True, to bypass the internal binning process.
 
+    Required Artifacts
+    ------------------
+        **Required Artifacts**
+
+        Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+        handles evaluator setup. However, if you are using the evaluator directly, you
+        will need to pass the following artifacts when instantiating the evaluator:
+
+        - model: :class:`credoai.artifacts.Model`
+        - assessment_data: :class:`credoai.artifacts.TabularData`
+        - training_data: :class:`credoai.artifacts.TabularData`
+
 
     Parameters
     ----------
     buckets : int, optional
         Number of buckets to consider to bin the predictions, by default 10
     buckettype :  Literal["bins", "quantiles"]
         Type of strategy for creating buckets, bins splits into even splits,
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/identity_verification.py` & `credoai-lens-1.1.8/credoai/evaluators/identity_verification.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,25 @@
 class IdentityVerification(Evaluator):
     """
     Pair-wise-comparison-based identity verification evaluator for Credo AI (Experimental)
 
     This evaluator takes in identity verification data and
     provides functionality to perform performance and fairness assessment
 
+    Required Artifacts
+    ------------------
+        **Required Artifacts**
+
+        Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+        handles evaluator setup. However, if you are using the evaluator directly, you
+        will need to pass the following artifacts when instantiating the evaluator:
+
+        model: :class:`credoai.artifacts.ComparisonModel`
+        assessment_data: :class:`credoai.artifacts.ComparisonData`
+
     Parameters
     ----------
     pairs : pd.DataFrame of shape (n_pairs, 4)
         Dataframe where each row represents a data sample pair and associated subjects
         Type of data sample is decided by the ComparisonModel's `compare` function, which takes
         data sample pairs and returns their similarity scores. Examples are selfies, fingerprint scans,
         or voices of a person.
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/model_profiler.py` & `credoai-lens-1.1.8/credoai/evaluators/model_profiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,24 @@
     1. Extract all potentially useful info from the model itself in an
        automatic fashion.
     2. Allow the user to personalize the model card freely.
 
     The method generate_template() provides a dictionary with several entries the
     user could be interested in filling up.
 
+    Required Artifacts
+    ------------------
+        **Required Artifacts**
+
+        Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+        handles evaluator setup. However, if you are using the evaluator directly, you
+        will need to pass the following artifacts when instantiating the evaluator:
+
+        - model: :class:`credoai.artifacts.Model`
+
     Parameters
     ----------
     model_info : Optional[dict]
         Information provided by the user that cannot be inferred by
         the model itself. The dictionary con contain any number of elements,
         a template can be provided by running the generate_template() method.
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/performance.py` & `credoai-lens-1.1.8/credoai/evaluators/performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,25 @@
     e.g., binary classification, multi class classification, regression.
 
     This module takes in a set of metrics and provides functionality to:
 
     - calculate the metrics
     - create disaggregated metrics
 
+    Required Artifacts
+    ------------------
+        **Required Artifacts**
+
+        Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+        handles evaluator setup. However, if you are using the evaluator directly, you
+        will need to pass the following artifacts when instantiating the evaluator:
+
+        - model: :class:`credoai.artifacts.Model`
+        - assessment_data: :class:`credoai.artifacts.TabularData`
+
     Parameters
     ----------
     metrics : List-like
         list of metric names as strings or list of Metric objects (credoai.modules.metrics.Metric).
         Metric strings should in list returned by credoai.modules.metric_utils.list_metrics().
         Note for performance parity metrics like
         "false negative rate parity" just list "false negative rate". Parity metrics
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/privacy.py` & `credoai-lens-1.1.8/credoai/evaluators/privacy.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,26 @@
     * `Attribute Inference Baseline`_: Trains a neural network to learn the attacked feature from the other features.
     * `Attribute Inference BlackBox`_: Trains a neural network to learn the attacked feature from the other features and
       the model's prediction.
     * `Membership Inference BlackBox`_: Trains a neural network to assess if some records were used for the model training.
     * `Membership Inference BlackBox Rule Based`_: Use a simple rule based approach to assess if some records
       were used for the model training.
 
+    Required Artifacts
+    ------------------
+        **Required Artifacts**
+
+        Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+        handles evaluator setup. However, if you are using the evaluator directly, you
+        will need to pass the following artifacts when instantiating the evaluator:
+
+        - model: :class:`credoai.artifacts.Model`
+        - assessment_data: :class:`credoai.artifacts.TabularData`
+        - training_data: :class:`credoai.artifacts.TabularData`
+
     Parameters
     ----------
     attack_feature : Union[str, int, None], optional
         Either the name or the column number of the feature to be attacked. If the column
         number is provided, the following parameter `attack_feature_name` needs to be provided.
         Default is None, in this case no attack feature is performed.
     attack_feature_name : Optional[str], optional
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/ranking_fairness.py` & `credoai-lens-1.1.8/credoai/evaluators/ranking_fairness.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 ]
 
 
 class RankingFairness(Evaluator):
     """
     Ranking fairness evaluator for Credo AI (Experimental)
 
-    This module takes in ranking results and provides functionality to perform fairness assessment
+    This module takes in ranking results (an outcome column of scores representing the ranking
+    of items or people) and provides functionality to perform fairness assessment
     The results should include rankings, sensitive features, and optionally, scores.
 
     The scores that the evaluator can calculate are:
 
     * **skew_parity_difference**: max_skew - min_skew, where skew is the proportion of the selected
       items from a group over the desired proportion for that group.
       It ranges from 0 to inf and the ideal value is 0.
@@ -89,25 +90,29 @@
     * **score_balance_ratio**: min_total_Score / max_total_Score, where total score
       is the total score of the selected items from a group. It ranges from 0 to 1 and ideal value is 1.
 
     * **score_empirical_distribution**: score empirical distributions for each demographic group as tables.
       The x axis is scores and the y axis is cumulative probabilities (ranges from 0 to 1)
       It is useful for a visual examination of the distribution of scores for the different groups.
 
+    Required Artifacts
+    ------------------
+        **Required Artifacts**
+
+        Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+        handles evaluator setup. However, if you are using the evaluator directly, you
+        will need to pass the following artifacts when instantiating the evaluator:
+
+        - data: :class:`credoai.artifacts.TabularData`
+            A dataset with rankings. The y variable should be a dataframe or series with
+            a "rankings" column (int) and (optionally) a "scores" column (int or float).
+            The data must also have sensitive features.
+
     Parameters
     ----------
-    sensitive_features : pandas.Series
-        A series of the sensitive feature labels (e.g., "male", "female") which should
-        be used to create subgroups
-    rankings : pandas.Series of type int
-        The computed ranks
-        It should be passed to TabularData's y argument with the column name `rankings`
-    scores : pandas.Series of type int or float, Optional
-        A series of the scores
-        It should be passed to TabularData's y argument with the column name `scores`
     k: int, Optional
         The top k items are considered as the selected subset
         If not provided, the top 50% of the items are considered as selected
     q: float, Optional
         The relevance score for which items in the pool that have score >= q are "relevant".
         These two metrics require this to be provided: `qualified_demographic_parity_ratio`
         and `qualified_balance_ratio`
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/security.py` & `credoai-lens-1.1.8/credoai/evaluators/security.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,26 @@
     (click on the links for more details):
 
     1. `Evasion Attack`_: attempts to create a set of samples that will be
        misclassified by the model
     2. `Extraction Attack`_: attempts to infer enough information from the model
        prediction to train a substitutive model.
 
+    Required Artifacts
+    ------------------
+        **Required Artifacts**
+
+        Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+        handles evaluator setup. However, if you are using the evaluator directly, you
+        will need to pass the following artifacts when instantiating the evaluator:
+
+        - model: :class:`credoai.artifacts.Model`
+        - assessment_data: :class:`credoai.artifacts.TabularData`
+        - training_data: :class:`credoai.artifacts.TabularData`
+
     Parameters
     ----------
     model : model
         A trained binary or multi-class classification model
         The only requirement for the model is to have a `predict` function that returns
         predicted classes for a given feature vectors as a one-dimensional array.
     x_train : pandas.DataFrame
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/shap_credoai.py` & `credoai-lens-1.1.8/credoai/evaluators/shap_credoai.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,24 @@
 
     There is no agreement as to what is the best strategy as far as categorical variables are
     concerned. A good discussion on this can be found here: https://github.com/slundberg/shap/issues/451
 
     No restriction on feature type is imposed by the evaluator, so user discretion in the
     interpretation of shap values for categorical variables is advised.
 
+    Required Artifacts
+    ------------------
+        **Required Artifacts**
+
+        Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+        handles evaluator setup. However, if you are using the evaluator directly, you
+        will need to pass the following artifacts when instantiating the evaluator:
+
+        - model: :class:`credoai.artifacts.Model`
+        - assessment_data: :class:`credoai.artifacts.TabularData`
 
     Parameters
     ----------
     samples_ind : Optional[List[int]], optional
         List of row numbers representing the samples for which to extract individual
         shapley values. This must be a list of integer indices. The underlying SHAP
         library does not support non-integer indexing.
@@ -66,15 +76,15 @@
         If True, use SHAP kmeans to create a data summary to serve as background data for the
         SHAP explainer using 50 centroids by default. If an int is provided,
         that will be used as the number of centroids. If False, random sampling will take place.
 
 
     """
 
-    required_artifacts = ["assessment_data", "model"]
+    required_artifacts = ["model", "assessment_data"]
 
     def __init__(
         self,
         samples_ind: Optional[List[int]] = None,
         background_samples: int = 100,
         background_kmeans: Union[bool, int] = False,
     ):
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/survival_fairness.py` & `credoai-lens-1.1.8/credoai/evaluators/survival_fairness.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,27 @@
 from credoai.utils import ValidationError
 
 
 class SurvivalFairness(Evaluator):
     """
     Calculate Survival fairness (Experimental)
 
+    Required Artifacts
+    ------------------
+        **Required Artifacts**
+
+        Generally artifacts are passed directly to :class:`credoai.lens.Lens`, which
+        handles evaluator setup. However, if you are using the evaluator directly, you
+        will need to pass the following artifacts when instantiating the evaluator:
+
+        - model: :class:`credoai.artifacts.Model`
+        - assessment_data: :class:`credoai.artifacts.TabularData`
+            Assessment data must have sensitive features
+        - training_data: :class:`credoai.artifacts.TabularData`
+
     Parameters
     ----------
         CoxPh_kwargs : _type_, optional
             _description_, by default None
         confounds : _type_, optional
             _description_, by default None
```

### Comparing `credoai-lens-1.1.7/credoai/evaluators/utils/fairlearn.py` & `credoai-lens-1.1.8/credoai/evaluators/utils/fairlearn.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/evaluators/utils/utils.py` & `credoai-lens-1.1.8/credoai/evaluators/utils/utils.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/evaluators/utils/validation.py` & `credoai-lens-1.1.8/credoai/evaluators/utils/validation.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/lens/lens.py` & `credoai-lens-1.1.8/credoai/lens/lens.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/lens/lens_validation.py` & `credoai-lens-1.1.8/credoai/lens/lens_validation.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/lens/pipeline_creator.py` & `credoai-lens-1.1.8/credoai/lens/pipeline_creator.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/lens/utils.py` & `credoai-lens-1.1.8/credoai/lens/utils.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/modules/constants_metrics.py` & `credoai-lens-1.1.8/credoai/modules/constants_metrics.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/modules/constants_threshold_metrics.py` & `credoai-lens-1.1.8/credoai/modules/constants_threshold_metrics.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/modules/metric_utils.py` & `credoai-lens-1.1.8/credoai/modules/metric_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import textwrap
 from collections import defaultdict
 
-from credoai.modules.metrics import ALL_METRICS, MODEL_METRIC_CATEGORIES
 from pandas import DataFrame
 
+from credoai.modules.metrics import ALL_METRICS, METRIC_CATEGORIES
+
 
 def list_metrics(verbose=True):
     metrics = defaultdict(set)
     for metric in ALL_METRICS:
-        if metric.metric_category in MODEL_METRIC_CATEGORIES:
+        if metric.metric_category in METRIC_CATEGORIES:
             metrics[metric.metric_category] |= metric.equivalent_names
     if verbose:
         for key, val in metrics.items():
             metric_str = textwrap.fill(
                 ", ".join(sorted(list(val))),
-                width=50,
+                width=80,
                 initial_indent="\t",
                 subsequent_indent="\t",
             )
             print(key)
             print(metric_str)
             print("")
     return metrics
```

### Comparing `credoai-lens-1.1.7/credoai/modules/metrics.py` & `credoai-lens-1.1.8/credoai/modules/metrics.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/modules/metrics_credoai.py` & `credoai-lens-1.1.8/credoai/modules/metrics_credoai.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Custom metrics defined by Credo AI"""
 
 from functools import partial
-from typing import Literal
 
 import numpy as np
 import pandas as pd
 import scipy.stats as st
 from fairlearn.metrics import make_derived_metric, true_positive_rate
 from sklearn import metrics as sk_metrics
 from sklearn.metrics import accuracy_score, confusion_matrix
 from sklearn.utils import check_consistent_length
+from typing_extensions import Literal
 
 
 def multiclass_confusion_metrics(y_true, y_pred, metric=None, average="weighted"):
     """Calculate
 
     Parameters
     ----------
@@ -592,15 +592,15 @@
         Proceedings of the 25th acm sigkdd international conference on knowledge discovery &
         data mining. 2019.
 
     Examples
     --------
     >>> ranked_list = ['female', 'male', 'male', 'female', 'male', 'male']
     >>> desired_proportions = {'female': 0.6, 'male': 0.4}
-    >>> normalized_discounted_cumulative_kl_divergence(ranked_list, desired_proportions)
+    >>> round(normalized_discounted_cumulative_kl_divergence(ranked_list, desired_proportions), 15)
     0.208096993149323
     """
     num_items = len(ranked_list)
     Z = np.sum(1 / (np.log2(np.arange(1, num_items + 1) + 1)))
 
     total = 0.0
     for k in range(1, num_items + 1):
```

### Comparing `credoai-lens-1.1.7/credoai/modules/stats.py` & `credoai-lens-1.1.8/credoai/modules/stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import traceback
 from itertools import combinations, product
 
 import numpy as np
 import pandas as pd
 from lifelines import CoxPHFitter
-from scipy.stats import chi2_contingency, f_oneway, tukey_hsd
+from scipy.stats import chi2_contingency, f_oneway
+from statsmodels.stats.multicomp import pairwise_tukeyhsd
 
 from credoai.modules.stats_utils import columns_from_formula
 from credoai.utils import global_logger
 
 
 class CoxPH:
     def __init__(self, **kwargs):
@@ -54,15 +55,15 @@
         survival_curves = survival_curves[survival_curves["time_step"] % 5 == 0]
         survival_curves.name = f"{self.name} Survival Curves"
         return survival_curves
 
     def _get_prediction_data(self):
         columns = columns_from_formula(self.fit_kwargs.get("formula"))
         df = pd.DataFrame(
-            list(product(*[i.unique() for _, i in self.data[columns].iteritems()])),
+            list(product(*[i.unique() for _, i in self.data[columns].items()])),
             columns=columns,
         )
         return df
 
 
 class ChiSquare:
     def __init__(self, pvalue=0.05):
@@ -184,34 +185,37 @@
         overall_test = f_oneway(*self.data["groups"])
         results = {
             "test_type": "oneway_anova",
             "statistic": overall_test.statistic,
             "pvalue": overall_test.pvalue,
         }
         if run_posthoc and results["pvalue"] < self.pvalue:
-            results["significant_posthoc_tests"] = self._posthoc_tests()
+            results["significant_posthoc_tests"] = self._posthoc_tests(
+                df[outcome_col], df[outcome_col]
+            )
         return results
 
     def _setup(self, df, grouping_col, outcome_col):
         groups = df.groupby(grouping_col)[outcome_col]
         group_lists = groups.apply(list)
         labels = np.array(group_lists.index)
         self.data = {"groups": group_lists, "labels": labels}
 
-    def _posthoc_tests(self):
+    def _posthoc_tests(self, outcome_col, grouping_col):
         """Run Tukey HSD posthoc tests on each label"""
         posthoc_tests = []
-        r = tukey_hsd(*self.data["groups"].values)
-        sig_compares = r.pvalue < self.pvalue
-        for indices in zip(*np.where(sig_compares)):
-            specific_labels = np.take(self.data["labels"], indices)
-            statistic = r.statistic[indices]
-            posthoc_tests.append(
-                {
-                    "test_type": "tukey_hsd",
-                    "comparison": specific_labels,
-                    "statistic": statistic,
-                    "pvalue": r.pvalue[indices],
-                    "significance_threshold": self.pvalue,
-                }
-            )
+
+        results = pairwise_tukeyhsd(outcome_col, grouping_col)
+        results_df = pd.DataFrame(
+            {
+                "test_type": "tukey_hsd",
+                "pvalue": results.pvalues,
+                "statistic": results.meandiffs,
+                "reject": results.reject,
+                "comparison": list(combinations(results.groupsunique, 2)),
+                "significance_threshold": self.pvalue,
+            }
+        )
+        results_df = results_df[results_df["reject"] == True]
+        posthoc_tests = results_df.to_dict(orient="records")
+
         return sorted(posthoc_tests, key=lambda x: x["pvalue"])
```

### Comparing `credoai-lens-1.1.7/credoai/prism/compare.py` & `credoai-lens-1.1.8/credoai/prism/compare.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Performs comparison between 2 pipelines"""
-from typing import Literal, Optional
+from typing import Optional
 
 from connect.evidence.containers import MetricContainer
+from typing_extensions import Literal
 
 from credoai.evaluators.utils.validation import check_instance
 from credoai.lens import Lens
 from credoai.prism.comparators.metric_comparator import MetricComparator
 from credoai.prism.task import Task
 from credoai.utils import flatten_list
 from credoai.utils.common import ValidationError
```

### Comparing `credoai-lens-1.1.7/credoai/prism/prism.py` & `credoai-lens-1.1.8/credoai/prism/prism.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/prism/task.py` & `credoai-lens-1.1.8/credoai/prism/task.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/utils/common.py` & `credoai-lens-1.1.8/credoai/utils/common.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/utils/dataset_utils.py` & `credoai-lens-1.1.8/credoai/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/utils/logging.py` & `credoai-lens-1.1.8/credoai/utils/logging.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/utils/model_utils.py` & `credoai-lens-1.1.8/credoai/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/utils/policy_utils.py` & `credoai-lens-1.1.8/credoai/utils/policy_utils.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai/utils/version_check.py` & `credoai-lens-1.1.8/credoai/utils/version_check.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/credoai_lens.egg-info/PKG-INFO` & `credoai-lens-1.1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,100 +1,102 @@
 Metadata-Version: 2.1
 Name: credoai-lens
-Version: 1.1.7
+Version: 1.1.8
 Summary: Lens: comprehensive assessment framework for AI systems
-Home-page: 
-Download-URL: https://github.com/credo-ai/credoai_lens
+Home-page: UNKNOWN
 Author: Ian Eisenberg
 Author-email: ian@credo.ai
 Maintainer: Ian Eisenberg
 Maintainer-email: ian@credo.ai
+License: UNKNOWN
+Download-URL: https://github.com/credo-ai/credoai_lens
+Description: <img src="https://raw.githubusercontent.com/credo-ai/credoai_lens/develop/docs/_static/images/credo_ai-lens.png" width="250" alt="Credo AI Lens"><br>
+        
+        ![Workflow](https://github.com/credo-ai/credoai_lens/actions/workflows/test-reports.yml/badge.svg)
+        ![Tests](https://credoai-cicd-public-artifacts.s3.us-west-2.amazonaws.com/credoai_lens/main/tests-badge.svg)
+        [![Coverage](https://credoai-cicd-public-artifacts.s3.us-west-2.amazonaws.com/credoai_lens/main/coverage-badge.svg)](https://credoai-cicd-public-artifacts.s3.us-west-2.amazonaws.com/credoai_lens/main/html/index.html)
+        
+        --------------------------------------
+        
+        # Lens by Credo AI - Responsible AI Assessment Framework
+        
+        Lens is a comprehensive assessment framework for AI systems. 
+        Lens standardizes model and data assessment, and acts as a central gateway to assessments 
+        created in the open source community. In short, Lens connects arbitrary AI models and datasets
+        with Responsible AI tools throughout the ecosystem.
+        
+        Lens can be run in a notebook, a CI/CD pipeline, or anywhere else you do your ML analytics.
+        It is extensible, and easily customized to your organizations assessments if they are not 
+        supported by default. 
+        
+        Though it can be used alone, Lens shows its full value when connected to your organization's 
+        [Credo AI App](https://www.credo.ai/product). Credo AI is an end-to-end AI Governance
+        App that supports multi-stakeholder alignment, AI assessment (via Lens) and AI risk assessment.
+        
+        
+        
+        ## Dependencies
+        
+        - Credo AI Lens supports Python 3.8+
+        - Sphinx (optional for local docs site)
+        
+        
+        ## Installation
+        
+        The latest stable release (and required dependencies) can be installed from PyPI.
+        
+        ```
+        pip install credoai-lens
+        ```
+        
+        Additional installation instructions can be found in our [setup documentation](https://credoai-lens.readthedocs.io/en/stable/pages/setup.html)
+        
+        ## Getting Started
+        To get started, see the [quickstart demo](https://credoai-lens.readthedocs.io/en/stable/notebooks/quickstart.html).
+        
+        If you are using the Credo AI Governance App, also check out the [governance integration demo](https://credoai-lens.readthedocs.io/en/stable/notebooks/governance_integration.html).
+        
+        ## Documentation
+        
+        Documentation is hosted by [readthedocs](https://credoai-lens.readthedocs.io/en/stable/).
+        
+        For dev documentation, see [latest](https://credoai-lens.readthedocs.io/en/stable/index.html).
+        
+        ## AI Governance
+        
+        As an assessment framework, Lens is an important component of your overall **AI Governance** strategy.
+        But it's not the only component! Credo AI, the developer of Lens, also develops
+        tools to satisfy your general AI Governance needs, which integrate easily with Lens.
+        
+        To connect to [Credo AI's Governance App](https://www.credo.ai/product), see the Governance
+        tutorial on [readthedocs](https://credoai-lens.readthedocs.io/en/stable/notebooks/governance_integration.html).
+         
+        # For Lens developers
+        
+        ## Running tests
+        
+        
+        Running a test
+        
+        ```shell
+        scripts/test.sh
+        ```
+        
+        Running tests with pytest-watch
+        
+        ```shell
+        ptw --runner "pytest -s"
+        ```
+        
+Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: full
-License-File: LICENSE
-
-<img src="https://raw.githubusercontent.com/credo-ai/credoai_lens/develop/docs/_static/images/credo_ai-lens.png" width="250" alt="Credo AI Lens"><br>
-
-![Workflow](https://github.com/credo-ai/credoai_lens/actions/workflows/test-reports.yml/badge.svg)
-![Tests](https://credoai-cicd-public-artifacts.s3.us-west-2.amazonaws.com/credoai_lens/main/tests-badge.svg)
-[![Coverage](https://credoai-cicd-public-artifacts.s3.us-west-2.amazonaws.com/credoai_lens/main/coverage-badge.svg)](https://credoai-cicd-public-artifacts.s3.us-west-2.amazonaws.com/credoai_lens/main/html/index.html)
-
---------------------------------------
-
-# Lens by Credo AI - Responsible AI Assessment Framework
-
-Lens is a comprehensive assessment framework for AI systems. 
-Lens standardizes model and data assessment, and acts as a central gateway to assessments 
-created in the open source community. In short, Lens connects arbitrary AI models and datasets
-with Responsible AI tools throughout the ecosystem.
-
-Lens can be run in a notebook, a CI/CD pipeline, or anywhere else you do your ML analytics.
-It is extensible, and easily customized to your organizations assessments if they are not 
-supported by default. 
-
-Though it can be used alone, Lens shows its full value when connected to your organization's 
-[Credo AI App](https://www.credo.ai/product). Credo AI is an end-to-end AI Governance
-App that supports multi-stakeholder alignment, AI assessment (via Lens) and AI risk assessment.
-
-
-
-## Dependencies
-
-- Credo AI Lens supports Python 3.8+
-- Sphinx (optional for local docs site)
-
-
-## Installation
-
-The latest stable release (and required dependencies) can be installed from PyPI.
-
-```
-pip install credoai-lens
-```
-
-Additional installation instructions can be found in our [setup documentation](https://credoai-lens.readthedocs.io/en/stable/notebooks/quickstart.html)
-
-## Getting Started
-
-To get started, see the [quickstart demo](https://credoai-lens.readthedocs.io/en/stable/notebooks/quickstart.html).
-
-If you are using the Credo AI Governance App, also check out the [governance integration demo](https://credoai-lens.readthedocs.io/en/stable/notebooks/governance_integration.html).
-
-## Documentation
-
-Documentation is hosted by [readthedocs](https://credoai-lens.readthedocs.io/en/stable/).
-
-For dev documentation, see [latest](https://credoai-lens.readthedocs.io/en/stable/index.html).
-
-## AI Governance
-
-As an assessment framework, Lens is an important component of your overall **AI Governance** strategy.
-But it's not the only component! Credo AI, the developer of Lens, also develops
-tools to satisfy your general AI Governance needs, which integrate easily with Lens.
-
-To connect to [Credo AI's Governance App](https://www.credo.ai/product), see the Governance
-tutorial on [readthedocs](https://credoai-lens.readthedocs.io/en/stable/notebooks/governance_integration.html).
- 
-# For Lens developers
-
-## Running tests
-
-
-Running a test
-
-```shell
-scripts/test.sh
-```
-
-Running tests with pytest-watch
-
-```shell
-ptw --runner "pytest -s"
-```
```

### Comparing `credoai-lens-1.1.7/credoai_lens.egg-info/requires.txt` & `credoai-lens-1.1.8/credoai_lens.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,53 @@
-absl-py>=1.0.0
-cloudpickle>=2.0.0
-credoai-connect>=0.0.7
+credoai-connect>=0.1.2
 fairlearn>=0.7.0
+finsfairauditing>=0.0.2
 lifelines>=0.27.3
-json-api-doc>=0.15.0
 matplotlib>=3.0
-nest_asyncio>=1.5.4
-protobuf~=3.19.0
-python-dotenv>=0.19.2
 requests>=2.25.1
 scikit-learn>=0.24
-scipy>=1.8.1
-pandas_profiling==3.3.0
+scipy>=1.7.3
 shap>=0.41.0
-finsfairauditing>=0.0.2
+statsmodels>=0.13.5
+typing_extensions>=4.3.0
+ydata-profiling>=4.0.0
 
 [dev]
 black==22.10.0
-pytest>=6.2.5
-pytest-cov>=3.0.0
-pytest-watch>=4.2
-responses>=0.21.0
-pytest-mock>=3.8
-pytest-assume>=2.4.3
-ipykernel
+credoai-connect
+fairlearn==0.7.0
 furo==2022.3.4
+ipykernel
+lifelines>=0.27.3
 nbsphinx==0.8.7
+numpy==1.23.3
+pandas==1.4.4
 pandoc==1.1.0
 prompt-toolkit<3.0.0
 pydata-sphinx-theme==0.6.3
-sphinx==4.3.0
+pytest-assume>=2.4.3
+pytest-cov>=3.0.0
+pytest-mock>=3.8
+pytest-watch>=4.2
+pytest>=6.2.5
+responses>=0.21.0
+scikit-learn==1.1.2
+scipy==1.9.1
 sphinx-autodoc-typehints==1.12.0
 sphinx-copybutton==0.5.0
+sphinx-exec-code==0.8
+sphinx-fontawesome==0.0.6
 sphinx-gallery==0.10.1
 sphinx-rtd-theme==1.0.0
-sphinx-exec-code==0.8
-numpy==1.23.3
-scipy==1.9.1
-scikit-learn==1.1.2
-pandas==1.4.4
-fairlearn==0.7.0
-lifelines>=0.27.3
-credoai-connect
+sphinx==4.3.0
 tensorflow==2.11.1
 
 [full]
 adversarial-robustness-toolbox>=1.10.1
-torch>=1.12.1
 deepchecks>=0.9.1
+torch>=1.12.1
 
 [full:sys_platform != "darwin"]
-tensorflow==2.11.1
+tensorflow>=2.11.0
 
 [full:sys_platform == "darwin"]
 tensorflow-macos==2.10.0
```

### Comparing `credoai-lens-1.1.7/setup.py` & `credoai-lens-1.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 DISTNAME = "credoai-lens"
 MAINTAINER = "Ian Eisenberg"
 MAINTAINER_EMAIL = "ian@credo.ai"
 URL = ""
 LICENSE = ""
 DOWNLOAD_URL = "https://github.com/credo-ai/credoai_lens"
 VERSION = __version__
-PYTHON_REQUIRES = ">=3.8"
+PYTHON_REQUIRES = ">=3.7, <3.11"
+
 
 # Fetch ReadMe
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 # Use requirements.txt to set the install_requires
 with open("requirements.txt") as f:
@@ -38,31 +39,32 @@
 
 EXTRAS_REQUIRES = {"dev": dev_requirements, "full": full_requirements}
 
 
 CLASSIFIERS = [
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
+    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Operating System :: OS Independent",
 ]
 
 PACKAGE_DATA = {
     "credoai": [
         "datasets/*",
         "datasets/static/nlp_generator_analyzer/persisted_models/*",
         "datasets/static/nlp_generator_analyzer/prompts/*",
     ]
 }
 
 
 if __name__ == "__main__":
-
     import sys
 
     from setuptools import setup
 
     setup(
         name=DISTNAME,
         author=MAINTAINER,
```

### Comparing `credoai-lens-1.1.7/tests/conftest.py` & `credoai-lens-1.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/tests/fixtures/datasets.py` & `credoai-lens-1.1.8/tests/fixtures/datasets.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/tests/fixtures/frozen_tests.py` & `credoai-lens-1.1.8/tests/fixtures/frozen_tests.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/tests/fixtures/lens_artifacts.py` & `credoai-lens-1.1.8/tests/fixtures/lens_artifacts.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/tests/fixtures/lens_inits.py` & `credoai-lens-1.1.8/tests/fixtures/lens_inits.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/tests/test_artifacts.py` & `credoai-lens-1.1.8/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/tests/test_binary_classification.py` & `credoai-lens-1.1.8/tests/test_binary_classification.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/tests/test_frozen_results.py` & `credoai-lens-1.1.8/tests/test_frozen_results.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/tests/test_integration.py` & `credoai-lens-1.1.8/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/tests/test_multiclass_classification.py` & `credoai-lens-1.1.8/tests/test_multiclass_classification.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/tests/test_prism.py` & `credoai-lens-1.1.8/tests/test_prism.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/tests/test_quickstart.py` & `credoai-lens-1.1.8/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `credoai-lens-1.1.7/tests/test_regression.py` & `credoai-lens-1.1.8/tests/test_regression.py`

 * *Files identical despite different names*

