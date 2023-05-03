# Comparing `tmp/hsfs-3.2.0rc0.tar.gz` & `tmp/hsfs-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsfs-3.2.0rc0.tar", last modified: Wed Apr 12 12:41:00 2023, max compression
+gzip compressed data, was "hsfs-3.2.0rc1.tar", last modified: Wed May  3 08:10:55 2023, max compression
```

## Comparing `hsfs-3.2.0rc0.tar` & `hsfs-3.2.0rc1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.155222 hsfs-3.2.0rc0/
--rw-r--r--   0     1006     1006       40 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/MANIFEST.in
--rw-r--r--   0     1006     1006     7663 2023-04-12 12:41:00.155222 hsfs-3.2.0rc0/PKG-INFO
--rw-r--r--   0     1006     1006     5539 2023-04-12 12:40:58.000000 hsfs-3.2.0rc0/README.md
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.135222 hsfs-3.2.0rc0/hsfs/
--rw-r--r--   0     1006     1006     1182 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.139222 hsfs-3.2.0rc0/hsfs/client/
--rw-r--r--   0     1006     1006     1694 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/client/__init__.py
--rw-r--r--   0     1006     1006     1132 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/client/auth.py
--rw-r--r--   0     1006     1006     6622 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/client/base.py
--rw-r--r--   0     1006     1006     2090 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/client/exceptions.py
--rw-r--r--   0     1006     1006    11621 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/client/external.py
--rw-r--r--   0     1006     1006     7924 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/client/hopsworks.py
--rw-r--r--   0     1006     1006     1536 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/code.py
--rw-r--r--   0     1006     1006    18899 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/connection.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.143222 hsfs-3.2.0rc0/hsfs/constructor/
--rw-r--r--   0     1006     1006      605 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/__init__.py
--rw-r--r--   0     1006     1006     1261 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/external_feature_group_alias.py
--rw-r--r--   0     1006     1006     5106 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/filter.py
--rw-r--r--   0     1006     1006     2981 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/fs_query.py
--rw-r--r--   0     1006     1006     1731 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/hudi_feature_group_alias.py
--rw-r--r--   0     1006     1006     2157 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/join.py
--rw-r--r--   0     1006     1006     1577 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/prepared_statement_parameter.py
--rw-r--r--   0     1006     1006    20138 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/query.py
--rw-r--r--   0     1006     1006     3331 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/serving_prepared_statement.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.155222 hsfs-3.2.0rc0/hsfs/core/
--rw-r--r--   0     1006     1006      605 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/__init__.py
--rw-r--r--   0     1006     1006     3688 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/builtin_transformation_function.py
--rw-r--r--   0     1006     1006     1853 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/code_api.py
--rw-r--r--   0     1006     1006     3292 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/code_engine.py
--rw-r--r--   0     1006     1006     3509 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/dataset_api.py
--rw-r--r--   0     1006     1006     1030 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/deltastreamer_jobconf.py
--rw-r--r--   0     1006     1006     1609 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/execution.py
--rw-r--r--   0     1006     1006     5396 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/expectation_api.py
--rw-r--r--   0     1006     1006     2632 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/expectation_engine.py
--rw-r--r--   0     1006     1006     6356 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/expectation_suite_api.py
--rw-r--r--   0     1006     1006     4002 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/expectation_suite_engine.py
--rw-r--r--   0     1006     1006     9792 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/explicit_provenance.py
--rw-r--r--   0     1006     1006     5418 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/core/external_feature_group_engine.py
--rw-r--r--   0     1006     1006    13334 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/feature_group_api.py
--rw-r--r--   0     1006     1006     6610 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/core/feature_group_base_engine.py
--rw-r--r--   0     1006     1006    13164 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/core/feature_group_engine.py
--rw-r--r--   0     1006     1006     1238 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/feature_store_api.py
--rw-r--r--   0     1006     1006     9739 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/feature_view_api.py
--rw-r--r--   0     1006     1006    24896 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/core/feature_view_engine.py
--rw-r--r--   0     1006     1006     5024 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/core/great_expectation_engine.py
--rw-r--r--   0     1006     1006      828 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/hosts_api.py
--rw-r--r--   0     1006     1006    11546 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/hudi_engine.py
--rw-r--r--   0     1006     1006     1211 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/ingestion_job.py
--rw-r--r--   0     1006     1006     2262 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/ingestion_job_conf.py
--rw-r--r--   0     1006     1006     1077 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/inode.py
--rw-r--r--   0     1006     1006     2539 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/job.py
--rw-r--r--   0     1006     1006     1975 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/job_api.py
--rw-r--r--   0     1006     1006     2048 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/job_configuration.py
--rw-r--r--   0     1006     1006     1530 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/kafka_api.py
--rw-r--r--   0     1006     1006      898 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/project_api.py
--rw-r--r--   0     1006     1006     1093 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/query_constructor_api.py
--rw-r--r--   0     1006     1006      875 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/services_api.py
--rw-r--r--   0     1006     1006     4204 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/statistics_api.py
--rw-r--r--   0     1006     1006     8159 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/statistics_engine.py
--rw-r--r--   0     1006     1006     2325 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/storage_connector_api.py
--rw-r--r--   0     1006     1006     4696 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/tags_api.py
--rw-r--r--   0     1006     1006     6685 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/training_dataset_api.py
--rw-r--r--   0     1006     1006     6357 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/training_dataset_engine.py
--rw-r--r--   0     1006     1006     2148 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/training_dataset_job_conf.py
--rw-r--r--   0     1006     1006     4161 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/transformation_function_api.py
--rw-r--r--   0     1006     1006    14792 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/transformation_function_engine.py
--rw-r--r--   0     1006     1006     4773 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/validation_report_api.py
--rw-r--r--   0     1006     1006     3640 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/validation_report_engine.py
--rw-r--r--   0     1006     1006     2158 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/validation_result_api.py
--rw-r--r--   0     1006     1006     5469 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/validation_result_engine.py
--rw-r--r--   0     1006     1006     1261 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/variable_api.py
--rw-r--r--   0     1006     1006    18519 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/core/vector_server.py
--rw-r--r--   0     1006     1006     1655 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/decorators.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.155222 hsfs-3.2.0rc0/hsfs/engine/
--rw-r--r--   0     1006     1006     2244 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/engine/__init__.py
--rw-r--r--   0     1006     1006    45592 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/engine/python.py
--rw-r--r--   0     1006     1006    42820 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/engine/spark.py
--rw-r--r--   0     1006     1006    21585 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/expectation_suite.py
--rw-r--r--   0     1006     1006     6857 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/feature.py
--rw-r--r--   0     1006     1006   110708 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/feature_group.py
--rw-r--r--   0     1006     1006     3424 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/feature_group_commit.py
--rw-r--r--   0     1006     1006     1986 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/feature_group_writer.py
--rw-r--r--   0     1006     1006    62935 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/feature_store.py
--rw-r--r--   0     1006     1006    95713 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/feature_view.py
--rw-r--r--   0     1006     1006     4822 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/ge_expectation.py
--rw-r--r--   0     1006     1006     8633 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/ge_validation_result.py
--rw-r--r--   0     1006     1006     1450 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/split_statistics.py
--rw-r--r--   0     1006     1006     2893 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/statistics.py
--rw-r--r--   0     1006     1006     3313 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/statistics_config.py
--rw-r--r--   0     1006     1006    39092 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/storage_connector.py
--rw-r--r--   0     1006     1006     1850 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/tag.py
--rw-r--r--   0     1006     1006    35625 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/training_dataset.py
--rw-r--r--   0     1006     1006     3542 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/training_dataset_feature.py
--rw-r--r--   0     1006     1006     2759 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/training_dataset_split.py
--rw-r--r--   0     1006     1006     8929 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/transformation_function.py
--rw-r--r--   0     1006     1006     2179 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/transformation_function_attached.py
--rw-r--r--   0     1006     1006     3491 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/user.py
--rw-r--r--   0     1006     1006    11410 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/util.py
--rw-r--r--   0     1006     1006     7519 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/validation_report.py
--rw-r--r--   0     1006     1006      631 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/version.py
-drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.139222 hsfs-3.2.0rc0/hsfs.egg-info/
--rw-r--r--   0     1006     1006     7663 2023-04-12 12:40:59.000000 hsfs-3.2.0rc0/hsfs.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     2805 2023-04-12 12:41:00.000000 hsfs-3.2.0rc0/hsfs.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2023-04-12 12:40:59.000000 hsfs-3.2.0rc0/hsfs.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      679 2023-04-12 12:40:59.000000 hsfs-3.2.0rc0/hsfs.egg-info/requires.txt
--rw-r--r--   0     1006     1006        5 2023-04-12 12:40:59.000000 hsfs-3.2.0rc0/hsfs.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2023-04-12 12:41:00.155222 hsfs-3.2.0rc0/setup.cfg
--rw-r--r--   0     1006     1006     2706 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/setup.py
+drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.312981 hsfs-3.2.0rc1/
+-rw-r--r--   0     1006     1006       40 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/MANIFEST.in
+-rw-r--r--   0     1006     1006     7714 2023-05-03 08:10:55.312981 hsfs-3.2.0rc1/PKG-INFO
+-rw-r--r--   0     1006     1006     5539 2023-05-03 08:10:53.000000 hsfs-3.2.0rc1/README.md
+drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.292981 hsfs-3.2.0rc1/hsfs/
+-rw-r--r--   0     1006     1006     1182 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.296981 hsfs-3.2.0rc1/hsfs/client/
+-rw-r--r--   0     1006     1006     1694 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/client/__init__.py
+-rw-r--r--   0     1006     1006     1132 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/client/auth.py
+-rw-r--r--   0     1006     1006     6622 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/client/base.py
+-rw-r--r--   0     1006     1006     2090 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/client/exceptions.py
+-rw-r--r--   0     1006     1006    11621 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/client/external.py
+-rw-r--r--   0     1006     1006     7924 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/client/hopsworks.py
+-rw-r--r--   0     1006     1006     1536 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/code.py
+-rw-r--r--   0     1006     1006    18899 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/connection.py
+drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.300981 hsfs-3.2.0rc1/hsfs/constructor/
+-rw-r--r--   0     1006     1006      605 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/constructor/__init__.py
+-rw-r--r--   0     1006     1006     1261 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/constructor/external_feature_group_alias.py
+-rw-r--r--   0     1006     1006     5106 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/constructor/filter.py
+-rw-r--r--   0     1006     1006     2981 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/constructor/fs_query.py
+-rw-r--r--   0     1006     1006     1731 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/constructor/hudi_feature_group_alias.py
+-rw-r--r--   0     1006     1006     2157 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/constructor/join.py
+-rw-r--r--   0     1006     1006     1577 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/constructor/prepared_statement_parameter.py
+-rw-r--r--   0     1006     1006    20138 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/constructor/query.py
+-rw-r--r--   0     1006     1006     3331 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/constructor/serving_prepared_statement.py
+drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.312981 hsfs-3.2.0rc1/hsfs/core/
+-rw-r--r--   0     1006     1006      605 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/__init__.py
+-rw-r--r--   0     1006     1006     3688 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/builtin_transformation_function.py
+-rw-r--r--   0     1006     1006     1853 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/code_api.py
+-rw-r--r--   0     1006     1006     3292 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/code_engine.py
+-rw-r--r--   0     1006     1006     3509 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/dataset_api.py
+-rw-r--r--   0     1006     1006     1030 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/deltastreamer_jobconf.py
+-rw-r--r--   0     1006     1006     1609 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/execution.py
+-rw-r--r--   0     1006     1006     5396 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/expectation_api.py
+-rw-r--r--   0     1006     1006     2632 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/expectation_engine.py
+-rw-r--r--   0     1006     1006     6356 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/expectation_suite_api.py
+-rw-r--r--   0     1006     1006     4002 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/expectation_suite_engine.py
+-rw-r--r--   0     1006     1006     9792 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/explicit_provenance.py
+-rw-r--r--   0     1006     1006     5418 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/external_feature_group_engine.py
+-rw-r--r--   0     1006     1006    13334 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/feature_group_api.py
+-rw-r--r--   0     1006     1006     6610 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/feature_group_base_engine.py
+-rw-r--r--   0     1006     1006    13164 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/feature_group_engine.py
+-rw-r--r--   0     1006     1006     1238 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/feature_store_api.py
+-rw-r--r--   0     1006     1006     9739 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/feature_view_api.py
+-rw-r--r--   0     1006     1006    24896 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/feature_view_engine.py
+-rw-r--r--   0     1006     1006     5024 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/great_expectation_engine.py
+-rw-r--r--   0     1006     1006      828 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/hosts_api.py
+-rw-r--r--   0     1006     1006    11546 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/hudi_engine.py
+-rw-r--r--   0     1006     1006     1211 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/ingestion_job.py
+-rw-r--r--   0     1006     1006     2262 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/ingestion_job_conf.py
+-rw-r--r--   0     1006     1006     1077 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/inode.py
+-rw-r--r--   0     1006     1006     2906 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/job.py
+-rw-r--r--   0     1006     1006     2004 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/job_api.py
+-rw-r--r--   0     1006     1006     2048 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/job_configuration.py
+-rw-r--r--   0     1006     1006     1530 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/kafka_api.py
+-rw-r--r--   0     1006     1006      898 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/project_api.py
+-rw-r--r--   0     1006     1006     1093 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/query_constructor_api.py
+-rw-r--r--   0     1006     1006      875 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/services_api.py
+-rw-r--r--   0     1006     1006     4204 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/statistics_api.py
+-rw-r--r--   0     1006     1006     8159 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/statistics_engine.py
+-rw-r--r--   0     1006     1006     2325 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/storage_connector_api.py
+-rw-r--r--   0     1006     1006     4696 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/tags_api.py
+-rw-r--r--   0     1006     1006     6685 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/training_dataset_api.py
+-rw-r--r--   0     1006     1006     6357 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/training_dataset_engine.py
+-rw-r--r--   0     1006     1006     2148 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/training_dataset_job_conf.py
+-rw-r--r--   0     1006     1006     4161 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/transformation_function_api.py
+-rw-r--r--   0     1006     1006    14792 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/transformation_function_engine.py
+-rw-r--r--   0     1006     1006     4773 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/validation_report_api.py
+-rw-r--r--   0     1006     1006     3640 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/validation_report_engine.py
+-rw-r--r--   0     1006     1006     2158 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/validation_result_api.py
+-rw-r--r--   0     1006     1006     5469 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/validation_result_engine.py
+-rw-r--r--   0     1006     1006     1261 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/variable_api.py
+-rw-r--r--   0     1006     1006    18519 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/vector_server.py
+-rw-r--r--   0     1006     1006     1655 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/decorators.py
+drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.312981 hsfs-3.2.0rc1/hsfs/engine/
+-rw-r--r--   0     1006     1006     2244 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/engine/__init__.py
+-rw-r--r--   0     1006     1006    46808 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/engine/python.py
+-rw-r--r--   0     1006     1006    42820 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/engine/spark.py
+-rw-r--r--   0     1006     1006    21585 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/expectation_suite.py
+-rw-r--r--   0     1006     1006     6857 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/feature.py
+-rw-r--r--   0     1006     1006   110708 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/feature_group.py
+-rw-r--r--   0     1006     1006     3424 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/feature_group_commit.py
+-rw-r--r--   0     1006     1006     1986 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/feature_group_writer.py
+-rw-r--r--   0     1006     1006    62935 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/feature_store.py
+-rw-r--r--   0     1006     1006    95713 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/feature_view.py
+-rw-r--r--   0     1006     1006     4822 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/ge_expectation.py
+-rw-r--r--   0     1006     1006     8633 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/ge_validation_result.py
+-rw-r--r--   0     1006     1006     1450 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/split_statistics.py
+-rw-r--r--   0     1006     1006     2893 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/statistics.py
+-rw-r--r--   0     1006     1006     3313 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/statistics_config.py
+-rw-r--r--   0     1006     1006    39092 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/storage_connector.py
+-rw-r--r--   0     1006     1006     1850 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/tag.py
+-rw-r--r--   0     1006     1006    35625 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/training_dataset.py
+-rw-r--r--   0     1006     1006     3542 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/training_dataset_feature.py
+-rw-r--r--   0     1006     1006     2759 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/training_dataset_split.py
+-rw-r--r--   0     1006     1006     8929 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/transformation_function.py
+-rw-r--r--   0     1006     1006     2179 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/transformation_function_attached.py
+-rw-r--r--   0     1006     1006     3491 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/user.py
+-rw-r--r--   0     1006     1006    11410 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/util.py
+-rw-r--r--   0     1006     1006     7519 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/validation_report.py
+-rw-r--r--   0     1006     1006      631 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/version.py
+drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.296981 hsfs-3.2.0rc1/hsfs.egg-info/
+-rw-r--r--   0     1006     1006     7714 2023-05-03 08:10:54.000000 hsfs-3.2.0rc1/hsfs.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     2805 2023-05-03 08:10:55.000000 hsfs-3.2.0rc1/hsfs.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2023-05-03 08:10:54.000000 hsfs-3.2.0rc1/hsfs.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      679 2023-05-03 08:10:54.000000 hsfs-3.2.0rc1/hsfs.egg-info/requires.txt
+-rw-r--r--   0     1006     1006        5 2023-05-03 08:10:54.000000 hsfs-3.2.0rc1/hsfs.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2023-05-03 08:10:55.312981 hsfs-3.2.0rc1/setup.cfg
+-rw-r--r--   0     1006     1006     2756 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/setup.py
```

### Comparing `hsfs-3.2.0rc0/PKG-INFO` & `hsfs-3.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.2.0rc0
+Version: 3.2.0rc1
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc0
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc1
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
@@ -160,14 +160,15 @@
 Keywords: Hopsworks,Feature Store,Spark,Machine Learning,MLOps,DataOps
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.7,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: hive
 Provides-Extra: python
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc0 Summary: HSFS: An
+Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc1 Summary: HSFS: An
 environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api Author: Hopsworks
 AB Author-email: moritz@logicalclocks.com License: Apache License 2.0 Download-
