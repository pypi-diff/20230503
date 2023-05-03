# Comparing `tmp/ai_transform-0.30.9.tar.gz` & `tmp/ai_transform-0.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.30.9.tar", last modified: Fri Apr 21 04:29:28 2023, max compression
+gzip compressed data, was "ai_transform-0.31.0.tar", last modified: Wed May  3 04:24:59 2023, max compression
```

## Comparing `ai_transform-0.30.9.tar` & `ai_transform-0.31.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-21 04:29:09.000000 ai_transform-0.30.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-21 04:29:28.958745 ai_transform-0.30.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-21 04:29:09.000000 ai_transform-0.30.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.950744 ai_transform-0.30.9/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.950744 ai_transform-0.30.9/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30029 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.954745 ai_transform-0.30.9/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.954745 ai_transform-0.30.9/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.954745 ai_transform-0.30.9/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15582 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.954745 ai_transform-0.30.9/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.954745 ai_transform-0.30.9/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.954745 ai_transform-0.30.9/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-21 04:29:09.000000 ai_transform-0.30.9/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.950744 ai_transform-0.30.9/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-21 04:29:28.000000 ai_transform-0.30.9/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-21 04:29:28.000000 ai_transform-0.30.9/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 04:29:28.000000 ai_transform-0.30.9/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-21 04:29:28.000000 ai_transform-0.30.9/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 04:29:28.000000 ai_transform-0.30.9/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-21 04:29:09.000000 ai_transform-0.30.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 04:29:28.958745 ai_transform-0.30.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-21 04:29:09.000000 ai_transform-0.30.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:28.958745 ai_transform-0.30.9/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-21 04:29:09.000000 ai_transform-0.30.9/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.480532 ai_transform-0.31.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-03 04:24:42.000000 ai_transform-0.31.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-03 04:24:59.480532 ai_transform-0.31.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-03 04:24:42.000000 ai_transform-0.31.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.472532 ai_transform-0.31.0/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.472532 ai_transform-0.31.0/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29326 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15346 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.472532 ai_transform-0.31.0/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-03 04:24:59.000000 ai_transform-0.31.0/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-03 04:24:59.000000 ai_transform-0.31.0/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:24:59.000000 ai_transform-0.31.0/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-03 04:24:59.000000 ai_transform-0.31.0/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 04:24:59.000000 ai_transform-0.31.0/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 04:24:42.000000 ai_transform-0.31.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 04:24:59.480532 ai_transform-0.31.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-03 04:24:42.000000 ai_transform-0.31.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.480532 ai_transform-0.31.0/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.480532 ai_transform-0.31.0/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.480532 ai_transform-0.31.0/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.480532 ai_transform-0.31.0/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.30.9/LICENSE` & `ai_transform-0.31.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/README.md` & `ai_transform-0.31.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/__init__.py` & `ai_transform-0.31.0/ai_transform/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-__version__ = "0.30.9"
+__version__ = "0.31.0"
 
 from ai_transform.timer import Timer
 
-
 _TIMER = Timer()
 _TIMER.start()
 
 
 def add_config_paths(verbose: bool = False):
     # Support all config paths
     # Add config paths
```

### Comparing `ai_transform-0.30.9/ai_transform/api/api.py` & `ai_transform-0.31.0/ai_transform/api/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,31 +9,30 @@
 from functools import wraps
 
 from typing import Any, Dict, List, Optional, Literal
 
 from ai_transform.logger import format_logging_info
 from ai_transform.utils import document
 from ai_transform.types import Credentials, FieldTransformer, Filter, Schema
+from ai_transform.api.wrappers import request_wrapper
 
 from ai_transform import __version__
+from ai_transform.logger import ic
 
 
 LOG_REQUESTS = bool(os.getenv("LOG_REQUESTS"))
 if LOG_REQUESTS:
     # Get the current Unix timestamp as a string
     timestamp = str(int(time.time()))
 
     logging.basicConfig(
         level=logging.DEBUG,
         format="%(asctime)s - %(levelname)s - %(message)s",
         handlers=[logging.FileHandler(f"{timestamp}_request_logs.log")],
     )
