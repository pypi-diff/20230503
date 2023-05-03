# Comparing `tmp/bigeye_sdk-0.4.52.tar.gz` & `tmp/bigeye_sdk-0.4.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigeye_sdk-0.4.52.tar", max compression
+gzip compressed data, was "bigeye_sdk-0.4.53.tar", max compression
```

## Comparing `bigeye_sdk-0.4.52.tar` & `bigeye_sdk-0.4.53.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     2092 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/LICENSE
--rw-r--r--   0        0        0      873 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/README.md
--rw-r--r--   0        0        0     3727 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/__init__.py
--rw-r--r--   0        0        0       82 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/__version__.py
--rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/authentication/__init__.py
--rw-r--r--   0        0        0    17489 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/authentication/api_authentication.py
--rw-r--r--   0        0        0     2122 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/authentication/credentials.py
--rw-r--r--   0        0        0      734 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/authentication/enums.py
--rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/__init__.py
--rw-r--r--   0        0        0    10223 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/big_config_reports.py
--rw-r--r--   0        0        0     8116 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/validation_context.py
--rw-r--r--   0        0        0     1579 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/validation_functions.py
--rw-r--r--   0        0        0      701 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/validation_models.py
--rw-r--r--   0        0        0     9206 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/yaml_model_base.py
--rw-r--r--   0        0        0     3042 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
--rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/class_ext/__init__.py
--rw-r--r--   0        0        0      233 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/class_ext/dataclass_ext.py
--rw-r--r--   0        0        0      402 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/class_ext/enum_ext.py
--rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/client/__init__.py
--rw-r--r--   0        0        0      389 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/client/base_client.py
--rw-r--r--   0        0        0    39770 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/client/datawatch_client.py
--rw-r--r--   0        0        0      201 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/client/enum.py
--rw-r--r--   0        0        0    38235 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/client/generated_datawatch_client.py
--rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/controller/__init__.py
--rw-r--r--   0        0        0      390 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/controller/metric_controller.py
--rw-r--r--   0        0        0    32599 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/controller/metric_suite_controller.py
--rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/decorators/__init__.py
--rw-r--r--   0        0        0      307 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/decorators/dataclass_decorators.py
--rw-r--r--   0        0        0       97 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0      907 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/__init__.py
--rw-r--r--   0        0        0     4469 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/athena.py
--rw-r--r--   0        0        0     5202 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/aws.py
--rw-r--r--   0        0        0     3343 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/bigconfig_functions.py
--rw-r--r--   0        0        0     3469 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/casing.py
--rw-r--r--   0        0        0     3215 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/core_py_functs.py
--rw-r--r--   0        0        0     4517 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/delta_functions.py
--rw-r--r--   0        0        0     2544 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/file_functs.py
--rw-r--r--   0        0        0      117 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/helpers.py
--rw-r--r--   0        0        0    20233 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/metric_functions.py
--rw-r--r--   0        0        0     1554 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/metric_run_functions.py
--rw-r--r--   0        0        0     1227 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/s3.py
--rw-r--r--   0        0        0     1676 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/schema_functions.py
--rw-r--r--   0        0        0     5089 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/search_and_match_functions.py
--rw-r--r--   0        0        0     4032 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/table_functions.py
--rw-r--r--   0        0        0     1701 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/functions/urlfuncts.py
--rw-r--r--   0        0        0        0 2023-04-26 20:04:19.590497 bigeye_sdk-0.4.52/bigeye_sdk/generated/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/generated/com/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/generated/com/bigeye/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/generated/com/bigeye/models/__init__.py
--rw-r--r--   0        0        0   202792 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/generated/com/bigeye/models/generated.py
--rw-r--r--   0        0        0        0 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/generated/google/__init__.py
--rw-r--r--   0        0        0    14816 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/generated/google/api.py
--rw-r--r--   0        0        0      507 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/log/__init__.py
--rw-r--r--   0        0        0        1 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/__init__.py
--rw-r--r--   0        0        0      489 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/base_datawatch_facade.py
--rw-r--r--   0        0        0    22303 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/big_config.py
--rw-r--r--   0        0        0      778 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/collection_models.py
--rw-r--r--   0        0        0     3584 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/dbt_schema.py
--rw-r--r--   0        0        0     3504 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/delta_facade.py
--rw-r--r--   0        0        0     9456 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/metric_facade.py
--rw-r--r--   0        0        0     8396 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/protobuf_enum_facade.py
--rw-r--r--   0        0        0      220 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/protobuf_extensions.py
--rw-r--r--   0        0        0    45112 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/protobuf_message_facade.py
--rw-r--r--   0        0        0      865 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/model/sla_models.py
--rw-r--r--   0        0        0     7114 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/bigeye_sdk/serializable.py
--rw-r--r--   0        0        0     3709 2023-04-26 20:04:19.594497 bigeye_sdk-0.4.52/pyproject.toml
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.52/setup.py
--rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.52/PKG-INFO
+-rw-r--r--   0        0        0     2092 2023-01-13 19:29:40.987774 bigeye_sdk-0.4.53/LICENSE
+-rw-r--r--   0        0        0      873 2022-09-21 14:26:02.564243 bigeye_sdk-0.4.53/README.md
+-rw-r--r--   0        0        0     3727 2022-09-21 19:14:17.084238 bigeye_sdk-0.4.53/bigeye_sdk/__init__.py
+-rw-r--r--   0        0        0       82 2022-09-21 19:14:17.084343 bigeye_sdk-0.4.53/bigeye_sdk/__version__.py
+-rw-r--r--   0        0        0        0 2022-09-21 14:26:02.564505 bigeye_sdk-0.4.53/bigeye_sdk/authentication/__init__.py
+-rw-r--r--   0        0        0    17489 2023-03-24 00:17:08.953130 bigeye_sdk-0.4.53/bigeye_sdk/authentication/api_authentication.py
+-rw-r--r--   0        0        0     2122 2023-04-21 16:45:36.590395 bigeye_sdk-0.4.53/bigeye_sdk/authentication/credentials.py
+-rw-r--r--   0        0        0      734 2022-09-21 14:26:02.564714 bigeye_sdk-0.4.53/bigeye_sdk/authentication/enums.py
+-rw-r--r--   0        0        0        0 2022-09-21 19:14:17.084676 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/__init__.py
+-rw-r--r--   0        0        0    10264 2023-05-03 14:18:05.249247 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/big_config_reports.py
+-rw-r--r--   0        0        0     8116 2023-03-24 00:17:08.953740 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/validation_context.py
+-rw-r--r--   0        0        0     1579 2023-03-24 00:17:08.953972 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/validation_functions.py
+-rw-r--r--   0        0        0      701 2022-09-21 19:14:17.085326 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/validation_models.py
+-rw-r--r--   0        0        0     9206 2023-03-24 00:17:08.954155 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/yaml_model_base.py
+-rw-r--r--   0        0        0     3042 2023-03-24 00:17:08.954346 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
+-rw-r--r--   0        0        0        0 2022-09-21 14:26:02.565379 bigeye_sdk-0.4.53/bigeye_sdk/class_ext/__init__.py
+-rw-r--r--   0        0        0      233 2022-09-21 14:26:02.565502 bigeye_sdk-0.4.53/bigeye_sdk/class_ext/dataclass_ext.py
+-rw-r--r--   0        0        0      402 2022-10-11 14:47:52.093321 bigeye_sdk-0.4.53/bigeye_sdk/class_ext/enum_ext.py
+-rw-r--r--   0        0        0        0 2022-09-21 14:26:02.565649 bigeye_sdk-0.4.53/bigeye_sdk/client/__init__.py
+-rw-r--r--   0        0        0      389 2022-12-01 16:53:45.901990 bigeye_sdk-0.4.53/bigeye_sdk/client/base_client.py
+-rw-r--r--   0        0        0    39770 2023-03-24 00:17:08.954904 bigeye_sdk-0.4.53/bigeye_sdk/client/datawatch_client.py
+-rw-r--r--   0        0        0      201 2022-09-21 14:26:02.566284 bigeye_sdk-0.4.53/bigeye_sdk/client/enum.py
+-rw-r--r--   0        0        0    38235 2023-04-21 16:45:36.591609 bigeye_sdk-0.4.53/bigeye_sdk/client/generated_datawatch_client.py
+-rw-r--r--   0        0        0        0 2022-09-21 19:14:17.086145 bigeye_sdk-0.4.53/bigeye_sdk/controller/__init__.py
+-rw-r--r--   0        0        0      390 2022-11-30 18:19:48.731219 bigeye_sdk-0.4.53/bigeye_sdk/controller/metric_controller.py
+-rw-r--r--   0        0        0    32795 2023-05-03 14:18:05.249942 bigeye_sdk-0.4.53/bigeye_sdk/controller/metric_suite_controller.py
+-rw-r--r--   0        0        0        0 2022-09-21 14:26:02.566925 bigeye_sdk-0.4.53/bigeye_sdk/decorators/__init__.py
+-rw-r--r--   0        0        0      307 2022-09-21 19:14:17.086414 bigeye_sdk-0.4.53/bigeye_sdk/decorators/dataclass_decorators.py
+-rw-r--r--   0        0        0       97 2022-09-21 14:26:02.567122 bigeye_sdk-0.4.53/bigeye_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0      907 2023-03-24 00:17:08.955789 bigeye_sdk-0.4.53/bigeye_sdk/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2022-09-21 14:26:02.567221 bigeye_sdk-0.4.53/bigeye_sdk/functions/__init__.py
+-rw-r--r--   0        0        0     4469 2023-01-13 19:29:40.988379 bigeye_sdk-0.4.53/bigeye_sdk/functions/athena.py
+-rw-r--r--   0        0        0     5202 2022-10-18 15:49:05.166354 bigeye_sdk-0.4.53/bigeye_sdk/functions/aws.py
+-rw-r--r--   0        0        0     3343 2023-02-03 22:21:16.752839 bigeye_sdk-0.4.53/bigeye_sdk/functions/bigconfig_functions.py
+-rw-r--r--   0        0        0     3469 2022-09-21 14:26:02.567414 bigeye_sdk-0.4.53/bigeye_sdk/functions/casing.py
+-rw-r--r--   0        0        0     3215 2022-09-21 19:14:17.086730 bigeye_sdk-0.4.53/bigeye_sdk/functions/core_py_functs.py
+-rw-r--r--   0        0        0     4517 2022-11-30 18:19:48.731507 bigeye_sdk-0.4.53/bigeye_sdk/functions/delta_functions.py
+-rw-r--r--   0        0        0     2544 2023-03-24 00:17:08.955960 bigeye_sdk-0.4.53/bigeye_sdk/functions/file_functs.py
+-rw-r--r--   0        0        0      117 2023-04-21 16:45:36.592265 bigeye_sdk-0.4.53/bigeye_sdk/functions/helpers.py
+-rw-r--r--   0        0        0    20235 2023-04-26 20:01:53.246118 bigeye_sdk-0.4.53/bigeye_sdk/functions/metric_functions.py
+-rw-r--r--   0        0        0     1554 2022-12-01 16:53:45.902364 bigeye_sdk-0.4.53/bigeye_sdk/functions/metric_run_functions.py
+-rw-r--r--   0        0        0     1227 2022-10-11 14:47:52.094658 bigeye_sdk-0.4.53/bigeye_sdk/functions/s3.py
+-rw-r--r--   0        0        0     1676 2023-01-13 19:29:40.988609 bigeye_sdk-0.4.53/bigeye_sdk/functions/schema_functions.py
+-rw-r--r--   0        0        0     5089 2023-03-24 00:17:08.956184 bigeye_sdk-0.4.53/bigeye_sdk/functions/search_and_match_functions.py
+-rw-r--r--   0        0        0     4032 2023-03-24 00:17:08.956445 bigeye_sdk-0.4.53/bigeye_sdk/functions/table_functions.py
+-rw-r--r--   0        0        0     1701 2023-04-21 16:45:36.592782 bigeye_sdk-0.4.53/bigeye_sdk/functions/urlfuncts.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:16:32.073745 bigeye_sdk-0.4.53/bigeye_sdk/generated/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:16:32.073842 bigeye_sdk-0.4.53/bigeye_sdk/generated/com/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:16:32.073917 bigeye_sdk-0.4.53/bigeye_sdk/generated/com/bigeye/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:16:32.073968 bigeye_sdk-0.4.53/bigeye_sdk/generated/com/bigeye/models/__init__.py
+-rw-r--r--   0        0        0   206459 2023-05-03 15:16:32.074052 bigeye_sdk-0.4.53/bigeye_sdk/generated/com/bigeye/models/generated.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:16:32.074184 bigeye_sdk-0.4.53/bigeye_sdk/generated/google/__init__.py
+-rw-r--r--   0        0        0    14816 2023-05-03 15:16:32.074235 bigeye_sdk-0.4.53/bigeye_sdk/generated/google/api.py
+-rw-r--r--   0        0        0      507 2022-09-21 14:26:02.569285 bigeye_sdk-0.4.53/bigeye_sdk/log/__init__.py
+-rw-r--r--   0        0        0        1 2022-09-21 19:14:17.088368 bigeye_sdk-0.4.53/bigeye_sdk/model/__init__.py
+-rw-r--r--   0        0        0      489 2022-09-21 19:14:17.088495 bigeye_sdk-0.4.53/bigeye_sdk/model/base_datawatch_facade.py
+-rw-r--r--   0        0        0    22303 2023-03-24 00:17:08.956794 bigeye_sdk-0.4.53/bigeye_sdk/model/big_config.py
+-rw-r--r--   0        0        0      778 2023-02-23 17:53:03.561875 bigeye_sdk-0.4.53/bigeye_sdk/model/collection_models.py
+-rw-r--r--   0        0        0     3948 2023-05-03 14:18:05.251140 bigeye_sdk-0.4.53/bigeye_sdk/model/dbt_schema.py
+-rw-r--r--   0        0        0     3504 2023-03-24 00:17:08.957102 bigeye_sdk-0.4.53/bigeye_sdk/model/delta_facade.py
+-rw-r--r--   0        0        0     9456 2023-01-13 19:29:40.989263 bigeye_sdk-0.4.53/bigeye_sdk/model/metric_facade.py
+-rw-r--r--   0        0        0     8396 2023-04-21 16:45:36.594969 bigeye_sdk-0.4.53/bigeye_sdk/model/protobuf_enum_facade.py
+-rw-r--r--   0        0        0      220 2022-11-30 18:19:48.733054 bigeye_sdk-0.4.53/bigeye_sdk/model/protobuf_extensions.py
+-rw-r--r--   0        0        0    45112 2023-04-25 19:45:34.950560 bigeye_sdk-0.4.53/bigeye_sdk/model/protobuf_message_facade.py
+-rw-r--r--   0        0        0      865 2023-02-22 23:48:15.904646 bigeye_sdk-0.4.53/bigeye_sdk/model/sla_models.py
+-rw-r--r--   0        0        0     7114 2023-04-20 17:39:55.335256 bigeye_sdk-0.4.53/bigeye_sdk/serializable.py
+-rw-r--r--   0        0        0     3709 2023-05-03 14:18:05.251555 bigeye_sdk-0.4.53/pyproject.toml
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.53/setup.py
+-rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.53/PKG-INFO
```

### Comparing `bigeye_sdk-0.4.52/LICENSE` & `bigeye_sdk-0.4.53/LICENSE`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/README.md` & `bigeye_sdk-0.4.53/README.md`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/__init__.py` & `bigeye_sdk-0.4.53/bigeye_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/authentication/api_authentication.py` & `bigeye_sdk-0.4.53/bigeye_sdk/authentication/api_authentication.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/authentication/credentials.py` & `bigeye_sdk-0.4.53/bigeye_sdk/authentication/credentials.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/authentication/enums.py` & `bigeye_sdk-0.4.53/bigeye_sdk/authentication/enums.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/big_config_reports.py` & `bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/big_config_reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,34 +80,42 @@
     not_supported = True
     return not_supported in [
         True if f"Metric type {mm.predefined_metric} not supported on table {invalid.fq_asset_name}" in
                 invalid.error_messages else False for mm in SimpleMetricType.get_metadata_metrics()
     ]
 
 