-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc0
+URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc1
 Description: # Hopsworks Feature Store
   [Hopsworks_Community] [Hopsworks_Feature_Store_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
@@ -60,11 +60,12 @@
 community.hopsworks.ai/). Please report any issue using [Github issue tracking]
 (https://github.com/logicalclocks/feature-store-api/issues). ## Contributing If
 you would like to contribute to this library, please see the [Contribution
 Guidelines](CONTRIBUTING.md). Keywords: Hopsworks,Feature Store,Spark,Machine
 Learning,MLOps,DataOps Platform: UNKNOWN Classifier: Development Status :: 5 -
 Production/Stable Classifier: Topic :: Utilities Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Intended
-Audience :: Developers Requires-Python: >=3.7,<3.10 Description-Content-Type:
-text/markdown Provides-Extra: dev Provides-Extra: docs Provides-Extra: hive
-Provides-Extra: python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Intended Audience ::
+Developers Requires-Python: >=3.7,<3.11 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: docs Provides-Extra: hive Provides-Extra:
+python
```

### Comparing `hsfs-3.2.0rc0/README.md` & `hsfs-3.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/__init__.py` & `hsfs-3.2.0rc1/hsfs/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/client/__init__.py` & `hsfs-3.2.0rc1/hsfs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/client/auth.py` & `hsfs-3.2.0rc1/hsfs/client/auth.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/client/base.py` & `hsfs-3.2.0rc1/hsfs/client/base.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/client/exceptions.py` & `hsfs-3.2.0rc1/hsfs/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/client/external.py` & `hsfs-3.2.0rc1/hsfs/client/external.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/client/hopsworks.py` & `hsfs-3.2.0rc1/hsfs/client/hopsworks.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/code.py` & `hsfs-3.2.0rc1/hsfs/code.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/connection.py` & `hsfs-3.2.0rc1/hsfs/connection.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/constructor/__init__.py` & `hsfs-3.2.0rc1/hsfs/constructor/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/constructor/external_feature_group_alias.py` & `hsfs-3.2.0rc1/hsfs/constructor/external_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/constructor/filter.py` & `hsfs-3.2.0rc1/hsfs/constructor/filter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/constructor/fs_query.py` & `hsfs-3.2.0rc1/hsfs/constructor/fs_query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/constructor/hudi_feature_group_alias.py` & `hsfs-3.2.0rc1/hsfs/constructor/hudi_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/constructor/join.py` & `hsfs-3.2.0rc1/hsfs/constructor/join.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/constructor/prepared_statement_parameter.py` & `hsfs-3.2.0rc1/hsfs/constructor/prepared_statement_parameter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/constructor/query.py` & `hsfs-3.2.0rc1/hsfs/constructor/query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/constructor/serving_prepared_statement.py` & `hsfs-3.2.0rc1/hsfs/constructor/serving_prepared_statement.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/__init__.py` & `hsfs-3.2.0rc1/hsfs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/builtin_transformation_function.py` & `hsfs-3.2.0rc1/hsfs/core/builtin_transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/code_api.py` & `hsfs-3.2.0rc1/hsfs/core/code_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/code_engine.py` & `hsfs-3.2.0rc1/hsfs/core/code_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/dataset_api.py` & `hsfs-3.2.0rc1/hsfs/core/dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/deltastreamer_jobconf.py` & `hsfs-3.2.0rc1/hsfs/core/deltastreamer_jobconf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/execution.py` & `hsfs-3.2.0rc1/hsfs/core/execution.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/expectation_api.py` & `hsfs-3.2.0rc1/hsfs/core/expectation_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/expectation_engine.py` & `hsfs-3.2.0rc1/hsfs/core/expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/expectation_suite_api.py` & `hsfs-3.2.0rc1/hsfs/core/expectation_suite_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/expectation_suite_engine.py` & `hsfs-3.2.0rc1/hsfs/core/expectation_suite_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/explicit_provenance.py` & `hsfs-3.2.0rc1/hsfs/core/explicit_provenance.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/external_feature_group_engine.py` & `hsfs-3.2.0rc1/hsfs/core/external_feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/feature_group_api.py` & `hsfs-3.2.0rc1/hsfs/core/feature_group_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/feature_group_base_engine.py` & `hsfs-3.2.0rc1/hsfs/core/feature_group_base_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/feature_group_engine.py` & `hsfs-3.2.0rc1/hsfs/core/feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/feature_store_api.py` & `hsfs-3.2.0rc1/hsfs/core/feature_store_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/feature_view_api.py` & `hsfs-3.2.0rc1/hsfs/core/feature_view_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/feature_view_engine.py` & `hsfs-3.2.0rc1/hsfs/core/feature_view_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/great_expectation_engine.py` & `hsfs-3.2.0rc1/hsfs/core/great_expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/hosts_api.py` & `hsfs-3.2.0rc1/hsfs/core/hosts_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/hudi_engine.py` & `hsfs-3.2.0rc1/hsfs/core/hudi_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/ingestion_job.py` & `hsfs-3.2.0rc1/hsfs/core/ingestion_job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/ingestion_job_conf.py` & `hsfs-3.2.0rc1/hsfs/core/ingestion_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/inode.py` & `hsfs-3.2.0rc1/hsfs/core/inode.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/job.py` & `hsfs-3.2.0rc1/hsfs/core/job.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,20 +35,24 @@
         items=None,
         count=None,
     ):
         self._id = id
         self._name = name
         self._executions = executions
         self._href = href
