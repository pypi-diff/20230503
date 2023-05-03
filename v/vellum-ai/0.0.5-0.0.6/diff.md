# Comparing `tmp/vellum_ai-0.0.5.tar.gz` & `tmp/vellum_ai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vellum_ai-0.0.5.tar", max compression
+gzip compressed data, was "vellum_ai-0.0.6.tar", max compression
```

## Comparing `vellum_ai-0.0.5.tar` & `vellum_ai-0.0.6.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0      413 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2619 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/__init__.py
--rw-r--r--   0        0        0     8763 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/client.py
--rw-r--r--   0        0        0      348 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/core/__init__.py
--rw-r--r--   0        0        0      426 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      498 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/environment.py
--rw-r--r--   0        0        0        0 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/py.typed
--rw-r--r--   0        0        0      148 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/resources/documents/__init__.py
--rw-r--r--   0        0        0     5625 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/resources/model_versions/__init__.py
--rw-r--r--   0        0        0     2282 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/resources/model_versions/client.py
--rw-r--r--   0        0        0     3803 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/__init__.py
--rw-r--r--   0        0        0      830 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/block_type_enum.py
--rw-r--r--   0        0        0      633 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/chat_role_enum.py
--rw-r--r--   0        0        0     1117 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/document.py
--rw-r--r--   0        0        0     1268 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/document_document_to_document_index.py
--rw-r--r--   0        0        0     1714 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/enriched_normalized_completion.py
--rw-r--r--   0        0        0      639 2023-04-26 01:08:16.267506 vellum_ai-0.0.5/src/vellum/types/finish_reason_enum.py
--rw-r--r--   0        0        0      831 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_error_response.py
--rw-r--r--   0        0        0      929 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_options_request.py
--rw-r--r--   0        0        0     1186 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_request.py
--rw-r--r--   0        0        0     1246 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_response.py
--rw-r--r--   0        0        0     1326 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_result.py
--rw-r--r--   0        0        0      992 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_result_data.py
--rw-r--r--   0        0        0      840 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/generate_result_error.py
--rw-r--r--   0        0        0     1012 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/indexing_state_enum.py
--rw-r--r--   0        0        0      435 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/logprobs_enum.py
--rw-r--r--   0        0        0      483 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_type_enum.py
--rw-r--r--   0        0        0     1241 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_version_build_config.py
--rw-r--r--   0        0        0     1004 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_version_exec_config_parameters.py
--rw-r--r--   0        0        0     1421 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_version_exec_config_read.py
--rw-r--r--   0        0        0     2056 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_version_read.py
--rw-r--r--   0        0        0      895 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_version_read_status_enum.py
--rw-r--r--   0        0        0      934 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/model_version_sandbox_snapshot.py
--rw-r--r--   0        0        0      873 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/normalized_log_probs.py
--rw-r--r--   0        0        0      840 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/normalized_token_log_probs.py
--rw-r--r--   0        0        0      939 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/paginated_slim_document_list.py
--rw-r--r--   0        0        0      835 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/processing_state_enum.py
--rw-r--r--   0        0        0      934 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/prompt_template_block.py
--rw-r--r--   0        0        0      860 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/prompt_template_block_data.py
--rw-r--r--   0        0        0      977 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/prompt_template_block_properties.py
--rw-r--r--   0        0        0     1039 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/provider_enum.py
--rw-r--r--   0        0        0      829 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_error_response.py
--rw-r--r--   0        0        0      881 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_filters_request.py
--rw-r--r--   0        0        0     1486 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_request_options_request.py
--rw-r--r--   0        0        0      952 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_response.py
--rw-r--r--   0        0        0     1157 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_result.py
--rw-r--r--   0        0        0      834 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_result_merging_request.py
--rw-r--r--   0        0        0      961 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/search_weights_request.py
--rw-r--r--   0        0        0     2009 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/slim_document.py
--rw-r--r--   0        0        0      351 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/slim_document_status_enum.py
--rw-r--r--   0        0        0     1778 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/submit_completion_actual_request.py
--rw-r--r--   0        0        0      772 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/submit_completion_actuals_error_response.py
--rw-r--r--   0        0        0      763 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/upload_document_error_response.py
--rw-r--r--   0        0        0      837 2023-04-26 01:08:16.271506 vellum_ai-0.0.5/src/vellum/types/upload_document_response.py
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 vellum_ai-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      413 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2675 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/__init__.py
+-rw-r--r--   0        0        0     8763 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/client.py
+-rw-r--r--   0        0        0      348 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      498 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/environment.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/py.typed
+-rw-r--r--   0        0        0      148 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/resources/documents/__init__.py
+-rw-r--r--   0        0        0     5769 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/resources/model_versions/__init__.py
+-rw-r--r--   0        0        0     2282 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/resources/model_versions/client.py
+-rw-r--r--   0        0        0     3891 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/__init__.py
+-rw-r--r--   0        0        0      830 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/block_type_enum.py
+-rw-r--r--   0        0        0      825 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/chat_message_request.py
+-rw-r--r--   0        0        0      645 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/chat_message_role.py
+-rw-r--r--   0        0        0     1117 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/document.py
+-rw-r--r--   0        0        0     1268 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/document_document_to_document_index.py
+-rw-r--r--   0        0        0     1745 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/enriched_normalized_completion.py
+-rw-r--r--   0        0        0      639 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/finish_reason_enum.py
+-rw-r--r--   0        0        0      831 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_error_response.py
+-rw-r--r--   0        0        0      929 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_options_request.py
+-rw-r--r--   0        0        0     1514 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_request.py
+-rw-r--r--   0        0        0     1246 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_response.py
+-rw-r--r--   0        0        0     1326 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_result.py
+-rw-r--r--   0        0        0      992 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_result_data.py
+-rw-r--r--   0        0        0      840 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/generate_result_error.py
+-rw-r--r--   0        0        0     1012 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/indexing_state_enum.py
+-rw-r--r--   0        0        0      435 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/logprobs_enum.py
+-rw-r--r--   0        0        0      483 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_type_enum.py
+-rw-r--r--   0        0        0     1241 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_version_build_config.py
+-rw-r--r--   0        0        0     1021 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_version_exec_config_parameters.py
+-rw-r--r--   0        0        0     1421 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_version_exec_config_read.py
+-rw-r--r--   0        0        0     2056 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_version_read.py
+-rw-r--r--   0        0        0      895 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_version_read_status_enum.py
+-rw-r--r--   0        0        0      934 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/model_version_sandbox_snapshot.py
+-rw-r--r--   0        0        0      890 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/normalized_log_probs.py
+-rw-r--r--   0        0        0      891 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/normalized_token_log_probs.py
+-rw-r--r--   0        0        0      939 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/paginated_slim_document_list.py
+-rw-r--r--   0        0        0      835 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/processing_state_enum.py
+-rw-r--r--   0        0        0      934 2023-05-03 19:14:31.932031 vellum_ai-0.0.6/src/vellum/types/prompt_template_block.py
+-rw-r--r--   0        0        0      860 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/prompt_template_block_data.py
+-rw-r--r--   0        0        0      986 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/prompt_template_block_properties.py
+-rw-r--r--   0        0        0     1039 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/provider_enum.py
+-rw-r--r--   0        0        0      829 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_error_response.py
+-rw-r--r--   0        0        0      881 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_filters_request.py
+-rw-r--r--   0        0        0     1486 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_request_options_request.py
+-rw-r--r--   0        0        0      952 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_response.py
+-rw-r--r--   0        0        0     1157 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_result.py
+-rw-r--r--   0        0        0      834 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_result_merging_request.py
+-rw-r--r--   0        0        0      961 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/search_weights_request.py
+-rw-r--r--   0        0        0     2009 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/slim_document.py
+-rw-r--r--   0        0        0      351 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/slim_document_status_enum.py
+-rw-r--r--   0        0        0     1778 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/submit_completion_actual_request.py
+-rw-r--r--   0        0        0      772 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/submit_completion_actuals_error_response.py
+-rw-r--r--   0        0        0      763 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/upload_document_error_response.py
+-rw-r--r--   0        0        0      837 2023-05-03 19:14:31.936031 vellum_ai-0.0.6/src/vellum/types/upload_document_response.py
+-rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 vellum_ai-0.0.6/PKG-INFO
```

### Comparing `vellum_ai-0.0.5/src/vellum/__init__.py` & `vellum_ai-0.0.6/src/vellum/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .environment import VellumEnvironment
 from .resources import documents, model_versions
 from .types import (
     BlockTypeEnum,
-    ChatRoleEnum,
+    ChatMessageRequest,
+    ChatMessageRole,
     Document,
     DocumentDocumentToDocumentIndex,
     EnrichedNormalizedCompletion,
     FinishReasonEnum,
     GenerateErrorResponse,
     GenerateOptionsRequest,
     GenerateRequest,
@@ -46,15 +47,16 @@
     SubmitCompletionActualsErrorResponse,
     UploadDocumentErrorResponse,
     UploadDocumentResponse,
 )
 
 __all__ = [
     "BlockTypeEnum",
-    "ChatRoleEnum",
+    "ChatMessageRequest",
+    "ChatMessageRole",
     "Document",
     "DocumentDocumentToDocumentIndex",
     "EnrichedNormalizedCompletion",
     "FinishReasonEnum",
     "GenerateErrorResponse",
     "GenerateOptionsRequest",
     "GenerateRequest",
```

### Comparing `vellum_ai-0.0.5/src/vellum/client.py` & `vellum_ai-0.0.6/src/vellum/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/core/datetime_utils.py` & `vellum_ai-0.0.6/src/vellum/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/core/jsonable_encoder.py` & `vellum_ai-0.0.6/src/vellum/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/resources/documents/client.py` & `vellum_ai-0.0.6/src/vellum/resources/documents/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,19 +42,19 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def upload(
         self,
         *,
-        add_to_index_names: typing.List[str],
-        external_id: str,
+        add_to_index_names: typing.Optional[typing.List[str]] = None,
+        external_id: typing.Optional[str] = None,
         label: str,
         contents: typing.IO,
-        keywords: typing.List[str],
+        keywords: typing.Optional[typing.List[str]] = None,
     ) -> UploadDocumentResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.documents}/", "v1/upload-document"),
             data=jsonable_encoder(
                 {
                     "add_to_index_names": add_to_index_names,
@@ -104,19 +104,19 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def upload(
         self,
         *,
-        add_to_index_names: typing.List[str],
-        external_id: str,
+        add_to_index_names: typing.Optional[typing.List[str]] = None,
+        external_id: typing.Optional[str] = None,
         label: str,
         contents: typing.IO,
-        keywords: typing.List[str],
+        keywords: typing.Optional[typing.List[str]] = None,
     ) -> UploadDocumentResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.documents}/", "v1/upload-document"),
                 data=jsonable_encoder(
                     {
```

### Comparing `vellum_ai-0.0.5/src/vellum/resources/model_versions/client.py` & `vellum_ai-0.0.6/src/vellum/resources/model_versions/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/__init__.py` & `vellum_ai-0.0.6/src/vellum/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .block_type_enum import BlockTypeEnum
-from .chat_role_enum import ChatRoleEnum
+from .chat_message_request import ChatMessageRequest
+from .chat_message_role import ChatMessageRole
 from .document import Document
 from .document_document_to_document_index import DocumentDocumentToDocumentIndex
 from .enriched_normalized_completion import EnrichedNormalizedCompletion
 from .finish_reason_enum import FinishReasonEnum
 from .generate_error_response import GenerateErrorResponse
 from .generate_options_request import GenerateOptionsRequest
 from .generate_request import GenerateRequest
@@ -42,15 +43,16 @@
 from .submit_completion_actual_request import SubmitCompletionActualRequest
 from .submit_completion_actuals_error_response import SubmitCompletionActualsErrorResponse
 from .upload_document_error_response import UploadDocumentErrorResponse
 from .upload_document_response import UploadDocumentResponse
 
 __all__ = [
     "BlockTypeEnum",
-    "ChatRoleEnum",
+    "ChatMessageRequest",
+    "ChatMessageRole",
     "Document",
     "DocumentDocumentToDocumentIndex",
     "EnrichedNormalizedCompletion",
     "FinishReasonEnum",
     "GenerateErrorResponse",
     "GenerateOptionsRequest",
     "GenerateRequest",
```

### Comparing `vellum_ai-0.0.5/src/vellum/types/block_type_enum.py` & `vellum_ai-0.0.6/src/vellum/types/block_type_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/document.py` & `vellum_ai-0.0.6/src/vellum/types/document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/document_document_to_document_index.py` & `vellum_ai-0.0.6/src/vellum/types/document_document_to_document_index.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/enriched_normalized_completion.py` & `vellum_ai-0.0.6/src/vellum/types/enriched_normalized_completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     id: str = pydantic.Field(description=("The Vellum-generated ID of the completion.\n"))
     external_id: typing.Optional[str] = pydantic.Field(
         description=(
             "The external ID that was originally provided along with the generation request, which uniquely identifies this generation in an external system.\n"
         )
     )
     text: str = pydantic.Field(description=("The text generated by the LLM.\n"))
-    finish_reason: FinishReasonEnum = pydantic.Field(description=("The reason the generation finished.\n"))
+    finish_reason: typing.Optional[FinishReasonEnum] = pydantic.Field(
+        description=("The reason the generation finished.\n")
+    )
     logprobs: typing.Optional[NormalizedLogProbs] = pydantic.Field(
         description=("The logprobs of the completion. Only present if specified in the original request options.\n")
     )
     model_version_id: str = pydantic.Field(
         description=("The ID of the model version used to generate this completion.\n")
     )
```

### Comparing `vellum_ai-0.0.5/src/vellum/types/finish_reason_enum.py` & `vellum_ai-0.0.6/src/vellum/types/finish_reason_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/generate_error_response.py` & `vellum_ai-0.0.6/src/vellum/types/generate_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/generate_options_request.py` & `vellum_ai-0.0.6/src/vellum/types/generate_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/generate_request.py` & `vellum_ai-0.0.6/src/vellum/types/generate_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .chat_message_request import ChatMessageRequest
 
 
 class GenerateRequest(pydantic.BaseModel):
     input_values: typing.Dict[str, typing.Any] = pydantic.Field(
         description=("Key/value pairs for each template variable defined in the deployment's prompt.\n")
     )
+    chat_history: typing.Optional[typing.List[ChatMessageRequest]] = pydantic.Field(
+        description=(
+            "Optionally provide a list of chat messages that'll be used in place of the special {$chat_history} variable, if included in the prompt.\n"
+        )
+    )
     external_ids: typing.Optional[typing.List[str]] = pydantic.Field(
         description=(
             "Optionally include a unique identifier for each generation, as represented outside of Vellum. Note that this should generally be a list of length one.\n"
         )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `vellum_ai-0.0.5/src/vellum/types/generate_response.py` & `vellum_ai-0.0.6/src/vellum/types/generate_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/generate_result.py` & `vellum_ai-0.0.6/src/vellum/types/generate_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/generate_result_data.py` & `vellum_ai-0.0.6/src/vellum/types/generate_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/generate_result_error.py` & `vellum_ai-0.0.6/src/vellum/types/generate_result_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/indexing_state_enum.py` & `vellum_ai-0.0.6/src/vellum/types/indexing_state_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/model_version_build_config.py` & `vellum_ai-0.0.6/src/vellum/types/model_version_build_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/model_version_exec_config_parameters.py` & `vellum_ai-0.0.6/src/vellum/types/normalized_token_log_probs.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,23 +4,19 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class ModelVersionExecConfigParameters(pydantic.BaseModel):
-    temperature: float
-    max_tokens: int
-    stop: typing.List[str]
-    top_p: float
-    top_k: typing.Optional[float]
-    frequency_penalty: float
-    presence_penalty: float
-    logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]]
+class NormalizedTokenLogProbs(pydantic.BaseModel):
+    token: str
+    logprob: typing.Optional[float]
+    top_logprobs: typing.Optional[typing.Dict[str, typing.Optional[float]]]
+    text_offset: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.0.5/src/vellum/types/model_version_exec_config_read.py` & `vellum_ai-0.0.6/src/vellum/types/model_version_exec_config_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/model_version_read.py` & `vellum_ai-0.0.6/src/vellum/types/model_version_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/model_version_read_status_enum.py` & `vellum_ai-0.0.6/src/vellum/types/model_version_read_status_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/model_version_sandbox_snapshot.py` & `vellum_ai-0.0.6/src/vellum/types/model_version_sandbox_snapshot.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/normalized_log_probs.py` & `vellum_ai-0.0.6/src/vellum/types/normalized_log_probs.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ..core.datetime_utils import serialize_datetime
 from .normalized_token_log_probs import NormalizedTokenLogProbs
 
 
 class NormalizedLogProbs(pydantic.BaseModel):
     tokens: typing.List[NormalizedTokenLogProbs]
-    likelihood: float
+    likelihood: typing.Optional[float]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.0.5/src/vellum/types/normalized_token_log_probs.py` & `vellum_ai-0.0.6/src/vellum/types/paginated_slim_document_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .slim_document import SlimDocument
 
 
-class NormalizedTokenLogProbs(pydantic.BaseModel):
-    token: str
-    logprob: float
-    top_logprobs: typing.Dict[str, float]
-    text_offset: int
+class PaginatedSlimDocumentList(pydantic.BaseModel):
+    count: typing.Optional[int]
+    next: typing.Optional[str]
+    previous: typing.Optional[str]
+    results: typing.Optional[typing.List[SlimDocument]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.0.5/src/vellum/types/paginated_slim_document_list.py` & `vellum_ai-0.0.6/src/vellum/types/model_version_exec_config_parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .slim_document import SlimDocument
 
 
-class PaginatedSlimDocumentList(pydantic.BaseModel):
-    count: typing.Optional[int]
-    next: typing.Optional[str]
-    previous: typing.Optional[str]
-    results: typing.Optional[typing.List[SlimDocument]]
+class ModelVersionExecConfigParameters(pydantic.BaseModel):
+    temperature: float
+    max_tokens: int
+    stop: typing.Optional[typing.List[str]]
+    top_p: float
+    top_k: typing.Optional[float]
+    frequency_penalty: float
+    presence_penalty: float
+    logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.0.5/src/vellum/types/processing_state_enum.py` & `vellum_ai-0.0.6/src/vellum/types/processing_state_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/prompt_template_block.py` & `vellum_ai-0.0.6/src/vellum/types/prompt_template_block.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/prompt_template_block_data.py` & `vellum_ai-0.0.6/src/vellum/types/prompt_template_block_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/prompt_template_block_properties.py` & `vellum_ai-0.0.6/src/vellum/types/search_filters_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_role_enum import ChatRoleEnum
 
 
-class PromptTemplateBlockProperties(pydantic.BaseModel):
-    chat_role: typing.Optional[ChatRoleEnum]
-    text: typing.Optional[str]
-    variable_name: typing.Optional[str]
-    blocks: typing.Optional[typing.List[typing.Dict[str, typing.Any]]]
+class SearchFiltersRequest(pydantic.BaseModel):
+    external_ids: typing.Optional[typing.List[str]] = pydantic.Field(
+        description=("The document external IDs to filter by\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.0.5/src/vellum/types/provider_enum.py` & `vellum_ai-0.0.6/src/vellum/types/provider_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/search_error_response.py` & `vellum_ai-0.0.6/src/vellum/types/search_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/search_filters_request.py` & `vellum_ai-0.0.6/src/vellum/types/upload_document_error_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class SearchFiltersRequest(pydantic.BaseModel):
-    external_ids: typing.Optional[typing.List[str]] = pydantic.Field(
-        description=("The document external IDs to filter by\n")
-    )
+class UploadDocumentErrorResponse(pydantic.BaseModel):
+    detail: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.0.5/src/vellum/types/search_request_options_request.py` & `vellum_ai-0.0.6/src/vellum/types/search_request_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/search_response.py` & `vellum_ai-0.0.6/src/vellum/types/search_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/search_result.py` & `vellum_ai-0.0.6/src/vellum/types/search_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/search_result_merging_request.py` & `vellum_ai-0.0.6/src/vellum/types/search_result_merging_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/search_weights_request.py` & `vellum_ai-0.0.6/src/vellum/types/search_weights_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/slim_document.py` & `vellum_ai-0.0.6/src/vellum/types/slim_document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/submit_completion_actual_request.py` & `vellum_ai-0.0.6/src/vellum/types/submit_completion_actual_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/submit_completion_actuals_error_response.py` & `vellum_ai-0.0.6/src/vellum/types/submit_completion_actuals_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/src/vellum/types/upload_document_error_response.py` & `vellum_ai-0.0.6/src/vellum/types/prompt_template_block_properties.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .chat_message_role import ChatMessageRole
 
 
-class UploadDocumentErrorResponse(pydantic.BaseModel):
-    detail: str
+class PromptTemplateBlockProperties(pydantic.BaseModel):
+    chat_role: typing.Optional[ChatMessageRole]
+    text: typing.Optional[str]
+    variable_name: typing.Optional[str]
+    blocks: typing.Optional[typing.List[typing.Dict[str, typing.Any]]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.0.5/src/vellum/types/upload_document_response.py` & `vellum_ai-0.0.6/src/vellum/types/upload_document_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.0.5/PKG-INFO` & `vellum_ai-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vellum-ai
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

