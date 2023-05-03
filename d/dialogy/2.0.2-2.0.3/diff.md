# Comparing `tmp/dialogy-2.0.2.tar.gz` & `tmp/dialogy-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialogy-2.0.2.tar", max compression
+gzip compressed data, was "dialogy-2.0.3.tar", max compression
```

## Comparing `dialogy-2.0.2.tar` & `dialogy-2.0.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1069 2023-04-27 12:34:11.572003 dialogy-2.0.2/LICENSE.md
--rw-r--r--   0        0        0        0 2023-04-27 12:34:11.572003 dialogy-2.0.2/dialogy/__init__.py
--rw-r--r--   0        0        0      183 2023-04-27 12:34:11.572003 dialogy-2.0.2/dialogy/base/__init__.py
--rw-r--r--   0        0        0     4949 2023-04-27 12:34:11.572003 dialogy-2.0.2/dialogy/base/entity_extractor/__init__.py
--rw-r--r--   0        0        0     9794 2023-04-27 12:34:11.572003 dialogy-2.0.2/dialogy/base/input/__init__.py
--rw-r--r--   0        0        0     4595 2023-04-27 12:34:11.572003 dialogy-2.0.2/dialogy/base/output/__init__.py
--rw-r--r--   0        0        0    15662 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/base/plugin/__init__.py
--rw-r--r--   0        0        0     3908 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/cli/__init__.py
--rw-r--r--   0        0        0     2587 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/cli/project.py
--rw-r--r--   0        0        0     1865 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/cli/workflow.py
--rw-r--r--   0        0        0     5017 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/constants/__init__.py
--rw-r--r--   0        0        0     2011 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/registry.py
--rw-r--r--   0        0        0        0 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/__init__.py
--rw-r--r--   0        0        0     3995 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/address_parser/__init__.py
--rw-r--r--   0        0        0     1406 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/address_parser/mapmyindia.py
--rw-r--r--   0        0        0     4978 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/address_parser/maps.py
--rw-r--r--   0        0        0        0 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/calibration/__init__.py
--rw-r--r--   0        0        0     8868 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/calibration/xgb.py
--rw-r--r--   0        0        0     3790 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/canonicalization/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/classification/__init__.py
--rw-r--r--   0        0        0    11805 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/classification/mlp.py
--rw-r--r--   0        0        0     1179 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/classification/retain_intent.py
--rw-r--r--   0        0        0       58 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/classification/tokenizers.py
--rw-r--r--   0        0        0    17162 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/classification/xlmr.py
--rw-r--r--   0        0        0     7676 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/combine_date_time/__init__.py
--rw-r--r--   0        0        0    39327 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/duckling_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/error_recovery/__init__.py
--rw-r--r--   0        0        0    20334 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/error_recovery/error_recovery.py
--rw-r--r--   0        0        0    12300 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/intent_entity_mutator/__init__.py
--rw-r--r--   0        0        0      743 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
--rw-r--r--   0        0        0      797 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/intent_entity_mutator/const.py
--rw-r--r--   0        0        0      313 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/intent_entity_mutator/registry.py
--rw-r--r--   0        0        0     1792 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/lb_plugin/__init__.py
--rw-r--r--   0        0        0    14123 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/list_entity_plugin/__init__.py
--rw-r--r--   0        0        0    11523 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/list_search_plugin/__init__.py
--rw-r--r--   0        0        0     4841 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/list_search_plugin/sample_config.yaml
--rw-r--r--   0        0        0     4699 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/merge_asr_output/__init__.py
--rw-r--r--   0        0        0     1565 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/oos_filter/__init__.py
--rw-r--r--   0        0        0     4247 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/qc_plugin/__init__.py
--rw-r--r--   0        0        0      833 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/slot_filler/__init__.py
--rw-r--r--   0        0        0     4148 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/slot_filler/rule_slot_filler.py
--rw-r--r--   0        0        0        0 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/plugins/text/voting/__init__.py
--rw-r--r--   0        0        0     1862 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/types/__init__.py
--rw-r--r--   0        0        0      170 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/types/entity/__init__.py
--rw-r--r--   0        0        0      914 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/types/entity/address/__init__.py
--rw-r--r--   0        0        0     1811 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/types/entity/amount_of_money/__init__.py
--rw-r--r--   0        0        0     7338 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/types/entity/base_entity/__init__.py
--rw-r--r--   0        0        0     2281 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/types/entity/credit_card_number/__init__.py
--rw-r--r--   0        0        0     3637 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/types/entity/deserialize/__init__.py
--rw-r--r--   0        0        0     4317 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/types/entity/duration/__init__.py
--rw-r--r--   0        0        0      975 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/types/entity/keyword/__init__.py
--rw-r--r--   0        0        0     4698 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/types/entity/numerical/__init__.py
--rw-r--r--   0        0        0     2271 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/types/entity/people/__init__.py
--rw-r--r--   0        0        0      910 2023-04-27 12:34:11.576003 dialogy-2.0.2/dialogy/types/entity/pincode/__init__.py
--rw-r--r--   0        0        0    13534 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/types/entity/time/__init__.py
--rw-r--r--   0        0        0     8803 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/types/entity/time_interval/__init__.py
--rw-r--r--   0        0        0     8893 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/types/intent/__init__.py
--rw-r--r--   0        0        0      154 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/types/plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/types/signal/__init__.py
--rw-r--r--   0        0        0      194 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/types/signal/signal.py
--rw-r--r--   0        0        0      991 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/types/slots/__init__.py
--rw-r--r--   0        0        0      191 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/types/utterances/__init__.py
--rw-r--r--   0        0        0      638 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/utils/__init__.py
--rw-r--r--   0        0        0    10469 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/utils/config.py
--rw-r--r--   0        0        0     2180 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/utils/datetime.py
--rw-r--r--   0        0        0     3437 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/utils/file_handler.py
--rw-r--r--   0        0        0      808 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/utils/logger.py
--rw-r--r--   0        0        0     2687 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/utils/misc.py
--rw-r--r--   0        0        0      584 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/utils/naive_lang_detect.py
--rw-r--r--   0        0        0     8236 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/utils/normalize_utterance.py
--rw-r--r--   0        0        0     3605 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/utils/temperature_scaling.py
--rw-r--r--   0        0        0       47 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/workflow/__init__.py
--rw-r--r--   0        0        0     6795 2023-04-27 12:34:11.580004 dialogy-2.0.2/dialogy/workflow/workflow.py
--rw-r--r--   0        0        0     1426 2023-04-27 12:34:31.984245 dialogy-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 dialogy-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-03 09:39:48.355294 dialogy-2.0.3/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/base/__init__.py
+-rw-r--r--   0        0        0     4949 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/base/entity_extractor/__init__.py
+-rw-r--r--   0        0        0     9794 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/base/input/__init__.py
+-rw-r--r--   0        0        0     4595 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/base/output/__init__.py
+-rw-r--r--   0        0        0    15662 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/base/plugin/__init__.py
+-rw-r--r--   0        0        0     3908 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/cli/__init__.py
+-rw-r--r--   0        0        0     2587 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/cli/project.py
+-rw-r--r--   0        0        0     1865 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/cli/workflow.py
+-rw-r--r--   0        0        0     5017 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/constants/__init__.py
+-rw-r--r--   0        0        0     2011 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/registry.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/__init__.py
+-rw-r--r--   0        0        0     3995 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/address_parser/__init__.py
+-rw-r--r--   0        0        0     1406 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/address_parser/mapmyindia.py
+-rw-r--r--   0        0        0     4978 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/address_parser/maps.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/calibration/__init__.py
+-rw-r--r--   0        0        0     8868 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/calibration/xgb.py
+-rw-r--r--   0        0        0     3790 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/canonicalization/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/classification/__init__.py
+-rw-r--r--   0        0        0    11805 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/classification/mlp.py
+-rw-r--r--   0        0        0     1179 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/classification/retain_intent.py
+-rw-r--r--   0        0        0       58 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/classification/tokenizers.py
+-rw-r--r--   0        0        0    17246 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/classification/xlmr.py
+-rw-r--r--   0        0        0     7676 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/combine_date_time/__init__.py
+-rw-r--r--   0        0        0    39327 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/duckling_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/error_recovery/__init__.py
+-rw-r--r--   0        0        0    20334 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/error_recovery/error_recovery.py
+-rw-r--r--   0        0        0    12300 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/intent_entity_mutator/__init__.py
+-rw-r--r--   0        0        0      743 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
+-rw-r--r--   0        0        0      797 2023-05-03 09:39:48.355294 dialogy-2.0.3/dialogy/plugins/text/intent_entity_mutator/const.py
+-rw-r--r--   0        0        0      313 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/plugins/text/intent_entity_mutator/registry.py
+-rw-r--r--   0        0        0     1792 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/plugins/text/lb_plugin/__init__.py
+-rw-r--r--   0        0        0    14123 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/plugins/text/list_entity_plugin/__init__.py
+-rw-r--r--   0        0        0    11523 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/plugins/text/list_search_plugin/__init__.py
+-rw-r--r--   0        0        0     4841 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/plugins/text/list_search_plugin/sample_config.yaml
+-rw-r--r--   0        0        0     4699 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/plugins/text/merge_asr_output/__init__.py
+-rw-r--r--   0        0        0     1565 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/plugins/text/oos_filter/__init__.py
+-rw-r--r--   0        0        0     4247 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/plugins/text/qc_plugin/__init__.py
+-rw-r--r--   0        0        0      833 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/plugins/text/slot_filler/__init__.py
+-rw-r--r--   0        0        0     4148 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/plugins/text/slot_filler/rule_slot_filler.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/plugins/text/voting/__init__.py
+-rw-r--r--   0        0        0     1862 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/entity/__init__.py
+-rw-r--r--   0        0        0      914 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/entity/address/__init__.py
+-rw-r--r--   0        0        0     1811 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/entity/amount_of_money/__init__.py
+-rw-r--r--   0        0        0     7338 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/entity/base_entity/__init__.py
+-rw-r--r--   0        0        0     2281 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/entity/credit_card_number/__init__.py
+-rw-r--r--   0        0        0     3637 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/entity/deserialize/__init__.py
+-rw-r--r--   0        0        0     4317 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/entity/duration/__init__.py
+-rw-r--r--   0        0        0      975 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/entity/keyword/__init__.py
+-rw-r--r--   0        0        0     4698 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/entity/numerical/__init__.py
+-rw-r--r--   0        0        0     2271 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/entity/people/__init__.py
+-rw-r--r--   0        0        0      910 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/entity/pincode/__init__.py
+-rw-r--r--   0        0        0    13534 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/entity/time/__init__.py
+-rw-r--r--   0        0        0     8803 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/entity/time_interval/__init__.py
+-rw-r--r--   0        0        0     8893 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/intent/__init__.py
+-rw-r--r--   0        0        0      154 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/signal/__init__.py
+-rw-r--r--   0        0        0      194 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/signal/signal.py
+-rw-r--r--   0        0        0      991 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/slots/__init__.py
+-rw-r--r--   0        0        0      191 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/types/utterances/__init__.py
+-rw-r--r--   0        0        0      638 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/utils/__init__.py
+-rw-r--r--   0        0        0    10469 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/utils/config.py
+-rw-r--r--   0        0        0     2180 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/utils/datetime.py
+-rw-r--r--   0        0        0     3437 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/utils/file_handler.py
+-rw-r--r--   0        0        0      808 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/utils/logger.py
+-rw-r--r--   0        0        0     2687 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/utils/misc.py
+-rw-r--r--   0        0        0      584 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/utils/naive_lang_detect.py
+-rw-r--r--   0        0        0     8236 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/utils/normalize_utterance.py
+-rw-r--r--   0        0        0     3605 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/utils/temperature_scaling.py
+-rw-r--r--   0        0        0       47 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/workflow/__init__.py
+-rw-r--r--   0        0        0     6795 2023-05-03 09:39:48.359294 dialogy-2.0.3/dialogy/workflow/workflow.py
+-rw-r--r--   0        0        0     1426 2023-05-03 09:40:10.691505 dialogy-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 dialogy-2.0.3/PKG-INFO
```

### Comparing `dialogy-2.0.2/LICENSE.md` & `dialogy-2.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/base/entity_extractor/__init__.py` & `dialogy-2.0.3/dialogy/base/entity_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/base/input/__init__.py` & `dialogy-2.0.3/dialogy/base/input/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/base/output/__init__.py` & `dialogy-2.0.3/dialogy/base/output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/base/plugin/__init__.py` & `dialogy-2.0.3/dialogy/base/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/cli/__init__.py` & `dialogy-2.0.3/dialogy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/cli/project.py` & `dialogy-2.0.3/dialogy/cli/project.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/cli/workflow.py` & `dialogy-2.0.3/dialogy/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/constants/__init__.py` & `dialogy-2.0.3/dialogy/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/registry.py` & `dialogy-2.0.3/dialogy/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/address_parser/__init__.py` & `dialogy-2.0.3/dialogy/plugins/text/address_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/address_parser/mapmyindia.py` & `dialogy-2.0.3/dialogy/plugins/text/address_parser/mapmyindia.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/address_parser/maps.py` & `dialogy-2.0.3/dialogy/plugins/text/address_parser/maps.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/calibration/xgb.py` & `dialogy-2.0.3/dialogy/plugins/text/calibration/xgb.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/canonicalization/__init__.py` & `dialogy-2.0.3/dialogy/plugins/text/canonicalization/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/classification/mlp.py` & `dialogy-2.0.3/dialogy/plugins/text/classification/mlp.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/classification/retain_intent.py` & `dialogy-2.0.3/dialogy/plugins/text/classification/retain_intent.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/classification/xlmr.py` & `dialogy-2.0.3/dialogy/plugins/text/classification/xlmr.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,16 @@
             self.kwargs = kwargs or {}
 
             # TODO: check if this can be avoided
             if "name" in self.kwargs:
                 del self.kwargs["name"]
             if "imported" in self.kwargs:
                 del self.kwargs["imported"]