+        self._config = config
 
         self._job_api = job_api.JobApi()
 
     @classmethod
     def from_response_json(cls, json_dict):
+        # Job config should not be decamelized when updated
+        config = json_dict.pop("config")
         json_decamelized = humps.decamelize(json_dict)
+        json_decamelized["config"] = config
         return cls(**json_decamelized)
 
     @property
     def name(self):
         return self._name
 
     @property
@@ -59,15 +63,20 @@
     def executions(self):
         return self._executions
 
     @property
     def href(self):
         return self._href
 
-    def run(self, await_termination: bool = True):
+    @property
+    def config(self):
+        """Configuration for the job"""
+        return self._config
+
+    def run(self, args: str = None, await_termination: bool = True):
         """Run the job.
 
         Runs the job, by default awaiting its completion.
 
         !!! example
             ```python
             # connect to the Feature Store
@@ -80,17 +89,18 @@
             job, _ = fg.insert(df, write_options={"start_offline_backfill": False})
 
             # run job
             job.run()
             ```
 
         # Arguments
+            args: Optional runtime arguments for the job.
             await_termination: Identifies if the client should wait for the job to complete, defaults to True.
         """
         print(f"Launching job: {self.name}")
-        self._job_api.launch(self.name)
+        self._job_api.launch(self.name, args=args)
         print(
             "Job started successfully, you can follow the progress at \n{}".format(
                 engine.get_instance().get_job_url(self.href)
             )
         )
         engine.get_instance().wait_for_job(self, await_termination=await_termination)