-def process_reports(output_path: str):
+def process_reports(output_path: str, strict_mode: bool):
     report_files = []
     errors_reported = False
 
     source_reports = []
 
     for report in REPORTS:
         file_name = f'{output_path}/{report.source_name.replace(" ", "_")}_{report.process_stage}.yml'
         report.save(file_name)
         report_files.append(file_name)
         errors_reported = errors_reported or report.has_errors()
         source_reports.append(report.get_console_report())
 
-    if errors_reported:
+    if errors_reported and strict_mode:
         raise BigConfigValidationException(
             FAILED_API_EXECUTION_MSG.format(
                 source_reports="\n".join(source_reports),
                 report_file_list="\n".join(report_files)
             )
         )
+    elif errors_reported:
+        print(
+            FAILED_API_EXECUTION_MSG.format(
+                source_reports="\n".join(source_reports),
+                report_file_list="\n".join(report_files)
+            )
+        )
+        print(f"Strict mode is OFF. There are errors reported.")
     else:
         print(
             SUCCESSFUL_API_EXECUTION_MSG.format(
                 source_reports="\n".join(source_reports),
                 report_file_list="\n".join(report_files)
             )
         )
@@ -201,31 +209,32 @@
 Deleted Metric Count: {self.deleted_metric_count}
 Unchanged Metric Count: {self.unchanged_metric_count}
 Row Creation Time Upsert Failure Count: {self.row_creation_time_upsert_failure_count}
 Metric Application Error Count: {self.metric_application_error_count}
 Invalid Asset Identifier Count: {self.invalid_asset_identifier_count}
 Total Error Count: {self.tot_error_count()}"""
 
-        if self.row_creation_time_upsert_failure_count:
-            source_report = f"""{source_report}
-
-Row creation Time Upsert Failures:
-{yaml.safe_dump(self.row_creation_time_report['row_creation_time_upsert_failures'])}"""
-
-        if self.metric_application_errors:
-            source_report = f"""{source_report}
-        
-Metric Application Errors:
-{yaml.safe_dump(self.metric_application_errors)}"""
-
-        if self.invalid_asset_identifier_errors:
-            source_report = f"""{source_report}
-
-Invalid Asset Identifier Errors:
-{yaml.safe_dump(self.invalid_asset_identifier_errors)}"""
+# These are all available in the report and clutter the console.
+#         if self.row_creation_time_upsert_failure_count:
+#             source_report = f"""{source_report}
+#
+# Row creation Time Upsert Failures:
+# {yaml.safe_dump(self.row_creation_time_report['row_creation_time_upsert_failures'])}"""
+#
+#         if self.metric_application_errors:
+#             source_report = f"""{source_report}
+#
+# Metric Application Errors:
+# {yaml.safe_dump(self.metric_application_errors)}"""
+#
+#         if self.invalid_asset_identifier_errors:
+#             source_report = f"""{source_report}
+#
+# Invalid Asset Identifier Errors:
+# {yaml.safe_dump(self.invalid_asset_identifier_errors)}"""
 
         return source_report
 
     def tot_error_count(self) -> int:
         return self.total_error_count
 
     def __init__(self, **data: Any):