+            if "purpose" in self.kwargs:
+                del self.kwargs["purpose"]
 
             try:
                 if os.path.exists(self.labelencoder_file_path):
                     logger.debug(f"initializing label encoder file from {self.labelencoder_file_path}")
                     self.init_model()
             except EOFError:
                 logger.error(
```

### Comparing `dialogy-2.0.2/dialogy/plugins/text/combine_date_time/__init__.py` & `dialogy-2.0.3/dialogy/plugins/text/combine_date_time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/duckling_plugin/__init__.py` & `dialogy-2.0.3/dialogy/plugins/text/duckling_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/error_recovery/error_recovery.py` & `dialogy-2.0.3/dialogy/plugins/text/error_recovery/error_recovery.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/intent_entity_mutator/__init__.py` & `dialogy-2.0.3/dialogy/plugins/text/intent_entity_mutator/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py` & `dialogy-2.0.3/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/intent_entity_mutator/const.py` & `dialogy-2.0.3/dialogy/plugins/text/intent_entity_mutator/const.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/lb_plugin/__init__.py` & `dialogy-2.0.3/dialogy/plugins/text/lb_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/list_entity_plugin/__init__.py` & `dialogy-2.0.3/dialogy/plugins/text/list_entity_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/list_search_plugin/__init__.py` & `dialogy-2.0.3/dialogy/plugins/text/list_search_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/list_search_plugin/sample_config.yaml` & `dialogy-2.0.3/dialogy/plugins/text/list_search_plugin/sample_config.yaml`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/merge_asr_output/__init__.py` & `dialogy-2.0.3/dialogy/plugins/text/merge_asr_output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/oos_filter/__init__.py` & `dialogy-2.0.3/dialogy/plugins/text/oos_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/qc_plugin/__init__.py` & `dialogy-2.0.3/dialogy/plugins/text/qc_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/slot_filler/__init__.py` & `dialogy-2.0.3/dialogy/plugins/text/slot_filler/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/plugins/text/slot_filler/rule_slot_filler.py` & `dialogy-2.0.3/dialogy/plugins/text/slot_filler/rule_slot_filler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/__init__.py` & `dialogy-2.0.3/dialogy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/entity/address/__init__.py` & `dialogy-2.0.3/dialogy/types/entity/address/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/entity/amount_of_money/__init__.py` & `dialogy-2.0.3/dialogy/types/entity/amount_of_money/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/entity/base_entity/__init__.py` & `dialogy-2.0.3/dialogy/types/entity/base_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/entity/credit_card_number/__init__.py` & `dialogy-2.0.3/dialogy/types/entity/credit_card_number/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/entity/deserialize/__init__.py` & `dialogy-2.0.3/dialogy/types/entity/deserialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/entity/duration/__init__.py` & `dialogy-2.0.3/dialogy/types/entity/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/entity/keyword/__init__.py` & `dialogy-2.0.3/dialogy/types/entity/keyword/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/entity/numerical/__init__.py` & `dialogy-2.0.3/dialogy/types/entity/numerical/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/entity/people/__init__.py` & `dialogy-2.0.3/dialogy/types/entity/people/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/entity/pincode/__init__.py` & `dialogy-2.0.3/dialogy/types/entity/pincode/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/entity/time/__init__.py` & `dialogy-2.0.3/dialogy/types/entity/time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/entity/time_interval/__init__.py` & `dialogy-2.0.3/dialogy/types/entity/time_interval/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/intent/__init__.py` & `dialogy-2.0.3/dialogy/types/intent/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/types/slots/__init__.py` & `dialogy-2.0.3/dialogy/types/slots/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/utils/__init__.py` & `dialogy-2.0.3/dialogy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/utils/config.py` & `dialogy-2.0.3/dialogy/utils/config.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/utils/datetime.py` & `dialogy-2.0.3/dialogy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/utils/file_handler.py` & `dialogy-2.0.3/dialogy/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/utils/logger.py` & `dialogy-2.0.3/dialogy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/utils/misc.py` & `dialogy-2.0.3/dialogy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/utils/naive_lang_detect.py` & `dialogy-2.0.3/dialogy/utils/naive_lang_detect.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/utils/normalize_utterance.py` & `dialogy-2.0.3/dialogy/utils/normalize_utterance.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/utils/temperature_scaling.py` & `dialogy-2.0.3/dialogy/utils/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/dialogy/workflow/workflow.py` & `dialogy-2.0.3/dialogy/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.2/pyproject.toml` & `dialogy-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dialogy"
-version = "2.0.2"
+version = "2.0.3"
 description = "Dialogy is a library for building and managing SLU applications."
 authors = ["Amresh Venugopal <amresh.venugopal@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/skit-ai/dialogy"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `dialogy-2.0.2/PKG-INFO` & `dialogy-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialogy
-Version: 2.0.2
+Version: 2.0.3
 Summary: Dialogy is a library for building and managing SLU applications.
 Home-page: https://github.com/skit-ai/dialogy
 License: MIT
 Author: Amresh Venugopal
 Author-email: amresh.venugopal@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