```

### Comparing `hsfs-3.2.0rc0/hsfs/core/job_api.py` & `hsfs-3.2.0rc1/hsfs/core/job_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,19 @@
         headers = {"content-type": "application/json"}
         return job.Job.from_response_json(
             _client._send_request(
                 "PUT", path_params, headers=headers, data=job_conf.json()
             )
         )
 
-    def launch(self, name):
+    def launch(self, name, args: str = None):
         _client = client.get_instance()
         path_params = ["project", _client._project_id, "jobs", name, "executions"]
 
-        _client._send_request("POST", path_params)
+        _client._send_request("POST", path_params, data=args)
 
     def get(self, name: str):
         _client = client.get_instance()
         path_params = ["project", _client._project_id, "jobs", name]
 
         return job.Job.from_response_json(_client._send_request("GET", path_params))
```

### Comparing `hsfs-3.2.0rc0/hsfs/core/job_configuration.py` & `hsfs-3.2.0rc1/hsfs/core/job_configuration.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/kafka_api.py` & `hsfs-3.2.0rc1/hsfs/core/kafka_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/project_api.py` & `hsfs-3.2.0rc1/hsfs/core/project_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/query_constructor_api.py` & `hsfs-3.2.0rc1/hsfs/core/query_constructor_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/services_api.py` & `hsfs-3.2.0rc1/hsfs/core/services_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/statistics_api.py` & `hsfs-3.2.0rc1/hsfs/core/statistics_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/statistics_engine.py` & `hsfs-3.2.0rc1/hsfs/core/statistics_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/storage_connector_api.py` & `hsfs-3.2.0rc1/hsfs/core/storage_connector_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/tags_api.py` & `hsfs-3.2.0rc1/hsfs/core/tags_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/training_dataset_api.py` & `hsfs-3.2.0rc1/hsfs/core/training_dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/training_dataset_engine.py` & `hsfs-3.2.0rc1/hsfs/core/training_dataset_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/training_dataset_job_conf.py` & `hsfs-3.2.0rc1/hsfs/core/training_dataset_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/transformation_function_api.py` & `hsfs-3.2.0rc1/hsfs/core/transformation_function_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/transformation_function_engine.py` & `hsfs-3.2.0rc1/hsfs/core/transformation_function_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/validation_report_api.py` & `hsfs-3.2.0rc1/hsfs/core/validation_report_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/validation_report_engine.py` & `hsfs-3.2.0rc1/hsfs/core/validation_report_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/validation_result_api.py` & `hsfs-3.2.0rc1/hsfs/core/validation_result_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/validation_result_engine.py` & `hsfs-3.2.0rc1/hsfs/core/validation_result_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/variable_api.py` & `hsfs-3.2.0rc1/hsfs/core/variable_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/core/vector_server.py` & `hsfs-3.2.0rc1/hsfs/core/vector_server.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/decorators.py` & `hsfs-3.2.0rc1/hsfs/decorators.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/engine/__init__.py` & `hsfs-3.2.0rc1/hsfs/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/engine/python.py` & `hsfs-3.2.0rc1/hsfs/engine/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -816,14 +816,15 @@
 
     def _write_dataframe_kafka(
         self,
         feature_group: FeatureGroup,
         dataframe: pd.DataFrame,
         offline_write_options: dict,
     ):