-else:
-    logger = logging.getLogger(__name__)
-    logger.setLevel(logging.DEBUG)
 
 
 def to_curl(request: requests.PreparedRequest):
     command = "curl -X {method} '{url}'".format(method=request.method, url=request.url)
 
     for header, value in request.headers.items():
         if header.lower() == "authorization":
@@ -59,62 +58,49 @@
 def get_response(response: requests.Response) -> Dict[str, Any]:
     # get a json response
     # if errors - print what the response contains
     if response.status_code == 200:
         try:
             return response.json()
         except Exception as e:
-            logger.exception(e)
-            logger.error(format_logging_info({"x-trace-id": response.headers["x-trace-id"]}))
+            ic(e)
+            ic(format_logging_info({"x-trace-id": response.headers["x-trace-id"]}))
             raise e
     else:
         datum = {"error": response.content.decode("utf-8")}
         if "x-trace-id" in response.headers:
             datum["x-trace-id"] = response.headers["x-trace-id"]
 
         try:
             # Log this somewhere if it errors
-            logger.error(format_logging_info(datum))
+            ic(format_logging_info(datum))
         except Exception as no_content_e:
             # in case there's no content
-            logger.exception(no_content_e)
+            ic(no_content_e)
             # we still want to raise the right error for retrying
             # continue to raise exception so that any retry logic still holds
             raise no_content_e
 
 
 # We implement retry as a function for several reasons
 # first - we can get a
 def retry(num_of_retries: int = 3, timeout: int = 30):
     """
     Allows the function to retry upon failure.
     Args:
         num_of_retries: The number of times the function should retry
         timeout: The number of seconds to wait between each retry
     """
-    num_of_retries = 3
-    timeout = 30
 
     def _retry(func):
         @wraps(func)
         def function_wrapper(*args, **kwargs):
-            for i in range(num_of_retries):
-                try:
-                    return func(*args, **kwargs)
-                # Using general error to avoid any possible error dependencies.
-                except (ConnectionError, JSONDecodeError) as error:
-                    logger.exception(error)
-                    print(f"Sleeping in {timeout}")
-                    time.sleep(timeout)
-                    if i == num_of_retries - 1:
-                        raise error
-                    continue
-                except Exception as error:
-                    print(error)
-                    logger.exception(error)
+            return request_wrapper(
+                func, args, kwargs, num_retries=num_of_retries, timeout=timeout, exponential_backoff=2
+            )
 
         return function_wrapper
 
     return _retry
 
 
 class API:
@@ -351,15 +337,15 @@
             assert isinstance(email, dict)
             assert "secondary_cta" in email
             assert "url" in email["secondary_cta"]
             assert "text" in email["secondary_cta"]
 
             parameters["email"] = email
 