@@ -251,20 +260,16 @@
 
         def is_wildcard_search(cohort: CohortDefinition):
             return '*' in cohort.column_name_pattern or \
                 '*' in cohort.table_name_pattern or \
                 '*' in cohort.schema_name_pattern
 
         for mae in obj.metric_application_errors:
-            if is_wildcard_search(mae.from_cohort) and metric_type_not_supported(mae):
-                continue
-            else:
-                "Adding error reporting where the metrics were not applied to assets containing wild cards and MMs not supported."
-                metric_application_errors.append(mae.to_dict())
-                # TODO add validation error.  Problem is that I cannot match back to the full fq pattern.
+            metric_application_errors.append(mae.to_dict())
+
 
         invalid_asset_identifier_errors = [ice.to_dict() for ice in obj.invalid_cohort_errors]
 
         pr = MetricSuiteReport(
             process_stage=process_stage,
             source_name=source_name,
             created_metrics=[i.to_dict(casing=Casing.SNAKE) for i in obj.created_metrics],
```

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/validation_context.py` & `bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/validation_context.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/validation_functions.py` & `bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/validation_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/validation_models.py` & `bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/validation_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/yaml_model_base.py` & `bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/yaml_model_base.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py` & `bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/client/datawatch_client.py` & `bigeye_sdk-0.4.53/bigeye_sdk/client/datawatch_client.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/client/generated_datawatch_client.py` & `bigeye_sdk-0.4.53/bigeye_sdk/client/generated_datawatch_client.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/controller/metric_suite_controller.py` & `bigeye_sdk-0.4.53/bigeye_sdk/controller/metric_suite_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,31 +520,34 @@
             apply: If true then Big Config will be applied to the workspace.  If false then a plan will be generated.
         """
         try:
             self.client.purge_metric_suites(source_names=purge_source_names,
                                             purge_all_sources=purge_all_sources,
                                             apply=apply
                                             )
-            process_reports(output_path=output_path)
+            process_reports(output_path=output_path, strict_mode=False)
         except NoSourcesFoundException as e:
             sys.exit(e.message)
 
     def execute_bigconfig(self,
                           input_path: List[str] = (Path.cwd()),
                           output_path: str = Path.cwd(),
                           apply: bool = False,
-                          no_queue: bool = False, recursive: bool = False):
+                          no_queue: bool = False,
+                          recursive: bool = False,
+                          strict_mode: bool = False):
         """
         Executes an Apply or Plan for a Big Config.
         Args:
             input_path: path of source files.  If no path is given the current working directory will be used.
             output_path: path to dump the reports.  If no path is given the current working directory will be used.
             apply: If true then Big Config will be applied to the workspace.  If false then a plan will be generated.
             no_queue: If true, the bigconfig will be run without queuing
             recursive: If true, search for files recursively
+            strict_mode: If true errors from the API raise an exception.
         Returns: None
 
         """
         files: List[BIGCONFIG_FILE] = _find_bigconfig_files(input_path, recursive=recursive)
 
         bigconfig: BigConfig = combine_bigconfigs(files)
 
@@ -583,15 +586,15 @@
             else:
                 response = self.client.post_metric_suite_queue(metric_suite=metric_suite)
             process_stage = ProcessStage.APPLY if apply else ProcessStage.PLAN
             MetricSuiteReport.from_datawatch_object(response,
                                                     source_name=self.sources_by_id_ix[metric_suite.source_id].name,
                                                     process_stage=process_stage)
 
-        process_reports(output_path=output_path)
+        process_reports(output_path=output_path, strict_mode=strict_mode)
 
 
 def combine_bigconfigs(bigconfigs: List[BigConfig]) -> BigConfig:
     to_return: BigConfig = BigConfig(
         type="BIGCONFIG_FILE",
         tag_definitions=[],
         row_creation_times=RowCreationTimes(),
```

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/exceptions/exceptions.py` & `bigeye_sdk-0.4.53/bigeye_sdk/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/athena.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/athena.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/aws.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/aws.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/bigconfig_functions.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/bigconfig_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/casing.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/casing.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/core_py_functs.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/core_py_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/delta_functions.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/delta_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/file_functs.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/file_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/metric_functions.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/metric_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
     :param update_schedule: The update schedule as a cron string.
 
     :returns: dict
 
     >>> get_time_interval_for_delay_string("1 day", "HOURS_SINCE_MAX_DATE", "10 14 * * 1")
     {'intervalValue': 38, 'intervalType': 'HOURS_TIME_INTERVAL_TYPE'}
     """
-    split_input = delay_at_update.split(" ")
+    split_input = delay_at_update.split(" ",1)
     interval_value = int(split_input[0])
     interval_type = get_proto_interval_type(split_input[1])
     if metric_type == "HOURS_SINCE_MAX_DATE":
         hours_from_cron = get_max_hours_from_cron(update_schedule)
         if interval_type == "HOURS_TIME_INTERVAL_TYPE" or interval_type == "MINUTES_TIME_INTERVAL_TYPE":
             logging.warning("Delay granularity for date column must be in days, ignoring value")
             interval_type = "HOURS_TIME_INTERVAL_TYPE"
```

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/metric_run_functions.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/metric_run_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/s3.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/s3.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/schema_functions.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/schema_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/search_and_match_functions.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/search_and_match_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/table_functions.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/table_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/functions/urlfuncts.py` & `bigeye_sdk-0.4.53/bigeye_sdk/functions/urlfuncts.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/generated/com/bigeye/models/generated.py` & `bigeye_sdk-0.4.53/bigeye_sdk/generated/com/bigeye/models/generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
     TAGGABLE_ENTITY_TYPE_METRIC = 4
     TAGGABLE_ENTITY_TYPE_DELTA = 5
     TAGGABLE_ENTITY_TYPE_COLUMN = 6
     TAGGABLE_ENTITY_TYPE_SLA = 7
     TAGGABLE_ENTITY_TYPE_BI_TOOL = 8
     TAGGABLE_ENTITY_TYPE_TABLEAU_WORKBOOK = 9
     TAGGABLE_ENTITY_TYPE_N_WAY_DELTA = 10
+    TAGGABLE_ENTITY_TYPE_VIRTUAL_TABLE = 11
 
 
 class TableType(betterproto.Enum):
     TABLE_TYPE_UNSPECIFIED = 0
     TABLE_TYPE_TABLE = 1
     TABLE_TYPE_VIEW = 2
     TABLE_TYPE_VIRTUAL = 3
@@ -211,14 +212,24 @@
     PERCENT_AGGREGATION_TYPE = 2
     MIN_AGGREGATION_TYPE = 3
     MAX_AGGREGATION_TYPE = 4
     AVG_AGGREGATION_TYPE = 5
     SUM_AGGREGATION_TYPE = 6
 
 
+class MetricCategory(betterproto.Enum):
+    METRIC_CATEGORY_UNSPECIFIED = 0
+    METRIC_CATEGORY_PIPELINE_RELIABILITY = 1
+    METRIC_CATEGORY_UNIQUENESS = 2
+    METRIC_CATEGORY_COMPLETENESS = 3
+    METRIC_CATEGORY_DISTRIBUTIONS = 4
+    METRIC_CATEGORY_VALIDITY = 5
+    METRIC_CATEGORY_CUSTOM = 6
+
+
 class LookbackType(betterproto.Enum):
     UNDEFINED_LOOKBACK_TYPE = 0
     DATA_TIME_LOOKBACK_TYPE = 1
     CLOCK_TIME_LOOKBACK_TYPE = 2
     METRIC_TIME_LOOKBACK_TYPE = 3
 
 
@@ -577,14 +588,20 @@
 class RevisionType(betterproto.Enum):
     REVISION_TYPE_UNSPECIFIED = 0
     REVISION_TYPE_CREATE = 1
     REVISION_TYPE_UPDATE = 2
     REVISION_TYPE_DELETE = 3
 
 
+class DashboardDataPointType(betterproto.Enum):
+    NUMBER_OPEN_ISSUES = 0
+    AVERAGE_ISSUE_TIME_TO_ACTION = 1
+    AVERAGE_ISSUE_TIME_TO_CLOSE = 2
+
+
 class ModelTypes(betterproto.Enum):
     MODEL_TYPE_UNDEFINED = 0
     MODEL_TYPE_MONOCLE = 1
 
 
 class MetadataOperation(betterproto.Enum):
     METADATA_OPERATION_UNSPECIFIED = 0
@@ -2234,28 +2251,48 @@
     table_ids: List[int] = betterproto.int32_field(6)
     column_ids: List[int] = betterproto.int32_field(7)
     statuses: List[str] = betterproto.string_field(8)
     metric_types: List["PredefinedMetricName"] = betterproto.enum_field(9)
 
 
 @dataclass
+class BulkIssueUpdateWhereClause(betterproto.Message):
+    ids: List[int] = betterproto.int32_field(1)
+    search: str = betterproto.string_field(2)
+    search_all: bool = betterproto.bool_field(3)
+    source_ids: List[int] = betterproto.int32_field(4)
+    schema_ids: List[int] = betterproto.int32_field(5)
+    table_ids: List[int] = betterproto.int32_field(6)
+    column_ids: List[int] = betterproto.int32_field(7)
+    statuses: List[str] = betterproto.string_field(8)
+    metric_types: List["PredefinedMetricName"] = betterproto.enum_field(9)
+    metric_ids: List[int] = betterproto.int32_field(10)
+    collection_ids: List[int] = betterproto.int32_field(11)
+    priority: List["IssuePriority"] = betterproto.enum_field(12)
+    metric_status: List["MetricStatus"] = betterproto.enum_field(13)
+    metric_type: List["MetricType"] = betterproto.message_field(14)
+    min_opened_time: int = betterproto.int64_field(15)
+    max_opened_time: int = betterproto.int64_field(16)
+
+
+@dataclass
 class BulkMetricOperation(betterproto.Message):
     where: "WhereClause" = betterproto.message_field(1)
     edit_request: "MetricConfiguration" = betterproto.message_field(2)
     mute_request: "MuteRequest" = betterproto.message_field(3)
     is_run: bool = betterproto.bool_field(4)
     is_delete: bool = betterproto.bool_field(5)
     add_to_collection: int = betterproto.int32_field(6)
     remove_from_collection: int = betterproto.int32_field(7)
     backfill_request: "MetricBackfillRequest" = betterproto.message_field(8)
 
 
 @dataclass
 class BulkIssueUpdate(betterproto.Message):
-    where: "WhereClause" = betterproto.message_field(1)
+    where: "BulkIssueUpdateWhereClause" = betterproto.message_field(1)
     status_update: "IssueStatusUpdate" = betterproto.message_field(2)
     config_update: "IssueConfigUpdate" = betterproto.message_field(3)
 
 
 @dataclass
 class BulkDeltaOperation(betterproto.Message):
     where: "WhereClause" = betterproto.message_field(1)
@@ -3158,14 +3195,15 @@
     metric_names: List["PredefinedMetricName"] = betterproto.enum_field(1)
 
 
 @dataclass
 class FavoriteItem(betterproto.Message):
     entity_id: int = betterproto.int32_field(1)
     entity_type: "TaggableEntityType" = betterproto.enum_field(2)
+    entity_name: str = betterproto.string_field(3)
 
 
 @dataclass
 class FavoriteListResponse(betterproto.Message):
     favorites: List["FavoriteItem"] = betterproto.message_field(1)
 
 
@@ -3321,14 +3359,65 @@
 
 @dataclass
 class GetUserAuditLogResponse(betterproto.Message):
     revisions: List["UserRevision"] = betterproto.message_field(1)
 
 
 @dataclass
+class CalculateDashboardDataPointsRequest(betterproto.Message):
+    source_id: List[int] = betterproto.int32_field(1)
+    timestamp: int = betterproto.int64_field(2)
+
+
+@dataclass
+class DashboardDataPointsRequest(betterproto.Message):
+    company_id: str = betterproto.string_field(1)
+    workspace_ids: List[str] = betterproto.string_field(2)
+    source_ids: List[int] = betterproto.int32_field(3)
+    starting_timestamp: int = betterproto.int64_field(4)
+    ending_timestamp: int = betterproto.int64_field(5)
+    data_point_types: List["DashboardDataPointType"] = betterproto.enum_field(6)
+
+
+@dataclass
+class DashboardDataPointsResponse(betterproto.Message):
+    company_id: str = betterproto.string_field(1)
+    workspace_id: str = betterproto.string_field(2)
+    source_id: int = betterproto.int32_field(3)
+    starting_timestamp: int = betterproto.int64_field(4)
+    ending_timestamp: int = betterproto.int64_field(5)
+    data_point_types: List["DashboardDataPointType"] = betterproto.enum_field(6)
+    data_point_series: List["DashboardDataPointSeries"] = betterproto.message_field(7)
+
+
+@dataclass
+class DashboardDataPointSeries(betterproto.Message):
+    company_id: str = betterproto.string_field(1)
+    workspace_id: str = betterproto.string_field(2)
+    source_id: int = betterproto.int32_field(3)
+    key: str = betterproto.string_field(4)
+    starting_timestamp: int = betterproto.int64_field(5)
+    ending_timestamp: int = betterproto.int64_field(6)
+    data_point_type: "DashboardDataPointType" = betterproto.enum_field(7)
+    data_points: List["DashboardDataPoint"] = betterproto.message_field(8)
+
+
+@dataclass
+class DashboardDataPoint(betterproto.Message):
+    company_id: str = betterproto.string_field(1)
+    workspace_id: str = betterproto.string_field(2)
+    source_id: int = betterproto.int32_field(3)
+    key: str = betterproto.string_field(4)
+    data_timestamp: int = betterproto.int64_field(5)
+    data_point_type: "DashboardDataPointType" = betterproto.enum_field(6)
+    value: float = betterproto.double_field(7)
+    collected_timestamp: int = betterproto.int64_field(8)
+
+
+@dataclass
 class Empty(betterproto.Message):
     pass
 
 
 @dataclass
 class DimensionRun(betterproto.Message):
     dim_name: str = betterproto.string_field(1)
@@ -5069,15 +5158,15 @@
             request,
             GetIssueTableSummaryResponse,
         )
 
     async def bulk_update_issues(
         self,
         *,
-        where: Optional["WhereClause"] = None,
+        where: Optional["BulkIssueUpdateWhereClause"] = None,
         status_update: Optional["IssueStatusUpdate"] = None,
         config_update: Optional["IssueConfigUpdate"] = None,
     ) -> BulkResponse:
         """Performs bulk issues updates"""
 
         request = BulkIssueUpdate()
         if where is not None:
```

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/generated/google/api.py` & `bigeye_sdk-0.4.53/bigeye_sdk/generated/google/api.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/model/big_config.py` & `bigeye_sdk-0.4.53/bigeye_sdk/model/big_config.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/model/collection_models.py` & `bigeye_sdk-0.4.53/bigeye_sdk/model/collection_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/model/dbt_schema.py` & `bigeye_sdk-0.4.53/bigeye_sdk/model/dbt_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional
 
-from pydantic import Field, root_validator
+from pydantic import Field, root_validator, validator
 from pydantic_yaml import YamlModel
 
 from bigeye_sdk.model.protobuf_enum_facade import SimpleDbtTestToMetricType, SimpleAggregationType
 from bigeye_sdk.model.protobuf_message_facade import SimpleMetricDefinition, SimplePredefinedMetric, \
     SimpleMetricParameter, SimpleConstantThreshold, SimpleTemplateMetric
 
 relationships_test_names = ["relationships", "referential integrity", "referential integrity check"]
@@ -66,13 +66,23 @@
 
 
 class SimpleDbtModel(YamlModel):
     type = "model"
     name: str = ""
     description: Optional[str] = None
     columns: Optional[List[SimpleDbtColumn]] = Field(default_factory=lambda: [])
+    model_tests: Optional[List[SimpleMetricDefinition]] = Field(default_factory=lambda: [])
+
+    @validator('model_tests', always=True)
+    def add_model_tests(cls, field_value, values):
+        if values["columns"]:
+            cols = values["columns"]
+            for c in cols:
+                field_value.extend(c.tests)
+
+        return field_value
 
 
 class SimpleDbtSchema(YamlModel):
     type = "schema"
     version: int = 0
     models: List[SimpleDbtModel] = Field(default_factory=lambda: [])
```

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/model/delta_facade.py` & `bigeye_sdk-0.4.53/bigeye_sdk/model/delta_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/model/metric_facade.py` & `bigeye_sdk-0.4.53/bigeye_sdk/model/metric_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/model/protobuf_enum_facade.py` & `bigeye_sdk-0.4.53/bigeye_sdk/model/protobuf_enum_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/model/protobuf_message_facade.py` & `bigeye_sdk-0.4.53/bigeye_sdk/model/protobuf_message_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/model/sla_models.py` & `bigeye_sdk-0.4.53/bigeye_sdk/model/sla_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/bigeye_sdk/serializable.py` & `bigeye_sdk-0.4.53/bigeye_sdk/serializable.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.52/pyproject.toml` & `bigeye_sdk-0.4.53/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bigeye-sdk"
-version = "0.4.52"
+version = "0.4.53"
 description = "Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically."
 license = "Proprietary"
 authors = ["Bigeye <support@bigeye.com>"]
 readme = "README.md"
 homepage = "https://docs.bigeye.com/docs"
 
 [[tool.poetry.source]]
```

### Comparing `bigeye_sdk-0.4.52/setup.py` & `bigeye_sdk-0.4.53/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
  'requests==2.28.1',
  'setuptools>=59.6.0,<60.0.0',
  'smart-open>=6.1.0,<7.0.0',
  'types-PyYAML>=6.0.11,<7.0.0']
 
 setup_kwargs = {
     'name': 'bigeye-sdk',
-    'version': '0.4.52',
+    'version': '0.4.53',
     'description': 'Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically.',
     'long_description': '# Bigeye SDK\n\nBigeye SDK is a collection of protobuf generated code, functions, and models used to interact programmatically\nwith the Bigeye API.  Bigeye currently supports a Python SDK.  The main entry point is the DatawatchClient \nabstraction and, in this core package, a basic auth client has been implemented.  The abstract base class \nincludes core functionality (methods to interact with the API) and each implementation should enable a \ndifferent authorization methods.\n\n## Install\n\n```shell\npip install bigeye_sdk\n```\n\n## Basic Auth\n\nBasic authorization credentials can be stored as Json either on disk or in a secrets/credentials manager.  This\nformat will be marshalled into an instance of [BasicAuthRequestLibApiConf](bigeye_sdk/authentication/api_authentication.py).\n\n```json\n{\n    "base_url": "https://app.bigeye.com",\n    "user": "",\n    "password": ""\n}\n```\n',
     'author': 'Bigeye',
     'author_email': 'support@bigeye.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://docs.bigeye.com/docs',
```

### Comparing `bigeye_sdk-0.4.52/PKG-INFO` & `bigeye_sdk-0.4.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigeye-sdk
-Version: 0.4.52
+Version: 0.4.53
 Summary: Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically.
 Home-page: https://docs.bigeye.com/docs
 License: Proprietary
 Author: Bigeye
 Author-email: support@bigeye.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: Other/Proprietary License
```