+        reset_offsets = False
         if feature_group._multi_part_insert:
             if feature_group._kafka_producer is None:
                 producer, feature_writers, writer = self._init_kafka_resources(
                     feature_group, offline_write_options
                 )
                 feature_group._kafka_producer = producer
                 feature_group._feature_writers = feature_writers
@@ -842,14 +843,20 @@
                 total=dataframe.shape[0],
                 bar_format="{desc}: {percentage:.2f}% |{bar}| Rows {n_fmt}/{total_fmt} | "
                 "Elapsed Time: {elapsed} | Remaining Time: {remaining}",
                 desc="Uploading Dataframe",
                 mininterval=1,
             )
 
+            reset_offsets = (
+                feature_group._online_topic_name
+                not in producer.list_topics(timeout=1).topics.keys()
+                and len(feature_group.commit_details(limit=1)) == 1
+            )
+
         def acked(err, msg):
             if err is not None:
                 if offline_write_options.get("debug_kafka", False):
                     print("Failed to deliver message: %s: %s" % (str(msg), str(err)))
                 if err.code() in [
                     KafkaError.TOPIC_AUTHORIZATION_FAILED,
                     KafkaError._MSG_TIMED_OUT,
@@ -896,16 +903,34 @@
 
         # make sure producer blocks and everything is delivered
         if not feature_group._multi_part_insert:
             producer.flush()
             progress_bar.close()
 
         # start backfilling job
+        # if topic didn't exist, always run the backfill job to reset the offsets except if it's a multi insert
         if (
             not isinstance(feature_group, ExternalFeatureGroup)
+            and reset_offsets
+            and not feature_group._multi_part_insert
+        ):
+            if offline_write_options is not None and not offline_write_options.get(
+                "start_offline_backfill", True
+            ):
+                warnings.warn(
+                    "This is the first ingestion after an upgrade or backup/restore, running backfill job even though `start_offline_backfill` was set to `False`.",
+                    util.FeatureGroupWarning,
+                )
+            feature_group.backfill_job.run(
+                args=feature_group.backfill_job.config.get("defaultArgs", "")
+                + " -kafkaOffsetReset true",
+                await_termination=offline_write_options.get("wait_for_job", True),
+            )
+        elif (
+            not isinstance(feature_group, ExternalFeatureGroup)
             and offline_write_options is not None
             and offline_write_options.get("start_offline_backfill", True)
         ):
             feature_group.backfill_job.run(
                 await_termination=offline_write_options.get("wait_for_job", True)
             )
         if isinstance(feature_group, ExternalFeatureGroup):
```

### Comparing `hsfs-3.2.0rc0/hsfs/engine/spark.py` & `hsfs-3.2.0rc1/hsfs/engine/spark.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/expectation_suite.py` & `hsfs-3.2.0rc1/hsfs/expectation_suite.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/feature.py` & `hsfs-3.2.0rc1/hsfs/feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/feature_group.py` & `hsfs-3.2.0rc1/hsfs/feature_group.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/feature_group_commit.py` & `hsfs-3.2.0rc1/hsfs/feature_group_commit.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/feature_group_writer.py` & `hsfs-3.2.0rc1/hsfs/feature_group_writer.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/feature_store.py` & `hsfs-3.2.0rc1/hsfs/feature_store.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/feature_view.py` & `hsfs-3.2.0rc1/hsfs/feature_view.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/ge_expectation.py` & `hsfs-3.2.0rc1/hsfs/ge_expectation.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/ge_validation_result.py` & `hsfs-3.2.0rc1/hsfs/ge_validation_result.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/split_statistics.py` & `hsfs-3.2.0rc1/hsfs/split_statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/statistics.py` & `hsfs-3.2.0rc1/hsfs/statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/statistics_config.py` & `hsfs-3.2.0rc1/hsfs/statistics_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/storage_connector.py` & `hsfs-3.2.0rc1/hsfs/storage_connector.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/tag.py` & `hsfs-3.2.0rc1/hsfs/tag.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/training_dataset.py` & `hsfs-3.2.0rc1/hsfs/training_dataset.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/training_dataset_feature.py` & `hsfs-3.2.0rc1/hsfs/training_dataset_feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/training_dataset_split.py` & `hsfs-3.2.0rc1/hsfs/training_dataset_split.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/transformation_function.py` & `hsfs-3.2.0rc1/hsfs/transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/transformation_function_attached.py` & `hsfs-3.2.0rc1/hsfs/transformation_function_attached.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/user.py` & `hsfs-3.2.0rc1/hsfs/user.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/util.py` & `hsfs-3.2.0rc1/hsfs/util.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/validation_report.py` & `hsfs-3.2.0rc1/hsfs/validation_report.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs/version.py` & `hsfs-3.2.0rc1/hsfs/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.2.0rc0"
+__version__ = "3.2.0rc1"
```

### Comparing `hsfs-3.2.0rc0/hsfs.egg-info/PKG-INFO` & `hsfs-3.2.0rc1/hsfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.2.0rc0
+Version: 3.2.0rc1
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc0
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc1
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
@@ -160,14 +160,15 @@
 Keywords: Hopsworks,Feature Store,Spark,Machine Learning,MLOps,DataOps
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.7,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: hive
 Provides-Extra: python
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc0 Summary: HSFS: An
+Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc1 Summary: HSFS: An
 environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api Author: Hopsworks
 AB Author-email: moritz@logicalclocks.com License: Apache License 2.0 Download-
-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc0
+URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc1
 Description: # Hopsworks Feature Store
   [Hopsworks_Community] [Hopsworks_Feature_Store_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
@@ -60,11 +60,12 @@
 community.hopsworks.ai/). Please report any issue using [Github issue tracking]
 (https://github.com/logicalclocks/feature-store-api/issues). ## Contributing If
 you would like to contribute to this library, please see the [Contribution
 Guidelines](CONTRIBUTING.md). Keywords: Hopsworks,Feature Store,Spark,Machine
 Learning,MLOps,DataOps Platform: UNKNOWN Classifier: Development Status :: 5 -
 Production/Stable Classifier: Topic :: Utilities Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Intended
-Audience :: Developers Requires-Python: >=3.7,<3.10 Description-Content-Type:
-text/markdown Provides-Extra: dev Provides-Extra: docs Provides-Extra: hive
-Provides-Extra: python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Intended Audience ::
+Developers Requires-Python: >=3.7,<3.11 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: docs Provides-Extra: hive Provides-Extra:
+python
```

### Comparing `hsfs-3.2.0rc0/hsfs.egg-info/SOURCES.txt` & `hsfs-3.2.0rc1/hsfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc0/hsfs.egg-info/requires.txt` & `hsfs-3.2.0rc1/hsfs.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 mkdocs-macros-plugin==0.7.0
 mkdocs-material==8.2.8
 mkdocs==1.3.0
 pymdown-extensions
 sphinx==3.5.4
 
 [hive]
-confluent-kafka==1.8.2
+confluent-kafka<=1.9.0
 fastavro<=1.7.3,>=1.4.11
 pyarrow
 pyhopshive[thrift]
 
 [python]
-confluent-kafka==1.8.2
+confluent-kafka<=1.9.0
 fastavro<=1.7.3,>=1.4.11
 pyarrow
 pyhopshive[thrift]
 tqdm
```

### Comparing `hsfs-3.2.0rc0/setup.py` & `hsfs-3.2.0rc1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="hsfs",
     version=__version__,
-    python_requires=">=3.7,<3.10",
+    python_requires=">=3.7,<3.11",
     install_requires=[
         "pyhumps==1.6.1",
         "requests",
         "furl",
         "boto3",
         "pandas>=1.2.0,<2.0.0",
         "numpy",
@@ -52,21 +52,21 @@
             "markdown==3.3.7",
             "pymdown-extensions",
             "mkdocs-macros-plugin==0.7.0",
         ],
         "hive": [
             "pyhopshive[thrift]",
             "pyarrow",
-            "confluent-kafka==1.8.2",
+            "confluent-kafka<=1.9.0",
             "fastavro>=1.4.11,<=1.7.3",
         ],
         "python": [
             "pyhopshive[thrift]",
             "pyarrow",
-            "confluent-kafka==1.8.2",
+            "confluent-kafka<=1.9.0",
             "fastavro>=1.4.11,<=1.7.3",
             "tqdm",
         ],
     },
     author="Hopsworks AB",
     author_email="moritz@logicalclocks.com",
     description="HSFS: An environment independent client to interact with the Hopsworks Featurestore",
@@ -80,10 +80,11 @@
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Intended Audience :: Developers",
     ],
 )
```