-        logger.debug(format_logging_info(parameters))
+        ic(parameters)
 
         response = self.post(suffix=f"/workflows/{job_id}/status", json=parameters)
         return get_response(response)
 
     def _set_field_children(
         self,
         dataset_id: str,
@@ -381,15 +367,15 @@
         """
         params = dict(
             field=field,
             field_children=field_children,
             category=fieldchildren_id,
             metadata={} if metadata is None else metadata,
         )
-        logger.debug(format_logging_info(params))
+        ic(params)
         response = self.post(suffix=f"/datasets/{dataset_id}/field_children/{str(uuid.uuid4())}/update", json=params)
         return get_response(response)
 
     def _delete_field_children(self, dataset_id: str, fieldchildren_id: str):
         response = self.post(suffix=f"/datasets/{dataset_id}/field_children/{fieldchildren_id}/delete")
         return get_response(response)
 
@@ -508,16 +494,16 @@
             worker_number = 0
 
         if n_processed_pricing:
             params["n_processed_pricing "] = n_processed_pricing
 
         params = dict(worker_number=worker_number, step=step, n_processed=n_processed, n_total=n_total)
 
-        logger.debug("adding progress...")
-        logger.debug(format_logging_info(params))
+        ic("adding progress...")
+        ic(params)
 
         response = self.post(suffix=f"/workflows/{workflow_id}/progress", json=params)
         return get_response(response)
 
     def _update_workflow_pricing(
         self,
         workflow_id: str,
@@ -530,16 +516,16 @@
         abstracted away for now due to the fact that the pricing is actually
         something outside of progress.
         """
         if worker_number is None:
             worker_number = 0
 
         params = dict(worker_number=worker_number, step=step, n_processed_pricing=n_processed_pricing)
-        logger.debug("adding progress...")
-        logger.debug(format_logging_info(params))
+        ic("adding progress...")
+        ic(params)
         response = self.post(suffix=f"/workflows/{workflow_id}/progress", json=params)
         return get_response(response)
 
     def _append_tags(self, dataset_id: str, field: str, tags_to_add: List[str], filters: List[Filter]):
         response = self.post(
             suffix=f"/datasets/{dataset_id}/tags/append",
             json=dict(field=field, tags_to_add=tags_to_add, filters=filters),
```

### Comparing `ai_transform-0.30.9/ai_transform/api/client.py` & `ai_transform-0.31.0/ai_transform/api/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import os
-import logging
+import warnings
 
 from typing import Optional, Dict, Any
 
 from ai_transform.api.api import API
 from ai_transform.api.helpers import process_token
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.types import Schema
 from ai_transform.errors import AuthException
 from ai_transform.constants import WELCOME_MESSAGE
 from ai_transform.workflow.context_manager import WorkflowContextManager
-
-
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+from ai_transform.logger import ic
 
 
 class Client:
-    def __init__(self, token: str) -> None:
+    def __init__(self, token: str, authenticate: bool = True) -> None:
 
         self._credentials = process_token(token)
         self._token = token
         self._api = API(credentials=self.credentials)
 
-        try:
-            self.list_datasets()["datasets"]
-        except:
-            raise AuthException
+        if authenticate:
+            try:
+                self.list_datasets()["datasets"]
+            except:
+                raise AuthException
+            else:
+                print(WELCOME_MESSAGE.format(self.credentials.project))
         else:
-            print(WELCOME_MESSAGE.format(self.credentials.project))
+            warnings.warn(
+                "You have opted to not authenticate on client instantiation. Your token may or may not be valid."
+            )
 
     @property
     def credentials(self):
         return self._credentials
 
     @property
     def api(self) -> API:
@@ -82,15 +84,15 @@
         """
         data = self.api._get_temp_file_upload_url()
         upload_url = data["upload_url"]
         download_url = data["download_url"]
         with open(file_path, "rb") as fn_byte:
             media_content = bytes(fn_byte.read())
         response = self.api._upload_temporary_media(presigned_url=upload_url, media_content=media_content)
-        logger.debug(response.content)
+        ic(response.content)
         return {"download_url": download_url}
 
     def list_project_keys(self):
         return self.api._list_project_keys()
 
     def get_project_key(self, key: str, token: str):
         return self.api._get_project_key(key=key, token=token)
```

### Comparing `ai_transform-0.30.9/ai_transform/api/helpers.py` & `ai_transform-0.31.0/ai_transform/api/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         url=f"https://api-{region}.stack.tryrelevance.com/latest/workflows/types/bulk_update",
         headers={"Authorization": auth},
         json={
             "updates": workflows[0:20],
             "version": "vtest"
         }
     )
-    print(response)
+    ic(response)
     """
     # TODO: Add get request etc.
     if headers is None:
         headers = {}
     if json is None:
         json = {}
     return f"""
```

### Comparing `ai_transform-0.30.9/ai_transform/api/wrappers.py` & `ai_transform-0.31.0/ai_transform/api/wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import time
 import logging
 import requests
 
 from json import JSONDecodeError
-from ai_transform.logger import format_logging_info
+from ai_transform.logger import format_logging_info, ic
 from requests.models import Response
-
 from typing import Union, Sequence, Mapping, Callable, Any
 
 logger = logging.getLogger(__file__)
 logging.basicConfig()
 
 
 class ManualRetryError(Exception):
@@ -29,21 +28,21 @@
         json_response = result.json()
         if key_for_error in json_response:
             raise KeyError
 
     except JSONDecodeError as e:
         error_message = "Response is not JSON decodable"
         if output_to_stdout:
-            print(error_message)
+            ic(error_message)
         raise JSONDecodeError(e.msg, e.doc, e.pos)
 
     except KeyError:
         error_message = f"{key_for_error} not in JSON response"
         if output_to_stdout:
-            print(error_message)
+            ic(error_message)
         raise KeyError(error_message)
 
 
 def request_wrapper(
     fn: Union[requests.get, requests.post],
     args: Sequence = None,
     kwargs: Mapping[str, Any] = None,
@@ -70,26 +69,26 @@
     for n in range(1, num_retries + 1):
         try:
             result = fn(*args, **kwargs)
 
             if not result.ok:
                 to_log = format_logging_info({"message": result.content.decode(), "status_code": result.status_code})
                 if output_to_stdout:
-                    print(to_log)
+                    ic(to_log)
                 raise ResultNotOKError(to_log)
 
             if retry_func(result):
                 to_log_for_retry = "Manual Retry Triggered..."
                 if output_to_stdout:
-                    print(to_log_for_retry)
+                    ic(to_log_for_retry)
                 raise ManualRetryError(to_log_for_retry)
 
             if is_json_decodable or key_for_error:
                 is_response_bad(result=result, key_for_error=key_for_error, output_to_stdout=output_to_stdout)
 
         except (ResultNotOKError, ManualRetryError, JSONDecodeError, KeyError) as e:
-            logger.exception(e)
+            ic(e)
             time.sleep(timeout * exponential_backoff**n)
         else:
             return result
 
     return result
```

### Comparing `ai_transform-0.30.9/ai_transform/components/components.py` & `ai_transform-0.31.0/ai_transform/components/components.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/config.py` & `ai_transform-0.31.0/ai_transform/config.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/dataset/dataset.py` & `ai_transform-0.31.0/ai_transform/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ai_transform.api.api import API
 from ai_transform.api.helpers import process_token
 from ai_transform.types import Filter, Schema, GroupBy, Metric
 from ai_transform.errors import MaxRetriesError
 from ai_transform.dataset.field import Field, KeyphraseField, ClusterField
 from ai_transform.utils.document import Document
 from ai_transform.utils.document_list import DocumentList
-
+from ai_transform.logger import ic
 from concurrent.futures import ThreadPoolExecutor
 
 
 logging.basicConfig(level=logging.DEBUG)
 logger = logging.getLogger()
 
 
@@ -173,23 +173,23 @@
                     worker_number=worker_number,
                     sort=sort,
                     include_vector=include_vector,
                     random_state=random_state,
                     is_random=is_random,
                 )
             except ConnectionError as e:
-                logger.exception(e)
+                ic(e)
                 retry_count += 1
                 time.sleep(retry_delay)
 
                 if retry_count >= max_retries:
                     raise MaxRetriesError("max number of retries exceeded")
 
             except JSONDecodeError as e:
-                logger.exception(e)
+                ic(e)
                 retry_count += 1
                 time.sleep(retry_delay)
 
                 if retry_count >= max_retries:
                     raise MaxRetriesError("max number of retries exceeded")
 
             else:
```

### Comparing `ai_transform-0.30.9/ai_transform/dataset/field.py` & `ai_transform-0.31.0/ai_transform/dataset/field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/engine/abstract_engine.py` & `ai_transform-0.31.0/ai_transform/engine/abstract_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,24 @@
 
 from json import JSONDecodeError
 from typing import Any, List, Optional, Sequence, Iterator
 from abc import ABC, abstractmethod
 
 from tqdm.auto import tqdm
 
-from ai_transform.logger import format_logging_info
+from ai_transform.logger import format_logging_info, ic
 from ai_transform.types import Filter
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.operator.abstract_operator import AbstractOperator
 
 from ai_transform.utils.document import Document
 from ai_transform.utils.document_list import DocumentList
 
 from ai_transform.errors import MaxRetriesError
 
-logging.basicConfig(level=logging.DEBUG, format="%(asctime)s:%(levelname)s:%(name)s:%(message)s")
-logger = logging.getLogger(__name__)
-
 
 class AbstractEngine(ABC):
     MAX_SCHEMA_UPDATE_LIMITER: int = 1
 
     def __init__(
         self,
         dataset: Dataset = None,
@@ -195,16 +192,16 @@
         self.set_success_ratio()
 
     def _operate(self, mini_batch):
         try:
             # note: do not put an IF inside ths try-except-else loop - the if code will not work
             transformed_batch = self.operator(mini_batch)
         except Exception as e:
-            logger.exception(e)
-            logger.error(format_logging_info({"chunk_ids": self._get_chunks_ids(mini_batch)}))
+            ic(e)
+            ic({"chunk_ids": self._get_chunks_ids(mini_batch)})
         else:
             # if there is no exception then this block will be executed
             # we only update schema on the first chunk
             # otherwise it breaks down how the backend handles
             # schema updates
             self._successful_documents += len(mini_batch)
             return transformed_batch
@@ -295,15 +292,15 @@
                     worker_number=self.worker_number,
                     sort=sort,
                     include_vector=include_vector,
                     random_state=random_state,
                     is_random=is_random,
                 )
             except (ConnectionError, JSONDecodeError) as e:
-                logger.exception(e)
+                ic(e)
                 retry_count += 1
                 time.sleep(1)
 
                 if retry_count >= max_retries:
                     raise MaxRetriesError("max number of retries exceeded")
             else:
                 self._after_id = chunk["after_id"]
@@ -341,15 +338,15 @@
         if chunk:
             for _ in range(max_retries):
                 try:
                     update_json = self._dataset.update_documents(
                         documents=chunk, ingest_in_background=ingest_in_background, update_schema=update_schema
                     )
                 except Exception as e:
-                    logger.exception(e)
+                    ic(e)
                 else:
                     return update_json
 
             raise MaxRetriesError("max number of retries exceeded")
 
     def api_progress(
         self,
@@ -409,15 +406,15 @@
 
     def set_success_ratio(self) -> None:
         if self.size:
             denominator = self.size * len(self.operators)
             self._success_ratio = self._successful_documents / denominator
         else:
             self._success_ratio = 1
-        logger.debug(format_logging_info({"success_ratio": self._success_ratio}))
+        ic({"success_ratio": self._success_ratio})
 
     @staticmethod
     def _filter_for_non_empty_list(documents: List[Document]) -> List[Document]:
         # if there are more keys than just _id in each document
         # then return that as a list of Documents
         # length of a dictionary is just 1 if there is only 1 key
         return DocumentList([document for document in documents if len(document.keys()) > 1])
```

### Comparing `ai_transform-0.30.9/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.31.0/ai_transform/engine/dense_output_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 
 from typing import Optional, List, Sequence
 
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.operator.dense_operator import DenseOperator
 from ai_transform.engine.abstract_engine import AbstractEngine
 from ai_transform.types import Filter
-
-
-logger = logging.getLogger(__file__)
+from ai_transform.logger import ic
 
 
 class DenseOutputEngine(AbstractEngine):
     def __init__(
         self,
         dataset: Dataset = None,
         operator: DenseOperator = None,
@@ -74,15 +72,15 @@
         for mega_batch in self.api_progress(iterator):
             for mini_batch in AbstractEngine.chunk_documents(self._transform_chunksize, mega_batch):
                 document_mapping = self._operate(mini_batch)
                 for dataset_id, documents in document_mapping.items():
                     output_dataset_ids.append(dataset_id)
                     dataset = Dataset.from_details(dataset_id, self.token)
                     result = dataset.bulk_insert(documents)
-                    logger.debug({"dataset_id": dataset_id, "result": result})
+                    ic({"dataset_id": dataset_id, "result": result})
 
         self.operator.post_hooks(self._dataset)
 
         output_datasets = self.datasets_from_ids(output_dataset_ids)
         self.operator.store_dataset_relationship(self.dataset, output_datasets)
 
     def datasets_from_ids(self, dataset_ids: Sequence[str]) -> Sequence[Dataset]:
```

### Comparing `ai_transform-0.30.9/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.31.0/ai_transform/engine/in_memory_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/engine/multipass_engine.py` & `ai_transform-0.31.0/ai_transform/engine/multipass_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import logging
 
 from typing import Optional, Sequence, List
 
-from ai_transform.logger import format_logging_info
+from ai_transform.logger import format_logging_info, ic
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.operator.abstract_operator import AbstractOperator
 from ai_transform.engine.abstract_engine import AbstractEngine
 from ai_transform.utils.document import Document
 from ai_transform.types import Filter
 
-logger = logging.getLogger(__file__)
-
 
 class MultiPassEngine(AbstractEngine):
     def __init__(
         self,
         dataset: Dataset = None,
         operators: Sequence[AbstractOperator] = None,
         filters: Optional[List[Filter]] = None,
@@ -70,23 +68,23 @@
                 ingest_in_background = True
 
             result = self.update_chunk(
                 batch_to_insert,
                 update_schema=batch_index < self.MAX_SCHEMA_UPDATE_LIMITER,
                 ingest_in_background=ingest_in_background,
             )
-            logger.debug(format_logging_info(result))
+            ic(result)
 
     def _operate(self, operator: AbstractOperator, mini_batch: List[Document]):
         try:
             # note: do not put an IF inside ths try-except-else loop - the if code will not work
             transformed_batch = operator(mini_batch)
         except Exception as e:
-            logger.exception(e)
-            logger.error(format_logging_info({"chunk_ids": self._get_chunks_ids(mini_batch)}))
+            ic(e)
+            ic({"chunk_ids": self._get_chunks_ids(mini_batch)})
         else:
             # if there is no exception then this block will be executed
             # we only update schema on the first chunk
             # otherwise it breaks down how the backend handles
             # schema updates
             self._successful_documents += len(mini_batch)
             return transformed_batch
```

### Comparing `ai_transform-0.30.9/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.31.0/ai_transform/engine/small_batch_stable_engine.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,27 +5,22 @@
         3. Upserts all 1000 documents.
         4. Repeat until dataset has finished looping
 
     We download a large chunk and upsert large chunks to avoid hammering
     our servers.
 
 """
-import logging
-
 from typing import List
-
-from ai_transform.logger import format_logging_info
+from ai_transform.logger import format_logging_info, ic
 from ai_transform.operator.abstract_operator import AbstractOperator
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.engine.abstract_engine import AbstractEngine
 from ai_transform.utils.document_list import DocumentList
 from ai_transform.utils.document import Document
 
-logger = logging.getLogger(__file__)
-
 
 class SmallBatchStableEngine(AbstractEngine):
     def __init__(
         self,
         dataset: Dataset,
         operator: AbstractOperator,
         pull_chunksize: int = 5,
@@ -56,15 +51,15 @@
             ingest_in_background = True
 
         result = self.update_chunk(
             chunk_to_update,
             update_schema=chunk_counter < self.MAX_SCHEMA_UPDATE_LIMITER,
             ingest_in_background=ingest_in_background,
         )
-        logger.debug(format_logging_info(result))
+        ic(result)
 
     def _transform_and_upsert(self, batch_index: int, batch: List[Document]):
         batch_to_insert = []
 
         for chunk in AbstractEngine.chunk_documents(self._transform_chunksize, batch):
             transformed_batch = self._operate(chunk)
             if transformed_batch is not None:
```

### Comparing `ai_transform-0.30.9/ai_transform/engine/stable_engine.py` & `ai_transform-0.31.0/ai_transform/engine/stable_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,21 @@
     our servers.
 
 """
 import logging
 
 from typing import Optional, List
 
-from ai_transform.logger import format_logging_info
+from ai_transform.logger import ic, format_logging_info
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.operator.abstract_operator import AbstractOperator
 from ai_transform.engine.abstract_engine import AbstractEngine
 from ai_transform.utils.document import Document
 from ai_transform.types import Filter
 
-logger = logging.getLogger(__file__)
-
 
 class StableEngine(AbstractEngine):
     def __init__(
         self,
         dataset: Dataset = None,
         operator: AbstractOperator = None,
         filters: Optional[List[Filter]] = None,
@@ -75,15 +73,15 @@
                 ingest_in_background = True
 
             result = self.update_chunk(
                 batch_to_insert,
                 update_schema=batch_index < self.MAX_SCHEMA_UPDATE_LIMITER,
                 ingest_in_background=ingest_in_background,
             )
-            logger.debug(format_logging_info(result))
+            ic(result)
 
     def apply(self) -> None:
         """
         Returns the ratio of successful chunks / total chunks needed to iterate over the dataset
         """
         iterator = self.get_iterator()
```

### Comparing `ai_transform-0.30.9/ai_transform/errors.py` & `ai_transform-0.31.0/ai_transform/errors.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/logger.py` & `ai_transform-0.31.0/ai_transform/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pprint
 import logging
-
+import datetime
+from icecream import ic
 from typing import Dict, Any, List
 from ai_transform.utils.document import Document
 from ai_transform.utils.document_list import DocumentList
 
 
 def format_logging_info(info: Dict[str, Any], indent=4, width=80, depth=None, compact=True, sort_dicts=False):
     return "\n" + pprint.pformat(info, indent=indent, width=width, depth=depth, compact=compact, sort_dicts=sort_dicts)
@@ -28,7 +29,16 @@
             if isinstance(info[0], Document):
                 info_to_log = [document.to_json() for document in info]
 
         else:
             info_to_log = info
 
         self._logger.debug(format_logging_info(info_to_log))
+
+
+def time_format():
+    timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+    return f"{timestamp} | "
+
+
+ic.configureOutput(prefix=time_format, includeContext=True)
+# Change all printing statements
```

### Comparing `ai_transform-0.30.9/ai_transform/operator/abstract_operator.py` & `ai_transform-0.31.0/ai_transform/operator/abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/operator/dense_operator.py` & `ai_transform-0.31.0/ai_transform/operator/dense_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/timer.py` & `ai_transform-0.31.0/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/types.py` & `ai_transform-0.31.0/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/utils/document.py` & `ai_transform-0.31.0/ai_transform/utils/document.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/utils/document_list.py` & `ai_transform-0.31.0/ai_transform/utils/document_list.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/utils/example_documents.py` & `ai_transform-0.31.0/ai_transform/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/utils/json_encoder.py` & `ai_transform-0.31.0/ai_transform/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/utils/keyphrase.py` & `ai_transform-0.31.0/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.31.0/ai_transform/workflow/abstract_workflow.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform/workflow/context_manager.py` & `ai_transform-0.31.0/ai_transform/workflow/context_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,15 @@
 from ai_transform.types import Credentials
 from ai_transform.dataset import dataset
 from ai_transform.operator import abstract_operator
 from ai_transform.engine import abstract_engine
 from ai_transform.logger import format_logging_info
 from ai_transform.api.wrappers import request_wrapper
 from ai_transform.errors import UserFacingError
-
-logging.basicConfig(level=logging.DEBUG, format="%(asctime)s:%(levelname)s:%(name)s:%(message)s")
-
-logger = logging.getLogger(__file__)
-
+from ai_transform.logger import ic
 
 WORKFLOW_FAIL_MESSAGE = (
     "Workflow processed {:.2f}%" + " of documents. This is less than the success threshold of {:.2f}%"
 )
 
 
 class WorkflowContextManager:
@@ -107,15 +103,15 @@
                         metadata.update(operator.output_fields)
 
                     output_fields = list(operator.output_fields)
 
                     res = self.dataset[input_field].add_field_children(
                         field_children=output_fields, fieldchildren_id=self.job_id, metadata=metadata, recursive=True
                     )
-                    logger.debug(format_logging_info(res))
+                    ic(res)
 
     def _get_output_to_status_obj(self):
         if self.output is not None:
             output = self.output
             if self.output_documents is not None:
                 output["documents"] = self.output_documents
         else:
@@ -131,27 +127,27 @@
             additional_information=self.additional_information,
             send_email=self.send_email,
             email=self.email,
             worker_number=self.worker_number,
             user_errors=user_errors,
             output=self._get_output_to_status_obj(),
         )
-        logger.debug(format_logging_info(result))
+        ic(result)
         return result
 
     def __enter__(self):
         if self.operators is not None:
             self._set_field_children_recursively()
         self.set_workflow_status(status=self.IN_PROGRESS)
         return self
 
     def _handle_workflow_fail(
         self, exc_type: type, exc_value: BaseException, traceback: Traceback, user_errors: str = None
     ):
-        logger.exception(exc_value)
+        ic(exc_value)
         self.set_workflow_status(status=self.FAILED, user_errors=user_errors)
         return False
 
     def _handle_workflow_complete(self):
         self.set_workflow_status(status=self.COMPLETE)
         return True
```

### Comparing `ai_transform-0.30.9/ai_transform/workflow/helpers.py` & `ai_transform-0.31.0/ai_transform/workflow/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.31.0/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/setup.py` & `ai_transform-0.31.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 from ai_transform import __version__
 
-requirements = ["tqdm>=4.49.0", "requests>=2.0.0", "pandas>=1.5.0", "pydantic>=1.10.2"]
+requirements = ["tqdm>=4.49.0", "requests>=2.0.0", "pandas>=1.5.0", "pydantic>=1.10.2", "icecream==2.1.3"]
 
 ray_requirements = ["numpy>=1.19.0", "pyarrow==9.0.0", "ray==2.0.0"]
 
 core_test_requirements = ["pytest", "pytest-xdist", "pytest-cov", "sentence-splitter"]
 
 example_test_requirements = core_test_requirements + ["torch", "scikit-learn>=0.20.0", "transformers[torch]==4.18.0"]
```

### Comparing `ai_transform-0.30.9/tests/conftest.py` & `ai_transform-0.31.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_api/test_client.py` & `ai_transform-0.31.0/tests/core/test_api/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,7 +31,11 @@
         time.sleep(2)
 
         all_documents = dataset.get_all_documents()["documents"]
         all_ids = [document["_id"] for document in all_documents]
 
         assert len(all_documents) == (n_test_docs - len(_ids))
         assert all([_id not in all_ids for _id in _ids])
+
+    def test_no_auth_client(self):
+        client = Client(token="this:token:doesn't:work", authenticate=False)
+        assert True
```

### Comparing `ai_transform-0.30.9/tests/core/test_api/test_endpoints.py` & `ai_transform-0.31.0/tests/core/test_api/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.31.0/tests/core/test_api/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_api/test_wrappers.py` & `ai_transform-0.31.0/tests/core/test_api/test_wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from ai_transform.api.wrappers import request_wrapper
 from contextlib import redirect_stdout, redirect_stderr
 
 
 class TestWrappers:
     def test_request_wrapper_fail_with_error_in_logs(self):
         f = io.StringIO()
-        saved_stdout = sys.stdout
-        sys.stdout = f
+        saved_stdout = sys.stderr
+        sys.stderr = f
         resp = request_wrapper(
             requests.post, args=["https://www.google.com"], num_retries=1, timeout=1, output_to_stdout=True
         )
         output = f.getvalue()
-        sys.stdout = saved_stdout
+        sys.stderr = saved_stdout
         assert "status_code" in output
         assert "message" in output
 
     def test_request_wrapper_fail_2(self):
         f = io.StringIO()
         u = io.StringIO()
 
@@ -90,15 +90,15 @@
                 TestRequest(), ("https://www.google.com",), num_retries=3, timeout=1, output_to_stdout=True
             )
 
         assert resp.status_code == 200
 
         logs = str(u.getvalue()) + str(f.getvalue())
 
-        assert logs.count("Simulated Rate Error") == 2
+        assert logs.count("Simulated Rate Error") == 4
 
     def test_request_wrapper_json(self):
         f = io.StringIO()
         u = io.StringIO()
 
         class TestRequest:
             def __init__(self):
@@ -160,8 +160,8 @@
                 key_for_error="bad_key",
             )
 
         assert resp.status_code == 200
 
         logs = str(u.getvalue()) + str(f.getvalue())
 
-        assert logs.count("bad_key") == 2
+        assert logs.count("bad_key") == 4
```

### Comparing `ai_transform-0.30.9/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.31.0/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_dataset/test_field.py` & `ai_transform-0.31.0/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.31.0/tests/core/test_dataset/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_engine/test_dense_output_engine.py` & `ai_transform-0.31.0/tests/core/test_engine/test_dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_engine/test_engine.py` & `ai_transform-0.31.0/tests/core/test_engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.31.0/tests/core/test_engine/test_engine_playground.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.31.0/tests/core/test_engine/test_multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.31.0/tests/core/test_engine/test_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_operator/test_abstract_operator.py` & `ai_transform-0.31.0/tests/core/test_operator/test_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.31.0/tests/core/test_operator/test_document_diff.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.31.0/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.30.9/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.31.0/tests/core/test_workflow/test_workflow.py`

 * *Files identical despite different names*

