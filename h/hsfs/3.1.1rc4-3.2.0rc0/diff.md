# Comparing `tmp/hsfs-3.1.1rc4.tar.gz` & `tmp/hsfs-3.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsfs-3.1.1rc4.tar", last modified: Mon Mar 27 15:48:09 2023, max compression
+gzip compressed data, was "hsfs-3.2.0rc0.tar", last modified: Wed Apr 12 12:41:00 2023, max compression
```

## Comparing `hsfs-3.1.1rc4.tar` & `hsfs-3.2.0rc0.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0     1006     1006        0 2023-03-27 15:48:09.260014 hsfs-3.1.1rc4/
--rw-r--r--   0     1006     1006       40 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/MANIFEST.in
--rw-r--r--   0     1006     1006     7663 2023-03-27 15:48:09.260014 hsfs-3.1.1rc4/PKG-INFO
--rw-r--r--   0     1006     1006     5539 2023-03-27 15:48:08.000000 hsfs-3.1.1rc4/README.md
-drwxr-xr-x   0     1006     1006        0 2023-03-27 15:48:09.236014 hsfs-3.1.1rc4/hsfs/
--rw-r--r--   0     1006     1006     1182 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-03-27 15:48:09.240014 hsfs-3.1.1rc4/hsfs/client/
--rw-r--r--   0     1006     1006     1694 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/client/__init__.py
--rw-r--r--   0     1006     1006     1132 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/client/auth.py
--rw-r--r--   0     1006     1006     6622 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/client/base.py
--rw-r--r--   0     1006     1006     2090 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/client/exceptions.py
--rw-r--r--   0     1006     1006    11621 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/client/external.py
--rw-r--r--   0     1006     1006     7924 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/client/hopsworks.py
--rw-r--r--   0     1006     1006     1536 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/code.py
--rw-r--r--   0     1006     1006    18899 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/connection.py
-drwxr-xr-x   0     1006     1006        0 2023-03-27 15:48:09.244014 hsfs-3.1.1rc4/hsfs/constructor/
--rw-r--r--   0     1006     1006      605 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/constructor/__init__.py
--rw-r--r--   0     1006     1006     1261 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/constructor/external_feature_group_alias.py
--rw-r--r--   0     1006     1006     5106 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/constructor/filter.py
--rw-r--r--   0     1006     1006     2981 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/constructor/fs_query.py
--rw-r--r--   0     1006     1006     1731 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/constructor/hudi_feature_group_alias.py
--rw-r--r--   0     1006     1006     2157 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/constructor/join.py
--rw-r--r--   0     1006     1006     1577 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/constructor/prepared_statement_parameter.py
--rw-r--r--   0     1006     1006    20138 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/constructor/query.py
--rw-r--r--   0     1006     1006     3331 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/constructor/serving_prepared_statement.py
-drwxr-xr-x   0     1006     1006        0 2023-03-27 15:48:09.256014 hsfs-3.1.1rc4/hsfs/core/
--rw-r--r--   0     1006     1006      605 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/__init__.py
--rw-r--r--   0     1006     1006     3688 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/builtin_transformation_function.py
--rw-r--r--   0     1006     1006     1853 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/code_api.py
--rw-r--r--   0     1006     1006     3292 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/code_engine.py
--rw-r--r--   0     1006     1006     3509 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/dataset_api.py
--rw-r--r--   0     1006     1006     1030 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/deltastreamer_jobconf.py
--rw-r--r--   0     1006     1006     1609 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/execution.py
--rw-r--r--   0     1006     1006     5396 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/expectation_api.py
--rw-r--r--   0     1006     1006     2632 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/expectation_engine.py
--rw-r--r--   0     1006     1006     6356 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/expectation_suite_api.py
--rw-r--r--   0     1006     1006     4002 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/expectation_suite_engine.py
--rw-r--r--   0     1006     1006     9792 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/explicit_provenance.py
--rw-r--r--   0     1006     1006     3576 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/external_feature_group_engine.py
--rw-r--r--   0     1006     1006    13334 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/feature_group_api.py
--rw-r--r--   0     1006     1006     4607 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/feature_group_base_engine.py
--rw-r--r--   0     1006     1006    16146 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/feature_group_engine.py
--rw-r--r--   0     1006     1006     1238 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/feature_store_api.py
--rw-r--r--   0     1006     1006     9739 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/feature_view_api.py
--rw-r--r--   0     1006     1006    24618 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/feature_view_engine.py
--rw-r--r--   0     1006     1006     4899 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/great_expectation_engine.py
--rw-r--r--   0     1006     1006      828 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/hosts_api.py
--rw-r--r--   0     1006     1006    11546 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/hudi_engine.py
--rw-r--r--   0     1006     1006     1211 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/ingestion_job.py
--rw-r--r--   0     1006     1006     2262 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/ingestion_job_conf.py
--rw-r--r--   0     1006     1006     1077 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/inode.py
--rw-r--r--   0     1006     1006     2539 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/job.py
--rw-r--r--   0     1006     1006     1975 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/job_api.py
--rw-r--r--   0     1006     1006     2048 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/job_configuration.py
--rw-r--r--   0     1006     1006     1530 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/kafka_api.py
--rw-r--r--   0     1006     1006      898 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/project_api.py
--rw-r--r--   0     1006     1006     1093 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/query_constructor_api.py
--rw-r--r--   0     1006     1006      875 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/services_api.py
--rw-r--r--   0     1006     1006     4204 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/statistics_api.py
--rw-r--r--   0     1006     1006     8159 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/statistics_engine.py
--rw-r--r--   0     1006     1006     2325 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/storage_connector_api.py
--rw-r--r--   0     1006     1006     4696 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/tags_api.py
--rw-r--r--   0     1006     1006     6685 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/training_dataset_api.py
--rw-r--r--   0     1006     1006     6357 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/training_dataset_engine.py
--rw-r--r--   0     1006     1006     2148 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/training_dataset_job_conf.py
--rw-r--r--   0     1006     1006     4161 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/transformation_function_api.py
--rw-r--r--   0     1006     1006    14792 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/transformation_function_engine.py
--rw-r--r--   0     1006     1006     4773 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/validation_report_api.py
--rw-r--r--   0     1006     1006     3640 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/validation_report_engine.py
--rw-r--r--   0     1006     1006     2158 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/validation_result_api.py
--rw-r--r--   0     1006     1006     5469 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/validation_result_engine.py
--rw-r--r--   0     1006     1006     1261 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/variable_api.py
--rw-r--r--   0     1006     1006    18428 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/core/vector_server.py
--rw-r--r--   0     1006     1006     1655 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/decorators.py
-drwxr-xr-x   0     1006     1006        0 2023-03-27 15:48:09.260014 hsfs-3.1.1rc4/hsfs/engine/
--rw-r--r--   0     1006     1006     2244 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/engine/__init__.py
--rw-r--r--   0     1006     1006    44262 2023-03-23 12:58:41.000000 hsfs-3.1.1rc4/hsfs/engine/python.py
--rw-r--r--   0     1006     1006    41444 2023-03-27 15:48:04.000000 hsfs-3.1.1rc4/hsfs/engine/spark.py
--rw-r--r--   0     1006     1006    21585 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/expectation_suite.py
--rw-r--r--   0     1006     1006     6857 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/feature.py
--rw-r--r--   0     1006     1006    98721 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/feature_group.py
--rw-r--r--   0     1006     1006     3424 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/feature_group_commit.py
--rw-r--r--   0     1006     1006    61106 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/feature_store.py
--rw-r--r--   0     1006     1006    94803 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/feature_view.py
--rw-r--r--   0     1006     1006     4822 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/ge_expectation.py
--rw-r--r--   0     1006     1006     8633 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/ge_validation_result.py
--rw-r--r--   0     1006     1006     1450 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/split_statistics.py
--rw-r--r--   0     1006     1006     2893 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/statistics.py
--rw-r--r--   0     1006     1006     3313 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/statistics_config.py
--rw-r--r--   0     1006     1006    39092 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/storage_connector.py
--rw-r--r--   0     1006     1006     1850 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/tag.py
--rw-r--r--   0     1006     1006    35625 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/training_dataset.py
--rw-r--r--   0     1006     1006     3542 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/training_dataset_feature.py
--rw-r--r--   0     1006     1006     2759 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/training_dataset_split.py
--rw-r--r--   0     1006     1006     8929 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/transformation_function.py
--rw-r--r--   0     1006     1006     2179 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/transformation_function_attached.py
--rw-r--r--   0     1006     1006     3491 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/user.py
--rw-r--r--   0     1006     1006    11141 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/util.py
--rw-r--r--   0     1006     1006     7519 2023-03-13 10:42:53.000000 hsfs-3.1.1rc4/hsfs/validation_report.py
--rw-r--r--   0     1006     1006      631 2023-03-27 15:48:04.000000 hsfs-3.1.1rc4/hsfs/version.py
-drwxr-xr-x   0     1006     1006        0 2023-03-27 15:48:09.236014 hsfs-3.1.1rc4/hsfs.egg-info/
--rw-r--r--   0     1006     1006     7663 2023-03-27 15:48:09.000000 hsfs-3.1.1rc4/hsfs.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     2776 2023-03-27 15:48:09.000000 hsfs-3.1.1rc4/hsfs.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2023-03-27 15:48:09.000000 hsfs-3.1.1rc4/hsfs.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      679 2023-03-27 15:48:09.000000 hsfs-3.1.1rc4/hsfs.egg-info/requires.txt
--rw-r--r--   0     1006     1006        5 2023-03-27 15:48:09.000000 hsfs-3.1.1rc4/hsfs.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2023-03-27 15:48:09.260014 hsfs-3.1.1rc4/setup.cfg
--rw-r--r--   0     1006     1006     2706 2023-03-22 14:06:38.000000 hsfs-3.1.1rc4/setup.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.155222 hsfs-3.2.0rc0/
+-rw-r--r--   0     1006     1006       40 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/MANIFEST.in
+-rw-r--r--   0     1006     1006     7663 2023-04-12 12:41:00.155222 hsfs-3.2.0rc0/PKG-INFO
+-rw-r--r--   0     1006     1006     5539 2023-04-12 12:40:58.000000 hsfs-3.2.0rc0/README.md
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.135222 hsfs-3.2.0rc0/hsfs/
+-rw-r--r--   0     1006     1006     1182 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.139222 hsfs-3.2.0rc0/hsfs/client/
+-rw-r--r--   0     1006     1006     1694 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/client/__init__.py
+-rw-r--r--   0     1006     1006     1132 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/client/auth.py
+-rw-r--r--   0     1006     1006     6622 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/client/base.py
+-rw-r--r--   0     1006     1006     2090 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/client/exceptions.py
+-rw-r--r--   0     1006     1006    11621 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/client/external.py
+-rw-r--r--   0     1006     1006     7924 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/client/hopsworks.py
+-rw-r--r--   0     1006     1006     1536 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/code.py
+-rw-r--r--   0     1006     1006    18899 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/connection.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.143222 hsfs-3.2.0rc0/hsfs/constructor/
+-rw-r--r--   0     1006     1006      605 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/__init__.py
+-rw-r--r--   0     1006     1006     1261 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/external_feature_group_alias.py
+-rw-r--r--   0     1006     1006     5106 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/filter.py
+-rw-r--r--   0     1006     1006     2981 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/fs_query.py
+-rw-r--r--   0     1006     1006     1731 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/hudi_feature_group_alias.py
+-rw-r--r--   0     1006     1006     2157 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/join.py
+-rw-r--r--   0     1006     1006     1577 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/prepared_statement_parameter.py
+-rw-r--r--   0     1006     1006    20138 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/query.py
+-rw-r--r--   0     1006     1006     3331 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/constructor/serving_prepared_statement.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.155222 hsfs-3.2.0rc0/hsfs/core/
+-rw-r--r--   0     1006     1006      605 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/__init__.py
+-rw-r--r--   0     1006     1006     3688 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/builtin_transformation_function.py
+-rw-r--r--   0     1006     1006     1853 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/code_api.py
+-rw-r--r--   0     1006     1006     3292 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/code_engine.py
+-rw-r--r--   0     1006     1006     3509 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/dataset_api.py
+-rw-r--r--   0     1006     1006     1030 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/deltastreamer_jobconf.py
+-rw-r--r--   0     1006     1006     1609 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/execution.py
+-rw-r--r--   0     1006     1006     5396 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/expectation_api.py
+-rw-r--r--   0     1006     1006     2632 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/expectation_engine.py
+-rw-r--r--   0     1006     1006     6356 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/expectation_suite_api.py
+-rw-r--r--   0     1006     1006     4002 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/expectation_suite_engine.py
+-rw-r--r--   0     1006     1006     9792 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/explicit_provenance.py
+-rw-r--r--   0     1006     1006     5418 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/core/external_feature_group_engine.py
+-rw-r--r--   0     1006     1006    13334 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/feature_group_api.py
+-rw-r--r--   0     1006     1006     6610 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/core/feature_group_base_engine.py
+-rw-r--r--   0     1006     1006    13164 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/core/feature_group_engine.py
+-rw-r--r--   0     1006     1006     1238 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/feature_store_api.py
+-rw-r--r--   0     1006     1006     9739 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/feature_view_api.py
+-rw-r--r--   0     1006     1006    24896 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/core/feature_view_engine.py
+-rw-r--r--   0     1006     1006     5024 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/core/great_expectation_engine.py
+-rw-r--r--   0     1006     1006      828 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/hosts_api.py
+-rw-r--r--   0     1006     1006    11546 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/hudi_engine.py
+-rw-r--r--   0     1006     1006     1211 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/ingestion_job.py
+-rw-r--r--   0     1006     1006     2262 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/ingestion_job_conf.py
+-rw-r--r--   0     1006     1006     1077 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/inode.py
+-rw-r--r--   0     1006     1006     2539 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/job.py
+-rw-r--r--   0     1006     1006     1975 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/job_api.py
+-rw-r--r--   0     1006     1006     2048 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/job_configuration.py
+-rw-r--r--   0     1006     1006     1530 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/kafka_api.py
+-rw-r--r--   0     1006     1006      898 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/project_api.py
+-rw-r--r--   0     1006     1006     1093 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/query_constructor_api.py
+-rw-r--r--   0     1006     1006      875 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/services_api.py
+-rw-r--r--   0     1006     1006     4204 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/statistics_api.py
+-rw-r--r--   0     1006     1006     8159 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/statistics_engine.py
+-rw-r--r--   0     1006     1006     2325 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/storage_connector_api.py
+-rw-r--r--   0     1006     1006     4696 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/tags_api.py
+-rw-r--r--   0     1006     1006     6685 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/training_dataset_api.py
+-rw-r--r--   0     1006     1006     6357 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/training_dataset_engine.py
+-rw-r--r--   0     1006     1006     2148 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/training_dataset_job_conf.py
+-rw-r--r--   0     1006     1006     4161 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/transformation_function_api.py
+-rw-r--r--   0     1006     1006    14792 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/transformation_function_engine.py
+-rw-r--r--   0     1006     1006     4773 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/validation_report_api.py
+-rw-r--r--   0     1006     1006     3640 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/validation_report_engine.py
+-rw-r--r--   0     1006     1006     2158 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/validation_result_api.py
+-rw-r--r--   0     1006     1006     5469 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/validation_result_engine.py
+-rw-r--r--   0     1006     1006     1261 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/core/variable_api.py
+-rw-r--r--   0     1006     1006    18519 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/core/vector_server.py
+-rw-r--r--   0     1006     1006     1655 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/decorators.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.155222 hsfs-3.2.0rc0/hsfs/engine/
+-rw-r--r--   0     1006     1006     2244 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/engine/__init__.py
+-rw-r--r--   0     1006     1006    45592 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/engine/python.py
+-rw-r--r--   0     1006     1006    42820 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/engine/spark.py
+-rw-r--r--   0     1006     1006    21585 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/expectation_suite.py
+-rw-r--r--   0     1006     1006     6857 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/feature.py
+-rw-r--r--   0     1006     1006   110708 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/feature_group.py
+-rw-r--r--   0     1006     1006     3424 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/feature_group_commit.py
+-rw-r--r--   0     1006     1006     1986 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/feature_group_writer.py
+-rw-r--r--   0     1006     1006    62935 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/feature_store.py
+-rw-r--r--   0     1006     1006    95713 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/feature_view.py
+-rw-r--r--   0     1006     1006     4822 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/ge_expectation.py
+-rw-r--r--   0     1006     1006     8633 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/ge_validation_result.py
+-rw-r--r--   0     1006     1006     1450 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/split_statistics.py
+-rw-r--r--   0     1006     1006     2893 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/statistics.py
+-rw-r--r--   0     1006     1006     3313 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/statistics_config.py
+-rw-r--r--   0     1006     1006    39092 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/storage_connector.py
+-rw-r--r--   0     1006     1006     1850 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/tag.py
+-rw-r--r--   0     1006     1006    35625 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/training_dataset.py
+-rw-r--r--   0     1006     1006     3542 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/training_dataset_feature.py
+-rw-r--r--   0     1006     1006     2759 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/training_dataset_split.py
+-rw-r--r--   0     1006     1006     8929 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/transformation_function.py
+-rw-r--r--   0     1006     1006     2179 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/transformation_function_attached.py
+-rw-r--r--   0     1006     1006     3491 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/user.py
+-rw-r--r--   0     1006     1006    11410 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/util.py
+-rw-r--r--   0     1006     1006     7519 2023-03-13 10:42:53.000000 hsfs-3.2.0rc0/hsfs/validation_report.py
+-rw-r--r--   0     1006     1006      631 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/hsfs/version.py
+drwxr-xr-x   0     1006     1006        0 2023-04-12 12:41:00.139222 hsfs-3.2.0rc0/hsfs.egg-info/
+-rw-r--r--   0     1006     1006     7663 2023-04-12 12:40:59.000000 hsfs-3.2.0rc0/hsfs.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     2805 2023-04-12 12:41:00.000000 hsfs-3.2.0rc0/hsfs.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2023-04-12 12:40:59.000000 hsfs-3.2.0rc0/hsfs.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      679 2023-04-12 12:40:59.000000 hsfs-3.2.0rc0/hsfs.egg-info/requires.txt
+-rw-r--r--   0     1006     1006        5 2023-04-12 12:40:59.000000 hsfs-3.2.0rc0/hsfs.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2023-04-12 12:41:00.155222 hsfs-3.2.0rc0/setup.cfg
+-rw-r--r--   0     1006     1006     2706 2023-04-12 12:40:55.000000 hsfs-3.2.0rc0/setup.py
```

### Comparing `hsfs-3.1.1rc4/PKG-INFO` & `hsfs-3.2.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.1.1rc4
+Version: 3.2.0rc0
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.1.1rc4
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc0
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.1.1rc4 Summary: HSFS: An
+Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc0 Summary: HSFS: An
 environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api Author: Hopsworks
 AB Author-email: moritz@logicalclocks.com License: Apache License 2.0 Download-
-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.1.1rc4
+URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc0
 Description: # Hopsworks Feature Store
   [Hopsworks_Community] [Hopsworks_Feature_Store_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.1.1rc4/README.md` & `hsfs-3.2.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/__init__.py` & `hsfs-3.2.0rc0/hsfs/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/client/__init__.py` & `hsfs-3.2.0rc0/hsfs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/client/auth.py` & `hsfs-3.2.0rc0/hsfs/client/auth.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/client/base.py` & `hsfs-3.2.0rc0/hsfs/client/base.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/client/exceptions.py` & `hsfs-3.2.0rc0/hsfs/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/client/external.py` & `hsfs-3.2.0rc0/hsfs/client/external.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/client/hopsworks.py` & `hsfs-3.2.0rc0/hsfs/client/hopsworks.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/code.py` & `hsfs-3.2.0rc0/hsfs/code.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/connection.py` & `hsfs-3.2.0rc0/hsfs/connection.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/constructor/__init__.py` & `hsfs-3.2.0rc0/hsfs/constructor/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/constructor/external_feature_group_alias.py` & `hsfs-3.2.0rc0/hsfs/constructor/external_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/constructor/filter.py` & `hsfs-3.2.0rc0/hsfs/constructor/filter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/constructor/fs_query.py` & `hsfs-3.2.0rc0/hsfs/constructor/fs_query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/constructor/hudi_feature_group_alias.py` & `hsfs-3.2.0rc0/hsfs/constructor/hudi_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/constructor/join.py` & `hsfs-3.2.0rc0/hsfs/constructor/join.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/constructor/prepared_statement_parameter.py` & `hsfs-3.2.0rc0/hsfs/constructor/prepared_statement_parameter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/constructor/query.py` & `hsfs-3.2.0rc0/hsfs/constructor/query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/constructor/serving_prepared_statement.py` & `hsfs-3.2.0rc0/hsfs/constructor/serving_prepared_statement.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/__init__.py` & `hsfs-3.2.0rc0/hsfs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/builtin_transformation_function.py` & `hsfs-3.2.0rc0/hsfs/core/builtin_transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/code_api.py` & `hsfs-3.2.0rc0/hsfs/core/code_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/code_engine.py` & `hsfs-3.2.0rc0/hsfs/core/code_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/dataset_api.py` & `hsfs-3.2.0rc0/hsfs/core/dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/deltastreamer_jobconf.py` & `hsfs-3.2.0rc0/hsfs/core/deltastreamer_jobconf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/execution.py` & `hsfs-3.2.0rc0/hsfs/core/execution.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/expectation_api.py` & `hsfs-3.2.0rc0/hsfs/core/expectation_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/expectation_engine.py` & `hsfs-3.2.0rc0/hsfs/core/expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/expectation_suite_api.py` & `hsfs-3.2.0rc0/hsfs/core/expectation_suite_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/expectation_suite_engine.py` & `hsfs-3.2.0rc0/hsfs/core/expectation_suite_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/explicit_provenance.py` & `hsfs-3.2.0rc0/hsfs/core/explicit_provenance.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/external_feature_group_engine.py` & `hsfs-3.2.0rc0/hsfs/core/external_feature_group_engine.py`

 * *Files 26% similar despite different names*

```diff
@@ -43,14 +43,62 @@
         util.verify_attribute_key_names(feature_group, True)
         for feat in feature_group.features:
             if feat.name in feature_group.primary_key:
                 feat.primary = True
 
         self._feature_group_api.save(feature_group)
 
+    def insert(
+        self,
+        feature_group,
+        feature_dataframe,
+        write_options: dict,
+        validation_options: dict = {},
+    ):
+        if not feature_group.online_enabled:
+            raise FeatureStoreException(
+                "Online storage is not enabled for this feature group. External feature groups can only store data in"
+                + " online storage. To create an offline only external feature group, use the `save` method."
+            )
+
+        schema = engine.get_instance().parse_schema_feature_group(feature_dataframe)
+
+        if not feature_group._id:
+            # only save metadata if feature group does not exist
+            feature_group.features = schema
+            self.save(feature_group)
+        else:
+            # else, just verify that feature group schema matches user-provided dataframe
+            self._verify_schema_compatibility(feature_group.features, schema)
+
+        # ge validation on python and non stream feature groups on spark
+        ge_report = feature_group._great_expectation_engine.validate(
+            feature_group=feature_group,
+            dataframe=feature_dataframe,
+            validation_options=validation_options,
+            ingestion_result="INGESTED",
+            ge_type=False,
+        )
+
+        if ge_report is not None and ge_report.ingestion_result == "REJECTED":
+            return None, ge_report
+
+        return (
+            engine.get_instance().save_dataframe(
+                feature_group=feature_group,
+                dataframe=feature_dataframe,
+                operation=None,
+                online_enabled=feature_group.online_enabled,
+                storage="online",
+                offline_write_options=write_options,
+                online_write_options=write_options,
+            ),
+            ge_report,
+        )
+
     def _update_features_metadata(self, feature_group, features):
         # perform changes on copy in case the update fails, so we don't leave
         # the user object in corrupted state
         copy_feature_group = fg.ExternalFeatureGroup(
             storage_connector=feature_group.storage_connector,
             id=feature_group.id,
             features=features,
```

### Comparing `hsfs-3.1.1rc4/hsfs/core/feature_group_api.py` & `hsfs-3.2.0rc0/hsfs/core/feature_group_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/feature_group_engine.py` & `hsfs-3.2.0rc0/hsfs/core/feature_group_engine.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 #   limitations under the License.
 #
 import warnings
 
 from hsfs import engine, client, util
 from hsfs import feature_group as fg
 from hsfs.client import exceptions
-from hsfs.client.exceptions import FeatureStoreException
 from hsfs.core import feature_group_base_engine, hudi_engine
 from hsfs.core.deltastreamer_jobconf import DeltaStreamerJobConf
 
 
 class FeatureGroupEngine(feature_group_base_engine.FeatureGroupBaseEngine):
     def __init__(self, feature_store_id):
         super().__init__(feature_store_id)
@@ -53,15 +52,15 @@
             ingestion_result="INGESTED",
         )
 
         if ge_report is not None and ge_report.ingestion_result == "REJECTED":
             return None, ge_report
 
         offline_write_options = write_options
-        online_write_options = self.get_kafka_config(write_options)
+        online_write_options = write_options
 
         return (
             engine.get_instance().save_dataframe(
                 feature_group,
                 feature_dataframe,
                 hudi_engine.HudiEngine.HUDI_BULK_INSERT
                 if feature_group.time_travel_format == "HUDI"
@@ -109,15 +108,15 @@
             ge_type=False,
         )
 
         if ge_report is not None and ge_report.ingestion_result == "REJECTED":
             return None, ge_report
 
         offline_write_options = write_options
-        online_write_options = self.get_kafka_config(write_options)
+        online_write_options = write_options
 
         if not feature_group.online_enabled and storage == "online":
             raise exceptions.FeatureStoreException(
                 "Online storage is not enabled for this feature group."
             )
 
         if overwrite:
@@ -230,35 +229,14 @@
             stream=feature_group.stream,
             features=feature_group.features,
         )
         self._feature_group_api.update_metadata(
             feature_group, copy_feature_group, "updateMetadata"
         )
 
-    def get_subject(self, feature_group):
-        return self._kafka_api.get_topic_subject(feature_group._online_topic_name)
-
-    def get_kafka_config(self, online_write_options):
-        config = {
-            "kafka.bootstrap.servers": ",".join(
-                [
-                    endpoint.replace("INTERNAL://", "")
-                    for endpoint in self._kafka_api.get_broker_endpoints()
-                ]
-            ),
-            "kafka.security.protocol": "SSL",
-            "kafka.ssl.truststore.location": client.get_instance()._get_jks_trust_store_path(),
-            "kafka.ssl.truststore.password": client.get_instance()._cert_key,
-            "kafka.ssl.keystore.location": client.get_instance()._get_jks_key_store_path(),
-            "kafka.ssl.keystore.password": client.get_instance()._cert_key,
-            "kafka.ssl.key.password": client.get_instance()._cert_key,
-            "kafka.ssl.endpoint.identification.algorithm": "",
-        }
-        return {**online_write_options, **config}
-
     def insert_stream(
         self,
         feature_group,
         dataframe,
         query_name,
         output_mode,
         await_termination,
@@ -282,15 +260,15 @@
                 feature_group, dataframe_features, write_options
             )
 
             if not feature_group.stream:
                 # insert_stream method was called on non stream feature group object that has not been saved.
                 # we will use save_dataframe method on empty dataframe to create directory structure
                 offline_write_options = write_options
-                online_write_options = self.get_kafka_config(write_options)
+                online_write_options = write_options
                 engine.get_instance().save_dataframe(
                     feature_group,
                     engine.get_instance().create_empty_df(dataframe),
                     hudi_engine.HudiEngine.HUDI_BULK_INSERT
                     if feature_group.time_travel_format == "HUDI"
                     else None,
                     feature_group.online_enabled,
@@ -314,62 +292,19 @@
             feature_group,
             dataframe,
             query_name,
             output_mode,
             await_termination,
             timeout,
             checkpoint_dir,
-            self.get_kafka_config(write_options),
+            write_options,
         )
 
         return streaming_query
 
-    def _verify_schema_compatibility(self, feature_group_features, dataframe_features):
-        err = []
-        feature_df_dict = {feat.name: feat.type for feat in dataframe_features}
-        for feature_fg in feature_group_features:
-            fg_type = feature_fg.type.lower().replace(" ", "")
-            # check if feature exists dataframe
-            if feature_fg.name in feature_df_dict:
-                df_type = feature_df_dict[feature_fg.name].lower().replace(" ", "")
-                # remove match from lookup table
-                del feature_df_dict[feature_fg.name]
-
-                # check if types match
-                if fg_type != df_type:
-                    # don't check structs for exact match
-                    if fg_type.startswith("struct") and df_type.startswith("struct"):
-                        continue
-
-                    err += [
-                        f"{feature_fg.name} ("
-                        f"expected type: '{fg_type}', "
-                        f"derived from input: '{df_type}') has the wrong type."
-                    ]
-
-            else:
-                err += [
-                    f"{feature_fg.name} (type: '{feature_fg.type}') is missing from "
-                    f"input dataframe."
-                ]
-
-        # any features that are left in lookup table are superfluous
-        for feature_df_name, feature_df_type in feature_df_dict.items():
-            err += [
-                f"{feature_df_name} (type: '{feature_df_type}') does not exist "
-                f"in feature group."
-            ]
-
-        # raise exception if any errors were found.
-        if len(err) > 0:
-            raise FeatureStoreException(
-                "Features are not compatible with Feature Group schema: "
-                + "".join(["\n - " + e for e in err])
-            )
-
     def _save_feature_group_metadata(
         self, feature_group, dataframe_features, write_options
     ):
 
         # this means FG doesn't exist and should create the new one
         if len(feature_group.features) == 0:
             # User didn't provide a schema; extract it from the dataframe
```

### Comparing `hsfs-3.1.1rc4/hsfs/core/feature_store_api.py` & `hsfs-3.2.0rc0/hsfs/core/feature_store_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/feature_view_api.py` & `hsfs-3.2.0rc0/hsfs/core/feature_view_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/feature_view_engine.py` & `hsfs-3.2.0rc0/hsfs/core/feature_view_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,38 +121,45 @@
                     )
                 else:
                     raise FeatureStoreException(
                         FeatureViewEngine.LABEL_NOT_EXIST_ERROR.format(label_name)
                     )
         self._transformation_function_engine.attach_transformation_fn(feature_view_obj)
         updated_fv = self._feature_view_api.post(feature_view_obj)
+        self.attach_transformation_function(updated_fv)
         print(
             "Feature view created successfully, explore it at \n"
             + self._get_feature_view_url(updated_fv)
         )
         return updated_fv
 
     def update(self, feature_view_obj):
         self._feature_view_api.update(feature_view_obj)
         return feature_view_obj
 
     def get(self, name, version=None):
         if version:
             fv = self._feature_view_api.get_by_name_version(name, version)
-            fv.transformation_functions = self.get_attached_transformation_fn(
-                fv.name, fv.version
-            )
+            self.attach_transformation_function(fv)
         else:
             fv = self._feature_view_api.get_by_name(name)
             for _fv in fv:
-                _fv.transformation_functions = self.get_attached_transformation_fn(
-                    _fv.name, _fv.version
-                )
+                self.attach_transformation_function(_fv)
         return fv
 
+    def attach_transformation_function(self, fv):
+        fv.transformation_functions = self.get_attached_transformation_fn(
+            fv.name, fv.version
+        )
+        if fv.transformation_functions:
+            for feature in fv.schema:
+                feature.transformation_function = fv.transformation_functions.get(
+                    feature.name, None
+                )
+
     def delete(self, name, version=None):
         if version:
             return self._feature_view_api.delete_by_name_version(name, version)
         else:
             return self._feature_view_api.delete_by_name(name)
 
     def get_batch_query(
```

### Comparing `hsfs-3.1.1rc4/hsfs/core/great_expectation_engine.py` & `hsfs-3.2.0rc0/hsfs/core/great_expectation_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         ingestion_result: str = "UNKNOWN",
     ) -> Union[
         ge.core.ExpectationSuiteValidationResult,
         validation_report.ValidationReport,
         None,
     ]:
         suite = self.fetch_or_convert_expectation_suite(
-            feature_group, expectation_suite
+            feature_group, expectation_suite, validation_options
         )
 
         if self.should_run_validation(
             expectation_suite=suite, validation_options=validation_options
         ):
             report = engine.get_instance().validate_with_great_expectations(
                 dataframe=dataframe,
@@ -84,25 +84,24 @@
 
     def fetch_or_convert_expectation_suite(
         self,
         feature_group,
         expectation_suite: Union[
             ge.core.ExpectationSuite, es.ExpectationSuite, None
         ] = None,
+        validation_options: dict = {},
     ) -> Optional[es.ExpectationSuite]:
         """Convert provided expectation suite or fetch the one attached to the Feature Group from backend."""
-        if expectation_suite:
+        if expectation_suite is not None:
             if isinstance(expectation_suite, es.ExpectationSuite):
-                suite = expectation_suite
-            else:
-                suite = es.ExpectationSuite.from_ge_type(expectation_suite)
-        else:
-            suite = feature_group.get_expectation_suite(False)
-
-        return suite
+                return expectation_suite
+            return es.ExpectationSuite.from_ge_type(expectation_suite)
+        if validation_options.get("fetch_expectation_suite", True):
+            return feature_group.get_expectation_suite(False)
+        return feature_group.expectation_suite
 
     def should_run_validation(
         self,
         expectation_suite: Optional[es.ExpectationSuite],
         validation_options: Dict[str, Any],
     ) -> bool:
         # Suite is None if not provided and nothing attached to FG.
```

### Comparing `hsfs-3.1.1rc4/hsfs/core/hosts_api.py` & `hsfs-3.2.0rc0/hsfs/core/hosts_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/hudi_engine.py` & `hsfs-3.2.0rc0/hsfs/core/hudi_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/ingestion_job.py` & `hsfs-3.2.0rc0/hsfs/core/ingestion_job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/ingestion_job_conf.py` & `hsfs-3.2.0rc0/hsfs/core/ingestion_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/inode.py` & `hsfs-3.2.0rc0/hsfs/core/inode.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/job.py` & `hsfs-3.2.0rc0/hsfs/core/job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/job_api.py` & `hsfs-3.2.0rc0/hsfs/core/job_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/job_configuration.py` & `hsfs-3.2.0rc0/hsfs/core/job_configuration.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/kafka_api.py` & `hsfs-3.2.0rc0/hsfs/core/kafka_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/project_api.py` & `hsfs-3.2.0rc0/hsfs/core/project_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/query_constructor_api.py` & `hsfs-3.2.0rc0/hsfs/core/query_constructor_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/services_api.py` & `hsfs-3.2.0rc0/hsfs/core/services_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/statistics_api.py` & `hsfs-3.2.0rc0/hsfs/core/statistics_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/statistics_engine.py` & `hsfs-3.2.0rc0/hsfs/core/statistics_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/storage_connector_api.py` & `hsfs-3.2.0rc0/hsfs/core/storage_connector_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/tags_api.py` & `hsfs-3.2.0rc0/hsfs/core/tags_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/training_dataset_api.py` & `hsfs-3.2.0rc0/hsfs/core/training_dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/training_dataset_engine.py` & `hsfs-3.2.0rc0/hsfs/core/training_dataset_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/training_dataset_job_conf.py` & `hsfs-3.2.0rc0/hsfs/core/training_dataset_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/transformation_function_api.py` & `hsfs-3.2.0rc0/hsfs/core/transformation_function_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/transformation_function_engine.py` & `hsfs-3.2.0rc0/hsfs/core/transformation_function_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/validation_report_api.py` & `hsfs-3.2.0rc0/hsfs/core/validation_report_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/validation_report_engine.py` & `hsfs-3.2.0rc0/hsfs/core/validation_report_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/validation_result_api.py` & `hsfs-3.2.0rc0/hsfs/core/validation_result_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/validation_result_engine.py` & `hsfs-3.2.0rc0/hsfs/core/validation_result_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/variable_api.py` & `hsfs-3.2.0rc0/hsfs/core/variable_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/core/vector_server.py` & `hsfs-3.2.0rc0/hsfs/core/vector_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,30 +52,30 @@
                 feature_store_id
             )
         )
         self._feature_view_engine = feature_view_engine.FeatureViewEngine(
             feature_store_id
         )
 
-    def init_serving(self, entity, batch, external):
+    def init_serving(self, entity, batch, external, options=None):
         if external is None:
             external = isinstance(client.get_instance(), client.external.Client)
         # `init_prepared_statement` should be the last because other initialisations
         # has to be done successfully before it is able to fetch feature vectors.
         self.init_transformation(entity)
-        self.init_prepared_statement(entity, batch, external)
+        self.init_prepared_statement(entity, batch, external, options=options)
 
     def init_batch_scoring(self, entity):
         self.init_transformation(entity)
 
     def init_transformation(self, entity):
         # attach transformation functions
         self._transformation_functions = self._get_transformation_fns(entity)
 
-    def init_prepared_statement(self, entity, batch, external):
+    def init_prepared_statement(self, entity, batch, external, options=None):
         if isinstance(entity, feature_view.FeatureView):
             prepared_statements = self._feature_view_api.get_serving_prepared_statement(
                 entity.name, entity.version, batch
             )
         elif isinstance(entity, training_dataset.TrainingDataset):
             prepared_statements = (
                 self._training_dataset_api.get_serving_prepared_statement(entity, batch)
@@ -86,15 +86,15 @@
             )
         # reset values to default, as user may be re-initialising with different parameters
         self._prepared_statement_engine = None
         self._prepared_statements = None
         self._serving_keys = None
         self._external = external
 
-        self._set_mysql_connection()
+        self._set_mysql_connection(options=options)
 
         prepared_statements_dict = {}
         pkname_by_serving_index = {}
         prefix_by_serving_index = {}
         serving_vector_keys = set()
         for prepared_statement in prepared_statements:
             query_online = str(prepared_statement.query_online).replace("\n", " ")
@@ -295,18 +295,18 @@
                 pass
         except exc.OperationalError:
             self._set_mysql_connection()
 
     def _make_preview_statement(self, statement, n):
         return text(statement.text[: statement.text.find(" WHERE ")] + f" LIMIT {n}")
 
-    def _set_mysql_connection(self):
+    def _set_mysql_connection(self, options=None):
         online_conn = self._storage_connector_api.get_online_connector()
         self._prepared_statement_engine = util.create_mysql_engine(
-            online_conn, self._external
+            online_conn, self._external, options=options
         )
 
     def _generate_vector(self, result_dict):
         vector = []
         for feature in self._features:
             if feature.label:
                 # Skip the label
```

### Comparing `hsfs-3.1.1rc4/hsfs/decorators.py` & `hsfs-3.2.0rc0/hsfs/decorators.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/engine/__init__.py` & `hsfs-3.2.0rc0/hsfs/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/engine/python.py` & `hsfs-3.2.0rc0/hsfs/engine/python.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from typing import TypeVar, Optional, Dict, Any
 from confluent_kafka import Producer, KafkaError
 from tqdm.auto import tqdm
 from botocore.response import StreamingBody
 from sqlalchemy import sql
 
 from hsfs import client, feature, util
+from hsfs.feature_group import ExternalFeatureGroup
 from hsfs.client.exceptions import FeatureStoreException
 from hsfs.core import (
     feature_group_api,
     dataset_api,
     job_api,
     ingestion_job_conf,
     kafka_api,
@@ -372,35 +373,36 @@
         pass
 
     def convert_to_default_dataframe(self, dataframe):
         if isinstance(dataframe, pd.DataFrame):
             upper_case_features = [
                 col for col in dataframe.columns if any(re.finditer("[A-Z]", col))
             ]
+
+            # make shallow copy so the original df does not get changed
+            # this is always needed to keep the user df unchanged
+            dataframe_copy = dataframe.copy(deep=False)
+
+            # making a shallow copy of the dataframe so that column names are unchanged
             if len(upper_case_features) > 0:
                 warnings.warn(
                     "The ingested dataframe contains upper case letters in feature names: `{}`. "
                     "Feature names are sanitized to lower case in the feature store.".format(
                         upper_case_features
                     ),
                     util.FeatureGroupWarning,
                 )
-
-            # make shallow copy so the original df does not get changed
-            dataframe_copy = dataframe.copy(deep=False)
+                dataframe_copy.columns = [x.lower() for x in dataframe_copy.columns]
 
             # convert timestamps with timezone to UTC
             for col in dataframe_copy.columns:
                 if isinstance(
                     dataframe_copy[col].dtype, pd.core.dtypes.dtypes.DatetimeTZDtype
                 ):
                     dataframe_copy[col] = dataframe_copy[col].dt.tz_convert(None)
-
-            # making a shallow copy of the dataframe so that column names are unchanged
-            dataframe_copy.columns = [x.lower() for x in dataframe_copy.columns]
             return dataframe_copy
 
         raise TypeError(
             "The provided dataframe type is not recognized. Supported types are: pandas dataframe. "
             + "The provided dataframe has type: {}".format(type(dataframe))
         )
 
@@ -431,15 +433,18 @@
         operation: str,
         online_enabled: bool,
         storage: bool,
         offline_write_options: dict,
         online_write_options: dict,
         validation_id: int = None,
     ):
-        if feature_group.stream:
+        if (
+            isinstance(feature_group, ExternalFeatureGroup)
+            and feature_group.online_enabled
+        ) or feature_group.stream:
             return self._write_dataframe_kafka(
                 feature_group, dataframe, offline_write_options
             )
         else:
             # for backwards compatibility
             return self.legacy_save_dataframe(
                 feature_group,
@@ -789,55 +794,76 @@
 
         return dataset
 
     @staticmethod
     def get_unique_values(feature_dataframe, feature_name):
         return feature_dataframe[feature_name].unique()
 
-    def _write_dataframe_kafka(
-        self,
-        feature_group: FeatureGroup,
-        dataframe: pd.DataFrame,
-        offline_write_options: dict,
-    ):
+    def _init_kafka_resources(self, feature_group, offline_write_options):
         # setup kafka producer
         producer = Producer(self._get_kafka_config(offline_write_options))
 
         # setup complex feature writers
         feature_writers = {
             feature: self._get_encoder_func(
                 feature_group._get_feature_avro_schema(feature)
             )
             for feature in feature_group.get_complex_features()
         }
 
         # setup row writer function
         writer = self._get_encoder_func(feature_group._get_encoded_avro_schema())
+        return producer, feature_writers, writer
+
+    def _write_dataframe_kafka(
+        self,
+        feature_group: FeatureGroup,
+        dataframe: pd.DataFrame,
+        offline_write_options: dict,
+    ):
+        if feature_group._multi_part_insert:
+            if feature_group._kafka_producer is None:
+                producer, feature_writers, writer = self._init_kafka_resources(
+                    feature_group, offline_write_options
+                )
+                feature_group._kafka_producer = producer
+                feature_group._feature_writers = feature_writers
+                feature_group._writer = writer
+            else:
+                producer = feature_group._kafka_producer
+                feature_writers = feature_group._feature_writers
+                writer = feature_group._writer
+        else:
+            producer, feature_writers, writer = self._init_kafka_resources(
+                feature_group, offline_write_options
+            )
+
+            # initialize progress bar
+            progress_bar = tqdm(
+                total=dataframe.shape[0],
+                bar_format="{desc}: {percentage:.2f}% |{bar}| Rows {n_fmt}/{total_fmt} | "
+                "Elapsed Time: {elapsed} | Remaining Time: {remaining}",
+                desc="Uploading Dataframe",
+                mininterval=1,
+            )
 
         def acked(err, msg):
             if err is not None:
                 if offline_write_options.get("debug_kafka", False):
                     print("Failed to deliver message: %s: %s" % (str(msg), str(err)))
                 if err.code() in [
                     KafkaError.TOPIC_AUTHORIZATION_FAILED,
                     KafkaError._MSG_TIMED_OUT,
                 ]:
                     progress_bar.colour = "RED"
                     raise err  # Stop producing and show error
             # update progress bar for each msg
-            progress_bar.update()
+            if not feature_group._multi_part_insert:
+                progress_bar.update()
 
-        # initialize progress bar
-        progress_bar = tqdm(
-            total=dataframe.shape[0],
-            bar_format="{desc}: {percentage:.2f}% |{bar}| Rows {n_fmt}/{total_fmt} | "
-            "Elapsed Time: {elapsed} | Remaining Time: {remaining}",
-            desc="Uploading Dataframe",
-            mininterval=1,
-        )
         # loop over rows
         for r in dataframe.itertuples(index=False):
             # itertuples returns Python NamedTyple, to be able to serialize it using
             # avro, create copy of row only by converting to dict, which preserves datatypes
             row = r._asdict()
 
             # transform special data types
@@ -865,29 +891,30 @@
             key = "".join([str(row[pk]) for pk in sorted(feature_group.primary_key)])
 
             self._kafka_produce(
                 producer, feature_group, key, encoded_row, acked, offline_write_options
             )
 
         # make sure producer blocks and everything is delivered
-        producer.flush()
-        progress_bar.close()
+        if not feature_group._multi_part_insert:
+            producer.flush()
+            progress_bar.close()
 
         # start backfilling job
-        job_name = "{fg_name}_{version}_offline_fg_backfill".format(
-            fg_name=feature_group.name, version=feature_group.version
-        )
-        job = self._job_api.get(job_name)
-
-        if offline_write_options is not None and offline_write_options.get(
-            "start_offline_backfill", True
+        if (
+            not isinstance(feature_group, ExternalFeatureGroup)
+            and offline_write_options is not None
+            and offline_write_options.get("start_offline_backfill", True)
         ):
-            job.run(await_termination=offline_write_options.get("wait_for_job", True))
-
-        return job
+            feature_group.backfill_job.run(
+                await_termination=offline_write_options.get("wait_for_job", True)
+            )
+        if isinstance(feature_group, ExternalFeatureGroup):
+            return None
+        return feature_group.backfill_job
 
     def _kafka_produce(
         self, producer, feature_group, key, encoded_row, acked, offline_write_options
     ):
         while True:
             # if BufferError is thrown, we can be sure, message hasn't been send so we retry
             try:
```

### Comparing `hsfs-3.1.1rc4/hsfs/engine/spark.py` & `hsfs-3.2.0rc0/hsfs/engine/spark.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,18 @@
         BooleanType,
         StructField,
     )
 except ImportError:
     pass
 
 from hsfs import feature, training_dataset_feature, client, util
+from hsfs.feature_group import ExternalFeatureGroup
 from hsfs.storage_connector import StorageConnector
 from hsfs.client.exceptions import FeatureStoreException
-from hsfs.core import hudi_engine, transformation_function_engine
+from hsfs.core import hudi_engine, transformation_function_engine, kafka_api
 from hsfs.constructor import query
 from hsfs.training_dataset_split import TrainingDatasetSplit
 
 from great_expectations.core.batch import RuntimeBatchRequest
 from great_expectations.data_context import BaseDataContext
 from great_expectations.data_context.types.base import (
     DataContextConfig,
@@ -97,14 +98,17 @@
         self._spark_session.conf.set("spark.sql.hive.convertMetastoreParquet", "false")
         self._spark_session.conf.set("spark.sql.session.timeZone", "UTC")
 
         if importlib.util.find_spec("pydoop"):
             # If we are on Databricks don't setup Pydoop as it's not available and cannot be easily installed.
             util.setup_pydoop()
 
+        self._kafka_api = kafka_api.KafkaApi()
+        self._kafka_config = None
+
     def sql(
         self,
         sql_query,
         feature_store,
         connector,
         dataframe_type,
         read_options,
@@ -254,15 +258,18 @@
         online_enabled,
         storage,
         offline_write_options,
         online_write_options,
         validation_id=None,
     ):
         try:
-            if feature_group.stream:
+            if (
+                isinstance(feature_group, ExternalFeatureGroup)
+                and feature_group.online_enabled
+            ) or feature_group.stream:
                 self._save_online_dataframe(
                     feature_group, dataframe, online_write_options
                 )
             else:
                 if storage == "offline" or not online_enabled:
                     self._save_offline_dataframe(
                         feature_group,
@@ -295,14 +302,15 @@
         query_name,
         output_mode,
         await_termination,
         timeout,
         checkpoint_dir,
         write_options,
     ):
+        write_options = self._get_kafka_config(write_options)
         serialized_df = self._online_fg_to_avro(
             feature_group, self._encode_complex_features(feature_group, dataframe)
         )
 
         if query_name is None:
             query_name = "insert_stream_" + feature_group._online_topic_name
 
@@ -363,14 +371,16 @@
                 feature_group.partition_key if feature_group.partition_key else []
             ).saveAsTable(
                 feature_group._get_table_name()
             )
 
     def _save_online_dataframe(self, feature_group, dataframe, write_options):
 
+        write_options = self._get_kafka_config(write_options)
+
         serialized_df = self._online_fg_to_avro(
             feature_group, self._encode_complex_features(feature_group, dataframe)
         )
 
         version = str(feature_group.subject["version"]).encode("utf8")
 
         serialized_df.withColumn(
@@ -696,22 +706,20 @@
         dataframe,
         relevant_columns,
         correlations,
         histograms,
         exact_uniqueness=True,
     ):
         """Profile a dataframe with Deequ."""
-        return (
-            self._jvm.com.logicalclocks.hsfs.engine.SparkEngine.getInstance().profile(
-                dataframe._jdf,
-                relevant_columns,
-                correlations,
-                histograms,
-                exact_uniqueness,
-            )
+        return self._jvm.com.logicalclocks.hsfs.spark.engine.SparkEngine.getInstance().profile(
+            dataframe._jdf,
+            relevant_columns,
+            correlations,
+            histograms,
+            exact_uniqueness,
         )
 
     def validate_with_great_expectations(
         self,
         dataframe: TypeVar("pyspark.sql.DataFrame"),  # noqa: F821
         expectation_suite: TypeVar("ge.core.ExpectationSuite"),  # noqa: F821
         ge_validate_kwargs: Optional[dict],
@@ -1093,10 +1101,29 @@
                 for _feat in schema
             ]
         )
         for _feat in pyspark_schema:
             df = df.withColumn(_feat, col(_feat).cast(pyspark_schema[_feat]))
         return df
 
+    def _get_kafka_config(self, write_options: dict = {}) -> dict:
+        if self._kafka_config is None:
+            self._kafka_config = {
+                "kafka.bootstrap.servers": ",".join(
+                    [
+                        endpoint.replace("INTERNAL://", "")
+                        for endpoint in self._kafka_api.get_broker_endpoints()
+                    ]
+                ),
+                "kafka.security.protocol": "SSL",
+                "kafka.ssl.truststore.location": client.get_instance()._get_jks_trust_store_path(),
+                "kafka.ssl.truststore.password": client.get_instance()._cert_key,
+                "kafka.ssl.keystore.location": client.get_instance()._get_jks_key_store_path(),
+                "kafka.ssl.keystore.password": client.get_instance()._cert_key,
+                "kafka.ssl.key.password": client.get_instance()._cert_key,
+                "kafka.ssl.endpoint.identification.algorithm": "",
+            }
+        return {**write_options, **self._kafka_config}
+
 
 class SchemaError(Exception):
     """Thrown when schemas don't match"""
```

### Comparing `hsfs-3.1.1rc4/hsfs/expectation_suite.py` & `hsfs-3.2.0rc0/hsfs/expectation_suite.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/feature.py` & `hsfs-3.2.0rc0/hsfs/feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/feature_group.py` & `hsfs-3.2.0rc0/hsfs/feature_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,6121 +51,6870 @@
 00000320: 656d 610a 6672 6f6d 2074 7970 696e 6720  ema.from typing 
 00000330: 696d 706f 7274 204f 7074 696f 6e61 6c2c  import Optional,
 00000340: 2055 6e69 6f6e 2c20 416e 792c 2044 6963   Union, Any, Dic
 00000350: 742c 204c 6973 742c 2054 7970 6556 6172  t, List, TypeVar
 00000360: 2c20 5475 706c 650a 0a66 726f 6d20 6461  , Tuple..from da
 00000370: 7465 7469 6d65 2069 6d70 6f72 7420 6461  tetime import da
 00000380: 7465 7469 6d65 2c20 6461 7465 0a0a 6672  tetime, date..fr
-00000390: 6f6d 2068 7366 7320 696d 706f 7274 2075  om hsfs import u
-000003a0: 7469 6c2c 2065 6e67 696e 652c 2066 6561  til, engine, fea
-000003b0: 7475 7265 2c20 7573 6572 2c20 7374 6f72  ture, user, stor
-000003c0: 6167 655f 636f 6e6e 6563 746f 7220 6173  age_connector as
-000003d0: 2073 630a 6672 6f6d 2068 7366 732e 636f   sc.from hsfs.co
-000003e0: 7265 2069 6d70 6f72 7420 280a 2020 2020  re import (.    
-000003f0: 6665 6174 7572 655f 6772 6f75 705f 656e  feature_group_en
-00000400: 6769 6e65 2c0a 2020 2020 7374 6174 6973  gine,.    statis
-00000410: 7469 6373 5f65 6e67 696e 652c 0a20 2020  tics_engine,.   
-00000420: 2065 7870 6563 7461 7469 6f6e 5f73 7569   expectation_sui
-00000430: 7465 5f65 6e67 696e 652c 0a20 2020 2076  te_engine,.    v
-00000440: 616c 6964 6174 696f 6e5f 7265 706f 7274  alidation_report
-00000450: 5f65 6e67 696e 652c 0a20 2020 2063 6f64  _engine,.    cod
-00000460: 655f 656e 6769 6e65 2c0a 2020 2020 6578  e_engine,.    ex
-00000470: 7465 726e 616c 5f66 6561 7475 7265 5f67  ternal_feature_g
-00000480: 726f 7570 5f65 6e67 696e 652c 0a20 2020  roup_engine,.   
-00000490: 2076 616c 6964 6174 696f 6e5f 7265 7375   validation_resu
-000004a0: 6c74 5f65 6e67 696e 652c 0a29 0a0a 6672  lt_engine,.)..fr
-000004b0: 6f6d 2068 7366 732e 7374 6174 6973 7469  om hsfs.statisti
-000004c0: 6373 5f63 6f6e 6669 6720 696d 706f 7274  cs_config import
-000004d0: 2053 7461 7469 7374 6963 7343 6f6e 6669   StatisticsConfi
-000004e0: 670a 6672 6f6d 2068 7366 732e 6578 7065  g.from hsfs.expe
-000004f0: 6374 6174 696f 6e5f 7375 6974 6520 696d  ctation_suite im
-00000500: 706f 7274 2045 7870 6563 7461 7469 6f6e  port Expectation
-00000510: 5375 6974 650a 6672 6f6d 2068 7366 732e  Suite.from hsfs.
-00000520: 7661 6c69 6461 7469 6f6e 5f72 6570 6f72  validation_repor
-00000530: 7420 696d 706f 7274 2056 616c 6964 6174  t import Validat
-00000540: 696f 6e52 6570 6f72 740a 6672 6f6d 2068  ionReport.from h
-00000550: 7366 732e 636f 6e73 7472 7563 746f 7220  sfs.constructor 
-00000560: 696d 706f 7274 2071 7565 7279 2c20 6669  import query, fi
-00000570: 6c74 6572 0a66 726f 6d20 6873 6673 2e63  lter.from hsfs.c
-00000580: 6c69 656e 742e 6578 6365 7074 696f 6e73  lient.exceptions
-00000590: 2069 6d70 6f72 7420 4665 6174 7572 6553   import FeatureS
-000005a0: 746f 7265 4578 6365 7074 696f 6e0a 6672  toreException.fr
-000005b0: 6f6d 2068 7366 732e 636f 7265 2e6a 6f62  om hsfs.core.job
-000005c0: 2069 6d70 6f72 7420 4a6f 620a 6672 6f6d   import Job.from
-000005d0: 2068 7366 732e 636f 7265 2e76 6172 6961   hsfs.core.varia
-000005e0: 626c 655f 6170 6920 696d 706f 7274 2056  ble_api import V
-000005f0: 6172 6961 626c 6541 7069 0a66 726f 6d20  ariableApi.from 
-00000600: 6873 6673 2e63 6f72 6520 696d 706f 7274  hsfs.core import
-00000610: 2067 7265 6174 5f65 7870 6563 7461 7469   great_expectati
-00000620: 6f6e 5f65 6e67 696e 650a 0a0a 636c 6173  on_engine...clas
-00000630: 7320 4665 6174 7572 6547 726f 7570 4261  s FeatureGroupBa
-00000640: 7365 3a0a 2020 2020 6465 6620 5f5f 696e  se:.    def __in
-00000650: 6974 5f5f 2873 656c 662c 2066 6561 7475  it__(self, featu
-00000660: 7265 7374 6f72 655f 6964 2c20 6c6f 6361  restore_id, loca
-00000670: 7469 6f6e 2c20 6576 656e 745f 7469 6d65  tion, event_time
-00000680: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00000690: 7365 6c66 2e65 7665 6e74 5f74 696d 6520  self.event_time 
-000006a0: 3d20 6576 656e 745f 7469 6d65 0a20 2020  = event_time.   
-000006b0: 2020 2020 2073 656c 662e 5f6c 6f63 6174       self._locat
-000006c0: 696f 6e20 3d20 6c6f 6361 7469 6f6e 0a20  ion = location. 
-000006d0: 2020 2020 2020 2073 656c 662e 5f73 7461         self._sta
-000006e0: 7469 7374 6963 735f 656e 6769 6e65 203d  tistics_engine =
-000006f0: 2073 7461 7469 7374 6963 735f 656e 6769   statistics_engi
-00000700: 6e65 2e53 7461 7469 7374 6963 7345 6e67  ne.StatisticsEng
-00000710: 696e 6528 0a20 2020 2020 2020 2020 2020  ine(.           
-00000720: 2066 6561 7475 7265 7374 6f72 655f 6964   featurestore_id
-00000730: 2c20 7365 6c66 2e45 4e54 4954 595f 5459  , self.ENTITY_TY
-00000740: 5045 0a20 2020 2020 2020 2029 0a20 2020  PE.        ).   
-00000750: 2020 2020 2073 656c 662e 5f63 6f64 655f       self._code_
-00000760: 656e 6769 6e65 203d 2063 6f64 655f 656e  engine = code_en
-00000770: 6769 6e65 2e43 6f64 6545 6e67 696e 6528  gine.CodeEngine(
-00000780: 6665 6174 7572 6573 746f 7265 5f69 642c  featurestore_id,
-00000790: 2073 656c 662e 454e 5449 5459 5f54 5950   self.ENTITY_TYP
-000007a0: 4529 0a20 2020 2020 2020 2073 656c 662e  E).        self.
-000007b0: 5f67 7265 6174 5f65 7870 6563 7461 7469  _great_expectati
-000007c0: 6f6e 5f65 6e67 696e 6520 3d20 280a 2020  on_engine = (.  
-000007d0: 2020 2020 2020 2020 2020 6772 6561 745f            great_
-000007e0: 6578 7065 6374 6174 696f 6e5f 656e 6769  expectation_engi
-000007f0: 6e65 2e47 7265 6174 4578 7065 6374 6174  ne.GreatExpectat
-00000800: 696f 6e45 6e67 696e 6528 6665 6174 7572  ionEngine(featur
-00000810: 6573 746f 7265 5f69 6429 0a20 2020 2020  estore_id).     
-00000820: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-00000830: 662e 5f66 6561 7475 7265 5f73 746f 7265  f._feature_store
-00000840: 5f69 6420 3d20 6665 6174 7572 6573 746f  _id = featuresto
-00000850: 7265 5f69 640a 2020 2020 2020 2020 7365  re_id.        se
-00000860: 6c66 2e5f 7661 7269 6162 6c65 5f61 7069  lf._variable_api
-00000870: 203d 2056 6172 6961 626c 6541 7069 2829   = VariableApi()
-00000880: 0a0a 2020 2020 6465 6620 6465 6c65 7465  ..    def delete
-00000890: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000008a0: 2222 2244 726f 7020 7468 6520 656e 7469  """Drop the enti
-000008b0: 7265 2066 6561 7475 7265 2067 726f 7570  re feature group
-000008c0: 2061 6c6f 6e67 2077 6974 6820 6974 7320   along with its 
-000008d0: 6665 6174 7572 6520 6461 7461 2e0a 0a20  feature data... 
-000008e0: 2020 2020 2020 2021 2121 2065 7861 6d70         !!! examp
-000008f0: 6c65 0a20 2020 2020 2020 2020 2020 2060  le.            `
-00000900: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
-00000910: 2020 2020 2023 2063 6f6e 6e65 6374 2074       # connect t
-00000920: 6f20 7468 6520 4665 6174 7572 6520 5374  o the Feature St
-00000930: 6f72 650a 2020 2020 2020 2020 2020 2020  ore.            
-00000940: 6673 203d 202e 2e2e 0a0a 2020 2020 2020  fs = .....      
-00000950: 2020 2020 2020 2320 6765 7420 7468 6520        # get the 
-00000960: 4665 6174 7572 6520 4772 6f75 7020 696e  Feature Group in
-00000970: 7374 616e 6365 0a20 2020 2020 2020 2020  stance.         
-00000980: 2020 2066 6720 3d20 6673 2e67 6574 5f6f     fg = fs.get_o
-00000990: 725f 6372 6561 7465 5f66 6561 7475 7265  r_create_feature
-000009a0: 5f67 726f 7570 280a 2020 2020 2020 2020  _group(.        
-000009b0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-000009c0: 3d27 6269 7463 6f69 6e5f 7072 6963 6527  ='bitcoin_price'
-000009d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000009e0: 2020 2020 2020 7665 7273 696f 6e3d 310a        version=1.
-000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a00: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-00000a10: 2020 2023 2064 656c 6574 6520 7468 6520     # delete the 
-00000a20: 6665 6174 7572 6520 6772 6f75 700a 2020  feature group.  
-00000a30: 2020 2020 2020 2020 2020 6667 2e64 656c            fg.del
-00000a40: 6574 6528 290a 2020 2020 2020 2020 2020  ete().          
-00000a50: 2020 6060 600a 0a20 2020 2020 2020 2021    ```..        !
-00000a60: 2121 2064 616e 6765 7220 2250 6f74 656e  !! danger "Poten
-00000a70: 7469 616c 6c79 2064 616e 6765 726f 7573  tially dangerous
-00000a80: 206f 7065 7261 7469 6f6e 220a 2020 2020   operation".    
-00000a90: 2020 2020 2020 2020 5468 6973 206f 7065          This ope
-00000aa0: 7261 7469 6f6e 2064 726f 7073 2061 6c6c  ration drops all
-00000ab0: 206d 6574 6164 6174 6120 6173 736f 6369   metadata associ
-00000ac0: 6174 6564 2077 6974 6820 2a2a 7468 6973  ated with **this
-00000ad0: 2076 6572 7369 6f6e 2a2a 206f 6620 7468   version** of th
-00000ae0: 650a 2020 2020 2020 2020 2020 2020 6665  e.            fe
-00000af0: 6174 7572 6520 6772 6f75 7020 2a2a 616e  ature group **an
-00000b00: 642a 2a20 616c 6c20 7468 6520 6665 6174  d** all the feat
-00000b10: 7572 6520 6461 7461 2069 6e20 6f66 666c  ure data in offl
-00000b20: 696e 6520 616e 6420 6f6e 6c69 6e65 2073  ine and online s
-00000b30: 746f 7261 6765 0a20 2020 2020 2020 2020  torage.         
-00000b40: 2020 2061 7373 6f63 6961 7465 6420 7769     associated wi
-00000b50: 7468 2069 742e 0a0a 2020 2020 2020 2020  th it...        
-00000b60: 2320 5261 6973 6573 0a20 2020 2020 2020  # Raises.       
-00000b70: 2020 2020 2060 6873 6673 2e63 6c69 656e       `hsfs.clien
-00000b80: 742e 6578 6365 7074 696f 6e73 2e52 6573  t.exceptions.Res
-00000b90: 7441 5049 4572 726f 7260 2e0a 2020 2020  tAPIError`..    
-00000ba0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00000bb0: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
-00000bc0: 2020 2020 2020 2020 2020 2022 416c 6c20             "All 
-00000bd0: 6a6f 6273 2061 7373 6f63 6961 7465 6420  jobs associated 
-00000be0: 746f 2066 6561 7475 7265 2067 726f 7570  to feature group
-00000bf0: 2060 7b7d 602c 2076 6572 7369 6f6e 2060   `{}`, version `
-00000c00: 7b7d 6020 7769 6c6c 2062 6520 7265 6d6f  {}` will be remo
-00000c10: 7665 642e 222e 666f 726d 6174 280a 2020  ved.".format(.  
-00000c20: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00000c30: 6c66 2e5f 6e61 6d65 2c20 7365 6c66 2e5f  lf._name, self._
-00000c40: 7665 7273 696f 6e0a 2020 2020 2020 2020  version.        
-00000c50: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-00000c60: 2020 2075 7469 6c2e 4a6f 6257 6172 6e69     util.JobWarni
-00000c70: 6e67 2c0a 2020 2020 2020 2020 290a 2020  ng,.        ).  
-00000c80: 2020 2020 2020 7365 6c66 2e5f 6665 6174        self._feat
-00000c90: 7572 655f 6772 6f75 705f 656e 6769 6e65  ure_group_engine
-00000ca0: 2e64 656c 6574 6528 7365 6c66 290a 0a20  .delete(self).. 
-00000cb0: 2020 2064 6566 2073 656c 6563 745f 616c     def select_al
-00000cc0: 6c28 0a20 2020 2020 2020 2073 656c 662c  l(.        self,
-00000cd0: 0a20 2020 2020 2020 2069 6e63 6c75 6465  .        include
-00000ce0: 5f70 7269 6d61 7279 5f6b 6579 3a20 4f70  _primary_key: Op
-00000cf0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2054  tional[bool] = T
-00000d00: 7275 652c 0a20 2020 2020 2020 2069 6e63  rue,.        inc
-00000d10: 6c75 6465 5f65 7665 6e74 5f74 696d 653a  lude_event_time:
-00000d20: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
-00000d30: 3d20 5472 7565 2c0a 2020 2020 293a 0a20  = True,.    ):. 
-00000d40: 2020 2020 2020 2022 2222 5365 6c65 6374         """Select
-00000d50: 2061 6c6c 2066 6561 7475 7265 7320 696e   all features in
-00000d60: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
-00000d70: 7570 2061 6e64 2072 6574 7572 6e20 6120  up and return a 
-00000d80: 7175 6572 7920 6f62 6a65 6374 2e0a 0a20  query object... 
-00000d90: 2020 2020 2020 2054 6865 2071 7565 7279         The query
-00000da0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-00000db0: 636f 6e73 7472 7563 7420 6a6f 696e 7320  construct joins 
-00000dc0: 6f66 2066 6561 7475 7265 2067 726f 7570  of feature group
-00000dd0: 7320 6f72 2063 7265 6174 6520 610a 2020  s or create a.  
-00000de0: 2020 2020 2020 6665 6174 7572 6520 7669        feature vi
-00000df0: 6577 2e0a 0a20 2020 2020 2020 2021 2121  ew...        !!!
-00000e00: 2065 7861 6d70 6c65 0a20 2020 2020 2020   example.       
-00000e10: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
-00000e20: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
-00000e30: 6e65 6374 2074 6f20 7468 6520 4665 6174  nect to the Feat
-00000e40: 7572 6520 5374 6f72 650a 2020 2020 2020  ure Store.      
-00000e50: 2020 2020 2020 6673 203d 202e 2e2e 0a0a        fs = .....
-00000e60: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
-00000e70: 7420 7468 6520 4665 6174 7572 6520 4772  t the Feature Gr
-00000e80: 6f75 7020 696e 7374 616e 6365 730a 2020  oup instances.  
-00000e90: 2020 2020 2020 2020 2020 6667 3120 3d20            fg1 = 
-00000ea0: 6673 2e67 6574 5f6f 725f 6372 6561 7465  fs.get_or_create
-00000eb0: 5f66 6561 7475 7265 5f67 726f 7570 282e  _feature_group(.
-00000ec0: 2e2e 290a 2020 2020 2020 2020 2020 2020  ..).            
-00000ed0: 6667 3220 3d20 6673 2e67 6574 5f6f 725f  fg2 = fs.get_or_
-00000ee0: 6372 6561 7465 5f66 6561 7475 7265 5f67  create_feature_g
-00000ef0: 726f 7570 282e 2e2e 290a 0a20 2020 2020  roup(...)..     
-00000f00: 2020 2020 2020 2023 2063 6f6e 7374 7275         # constru
-00000f10: 6374 2074 6865 2071 7565 7279 0a20 2020  ct the query.   
-00000f20: 2020 2020 2020 2020 2071 7565 7279 203d           query =
-00000f30: 2066 6731 2e73 656c 6563 745f 616c 6c28   fg1.select_all(
-00000f40: 292e 6a6f 696e 2866 6732 2e73 656c 6563  ).join(fg2.selec
-00000f50: 745f 616c 6c28 2929 0a0a 2020 2020 2020  t_all())..      
-00000f60: 2020 2020 2020 2320 7368 6f77 2066 6972        # show fir
-00000f70: 7374 2035 2072 6f77 730a 2020 2020 2020  st 5 rows.      
-00000f80: 2020 2020 2020 7175 6572 792e 7368 6f77        query.show
-00000f90: 2835 290a 0a0a 2020 2020 2020 2020 2020  (5)...          
-00000fa0: 2020 2320 7365 6c65 6374 2061 6c6c 2066    # select all f
-00000fb0: 6561 7475 7265 7320 6578 636c 7564 6520  eatures exclude 
-00000fc0: 7072 696d 6172 7920 6b65 7920 616e 6420  primary key and 
-00000fd0: 6576 656e 7420 7469 6d65 0a20 2020 2020  event time.     
-00000fe0: 2020 2020 2020 2066 726f 6d20 6873 6673         from hsfs
-00000ff0: 2e66 6561 7475 7265 2069 6d70 6f72 7420  .feature import 
-00001000: 4665 6174 7572 650a 2020 2020 2020 2020  Feature.        
-00001010: 2020 2020 6667 203d 2066 732e 6372 6561      fg = fs.crea
-00001020: 7465 5f66 6561 7475 7265 5f67 726f 7570  te_feature_group
-00001030: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00001040: 2020 2020 2020 2266 6722 2c0a 2020 2020        "fg",.    
-00001050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001060: 6665 6174 7572 6573 3d5b 0a20 2020 2020  features=[.     
-00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001080: 2020 2020 2020 2046 6561 7475 7265 2822         Feature("
-00001090: 6964 222c 2074 7970 653d 2273 7472 696e  id", type="strin
-000010a0: 6722 292c 0a20 2020 2020 2020 2020 2020  g"),.           
-000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010c0: 2046 6561 7475 7265 2822 7473 222c 2074   Feature("ts", t
-000010d0: 7970 653d 2262 6967 696e 7422 292c 0a20  ype="bigint"),. 
-000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010f0: 2020 2020 2020 2020 2020 2046 6561 7475             Featu
-00001100: 7265 2822 6631 222c 2074 7970 653d 2264  re("f1", type="d
-00001110: 6174 6522 292c 0a20 2020 2020 2020 2020  ate"),.         
-00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001130: 2020 2046 6561 7475 7265 2822 6632 222c     Feature("f2",
-00001140: 2074 7970 653d 2264 6f75 626c 6522 290a   type="double").
-00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001160: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
-00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001180: 2020 2070 7269 6d61 7279 5f6b 6579 3d5b     primary_key=[
-00001190: 2269 6422 5d2c 0a20 2020 2020 2020 2020  "id"],.         
-000011a0: 2020 2020 2020 2020 2020 2065 7665 6e74             event
-000011b0: 5f74 696d 653d 2274 7322 290a 0a20 2020  _time="ts")..   
-000011c0: 2020 2020 2020 2020 2071 7565 7279 203d           query =
-000011d0: 2066 672e 7365 6c65 6374 5f61 6c6c 2829   fg.select_all()
-000011e0: 0a20 2020 2020 2020 2020 2020 2071 7565  .            que
-000011f0: 7279 2e66 6561 7475 7265 730a 2020 2020  ry.features.    
-00001200: 2020 2020 2020 2020 2320 5b46 6561 7475          # [Featu
-00001210: 7265 2827 6964 272c 202e 2e2e 292c 2046  re('id', ...), F
-00001220: 6561 7475 7265 2827 7473 272c 202e 2e2e  eature('ts', ...
-00001230: 292c 2046 6561 7475 7265 2827 6631 272c  ), Feature('f1',
-00001240: 202e 2e2e 292c 2046 6561 7475 7265 2827   ...), Feature('
-00001250: 6632 272c 202e 2e2e 295d 0a0a 2020 2020  f2', ...)]..    
-00001260: 2020 2020 2020 2020 7175 6572 7920 3d20          query = 
-00001270: 6667 2e73 656c 6563 745f 616c 6c28 696e  fg.select_all(in
-00001280: 636c 7564 655f 7072 696d 6172 795f 6b65  clude_primary_ke
-00001290: 793d 4661 6c73 652c 2069 6e63 6c75 6465  y=False, include
-000012a0: 5f65 7665 6e74 5f74 696d 653d 4661 6c73  _event_time=Fals
-000012b0: 6529 0a20 2020 2020 2020 2020 2020 2071  e).            q
-000012c0: 7565 7279 2e66 6561 7475 7265 730a 2020  uery.features.  
-000012d0: 2020 2020 2020 2020 2020 2320 5b46 6561            # [Fea
-000012e0: 7475 7265 2827 6631 272c 202e 2e2e 292c  ture('f1', ...),
-000012f0: 2046 6561 7475 7265 2827 6632 272c 202e   Feature('f2', .
-00001300: 2e2e 295d 0a20 2020 2020 2020 2020 2020  ..)].           
-00001310: 2060 6060 0a0a 2020 2020 2020 2020 2320   ```..        # 
-00001320: 4172 6775 6d65 6e74 730a 2020 2020 2020  Arguments.      
-00001330: 2020 2020 2020 696e 636c 7564 655f 7072        include_pr
-00001340: 696d 6172 795f 6b65 793a 2049 6620 5472  imary_key: If Tr
-00001350: 7565 2c20 696e 636c 7564 6520 7072 696d  ue, include prim
-00001360: 6172 7920 6b65 7920 6f66 2074 6865 2066  ary key of the f
-00001370: 6561 7475 7265 2067 726f 7570 0a20 2020  eature group.   
-00001380: 2020 2020 2020 2020 2020 2020 2074 6f20               to 
-00001390: 7468 6520 6665 6174 7572 6520 6c69 7374  the feature list
-000013a0: 2e20 4465 6661 756c 7473 2074 6f20 5472  . Defaults to Tr
-000013b0: 7565 2e0a 2020 2020 2020 2020 2020 2020  ue..            
-000013c0: 696e 636c 7564 655f 6576 656e 745f 7469  include_event_ti
-000013d0: 6d65 3a20 4966 2054 7275 652c 2069 6e63  me: If True, inc
-000013e0: 6c75 6465 2065 7665 6e74 2074 696d 6520  lude event time 
-000013f0: 6f66 2074 6865 2066 6561 7475 7265 2067  of the feature g
-00001400: 726f 7570 0a20 2020 2020 2020 2020 2020  roup.           
-00001410: 2020 2020 2074 6f20 7468 6520 6665 6174       to the feat
-00001420: 7572 6520 6c69 7374 2e20 4465 6661 756c  ure list. Defaul
-00001430: 7473 2074 6f20 5472 7565 2e0a 2020 2020  ts to True..    
-00001440: 2020 2020 2320 5265 7475 726e 730a 2020      # Returns.  
-00001450: 2020 2020 2020 2020 2020 6051 7565 7279            `Query
-00001460: 602e 2041 2071 7565 7279 206f 626a 6563  `. A query objec
-00001470: 7420 7769 7468 2061 6c6c 2066 6561 7475  t with all featu
-00001480: 7265 7320 6f66 2074 6865 2066 6561 7475  res of the featu
-00001490: 7265 2067 726f 7570 2e0a 2020 2020 2020  re group..      
-000014a0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-000014b0: 2069 6e63 6c75 6465 5f65 7665 6e74 5f74   include_event_t
-000014c0: 696d 6520 616e 6420 696e 636c 7564 655f  ime and include_
-000014d0: 7072 696d 6172 795f 6b65 793a 0a20 2020  primary_key:.   
-000014e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000014f0: 7175 6572 792e 5175 6572 7928 0a20 2020  query.Query(.   
-00001500: 2020 2020 2020 2020 2020 2020 206c 6566               lef
-00001510: 745f 6665 6174 7572 655f 6772 6f75 703d  t_feature_group=
-00001520: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-00001530: 2020 2020 2020 6c65 6674 5f66 6561 7475        left_featu
-00001540: 7265 733d 7365 6c66 2e5f 6665 6174 7572  res=self._featur
-00001550: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00001560: 2020 2020 6665 6174 7572 655f 7374 6f72      feature_stor
-00001570: 655f 6e61 6d65 3d73 656c 662e 5f66 6561  e_name=self._fea
-00001580: 7475 7265 5f73 746f 7265 5f6e 616d 652c  ture_store_name,
-00001590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000015a0: 2066 6561 7475 7265 5f73 746f 7265 5f69   feature_store_i
-000015b0: 643d 7365 6c66 2e5f 6665 6174 7572 655f  d=self._feature_
-000015c0: 7374 6f72 655f 6964 2c0a 2020 2020 2020  store_id,.      
-000015d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000015e0: 656c 6966 2069 6e63 6c75 6465 5f65 7665  elif include_eve
-000015f0: 6e74 5f74 696d 653a 0a20 2020 2020 2020  nt_time:.       
-00001600: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00001610: 2e73 656c 6563 745f 6578 6365 7074 2873  .select_except(s
-00001620: 656c 662e 7072 696d 6172 795f 6b65 7929  elf.primary_key)
-00001630: 0a20 2020 2020 2020 2065 6c69 6620 696e  .        elif in
-00001640: 636c 7564 655f 7072 696d 6172 795f 6b65  clude_primary_ke
-00001650: 793a 0a20 2020 2020 2020 2020 2020 2072  y:.            r
-00001660: 6574 7572 6e20 7365 6c66 2e73 656c 6563  eturn self.selec
-00001670: 745f 6578 6365 7074 285b 7365 6c66 2e65  t_except([self.e
-00001680: 7665 6e74 5f74 696d 655d 290a 2020 2020  vent_time]).    
-00001690: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000016a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000016b0: 662e 7365 6c65 6374 5f65 7863 6570 7428  f.select_except(
-000016c0: 7365 6c66 2e70 7269 6d61 7279 5f6b 6579  self.primary_key
-000016d0: 202b 205b 7365 6c66 2e65 7665 6e74 5f74   + [self.event_t
-000016e0: 696d 655d 290a 0a20 2020 2064 6566 2073  ime])..    def s
-000016f0: 656c 6563 7428 7365 6c66 2c20 6665 6174  elect(self, feat
-00001700: 7572 6573 3a20 4f70 7469 6f6e 616c 5b4c  ures: Optional[L
-00001710: 6973 745b 556e 696f 6e5b 7374 722c 2066  ist[Union[str, f
-00001720: 6561 7475 7265 2e46 6561 7475 7265 5d5d  eature.Feature]]
-00001730: 5d20 3d20 5b5d 293a 0a20 2020 2020 2020  ] = []):.       
-00001740: 2022 2222 5365 6c65 6374 2061 2073 7562   """Select a sub
-00001750: 7365 7420 6f66 2066 6561 7475 7265 7320  set of features 
-00001760: 6f66 2074 6865 2066 6561 7475 7265 2067  of the feature g
-00001770: 726f 7570 2061 6e64 2072 6574 7572 6e20  roup and return 
-00001780: 6120 7175 6572 7920 6f62 6a65 6374 2e0a  a query object..
-00001790: 0a20 2020 2020 2020 2054 6865 2071 7565  .        The que
-000017a0: 7279 2063 616e 2062 6520 7573 6564 2074  ry can be used t
-000017b0: 6f20 636f 6e73 7472 7563 7420 6a6f 696e  o construct join
-000017c0: 7320 6f66 2066 6561 7475 7265 2067 726f  s of feature gro
-000017d0: 7570 7320 6f72 2063 7265 6174 6520 610a  ups or create a.
-000017e0: 2020 2020 2020 2020 6665 6174 7572 6520          feature 
-000017f0: 7669 6577 2077 6974 6820 6120 7375 6273  view with a subs
-00001800: 6574 206f 6620 6665 6174 7572 6573 206f  et of features o
-00001810: 6620 7468 6520 6665 6174 7572 6520 6772  f the feature gr
-00001820: 6f75 702e 0a0a 2020 2020 2020 2020 2121  oup...        !!
-00001830: 2120 6578 616d 706c 650a 2020 2020 2020  ! example.      
-00001840: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00001850: 2020 2020 2020 2020 2020 2020 2320 636f              # co
-00001860: 6e6e 6563 7420 746f 2074 6865 2046 6561  nnect to the Fea
-00001870: 7475 7265 2053 746f 7265 0a20 2020 2020  ture Store.     
-00001880: 2020 2020 2020 2066 7320 3d20 2e2e 2e0a         fs = ....
-00001890: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
-000018a0: 6574 2074 6865 2046 6561 7475 7265 2047  et the Feature G
-000018b0: 726f 7570 2069 6e73 7461 6e63 650a 2020  roup instance.  
-000018c0: 2020 2020 2020 2020 2020 6672 6f6d 2068            from h
-000018d0: 7366 732e 6665 6174 7572 6520 696d 706f  sfs.feature impo
-000018e0: 7274 2046 6561 7475 7265 0a20 2020 2020  rt Feature.     
-000018f0: 2020 2020 2020 2066 6720 3d20 6673 2e63         fg = fs.c
-00001900: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
-00001910: 6f75 7028 0a20 2020 2020 2020 2020 2020  oup(.           
-00001920: 2020 2020 2020 2020 2022 6667 222c 0a20           "fg",. 
-00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001940: 2020 2066 6561 7475 7265 733d 5b0a 2020     features=[.  
-00001950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001960: 2020 2020 2020 2020 2020 4665 6174 7572            Featur
-00001970: 6528 2269 6422 2c20 7479 7065 3d22 7374  e("id", type="st
-00001980: 7269 6e67 2229 2c0a 2020 2020 2020 2020  ring"),.        
-00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019a0: 2020 2020 4665 6174 7572 6528 2274 7322      Feature("ts"
-000019b0: 2c20 7479 7065 3d22 6269 6769 6e74 2229  , type="bigint")
-000019c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000019d0: 2020 2020 2020 2020 2020 2020 2020 4665                Fe
-000019e0: 6174 7572 6528 2266 3122 2c20 7479 7065  ature("f1", type
-000019f0: 3d22 6461 7465 2229 2c0a 2020 2020 2020  ="date"),.      
-00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a10: 2020 2020 2020 4665 6174 7572 6528 2266        Feature("f
-00001a20: 3222 2c20 7479 7065 3d22 646f 7562 6c65  2", type="double
-00001a30: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00001a40: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00001a50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001a60: 2020 2020 2020 7072 696d 6172 795f 6b65        primary_ke
-00001a70: 793d 5b22 6964 225d 2c0a 2020 2020 2020  y=["id"],.      
-00001a80: 2020 2020 2020 2020 2020 2020 2020 6576                ev
-00001a90: 656e 745f 7469 6d65 3d22 7473 2229 0a0a  ent_time="ts")..
-00001aa0: 2020 2020 2020 2020 2020 2020 2320 636f              # co
-00001ab0: 6e73 7472 7563 7420 7175 6572 790a 2020  nstruct query.  
-00001ac0: 2020 2020 2020 2020 2020 7175 6572 7920            query 
-00001ad0: 3d20 6667 2e73 656c 6563 7428 5b22 6964  = fg.select(["id
-00001ae0: 222c 2022 6631 225d 290a 2020 2020 2020  ", "f1"]).      
-00001af0: 2020 2020 2020 7175 6572 792e 6665 6174        query.feat
-00001b00: 7572 6573 0a20 2020 2020 2020 2020 2020  ures.           
-00001b10: 2023 205b 4665 6174 7572 6528 2769 6427   # [Feature('id'
-00001b20: 2c20 2e2e 2e29 2c20 4665 6174 7572 6528  , ...), Feature(
-00001b30: 2766 3127 2c20 2e2e 2e29 5d0a 2020 2020  'f1', ...)].    
-00001b40: 2020 2020 2020 2020 6060 600a 0a20 2020          ```..   
-00001b50: 2020 2020 2023 2041 7267 756d 656e 7473       # Arguments
-00001b60: 0a20 2020 2020 2020 2020 2020 2066 6561  .            fea
-00001b70: 7475 7265 733a 2041 206c 6973 7420 6f66  tures: A list of
-00001b80: 2060 4665 6174 7572 6560 206f 626a 6563   `Feature` objec
-00001b90: 7473 206f 7220 6665 6174 7572 6520 6e61  ts or feature na
-00001ba0: 6d65 7320 6173 0a20 2020 2020 2020 2020  mes as.         
-00001bb0: 2020 2020 2020 2073 7472 696e 6773 2074         strings t
-00001bc0: 6f20 6265 2073 656c 6563 7465 642c 2064  o be selected, d
-00001bd0: 6566 6175 6c74 7320 746f 205b 5d2e 0a0a  efaults to []...
-00001be0: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
-00001bf0: 730a 2020 2020 2020 2020 2020 2020 6051  s.            `Q
-00001c00: 7565 7279 603a 2041 2071 7565 7279 206f  uery`: A query o
-00001c10: 626a 6563 7420 7769 7468 2074 6865 2073  bject with the s
-00001c20: 656c 6563 7465 6420 6665 6174 7572 6573  elected features
-00001c30: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
-00001c40: 6772 6f75 702e 0a20 2020 2020 2020 2022  group..        "
-00001c50: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00001c60: 6e20 7175 6572 792e 5175 6572 7928 0a20  n query.Query(. 
-00001c70: 2020 2020 2020 2020 2020 206c 6566 745f             left_
-00001c80: 6665 6174 7572 655f 6772 6f75 703d 7365  feature_group=se
-00001c90: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-00001ca0: 6c65 6674 5f66 6561 7475 7265 733d 6665  left_features=fe
-00001cb0: 6174 7572 6573 2c0a 2020 2020 2020 2020  atures,.        
-00001cc0: 2020 2020 6665 6174 7572 655f 7374 6f72      feature_stor
-00001cd0: 655f 6e61 6d65 3d73 656c 662e 5f66 6561  e_name=self._fea
-00001ce0: 7475 7265 5f73 746f 7265 5f6e 616d 652c  ture_store_name,
-00001cf0: 0a20 2020 2020 2020 2020 2020 2066 6561  .            fea
-00001d00: 7475 7265 5f73 746f 7265 5f69 643d 7365  ture_store_id=se
-00001d10: 6c66 2e5f 6665 6174 7572 655f 7374 6f72  lf._feature_stor
-00001d20: 655f 6964 2c0a 2020 2020 2020 2020 290a  e_id,.        ).
-00001d30: 0a20 2020 2064 6566 2073 656c 6563 745f  .    def select_
-00001d40: 6578 6365 7074 2873 656c 662c 2066 6561  except(self, fea
-00001d50: 7475 7265 733a 204f 7074 696f 6e61 6c5b  tures: Optional[
-00001d60: 4c69 7374 5b55 6e69 6f6e 5b73 7472 2c20  List[Union[str, 
-00001d70: 6665 6174 7572 652e 4665 6174 7572 655d  feature.Feature]
-00001d80: 5d5d 203d 205b 5d29 3a0a 2020 2020 2020  ]] = []):.      
-00001d90: 2020 2222 2253 656c 6563 7420 616c 6c20    """Select all 
-00001da0: 6665 6174 7572 6573 2069 6e63 6c75 6469  features includi
-00001db0: 6e67 2070 7269 6d61 7279 206b 6579 2061  ng primary key a
-00001dc0: 6e64 2065 7665 6e74 2074 696d 6520 6665  nd event time fe
-00001dd0: 6174 7572 650a 2020 2020 2020 2020 6f66  ature.        of
-00001de0: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
-00001df0: 7570 2065 7863 6570 7420 7072 6f76 6964  up except provid
-00001e00: 6564 2060 6665 6174 7572 6573 6020 616e  ed `features` an
-00001e10: 6420 7265 7475 726e 2061 2071 7565 7279  d return a query
-00001e20: 206f 626a 6563 742e 0a0a 2020 2020 2020   object...      
-00001e30: 2020 5468 6520 7175 6572 7920 6361 6e20    The query can 
-00001e40: 6265 2075 7365 6420 746f 2063 6f6e 7374  be used to const
-00001e50: 7275 6374 206a 6f69 6e73 206f 6620 6665  ruct joins of fe
-00001e60: 6174 7572 6520 6772 6f75 7073 206f 7220  ature groups or 
-00001e70: 6372 6561 7465 2061 0a20 2020 2020 2020  create a.       
-00001e80: 2066 6561 7475 7265 2076 6965 7720 7769   feature view wi
-00001e90: 7468 2061 2073 7562 7365 7420 6f66 2066  th a subset of f
-00001ea0: 6561 7475 7265 7320 6f66 2074 6865 2066  eatures of the f
-00001eb0: 6561 7475 7265 2067 726f 7570 2e0a 0a20  eature group... 
-00001ec0: 2020 2020 2020 2021 2121 2065 7861 6d70         !!! examp
-00001ed0: 6c65 0a20 2020 2020 2020 2020 2020 2060  le.            `
-00001ee0: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
-00001ef0: 2020 2020 2023 2063 6f6e 6e65 6374 2074       # connect t
-00001f00: 6f20 7468 6520 4665 6174 7572 6520 5374  o the Feature St
-00001f10: 6f72 650a 2020 2020 2020 2020 2020 2020  ore.            
-00001f20: 6673 203d 202e 2e2e 0a0a 2020 2020 2020  fs = .....      
-00001f30: 2020 2020 2020 2320 6765 7420 7468 6520        # get the 
-00001f40: 4665 6174 7572 6520 4772 6f75 7020 696e  Feature Group in
-00001f50: 7374 616e 6365 0a20 2020 2020 2020 2020  stance.         
-00001f60: 2020 2066 726f 6d20 6873 6673 2e66 6561     from hsfs.fea
-00001f70: 7475 7265 2069 6d70 6f72 7420 4665 6174  ture import Feat
-00001f80: 7572 650a 2020 2020 2020 2020 2020 2020  ure.            
-00001f90: 6667 203d 2066 732e 6372 6561 7465 5f66  fg = fs.create_f
-00001fa0: 6561 7475 7265 5f67 726f 7570 280a 2020  eature_group(.  
-00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fc0: 2020 2266 6722 2c0a 2020 2020 2020 2020    "fg",.        
-00001fd0: 2020 2020 2020 2020 2020 2020 6665 6174              feat
-00001fe0: 7572 6573 3d5b 0a20 2020 2020 2020 2020  ures=[.         
-00001ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002000: 2020 2046 6561 7475 7265 2822 6964 222c     Feature("id",
-00002010: 2074 7970 653d 2273 7472 696e 6722 292c   type="string"),
-00002020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002030: 2020 2020 2020 2020 2020 2020 2046 6561               Fea
-00002040: 7475 7265 2822 7473 222c 2074 7970 653d  ture("ts", type=
-00002050: 2262 6967 696e 7422 292c 0a20 2020 2020  "bigint"),.     
-00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002070: 2020 2020 2020 2046 6561 7475 7265 2822         Feature("
-00002080: 6631 222c 2074 7970 653d 2264 6174 6522  f1", type="date"
-00002090: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000020a0: 2020 2020 2020 2020 2020 2020 2020 2046                 F
-000020b0: 6561 7475 7265 2822 6632 222c 2074 7970  eature("f2", typ
-000020c0: 653d 2264 6f75 626c 6522 290a 2020 2020  e="double").    
-000020d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020e0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-000020f0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00002100: 7269 6d61 7279 5f6b 6579 3d5b 2269 6422  rimary_key=["id"
-00002110: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00002120: 2020 2020 2020 2065 7665 6e74 5f74 696d         event_tim
-00002130: 653d 2274 7322 290a 0a20 2020 2020 2020  e="ts")..       
-00002140: 2020 2020 2023 2063 6f6e 7374 7275 6374       # construct
-00002150: 2071 7565 7279 0a20 2020 2020 2020 2020   query.         
-00002160: 2020 2071 7565 7279 203d 2066 672e 7365     query = fg.se
-00002170: 6c65 6374 5f65 7863 6570 7428 5b22 7473  lect_except(["ts
-00002180: 222c 2022 6631 225d 290a 2020 2020 2020  ", "f1"]).      
-00002190: 2020 2020 2020 7175 6572 792e 6665 6174        query.feat
-000021a0: 7572 6573 0a20 2020 2020 2020 2020 2020  ures.           
-000021b0: 2023 205b 4665 6174 7572 6528 2769 6427   # [Feature('id'
-000021c0: 2c20 2e2e 2e29 2c20 4665 6174 7572 6528  , ...), Feature(
-000021d0: 2766 3127 2c20 2e2e 2e29 5d0a 2020 2020  'f1', ...)].    
-000021e0: 2020 2020 2020 2020 6060 600a 0a20 2020          ```..   
-000021f0: 2020 2020 2023 2041 7267 756d 656e 7473       # Arguments
-00002200: 0a20 2020 2020 2020 2020 2020 2066 6561  .            fea
-00002210: 7475 7265 733a 2041 206c 6973 7420 6f66  tures: A list of
-00002220: 2060 4665 6174 7572 6560 206f 626a 6563   `Feature` objec
-00002230: 7473 206f 7220 6665 6174 7572 6520 6e61  ts or feature na
-00002240: 6d65 7320 6173 0a20 2020 2020 2020 2020  mes as.         
-00002250: 2020 2020 2020 2073 7472 696e 6773 2074         strings t
-00002260: 6f20 6265 2065 7863 6c75 6465 6420 6672  o be excluded fr
-00002270: 6f6d 2074 6865 2073 656c 6563 7469 6f6e  om the selection
-00002280: 2e20 4465 6661 756c 7473 2074 6f20 5b5d  . Defaults to []
-00002290: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000022a0: 2020 7365 6c65 6374 696e 6720 616c 6c20    selecting all 
-000022b0: 6665 6174 7572 6573 2e0a 0a20 2020 2020  features...     
-000022c0: 2020 2023 2052 6574 7572 6e73 0a20 2020     # Returns.   
-000022d0: 2020 2020 2020 2020 2060 5175 6572 7960           `Query`
-000022e0: 3a20 4120 7175 6572 7920 6f62 6a65 6374  : A query object
-000022f0: 2077 6974 6820 7468 6520 7365 6c65 6374   with the select
-00002300: 6564 2066 6561 7475 7265 7320 6f66 2074  ed features of t
-00002310: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
-00002320: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00002330: 2020 2020 2020 6966 2066 6561 7475 7265        if feature
-00002340: 733a 0a20 2020 2020 2020 2020 2020 2065  s:.            e
-00002350: 7863 6570 745f 6665 6174 7572 6573 203d  xcept_features =
-00002360: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00002370: 2020 2066 2e6e 616d 6520 6966 2069 7369     f.name if isi
-00002380: 6e73 7461 6e63 6528 662c 2066 6561 7475  nstance(f, featu
-00002390: 7265 2e46 6561 7475 7265 2920 656c 7365  re.Feature) else
-000023a0: 2066 2066 6f72 2066 2069 6e20 6665 6174   f for f in feat
-000023b0: 7572 6573 0a20 2020 2020 2020 2020 2020  ures.           
-000023c0: 205d 0a20 2020 2020 2020 2020 2020 2072   ].            r
-000023d0: 6574 7572 6e20 7175 6572 792e 5175 6572  eturn query.Quer
-000023e0: 7928 0a20 2020 2020 2020 2020 2020 2020  y(.             
-000023f0: 2020 206c 6566 745f 6665 6174 7572 655f     left_feature_
-00002400: 6772 6f75 703d 7365 6c66 2c0a 2020 2020  group=self,.    
-00002410: 2020 2020 2020 2020 2020 2020 6c65 6674              left
-00002420: 5f66 6561 7475 7265 733d 5b0a 2020 2020  _features=[.    
-00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002440: 6620 666f 7220 6620 696e 2073 656c 662e  f for f in self.
-00002450: 5f66 6561 7475 7265 7320 6966 2066 2e6e  _features if f.n
-00002460: 616d 6520 6e6f 7420 696e 2065 7863 6570  ame not in excep
-00002470: 745f 6665 6174 7572 6573 0a20 2020 2020  t_features.     
-00002480: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
-00002490: 2020 2020 2020 2020 2020 2020 2020 6665                fe
-000024a0: 6174 7572 655f 7374 6f72 655f 6e61 6d65  ature_store_name
-000024b0: 3d73 656c 662e 5f66 6561 7475 7265 5f73  =self._feature_s
-000024c0: 746f 7265 5f6e 616d 652c 0a20 2020 2020  tore_name,.     
-000024d0: 2020 2020 2020 2020 2020 2066 6561 7475             featu
-000024e0: 7265 5f73 746f 7265 5f69 643d 7365 6c66  re_store_id=self
-000024f0: 2e5f 6665 6174 7572 655f 7374 6f72 655f  ._feature_store_
-00002500: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00002510: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00002520: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002530: 726e 2073 656c 662e 7365 6c65 6374 5f61  rn self.select_a
-00002540: 6c6c 2829 0a0a 2020 2020 6465 6620 6669  ll()..    def fi
-00002550: 6c74 6572 2873 656c 662c 2066 3a20 556e  lter(self, f: Un
-00002560: 696f 6e5b 6669 6c74 6572 2e46 696c 7465  ion[filter.Filte
-00002570: 722c 2066 696c 7465 722e 4c6f 6769 635d  r, filter.Logic]
-00002580: 293a 0a20 2020 2020 2020 2022 2222 4170  ):.        """Ap
-00002590: 706c 7920 6669 6c74 6572 2074 6f20 7468  ply filter to th
-000025a0: 6520 6665 6174 7572 6520 6772 6f75 702e  e feature group.
-000025b0: 0a0a 2020 2020 2020 2020 5365 6c65 6374  ..        Select
-000025c0: 7320 616c 6c20 6665 6174 7572 6573 2061  s all features a
-000025d0: 6e64 2072 6574 7572 6e73 2074 6865 2072  nd returns the r
-000025e0: 6573 756c 7469 6e67 2060 5175 6572 7960  esulting `Query`
-000025f0: 2077 6974 6820 7468 6520 6170 706c 6965   with the applie
-00002600: 6420 6669 6c74 6572 2e0a 2020 2020 2020  d filter..      
-00002610: 2020 2121 2120 6578 616d 706c 650a 2020    !!! example.  
-00002620: 2020 2020 2020 2020 2020 6060 6070 7974            ```pyt
-00002630: 686f 6e0a 2020 2020 2020 2020 2020 2020  hon.            
-00002640: 6672 6f6d 2068 7366 732e 6665 6174 7572  from hsfs.featur
-00002650: 6520 696d 706f 7274 2046 6561 7475 7265  e import Feature
-00002660: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00002670: 636f 6e6e 6563 7420 746f 2074 6865 2046  connect to the F
-00002680: 6561 7475 7265 2053 746f 7265 0a20 2020  eature Store.   
-00002690: 2020 2020 2020 2020 2066 7320 3d20 2e2e           fs = ..
-000026a0: 2e0a 0a20 2020 2020 2020 2020 2020 2023  ...            #
-000026b0: 2067 6574 2074 6865 2046 6561 7475 7265   get the Feature
-000026c0: 2047 726f 7570 2069 6e73 7461 6e63 650a   Group instance.
-000026d0: 2020 2020 2020 2020 2020 2020 6667 203d              fg =
-000026e0: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
-000026f0: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
-00002700: 2e2e 2e29 0a0a 2020 2020 2020 2020 2020  ...)..          
-00002710: 2020 6667 2e66 696c 7465 7228 4665 6174    fg.filter(Feat
-00002720: 7572 6528 2277 6565 6b6c 795f 7361 6c65  ure("weekly_sale
-00002730: 7322 2920 3e20 3130 3030 290a 2020 2020  s") > 1000).    
-00002740: 2020 2020 2020 2020 6060 600a 0a20 2020          ```..   
-00002750: 2020 2020 2049 6620 796f 7520 6172 6520       If you are 
-00002760: 706c 616e 6e69 6e67 2074 6f20 6a6f 696e  planning to join
-00002770: 2074 6865 2066 696c 7465 7265 6420 6665   the filtered fe
-00002780: 6174 7572 6520 6772 6f75 7020 6c61 7465  ature group late
-00002790: 7220 6f6e 2077 6974 6820 616e 6f74 6865  r on with anothe
-000027a0: 720a 2020 2020 2020 2020 6665 6174 7572  r.        featur
-000027b0: 6520 6772 6f75 702c 206d 616b 6520 7375  e group, make su
-000027c0: 7265 2074 6f20 7365 6c65 6374 2074 6865  re to select the
-000027d0: 2066 696c 7465 7265 6420 6665 6174 7572   filtered featur
-000027e0: 6520 6578 706c 6963 6974 6c79 2066 726f  e explicitly fro
-000027f0: 6d20 7468 650a 2020 2020 2020 2020 7265  m the.        re
-00002800: 7370 6563 7469 7665 2066 6561 7475 7265  spective feature
-00002810: 2067 726f 7570 3a0a 2020 2020 2020 2020   group:.        
-00002820: 2121 2120 6578 616d 706c 650a 2020 2020  !!! example.    
-00002830: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-00002840: 6e0a 2020 2020 2020 2020 2020 2020 6667  n.            fg
-00002850: 2e66 696c 7465 7228 6667 2e66 6561 7475  .filter(fg.featu
-00002860: 7265 3120 3d3d 2031 292e 7368 6f77 2831  re1 == 1).show(1
-00002870: 3029 0a20 2020 2020 2020 2020 2020 2060  0).            `
-00002880: 6060 0a0a 2020 2020 2020 2020 436f 6d70  ``..        Comp
-00002890: 6f73 6974 6520 6669 6c74 6572 7320 7265  osite filters re
-000028a0: 7175 6972 6520 7061 7265 6e74 6865 7369  quire parenthesi
-000028b0: 733a 0a20 2020 2020 2020 2021 2121 2065  s:.        !!! e
-000028c0: 7861 6d70 6c65 0a20 2020 2020 2020 2020  xample.         
-000028d0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-000028e0: 2020 2020 2020 2020 2066 672e 6669 6c74           fg.filt
-000028f0: 6572 2828 6667 2e66 6561 7475 7265 3120  er((fg.feature1 
-00002900: 3d3d 2031 2920 7c20 2866 672e 6665 6174  == 1) | (fg.feat
-00002910: 7572 6532 203e 3d20 3229 290a 2020 2020  ure2 >= 2)).    
-00002920: 2020 2020 2020 2020 6060 600a 0a20 2020          ```..   
-00002930: 2020 2020 2023 2041 7267 756d 656e 7473       # Arguments
-00002940: 0a20 2020 2020 2020 2020 2020 2066 3a20  .            f: 
-00002950: 4669 6c74 6572 206f 626a 6563 742e 0a0a  Filter object...
-00002960: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
-00002970: 730a 2020 2020 2020 2020 2020 2020 6051  s.            `Q
-00002980: 7565 7279 602e 2054 6865 2071 7565 7279  uery`. The query
-00002990: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
-000029a0: 2061 7070 6c69 6564 2066 696c 7465 722e   applied filter.
-000029b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000029c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000029d0: 2e73 656c 6563 745f 616c 6c28 292e 6669  .select_all().fi
-000029e0: 6c74 6572 2866 290a 0a20 2020 2064 6566  lter(f)..    def
-000029f0: 2061 6464 5f74 6167 2873 656c 662c 206e   add_tag(self, n
-00002a00: 616d 653a 2073 7472 2c20 7661 6c75 6529  ame: str, value)
-00002a10: 3a0a 2020 2020 2020 2020 2222 2241 7474  :.        """Att
-00002a20: 6163 6820 6120 7461 6720 746f 2061 2066  ach a tag to a f
-00002a30: 6561 7475 7265 2067 726f 7570 2e0a 0a20  eature group... 
-00002a40: 2020 2020 2020 2041 2074 6167 2063 6f6e         A tag con
-00002a50: 7369 7374 7320 6f66 2061 203c 6e61 6d65  sists of a <name
-00002a60: 2c76 616c 7565 3e20 7061 6972 2e20 5461  ,value> pair. Ta
-00002a70: 6720 6e61 6d65 7320 6172 6520 756e 6971  g names are uniq
-00002a80: 7565 2069 6465 6e74 6966 6965 7273 2061  ue identifiers a
-00002a90: 6372 6f73 7320 7468 6520 7768 6f6c 6520  cross the whole 
-00002aa0: 636c 7573 7465 722e 0a20 2020 2020 2020  cluster..       
-00002ab0: 2054 6865 2076 616c 7565 206f 6620 6120   The value of a 
-00002ac0: 7461 6720 6361 6e20 6265 2061 6e79 2076  tag can be any v
-00002ad0: 616c 6964 206a 736f 6e20 2d20 7072 696d  alid json - prim
-00002ae0: 6974 6976 6573 2c20 6172 7261 7973 206f  itives, arrays o
-00002af0: 7220 6a73 6f6e 206f 626a 6563 7473 2e0a  r json objects..
-00002b00: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
-00002b10: 6d70 6c65 0a20 2020 2020 2020 2020 2020  mple.           
-00002b20: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
-00002b30: 2020 2020 2020 2023 2063 6f6e 6e65 6374         # connect
-00002b40: 2074 6f20 7468 6520 4665 6174 7572 6520   to the Feature 
-00002b50: 5374 6f72 650a 2020 2020 2020 2020 2020  Store.          
-00002b60: 2020 6673 203d 202e 2e2e 0a0a 2020 2020    fs = .....    
-00002b70: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
-00002b80: 6520 4665 6174 7572 6520 4772 6f75 7020  e Feature Group 
-00002b90: 696e 7374 616e 6365 0a20 2020 2020 2020  instance.       
-00002ba0: 2020 2020 2066 6720 3d20 6673 2e67 6574       fg = fs.get
-00002bb0: 5f6f 725f 6372 6561 7465 5f66 6561 7475  _or_create_featu
-00002bc0: 7265 5f67 726f 7570 282e 2e2e 290a 0a20  re_group(...).. 
-00002bd0: 2020 2020 2020 2020 2020 2066 672e 6164             fg.ad
-00002be0: 645f 7461 6728 6e61 6d65 3d22 6578 616d  d_tag(name="exam
-00002bf0: 706c 655f 7461 6722 2c20 7661 6c75 653d  ple_tag", value=
-00002c00: 2234 3222 290a 2020 2020 2020 2020 2020  "42").          
-00002c10: 2020 6060 600a 0a20 2020 2020 2020 2023    ```..        #
-00002c20: 2041 7267 756d 656e 7473 0a20 2020 2020   Arguments.     
-00002c30: 2020 2020 2020 206e 616d 653a 204e 616d         name: Nam
-00002c40: 6520 6f66 2074 6865 2074 6167 2074 6f20  e of the tag to 
-00002c50: 6265 2061 6464 6564 2e0a 2020 2020 2020  be added..      
-00002c60: 2020 2020 2020 7661 6c75 653a 2056 616c        value: Val
-00002c70: 7565 206f 6620 7468 6520 7461 6720 746f  ue of the tag to
-00002c80: 2062 6520 6164 6465 642e 0a0a 2020 2020   be added...    
-00002c90: 2020 2020 2320 5261 6973 6573 0a20 2020      # Raises.   
-00002ca0: 2020 2020 2020 2020 2060 6873 6673 2e63           `hsfs.c
-00002cb0: 6c69 656e 742e 6578 6365 7074 696f 6e73  lient.exceptions
-00002cc0: 2e52 6573 7441 5049 4572 726f 7260 2069  .RestAPIError` i
-00002cd0: 6e20 6361 7365 2074 6865 2062 6163 6b65  n case the backe
-00002ce0: 6e64 2066 6169 6c73 2074 6f20 6164 6420  nd fails to add 
-00002cf0: 7468 6520 7461 672e 0a20 2020 2020 2020  the tag..       
-00002d00: 2022 2222 0a0a 2020 2020 2020 2020 7365   """..        se
-00002d10: 6c66 2e5f 6665 6174 7572 655f 6772 6f75  lf._feature_grou
-00002d20: 705f 656e 6769 6e65 2e61 6464 5f74 6167  p_engine.add_tag
-00002d30: 2873 656c 662c 206e 616d 652c 2076 616c  (self, name, val
-00002d40: 7565 290a 0a20 2020 2064 6566 2064 656c  ue)..    def del
-00002d50: 6574 655f 7461 6728 7365 6c66 2c20 6e61  ete_tag(self, na
-00002d60: 6d65 3a20 7374 7229 3a0a 2020 2020 2020  me: str):.      
-00002d70: 2020 2222 2244 656c 6574 6520 6120 7461    """Delete a ta
-00002d80: 6720 6174 7461 6368 6564 2074 6f20 6120  g attached to a 
-00002d90: 6665 6174 7572 6520 6772 6f75 702e 0a0a  feature group...
-00002da0: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
-00002db0: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
-00002dc0: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-00002dd0: 2020 2020 2020 2320 636f 6e6e 6563 7420        # connect 
-00002de0: 746f 2074 6865 2046 6561 7475 7265 2053  to the Feature S
-00002df0: 746f 7265 0a20 2020 2020 2020 2020 2020  tore.           
-00002e00: 2066 7320 3d20 2e2e 2e0a 0a20 2020 2020   fs = .....     
-00002e10: 2020 2020 2020 2023 2067 6574 2074 6865         # get the
-00002e20: 2046 6561 7475 7265 2047 726f 7570 2069   Feature Group i
-00002e30: 6e73 7461 6e63 650a 2020 2020 2020 2020  nstance.        
-00002e40: 2020 2020 6667 203d 2066 732e 6765 745f      fg = fs.get_
-00002e50: 6f72 5f63 7265 6174 655f 6665 6174 7572  or_create_featur
-00002e60: 655f 6772 6f75 7028 2e2e 2e29 0a0a 2020  e_group(...)..  
-00002e70: 2020 2020 2020 2020 2020 6667 2e64 656c            fg.del
-00002e80: 6574 655f 7461 6728 2265 7861 6d70 6c65  ete_tag("example
-00002e90: 5f74 6167 2229 0a20 2020 2020 2020 2020  _tag").         
-00002ea0: 2020 2060 6060 0a0a 2020 2020 2020 2020     ```..        
-00002eb0: 2320 4172 6775 6d65 6e74 730a 2020 2020  # Arguments.    
-00002ec0: 2020 2020 2020 2020 6e61 6d65 3a20 4e61          name: Na
-00002ed0: 6d65 206f 6620 7468 6520 7461 6720 746f  me of the tag to
-00002ee0: 2062 6520 7265 6d6f 7665 642e 0a0a 2020   be removed...  
-00002ef0: 2020 2020 2020 2320 5261 6973 6573 0a20        # Raises. 
-00002f00: 2020 2020 2020 2020 2020 2060 6873 6673             `hsfs
-00002f10: 2e63 6c69 656e 742e 6578 6365 7074 696f  .client.exceptio
-00002f20: 6e73 2e52 6573 7441 5049 4572 726f 7260  ns.RestAPIError`
-00002f30: 2069 6e20 6361 7365 2074 6865 2062 6163   in case the bac
-00002f40: 6b65 6e64 2066 6169 6c73 2074 6f20 6465  kend fails to de
-00002f50: 6c65 7465 2074 6865 2074 6167 2e0a 2020  lete the tag..  
-00002f60: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00002f70: 2020 7365 6c66 2e5f 6665 6174 7572 655f    self._feature_
-00002f80: 6772 6f75 705f 656e 6769 6e65 2e64 656c  group_engine.del
-00002f90: 6574 655f 7461 6728 7365 6c66 2c20 6e61  ete_tag(self, na
-00002fa0: 6d65 290a 0a20 2020 2064 6566 2067 6574  me)..    def get
-00002fb0: 5f74 6167 2873 656c 662c 206e 616d 653a  _tag(self, name:
-00002fc0: 2073 7472 293a 0a20 2020 2020 2020 2022   str):.        "
-00002fd0: 2222 4765 7420 7468 6520 7461 6773 206f  ""Get the tags o
-00002fe0: 6620 6120 6665 6174 7572 6520 6772 6f75  f a feature grou
-00002ff0: 702e 0a0a 2020 2020 2020 2020 2121 2120  p...        !!! 
-00003000: 6578 616d 706c 650a 2020 2020 2020 2020  example.        
-00003010: 2020 2020 6060 6070 7974 686f 6e0a 2020      ```python.  
-00003020: 2020 2020 2020 2020 2020 2320 636f 6e6e            # conn
-00003030: 6563 7420 746f 2074 6865 2046 6561 7475  ect to the Featu
-00003040: 7265 2053 746f 7265 0a20 2020 2020 2020  re Store.       
-00003050: 2020 2020 2066 7320 3d20 2e2e 2e0a 0a20       fs = ..... 
-00003060: 2020 2020 2020 2020 2020 2023 2067 6574             # get
-00003070: 2074 6865 2046 6561 7475 7265 2047 726f   the Feature Gro
-00003080: 7570 2069 6e73 7461 6e63 650a 2020 2020  up instance.    
-00003090: 2020 2020 2020 2020 6667 203d 2066 732e          fg = fs.
-000030a0: 6765 745f 6f72 5f63 7265 6174 655f 6665  get_or_create_fe
-000030b0: 6174 7572 655f 6772 6f75 7028 2e2e 2e29  ature_group(...)
-000030c0: 0a0a 2020 2020 2020 2020 2020 2020 6667  ..            fg
-000030d0: 5f74 6167 5f76 616c 7565 203d 2066 672e  _tag_value = fg.
-000030e0: 6765 745f 7461 6728 2265 7861 6d70 6c65  get_tag("example
-000030f0: 5f74 6167 2229 0a20 2020 2020 2020 2020  _tag").         
-00003100: 2020 2060 6060 0a0a 2020 2020 2020 2020     ```..        
-00003110: 2320 4172 6775 6d65 6e74 730a 2020 2020  # Arguments.    
-00003120: 2020 2020 2020 2020 6e61 6d65 3a20 4e61          name: Na
-00003130: 6d65 206f 6620 7468 6520 7461 6720 746f  me of the tag to
-00003140: 2067 6574 2e0a 0a20 2020 2020 2020 2023   get...        #
-00003150: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00003160: 2020 2020 2074 6167 2076 616c 7565 0a0a       tag value..
-00003170: 2020 2020 2020 2020 2320 5261 6973 6573          # Raises
-00003180: 0a20 2020 2020 2020 2020 2020 2060 6873  .            `hs
-00003190: 6673 2e63 6c69 656e 742e 6578 6365 7074  fs.client.except
-000031a0: 696f 6e73 2e52 6573 7441 5049 4572 726f  ions.RestAPIErro
-000031b0: 7260 2069 6e20 6361 7365 2074 6865 2062  r` in case the b
-000031c0: 6163 6b65 6e64 2066 6169 6c73 2074 6f20  ackend fails to 
-000031d0: 7265 7472 6965 7665 2074 6865 2074 6167  retrieve the tag
-000031e0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000031f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00003200: 662e 5f66 6561 7475 7265 5f67 726f 7570  f._feature_group
-00003210: 5f65 6e67 696e 652e 6765 745f 7461 6728  _engine.get_tag(
-00003220: 7365 6c66 2c20 6e61 6d65 290a 0a20 2020  self, name)..   
-00003230: 2064 6566 2067 6574 5f74 6167 7328 7365   def get_tags(se
-00003240: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00003250: 5265 7472 6965 7665 7320 616c 6c20 7461  Retrieves all ta
-00003260: 6773 2061 7474 6163 6865 6420 746f 2061  gs attached to a
-00003270: 2066 6561 7475 7265 2067 726f 7570 2e0a   feature group..
-00003280: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
-00003290: 6e73 0a20 2020 2020 2020 2020 2020 2060  ns.            `
-000032a0: 4469 6374 5b73 7472 2c20 6f62 6a5d 6020  Dict[str, obj]` 
-000032b0: 6f66 2074 6167 732e 0a0a 2020 2020 2020  of tags...      
-000032c0: 2020 2320 5261 6973 6573 0a20 2020 2020    # Raises.     
-000032d0: 2020 2020 2020 2060 6873 6673 2e63 6c69         `hsfs.cli
-000032e0: 656e 742e 6578 6365 7074 696f 6e73 2e52  ent.exceptions.R
-000032f0: 6573 7441 5049 4572 726f 7260 2069 6e20  estAPIError` in 
-00003300: 6361 7365 2074 6865 2062 6163 6b65 6e64  case the backend
-00003310: 2066 6169 6c73 2074 6f20 7265 7472 6965   fails to retrie
-00003320: 7665 2074 6865 2074 6167 732e 0a20 2020  ve the tags..   
-00003330: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00003340: 2072 6574 7572 6e20 7365 6c66 2e5f 6665   return self._fe
-00003350: 6174 7572 655f 6772 6f75 705f 656e 6769  ature_group_engi
-00003360: 6e65 2e67 6574 5f74 6167 7328 7365 6c66  ne.get_tags(self
-00003370: 290a 0a20 2020 2064 6566 2067 6574 5f70  )..    def get_p
-00003380: 6172 656e 745f 6665 6174 7572 655f 6772  arent_feature_gr
-00003390: 6f75 7073 2873 656c 6629 3a0a 2020 2020  oups(self):.    
-000033a0: 2020 2020 2222 2247 6574 2074 6865 2070      """Get the p
-000033b0: 6172 656e 7473 206f 6620 7468 6973 2066  arents of this f
-000033c0: 6561 7475 7265 2067 726f 7570 2c20 6261  eature group, ba
-000033d0: 7365 6420 6f6e 2065 7870 6c69 6369 7420  sed on explicit 
-000033e0: 7072 6f76 656e 616e 6365 2e0a 2020 2020  provenance..    
-000033f0: 2020 2020 5061 7265 6e74 7320 6172 6520      Parents are 
-00003400: 6665 6174 7572 6520 6772 6f75 7073 206f  feature groups o
-00003410: 7220 6578 7465 726e 616c 2066 6561 7475  r external featu
-00003420: 7265 2067 726f 7570 732e 2054 6865 7365  re groups. These
-00003430: 2066 6561 7475 7265 0a20 2020 2020 2020   feature.       
-00003440: 2067 726f 7570 7320 6361 6e20 6265 2061   groups can be a
-00003450: 6363 6573 7369 626c 652c 2064 656c 6574  ccessible, delet
-00003460: 6564 206f 7220 696e 6163 6365 7373 6962  ed or inaccessib
-00003470: 6c65 2e0a 2020 2020 2020 2020 466f 7220  le..        For 
-00003480: 6465 6c65 7465 6420 616e 6420 696e 6163  deleted and inac
-00003490: 6365 7373 6962 6c65 2066 6561 7475 7265  cessible feature
-000034a0: 2067 726f 7570 732c 206f 6e6c 7920 6120   groups, only a 
-000034b0: 6d69 6e69 6d61 6c20 696e 666f 726d 6174  minimal informat
-000034c0: 696f 6e20 6973 0a20 2020 2020 2020 2072  ion is.        r
-000034d0: 6574 7572 6e65 642e 0a0a 2020 2020 2020  eturned...      
-000034e0: 2020 2320 5265 7475 726e 730a 2020 2020    # Returns.    
-000034f0: 2020 2020 2020 2020 6050 726f 7665 6e61          `Provena
-00003500: 6e63 654c 696e 6b73 603a 204f 626a 6563  nceLinks`: Objec
-00003510: 7420 636f 6e74 6169 6e69 6e67 2074 6865  t containing the
-00003520: 2073 6563 7469 6f6e 206f 6620 7072 6f76   section of prov
-00003530: 656e 616e 6365 2067 7261 7068 2072 6571  enance graph req
-00003540: 7565 7374 6564 2e0a 0a20 2020 2020 2020  uested...       
-00003550: 2023 2052 6169 7365 730a 2020 2020 2020   # Raises.      
-00003560: 2020 2020 2020 6068 7366 732e 636c 6965        `hsfs.clie
-00003570: 6e74 2e65 7863 6570 7469 6f6e 732e 5265  nt.exceptions.Re
-00003580: 7374 4150 4945 7272 6f72 602e 0a20 2020  stAPIError`..   
-00003590: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000035a0: 2072 6574 7572 6e20 7365 6c66 2e5f 6665   return self._fe
-000035b0: 6174 7572 655f 6772 6f75 705f 656e 6769  ature_group_engi
-000035c0: 6e65 2e67 6574 5f70 6172 656e 745f 6665  ne.get_parent_fe
-000035d0: 6174 7572 655f 6772 6f75 7073 2873 656c  ature_groups(sel
-000035e0: 6629 0a0a 2020 2020 6465 6620 6765 745f  f)..    def get_
-000035f0: 6765 6e65 7261 7465 645f 6665 6174 7572  generated_featur
-00003600: 655f 7669 6577 7328 7365 6c66 293a 0a20  e_views(self):. 
-00003610: 2020 2020 2020 2022 2222 4765 7420 7468         """Get th
-00003620: 6520 6765 6e65 7261 7465 6420 6665 6174  e generated feat
-00003630: 7572 6520 7669 6577 2075 7369 6e67 2074  ure view using t
-00003640: 6869 7320 6665 6174 7572 6520 6772 6f75  his feature grou
-00003650: 702c 2062 6173 6564 206f 6e20 6578 706c  p, based on expl
-00003660: 6963 6974 0a20 2020 2020 2020 2070 726f  icit.        pro
-00003670: 7665 6e61 6e63 652e 2054 6865 7365 2066  venance. These f
-00003680: 6561 7475 7265 2076 6965 7773 2063 616e  eature views can
-00003690: 2062 6520 6163 6365 7373 6962 6c65 206f   be accessible o
-000036a0: 7220 696e 6163 6365 7373 6962 6c65 2e20  r inaccessible. 
-000036b0: 4578 706c 6963 6974 0a20 2020 2020 2020  Explicit.       
-000036c0: 2070 726f 7665 6e61 6e63 6520 646f 6573   provenance does
-000036d0: 206e 6f74 2074 7261 636b 2064 656c 6574   not track delet
-000036e0: 6564 2067 656e 6572 6174 6564 2066 6561  ed generated fea
-000036f0: 7475 7265 2076 6965 7720 6c69 6e6b 732c  ture view links,
-00003700: 2073 6f20 6465 6c65 7465 640a 2020 2020   so deleted.    
-00003710: 2020 2020 7769 6c6c 2061 6c77 6179 7320      will always 
-00003720: 6265 2065 6d70 7479 2e0a 2020 2020 2020  be empty..      
-00003730: 2020 466f 7220 696e 6163 6365 7373 6962    For inaccessib
-00003740: 6c65 2066 6561 7475 7265 2076 6965 7773  le feature views
-00003750: 2c20 6f6e 6c79 2061 206d 696e 696d 616c  , only a minimal
-00003760: 2069 6e66 6f72 6d61 7469 6f6e 2069 7320   information is 
-00003770: 7265 7475 726e 6564 2e0a 0a20 2020 2020  returned...     
-00003780: 2020 2023 2052 6574 7572 6e73 0a20 2020     # Returns.   
-00003790: 2020 2020 2020 2020 2060 5072 6f76 656e           `Proven
-000037a0: 616e 6365 4c69 6e6b 7360 3a20 4f62 6a65  anceLinks`: Obje
-000037b0: 6374 2063 6f6e 7461 696e 696e 6720 7468  ct containing th
-000037c0: 6520 7365 6374 696f 6e20 6f66 2070 726f  e section of pro
-000037d0: 7665 6e61 6e63 6520 6772 6170 6820 7265  venance graph re
-000037e0: 7175 6573 7465 642e 0a0a 2020 2020 2020  quested...      
-000037f0: 2020 2320 5261 6973 6573 0a20 2020 2020    # Raises.     
-00003800: 2020 2020 2020 2060 6873 6673 2e63 6c69         `hsfs.cli
-00003810: 656e 742e 6578 6365 7074 696f 6e73 2e52  ent.exceptions.R
-00003820: 6573 7441 5049 4572 726f 7260 2e0a 2020  estAPIError`..  
-00003830: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00003840: 2020 7265 7475 726e 2073 656c 662e 5f66    return self._f
-00003850: 6561 7475 7265 5f67 726f 7570 5f65 6e67  eature_group_eng
-00003860: 696e 652e 6765 745f 6765 6e65 7261 7465  ine.get_generate
-00003870: 645f 6665 6174 7572 655f 7669 6577 7328  d_feature_views(
-00003880: 7365 6c66 290a 0a20 2020 2064 6566 2067  self)..    def g
-00003890: 6574 5f67 656e 6572 6174 6564 5f66 6561  et_generated_fea
-000038a0: 7475 7265 5f67 726f 7570 7328 7365 6c66  ture_groups(self
-000038b0: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
-000038c0: 7420 7468 6520 6765 6e65 7261 7465 6420  t the generated 
-000038d0: 6665 6174 7572 6520 6772 6f75 7073 2075  feature groups u
-000038e0: 7369 6e67 2074 6869 7320 6665 6174 7572  sing this featur
-000038f0: 6520 6772 6f75 702c 2062 6173 6564 206f  e group, based o
-00003900: 6e20 6578 706c 6963 6974 0a20 2020 2020  n explicit.     
-00003910: 2020 2070 726f 7665 6e61 6e63 652e 2054     provenance. T
-00003920: 6865 7365 2066 6561 7475 7265 2067 726f  hese feature gro
-00003930: 7570 7320 6361 6e20 6265 2061 6363 6573  ups can be acces
-00003940: 7369 626c 6520 6f72 2069 6e61 6363 6573  sible or inacces
-00003950: 7369 626c 652e 2045 7870 6c69 6369 740a  sible. Explicit.
-00003960: 2020 2020 2020 2020 7072 6f76 656e 616e          provenan
-00003970: 6365 2064 6f65 7320 6e6f 7420 7472 6163  ce does not trac
-00003980: 6b20 6465 6c65 7465 6420 6765 6e65 7261  k deleted genera
-00003990: 7465 6420 6665 6174 7572 6520 6772 6f75  ted feature grou
-000039a0: 7020 6c69 6e6b 732c 2073 6f20 6465 6c65  p links, so dele
-000039b0: 7465 640a 2020 2020 2020 2020 7769 6c6c  ted.        will
-000039c0: 2061 6c77 6179 7320 6265 2065 6d70 7479   always be empty
-000039d0: 2e0a 2020 2020 2020 2020 466f 7220 696e  ..        For in
-000039e0: 6163 6365 7373 6962 6c65 2066 6561 7475  accessible featu
-000039f0: 7265 2067 726f 7570 732c 206f 6e6c 7920  re groups, only 
-00003a00: 6120 6d69 6e69 6d61 6c20 696e 666f 726d  a minimal inform
-00003a10: 6174 696f 6e20 6973 2072 6574 7572 6e65  ation is returne
-00003a20: 642e 0a0a 2020 2020 2020 2020 2320 5265  d...        # Re
-00003a30: 7475 726e 730a 2020 2020 2020 2020 2020  turns.          
-00003a40: 2020 6050 726f 7665 6e61 6e63 654c 696e    `ProvenanceLin
-00003a50: 6b73 603a 204f 626a 6563 7420 636f 6e74  ks`: Object cont
-00003a60: 6169 6e69 6e67 2074 6865 2073 6563 7469  aining the secti
-00003a70: 6f6e 206f 6620 7072 6f76 656e 616e 6365  on of provenance
-00003a80: 2067 7261 7068 2072 6571 7565 7374 6564   graph requested
-00003a90: 2e0a 0a20 2020 2020 2020 2023 2052 6169  ...        # Rai
-00003aa0: 7365 730a 2020 2020 2020 2020 2020 2020  ses.            
-00003ab0: 6068 7366 732e 636c 6965 6e74 2e65 7863  `hsfs.client.exc
-00003ac0: 6570 7469 6f6e 732e 5265 7374 4150 4945  eptions.RestAPIE
-00003ad0: 7272 6f72 602e 0a20 2020 2020 2020 2022  rror`..        "
-00003ae0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00003af0: 6e20 7365 6c66 2e5f 6665 6174 7572 655f  n self._feature_
-00003b00: 6772 6f75 705f 656e 6769 6e65 2e67 6574  group_engine.get
-00003b10: 5f67 656e 6572 6174 6564 5f66 6561 7475  _generated_featu
-00003b20: 7265 5f67 726f 7570 7328 7365 6c66 290a  re_groups(self).
-00003b30: 0a20 2020 2064 6566 2067 6574 5f66 6561  .    def get_fea
-00003b40: 7475 7265 2873 656c 662c 206e 616d 653a  ture(self, name:
-00003b50: 2073 7472 293a 0a20 2020 2020 2020 2022   str):.        "
-00003b60: 2222 5265 7472 6965 7665 2061 2060 4665  ""Retrieve a `Fe
-00003b70: 6174 7572 6560 206f 626a 6563 7420 6672  ature` object fr
-00003b80: 6f6d 2074 6865 2073 6368 656d 6120 6f66  om the schema of
-00003b90: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
-00003ba0: 7570 2e0a 0a20 2020 2020 2020 2054 6865  up...        The
-00003bb0: 7265 2061 7265 2073 6576 6572 616c 2077  re are several w
-00003bc0: 6179 7320 746f 2061 6363 6573 7320 6665  ays to access fe
-00003bd0: 6174 7572 6573 206f 6620 6120 6665 6174  atures of a feat
-00003be0: 7572 6520 6772 6f75 703a 0a0a 2020 2020  ure group:..    
-00003bf0: 2020 2020 2121 2120 6578 616d 706c 650a      !!! example.
-00003c00: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
-00003c10: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
-00003c20: 2020 2320 636f 6e6e 6563 7420 746f 2074    # connect to t
-00003c30: 6865 2046 6561 7475 7265 2053 746f 7265  he Feature Store
-00003c40: 0a20 2020 2020 2020 2020 2020 2066 7320  .            fs 
-00003c50: 3d20 2e2e 2e0a 0a20 2020 2020 2020 2020  = .....         
-00003c60: 2020 2023 2067 6574 2074 6865 2046 6561     # get the Fea
-00003c70: 7475 7265 2047 726f 7570 2069 6e73 7461  ture Group insta
-00003c80: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
-00003c90: 6667 203d 2066 732e 6765 745f 6f72 5f63  fg = fs.get_or_c
-00003ca0: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
-00003cb0: 6f75 7028 2e2e 2e29 0a0a 2020 2020 2020  oup(...)..      
-00003cc0: 2020 2020 2020 2320 6765 7420 4665 6174        # get Feat
-00003cd0: 7572 6520 696e 7374 616e 7365 0a20 2020  ure instanse.   
-00003ce0: 2020 2020 2020 2020 2066 672e 6665 6174           fg.feat
-00003cf0: 7572 6531 0a20 2020 2020 2020 2020 2020  ure1.           
-00003d00: 2066 675b 2266 6561 7475 7265 3122 5d0a   fg["feature1"].
-00003d10: 2020 2020 2020 2020 2020 2020 6667 2e67              fg.g
-00003d20: 6574 5f66 6561 7475 7265 2822 6665 6174  et_feature("feat
-00003d30: 7572 6531 2229 0a20 2020 2020 2020 2020  ure1").         
-00003d40: 2020 2060 6060 0a0a 2020 2020 2020 2020     ```..        
-00003d50: 2121 2120 6e6f 7465 0a20 2020 2020 2020  !!! note.       
-00003d60: 2020 2020 2041 7474 7269 6275 7465 2061       Attribute a
-00003d70: 6363 6573 7320 746f 2066 6561 7475 7265  ccess to feature
-00003d80: 7320 776f 726b 7320 6f6e 6c79 2066 6f72  s works only for
-00003d90: 206e 6f6e 2d72 6573 6572 7665 6420 6e61   non-reserved na
-00003da0: 6d65 732e 2046 6f72 2065 7861 6d70 6c65  mes. For example
-00003db0: 0a20 2020 2020 2020 2020 2020 2066 6561  .            fea
-00003dc0: 7475 7265 7320 6e61 6d65 6420 6069 6460  tures named `id`
-00003dd0: 206f 7220 606e 616d 6560 2077 696c 6c20   or `name` will 
-00003de0: 6e6f 7420 6265 2061 6363 6573 7369 626c  not be accessibl
-00003df0: 6520 7669 6120 6066 672e 6e61 6d65 602c  e via `fg.name`,
-00003e00: 2069 6e73 7465 6164 0a20 2020 2020 2020   instead.       
-00003e10: 2020 2020 2074 6869 7320 7769 6c6c 2072       this will r
-00003e20: 6574 7572 6e20 7468 6520 6e61 6d65 206f  eturn the name o
-00003e30: 6620 7468 6520 6665 6174 7572 6520 6772  f the feature gr
-00003e40: 6f75 7020 6974 7365 6c66 2e20 4661 6c6c  oup itself. Fall
-00003e50: 2062 6163 6b20 6f6e 2075 7369 6e67 0a20   back on using. 
-00003e60: 2020 2020 2020 2020 2020 2074 6865 2060             the `
-00003e70: 6765 745f 6665 6174 7572 6560 206d 6574  get_feature` met
-00003e80: 686f 642e 0a0a 2020 2020 2020 2020 2320  hod...        # 
-00003e90: 4172 6775 6d65 6e74 733a 0a20 2020 2020  Arguments:.     
-00003ea0: 2020 2020 2020 206e 616d 653a 2054 6865         name: The
-00003eb0: 206e 616d 6520 6f66 2074 6865 2066 6561   name of the fea
-00003ec0: 7475 7265 2074 6f20 7265 7472 6965 7665  ture to retrieve
-00003ed0: 0a0a 2020 2020 2020 2020 2320 5265 7475  ..        # Retu
-00003ee0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00003ef0: 2046 6561 7475 7265 3a20 5468 6520 6665   Feature: The fe
-00003f00: 6174 7572 6520 6f62 6a65 6374 0a0a 2020  ature object..  
-00003f10: 2020 2020 2020 2320 5261 6973 6573 0a20        # Raises. 
-00003f20: 2020 2020 2020 2020 2020 2060 6873 6673             `hsfs
-00003f30: 2e63 6c69 656e 742e 6578 6365 7074 696f  .client.exceptio
-00003f40: 6e73 2e46 6561 7475 7265 5374 6f72 6545  ns.FeatureStoreE
-00003f50: 7863 6570 7469 6f6e 602e 0a20 2020 2020  xception`..     
-00003f60: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
-00003f70: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00003f80: 7265 7475 726e 2073 656c 662e 5f5f 6765  return self.__ge
-00003f90: 7469 7465 6d5f 5f28 6e61 6d65 290a 2020  titem__(name).  
-00003fa0: 2020 2020 2020 6578 6365 7074 204b 6579        except Key
-00003fb0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-00003fc0: 2020 2072 6169 7365 2046 6561 7475 7265     raise Feature
-00003fd0: 5374 6f72 6545 7863 6570 7469 6f6e 280a  StoreException(.
-00003fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ff0: 6622 2746 6561 7475 7265 4772 6f75 7027  f"'FeatureGroup'
-00004000: 206f 626a 6563 7420 6861 7320 6e6f 2066   object has no f
-00004010: 6561 7475 7265 2063 616c 6c65 6420 277b  eature called '{
-00004020: 6e61 6d65 7d27 2e22 0a20 2020 2020 2020  name}'.".       
-00004030: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-00004040: 7570 6461 7465 5f73 7461 7469 7374 6963  update_statistic
-00004050: 735f 636f 6e66 6967 2873 656c 6629 3a0a  s_config(self):.
-00004060: 2020 2020 2020 2020 2222 2255 7064 6174          """Updat
-00004070: 6520 7468 6520 7374 6174 6973 7469 6373  e the statistics
-00004080: 2063 6f6e 6669 6775 7261 7469 6f6e 206f   configuration o
-00004090: 6620 7468 6520 6665 6174 7572 6520 6772  f the feature gr
-000040a0: 6f75 702e 0a0a 2020 2020 2020 2020 4368  oup...        Ch
-000040b0: 616e 6765 2074 6865 2060 7374 6174 6973  ange the `statis
-000040c0: 7469 6373 5f63 6f6e 6669 6760 206f 626a  tics_config` obj
-000040d0: 6563 7420 616e 6420 7065 7273 6973 7420  ect and persist 
-000040e0: 7468 6520 6368 616e 6765 7320 6279 2063  the changes by c
-000040f0: 616c 6c69 6e67 0a20 2020 2020 2020 2074  alling.        t
-00004100: 6869 7320 6d65 7468 6f64 2e0a 0a20 2020  his method...   
-00004110: 2020 2020 2021 2121 2065 7861 6d70 6c65       !!! example
-00004120: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
-00004130: 7079 7468 6f6e 0a20 2020 2020 2020 2020  python.         
-00004140: 2020 2023 2063 6f6e 6e65 6374 2074 6f20     # connect to 
-00004150: 7468 6520 4665 6174 7572 6520 5374 6f72  the Feature Stor
-00004160: 650a 2020 2020 2020 2020 2020 2020 6673  e.            fs
-00004170: 203d 202e 2e2e 0a0a 2020 2020 2020 2020   = .....        
-00004180: 2020 2020 2320 6765 7420 7468 6520 4665      # get the Fe
-00004190: 6174 7572 6520 4772 6f75 7020 696e 7374  ature Group inst
-000041a0: 616e 6365 0a20 2020 2020 2020 2020 2020  ance.           
-000041b0: 2066 6720 3d20 6673 2e67 6574 5f6f 725f   fg = fs.get_or_
-000041c0: 6372 6561 7465 5f66 6561 7475 7265 5f67  create_feature_g
-000041d0: 726f 7570 282e 2e2e 290a 0a20 2020 2020  roup(...)..     
-000041e0: 2020 2020 2020 2066 672e 7570 6461 7465         fg.update
-000041f0: 5f73 7461 7469 7374 6963 735f 636f 6e66  _statistics_conf
-00004200: 6967 2829 0a20 2020 2020 2020 2020 2020  ig().           
-00004210: 2060 6060 0a0a 2020 2020 2020 2020 2320   ```..        # 
-00004220: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00004230: 2020 2020 6046 6561 7475 7265 4772 6f75      `FeatureGrou
-00004240: 7060 2e20 5468 6520 7570 6461 7465 6420  p`. The updated 
-00004250: 6d65 7461 6461 7461 206f 626a 6563 7420  metadata object 
-00004260: 6f66 2074 6865 2066 6561 7475 7265 2067  of the feature g
-00004270: 726f 7570 2e0a 0a20 2020 2020 2020 2023  roup...        #
-00004280: 2052 6169 7365 730a 2020 2020 2020 2020   Raises.        
-00004290: 2020 2020 6068 7366 732e 636c 6965 6e74      `hsfs.client
-000042a0: 2e65 7863 6570 7469 6f6e 732e 5265 7374  .exceptions.Rest
-000042b0: 4150 4945 7272 6f72 602e 0a20 2020 2020  APIError`..     
-000042c0: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-000042d0: 656c 662e 5f66 6561 7475 7265 5f67 726f  elf._feature_gro
-000042e0: 7570 5f65 6e67 696e 652e 7570 6461 7465  up_engine.update
-000042f0: 5f73 7461 7469 7374 6963 735f 636f 6e66  _statistics_conf
-00004300: 6967 2873 656c 6629 0a20 2020 2020 2020  ig(self).       
-00004310: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
-00004320: 2020 6465 6620 7570 6461 7465 5f64 6573    def update_des
-00004330: 6372 6970 7469 6f6e 2873 656c 662c 2064  cription(self, d
-00004340: 6573 6372 6970 7469 6f6e 3a20 7374 7229  escription: str)
-00004350: 3a0a 2020 2020 2020 2020 2222 2255 7064  :.        """Upd
-00004360: 6174 6520 7468 6520 6465 7363 7269 7074  ate the descript
-00004370: 696f 6e20 6f66 2074 6865 2066 6561 7475  ion of the featu
-00004380: 7265 2067 726f 7570 2e0a 0a20 2020 2020  re group...     
-00004390: 2020 2021 2121 2065 7861 6d70 6c65 0a20     !!! example. 
-000043a0: 2020 2020 2020 2020 2020 2060 6060 7079             ```py
-000043b0: 7468 6f6e 0a20 2020 2020 2020 2020 2020  thon.           
-000043c0: 2023 2063 6f6e 6e65 6374 2074 6f20 7468   # connect to th
-000043d0: 6520 4665 6174 7572 6520 5374 6f72 650a  e Feature Store.
-000043e0: 2020 2020 2020 2020 2020 2020 6673 203d              fs =
-000043f0: 202e 2e2e 0a0a 2020 2020 2020 2020 2020   .....          
-00004400: 2020 2320 6765 7420 7468 6520 4665 6174    # get the Feat
-00004410: 7572 6520 4772 6f75 7020 696e 7374 616e  ure Group instan
-00004420: 6365 0a20 2020 2020 2020 2020 2020 2066  ce.            f
-00004430: 6720 3d20 6673 2e67 6574 5f6f 725f 6372  g = fs.get_or_cr
-00004440: 6561 7465 5f66 6561 7475 7265 5f67 726f  eate_feature_gro
-00004450: 7570 282e 2e2e 290a 0a20 2020 2020 2020  up(...)..       
-00004460: 2020 2020 2066 672e 7570 6461 7465 5f64       fg.update_d
-00004470: 6573 6372 6970 7469 6f6e 2864 6573 6372  escription(descr
-00004480: 6970 7469 6f6e 3d22 4d75 6368 2062 6574  iption="Much bet
-00004490: 7465 7220 6465 7363 7269 7074 696f 6e2e  ter description.
-000044a0: 2229 0a20 2020 2020 2020 2020 2020 2060  ").            `
-000044b0: 6060 0a0a 2020 2020 2020 2020 2121 2120  ``..        !!! 
-000044c0: 696e 666f 2022 5361 6665 2075 7064 6174  info "Safe updat
-000044d0: 6522 0a20 2020 2020 2020 2020 2020 2054  e".            T
-000044e0: 6869 7320 6d65 7468 6f64 2075 7064 6174  his method updat
-000044f0: 6573 2074 6865 2066 6561 7475 7265 2067  es the feature g
-00004500: 726f 7570 2064 6573 6372 6970 7469 6f6e  roup description
-00004510: 2073 6166 656c 792e 2049 6e20 6361 7365   safely. In case
-00004520: 206f 6620 6661 696c 7572 650a 2020 2020   of failure.    
-00004530: 2020 2020 2020 2020 796f 7572 206c 6f63          your loc
-00004540: 616c 206d 6574 6164 6174 6120 6f62 6a65  al metadata obje
-00004550: 6374 2077 696c 6c20 6b65 6570 2074 6865  ct will keep the
-00004560: 206f 6c64 2064 6573 6372 6970 7469 6f6e   old description
-00004570: 2e0a 0a20 2020 2020 2020 2023 2041 7267  ...        # Arg
-00004580: 756d 656e 7473 0a20 2020 2020 2020 2020  uments.         
-00004590: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-000045a0: 4e65 7720 6465 7363 7269 7074 696f 6e20  New description 
-000045b0: 7374 7269 6e67 2e0a 0a20 2020 2020 2020  string...       
-000045c0: 2023 2052 6574 7572 6e73 0a20 2020 2020   # Returns.     
-000045d0: 2020 2020 2020 2060 4665 6174 7572 6547         `FeatureG
-000045e0: 726f 7570 602e 2054 6865 2075 7064 6174  roup`. The updat
-000045f0: 6564 2066 6561 7475 7265 2067 726f 7570  ed feature group
-00004600: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
-00004610: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
-00004620: 662e 5f66 6561 7475 7265 5f67 726f 7570  f._feature_group
-00004630: 5f65 6e67 696e 652e 7570 6461 7465 5f64  _engine.update_d
-00004640: 6573 6372 6970 7469 6f6e 2873 656c 662c  escription(self,
-00004650: 2064 6573 6372 6970 7469 6f6e 290a 2020   description).  
-00004660: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00004670: 660a 0a20 2020 2064 6566 2075 7064 6174  f..    def updat
-00004680: 655f 6665 6174 7572 6573 2873 656c 662c  e_features(self,
-00004690: 2066 6561 7475 7265 733a 2055 6e69 6f6e   features: Union
-000046a0: 5b66 6561 7475 7265 2e46 6561 7475 7265  [feature.Feature
-000046b0: 2c20 4c69 7374 5b66 6561 7475 7265 2e46  , List[feature.F
-000046c0: 6561 7475 7265 5d5d 293a 0a20 2020 2020  eature]]):.     
-000046d0: 2020 2022 2222 5570 6461 7465 206d 6574     """Update met
-000046e0: 6164 6174 6120 6f66 2066 6561 7475 7265  adata of feature
-000046f0: 7320 696e 2074 6869 7320 6665 6174 7572  s in this featur
-00004700: 6520 6772 6f75 702e 0a0a 2020 2020 2020  e group...      
-00004710: 2020 4375 7272 656e 746c 7920 6974 2773    Currently it's
-00004720: 206f 6e6c 7920 7375 7070 6f72 7465 6420   only supported 
-00004730: 746f 2075 7064 6174 6520 7468 6520 6465  to update the de
-00004740: 7363 7269 7074 696f 6e20 6f66 2061 2066  scription of a f
-00004750: 6561 7475 7265 2e0a 0a20 2020 2020 2020  eature...       
-00004760: 2021 2121 2064 616e 6765 7220 2255 6e73   !!! danger "Uns
-00004770: 6166 6520 7570 6461 7465 220a 2020 2020  afe update".    
-00004780: 2020 2020 2020 2020 4e6f 7465 2074 6861          Note tha
-00004790: 7420 6966 2079 6f75 2075 7365 2061 6e20  t if you use an 
-000047a0: 6578 6973 7469 6e67 2060 4665 6174 7572  existing `Featur
-000047b0: 6560 206f 626a 6563 7420 6f66 2074 6865  e` object of the
-000047c0: 2073 6368 656d 6120 696e 2074 6865 0a20   schema in the. 
-000047d0: 2020 2020 2020 2020 2020 2066 6561 7475             featu
-000047e0: 7265 2067 726f 7570 206d 6574 6164 6174  re group metadat
-000047f0: 6120 6f62 6a65 6374 2c20 7468 6973 206d  a object, this m
-00004800: 6967 6874 206c 6561 7665 2079 6f75 7220  ight leave your 
-00004810: 6d65 7461 6461 7461 206f 626a 6563 7420  metadata object 
-00004820: 696e 2061 0a20 2020 2020 2020 2020 2020  in a.           
-00004830: 2063 6f72 7275 7074 6564 2073 7461 7465   corrupted state
-00004840: 2069 6620 7468 6520 7570 6461 7465 2066   if the update f
-00004850: 6169 6c73 2e0a 0a20 2020 2020 2020 2023  ails...        #
-00004860: 2041 7267 756d 656e 7473 0a20 2020 2020   Arguments.     
-00004870: 2020 2020 2020 2066 6561 7475 7265 733a         features:
-00004880: 2060 4665 6174 7572 6560 206f 7220 6c69   `Feature` or li
-00004890: 7374 206f 6620 6665 6174 7572 6573 2e20  st of features. 
-000048a0: 4120 6665 6174 7572 6520 6f62 6a65 6374  A feature object
-000048b0: 206f 7220 6c69 7374 2074 6865 7265 6f66   or list thereof
-000048c0: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-000048d0: 2020 2020 6265 2075 7064 6174 6564 2e0a      be updated..
-000048e0: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
-000048f0: 6e73 0a20 2020 2020 2020 2020 2020 2060  ns.            `
-00004900: 4665 6174 7572 6547 726f 7570 602e 2054  FeatureGroup`. T
-00004910: 6865 2075 7064 6174 6564 2066 6561 7475  he updated featu
-00004920: 7265 2067 726f 7570 206f 626a 6563 742e  re group object.
-00004930: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00004940: 2020 2020 206e 6577 5f66 6561 7475 7265       new_feature
-00004950: 7320 3d20 5b5d 0a20 2020 2020 2020 2069  s = [].        i
-00004960: 6620 6973 696e 7374 616e 6365 2866 6561  f isinstance(fea
-00004970: 7475 7265 732c 2066 6561 7475 7265 2e46  tures, feature.F
-00004980: 6561 7475 7265 293a 0a20 2020 2020 2020  eature):.       
-00004990: 2020 2020 206e 6577 5f66 6561 7475 7265       new_feature
-000049a0: 732e 6170 7065 6e64 2866 6561 7475 7265  s.append(feature
-000049b0: 7329 0a20 2020 2020 2020 2065 6c69 6620  s).        elif 
-000049c0: 6973 696e 7374 616e 6365 2866 6561 7475  isinstance(featu
-000049d0: 7265 732c 206c 6973 7429 3a0a 2020 2020  res, list):.    
-000049e0: 2020 2020 2020 2020 666f 7220 6665 6174          for feat
-000049f0: 2069 6e20 6665 6174 7572 6573 3a0a 2020   in features:.  
-00004a00: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00004a10: 2069 7369 6e73 7461 6e63 6528 6665 6174   isinstance(feat
-00004a20: 2c20 6665 6174 7572 652e 4665 6174 7572  , feature.Featur
-00004a30: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00004a40: 2020 2020 2020 2020 6e65 775f 6665 6174          new_feat
-00004a50: 7572 6573 2e61 7070 656e 6428 6665 6174  ures.append(feat
-00004a60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004a70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00004a80: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00004a90: 6520 5479 7065 4572 726f 7228 0a20 2020  e TypeError(.   
-00004aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ab0: 2020 2020 2022 5468 6520 6172 6775 6d65       "The argume
-00004ac0: 6e74 2060 6665 6174 7572 6573 6020 6861  nt `features` ha
-00004ad0: 7320 746f 2062 6520 6f66 2074 7970 6520  s to be of type 
-00004ae0: 6046 6561 7475 7265 6020 6f72 2022 0a20  `Feature` or ". 
-00004af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b00: 2020 2020 2020 2022 6120 6c69 7374 2074         "a list t
-00004b10: 6865 7265 6f66 2c20 6275 7420 616e 2065  hereof, but an e
-00004b20: 6c65 6d65 6e74 2069 7320 6f66 2074 7970  lement is of typ
-00004b30: 653a 2060 7b7d 6022 2e66 6f72 6d61 7428  e: `{}`".format(
-00004b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b50: 2020 2020 2020 2020 2020 2020 2074 7970               typ
-00004b60: 6528 6665 6174 7572 6573 290a 2020 2020  e(features).    
-00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b80: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00004b90: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00004ba0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00004bb0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-00004bc0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00004bd0: 2020 2020 2020 2022 5468 6520 6172 6775         "The argu
-00004be0: 6d65 6e74 2060 6665 6174 7572 6573 6020  ment `features` 
-00004bf0: 6861 7320 746f 2062 6520 6f66 2074 7970  has to be of typ
-00004c00: 6520 6046 6561 7475 7265 6020 6f72 2061  e `Feature` or a
-00004c10: 206c 6973 7420 220a 2020 2020 2020 2020   list ".        
-00004c20: 2020 2020 2020 2020 2274 6865 7265 6f66          "thereof
-00004c30: 2c20 6275 7420 6973 206f 6620 7479 7065  , but is of type
-00004c40: 3a20 607b 7d60 222e 666f 726d 6174 2874  : `{}`".format(t
-00004c50: 7970 6528 6665 6174 7572 6573 2929 0a20  ype(features)). 
-00004c60: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00004c70: 2020 2020 2073 656c 662e 5f66 6561 7475       self._featu
-00004c80: 7265 5f67 726f 7570 5f65 6e67 696e 652e  re_group_engine.
-00004c90: 7570 6461 7465 5f66 6561 7475 7265 7328  update_features(
-00004ca0: 7365 6c66 2c20 6e65 775f 6665 6174 7572  self, new_featur
-00004cb0: 6573 290a 2020 2020 2020 2020 7265 7475  es).        retu
-00004cc0: 726e 2073 656c 660a 0a20 2020 2064 6566  rn self..    def
-00004cd0: 2075 7064 6174 655f 6665 6174 7572 655f   update_feature_
-00004ce0: 6465 7363 7269 7074 696f 6e28 7365 6c66  description(self
-00004cf0: 2c20 6665 6174 7572 655f 6e61 6d65 3a20  , feature_name: 
-00004d00: 7374 722c 2064 6573 6372 6970 7469 6f6e  str, description
-00004d10: 3a20 7374 7229 3a0a 2020 2020 2020 2020  : str):.        
-00004d20: 2222 2255 7064 6174 6520 7468 6520 6465  """Update the de
-00004d30: 7363 7269 7074 696f 6e20 6f66 2061 2073  scription of a s
-00004d40: 696e 676c 6520 6665 6174 7572 6520 696e  ingle feature in
-00004d50: 2074 6869 7320 6665 6174 7572 6520 6772   this feature gr
-00004d60: 6f75 702e 0a0a 2020 2020 2020 2020 2121  oup...        !!
-00004d70: 2120 6578 616d 706c 650a 2020 2020 2020  ! example.      
-00004d80: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00004d90: 2020 2020 2020 2020 2020 2020 2320 636f              # co
-00004da0: 6e6e 6563 7420 746f 2074 6865 2046 6561  nnect to the Fea
-00004db0: 7475 7265 2053 746f 7265 0a20 2020 2020  ture Store.     
-00004dc0: 2020 2020 2020 2066 7320 3d20 2e2e 2e0a         fs = ....
-00004dd0: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
-00004de0: 6574 2074 6865 2046 6561 7475 7265 2047  et the Feature G
-00004df0: 726f 7570 2069 6e73 7461 6e63 650a 2020  roup instance.  
-00004e00: 2020 2020 2020 2020 2020 6667 203d 2066            fg = f
-00004e10: 732e 6765 745f 6f72 5f63 7265 6174 655f  s.get_or_create_
-00004e20: 6665 6174 7572 655f 6772 6f75 7028 2e2e  feature_group(..
-00004e30: 2e29 0a0a 2020 2020 2020 2020 2020 2020  .)..            
-00004e40: 6667 2e75 7064 6174 655f 6665 6174 7572  fg.update_featur
-00004e50: 655f 6465 7363 7269 7074 696f 6e28 6665  e_description(fe
-00004e60: 6174 7572 655f 6e61 6d65 3d22 6d69 6e5f  ature_name="min_
-00004e70: 7465 6d70 222c 0a20 2020 2020 2020 2020  temp",.         
-00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ea0: 2064 6573 6372 6970 7469 6f6e 3d22 4d75   description="Mu
-00004eb0: 6368 2062 6574 7465 7220 6665 6174 7572  ch better featur
-00004ec0: 6520 6465 7363 7269 7074 696f 6e2e 2229  e description.")
-00004ed0: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
-00004ee0: 0a0a 2020 2020 2020 2020 2121 2120 696e  ..        !!! in
-00004ef0: 666f 2022 5361 6665 2075 7064 6174 6522  fo "Safe update"
-00004f00: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-00004f10: 7320 6d65 7468 6f64 2075 7064 6174 6573  s method updates
-00004f20: 2074 6865 2066 6561 7475 7265 2064 6573   the feature des
-00004f30: 6372 6970 7469 6f6e 2073 6166 656c 792e  cription safely.
-00004f40: 2049 6e20 6361 7365 206f 6620 6661 696c   In case of fail
-00004f50: 7572 650a 2020 2020 2020 2020 2020 2020  ure.            
-00004f60: 796f 7572 206c 6f63 616c 206d 6574 6164  your local metad
-00004f70: 6174 6120 6f62 6a65 6374 2077 696c 6c20  ata object will 
-00004f80: 6b65 6570 2074 6865 206f 6c64 2064 6573  keep the old des
-00004f90: 6372 6970 7469 6f6e 2e0a 0a20 2020 2020  cription...     
-00004fa0: 2020 2023 2041 7267 756d 656e 7473 0a20     # Arguments. 
-00004fb0: 2020 2020 2020 2020 2020 2066 6561 7475             featu
-00004fc0: 7265 5f6e 616d 653a 204e 616d 6520 6f66  re_name: Name of
-00004fd0: 2074 6865 2066 6561 7475 7265 2074 6f20   the feature to 
-00004fe0: 6265 2075 7064 6174 6564 2e0a 2020 2020  be updated..    
-00004ff0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00005000: 696f 6e3a 204e 6577 2064 6573 6372 6970  ion: New descrip
-00005010: 7469 6f6e 2073 7472 696e 672e 0a0a 2020  tion string...  
-00005020: 2020 2020 2020 2320 5265 7475 726e 730a        # Returns.
-00005030: 2020 2020 2020 2020 2020 2020 6046 6561              `Fea
-00005040: 7475 7265 4772 6f75 7060 2e20 5468 6520  tureGroup`. The 
-00005050: 7570 6461 7465 6420 6665 6174 7572 6520  updated feature 
-00005060: 6772 6f75 7020 6f62 6a65 6374 2e0a 2020  group object..  
-00005070: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00005080: 2020 665f 636f 7079 203d 2063 6f70 792e    f_copy = copy.
-00005090: 6465 6570 636f 7079 2873 656c 665b 6665  deepcopy(self[fe
-000050a0: 6174 7572 655f 6e61 6d65 5d29 0a20 2020  ature_name]).   
-000050b0: 2020 2020 2066 5f63 6f70 792e 6465 7363       f_copy.desc
-000050c0: 7269 7074 696f 6e20 3d20 6465 7363 7269  ription = descri
-000050d0: 7074 696f 6e0a 2020 2020 2020 2020 7365  ption.        se
-000050e0: 6c66 2e5f 6665 6174 7572 655f 6772 6f75  lf._feature_grou
-000050f0: 705f 656e 6769 6e65 2e75 7064 6174 655f  p_engine.update_
-00005100: 6665 6174 7572 6573 2873 656c 662c 205b  features(self, [
-00005110: 665f 636f 7079 5d29 0a20 2020 2020 2020  f_copy]).       
-00005120: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
-00005130: 2020 6465 6620 6170 7065 6e64 5f66 6561    def append_fea
-00005140: 7475 7265 7328 7365 6c66 2c20 6665 6174  tures(self, feat
-00005150: 7572 6573 3a20 556e 696f 6e5b 6665 6174  ures: Union[feat
-00005160: 7572 652e 4665 6174 7572 652c 204c 6973  ure.Feature, Lis
-00005170: 745b 6665 6174 7572 652e 4665 6174 7572  t[feature.Featur
-00005180: 655d 5d29 3a0a 2020 2020 2020 2020 2222  e]]):.        ""
-00005190: 2241 7070 656e 6420 6665 6174 7572 6573  "Append features
-000051a0: 2074 6f20 7468 6520 7363 6865 6d61 206f   to the schema o
-000051b0: 6620 7468 6520 6665 6174 7572 6520 6772  f the feature gr
-000051c0: 6f75 702e 0a0a 2020 2020 2020 2020 2121  oup...        !!
-000051d0: 2120 6578 616d 706c 650a 2020 2020 2020  ! example.      
-000051e0: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-000051f0: 2020 2020 2020 2020 2020 2020 2320 636f              # co
-00005200: 6e6e 6563 7420 746f 2074 6865 2046 6561  nnect to the Fea
-00005210: 7475 7265 2053 746f 7265 0a20 2020 2020  ture Store.     
-00005220: 2020 2020 2020 2066 7320 3d20 2e2e 2e0a         fs = ....
-00005230: 0a20 2020 2020 2020 2020 2020 2023 2064  .            # d
-00005240: 6566 696e 6520 6665 6174 7572 6573 2074  efine features t
-00005250: 6f20 6265 2069 6e73 6572 7465 6420 696e  o be inserted in
-00005260: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
-00005270: 7570 0a20 2020 2020 2020 2020 2020 2066  up.            f
-00005280: 6561 7475 7265 7320 3d20 5b0a 2020 2020  eatures = [.    
-00005290: 2020 2020 2020 2020 2020 2020 4665 6174              Feat
-000052a0: 7572 6528 6e61 6d65 3d22 6964 222c 7479  ure(name="id",ty
-000052b0: 7065 3d22 696e 7422 2c6f 6e6c 696e 655f  pe="int",online_
-000052c0: 7479 7065 3d22 696e 7422 292c 0a20 2020  type="int"),.   
-000052d0: 2020 2020 2020 2020 2020 2020 2046 6561               Fea
-000052e0: 7475 7265 286e 616d 653d 226e 616d 6522  ture(name="name"
-000052f0: 2c74 7970 653d 2273 7472 696e 6722 2c6f  ,type="string",o
-00005300: 6e6c 696e 655f 7479 7065 3d22 7661 7263  nline_type="varc
-00005310: 6861 7228 3230 2922 290a 2020 2020 2020  har(20)").      
-00005320: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
-00005330: 2020 2020 2023 2067 6574 2074 6865 2046       # get the F
-00005340: 6561 7475 7265 2047 726f 7570 2069 6e73  eature Group ins
-00005350: 7461 6e63 650a 2020 2020 2020 2020 2020  tance.          
-00005360: 2020 6667 203d 2066 732e 6765 745f 6f72    fg = fs.get_or
-00005370: 5f63 7265 6174 655f 6665 6174 7572 655f  _create_feature_
-00005380: 6772 6f75 7028 2e2e 2e29 0a0a 2020 2020  group(...)..    
-00005390: 2020 2020 2020 2020 6667 2e61 7070 656e          fg.appen
-000053a0: 645f 6665 6174 7572 6573 2866 6561 7475  d_features(featu
-000053b0: 7265 7329 0a20 2020 2020 2020 2020 2020  res).           
-000053c0: 2060 6060 0a0a 2020 2020 2020 2020 2121   ```..        !!
-000053d0: 2120 696e 666f 2022 5361 6665 2061 7070  ! info "Safe app
-000053e0: 656e 6422 0a20 2020 2020 2020 2020 2020  end".           
-000053f0: 2054 6869 7320 6d65 7468 6f64 2061 7070   This method app
-00005400: 656e 6473 2074 6865 2066 6561 7475 7265  ends the feature
-00005410: 7320 746f 2074 6865 2066 6561 7475 7265  s to the feature
-00005420: 2067 726f 7570 2064 6573 6372 6970 7469   group descripti
-00005430: 6f6e 2073 6166 656c 792e 0a20 2020 2020  on safely..     
-00005440: 2020 2020 2020 2049 6e20 6361 7365 206f         In case o
-00005450: 6620 6661 696c 7572 6520 796f 7572 206c  f failure your l
-00005460: 6f63 616c 206d 6574 6164 6174 6120 6f62  ocal metadata ob
-00005470: 6a65 6374 2077 696c 6c20 636f 6e74 6169  ject will contai
-00005480: 6e20 7468 6520 636f 7272 6563 740a 2020  n the correct.  
-00005490: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-000054a0: 2e0a 0a20 2020 2020 2020 2049 7420 6973  ...        It is
-000054b0: 206f 6e6c 7920 706f 7373 6962 6c65 2074   only possible t
-000054c0: 6f20 6170 7065 6e64 2066 6561 7475 7265  o append feature
-000054d0: 7320 746f 2061 2066 6561 7475 7265 2067  s to a feature g
-000054e0: 726f 7570 2e20 5265 6d6f 7669 6e67 0a20  roup. Removing. 
-000054f0: 2020 2020 2020 2066 6561 7475 7265 7320         features 
-00005500: 6973 2063 6f6e 7369 6465 7265 6420 6120  is considered a 
-00005510: 6272 6561 6b69 6e67 2063 6861 6e67 652e  breaking change.
-00005520: 0a0a 2020 2020 2020 2020 2320 4172 6775  ..        # Argu
-00005530: 6d65 6e74 730a 2020 2020 2020 2020 2020  ments.          
-00005540: 2020 6665 6174 7572 6573 3a20 4665 6174    features: Feat
-00005550: 7572 6520 6f72 206c 6973 742e 2041 2066  ure or list. A f
-00005560: 6561 7475 7265 206f 626a 6563 7420 6f72  eature object or
-00005570: 206c 6973 7420 7468 6572 656f 6620 746f   list thereof to
-00005580: 2061 7070 656e 6420 746f 0a20 2020 2020   append to.     
-00005590: 2020 2020 2020 2020 2020 2074 6865 2073             the s
-000055a0: 6368 656d 6120 6f66 2074 6865 2066 6561  chema of the fea
-000055b0: 7475 7265 2067 726f 7570 2e0a 0a20 2020  ture group...   
-000055c0: 2020 2020 2023 2052 6574 7572 6e73 0a20       # Returns. 
-000055d0: 2020 2020 2020 2020 2020 2060 4665 6174             `Feat
-000055e0: 7572 6547 726f 7570 602e 2054 6865 2075  ureGroup`. The u
-000055f0: 7064 6174 6564 2066 6561 7475 7265 2067  pdated feature g
-00005600: 726f 7570 206f 626a 6563 742e 0a20 2020  roup object..   
-00005610: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00005620: 206e 6577 5f66 6561 7475 7265 7320 3d20   new_features = 
-00005630: 5b5d 0a20 2020 2020 2020 2069 6620 6973  [].        if is
-00005640: 696e 7374 616e 6365 2866 6561 7475 7265  instance(feature
-00005650: 732c 2066 6561 7475 7265 2e46 6561 7475  s, feature.Featu
-00005660: 7265 293a 0a20 2020 2020 2020 2020 2020  re):.           
-00005670: 206e 6577 5f66 6561 7475 7265 732e 6170   new_features.ap
-00005680: 7065 6e64 2866 6561 7475 7265 7329 0a20  pend(features). 
-00005690: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-000056a0: 7374 616e 6365 2866 6561 7475 7265 732c  stance(features,
-000056b0: 206c 6973 7429 3a0a 2020 2020 2020 2020   list):.        
-000056c0: 2020 2020 666f 7220 6665 6174 2069 6e20      for feat in 
-000056d0: 6665 6174 7572 6573 3a0a 2020 2020 2020  features:.      
-000056e0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-000056f0: 6e73 7461 6e63 6528 6665 6174 2c20 6665  nstance(feat, fe
-00005700: 6174 7572 652e 4665 6174 7572 6529 3a0a  ature.Feature):.
-00005710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005720: 2020 2020 6e65 775f 6665 6174 7572 6573      new_features
-00005730: 2e61 7070 656e 6428 6665 6174 290a 2020  .append(feat).  
-00005740: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00005750: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00005760: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
-00005770: 7065 4572 726f 7228 0a20 2020 2020 2020  peError(.       
-00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005790: 2022 5468 6520 6172 6775 6d65 6e74 2060   "The argument `
-000057a0: 6665 6174 7572 6573 6020 6861 7320 746f  features` has to
-000057b0: 2062 6520 6f66 2074 7970 6520 6046 6561   be of type `Fea
-000057c0: 7475 7265 6020 6f72 2022 0a20 2020 2020  ture` or ".     
-000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057e0: 2020 2022 6120 6c69 7374 2074 6865 7265     "a list there
-000057f0: 6f66 2c20 6275 7420 616e 2065 6c65 6d65  of, but an eleme
-00005800: 6e74 2069 7320 6f66 2074 7970 653a 2060  nt is of type: `
-00005810: 7b7d 6022 2e66 6f72 6d61 7428 0a20 2020  {}`".format(.   
-00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005830: 2020 2020 2020 2020 2074 7970 6528 6665           type(fe
-00005840: 6174 7572 6573 290a 2020 2020 2020 2020  atures).        
-00005850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005860: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005870: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00005880: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00005890: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-000058a0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-000058b0: 2020 2022 5468 6520 6172 6775 6d65 6e74     "The argument
-000058c0: 2060 6665 6174 7572 6573 6020 6861 7320   `features` has 
-000058d0: 746f 2062 6520 6f66 2074 7970 6520 6046  to be of type `F
-000058e0: 6561 7475 7265 6020 6f72 2061 206c 6973  eature` or a lis
-000058f0: 7420 220a 2020 2020 2020 2020 2020 2020  t ".            
-00005900: 2020 2020 2274 6865 7265 6f66 2c20 6275      "thereof, bu
-00005910: 7420 6973 206f 6620 7479 7065 3a20 607b  t is of type: `{
-00005920: 7d60 222e 666f 726d 6174 2874 7970 6528  }`".format(type(
-00005930: 6665 6174 7572 6573 2929 0a20 2020 2020  features)).     
-00005940: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00005950: 2073 656c 662e 5f66 6561 7475 7265 5f67   self._feature_g
-00005960: 726f 7570 5f65 6e67 696e 652e 6170 7065  roup_engine.appe
-00005970: 6e64 5f66 6561 7475 7265 7328 7365 6c66  nd_features(self
-00005980: 2c20 6e65 775f 6665 6174 7572 6573 290a  , new_features).
-00005990: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000059a0: 656c 660a 0a20 2020 2064 6566 2067 6574  elf..    def get
-000059b0: 5f65 7870 6563 7461 7469 6f6e 5f73 7569  _expectation_sui
-000059c0: 7465 280a 2020 2020 2020 2020 7365 6c66  te(.        self
-000059d0: 2c20 6765 5f74 7970 653a 2062 6f6f 6c20  , ge_type: bool 
-000059e0: 3d20 5472 7565 0a20 2020 2029 202d 3e20  = True.    ) -> 
-000059f0: 556e 696f 6e5b 4578 7065 6374 6174 696f  Union[Expectatio
-00005a00: 6e53 7569 7465 2c20 6765 2e63 6f72 652e  nSuite, ge.core.
-00005a10: 4578 7065 6374 6174 696f 6e53 7569 7465  ExpectationSuite
-00005a20: 2c20 4e6f 6e65 5d3a 0a20 2020 2020 2020  , None]:.       
-00005a30: 2022 2222 5265 7475 726e 2074 6865 2065   """Return the e
-00005a40: 7870 6563 7461 7469 6f6e 2073 7569 7465  xpectation suite
-00005a50: 2061 7474 6163 6865 6420 746f 2074 6865   attached to the
-00005a60: 2066 6561 7475 7265 2067 726f 7570 2069   feature group i
-00005a70: 6620 6974 2065 7869 7374 732e 0a0a 2020  f it exists...  
-00005a80: 2020 2020 2020 2121 2120 6578 616d 706c        !!! exampl
-00005a90: 650a 2020 2020 2020 2020 2020 2020 6060  e.            ``
-00005aa0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
-00005ab0: 2020 2020 2320 636f 6e6e 6563 7420 746f      # connect to
-00005ac0: 2074 6865 2046 6561 7475 7265 2053 746f   the Feature Sto
-00005ad0: 7265 0a20 2020 2020 2020 2020 2020 2066  re.            f
-00005ae0: 7320 3d20 2e2e 2e0a 0a20 2020 2020 2020  s = .....       
-00005af0: 2020 2020 2023 2067 6574 2074 6865 2046       # get the F
-00005b00: 6561 7475 7265 2047 726f 7570 2069 6e73  eature Group ins
-00005b10: 7461 6e63 650a 2020 2020 2020 2020 2020  tance.          
-00005b20: 2020 6667 203d 2066 732e 6765 745f 6f72    fg = fs.get_or
-00005b30: 5f63 7265 6174 655f 6665 6174 7572 655f  _create_feature_
-00005b40: 6772 6f75 7028 2e2e 2e29 0a0a 2020 2020  group(...)..    
-00005b50: 2020 2020 2020 2020 6578 705f 7375 6974          exp_suit
-00005b60: 6520 3d20 6667 2e67 6574 5f65 7870 6563  e = fg.get_expec
-00005b70: 7461 7469 6f6e 5f73 7569 7465 2829 0a20  tation_suite(). 
-00005b80: 2020 2020 2020 2020 2020 2060 6060 0a0a             ```..
-00005b90: 2020 2020 2020 2020 2320 4172 6775 6d65          # Argume
-00005ba0: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-00005bb0: 6765 5f74 7970 653a 2049 6620 6054 7275  ge_type: If `Tru
-00005bc0: 6560 2072 6574 7572 6e73 2061 206e 6174  e` returns a nat
-00005bd0: 6976 6520 4772 6561 7420 4578 7065 6374  ive Great Expect
-00005be0: 6174 696f 6e20 7479 7065 2c20 486f 7073  ation type, Hops
-00005bf0: 776f 726b 730a 2020 2020 2020 2020 2020  works.          
-00005c00: 2020 2020 2020 6375 7374 6f6d 2074 7970        custom typ
-00005c10: 6520 6f74 6865 7277 6973 652e 2043 6f6e  e otherwise. Con
-00005c20: 7665 7273 696f 6e20 6361 6e20 6265 2070  version can be p
-00005c30: 6572 666f 726d 6564 2076 6961 2074 6865  erformed via the
-00005c40: 2060 746f 5f67 655f 7479 7065 2829 600a   `to_ge_type()`.
-00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c60: 6d65 7468 6f64 206f 6e20 686f 7073 776f  method on hopswo
-00005c70: 726b 7320 7479 7065 2e20 4465 6661 756c  rks type. Defaul
-00005c80: 7473 2074 6f20 6054 7275 6560 2e0a 0a20  ts to `True`... 
-00005c90: 2020 2020 2020 2023 2052 6574 7572 6e73         # Returns
-00005ca0: 0a20 2020 2020 2020 2020 2020 2060 4578  .            `Ex
-00005cb0: 7065 6374 6174 696f 6e53 7569 7465 602e  pectationSuite`.
-00005cc0: 2054 6865 2065 7870 6563 7461 7469 6f6e   The expectation
-00005cd0: 2073 7569 7465 2061 7474 6163 6865 6420   suite attached 
-00005ce0: 746f 2074 6865 2066 6561 7475 7265 2067  to the feature g
-00005cf0: 726f 7570 2e0a 0a20 2020 2020 2020 2023  roup...        #
-00005d00: 2052 6169 7365 730a 2020 2020 2020 2020   Raises.        
-00005d10: 2020 2020 6068 7366 732e 636c 6965 6e74      `hsfs.client
-00005d20: 2e65 7863 6570 7469 6f6e 732e 5265 7374  .exceptions.Rest
-00005d30: 4150 4945 7272 6f72 602e 0a20 2020 2020  APIError`..     
-00005d40: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-00005d50: 2041 766f 6964 2074 6872 6f77 696e 6720   Avoid throwing 
-00005d60: 616e 2065 7272 6f72 2069 6620 4665 6174  an error if Feat
-00005d70: 7572 6520 4772 6f75 7020 6e6f 7420 696e  ure Group not in
-00005d80: 6974 6961 6c69 7365 642e 0a20 2020 2020  itialised..     
-00005d90: 2020 2069 6620 7365 6c66 2e5f 6964 3a0a     if self._id:.
-00005da0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005db0: 2e5f 6578 7065 6374 6174 696f 6e5f 7375  ._expectation_su
-00005dc0: 6974 6520 3d20 7365 6c66 2e5f 6578 7065  ite = self._expe
-00005dd0: 6374 6174 696f 6e5f 7375 6974 655f 656e  ctation_suite_en
-00005de0: 6769 6e65 2e67 6574 2829 0a0a 2020 2020  gine.get()..    
-00005df0: 2020 2020 6966 2073 656c 662e 5f65 7870      if self._exp
-00005e00: 6563 7461 7469 6f6e 5f73 7569 7465 2069  ectation_suite i
-00005e10: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2067  s not None and g
-00005e20: 655f 7479 7065 2069 7320 5472 7565 3a0a  e_type is True:.
-00005e30: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00005e40: 726e 2073 656c 662e 5f65 7870 6563 7461  rn self._expecta
-00005e50: 7469 6f6e 5f73 7569 7465 2e74 6f5f 6765  tion_suite.to_ge
-00005e60: 5f74 7970 6528 290a 2020 2020 2020 2020  _type().        
-00005e70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00005e80: 2020 7265 7475 726e 2073 656c 662e 5f65    return self._e
-00005e90: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-00005ea0: 0a0a 2020 2020 6465 6620 7361 7665 5f65  ..    def save_e
-00005eb0: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-00005ec0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00005ed0: 2020 2020 2020 2020 6578 7065 6374 6174          expectat
-00005ee0: 696f 6e5f 7375 6974 653a 2055 6e69 6f6e  ion_suite: Union
-00005ef0: 5b45 7870 6563 7461 7469 6f6e 5375 6974  [ExpectationSuit
-00005f00: 652c 2067 652e 636f 7265 2e45 7870 6563  e, ge.core.Expec
-00005f10: 7461 7469 6f6e 5375 6974 655d 2c0a 2020  tationSuite],.  
-00005f20: 2020 2020 2020 7275 6e5f 7661 6c69 6461        run_valida
-00005f30: 7469 6f6e 3a20 626f 6f6c 203d 2054 7275  tion: bool = Tru
-00005f40: 652c 0a20 2020 2020 2020 2076 616c 6964  e,.        valid
-00005f50: 6174 696f 6e5f 696e 6765 7374 696f 6e5f  ation_ingestion_
-00005f60: 706f 6c69 6379 3a20 7374 7220 3d20 2241  policy: str = "A
-00005f70: 4c57 4159 5322 2c0a 2020 2020 2020 2020  LWAYS",.        
-00005f80: 6f76 6572 7772 6974 653a 2062 6f6f 6c20  overwrite: bool 
-00005f90: 3d20 4661 6c73 652c 0a20 2020 2029 202d  = False,.    ) -
-00005fa0: 3e20 556e 696f 6e5b 4578 7065 6374 6174  > Union[Expectat
-00005fb0: 696f 6e53 7569 7465 2c20 6765 2e63 6f72  ionSuite, ge.cor
-00005fc0: 652e 4578 7065 6374 6174 696f 6e53 7569  e.ExpectationSui
-00005fd0: 7465 5d3a 0a20 2020 2020 2020 2022 2222  te]:.        """
-00005fe0: 4174 7461 6368 2061 6e20 6578 7065 6374  Attach an expect
-00005ff0: 6174 696f 6e20 7375 6974 6520 746f 2061  ation suite to a
-00006000: 2066 6561 7475 7265 2067 726f 7570 2061   feature group a
-00006010: 6e64 2073 6176 6573 2069 7420 666f 7220  nd saves it for 
-00006020: 6675 7475 7265 2075 7365 2e20 4966 2061  future use. If a
-00006030: 6e20 6578 7065 6374 6174 696f 6e0a 2020  n expectation.  
-00006040: 2020 2020 2020 7375 6974 6520 6973 2061        suite is a
-00006050: 6c72 6561 6479 2061 7474 6163 6865 642c  lready attached,
-00006060: 2069 7420 6973 2072 6570 6c61 6365 642e   it is replaced.
-00006070: 204e 6f74 6520 7468 6174 2074 6865 2070   Note that the p
-00006080: 726f 7669 6465 6420 6578 7065 6374 6174  rovided expectat
-00006090: 696f 6e20 7375 6974 6520 6973 206d 6f64  ion suite is mod
-000060a0: 6966 6965 640a 2020 2020 2020 2020 696e  ified.        in
-000060b0: 706c 6163 6520 746f 2069 6e63 6c75 6465  place to include
-000060c0: 2065 7870 6563 7461 7469 6f6e 4964 2066   expectationId f
-000060d0: 6965 6c64 732e 0a0a 2020 2020 2020 2020  ields...        
-000060e0: 2121 2120 6578 616d 706c 650a 2020 2020  !!! example.    
-000060f0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-00006100: 6e0a 2020 2020 2020 2020 2020 2020 2320  n.            # 
-00006110: 636f 6e6e 6563 7420 746f 2074 6865 2046  connect to the F
-00006120: 6561 7475 7265 2053 746f 7265 0a20 2020  eature Store.   
-00006130: 2020 2020 2020 2020 2066 7320 3d20 2e2e           fs = ..
-00006140: 2e0a 0a20 2020 2020 2020 2020 2020 2023  ...            #
-00006150: 2067 6574 2074 6865 2046 6561 7475 7265   get the Feature
-00006160: 2047 726f 7570 2069 6e73 7461 6e63 650a   Group instance.
-00006170: 2020 2020 2020 2020 2020 2020 6667 203d              fg =
-00006180: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
-00006190: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
-000061a0: 2e2e 2e29 0a0a 2020 2020 2020 2020 2020  ...)..          
-000061b0: 2020 6667 2e73 6176 655f 6578 7065 6374    fg.save_expect
-000061c0: 6174 696f 6e5f 7375 6974 6528 6578 7065  ation_suite(expe
-000061d0: 6374 6174 696f 6e5f 7375 6974 652c 2072  ctation_suite, r
-000061e0: 756e 5f76 616c 6964 6174 696f 6e3d 5472  un_validation=Tr
-000061f0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-00006200: 6060 600a 0a20 2020 2020 2020 2023 2041  ```..        # A
-00006210: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
-00006220: 2020 2020 2065 7870 6563 7461 7469 6f6e       expectation
-00006230: 5f73 7569 7465 3a20 5468 6520 6578 7065  _suite: The expe
-00006240: 6374 6174 696f 6e20 7375 6974 6520 746f  ctation suite to
-00006250: 2061 7474 6163 6820 746f 2074 6865 2046   attach to the F
-00006260: 6561 7475 7265 2047 726f 7570 2e0a 2020  eature Group..  
-00006270: 2020 2020 2020 2020 2020 6f76 6572 7772            overwr
-00006280: 6974 653a 2049 6620 616e 2045 7870 6563  ite: If an Expec
-00006290: 7461 7469 6f6e 2053 7569 7465 2069 7320  tation Suite is 
-000062a0: 616c 7265 6164 7920 6174 7461 6368 6564  already attached
-000062b0: 2c20 6f76 6572 7772 6974 6520 6974 2e0a  , overwrite it..
-000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062d0: 5468 6520 6e65 7720 7375 6974 6520 7769  The new suite wi
-000062e0: 6c6c 2068 6176 6520 6974 7320 6f77 6e20  ll have its own 
-000062f0: 7661 6c69 6461 7469 6f6e 2068 6973 746f  validation histo
-00006300: 7279 2c20 6275 7420 666f 726d 6572 2072  ry, but former r
-00006310: 6570 6f72 7473 2061 7265 2070 7265 7365  eports are prese
-00006320: 7276 6564 2e0a 2020 2020 2020 2020 2020  rved..          
-00006330: 2020 7275 6e5f 7661 6c69 6461 7469 6f6e    run_validation
-00006340: 3a20 5365 7420 7768 6574 6865 7220 7468  : Set whether th
-00006350: 6520 6578 7065 6374 6174 696f 6e5f 7375  e expectation_su
-00006360: 6974 6520 7769 6c6c 2072 756e 206f 6e20  ite will run on 
-00006370: 696e 6765 7374 696f 6e0a 2020 2020 2020  ingestion.      
-00006380: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
-00006390: 5f69 6e67 6573 7469 6f6e 5f70 6f6c 6963  _ingestion_polic
-000063a0: 793a 2053 6574 2074 6865 2070 6f6c 6963  y: Set the polic
-000063b0: 7920 666f 7220 696e 6765 7374 696f 6e20  y for ingestion 
-000063c0: 746f 2074 6865 2046 6561 7475 7265 2047  to the Feature G
-000063d0: 726f 7570 2e0a 2020 2020 2020 2020 2020  roup..          
-000063e0: 2020 2020 2020 2d20 2253 5452 4943 5422        - "STRICT"
-000063f0: 206f 6e6c 7920 616c 6c6f 7773 2044 6174   only allows Dat
-00006400: 6146 7261 6d65 2070 6173 7369 6e67 2076  aFrame passing v
-00006410: 616c 6964 6174 696f 6e20 746f 2062 6520  alidation to be 
-00006420: 696e 7365 7274 6564 2069 6e74 6f20 4665  inserted into Fe
-00006430: 6174 7572 6520 4772 6f75 702e 0a20 2020  ature Group..   
-00006440: 2020 2020 2020 2020 2020 2020 202d 2022               - "
-00006450: 414c 5741 5953 2220 616c 7761 7973 2069  ALWAYS" always i
-00006460: 6e73 6572 7420 7468 6520 4461 7461 4672  nsert the DataFr
-00006470: 616d 6520 746f 2074 6865 2046 6561 7475  ame to the Featu
-00006480: 7265 2047 726f 7570 2c20 6972 7265 7370  re Group, irresp
-00006490: 6563 7469 7665 206f 6620 6f76 6572 616c  ective of overal
-000064a0: 6c20 7661 6c69 6461 7469 6f6e 2072 6573  l validation res
-000064b0: 756c 742e 0a0a 2020 2020 2020 2020 2320  ult...        # 
-000064c0: 5261 6973 6573 0a20 2020 2020 2020 2020  Raises.         
-000064d0: 2020 2060 6873 6673 2e63 6c69 656e 742e     `hsfs.client.
-000064e0: 6578 6365 7074 696f 6e73 2e52 6573 7441  exceptions.RestA
-000064f0: 5049 4572 726f 7260 2e0a 2020 2020 2020  PIError`..      
-00006500: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00006510: 2069 7369 6e73 7461 6e63 6528 6578 7065   isinstance(expe
-00006520: 6374 6174 696f 6e5f 7375 6974 652c 2067  ctation_suite, g
-00006530: 652e 636f 7265 2e45 7870 6563 7461 7469  e.core.Expectati
-00006540: 6f6e 5375 6974 6529 3a0a 2020 2020 2020  onSuite):.      
-00006550: 2020 2020 2020 746d 705f 6578 7065 6374        tmp_expect
-00006560: 6174 696f 6e5f 7375 6974 6520 3d20 4578  ation_suite = Ex
-00006570: 7065 6374 6174 696f 6e53 7569 7465 2e66  pectationSuite.f
-00006580: 726f 6d5f 6765 5f74 7970 6528 0a20 2020  rom_ge_type(.   
-00006590: 2020 2020 2020 2020 2020 2020 2067 655f               ge_
-000065a0: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
-000065b0: 653d 6578 7065 6374 6174 696f 6e5f 7375  e=expectation_su
-000065c0: 6974 652c 0a20 2020 2020 2020 2020 2020  ite,.           
-000065d0: 2020 2020 2072 756e 5f76 616c 6964 6174       run_validat
-000065e0: 696f 6e3d 7275 6e5f 7661 6c69 6461 7469  ion=run_validati
-000065f0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-00006600: 2020 2020 7661 6c69 6461 7469 6f6e 5f69      validation_i
-00006610: 6e67 6573 7469 6f6e 5f70 6f6c 6963 793d  ngestion_policy=
-00006620: 7661 6c69 6461 7469 6f6e 5f69 6e67 6573  validation_inges
-00006630: 7469 6f6e 5f70 6f6c 6963 792c 0a20 2020  tion_policy,.   
-00006640: 2020 2020 2020 2020 2020 2020 2066 6561               fea
-00006650: 7475 7265 5f73 746f 7265 5f69 643d 7365  ture_store_id=se
-00006660: 6c66 2e5f 6665 6174 7572 655f 7374 6f72  lf._feature_stor
-00006670: 655f 6964 2c0a 2020 2020 2020 2020 2020  e_id,.          
-00006680: 2020 2020 2020 6665 6174 7572 655f 6772        feature_gr
-00006690: 6f75 705f 6964 3d73 656c 662e 5f69 642c  oup_id=self._id,
-000066a0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-000066b0: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-000066c0: 7374 616e 6365 2865 7870 6563 7461 7469  stance(expectati
-000066d0: 6f6e 5f73 7569 7465 2c20 4578 7065 6374  on_suite, Expect
-000066e0: 6174 696f 6e53 7569 7465 293a 0a20 2020  ationSuite):.   
-000066f0: 2020 2020 2020 2020 2074 6d70 5f65 7870           tmp_exp
-00006700: 6563 7461 7469 6f6e 5f73 7569 7465 203d  ectation_suite =
-00006710: 2065 7870 6563 7461 7469 6f6e 5f73 7569   expectation_sui
-00006720: 7465 2e74 6f5f 6a73 6f6e 5f64 6963 7428  te.to_json_dict(
-00006730: 6465 6361 6d65 6c69 7a65 3d54 7275 6529  decamelize=True)
-00006740: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
-00006750: 5f65 7870 6563 7461 7469 6f6e 5f73 7569  _expectation_sui
-00006760: 7465 5b22 6665 6174 7572 655f 6772 6f75  te["feature_grou
-00006770: 705f 6964 225d 203d 2073 656c 662e 5f69  p_id"] = self._i
-00006780: 640a 2020 2020 2020 2020 2020 2020 746d  d.            tm
-00006790: 705f 6578 7065 6374 6174 696f 6e5f 7375  p_expectation_su
-000067a0: 6974 655b 2266 6561 7475 7265 5f73 746f  ite["feature_sto
-000067b0: 7265 5f69 6422 5d20 3d20 7365 6c66 2e5f  re_id"] = self._
-000067c0: 6665 6174 7572 655f 7374 6f72 655f 6964  feature_store_id
-000067d0: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
-000067e0: 5f65 7870 6563 7461 7469 6f6e 5f73 7569  _expectation_sui
-000067f0: 7465 203d 2045 7870 6563 7461 7469 6f6e  te = Expectation
-00006800: 5375 6974 6528 2a2a 746d 705f 6578 7065  Suite(**tmp_expe
-00006810: 6374 6174 696f 6e5f 7375 6974 6529 0a20  ctation_suite). 
-00006820: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00006830: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00006840: 7970 6545 7272 6f72 280a 2020 2020 2020  ypeError(.      
-00006850: 2020 2020 2020 2020 2020 2254 6865 2070            "The p
-00006860: 726f 7669 6465 6420 6578 7065 6374 6174  rovided expectat
-00006870: 696f 6e20 7375 6974 6520 7479 7065 2060  ion suite type `
-00006880: 7b7d 6020 6973 206e 6f74 2073 7570 706f  {}` is not suppo
-00006890: 7274 6564 2e20 5573 6520 4772 6561 7420  rted. Use Great 
-000068a0: 4578 7065 6374 6174 696f 6e20 6045 7870  Expectation `Exp
-000068b0: 6563 7461 7469 6f6e 5375 6974 6560 206f  ectationSuite` o
-000068c0: 7220 4853 4653 2720 6f77 6e20 6045 7870  r HSFS' own `Exp
-000068d0: 6563 7461 7469 6f6e 5375 6974 6560 206f  ectationSuite` o
-000068e0: 626a 6563 742e 222e 666f 726d 6174 280a  bject.".format(.
-000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006900: 2020 2020 7479 7065 2865 7870 6563 7461      type(expecta
-00006910: 7469 6f6e 5f73 7569 7465 290a 2020 2020  tion_suite).    
-00006920: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00006930: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00006940: 2020 2020 2069 6620 6f76 6572 7772 6974       if overwrit
-00006950: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00006960: 656c 662e 6465 6c65 7465 5f65 7870 6563  elf.delete_expec
-00006970: 7461 7469 6f6e 5f73 7569 7465 2829 0a0a  tation_suite()..
-00006980: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00006990: 5f69 643a 0a20 2020 2020 2020 2020 2020  _id:.           
-000069a0: 2073 656c 662e 5f65 7870 6563 7461 7469   self._expectati
-000069b0: 6f6e 5f73 7569 7465 203d 2073 656c 662e  on_suite = self.
-000069c0: 5f65 7870 6563 7461 7469 6f6e 5f73 7569  _expectation_sui
-000069d0: 7465 5f65 6e67 696e 652e 7361 7665 280a  te_engine.save(.
-000069e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069f0: 746d 705f 6578 7065 6374 6174 696f 6e5f  tmp_expectation_
-00006a00: 7375 6974 650a 2020 2020 2020 2020 2020  suite.          
-00006a10: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00006a20: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
-00006a30: 6520 3d20 7365 6c66 2e5f 6578 7065 6374  e = self._expect
-00006a40: 6174 696f 6e5f 7375 6974 652e 746f 5f67  ation_suite.to_g
-00006a50: 655f 7479 7065 2829 0a20 2020 2020 2020  e_type().       
-00006a60: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00006a70: 2020 2023 2041 6464 6564 2074 6f20 6176     # Added to av
-00006a80: 6f69 6420 7468 726f 7769 6e67 2061 6e20  oid throwing an 
-00006a90: 6572 726f 7220 6966 2046 6561 7475 7265  error if Feature
-00006aa0: 2047 726f 7570 2069 7320 6e6f 7420 696e   Group is not in
-00006ab0: 6974 6961 6c69 7365 6420 7769 7468 2074  itialised with t
-00006ac0: 6865 2062 6163 6b65 6e64 0a20 2020 2020  he backend.     
-00006ad0: 2020 2020 2020 2073 656c 662e 5f65 7870         self._exp
-00006ae0: 6563 7461 7469 6f6e 5f73 7569 7465 203d  ectation_suite =
-00006af0: 2074 6d70 5f65 7870 6563 7461 7469 6f6e   tmp_expectation
-00006b00: 5f73 7569 7465 0a0a 2020 2020 6465 6620  _suite..    def 
-00006b10: 6465 6c65 7465 5f65 7870 6563 7461 7469  delete_expectati
-00006b20: 6f6e 5f73 7569 7465 2873 656c 6629 202d  on_suite(self) -
-00006b30: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00006b40: 2222 2244 656c 6574 6520 7468 6520 6578  """Delete the ex
-00006b50: 7065 6374 6174 696f 6e20 7375 6974 6520  pectation suite 
-00006b60: 6174 7461 6368 6564 2074 6f20 7468 6520  attached to the 
-00006b70: 4665 6174 7572 6520 4772 6f75 702e 0a0a  Feature Group...
-00006b80: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
-00006b90: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
-00006ba0: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-00006bb0: 2020 2020 2020 2320 636f 6e6e 6563 7420        # connect 
-00006bc0: 746f 2074 6865 2046 6561 7475 7265 2053  to the Feature S
-00006bd0: 746f 7265 0a20 2020 2020 2020 2020 2020  tore.           
-00006be0: 2066 7320 3d20 2e2e 2e0a 0a20 2020 2020   fs = .....     
-00006bf0: 2020 2020 2020 2023 2067 6574 2074 6865         # get the
-00006c00: 2046 6561 7475 7265 2047 726f 7570 2069   Feature Group i
-00006c10: 6e73 7461 6e63 650a 2020 2020 2020 2020  nstance.        
-00006c20: 2020 2020 6667 203d 2066 732e 6765 745f      fg = fs.get_
-00006c30: 6f72 5f63 7265 6174 655f 6665 6174 7572  or_create_featur
-00006c40: 655f 6772 6f75 7028 2e2e 2e29 0a0a 2020  e_group(...)..  
-00006c50: 2020 2020 2020 2020 2020 6667 2e64 656c            fg.del
-00006c60: 6574 655f 6578 7065 6374 6174 696f 6e5f  ete_expectation_
-00006c70: 7375 6974 6528 290a 2020 2020 2020 2020  suite().        
-00006c80: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
-00006c90: 2023 2052 6169 7365 730a 2020 2020 2020   # Raises.      
-00006ca0: 2020 2020 2020 6068 7366 732e 636c 6965        `hsfs.clie
-00006cb0: 6e74 2e65 7863 6570 7469 6f6e 732e 5265  nt.exceptions.Re
-00006cc0: 7374 4150 4945 7272 6f72 602e 0a20 2020  stAPIError`..   
-00006cd0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00006ce0: 2069 6620 7365 6c66 2e67 6574 5f65 7870   if self.get_exp
-00006cf0: 6563 7461 7469 6f6e 5f73 7569 7465 2829  ectation_suite()
-00006d00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00006d10: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00006d20: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
-00006d30: 655f 656e 6769 6e65 2e64 656c 6574 6528  e_engine.delete(
-00006d40: 7365 6c66 2e5f 6578 7065 6374 6174 696f  self._expectatio
-00006d50: 6e5f 7375 6974 652e 6964 290a 2020 2020  n_suite.id).    
-00006d60: 2020 2020 7365 6c66 2e5f 6578 7065 6374      self._expect
-00006d70: 6174 696f 6e5f 7375 6974 6520 3d20 4e6f  ation_suite = No
-00006d80: 6e65 0a0a 2020 2020 6465 6620 6765 745f  ne..    def get_
-00006d90: 6c61 7465 7374 5f76 616c 6964 6174 696f  latest_validatio
-00006da0: 6e5f 7265 706f 7274 280a 2020 2020 2020  n_report(.      
-00006db0: 2020 7365 6c66 2c20 6765 5f74 7970 653a    self, ge_type:
-00006dc0: 2062 6f6f 6c20 3d20 5472 7565 0a20 2020   bool = True.   
-00006dd0: 2029 202d 3e20 556e 696f 6e5b 5661 6c69   ) -> Union[Vali
-00006de0: 6461 7469 6f6e 5265 706f 7274 2c20 6765  dationReport, ge
-00006df0: 2e63 6f72 652e 4578 7065 6374 6174 696f  .core.Expectatio
-00006e00: 6e53 7569 7465 5661 6c69 6461 7469 6f6e  nSuiteValidation
-00006e10: 5265 7375 6c74 2c20 4e6f 6e65 5d3a 0a20  Result, None]:. 
-00006e20: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-00006e30: 2074 6865 206c 6174 6573 7420 7661 6c69   the latest vali
-00006e40: 6461 7469 6f6e 2072 6570 6f72 7420 6174  dation report at
-00006e50: 7461 6368 6564 2074 6f20 7468 6520 4665  tached to the Fe
-00006e60: 6174 7572 6520 4772 6f75 7020 6966 2069  ature Group if i
-00006e70: 7420 6578 6973 7473 2e0a 0a20 2020 2020  t exists...     
-00006e80: 2020 2021 2121 2065 7861 6d70 6c65 0a20     !!! example. 
-00006e90: 2020 2020 2020 2020 2020 2060 6060 7079             ```py
-00006ea0: 7468 6f6e 0a20 2020 2020 2020 2020 2020  thon.           
-00006eb0: 2023 2063 6f6e 6e65 6374 2074 6f20 7468   # connect to th
-00006ec0: 6520 4665 6174 7572 6520 5374 6f72 650a  e Feature Store.
-00006ed0: 2020 2020 2020 2020 2020 2020 6673 203d              fs =
-00006ee0: 202e 2e2e 0a0a 2020 2020 2020 2020 2020   .....          
-00006ef0: 2020 2320 6765 7420 7468 6520 4665 6174    # get the Feat
-00006f00: 7572 6520 4772 6f75 7020 696e 7374 616e  ure Group instan
-00006f10: 6365 0a20 2020 2020 2020 2020 2020 2066  ce.            f
-00006f20: 6720 3d20 6673 2e67 6574 5f6f 725f 6372  g = fs.get_or_cr
-00006f30: 6561 7465 5f66 6561 7475 7265 5f67 726f  eate_feature_gro
-00006f40: 7570 282e 2e2e 290a 0a20 2020 2020 2020  up(...)..       
-00006f50: 2020 2020 206c 6174 6573 745f 7661 6c5f       latest_val_
-00006f60: 7265 706f 7274 203d 2066 672e 6765 745f  report = fg.get_
-00006f70: 6c61 7465 7374 5f76 616c 6964 6174 696f  latest_validatio
-00006f80: 6e5f 7265 706f 7274 2829 0a20 2020 2020  n_report().     
-00006f90: 2020 2020 2020 2060 6060 0a0a 2020 2020         ```..    
-00006fa0: 2020 2020 2320 4172 6775 6d65 6e74 730a      # Arguments.
-00006fb0: 2020 2020 2020 2020 2020 2020 6765 5f74              ge_t
-00006fc0: 7970 653a 2049 6620 6054 7275 6560 2072  ype: If `True` r
-00006fd0: 6574 7572 6e73 2061 206e 6174 6976 6520  eturns a native 
-00006fe0: 4772 6561 7420 4578 7065 6374 6174 696f  Great Expectatio
-00006ff0: 6e20 7479 7065 2c20 486f 7073 776f 726b  n type, Hopswork
-00007000: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00007010: 2020 6375 7374 6f6d 2074 7970 6520 6f74    custom type ot
-00007020: 6865 7277 6973 652e 2043 6f6e 7665 7273  herwise. Convers
-00007030: 696f 6e20 6361 6e20 6265 2070 6572 666f  ion can be perfo
-00007040: 726d 6564 2076 6961 2074 6865 2060 746f  rmed via the `to
-00007050: 5f67 655f 7479 7065 2829 600a 2020 2020  _ge_type()`.    
-00007060: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
-00007070: 6f64 206f 6e20 686f 7073 776f 726b 7320  od on hopsworks 
-00007080: 7479 7065 2e20 4465 6661 756c 7473 2074  type. Defaults t
-00007090: 6f20 6054 7275 6560 2e0a 0a20 2020 2020  o `True`...     
-000070a0: 2020 2023 2052 6574 7572 6e73 0a20 2020     # Returns.   
-000070b0: 2020 2020 2020 2020 2060 5661 6c69 6461           `Valida
-000070c0: 7469 6f6e 5265 706f 7274 602e 2054 6865  tionReport`. The
-000070d0: 206c 6174 6573 7420 7661 6c69 6461 7469   latest validati
-000070e0: 6f6e 2072 6570 6f72 7420 6174 7461 6368  on report attach
-000070f0: 6564 2074 6f20 7468 6520 4665 6174 7572  ed to the Featur
-00007100: 6520 4772 6f75 702e 0a0a 2020 2020 2020  e Group...      
-00007110: 2020 2320 5261 6973 6573 0a20 2020 2020    # Raises.     
-00007120: 2020 2020 2020 2060 6873 6673 2e63 6c69         `hsfs.cli
-00007130: 656e 742e 6578 6365 7074 696f 6e73 2e52  ent.exceptions.R
-00007140: 6573 7441 5049 4572 726f 7260 2e0a 2020  estAPIError`..  
-00007150: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00007160: 2020 7265 7475 726e 2073 656c 662e 5f76    return self._v
-00007170: 616c 6964 6174 696f 6e5f 7265 706f 7274  alidation_report
-00007180: 5f65 6e67 696e 652e 6765 745f 6c61 7374  _engine.get_last
-00007190: 2867 655f 7479 7065 3d67 655f 7479 7065  (ge_type=ge_type
-000071a0: 290a 0a20 2020 2064 6566 2067 6574 5f61  )..    def get_a
-000071b0: 6c6c 5f76 616c 6964 6174 696f 6e5f 7265  ll_validation_re
-000071c0: 706f 7274 7328 0a20 2020 2020 2020 2073  ports(.        s
-000071d0: 656c 662c 2067 655f 7479 7065 3a20 626f  elf, ge_type: bo
-000071e0: 6f6c 203d 2054 7275 650a 2020 2020 2920  ol = True.    ) 
-000071f0: 2d3e 204c 6973 745b 556e 696f 6e5b 5661  -> List[Union[Va
-00007200: 6c69 6461 7469 6f6e 5265 706f 7274 2c20  lidationReport, 
-00007210: 6765 2e63 6f72 652e 4578 7065 6374 6174  ge.core.Expectat
-00007220: 696f 6e53 7569 7465 5661 6c69 6461 7469  ionSuiteValidati
-00007230: 6f6e 5265 7375 6c74 5d5d 3a0a 2020 2020  onResult]]:.    
-00007240: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
-00007250: 6520 6c61 7465 7374 2076 616c 6964 6174  e latest validat
-00007260: 696f 6e20 7265 706f 7274 2061 7474 6163  ion report attac
-00007270: 6865 6420 746f 2074 6865 2066 6561 7475  hed to the featu
-00007280: 7265 2067 726f 7570 2069 6620 6974 2065  re group if it e
-00007290: 7869 7374 732e 0a0a 2020 2020 2020 2020  xists...        
-000072a0: 2121 2120 6578 616d 706c 650a 2020 2020  !!! example.    
-000072b0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-000072c0: 6e0a 2020 2020 2020 2020 2020 2020 2320  n.            # 
-000072d0: 636f 6e6e 6563 7420 746f 2074 6865 2046  connect to the F
-000072e0: 6561 7475 7265 2053 746f 7265 0a20 2020  eature Store.   
-000072f0: 2020 2020 2020 2020 2066 7320 3d20 2e2e           fs = ..
-00007300: 2e0a 0a20 2020 2020 2020 2020 2020 2023  ...            #
-00007310: 2067 6574 2074 6865 2046 6561 7475 7265   get the Feature
-00007320: 2047 726f 7570 2069 6e73 7461 6e63 650a   Group instance.
-00007330: 2020 2020 2020 2020 2020 2020 6667 203d              fg =
-00007340: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
-00007350: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
-00007360: 2e2e 2e29 0a0a 2020 2020 2020 2020 2020  ...)..          
-00007370: 2020 7661 6c5f 7265 706f 7274 7320 3d20    val_reports = 
-00007380: 6667 2e67 6574 5f61 6c6c 5f76 616c 6964  fg.get_all_valid
-00007390: 6174 696f 6e5f 7265 706f 7274 7328 290a  ation_reports().
-000073a0: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
-000073b0: 0a20 2020 2020 2020 2023 2041 7267 756d  .        # Argum
-000073c0: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
-000073d0: 2067 655f 7479 7065 3a20 4966 2060 5472   ge_type: If `Tr
-000073e0: 7565 6020 7265 7475 726e 7320 6120 6e61  ue` returns a na
-000073f0: 7469 7665 2047 7265 6174 2045 7870 6563  tive Great Expec
-00007400: 7461 7469 6f6e 2074 7970 652c 2048 6f70  tation type, Hop
-00007410: 7377 6f72 6b73 0a20 2020 2020 2020 2020  sworks.         
-00007420: 2020 2020 2020 2063 7573 746f 6d20 7479         custom ty
-00007430: 7065 206f 7468 6572 7769 7365 2e20 436f  pe otherwise. Co
-00007440: 6e76 6572 7369 6f6e 2063 616e 2062 6520  nversion can be 
-00007450: 7065 7266 6f72 6d65 6420 7669 6120 7468  performed via th
-00007460: 6520 6074 6f5f 6765 5f74 7970 6528 2960  e `to_ge_type()`
-00007470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007480: 206d 6574 686f 6420 6f6e 2068 6f70 7377   method on hopsw
-00007490: 6f72 6b73 2074 7970 652e 2044 6566 6175  orks type. Defau
-000074a0: 6c74 7320 746f 2060 5472 7565 602e 0a0a  lts to `True`...
-000074b0: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
-000074c0: 730a 2020 2020 2020 2020 2020 2020 556e  s.            Un
-000074d0: 696f 6e5b 4c69 7374 5b60 5661 6c69 6461  ion[List[`Valida
-000074e0: 7469 6f6e 5265 706f 7274 605d 2c20 6056  tionReport`], `V
-000074f0: 616c 6964 6174 696f 6e52 6570 6f72 7460  alidationReport`
-00007500: 5d2e 2041 6c6c 2076 616c 6964 6174 696f  ]. All validatio
-00007510: 6e20 7265 706f 7274 7320 6174 7461 6368  n reports attach
-00007520: 6564 2074 6f20 7468 6520 6665 6174 7572  ed to the featur
-00007530: 6520 6772 6f75 702e 0a0a 2020 2020 2020  e group...      
-00007540: 2020 2320 5261 6973 6573 0a20 2020 2020    # Raises.     
-00007550: 2020 2020 2020 2060 6873 6673 2e63 6c69         `hsfs.cli
-00007560: 656e 742e 6578 6365 7074 696f 6e73 2e52  ent.exceptions.R
-00007570: 6573 7441 5049 4572 726f 7260 2e0a 2020  estAPIError`..  
-00007580: 2020 2020 2020 2020 2020 6068 7366 732e            `hsfs.
-00007590: 636c 6965 6e74 2e65 7863 6570 7469 6f6e  client.exception
-000075a0: 732e 4665 6174 7572 6553 746f 7265 4578  s.FeatureStoreEx
-000075b0: 6365 7074 696f 6e60 2e0a 2020 2020 2020  ception`..      
-000075c0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-000075d0: 2073 656c 662e 5f69 643a 0a20 2020 2020   self._id:.     
-000075e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000075f0: 6c66 2e5f 7661 6c69 6461 7469 6f6e 5f72  lf._validation_r
-00007600: 6570 6f72 745f 656e 6769 6e65 2e67 6574  eport_engine.get
-00007610: 5f61 6c6c 2867 655f 7479 7065 3d67 655f  _all(ge_type=ge_
-00007620: 7479 7065 290a 2020 2020 2020 2020 656c  type).        el
-00007630: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00007640: 7261 6973 6520 4665 6174 7572 6553 746f  raise FeatureSto
-00007650: 7265 4578 6365 7074 696f 6e28 0a20 2020  reException(.   
-00007660: 2020 2020 2020 2020 2020 2020 2022 4f6e               "On
-00007670: 6c79 2046 6561 7475 7265 2047 726f 7570  ly Feature Group
-00007680: 2072 6567 6973 7465 7265 6420 7769 7468   registered with
-00007690: 2048 6f70 7377 6f72 6b73 2063 616e 2066   Hopsworks can f
-000076a0: 6574 6368 2076 616c 6964 6174 696f 6e20  etch validation 
-000076b0: 7265 706f 7274 732e 220a 2020 2020 2020  reports.".      
-000076c0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-000076d0: 2073 6176 655f 7661 6c69 6461 7469 6f6e   save_validation
-000076e0: 5f72 6570 6f72 7428 0a20 2020 2020 2020  _report(.       
-000076f0: 2073 656c 662c 0a20 2020 2020 2020 2076   self,.        v
-00007700: 616c 6964 6174 696f 6e5f 7265 706f 7274  alidation_report
-00007710: 3a20 556e 696f 6e5b 0a20 2020 2020 2020  : Union[.       
-00007720: 2020 2020 2064 6963 742c 0a20 2020 2020       dict,.     
-00007730: 2020 2020 2020 2056 616c 6964 6174 696f         Validatio
-00007740: 6e52 6570 6f72 742c 0a20 2020 2020 2020  nReport,.       
-00007750: 2020 2020 2067 652e 636f 7265 2e65 7870       ge.core.exp
-00007760: 6563 7461 7469 6f6e 5f76 616c 6964 6174  ectation_validat
-00007770: 696f 6e5f 7265 7375 6c74 2e45 7870 6563  ion_result.Expec
-00007780: 7461 7469 6f6e 5375 6974 6556 616c 6964  tationSuiteValid
-00007790: 6174 696f 6e52 6573 756c 742c 0a20 2020  ationResult,.   
-000077a0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-000077b0: 696e 6765 7374 696f 6e5f 7265 7375 6c74  ingestion_result
-000077c0: 3a20 7374 7220 3d20 2255 4e4b 4e4f 574e  : str = "UNKNOWN
-000077d0: 222c 0a20 2020 2020 2020 2067 655f 7479  ",.        ge_ty
-000077e0: 7065 3a20 626f 6f6c 203d 2054 7275 652c  pe: bool = True,
-000077f0: 0a20 2020 2029 202d 3e20 556e 696f 6e5b  .    ) -> Union[
-00007800: 5661 6c69 6461 7469 6f6e 5265 706f 7274  ValidationReport
-00007810: 2c20 6765 2e63 6f72 652e 4578 7065 6374  , ge.core.Expect
-00007820: 6174 696f 6e53 7569 7465 5661 6c69 6461  ationSuiteValida
-00007830: 7469 6f6e 5265 7375 6c74 5d3a 0a20 2020  tionResult]:.   
-00007840: 2020 2020 2022 2222 5361 7665 2076 616c       """Save val
-00007850: 6964 6174 696f 6e20 7265 706f 7274 2074  idation report t
-00007860: 6f20 686f 7073 776f 726b 7320 706c 6174  o hopsworks plat
-00007870: 666f 726d 2061 6c6f 6e67 2070 7265 7669  form along previ
-00007880: 6f75 7320 7265 706f 7274 7320 6f66 2074  ous reports of t
-00007890: 6865 2073 616d 6520 4665 6174 7572 6520  he same Feature 
-000078a0: 4772 6f75 702e 0a0a 2020 2020 2020 2020  Group...        
-000078b0: 2121 2120 6578 616d 706c 650a 2020 2020  !!! example.    
-000078c0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-000078d0: 6e0a 2020 2020 2020 2020 2020 2020 2320  n.            # 
-000078e0: 636f 6e6e 6563 7420 746f 2074 6865 2046  connect to the F
-000078f0: 6561 7475 7265 2053 746f 7265 0a20 2020  eature Store.   
-00007900: 2020 2020 2020 2020 2066 7320 3d20 2e2e           fs = ..
-00007910: 2e0a 0a20 2020 2020 2020 2020 2020 2023  ...            #
-00007920: 2067 6574 2074 6865 2046 6561 7475 7265   get the Feature
-00007930: 2047 726f 7570 2069 6e73 7461 6e63 650a   Group instance.
-00007940: 2020 2020 2020 2020 2020 2020 6667 203d              fg =
-00007950: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
-00007960: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
-00007970: 2e2e 2e2c 2065 7870 6563 7461 7469 6f6e  ..., expectation
-00007980: 5f73 7569 7465 3d65 7870 6563 7461 7469  _suite=expectati
-00007990: 6f6e 5f73 7569 7465 290a 0a20 2020 2020  on_suite)..     
-000079a0: 2020 2020 2020 2076 616c 6964 6174 696f         validatio
-000079b0: 6e5f 7265 706f 7274 203d 2067 7265 6174  n_report = great
-000079c0: 5f65 7870 6563 7461 7469 6f6e 732e 6672  _expectations.fr
-000079d0: 6f6d 5f70 616e 6461 7328 0a20 2020 2020  om_pandas(.     
-000079e0: 2020 2020 2020 2020 2020 206d 795f 6578             my_ex
-000079f0: 7065 7269 6d65 6e74 616c 5f66 6561 7475  perimental_featu
-00007a00: 7265 735f 6466 2c0a 2020 2020 2020 2020  res_df,.        
-00007a10: 2020 2020 2020 2020 6667 2e67 6574 5f65          fg.get_e
-00007a20: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-00007a30: 2829 292e 7661 6c69 6461 7465 2829 0a0a  ()).validate()..
-00007a40: 2020 2020 2020 2020 2020 2020 6667 2e73              fg.s
-00007a50: 6176 655f 7661 6c69 6461 7469 6f6e 5f72  ave_validation_r
-00007a60: 6570 6f72 7428 7661 6c69 6461 7469 6f6e  eport(validation
-00007a70: 5f72 6570 6f72 742c 2069 6e67 6573 7469  _report, ingesti
-00007a80: 6f6e 5f72 6573 756c 743d 2245 5850 4552  on_result="EXPER
-00007a90: 494d 454e 5422 290a 2020 2020 2020 2020  IMENT").        
-00007aa0: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
-00007ab0: 2023 2041 7267 756d 656e 7473 0a20 2020   # Arguments.   
-00007ac0: 2020 2020 2020 2020 2076 616c 6964 6174           validat
-00007ad0: 696f 6e5f 7265 706f 7274 3a20 5468 6520  ion_report: The 
-00007ae0: 7661 6c69 6461 7469 6f6e 2072 6570 6f72  validation repor
-00007af0: 7420 746f 2061 7474 6163 6820 746f 2074  t to attach to t
-00007b00: 6865 2046 6561 7475 7265 2047 726f 7570  he Feature Group
-00007b10: 2e0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-00007b20: 6765 7374 696f 6e5f 7265 7375 6c74 3a20  gestion_result: 
-00007b30: 5370 6563 6966 7920 7468 6520 6661 7465  Specify the fate
-00007b40: 206f 6620 7468 6520 6173 736f 6369 6174   of the associat
-00007b50: 6564 2064 6174 612c 2064 6566 6175 6c74  ed data, default
-00007b60: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00007b70: 2020 746f 2022 554e 4b4e 4f57 4e22 2e20    to "UNKNOWN". 
-00007b80: 5375 7070 6f72 7465 6420 6f70 7469 6f6e  Supported option
-00007b90: 7320 6172 6520 2022 554e 4b4e 4f57 4e22  s are  "UNKNOWN"
-00007ba0: 2c20 2249 4e47 4553 5445 4422 2c20 2252  , "INGESTED", "R
-00007bb0: 454a 4543 5445 4422 2c0a 2020 2020 2020  EJECTED",.      
-00007bc0: 2020 2020 2020 2020 2020 2245 5850 4552            "EXPER
-00007bd0: 494d 454e 5422 2c20 2246 475f 4441 5441  IMENT", "FG_DATA
-00007be0: 222e 2055 7365 2022 494e 4745 5354 4544  ". Use "INGESTED
-00007bf0: 2220 6f72 2022 5245 4a45 4354 4544 2220  " or "REJECTED" 
-00007c00: 666f 7220 7661 6c69 6461 7469 6f6e 0a20  for validation. 
-00007c10: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00007c20: 6620 4461 7461 4672 616d 6573 2074 6f20  f DataFrames to 
-00007c30: 6265 2069 6e73 6572 7465 6420 696e 2074  be inserted in t
-00007c40: 6865 2046 6561 7475 7265 2047 726f 7570  he Feature Group
-00007c50: 2e20 5573 6520 2245 5850 4552 494d 454e  . Use "EXPERIMEN
-00007c60: 5422 0a20 2020 2020 2020 2020 2020 2020  T".             
-00007c70: 2020 2066 6f72 2074 6573 7469 6e67 2061     for testing a
-00007c80: 6e64 2064 6576 656c 6f70 6d65 6e74 2061  nd development a
-00007c90: 6e64 2022 4647 5f44 4154 4122 2077 6865  nd "FG_DATA" whe
-00007ca0: 6e20 7661 6c69 6461 7469 6e67 2064 6174  n validating dat
-00007cb0: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
-00007cc0: 2020 616c 7265 6164 7920 696e 2074 6865    already in the
-00007cd0: 2046 6561 7475 7265 2047 726f 7570 2e0a   Feature Group..
-00007ce0: 2020 2020 2020 2020 2020 2020 6765 5f74              ge_t
-00007cf0: 7970 653a 2049 6620 6054 7275 6560 2072  ype: If `True` r
-00007d00: 6574 7572 6e73 2061 206e 6174 6976 6520  eturns a native 
-00007d10: 4772 6561 7420 4578 7065 6374 6174 696f  Great Expectatio
-00007d20: 6e20 7479 7065 2c20 486f 7073 776f 726b  n type, Hopswork
-00007d30: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00007d40: 2020 6375 7374 6f6d 2074 7970 6520 6f74    custom type ot
-00007d50: 6865 7277 6973 652e 2043 6f6e 7665 7273  herwise. Convers
-00007d60: 696f 6e20 6361 6e20 6265 2070 6572 666f  ion can be perfo
-00007d70: 726d 6564 2076 6961 2074 6865 2060 746f  rmed via the `to
-00007d80: 5f67 655f 7479 7065 2829 600a 2020 2020  _ge_type()`.    
-00007d90: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
-00007da0: 6f64 206f 6e20 686f 7073 776f 726b 7320  od on hopsworks 
-00007db0: 7479 7065 2e20 4465 6661 756c 7473 2074  type. Defaults t
-00007dc0: 6f20 6054 7275 6560 2e0a 0a20 2020 2020  o `True`...     
-00007dd0: 2020 2023 2052 6169 7365 730a 2020 2020     # Raises.    
-00007de0: 2020 2020 2020 2020 6068 7366 732e 636c          `hsfs.cl
-00007df0: 6965 6e74 2e65 7863 6570 7469 6f6e 732e  ient.exceptions.
-00007e00: 5265 7374 4150 4945 7272 6f72 602e 0a20  RestAPIError`.. 
-00007e10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00007e20: 2020 2069 6620 7365 6c66 2e5f 6964 3a0a     if self._id:.
-00007e30: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00007e40: 7369 6e73 7461 6e63 6528 0a20 2020 2020  sinstance(.     
-00007e50: 2020 2020 2020 2020 2020 2076 616c 6964             valid
-00007e60: 6174 696f 6e5f 7265 706f 7274 2c0a 2020  ation_report,.  
-00007e70: 2020 2020 2020 2020 2020 2020 2020 6765                ge
-00007e80: 2e63 6f72 652e 6578 7065 6374 6174 696f  .core.expectatio
-00007e90: 6e5f 7661 6c69 6461 7469 6f6e 5f72 6573  n_validation_res
-00007ea0: 756c 742e 4578 7065 6374 6174 696f 6e53  ult.ExpectationS
-00007eb0: 7569 7465 5661 6c69 6461 7469 6f6e 5265  uiteValidationRe
-00007ec0: 7375 6c74 2c0a 2020 2020 2020 2020 2020  sult,.          
-00007ed0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-00007ee0: 2020 2020 2072 6570 6f72 7420 3d20 5661       report = Va
-00007ef0: 6c69 6461 7469 6f6e 5265 706f 7274 280a  lidationReport(.
-00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f10: 2020 2020 2a2a 7661 6c69 6461 7469 6f6e      **validation
-00007f20: 5f72 6570 6f72 742e 746f 5f6a 736f 6e5f  _report.to_json_
-00007f30: 6469 6374 2829 2c0a 2020 2020 2020 2020  dict(),.        
-00007f40: 2020 2020 2020 2020 2020 2020 696e 6765              inge
-00007f50: 7374 696f 6e5f 7265 7375 6c74 3d69 6e67  stion_result=ing
-00007f60: 6573 7469 6f6e 5f72 6573 756c 742c 0a20  estion_result,. 
-00007f70: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00007f80: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00007f90: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
-00007fa0: 6964 6174 696f 6e5f 7265 706f 7274 2c20  idation_report, 
-00007fb0: 6469 6374 293a 0a20 2020 2020 2020 2020  dict):.         
-00007fc0: 2020 2020 2020 2072 6570 6f72 7420 3d20         report = 
-00007fd0: 5661 6c69 6461 7469 6f6e 5265 706f 7274  ValidationReport
-00007fe0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00007ff0: 2020 2020 2020 2a2a 7661 6c69 6461 7469        **validati
-00008000: 6f6e 5f72 6570 6f72 742c 2069 6e67 6573  on_report, inges
-00008010: 7469 6f6e 5f72 6573 756c 743d 696e 6765  tion_result=inge
-00008020: 7374 696f 6e5f 7265 7375 6c74 0a20 2020  stion_result.   
-00008030: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00008040: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00008050: 6973 696e 7374 616e 6365 2876 616c 6964  isinstance(valid
-00008060: 6174 696f 6e5f 7265 706f 7274 2c20 5661  ation_report, Va
-00008070: 6c69 6461 7469 6f6e 5265 706f 7274 293a  lidationReport):
-00008080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008090: 2072 6570 6f72 7420 3d20 7661 6c69 6461   report = valida
-000080a0: 7469 6f6e 5f72 6570 6f72 740a 2020 2020  tion_report.    
-000080b0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-000080c0: 6e67 6573 7469 6f6e 5f72 6573 756c 7420  ngestion_result 
-000080d0: 213d 2022 554e 4b4e 4f57 4e22 3a0a 2020  != "UNKNOWN":.  
-000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080f0: 2020 7265 706f 7274 2e69 6e67 6573 7469    report.ingesti
-00008100: 6f6e 5f72 6573 756c 7420 3d20 696e 6765  on_result = inge
-00008110: 7374 696f 6e5f 7265 7375 6c74 0a0a 2020  stion_result..  
-00008120: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00008130: 2073 656c 662e 5f76 616c 6964 6174 696f   self._validatio
-00008140: 6e5f 7265 706f 7274 5f65 6e67 696e 652e  n_report_engine.
-00008150: 7361 7665 280a 2020 2020 2020 2020 2020  save(.          
-00008160: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
-00008170: 5f72 6570 6f72 743d 7265 706f 7274 2c20  _report=report, 
-00008180: 6765 5f74 7970 653d 6765 5f74 7970 650a  ge_type=ge_type.
-00008190: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000081a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000081b0: 2020 2020 2020 2020 7261 6973 6520 4665          raise Fe
-000081c0: 6174 7572 6553 746f 7265 4578 6365 7074  atureStoreExcept
-000081d0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-000081e0: 2020 2020 2022 4f6e 6c79 2046 6561 7475       "Only Featu
-000081f0: 7265 2047 726f 7570 2072 6567 6973 7465  re Group registe
-00008200: 7265 6420 7769 7468 2048 6f70 7377 6f72  red with Hopswor
-00008210: 6b73 2063 616e 2075 706c 6f61 6420 7661  ks can upload va
-00008220: 6c69 6461 7469 6f6e 2072 6570 6f72 7473  lidation reports
-00008230: 2e22 0a20 2020 2020 2020 2020 2020 2029  .".            )
-00008240: 0a0a 2020 2020 6465 6620 6765 745f 7661  ..    def get_va
-00008250: 6c69 6461 7469 6f6e 5f68 6973 746f 7279  lidation_history
-00008260: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00008270: 2020 2020 2020 2020 6578 7065 6374 6174          expectat
-00008280: 696f 6e5f 6964 3a20 696e 742c 0a20 2020  ion_id: int,.   
-00008290: 2020 2020 2073 7461 7274 5f76 616c 6964       start_valid
-000082a0: 6174 696f 6e5f 7469 6d65 3a20 556e 696f  ation_time: Unio
-000082b0: 6e5b 7374 722c 2069 6e74 2c20 6461 7465  n[str, int, date
-000082c0: 7469 6d65 2c20 6461 7465 2c20 4e6f 6e65  time, date, None
-000082d0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-000082e0: 2020 656e 645f 7661 6c69 6461 7469 6f6e    end_validation
-000082f0: 5f74 696d 653a 2055 6e69 6f6e 5b73 7472  _time: Union[str
-00008300: 2c20 696e 742c 2064 6174 6574 696d 652c  , int, datetime,
-00008310: 2064 6174 652c 204e 6f6e 655d 203d 204e   date, None] = N
-00008320: 6f6e 652c 0a20 2020 2020 2020 2066 696c  one,.        fil
-00008330: 7465 725f 6279 3a20 4c69 7374 5b73 7472  ter_by: List[str
-00008340: 5d20 3d20 5b5d 2c0a 2020 2020 2020 2020  ] = [],.        
-00008350: 6765 5f74 7970 653a 2062 6f6f 6c20 3d20  ge_type: bool = 
-00008360: 5472 7565 2c0a 2020 2020 2920 2d3e 2055  True,.    ) -> U
-00008370: 6e69 6f6e 5b4c 6973 745b 5661 6c69 6461  nion[List[Valida
-00008380: 7469 6f6e 5265 7375 6c74 5d2c 204c 6973  tionResult], Lis
-00008390: 745b 6765 2e63 6f72 652e 4578 7065 6374  t[ge.core.Expect
-000083a0: 6174 696f 6e56 616c 6964 6174 696f 6e52  ationValidationR
-000083b0: 6573 756c 745d 5d3a 0a20 2020 2020 2020  esult]]:.       
-000083c0: 2022 2222 4665 7463 6820 7661 6c69 6461   """Fetch valida
-000083d0: 7469 6f6e 2068 6973 746f 7279 206f 6620  tion history of 
-000083e0: 616e 2045 7870 6563 7461 7469 6f6e 2073  an Expectation s
-000083f0: 7065 6369 6669 6564 2062 7920 6974 7320  pecified by its 
-00008400: 6964 2e0a 0a20 2020 2020 2020 2021 2121  id...        !!!
-00008410: 2065 7861 6d70 6c65 0a20 2020 2020 2020   example.       
-00008420: 2060 6060 7079 7468 6f6e 330a 2020 2020   ```python3.    
-00008430: 2020 2020 7661 6c69 6461 7469 6f6e 5f68      validation_h
-00008440: 6973 746f 7279 203d 2066 672e 6765 745f  istory = fg.get_
-00008450: 7661 6c69 6461 7469 6f6e 5f68 6973 746f  validation_histo
-00008460: 7279 280a 2020 2020 2020 2020 2020 2020  ry(.            
-00008470: 6578 7065 6374 6174 696f 6e5f 6964 3d31  expectation_id=1
-00008480: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
-00008490: 6c74 6572 5f62 793d 5b22 5245 4a45 4354  lter_by=["REJECT
-000084a0: 4544 222c 2022 554e 4b4e 4f57 4e22 5d2c  ED", "UNKNOWN"],
-000084b0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-000084c0: 7274 5f76 616c 6964 6174 696f 6e5f 7469  rt_validation_ti
-000084d0: 6d65 3d22 3230 3232 2d30 312d 3031 2030  me="2022-01-01 0
-000084e0: 303a 3030 3a30 3022 2c0a 2020 2020 2020  0:00:00",.      
-000084f0: 2020 2020 2020 656e 645f 7661 6c69 6461        end_valida
-00008500: 7469 6f6e 5f74 696d 653d 6461 7465 7469  tion_time=dateti
-00008510: 6d65 2e64 6174 6574 696d 652e 6e6f 7728  me.datetime.now(
-00008520: 292c 0a20 2020 2020 2020 2020 2020 2067  ),.            g
-00008530: 655f 7479 7065 3d46 616c 7365 0a20 2020  e_type=False.   
-00008540: 2020 2020 2029 0a20 2020 2020 2020 2060       ).        `
-00008550: 6060 0a0a 2020 2020 2020 2020 2320 4172  ``..        # Ar
-00008560: 6775 6d65 6e74 730a 2020 2020 2020 2020  guments.        
-00008570: 2020 2020 6578 7065 6374 6174 696f 6e5f      expectation_
-00008580: 6964 3a20 6964 206f 6620 7468 6520 4578  id: id of the Ex
-00008590: 7065 6374 6174 696f 6e20 666f 7220 7768  pectation for wh
-000085a0: 6963 6820 746f 2066 6574 6368 2074 6865  ich to fetch the
-000085b0: 2076 616c 6964 6174 696f 6e20 6869 7374   validation hist
-000085c0: 6f72 790a 2020 2020 2020 2020 2020 2020  ory.            
-000085d0: 6669 6c74 6572 5f62 793a 206c 6973 7420  filter_by: list 
-000085e0: 6f66 2069 6e67 6573 7469 6f6e 5f72 6573  of ingestion_res
-000085f0: 756c 7420 6361 7465 676f 7279 2074 6f20  ult category to 
-00008600: 6b65 6570 2e20 4f6f 7074 696f 6e73 2061  keep. Ooptions a
-00008610: 7265 2022 494e 4745 5354 4544 222c 2022  re "INGESTED", "
-00008620: 5245 4a45 4354 4544 222c 2022 4647 5f44  REJECTED", "FG_D
-00008630: 4154 4122 2c20 2245 5850 4552 494d 454e  ATA", "EXPERIMEN
-00008640: 5422 2c20 2255 4e4b 4e4f 574e 222e 0a20  T", "UNKNOWN".. 
-00008650: 2020 2020 2020 2020 2020 2073 7461 7274             start
-00008660: 5f76 616c 6964 6174 696f 6e5f 7469 6d65  _validation_time
-00008670: 3a20 6665 7463 6820 6f6e 6c79 2076 616c  : fetch only val
-00008680: 6964 6174 696f 6e20 7265 7375 6c74 2070  idation result p
-00008690: 6f73 7465 7269 6f72 2074 6f20 7468 6520  osterior to the 
-000086a0: 7072 6f76 6964 6564 2074 696d 652c 2069  provided time, i
-000086b0: 6e63 6c75 7369 7665 2e0a 2020 2020 2020  nclusive..      
-000086c0: 2020 2020 2020 5375 7070 6f72 7465 6420        Supported 
-000086d0: 666f 726d 6174 2069 6e63 6c75 6465 2074  format include t
-000086e0: 696d 6573 7461 6d70 7328 696e 7429 2c20  imestamps(int), 
-000086f0: 6461 7465 7469 6d65 2c20 6461 7465 206f  datetime, date o
-00008700: 7220 7374 7269 6e67 2066 6f72 6d61 7474  r string formatt
-00008710: 6564 2074 6f20 6265 2064 6174 7574 696c  ed to be datutil
-00008720: 7320 7061 7273 6162 6c65 2e20 5365 6520  s parsable. See 
-00008730: 6578 616d 706c 6573 2061 626f 7665 2e0a  examples above..
-00008740: 2020 2020 2020 2020 2020 2020 656e 645f              end_
-00008750: 7661 6c69 6461 7469 6f6e 5f74 696d 653a  validation_time:
-00008760: 2066 6574 6368 206f 6e6c 7920 7661 6c69   fetch only vali
-00008770: 6461 7469 6f6e 2072 6573 756c 7420 7072  dation result pr
-00008780: 696f 7220 746f 2074 6865 2070 726f 7669  ior to the provi
-00008790: 6465 6420 7469 6d65 2c20 696e 636c 7573  ded time, inclus
-000087a0: 6976 652e 0a20 2020 2020 2020 2020 2020  ive..           
-000087b0: 2053 7570 706f 7274 6564 2066 6f72 6d61   Supported forma
-000087c0: 7420 696e 636c 7564 6520 7469 6d65 7374  t include timest
-000087d0: 616d 7073 2869 6e74 292c 2064 6174 6574  amps(int), datet
-000087e0: 696d 652c 2064 6174 6520 6f72 2073 7472  ime, date or str
-000087f0: 696e 6720 666f 726d 6174 7465 6420 746f  ing formatted to
-00008800: 2062 6520 6461 7475 7469 6c73 2070 6172   be datutils par
-00008810: 7361 626c 652e 2053 6565 2065 7861 6d70  sable. See examp
-00008820: 6c65 7320 6162 6f76 652e 0a0a 2020 2020  les above...    
-00008830: 2020 2020 2320 5261 6973 6573 0a20 2020      # Raises.   
-00008840: 2020 2020 2020 2020 2060 6873 6673 2e63           `hsfs.c
-00008850: 6c69 656e 742e 6578 6365 7074 696f 6e73  lient.exceptions
-00008860: 2e52 6573 7441 5049 4572 726f 7260 2e0a  .RestAPIError`..
-00008870: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
-00008880: 6e0a 2020 2020 2020 2020 2020 2020 556e  n.            Un
-00008890: 696f 6e5b 4c69 7374 5b60 5661 6c69 6461  ion[List[`Valida
-000088a0: 7469 6f6e 5265 7375 6c74 605d 2c20 4c69  tionResult`], Li
-000088b0: 7374 5b60 4578 7065 6374 6174 696f 6e56  st[`ExpectationV
-000088c0: 616c 6964 6174 696f 6e52 6573 756c 7460  alidationResult`
-000088d0: 5d5d 2041 206c 6973 7420 6f66 2076 616c  ]] A list of val
-000088e0: 6964 6174 696f 6e20 7265 7375 6c74 2063  idation result c
-000088f0: 6f6e 6e65 6374 6564 2074 6f20 7468 6520  onnected to the 
-00008900: 6578 7065 6374 6174 696f 6e5f 6964 0a20  expectation_id. 
-00008910: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00008920: 2020 206d 616a 6f72 2c20 6d69 6e6f 7220     major, minor 
-00008930: 3d20 7365 6c66 2e5f 7661 7269 6162 6c65  = self._variable
-00008940: 5f61 7069 2e70 6172 7365 5f6d 616a 6f72  _api.parse_major
-00008950: 5f61 6e64 5f6d 696e 6f72 280a 2020 2020  _and_minor(.    
-00008960: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
-00008970: 7269 6162 6c65 5f61 7069 2e67 6574 5f76  riable_api.get_v
-00008980: 6572 7369 6f6e 2822 686f 7073 776f 726b  ersion("hopswork
-00008990: 7322 290a 2020 2020 2020 2020 290a 2020  s").        ).  
-000089a0: 2020 2020 2020 6966 206d 616a 6f72 203d        if major =
-000089b0: 3d20 2233 2220 616e 6420 6d69 6e6f 7220  = "3" and minor 
-000089c0: 3d3d 2022 3022 3a0a 2020 2020 2020 2020  == "0":.        
-000089d0: 2020 2020 7261 6973 6520 4665 6174 7572      raise Featur
-000089e0: 6553 746f 7265 4578 6365 7074 696f 6e28  eStoreException(
-000089f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008a00: 2022 5468 6520 686f 7073 776f 726b 7320   "The hopsworks 
-00008a10: 7365 7276 6572 2064 6f65 7320 6e6f 7420  server does not 
-00008a20: 7375 7070 6f72 7420 7468 6973 206f 7065  support this ope
-00008a30: 7261 7469 6f6e 2e20 5570 6461 7465 2073  ration. Update s
-00008a40: 6572 7665 7220 746f 2068 6f70 7377 6f72  erver to hopswor
-00008a50: 6b73 203e 332e 3120 746f 2065 6e61 626c  ks >3.1 to enabl
-00008a60: 6520 7375 7070 6f72 742e 220a 2020 2020  e support.".    
-00008a70: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00008a80: 2020 2069 6620 7365 6c66 2e5f 6964 3a0a     if self._id:.
-00008a90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00008aa0: 726e 2073 656c 662e 5f76 616c 6964 6174  rn self._validat
-00008ab0: 696f 6e5f 7265 7375 6c74 5f65 6e67 696e  ion_result_engin
-00008ac0: 652e 6765 745f 7661 6c69 6461 7469 6f6e  e.get_validation
-00008ad0: 5f68 6973 746f 7279 280a 2020 2020 2020  _history(.      
-00008ae0: 2020 2020 2020 2020 2020 6578 7065 6374            expect
-00008af0: 6174 696f 6e5f 6964 3d65 7870 6563 7461  ation_id=expecta
-00008b00: 7469 6f6e 5f69 642c 0a20 2020 2020 2020  tion_id,.       
-00008b10: 2020 2020 2020 2020 2073 7461 7274 5f76           start_v
-00008b20: 616c 6964 6174 696f 6e5f 7469 6d65 3d73  alidation_time=s
-00008b30: 7461 7274 5f76 616c 6964 6174 696f 6e5f  tart_validation_
-00008b40: 7469 6d65 2c0a 2020 2020 2020 2020 2020  time,.          
-00008b50: 2020 2020 2020 656e 645f 7661 6c69 6461        end_valida
-00008b60: 7469 6f6e 5f74 696d 653d 656e 645f 7661  tion_time=end_va
-00008b70: 6c69 6461 7469 6f6e 5f74 696d 652c 0a20  lidation_time,. 
-00008b80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00008b90: 696c 7465 725f 6279 3d66 696c 7465 725f  ilter_by=filter_
-00008ba0: 6279 2c0a 2020 2020 2020 2020 2020 2020  by,.            
-00008bb0: 2020 2020 6765 5f74 7970 653d 6765 5f74      ge_type=ge_t
-00008bc0: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
-00008bd0: 2029 0a20 2020 2020 2020 2065 6c73 653a   ).        else:
-00008be0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00008bf0: 7365 2046 6561 7475 7265 5374 6f72 6545  se FeatureStoreE
-00008c00: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
-00008c10: 2020 2020 2020 2020 2020 224f 6e6c 7920            "Only 
-00008c20: 4665 6174 7572 6520 4772 6f75 7020 7265  Feature Group re
-00008c30: 6769 7374 6572 6564 2077 6974 6820 486f  gistered with Ho
-00008c40: 7073 776f 726b 7320 6361 6e20 6665 7463  psworks can fetc
-00008c50: 6820 7661 6c69 6461 7469 6f6e 2068 6973  h validation his
-00008c60: 746f 7279 2e22 0a20 2020 2020 2020 2020  tory.".         
-00008c70: 2020 2029 0a0a 2020 2020 6465 6620 5f5f     )..    def __
-00008c80: 6765 7461 7474 725f 5f28 7365 6c66 2c20  getattr__(self, 
-00008c90: 6e61 6d65 293a 0a20 2020 2020 2020 2074  name):.        t
-00008ca0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00008cb0: 7265 7475 726e 2073 656c 662e 5f5f 6765  return self.__ge
-00008cc0: 7469 7465 6d5f 5f28 6e61 6d65 290a 2020  titem__(name).  
-00008cd0: 2020 2020 2020 6578 6365 7074 204b 6579        except Key
-00008ce0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-00008cf0: 2020 2072 6169 7365 2041 7474 7269 6275     raise Attribu
-00008d00: 7465 4572 726f 7228 0a20 2020 2020 2020  teError(.       
-00008d10: 2020 2020 2020 2020 2066 2227 4665 6174           f"'Feat
-00008d20: 7572 6547 726f 7570 2720 6f62 6a65 6374  ureGroup' object
-00008d30: 2068 6173 206e 6f20 6174 7472 6962 7574   has no attribut
-00008d40: 6520 277b 6e61 6d65 7d27 2e20 220a 2020  e '{name}'. ".  
-00008d50: 2020 2020 2020 2020 2020 2020 2020 2249                "I
-00008d60: 6620 796f 7520 6172 6520 7472 7969 6e67  f you are trying
-00008d70: 2074 6f20 6163 6365 7373 2061 2066 6561   to access a fea
-00008d80: 7475 7265 2c20 6661 6c6c 2062 6163 6b20  ture, fall back 
-00008d90: 6f6e 2022 0a20 2020 2020 2020 2020 2020  on ".           
-00008da0: 2020 2020 2022 7573 696e 6720 7468 6520       "using the 
-00008db0: 6067 6574 5f66 6561 7475 7265 6020 6d65  `get_feature` me
-00008dc0: 7468 6f64 2e22 0a20 2020 2020 2020 2020  thod.".         
-00008dd0: 2020 2029 0a0a 2020 2020 6465 6620 5f5f     )..    def __
-00008de0: 6765 7469 7465 6d5f 5f28 7365 6c66 2c20  getitem__(self, 
-00008df0: 6e61 6d65 293a 0a20 2020 2020 2020 2069  name):.        i
-00008e00: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-00008e10: 286e 616d 652c 2073 7472 293a 0a20 2020  (name, str):.   
-00008e20: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00008e30: 7970 6545 7272 6f72 280a 2020 2020 2020  ypeError(.      
-00008e40: 2020 2020 2020 2020 2020 6622 4578 7065            f"Expe
-00008e50: 6374 6564 2074 7970 6520 6073 7472 602c  cted type `str`,
-00008e60: 2067 6f74 2060 7b74 7970 6528 6e61 6d65   got `{type(name
-00008e70: 297d 602e 2022 0a20 2020 2020 2020 2020  )}`. ".         
-00008e80: 2020 2020 2020 2022 4665 6174 7572 6573         "Features
-00008e90: 2061 7265 2061 6363 6573 7369 626c 6520   are accessible 
-00008ea0: 6279 206e 616d 652e 220a 2020 2020 2020  by name.".      
-00008eb0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00008ec0: 6665 6174 7572 6520 3d20 5b66 2066 6f72  feature = [f for
-00008ed0: 2066 2069 6e20 7365 6c66 2e5f 5f67 6574   f in self.__get
-00008ee0: 6174 7472 6962 7574 655f 5f28 225f 6665  attribute__("_fe
-00008ef0: 6174 7572 6573 2229 2069 6620 662e 6e61  atures") if f.na
-00008f00: 6d65 203d 3d20 6e61 6d65 5d0a 2020 2020  me == name].    
-00008f10: 2020 2020 6966 206c 656e 2866 6561 7475      if len(featu
-00008f20: 7265 2920 3d3d 2031 3a0a 2020 2020 2020  re) == 1:.      
-00008f30: 2020 2020 2020 7265 7475 726e 2066 6561        return fea
-00008f40: 7475 7265 5b30 5d0a 2020 2020 2020 2020  ture[0].        
-00008f50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00008f60: 2020 7261 6973 6520 4b65 7945 7272 6f72    raise KeyError
-00008f70: 2866 2227 4665 6174 7572 6547 726f 7570  (f"'FeatureGroup
-00008f80: 2720 6f62 6a65 6374 2068 6173 206e 6f20  ' object has no 
-00008f90: 6665 6174 7572 6520 6361 6c6c 6564 2027  feature called '
-00008fa0: 7b6e 616d 657d 272e 2229 0a0a 2020 2020  {name}'.")..    
-00008fb0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00008fc0: 6620 7374 6174 6973 7469 6373 5f63 6f6e  f statistics_con
-00008fd0: 6669 6728 7365 6c66 293a 0a20 2020 2020  fig(self):.     
-00008fe0: 2020 2022 2222 5374 6174 6973 7469 6373     """Statistics
-00008ff0: 2063 6f6e 6669 6775 7261 7469 6f6e 206f   configuration o
-00009000: 626a 6563 7420 6465 6669 6e69 6e67 2074  bject defining t
-00009010: 6865 2073 6574 7469 6e67 7320 666f 7220  he settings for 
-00009020: 7374 6174 6973 7469 6373 0a20 2020 2020  statistics.     
-00009030: 2020 2063 6f6d 7075 7461 7469 6f6e 206f     computation o
-00009040: 6620 7468 6520 6665 6174 7572 6520 6772  f the feature gr
-00009050: 6f75 702e 2222 220a 2020 2020 2020 2020  oup.""".        
-00009060: 7265 7475 726e 2073 656c 662e 5f73 7461  return self._sta
-00009070: 7469 7374 6963 735f 636f 6e66 6967 0a0a  tistics_config..
-00009080: 2020 2020 4073 7461 7469 7374 6963 735f      @statistics_
-00009090: 636f 6e66 6967 2e73 6574 7465 720a 2020  config.setter.  
-000090a0: 2020 6465 6620 7374 6174 6973 7469 6373    def statistics
-000090b0: 5f63 6f6e 6669 6728 7365 6c66 2c20 7374  _config(self, st
-000090c0: 6174 6973 7469 6373 5f63 6f6e 6669 6729  atistics_config)
-000090d0: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
-000090e0: 6e73 7461 6e63 6528 7374 6174 6973 7469  nstance(statisti
-000090f0: 6373 5f63 6f6e 6669 672c 2053 7461 7469  cs_config, Stati
-00009100: 7374 6963 7343 6f6e 6669 6729 3a0a 2020  sticsConfig):.  
-00009110: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00009120: 7374 6174 6973 7469 6373 5f63 6f6e 6669  statistics_confi
-00009130: 6720 3d20 7374 6174 6973 7469 6373 5f63  g = statistics_c
-00009140: 6f6e 6669 670a 2020 2020 2020 2020 656c  onfig.        el
-00009150: 6966 2069 7369 6e73 7461 6e63 6528 7374  if isinstance(st
-00009160: 6174 6973 7469 6373 5f63 6f6e 6669 672c  atistics_config,
-00009170: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
-00009180: 2020 2020 7365 6c66 2e5f 7374 6174 6973      self._statis
-00009190: 7469 6373 5f63 6f6e 6669 6720 3d20 5374  tics_config = St
-000091a0: 6174 6973 7469 6373 436f 6e66 6967 282a  atisticsConfig(*
-000091b0: 2a73 7461 7469 7374 6963 735f 636f 6e66  *statistics_conf
-000091c0: 6967 290a 2020 2020 2020 2020 656c 6966  ig).        elif
-000091d0: 2069 7369 6e73 7461 6e63 6528 7374 6174   isinstance(stat
-000091e0: 6973 7469 6373 5f63 6f6e 6669 672c 2062  istics_config, b
-000091f0: 6f6f 6c29 3a0a 2020 2020 2020 2020 2020  ool):.          
-00009200: 2020 7365 6c66 2e5f 7374 6174 6973 7469    self._statisti
-00009210: 6373 5f63 6f6e 6669 6720 3d20 5374 6174  cs_config = Stat
-00009220: 6973 7469 6373 436f 6e66 6967 2873 7461  isticsConfig(sta
-00009230: 7469 7374 6963 735f 636f 6e66 6967 290a  tistics_config).
-00009240: 2020 2020 2020 2020 656c 6966 2073 7461          elif sta
-00009250: 7469 7374 6963 735f 636f 6e66 6967 2069  tistics_config i
-00009260: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00009270: 2020 2020 7365 6c66 2e5f 7374 6174 6973      self._statis
-00009280: 7469 6373 5f63 6f6e 6669 6720 3d20 5374  tics_config = St
-00009290: 6174 6973 7469 6373 436f 6e66 6967 2829  atisticsConfig()
-000092a0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000092b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000092c0: 2054 7970 6545 7272 6f72 280a 2020 2020   TypeError(.    
-000092d0: 2020 2020 2020 2020 2020 2020 2254 6865              "The
-000092e0: 2061 7267 756d 656e 7420 6073 7461 7469   argument `stati
-000092f0: 7374 6963 735f 636f 6e66 6967 6020 6861  stics_config` ha
-00009300: 7320 746f 2062 6520 604e 6f6e 6560 206f  s to be `None` o
-00009310: 6620 7479 7065 2060 5374 6174 6973 7469  f type `Statisti
-00009320: 6373 436f 6e66 6967 2c20 6062 6f6f 6c60  csConfig, `bool`
-00009330: 206f 7220 6064 6963 7460 2c20 6275 7420   or `dict`, but 
-00009340: 6973 206f 6620 7479 7065 3a20 607b 7d60  is of type: `{}`
-00009350: 222e 666f 726d 6174 280a 2020 2020 2020  ".format(.      
-00009360: 2020 2020 2020 2020 2020 2020 2020 7479                ty
-00009370: 7065 2873 7461 7469 7374 6963 735f 636f  pe(statistics_co
-00009380: 6e66 6967 290a 2020 2020 2020 2020 2020  nfig).          
-00009390: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000093a0: 2020 2020 290a 0a20 2020 2040 7072 6f70      )..    @prop
-000093b0: 6572 7479 0a20 2020 2064 6566 2073 7461  erty.    def sta
-000093c0: 7469 7374 6963 7328 7365 6c66 293a 0a20  tistics(self):. 
-000093d0: 2020 2020 2020 2022 2222 4765 7420 7468         """Get th
-000093e0: 6520 6c61 7465 7374 2063 6f6d 7075 7465  e latest compute
-000093f0: 6420 7374 6174 6973 7469 6373 2066 6f72  d statistics for
-00009400: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
-00009410: 7570 2e22 2222 0a20 2020 2020 2020 2072  up.""".        r
-00009420: 6574 7572 6e20 7365 6c66 2e5f 7374 6174  eturn self._stat
-00009430: 6973 7469 6373 5f65 6e67 696e 652e 6765  istics_engine.ge
-00009440: 745f 6c61 7374 2873 656c 6629 0a0a 2020  t_last(self)..  
-00009450: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00009460: 6465 6620 7072 696d 6172 795f 6b65 7928  def primary_key(
-00009470: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00009480: 2222 4c69 7374 206f 6620 6665 6174 7572  ""List of featur
-00009490: 6573 2062 7569 6c64 696e 6720 7468 6520  es building the 
-000094a0: 7072 696d 6172 7920 6b65 792e 2222 220a  primary key.""".
-000094b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000094c0: 656c 662e 5f70 7269 6d61 7279 5f6b 6579  elf._primary_key
-000094d0: 0a0a 2020 2020 4070 7269 6d61 7279 5f6b  ..    @primary_k
-000094e0: 6579 2e73 6574 7465 720a 2020 2020 6465  ey.setter.    de
-000094f0: 6620 7072 696d 6172 795f 6b65 7928 7365  f primary_key(se
-00009500: 6c66 2c20 6e65 775f 7072 696d 6172 795f  lf, new_primary_
-00009510: 6b65 7929 3a0a 2020 2020 2020 2020 7365  key):.        se
-00009520: 6c66 2e5f 7072 696d 6172 795f 6b65 7920  lf._primary_key 
-00009530: 3d20 5b70 6b2e 6c6f 7765 7228 2920 666f  = [pk.lower() fo
-00009540: 7220 706b 2069 6e20 6e65 775f 7072 696d  r pk in new_prim
-00009550: 6172 795f 6b65 795d 0a0a 2020 2020 6465  ary_key]..    de
-00009560: 6620 6765 745f 7374 6174 6973 7469 6373  f get_statistics
-00009570: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-00009580: 636f 6d6d 6974 5f74 696d 653a 204f 7074  commit_time: Opt
-00009590: 696f 6e61 6c5b 556e 696f 6e5b 7374 722c  ional[Union[str,
-000095a0: 2069 6e74 2c20 6461 7465 7469 6d65 2c20   int, datetime, 
-000095b0: 6461 7465 5d5d 203d 204e 6f6e 650a 2020  date]] = None.  
-000095c0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-000095d0: 5265 7475 726e 7320 7468 6520 7374 6174  Returns the stat
-000095e0: 6973 7469 6373 2066 6f72 2074 6869 7320  istics for this 
-000095f0: 6665 6174 7572 6520 6772 6f75 7020 6174  feature group at
-00009600: 2061 2073 7065 6369 6669 6320 7469 6d65   a specific time
-00009610: 2e0a 0a20 2020 2020 2020 2049 6620 6063  ...        If `c
-00009620: 6f6d 6d69 745f 7469 6d65 6020 6973 2060  ommit_time` is `
-00009630: 4e6f 6e65 602c 2074 6865 206d 6f73 7420  None`, the most 
-00009640: 7265 6365 6e74 2073 7461 7469 7374 6963  recent statistic
-00009650: 7320 6172 6520 7265 7475 726e 6564 2e0a  s are returned..
-00009660: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
-00009670: 6d70 6c65 0a20 2020 2020 2020 2020 2020  mple.           
-00009680: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
-00009690: 2020 2020 2020 2023 2063 6f6e 6e65 6374         # connect
-000096a0: 2074 6f20 7468 6520 4665 6174 7572 6520   to the Feature 
-000096b0: 5374 6f72 650a 2020 2020 2020 2020 2020  Store.          
-000096c0: 2020 6673 203d 202e 2e2e 0a0a 2020 2020    fs = .....    
-000096d0: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
-000096e0: 6520 4665 6174 7572 6520 4772 6f75 7020  e Feature Group 
-000096f0: 696e 7374 616e 6365 0a20 2020 2020 2020  instance.       
-00009700: 2020 2020 2066 6720 3d20 6673 2e67 6574       fg = fs.get
-00009710: 5f6f 725f 6372 6561 7465 5f66 6561 7475  _or_create_featu
-00009720: 7265 5f67 726f 7570 282e 2e2e 290a 0a20  re_group(...).. 
-00009730: 2020 2020 2020 2020 2020 2066 675f 7374             fg_st
-00009740: 6174 6973 7469 6373 203d 2066 672e 6765  atistics = fg.ge
-00009750: 745f 7374 6174 6973 7469 6373 2863 6f6d  t_statistics(com
-00009760: 6d69 745f 7469 6d65 3d4e 6f6e 6529 0a20  mit_time=None). 
-00009770: 2020 2020 2020 2020 2020 2060 6060 0a0a             ```..
-00009780: 2020 2020 2020 2020 2320 4172 6775 6d65          # Argume
-00009790: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-000097a0: 636f 6d6d 6974 5f74 696d 653a 2044 6174  commit_time: Dat
-000097b0: 6520 616e 6420 7469 6d65 206f 6620 7468  e and time of th
-000097c0: 6520 636f 6d6d 6974 2e20 4465 6661 756c  e commit. Defaul
-000097d0: 7473 2074 6f20 604e 6f6e 6560 2e20 5374  ts to `None`. St
-000097e0: 7269 6e67 7320 7368 6f75 6c64 0a20 2020  rings should.   
-000097f0: 2020 2020 2020 2020 2020 2020 2062 6520               be 
-00009800: 666f 726d 6174 7465 6420 696e 206f 6e65  formatted in one
-00009810: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
-00009820: 6720 666f 726d 6174 7320 6025 592d 256d  g formats `%Y-%m
-00009830: 2d25 6460 2c20 6025 592d 256d 2d25 6420  -%d`, `%Y-%m-%d 
-00009840: 2548 602c 2060 2559 2d25 6d2d 2564 2025  %H`, `%Y-%m-%d %
-00009850: 483a 254d 602c 2060 2559 2d25 6d2d 2564  H:%M`, `%Y-%m-%d
-00009860: 2025 483a 254d 3a25 5360 2c0a 2020 2020   %H:%M:%S`,.    
-00009870: 2020 2020 2020 2020 2020 2020 6f72 2060              or `
-00009880: 2559 2d25 6d2d 2564 2025 483a 254d 3a25  %Y-%m-%d %H:%M:%
-00009890: 532e 2566 602e 0a0a 2020 2020 2020 2020  S.%f`...        
-000098a0: 2320 5265 7475 726e 730a 2020 2020 2020  # Returns.      
-000098b0: 2020 2020 2020 6053 7461 7469 7374 6963        `Statistic
-000098c0: 7360 2e20 5374 6174 6973 7469 6373 206f  s`. Statistics o
-000098d0: 626a 6563 742e 0a0a 2020 2020 2020 2020  bject...        
-000098e0: 2320 5261 6973 6573 0a20 2020 2020 2020  # Raises.       
-000098f0: 2020 2020 2060 6873 6673 2e63 6c69 656e       `hsfs.clien
-00009900: 742e 6578 6365 7074 696f 6e73 2e52 6573  t.exceptions.Res
-00009910: 7441 5049 4572 726f 7260 2e0a 2020 2020  tAPIError`..    
-00009920: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00009930: 6966 2063 6f6d 6d69 745f 7469 6d65 2069  if commit_time i
-00009940: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00009950: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00009960: 7374 6174 6973 7469 6373 0a20 2020 2020  statistics.     
-00009970: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00009980: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00009990: 2e5f 7374 6174 6973 7469 6373 5f65 6e67  ._statistics_eng
-000099a0: 696e 652e 6765 7428 7365 6c66 2c20 636f  ine.get(self, co
-000099b0: 6d6d 6974 5f74 696d 6529 0a0a 2020 2020  mmit_time)..    
-000099c0: 6465 6620 636f 6d70 7574 655f 7374 6174  def compute_stat
-000099d0: 6973 7469 6373 2873 656c 6629 3a0a 2020  istics(self):.  
-000099e0: 2020 2020 2020 2222 2252 6563 6f6d 7075        """Recompu
-000099f0: 7465 2074 6865 2073 7461 7469 7374 6963  te the statistic
-00009a00: 7320 666f 7220 7468 6520 6665 6174 7572  s for the featur
-00009a10: 6520 6772 6f75 7020 616e 6420 7361 7665  e group and save
-00009a20: 2074 6865 6d20 746f 2074 6865 0a20 2020   them to the.   
-00009a30: 2020 2020 2066 6561 7475 7265 2073 746f       feature sto
-00009a40: 7265 2e0a 2020 2020 2020 2020 5374 6174  re..        Stat
-00009a50: 6973 7469 6373 2061 7265 206f 6e6c 7920  istics are only 
-00009a60: 636f 6d70 7574 6564 2066 6f72 2064 6174  computed for dat
-00009a70: 6120 696e 2074 6865 206f 6666 6c69 6e65  a in the offline
-00009a80: 2073 746f 7261 6765 206f 6620 7468 6520   storage of the 
-00009a90: 6665 6174 7572 650a 2020 2020 2020 2020  feature.        
-00009aa0: 6772 6f75 702e 0a0a 2020 2020 2020 2020  group...        
-00009ab0: 2121 2120 6578 616d 706c 650a 2020 2020  !!! example.    
-00009ac0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-00009ad0: 6e0a 2020 2020 2020 2020 2020 2020 2320  n.            # 
-00009ae0: 636f 6e6e 6563 7420 746f 2074 6865 2046  connect to the F
-00009af0: 6561 7475 7265 2053 746f 7265 0a20 2020  eature Store.   
-00009b00: 2020 2020 2020 2020 2066 7320 3d20 2e2e           fs = ..
-00009b10: 2e0a 0a20 2020 2020 2020 2020 2020 2023  ...            #
-00009b20: 2067 6574 2074 6865 2046 6561 7475 7265   get the Feature
-00009b30: 2047 726f 7570 2069 6e73 7461 6e63 650a   Group instance.
-00009b40: 2020 2020 2020 2020 2020 2020 6667 203d              fg =
-00009b50: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
-00009b60: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
-00009b70: 2e2e 2e29 0a0a 2020 2020 2020 2020 2020  ...)..          
-00009b80: 2020 7374 6174 6973 7469 6373 5f6d 6574    statistics_met
-00009b90: 6164 6174 6120 3d20 6667 2e63 6f6d 7075  adata = fg.compu
-00009ba0: 7465 5f73 7461 7469 7374 6963 7328 290a  te_statistics().
-00009bb0: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
-00009bc0: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
-00009bd0: 6e73 0a20 2020 2020 2020 2020 2020 2060  ns.            `
-00009be0: 5374 6174 6973 7469 6373 602e 2054 6865  Statistics`. The
-00009bf0: 2073 7461 7469 7374 6963 7320 6d65 7461   statistics meta
-00009c00: 6461 7461 206f 626a 6563 742e 0a0a 2020  data object...  
-00009c10: 2020 2020 2020 2320 5261 6973 6573 0a20        # Raises. 
-00009c20: 2020 2020 2020 2020 2020 2060 6873 6673             `hsfs
-00009c30: 2e63 6c69 656e 742e 6578 6365 7074 696f  .client.exceptio
-00009c40: 6e73 2e52 6573 7441 5049 4572 726f 7260  ns.RestAPIError`
-00009c50: 2e20 556e 6162 6c65 2074 6f20 7065 7273  . Unable to pers
-00009c60: 6973 7420 7468 6520 7374 6174 6973 7469  ist the statisti
-00009c70: 6373 2e0a 2020 2020 2020 2020 2222 220a  cs..        """.
-00009c80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00009c90: 7374 6174 6973 7469 6373 5f63 6f6e 6669  statistics_confi
-00009ca0: 672e 656e 6162 6c65 643a 0a20 2020 2020  g.enabled:.     
-00009cb0: 2020 2020 2020 2023 2044 6f6e 2774 2072         # Don't r
-00009cc0: 6561 6420 7468 6520 6461 7461 6672 616d  ead the datafram
-00009cd0: 6520 6865 7265 2c20 746f 2061 766f 6964  e here, to avoid
-00009ce0: 2074 7269 6767 6572 696e 6720 6120 7265   triggering a re
-00009cf0: 6164 206f 7065 7261 7469 6f6e 0a20 2020  ad operation.   
-00009d00: 2020 2020 2020 2020 2023 2066 6f72 2074           # for t
-00009d10: 6865 2050 7974 686f 6e20 656e 6769 6e65  he Python engine
-00009d20: 2e20 5468 6520 5079 7468 6f6e 2065 6e67  . The Python eng
-00009d30: 696e 6520 6973 2067 6f69 6e67 2074 6f20  ine is going to 
-00009d40: 7365 7475 7020 6120 5370 6172 6b20 4a6f  setup a Spark Jo
-00009d50: 620a 2020 2020 2020 2020 2020 2020 2320  b.            # 
-00009d60: 746f 2075 7064 6174 6520 7468 6520 7374  to update the st
-00009d70: 6174 6973 7469 6373 2e0a 2020 2020 2020  atistics..      
-00009d80: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00009d90: 662e 5f73 7461 7469 7374 6963 735f 656e  f._statistics_en
-00009da0: 6769 6e65 2e63 6f6d 7075 7465 5f73 7461  gine.compute_sta
-00009db0: 7469 7374 6963 7328 7365 6c66 290a 2020  tistics(self).  
-00009dc0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00009dd0: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-00009de0: 2e77 6172 6e28 0a20 2020 2020 2020 2020  .warn(.         
-00009df0: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
-00009e00: 2020 2020 2020 2020 2020 2020 2022 5468               "Th
-00009e10: 6520 7374 6174 6973 7469 6373 2061 7265  e statistics are
-00009e20: 206e 6f74 2065 6e61 626c 6564 206f 6620   not enabled of 
-00009e30: 6665 6174 7572 6520 6772 6f75 7020 607b  feature group `{
-00009e40: 7d60 2c20 7769 7468 2076 6572 7369 6f6e  }`, with version
-00009e50: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00009e60: 2020 2020 2020 2220 607b 7d60 2e20 4e6f        " `{}`. No
-00009e70: 2073 7461 7469 7374 6963 7320 636f 6d70   statistics comp
-00009e80: 7574 6564 2e22 0a20 2020 2020 2020 2020  uted.".         
-00009e90: 2020 2020 2020 2029 2e66 6f72 6d61 7428         ).format(
-00009ea0: 7365 6c66 2e5f 6e61 6d65 2c20 7365 6c66  self._name, self
-00009eb0: 2e5f 7665 7273 696f 6e29 2c0a 2020 2020  ._version),.    
-00009ec0: 2020 2020 2020 2020 2020 2020 7574 696c              util
-00009ed0: 2e53 746f 7261 6765 5761 726e 696e 672c  .StorageWarning,
-00009ee0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00009ef0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00009f00: 2020 6465 6620 6576 656e 745f 7469 6d65    def event_time
-00009f10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00009f20: 2222 2245 7665 6e74 2074 696d 6520 6665  """Event time fe
-00009f30: 6174 7572 6520 696e 2074 6865 2066 6561  ature in the fea
-00009f40: 7475 7265 2067 726f 7570 2e22 2222 0a20  ture group.""". 
-00009f50: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00009f60: 6c66 2e5f 6576 656e 745f 7469 6d65 0a0a  lf._event_time..
-00009f70: 2020 2020 4065 7665 6e74 5f74 696d 652e      @event_time.
-00009f80: 7365 7474 6572 0a20 2020 2064 6566 2065  setter.    def e
-00009f90: 7665 6e74 5f74 696d 6528 7365 6c66 2c20  vent_time(self, 
-00009fa0: 6665 6174 7572 655f 6e61 6d65 3a20 4f70  feature_name: Op
-00009fb0: 7469 6f6e 616c 5b73 7472 5d29 3a0a 2020  tional[str]):.  
-00009fc0: 2020 2020 2020 6966 2066 6561 7475 7265        if feature
-00009fd0: 5f6e 616d 6520 6973 204e 6f6e 653a 0a20  _name is None:. 
-00009fe0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009ff0: 5f65 7665 6e74 5f74 696d 6520 3d20 4e6f  _event_time = No
-0000a000: 6e65 0a20 2020 2020 2020 2020 2020 2072  ne.            r
-0000a010: 6574 7572 6e0a 2020 2020 2020 2020 656c  eturn.        el
-0000a020: 6966 2069 7369 6e73 7461 6e63 6528 6665  if isinstance(fe
-0000a030: 6174 7572 655f 6e61 6d65 2c20 7374 7229  ature_name, str)
-0000a040: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000a050: 6c66 2e5f 6576 656e 745f 7469 6d65 203d  lf._event_time =
-0000a060: 2066 6561 7475 7265 5f6e 616d 650a 2020   feature_name.  
-0000a070: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000a080: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
-0000a090: 696e 7374 616e 6365 2866 6561 7475 7265  instance(feature
-0000a0a0: 5f6e 616d 652c 206c 6973 7429 2061 6e64  _name, list) and
-0000a0b0: 206c 656e 2866 6561 7475 7265 5f6e 616d   len(feature_nam
-0000a0c0: 6529 203d 3d20 313a 0a20 2020 2020 2020  e) == 1:.       
-0000a0d0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0000a0e0: 6365 2866 6561 7475 7265 5f6e 616d 655b  ce(feature_name[
-0000a0f0: 305d 2c20 7374 7229 3a0a 2020 2020 2020  0], str):.      
-0000a100: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-0000a110: 6773 2e77 6172 6e28 0a20 2020 2020 2020  gs.warn(.       
-0000a120: 2020 2020 2020 2020 2020 2020 2022 5072               "Pr
-0000a130: 6f76 6964 696e 6720 6576 656e 745f 7469  oviding event_ti
-0000a140: 6d65 2061 7320 6120 7369 6e67 6c65 2d65  me as a single-e
-0000a150: 6c65 6d65 6e74 206c 6973 7420 6973 2064  lement list is d
-0000a160: 6570 7265 6361 7465 6422 0a20 2020 2020  eprecated".     
-0000a170: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0000a180: 2022 2061 6e64 2077 696c 6c20 6265 2064   " and will be d
-0000a190: 726f 7070 6564 2069 6e20 6675 7475 7265  ropped in future
-0000a1a0: 2076 6572 7369 6f6e 732e 2050 726f 7669   versions. Provi
-0000a1b0: 6465 2074 6865 2066 6561 7475 7265 5f6e  de the feature_n
-0000a1c0: 616d 6520 7374 7269 6e67 2069 6e73 7465  ame string inste
-0000a1d0: 6164 2e22 2c0a 2020 2020 2020 2020 2020  ad.",.          
-0000a1e0: 2020 2020 2020 2020 2020 4465 7072 6563            Deprec
-0000a1f0: 6174 696f 6e57 6172 6e69 6e67 2c0a 2020  ationWarning,.  
-0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a210: 2020 7374 6163 6b6c 6576 656c 3d32 2c0a    stacklevel=2,.
-0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a230: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a240: 2020 7365 6c66 2e5f 6576 656e 745f 7469    self._event_ti
-0000a250: 6d65 203d 2066 6561 7475 7265 5f6e 616d  me = feature_nam
-0000a260: 655b 305d 0a20 2020 2020 2020 2020 2020  e[0].           
-0000a270: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-0000a280: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0000a290: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-0000a2a0: 2020 2022 6576 656e 745f 7469 6d65 206d     "event_time m
-0000a2b0: 7573 7420 6265 2061 2073 7472 696e 6720  ust be a string 
-0000a2c0: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
-0000a2d0: 2061 6e20 6578 6973 7469 6e67 2066 6561   an existing fea
-0000a2e0: 7475 7265 206e 616d 6520 6f66 2074 6865  ture name of the
-0000a2f0: 2046 6561 7475 7265 2047 726f 7570 2e22   Feature Group."
-0000a300: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000a310: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0000a320: 6620 6c6f 6361 7469 6f6e 2873 656c 6629  f location(self)
-0000a330: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0000a340: 2073 656c 662e 5f6c 6f63 6174 696f 6e0a   self._location.
-0000a350: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-0000a360: 2020 2064 6566 2065 7870 6563 7461 7469     def expectati
-0000a370: 6f6e 5f73 7569 7465 280a 2020 2020 2020  on_suite(.      
-0000a380: 2020 7365 6c66 2c0a 2020 2020 2920 2d3e    self,.    ) ->
-0000a390: 204f 7074 696f 6e61 6c5b 4578 7065 6374   Optional[Expect
-0000a3a0: 6174 696f 6e53 7569 7465 5d3a 0a20 2020  ationSuite]:.   
-0000a3b0: 2020 2020 2022 2222 4578 7065 6374 6174       """Expectat
-0000a3c0: 696f 6e20 5375 6974 6520 636f 6e66 6967  ion Suite config
-0000a3d0: 7572 6174 696f 6e20 6f62 6a65 6374 2064  uration object d
-0000a3e0: 6566 696e 696e 6720 7468 6520 7365 7474  efining the sett
-0000a3f0: 696e 6773 2066 6f72 0a20 2020 2020 2020  ings for.       
-0000a400: 2064 6174 6120 7661 6c69 6461 7469 6f6e   data validation
-0000a410: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
-0000a420: 6772 6f75 702e 2222 220a 2020 2020 2020  group.""".      
-0000a430: 2020 7265 7475 726e 2073 656c 662e 5f65    return self._e
-0000a440: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-0000a450: 0a0a 2020 2020 4065 7870 6563 7461 7469  ..    @expectati
-0000a460: 6f6e 5f73 7569 7465 2e73 6574 7465 720a  on_suite.setter.
-0000a470: 2020 2020 6465 6620 6578 7065 6374 6174      def expectat
-0000a480: 696f 6e5f 7375 6974 6528 0a20 2020 2020  ion_suite(.     
-0000a490: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000a4a0: 2065 7870 6563 7461 7469 6f6e 5f73 7569   expectation_sui
-0000a4b0: 7465 3a20 556e 696f 6e5b 0a20 2020 2020  te: Union[.     
-0000a4c0: 2020 2020 2020 2045 7870 6563 7461 7469         Expectati
-0000a4d0: 6f6e 5375 6974 652c 2067 652e 636f 7265  onSuite, ge.core
-0000a4e0: 2e45 7870 6563 7461 7469 6f6e 5375 6974  .ExpectationSuit
-0000a4f0: 652c 2064 6963 742c 204e 6f6e 650a 2020  e, dict, None.  
-0000a500: 2020 2020 2020 5d2c 0a20 2020 2029 3a0a        ],.    ):.
-0000a510: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-0000a520: 7461 6e63 6528 6578 7065 6374 6174 696f  tance(expectatio
-0000a530: 6e5f 7375 6974 652c 2045 7870 6563 7461  n_suite, Expecta
-0000a540: 7469 6f6e 5375 6974 6529 3a0a 2020 2020  tionSuite):.    
-0000a550: 2020 2020 2020 2020 746d 705f 6578 7065          tmp_expe
-0000a560: 6374 6174 696f 6e5f 7375 6974 6520 3d20  ctation_suite = 
-0000a570: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
-0000a580: 652e 746f 5f6a 736f 6e5f 6469 6374 2829  e.to_json_dict()
-0000a590: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
-0000a5a0: 5f65 7870 6563 7461 7469 6f6e 5f73 7569  _expectation_sui
-0000a5b0: 7465 5b22 6665 6174 7572 6567 726f 7570  te["featuregroup
-0000a5c0: 5f69 6422 5d20 3d20 7365 6c66 2e5f 6964  _id"] = self._id
-0000a5d0: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
-0000a5e0: 5f65 7870 6563 7461 7469 6f6e 5f73 7569  _expectation_sui
-0000a5f0: 7465 5b22 6665 6174 7572 6573 746f 7265  te["featurestore
-0000a600: 5f69 6422 5d20 3d20 7365 6c66 2e5f 6665  _id"] = self._fe
-0000a610: 6174 7572 655f 7374 6f72 655f 6964 0a20  ature_store_id. 
-0000a620: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a630: 5f65 7870 6563 7461 7469 6f6e 5f73 7569  _expectation_sui
-0000a640: 7465 203d 2045 7870 6563 7461 7469 6f6e  te = Expectation
-0000a650: 5375 6974 6528 2a2a 746d 705f 6578 7065  Suite(**tmp_expe
-0000a660: 6374 6174 696f 6e5f 7375 6974 6529 0a20  ctation_suite). 
-0000a670: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-0000a680: 7374 616e 6365 2865 7870 6563 7461 7469  stance(expectati
-0000a690: 6f6e 5f73 7569 7465 2c20 6765 2e63 6f72  on_suite, ge.cor
-0000a6a0: 652e 6578 7065 6374 6174 696f 6e5f 7375  e.expectation_su
-0000a6b0: 6974 652e 4578 7065 6374 6174 696f 6e53  ite.ExpectationS
-0000a6c0: 7569 7465 293a 0a20 2020 2020 2020 2020  uite):.         
-0000a6d0: 2020 2073 656c 662e 5f65 7870 6563 7461     self._expecta
-0000a6e0: 7469 6f6e 5f73 7569 7465 203d 2045 7870  tion_suite = Exp
-0000a6f0: 6563 7461 7469 6f6e 5375 6974 6528 0a20  ectationSuite(. 
-0000a700: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-0000a710: 2a65 7870 6563 7461 7469 6f6e 5f73 7569  *expectation_sui
-0000a720: 7465 2e74 6f5f 6a73 6f6e 5f64 6963 7428  te.to_json_dict(
-0000a730: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000a740: 2020 2066 6561 7475 7265 5f73 746f 7265     feature_store
-0000a750: 5f69 643d 7365 6c66 2e5f 6665 6174 7572  _id=self._featur
-0000a760: 655f 7374 6f72 655f 6964 2c0a 2020 2020  e_store_id,.    
-0000a770: 2020 2020 2020 2020 2020 2020 6665 6174              feat
-0000a780: 7572 655f 6772 6f75 705f 6964 3d73 656c  ure_group_id=sel
-0000a790: 662e 5f69 642c 0a20 2020 2020 2020 2020  f._id,.         
-0000a7a0: 2020 2029 0a20 2020 2020 2020 2065 6c69     ).        eli
-0000a7b0: 6620 6973 696e 7374 616e 6365 2865 7870  f isinstance(exp
-0000a7c0: 6563 7461 7469 6f6e 5f73 7569 7465 2c20  ectation_suite, 
-0000a7d0: 6469 6374 293a 0a20 2020 2020 2020 2020  dict):.         
-0000a7e0: 2020 2074 6d70 5f65 7870 6563 7461 7469     tmp_expectati
-0000a7f0: 6f6e 5f73 7569 7465 203d 2065 7870 6563  on_suite = expec
-0000a800: 7461 7469 6f6e 5f73 7569 7465 2e63 6f70  tation_suite.cop
-0000a810: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-0000a820: 746d 705f 6578 7065 6374 6174 696f 6e5f  tmp_expectation_
-0000a830: 7375 6974 655b 2266 6561 7475 7265 5f73  suite["feature_s
-0000a840: 746f 7265 5f69 6422 5d20 3d20 7365 6c66  tore_id"] = self
-0000a850: 2e5f 6665 6174 7572 655f 7374 6f72 655f  ._feature_store_
-0000a860: 6964 0a20 2020 2020 2020 2020 2020 2074  id.            t
-0000a870: 6d70 5f65 7870 6563 7461 7469 6f6e 5f73  mp_expectation_s
-0000a880: 7569 7465 5b22 6665 6174 7572 655f 6772  uite["feature_gr
-0000a890: 6f75 705f 6964 225d 203d 2073 656c 662e  oup_id"] = self.
-0000a8a0: 5f69 640a 2020 2020 2020 2020 2020 2020  _id.            
-0000a8b0: 7365 6c66 2e5f 6578 7065 6374 6174 696f  self._expectatio
-0000a8c0: 6e5f 7375 6974 6520 3d20 4578 7065 6374  n_suite = Expect
-0000a8d0: 6174 696f 6e53 7569 7465 282a 2a74 6d70  ationSuite(**tmp
-0000a8e0: 5f65 7870 6563 7461 7469 6f6e 5f73 7569  _expectation_sui
-0000a8f0: 7465 290a 2020 2020 2020 2020 656c 6966  te).        elif
-0000a900: 2065 7870 6563 7461 7469 6f6e 5f73 7569   expectation_sui
-0000a910: 7465 2069 7320 4e6f 6e65 3a0a 2020 2020  te is None:.    
-0000a920: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
-0000a930: 7065 6374 6174 696f 6e5f 7375 6974 6520  pectation_suite 
-0000a940: 3d20 4e6f 6e65 0a20 2020 2020 2020 2065  = None.        e
-0000a950: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000a960: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-0000a970: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000a980: 2020 2254 6865 2061 7267 756d 656e 7420    "The argument 
-0000a990: 6065 7870 6563 7461 7469 6f6e 5f73 7569  `expectation_sui
-0000a9a0: 7465 6020 6861 7320 746f 2062 6520 604e  te` has to be `N
-0000a9b0: 6f6e 6560 206f 6620 7479 7065 2060 4578  one` of type `Ex
-0000a9c0: 7065 6374 6174 696f 6e53 7569 7465 6020  pectationSuite` 
-0000a9d0: 6f72 2060 6469 6374 602c 2062 7574 2069  or `dict`, but i
-0000a9e0: 7320 6f66 2074 7970 653a 2060 7b7d 6022  s of type: `{}`"
-0000a9f0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-0000aa00: 2020 2020 2020 2020 2020 2020 2074 7970               typ
-0000aa10: 6528 6578 7065 6374 6174 696f 6e5f 7375  e(expectation_su
-0000aa20: 6974 6529 0a20 2020 2020 2020 2020 2020  ite).           
-0000aa30: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000aa40: 2020 2029 0a0a 0a63 6c61 7373 2046 6561     )...class Fea
-0000aa50: 7475 7265 4772 6f75 7028 4665 6174 7572  tureGroup(Featur
-0000aa60: 6547 726f 7570 4261 7365 293a 0a20 2020  eGroupBase):.   
-0000aa70: 2043 4143 4845 445f 4645 4154 5552 455f   CACHED_FEATURE_
-0000aa80: 4752 4f55 5020 3d20 2243 4143 4845 445f  GROUP = "CACHED_
-0000aa90: 4645 4154 5552 455f 4752 4f55 5022 0a20  FEATURE_GROUP". 
-0000aaa0: 2020 2053 5452 4541 4d5f 4645 4154 5552     STREAM_FEATUR
-0000aab0: 455f 4752 4f55 5020 3d20 2253 5452 4541  E_GROUP = "STREA
-0000aac0: 4d5f 4645 4154 5552 455f 4752 4f55 5022  M_FEATURE_GROUP"
-0000aad0: 0a20 2020 2045 4e54 4954 595f 5459 5045  .    ENTITY_TYPE
-0000aae0: 203d 2022 6665 6174 7572 6567 726f 7570   = "featuregroup
-0000aaf0: 7322 0a0a 2020 2020 6465 6620 5f5f 696e  s"..    def __in
-0000ab00: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-0000ab10: 6c66 2c0a 2020 2020 2020 2020 6e61 6d65  lf,.        name
-0000ab20: 2c0a 2020 2020 2020 2020 7665 7273 696f  ,.        versio
-0000ab30: 6e2c 0a20 2020 2020 2020 2066 6561 7475  n,.        featu
-0000ab40: 7265 7374 6f72 655f 6964 2c0a 2020 2020  restore_id,.    
-0000ab50: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-0000ab60: 2222 2c0a 2020 2020 2020 2020 7061 7274  "",.        part
-0000ab70: 6974 696f 6e5f 6b65 793d 4e6f 6e65 2c0a  ition_key=None,.
-0000ab80: 2020 2020 2020 2020 7072 696d 6172 795f          primary_
-0000ab90: 6b65 793d 4e6f 6e65 2c0a 2020 2020 2020  key=None,.      
-0000aba0: 2020 6875 6469 5f70 7265 636f 6d62 696e    hudi_precombin
-0000abb0: 655f 6b65 793d 4e6f 6e65 2c0a 2020 2020  e_key=None,.    
-0000abc0: 2020 2020 6665 6174 7572 6573 746f 7265      featurestore
-0000abd0: 5f6e 616d 653d 4e6f 6e65 2c0a 2020 2020  _name=None,.    
-0000abe0: 2020 2020 6372 6561 7465 643d 4e6f 6e65      created=None
-0000abf0: 2c0a 2020 2020 2020 2020 6372 6561 746f  ,.        creato
-0000ac00: 723d 4e6f 6e65 2c0a 2020 2020 2020 2020  r=None,.        
-0000ac10: 6964 3d4e 6f6e 652c 0a20 2020 2020 2020  id=None,.       
-0000ac20: 2066 6561 7475 7265 733d 4e6f 6e65 2c0a   features=None,.
-0000ac30: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
-0000ac40: 3d4e 6f6e 652c 0a20 2020 2020 2020 206f  =None,.        o
-0000ac50: 6e6c 696e 655f 656e 6162 6c65 643d 4661  nline_enabled=Fa
-0000ac60: 6c73 652c 0a20 2020 2020 2020 2074 696d  lse,.        tim
-0000ac70: 655f 7472 6176 656c 5f66 6f72 6d61 743d  e_travel_format=
-0000ac80: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-0000ac90: 6174 6973 7469 6373 5f63 6f6e 6669 673d  atistics_config=
-0000aca0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f6e  None,.        on
-0000acb0: 6c69 6e65 5f74 6f70 6963 5f6e 616d 653d  line_topic_name=
-0000acc0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6576  None,.        ev
-0000acd0: 656e 745f 7469 6d65 3d4e 6f6e 652c 0a20  ent_time=None,. 
-0000ace0: 2020 2020 2020 2073 7472 6561 6d3d 4661         stream=Fa
-0000acf0: 6c73 652c 0a20 2020 2020 2020 2065 7870  lse,.        exp
-0000ad00: 6563 7461 7469 6f6e 5f73 7569 7465 3d4e  ectation_suite=N
-0000ad10: 6f6e 652c 0a20 2020 2020 2020 2070 6172  one,.        par
-0000ad20: 656e 7473 3d4e 6f6e 652c 0a20 2020 2020  ents=None,.     
-0000ad30: 2020 2068 7265 663d 4e6f 6e65 2c0a 2020     href=None,.  
-0000ad40: 2020 293a 0a20 2020 2020 2020 2073 7570    ):.        sup
-0000ad50: 6572 2829 2e5f 5f69 6e69 745f 5f28 6665  er().__init__(fe
-0000ad60: 6174 7572 6573 746f 7265 5f69 642c 206c  aturestore_id, l
-0000ad70: 6f63 6174 696f 6e2c 2065 7665 6e74 5f74  ocation, event_t
-0000ad80: 696d 653d 6576 656e 745f 7469 6d65 290a  ime=event_time).
-0000ad90: 0a20 2020 2020 2020 2073 656c 662e 5f66  .        self._f
-0000ada0: 6561 7475 7265 5f73 746f 7265 5f6e 616d  eature_store_nam
-0000adb0: 6520 3d20 6665 6174 7572 6573 746f 7265  e = featurestore
-0000adc0: 5f6e 616d 650a 2020 2020 2020 2020 7365  _name.        se
-0000add0: 6c66 2e5f 6465 7363 7269 7074 696f 6e20  lf._description 
-0000ade0: 3d20 6465 7363 7269 7074 696f 6e0a 2020  = description.  
-0000adf0: 2020 2020 2020 7365 6c66 2e5f 6372 6561        self._crea
-0000ae00: 7465 6420 3d20 6372 6561 7465 640a 2020  ted = created.  
-0000ae10: 2020 2020 2020 7365 6c66 2e5f 6372 6561        self._crea
-0000ae20: 746f 7220 3d20 7573 6572 2e55 7365 722e  tor = user.User.
-0000ae30: 6672 6f6d 5f72 6573 706f 6e73 655f 6a73  from_response_js
-0000ae40: 6f6e 2863 7265 6174 6f72 290a 2020 2020  on(creator).    
-0000ae50: 2020 2020 7365 6c66 2e5f 7665 7273 696f      self._versio
-0000ae60: 6e20 3d20 7665 7273 696f 6e0a 2020 2020  n = version.    
-0000ae70: 2020 2020 7365 6c66 2e5f 6e61 6d65 203d      self._name =
-0000ae80: 206e 616d 650a 2020 2020 2020 2020 7365   name.        se
-0000ae90: 6c66 2e5f 6964 203d 2069 640a 2020 2020  lf._id = id.    
-0000aea0: 2020 2020 7365 6c66 2e5f 6665 6174 7572      self._featur
-0000aeb0: 6573 203d 205b 0a20 2020 2020 2020 2020  es = [.         
-0000aec0: 2020 2066 6561 7475 7265 2e46 6561 7475     feature.Featu
-0000aed0: 7265 2e66 726f 6d5f 7265 7370 6f6e 7365  re.from_response
-0000aee0: 5f6a 736f 6e28 6665 6174 2920 6966 2069  _json(feat) if i
-0000aef0: 7369 6e73 7461 6e63 6528 6665 6174 2c20  sinstance(feat, 
-0000af00: 6469 6374 2920 656c 7365 2066 6561 740a  dict) else feat.
-0000af10: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000af20: 6665 6174 2069 6e20 2866 6561 7475 7265  feat in (feature
-0000af30: 7320 6f72 205b 5d29 0a20 2020 2020 2020  s or []).       
-0000af40: 205d 0a0a 2020 2020 2020 2020 7365 6c66   ]..        self
-0000af50: 2e5f 6f6e 6c69 6e65 5f65 6e61 626c 6564  ._online_enabled
-0000af60: 203d 206f 6e6c 696e 655f 656e 6162 6c65   = online_enable
-0000af70: 640a 2020 2020 2020 2020 7365 6c66 2e5f  d.        self._
-0000af80: 7469 6d65 5f74 7261 7665 6c5f 666f 726d  time_travel_form
-0000af90: 6174 203d 2028 0a20 2020 2020 2020 2020  at = (.         
-0000afa0: 2020 2074 696d 655f 7472 6176 656c 5f66     time_travel_f
-0000afb0: 6f72 6d61 742e 7570 7065 7228 2920 6966  ormat.upper() if
-0000afc0: 2074 696d 655f 7472 6176 656c 5f66 6f72   time_travel_for
-0000afd0: 6d61 7420 6973 206e 6f74 204e 6f6e 6520  mat is not None 
-0000afe0: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
-0000aff0: 2020 290a 0a20 2020 2020 2020 2073 656c    )..        sel
-0000b000: 662e 5f73 7562 6a65 6374 203d 204e 6f6e  f._subject = Non
-0000b010: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-0000b020: 6f6e 6c69 6e65 5f74 6f70 6963 5f6e 616d  online_topic_nam
-0000b030: 6520 3d20 6f6e 6c69 6e65 5f74 6f70 6963  e = online_topic
-0000b040: 5f6e 616d 650a 2020 2020 2020 2020 7365  _name.        se
-0000b050: 6c66 2e5f 7374 7265 616d 203d 2073 7472  lf._stream = str
-0000b060: 6561 6d0a 2020 2020 2020 2020 7365 6c66  eam.        self
-0000b070: 2e5f 7061 7265 6e74 7320 3d20 7061 7265  ._parents = pare
-0000b080: 6e74 730a 2020 2020 2020 2020 7365 6c66  nts.        self
-0000b090: 2e5f 6465 6c74 6173 7472 6561 6d65 725f  ._deltastreamer_
-0000b0a0: 6a6f 6263 6f6e 6620 3d20 4e6f 6e65 0a0a  jobconf = None..
-0000b0b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000b0c0: 5f69 643a 0a20 2020 2020 2020 2020 2020  _id:.           
-0000b0d0: 2023 2069 6e69 7469 616c 697a 6564 2062   # initialized b
-0000b0e0: 7920 6261 636b 656e 640a 2020 2020 2020  y backend.      
-0000b0f0: 2020 2020 2020 7365 6c66 2e70 7269 6d61        self.prima
-0000b100: 7279 5f6b 6579 203d 205b 0a20 2020 2020  ry_key = [.     
-0000b110: 2020 2020 2020 2020 2020 2066 6561 742e             feat.
-0000b120: 6e61 6d65 2066 6f72 2066 6561 7420 696e  name for feat in
-0000b130: 2073 656c 662e 5f66 6561 7475 7265 7320   self._features 
-0000b140: 6966 2066 6561 742e 7072 696d 6172 7920  if feat.primary 
-0000b150: 6973 2054 7275 650a 2020 2020 2020 2020  is True.        
-0000b160: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
-0000b170: 2020 7365 6c66 2e5f 7061 7274 6974 696f    self._partitio
-0000b180: 6e5f 6b65 7920 3d20 5b0a 2020 2020 2020  n_key = [.      
-0000b190: 2020 2020 2020 2020 2020 6665 6174 2e6e            feat.n
-0000b1a0: 616d 6520 666f 7220 6665 6174 2069 6e20  ame for feat in 
-0000b1b0: 7365 6c66 2e5f 6665 6174 7572 6573 2069  self._features i
-0000b1c0: 6620 6665 6174 2e70 6172 7469 7469 6f6e  f feat.partition
-0000b1d0: 2069 7320 5472 7565 0a20 2020 2020 2020   is True.       
-0000b1e0: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
-0000b1f0: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-0000b200: 2020 2020 2020 2020 7469 6d65 5f74 7261          time_tra
-0000b210: 7665 6c5f 666f 726d 6174 2069 7320 6e6f  vel_format is no
-0000b220: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
-0000b230: 2020 2020 2020 2061 6e64 2074 696d 655f         and time_
-0000b240: 7472 6176 656c 5f66 6f72 6d61 742e 7570  travel_format.up
-0000b250: 7065 7228 2920 3d3d 2022 4855 4449 220a  per() == "HUDI".
-0000b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b270: 616e 6420 7365 6c66 2e5f 6665 6174 7572  and self._featur
-0000b280: 6573 0a20 2020 2020 2020 2020 2020 2029  es.            )
-0000b290: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b2a0: 2020 2320 6875 6469 2070 7265 636f 6d62    # hudi precomb
-0000b2b0: 696e 6520 6b65 7920 6973 2061 6c77 6179  ine key is alway
-0000b2c0: 7320 6120 7369 6e67 6c65 2066 6561 7475  s a single featu
-0000b2d0: 7265 0a20 2020 2020 2020 2020 2020 2020  re.             
-0000b2e0: 2020 2073 656c 662e 5f68 7564 695f 7072     self._hudi_pr
-0000b2f0: 6563 6f6d 6269 6e65 5f6b 6579 203d 205b  ecombine_key = [
-0000b300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b310: 2020 2020 2066 6561 742e 6e61 6d65 0a20       feat.name. 
+00000390: 6f6d 2068 7366 7320 696d 706f 7274 2028  om hsfs import (
+000003a0: 0a20 2020 2075 7469 6c2c 0a20 2020 2065  .    util,.    e
+000003b0: 6e67 696e 652c 0a20 2020 2066 6561 7475  ngine,.    featu
+000003c0: 7265 2c0a 2020 2020 7573 6572 2c0a 2020  re,.    user,.  
+000003d0: 2020 6665 6174 7572 655f 6772 6f75 705f    feature_group_
+000003e0: 7772 6974 6572 2c0a 2020 2020 7374 6f72  writer,.    stor
+000003f0: 6167 655f 636f 6e6e 6563 746f 7220 6173  age_connector as
+00000400: 2073 632c 0a29 0a66 726f 6d20 6873 6673   sc,.).from hsfs
+00000410: 2e63 6f72 6520 696d 706f 7274 2028 0a20  .core import (. 
+00000420: 2020 2066 6561 7475 7265 5f67 726f 7570     feature_group
+00000430: 5f65 6e67 696e 652c 0a20 2020 2073 7461  _engine,.    sta
+00000440: 7469 7374 6963 735f 656e 6769 6e65 2c0a  tistics_engine,.
+00000450: 2020 2020 6578 7065 6374 6174 696f 6e5f      expectation_
+00000460: 7375 6974 655f 656e 6769 6e65 2c0a 2020  suite_engine,.  
+00000470: 2020 7661 6c69 6461 7469 6f6e 5f72 6570    validation_rep
+00000480: 6f72 745f 656e 6769 6e65 2c0a 2020 2020  ort_engine,.    
+00000490: 636f 6465 5f65 6e67 696e 652c 0a20 2020  code_engine,.   
+000004a0: 2065 7874 6572 6e61 6c5f 6665 6174 7572   external_featur
+000004b0: 655f 6772 6f75 705f 656e 6769 6e65 2c0a  e_group_engine,.
+000004c0: 2020 2020 7661 6c69 6461 7469 6f6e 5f72      validation_r
+000004d0: 6573 756c 745f 656e 6769 6e65 2c0a 2020  esult_engine,.  
+000004e0: 2020 6a6f 625f 6170 692c 0a29 0a0a 6672    job_api,.)..fr
+000004f0: 6f6d 2068 7366 732e 7374 6174 6973 7469  om hsfs.statisti
+00000500: 6373 5f63 6f6e 6669 6720 696d 706f 7274  cs_config import
+00000510: 2053 7461 7469 7374 6963 7343 6f6e 6669   StatisticsConfi
+00000520: 670a 6672 6f6d 2068 7366 732e 6578 7065  g.from hsfs.expe
+00000530: 6374 6174 696f 6e5f 7375 6974 6520 696d  ctation_suite im
+00000540: 706f 7274 2045 7870 6563 7461 7469 6f6e  port Expectation
+00000550: 5375 6974 650a 6672 6f6d 2068 7366 732e  Suite.from hsfs.
+00000560: 7661 6c69 6461 7469 6f6e 5f72 6570 6f72  validation_repor
+00000570: 7420 696d 706f 7274 2056 616c 6964 6174  t import Validat
+00000580: 696f 6e52 6570 6f72 740a 6672 6f6d 2068  ionReport.from h
+00000590: 7366 732e 636f 6e73 7472 7563 746f 7220  sfs.constructor 
+000005a0: 696d 706f 7274 2071 7565 7279 2c20 6669  import query, fi
+000005b0: 6c74 6572 0a66 726f 6d20 6873 6673 2e63  lter.from hsfs.c
+000005c0: 6c69 656e 742e 6578 6365 7074 696f 6e73  lient.exceptions
+000005d0: 2069 6d70 6f72 7420 4665 6174 7572 6553   import FeatureS
+000005e0: 746f 7265 4578 6365 7074 696f 6e0a 6672  toreException.fr
+000005f0: 6f6d 2068 7366 732e 636f 7265 2e6a 6f62  om hsfs.core.job
+00000600: 2069 6d70 6f72 7420 4a6f 620a 6672 6f6d   import Job.from
+00000610: 2068 7366 732e 636f 7265 2e76 6172 6961   hsfs.core.varia
+00000620: 626c 655f 6170 6920 696d 706f 7274 2056  ble_api import V
+00000630: 6172 6961 626c 6541 7069 0a66 726f 6d20  ariableApi.from 
+00000640: 6873 6673 2e63 6f72 6520 696d 706f 7274  hsfs.core import
+00000650: 2067 7265 6174 5f65 7870 6563 7461 7469   great_expectati
+00000660: 6f6e 5f65 6e67 696e 650a 0a0a 636c 6173  on_engine...clas
+00000670: 7320 4665 6174 7572 6547 726f 7570 4261  s FeatureGroupBa
+00000680: 7365 3a0a 2020 2020 6465 6620 5f5f 696e  se:.    def __in
+00000690: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+000006a0: 6c66 2c0a 2020 2020 2020 2020 6665 6174  lf,.        feat
+000006b0: 7572 6573 746f 7265 5f69 642c 0a20 2020  urestore_id,.   
+000006c0: 2020 2020 206c 6f63 6174 696f 6e2c 0a20       location,. 
+000006d0: 2020 2020 2020 2065 7665 6e74 5f74 696d         event_tim
+000006e0: 653d 4e6f 6e65 2c0a 2020 2020 2020 2020  e=None,.        
+000006f0: 6f6e 6c69 6e65 5f65 6e61 626c 6564 3d46  online_enabled=F
+00000700: 616c 7365 2c0a 2020 2020 2020 2020 6964  alse,.        id
+00000710: 3d4e 6f6e 652c 0a20 2020 2020 2020 2065  =None,.        e
+00000720: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
+00000730: 3d4e 6f6e 652c 0a20 2020 2020 2020 206f  =None,.        o
+00000740: 6e6c 696e 655f 746f 7069 635f 6e61 6d65  nline_topic_name
+00000750: 3d4e 6f6e 652c 0a20 2020 2029 3a0a 2020  =None,.    ):.  
+00000760: 2020 2020 2020 7365 6c66 2e65 7665 6e74        self.event
+00000770: 5f74 696d 6520 3d20 6576 656e 745f 7469  _time = event_ti
+00000780: 6d65 0a20 2020 2020 2020 2073 656c 662e  me.        self.
+00000790: 5f6f 6e6c 696e 655f 656e 6162 6c65 6420  _online_enabled 
+000007a0: 3d20 6f6e 6c69 6e65 5f65 6e61 626c 6564  = online_enabled
+000007b0: 0a20 2020 2020 2020 2073 656c 662e 5f6c  .        self._l
+000007c0: 6f63 6174 696f 6e20 3d20 6c6f 6361 7469  ocation = locati
+000007d0: 6f6e 0a20 2020 2020 2020 2073 656c 662e  on.        self.
+000007e0: 5f69 6420 3d20 6964 0a20 2020 2020 2020  _id = id.       
+000007f0: 2073 656c 662e 5f73 7562 6a65 6374 203d   self._subject =
+00000800: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+00000810: 6c66 2e5f 6f6e 6c69 6e65 5f74 6f70 6963  lf._online_topic
+00000820: 5f6e 616d 6520 3d20 6f6e 6c69 6e65 5f74  _name = online_t
+00000830: 6f70 6963 5f6e 616d 650a 2020 2020 2020  opic_name.      
+00000840: 2020 7365 6c66 2e5f 6665 6174 7572 655f    self._feature_
+00000850: 7374 6f72 655f 6964 203d 2066 6561 7475  store_id = featu
+00000860: 7265 7374 6f72 655f 6964 0a20 2020 2020  restore_id.     
+00000870: 2020 2023 2075 7365 2073 6574 7465 7220     # use setter 
+00000880: 666f 7220 636f 7272 6563 7420 636f 6e76  for correct conv
+00000890: 6572 7369 6f6e 0a20 2020 2020 2020 2073  ersion.        s
+000008a0: 656c 662e 6578 7065 6374 6174 696f 6e5f  elf.expectation_
+000008b0: 7375 6974 6520 3d20 6578 7065 6374 6174  suite = expectat
+000008c0: 696f 6e5f 7375 6974 650a 2020 2020 2020  ion_suite.      
+000008d0: 2020 7365 6c66 2e5f 7374 6174 6973 7469    self._statisti
+000008e0: 6373 5f65 6e67 696e 6520 3d20 7374 6174  cs_engine = stat
+000008f0: 6973 7469 6373 5f65 6e67 696e 652e 5374  istics_engine.St
+00000900: 6174 6973 7469 6373 456e 6769 6e65 280a  atisticsEngine(.
+00000910: 2020 2020 2020 2020 2020 2020 6665 6174              feat
+00000920: 7572 6573 746f 7265 5f69 642c 2073 656c  urestore_id, sel
+00000930: 662e 454e 5449 5459 5f54 5950 450a 2020  f.ENTITY_TYPE.  
+00000940: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00000950: 7365 6c66 2e5f 636f 6465 5f65 6e67 696e  self._code_engin
+00000960: 6520 3d20 636f 6465 5f65 6e67 696e 652e  e = code_engine.
+00000970: 436f 6465 456e 6769 6e65 2866 6561 7475  CodeEngine(featu
+00000980: 7265 7374 6f72 655f 6964 2c20 7365 6c66  restore_id, self
+00000990: 2e45 4e54 4954 595f 5459 5045 290a 2020  .ENTITY_TYPE).  
+000009a0: 2020 2020 2020 7365 6c66 2e5f 6772 6561        self._grea
+000009b0: 745f 6578 7065 6374 6174 696f 6e5f 656e  t_expectation_en
+000009c0: 6769 6e65 203d 2028 0a20 2020 2020 2020  gine = (.       
+000009d0: 2020 2020 2067 7265 6174 5f65 7870 6563       great_expec
+000009e0: 7461 7469 6f6e 5f65 6e67 696e 652e 4772  tation_engine.Gr
+000009f0: 6561 7445 7870 6563 7461 7469 6f6e 456e  eatExpectationEn
+00000a00: 6769 6e65 2866 6561 7475 7265 7374 6f72  gine(featurestor
+00000a10: 655f 6964 290a 2020 2020 2020 2020 290a  e_id).        ).
+00000a20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00000a30: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00000a40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00000a50: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
+00000a60: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00000a70: 2020 2073 656c 662e 5f65 7870 6563 7461     self._expecta
+00000a80: 7469 6f6e 5f73 7569 7465 2e5f 696e 6974  tion_suite._init
+00000a90: 5f65 7870 6563 7461 7469 6f6e 5f65 6e67  _expectation_eng
+00000aa0: 696e 6528 0a20 2020 2020 2020 2020 2020  ine(.           
+00000ab0: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+00000ac0: 5f73 746f 7265 5f69 643d 6665 6174 7572  _store_id=featur
+00000ad0: 6573 746f 7265 5f69 642c 2066 6561 7475  estore_id, featu
+00000ae0: 7265 5f67 726f 7570 5f69 643d 7365 6c66  re_group_id=self
+00000af0: 2e5f 6964 0a20 2020 2020 2020 2020 2020  ._id.           
+00000b00: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00000b10: 2020 2073 656c 662e 5f65 7870 6563 7461     self._expecta
+00000b20: 7469 6f6e 5f73 7569 7465 5f65 6e67 696e  tion_suite_engin
+00000b30: 6520 3d20 280a 2020 2020 2020 2020 2020  e = (.          
+00000b40: 2020 2020 2020 6578 7065 6374 6174 696f        expectatio
+00000b50: 6e5f 7375 6974 655f 656e 6769 6e65 2e45  n_suite_engine.E
+00000b60: 7870 6563 7461 7469 6f6e 5375 6974 6545  xpectationSuiteE
+00000b70: 6e67 696e 6528 0a20 2020 2020 2020 2020  ngine(.         
+00000b80: 2020 2020 2020 2020 2020 2066 6561 7475             featu
+00000b90: 7265 5f73 746f 7265 5f69 643d 6665 6174  re_store_id=feat
+00000ba0: 7572 6573 746f 7265 5f69 642c 2066 6561  urestore_id, fea
+00000bb0: 7475 7265 5f67 726f 7570 5f69 643d 7365  ture_group_id=se
+00000bc0: 6c66 2e5f 6964 0a20 2020 2020 2020 2020  lf._id.         
+00000bd0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00000be0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00000bf0: 2020 2073 656c 662e 5f76 616c 6964 6174     self._validat
+00000c00: 696f 6e5f 7265 706f 7274 5f65 6e67 696e  ion_report_engin
+00000c10: 6520 3d20 280a 2020 2020 2020 2020 2020  e = (.          
+00000c20: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
+00000c30: 5f72 6570 6f72 745f 656e 6769 6e65 2e56  _report_engine.V
+00000c40: 616c 6964 6174 696f 6e52 6570 6f72 7445  alidationReportE
+00000c50: 6e67 696e 6528 0a20 2020 2020 2020 2020  ngine(.         
+00000c60: 2020 2020 2020 2020 2020 2066 6561 7475             featu
+00000c70: 7265 7374 6f72 655f 6964 2c20 7365 6c66  restore_id, self
+00000c80: 2e5f 6964 0a20 2020 2020 2020 2020 2020  ._id.           
+00000c90: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00000ca0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00000cb0: 2073 656c 662e 5f76 616c 6964 6174 696f   self._validatio
+00000cc0: 6e5f 7265 7375 6c74 5f65 6e67 696e 6520  n_result_engine 
+00000cd0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00000ce0: 2020 2020 7661 6c69 6461 7469 6f6e 5f72      validation_r
+00000cf0: 6573 756c 745f 656e 6769 6e65 2e56 616c  esult_engine.Val
+00000d00: 6964 6174 696f 6e52 6573 756c 7445 6e67  idationResultEng
+00000d10: 696e 6528 0a20 2020 2020 2020 2020 2020  ine(.           
+00000d20: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+00000d30: 7374 6f72 655f 6964 2c20 7365 6c66 2e5f  store_id, self._
+00000d40: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
+00000d50: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00000d60: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
+00000d70: 2e5f 6665 6174 7572 655f 7374 6f72 655f  ._feature_store_
+00000d80: 6964 203d 2066 6561 7475 7265 7374 6f72  id = featurestor
+00000d90: 655f 6964 0a20 2020 2020 2020 2073 656c  e_id.        sel
+00000da0: 662e 5f76 6172 6961 626c 655f 6170 6920  f._variable_api 
+00000db0: 3d20 5661 7269 6162 6c65 4170 6928 290a  = VariableApi().
+00000dc0: 2020 2020 2020 2020 7365 6c66 2e5f 6665          self._fe
+00000dd0: 6174 7572 655f 6772 6f75 705f 656e 6769  ature_group_engi
+00000de0: 6e65 203d 204e 6f6e 650a 2020 2020 2020  ne = None.      
+00000df0: 2020 7365 6c66 2e5f 6d75 6c74 695f 7061    self._multi_pa
+00000e00: 7274 5f69 6e73 6572 7420 3d20 4661 6c73  rt_insert = Fals
+00000e10: 650a 0a20 2020 2064 6566 2064 656c 6574  e..    def delet
+00000e20: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00000e30: 2022 2222 4472 6f70 2074 6865 2065 6e74   """Drop the ent
+00000e40: 6972 6520 6665 6174 7572 6520 6772 6f75  ire feature grou
+00000e50: 7020 616c 6f6e 6720 7769 7468 2069 7473  p along with its
+00000e60: 2066 6561 7475 7265 2064 6174 612e 0a0a   feature data...
+00000e70: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
+00000e80: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
+00000e90: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
+00000ea0: 2020 2020 2020 2320 636f 6e6e 6563 7420        # connect 
+00000eb0: 746f 2074 6865 2046 6561 7475 7265 2053  to the Feature S
+00000ec0: 746f 7265 0a20 2020 2020 2020 2020 2020  tore.           
+00000ed0: 2066 7320 3d20 2e2e 2e0a 0a20 2020 2020   fs = .....     
+00000ee0: 2020 2020 2020 2023 2067 6574 2074 6865         # get the
+00000ef0: 2046 6561 7475 7265 2047 726f 7570 2069   Feature Group i
+00000f00: 6e73 7461 6e63 650a 2020 2020 2020 2020  nstance.        
+00000f10: 2020 2020 6667 203d 2066 732e 6765 745f      fg = fs.get_
+00000f20: 6f72 5f63 7265 6174 655f 6665 6174 7572  or_create_featur
+00000f30: 655f 6772 6f75 7028 0a20 2020 2020 2020  e_group(.       
+00000f40: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00000f50: 653d 2762 6974 636f 696e 5f70 7269 6365  e='bitcoin_price
+00000f60: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00000f70: 2020 2020 2020 2076 6572 7369 6f6e 3d31         version=1
+00000f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000f90: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00000fa0: 2020 2020 2320 6465 6c65 7465 2074 6865      # delete the
+00000fb0: 2066 6561 7475 7265 2067 726f 7570 0a20   feature group. 
+00000fc0: 2020 2020 2020 2020 2020 2066 672e 6465             fg.de
+00000fd0: 6c65 7465 2829 0a20 2020 2020 2020 2020  lete().         
+00000fe0: 2020 2060 6060 0a0a 2020 2020 2020 2020     ```..        
+00000ff0: 2121 2120 6461 6e67 6572 2022 506f 7465  !!! danger "Pote
+00001000: 6e74 6961 6c6c 7920 6461 6e67 6572 6f75  ntially dangerou
+00001010: 7320 6f70 6572 6174 696f 6e22 0a20 2020  s operation".   
+00001020: 2020 2020 2020 2020 2054 6869 7320 6f70           This op
+00001030: 6572 6174 696f 6e20 6472 6f70 7320 616c  eration drops al
+00001040: 6c20 6d65 7461 6461 7461 2061 7373 6f63  l metadata assoc
+00001050: 6961 7465 6420 7769 7468 202a 2a74 6869  iated with **thi
+00001060: 7320 7665 7273 696f 6e2a 2a20 6f66 2074  s version** of t
+00001070: 6865 0a20 2020 2020 2020 2020 2020 2066  he.            f
+00001080: 6561 7475 7265 2067 726f 7570 202a 2a61  eature group **a
+00001090: 6e64 2a2a 2061 6c6c 2074 6865 2066 6561  nd** all the fea
+000010a0: 7475 7265 2064 6174 6120 696e 206f 6666  ture data in off
+000010b0: 6c69 6e65 2061 6e64 206f 6e6c 696e 6520  line and online 
+000010c0: 7374 6f72 6167 650a 2020 2020 2020 2020  storage.        
+000010d0: 2020 2020 6173 736f 6369 6174 6564 2077      associated w
+000010e0: 6974 6820 6974 2e0a 0a20 2020 2020 2020  ith it...       
+000010f0: 2023 2052 6169 7365 730a 2020 2020 2020   # Raises.      
+00001100: 2020 2020 2020 6068 7366 732e 636c 6965        `hsfs.clie
+00001110: 6e74 2e65 7863 6570 7469 6f6e 732e 5265  nt.exceptions.Re
+00001120: 7374 4150 4945 7272 6f72 602e 0a20 2020  stAPIError`..   
+00001130: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00001140: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
+00001150: 2020 2020 2020 2020 2020 2020 2241 6c6c              "All
+00001160: 206a 6f62 7320 6173 736f 6369 6174 6564   jobs associated
+00001170: 2074 6f20 6665 6174 7572 6520 6772 6f75   to feature grou
+00001180: 7020 607b 7d60 2c20 7665 7273 696f 6e20  p `{}`, version 
+00001190: 607b 7d60 2077 696c 6c20 6265 2072 656d  `{}` will be rem
+000011a0: 6f76 6564 2e22 2e66 6f72 6d61 7428 0a20  oved.".format(. 
+000011b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000011c0: 656c 662e 5f6e 616d 652c 2073 656c 662e  elf._name, self.
+000011d0: 5f76 6572 7369 6f6e 0a20 2020 2020 2020  _version.       
+000011e0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+000011f0: 2020 2020 7574 696c 2e4a 6f62 5761 726e      util.JobWarn
+00001200: 696e 672c 0a20 2020 2020 2020 2029 0a20  ing,.        ). 
+00001210: 2020 2020 2020 2073 656c 662e 5f66 6561         self._fea
+00001220: 7475 7265 5f67 726f 7570 5f65 6e67 696e  ture_group_engin
+00001230: 652e 6465 6c65 7465 2873 656c 6629 0a0a  e.delete(self)..
+00001240: 2020 2020 6465 6620 7365 6c65 6374 5f61      def select_a
+00001250: 6c6c 280a 2020 2020 2020 2020 7365 6c66  ll(.        self
+00001260: 2c0a 2020 2020 2020 2020 696e 636c 7564  ,.        includ
+00001270: 655f 7072 696d 6172 795f 6b65 793a 204f  e_primary_key: O
+00001280: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+00001290: 5472 7565 2c0a 2020 2020 2020 2020 696e  True,.        in
+000012a0: 636c 7564 655f 6576 656e 745f 7469 6d65  clude_event_time
+000012b0: 3a20 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  : Optional[bool]
+000012c0: 203d 2054 7275 652c 0a20 2020 2029 3a0a   = True,.    ):.
+000012d0: 2020 2020 2020 2020 2222 2253 656c 6563          """Selec
+000012e0: 7420 616c 6c20 6665 6174 7572 6573 2069  t all features i
+000012f0: 6e20 7468 6520 6665 6174 7572 6520 6772  n the feature gr
+00001300: 6f75 7020 616e 6420 7265 7475 726e 2061  oup and return a
+00001310: 2071 7565 7279 206f 626a 6563 742e 0a0a   query object...
+00001320: 2020 2020 2020 2020 5468 6520 7175 6572          The quer
+00001330: 7920 6361 6e20 6265 2075 7365 6420 746f  y can be used to
+00001340: 2063 6f6e 7374 7275 6374 206a 6f69 6e73   construct joins
+00001350: 206f 6620 6665 6174 7572 6520 6772 6f75   of feature grou
+00001360: 7073 206f 7220 6372 6561 7465 2061 0a20  ps or create a. 
+00001370: 2020 2020 2020 2066 6561 7475 7265 2076         feature v
+00001380: 6965 772e 0a0a 2020 2020 2020 2020 2121  iew...        !!
+00001390: 2120 6578 616d 706c 650a 2020 2020 2020  ! example.      
+000013a0: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+000013b0: 2020 2020 2020 2020 2020 2020 2320 636f              # co
+000013c0: 6e6e 6563 7420 746f 2074 6865 2046 6561  nnect to the Fea
+000013d0: 7475 7265 2053 746f 7265 0a20 2020 2020  ture Store.     
+000013e0: 2020 2020 2020 2066 7320 3d20 2e2e 2e0a         fs = ....
+000013f0: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
+00001400: 6574 2074 6865 2046 6561 7475 7265 2047  et the Feature G
+00001410: 726f 7570 2069 6e73 7461 6e63 6573 0a20  roup instances. 
+00001420: 2020 2020 2020 2020 2020 2066 6731 203d             fg1 =
+00001430: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
+00001440: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
+00001450: 2e2e 2e29 0a20 2020 2020 2020 2020 2020  ...).           
+00001460: 2066 6732 203d 2066 732e 6765 745f 6f72   fg2 = fs.get_or
+00001470: 5f63 7265 6174 655f 6665 6174 7572 655f  _create_feature_
+00001480: 6772 6f75 7028 2e2e 2e29 0a0a 2020 2020  group(...)..    
+00001490: 2020 2020 2020 2020 2320 636f 6e73 7472          # constr
+000014a0: 7563 7420 7468 6520 7175 6572 790a 2020  uct the query.  
+000014b0: 2020 2020 2020 2020 2020 7175 6572 7920            query 
+000014c0: 3d20 6667 312e 7365 6c65 6374 5f61 6c6c  = fg1.select_all
+000014d0: 2829 2e6a 6f69 6e28 6667 322e 7365 6c65  ().join(fg2.sele
+000014e0: 6374 5f61 6c6c 2829 290a 0a20 2020 2020  ct_all())..     
+000014f0: 2020 2020 2020 2023 2073 686f 7720 6669         # show fi
+00001500: 7273 7420 3520 726f 7773 0a20 2020 2020  rst 5 rows.     
+00001510: 2020 2020 2020 2071 7565 7279 2e73 686f         query.sho
+00001520: 7728 3529 0a0a 0a20 2020 2020 2020 2020  w(5)...         
+00001530: 2020 2023 2073 656c 6563 7420 616c 6c20     # select all 
+00001540: 6665 6174 7572 6573 2065 7863 6c75 6465  features exclude
+00001550: 2070 7269 6d61 7279 206b 6579 2061 6e64   primary key and
+00001560: 2065 7665 6e74 2074 696d 650a 2020 2020   event time.    
+00001570: 2020 2020 2020 2020 6672 6f6d 2068 7366          from hsf
+00001580: 732e 6665 6174 7572 6520 696d 706f 7274  s.feature import
+00001590: 2046 6561 7475 7265 0a20 2020 2020 2020   Feature.       
+000015a0: 2020 2020 2066 6720 3d20 6673 2e63 7265       fg = fs.cre
+000015b0: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
+000015c0: 7028 0a20 2020 2020 2020 2020 2020 2020  p(.             
+000015d0: 2020 2020 2020 2022 6667 222c 0a20 2020         "fg",.   
+000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015f0: 2066 6561 7475 7265 733d 5b0a 2020 2020   features=[.    
+00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001610: 2020 2020 2020 2020 4665 6174 7572 6528          Feature(
+00001620: 2269 6422 2c20 7479 7065 3d22 7374 7269  "id", type="stri
+00001630: 6e67 2229 2c0a 2020 2020 2020 2020 2020  ng"),.          
+00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001650: 2020 4665 6174 7572 6528 2274 7322 2c20    Feature("ts", 
+00001660: 7479 7065 3d22 6269 6769 6e74 2229 2c0a  type="bigint"),.
+00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001680: 2020 2020 2020 2020 2020 2020 4665 6174              Feat
+00001690: 7572 6528 2266 3122 2c20 7479 7065 3d22  ure("f1", type="
+000016a0: 6461 7465 2229 2c0a 2020 2020 2020 2020  date"),.        
+000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016c0: 2020 2020 4665 6174 7572 6528 2266 3222      Feature("f2"
+000016d0: 2c20 7479 7065 3d22 646f 7562 6c65 2229  , type="double")
+000016e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000016f0: 2020 2020 2020 2020 2020 2020 205d 2c0a               ],.
+00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001710: 2020 2020 7072 696d 6172 795f 6b65 793d      primary_key=
+00001720: 5b22 6964 225d 2c0a 2020 2020 2020 2020  ["id"],.        
+00001730: 2020 2020 2020 2020 2020 2020 6576 656e              even
+00001740: 745f 7469 6d65 3d22 7473 2229 0a0a 2020  t_time="ts")..  
+00001750: 2020 2020 2020 2020 2020 7175 6572 7920            query 
+00001760: 3d20 6667 2e73 656c 6563 745f 616c 6c28  = fg.select_all(
+00001770: 290a 2020 2020 2020 2020 2020 2020 7175  ).            qu
+00001780: 6572 792e 6665 6174 7572 6573 0a20 2020  ery.features.   
+00001790: 2020 2020 2020 2020 2023 205b 4665 6174           # [Feat
+000017a0: 7572 6528 2769 6427 2c20 2e2e 2e29 2c20  ure('id', ...), 
+000017b0: 4665 6174 7572 6528 2774 7327 2c20 2e2e  Feature('ts', ..
+000017c0: 2e29 2c20 4665 6174 7572 6528 2766 3127  .), Feature('f1'
+000017d0: 2c20 2e2e 2e29 2c20 4665 6174 7572 6528  , ...), Feature(
+000017e0: 2766 3227 2c20 2e2e 2e29 5d0a 0a20 2020  'f2', ...)]..   
+000017f0: 2020 2020 2020 2020 2071 7565 7279 203d           query =
+00001800: 2066 672e 7365 6c65 6374 5f61 6c6c 2869   fg.select_all(i
+00001810: 6e63 6c75 6465 5f70 7269 6d61 7279 5f6b  nclude_primary_k
+00001820: 6579 3d46 616c 7365 2c20 696e 636c 7564  ey=False, includ
+00001830: 655f 6576 656e 745f 7469 6d65 3d46 616c  e_event_time=Fal
+00001840: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+00001850: 7175 6572 792e 6665 6174 7572 6573 0a20  query.features. 
+00001860: 2020 2020 2020 2020 2020 2023 205b 4665             # [Fe
+00001870: 6174 7572 6528 2766 3127 2c20 2e2e 2e29  ature('f1', ...)
+00001880: 2c20 4665 6174 7572 6528 2766 3227 2c20  , Feature('f2', 
+00001890: 2e2e 2e29 5d0a 2020 2020 2020 2020 2020  ...)].          
+000018a0: 2020 6060 600a 0a20 2020 2020 2020 2023    ```..        #
+000018b0: 2041 7267 756d 656e 7473 0a20 2020 2020   Arguments.     
+000018c0: 2020 2020 2020 2069 6e63 6c75 6465 5f70         include_p
+000018d0: 7269 6d61 7279 5f6b 6579 3a20 4966 2054  rimary_key: If T
+000018e0: 7275 652c 2069 6e63 6c75 6465 2070 7269  rue, include pri
+000018f0: 6d61 7279 206b 6579 206f 6620 7468 6520  mary key of the 
+00001900: 6665 6174 7572 6520 6772 6f75 700a 2020  feature group.  
+00001910: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00001920: 2074 6865 2066 6561 7475 7265 206c 6973   the feature lis
+00001930: 742e 2044 6566 6175 6c74 7320 746f 2054  t. Defaults to T
+00001940: 7275 652e 0a20 2020 2020 2020 2020 2020  rue..           
+00001950: 2069 6e63 6c75 6465 5f65 7665 6e74 5f74   include_event_t
+00001960: 696d 653a 2049 6620 5472 7565 2c20 696e  ime: If True, in
+00001970: 636c 7564 6520 6576 656e 7420 7469 6d65  clude event time
+00001980: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
+00001990: 6772 6f75 700a 2020 2020 2020 2020 2020  group.          
+000019a0: 2020 2020 2020 746f 2074 6865 2066 6561        to the fea
+000019b0: 7475 7265 206c 6973 742e 2044 6566 6175  ture list. Defau
+000019c0: 6c74 7320 746f 2054 7275 652e 0a20 2020  lts to True..   
+000019d0: 2020 2020 2023 2052 6574 7572 6e73 0a20       # Returns. 
+000019e0: 2020 2020 2020 2020 2020 2060 5175 6572             `Quer
+000019f0: 7960 2e20 4120 7175 6572 7920 6f62 6a65  y`. A query obje
+00001a00: 6374 2077 6974 6820 616c 6c20 6665 6174  ct with all feat
+00001a10: 7572 6573 206f 6620 7468 6520 6665 6174  ures of the feat
+00001a20: 7572 6520 6772 6f75 702e 0a20 2020 2020  ure group..     
+00001a30: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00001a40: 6620 696e 636c 7564 655f 6576 656e 745f  f include_event_
+00001a50: 7469 6d65 2061 6e64 2069 6e63 6c75 6465  time and include
+00001a60: 5f70 7269 6d61 7279 5f6b 6579 3a0a 2020  _primary_key:.  
+00001a70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00001a80: 2071 7565 7279 2e51 7565 7279 280a 2020   query.Query(.  
+00001a90: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+00001aa0: 6674 5f66 6561 7475 7265 5f67 726f 7570  ft_feature_group
+00001ab0: 3d73 656c 662c 0a20 2020 2020 2020 2020  =self,.         
+00001ac0: 2020 2020 2020 206c 6566 745f 6665 6174         left_feat
+00001ad0: 7572 6573 3d73 656c 662e 5f66 6561 7475  ures=self._featu
+00001ae0: 7265 732c 0a20 2020 2020 2020 2020 2020  res,.           
+00001af0: 2020 2020 2066 6561 7475 7265 5f73 746f       feature_sto
+00001b00: 7265 5f6e 616d 653d 7365 6c66 2e5f 6665  re_name=self._fe
+00001b10: 6174 7572 655f 7374 6f72 655f 6e61 6d65  ature_store_name
+00001b20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001b30: 2020 6665 6174 7572 655f 7374 6f72 655f    feature_store_
+00001b40: 6964 3d73 656c 662e 5f66 6561 7475 7265  id=self._feature
+00001b50: 5f73 746f 7265 5f69 642c 0a20 2020 2020  _store_id,.     
+00001b60: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00001b70: 2065 6c69 6620 696e 636c 7564 655f 6576   elif include_ev
+00001b80: 656e 745f 7469 6d65 3a0a 2020 2020 2020  ent_time:.      
+00001b90: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00001ba0: 662e 7365 6c65 6374 5f65 7863 6570 7428  f.select_except(
+00001bb0: 7365 6c66 2e70 7269 6d61 7279 5f6b 6579  self.primary_key
+00001bc0: 290a 2020 2020 2020 2020 656c 6966 2069  ).        elif i
+00001bd0: 6e63 6c75 6465 5f70 7269 6d61 7279 5f6b  nclude_primary_k
+00001be0: 6579 3a0a 2020 2020 2020 2020 2020 2020  ey:.            
+00001bf0: 7265 7475 726e 2073 656c 662e 7365 6c65  return self.sele
+00001c00: 6374 5f65 7863 6570 7428 5b73 656c 662e  ct_except([self.
+00001c10: 6576 656e 745f 7469 6d65 5d29 0a20 2020  event_time]).   
+00001c20: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00001c30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00001c40: 6c66 2e73 656c 6563 745f 6578 6365 7074  lf.select_except
+00001c50: 2873 656c 662e 7072 696d 6172 795f 6b65  (self.primary_ke
+00001c60: 7920 2b20 5b73 656c 662e 6576 656e 745f  y + [self.event_
+00001c70: 7469 6d65 5d29 0a0a 2020 2020 6465 6620  time])..    def 
+00001c80: 7365 6c65 6374 2873 656c 662c 2066 6561  select(self, fea
+00001c90: 7475 7265 733a 204f 7074 696f 6e61 6c5b  tures: Optional[
+00001ca0: 4c69 7374 5b55 6e69 6f6e 5b73 7472 2c20  List[Union[str, 
+00001cb0: 6665 6174 7572 652e 4665 6174 7572 655d  feature.Feature]
+00001cc0: 5d5d 203d 205b 5d29 3a0a 2020 2020 2020  ]] = []):.      
+00001cd0: 2020 2222 2253 656c 6563 7420 6120 7375    """Select a su
+00001ce0: 6273 6574 206f 6620 6665 6174 7572 6573  bset of features
+00001cf0: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
+00001d00: 6772 6f75 7020 616e 6420 7265 7475 726e  group and return
+00001d10: 2061 2071 7565 7279 206f 626a 6563 742e   a query object.
+00001d20: 0a0a 2020 2020 2020 2020 5468 6520 7175  ..        The qu
+00001d30: 6572 7920 6361 6e20 6265 2075 7365 6420  ery can be used 
+00001d40: 746f 2063 6f6e 7374 7275 6374 206a 6f69  to construct joi
+00001d50: 6e73 206f 6620 6665 6174 7572 6520 6772  ns of feature gr
+00001d60: 6f75 7073 206f 7220 6372 6561 7465 2061  oups or create a
+00001d70: 0a20 2020 2020 2020 2066 6561 7475 7265  .        feature
+00001d80: 2076 6965 7720 7769 7468 2061 2073 7562   view with a sub
+00001d90: 7365 7420 6f66 2066 6561 7475 7265 7320  set of features 
+00001da0: 6f66 2074 6865 2066 6561 7475 7265 2067  of the feature g
+00001db0: 726f 7570 2e0a 0a20 2020 2020 2020 2021  roup...        !
+00001dc0: 2121 2065 7861 6d70 6c65 0a20 2020 2020  !! example.     
+00001dd0: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+00001de0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+00001df0: 6f6e 6e65 6374 2074 6f20 7468 6520 4665  onnect to the Fe
+00001e00: 6174 7572 6520 5374 6f72 650a 2020 2020  ature Store.    
+00001e10: 2020 2020 2020 2020 6673 203d 202e 2e2e          fs = ...
+00001e20: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00001e30: 6765 7420 7468 6520 4665 6174 7572 6520  get the Feature 
+00001e40: 4772 6f75 7020 696e 7374 616e 6365 0a20  Group instance. 
+00001e50: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
+00001e60: 6873 6673 2e66 6561 7475 7265 2069 6d70  hsfs.feature imp
+00001e70: 6f72 7420 4665 6174 7572 650a 2020 2020  ort Feature.    
+00001e80: 2020 2020 2020 2020 6667 203d 2066 732e          fg = fs.
+00001e90: 6372 6561 7465 5f66 6561 7475 7265 5f67  create_feature_g
+00001ea0: 726f 7570 280a 2020 2020 2020 2020 2020  roup(.          
+00001eb0: 2020 2020 2020 2020 2020 2266 6722 2c0a            "fg",.
+00001ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ed0: 2020 2020 6665 6174 7572 6573 3d5b 0a20      features=[. 
+00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ef0: 2020 2020 2020 2020 2020 2046 6561 7475             Featu
+00001f00: 7265 2822 6964 222c 2074 7970 653d 2273  re("id", type="s
+00001f10: 7472 696e 6722 292c 0a20 2020 2020 2020  tring"),.       
+00001f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f30: 2020 2020 2046 6561 7475 7265 2822 7473       Feature("ts
+00001f40: 222c 2074 7970 653d 2262 6967 696e 7422  ", type="bigint"
+00001f50: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00001f60: 2020 2020 2020 2020 2020 2020 2020 2046                 F
+00001f70: 6561 7475 7265 2822 6631 222c 2074 7970  eature("f1", typ
+00001f80: 653d 2264 6174 6522 292c 0a20 2020 2020  e="date"),.     
+00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fa0: 2020 2020 2020 2046 6561 7475 7265 2822         Feature("
+00001fb0: 6632 222c 2074 7970 653d 2264 6f75 626c  f2", type="doubl
+00001fc0: 6522 290a 2020 2020 2020 2020 2020 2020  e").            
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fe0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00001ff0: 2020 2020 2020 2070 7269 6d61 7279 5f6b         primary_k
+00002000: 6579 3d5b 2269 6422 5d2c 0a20 2020 2020  ey=["id"],.     
+00002010: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00002020: 7665 6e74 5f74 696d 653d 2274 7322 290a  vent_time="ts").
+00002030: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+00002040: 6f6e 7374 7275 6374 2071 7565 7279 0a20  onstruct query. 
+00002050: 2020 2020 2020 2020 2020 2071 7565 7279             query
+00002060: 203d 2066 672e 7365 6c65 6374 285b 2269   = fg.select(["i
+00002070: 6422 2c20 2266 3122 5d29 0a20 2020 2020  d", "f1"]).     
+00002080: 2020 2020 2020 2071 7565 7279 2e66 6561         query.fea
+00002090: 7475 7265 730a 2020 2020 2020 2020 2020  tures.          
+000020a0: 2020 2320 5b46 6561 7475 7265 2827 6964    # [Feature('id
+000020b0: 272c 202e 2e2e 292c 2046 6561 7475 7265  ', ...), Feature
+000020c0: 2827 6631 272c 202e 2e2e 295d 0a20 2020  ('f1', ...)].   
+000020d0: 2020 2020 2020 2020 2060 6060 0a0a 2020           ```..  
+000020e0: 2020 2020 2020 2320 4172 6775 6d65 6e74        # Argument
+000020f0: 730a 2020 2020 2020 2020 2020 2020 6665  s.            fe
+00002100: 6174 7572 6573 3a20 4120 6c69 7374 206f  atures: A list o
+00002110: 6620 6046 6561 7475 7265 6020 6f62 6a65  f `Feature` obje
+00002120: 6374 7320 6f72 2066 6561 7475 7265 206e  cts or feature n
+00002130: 616d 6573 2061 730a 2020 2020 2020 2020  ames as.        
+00002140: 2020 2020 2020 2020 7374 7269 6e67 7320          strings 
+00002150: 746f 2062 6520 7365 6c65 6374 6564 2c20  to be selected, 
+00002160: 6465 6661 756c 7473 2074 6f20 5b5d 2e0a  defaults to []..
+00002170: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
+00002180: 6e73 0a20 2020 2020 2020 2020 2020 2060  ns.            `
+00002190: 5175 6572 7960 3a20 4120 7175 6572 7920  Query`: A query 
+000021a0: 6f62 6a65 6374 2077 6974 6820 7468 6520  object with the 
+000021b0: 7365 6c65 6374 6564 2066 6561 7475 7265  selected feature
+000021c0: 7320 6f66 2074 6865 2066 6561 7475 7265  s of the feature
+000021d0: 2067 726f 7570 2e0a 2020 2020 2020 2020   group..        
+000021e0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+000021f0: 726e 2071 7565 7279 2e51 7565 7279 280a  rn query.Query(.
+00002200: 2020 2020 2020 2020 2020 2020 6c65 6674              left
+00002210: 5f66 6561 7475 7265 5f67 726f 7570 3d73  _feature_group=s
+00002220: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00002230: 206c 6566 745f 6665 6174 7572 6573 3d66   left_features=f
+00002240: 6561 7475 7265 732c 0a20 2020 2020 2020  eatures,.       
+00002250: 2020 2020 2066 6561 7475 7265 5f73 746f       feature_sto
+00002260: 7265 5f6e 616d 653d 7365 6c66 2e5f 6665  re_name=self._fe
+00002270: 6174 7572 655f 7374 6f72 655f 6e61 6d65  ature_store_name
+00002280: 2c0a 2020 2020 2020 2020 2020 2020 6665  ,.            fe
+00002290: 6174 7572 655f 7374 6f72 655f 6964 3d73  ature_store_id=s
+000022a0: 656c 662e 5f66 6561 7475 7265 5f73 746f  elf._feature_sto
+000022b0: 7265 5f69 642c 0a20 2020 2020 2020 2029  re_id,.        )
+000022c0: 0a0a 2020 2020 6465 6620 7365 6c65 6374  ..    def select
+000022d0: 5f65 7863 6570 7428 7365 6c66 2c20 6665  _except(self, fe
+000022e0: 6174 7572 6573 3a20 4f70 7469 6f6e 616c  atures: Optional
+000022f0: 5b4c 6973 745b 556e 696f 6e5b 7374 722c  [List[Union[str,
+00002300: 2066 6561 7475 7265 2e46 6561 7475 7265   feature.Feature
+00002310: 5d5d 5d20 3d20 5b5d 293a 0a20 2020 2020  ]]] = []):.     
+00002320: 2020 2022 2222 5365 6c65 6374 2061 6c6c     """Select all
+00002330: 2066 6561 7475 7265 7320 696e 636c 7564   features includ
+00002340: 696e 6720 7072 696d 6172 7920 6b65 7920  ing primary key 
+00002350: 616e 6420 6576 656e 7420 7469 6d65 2066  and event time f
+00002360: 6561 7475 7265 0a20 2020 2020 2020 206f  eature.        o
+00002370: 6620 7468 6520 6665 6174 7572 6520 6772  f the feature gr
+00002380: 6f75 7020 6578 6365 7074 2070 726f 7669  oup except provi
+00002390: 6465 6420 6066 6561 7475 7265 7360 2061  ded `features` a
+000023a0: 6e64 2072 6574 7572 6e20 6120 7175 6572  nd return a quer
+000023b0: 7920 6f62 6a65 6374 2e0a 0a20 2020 2020  y object...     
+000023c0: 2020 2054 6865 2071 7565 7279 2063 616e     The query can
+000023d0: 2062 6520 7573 6564 2074 6f20 636f 6e73   be used to cons
+000023e0: 7472 7563 7420 6a6f 696e 7320 6f66 2066  truct joins of f
+000023f0: 6561 7475 7265 2067 726f 7570 7320 6f72  eature groups or
+00002400: 2063 7265 6174 6520 610a 2020 2020 2020   create a.      
+00002410: 2020 6665 6174 7572 6520 7669 6577 2077    feature view w
+00002420: 6974 6820 6120 7375 6273 6574 206f 6620  ith a subset of 
+00002430: 6665 6174 7572 6573 206f 6620 7468 6520  features of the 
+00002440: 6665 6174 7572 6520 6772 6f75 702e 0a0a  feature group...
+00002450: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
+00002460: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
+00002470: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
+00002480: 2020 2020 2020 2320 636f 6e6e 6563 7420        # connect 
+00002490: 746f 2074 6865 2046 6561 7475 7265 2053  to the Feature S
+000024a0: 746f 7265 0a20 2020 2020 2020 2020 2020  tore.           
+000024b0: 2066 7320 3d20 2e2e 2e0a 0a20 2020 2020   fs = .....     
+000024c0: 2020 2020 2020 2023 2067 6574 2074 6865         # get the
+000024d0: 2046 6561 7475 7265 2047 726f 7570 2069   Feature Group i
+000024e0: 6e73 7461 6e63 650a 2020 2020 2020 2020  nstance.        
+000024f0: 2020 2020 6672 6f6d 2068 7366 732e 6665      from hsfs.fe
+00002500: 6174 7572 6520 696d 706f 7274 2046 6561  ature import Fea
+00002510: 7475 7265 0a20 2020 2020 2020 2020 2020  ture.           
+00002520: 2066 6720 3d20 6673 2e63 7265 6174 655f   fg = fs.create_
+00002530: 6665 6174 7572 655f 6772 6f75 7028 0a20  feature_group(. 
+00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002550: 2020 2022 6667 222c 0a20 2020 2020 2020     "fg",.       
+00002560: 2020 2020 2020 2020 2020 2020 2066 6561               fea
+00002570: 7475 7265 733d 5b0a 2020 2020 2020 2020  tures=[.        
+00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002590: 2020 2020 4665 6174 7572 6528 2269 6422      Feature("id"
+000025a0: 2c20 7479 7065 3d22 7374 7269 6e67 2229  , type="string")
+000025b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000025c0: 2020 2020 2020 2020 2020 2020 2020 4665                Fe
+000025d0: 6174 7572 6528 2274 7322 2c20 7479 7065  ature("ts", type
+000025e0: 3d22 6269 6769 6e74 2229 2c0a 2020 2020  ="bigint"),.    
+000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002600: 2020 2020 2020 2020 4665 6174 7572 6528          Feature(
+00002610: 2266 3122 2c20 7479 7065 3d22 6461 7465  "f1", type="date
+00002620: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002640: 4665 6174 7572 6528 2266 3222 2c20 7479  Feature("f2", ty
+00002650: 7065 3d22 646f 7562 6c65 2229 0a20 2020  pe="double").   
+00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002670: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002690: 7072 696d 6172 795f 6b65 793d 5b22 6964  primary_key=["id
+000026a0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+000026b0: 2020 2020 2020 2020 6576 656e 745f 7469          event_ti
+000026c0: 6d65 3d22 7473 2229 0a0a 2020 2020 2020  me="ts")..      
+000026d0: 2020 2020 2020 2320 636f 6e73 7472 7563        # construc
+000026e0: 7420 7175 6572 790a 2020 2020 2020 2020  t query.        
+000026f0: 2020 2020 7175 6572 7920 3d20 6667 2e73      query = fg.s
+00002700: 656c 6563 745f 6578 6365 7074 285b 2274  elect_except(["t
+00002710: 7322 2c20 2266 3122 5d29 0a20 2020 2020  s", "f1"]).     
+00002720: 2020 2020 2020 2071 7565 7279 2e66 6561         query.fea
+00002730: 7475 7265 730a 2020 2020 2020 2020 2020  tures.          
+00002740: 2020 2320 5b46 6561 7475 7265 2827 6964    # [Feature('id
+00002750: 272c 202e 2e2e 292c 2046 6561 7475 7265  ', ...), Feature
+00002760: 2827 6631 272c 202e 2e2e 295d 0a20 2020  ('f1', ...)].   
+00002770: 2020 2020 2020 2020 2060 6060 0a0a 2020           ```..  
+00002780: 2020 2020 2020 2320 4172 6775 6d65 6e74        # Argument
+00002790: 730a 2020 2020 2020 2020 2020 2020 6665  s.            fe
+000027a0: 6174 7572 6573 3a20 4120 6c69 7374 206f  atures: A list o
+000027b0: 6620 6046 6561 7475 7265 6020 6f62 6a65  f `Feature` obje
+000027c0: 6374 7320 6f72 2066 6561 7475 7265 206e  cts or feature n
+000027d0: 616d 6573 2061 730a 2020 2020 2020 2020  ames as.        
+000027e0: 2020 2020 2020 2020 7374 7269 6e67 7320          strings 
+000027f0: 746f 2062 6520 6578 636c 7564 6564 2066  to be excluded f
+00002800: 726f 6d20 7468 6520 7365 6c65 6374 696f  rom the selectio
+00002810: 6e2e 2044 6566 6175 6c74 7320 746f 205b  n. Defaults to [
+00002820: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00002830: 2020 2073 656c 6563 7469 6e67 2061 6c6c     selecting all
+00002840: 2066 6561 7475 7265 732e 0a0a 2020 2020   features...    
+00002850: 2020 2020 2320 5265 7475 726e 730a 2020      # Returns.  
+00002860: 2020 2020 2020 2020 2020 6051 7565 7279            `Query
+00002870: 603a 2041 2071 7565 7279 206f 626a 6563  `: A query objec
+00002880: 7420 7769 7468 2074 6865 2073 656c 6563  t with the selec
+00002890: 7465 6420 6665 6174 7572 6573 206f 6620  ted features of 
+000028a0: 7468 6520 6665 6174 7572 6520 6772 6f75  the feature grou
+000028b0: 702e 0a20 2020 2020 2020 2022 2222 0a20  p..        """. 
+000028c0: 2020 2020 2020 2069 6620 6665 6174 7572         if featur
+000028d0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+000028e0: 6578 6365 7074 5f66 6561 7475 7265 7320  except_features 
+000028f0: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00002900: 2020 2020 662e 6e61 6d65 2069 6620 6973      f.name if is
+00002910: 696e 7374 616e 6365 2866 2c20 6665 6174  instance(f, feat
+00002920: 7572 652e 4665 6174 7572 6529 2065 6c73  ure.Feature) els
+00002930: 6520 6620 666f 7220 6620 696e 2066 6561  e f for f in fea
+00002940: 7475 7265 730a 2020 2020 2020 2020 2020  tures.          
+00002950: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+00002960: 7265 7475 726e 2071 7565 7279 2e51 7565  return query.Que
+00002970: 7279 280a 2020 2020 2020 2020 2020 2020  ry(.            
+00002980: 2020 2020 6c65 6674 5f66 6561 7475 7265      left_feature
+00002990: 5f67 726f 7570 3d73 656c 662c 0a20 2020  _group=self,.   
+000029a0: 2020 2020 2020 2020 2020 2020 206c 6566               lef
+000029b0: 745f 6665 6174 7572 6573 3d5b 0a20 2020  t_features=[.   
+000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029d0: 2066 2066 6f72 2066 2069 6e20 7365 6c66   f for f in self
+000029e0: 2e5f 6665 6174 7572 6573 2069 6620 662e  ._features if f.
+000029f0: 6e61 6d65 206e 6f74 2069 6e20 6578 6365  name not in exce
+00002a00: 7074 5f66 6561 7475 7265 730a 2020 2020  pt_features.    
+00002a10: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
+00002a20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00002a30: 6561 7475 7265 5f73 746f 7265 5f6e 616d  eature_store_nam
+00002a40: 653d 7365 6c66 2e5f 6665 6174 7572 655f  e=self._feature_
+00002a50: 7374 6f72 655f 6e61 6d65 2c0a 2020 2020  store_name,.    
+00002a60: 2020 2020 2020 2020 2020 2020 6665 6174              feat
+00002a70: 7572 655f 7374 6f72 655f 6964 3d73 656c  ure_store_id=sel
+00002a80: 662e 5f66 6561 7475 7265 5f73 746f 7265  f._feature_store
+00002a90: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+00002aa0: 2029 0a20 2020 2020 2020 2065 6c73 653a   ).        else:
+00002ab0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00002ac0: 7572 6e20 7365 6c66 2e73 656c 6563 745f  urn self.select_
+00002ad0: 616c 6c28 290a 0a20 2020 2064 6566 2066  all()..    def f
+00002ae0: 696c 7465 7228 7365 6c66 2c20 663a 2055  ilter(self, f: U
+00002af0: 6e69 6f6e 5b66 696c 7465 722e 4669 6c74  nion[filter.Filt
+00002b00: 6572 2c20 6669 6c74 6572 2e4c 6f67 6963  er, filter.Logic
+00002b10: 5d29 3a0a 2020 2020 2020 2020 2222 2241  ]):.        """A
+00002b20: 7070 6c79 2066 696c 7465 7220 746f 2074  pply filter to t
+00002b30: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
+00002b40: 2e0a 0a20 2020 2020 2020 2053 656c 6563  ...        Selec
+00002b50: 7473 2061 6c6c 2066 6561 7475 7265 7320  ts all features 
+00002b60: 616e 6420 7265 7475 726e 7320 7468 6520  and returns the 
+00002b70: 7265 7375 6c74 696e 6720 6051 7565 7279  resulting `Query
+00002b80: 6020 7769 7468 2074 6865 2061 7070 6c69  ` with the appli
+00002b90: 6564 2066 696c 7465 722e 0a20 2020 2020  ed filter..     
+00002ba0: 2020 2021 2121 2065 7861 6d70 6c65 0a20     !!! example. 
+00002bb0: 2020 2020 2020 2020 2020 2060 6060 7079             ```py
+00002bc0: 7468 6f6e 0a20 2020 2020 2020 2020 2020  thon.           
+00002bd0: 2066 726f 6d20 6873 6673 2e66 6561 7475   from hsfs.featu
+00002be0: 7265 2069 6d70 6f72 7420 4665 6174 7572  re import Featur
+00002bf0: 650a 0a20 2020 2020 2020 2020 2020 2023  e..            #
+00002c00: 2063 6f6e 6e65 6374 2074 6f20 7468 6520   connect to the 
+00002c10: 4665 6174 7572 6520 5374 6f72 650a 2020  Feature Store.  
+00002c20: 2020 2020 2020 2020 2020 6673 203d 202e            fs = .
+00002c30: 2e2e 0a0a 2020 2020 2020 2020 2020 2020  ....            
+00002c40: 2320 6765 7420 7468 6520 4665 6174 7572  # get the Featur
+00002c50: 6520 4772 6f75 7020 696e 7374 616e 6365  e Group instance
+00002c60: 0a20 2020 2020 2020 2020 2020 2066 6720  .            fg 
+00002c70: 3d20 6673 2e67 6574 5f6f 725f 6372 6561  = fs.get_or_crea
+00002c80: 7465 5f66 6561 7475 7265 5f67 726f 7570  te_feature_group
+00002c90: 282e 2e2e 290a 0a20 2020 2020 2020 2020  (...)..         
+00002ca0: 2020 2066 672e 6669 6c74 6572 2846 6561     fg.filter(Fea
+00002cb0: 7475 7265 2822 7765 656b 6c79 5f73 616c  ture("weekly_sal
+00002cc0: 6573 2229 203e 2031 3030 3029 0a20 2020  es") > 1000).   
+00002cd0: 2020 2020 2020 2020 2060 6060 0a0a 2020           ```..  
+00002ce0: 2020 2020 2020 4966 2079 6f75 2061 7265        If you are
+00002cf0: 2070 6c61 6e6e 696e 6720 746f 206a 6f69   planning to joi
+00002d00: 6e20 7468 6520 6669 6c74 6572 6564 2066  n the filtered f
+00002d10: 6561 7475 7265 2067 726f 7570 206c 6174  eature group lat
+00002d20: 6572 206f 6e20 7769 7468 2061 6e6f 7468  er on with anoth
+00002d30: 6572 0a20 2020 2020 2020 2066 6561 7475  er.        featu
+00002d40: 7265 2067 726f 7570 2c20 6d61 6b65 2073  re group, make s
+00002d50: 7572 6520 746f 2073 656c 6563 7420 7468  ure to select th
+00002d60: 6520 6669 6c74 6572 6564 2066 6561 7475  e filtered featu
+00002d70: 7265 2065 7870 6c69 6369 746c 7920 6672  re explicitly fr
+00002d80: 6f6d 2074 6865 0a20 2020 2020 2020 2072  om the.        r
+00002d90: 6573 7065 6374 6976 6520 6665 6174 7572  espective featur
+00002da0: 6520 6772 6f75 703a 0a20 2020 2020 2020  e group:.       
+00002db0: 2021 2121 2065 7861 6d70 6c65 0a20 2020   !!! example.   
+00002dc0: 2020 2020 2020 2020 2060 6060 7079 7468           ```pyth
+00002dd0: 6f6e 0a20 2020 2020 2020 2020 2020 2066  on.            f
+00002de0: 672e 6669 6c74 6572 2866 672e 6665 6174  g.filter(fg.feat
+00002df0: 7572 6531 203d 3d20 3129 2e73 686f 7728  ure1 == 1).show(
+00002e00: 3130 290a 2020 2020 2020 2020 2020 2020  10).            
+00002e10: 6060 600a 0a20 2020 2020 2020 2043 6f6d  ```..        Com
+00002e20: 706f 7369 7465 2066 696c 7465 7273 2072  posite filters r
+00002e30: 6571 7569 7265 2070 6172 656e 7468 6573  equire parenthes
+00002e40: 6973 3a0a 2020 2020 2020 2020 2121 2120  is:.        !!! 
+00002e50: 6578 616d 706c 650a 2020 2020 2020 2020  example.        
+00002e60: 2020 2020 6060 6070 7974 686f 6e0a 2020      ```python.  
+00002e70: 2020 2020 2020 2020 2020 6667 2e66 696c            fg.fil
+00002e80: 7465 7228 2866 672e 6665 6174 7572 6531  ter((fg.feature1
+00002e90: 203d 3d20 3129 207c 2028 6667 2e66 6561   == 1) | (fg.fea
+00002ea0: 7475 7265 3220 3e3d 2032 2929 0a20 2020  ture2 >= 2)).   
+00002eb0: 2020 2020 2020 2020 2060 6060 0a0a 2020           ```..  
+00002ec0: 2020 2020 2020 2320 4172 6775 6d65 6e74        # Argument
+00002ed0: 730a 2020 2020 2020 2020 2020 2020 663a  s.            f:
+00002ee0: 2046 696c 7465 7220 6f62 6a65 6374 2e0a   Filter object..
+00002ef0: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
+00002f00: 6e73 0a20 2020 2020 2020 2020 2020 2060  ns.            `
+00002f10: 5175 6572 7960 2e20 5468 6520 7175 6572  Query`. The quer
+00002f20: 7920 6f62 6a65 6374 2077 6974 6820 7468  y object with th
+00002f30: 6520 6170 706c 6965 6420 6669 6c74 6572  e applied filter
+00002f40: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00002f50: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00002f60: 662e 7365 6c65 6374 5f61 6c6c 2829 2e66  f.select_all().f
+00002f70: 696c 7465 7228 6629 0a0a 2020 2020 6465  ilter(f)..    de
+00002f80: 6620 6164 645f 7461 6728 7365 6c66 2c20  f add_tag(self, 
+00002f90: 6e61 6d65 3a20 7374 722c 2076 616c 7565  name: str, value
+00002fa0: 293a 0a20 2020 2020 2020 2022 2222 4174  ):.        """At
+00002fb0: 7461 6368 2061 2074 6167 2074 6f20 6120  tach a tag to a 
+00002fc0: 6665 6174 7572 6520 6772 6f75 702e 0a0a  feature group...
+00002fd0: 2020 2020 2020 2020 4120 7461 6720 636f          A tag co
+00002fe0: 6e73 6973 7473 206f 6620 6120 3c6e 616d  nsists of a <nam
+00002ff0: 652c 7661 6c75 653e 2070 6169 722e 2054  e,value> pair. T
+00003000: 6167 206e 616d 6573 2061 7265 2075 6e69  ag names are uni
+00003010: 7175 6520 6964 656e 7469 6669 6572 7320  que identifiers 
+00003020: 6163 726f 7373 2074 6865 2077 686f 6c65  across the whole
+00003030: 2063 6c75 7374 6572 2e0a 2020 2020 2020   cluster..      
+00003040: 2020 5468 6520 7661 6c75 6520 6f66 2061    The value of a
+00003050: 2074 6167 2063 616e 2062 6520 616e 7920   tag can be any 
+00003060: 7661 6c69 6420 6a73 6f6e 202d 2070 7269  valid json - pri
+00003070: 6d69 7469 7665 732c 2061 7272 6179 7320  mitives, arrays 
+00003080: 6f72 206a 736f 6e20 6f62 6a65 6374 732e  or json objects.
+00003090: 0a0a 2020 2020 2020 2020 2121 2120 6578  ..        !!! ex
+000030a0: 616d 706c 650a 2020 2020 2020 2020 2020  ample.          
+000030b0: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
+000030c0: 2020 2020 2020 2020 2320 636f 6e6e 6563          # connec
+000030d0: 7420 746f 2074 6865 2046 6561 7475 7265  t to the Feature
+000030e0: 2053 746f 7265 0a20 2020 2020 2020 2020   Store.         
+000030f0: 2020 2066 7320 3d20 2e2e 2e0a 0a20 2020     fs = .....   
+00003100: 2020 2020 2020 2020 2023 2067 6574 2074           # get t
+00003110: 6865 2046 6561 7475 7265 2047 726f 7570  he Feature Group
+00003120: 2069 6e73 7461 6e63 650a 2020 2020 2020   instance.      
+00003130: 2020 2020 2020 6667 203d 2066 732e 6765        fg = fs.ge
+00003140: 745f 6f72 5f63 7265 6174 655f 6665 6174  t_or_create_feat
+00003150: 7572 655f 6772 6f75 7028 2e2e 2e29 0a0a  ure_group(...)..
+00003160: 2020 2020 2020 2020 2020 2020 6667 2e61              fg.a
+00003170: 6464 5f74 6167 286e 616d 653d 2265 7861  dd_tag(name="exa
+00003180: 6d70 6c65 5f74 6167 222c 2076 616c 7565  mple_tag", value
+00003190: 3d22 3432 2229 0a20 2020 2020 2020 2020  ="42").         
+000031a0: 2020 2060 6060 0a0a 2020 2020 2020 2020     ```..        
+000031b0: 2320 4172 6775 6d65 6e74 730a 2020 2020  # Arguments.    
+000031c0: 2020 2020 2020 2020 6e61 6d65 3a20 4e61          name: Na
+000031d0: 6d65 206f 6620 7468 6520 7461 6720 746f  me of the tag to
+000031e0: 2062 6520 6164 6465 642e 0a20 2020 2020   be added..     
+000031f0: 2020 2020 2020 2076 616c 7565 3a20 5661         value: Va
+00003200: 6c75 6520 6f66 2074 6865 2074 6167 2074  lue of the tag t
+00003210: 6f20 6265 2061 6464 6564 2e0a 0a20 2020  o be added...   
+00003220: 2020 2020 2023 2052 6169 7365 730a 2020       # Raises.  
+00003230: 2020 2020 2020 2020 2020 6068 7366 732e            `hsfs.
+00003240: 636c 6965 6e74 2e65 7863 6570 7469 6f6e  client.exception
+00003250: 732e 5265 7374 4150 4945 7272 6f72 6020  s.RestAPIError` 
+00003260: 696e 2063 6173 6520 7468 6520 6261 636b  in case the back
+00003270: 656e 6420 6661 696c 7320 746f 2061 6464  end fails to add
+00003280: 2074 6865 2074 6167 2e0a 2020 2020 2020   the tag..      
+00003290: 2020 2222 220a 0a20 2020 2020 2020 2073    """..        s
+000032a0: 656c 662e 5f66 6561 7475 7265 5f67 726f  elf._feature_gro
+000032b0: 7570 5f65 6e67 696e 652e 6164 645f 7461  up_engine.add_ta
+000032c0: 6728 7365 6c66 2c20 6e61 6d65 2c20 7661  g(self, name, va
+000032d0: 6c75 6529 0a0a 2020 2020 6465 6620 6465  lue)..    def de
+000032e0: 6c65 7465 5f74 6167 2873 656c 662c 206e  lete_tag(self, n
+000032f0: 616d 653a 2073 7472 293a 0a20 2020 2020  ame: str):.     
+00003300: 2020 2022 2222 4465 6c65 7465 2061 2074     """Delete a t
+00003310: 6167 2061 7474 6163 6865 6420 746f 2061  ag attached to a
+00003320: 2066 6561 7475 7265 2067 726f 7570 2e0a   feature group..
+00003330: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
+00003340: 6d70 6c65 0a20 2020 2020 2020 2020 2020  mple.           
+00003350: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
+00003360: 2020 2020 2020 2023 2063 6f6e 6e65 6374         # connect
+00003370: 2074 6f20 7468 6520 4665 6174 7572 6520   to the Feature 
+00003380: 5374 6f72 650a 2020 2020 2020 2020 2020  Store.          
+00003390: 2020 6673 203d 202e 2e2e 0a0a 2020 2020    fs = .....    
+000033a0: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
+000033b0: 6520 4665 6174 7572 6520 4772 6f75 7020  e Feature Group 
+000033c0: 696e 7374 616e 6365 0a20 2020 2020 2020  instance.       
+000033d0: 2020 2020 2066 6720 3d20 6673 2e67 6574       fg = fs.get
+000033e0: 5f6f 725f 6372 6561 7465 5f66 6561 7475  _or_create_featu
+000033f0: 7265 5f67 726f 7570 282e 2e2e 290a 0a20  re_group(...).. 
+00003400: 2020 2020 2020 2020 2020 2066 672e 6465             fg.de
+00003410: 6c65 7465 5f74 6167 2822 6578 616d 706c  lete_tag("exampl
+00003420: 655f 7461 6722 290a 2020 2020 2020 2020  e_tag").        
+00003430: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
+00003440: 2023 2041 7267 756d 656e 7473 0a20 2020   # Arguments.   
+00003450: 2020 2020 2020 2020 206e 616d 653a 204e           name: N
+00003460: 616d 6520 6f66 2074 6865 2074 6167 2074  ame of the tag t
+00003470: 6f20 6265 2072 656d 6f76 6564 2e0a 0a20  o be removed... 
+00003480: 2020 2020 2020 2023 2052 6169 7365 730a         # Raises.
+00003490: 2020 2020 2020 2020 2020 2020 6068 7366              `hsf
+000034a0: 732e 636c 6965 6e74 2e65 7863 6570 7469  s.client.excepti
+000034b0: 6f6e 732e 5265 7374 4150 4945 7272 6f72  ons.RestAPIError
+000034c0: 6020 696e 2063 6173 6520 7468 6520 6261  ` in case the ba
+000034d0: 636b 656e 6420 6661 696c 7320 746f 2064  ckend fails to d
+000034e0: 656c 6574 6520 7468 6520 7461 672e 0a20  elete the tag.. 
+000034f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00003500: 2020 2073 656c 662e 5f66 6561 7475 7265     self._feature
+00003510: 5f67 726f 7570 5f65 6e67 696e 652e 6465  _group_engine.de
+00003520: 6c65 7465 5f74 6167 2873 656c 662c 206e  lete_tag(self, n
+00003530: 616d 6529 0a0a 2020 2020 6465 6620 6765  ame)..    def ge
+00003540: 745f 7461 6728 7365 6c66 2c20 6e61 6d65  t_tag(self, name
+00003550: 3a20 7374 7229 3a0a 2020 2020 2020 2020  : str):.        
+00003560: 2222 2247 6574 2074 6865 2074 6167 7320  """Get the tags 
+00003570: 6f66 2061 2066 6561 7475 7265 2067 726f  of a feature gro
+00003580: 7570 2e0a 0a20 2020 2020 2020 2021 2121  up...        !!!
+00003590: 2065 7861 6d70 6c65 0a20 2020 2020 2020   example.       
+000035a0: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
+000035b0: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
+000035c0: 6e65 6374 2074 6f20 7468 6520 4665 6174  nect to the Feat
+000035d0: 7572 6520 5374 6f72 650a 2020 2020 2020  ure Store.      
+000035e0: 2020 2020 2020 6673 203d 202e 2e2e 0a0a        fs = .....
+000035f0: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
+00003600: 7420 7468 6520 4665 6174 7572 6520 4772  t the Feature Gr
+00003610: 6f75 7020 696e 7374 616e 6365 0a20 2020  oup instance.   
+00003620: 2020 2020 2020 2020 2066 6720 3d20 6673           fg = fs
+00003630: 2e67 6574 5f6f 725f 6372 6561 7465 5f66  .get_or_create_f
+00003640: 6561 7475 7265 5f67 726f 7570 282e 2e2e  eature_group(...
+00003650: 290a 0a20 2020 2020 2020 2020 2020 2066  )..            f
+00003660: 675f 7461 675f 7661 6c75 6520 3d20 6667  g_tag_value = fg
+00003670: 2e67 6574 5f74 6167 2822 6578 616d 706c  .get_tag("exampl
+00003680: 655f 7461 6722 290a 2020 2020 2020 2020  e_tag").        
+00003690: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
+000036a0: 2023 2041 7267 756d 656e 7473 0a20 2020   # Arguments.   
+000036b0: 2020 2020 2020 2020 206e 616d 653a 204e           name: N
+000036c0: 616d 6520 6f66 2074 6865 2074 6167 2074  ame of the tag t
+000036d0: 6f20 6765 742e 0a0a 2020 2020 2020 2020  o get...        
+000036e0: 2320 5265 7475 726e 730a 2020 2020 2020  # Returns.      
+000036f0: 2020 2020 2020 7461 6720 7661 6c75 650a        tag value.
+00003700: 0a20 2020 2020 2020 2023 2052 6169 7365  .        # Raise
+00003710: 730a 2020 2020 2020 2020 2020 2020 6068  s.            `h
+00003720: 7366 732e 636c 6965 6e74 2e65 7863 6570  sfs.client.excep
+00003730: 7469 6f6e 732e 5265 7374 4150 4945 7272  tions.RestAPIErr
+00003740: 6f72 6020 696e 2063 6173 6520 7468 6520  or` in case the 
+00003750: 6261 636b 656e 6420 6661 696c 7320 746f  backend fails to
+00003760: 2072 6574 7269 6576 6520 7468 6520 7461   retrieve the ta
+00003770: 672e 0a20 2020 2020 2020 2022 2222 0a20  g..        """. 
+00003780: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00003790: 6c66 2e5f 6665 6174 7572 655f 6772 6f75  lf._feature_grou
+000037a0: 705f 656e 6769 6e65 2e67 6574 5f74 6167  p_engine.get_tag
+000037b0: 2873 656c 662c 206e 616d 6529 0a0a 2020  (self, name)..  
+000037c0: 2020 6465 6620 6765 745f 7461 6773 2873    def get_tags(s
+000037d0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+000037e0: 2252 6574 7269 6576 6573 2061 6c6c 2074  "Retrieves all t
+000037f0: 6167 7320 6174 7461 6368 6564 2074 6f20  ags attached to 
+00003800: 6120 6665 6174 7572 6520 6772 6f75 702e  a feature group.
+00003810: 0a0a 2020 2020 2020 2020 2320 5265 7475  ..        # Retu
+00003820: 726e 730a 2020 2020 2020 2020 2020 2020  rns.            
+00003830: 6044 6963 745b 7374 722c 206f 626a 5d60  `Dict[str, obj]`
+00003840: 206f 6620 7461 6773 2e0a 0a20 2020 2020   of tags...     
+00003850: 2020 2023 2052 6169 7365 730a 2020 2020     # Raises.    
+00003860: 2020 2020 2020 2020 6068 7366 732e 636c          `hsfs.cl
+00003870: 6965 6e74 2e65 7863 6570 7469 6f6e 732e  ient.exceptions.
+00003880: 5265 7374 4150 4945 7272 6f72 6020 696e  RestAPIError` in
+00003890: 2063 6173 6520 7468 6520 6261 636b 656e   case the backen
+000038a0: 6420 6661 696c 7320 746f 2072 6574 7269  d fails to retri
+000038b0: 6576 6520 7468 6520 7461 6773 2e0a 2020  eve the tags..  
+000038c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000038d0: 2020 7265 7475 726e 2073 656c 662e 5f66    return self._f
+000038e0: 6561 7475 7265 5f67 726f 7570 5f65 6e67  eature_group_eng
+000038f0: 696e 652e 6765 745f 7461 6773 2873 656c  ine.get_tags(sel
+00003900: 6629 0a0a 2020 2020 6465 6620 6765 745f  f)..    def get_
+00003910: 7061 7265 6e74 5f66 6561 7475 7265 5f67  parent_feature_g
+00003920: 726f 7570 7328 7365 6c66 293a 0a20 2020  roups(self):.   
+00003930: 2020 2020 2022 2222 4765 7420 7468 6520       """Get the 
+00003940: 7061 7265 6e74 7320 6f66 2074 6869 7320  parents of this 
+00003950: 6665 6174 7572 6520 6772 6f75 702c 2062  feature group, b
+00003960: 6173 6564 206f 6e20 6578 706c 6963 6974  ased on explicit
+00003970: 2070 726f 7665 6e61 6e63 652e 0a20 2020   provenance..   
+00003980: 2020 2020 2050 6172 656e 7473 2061 7265       Parents are
+00003990: 2066 6561 7475 7265 2067 726f 7570 7320   feature groups 
+000039a0: 6f72 2065 7874 6572 6e61 6c20 6665 6174  or external feat
+000039b0: 7572 6520 6772 6f75 7073 2e20 5468 6573  ure groups. Thes
+000039c0: 6520 6665 6174 7572 650a 2020 2020 2020  e feature.      
+000039d0: 2020 6772 6f75 7073 2063 616e 2062 6520    groups can be 
+000039e0: 6163 6365 7373 6962 6c65 2c20 6465 6c65  accessible, dele
+000039f0: 7465 6420 6f72 2069 6e61 6363 6573 7369  ted or inaccessi
+00003a00: 626c 652e 0a20 2020 2020 2020 2046 6f72  ble..        For
+00003a10: 2064 656c 6574 6564 2061 6e64 2069 6e61   deleted and ina
+00003a20: 6363 6573 7369 626c 6520 6665 6174 7572  ccessible featur
+00003a30: 6520 6772 6f75 7073 2c20 6f6e 6c79 2061  e groups, only a
+00003a40: 206d 696e 696d 616c 2069 6e66 6f72 6d61   minimal informa
+00003a50: 7469 6f6e 2069 730a 2020 2020 2020 2020  tion is.        
+00003a60: 7265 7475 726e 6564 2e0a 0a20 2020 2020  returned...     
+00003a70: 2020 2023 2052 6574 7572 6e73 0a20 2020     # Returns.   
+00003a80: 2020 2020 2020 2020 2060 5072 6f76 656e           `Proven
+00003a90: 616e 6365 4c69 6e6b 7360 3a20 4f62 6a65  anceLinks`: Obje
+00003aa0: 6374 2063 6f6e 7461 696e 696e 6720 7468  ct containing th
+00003ab0: 6520 7365 6374 696f 6e20 6f66 2070 726f  e section of pro
+00003ac0: 7665 6e61 6e63 6520 6772 6170 6820 7265  venance graph re
+00003ad0: 7175 6573 7465 642e 0a0a 2020 2020 2020  quested...      
+00003ae0: 2020 2320 5261 6973 6573 0a20 2020 2020    # Raises.     
+00003af0: 2020 2020 2020 2060 6873 6673 2e63 6c69         `hsfs.cli
+00003b00: 656e 742e 6578 6365 7074 696f 6e73 2e52  ent.exceptions.R
+00003b10: 6573 7441 5049 4572 726f 7260 2e0a 2020  estAPIError`..  
+00003b20: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00003b30: 2020 7265 7475 726e 2073 656c 662e 5f66    return self._f
+00003b40: 6561 7475 7265 5f67 726f 7570 5f65 6e67  eature_group_eng
+00003b50: 696e 652e 6765 745f 7061 7265 6e74 5f66  ine.get_parent_f
+00003b60: 6561 7475 7265 5f67 726f 7570 7328 7365  eature_groups(se
+00003b70: 6c66 290a 0a20 2020 2064 6566 2067 6574  lf)..    def get
+00003b80: 5f67 656e 6572 6174 6564 5f66 6561 7475  _generated_featu
+00003b90: 7265 5f76 6965 7773 2873 656c 6629 3a0a  re_views(self):.
+00003ba0: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
+00003bb0: 6865 2067 656e 6572 6174 6564 2066 6561  he generated fea
+00003bc0: 7475 7265 2076 6965 7720 7573 696e 6720  ture view using 
+00003bd0: 7468 6973 2066 6561 7475 7265 2067 726f  this feature gro
+00003be0: 7570 2c20 6261 7365 6420 6f6e 2065 7870  up, based on exp
+00003bf0: 6c69 6369 740a 2020 2020 2020 2020 7072  licit.        pr
+00003c00: 6f76 656e 616e 6365 2e20 5468 6573 6520  ovenance. These 
+00003c10: 6665 6174 7572 6520 7669 6577 7320 6361  feature views ca
+00003c20: 6e20 6265 2061 6363 6573 7369 626c 6520  n be accessible 
+00003c30: 6f72 2069 6e61 6363 6573 7369 626c 652e  or inaccessible.
+00003c40: 2045 7870 6c69 6369 740a 2020 2020 2020   Explicit.      
+00003c50: 2020 7072 6f76 656e 616e 6365 2064 6f65    provenance doe
+00003c60: 7320 6e6f 7420 7472 6163 6b20 6465 6c65  s not track dele
+00003c70: 7465 6420 6765 6e65 7261 7465 6420 6665  ted generated fe
+00003c80: 6174 7572 6520 7669 6577 206c 696e 6b73  ature view links
+00003c90: 2c20 736f 2064 656c 6574 6564 0a20 2020  , so deleted.   
+00003ca0: 2020 2020 2077 696c 6c20 616c 7761 7973       will always
+00003cb0: 2062 6520 656d 7074 792e 0a20 2020 2020   be empty..     
+00003cc0: 2020 2046 6f72 2069 6e61 6363 6573 7369     For inaccessi
+00003cd0: 626c 6520 6665 6174 7572 6520 7669 6577  ble feature view
+00003ce0: 732c 206f 6e6c 7920 6120 6d69 6e69 6d61  s, only a minima
+00003cf0: 6c20 696e 666f 726d 6174 696f 6e20 6973  l information is
+00003d00: 2072 6574 7572 6e65 642e 0a0a 2020 2020   returned...    
+00003d10: 2020 2020 2320 5265 7475 726e 730a 2020      # Returns.  
+00003d20: 2020 2020 2020 2020 2020 6050 726f 7665            `Prove
+00003d30: 6e61 6e63 654c 696e 6b73 603a 204f 626a  nanceLinks`: Obj
+00003d40: 6563 7420 636f 6e74 6169 6e69 6e67 2074  ect containing t
+00003d50: 6865 2073 6563 7469 6f6e 206f 6620 7072  he section of pr
+00003d60: 6f76 656e 616e 6365 2067 7261 7068 2072  ovenance graph r
+00003d70: 6571 7565 7374 6564 2e0a 0a20 2020 2020  equested...     
+00003d80: 2020 2023 2052 6169 7365 730a 2020 2020     # Raises.    
+00003d90: 2020 2020 2020 2020 6068 7366 732e 636c          `hsfs.cl
+00003da0: 6965 6e74 2e65 7863 6570 7469 6f6e 732e  ient.exceptions.
+00003db0: 5265 7374 4150 4945 7272 6f72 602e 0a20  RestAPIError`.. 
+00003dc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00003dd0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00003de0: 6665 6174 7572 655f 6772 6f75 705f 656e  feature_group_en
+00003df0: 6769 6e65 2e67 6574 5f67 656e 6572 6174  gine.get_generat
+00003e00: 6564 5f66 6561 7475 7265 5f76 6965 7773  ed_feature_views
+00003e10: 2873 656c 6629 0a0a 2020 2020 6465 6620  (self)..    def 
+00003e20: 6765 745f 6765 6e65 7261 7465 645f 6665  get_generated_fe
+00003e30: 6174 7572 655f 6772 6f75 7073 2873 656c  ature_groups(sel
+00003e40: 6629 3a0a 2020 2020 2020 2020 2222 2247  f):.        """G
+00003e50: 6574 2074 6865 2067 656e 6572 6174 6564  et the generated
+00003e60: 2066 6561 7475 7265 2067 726f 7570 7320   feature groups 
+00003e70: 7573 696e 6720 7468 6973 2066 6561 7475  using this featu
+00003e80: 7265 2067 726f 7570 2c20 6261 7365 6420  re group, based 
+00003e90: 6f6e 2065 7870 6c69 6369 740a 2020 2020  on explicit.    
+00003ea0: 2020 2020 7072 6f76 656e 616e 6365 2e20      provenance. 
+00003eb0: 5468 6573 6520 6665 6174 7572 6520 6772  These feature gr
+00003ec0: 6f75 7073 2063 616e 2062 6520 6163 6365  oups can be acce
+00003ed0: 7373 6962 6c65 206f 7220 696e 6163 6365  ssible or inacce
+00003ee0: 7373 6962 6c65 2e20 4578 706c 6963 6974  ssible. Explicit
+00003ef0: 0a20 2020 2020 2020 2070 726f 7665 6e61  .        provena
+00003f00: 6e63 6520 646f 6573 206e 6f74 2074 7261  nce does not tra
+00003f10: 636b 2064 656c 6574 6564 2067 656e 6572  ck deleted gener
+00003f20: 6174 6564 2066 6561 7475 7265 2067 726f  ated feature gro
+00003f30: 7570 206c 696e 6b73 2c20 736f 2064 656c  up links, so del
+00003f40: 6574 6564 0a20 2020 2020 2020 2077 696c  eted.        wil
+00003f50: 6c20 616c 7761 7973 2062 6520 656d 7074  l always be empt
+00003f60: 792e 0a20 2020 2020 2020 2046 6f72 2069  y..        For i
+00003f70: 6e61 6363 6573 7369 626c 6520 6665 6174  naccessible feat
+00003f80: 7572 6520 6772 6f75 7073 2c20 6f6e 6c79  ure groups, only
+00003f90: 2061 206d 696e 696d 616c 2069 6e66 6f72   a minimal infor
+00003fa0: 6d61 7469 6f6e 2069 7320 7265 7475 726e  mation is return
+00003fb0: 6564 2e0a 0a20 2020 2020 2020 2023 2052  ed...        # R
+00003fc0: 6574 7572 6e73 0a20 2020 2020 2020 2020  eturns.         
+00003fd0: 2020 2060 5072 6f76 656e 616e 6365 4c69     `ProvenanceLi
+00003fe0: 6e6b 7360 3a20 4f62 6a65 6374 2063 6f6e  nks`: Object con
+00003ff0: 7461 696e 696e 6720 7468 6520 7365 6374  taining the sect
+00004000: 696f 6e20 6f66 2070 726f 7665 6e61 6e63  ion of provenanc
+00004010: 6520 6772 6170 6820 7265 7175 6573 7465  e graph requeste
+00004020: 642e 0a0a 2020 2020 2020 2020 2320 5261  d...        # Ra
+00004030: 6973 6573 0a20 2020 2020 2020 2020 2020  ises.           
+00004040: 2060 6873 6673 2e63 6c69 656e 742e 6578   `hsfs.client.ex
+00004050: 6365 7074 696f 6e73 2e52 6573 7441 5049  ceptions.RestAPI
+00004060: 4572 726f 7260 2e0a 2020 2020 2020 2020  Error`..        
+00004070: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00004080: 726e 2073 656c 662e 5f66 6561 7475 7265  rn self._feature
+00004090: 5f67 726f 7570 5f65 6e67 696e 652e 6765  _group_engine.ge
+000040a0: 745f 6765 6e65 7261 7465 645f 6665 6174  t_generated_feat
+000040b0: 7572 655f 6772 6f75 7073 2873 656c 6629  ure_groups(self)
+000040c0: 0a0a 2020 2020 6465 6620 6765 745f 6665  ..    def get_fe
+000040d0: 6174 7572 6528 7365 6c66 2c20 6e61 6d65  ature(self, name
+000040e0: 3a20 7374 7229 3a0a 2020 2020 2020 2020  : str):.        
+000040f0: 2222 2252 6574 7269 6576 6520 6120 6046  """Retrieve a `F
+00004100: 6561 7475 7265 6020 6f62 6a65 6374 2066  eature` object f
+00004110: 726f 6d20 7468 6520 7363 6865 6d61 206f  rom the schema o
+00004120: 6620 7468 6520 6665 6174 7572 6520 6772  f the feature gr
+00004130: 6f75 702e 0a0a 2020 2020 2020 2020 5468  oup...        Th
+00004140: 6572 6520 6172 6520 7365 7665 7261 6c20  ere are several 
+00004150: 7761 7973 2074 6f20 6163 6365 7373 2066  ways to access f
+00004160: 6561 7475 7265 7320 6f66 2061 2066 6561  eatures of a fea
+00004170: 7475 7265 2067 726f 7570 3a0a 0a20 2020  ture group:..   
+00004180: 2020 2020 2021 2121 2065 7861 6d70 6c65       !!! example
+00004190: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
+000041a0: 7079 7468 6f6e 0a20 2020 2020 2020 2020  python.         
+000041b0: 2020 2023 2063 6f6e 6e65 6374 2074 6f20     # connect to 
+000041c0: 7468 6520 4665 6174 7572 6520 5374 6f72  the Feature Stor
+000041d0: 650a 2020 2020 2020 2020 2020 2020 6673  e.            fs
+000041e0: 203d 202e 2e2e 0a0a 2020 2020 2020 2020   = .....        
+000041f0: 2020 2020 2320 6765 7420 7468 6520 4665      # get the Fe
+00004200: 6174 7572 6520 4772 6f75 7020 696e 7374  ature Group inst
+00004210: 616e 6365 0a20 2020 2020 2020 2020 2020  ance.           
+00004220: 2066 6720 3d20 6673 2e67 6574 5f6f 725f   fg = fs.get_or_
+00004230: 6372 6561 7465 5f66 6561 7475 7265 5f67  create_feature_g
+00004240: 726f 7570 282e 2e2e 290a 0a20 2020 2020  roup(...)..     
+00004250: 2020 2020 2020 2023 2067 6574 2046 6561         # get Fea
+00004260: 7475 7265 2069 6e73 7461 6e73 650a 2020  ture instanse.  
+00004270: 2020 2020 2020 2020 2020 6667 2e66 6561            fg.fea
+00004280: 7475 7265 310a 2020 2020 2020 2020 2020  ture1.          
+00004290: 2020 6667 5b22 6665 6174 7572 6531 225d    fg["feature1"]
+000042a0: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
+000042b0: 6765 745f 6665 6174 7572 6528 2266 6561  get_feature("fea
+000042c0: 7475 7265 3122 290a 2020 2020 2020 2020  ture1").        
+000042d0: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
+000042e0: 2021 2121 206e 6f74 650a 2020 2020 2020   !!! note.      
+000042f0: 2020 2020 2020 4174 7472 6962 7574 6520        Attribute 
+00004300: 6163 6365 7373 2074 6f20 6665 6174 7572  access to featur
+00004310: 6573 2077 6f72 6b73 206f 6e6c 7920 666f  es works only fo
+00004320: 7220 6e6f 6e2d 7265 7365 7276 6564 206e  r non-reserved n
+00004330: 616d 6573 2e20 466f 7220 6578 616d 706c  ames. For exampl
+00004340: 650a 2020 2020 2020 2020 2020 2020 6665  e.            fe
+00004350: 6174 7572 6573 206e 616d 6564 2060 6964  atures named `id
+00004360: 6020 6f72 2060 6e61 6d65 6020 7769 6c6c  ` or `name` will
+00004370: 206e 6f74 2062 6520 6163 6365 7373 6962   not be accessib
+00004380: 6c65 2076 6961 2060 6667 2e6e 616d 6560  le via `fg.name`
+00004390: 2c20 696e 7374 6561 640a 2020 2020 2020  , instead.      
+000043a0: 2020 2020 2020 7468 6973 2077 696c 6c20        this will 
+000043b0: 7265 7475 726e 2074 6865 206e 616d 6520  return the name 
+000043c0: 6f66 2074 6865 2066 6561 7475 7265 2067  of the feature g
+000043d0: 726f 7570 2069 7473 656c 662e 2046 616c  roup itself. Fal
+000043e0: 6c20 6261 636b 206f 6e20 7573 696e 670a  l back on using.
+000043f0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00004400: 6067 6574 5f66 6561 7475 7265 6020 6d65  `get_feature` me
+00004410: 7468 6f64 2e0a 0a20 2020 2020 2020 2023  thod...        #
+00004420: 2041 7267 756d 656e 7473 3a0a 2020 2020   Arguments:.    
+00004430: 2020 2020 2020 2020 6e61 6d65 3a20 5468          name: Th
+00004440: 6520 6e61 6d65 206f 6620 7468 6520 6665  e name of the fe
+00004450: 6174 7572 6520 746f 2072 6574 7269 6576  ature to retriev
+00004460: 650a 0a20 2020 2020 2020 2023 2052 6574  e..        # Ret
+00004470: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00004480: 2020 4665 6174 7572 653a 2054 6865 2066    Feature: The f
+00004490: 6561 7475 7265 206f 626a 6563 740a 0a20  eature object.. 
+000044a0: 2020 2020 2020 2023 2052 6169 7365 730a         # Raises.
+000044b0: 2020 2020 2020 2020 2020 2020 6068 7366              `hsf
+000044c0: 732e 636c 6965 6e74 2e65 7863 6570 7469  s.client.excepti
+000044d0: 6f6e 732e 4665 6174 7572 6553 746f 7265  ons.FeatureStore
+000044e0: 4578 6365 7074 696f 6e60 2e0a 2020 2020  Exception`..    
+000044f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00004500: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00004510: 2072 6574 7572 6e20 7365 6c66 2e5f 5f67   return self.__g
+00004520: 6574 6974 656d 5f5f 286e 616d 6529 0a20  etitem__(name). 
+00004530: 2020 2020 2020 2065 7863 6570 7420 4b65         except Ke
+00004540: 7945 7272 6f72 3a0a 2020 2020 2020 2020  yError:.        
+00004550: 2020 2020 7261 6973 6520 4665 6174 7572      raise Featur
+00004560: 6553 746f 7265 4578 6365 7074 696f 6e28  eStoreException(
+00004570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004580: 2066 2227 4665 6174 7572 6547 726f 7570   f"'FeatureGroup
+00004590: 2720 6f62 6a65 6374 2068 6173 206e 6f20  ' object has no 
+000045a0: 6665 6174 7572 6520 6361 6c6c 6564 2027  feature called '
+000045b0: 7b6e 616d 657d 272e 220a 2020 2020 2020  {name}'.".      
+000045c0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+000045d0: 2075 7064 6174 655f 7374 6174 6973 7469   update_statisti
+000045e0: 6373 5f63 6f6e 6669 6728 7365 6c66 293a  cs_config(self):
+000045f0: 0a20 2020 2020 2020 2022 2222 5570 6461  .        """Upda
+00004600: 7465 2074 6865 2073 7461 7469 7374 6963  te the statistic
+00004610: 7320 636f 6e66 6967 7572 6174 696f 6e20  s configuration 
+00004620: 6f66 2074 6865 2066 6561 7475 7265 2067  of the feature g
+00004630: 726f 7570 2e0a 0a20 2020 2020 2020 2043  roup...        C
+00004640: 6861 6e67 6520 7468 6520 6073 7461 7469  hange the `stati
+00004650: 7374 6963 735f 636f 6e66 6967 6020 6f62  stics_config` ob
+00004660: 6a65 6374 2061 6e64 2070 6572 7369 7374  ject and persist
+00004670: 2074 6865 2063 6861 6e67 6573 2062 7920   the changes by 
+00004680: 6361 6c6c 696e 670a 2020 2020 2020 2020  calling.        
+00004690: 7468 6973 206d 6574 686f 642e 0a0a 2020  this method...  
+000046a0: 2020 2020 2020 2121 2120 6578 616d 706c        !!! exampl
+000046b0: 650a 2020 2020 2020 2020 2020 2020 6060  e.            ``
+000046c0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+000046d0: 2020 2020 2320 636f 6e6e 6563 7420 746f      # connect to
+000046e0: 2074 6865 2046 6561 7475 7265 2053 746f   the Feature Sto
+000046f0: 7265 0a20 2020 2020 2020 2020 2020 2066  re.            f
+00004700: 7320 3d20 2e2e 2e0a 0a20 2020 2020 2020  s = .....       
+00004710: 2020 2020 2023 2067 6574 2074 6865 2046       # get the F
+00004720: 6561 7475 7265 2047 726f 7570 2069 6e73  eature Group ins
+00004730: 7461 6e63 650a 2020 2020 2020 2020 2020  tance.          
+00004740: 2020 6667 203d 2066 732e 6765 745f 6f72    fg = fs.get_or
+00004750: 5f63 7265 6174 655f 6665 6174 7572 655f  _create_feature_
+00004760: 6772 6f75 7028 2e2e 2e29 0a0a 2020 2020  group(...)..    
+00004770: 2020 2020 2020 2020 6667 2e75 7064 6174          fg.updat
+00004780: 655f 7374 6174 6973 7469 6373 5f63 6f6e  e_statistics_con
+00004790: 6669 6728 290a 2020 2020 2020 2020 2020  fig().          
+000047a0: 2020 6060 600a 0a20 2020 2020 2020 2023    ```..        #
+000047b0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+000047c0: 2020 2020 2060 4665 6174 7572 6547 726f       `FeatureGro
+000047d0: 7570 602e 2054 6865 2075 7064 6174 6564  up`. The updated
+000047e0: 206d 6574 6164 6174 6120 6f62 6a65 6374   metadata object
+000047f0: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
+00004800: 6772 6f75 702e 0a0a 2020 2020 2020 2020  group...        
+00004810: 2320 5261 6973 6573 0a20 2020 2020 2020  # Raises.       
+00004820: 2020 2020 2060 6873 6673 2e63 6c69 656e       `hsfs.clien
+00004830: 742e 6578 6365 7074 696f 6e73 2e52 6573  t.exceptions.Res
+00004840: 7441 5049 4572 726f 7260 2e0a 2020 2020  tAPIError`..    
+00004850: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00004860: 7365 6c66 2e5f 6665 6174 7572 655f 6772  self._feature_gr
+00004870: 6f75 705f 656e 6769 6e65 2e75 7064 6174  oup_engine.updat
+00004880: 655f 7374 6174 6973 7469 6373 5f63 6f6e  e_statistics_con
+00004890: 6669 6728 7365 6c66 290a 2020 2020 2020  fig(self).      
+000048a0: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
+000048b0: 2020 2064 6566 2075 7064 6174 655f 6465     def update_de
+000048c0: 7363 7269 7074 696f 6e28 7365 6c66 2c20  scription(self, 
+000048d0: 6465 7363 7269 7074 696f 6e3a 2073 7472  description: str
+000048e0: 293a 0a20 2020 2020 2020 2022 2222 5570  ):.        """Up
+000048f0: 6461 7465 2074 6865 2064 6573 6372 6970  date the descrip
+00004900: 7469 6f6e 206f 6620 7468 6520 6665 6174  tion of the feat
+00004910: 7572 6520 6772 6f75 702e 0a0a 2020 2020  ure group...    
+00004920: 2020 2020 2121 2120 6578 616d 706c 650a      !!! example.
+00004930: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
+00004940: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
+00004950: 2020 2320 636f 6e6e 6563 7420 746f 2074    # connect to t
+00004960: 6865 2046 6561 7475 7265 2053 746f 7265  he Feature Store
+00004970: 0a20 2020 2020 2020 2020 2020 2066 7320  .            fs 
+00004980: 3d20 2e2e 2e0a 0a20 2020 2020 2020 2020  = .....         
+00004990: 2020 2023 2067 6574 2074 6865 2046 6561     # get the Fea
+000049a0: 7475 7265 2047 726f 7570 2069 6e73 7461  ture Group insta
+000049b0: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
+000049c0: 6667 203d 2066 732e 6765 745f 6f72 5f63  fg = fs.get_or_c
+000049d0: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
+000049e0: 6f75 7028 2e2e 2e29 0a0a 2020 2020 2020  oup(...)..      
+000049f0: 2020 2020 2020 6667 2e75 7064 6174 655f        fg.update_
+00004a00: 6465 7363 7269 7074 696f 6e28 6465 7363  description(desc
+00004a10: 7269 7074 696f 6e3d 224d 7563 6820 6265  ription="Much be
+00004a20: 7474 6572 2064 6573 6372 6970 7469 6f6e  tter description
+00004a30: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+00004a40: 6060 600a 0a20 2020 2020 2020 2021 2121  ```..        !!!
+00004a50: 2069 6e66 6f20 2253 6166 6520 7570 6461   info "Safe upda
+00004a60: 7465 220a 2020 2020 2020 2020 2020 2020  te".            
+00004a70: 5468 6973 206d 6574 686f 6420 7570 6461  This method upda
+00004a80: 7465 7320 7468 6520 6665 6174 7572 6520  tes the feature 
+00004a90: 6772 6f75 7020 6465 7363 7269 7074 696f  group descriptio
+00004aa0: 6e20 7361 6665 6c79 2e20 496e 2063 6173  n safely. In cas
+00004ab0: 6520 6f66 2066 6169 6c75 7265 0a20 2020  e of failure.   
+00004ac0: 2020 2020 2020 2020 2079 6f75 7220 6c6f           your lo
+00004ad0: 6361 6c20 6d65 7461 6461 7461 206f 626a  cal metadata obj
+00004ae0: 6563 7420 7769 6c6c 206b 6565 7020 7468  ect will keep th
+00004af0: 6520 6f6c 6420 6465 7363 7269 7074 696f  e old descriptio
+00004b00: 6e2e 0a0a 2020 2020 2020 2020 2320 4172  n...        # Ar
+00004b10: 6775 6d65 6e74 730a 2020 2020 2020 2020  guments.        
+00004b20: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00004b30: 204e 6577 2064 6573 6372 6970 7469 6f6e   New description
+00004b40: 2073 7472 696e 672e 0a0a 2020 2020 2020   string...      
+00004b50: 2020 2320 5265 7475 726e 730a 2020 2020    # Returns.    
+00004b60: 2020 2020 2020 2020 6046 6561 7475 7265          `Feature
+00004b70: 4772 6f75 7060 2e20 5468 6520 7570 6461  Group`. The upda
+00004b80: 7465 6420 6665 6174 7572 6520 6772 6f75  ted feature grou
+00004b90: 7020 6f62 6a65 6374 2e0a 2020 2020 2020  p object..      
+00004ba0: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
+00004bb0: 6c66 2e5f 6665 6174 7572 655f 6772 6f75  lf._feature_grou
+00004bc0: 705f 656e 6769 6e65 2e75 7064 6174 655f  p_engine.update_
+00004bd0: 6465 7363 7269 7074 696f 6e28 7365 6c66  description(self
+00004be0: 2c20 6465 7363 7269 7074 696f 6e29 0a20  , description). 
+00004bf0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00004c00: 6c66 0a0a 2020 2020 6465 6620 7570 6461  lf..    def upda
+00004c10: 7465 5f66 6561 7475 7265 7328 7365 6c66  te_features(self
+00004c20: 2c20 6665 6174 7572 6573 3a20 556e 696f  , features: Unio
+00004c30: 6e5b 6665 6174 7572 652e 4665 6174 7572  n[feature.Featur
+00004c40: 652c 204c 6973 745b 6665 6174 7572 652e  e, List[feature.
+00004c50: 4665 6174 7572 655d 5d29 3a0a 2020 2020  Feature]]):.    
+00004c60: 2020 2020 2222 2255 7064 6174 6520 6d65      """Update me
+00004c70: 7461 6461 7461 206f 6620 6665 6174 7572  tadata of featur
+00004c80: 6573 2069 6e20 7468 6973 2066 6561 7475  es in this featu
+00004c90: 7265 2067 726f 7570 2e0a 0a20 2020 2020  re group...     
+00004ca0: 2020 2043 7572 7265 6e74 6c79 2069 7427     Currently it'
+00004cb0: 7320 6f6e 6c79 2073 7570 706f 7274 6564  s only supported
+00004cc0: 2074 6f20 7570 6461 7465 2074 6865 2064   to update the d
+00004cd0: 6573 6372 6970 7469 6f6e 206f 6620 6120  escription of a 
+00004ce0: 6665 6174 7572 652e 0a0a 2020 2020 2020  feature...      
+00004cf0: 2020 2121 2120 6461 6e67 6572 2022 556e    !!! danger "Un
+00004d00: 7361 6665 2075 7064 6174 6522 0a20 2020  safe update".   
+00004d10: 2020 2020 2020 2020 204e 6f74 6520 7468           Note th
+00004d20: 6174 2069 6620 796f 7520 7573 6520 616e  at if you use an
+00004d30: 2065 7869 7374 696e 6720 6046 6561 7475   existing `Featu
+00004d40: 7265 6020 6f62 6a65 6374 206f 6620 7468  re` object of th
+00004d50: 6520 7363 6865 6d61 2069 6e20 7468 650a  e schema in the.
+00004d60: 2020 2020 2020 2020 2020 2020 6665 6174              feat
+00004d70: 7572 6520 6772 6f75 7020 6d65 7461 6461  ure group metada
+00004d80: 7461 206f 626a 6563 742c 2074 6869 7320  ta object, this 
+00004d90: 6d69 6768 7420 6c65 6176 6520 796f 7572  might leave your
+00004da0: 206d 6574 6164 6174 6120 6f62 6a65 6374   metadata object
+00004db0: 2069 6e20 610a 2020 2020 2020 2020 2020   in a.          
+00004dc0: 2020 636f 7272 7570 7465 6420 7374 6174    corrupted stat
+00004dd0: 6520 6966 2074 6865 2075 7064 6174 6520  e if the update 
+00004de0: 6661 696c 732e 0a0a 2020 2020 2020 2020  fails...        
+00004df0: 2320 4172 6775 6d65 6e74 730a 2020 2020  # Arguments.    
+00004e00: 2020 2020 2020 2020 6665 6174 7572 6573          features
+00004e10: 3a20 6046 6561 7475 7265 6020 6f72 206c  : `Feature` or l
+00004e20: 6973 7420 6f66 2066 6561 7475 7265 732e  ist of features.
+00004e30: 2041 2066 6561 7475 7265 206f 626a 6563   A feature objec
+00004e40: 7420 6f72 206c 6973 7420 7468 6572 656f  t or list thereo
+00004e50: 6620 746f 0a20 2020 2020 2020 2020 2020  f to.           
+00004e60: 2020 2020 2062 6520 7570 6461 7465 642e       be updated.
+00004e70: 0a0a 2020 2020 2020 2020 2320 5265 7475  ..        # Retu
+00004e80: 726e 730a 2020 2020 2020 2020 2020 2020  rns.            
+00004e90: 6046 6561 7475 7265 4772 6f75 7060 2e20  `FeatureGroup`. 
+00004ea0: 5468 6520 7570 6461 7465 6420 6665 6174  The updated feat
+00004eb0: 7572 6520 6772 6f75 7020 6f62 6a65 6374  ure group object
+00004ec0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00004ed0: 2020 2020 2020 6e65 775f 6665 6174 7572        new_featur
+00004ee0: 6573 203d 205b 5d0a 2020 2020 2020 2020  es = [].        
+00004ef0: 6966 2069 7369 6e73 7461 6e63 6528 6665  if isinstance(fe
+00004f00: 6174 7572 6573 2c20 6665 6174 7572 652e  atures, feature.
+00004f10: 4665 6174 7572 6529 3a0a 2020 2020 2020  Feature):.      
+00004f20: 2020 2020 2020 6e65 775f 6665 6174 7572        new_featur
+00004f30: 6573 2e61 7070 656e 6428 6665 6174 7572  es.append(featur
+00004f40: 6573 290a 2020 2020 2020 2020 656c 6966  es).        elif
+00004f50: 2069 7369 6e73 7461 6e63 6528 6665 6174   isinstance(feat
+00004f60: 7572 6573 2c20 6c69 7374 293a 0a20 2020  ures, list):.   
+00004f70: 2020 2020 2020 2020 2066 6f72 2066 6561           for fea
+00004f80: 7420 696e 2066 6561 7475 7265 733a 0a20  t in features:. 
+00004f90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00004fa0: 6620 6973 696e 7374 616e 6365 2866 6561  f isinstance(fea
+00004fb0: 742c 2066 6561 7475 7265 2e46 6561 7475  t, feature.Featu
+00004fc0: 7265 293a 0a20 2020 2020 2020 2020 2020  re):.           
+00004fd0: 2020 2020 2020 2020 206e 6577 5f66 6561           new_fea
+00004fe0: 7475 7265 732e 6170 7065 6e64 2866 6561  tures.append(fea
+00004ff0: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+00005000: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00005010: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00005020: 7365 2054 7970 6545 7272 6f72 280a 2020  se TypeError(.  
+00005030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005040: 2020 2020 2020 2254 6865 2061 7267 756d        "The argum
+00005050: 656e 7420 6066 6561 7475 7265 7360 2068  ent `features` h
+00005060: 6173 2074 6f20 6265 206f 6620 7479 7065  as to be of type
+00005070: 2060 4665 6174 7572 6560 206f 7220 220a   `Feature` or ".
+00005080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005090: 2020 2020 2020 2020 2261 206c 6973 7420          "a list 
+000050a0: 7468 6572 656f 662c 2062 7574 2061 6e20  thereof, but an 
+000050b0: 656c 656d 656e 7420 6973 206f 6620 7479  element is of ty
+000050c0: 7065 3a20 607b 7d60 222e 666f 726d 6174  pe: `{}`".format
+000050d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000050e0: 2020 2020 2020 2020 2020 2020 2020 7479                ty
+000050f0: 7065 2866 6561 7475 7265 7329 0a20 2020  pe(features).   
+00005100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005110: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00005120: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00005130: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00005140: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+00005150: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+00005160: 2020 2020 2020 2020 2254 6865 2061 7267          "The arg
+00005170: 756d 656e 7420 6066 6561 7475 7265 7360  ument `features`
+00005180: 2068 6173 2074 6f20 6265 206f 6620 7479   has to be of ty
+00005190: 7065 2060 4665 6174 7572 6560 206f 7220  pe `Feature` or 
+000051a0: 6120 6c69 7374 2022 0a20 2020 2020 2020  a list ".       
+000051b0: 2020 2020 2020 2020 2022 7468 6572 656f           "thereo
+000051c0: 662c 2062 7574 2069 7320 6f66 2074 7970  f, but is of typ
+000051d0: 653a 2060 7b7d 6022 2e66 6f72 6d61 7428  e: `{}`".format(
+000051e0: 7479 7065 2866 6561 7475 7265 7329 290a  type(features)).
+000051f0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00005200: 2020 2020 2020 7365 6c66 2e5f 6665 6174        self._feat
+00005210: 7572 655f 6772 6f75 705f 656e 6769 6e65  ure_group_engine
+00005220: 2e75 7064 6174 655f 6665 6174 7572 6573  .update_features
+00005230: 2873 656c 662c 206e 6577 5f66 6561 7475  (self, new_featu
+00005240: 7265 7329 0a20 2020 2020 2020 2072 6574  res).        ret
+00005250: 7572 6e20 7365 6c66 0a0a 2020 2020 6465  urn self..    de
+00005260: 6620 7570 6461 7465 5f66 6561 7475 7265  f update_feature
+00005270: 5f64 6573 6372 6970 7469 6f6e 2873 656c  _description(sel
+00005280: 662c 2066 6561 7475 7265 5f6e 616d 653a  f, feature_name:
+00005290: 2073 7472 2c20 6465 7363 7269 7074 696f   str, descriptio
+000052a0: 6e3a 2073 7472 293a 0a20 2020 2020 2020  n: str):.       
+000052b0: 2022 2222 5570 6461 7465 2074 6865 2064   """Update the d
+000052c0: 6573 6372 6970 7469 6f6e 206f 6620 6120  escription of a 
+000052d0: 7369 6e67 6c65 2066 6561 7475 7265 2069  single feature i
+000052e0: 6e20 7468 6973 2066 6561 7475 7265 2067  n this feature g
+000052f0: 726f 7570 2e0a 0a20 2020 2020 2020 2021  roup...        !
+00005300: 2121 2065 7861 6d70 6c65 0a20 2020 2020  !! example.     
+00005310: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+00005320: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+00005330: 6f6e 6e65 6374 2074 6f20 7468 6520 4665  onnect to the Fe
+00005340: 6174 7572 6520 5374 6f72 650a 2020 2020  ature Store.    
+00005350: 2020 2020 2020 2020 6673 203d 202e 2e2e          fs = ...
+00005360: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00005370: 6765 7420 7468 6520 4665 6174 7572 6520  get the Feature 
+00005380: 4772 6f75 7020 696e 7374 616e 6365 0a20  Group instance. 
+00005390: 2020 2020 2020 2020 2020 2066 6720 3d20             fg = 
+000053a0: 6673 2e67 6574 5f6f 725f 6372 6561 7465  fs.get_or_create
+000053b0: 5f66 6561 7475 7265 5f67 726f 7570 282e  _feature_group(.
+000053c0: 2e2e 290a 0a20 2020 2020 2020 2020 2020  ..)..           
+000053d0: 2066 672e 7570 6461 7465 5f66 6561 7475   fg.update_featu
+000053e0: 7265 5f64 6573 6372 6970 7469 6f6e 2866  re_description(f
+000053f0: 6561 7475 7265 5f6e 616d 653d 226d 696e  eature_name="min
+00005400: 5f74 656d 7022 2c0a 2020 2020 2020 2020  _temp",.        
+00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005430: 2020 6465 7363 7269 7074 696f 6e3d 224d    description="M
+00005440: 7563 6820 6265 7474 6572 2066 6561 7475  uch better featu
+00005450: 7265 2064 6573 6372 6970 7469 6f6e 2e22  re description."
+00005460: 290a 2020 2020 2020 2020 2020 2020 6060  ).            ``
+00005470: 600a 0a20 2020 2020 2020 2021 2121 2069  `..        !!! i
+00005480: 6e66 6f20 2253 6166 6520 7570 6461 7465  nfo "Safe update
+00005490: 220a 2020 2020 2020 2020 2020 2020 5468  ".            Th
+000054a0: 6973 206d 6574 686f 6420 7570 6461 7465  is method update
+000054b0: 7320 7468 6520 6665 6174 7572 6520 6465  s the feature de
+000054c0: 7363 7269 7074 696f 6e20 7361 6665 6c79  scription safely
+000054d0: 2e20 496e 2063 6173 6520 6f66 2066 6169  . In case of fai
+000054e0: 6c75 7265 0a20 2020 2020 2020 2020 2020  lure.           
+000054f0: 2079 6f75 7220 6c6f 6361 6c20 6d65 7461   your local meta
+00005500: 6461 7461 206f 626a 6563 7420 7769 6c6c  data object will
+00005510: 206b 6565 7020 7468 6520 6f6c 6420 6465   keep the old de
+00005520: 7363 7269 7074 696f 6e2e 0a0a 2020 2020  scription...    
+00005530: 2020 2020 2320 4172 6775 6d65 6e74 730a      # Arguments.
+00005540: 2020 2020 2020 2020 2020 2020 6665 6174              feat
+00005550: 7572 655f 6e61 6d65 3a20 4e61 6d65 206f  ure_name: Name o
+00005560: 6620 7468 6520 6665 6174 7572 6520 746f  f the feature to
+00005570: 2062 6520 7570 6461 7465 642e 0a20 2020   be updated..   
+00005580: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00005590: 7469 6f6e 3a20 4e65 7720 6465 7363 7269  tion: New descri
+000055a0: 7074 696f 6e20 7374 7269 6e67 2e0a 0a20  ption string... 
+000055b0: 2020 2020 2020 2023 2052 6574 7572 6e73         # Returns
+000055c0: 0a20 2020 2020 2020 2020 2020 2060 4665  .            `Fe
+000055d0: 6174 7572 6547 726f 7570 602e 2054 6865  atureGroup`. The
+000055e0: 2075 7064 6174 6564 2066 6561 7475 7265   updated feature
+000055f0: 2067 726f 7570 206f 626a 6563 742e 0a20   group object.. 
+00005600: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00005610: 2020 2066 5f63 6f70 7920 3d20 636f 7079     f_copy = copy
+00005620: 2e64 6565 7063 6f70 7928 7365 6c66 5b66  .deepcopy(self[f
+00005630: 6561 7475 7265 5f6e 616d 655d 290a 2020  eature_name]).  
+00005640: 2020 2020 2020 665f 636f 7079 2e64 6573        f_copy.des
+00005650: 6372 6970 7469 6f6e 203d 2064 6573 6372  cription = descr
+00005660: 6970 7469 6f6e 0a20 2020 2020 2020 2073  iption.        s
+00005670: 656c 662e 5f66 6561 7475 7265 5f67 726f  elf._feature_gro
+00005680: 7570 5f65 6e67 696e 652e 7570 6461 7465  up_engine.update
+00005690: 5f66 6561 7475 7265 7328 7365 6c66 2c20  _features(self, 
+000056a0: 5b66 5f63 6f70 795d 290a 2020 2020 2020  [f_copy]).      
+000056b0: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
+000056c0: 2020 2064 6566 2061 7070 656e 645f 6665     def append_fe
+000056d0: 6174 7572 6573 2873 656c 662c 2066 6561  atures(self, fea
+000056e0: 7475 7265 733a 2055 6e69 6f6e 5b66 6561  tures: Union[fea
+000056f0: 7475 7265 2e46 6561 7475 7265 2c20 4c69  ture.Feature, Li
+00005700: 7374 5b66 6561 7475 7265 2e46 6561 7475  st[feature.Featu
+00005710: 7265 5d5d 293a 0a20 2020 2020 2020 2022  re]]):.        "
+00005720: 2222 4170 7065 6e64 2066 6561 7475 7265  ""Append feature
+00005730: 7320 746f 2074 6865 2073 6368 656d 6120  s to the schema 
+00005740: 6f66 2074 6865 2066 6561 7475 7265 2067  of the feature g
+00005750: 726f 7570 2e0a 0a20 2020 2020 2020 2021  roup...        !
+00005760: 2121 2065 7861 6d70 6c65 0a20 2020 2020  !! example.     
+00005770: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+00005780: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+00005790: 6f6e 6e65 6374 2074 6f20 7468 6520 4665  onnect to the Fe
+000057a0: 6174 7572 6520 5374 6f72 650a 2020 2020  ature Store.    
+000057b0: 2020 2020 2020 2020 6673 203d 202e 2e2e          fs = ...
+000057c0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+000057d0: 6465 6669 6e65 2066 6561 7475 7265 7320  define features 
+000057e0: 746f 2062 6520 696e 7365 7274 6564 2069  to be inserted i
+000057f0: 6e20 7468 6520 6665 6174 7572 6520 6772  n the feature gr
+00005800: 6f75 700a 2020 2020 2020 2020 2020 2020  oup.            
+00005810: 6665 6174 7572 6573 203d 205b 0a20 2020  features = [.   
+00005820: 2020 2020 2020 2020 2020 2020 2046 6561               Fea
+00005830: 7475 7265 286e 616d 653d 2269 6422 2c74  ture(name="id",t
+00005840: 7970 653d 2269 6e74 222c 6f6e 6c69 6e65  ype="int",online
+00005850: 5f74 7970 653d 2269 6e74 2229 2c0a 2020  _type="int"),.  
+00005860: 2020 2020 2020 2020 2020 2020 2020 4665                Fe
+00005870: 6174 7572 6528 6e61 6d65 3d22 6e61 6d65  ature(name="name
+00005880: 222c 7479 7065 3d22 7374 7269 6e67 222c  ",type="string",
+00005890: 6f6e 6c69 6e65 5f74 7970 653d 2276 6172  online_type="var
+000058a0: 6368 6172 2832 3029 2229 0a20 2020 2020  char(20)").     
+000058b0: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
+000058c0: 2020 2020 2020 2320 6765 7420 7468 6520        # get the 
+000058d0: 4665 6174 7572 6520 4772 6f75 7020 696e  Feature Group in
+000058e0: 7374 616e 6365 0a20 2020 2020 2020 2020  stance.         
+000058f0: 2020 2066 6720 3d20 6673 2e67 6574 5f6f     fg = fs.get_o
+00005900: 725f 6372 6561 7465 5f66 6561 7475 7265  r_create_feature
+00005910: 5f67 726f 7570 282e 2e2e 290a 0a20 2020  _group(...)..   
+00005920: 2020 2020 2020 2020 2066 672e 6170 7065           fg.appe
+00005930: 6e64 5f66 6561 7475 7265 7328 6665 6174  nd_features(feat
+00005940: 7572 6573 290a 2020 2020 2020 2020 2020  ures).          
+00005950: 2020 6060 600a 0a20 2020 2020 2020 2021    ```..        !
+00005960: 2121 2069 6e66 6f20 2253 6166 6520 6170  !! info "Safe ap
+00005970: 7065 6e64 220a 2020 2020 2020 2020 2020  pend".          
+00005980: 2020 5468 6973 206d 6574 686f 6420 6170    This method ap
+00005990: 7065 6e64 7320 7468 6520 6665 6174 7572  pends the featur
+000059a0: 6573 2074 6f20 7468 6520 6665 6174 7572  es to the featur
+000059b0: 6520 6772 6f75 7020 6465 7363 7269 7074  e group descript
+000059c0: 696f 6e20 7361 6665 6c79 2e0a 2020 2020  ion safely..    
+000059d0: 2020 2020 2020 2020 496e 2063 6173 6520          In case 
+000059e0: 6f66 2066 6169 6c75 7265 2079 6f75 7220  of failure your 
+000059f0: 6c6f 6361 6c20 6d65 7461 6461 7461 206f  local metadata o
+00005a00: 626a 6563 7420 7769 6c6c 2063 6f6e 7461  bject will conta
+00005a10: 696e 2074 6865 2063 6f72 7265 6374 0a20  in the correct. 
+00005a20: 2020 2020 2020 2020 2020 2073 6368 656d             schem
+00005a30: 612e 0a0a 2020 2020 2020 2020 4974 2069  a...        It i
+00005a40: 7320 6f6e 6c79 2070 6f73 7369 626c 6520  s only possible 
+00005a50: 746f 2061 7070 656e 6420 6665 6174 7572  to append featur
+00005a60: 6573 2074 6f20 6120 6665 6174 7572 6520  es to a feature 
+00005a70: 6772 6f75 702e 2052 656d 6f76 696e 670a  group. Removing.
+00005a80: 2020 2020 2020 2020 6665 6174 7572 6573          features
+00005a90: 2069 7320 636f 6e73 6964 6572 6564 2061   is considered a
+00005aa0: 2062 7265 616b 696e 6720 6368 616e 6765   breaking change
+00005ab0: 2e0a 0a20 2020 2020 2020 2023 2041 7267  ...        # Arg
+00005ac0: 756d 656e 7473 0a20 2020 2020 2020 2020  uments.         
+00005ad0: 2020 2066 6561 7475 7265 733a 2046 6561     features: Fea
+00005ae0: 7475 7265 206f 7220 6c69 7374 2e20 4120  ture or list. A 
+00005af0: 6665 6174 7572 6520 6f62 6a65 6374 206f  feature object o
+00005b00: 7220 6c69 7374 2074 6865 7265 6f66 2074  r list thereof t
+00005b10: 6f20 6170 7065 6e64 2074 6f0a 2020 2020  o append to.    
+00005b20: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00005b30: 7363 6865 6d61 206f 6620 7468 6520 6665  schema of the fe
+00005b40: 6174 7572 6520 6772 6f75 702e 0a0a 2020  ature group...  
+00005b50: 2020 2020 2020 2320 5265 7475 726e 730a        # Returns.
+00005b60: 2020 2020 2020 2020 2020 2020 6046 6561              `Fea
+00005b70: 7475 7265 4772 6f75 7060 2e20 5468 6520  tureGroup`. The 
+00005b80: 7570 6461 7465 6420 6665 6174 7572 6520  updated feature 
+00005b90: 6772 6f75 7020 6f62 6a65 6374 2e0a 2020  group object..  
+00005ba0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00005bb0: 2020 6e65 775f 6665 6174 7572 6573 203d    new_features =
+00005bc0: 205b 5d0a 2020 2020 2020 2020 6966 2069   [].        if i
+00005bd0: 7369 6e73 7461 6e63 6528 6665 6174 7572  sinstance(featur
+00005be0: 6573 2c20 6665 6174 7572 652e 4665 6174  es, feature.Feat
+00005bf0: 7572 6529 3a0a 2020 2020 2020 2020 2020  ure):.          
+00005c00: 2020 6e65 775f 6665 6174 7572 6573 2e61    new_features.a
+00005c10: 7070 656e 6428 6665 6174 7572 6573 290a  ppend(features).
+00005c20: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+00005c30: 6e73 7461 6e63 6528 6665 6174 7572 6573  nstance(features
+00005c40: 2c20 6c69 7374 293a 0a20 2020 2020 2020  , list):.       
+00005c50: 2020 2020 2066 6f72 2066 6561 7420 696e       for feat in
+00005c60: 2066 6561 7475 7265 733a 0a20 2020 2020   features:.     
+00005c70: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00005c80: 696e 7374 616e 6365 2866 6561 742c 2066  instance(feat, f
+00005c90: 6561 7475 7265 2e46 6561 7475 7265 293a  eature.Feature):
+00005ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005cb0: 2020 2020 206e 6577 5f66 6561 7475 7265       new_feature
+00005cc0: 732e 6170 7065 6e64 2866 6561 7429 0a20  s.append(feat). 
+00005cd0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00005ce0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00005cf0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+00005d00: 7970 6545 7272 6f72 280a 2020 2020 2020  ypeError(.      
+00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d20: 2020 2254 6865 2061 7267 756d 656e 7420    "The argument 
+00005d30: 6066 6561 7475 7265 7360 2068 6173 2074  `features` has t
+00005d40: 6f20 6265 206f 6620 7479 7065 2060 4665  o be of type `Fe
+00005d50: 6174 7572 6560 206f 7220 220a 2020 2020  ature` or ".    
+00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d70: 2020 2020 2261 206c 6973 7420 7468 6572      "a list ther
+00005d80: 656f 662c 2062 7574 2061 6e20 656c 656d  eof, but an elem
+00005d90: 656e 7420 6973 206f 6620 7479 7065 3a20  ent is of type: 
+00005da0: 607b 7d60 222e 666f 726d 6174 280a 2020  `{}`".format(.  
+00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005dc0: 2020 2020 2020 2020 2020 7479 7065 2866            type(f
+00005dd0: 6561 7475 7265 7329 0a20 2020 2020 2020  eatures).       
+00005de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005df0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00005e00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00005e10: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00005e20: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
+00005e30: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+00005e40: 2020 2020 2254 6865 2061 7267 756d 656e      "The argumen
+00005e50: 7420 6066 6561 7475 7265 7360 2068 6173  t `features` has
+00005e60: 2074 6f20 6265 206f 6620 7479 7065 2060   to be of type `
+00005e70: 4665 6174 7572 6560 206f 7220 6120 6c69  Feature` or a li
+00005e80: 7374 2022 0a20 2020 2020 2020 2020 2020  st ".           
+00005e90: 2020 2020 2022 7468 6572 656f 662c 2062       "thereof, b
+00005ea0: 7574 2069 7320 6f66 2074 7970 653a 2060  ut is of type: `
+00005eb0: 7b7d 6022 2e66 6f72 6d61 7428 7479 7065  {}`".format(type
+00005ec0: 2866 6561 7475 7265 7329 290a 2020 2020  (features)).    
+00005ed0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00005ee0: 2020 7365 6c66 2e5f 6665 6174 7572 655f    self._feature_
+00005ef0: 6772 6f75 705f 656e 6769 6e65 2e61 7070  group_engine.app
+00005f00: 656e 645f 6665 6174 7572 6573 2873 656c  end_features(sel
+00005f10: 662c 206e 6577 5f66 6561 7475 7265 7329  f, new_features)
+00005f20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00005f30: 7365 6c66 0a0a 2020 2020 6465 6620 6765  self..    def ge
+00005f40: 745f 6578 7065 6374 6174 696f 6e5f 7375  t_expectation_su
+00005f50: 6974 6528 0a20 2020 2020 2020 2073 656c  ite(.        sel
+00005f60: 662c 2067 655f 7479 7065 3a20 626f 6f6c  f, ge_type: bool
+00005f70: 203d 2054 7275 650a 2020 2020 2920 2d3e   = True.    ) ->
+00005f80: 2055 6e69 6f6e 5b45 7870 6563 7461 7469   Union[Expectati
+00005f90: 6f6e 5375 6974 652c 2067 652e 636f 7265  onSuite, ge.core
+00005fa0: 2e45 7870 6563 7461 7469 6f6e 5375 6974  .ExpectationSuit
+00005fb0: 652c 204e 6f6e 655d 3a0a 2020 2020 2020  e, None]:.      
+00005fc0: 2020 2222 2252 6574 7572 6e20 7468 6520    """Return the 
+00005fd0: 6578 7065 6374 6174 696f 6e20 7375 6974  expectation suit
+00005fe0: 6520 6174 7461 6368 6564 2074 6f20 7468  e attached to th
+00005ff0: 6520 6665 6174 7572 6520 6772 6f75 7020  e feature group 
+00006000: 6966 2069 7420 6578 6973 7473 2e0a 0a20  if it exists... 
+00006010: 2020 2020 2020 2021 2121 2065 7861 6d70         !!! examp
+00006020: 6c65 0a20 2020 2020 2020 2020 2020 2060  le.            `
+00006030: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
+00006040: 2020 2020 2023 2063 6f6e 6e65 6374 2074       # connect t
+00006050: 6f20 7468 6520 4665 6174 7572 6520 5374  o the Feature St
+00006060: 6f72 650a 2020 2020 2020 2020 2020 2020  ore.            
+00006070: 6673 203d 202e 2e2e 0a0a 2020 2020 2020  fs = .....      
+00006080: 2020 2020 2020 2320 6765 7420 7468 6520        # get the 
+00006090: 4665 6174 7572 6520 4772 6f75 7020 696e  Feature Group in
+000060a0: 7374 616e 6365 0a20 2020 2020 2020 2020  stance.         
+000060b0: 2020 2066 6720 3d20 6673 2e67 6574 5f6f     fg = fs.get_o
+000060c0: 725f 6372 6561 7465 5f66 6561 7475 7265  r_create_feature
+000060d0: 5f67 726f 7570 282e 2e2e 290a 0a20 2020  _group(...)..   
+000060e0: 2020 2020 2020 2020 2065 7870 5f73 7569           exp_sui
+000060f0: 7465 203d 2066 672e 6765 745f 6578 7065  te = fg.get_expe
+00006100: 6374 6174 696f 6e5f 7375 6974 6528 290a  ctation_suite().
+00006110: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
+00006120: 0a20 2020 2020 2020 2023 2041 7267 756d  .        # Argum
+00006130: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
+00006140: 2067 655f 7479 7065 3a20 4966 2060 5472   ge_type: If `Tr
+00006150: 7565 6020 7265 7475 726e 7320 6120 6e61  ue` returns a na
+00006160: 7469 7665 2047 7265 6174 2045 7870 6563  tive Great Expec
+00006170: 7461 7469 6f6e 2074 7970 652c 2048 6f70  tation type, Hop
+00006180: 7377 6f72 6b73 0a20 2020 2020 2020 2020  sworks.         
+00006190: 2020 2020 2020 2063 7573 746f 6d20 7479         custom ty
+000061a0: 7065 206f 7468 6572 7769 7365 2e20 436f  pe otherwise. Co
+000061b0: 6e76 6572 7369 6f6e 2063 616e 2062 6520  nversion can be 
+000061c0: 7065 7266 6f72 6d65 6420 7669 6120 7468  performed via th
+000061d0: 6520 6074 6f5f 6765 5f74 7970 6528 2960  e `to_ge_type()`
+000061e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000061f0: 206d 6574 686f 6420 6f6e 2068 6f70 7377   method on hopsw
+00006200: 6f72 6b73 2074 7970 652e 2044 6566 6175  orks type. Defau
+00006210: 6c74 7320 746f 2060 5472 7565 602e 0a0a  lts to `True`...
+00006220: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
+00006230: 730a 2020 2020 2020 2020 2020 2020 6045  s.            `E
+00006240: 7870 6563 7461 7469 6f6e 5375 6974 6560  xpectationSuite`
+00006250: 2e20 5468 6520 6578 7065 6374 6174 696f  . The expectatio
+00006260: 6e20 7375 6974 6520 6174 7461 6368 6564  n suite attached
+00006270: 2074 6f20 7468 6520 6665 6174 7572 6520   to the feature 
+00006280: 6772 6f75 702e 0a0a 2020 2020 2020 2020  group...        
+00006290: 2320 5261 6973 6573 0a20 2020 2020 2020  # Raises.       
+000062a0: 2020 2020 2060 6873 6673 2e63 6c69 656e       `hsfs.clien
+000062b0: 742e 6578 6365 7074 696f 6e73 2e52 6573  t.exceptions.Res
+000062c0: 7441 5049 4572 726f 7260 2e0a 2020 2020  tAPIError`..    
+000062d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000062e0: 2320 4176 6f69 6420 7468 726f 7769 6e67  # Avoid throwing
+000062f0: 2061 6e20 6572 726f 7220 6966 2046 6561   an error if Fea
+00006300: 7475 7265 2047 726f 7570 206e 6f74 2069  ture Group not i
+00006310: 6e69 7469 616c 6973 6564 2e0a 2020 2020  nitialised..    
+00006320: 2020 2020 6966 2073 656c 662e 5f69 643a      if self._id:
+00006330: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006340: 662e 5f65 7870 6563 7461 7469 6f6e 5f73  f._expectation_s
+00006350: 7569 7465 203d 2073 656c 662e 5f65 7870  uite = self._exp
+00006360: 6563 7461 7469 6f6e 5f73 7569 7465 5f65  ectation_suite_e
+00006370: 6e67 696e 652e 6765 7428 290a 0a20 2020  ngine.get()..   
+00006380: 2020 2020 2069 6620 7365 6c66 2e5f 6578       if self._ex
+00006390: 7065 6374 6174 696f 6e5f 7375 6974 6520  pectation_suite 
+000063a0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+000063b0: 6765 5f74 7970 6520 6973 2054 7275 653a  ge_type is True:
+000063c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000063d0: 7572 6e20 7365 6c66 2e5f 6578 7065 6374  urn self._expect
+000063e0: 6174 696f 6e5f 7375 6974 652e 746f 5f67  ation_suite.to_g
+000063f0: 655f 7479 7065 2829 0a20 2020 2020 2020  e_type().       
+00006400: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00006410: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00006420: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
+00006430: 650a 0a20 2020 2064 6566 2073 6176 655f  e..    def save_
+00006440: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
+00006450: 6528 0a20 2020 2020 2020 2073 656c 662c  e(.        self,
+00006460: 0a20 2020 2020 2020 2065 7870 6563 7461  .        expecta
+00006470: 7469 6f6e 5f73 7569 7465 3a20 556e 696f  tion_suite: Unio
+00006480: 6e5b 4578 7065 6374 6174 696f 6e53 7569  n[ExpectationSui
+00006490: 7465 2c20 6765 2e63 6f72 652e 4578 7065  te, ge.core.Expe
+000064a0: 6374 6174 696f 6e53 7569 7465 5d2c 0a20  ctationSuite],. 
+000064b0: 2020 2020 2020 2072 756e 5f76 616c 6964         run_valid
+000064c0: 6174 696f 6e3a 2062 6f6f 6c20 3d20 5472  ation: bool = Tr
+000064d0: 7565 2c0a 2020 2020 2020 2020 7661 6c69  ue,.        vali
+000064e0: 6461 7469 6f6e 5f69 6e67 6573 7469 6f6e  dation_ingestion
+000064f0: 5f70 6f6c 6963 793a 2073 7472 203d 2022  _policy: str = "
+00006500: 414c 5741 5953 222c 0a20 2020 2020 2020  ALWAYS",.       
+00006510: 206f 7665 7277 7269 7465 3a20 626f 6f6c   overwrite: bool
+00006520: 203d 2046 616c 7365 2c0a 2020 2020 2920   = False,.    ) 
+00006530: 2d3e 2055 6e69 6f6e 5b45 7870 6563 7461  -> Union[Expecta
+00006540: 7469 6f6e 5375 6974 652c 2067 652e 636f  tionSuite, ge.co
+00006550: 7265 2e45 7870 6563 7461 7469 6f6e 5375  re.ExpectationSu
+00006560: 6974 655d 3a0a 2020 2020 2020 2020 2222  ite]:.        ""
+00006570: 2241 7474 6163 6820 616e 2065 7870 6563  "Attach an expec
+00006580: 7461 7469 6f6e 2073 7569 7465 2074 6f20  tation suite to 
+00006590: 6120 6665 6174 7572 6520 6772 6f75 7020  a feature group 
+000065a0: 616e 6420 7361 7665 7320 6974 2066 6f72  and saves it for
+000065b0: 2066 7574 7572 6520 7573 652e 2049 6620   future use. If 
+000065c0: 616e 2065 7870 6563 7461 7469 6f6e 0a20  an expectation. 
+000065d0: 2020 2020 2020 2073 7569 7465 2069 7320         suite is 
+000065e0: 616c 7265 6164 7920 6174 7461 6368 6564  already attached
+000065f0: 2c20 6974 2069 7320 7265 706c 6163 6564  , it is replaced
+00006600: 2e20 4e6f 7465 2074 6861 7420 7468 6520  . Note that the 
+00006610: 7072 6f76 6964 6564 2065 7870 6563 7461  provided expecta
+00006620: 7469 6f6e 2073 7569 7465 2069 7320 6d6f  tion suite is mo
+00006630: 6469 6669 6564 0a20 2020 2020 2020 2069  dified.        i
+00006640: 6e70 6c61 6365 2074 6f20 696e 636c 7564  nplace to includ
+00006650: 6520 6578 7065 6374 6174 696f 6e49 6420  e expectationId 
+00006660: 6669 656c 6473 2e0a 0a20 2020 2020 2020  fields...       
+00006670: 2021 2121 2065 7861 6d70 6c65 0a20 2020   !!! example.   
+00006680: 2020 2020 2020 2020 2060 6060 7079 7468           ```pyth
+00006690: 6f6e 0a20 2020 2020 2020 2020 2020 2023  on.            #
+000066a0: 2063 6f6e 6e65 6374 2074 6f20 7468 6520   connect to the 
+000066b0: 4665 6174 7572 6520 5374 6f72 650a 2020  Feature Store.  
+000066c0: 2020 2020 2020 2020 2020 6673 203d 202e            fs = .
+000066d0: 2e2e 0a0a 2020 2020 2020 2020 2020 2020  ....            
+000066e0: 2320 6765 7420 7468 6520 4665 6174 7572  # get the Featur
+000066f0: 6520 4772 6f75 7020 696e 7374 616e 6365  e Group instance
+00006700: 0a20 2020 2020 2020 2020 2020 2066 6720  .            fg 
+00006710: 3d20 6673 2e67 6574 5f6f 725f 6372 6561  = fs.get_or_crea
+00006720: 7465 5f66 6561 7475 7265 5f67 726f 7570  te_feature_group
+00006730: 282e 2e2e 290a 0a20 2020 2020 2020 2020  (...)..         
+00006740: 2020 2066 672e 7361 7665 5f65 7870 6563     fg.save_expec
+00006750: 7461 7469 6f6e 5f73 7569 7465 2865 7870  tation_suite(exp
+00006760: 6563 7461 7469 6f6e 5f73 7569 7465 2c20  ectation_suite, 
+00006770: 7275 6e5f 7661 6c69 6461 7469 6f6e 3d54  run_validation=T
+00006780: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00006790: 2060 6060 0a0a 2020 2020 2020 2020 2320   ```..        # 
+000067a0: 4172 6775 6d65 6e74 730a 2020 2020 2020  Arguments.      
+000067b0: 2020 2020 2020 6578 7065 6374 6174 696f        expectatio
+000067c0: 6e5f 7375 6974 653a 2054 6865 2065 7870  n_suite: The exp
+000067d0: 6563 7461 7469 6f6e 2073 7569 7465 2074  ectation suite t
+000067e0: 6f20 6174 7461 6368 2074 6f20 7468 6520  o attach to the 
+000067f0: 4665 6174 7572 6520 4772 6f75 702e 0a20  Feature Group.. 
+00006800: 2020 2020 2020 2020 2020 206f 7665 7277             overw
+00006810: 7269 7465 3a20 4966 2061 6e20 4578 7065  rite: If an Expe
+00006820: 6374 6174 696f 6e20 5375 6974 6520 6973  ctation Suite is
+00006830: 2061 6c72 6561 6479 2061 7474 6163 6865   already attache
+00006840: 642c 206f 7665 7277 7269 7465 2069 742e  d, overwrite it.
+00006850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006860: 2054 6865 206e 6577 2073 7569 7465 2077   The new suite w
+00006870: 696c 6c20 6861 7665 2069 7473 206f 776e  ill have its own
+00006880: 2076 616c 6964 6174 696f 6e20 6869 7374   validation hist
+00006890: 6f72 792c 2062 7574 2066 6f72 6d65 7220  ory, but former 
+000068a0: 7265 706f 7274 7320 6172 6520 7072 6573  reports are pres
+000068b0: 6572 7665 642e 0a20 2020 2020 2020 2020  erved..         
+000068c0: 2020 2072 756e 5f76 616c 6964 6174 696f     run_validatio
+000068d0: 6e3a 2053 6574 2077 6865 7468 6572 2074  n: Set whether t
+000068e0: 6865 2065 7870 6563 7461 7469 6f6e 5f73  he expectation_s
+000068f0: 7569 7465 2077 696c 6c20 7275 6e20 6f6e  uite will run on
+00006900: 2069 6e67 6573 7469 6f6e 0a20 2020 2020   ingestion.     
+00006910: 2020 2020 2020 2076 616c 6964 6174 696f         validatio
+00006920: 6e5f 696e 6765 7374 696f 6e5f 706f 6c69  n_ingestion_poli
+00006930: 6379 3a20 5365 7420 7468 6520 706f 6c69  cy: Set the poli
+00006940: 6379 2066 6f72 2069 6e67 6573 7469 6f6e  cy for ingestion
+00006950: 2074 6f20 7468 6520 4665 6174 7572 6520   to the Feature 
+00006960: 4772 6f75 702e 0a20 2020 2020 2020 2020  Group..         
+00006970: 2020 2020 2020 202d 2022 5354 5249 4354         - "STRICT
+00006980: 2220 6f6e 6c79 2061 6c6c 6f77 7320 4461  " only allows Da
+00006990: 7461 4672 616d 6520 7061 7373 696e 6720  taFrame passing 
+000069a0: 7661 6c69 6461 7469 6f6e 2074 6f20 6265  validation to be
+000069b0: 2069 6e73 6572 7465 6420 696e 746f 2046   inserted into F
+000069c0: 6561 7475 7265 2047 726f 7570 2e0a 2020  eature Group..  
+000069d0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+000069e0: 2241 4c57 4159 5322 2061 6c77 6179 7320  "ALWAYS" always 
+000069f0: 696e 7365 7274 2074 6865 2044 6174 6146  insert the DataF
+00006a00: 7261 6d65 2074 6f20 7468 6520 4665 6174  rame to the Feat
+00006a10: 7572 6520 4772 6f75 702c 2069 7272 6573  ure Group, irres
+00006a20: 7065 6374 6976 6520 6f66 206f 7665 7261  pective of overa
+00006a30: 6c6c 2076 616c 6964 6174 696f 6e20 7265  ll validation re
+00006a40: 7375 6c74 2e0a 0a20 2020 2020 2020 2023  sult...        #
+00006a50: 2052 6169 7365 730a 2020 2020 2020 2020   Raises.        
+00006a60: 2020 2020 6068 7366 732e 636c 6965 6e74      `hsfs.client
+00006a70: 2e65 7863 6570 7469 6f6e 732e 5265 7374  .exceptions.Rest
+00006a80: 4150 4945 7272 6f72 602e 0a20 2020 2020  APIError`..     
+00006a90: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00006aa0: 6620 6973 696e 7374 616e 6365 2865 7870  f isinstance(exp
+00006ab0: 6563 7461 7469 6f6e 5f73 7569 7465 2c20  ectation_suite, 
+00006ac0: 6765 2e63 6f72 652e 4578 7065 6374 6174  ge.core.Expectat
+00006ad0: 696f 6e53 7569 7465 293a 0a20 2020 2020  ionSuite):.     
+00006ae0: 2020 2020 2020 2074 6d70 5f65 7870 6563         tmp_expec
+00006af0: 7461 7469 6f6e 5f73 7569 7465 203d 2045  tation_suite = E
+00006b00: 7870 6563 7461 7469 6f6e 5375 6974 652e  xpectationSuite.
+00006b10: 6672 6f6d 5f67 655f 7479 7065 280a 2020  from_ge_type(.  
+00006b20: 2020 2020 2020 2020 2020 2020 2020 6765                ge
+00006b30: 5f65 7870 6563 7461 7469 6f6e 5f73 7569  _expectation_sui
+00006b40: 7465 3d65 7870 6563 7461 7469 6f6e 5f73  te=expectation_s
+00006b50: 7569 7465 2c0a 2020 2020 2020 2020 2020  uite,.          
+00006b60: 2020 2020 2020 7275 6e5f 7661 6c69 6461        run_valida
+00006b70: 7469 6f6e 3d72 756e 5f76 616c 6964 6174  tion=run_validat
+00006b80: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00006b90: 2020 2020 2076 616c 6964 6174 696f 6e5f       validation_
+00006ba0: 696e 6765 7374 696f 6e5f 706f 6c69 6379  ingestion_policy
+00006bb0: 3d76 616c 6964 6174 696f 6e5f 696e 6765  =validation_inge
+00006bc0: 7374 696f 6e5f 706f 6c69 6379 2c0a 2020  stion_policy,.  
+00006bd0: 2020 2020 2020 2020 2020 2020 2020 6665                fe
+00006be0: 6174 7572 655f 7374 6f72 655f 6964 3d73  ature_store_id=s
+00006bf0: 656c 662e 5f66 6561 7475 7265 5f73 746f  elf._feature_sto
+00006c00: 7265 5f69 642c 0a20 2020 2020 2020 2020  re_id,.         
+00006c10: 2020 2020 2020 2066 6561 7475 7265 5f67         feature_g
+00006c20: 726f 7570 5f69 643d 7365 6c66 2e5f 6964  roup_id=self._id
+00006c30: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00006c40: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+00006c50: 6e73 7461 6e63 6528 6578 7065 6374 6174  nstance(expectat
+00006c60: 696f 6e5f 7375 6974 652c 2045 7870 6563  ion_suite, Expec
+00006c70: 7461 7469 6f6e 5375 6974 6529 3a0a 2020  tationSuite):.  
+00006c80: 2020 2020 2020 2020 2020 746d 705f 6578            tmp_ex
+00006c90: 7065 6374 6174 696f 6e5f 7375 6974 6520  pectation_suite 
+00006ca0: 3d20 6578 7065 6374 6174 696f 6e5f 7375  = expectation_su
+00006cb0: 6974 652e 746f 5f6a 736f 6e5f 6469 6374  ite.to_json_dict
+00006cc0: 2864 6563 616d 656c 697a 653d 5472 7565  (decamelize=True
+00006cd0: 290a 2020 2020 2020 2020 2020 2020 746d  ).            tm
+00006ce0: 705f 6578 7065 6374 6174 696f 6e5f 7375  p_expectation_su
+00006cf0: 6974 655b 2266 6561 7475 7265 5f67 726f  ite["feature_gro
+00006d00: 7570 5f69 6422 5d20 3d20 7365 6c66 2e5f  up_id"] = self._
+00006d10: 6964 0a20 2020 2020 2020 2020 2020 2074  id.            t
+00006d20: 6d70 5f65 7870 6563 7461 7469 6f6e 5f73  mp_expectation_s
+00006d30: 7569 7465 5b22 6665 6174 7572 655f 7374  uite["feature_st
+00006d40: 6f72 655f 6964 225d 203d 2073 656c 662e  ore_id"] = self.
+00006d50: 5f66 6561 7475 7265 5f73 746f 7265 5f69  _feature_store_i
+00006d60: 640a 2020 2020 2020 2020 2020 2020 746d  d.            tm
+00006d70: 705f 6578 7065 6374 6174 696f 6e5f 7375  p_expectation_su
+00006d80: 6974 6520 3d20 4578 7065 6374 6174 696f  ite = Expectatio
+00006d90: 6e53 7569 7465 282a 2a74 6d70 5f65 7870  nSuite(**tmp_exp
+00006da0: 6563 7461 7469 6f6e 5f73 7569 7465 290a  ectation_suite).
+00006db0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00006dc0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00006dd0: 5479 7065 4572 726f 7228 0a20 2020 2020  TypeError(.     
+00006de0: 2020 2020 2020 2020 2020 2022 5468 6520             "The 
+00006df0: 7072 6f76 6964 6564 2065 7870 6563 7461  provided expecta
+00006e00: 7469 6f6e 2073 7569 7465 2074 7970 6520  tion suite type 
+00006e10: 607b 7d60 2069 7320 6e6f 7420 7375 7070  `{}` is not supp
+00006e20: 6f72 7465 642e 2055 7365 2047 7265 6174  orted. Use Great
+00006e30: 2045 7870 6563 7461 7469 6f6e 2060 4578   Expectation `Ex
+00006e40: 7065 6374 6174 696f 6e53 7569 7465 6020  pectationSuite` 
+00006e50: 6f72 2048 5346 5327 206f 776e 2060 4578  or HSFS' own `Ex
+00006e60: 7065 6374 6174 696f 6e53 7569 7465 6020  pectationSuite` 
+00006e70: 6f62 6a65 6374 2e22 2e66 6f72 6d61 7428  object.".format(
+00006e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006e90: 2020 2020 2074 7970 6528 6578 7065 6374       type(expect
+00006ea0: 6174 696f 6e5f 7375 6974 6529 0a20 2020  ation_suite).   
+00006eb0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00006ec0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00006ed0: 2020 2020 2020 6966 206f 7665 7277 7269        if overwri
+00006ee0: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
+00006ef0: 7365 6c66 2e64 656c 6574 655f 6578 7065  self.delete_expe
+00006f00: 6374 6174 696f 6e5f 7375 6974 6528 290a  ctation_suite().
+00006f10: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00006f20: 2e5f 6964 3a0a 2020 2020 2020 2020 2020  ._id:.          
+00006f30: 2020 7365 6c66 2e5f 6578 7065 6374 6174    self._expectat
+00006f40: 696f 6e5f 7375 6974 6520 3d20 7365 6c66  ion_suite = self
+00006f50: 2e5f 6578 7065 6374 6174 696f 6e5f 7375  ._expectation_su
+00006f60: 6974 655f 656e 6769 6e65 2e73 6176 6528  ite_engine.save(
+00006f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006f80: 2074 6d70 5f65 7870 6563 7461 7469 6f6e   tmp_expectation
+00006f90: 5f73 7569 7465 0a20 2020 2020 2020 2020  _suite.         
+00006fa0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00006fb0: 2065 7870 6563 7461 7469 6f6e 5f73 7569   expectation_sui
+00006fc0: 7465 203d 2073 656c 662e 5f65 7870 6563  te = self._expec
+00006fd0: 7461 7469 6f6e 5f73 7569 7465 2e74 6f5f  tation_suite.to_
+00006fe0: 6765 5f74 7970 6528 290a 2020 2020 2020  ge_type().      
+00006ff0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00007000: 2020 2020 2320 4164 6465 6420 746f 2061      # Added to a
+00007010: 766f 6964 2074 6872 6f77 696e 6720 616e  void throwing an
+00007020: 2065 7272 6f72 2069 6620 4665 6174 7572   error if Featur
+00007030: 6520 4772 6f75 7020 6973 206e 6f74 2069  e Group is not i
+00007040: 6e69 7469 616c 6973 6564 2077 6974 6820  nitialised with 
+00007050: 7468 6520 6261 636b 656e 640a 2020 2020  the backend.    
+00007060: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
+00007070: 7065 6374 6174 696f 6e5f 7375 6974 6520  pectation_suite 
+00007080: 3d20 746d 705f 6578 7065 6374 6174 696f  = tmp_expectatio
+00007090: 6e5f 7375 6974 650a 0a20 2020 2064 6566  n_suite..    def
+000070a0: 2064 656c 6574 655f 6578 7065 6374 6174   delete_expectat
+000070b0: 696f 6e5f 7375 6974 6528 7365 6c66 2920  ion_suite(self) 
+000070c0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000070d0: 2022 2222 4465 6c65 7465 2074 6865 2065   """Delete the e
+000070e0: 7870 6563 7461 7469 6f6e 2073 7569 7465  xpectation suite
+000070f0: 2061 7474 6163 6865 6420 746f 2074 6865   attached to the
+00007100: 2046 6561 7475 7265 2047 726f 7570 2e0a   Feature Group..
+00007110: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
+00007120: 6d70 6c65 0a20 2020 2020 2020 2020 2020  mple.           
+00007130: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
+00007140: 2020 2020 2020 2023 2063 6f6e 6e65 6374         # connect
+00007150: 2074 6f20 7468 6520 4665 6174 7572 6520   to the Feature 
+00007160: 5374 6f72 650a 2020 2020 2020 2020 2020  Store.          
+00007170: 2020 6673 203d 202e 2e2e 0a0a 2020 2020    fs = .....    
+00007180: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
+00007190: 6520 4665 6174 7572 6520 4772 6f75 7020  e Feature Group 
+000071a0: 696e 7374 616e 6365 0a20 2020 2020 2020  instance.       
+000071b0: 2020 2020 2066 6720 3d20 6673 2e67 6574       fg = fs.get
+000071c0: 5f6f 725f 6372 6561 7465 5f66 6561 7475  _or_create_featu
+000071d0: 7265 5f67 726f 7570 282e 2e2e 290a 0a20  re_group(...).. 
+000071e0: 2020 2020 2020 2020 2020 2066 672e 6465             fg.de
+000071f0: 6c65 7465 5f65 7870 6563 7461 7469 6f6e  lete_expectation
+00007200: 5f73 7569 7465 2829 0a20 2020 2020 2020  _suite().       
+00007210: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
+00007220: 2020 2320 5261 6973 6573 0a20 2020 2020    # Raises.     
+00007230: 2020 2020 2020 2060 6873 6673 2e63 6c69         `hsfs.cli
+00007240: 656e 742e 6578 6365 7074 696f 6e73 2e52  ent.exceptions.R
+00007250: 6573 7441 5049 4572 726f 7260 2e0a 2020  estAPIError`..  
+00007260: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00007270: 2020 6966 2073 656c 662e 6765 745f 6578    if self.get_ex
+00007280: 7065 6374 6174 696f 6e5f 7375 6974 6528  pectation_suite(
+00007290: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000072a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000072b0: 5f65 7870 6563 7461 7469 6f6e 5f73 7569  _expectation_sui
+000072c0: 7465 5f65 6e67 696e 652e 6465 6c65 7465  te_engine.delete
+000072d0: 2873 656c 662e 5f65 7870 6563 7461 7469  (self._expectati
+000072e0: 6f6e 5f73 7569 7465 2e69 6429 0a20 2020  on_suite.id).   
+000072f0: 2020 2020 2073 656c 662e 5f65 7870 6563       self._expec
+00007300: 7461 7469 6f6e 5f73 7569 7465 203d 204e  tation_suite = N
+00007310: 6f6e 650a 0a20 2020 2064 6566 2067 6574  one..    def get
+00007320: 5f6c 6174 6573 745f 7661 6c69 6461 7469  _latest_validati
+00007330: 6f6e 5f72 6570 6f72 7428 0a20 2020 2020  on_report(.     
+00007340: 2020 2073 656c 662c 2067 655f 7479 7065     self, ge_type
+00007350: 3a20 626f 6f6c 203d 2054 7275 650a 2020  : bool = True.  
+00007360: 2020 2920 2d3e 2055 6e69 6f6e 5b56 616c    ) -> Union[Val
+00007370: 6964 6174 696f 6e52 6570 6f72 742c 2067  idationReport, g
+00007380: 652e 636f 7265 2e45 7870 6563 7461 7469  e.core.Expectati
+00007390: 6f6e 5375 6974 6556 616c 6964 6174 696f  onSuiteValidatio
+000073a0: 6e52 6573 756c 742c 204e 6f6e 655d 3a0a  nResult, None]:.
+000073b0: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+000073c0: 6e20 7468 6520 6c61 7465 7374 2076 616c  n the latest val
+000073d0: 6964 6174 696f 6e20 7265 706f 7274 2061  idation report a
+000073e0: 7474 6163 6865 6420 746f 2074 6865 2046  ttached to the F
+000073f0: 6561 7475 7265 2047 726f 7570 2069 6620  eature Group if 
+00007400: 6974 2065 7869 7374 732e 0a0a 2020 2020  it exists...    
+00007410: 2020 2020 2121 2120 6578 616d 706c 650a      !!! example.
+00007420: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
+00007430: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
+00007440: 2020 2320 636f 6e6e 6563 7420 746f 2074    # connect to t
+00007450: 6865 2046 6561 7475 7265 2053 746f 7265  he Feature Store
+00007460: 0a20 2020 2020 2020 2020 2020 2066 7320  .            fs 
+00007470: 3d20 2e2e 2e0a 0a20 2020 2020 2020 2020  = .....         
+00007480: 2020 2023 2067 6574 2074 6865 2046 6561     # get the Fea
+00007490: 7475 7265 2047 726f 7570 2069 6e73 7461  ture Group insta
+000074a0: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
+000074b0: 6667 203d 2066 732e 6765 745f 6f72 5f63  fg = fs.get_or_c
+000074c0: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
+000074d0: 6f75 7028 2e2e 2e29 0a0a 2020 2020 2020  oup(...)..      
+000074e0: 2020 2020 2020 6c61 7465 7374 5f76 616c        latest_val
+000074f0: 5f72 6570 6f72 7420 3d20 6667 2e67 6574  _report = fg.get
+00007500: 5f6c 6174 6573 745f 7661 6c69 6461 7469  _latest_validati
+00007510: 6f6e 5f72 6570 6f72 7428 290a 2020 2020  on_report().    
+00007520: 2020 2020 2020 2020 6060 600a 0a20 2020          ```..   
+00007530: 2020 2020 2023 2041 7267 756d 656e 7473       # Arguments
+00007540: 0a20 2020 2020 2020 2020 2020 2067 655f  .            ge_
+00007550: 7479 7065 3a20 4966 2060 5472 7565 6020  type: If `True` 
+00007560: 7265 7475 726e 7320 6120 6e61 7469 7665  returns a native
+00007570: 2047 7265 6174 2045 7870 6563 7461 7469   Great Expectati
+00007580: 6f6e 2074 7970 652c 2048 6f70 7377 6f72  on type, Hopswor
+00007590: 6b73 0a20 2020 2020 2020 2020 2020 2020  ks.             
+000075a0: 2020 2063 7573 746f 6d20 7479 7065 206f     custom type o
+000075b0: 7468 6572 7769 7365 2e20 436f 6e76 6572  therwise. Conver
+000075c0: 7369 6f6e 2063 616e 2062 6520 7065 7266  sion can be perf
+000075d0: 6f72 6d65 6420 7669 6120 7468 6520 6074  ormed via the `t
+000075e0: 6f5f 6765 5f74 7970 6528 2960 0a20 2020  o_ge_type()`.   
+000075f0: 2020 2020 2020 2020 2020 2020 206d 6574               met
+00007600: 686f 6420 6f6e 2068 6f70 7377 6f72 6b73  hod on hopsworks
+00007610: 2074 7970 652e 2044 6566 6175 6c74 7320   type. Defaults 
+00007620: 746f 2060 5472 7565 602e 0a0a 2020 2020  to `True`...    
+00007630: 2020 2020 2320 5265 7475 726e 730a 2020      # Returns.  
+00007640: 2020 2020 2020 2020 2020 6056 616c 6964            `Valid
+00007650: 6174 696f 6e52 6570 6f72 7460 2e20 5468  ationReport`. Th
+00007660: 6520 6c61 7465 7374 2076 616c 6964 6174  e latest validat
+00007670: 696f 6e20 7265 706f 7274 2061 7474 6163  ion report attac
+00007680: 6865 6420 746f 2074 6865 2046 6561 7475  hed to the Featu
+00007690: 7265 2047 726f 7570 2e0a 0a20 2020 2020  re Group...     
+000076a0: 2020 2023 2052 6169 7365 730a 2020 2020     # Raises.    
+000076b0: 2020 2020 2020 2020 6068 7366 732e 636c          `hsfs.cl
+000076c0: 6965 6e74 2e65 7863 6570 7469 6f6e 732e  ient.exceptions.
+000076d0: 5265 7374 4150 4945 7272 6f72 602e 0a20  RestAPIError`.. 
+000076e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000076f0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00007700: 7661 6c69 6461 7469 6f6e 5f72 6570 6f72  validation_repor
+00007710: 745f 656e 6769 6e65 2e67 6574 5f6c 6173  t_engine.get_las
+00007720: 7428 6765 5f74 7970 653d 6765 5f74 7970  t(ge_type=ge_typ
+00007730: 6529 0a0a 2020 2020 6465 6620 6765 745f  e)..    def get_
+00007740: 616c 6c5f 7661 6c69 6461 7469 6f6e 5f72  all_validation_r
+00007750: 6570 6f72 7473 280a 2020 2020 2020 2020  eports(.        
+00007760: 7365 6c66 2c20 6765 5f74 7970 653a 2062  self, ge_type: b
+00007770: 6f6f 6c20 3d20 5472 7565 0a20 2020 2029  ool = True.    )
+00007780: 202d 3e20 4c69 7374 5b55 6e69 6f6e 5b56   -> List[Union[V
+00007790: 616c 6964 6174 696f 6e52 6570 6f72 742c  alidationReport,
+000077a0: 2067 652e 636f 7265 2e45 7870 6563 7461   ge.core.Expecta
+000077b0: 7469 6f6e 5375 6974 6556 616c 6964 6174  tionSuiteValidat
+000077c0: 696f 6e52 6573 756c 745d 5d3a 0a20 2020  ionResult]]:.   
+000077d0: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
+000077e0: 6865 206c 6174 6573 7420 7661 6c69 6461  he latest valida
+000077f0: 7469 6f6e 2072 6570 6f72 7420 6174 7461  tion report atta
+00007800: 6368 6564 2074 6f20 7468 6520 6665 6174  ched to the feat
+00007810: 7572 6520 6772 6f75 7020 6966 2069 7420  ure group if it 
+00007820: 6578 6973 7473 2e0a 0a20 2020 2020 2020  exists...       
+00007830: 2021 2121 2065 7861 6d70 6c65 0a20 2020   !!! example.   
+00007840: 2020 2020 2020 2020 2060 6060 7079 7468           ```pyth
+00007850: 6f6e 0a20 2020 2020 2020 2020 2020 2023  on.            #
+00007860: 2063 6f6e 6e65 6374 2074 6f20 7468 6520   connect to the 
+00007870: 4665 6174 7572 6520 5374 6f72 650a 2020  Feature Store.  
+00007880: 2020 2020 2020 2020 2020 6673 203d 202e            fs = .
+00007890: 2e2e 0a0a 2020 2020 2020 2020 2020 2020  ....            
+000078a0: 2320 6765 7420 7468 6520 4665 6174 7572  # get the Featur
+000078b0: 6520 4772 6f75 7020 696e 7374 616e 6365  e Group instance
+000078c0: 0a20 2020 2020 2020 2020 2020 2066 6720  .            fg 
+000078d0: 3d20 6673 2e67 6574 5f6f 725f 6372 6561  = fs.get_or_crea
+000078e0: 7465 5f66 6561 7475 7265 5f67 726f 7570  te_feature_group
+000078f0: 282e 2e2e 290a 0a20 2020 2020 2020 2020  (...)..         
+00007900: 2020 2076 616c 5f72 6570 6f72 7473 203d     val_reports =
+00007910: 2066 672e 6765 745f 616c 6c5f 7661 6c69   fg.get_all_vali
+00007920: 6461 7469 6f6e 5f72 6570 6f72 7473 2829  dation_reports()
+00007930: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
+00007940: 0a0a 2020 2020 2020 2020 2320 4172 6775  ..        # Argu
+00007950: 6d65 6e74 730a 2020 2020 2020 2020 2020  ments.          
+00007960: 2020 6765 5f74 7970 653a 2049 6620 6054    ge_type: If `T
+00007970: 7275 6560 2072 6574 7572 6e73 2061 206e  rue` returns a n
+00007980: 6174 6976 6520 4772 6561 7420 4578 7065  ative Great Expe
+00007990: 6374 6174 696f 6e20 7479 7065 2c20 486f  ctation type, Ho
+000079a0: 7073 776f 726b 730a 2020 2020 2020 2020  psworks.        
+000079b0: 2020 2020 2020 2020 6375 7374 6f6d 2074          custom t
+000079c0: 7970 6520 6f74 6865 7277 6973 652e 2043  ype otherwise. C
+000079d0: 6f6e 7665 7273 696f 6e20 6361 6e20 6265  onversion can be
+000079e0: 2070 6572 666f 726d 6564 2076 6961 2074   performed via t
+000079f0: 6865 2060 746f 5f67 655f 7479 7065 2829  he `to_ge_type()
+00007a00: 600a 2020 2020 2020 2020 2020 2020 2020  `.              
+00007a10: 2020 6d65 7468 6f64 206f 6e20 686f 7073    method on hops
+00007a20: 776f 726b 7320 7479 7065 2e20 4465 6661  works type. Defa
+00007a30: 756c 7473 2074 6f20 6054 7275 6560 2e0a  ults to `True`..
+00007a40: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
+00007a50: 6e73 0a20 2020 2020 2020 2020 2020 2055  ns.            U
+00007a60: 6e69 6f6e 5b4c 6973 745b 6056 616c 6964  nion[List[`Valid
+00007a70: 6174 696f 6e52 6570 6f72 7460 5d2c 2060  ationReport`], `
+00007a80: 5661 6c69 6461 7469 6f6e 5265 706f 7274  ValidationReport
+00007a90: 605d 2e20 416c 6c20 7661 6c69 6461 7469  `]. All validati
+00007aa0: 6f6e 2072 6570 6f72 7473 2061 7474 6163  on reports attac
+00007ab0: 6865 6420 746f 2074 6865 2066 6561 7475  hed to the featu
+00007ac0: 7265 2067 726f 7570 2e0a 0a20 2020 2020  re group...     
+00007ad0: 2020 2023 2052 6169 7365 730a 2020 2020     # Raises.    
+00007ae0: 2020 2020 2020 2020 6068 7366 732e 636c          `hsfs.cl
+00007af0: 6965 6e74 2e65 7863 6570 7469 6f6e 732e  ient.exceptions.
+00007b00: 5265 7374 4150 4945 7272 6f72 602e 0a20  RestAPIError`.. 
+00007b10: 2020 2020 2020 2020 2020 2060 6873 6673             `hsfs
+00007b20: 2e63 6c69 656e 742e 6578 6365 7074 696f  .client.exceptio
+00007b30: 6e73 2e46 6561 7475 7265 5374 6f72 6545  ns.FeatureStoreE
+00007b40: 7863 6570 7469 6f6e 602e 0a20 2020 2020  xception`..     
+00007b50: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00007b60: 6620 7365 6c66 2e5f 6964 3a0a 2020 2020  f self._id:.    
+00007b70: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00007b80: 656c 662e 5f76 616c 6964 6174 696f 6e5f  elf._validation_
+00007b90: 7265 706f 7274 5f65 6e67 696e 652e 6765  report_engine.ge
+00007ba0: 745f 616c 6c28 6765 5f74 7970 653d 6765  t_all(ge_type=ge
+00007bb0: 5f74 7970 6529 0a20 2020 2020 2020 2065  _type).        e
+00007bc0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00007bd0: 2072 6169 7365 2046 6561 7475 7265 5374   raise FeatureSt
+00007be0: 6f72 6545 7863 6570 7469 6f6e 280a 2020  oreException(.  
+00007bf0: 2020 2020 2020 2020 2020 2020 2020 224f                "O
+00007c00: 6e6c 7920 4665 6174 7572 6520 4772 6f75  nly Feature Grou
+00007c10: 7020 7265 6769 7374 6572 6564 2077 6974  p registered wit
+00007c20: 6820 486f 7073 776f 726b 7320 6361 6e20  h Hopsworks can 
+00007c30: 6665 7463 6820 7661 6c69 6461 7469 6f6e  fetch validation
+00007c40: 2072 6570 6f72 7473 2e22 0a20 2020 2020   reports.".     
+00007c50: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00007c60: 6620 7361 7665 5f76 616c 6964 6174 696f  f save_validatio
+00007c70: 6e5f 7265 706f 7274 280a 2020 2020 2020  n_report(.      
+00007c80: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00007c90: 7661 6c69 6461 7469 6f6e 5f72 6570 6f72  validation_repor
+00007ca0: 743a 2055 6e69 6f6e 5b0a 2020 2020 2020  t: Union[.      
+00007cb0: 2020 2020 2020 6469 6374 2c0a 2020 2020        dict,.    
+00007cc0: 2020 2020 2020 2020 5661 6c69 6461 7469          Validati
+00007cd0: 6f6e 5265 706f 7274 2c0a 2020 2020 2020  onReport,.      
+00007ce0: 2020 2020 2020 6765 2e63 6f72 652e 6578        ge.core.ex
+00007cf0: 7065 6374 6174 696f 6e5f 7661 6c69 6461  pectation_valida
+00007d00: 7469 6f6e 5f72 6573 756c 742e 4578 7065  tion_result.Expe
+00007d10: 6374 6174 696f 6e53 7569 7465 5661 6c69  ctationSuiteVali
+00007d20: 6461 7469 6f6e 5265 7375 6c74 2c0a 2020  dationResult,.  
+00007d30: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00007d40: 2069 6e67 6573 7469 6f6e 5f72 6573 756c   ingestion_resul
+00007d50: 743a 2073 7472 203d 2022 554e 4b4e 4f57  t: str = "UNKNOW
+00007d60: 4e22 2c0a 2020 2020 2020 2020 6765 5f74  N",.        ge_t
+00007d70: 7970 653a 2062 6f6f 6c20 3d20 5472 7565  ype: bool = True
+00007d80: 2c0a 2020 2020 2920 2d3e 2055 6e69 6f6e  ,.    ) -> Union
+00007d90: 5b56 616c 6964 6174 696f 6e52 6570 6f72  [ValidationRepor
+00007da0: 742c 2067 652e 636f 7265 2e45 7870 6563  t, ge.core.Expec
+00007db0: 7461 7469 6f6e 5375 6974 6556 616c 6964  tationSuiteValid
+00007dc0: 6174 696f 6e52 6573 756c 745d 3a0a 2020  ationResult]:.  
+00007dd0: 2020 2020 2020 2222 2253 6176 6520 7661        """Save va
+00007de0: 6c69 6461 7469 6f6e 2072 6570 6f72 7420  lidation report 
+00007df0: 746f 2068 6f70 7377 6f72 6b73 2070 6c61  to hopsworks pla
+00007e00: 7466 6f72 6d20 616c 6f6e 6720 7072 6576  tform along prev
+00007e10: 696f 7573 2072 6570 6f72 7473 206f 6620  ious reports of 
+00007e20: 7468 6520 7361 6d65 2046 6561 7475 7265  the same Feature
+00007e30: 2047 726f 7570 2e0a 0a20 2020 2020 2020   Group...       
+00007e40: 2021 2121 2065 7861 6d70 6c65 0a20 2020   !!! example.   
+00007e50: 2020 2020 2020 2020 2060 6060 7079 7468           ```pyth
+00007e60: 6f6e 0a20 2020 2020 2020 2020 2020 2023  on.            #
+00007e70: 2063 6f6e 6e65 6374 2074 6f20 7468 6520   connect to the 
+00007e80: 4665 6174 7572 6520 5374 6f72 650a 2020  Feature Store.  
+00007e90: 2020 2020 2020 2020 2020 6673 203d 202e            fs = .
+00007ea0: 2e2e 0a0a 2020 2020 2020 2020 2020 2020  ....            
+00007eb0: 2320 6765 7420 7468 6520 4665 6174 7572  # get the Featur
+00007ec0: 6520 4772 6f75 7020 696e 7374 616e 6365  e Group instance
+00007ed0: 0a20 2020 2020 2020 2020 2020 2066 6720  .            fg 
+00007ee0: 3d20 6673 2e67 6574 5f6f 725f 6372 6561  = fs.get_or_crea
+00007ef0: 7465 5f66 6561 7475 7265 5f67 726f 7570  te_feature_group
+00007f00: 282e 2e2e 2c20 6578 7065 6374 6174 696f  (..., expectatio
+00007f10: 6e5f 7375 6974 653d 6578 7065 6374 6174  n_suite=expectat
+00007f20: 696f 6e5f 7375 6974 6529 0a0a 2020 2020  ion_suite)..    
+00007f30: 2020 2020 2020 2020 7661 6c69 6461 7469          validati
+00007f40: 6f6e 5f72 6570 6f72 7420 3d20 6772 6561  on_report = grea
+00007f50: 745f 6578 7065 6374 6174 696f 6e73 2e66  t_expectations.f
+00007f60: 726f 6d5f 7061 6e64 6173 280a 2020 2020  rom_pandas(.    
+00007f70: 2020 2020 2020 2020 2020 2020 6d79 5f65              my_e
+00007f80: 7870 6572 696d 656e 7461 6c5f 6665 6174  xperimental_feat
+00007f90: 7572 6573 5f64 662c 0a20 2020 2020 2020  ures_df,.       
+00007fa0: 2020 2020 2020 2020 2066 672e 6765 745f           fg.get_
+00007fb0: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
+00007fc0: 6528 2929 2e76 616c 6964 6174 6528 290a  e()).validate().
+00007fd0: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
+00007fe0: 7361 7665 5f76 616c 6964 6174 696f 6e5f  save_validation_
+00007ff0: 7265 706f 7274 2876 616c 6964 6174 696f  report(validatio
+00008000: 6e5f 7265 706f 7274 2c20 696e 6765 7374  n_report, ingest
+00008010: 696f 6e5f 7265 7375 6c74 3d22 4558 5045  ion_result="EXPE
+00008020: 5249 4d45 4e54 2229 0a20 2020 2020 2020  RIMENT").       
+00008030: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
+00008040: 2020 2320 4172 6775 6d65 6e74 730a 2020    # Arguments.  
+00008050: 2020 2020 2020 2020 2020 7661 6c69 6461            valida
+00008060: 7469 6f6e 5f72 6570 6f72 743a 2054 6865  tion_report: The
+00008070: 2076 616c 6964 6174 696f 6e20 7265 706f   validation repo
+00008080: 7274 2074 6f20 6174 7461 6368 2074 6f20  rt to attach to 
+00008090: 7468 6520 4665 6174 7572 6520 4772 6f75  the Feature Grou
+000080a0: 702e 0a20 2020 2020 2020 2020 2020 2069  p..            i
+000080b0: 6e67 6573 7469 6f6e 5f72 6573 756c 743a  ngestion_result:
+000080c0: 2053 7065 6369 6679 2074 6865 2066 6174   Specify the fat
+000080d0: 6520 6f66 2074 6865 2061 7373 6f63 6961  e of the associa
+000080e0: 7465 6420 6461 7461 2c20 6465 6661 756c  ted data, defaul
+000080f0: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
+00008100: 2020 2074 6f20 2255 4e4b 4e4f 574e 222e     to "UNKNOWN".
+00008110: 2053 7570 706f 7274 6564 206f 7074 696f   Supported optio
+00008120: 6e73 2061 7265 2020 2255 4e4b 4e4f 574e  ns are  "UNKNOWN
+00008130: 222c 2022 494e 4745 5354 4544 222c 2022  ", "INGESTED", "
+00008140: 5245 4a45 4354 4544 222c 0a20 2020 2020  REJECTED",.     
+00008150: 2020 2020 2020 2020 2020 2022 4558 5045             "EXPE
+00008160: 5249 4d45 4e54 222c 2022 4647 5f44 4154  RIMENT", "FG_DAT
+00008170: 4122 2e20 5573 6520 2249 4e47 4553 5445  A". Use "INGESTE
+00008180: 4422 206f 7220 2252 454a 4543 5445 4422  D" or "REJECTED"
+00008190: 2066 6f72 2076 616c 6964 6174 696f 6e0a   for validation.
+000081a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081b0: 6f66 2044 6174 6146 7261 6d65 7320 746f  of DataFrames to
+000081c0: 2062 6520 696e 7365 7274 6564 2069 6e20   be inserted in 
+000081d0: 7468 6520 4665 6174 7572 6520 4772 6f75  the Feature Grou
+000081e0: 702e 2055 7365 2022 4558 5045 5249 4d45  p. Use "EXPERIME
+000081f0: 4e54 220a 2020 2020 2020 2020 2020 2020  NT".            
+00008200: 2020 2020 666f 7220 7465 7374 696e 6720      for testing 
+00008210: 616e 6420 6465 7665 6c6f 706d 656e 7420  and development 
+00008220: 616e 6420 2246 475f 4441 5441 2220 7768  and "FG_DATA" wh
+00008230: 656e 2076 616c 6964 6174 696e 6720 6461  en validating da
+00008240: 7461 0a20 2020 2020 2020 2020 2020 2020  ta.             
+00008250: 2020 2061 6c72 6561 6479 2069 6e20 7468     already in th
+00008260: 6520 4665 6174 7572 6520 4772 6f75 702e  e Feature Group.
+00008270: 0a20 2020 2020 2020 2020 2020 2067 655f  .            ge_
+00008280: 7479 7065 3a20 4966 2060 5472 7565 6020  type: If `True` 
+00008290: 7265 7475 726e 7320 6120 6e61 7469 7665  returns a native
+000082a0: 2047 7265 6174 2045 7870 6563 7461 7469   Great Expectati
+000082b0: 6f6e 2074 7970 652c 2048 6f70 7377 6f72  on type, Hopswor
+000082c0: 6b73 0a20 2020 2020 2020 2020 2020 2020  ks.             
+000082d0: 2020 2063 7573 746f 6d20 7479 7065 206f     custom type o
+000082e0: 7468 6572 7769 7365 2e20 436f 6e76 6572  therwise. Conver
+000082f0: 7369 6f6e 2063 616e 2062 6520 7065 7266  sion can be perf
+00008300: 6f72 6d65 6420 7669 6120 7468 6520 6074  ormed via the `t
+00008310: 6f5f 6765 5f74 7970 6528 2960 0a20 2020  o_ge_type()`.   
+00008320: 2020 2020 2020 2020 2020 2020 206d 6574               met
+00008330: 686f 6420 6f6e 2068 6f70 7377 6f72 6b73  hod on hopsworks
+00008340: 2074 7970 652e 2044 6566 6175 6c74 7320   type. Defaults 
+00008350: 746f 2060 5472 7565 602e 0a0a 2020 2020  to `True`...    
+00008360: 2020 2020 2320 5261 6973 6573 0a20 2020      # Raises.   
+00008370: 2020 2020 2020 2020 2060 6873 6673 2e63           `hsfs.c
+00008380: 6c69 656e 742e 6578 6365 7074 696f 6e73  lient.exceptions
+00008390: 2e52 6573 7441 5049 4572 726f 7260 2e0a  .RestAPIError`..
+000083a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000083b0: 2020 2020 6966 2073 656c 662e 5f69 643a      if self._id:
+000083c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000083d0: 6973 696e 7374 616e 6365 280a 2020 2020  isinstance(.    
+000083e0: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
+000083f0: 6461 7469 6f6e 5f72 6570 6f72 742c 0a20  dation_report,. 
+00008400: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00008410: 652e 636f 7265 2e65 7870 6563 7461 7469  e.core.expectati
+00008420: 6f6e 5f76 616c 6964 6174 696f 6e5f 7265  on_validation_re
+00008430: 7375 6c74 2e45 7870 6563 7461 7469 6f6e  sult.Expectation
+00008440: 5375 6974 6556 616c 6964 6174 696f 6e52  SuiteValidationR
+00008450: 6573 756c 742c 0a20 2020 2020 2020 2020  esult,.         
+00008460: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00008470: 2020 2020 2020 7265 706f 7274 203d 2056        report = V
+00008480: 616c 6964 6174 696f 6e52 6570 6f72 7428  alidationReport(
+00008490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000084a0: 2020 2020 202a 2a76 616c 6964 6174 696f       **validatio
+000084b0: 6e5f 7265 706f 7274 2e74 6f5f 6a73 6f6e  n_report.to_json
+000084c0: 5f64 6963 7428 292c 0a20 2020 2020 2020  _dict(),.       
+000084d0: 2020 2020 2020 2020 2020 2020 2069 6e67               ing
+000084e0: 6573 7469 6f6e 5f72 6573 756c 743d 696e  estion_result=in
+000084f0: 6765 7374 696f 6e5f 7265 7375 6c74 2c0a  gestion_result,.
+00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008510: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00008520: 6966 2069 7369 6e73 7461 6e63 6528 7661  if isinstance(va
+00008530: 6c69 6461 7469 6f6e 5f72 6570 6f72 742c  lidation_report,
+00008540: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
+00008550: 2020 2020 2020 2020 7265 706f 7274 203d          report =
+00008560: 2056 616c 6964 6174 696f 6e52 6570 6f72   ValidationRepor
+00008570: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00008580: 2020 2020 2020 202a 2a76 616c 6964 6174         **validat
+00008590: 696f 6e5f 7265 706f 7274 2c20 696e 6765  ion_report, inge
+000085a0: 7374 696f 6e5f 7265 7375 6c74 3d69 6e67  stion_result=ing
+000085b0: 6573 7469 6f6e 5f72 6573 756c 740a 2020  estion_result.  
+000085c0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000085d0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+000085e0: 2069 7369 6e73 7461 6e63 6528 7661 6c69   isinstance(vali
+000085f0: 6461 7469 6f6e 5f72 6570 6f72 742c 2056  dation_report, V
+00008600: 616c 6964 6174 696f 6e52 6570 6f72 7429  alidationReport)
+00008610: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00008620: 2020 7265 706f 7274 203d 2076 616c 6964    report = valid
+00008630: 6174 696f 6e5f 7265 706f 7274 0a20 2020  ation_report.   
+00008640: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00008650: 696e 6765 7374 696f 6e5f 7265 7375 6c74  ingestion_result
+00008660: 2021 3d20 2255 4e4b 4e4f 574e 223a 0a20   != "UNKNOWN":. 
+00008670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008680: 2020 2072 6570 6f72 742e 696e 6765 7374     report.ingest
+00008690: 696f 6e5f 7265 7375 6c74 203d 2069 6e67  ion_result = ing
+000086a0: 6573 7469 6f6e 5f72 6573 756c 740a 0a20  estion_result.. 
+000086b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000086c0: 6e20 7365 6c66 2e5f 7661 6c69 6461 7469  n self._validati
+000086d0: 6f6e 5f72 6570 6f72 745f 656e 6769 6e65  on_report_engine
+000086e0: 2e73 6176 6528 0a20 2020 2020 2020 2020  .save(.         
+000086f0: 2020 2020 2020 2076 616c 6964 6174 696f         validatio
+00008700: 6e5f 7265 706f 7274 3d72 6570 6f72 742c  n_report=report,
+00008710: 2067 655f 7479 7065 3d67 655f 7479 7065   ge_type=ge_type
+00008720: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00008730: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00008740: 2020 2020 2020 2020 2072 6169 7365 2046           raise F
+00008750: 6561 7475 7265 5374 6f72 6545 7863 6570  eatureStoreExcep
+00008760: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+00008770: 2020 2020 2020 224f 6e6c 7920 4665 6174        "Only Feat
+00008780: 7572 6520 4772 6f75 7020 7265 6769 7374  ure Group regist
+00008790: 6572 6564 2077 6974 6820 486f 7073 776f  ered with Hopswo
+000087a0: 726b 7320 6361 6e20 7570 6c6f 6164 2076  rks can upload v
+000087b0: 616c 6964 6174 696f 6e20 7265 706f 7274  alidation report
+000087c0: 732e 220a 2020 2020 2020 2020 2020 2020  s.".            
+000087d0: 290a 0a20 2020 2064 6566 2067 6574 5f76  )..    def get_v
+000087e0: 616c 6964 6174 696f 6e5f 6869 7374 6f72  alidation_histor
+000087f0: 7928 0a20 2020 2020 2020 2073 656c 662c  y(.        self,
+00008800: 0a20 2020 2020 2020 2065 7870 6563 7461  .        expecta
+00008810: 7469 6f6e 5f69 643a 2069 6e74 2c0a 2020  tion_id: int,.  
+00008820: 2020 2020 2020 7374 6172 745f 7661 6c69        start_vali
+00008830: 6461 7469 6f6e 5f74 696d 653a 2055 6e69  dation_time: Uni
+00008840: 6f6e 5b73 7472 2c20 696e 742c 2064 6174  on[str, int, dat
+00008850: 6574 696d 652c 2064 6174 652c 204e 6f6e  etime, date, Non
+00008860: 655d 203d 204e 6f6e 652c 0a20 2020 2020  e] = None,.     
+00008870: 2020 2065 6e64 5f76 616c 6964 6174 696f     end_validatio
+00008880: 6e5f 7469 6d65 3a20 556e 696f 6e5b 7374  n_time: Union[st
+00008890: 722c 2069 6e74 2c20 6461 7465 7469 6d65  r, int, datetime
+000088a0: 2c20 6461 7465 2c20 4e6f 6e65 5d20 3d20  , date, None] = 
+000088b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6669  None,.        fi
+000088c0: 6c74 6572 5f62 793a 204c 6973 745b 7374  lter_by: List[st
+000088d0: 725d 203d 205b 5d2c 0a20 2020 2020 2020  r] = [],.       
+000088e0: 2067 655f 7479 7065 3a20 626f 6f6c 203d   ge_type: bool =
+000088f0: 2054 7275 652c 0a20 2020 2029 202d 3e20   True,.    ) -> 
+00008900: 556e 696f 6e5b 4c69 7374 5b56 616c 6964  Union[List[Valid
+00008910: 6174 696f 6e52 6573 756c 745d 2c20 4c69  ationResult], Li
+00008920: 7374 5b67 652e 636f 7265 2e45 7870 6563  st[ge.core.Expec
+00008930: 7461 7469 6f6e 5661 6c69 6461 7469 6f6e  tationValidation
+00008940: 5265 7375 6c74 5d5d 3a0a 2020 2020 2020  Result]]:.      
+00008950: 2020 2222 2246 6574 6368 2076 616c 6964    """Fetch valid
+00008960: 6174 696f 6e20 6869 7374 6f72 7920 6f66  ation history of
+00008970: 2061 6e20 4578 7065 6374 6174 696f 6e20   an Expectation 
+00008980: 7370 6563 6966 6965 6420 6279 2069 7473  specified by its
+00008990: 2069 642e 0a0a 2020 2020 2020 2020 2121   id...        !!
+000089a0: 2120 6578 616d 706c 650a 2020 2020 2020  ! example.      
+000089b0: 2020 6060 6070 7974 686f 6e33 0a20 2020    ```python3.   
+000089c0: 2020 2020 2076 616c 6964 6174 696f 6e5f       validation_
+000089d0: 6869 7374 6f72 7920 3d20 6667 2e67 6574  history = fg.get
+000089e0: 5f76 616c 6964 6174 696f 6e5f 6869 7374  _validation_hist
+000089f0: 6f72 7928 0a20 2020 2020 2020 2020 2020  ory(.           
+00008a00: 2065 7870 6563 7461 7469 6f6e 5f69 643d   expectation_id=
+00008a10: 312c 0a20 2020 2020 2020 2020 2020 2066  1,.            f
+00008a20: 696c 7465 725f 6279 3d5b 2252 454a 4543  ilter_by=["REJEC
+00008a30: 5445 4422 2c20 2255 4e4b 4e4f 574e 225d  TED", "UNKNOWN"]
+00008a40: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
+00008a50: 6172 745f 7661 6c69 6461 7469 6f6e 5f74  art_validation_t
+00008a60: 696d 653d 2232 3032 322d 3031 2d30 3120  ime="2022-01-01 
+00008a70: 3030 3a30 303a 3030 222c 0a20 2020 2020  00:00:00",.     
+00008a80: 2020 2020 2020 2065 6e64 5f76 616c 6964         end_valid
+00008a90: 6174 696f 6e5f 7469 6d65 3d64 6174 6574  ation_time=datet
+00008aa0: 696d 652e 6461 7465 7469 6d65 2e6e 6f77  ime.datetime.now
+00008ab0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+00008ac0: 6765 5f74 7970 653d 4661 6c73 650a 2020  ge_type=False.  
+00008ad0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00008ae0: 6060 600a 0a20 2020 2020 2020 2023 2041  ```..        # A
+00008af0: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
+00008b00: 2020 2020 2065 7870 6563 7461 7469 6f6e       expectation
+00008b10: 5f69 643a 2069 6420 6f66 2074 6865 2045  _id: id of the E
+00008b20: 7870 6563 7461 7469 6f6e 2066 6f72 2077  xpectation for w
+00008b30: 6869 6368 2074 6f20 6665 7463 6820 7468  hich to fetch th
+00008b40: 6520 7661 6c69 6461 7469 6f6e 2068 6973  e validation his
+00008b50: 746f 7279 0a20 2020 2020 2020 2020 2020  tory.           
+00008b60: 2066 696c 7465 725f 6279 3a20 6c69 7374   filter_by: list
+00008b70: 206f 6620 696e 6765 7374 696f 6e5f 7265   of ingestion_re
+00008b80: 7375 6c74 2063 6174 6567 6f72 7920 746f  sult category to
+00008b90: 206b 6565 702e 204f 6f70 7469 6f6e 7320   keep. Ooptions 
+00008ba0: 6172 6520 2249 4e47 4553 5445 4422 2c20  are "INGESTED", 
+00008bb0: 2252 454a 4543 5445 4422 2c20 2246 475f  "REJECTED", "FG_
+00008bc0: 4441 5441 222c 2022 4558 5045 5249 4d45  DATA", "EXPERIME
+00008bd0: 4e54 222c 2022 554e 4b4e 4f57 4e22 2e0a  NT", "UNKNOWN"..
+00008be0: 2020 2020 2020 2020 2020 2020 7374 6172              star
+00008bf0: 745f 7661 6c69 6461 7469 6f6e 5f74 696d  t_validation_tim
+00008c00: 653a 2066 6574 6368 206f 6e6c 7920 7661  e: fetch only va
+00008c10: 6c69 6461 7469 6f6e 2072 6573 756c 7420  lidation result 
+00008c20: 706f 7374 6572 696f 7220 746f 2074 6865  posterior to the
+00008c30: 2070 726f 7669 6465 6420 7469 6d65 2c20   provided time, 
+00008c40: 696e 636c 7573 6976 652e 0a20 2020 2020  inclusive..     
+00008c50: 2020 2020 2020 2053 7570 706f 7274 6564         Supported
+00008c60: 2066 6f72 6d61 7420 696e 636c 7564 6520   format include 
+00008c70: 7469 6d65 7374 616d 7073 2869 6e74 292c  timestamps(int),
+00008c80: 2064 6174 6574 696d 652c 2064 6174 6520   datetime, date 
+00008c90: 6f72 2073 7472 696e 6720 666f 726d 6174  or string format
+00008ca0: 7465 6420 746f 2062 6520 6461 7475 7469  ted to be datuti
+00008cb0: 6c73 2070 6172 7361 626c 652e 2053 6565  ls parsable. See
+00008cc0: 2065 7861 6d70 6c65 7320 6162 6f76 652e   examples above.
+00008cd0: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
+00008ce0: 5f76 616c 6964 6174 696f 6e5f 7469 6d65  _validation_time
+00008cf0: 3a20 6665 7463 6820 6f6e 6c79 2076 616c  : fetch only val
+00008d00: 6964 6174 696f 6e20 7265 7375 6c74 2070  idation result p
+00008d10: 7269 6f72 2074 6f20 7468 6520 7072 6f76  rior to the prov
+00008d20: 6964 6564 2074 696d 652c 2069 6e63 6c75  ided time, inclu
+00008d30: 7369 7665 2e0a 2020 2020 2020 2020 2020  sive..          
+00008d40: 2020 5375 7070 6f72 7465 6420 666f 726d    Supported form
+00008d50: 6174 2069 6e63 6c75 6465 2074 696d 6573  at include times
+00008d60: 7461 6d70 7328 696e 7429 2c20 6461 7465  tamps(int), date
+00008d70: 7469 6d65 2c20 6461 7465 206f 7220 7374  time, date or st
+00008d80: 7269 6e67 2066 6f72 6d61 7474 6564 2074  ring formatted t
+00008d90: 6f20 6265 2064 6174 7574 696c 7320 7061  o be datutils pa
+00008da0: 7273 6162 6c65 2e20 5365 6520 6578 616d  rsable. See exam
+00008db0: 706c 6573 2061 626f 7665 2e0a 0a20 2020  ples above...   
+00008dc0: 2020 2020 2023 2052 6169 7365 730a 2020       # Raises.  
+00008dd0: 2020 2020 2020 2020 2020 6068 7366 732e            `hsfs.
+00008de0: 636c 6965 6e74 2e65 7863 6570 7469 6f6e  client.exception
+00008df0: 732e 5265 7374 4150 4945 7272 6f72 602e  s.RestAPIError`.
+00008e00: 0a0a 2020 2020 2020 2020 2320 5265 7475  ..        # Retu
+00008e10: 726e 0a20 2020 2020 2020 2020 2020 2055  rn.            U
+00008e20: 6e69 6f6e 5b4c 6973 745b 6056 616c 6964  nion[List[`Valid
+00008e30: 6174 696f 6e52 6573 756c 7460 5d2c 204c  ationResult`], L
+00008e40: 6973 745b 6045 7870 6563 7461 7469 6f6e  ist[`Expectation
+00008e50: 5661 6c69 6461 7469 6f6e 5265 7375 6c74  ValidationResult
+00008e60: 605d 5d20 4120 6c69 7374 206f 6620 7661  `]] A list of va
+00008e70: 6c69 6461 7469 6f6e 2072 6573 756c 7420  lidation result 
+00008e80: 636f 6e6e 6563 7465 6420 746f 2074 6865  connected to the
+00008e90: 2065 7870 6563 7461 7469 6f6e 5f69 640a   expectation_id.
+00008ea0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00008eb0: 2020 2020 6d61 6a6f 722c 206d 696e 6f72      major, minor
+00008ec0: 203d 2073 656c 662e 5f76 6172 6961 626c   = self._variabl
+00008ed0: 655f 6170 692e 7061 7273 655f 6d61 6a6f  e_api.parse_majo
+00008ee0: 725f 616e 645f 6d69 6e6f 7228 0a20 2020  r_and_minor(.   
+00008ef0: 2020 2020 2020 2020 2073 656c 662e 5f76           self._v
+00008f00: 6172 6961 626c 655f 6170 692e 6765 745f  ariable_api.get_
+00008f10: 7665 7273 696f 6e28 2268 6f70 7377 6f72  version("hopswor
+00008f20: 6b73 2229 0a20 2020 2020 2020 2029 0a20  ks").        ). 
+00008f30: 2020 2020 2020 2069 6620 6d61 6a6f 7220         if major 
+00008f40: 3d3d 2022 3322 2061 6e64 206d 696e 6f72  == "3" and minor
+00008f50: 203d 3d20 2230 223a 0a20 2020 2020 2020   == "0":.       
+00008f60: 2020 2020 2072 6169 7365 2046 6561 7475       raise Featu
+00008f70: 7265 5374 6f72 6545 7863 6570 7469 6f6e  reStoreException
+00008f80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00008f90: 2020 2254 6865 2068 6f70 7377 6f72 6b73    "The hopsworks
+00008fa0: 2073 6572 7665 7220 646f 6573 206e 6f74   server does not
+00008fb0: 2073 7570 706f 7274 2074 6869 7320 6f70   support this op
+00008fc0: 6572 6174 696f 6e2e 2055 7064 6174 6520  eration. Update 
+00008fd0: 7365 7276 6572 2074 6f20 686f 7073 776f  server to hopswo
+00008fe0: 726b 7320 3e33 2e31 2074 6f20 656e 6162  rks >3.1 to enab
+00008ff0: 6c65 2073 7570 706f 7274 2e22 0a20 2020  le support.".   
+00009000: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00009010: 2020 2020 6966 2073 656c 662e 5f69 643a      if self._id:
+00009020: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00009030: 7572 6e20 7365 6c66 2e5f 7661 6c69 6461  urn self._valida
+00009040: 7469 6f6e 5f72 6573 756c 745f 656e 6769  tion_result_engi
+00009050: 6e65 2e67 6574 5f76 616c 6964 6174 696f  ne.get_validatio
+00009060: 6e5f 6869 7374 6f72 7928 0a20 2020 2020  n_history(.     
+00009070: 2020 2020 2020 2020 2020 2065 7870 6563             expec
+00009080: 7461 7469 6f6e 5f69 643d 6578 7065 6374  tation_id=expect
+00009090: 6174 696f 6e5f 6964 2c0a 2020 2020 2020  ation_id,.      
+000090a0: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+000090b0: 7661 6c69 6461 7469 6f6e 5f74 696d 653d  validation_time=
+000090c0: 7374 6172 745f 7661 6c69 6461 7469 6f6e  start_validation
+000090d0: 5f74 696d 652c 0a20 2020 2020 2020 2020  _time,.         
+000090e0: 2020 2020 2020 2065 6e64 5f76 616c 6964         end_valid
+000090f0: 6174 696f 6e5f 7469 6d65 3d65 6e64 5f76  ation_time=end_v
+00009100: 616c 6964 6174 696f 6e5f 7469 6d65 2c0a  alidation_time,.
+00009110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009120: 6669 6c74 6572 5f62 793d 6669 6c74 6572  filter_by=filter
+00009130: 5f62 792c 0a20 2020 2020 2020 2020 2020  _by,.           
+00009140: 2020 2020 2067 655f 7479 7065 3d67 655f       ge_type=ge_
+00009150: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
+00009160: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
+00009170: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00009180: 6973 6520 4665 6174 7572 6553 746f 7265  ise FeatureStore
+00009190: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
+000091a0: 2020 2020 2020 2020 2020 2022 4f6e 6c79             "Only
+000091b0: 2046 6561 7475 7265 2047 726f 7570 2072   Feature Group r
+000091c0: 6567 6973 7465 7265 6420 7769 7468 2048  egistered with H
+000091d0: 6f70 7377 6f72 6b73 2063 616e 2066 6574  opsworks can fet
+000091e0: 6368 2076 616c 6964 6174 696f 6e20 6869  ch validation hi
+000091f0: 7374 6f72 792e 220a 2020 2020 2020 2020  story.".        
+00009200: 2020 2020 290a 0a20 2020 2064 6566 2076      )..    def v
+00009210: 616c 6964 6174 6528 0a20 2020 2020 2020  alidate(.       
+00009220: 2073 656c 662c 0a20 2020 2020 2020 2064   self,.        d
+00009230: 6174 6166 7261 6d65 3a20 4f70 7469 6f6e  ataframe: Option
+00009240: 616c 5b0a 2020 2020 2020 2020 2020 2020  al[.            
+00009250: 556e 696f 6e5b 7064 2e44 6174 6146 7261  Union[pd.DataFra
+00009260: 6d65 2c20 5479 7065 5661 7228 2270 7973  me, TypeVar("pys
+00009270: 7061 726b 2e73 716c 2e44 6174 6146 7261  park.sql.DataFra
+00009280: 6d65 2229 5d20 2023 206e 6f71 613a 2046  me")]  # noqa: F
+00009290: 3832 310a 2020 2020 2020 2020 5d20 3d20  821.        ] = 
+000092a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6578  None,.        ex
+000092b0: 7065 6374 6174 696f 6e5f 7375 6974 653a  pectation_suite:
+000092c0: 204f 7074 696f 6e61 6c5b 4578 7065 6374   Optional[Expect
+000092d0: 6174 696f 6e53 7569 7465 5d20 3d20 4e6f  ationSuite] = No
+000092e0: 6e65 2c0a 2020 2020 2020 2020 7361 7665  ne,.        save
+000092f0: 5f72 6570 6f72 743a 204f 7074 696f 6e61  _report: Optiona
+00009300: 6c5b 626f 6f6c 5d20 3d20 4661 6c73 652c  l[bool] = False,
+00009310: 0a20 2020 2020 2020 2076 616c 6964 6174  .        validat
+00009320: 696f 6e5f 6f70 7469 6f6e 733a 204f 7074  ion_options: Opt
+00009330: 696f 6e61 6c5b 4469 6374 5b41 6e79 2c20  ional[Dict[Any, 
+00009340: 416e 795d 5d20 3d20 7b7d 2c0a 2020 2020  Any]] = {},.    
+00009350: 2020 2020 696e 6765 7374 696f 6e5f 7265      ingestion_re
+00009360: 7375 6c74 3a20 7374 7220 3d20 2255 4e4b  sult: str = "UNK
+00009370: 4e4f 574e 222c 0a20 2020 2020 2020 2067  NOWN",.        g
+00009380: 655f 7479 7065 3a20 626f 6f6c 203d 2054  e_type: bool = T
+00009390: 7275 652c 0a20 2020 2029 202d 3e20 556e  rue,.    ) -> Un
+000093a0: 696f 6e5b 6765 2e63 6f72 652e 4578 7065  ion[ge.core.Expe
+000093b0: 6374 6174 696f 6e53 7569 7465 5661 6c69  ctationSuiteVali
+000093c0: 6461 7469 6f6e 5265 7375 6c74 2c20 5661  dationResult, Va
+000093d0: 6c69 6461 7469 6f6e 5265 706f 7274 2c20  lidationReport, 
+000093e0: 4e6f 6e65 5d3a 0a20 2020 2020 2020 2022  None]:.        "
+000093f0: 2222 5275 6e20 7661 6c69 6461 7469 6f6e  ""Run validation
+00009400: 2062 6173 6564 206f 6e20 7468 6520 6174   based on the at
+00009410: 7461 6368 6564 2065 7870 6563 7461 7469  tached expectati
+00009420: 6f6e 732e 0a0a 2020 2020 2020 2020 5275  ons...        Ru
+00009430: 6e73 2061 6e79 2065 7870 6563 7461 7469  ns any expectati
+00009440: 6f6e 2061 7474 6163 6865 6420 7769 7468  on attached with
+00009450: 2044 6565 7175 2e20 4275 7420 616c 736f   Deequ. But also
+00009460: 2072 756e 7320 6174 7461 6368 6564 2047   runs attached G
+00009470: 7265 6174 2045 7870 6563 7461 7469 6f6e  reat Expectation
+00009480: 0a20 2020 2020 2020 2053 7569 7465 732e  .        Suites.
+00009490: 0a0a 2020 2020 2020 2020 2121 2120 6578  ..        !!! ex
+000094a0: 616d 706c 650a 2020 2020 2020 2020 2020  ample.          
+000094b0: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
+000094c0: 2020 2020 2020 2020 2320 636f 6e6e 6563          # connec
+000094d0: 7420 746f 2074 6865 2046 6561 7475 7265  t to the Feature
+000094e0: 2053 746f 7265 0a20 2020 2020 2020 2020   Store.         
+000094f0: 2020 2066 7320 3d20 2e2e 2e0a 0a20 2020     fs = .....   
+00009500: 2020 2020 2020 2020 2023 2067 6574 2066           # get f
+00009510: 6561 7475 7265 2067 726f 7570 2069 6e73  eature group ins
+00009520: 7461 6e63 650a 2020 2020 2020 2020 2020  tance.          
+00009530: 2020 6667 203d 2066 732e 6765 745f 6f72    fg = fs.get_or
+00009540: 5f63 7265 6174 655f 6665 6174 7572 655f  _create_feature_
+00009550: 6772 6f75 7028 2e2e 2e29 0a0a 2020 2020  group(...)..    
+00009560: 2020 2020 2020 2020 6765 5f72 6570 6f72          ge_repor
+00009570: 7420 3d20 6667 2e76 616c 6964 6174 6528  t = fg.validate(
+00009580: 6466 2c20 7361 7665 5f72 6570 6f72 743d  df, save_report=
+00009590: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+000095a0: 2020 2060 6060 0a0a 2020 2020 2020 2020     ```..        
+000095b0: 2320 4172 6775 6d65 6e74 730a 2020 2020  # Arguments.    
+000095c0: 2020 2020 2020 2020 6461 7461 6672 616d          datafram
+000095d0: 653a 2054 6865 2064 6174 6166 7261 6d65  e: The dataframe
+000095e0: 2074 6f20 7275 6e20 7468 6520 6461 7461   to run the data
+000095f0: 2076 616c 6964 6174 696f 6e20 6578 7065   validation expe
+00009600: 6374 6174 696f 6e73 2061 6761 696e 7374  ctations against
+00009610: 2e0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+00009620: 7065 6374 6174 696f 6e5f 7375 6974 653a  pectation_suite:
+00009630: 204f 7074 696f 6e61 6c6c 7920 7072 6f76   Optionally prov
+00009640: 6964 6520 616e 2045 7870 6563 7461 7469  ide an Expectati
+00009650: 6f6e 2053 7569 7465 2074 6f20 6f76 6572  on Suite to over
+00009660: 7269 6465 2074 6865 0a20 2020 2020 2020  ride the.       
+00009670: 2020 2020 2020 2020 206f 6e65 2074 6861           one tha
+00009680: 7420 6973 2070 6f73 7369 626c 7920 6174  t is possibly at
+00009690: 7461 6368 6564 2074 6f20 7468 6520 6665  tached to the fe
+000096a0: 6174 7572 6520 6772 6f75 702e 2054 6869  ature group. Thi
+000096b0: 7320 6973 2075 7365 6675 6c20 666f 720a  s is useful for.
+000096c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096d0: 7465 7374 696e 6720 6e65 7720 4578 7065  testing new Expe
+000096e0: 6374 6174 696f 6e20 7375 6974 6573 2e20  ctation suites. 
+000096f0: 5768 656e 2061 6e20 6578 7472 6120 7375  When an extra su
+00009700: 6974 6520 6973 2070 726f 7669 6465 642c  ite is provided,
+00009710: 2074 6865 2072 6573 756c 7473 0a20 2020   the results.   
+00009720: 2020 2020 2020 2020 2020 2020 2077 696c               wil
+00009730: 6c20 6e65 7665 7220 6265 2070 6572 7369  l never be persi
+00009740: 7374 6564 2e20 4465 6661 756c 7473 2074  sted. Defaults t
+00009750: 6f20 604e 6f6e 6560 2e0a 2020 2020 2020  o `None`..      
+00009760: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
+00009770: 5f6f 7074 696f 6e73 3a20 4164 6469 7469  _options: Additi
+00009780: 6f6e 616c 2076 616c 6964 6174 696f 6e20  onal validation 
+00009790: 6f70 7469 6f6e 7320 6173 206b 6579 2d76  options as key-v
+000097a0: 616c 7565 2070 6169 7273 2c20 6465 6661  alue pairs, defa
+000097b0: 756c 7473 2074 6f20 607b 7d60 2e0a 2020  ults to `{}`..  
+000097c0: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+000097d0: 6b65 7920 6072 756e 5f76 616c 6964 6174  key `run_validat
+000097e0: 696f 6e60 2062 6f6f 6c65 616e 2076 616c  ion` boolean val
+000097f0: 7565 2c20 7365 7420 746f 2060 4661 6c73  ue, set to `Fals
+00009800: 6560 2074 6f20 736b 6970 2076 616c 6964  e` to skip valid
+00009810: 6174 696f 6e20 7465 6d70 6f72 6172 696c  ation temporaril
+00009820: 7920 6f6e 2069 6e67 6573 7469 6f6e 2e0a  y on ingestion..
+00009830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009840: 2a20 6b65 7920 6067 655f 7661 6c69 6461  * key `ge_valida
+00009850: 7465 5f6b 7761 7267 7360 2061 2064 6963  te_kwargs` a dic
+00009860: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
+00009870: 6e67 206b 7761 7267 7320 666f 7220 7468  ng kwargs for th
+00009880: 6520 7661 6c69 6461 7465 206d 6574 686f  e validate metho
+00009890: 6420 6f66 2047 7265 6174 2045 7870 6563  d of Great Expec
+000098a0: 7461 7469 6f6e 732e 0a20 2020 2020 2020  tations..       
+000098b0: 2020 2020 2069 6e67 6573 7469 6f6e 5f72       ingestion_r
+000098c0: 6573 756c 743a 2053 7065 6369 6679 2074  esult: Specify t
+000098d0: 6865 2066 6174 6520 6f66 2074 6865 2061  he fate of the a
+000098e0: 7373 6f63 6961 7465 6420 6461 7461 2c20  ssociated data, 
+000098f0: 6465 6661 756c 7473 0a20 2020 2020 2020  defaults.       
+00009900: 2020 2020 2020 2020 2074 6f20 2255 4e4b           to "UNK
+00009910: 4e4f 574e 222e 2053 7570 706f 7274 6564  NOWN". Supported
+00009920: 206f 7074 696f 6e73 2061 7265 2020 2255   options are  "U
+00009930: 4e4b 4e4f 574e 222c 2022 494e 4745 5354  NKNOWN", "INGEST
+00009940: 4544 222c 2022 5245 4a45 4354 4544 222c  ED", "REJECTED",
+00009950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009960: 2022 4558 5045 5249 4d45 4e54 222c 2022   "EXPERIMENT", "
+00009970: 4647 5f44 4154 4122 2e20 5573 6520 2249  FG_DATA". Use "I
+00009980: 4e47 4553 5445 4422 206f 7220 2252 454a  NGESTED" or "REJ
+00009990: 4543 5445 4422 2066 6f72 2076 616c 6964  ECTED" for valid
+000099a0: 6174 696f 6e0a 2020 2020 2020 2020 2020  ation.          
+000099b0: 2020 2020 2020 6f66 2044 6174 6146 7261        of DataFra
+000099c0: 6d65 7320 746f 2062 6520 696e 7365 7274  mes to be insert
+000099d0: 6564 2069 6e20 7468 6520 4665 6174 7572  ed in the Featur
+000099e0: 6520 4772 6f75 702e 2055 7365 2022 4558  e Group. Use "EX
+000099f0: 5045 5249 4d45 4e54 220a 2020 2020 2020  PERIMENT".      
+00009a00: 2020 2020 2020 2020 2020 666f 7220 7465            for te
+00009a10: 7374 696e 6720 616e 6420 6465 7665 6c6f  sting and develo
+00009a20: 706d 656e 7420 616e 6420 2246 475f 4441  pment and "FG_DA
+00009a30: 5441 2220 7768 656e 2076 616c 6964 6174  TA" when validat
+00009a40: 696e 6720 6461 7461 0a20 2020 2020 2020  ing data.       
+00009a50: 2020 2020 2020 2020 2061 6c72 6561 6479           already
+00009a60: 2069 6e20 7468 6520 4665 6174 7572 6520   in the Feature 
+00009a70: 4772 6f75 702e 0a20 2020 2020 2020 2020  Group..         
+00009a80: 2020 2073 6176 655f 7265 706f 7274 3a20     save_report: 
+00009a90: 5768 6574 6865 7220 746f 2073 6176 6520  Whether to save 
+00009aa0: 7468 6520 7265 706f 7274 2074 6f20 7468  the report to th
+00009ab0: 6520 6261 636b 656e 642e 2054 6869 7320  e backend. This 
+00009ac0: 6973 206f 6e6c 7920 706f 7373 6962 6c65  is only possible
+00009ad0: 2069 6620 7468 6520 4578 7065 6374 6174   if the Expectat
+00009ae0: 696f 6e20 7375 6974 650a 2020 2020 2020  ion suite.      
+00009af0: 2020 2020 2020 2020 2020 6973 2069 6e69            is ini
+00009b00: 7469 616c 6973 6564 2061 6e64 2061 7474  tialised and att
+00009b10: 6163 6865 6420 746f 2074 6865 2046 6561  ached to the Fea
+00009b20: 7475 7265 2047 726f 7570 2e20 4465 6661  ture Group. Defa
+00009b30: 756c 7473 2074 6f20 4661 6c73 652e 0a20  ults to False.. 
+00009b40: 2020 2020 2020 2020 2020 2067 655f 7479             ge_ty
+00009b50: 7065 3a20 5768 6574 6865 7220 746f 2072  pe: Whether to r
+00009b60: 6574 7572 6e20 6120 4772 6561 7420 4578  eturn a Great Ex
+00009b70: 7065 6374 6174 696f 6e73 206f 626a 6563  pectations objec
+00009b80: 7420 6f72 2048 6f70 7377 6f72 6b73 206f  t or Hopsworks o
+00009b90: 776e 2061 6273 7472 6163 7469 6f6e 2e20  wn abstraction. 
+00009ba0: 4465 6661 756c 7473 2074 6f20 5472 7565  Defaults to True
+00009bb0: 2e0a 0a20 2020 2020 2020 2023 2052 6574  ...        # Ret
+00009bc0: 7572 6e73 0a20 2020 2020 2020 2020 2020  urns.           
+00009bd0: 2041 2056 616c 6964 6174 696f 6e20 5265   A Validation Re
+00009be0: 706f 7274 2070 726f 6475 6365 6420 6279  port produced by
+00009bf0: 2047 7265 6174 2045 7870 6563 7461 7469   Great Expectati
+00009c00: 6f6e 732e 0a20 2020 2020 2020 2022 2222  ons..        """
+00009c10: 0a20 2020 2020 2020 2023 2041 6374 6976  .        # Activ
+00009c20: 6974 7920 6973 206c 6f67 6765 6420 6f6e  ity is logged on
+00009c30: 6c79 2069 6620 6120 7468 6520 7661 6c69  ly if a the vali
+00009c40: 6461 7469 6f6e 2063 6f6e 6365 726e 7320  dation concerns 
+00009c50: 7468 6520 6665 6174 7572 6520 6772 6f75  the feature grou
+00009c60: 7020 616e 6420 6e6f 7420 6120 7370 6563  p and not a spec
+00009c70: 6966 6963 2064 6174 6166 7261 6d65 0a20  ific dataframe. 
+00009c80: 2020 2020 2020 2069 6620 6461 7461 6672         if datafr
+00009c90: 616d 6520 6973 204e 6f6e 653a 0a20 2020  ame is None:.   
+00009ca0: 2020 2020 2020 2020 2064 6174 6166 7261           datafra
+00009cb0: 6d65 203d 2073 656c 662e 7265 6164 2829  me = self.read()
+00009cc0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00009cd0: 696e 6765 7374 696f 6e5f 7265 7375 6c74  ingestion_result
+00009ce0: 203d 3d20 2255 4e4b 4e4f 574e 223a 0a20   == "UNKNOWN":. 
+00009cf0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00009d00: 6e67 6573 7469 6f6e 5f72 6573 756c 7420  ngestion_result 
+00009d10: 3d20 2246 475f 4441 5441 220a 0a20 2020  = "FG_DATA"..   
+00009d20: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00009d30: 2e5f 6772 6561 745f 6578 7065 6374 6174  ._great_expectat
+00009d40: 696f 6e5f 656e 6769 6e65 2e76 616c 6964  ion_engine.valid
+00009d50: 6174 6528 0a20 2020 2020 2020 2020 2020  ate(.           
+00009d60: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
+00009d70: 2020 2064 6174 6166 7261 6d65 3d65 6e67     dataframe=eng
+00009d80: 696e 652e 6765 745f 696e 7374 616e 6365  ine.get_instance
+00009d90: 2829 2e63 6f6e 7665 7274 5f74 6f5f 6465  ().convert_to_de
+00009da0: 6661 756c 745f 6461 7461 6672 616d 6528  fault_dataframe(
+00009db0: 6461 7461 6672 616d 6529 2c0a 2020 2020  dataframe),.    
+00009dc0: 2020 2020 2020 2020 6578 7065 6374 6174          expectat
+00009dd0: 696f 6e5f 7375 6974 653d 6578 7065 6374  ion_suite=expect
+00009de0: 6174 696f 6e5f 7375 6974 652c 0a20 2020  ation_suite,.   
+00009df0: 2020 2020 2020 2020 2073 6176 655f 7265           save_re
+00009e00: 706f 7274 3d73 6176 655f 7265 706f 7274  port=save_report
+00009e10: 2c0a 2020 2020 2020 2020 2020 2020 7661  ,.            va
+00009e20: 6c69 6461 7469 6f6e 5f6f 7074 696f 6e73  lidation_options
+00009e30: 3d76 616c 6964 6174 696f 6e5f 6f70 7469  =validation_opti
+00009e40: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
+00009e50: 2069 6e67 6573 7469 6f6e 5f72 6573 756c   ingestion_resul
+00009e60: 743d 696e 6765 7374 696f 6e5f 7265 7375  t=ingestion_resu
+00009e70: 6c74 2c0a 2020 2020 2020 2020 2020 2020  lt,.            
+00009e80: 6765 5f74 7970 653d 6765 5f74 7970 652c  ge_type=ge_type,
+00009e90: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00009ea0: 6465 6620 5f5f 6765 7461 7474 725f 5f28  def __getattr__(
+00009eb0: 7365 6c66 2c20 6e61 6d65 293a 0a20 2020  self, name):.   
+00009ec0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00009ed0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00009ee0: 662e 5f5f 6765 7469 7465 6d5f 5f28 6e61  f.__getitem__(na
+00009ef0: 6d65 290a 2020 2020 2020 2020 6578 6365  me).        exce
+00009f00: 7074 204b 6579 4572 726f 723a 0a20 2020  pt KeyError:.   
+00009f10: 2020 2020 2020 2020 2072 6169 7365 2041           raise A
+00009f20: 7474 7269 6275 7465 4572 726f 7228 0a20  ttributeError(. 
+00009f30: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00009f40: 2227 4665 6174 7572 6547 726f 7570 2720  "'FeatureGroup' 
+00009f50: 6f62 6a65 6374 2068 6173 206e 6f20 6174  object has no at
+00009f60: 7472 6962 7574 6520 277b 6e61 6d65 7d27  tribute '{name}'
+00009f70: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
+00009f80: 2020 2020 2249 6620 796f 7520 6172 6520      "If you are 
+00009f90: 7472 7969 6e67 2074 6f20 6163 6365 7373  trying to access
+00009fa0: 2061 2066 6561 7475 7265 2c20 6661 6c6c   a feature, fall
+00009fb0: 2062 6163 6b20 6f6e 2022 0a20 2020 2020   back on ".     
+00009fc0: 2020 2020 2020 2020 2020 2022 7573 696e             "usin
+00009fd0: 6720 7468 6520 6067 6574 5f66 6561 7475  g the `get_featu
+00009fe0: 7265 6020 6d65 7468 6f64 2e22 0a20 2020  re` method.".   
+00009ff0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000a000: 6465 6620 5f5f 6765 7469 7465 6d5f 5f28  def __getitem__(
+0000a010: 7365 6c66 2c20 6e61 6d65 293a 0a20 2020  self, name):.   
+0000a020: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+0000a030: 7374 616e 6365 286e 616d 652c 2073 7472  stance(name, str
+0000a040: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+0000a050: 6169 7365 2054 7970 6545 7272 6f72 280a  aise TypeError(.
+0000a060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a070: 6622 4578 7065 6374 6564 2074 7970 6520  f"Expected type 
+0000a080: 6073 7472 602c 2067 6f74 2060 7b74 7970  `str`, got `{typ
+0000a090: 6528 6e61 6d65 297d 602e 2022 0a20 2020  e(name)}`. ".   
+0000a0a0: 2020 2020 2020 2020 2020 2020 2022 4665               "Fe
+0000a0b0: 6174 7572 6573 2061 7265 2061 6363 6573  atures are acces
+0000a0c0: 7369 626c 6520 6279 206e 616d 652e 220a  sible by name.".
+0000a0d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000a0e0: 2020 2020 2020 6665 6174 7572 6520 3d20        feature = 
+0000a0f0: 5b66 2066 6f72 2066 2069 6e20 7365 6c66  [f for f in self
+0000a100: 2e5f 5f67 6574 6174 7472 6962 7574 655f  .__getattribute_
+0000a110: 5f28 225f 6665 6174 7572 6573 2229 2069  _("_features") i
+0000a120: 6620 662e 6e61 6d65 203d 3d20 6e61 6d65  f f.name == name
+0000a130: 5d0a 2020 2020 2020 2020 6966 206c 656e  ].        if len
+0000a140: 2866 6561 7475 7265 2920 3d3d 2031 3a0a  (feature) == 1:.
+0000a150: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000a160: 726e 2066 6561 7475 7265 5b30 5d0a 2020  rn feature[0].  
+0000a170: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000a180: 2020 2020 2020 2020 7261 6973 6520 4b65          raise Ke
+0000a190: 7945 7272 6f72 2866 2227 4665 6174 7572  yError(f"'Featur
+0000a1a0: 6547 726f 7570 2720 6f62 6a65 6374 2068  eGroup' object h
+0000a1b0: 6173 206e 6f20 6665 6174 7572 6520 6361  as no feature ca
+0000a1c0: 6c6c 6564 2027 7b6e 616d 657d 272e 2229  lled '{name}'.")
+0000a1d0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000a1e0: 2020 2020 6465 6620 7374 6174 6973 7469      def statisti
+0000a1f0: 6373 5f63 6f6e 6669 6728 7365 6c66 293a  cs_config(self):
+0000a200: 0a20 2020 2020 2020 2022 2222 5374 6174  .        """Stat
+0000a210: 6973 7469 6373 2063 6f6e 6669 6775 7261  istics configura
+0000a220: 7469 6f6e 206f 626a 6563 7420 6465 6669  tion object defi
+0000a230: 6e69 6e67 2074 6865 2073 6574 7469 6e67  ning the setting
+0000a240: 7320 666f 7220 7374 6174 6973 7469 6373  s for statistics
+0000a250: 0a20 2020 2020 2020 2063 6f6d 7075 7461  .        computa
+0000a260: 7469 6f6e 206f 6620 7468 6520 6665 6174  tion of the feat
+0000a270: 7572 6520 6772 6f75 702e 2222 220a 2020  ure group.""".  
+0000a280: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000a290: 662e 5f73 7461 7469 7374 6963 735f 636f  f._statistics_co
+0000a2a0: 6e66 6967 0a0a 2020 2020 4073 7461 7469  nfig..    @stati
+0000a2b0: 7374 6963 735f 636f 6e66 6967 2e73 6574  stics_config.set
+0000a2c0: 7465 720a 2020 2020 6465 6620 7374 6174  ter.    def stat
+0000a2d0: 6973 7469 6373 5f63 6f6e 6669 6728 7365  istics_config(se
+0000a2e0: 6c66 2c20 7374 6174 6973 7469 6373 5f63  lf, statistics_c
+0000a2f0: 6f6e 6669 6729 3a0a 2020 2020 2020 2020  onfig):.        
+0000a300: 6966 2069 7369 6e73 7461 6e63 6528 7374  if isinstance(st
+0000a310: 6174 6973 7469 6373 5f63 6f6e 6669 672c  atistics_config,
+0000a320: 2053 7461 7469 7374 6963 7343 6f6e 6669   StatisticsConfi
+0000a330: 6729 3a0a 2020 2020 2020 2020 2020 2020  g):.            
+0000a340: 7365 6c66 2e5f 7374 6174 6973 7469 6373  self._statistics
+0000a350: 5f63 6f6e 6669 6720 3d20 7374 6174 6973  _config = statis
+0000a360: 7469 6373 5f63 6f6e 6669 670a 2020 2020  tics_config.    
+0000a370: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+0000a380: 6e63 6528 7374 6174 6973 7469 6373 5f63  nce(statistics_c
+0000a390: 6f6e 6669 672c 2064 6963 7429 3a0a 2020  onfig, dict):.  
+0000a3a0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000a3b0: 7374 6174 6973 7469 6373 5f63 6f6e 6669  statistics_confi
+0000a3c0: 6720 3d20 5374 6174 6973 7469 6373 436f  g = StatisticsCo
+0000a3d0: 6e66 6967 282a 2a73 7461 7469 7374 6963  nfig(**statistic
+0000a3e0: 735f 636f 6e66 6967 290a 2020 2020 2020  s_config).      
+0000a3f0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+0000a400: 6528 7374 6174 6973 7469 6373 5f63 6f6e  e(statistics_con
+0000a410: 6669 672c 2062 6f6f 6c29 3a0a 2020 2020  fig, bool):.    
+0000a420: 2020 2020 2020 2020 7365 6c66 2e5f 7374          self._st
+0000a430: 6174 6973 7469 6373 5f63 6f6e 6669 6720  atistics_config 
+0000a440: 3d20 5374 6174 6973 7469 6373 436f 6e66  = StatisticsConf
+0000a450: 6967 2873 7461 7469 7374 6963 735f 636f  ig(statistics_co
+0000a460: 6e66 6967 290a 2020 2020 2020 2020 656c  nfig).        el
+0000a470: 6966 2073 7461 7469 7374 6963 735f 636f  if statistics_co
+0000a480: 6e66 6967 2069 7320 4e6f 6e65 3a0a 2020  nfig is None:.  
+0000a490: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0000a4a0: 7374 6174 6973 7469 6373 5f63 6f6e 6669  statistics_confi
+0000a4b0: 6720 3d20 5374 6174 6973 7469 6373 436f  g = StatisticsCo
+0000a4c0: 6e66 6967 2829 0a20 2020 2020 2020 2065  nfig().        e
+0000a4d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000a4e0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+0000a4f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000a500: 2020 2254 6865 2061 7267 756d 656e 7420    "The argument 
+0000a510: 6073 7461 7469 7374 6963 735f 636f 6e66  `statistics_conf
+0000a520: 6967 6020 6861 7320 746f 2062 6520 604e  ig` has to be `N
+0000a530: 6f6e 6560 206f 6620 7479 7065 2060 5374  one` of type `St
+0000a540: 6174 6973 7469 6373 436f 6e66 6967 2c20  atisticsConfig, 
+0000a550: 6062 6f6f 6c60 206f 7220 6064 6963 7460  `bool` or `dict`
+0000a560: 2c20 6275 7420 6973 206f 6620 7479 7065  , but is of type
+0000a570: 3a20 607b 7d60 222e 666f 726d 6174 280a  : `{}`".format(.
+0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a590: 2020 2020 7479 7065 2873 7461 7469 7374      type(statist
+0000a5a0: 6963 735f 636f 6e66 6967 290a 2020 2020  ics_config).    
+0000a5b0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000a5c0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000a5d0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+0000a5e0: 6566 2073 7461 7469 7374 6963 7328 7365  ef statistics(se
+0000a5f0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000a600: 4765 7420 7468 6520 6c61 7465 7374 2063  Get the latest c
+0000a610: 6f6d 7075 7465 6420 7374 6174 6973 7469  omputed statisti
+0000a620: 6373 2066 6f72 2074 6865 2066 6561 7475  cs for the featu
+0000a630: 7265 2067 726f 7570 2e22 2222 0a20 2020  re group.""".   
+0000a640: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000a650: 2e5f 7374 6174 6973 7469 6373 5f65 6e67  ._statistics_eng
+0000a660: 696e 652e 6765 745f 6c61 7374 2873 656c  ine.get_last(sel
+0000a670: 6629 0a0a 2020 2020 4070 726f 7065 7274  f)..    @propert
+0000a680: 790a 2020 2020 6465 6620 7072 696d 6172  y.    def primar
+0000a690: 795f 6b65 7928 7365 6c66 293a 0a20 2020  y_key(self):.   
+0000a6a0: 2020 2020 2022 2222 4c69 7374 206f 6620       """List of 
+0000a6b0: 6665 6174 7572 6573 2062 7569 6c64 696e  features buildin
+0000a6c0: 6720 7468 6520 7072 696d 6172 7920 6b65  g the primary ke
+0000a6d0: 792e 2222 220a 2020 2020 2020 2020 7265  y.""".        re
+0000a6e0: 7475 726e 2073 656c 662e 5f70 7269 6d61  turn self._prima
+0000a6f0: 7279 5f6b 6579 0a0a 2020 2020 4070 7269  ry_key..    @pri
+0000a700: 6d61 7279 5f6b 6579 2e73 6574 7465 720a  mary_key.setter.
+0000a710: 2020 2020 6465 6620 7072 696d 6172 795f      def primary_
+0000a720: 6b65 7928 7365 6c66 2c20 6e65 775f 7072  key(self, new_pr
+0000a730: 696d 6172 795f 6b65 7929 3a0a 2020 2020  imary_key):.    
+0000a740: 2020 2020 7365 6c66 2e5f 7072 696d 6172      self._primar
+0000a750: 795f 6b65 7920 3d20 5b70 6b2e 6c6f 7765  y_key = [pk.lowe
+0000a760: 7228 2920 666f 7220 706b 2069 6e20 6e65  r() for pk in ne
+0000a770: 775f 7072 696d 6172 795f 6b65 795d 0a0a  w_primary_key]..
+0000a780: 2020 2020 6465 6620 6765 745f 7374 6174      def get_stat
+0000a790: 6973 7469 6373 280a 2020 2020 2020 2020  istics(.        
+0000a7a0: 7365 6c66 2c20 636f 6d6d 6974 5f74 696d  self, commit_tim
+0000a7b0: 653a 204f 7074 696f 6e61 6c5b 556e 696f  e: Optional[Unio
+0000a7c0: 6e5b 7374 722c 2069 6e74 2c20 6461 7465  n[str, int, date
+0000a7d0: 7469 6d65 2c20 6461 7465 5d5d 203d 204e  time, date]] = N
+0000a7e0: 6f6e 650a 2020 2020 293a 0a20 2020 2020  one.    ):.     
+0000a7f0: 2020 2022 2222 5265 7475 726e 7320 7468     """Returns th
+0000a800: 6520 7374 6174 6973 7469 6373 2066 6f72  e statistics for
+0000a810: 2074 6869 7320 6665 6174 7572 6520 6772   this feature gr
+0000a820: 6f75 7020 6174 2061 2073 7065 6369 6669  oup at a specifi
+0000a830: 6320 7469 6d65 2e0a 0a20 2020 2020 2020  c time...       
+0000a840: 2049 6620 6063 6f6d 6d69 745f 7469 6d65   If `commit_time
+0000a850: 6020 6973 2060 4e6f 6e65 602c 2074 6865  ` is `None`, the
+0000a860: 206d 6f73 7420 7265 6365 6e74 2073 7461   most recent sta
+0000a870: 7469 7374 6963 7320 6172 6520 7265 7475  tistics are retu
+0000a880: 726e 6564 2e0a 0a20 2020 2020 2020 2021  rned...        !
+0000a890: 2121 2065 7861 6d70 6c65 0a20 2020 2020  !! example.     
+0000a8a0: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+0000a8b0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+0000a8c0: 6f6e 6e65 6374 2074 6f20 7468 6520 4665  onnect to the Fe
+0000a8d0: 6174 7572 6520 5374 6f72 650a 2020 2020  ature Store.    
+0000a8e0: 2020 2020 2020 2020 6673 203d 202e 2e2e          fs = ...
+0000a8f0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000a900: 6765 7420 7468 6520 4665 6174 7572 6520  get the Feature 
+0000a910: 4772 6f75 7020 696e 7374 616e 6365 0a20  Group instance. 
+0000a920: 2020 2020 2020 2020 2020 2066 6720 3d20             fg = 
+0000a930: 6673 2e67 6574 5f6f 725f 6372 6561 7465  fs.get_or_create
+0000a940: 5f66 6561 7475 7265 5f67 726f 7570 282e  _feature_group(.
+0000a950: 2e2e 290a 0a20 2020 2020 2020 2020 2020  ..)..           
+0000a960: 2066 675f 7374 6174 6973 7469 6373 203d   fg_statistics =
+0000a970: 2066 672e 6765 745f 7374 6174 6973 7469   fg.get_statisti
+0000a980: 6373 2863 6f6d 6d69 745f 7469 6d65 3d4e  cs(commit_time=N
+0000a990: 6f6e 6529 0a20 2020 2020 2020 2020 2020  one).           
+0000a9a0: 2060 6060 0a0a 2020 2020 2020 2020 2320   ```..        # 
+0000a9b0: 4172 6775 6d65 6e74 730a 2020 2020 2020  Arguments.      
+0000a9c0: 2020 2020 2020 636f 6d6d 6974 5f74 696d        commit_tim
+0000a9d0: 653a 2044 6174 6520 616e 6420 7469 6d65  e: Date and time
+0000a9e0: 206f 6620 7468 6520 636f 6d6d 6974 2e20   of the commit. 
+0000a9f0: 4465 6661 756c 7473 2074 6f20 604e 6f6e  Defaults to `Non
+0000aa00: 6560 2e20 5374 7269 6e67 7320 7368 6f75  e`. Strings shou
+0000aa10: 6c64 0a20 2020 2020 2020 2020 2020 2020  ld.             
+0000aa20: 2020 2062 6520 666f 726d 6174 7465 6420     be formatted 
+0000aa30: 696e 206f 6e65 206f 6620 7468 6520 666f  in one of the fo
+0000aa40: 6c6c 6f77 696e 6720 666f 726d 6174 7320  llowing formats 
+0000aa50: 6025 592d 256d 2d25 6460 2c20 6025 592d  `%Y-%m-%d`, `%Y-
+0000aa60: 256d 2d25 6420 2548 602c 2060 2559 2d25  %m-%d %H`, `%Y-%
+0000aa70: 6d2d 2564 2025 483a 254d 602c 2060 2559  m-%d %H:%M`, `%Y
+0000aa80: 2d25 6d2d 2564 2025 483a 254d 3a25 5360  -%m-%d %H:%M:%S`
+0000aa90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000aaa0: 2020 6f72 2060 2559 2d25 6d2d 2564 2025    or `%Y-%m-%d %
+0000aab0: 483a 254d 3a25 532e 2566 602e 0a0a 2020  H:%M:%S.%f`...  
+0000aac0: 2020 2020 2020 2320 5265 7475 726e 730a        # Returns.
+0000aad0: 2020 2020 2020 2020 2020 2020 6053 7461              `Sta
+0000aae0: 7469 7374 6963 7360 2e20 5374 6174 6973  tistics`. Statis
+0000aaf0: 7469 6373 206f 626a 6563 742e 0a0a 2020  tics object...  
+0000ab00: 2020 2020 2020 2320 5261 6973 6573 0a20        # Raises. 
+0000ab10: 2020 2020 2020 2020 2020 2060 6873 6673             `hsfs
+0000ab20: 2e63 6c69 656e 742e 6578 6365 7074 696f  .client.exceptio
+0000ab30: 6e73 2e52 6573 7441 5049 4572 726f 7260  ns.RestAPIError`
+0000ab40: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000ab50: 2020 2020 2020 6966 2063 6f6d 6d69 745f        if commit_
+0000ab60: 7469 6d65 2069 7320 4e6f 6e65 3a0a 2020  time is None:.  
+0000ab70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000ab80: 2073 656c 662e 7374 6174 6973 7469 6373   self.statistics
+0000ab90: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000aba0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000abb0: 6e20 7365 6c66 2e5f 7374 6174 6973 7469  n self._statisti
+0000abc0: 6373 5f65 6e67 696e 652e 6765 7428 7365  cs_engine.get(se
+0000abd0: 6c66 2c20 636f 6d6d 6974 5f74 696d 6529  lf, commit_time)
+0000abe0: 0a0a 2020 2020 6465 6620 636f 6d70 7574  ..    def comput
+0000abf0: 655f 7374 6174 6973 7469 6373 2873 656c  e_statistics(sel
+0000ac00: 6629 3a0a 2020 2020 2020 2020 2222 2252  f):.        """R
+0000ac10: 6563 6f6d 7075 7465 2074 6865 2073 7461  ecompute the sta
+0000ac20: 7469 7374 6963 7320 666f 7220 7468 6520  tistics for the 
+0000ac30: 6665 6174 7572 6520 6772 6f75 7020 616e  feature group an
+0000ac40: 6420 7361 7665 2074 6865 6d20 746f 2074  d save them to t
+0000ac50: 6865 0a20 2020 2020 2020 2066 6561 7475  he.        featu
+0000ac60: 7265 2073 746f 7265 2e0a 2020 2020 2020  re store..      
+0000ac70: 2020 5374 6174 6973 7469 6373 2061 7265    Statistics are
+0000ac80: 206f 6e6c 7920 636f 6d70 7574 6564 2066   only computed f
+0000ac90: 6f72 2064 6174 6120 696e 2074 6865 206f  or data in the o
+0000aca0: 6666 6c69 6e65 2073 746f 7261 6765 206f  ffline storage o
+0000acb0: 6620 7468 6520 6665 6174 7572 650a 2020  f the feature.  
+0000acc0: 2020 2020 2020 6772 6f75 702e 0a0a 2020        group...  
+0000acd0: 2020 2020 2020 2121 2120 6578 616d 706c        !!! exampl
+0000ace0: 650a 2020 2020 2020 2020 2020 2020 6060  e.            ``
+0000acf0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+0000ad00: 2020 2020 2320 636f 6e6e 6563 7420 746f      # connect to
+0000ad10: 2074 6865 2046 6561 7475 7265 2053 746f   the Feature Sto
+0000ad20: 7265 0a20 2020 2020 2020 2020 2020 2066  re.            f
+0000ad30: 7320 3d20 2e2e 2e0a 0a20 2020 2020 2020  s = .....       
+0000ad40: 2020 2020 2023 2067 6574 2074 6865 2046       # get the F
+0000ad50: 6561 7475 7265 2047 726f 7570 2069 6e73  eature Group ins
+0000ad60: 7461 6e63 650a 2020 2020 2020 2020 2020  tance.          
+0000ad70: 2020 6667 203d 2066 732e 6765 745f 6f72    fg = fs.get_or
+0000ad80: 5f63 7265 6174 655f 6665 6174 7572 655f  _create_feature_
+0000ad90: 6772 6f75 7028 2e2e 2e29 0a0a 2020 2020  group(...)..    
+0000ada0: 2020 2020 2020 2020 7374 6174 6973 7469          statisti
+0000adb0: 6373 5f6d 6574 6164 6174 6120 3d20 6667  cs_metadata = fg
+0000adc0: 2e63 6f6d 7075 7465 5f73 7461 7469 7374  .compute_statist
+0000add0: 6963 7328 290a 2020 2020 2020 2020 2020  ics().          
+0000ade0: 2020 6060 600a 0a20 2020 2020 2020 2023    ```..        #
+0000adf0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+0000ae00: 2020 2020 2060 5374 6174 6973 7469 6373       `Statistics
+0000ae10: 602e 2054 6865 2073 7461 7469 7374 6963  `. The statistic
+0000ae20: 7320 6d65 7461 6461 7461 206f 626a 6563  s metadata objec
+0000ae30: 742e 0a0a 2020 2020 2020 2020 2320 5261  t...        # Ra
+0000ae40: 6973 6573 0a20 2020 2020 2020 2020 2020  ises.           
+0000ae50: 2060 6873 6673 2e63 6c69 656e 742e 6578   `hsfs.client.ex
+0000ae60: 6365 7074 696f 6e73 2e52 6573 7441 5049  ceptions.RestAPI
+0000ae70: 4572 726f 7260 2e20 556e 6162 6c65 2074  Error`. Unable t
+0000ae80: 6f20 7065 7273 6973 7420 7468 6520 7374  o persist the st
+0000ae90: 6174 6973 7469 6373 2e0a 2020 2020 2020  atistics..      
+0000aea0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+0000aeb0: 2073 656c 662e 7374 6174 6973 7469 6373   self.statistics
+0000aec0: 5f63 6f6e 6669 672e 656e 6162 6c65 643a  _config.enabled:
+0000aed0: 0a20 2020 2020 2020 2020 2020 2023 2044  .            # D
+0000aee0: 6f6e 2774 2072 6561 6420 7468 6520 6461  on't read the da
+0000aef0: 7461 6672 616d 6520 6865 7265 2c20 746f  taframe here, to
+0000af00: 2061 766f 6964 2074 7269 6767 6572 696e   avoid triggerin
+0000af10: 6720 6120 7265 6164 206f 7065 7261 7469  g a read operati
+0000af20: 6f6e 0a20 2020 2020 2020 2020 2020 2023  on.            #
+0000af30: 2066 6f72 2074 6865 2050 7974 686f 6e20   for the Python 
+0000af40: 656e 6769 6e65 2e20 5468 6520 5079 7468  engine. The Pyth
+0000af50: 6f6e 2065 6e67 696e 6520 6973 2067 6f69  on engine is goi
+0000af60: 6e67 2074 6f20 7365 7475 7020 6120 5370  ng to setup a Sp
+0000af70: 6172 6b20 4a6f 620a 2020 2020 2020 2020  ark Job.        
+0000af80: 2020 2020 2320 746f 2075 7064 6174 6520      # to update 
+0000af90: 7468 6520 7374 6174 6973 7469 6373 2e0a  the statistics..
+0000afa0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000afb0: 726e 2073 656c 662e 5f73 7461 7469 7374  rn self._statist
+0000afc0: 6963 735f 656e 6769 6e65 2e63 6f6d 7075  ics_engine.compu
+0000afd0: 7465 5f73 7461 7469 7374 6963 7328 7365  te_statistics(se
+0000afe0: 6c66 290a 2020 2020 2020 2020 656c 7365  lf).        else
+0000aff0: 3a0a 2020 2020 2020 2020 2020 2020 7761  :.            wa
+0000b000: 726e 696e 6773 2e77 6172 6e28 0a20 2020  rnings.warn(.   
+0000b010: 2020 2020 2020 2020 2020 2020 2028 0a20               (. 
+0000b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b030: 2020 2022 5468 6520 7374 6174 6973 7469     "The statisti
+0000b040: 6373 2061 7265 206e 6f74 2065 6e61 626c  cs are not enabl
+0000b050: 6564 206f 6620 6665 6174 7572 6520 6772  ed of feature gr
+0000b060: 6f75 7020 607b 7d60 2c20 7769 7468 2076  oup `{}`, with v
+0000b070: 6572 7369 6f6e 220a 2020 2020 2020 2020  ersion".        
+0000b080: 2020 2020 2020 2020 2020 2020 2220 607b              " `{
+0000b090: 7d60 2e20 4e6f 2073 7461 7469 7374 6963  }`. No statistic
+0000b0a0: 7320 636f 6d70 7574 6564 2e22 0a20 2020  s computed.".   
+0000b0b0: 2020 2020 2020 2020 2020 2020 2029 2e66               ).f
+0000b0c0: 6f72 6d61 7428 7365 6c66 2e5f 6e61 6d65  ormat(self._name
+0000b0d0: 2c20 7365 6c66 2e5f 7665 7273 696f 6e29  , self._version)
+0000b0e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b0f0: 2020 7574 696c 2e53 746f 7261 6765 5761    util.StorageWa
+0000b100: 726e 696e 672c 0a20 2020 2020 2020 2020  rning,.         
+0000b110: 2020 2029 0a0a 2020 2020 4070 726f 7065     )..    @prope
+0000b120: 7274 790a 2020 2020 6465 6620 6576 656e  rty.    def even
+0000b130: 745f 7469 6d65 2873 656c 6629 3a0a 2020  t_time(self):.  
+0000b140: 2020 2020 2020 2222 2245 7665 6e74 2074        """Event t
+0000b150: 696d 6520 6665 6174 7572 6520 696e 2074  ime feature in t
+0000b160: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
+0000b170: 2e22 2222 0a20 2020 2020 2020 2072 6574  .""".        ret
+0000b180: 7572 6e20 7365 6c66 2e5f 6576 656e 745f  urn self._event_
+0000b190: 7469 6d65 0a0a 2020 2020 4065 7665 6e74  time..    @event
+0000b1a0: 5f74 696d 652e 7365 7474 6572 0a20 2020  _time.setter.   
+0000b1b0: 2064 6566 2065 7665 6e74 5f74 696d 6528   def event_time(
+0000b1c0: 7365 6c66 2c20 6665 6174 7572 655f 6e61  self, feature_na
+0000b1d0: 6d65 3a20 4f70 7469 6f6e 616c 5b73 7472  me: Optional[str
+0000b1e0: 5d29 3a0a 2020 2020 2020 2020 6966 2066  ]):.        if f
+0000b1f0: 6561 7475 7265 5f6e 616d 6520 6973 204e  eature_name is N
+0000b200: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000b210: 2073 656c 662e 5f65 7665 6e74 5f74 696d   self._event_tim
+0000b220: 6520 3d20 4e6f 6e65 0a20 2020 2020 2020  e = None.       
+0000b230: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000b240: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
+0000b250: 6e63 6528 6665 6174 7572 655f 6e61 6d65  nce(feature_name
+0000b260: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+0000b270: 2020 2020 7365 6c66 2e5f 6576 656e 745f      self._event_
+0000b280: 7469 6d65 203d 2066 6561 7475 7265 5f6e  time = feature_n
+0000b290: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+0000b2a0: 7265 7475 726e 0a20 2020 2020 2020 2065  return.        e
+0000b2b0: 6c69 6620 6973 696e 7374 616e 6365 2866  lif isinstance(f
+0000b2c0: 6561 7475 7265 5f6e 616d 652c 206c 6973  eature_name, lis
+0000b2d0: 7429 2061 6e64 206c 656e 2866 6561 7475  t) and len(featu
+0000b2e0: 7265 5f6e 616d 6529 203d 3d20 313a 0a20  re_name) == 1:. 
+0000b2f0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+0000b300: 696e 7374 616e 6365 2866 6561 7475 7265  instance(feature
+0000b310: 5f6e 616d 655b 305d 2c20 7374 7229 3a0a  _name[0], str):.
 0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b330: 2020 2066 6f72 2066 6561 7420 696e 2073     for feat in s
-0000b340: 656c 662e 5f66 6561 7475 7265 730a 2020  elf._features.  
-0000b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b360: 2020 6966 2066 6561 742e 6875 6469 5f70    if feat.hudi_p
-0000b370: 7265 636f 6d62 696e 655f 6b65 7920 6973  recombine_key is
-0000b380: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-0000b390: 2020 2020 2020 5d5b 305d 0a20 2020 2020        ][0].     
-0000b3a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000b3b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b3c0: 662e 5f68 7564 695f 7072 6563 6f6d 6269  f._hudi_precombi
-0000b3d0: 6e65 5f6b 6579 203d 204e 6f6e 650a 0a20  ne_key = None.. 
-0000b3e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b3f0: 7374 6174 6973 7469 6373 5f63 6f6e 6669  statistics_confi
-0000b400: 6720 3d20 7374 6174 6973 7469 6373 5f63  g = statistics_c
-0000b410: 6f6e 6669 670a 2020 2020 2020 2020 2020  onfig.          
-0000b420: 2020 7365 6c66 2e65 7870 6563 7461 7469    self.expectati
-0000b430: 6f6e 5f73 7569 7465 203d 2065 7870 6563  on_suite = expec
-0000b440: 7461 7469 6f6e 5f73 7569 7465 0a20 2020  tation_suite.   
-0000b450: 2020 2020 2020 2020 2069 6620 6578 7065           if expe
-0000b460: 6374 6174 696f 6e5f 7375 6974 653a 0a20  ctation_suite:. 
-0000b470: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b480: 656c 662e 5f65 7870 6563 7461 7469 6f6e  elf._expectation
-0000b490: 5f73 7569 7465 2e5f 696e 6974 5f65 7870  _suite._init_exp
-0000b4a0: 6563 7461 7469 6f6e 5f65 6e67 696e 6528  ectation_engine(
-0000b4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b4c0: 2020 2020 2066 6561 7475 7265 5f73 746f       feature_sto
-0000b4d0: 7265 5f69 643d 6665 6174 7572 6573 746f  re_id=featuresto
-0000b4e0: 7265 5f69 642c 2066 6561 7475 7265 5f67  re_id, feature_g
-0000b4f0: 726f 7570 5f69 643d 7365 6c66 2e5f 6964  roup_id=self._id
-0000b500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b510: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
-0000b520: 656c 662e 5f65 7870 6563 7461 7469 6f6e  elf._expectation
-0000b530: 5f73 7569 7465 5f65 6e67 696e 6520 3d20  _suite_engine = 
-0000b540: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000b550: 2020 6578 7065 6374 6174 696f 6e5f 7375    expectation_su
-0000b560: 6974 655f 656e 6769 6e65 2e45 7870 6563  ite_engine.Expec
-0000b570: 7461 7469 6f6e 5375 6974 6545 6e67 696e  tationSuiteEngin
-0000b580: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-0000b590: 2020 2020 2020 2066 6561 7475 7265 5f73         feature_s
-0000b5a0: 746f 7265 5f69 643d 7365 6c66 2e5f 6665  tore_id=self._fe
-0000b5b0: 6174 7572 655f 7374 6f72 655f 6964 2c20  ature_store_id, 
-0000b5c0: 6665 6174 7572 655f 6772 6f75 705f 6964  feature_group_id
-0000b5d0: 3d73 656c 662e 5f69 640a 2020 2020 2020  =self._id.      
-0000b5e0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000b5f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000b600: 2020 2020 2020 7365 6c66 2e5f 7661 6c69        self._vali
-0000b610: 6461 7469 6f6e 5f72 6570 6f72 745f 656e  dation_report_en
-0000b620: 6769 6e65 203d 2028 0a20 2020 2020 2020  gine = (.       
-0000b630: 2020 2020 2020 2020 2076 616c 6964 6174           validat
-0000b640: 696f 6e5f 7265 706f 7274 5f65 6e67 696e  ion_report_engin
-0000b650: 652e 5661 6c69 6461 7469 6f6e 5265 706f  e.ValidationRepo
-0000b660: 7274 456e 6769 6e65 280a 2020 2020 2020  rtEngine(.      
-0000b670: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000b680: 6c66 2e5f 6665 6174 7572 655f 7374 6f72  lf._feature_stor
-0000b690: 655f 6964 2c20 7365 6c66 2e5f 6964 0a20  e_id, self._id. 
-0000b6a0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000b6b0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000b6c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b6d0: 5f76 616c 6964 6174 696f 6e5f 7265 7375  _validation_resu
-0000b6e0: 6c74 5f65 6e67 696e 6520 3d20 280a 2020  lt_engine = (.  
-0000b6f0: 2020 2020 2020 2020 2020 2020 2020 7661                va
-0000b700: 6c69 6461 7469 6f6e 5f72 6573 756c 745f  lidation_result_
-0000b710: 656e 6769 6e65 2e56 616c 6964 6174 696f  engine.Validatio
-0000b720: 6e52 6573 756c 7445 6e67 696e 6528 0a20  nResultEngine(. 
-0000b730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b740: 2020 2073 656c 662e 5f66 6561 7475 7265     self._feature
-0000b750: 5f73 746f 7265 5f69 642c 2073 656c 662e  _store_id, self.
-0000b760: 5f69 640a 2020 2020 2020 2020 2020 2020  _id.            
-0000b770: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000b780: 2020 290a 0a20 2020 2020 2020 2065 6c73    )..        els
-0000b790: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-0000b7a0: 2069 6e69 7469 616c 697a 6564 2062 7920   initialized by 
-0000b7b0: 7573 6572 0a20 2020 2020 2020 2020 2020  user.           
-0000b7c0: 2023 2066 6f72 2070 7974 686f 6e20 656e   # for python en
-0000b7d0: 6769 6e65 2077 6520 616c 7761 7973 2075  gine we always u
-0000b7e0: 7365 2073 7472 6561 6d20 6665 6174 7572  se stream featur
-0000b7f0: 6520 6772 6f75 700a 2020 2020 2020 2020  e group.        
-0000b800: 2020 2020 6966 2065 6e67 696e 652e 6765      if engine.ge
-0000b810: 745f 7479 7065 2829 203d 3d20 2270 7974  t_type() == "pyt
-0000b820: 686f 6e22 3a0a 2020 2020 2020 2020 2020  hon":.          
-0000b830: 2020 2020 2020 7365 6c66 2e5f 7374 7265        self._stre
-0000b840: 616d 203d 2054 7275 650a 2020 2020 2020  am = True.      
-0000b850: 2020 2020 2020 2320 666f 7220 7374 7265        # for stre
-0000b860: 616d 2066 6561 7475 7265 2067 726f 7570  am feature group
-0000b870: 2074 696d 6520 7472 6176 656c 2066 6f72   time travel for
-0000b880: 6d61 7420 6973 2061 6c77 6179 7320 4855  mat is always HU
-0000b890: 4449 0a20 2020 2020 2020 2020 2020 2069  DI.            i
-0000b8a0: 6620 7365 6c66 2e5f 7374 7265 616d 3a0a  f self._stream:.
-0000b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8c0: 6578 7065 6374 6564 5f66 6f72 6d61 7420  expected_format 
-0000b8d0: 3d20 2248 5544 4922 0a20 2020 2020 2020  = "HUDI".       
-0000b8e0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000b8f0: 2e5f 7469 6d65 5f74 7261 7665 6c5f 666f  ._time_travel_fo
-0000b900: 726d 6174 2021 3d20 6578 7065 6374 6564  rmat != expected
-0000b910: 5f66 6f72 6d61 743a 0a20 2020 2020 2020  _format:.       
-0000b920: 2020 2020 2020 2020 2020 2020 2077 6172               war
-0000b930: 6e69 6e67 732e 7761 726e 280a 2020 2020  nings.warn(.    
-0000b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b950: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-0000b960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b970: 2020 2254 6865 2070 726f 7669 6465 6420    "The provided 
-0000b980: 7469 6d65 2074 7261 7665 6c20 666f 726d  time travel form
-0000b990: 6174 2060 7b7d 6020 6861 7320 6265 656e  at `{}` has been
-0000b9a0: 206f 7665 7277 7269 7474 656e 2022 0a20   overwritten ". 
-0000b9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9c0: 2020 2020 2020 2020 2020 2022 6265 6361             "beca
-0000b9d0: 7573 6520 5374 7265 616d 2065 6e61 626c  use Stream enabl
-0000b9e0: 6564 2066 6561 7475 7265 2067 726f 7570  ed feature group
-0000b9f0: 7320 6f6e 6c79 2073 7570 706f 7274 2060  s only support `
-0000ba00: 7b7d 6022 0a20 2020 2020 2020 2020 2020  {}`".           
-0000ba10: 2020 2020 2020 2020 2020 2020 2029 2e66               ).f
-0000ba20: 6f72 6d61 7428 7365 6c66 2e5f 7469 6d65  ormat(self._time
-0000ba30: 5f74 7261 7665 6c5f 666f 726d 6174 2c20  _travel_format, 
-0000ba40: 6578 7065 6374 6564 5f66 6f72 6d61 7429  expected_format)
-0000ba50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ba60: 2020 2020 2020 2020 2020 7574 696c 2e46            util.F
-0000ba70: 6561 7475 7265 4772 6f75 7057 6172 6e69  eatureGroupWarni
-0000ba80: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
-0000ba90: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000baa0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000bab0: 6c66 2e5f 7469 6d65 5f74 7261 7665 6c5f  lf._time_travel_
-0000bac0: 666f 726d 6174 203d 2065 7870 6563 7465  format = expecte
-0000bad0: 645f 666f 726d 6174 0a0a 2020 2020 2020  d_format..      
-0000bae0: 2020 2020 2020 7365 6c66 2e70 7269 6d61        self.prima
-0000baf0: 7279 5f6b 6579 203d 2070 7269 6d61 7279  ry_key = primary
-0000bb00: 5f6b 6579 0a20 2020 2020 2020 2020 2020  _key.           
-0000bb10: 2073 656c 662e 7061 7274 6974 696f 6e5f   self.partition_
-0000bb20: 6b65 7920 3d20 7061 7274 6974 696f 6e5f  key = partition_
-0000bb30: 6b65 790a 2020 2020 2020 2020 2020 2020  key.            
-0000bb40: 7365 6c66 2e5f 6875 6469 5f70 7265 636f  self._hudi_preco
-0000bb50: 6d62 696e 655f 6b65 7920 3d20 280a 2020  mbine_key = (.  
-0000bb60: 2020 2020 2020 2020 2020 2020 2020 6875                hu
-0000bb70: 6469 5f70 7265 636f 6d62 696e 655f 6b65  di_precombine_ke
-0000bb80: 792e 6c6f 7765 7228 290a 2020 2020 2020  y.lower().      
-0000bb90: 2020 2020 2020 2020 2020 6966 2068 7564            if hud
-0000bba0: 695f 7072 6563 6f6d 6269 6e65 5f6b 6579  i_precombine_key
-0000bbb0: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-0000bbc0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-0000bbd0: 2073 656c 662e 5f74 696d 655f 7472 6176   self._time_trav
-0000bbe0: 656c 5f66 6f72 6d61 7420 6973 206e 6f74  el_format is not
-0000bbf0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0000bc00: 2020 2020 2020 616e 6420 7365 6c66 2e5f        and self._
-0000bc10: 7469 6d65 5f74 7261 7665 6c5f 666f 726d  time_travel_form
-0000bc20: 6174 203d 3d20 2248 5544 4922 0a20 2020  at == "HUDI".   
-0000bc30: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000bc40: 6520 4e6f 6e65 0a20 2020 2020 2020 2020  e None.         
-0000bc50: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000bc60: 2073 656c 662e 7374 6174 6973 7469 6373   self.statistics
-0000bc70: 5f63 6f6e 6669 6720 3d20 7374 6174 6973  _config = statis
-0000bc80: 7469 6373 5f63 6f6e 6669 670a 2020 2020  tics_config.    
-0000bc90: 2020 2020 2020 2020 7365 6c66 2e65 7870          self.exp
-0000bca0: 6563 7461 7469 6f6e 5f73 7569 7465 203d  ectation_suite =
-0000bcb0: 2065 7870 6563 7461 7469 6f6e 5f73 7569   expectation_sui
-0000bcc0: 7465 0a0a 2020 2020 2020 2020 7365 6c66  te..        self
-0000bcd0: 2e5f 6665 6174 7572 655f 6772 6f75 705f  ._feature_group_
-0000bce0: 656e 6769 6e65 203d 2066 6561 7475 7265  engine = feature
-0000bcf0: 5f67 726f 7570 5f65 6e67 696e 652e 4665  _group_engine.Fe
-0000bd00: 6174 7572 6547 726f 7570 456e 6769 6e65  atureGroupEngine
-0000bd10: 280a 2020 2020 2020 2020 2020 2020 6665  (.            fe
-0000bd20: 6174 7572 6573 746f 7265 5f69 640a 2020  aturestore_id.  
-0000bd30: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000bd40: 7365 6c66 2e5f 6872 6566 203d 2068 7265  self._href = hre
-0000bd50: 660a 0a20 2020 2064 6566 2072 6561 6428  f..    def read(
-0000bd60: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0000bd70: 2020 2020 2020 2077 616c 6c63 6c6f 636b         wallclock
-0000bd80: 5f74 696d 653a 204f 7074 696f 6e61 6c5b  _time: Optional[
-0000bd90: 556e 696f 6e5b 7374 722c 2069 6e74 2c20  Union[str, int, 
-0000bda0: 6461 7465 7469 6d65 2c20 6461 7465 5d5d  datetime, date]]
-0000bdb0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000bdc0: 206f 6e6c 696e 653a 204f 7074 696f 6e61   online: Optiona
-0000bdd0: 6c5b 626f 6f6c 5d20 3d20 4661 6c73 652c  l[bool] = False,
-0000bde0: 0a20 2020 2020 2020 2064 6174 6166 7261  .        datafra
-0000bdf0: 6d65 5f74 7970 653a 204f 7074 696f 6e61  me_type: Optiona
-0000be00: 6c5b 7374 725d 203d 2022 6465 6661 756c  l[str] = "defaul
-0000be10: 7422 2c0a 2020 2020 2020 2020 7265 6164  t",.        read
-0000be20: 5f6f 7074 696f 6e73 3a20 4f70 7469 6f6e  _options: Option
-0000be30: 616c 5b64 6963 745d 203d 207b 7d2c 0a20  al[dict] = {},. 
-0000be40: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-0000be50: 220a 2020 2020 2020 2020 5265 6164 2074  ".        Read t
-0000be60: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
-0000be70: 2069 6e74 6f20 6120 6461 7461 6672 616d   into a datafram
-0000be80: 652e 0a0a 2020 2020 2020 2020 5265 6164  e...        Read
-0000be90: 7320 7468 6520 6665 6174 7572 6520 6772  s the feature gr
-0000bea0: 6f75 7020 6279 2064 6566 6175 6c74 2066  oup by default f
-0000beb0: 726f 6d20 7468 6520 6f66 666c 696e 6520  rom the offline 
-0000bec0: 7374 6f72 6167 6520 6173 2053 7061 726b  storage as Spark
-0000bed0: 2044 6174 6146 7261 6d65 0a20 2020 2020   DataFrame.     
-0000bee0: 2020 206f 6e20 486f 7073 776f 726b 7320     on Hopsworks 
-0000bef0: 616e 6420 4461 7461 6272 6963 6b73 2c20  and Databricks, 
-0000bf00: 616e 6420 6173 2050 616e 6461 7320 6461  and as Pandas da
-0000bf10: 7461 6672 616d 6520 6f6e 2041 5753 2053  taframe on AWS S
-0000bf20: 6167 656d 616b 6572 2061 6e64 2070 7572  agemaker and pur
-0000bf30: 650a 2020 2020 2020 2020 5079 7468 6f6e  e.        Python
-0000bf40: 2065 6e76 6972 6f6e 6d65 6e74 732e 0a0a   environments...
-0000bf50: 2020 2020 2020 2020 5365 7420 606f 6e6c          Set `onl
-0000bf60: 696e 6560 2074 6f20 6054 7275 6560 2074  ine` to `True` t
-0000bf70: 6f20 7265 6164 2066 726f 6d20 7468 6520  o read from the 
-0000bf80: 6f6e 6c69 6e65 2073 746f 7261 6765 2c20  online storage, 
-0000bf90: 6f72 2063 6861 6e67 650a 2020 2020 2020  or change.      
-0000bfa0: 2020 6064 6174 6166 7261 6d65 5f74 7970    `dataframe_typ
-0000bfb0: 6560 2074 6f20 7265 6164 2061 7320 6120  e` to read as a 
-0000bfc0: 6469 6666 6572 656e 7420 666f 726d 6174  different format
-0000bfd0: 2e0a 0a20 2020 2020 2020 2021 2121 2065  ...        !!! e
-0000bfe0: 7861 6d70 6c65 2022 5265 6164 2066 6561  xample "Read fea
-0000bff0: 7475 7265 2067 726f 7570 2061 7320 6f66  ture group as of
-0000c000: 206c 6174 6573 7420 7374 6174 653a 220a   latest state:".
-0000c010: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
-0000c020: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
-0000c030: 2020 2320 636f 6e6e 6563 7420 746f 2074    # connect to t
-0000c040: 6865 2046 6561 7475 7265 2053 746f 7265  he Feature Store
-0000c050: 0a20 2020 2020 2020 2020 2020 2066 7320  .            fs 
-0000c060: 3d20 2e2e 2e0a 0a20 2020 2020 2020 2020  = .....         
-0000c070: 2020 2023 2067 6574 2074 6865 2046 6561     # get the Fea
-0000c080: 7475 7265 2047 726f 7570 2069 6e73 7461  ture Group insta
-0000c090: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
-0000c0a0: 6667 203d 2066 732e 6765 745f 6f72 5f63  fg = fs.get_or_c
-0000c0b0: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
-0000c0c0: 6f75 7028 2e2e 2e29 0a20 2020 2020 2020  oup(...).       
-0000c0d0: 2020 2020 2066 672e 7265 6164 2829 0a20       fg.read(). 
-0000c0e0: 2020 2020 2020 2020 2020 2060 6060 0a0a             ```..
-0000c0f0: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
-0000c100: 706c 6520 2252 6561 6420 6665 6174 7572  ple "Read featur
-0000c110: 6520 6772 6f75 7020 6173 206f 6620 7370  e group as of sp
-0000c120: 6563 6966 6963 2070 6f69 6e74 2069 6e20  ecific point in 
-0000c130: 7469 6d65 3a22 0a20 2020 2020 2020 2020  time:".         
-0000c140: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-0000c150: 2020 2020 2020 2020 2066 6720 3d20 6673           fg = fs
-0000c160: 2e67 6574 5f6f 725f 6372 6561 7465 5f66  .get_or_create_f
-0000c170: 6561 7475 7265 5f67 726f 7570 282e 2e2e  eature_group(...
-0000c180: 290a 2020 2020 2020 2020 2020 2020 6667  ).            fg
-0000c190: 2e72 6561 6428 2232 3032 302d 3130 2d32  .read("2020-10-2
-0000c1a0: 3020 3037 3a33 343a 3131 2229 0a20 2020  0 07:34:11").   
-0000c1b0: 2020 2020 2020 2020 2060 6060 0a0a 2020           ```..  
-0000c1c0: 2020 2020 2020 2320 4172 6775 6d65 6e74        # Argument
-0000c1d0: 730a 2020 2020 2020 2020 2020 2020 7761  s.            wa
-0000c1e0: 6c6c 636c 6f63 6b5f 7469 6d65 3a20 4966  llclock_time: If
-0000c1f0: 2073 7065 6369 6669 6564 2077 696c 6c20   specified will 
-0000c200: 7265 7472 6965 7665 2066 6561 7475 7265  retrieve feature
-0000c210: 2067 726f 7570 2061 7320 6f66 2073 7065   group as of spe
-0000c220: 6369 6669 6320 706f 696e 7420 696e 2074  cific point in t
-0000c230: 696d 652e 2044 6566 6175 6c74 7320 746f  ime. Defaults to
-0000c240: 2060 4e6f 6e65 602e 0a20 2020 2020 2020   `None`..       
-0000c250: 2020 2020 2020 2020 2049 6620 6e6f 7420           If not 
-0000c260: 7370 6563 6966 6965 642c 2077 696c 6c20  specified, will 
-0000c270: 7265 7475 726e 2061 7320 6f66 206d 6f73  return as of mos
-0000c280: 7420 7265 6365 6e74 2074 696d 652e 0a20  t recent time.. 
-0000c290: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0000c2a0: 7472 696e 6773 2073 686f 756c 6420 6265  trings should be
-0000c2b0: 2066 6f72 6d61 7474 6564 2069 6e20 6f6e   formatted in on
-0000c2c0: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
-0000c2d0: 6e67 2066 6f72 6d61 7473 2060 2559 2d25  ng formats `%Y-%
-0000c2e0: 6d2d 2564 602c 2060 2559 2d25 6d2d 2564  m-%d`, `%Y-%m-%d
-0000c2f0: 2025 4860 2c20 6025 592d 256d 2d25 6420   %H`, `%Y-%m-%d 
-0000c300: 2548 3a25 4d60 2c20 6025 592d 256d 2d25  %H:%M`, `%Y-%m-%
-0000c310: 6420 2548 3a25 4d3a 2553 602c 0a20 2020  d %H:%M:%S`,.   
-0000c320: 2020 2020 2020 2020 2020 2020 206f 7220               or 
-0000c330: 6025 592d 256d 2d25 6420 2548 3a25 4d3a  `%Y-%m-%d %H:%M:
-0000c340: 2553 2e25 6660 2e0a 2020 2020 2020 2020  %S.%f`..        
-0000c350: 2020 2020 6f6e 6c69 6e65 3a20 626f 6f6c      online: bool
-0000c360: 2c20 6f70 7469 6f6e 616c 2e20 4966 2060  , optional. If `
-0000c370: 5472 7565 6020 7265 6164 2066 726f 6d20  True` read from 
-0000c380: 6f6e 6c69 6e65 2066 6561 7475 7265 2073  online feature s
-0000c390: 746f 7265 2c20 6465 6661 756c 7473 0a20  tore, defaults. 
-0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000c3b0: 6f20 6046 616c 7365 602e 0a20 2020 2020  o `False`..     
-0000c3c0: 2020 2020 2020 2064 6174 6166 7261 6d65         dataframe
-0000c3d0: 5f74 7970 653a 2073 7472 2c20 6f70 7469  _type: str, opti
-0000c3e0: 6f6e 616c 2e20 506f 7373 6962 6c65 2076  onal. Possible v
-0000c3f0: 616c 7565 7320 6172 6520 6022 6465 6661  alues are `"defa
-0000c400: 756c 7422 602c 2060 2273 7061 726b 2260  ult"`, `"spark"`
-0000c410: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000c420: 2020 6022 7061 6e64 6173 2260 2c20 6022    `"pandas"`, `"
-0000c430: 6e75 6d70 7922 6020 6f72 2060 2270 7974  numpy"` or `"pyt
-0000c440: 686f 6e22 602c 2064 6566 6175 6c74 7320  hon"`, defaults 
-0000c450: 746f 2060 2264 6566 6175 6c74 2260 2e0a  to `"default"`..
-0000c460: 2020 2020 2020 2020 2020 2020 7265 6164              read
-0000c470: 5f6f 7074 696f 6e73 3a20 4164 6469 7469  _options: Additi
-0000c480: 6f6e 616c 206f 7074 696f 6e73 2061 7320  onal options as 
-0000c490: 6b65 792f 7661 6c75 6520 7061 6972 7320  key/value pairs 
-0000c4a0: 746f 2070 6173 7320 746f 2074 6865 2065  to pass to the e
-0000c4b0: 7865 6375 7469 6f6e 2065 6e67 696e 652e  xecution engine.
-0000c4c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c4d0: 2046 6f72 2073 7061 726b 2065 6e67 696e   For spark engin
-0000c4e0: 653a 2044 6963 7469 6f6e 6172 7920 6f66  e: Dictionary of
-0000c4f0: 2072 6561 6420 6f70 7469 6f6e 7320 666f   read options fo
-0000c500: 7220 5370 6172 6b2e 0a20 2020 2020 2020  r Spark..       
-0000c510: 2020 2020 2020 2020 2046 6f72 2070 7974           For pyt
-0000c520: 686f 6e20 656e 6769 6e65 3a0a 2020 2020  hon engine:.    
-0000c530: 2020 2020 2020 2020 2020 2020 2a20 6b65              * ke
-0000c540: 7920 6022 6869 7665 5f63 6f6e 6669 6722  y `"hive_config"
-0000c550: 6020 746f 2070 6173 7320 6120 6469 6374  ` to pass a dict
-0000c560: 696f 6e61 7279 206f 6620 6869 7665 206f  ionary of hive o
-0000c570: 7220 7465 7a20 636f 6e66 6967 7572 6174  r tez configurat
-0000c580: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
-0000c590: 2020 2020 2020 2020 466f 7220 6578 616d          For exam
-0000c5a0: 706c 653a 2060 7b22 6869 7665 5f63 6f6e  ple: `{"hive_con
-0000c5b0: 6669 6722 3a20 7b22 6869 7665 2e74 657a  fig": {"hive.tez
-0000c5c0: 2e63 7075 2e76 636f 7265 7322 3a20 322c  .cpu.vcores": 2,
-0000c5d0: 2022 7465 7a2e 6772 6f75 7069 6e67 2e73   "tez.grouping.s
-0000c5e0: 706c 6974 2d63 6f75 6e74 223a 2022 3322  plit-count": "3"
-0000c5f0: 7d7d 600a 2020 2020 2020 2020 2020 2020  }}`.            
-0000c600: 2020 2020 2a20 6b65 7920 6022 7061 6e64      * key `"pand
-0000c610: 6173 5f74 7970 6573 2260 2061 6e64 2076  as_types"` and v
-0000c620: 616c 7565 2060 5472 7565 6020 746f 2072  alue `True` to r
-0000c630: 6574 7269 6576 6520 636f 6c75 6d6e 7320  etrieve columns 
-0000c640: 6173 2050 616e 6461 7320 6e75 6c6c 6162  as Pandas nullab
-0000c650: 6c65 2074 7970 6573 0a20 2020 2020 2020  le types.       
-0000c660: 2020 2020 2020 2020 2020 2072 6174 6865             rathe
-0000c670: 7220 7468 616e 206e 756d 7079 2f6f 626a  r than numpy/obj
-0000c680: 6563 7428 7374 7269 6e67 2920 7479 7065  ect(string) type
-0000c690: 7320 2865 7870 6572 696d 656e 7461 6c29  s (experimental)
-0000c6a0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c6b0: 2020 2020 2873 6565 2068 7474 7073 3a2f      (see https:/
-0000c6c0: 2f70 616e 6461 732e 7079 6461 7461 2e6f  /pandas.pydata.o
-0000c6d0: 7267 2f64 6f63 732f 7573 6572 5f67 7569  rg/docs/user_gui
-0000c6e0: 6465 2f69 6e74 6567 6572 5f6e 612e 6874  de/integer_na.ht
-0000c6f0: 6d6c 292e 0a20 2020 2020 2020 2020 2020  ml)..           
-0000c700: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-0000c710: 2060 7b7d 602e 0a0a 2020 2020 2020 2020   `{}`...        
-0000c720: 2320 5265 7475 726e 730a 2020 2020 2020  # Returns.      
-0000c730: 2020 2020 2020 6044 6174 6146 7261 6d65        `DataFrame
-0000c740: 603a 2054 6865 2073 7061 726b 2064 6174  `: The spark dat
-0000c750: 6166 7261 6d65 2063 6f6e 7461 696e 696e  aframe containin
-0000c760: 6720 7468 6520 6665 6174 7572 6520 6461  g the feature da
-0000c770: 7461 2e0a 2020 2020 2020 2020 2020 2020  ta..            
-0000c780: 6070 7973 7061 726b 2e44 6174 6146 7261  `pyspark.DataFra
-0000c790: 6d65 602e 2041 2053 7061 726b 2044 6174  me`. A Spark Dat
-0000c7a0: 6146 7261 6d65 2e0a 2020 2020 2020 2020  aFrame..        
-0000c7b0: 2020 2020 6070 616e 6461 732e 4461 7461      `pandas.Data
-0000c7c0: 4672 616d 6560 2e20 4120 5061 6e64 6173  Frame`. A Pandas
-0000c7d0: 2044 6174 6146 7261 6d65 2e0a 2020 2020   DataFrame..    
-0000c7e0: 2020 2020 2020 2020 606e 756d 7079 2e6e          `numpy.n
-0000c7f0: 6461 7272 6179 602e 2041 2074 776f 2d64  darray`. A two-d
-0000c800: 696d 656e 7369 6f6e 616c 204e 756d 7079  imensional Numpy
-0000c810: 2061 7272 6179 2e0a 2020 2020 2020 2020   array..        
-0000c820: 2020 2020 606c 6973 7460 2e20 4120 7477      `list`. A tw
-0000c830: 6f2d 6469 6d65 6e73 696f 6e61 6c20 5079  o-dimensional Py
-0000c840: 7468 6f6e 206c 6973 742e 0a0a 2020 2020  thon list...    
-0000c850: 2020 2020 2320 5261 6973 6573 0a20 2020      # Raises.   
-0000c860: 2020 2020 2020 2020 2060 6873 6673 2e63           `hsfs.c
-0000c870: 6c69 656e 742e 6578 6365 7074 696f 6e73  lient.exceptions
-0000c880: 2e52 6573 7441 5049 4572 726f 7260 2e20  .RestAPIError`. 
-0000c890: 4e6f 2064 6174 6120 6973 2061 7661 696c  No data is avail
-0000c8a0: 6162 6c65 2066 6f72 2066 6561 7475 7265  able for feature
-0000c8b0: 2067 726f 7570 2077 6974 6820 7468 6973   group with this
-0000c8c0: 2063 6f6d 6d69 7420 6461 7465 2c20 4966   commit date, If
-0000c8d0: 2074 696d 6520 7472 6176 656c 2065 6e61   time travel ena
-0000c8e0: 626c 6564 2e0a 2020 2020 2020 2020 2222  bled..        ""
-0000c8f0: 220a 2020 2020 2020 2020 656e 6769 6e65  ".        engine
-0000c900: 2e67 6574 5f69 6e73 7461 6e63 6528 292e  .get_instance().
-0000c910: 7365 745f 6a6f 625f 6772 6f75 7028 0a20  set_job_group(. 
-0000c920: 2020 2020 2020 2020 2020 2022 4665 7463             "Fetc
-0000c930: 6869 6e67 2046 6561 7475 7265 2067 726f  hing Feature gro
-0000c940: 7570 222c 0a20 2020 2020 2020 2020 2020  up",.           
-0000c950: 2022 4765 7474 696e 6720 6665 6174 7572   "Getting featur
-0000c960: 6520 6772 6f75 703a 207b 7d20 6672 6f6d  e group: {} from
-0000c970: 2074 6865 2066 6561 7475 7265 7374 6f72   the featurestor
-0000c980: 6520 7b7d 222e 666f 726d 6174 280a 2020  e {}".format(.  
-0000c990: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000c9a0: 6c66 2e5f 6e61 6d65 2c20 7365 6c66 2e5f  lf._name, self._
-0000c9b0: 6665 6174 7572 655f 7374 6f72 655f 6e61  feature_store_na
-0000c9c0: 6d65 0a20 2020 2020 2020 2020 2020 2029  me.            )
-0000c9d0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0000c9e0: 2020 2020 6966 2077 616c 6c63 6c6f 636b      if wallclock
-0000c9f0: 5f74 696d 653a 0a20 2020 2020 2020 2020  _time:.         
-0000ca00: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
-0000ca10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ca20: 2e73 656c 6563 745f 616c 6c28 290a 2020  .select_all().  
-0000ca30: 2020 2020 2020 2020 2020 2020 2020 2e61                .a
-0000ca40: 735f 6f66 2877 616c 6c63 6c6f 636b 5f74  s_of(wallclock_t
-0000ca50: 696d 6529 0a20 2020 2020 2020 2020 2020  ime).           
-0000ca60: 2020 2020 202e 7265 6164 280a 2020 2020       .read(.    
-0000ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca80: 6f6e 6c69 6e65 2c0a 2020 2020 2020 2020  online,.        
-0000ca90: 2020 2020 2020 2020 2020 2020 6461 7461              data
-0000caa0: 6672 616d 655f 7479 7065 2c0a 2020 2020  frame_type,.    
-0000cab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cac0: 7265 6164 5f6f 7074 696f 6e73 2c0a 2020  read_options,.  
-0000cad0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000cae0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000caf0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000cb00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000cb10: 656c 662e 7365 6c65 6374 5f61 6c6c 2829  elf.select_all()
-0000cb20: 2e72 6561 6428 0a20 2020 2020 2020 2020  .read(.         
-0000cb30: 2020 2020 2020 206f 6e6c 696e 652c 0a20         online,. 
-0000cb40: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000cb50: 6174 6166 7261 6d65 5f74 7970 652c 0a20  ataframe_type,. 
-0000cb60: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000cb70: 6561 645f 6f70 7469 6f6e 732c 0a20 2020  ead_options,.   
-0000cb80: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000cb90: 6465 6620 7265 6164 5f63 6861 6e67 6573  def read_changes
-0000cba0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000cbb0: 2020 2020 2020 2020 7374 6172 745f 7761          start_wa
-0000cbc0: 6c6c 636c 6f63 6b5f 7469 6d65 3a20 556e  llclock_time: Un
-0000cbd0: 696f 6e5b 7374 722c 2069 6e74 2c20 6461  ion[str, int, da
-0000cbe0: 7465 7469 6d65 2c20 6461 7465 5d2c 0a20  tetime, date],. 
-0000cbf0: 2020 2020 2020 2065 6e64 5f77 616c 6c63         end_wallc
-0000cc00: 6c6f 636b 5f74 696d 653a 2055 6e69 6f6e  lock_time: Union
-0000cc10: 5b73 7472 2c20 696e 742c 2064 6174 6574  [str, int, datet
-0000cc20: 696d 652c 2064 6174 655d 2c0a 2020 2020  ime, date],.    
-0000cc30: 2020 2020 7265 6164 5f6f 7074 696f 6e73      read_options
-0000cc40: 3a20 4f70 7469 6f6e 616c 5b64 6963 745d  : Optional[dict]
-0000cc50: 203d 207b 7d2c 0a20 2020 2029 3a0a 2020   = {},.    ):.  
-0000cc60: 2020 2020 2020 2222 2252 6561 6473 2075        """Reads u
-0000cc70: 7064 6174 6573 206f 6620 7468 6973 2066  pdates of this f
-0000cc80: 6561 7475 7265 2074 6861 7420 6f63 6375  eature that occu
-0000cc90: 7272 6564 2062 6574 7765 656e 2073 7065  rred between spe
-0000cca0: 6369 6669 6564 2070 6f69 6e74 7320 696e  cified points in
-0000ccb0: 2074 696d 652e 0a0a 2020 2020 2020 2020   time...        
-0000ccc0: 2121 2120 7761 726e 696e 6720 2244 6570  !!! warning "Dep
-0000ccd0: 7265 6361 7465 6422 0a20 2020 2020 2020  recated".       
-0000cce0: 2020 2020 2020 2020 2020 2020 2060 7265               `re
-0000ccf0: 6164 5f63 6861 6e67 6573 6020 6d65 7468  ad_changes` meth
-0000cd00: 6f64 2069 7320 6465 7072 6563 6174 6564  od is deprecated
-0000cd10: 2e20 5573 650a 2020 2020 2020 2020 2020  . Use.          
-0000cd20: 2020 2020 2020 2020 2020 6061 735f 6f66            `as_of
-0000cd30: 2865 6e64 5f77 616c 6c63 6c6f 636b 5f74  (end_wallclock_t
-0000cd40: 696d 652c 2065 7863 6c75 6465 5f75 6e74  ime, exclude_unt
-0000cd50: 696c 3d73 7461 7274 5f77 616c 6c63 6c6f  il=start_wallclo
-0000cd60: 636b 5f74 696d 6529 2e72 6561 6428 7265  ck_time).read(re
-0000cd70: 6164 5f6f 7074 696f 6e73 3d72 6561 645f  ad_options=read_
-0000cd80: 6f70 7469 6f6e 7329 600a 2020 2020 2020  options)`.      
-0000cd90: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000cda0: 7374 6561 642e 0a0a 2020 2020 2020 2020  stead...        
-0000cdb0: 5468 6973 2066 756e 6374 696f 6e20 6f6e  This function on
-0000cdc0: 6c79 2077 6f72 6b73 206f 6e20 6665 6174  ly works on feat
-0000cdd0: 7572 6520 6772 6f75 7073 2077 6974 6820  ure groups with 
-0000cde0: 6048 5544 4960 2074 696d 6520 7472 6176  `HUDI` time trav
-0000cdf0: 656c 2066 6f72 6d61 742e 0a0a 2020 2020  el format...    
-0000ce00: 2020 2020 2320 4172 6775 6d65 6e74 730a      # Arguments.
-0000ce10: 2020 2020 2020 2020 2020 2020 7374 6172              star
-0000ce20: 745f 7761 6c6c 636c 6f63 6b5f 7469 6d65  t_wallclock_time
-0000ce30: 3a20 5374 6172 7420 7469 6d65 206f 6620  : Start time of 
-0000ce40: 7468 6520 7469 6d65 2074 7261 7665 6c20  the time travel 
-0000ce50: 7175 6572 792e 2053 7472 696e 6773 2073  query. Strings s
-0000ce60: 686f 756c 6420 6265 2066 6f72 6d61 7474  hould be formatt
-0000ce70: 6564 2069 6e20 6f6e 6520 6f66 2074 6865  ed in one of the
-0000ce80: 2066 6f6c 6c6f 7769 6e67 2066 6f72 6d61   following forma
-0000ce90: 7473 2060 2559 2d25 6d2d 2564 602c 2060  ts `%Y-%m-%d`, `
-0000cea0: 2559 2d25 6d2d 2564 2025 4860 2c20 6025  %Y-%m-%d %H`, `%
-0000ceb0: 592d 256d 2d25 6420 2548 3a25 4d60 2c0a  Y-%m-%d %H:%M`,.
-0000cec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ced0: 6025 592d 256d 2d25 6420 2548 3a25 4d3a  `%Y-%m-%d %H:%M:
-0000cee0: 2553 602c 206f 7220 6025 592d 256d 2d25  %S`, or `%Y-%m-%
-0000cef0: 6420 2548 3a25 4d3a 2553 2e25 6660 2e0a  d %H:%M:%S.%f`..
-0000cf00: 2020 2020 2020 2020 2020 2020 656e 645f              end_
-0000cf10: 7761 6c6c 636c 6f63 6b5f 7469 6d65 3a20  wallclock_time: 
-0000cf20: 456e 6420 7469 6d65 206f 6620 7468 6520  End time of the 
-0000cf30: 7469 6d65 2074 7261 7665 6c20 7175 6572  time travel quer
-0000cf40: 792e 2053 7472 696e 6773 2073 686f 756c  y. Strings shoul
-0000cf50: 6420 6265 2066 6f72 6d61 7474 6564 2069  d be formatted i
-0000cf60: 6e20 6f6e 6520 6f66 2074 6865 2066 6f6c  n one of the fol
-0000cf70: 6c6f 7769 6e67 2066 6f72 6d61 7473 2060  lowing formats `
-0000cf80: 2559 2d25 6d2d 2564 602c 2060 2559 2d25  %Y-%m-%d`, `%Y-%
-0000cf90: 6d2d 2564 2025 4860 2c20 6025 592d 256d  m-%d %H`, `%Y-%m
-0000cfa0: 2d25 6420 2548 3a25 4d60 2c0a 2020 2020  -%d %H:%M`,.    
-0000cfb0: 2020 2020 2020 2020 2020 2020 6025 592d              `%Y-
-0000cfc0: 256d 2d25 6420 2548 3a25 4d3a 2553 602c  %m-%d %H:%M:%S`,
-0000cfd0: 206f 7220 6025 592d 256d 2d25 6420 2548   or `%Y-%m-%d %H
-0000cfe0: 3a25 4d3a 2553 2e25 6660 2e0a 2020 2020  :%M:%S.%f`..    
-0000cff0: 2020 2020 2020 2020 7265 6164 5f6f 7074          read_opt
-0000d000: 696f 6e73 3a20 4164 6469 7469 6f6e 616c  ions: Additional
-0000d010: 206f 7074 696f 6e73 2061 7320 6b65 792f   options as key/
-0000d020: 7661 6c75 6520 7061 6972 7320 746f 2070  value pairs to p
-0000d030: 6173 7320 746f 2074 6865 2065 7865 6375  ass to the execu
-0000d040: 7469 6f6e 2065 6e67 696e 652e 0a20 2020  tion engine..   
-0000d050: 2020 2020 2020 2020 2020 2020 2046 6f72               For
-0000d060: 2073 7061 726b 2065 6e67 696e 653a 2044   spark engine: D
-0000d070: 6963 7469 6f6e 6172 7920 6f66 2072 6561  ictionary of rea
-0000d080: 6420 6f70 7469 6f6e 7320 666f 7220 5370  d options for Sp
-0000d090: 6172 6b2e 0a20 2020 2020 2020 2020 2020  ark..           
-0000d0a0: 2020 2020 2046 6f72 2070 7974 686f 6e20       For python 
-0000d0b0: 656e 6769 6e65 3a0a 2020 2020 2020 2020  engine:.        
-0000d0c0: 2020 2020 2020 2020 2a20 6b65 7920 6022          * key `"
-0000d0d0: 6869 7665 5f63 6f6e 6669 6722 6020 746f  hive_config"` to
-0000d0e0: 2070 6173 7320 6120 6469 6374 696f 6e61   pass a dictiona
-0000d0f0: 7279 206f 6620 6869 7665 206f 7220 7465  ry of hive or te
-0000d100: 7a20 636f 6e66 6967 7572 6174 696f 6e73  z configurations
-0000d110: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d120: 2020 2020 466f 7220 6578 616d 706c 653a      For example:
-0000d130: 2060 7b22 6869 7665 5f63 6f6e 6669 6722   `{"hive_config"
-0000d140: 3a20 7b22 6869 7665 2e74 657a 2e63 7075  : {"hive.tez.cpu
-0000d150: 2e76 636f 7265 7322 3a20 322c 2022 7465  .vcores": 2, "te
-0000d160: 7a2e 6772 6f75 7069 6e67 2e73 706c 6974  z.grouping.split
-0000d170: 2d63 6f75 6e74 223a 2022 3322 7d7d 600a  -count": "3"}}`.
-0000d180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d190: 4465 6661 756c 7473 2074 6f20 607b 7d60  Defaults to `{}`
-0000d1a0: 2e0a 0a20 2020 2020 2020 2023 2052 6574  ...        # Ret
-0000d1b0: 7572 6e73 0a20 2020 2020 2020 2020 2020  urns.           
-0000d1c0: 2060 4461 7461 4672 616d 6560 2e20 5468   `DataFrame`. Th
-0000d1d0: 6520 7370 6172 6b20 6461 7461 6672 616d  e spark datafram
-0000d1e0: 6520 636f 6e74 6169 6e69 6e67 2074 6865  e containing the
-0000d1f0: 2069 6e63 7265 6d65 6e74 616c 2063 6861   incremental cha
-0000d200: 6e67 6573 206f 660a 2020 2020 2020 2020  nges of.        
-0000d210: 2020 2020 6665 6174 7572 6520 6461 7461      feature data
-0000d220: 2e0a 0a20 2020 2020 2020 2023 2052 6169  ...        # Rai
-0000d230: 7365 730a 2020 2020 2020 2020 2020 2020  ses.            
-0000d240: 6068 7366 732e 636c 6965 6e74 2e65 7863  `hsfs.client.exc
-0000d250: 6570 7469 6f6e 732e 5265 7374 4150 4945  eptions.RestAPIE
-0000d260: 7272 6f72 602e 2020 4e6f 2064 6174 6120  rror`.  No data 
-0000d270: 6973 2061 7661 696c 6162 6c65 2066 6f72  is available for
-0000d280: 2066 6561 7475 7265 2067 726f 7570 2077   feature group w
-0000d290: 6974 6820 7468 6973 2063 6f6d 6d69 7420  ith this commit 
-0000d2a0: 6461 7465 2e0a 2020 2020 2020 2020 2020  date..          
-0000d2b0: 2020 6068 7366 732e 636c 6965 6e74 2e65    `hsfs.client.e
-0000d2c0: 7863 6570 7469 6f6e 732e 4665 6174 7572  xceptions.Featur
-0000d2d0: 6553 746f 7265 4578 6365 7074 696f 6e60  eStoreException`
-0000d2e0: 2e20 4966 2074 6865 2066 6561 7475 7265  . If the feature
-0000d2f0: 2067 726f 7570 2064 6f65 7320 6e6f 7420   group does not 
-0000d300: 6861 7665 2060 4855 4449 6020 7469 6d65  have `HUDI` time
-0000d310: 2074 7261 7665 6c20 666f 726d 6174 0a20   travel format. 
-0000d320: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000d330: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
-0000d340: 2020 2020 2020 2020 7365 6c66 2e73 656c          self.sel
-0000d350: 6563 745f 616c 6c28 290a 2020 2020 2020  ect_all().      
-0000d360: 2020 2020 2020 2e70 756c 6c5f 6368 616e        .pull_chan
-0000d370: 6765 7328 7374 6172 745f 7761 6c6c 636c  ges(start_wallcl
-0000d380: 6f63 6b5f 7469 6d65 2c20 656e 645f 7761  ock_time, end_wa
-0000d390: 6c6c 636c 6f63 6b5f 7469 6d65 290a 2020  llclock_time).  
-0000d3a0: 2020 2020 2020 2020 2020 2e72 6561 6428            .read(
-0000d3b0: 4661 6c73 652c 2022 6465 6661 756c 7422  False, "default"
-0000d3c0: 2c20 7265 6164 5f6f 7074 696f 6e73 290a  , read_options).
-0000d3d0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-0000d3e0: 6566 2073 686f 7728 7365 6c66 2c20 6e3a  ef show(self, n:
-0000d3f0: 2069 6e74 2c20 6f6e 6c69 6e65 3a20 4f70   int, online: Op
-0000d400: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2046  tional[bool] = F
-0000d410: 616c 7365 293a 0a20 2020 2020 2020 2022  alse):.        "
-0000d420: 2222 5368 6f77 2074 6865 2066 6972 7374  ""Show the first
-0000d430: 2060 6e60 2072 6f77 7320 6f66 2074 6865   `n` rows of the
-0000d440: 2066 6561 7475 7265 2067 726f 7570 2e0a   feature group..
-0000d450: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
-0000d460: 6d70 6c65 0a20 2020 2020 2020 2020 2020  mple.           
-0000d470: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
-0000d480: 2020 2020 2020 2023 2063 6f6e 6e65 6374         # connect
-0000d490: 2074 6f20 7468 6520 4665 6174 7572 6520   to the Feature 
-0000d4a0: 5374 6f72 650a 2020 2020 2020 2020 2020  Store.          
-0000d4b0: 2020 6673 203d 202e 2e2e 0a0a 2020 2020    fs = .....    
-0000d4c0: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
-0000d4d0: 6520 4665 6174 7572 6520 4772 6f75 7020  e Feature Group 
-0000d4e0: 696e 7374 616e 6365 0a20 2020 2020 2020  instance.       
-0000d4f0: 2020 2020 2066 6720 3d20 6673 2e67 6574       fg = fs.get
-0000d500: 5f6f 725f 6372 6561 7465 5f66 6561 7475  _or_create_featu
-0000d510: 7265 5f67 726f 7570 282e 2e2e 290a 0a20  re_group(...).. 
-0000d520: 2020 2020 2020 2020 2020 2023 206d 616b             # mak
-0000d530: 6520 6120 7175 6572 7920 616e 6420 7368  e a query and sh
-0000d540: 6f77 2074 6f70 2035 2072 6f77 730a 2020  ow top 5 rows.  
-0000d550: 2020 2020 2020 2020 2020 6667 2e73 656c            fg.sel
-0000d560: 6563 7428 5b27 6461 7465 272c 2777 6565  ect(['date','wee
-0000d570: 6b6c 795f 7361 6c65 7327 2c27 6973 5f68  kly_sales','is_h
-0000d580: 6f6c 6964 6179 275d 292e 7368 6f77 2835  oliday']).show(5
-0000d590: 290a 2020 2020 2020 2020 2020 2020 6060  ).            ``
-0000d5a0: 600a 0a20 2020 2020 2020 2023 2041 7267  `..        # Arg
-0000d5b0: 756d 656e 7473 0a20 2020 2020 2020 2020  uments.         
-0000d5c0: 2020 206e 3a20 696e 742e 204e 756d 6265     n: int. Numbe
-0000d5d0: 7220 6f66 2072 6f77 7320 746f 2073 686f  r of rows to sho
-0000d5e0: 772e 0a20 2020 2020 2020 2020 2020 206f  w..            o
-0000d5f0: 6e6c 696e 653a 2062 6f6f 6c2c 206f 7074  nline: bool, opt
-0000d600: 696f 6e61 6c2e 2049 6620 6054 7275 6560  ional. If `True`
-0000d610: 2072 6561 6420 6672 6f6d 206f 6e6c 696e   read from onlin
-0000d620: 6520 6665 6174 7572 6520 7374 6f72 652c  e feature store,
-0000d630: 2064 6566 6175 6c74 730a 2020 2020 2020   defaults.      
-0000d640: 2020 2020 2020 2020 2020 746f 2060 4661            to `Fa
-0000d650: 6c73 6560 2e0a 2020 2020 2020 2020 2222  lse`..        ""
-0000d660: 220a 2020 2020 2020 2020 656e 6769 6e65  ".        engine
-0000d670: 2e67 6574 5f69 6e73 7461 6e63 6528 292e  .get_instance().
-0000d680: 7365 745f 6a6f 625f 6772 6f75 7028 0a20  set_job_group(. 
-0000d690: 2020 2020 2020 2020 2020 2022 4665 7463             "Fetc
-0000d6a0: 6869 6e67 2046 6561 7475 7265 2067 726f  hing Feature gro
-0000d6b0: 7570 222c 0a20 2020 2020 2020 2020 2020  up",.           
-0000d6c0: 2022 4765 7474 696e 6720 6665 6174 7572   "Getting featur
-0000d6d0: 6520 6772 6f75 703a 207b 7d20 6672 6f6d  e group: {} from
-0000d6e0: 2074 6865 2066 6561 7475 7265 7374 6f72   the featurestor
-0000d6f0: 6520 7b7d 222e 666f 726d 6174 280a 2020  e {}".format(.  
-0000d700: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d710: 6c66 2e5f 6e61 6d65 2c20 7365 6c66 2e5f  lf._name, self._
-0000d720: 6665 6174 7572 655f 7374 6f72 655f 6e61  feature_store_na
-0000d730: 6d65 0a20 2020 2020 2020 2020 2020 2029  me.            )
-0000d740: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0000d750: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000d760: 7365 6c65 6374 5f61 6c6c 2829 2e73 686f  select_all().sho
-0000d770: 7728 6e2c 206f 6e6c 696e 6529 0a0a 2020  w(n, online)..  
-0000d780: 2020 6465 6620 7361 7665 280a 2020 2020    def save(.    
-0000d790: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000d7a0: 2020 6665 6174 7572 6573 3a20 556e 696f    features: Unio
-0000d7b0: 6e5b 0a20 2020 2020 2020 2020 2020 2070  n[.            p
-0000d7c0: 642e 4461 7461 4672 616d 652c 0a20 2020  d.DataFrame,.   
-0000d7d0: 2020 2020 2020 2020 2054 7970 6556 6172           TypeVar
-0000d7e0: 2822 7079 7370 6172 6b2e 7371 6c2e 4461  ("pyspark.sql.Da
-0000d7f0: 7461 4672 616d 6522 292c 2020 2320 6e6f  taFrame"),  # no
-0000d800: 7161 3a20 4638 3231 0a20 2020 2020 2020  qa: F821.       
-0000d810: 2020 2020 2054 7970 6556 6172 2822 7079       TypeVar("py
-0000d820: 7370 6172 6b2e 5244 4422 292c 2020 2320  spark.RDD"),  # 
-0000d830: 6e6f 7161 3a20 4638 3231 0a20 2020 2020  noqa: F821.     
-0000d840: 2020 2020 2020 206e 702e 6e64 6172 7261         np.ndarra
-0000d850: 792c 0a20 2020 2020 2020 2020 2020 204c  y,.            L
-0000d860: 6973 745b 6c69 7374 5d2c 0a20 2020 2020  ist[list],.     
-0000d870: 2020 205d 2c0a 2020 2020 2020 2020 7772     ],.        wr
-0000d880: 6974 655f 6f70 7469 6f6e 733a 204f 7074  ite_options: Opt
-0000d890: 696f 6e61 6c5b 4469 6374 5b41 6e79 2c20  ional[Dict[Any, 
-0000d8a0: 416e 795d 5d20 3d20 7b7d 2c0a 2020 2020  Any]] = {},.    
-0000d8b0: 2020 2020 7661 6c69 6461 7469 6f6e 5f6f      validation_o
-0000d8c0: 7074 696f 6e73 3a20 4f70 7469 6f6e 616c  ptions: Optional
-0000d8d0: 5b44 6963 745b 416e 792c 2041 6e79 5d5d  [Dict[Any, Any]]
-0000d8e0: 203d 207b 7d2c 0a20 2020 2029 3a0a 2020   = {},.    ):.  
-0000d8f0: 2020 2020 2020 2222 2250 6572 7369 7374        """Persist
-0000d900: 2074 6865 206d 6574 6164 6174 6120 616e   the metadata an
-0000d910: 6420 6d61 7465 7269 616c 697a 6520 7468  d materialize th
-0000d920: 6520 6665 6174 7572 6520 6772 6f75 7020  e feature group 
-0000d930: 746f 2074 6865 2066 6561 7475 7265 2073  to the feature s
-0000d940: 746f 7265 2e0a 0a20 2020 2020 2020 2021  tore...        !
-0000d950: 2121 2077 6172 6e69 6e67 2022 4465 7072  !! warning "Depr
-0000d960: 6563 6174 6564 220a 2020 2020 2020 2020  ecated".        
-0000d970: 2020 2020 6073 6176 6560 206d 6574 686f      `save` metho
-0000d980: 6420 6973 2064 6570 7265 6361 7465 642e  d is deprecated.
-0000d990: 2055 7365 2074 6865 2060 696e 7365 7274   Use the `insert
-0000d9a0: 6020 6d65 7468 6f64 2069 6e73 7465 6164  ` method instead
-0000d9b0: 2e0a 0a20 2020 2020 2020 2043 616c 6c69  ...        Calli
-0000d9c0: 6e67 2060 7361 7665 6020 6372 6561 7465  ng `save` create
-0000d9d0: 7320 7468 6520 6d65 7461 6461 7461 2066  s the metadata f
-0000d9e0: 6f72 2074 6865 2066 6561 7475 7265 2067  or the feature g
-0000d9f0: 726f 7570 2069 6e20 7468 6520 6665 6174  roup in the feat
-0000da00: 7572 6520 7374 6f72 650a 2020 2020 2020  ure store.      
-0000da10: 2020 616e 6420 7772 6974 6573 2074 6865    and writes the
-0000da20: 2073 7065 6369 6669 6564 2060 6665 6174   specified `feat
-0000da30: 7572 6573 6020 6461 7461 6672 616d 6520  ures` dataframe 
-0000da40: 6173 2066 6561 7475 7265 2067 726f 7570  as feature group
-0000da50: 2074 6f20 7468 650a 2020 2020 2020 2020   to the.        
-0000da60: 6f6e 6c69 6e65 2f6f 6666 6c69 6e65 2066  online/offline f
-0000da70: 6561 7475 7265 2073 746f 7265 2061 7320  eature store as 
-0000da80: 7370 6563 6966 6965 642e 0a20 2020 2020  specified..     
-0000da90: 2020 2042 7920 6465 6661 756c 742c 2074     By default, t
-0000daa0: 6869 7320 7772 6974 6573 2074 6865 2066  his writes the f
-0000dab0: 6561 7475 7265 2067 726f 7570 2074 6f20  eature group to 
-0000dac0: 7468 6520 6f66 666c 696e 6520 7374 6f72  the offline stor
-0000dad0: 6167 652c 2061 6e64 2069 660a 2020 2020  age, and if.    
-0000dae0: 2020 2020 606f 6e6c 696e 655f 656e 6162      `online_enab
-0000daf0: 6c65 6460 2066 6f72 2074 6865 2066 6561  led` for the fea
-0000db00: 7475 7265 2067 726f 7570 2c20 616c 736f  ture group, also
-0000db10: 2074 6f20 7468 6520 6f6e 6c69 6e65 2066   to the online f
-0000db20: 6561 7475 7265 2073 746f 7265 2e0a 2020  eature store..  
-0000db30: 2020 2020 2020 5468 6520 6066 6561 7475        The `featu
-0000db40: 7265 7360 2064 6174 6166 7261 6d65 2063  res` dataframe c
-0000db50: 616e 2062 6520 6120 5370 6172 6b20 4461  an be a Spark Da
-0000db60: 7461 4672 616d 6520 6f72 2052 4444 2c20  taFrame or RDD, 
-0000db70: 6120 5061 6e64 6173 2044 6174 6146 7261  a Pandas DataFra
-0000db80: 6d65 2c0a 2020 2020 2020 2020 6f72 2061  me,.        or a
-0000db90: 2074 776f 2d64 696d 656e 7369 6f6e 616c   two-dimensional
-0000dba0: 204e 756d 7079 2061 7272 6179 206f 7220   Numpy array or 
-0000dbb0: 6120 7477 6f2d 6469 6d65 6e73 696f 6e61  a two-dimensiona
-0000dbc0: 6c20 5079 7468 6f6e 206e 6573 7465 6420  l Python nested 
-0000dbd0: 6c69 7374 2e0a 2020 2020 2020 2020 2320  list..        # 
-0000dbe0: 4172 6775 6d65 6e74 730a 2020 2020 2020  Arguments.      
-0000dbf0: 2020 2020 2020 6665 6174 7572 6573 3a20        features: 
-0000dc00: 5175 6572 792c 2044 6174 6146 7261 6d65  Query, DataFrame
-0000dc10: 2c20 5244 442c 204e 6461 7272 6179 2c20  , RDD, Ndarray, 
-0000dc20: 6c69 7374 2e20 4665 6174 7572 6573 2074  list. Features t
-0000dc30: 6f20 6265 2073 6176 6564 2e0a 2020 2020  o be saved..    
-0000dc40: 2020 2020 2020 2020 7772 6974 655f 6f70          write_op
-0000dc50: 7469 6f6e 733a 2041 6464 6974 696f 6e61  tions: Additiona
-0000dc60: 6c20 7772 6974 6520 6f70 7469 6f6e 7320  l write options 
-0000dc70: 6173 206b 6579 2d76 616c 7565 2070 6169  as key-value pai
-0000dc80: 7273 2c20 6465 6661 756c 7473 2074 6f20  rs, defaults to 
-0000dc90: 607b 7d60 2e0a 2020 2020 2020 2020 2020  `{}`..          
-0000dca0: 2020 2020 2020 5768 656e 2075 7369 6e67        When using
-0000dcb0: 2074 6865 2060 7079 7468 6f6e 6020 656e   the `python` en
-0000dcc0: 6769 6e65 2c20 7772 6974 655f 6f70 7469  gine, write_opti
-0000dcd0: 6f6e 7320 6361 6e20 636f 6e74 6169 6e20  ons can contain 
-0000dce0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-0000dcf0: 2020 2020 666f 6c6c 6f77 696e 6720 656e      following en
-0000dd00: 7472 6965 733a 0a20 2020 2020 2020 2020  tries:.         
-0000dd10: 2020 2020 2020 202a 206b 6579 2060 7370         * key `sp
-0000dd20: 6172 6b60 2061 6e64 2076 616c 7565 2061  ark` and value a
-0000dd30: 6e20 6f62 6a65 6374 206f 6620 7479 7065  n object of type
-0000dd40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dd50: 205b 6873 6673 2e63 6f72 652e 6a6f 625f   [hsfs.core.job_
-0000dd60: 636f 6e66 6967 7572 6174 696f 6e2e 4a6f  configuration.Jo
-0000dd70: 6243 6f6e 6669 6775 7261 7469 6f6e 5d28  bConfiguration](
-0000dd80: 2e2e 2f6a 6f62 5f63 6f6e 6669 6775 7261  ../job_configura
-0000dd90: 7469 6f6e 290a 2020 2020 2020 2020 2020  tion).          
-0000dda0: 2020 2020 2020 2020 746f 2063 6f6e 6669          to confi
-0000ddb0: 6775 7265 2074 6865 2048 6f70 7377 6f72  gure the Hopswor
-0000ddc0: 6b73 204a 6f62 2075 7365 6420 746f 2077  ks Job used to w
-0000ddd0: 7269 7465 2064 6174 6120 696e 746f 2074  rite data into t
-0000dde0: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
-0000ddf0: 2020 2020 2066 6561 7475 7265 2067 726f       feature gro
-0000de00: 7570 2e0a 2020 2020 2020 2020 2020 2020  up..            
-0000de10: 2020 2020 2a20 6b65 7920 6077 6169 745f      * key `wait_
-0000de20: 666f 725f 6a6f 6260 2061 6e64 2076 616c  for_job` and val
-0000de30: 7565 2060 5472 7565 6020 6f72 2060 4661  ue `True` or `Fa
-0000de40: 6c73 6560 2074 6f20 636f 6e66 6967 7572  lse` to configur
-0000de50: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000de60: 2020 2020 7768 6574 6865 7220 6f72 206e      whether or n
-0000de70: 6f74 2074 6f20 7468 6520 7361 7665 2063  ot to the save c
-0000de80: 616c 6c20 7368 6f75 6c64 2072 6574 7572  all should retur
-0000de90: 6e20 6f6e 6c79 0a20 2020 2020 2020 2020  n only.         
-0000dea0: 2020 2020 2020 2020 2061 6674 6572 2074           after t
-0000deb0: 6865 2048 6f70 7377 6f72 6b73 204a 6f62  he Hopsworks Job
-0000dec0: 2068 6173 2066 696e 6973 6865 642e 2042   has finished. B
-0000ded0: 7920 6465 6661 756c 7420 6974 2077 6169  y default it wai
-0000dee0: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
-0000def0: 2020 2020 2a20 6b65 7920 6073 7461 7274      * key `start
-0000df00: 5f6f 6666 6c69 6e65 5f62 6163 6b66 696c  _offline_backfil
-0000df10: 6c60 2061 6e64 2076 616c 7565 2060 5472  l` and value `Tr
-0000df20: 7565 6020 6f72 2060 4661 6c73 6560 2074  ue` or `False` t
-0000df30: 6f20 636f 6e66 6967 7572 650a 2020 2020  o configure.    
-0000df40: 2020 2020 2020 2020 2020 2020 2020 7768                wh
-0000df50: 6574 6865 7220 6f72 206e 6f74 2074 6f20  ether or not to 
-0000df60: 7374 6172 7420 7468 6520 6261 636b 6669  start the backfi
-0000df70: 6c6c 206a 6f62 2074 6f20 7772 6974 6520  ll job to write 
-0000df80: 6461 7461 2074 6f20 7468 6520 6f66 666c  data to the offl
-0000df90: 696e 650a 2020 2020 2020 2020 2020 2020  ine.            
-0000dfa0: 2020 2020 2020 7374 6f72 6167 652e 2042        storage. B
-0000dfb0: 7920 6465 6661 756c 7420 7468 6520 6261  y default the ba
-0000dfc0: 636b 6669 6c6c 206a 6f62 2067 6574 7320  ckfill job gets 
-0000dfd0: 7374 6172 7465 6420 696d 6d65 6469 6174  started immediat
-0000dfe0: 656c 792e 0a20 2020 2020 2020 2020 2020  ely..           
-0000dff0: 2020 2020 202a 206b 6579 2060 696e 7465       * key `inte
-0000e000: 726e 616c 5f6b 6166 6b61 6020 616e 6420  rnal_kafka` and 
-0000e010: 7661 6c75 6520 6054 7275 6560 206f 7220  value `True` or 
-0000e020: 6046 616c 7365 6020 696e 2063 6173 6520  `False` in case 
-0000e030: 796f 7520 6573 7461 626c 6973 6865 640a  you established.
-0000e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e050: 2020 636f 6e6e 6563 7469 7669 7479 2066    connectivity f
-0000e060: 726f 6d20 796f 7520 5079 7468 6f6e 2065  rom you Python e
-0000e070: 6e76 6972 6f6e 6d65 6e74 2074 6f20 7468  nvironment to th
-0000e080: 6520 696e 7465 726e 616c 2061 6476 6572  e internal adver
-0000e090: 7469 7365 640a 2020 2020 2020 2020 2020  tised.          
-0000e0a0: 2020 2020 2020 2020 6c69 7374 656e 6572          listener
-0000e0b0: 7320 6f66 2074 6865 2048 6f70 7377 6f72  s of the Hopswor
-0000e0c0: 6b73 204b 6166 6b61 2043 6c75 7374 6572  ks Kafka Cluster
-0000e0d0: 2e20 4465 6661 756c 7473 2074 6f20 6046  . Defaults to `F
-0000e0e0: 616c 7365 6020 616e 640a 2020 2020 2020  alse` and.      
-0000e0f0: 2020 2020 2020 2020 2020 2020 7769 6c6c              will
-0000e100: 2075 7365 2065 7874 6572 6e61 6c20 6c69   use external li
-0000e110: 7374 656e 6572 7320 7768 656e 2063 6f6e  steners when con
-0000e120: 6e65 6374 696e 6720 6672 6f6d 206f 7574  necting from out
-0000e130: 7369 6465 206f 6620 486f 7073 776f 726b  side of Hopswork
-0000e140: 732e 0a20 2020 2020 2020 2020 2020 2076  s..            v
-0000e150: 616c 6964 6174 696f 6e5f 6f70 7469 6f6e  alidation_option
-0000e160: 733a 2041 6464 6974 696f 6e61 6c20 7661  s: Additional va
-0000e170: 6c69 6461 7469 6f6e 206f 7074 696f 6e73  lidation options
-0000e180: 2061 7320 6b65 792d 7661 6c75 6520 7061   as key-value pa
-0000e190: 6972 732c 2064 6566 6175 6c74 7320 746f  irs, defaults to
-0000e1a0: 2060 7b7d 602e 0a20 2020 2020 2020 2020   `{}`..         
-0000e1b0: 2020 2020 2020 202a 206b 6579 2060 7275         * key `ru
-0000e1c0: 6e5f 7661 6c69 6461 7469 6f6e 6020 626f  n_validation` bo
-0000e1d0: 6f6c 6561 6e20 7661 6c75 652c 2073 6574  olean value, set
-0000e1e0: 2074 6f20 6046 616c 7365 6020 746f 2073   to `False` to s
-0000e1f0: 6b69 7020 7661 6c69 6461 7469 6f6e 2074  kip validation t
-0000e200: 656d 706f 7261 7269 6c79 206f 6e20 696e  emporarily on in
-0000e210: 6765 7374 696f 6e2e 0a20 2020 2020 2020  gestion..       
-0000e220: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
-0000e230: 7361 7665 5f72 6570 6f72 7460 2062 6f6f  save_report` boo
-0000e240: 6c65 616e 2076 616c 7565 2c20 7365 7420  lean value, set 
-0000e250: 746f 2060 4661 6c73 6560 2074 6f20 736b  to `False` to sk
-0000e260: 6970 2075 706c 6f61 6420 6f66 2074 6865  ip upload of the
-0000e270: 2076 616c 6964 6174 696f 6e20 7265 706f   validation repo
-0000e280: 7274 2074 6f20 486f 7073 776f 726b 732e  rt to Hopsworks.
-0000e290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e2a0: 202a 206b 6579 2060 6765 5f76 616c 6964   * key `ge_valid
-0000e2b0: 6174 655f 6b77 6172 6773 6020 6120 6469  ate_kwargs` a di
-0000e2c0: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
-0000e2d0: 696e 6720 6b77 6172 6773 2066 6f72 2074  ing kwargs for t
-0000e2e0: 6865 2076 616c 6964 6174 6520 6d65 7468  he validate meth
-0000e2f0: 6f64 206f 6620 4772 6561 7420 4578 7065  od of Great Expe
-0000e300: 6374 6174 696f 6e73 2e0a 0a20 2020 2020  ctations...     
-0000e310: 2020 2023 2052 6574 7572 6e73 0a20 2020     # Returns.   
-0000e320: 2020 2020 2020 2020 2060 4a6f 6260 3a20           `Job`: 
-0000e330: 5768 656e 2075 7369 6e67 2074 6865 2060  When using the `
-0000e340: 7079 7468 6f6e 6020 656e 6769 6e65 2c20  python` engine, 
-0000e350: 6974 2072 6574 7572 6e73 2074 6865 2048  it returns the H
-0000e360: 6f70 7377 6f72 6b73 204a 6f62 0a20 2020  opsworks Job.   
-0000e370: 2020 2020 2020 2020 2020 2020 2074 6861               tha
-0000e380: 7420 7761 7320 6c61 756e 6368 6564 2074  t was launched t
-0000e390: 6f20 696e 6765 7374 2074 6865 2066 6561  o ingest the fea
-0000e3a0: 7475 7265 2067 726f 7570 2064 6174 612e  ture group data.
-0000e3b0: 0a0a 2020 2020 2020 2020 2320 5261 6973  ..        # Rais
-0000e3c0: 6573 0a20 2020 2020 2020 2020 2020 2060  es.            `
-0000e3d0: 6873 6673 2e63 6c69 656e 742e 6578 6365  hsfs.client.exce
-0000e3e0: 7074 696f 6e73 2e52 6573 7441 5049 4572  ptions.RestAPIEr
-0000e3f0: 726f 7260 2e20 556e 6162 6c65 2074 6f20  ror`. Unable to 
-0000e400: 6372 6561 7465 2066 6561 7475 7265 2067  create feature g
-0000e410: 726f 7570 2e0a 2020 2020 2020 2020 2222  roup..        ""
-0000e420: 220a 2020 2020 2020 2020 6665 6174 7572  ".        featur
-0000e430: 655f 6461 7461 6672 616d 6520 3d20 656e  e_dataframe = en
-0000e440: 6769 6e65 2e67 6574 5f69 6e73 7461 6e63  gine.get_instanc
-0000e450: 6528 292e 636f 6e76 6572 745f 746f 5f64  e().convert_to_d
-0000e460: 6566 6175 6c74 5f64 6174 6166 7261 6d65  efault_dataframe
-0000e470: 2866 6561 7475 7265 7329 0a0a 2020 2020  (features)..    
-0000e480: 2020 2020 7573 6572 5f76 6572 7369 6f6e      user_version
-0000e490: 203d 2073 656c 662e 5f76 6572 7369 6f6e   = self._version
-0000e4a0: 0a0a 2020 2020 2020 2020 2320 6667 5f6a  ..        # fg_j
-0000e4b0: 6f62 2069 7320 7573 6564 206f 6e6c 7920  ob is used only 
-0000e4c0: 6966 2074 6865 2070 7974 686f 6e20 656e  if the python en
-0000e4d0: 6769 6e65 2069 7320 7573 6564 0a20 2020  gine is used.   
-0000e4e0: 2020 2020 2066 675f 6a6f 622c 2067 655f       fg_job, ge_
-0000e4f0: 7265 706f 7274 203d 2073 656c 662e 5f66  report = self._f
-0000e500: 6561 7475 7265 5f67 726f 7570 5f65 6e67  eature_group_eng
-0000e510: 696e 652e 7361 7665 280a 2020 2020 2020  ine.save(.      
-0000e520: 2020 2020 2020 7365 6c66 2c20 6665 6174        self, feat
-0000e530: 7572 655f 6461 7461 6672 616d 652c 2077  ure_dataframe, w
-0000e540: 7269 7465 5f6f 7074 696f 6e73 2c20 7661  rite_options, va
-0000e550: 6c69 6461 7469 6f6e 5f6f 7074 696f 6e73  lidation_options
-0000e560: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000e570: 2020 2069 6620 6765 5f72 6570 6f72 7420     if ge_report 
-0000e580: 6973 204e 6f6e 6520 6f72 2067 655f 7265  is None or ge_re
-0000e590: 706f 7274 2e69 6e67 6573 7469 6f6e 5f72  port.ingestion_r
-0000e5a0: 6573 756c 7420 3d3d 2022 494e 4745 5354  esult == "INGEST
-0000e5b0: 4544 223a 0a20 2020 2020 2020 2020 2020  ED":.           
-0000e5c0: 2073 656c 662e 5f63 6f64 655f 656e 6769   self._code_engi
-0000e5d0: 6e65 2e73 6176 655f 636f 6465 2873 656c  ne.save_code(sel
-0000e5e0: 6629 0a0a 2020 2020 2020 2020 6966 2073  f)..        if s
-0000e5f0: 656c 662e 7374 6174 6973 7469 6373 5f63  elf.statistics_c
-0000e600: 6f6e 6669 672e 656e 6162 6c65 6420 616e  onfig.enabled an
-0000e610: 6420 656e 6769 6e65 2e67 6574 5f74 7970  d engine.get_typ
-0000e620: 6528 2920 3d3d 2022 7370 6172 6b22 3a0a  e() == "spark":.
-0000e630: 2020 2020 2020 2020 2020 2020 2320 4f6e              # On
-0000e640: 6c79 2063 6f6d 7075 7465 2073 7461 7469  ly compute stati
-0000e650: 7374 6963 7320 6966 2074 6865 2065 6e67  stics if the eng
-0000e660: 696e 6520 6973 2053 7061 726b 2e0a 2020  ine is Spark..  
-0000e670: 2020 2020 2020 2020 2020 2320 466f 7220            # For 
-0000e680: 5079 7468 6f6e 2065 6e67 696e 652c 2074  Python engine, t
-0000e690: 6865 2063 6f6d 7075 7461 7469 6f6e 2068  he computation h
-0000e6a0: 6170 7065 6e73 2069 6e20 7468 6520 486f  appens in the Ho
-0000e6b0: 7073 776f 726b 7320 6170 706c 6963 6174  psworks applicat
-0000e6c0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-0000e6d0: 7365 6c66 2e5f 7374 6174 6973 7469 6373  self._statistics
-0000e6e0: 5f65 6e67 696e 652e 636f 6d70 7574 655f  _engine.compute_
-0000e6f0: 7374 6174 6973 7469 6373 2873 656c 662c  statistics(self,
-0000e700: 2066 6561 7475 7265 5f64 6174 6166 7261   feature_datafra
-0000e710: 6d65 290a 2020 2020 2020 2020 6966 2075  me).        if u
-0000e720: 7365 725f 7665 7273 696f 6e20 6973 204e  ser_version is N
-0000e730: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000e740: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
-0000e750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e760: 224e 6f20 7665 7273 696f 6e20 7072 6f76  "No version prov
-0000e770: 6964 6564 2066 6f72 2063 7265 6174 696e  ided for creatin
-0000e780: 6720 6665 6174 7572 6520 6772 6f75 7020  g feature group 
-0000e790: 607b 7d60 2c20 696e 6372 656d 656e 7465  `{}`, incremente
-0000e7a0: 6420 7665 7273 696f 6e20 746f 2060 7b7d  d version to `{}
-0000e7b0: 602e 222e 666f 726d 6174 280a 2020 2020  `.".format(.    
-0000e7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7d0: 7365 6c66 2e5f 6e61 6d65 2c20 7365 6c66  self._name, self
-0000e7e0: 2e5f 7665 7273 696f 6e0a 2020 2020 2020  ._version.      
-0000e7f0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-0000e800: 2020 2020 2020 2020 2020 2020 2075 7469               uti
-0000e810: 6c2e 5665 7273 696f 6e57 6172 6e69 6e67  l.VersionWarning
-0000e820: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000e830: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-0000e840: 0a20 2020 2020 2020 2020 2020 2066 675f  .            fg_
-0000e850: 6a6f 622c 0a20 2020 2020 2020 2020 2020  job,.           
-0000e860: 2067 655f 7265 706f 7274 2e74 6f5f 6765   ge_report.to_ge
-0000e870: 5f74 7970 6528 2920 6966 2067 655f 7265  _type() if ge_re
-0000e880: 706f 7274 2069 7320 6e6f 7420 4e6f 6e65  port is not None
-0000e890: 2065 6c73 6520 4e6f 6e65 2c0a 2020 2020   else None,.    
-0000e8a0: 2020 2020 290a 0a20 2020 2064 6566 2069      )..    def i
-0000e8b0: 6e73 6572 7428 0a20 2020 2020 2020 2073  nsert(.        s
-0000e8c0: 656c 662c 0a20 2020 2020 2020 2066 6561  elf,.        fea
-0000e8d0: 7475 7265 733a 2055 6e69 6f6e 5b0a 2020  tures: Union[.  
-0000e8e0: 2020 2020 2020 2020 2020 7064 2e44 6174            pd.Dat
-0000e8f0: 6146 7261 6d65 2c0a 2020 2020 2020 2020  aFrame,.        
-0000e900: 2020 2020 5479 7065 5661 7228 2270 7973      TypeVar("pys
-0000e910: 7061 726b 2e73 716c 2e44 6174 6146 7261  park.sql.DataFra
-0000e920: 6d65 2229 2c20 2023 206e 6f71 613a 2046  me"),  # noqa: F
-0000e930: 3832 310a 2020 2020 2020 2020 2020 2020  821.            
-0000e940: 5479 7065 5661 7228 2270 7973 7061 726b  TypeVar("pyspark
-0000e950: 2e52 4444 2229 2c20 2023 206e 6f71 613a  .RDD"),  # noqa:
-0000e960: 2046 3832 310a 2020 2020 2020 2020 2020   F821.          
-0000e970: 2020 6e70 2e6e 6461 7272 6179 2c0a 2020    np.ndarray,.  
-0000e980: 2020 2020 2020 2020 2020 4c69 7374 5b6c            List[l
-0000e990: 6973 745d 2c0a 2020 2020 2020 2020 5d2c  ist],.        ],
-0000e9a0: 0a20 2020 2020 2020 206f 7665 7277 7269  .        overwri
-0000e9b0: 7465 3a20 4f70 7469 6f6e 616c 5b62 6f6f  te: Optional[boo
-0000e9c0: 6c5d 203d 2046 616c 7365 2c0a 2020 2020  l] = False,.    
-0000e9d0: 2020 2020 6f70 6572 6174 696f 6e3a 204f      operation: O
-0000e9e0: 7074 696f 6e61 6c5b 7374 725d 203d 2022  ptional[str] = "
-0000e9f0: 7570 7365 7274 222c 0a20 2020 2020 2020  upsert",.       
-0000ea00: 2073 746f 7261 6765 3a20 4f70 7469 6f6e   storage: Option
-0000ea10: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-0000ea20: 2020 2020 2020 2020 7772 6974 655f 6f70          write_op
-0000ea30: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
-0000ea40: 4469 6374 5b73 7472 2c20 416e 795d 5d20  Dict[str, Any]] 
-0000ea50: 3d20 7b7d 2c0a 2020 2020 2020 2020 7661  = {},.        va
-0000ea60: 6c69 6461 7469 6f6e 5f6f 7074 696f 6e73  lidation_options
-0000ea70: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
-0000ea80: 7374 722c 2041 6e79 5d5d 203d 204e 6f6e  str, Any]] = Non
-0000ea90: 652c 0a20 2020 2029 202d 3e20 5475 706c  e,.    ) -> Tupl
-0000eaa0: 655b 4f70 7469 6f6e 616c 5b4a 6f62 5d2c  e[Optional[Job],
-0000eab0: 204f 7074 696f 6e61 6c5b 5661 6c69 6461   Optional[Valida
-0000eac0: 7469 6f6e 5265 706f 7274 5d5d 3a0a 2020  tionReport]]:.  
-0000ead0: 2020 2020 2020 2222 2250 6572 7369 7374        """Persist
-0000eae0: 2074 6865 206d 6574 6164 6174 6120 616e   the metadata an
-0000eaf0: 6420 6d61 7465 7269 616c 697a 6520 7468  d materialize th
-0000eb00: 6520 6665 6174 7572 6520 6772 6f75 7020  e feature group 
-0000eb10: 746f 2074 6865 2066 6561 7475 7265 2073  to the feature s
-0000eb20: 746f 7265 0a20 2020 2020 2020 206f 7220  tore.        or 
-0000eb30: 696e 7365 7274 2064 6174 6120 6672 6f6d  insert data from
-0000eb40: 2061 2064 6174 6166 7261 6d65 2069 6e74   a dataframe int
-0000eb50: 6f20 7468 6520 6578 6973 7469 6e67 2066  o the existing f
-0000eb60: 6561 7475 7265 2067 726f 7570 2e0a 0a20  eature group... 
-0000eb70: 2020 2020 2020 2049 6e63 7265 6d65 6e74         Increment
-0000eb80: 616c 6c79 2069 6e73 6572 7420 6461 7461  ally insert data
-0000eb90: 2074 6f20 6120 6665 6174 7572 6520 6772   to a feature gr
-0000eba0: 6f75 7020 6f72 206f 7665 7277 7269 7465  oup or overwrite
-0000ebb0: 2061 6c6c 2020 6461 7461 2063 6f6e 7461   all  data conta
-0000ebc0: 696e 6564 2069 6e20 7468 6520 6665 6174  ined in the feat
-0000ebd0: 7572 6520 6772 6f75 702e 2042 790a 2020  ure group. By.  
-0000ebe0: 2020 2020 2020 6465 6661 756c 742c 2074        default, t
-0000ebf0: 6865 2064 6174 6120 6973 2069 6e73 6572  he data is inser
-0000ec00: 7465 6420 696e 746f 2074 6865 206f 6666  ted into the off
-0000ec10: 6c69 6e65 2073 746f 7261 6720 6173 2077  line storag as w
-0000ec20: 656c 6c20 6173 2074 6865 206f 6e6c 696e  ell as the onlin
-0000ec30: 6520 7374 6f72 6167 6520 6966 2074 6865  e storage if the
-0000ec40: 2066 6561 7475 7265 2067 726f 7570 2069   feature group i
-0000ec50: 730a 2020 2020 2020 2020 606f 6e6c 696e  s.        `onlin
-0000ec60: 655f 656e 6162 6c65 643d 5472 7565 602e  e_enabled=True`.
-0000ec70: 2054 6f20 696e 7365 7274 206f 6e6c 7920   To insert only 
-0000ec80: 696e 746f 2074 6865 206f 6e6c 696e 6520  into the online 
-0000ec90: 7374 6f72 6167 652c 2073 6574 2060 7374  storage, set `st
-0000eca0: 6f72 6167 653d 226f 6e6c 696e 6522 602c  orage="online"`,
-0000ecb0: 206f 7220 6f70 706f 7369 7465 6c79 0a20   or oppositely. 
-0000ecc0: 2020 2020 2020 2060 7374 6f72 6167 653d         `storage=
-0000ecd0: 226f 6666 6c69 6e65 2260 2e0a 0a20 2020  "offline"`...   
-0000ece0: 2020 2020 2054 6865 2060 6665 6174 7572       The `featur
-0000ecf0: 6573 6020 6461 7461 6672 616d 6520 6361  es` dataframe ca
-0000ed00: 6e20 6265 2061 2053 7061 726b 2044 6174  n be a Spark Dat
-0000ed10: 6146 7261 6d65 206f 7220 5244 442c 2061  aFrame or RDD, a
-0000ed20: 2050 616e 6461 7320 4461 7461 4672 616d   Pandas DataFram
-0000ed30: 652c 0a20 2020 2020 2020 206f 7220 6120  e,.        or a 
-0000ed40: 7477 6f2d 6469 6d65 6e73 696f 6e61 6c20  two-dimensional 
-0000ed50: 4e75 6d70 7920 6172 7261 7920 6f72 2061  Numpy array or a
-0000ed60: 2074 776f 2d64 696d 656e 7369 6f6e 616c   two-dimensional
-0000ed70: 2050 7974 686f 6e20 6e65 7374 6564 206c   Python nested l
-0000ed80: 6973 742e 0a20 2020 2020 2020 2049 6620  ist..        If 
-0000ed90: 7374 6174 6973 7469 6373 2061 7265 2065  statistics are e
-0000eda0: 6e61 626c 6564 2c20 7374 6174 6973 7469  nabled, statisti
-0000edb0: 6373 2061 7265 2072 6563 6f6d 7075 7465  cs are recompute
-0000edc0: 6420 666f 7220 7468 6520 656e 7469 7265  d for the entire
-0000edd0: 2066 6561 7475 7265 0a20 2020 2020 2020   feature.       
-0000ede0: 2067 726f 7570 2e0a 2020 2020 2020 2020   group..        
-0000edf0: 4966 2066 6561 7475 7265 2067 726f 7570  If feature group
-0000ee00: 2773 2074 696d 6520 7472 6176 656c 2066  's time travel f
-0000ee10: 6f72 6d61 7420 6973 2060 4855 4449 6020  ormat is `HUDI` 
-0000ee20: 7468 656e 2060 6f70 6572 6174 696f 6e60  then `operation`
-0000ee30: 2061 7267 756d 656e 7420 6361 6e20 6265   argument can be
-0000ee40: 0a20 2020 2020 2020 2065 6974 6865 7220  .        either 
-0000ee50: 6069 6e73 6572 7460 206f 7220 6075 7073  `insert` or `ups
-0000ee60: 6572 7460 2e0a 0a20 2020 2020 2020 2049  ert`...        I
-0000ee70: 6620 6665 6174 7572 6520 6772 6f75 7020  f feature group 
-0000ee80: 646f 6573 6e27 7420 6578 6973 7473 2020  doesn't exists  
-0000ee90: 7468 6520 696e 7365 7274 206d 6574 686f  the insert metho
-0000eea0: 6420 7769 6c6c 2063 7265 6174 6520 7468  d will create th
-0000eeb0: 6520 6e65 6365 7373 6172 7920 6d65 7461  e necessary meta
-0000eec0: 6461 7461 2074 6865 2066 6972 7374 2074  data the first t
-0000eed0: 696d 6520 6974 2069 730a 2020 2020 2020  ime it is.      
-0000eee0: 2020 696e 766f 6b65 6420 616e 6420 7772    invoked and wr
-0000eef0: 6974 6573 2074 6865 2073 7065 6369 6669  ites the specifi
-0000ef00: 6564 2060 6665 6174 7572 6573 6020 6461  ed `features` da
-0000ef10: 7461 6672 616d 6520 6173 2066 6561 7475  taframe as featu
-0000ef20: 7265 2067 726f 7570 2074 6f20 7468 6520  re group to the 
-0000ef30: 6f6e 6c69 6e65 2f6f 6666 6c69 6e65 2066  online/offline f
-0000ef40: 6561 7475 7265 2073 746f 7265 2e0a 0a20  eature store... 
-0000ef50: 2020 2020 2020 2021 2121 2065 7861 6d70         !!! examp
-0000ef60: 6c65 2022 5570 7365 7274 206e 6577 2066  le "Upsert new f
-0000ef70: 6561 7475 7265 2064 6174 6120 7769 7468  eature data with
-0000ef80: 2074 696d 6520 7472 6176 656c 2066 6f72   time travel for
-0000ef90: 6d61 7420 6048 5544 4960 220a 2020 2020  mat `HUDI`".    
-0000efa0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-0000efb0: 6e0a 2020 2020 2020 2020 2020 2020 2320  n.            # 
-0000efc0: 636f 6e6e 6563 7420 746f 2074 6865 2046  connect to the F
-0000efd0: 6561 7475 7265 2053 746f 7265 0a20 2020  eature Store.   
-0000efe0: 2020 2020 2020 2020 2066 7320 3d20 2e2e           fs = ..
-0000eff0: 2e0a 0a20 2020 2020 2020 2020 2020 2066  ...            f
-0000f000: 6720 3d20 6673 2e67 6574 5f6f 725f 6372  g = fs.get_or_cr
-0000f010: 6561 7465 5f66 6561 7475 7265 5f67 726f  eate_feature_gro
-0000f020: 7570 280a 2020 2020 2020 2020 2020 2020  up(.            
-0000f030: 2020 2020 6e61 6d65 3d27 6269 7463 6f69      name='bitcoi
-0000f040: 6e5f 7072 6963 6527 2c0a 2020 2020 2020  n_price',.      
-0000f050: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-0000f060: 7074 696f 6e3d 2742 6974 636f 696e 2070  ption='Bitcoin p
-0000f070: 7269 6365 2061 6767 7265 6761 7465 6420  rice aggregated 
-0000f080: 666f 7220 6461 7973 272c 0a20 2020 2020  for days',.     
-0000f090: 2020 2020 2020 2020 2020 2076 6572 7369             versi
-0000f0a0: 6f6e 3d31 2c0a 2020 2020 2020 2020 2020  on=1,.          
-0000f0b0: 2020 2020 2020 7072 696d 6172 795f 6b65        primary_ke
-0000f0c0: 793d 5b27 756e 6978 275d 2c0a 2020 2020  y=['unix'],.    
-0000f0d0: 2020 2020 2020 2020 2020 2020 6f6e 6c69              onli
-0000f0e0: 6e65 5f65 6e61 626c 6564 3d54 7275 652c  ne_enabled=True,
-0000f0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f100: 2065 7665 6e74 5f74 696d 653d 2775 6e69   event_time='uni
-0000f110: 7827 0a20 2020 2020 2020 2020 2020 2029  x'.            )
-0000f120: 0a0a 2020 2020 2020 2020 2020 2020 6667  ..            fg
-0000f130: 2e69 6e73 6572 7428 6466 5f62 6974 636f  .insert(df_bitco
-0000f140: 696e 5f70 726f 6365 7373 6564 290a 2020  in_processed).  
-0000f150: 2020 2020 2020 2020 2020 6060 600a 0a20            ```.. 
-0000f160: 2020 2020 2020 2021 2121 2065 7861 6d70         !!! examp
-0000f170: 6c65 2022 4173 796e 6320 696e 7365 7274  le "Async insert
-0000f180: 220a 2020 2020 2020 2020 2020 2020 6060  ".            ``
-0000f190: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
-0000f1a0: 2020 2020 2320 636f 6e6e 6563 7420 746f      # connect to
-0000f1b0: 2074 6865 2046 6561 7475 7265 2053 746f   the Feature Sto
-0000f1c0: 7265 0a20 2020 2020 2020 2020 2020 2066  re.            f
-0000f1d0: 7320 3d20 2e2e 2e0a 0a20 2020 2020 2020  s = .....       
-0000f1e0: 2020 2020 2066 6731 203d 2066 732e 6765       fg1 = fs.ge
-0000f1f0: 745f 6f72 5f63 7265 6174 655f 6665 6174  t_or_create_feat
-0000f200: 7572 655f 6772 6f75 7028 0a20 2020 2020  ure_group(.     
-0000f210: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-0000f220: 2766 6561 7475 7265 5f67 726f 7570 5f6e  'feature_group_n
-0000f230: 616d 6531 272c 0a20 2020 2020 2020 2020  ame1',.         
-0000f240: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-0000f250: 6f6e 3d27 4465 7363 7269 7074 696f 6e20  on='Description 
-0000f260: 6f66 2074 6865 2066 6972 7374 2046 4727  of the first FG'
-0000f270: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f280: 2020 7665 7273 696f 6e3d 312c 0a20 2020    version=1,.   
-0000f290: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-0000f2a0: 6d61 7279 5f6b 6579 3d5b 2775 6e69 7827  mary_key=['unix'
-0000f2b0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000f2c0: 2020 206f 6e6c 696e 655f 656e 6162 6c65     online_enable
-0000f2d0: 643d 5472 7565 2c0a 2020 2020 2020 2020  d=True,.        
-0000f2e0: 2020 2020 2020 2020 6576 656e 745f 7469          event_ti
-0000f2f0: 6d65 3d27 756e 6978 270a 2020 2020 2020  me='unix'.      
-0000f300: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000f310: 2020 2020 2320 6173 796e 6320 696e 7365      # async inse
-0000f320: 7274 696f 6e20 696e 206f 7264 6572 206e  rtion in order n
-0000f330: 6f74 2074 6f20 7761 6974 2074 696c 6c20  ot to wait till 
-0000f340: 6669 6e69 7368 206f 6620 7468 6520 6a6f  finish of the jo
-0000f350: 620a 2020 2020 2020 2020 2020 2020 6667  b.            fg
-0000f360: 2e69 6e73 6572 7428 6466 5f66 6f72 5f66  .insert(df_for_f
-0000f370: 6731 2c20 7772 6974 655f 6f70 7469 6f6e  g1, write_option
-0000f380: 733d 7b22 7761 6974 5f66 6f72 5f6a 6f62  s={"wait_for_job
-0000f390: 2220 3a20 4661 6c73 657d 290a 0a20 2020  " : False})..   
-0000f3a0: 2020 2020 2020 2020 2066 6732 203d 2066           fg2 = f
-0000f3b0: 732e 6765 745f 6f72 5f63 7265 6174 655f  s.get_or_create_
-0000f3c0: 6665 6174 7572 655f 6772 6f75 7028 0a20  feature_group(. 
-0000f3d0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000f3e0: 616d 653d 2766 6561 7475 7265 5f67 726f  ame='feature_gro
-0000f3f0: 7570 5f6e 616d 6532 272c 0a20 2020 2020  up_name2',.     
-0000f400: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-0000f410: 6970 7469 6f6e 3d27 4465 7363 7269 7074  iption='Descript
-0000f420: 696f 6e20 6f66 2074 6865 2073 6563 6f6e  ion of the secon
-0000f430: 6420 4647 272c 0a20 2020 2020 2020 2020  d FG',.         
-0000f440: 2020 2020 2020 2076 6572 7369 6f6e 3d31         version=1
-0000f450: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f460: 2020 7072 696d 6172 795f 6b65 793d 5b27    primary_key=['
-0000f470: 756e 6978 275d 2c0a 2020 2020 2020 2020  unix'],.        
-0000f480: 2020 2020 2020 2020 6f6e 6c69 6e65 5f65          online_e
-0000f490: 6e61 626c 6564 3d54 7275 652c 0a20 2020  nabled=True,.   
-0000f4a0: 2020 2020 2020 2020 2020 2020 2065 7665               eve
-0000f4b0: 6e74 5f74 696d 653d 2775 6e69 7827 0a20  nt_time='unix'. 
-0000f4c0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000f4d0: 2020 2020 2020 2020 2066 672e 696e 7365           fg.inse
-0000f4e0: 7274 2864 665f 666f 725f 6667 3229 0a20  rt(df_for_fg2). 
-0000f4f0: 2020 2020 2020 2020 2020 2060 6060 0a0a             ```..
-0000f500: 2020 2020 2020 2020 2320 4172 6775 6d65          # Argume
-0000f510: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-0000f520: 6665 6174 7572 6573 3a20 4461 7461 4672  features: DataFr
-0000f530: 616d 652c 2052 4444 2c20 4e64 6172 7261  ame, RDD, Ndarra
-0000f540: 792c 206c 6973 742e 2046 6561 7475 7265  y, list. Feature
-0000f550: 7320 746f 2062 6520 7361 7665 642e 0a20  s to be saved.. 
-0000f560: 2020 2020 2020 2020 2020 206f 7665 7277             overw
-0000f570: 7269 7465 3a20 4472 6f70 2061 6c6c 2064  rite: Drop all d
-0000f580: 6174 6120 696e 2074 6865 2066 6561 7475  ata in the featu
-0000f590: 7265 2067 726f 7570 2062 6566 6f72 650a  re group before.
-0000f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5b0: 696e 7365 7274 696e 6720 6e65 7720 6461  inserting new da
-0000f5c0: 7461 2e20 5468 6973 2064 6f65 7320 6e6f  ta. This does no
-0000f5d0: 7420 6166 6665 6374 206d 6574 6164 6174  t affect metadat
-0000f5e0: 612c 2064 6566 6175 6c74 7320 746f 2046  a, defaults to F
-0000f5f0: 616c 7365 2e0a 2020 2020 2020 2020 2020  alse..          
-0000f600: 2020 6f70 6572 6174 696f 6e3a 2041 7061    operation: Apa
-0000f610: 6368 6520 4875 6469 206f 7065 7261 7469  che Hudi operati
-0000f620: 6f6e 2074 7970 6520 6022 696e 7365 7274  on type `"insert
-0000f630: 2260 206f 7220 6022 7570 7365 7274 2260  "` or `"upsert"`
-0000f640: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f650: 2020 4465 6661 756c 7473 2074 6f20 6022    Defaults to `"
-0000f660: 7570 7365 7274 2260 2e0a 2020 2020 2020  upsert"`..      
-0000f670: 2020 2020 2020 7374 6f72 6167 653a 204f        storage: O
-0000f680: 7665 7277 7269 7465 2064 6566 6175 6c74  verwrite default
-0000f690: 2062 6568 6176 696f 7572 2c20 7772 6974   behaviour, writ
-0000f6a0: 6520 746f 206f 6666 6c69 6e65 0a20 2020  e to offline.   
-0000f6b0: 2020 2020 2020 2020 2020 2020 2073 746f               sto
-0000f6c0: 7261 6765 206f 6e6c 7920 7769 7468 2060  rage only with `
-0000f6d0: 226f 6666 6c69 6e65 2260 206f 7220 6f6e  "offline"` or on
-0000f6e0: 6c69 6e65 206f 6e6c 7920 7769 7468 2060  line only with `
-0000f6f0: 226f 6e6c 696e 6522 602c 2064 6566 6175  "online"`, defau
-0000f700: 6c74 730a 2020 2020 2020 2020 2020 2020  lts.            
-0000f710: 2020 2020 746f 2060 4e6f 6e65 602e 0a20      to `None`.. 
-0000f720: 2020 2020 2020 2020 2020 2077 7269 7465             write
-0000f730: 5f6f 7074 696f 6e73 3a20 4164 6469 7469  _options: Additi
-0000f740: 6f6e 616c 2077 7269 7465 206f 7074 696f  onal write optio
-0000f750: 6e73 2061 7320 6b65 792d 7661 6c75 6520  ns as key-value 
-0000f760: 7061 6972 732c 2064 6566 6175 6c74 7320  pairs, defaults 
-0000f770: 746f 2060 7b7d 602e 0a20 2020 2020 2020  to `{}`..       
-0000f780: 2020 2020 2020 2020 2057 6865 6e20 7573           When us
-0000f790: 696e 6720 7468 6520 6070 7974 686f 6e60  ing the `python`
-0000f7a0: 2065 6e67 696e 652c 2077 7269 7465 5f6f   engine, write_o
-0000f7b0: 7074 696f 6e73 2063 616e 2063 6f6e 7461  ptions can conta
-0000f7c0: 696e 2074 6865 0a20 2020 2020 2020 2020  in the.         
-0000f7d0: 2020 2020 2020 2066 6f6c 6c6f 7769 6e67         following
-0000f7e0: 2065 6e74 7269 6573 3a0a 2020 2020 2020   entries:.      
-0000f7f0: 2020 2020 2020 2020 2020 2a20 6b65 7920            * key 
-0000f800: 6073 7061 726b 6020 616e 6420 7661 6c75  `spark` and valu
-0000f810: 6520 616e 206f 626a 6563 7420 6f66 2074  e an object of t
-0000f820: 7970 650a 2020 2020 2020 2020 2020 2020  ype.            
-0000f830: 2020 2020 5b68 7366 732e 636f 7265 2e6a      [hsfs.core.j
-0000f840: 6f62 5f63 6f6e 6669 6775 7261 7469 6f6e  ob_configuration
-0000f850: 2e4a 6f62 436f 6e66 6967 7572 6174 696f  .JobConfiguratio
-0000f860: 6e5d 282e 2e2f 6a6f 625f 636f 6e66 6967  n](../job_config
-0000f870: 7572 6174 696f 6e29 0a20 2020 2020 2020  uration).       
-0000f880: 2020 2020 2020 2020 2020 2074 6f20 636f             to co
-0000f890: 6e66 6967 7572 6520 7468 6520 486f 7073  nfigure the Hops
-0000f8a0: 776f 726b 7320 4a6f 6220 7573 6564 2074  works Job used t
-0000f8b0: 6f20 7772 6974 6520 6461 7461 2069 6e74  o write data int
-0000f8c0: 6f20 7468 650a 2020 2020 2020 2020 2020  o the.          
-0000f8d0: 2020 2020 2020 2020 6665 6174 7572 6520          feature 
-0000f8e0: 6772 6f75 702e 0a20 2020 2020 2020 2020  group..         
-0000f8f0: 2020 2020 2020 202a 206b 6579 2060 7761         * key `wa
-0000f900: 6974 5f66 6f72 5f6a 6f62 6020 616e 6420  it_for_job` and 
-0000f910: 7661 6c75 6520 6054 7275 6560 206f 7220  value `True` or 
-0000f920: 6046 616c 7365 6020 746f 2063 6f6e 6669  `False` to confi
-0000f930: 6775 7265 0a20 2020 2020 2020 2020 2020  gure.           
-0000f940: 2020 2020 2020 2077 6865 7468 6572 206f         whether o
-0000f950: 7220 6e6f 7420 746f 2074 6865 2069 6e73  r not to the ins
-0000f960: 6572 7420 6361 6c6c 2073 686f 756c 6420  ert call should 
-0000f970: 7265 7475 726e 206f 6e6c 790a 2020 2020  return only.    
-0000f980: 2020 2020 2020 2020 2020 2020 2020 6166                af
-0000f990: 7465 7220 7468 6520 486f 7073 776f 726b  ter the Hopswork
-0000f9a0: 7320 4a6f 6220 6861 7320 6669 6e69 7368  s Job has finish
-0000f9b0: 6564 2e20 4279 2064 6566 6175 6c74 2069  ed. By default i
-0000f9c0: 7420 7761 6974 732e 0a20 2020 2020 2020  t waits..       
-0000f9d0: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
-0000f9e0: 7374 6172 745f 6f66 666c 696e 655f 6261  start_offline_ba
-0000f9f0: 636b 6669 6c6c 6020 616e 6420 7661 6c75  ckfill` and valu
-0000fa00: 6520 6054 7275 6560 206f 7220 6046 616c  e `True` or `Fal
-0000fa10: 7365 6020 746f 2063 6f6e 6669 6775 7265  se` to configure
-0000fa20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fa30: 2020 2077 6865 7468 6572 206f 7220 6e6f     whether or no
-0000fa40: 7420 746f 2073 7461 7274 2074 6865 2062  t to start the b
-0000fa50: 6163 6b66 696c 6c20 6a6f 6220 746f 2077  ackfill job to w
-0000fa60: 7269 7465 2064 6174 6120 746f 2074 6865  rite data to the
-0000fa70: 206f 6666 6c69 6e65 0a20 2020 2020 2020   offline.       
-0000fa80: 2020 2020 2020 2020 2020 2073 746f 7261             stora
-0000fa90: 6765 2e20 4279 2064 6566 6175 6c74 2074  ge. By default t
-0000faa0: 6865 2062 6163 6b66 696c 6c20 6a6f 6220  he backfill job 
-0000fab0: 6765 7473 2073 7461 7274 6564 2069 6d6d  gets started imm
-0000fac0: 6564 6961 7465 6c79 2e0a 2020 2020 2020  ediately..      
-0000fad0: 2020 2020 2020 2020 2020 2a20 6b65 7920            * key 
-0000fae0: 6069 6e74 6572 6e61 6c5f 6b61 666b 6160  `internal_kafka`
-0000faf0: 2061 6e64 2076 616c 7565 2060 5472 7565   and value `True
-0000fb00: 6020 6f72 2060 4661 6c73 6560 2069 6e20  ` or `False` in 
-0000fb10: 6361 7365 2079 6f75 2065 7374 6162 6c69  case you establi
-0000fb20: 7368 6564 0a20 2020 2020 2020 2020 2020  shed.           
-0000fb30: 2020 2020 2020 2063 6f6e 6e65 6374 6976         connectiv
-0000fb40: 6974 7920 6672 6f6d 2079 6f75 2050 7974  ity from you Pyt
-0000fb50: 686f 6e20 656e 7669 726f 6e6d 656e 7420  hon environment 
-0000fb60: 746f 2074 6865 2069 6e74 6572 6e61 6c20  to the internal 
-0000fb70: 6164 7665 7274 6973 6564 0a20 2020 2020  advertised.     
-0000fb80: 2020 2020 2020 2020 2020 2020 206c 6973               lis
-0000fb90: 7465 6e65 7273 206f 6620 7468 6520 486f  teners of the Ho
-0000fba0: 7073 776f 726b 7320 4b61 666b 6120 436c  psworks Kafka Cl
-0000fbb0: 7573 7465 722e 2044 6566 6175 6c74 7320  uster. Defaults 
-0000fbc0: 746f 2060 4661 6c73 6560 2061 6e64 0a20  to `False` and. 
-0000fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbe0: 2077 696c 6c20 7573 6520 6578 7465 726e   will use extern
-0000fbf0: 616c 206c 6973 7465 6e65 7273 2077 6865  al listeners whe
-0000fc00: 6e20 636f 6e6e 6563 7469 6e67 2066 726f  n connecting fro
-0000fc10: 6d20 6f75 7473 6964 6520 6f66 2048 6f70  m outside of Hop
-0000fc20: 7377 6f72 6b73 2e0a 2020 2020 2020 2020  sworks..        
-0000fc30: 2020 2020 7661 6c69 6461 7469 6f6e 5f6f      validation_o
-0000fc40: 7074 696f 6e73 3a20 4164 6469 7469 6f6e  ptions: Addition
-0000fc50: 616c 2076 616c 6964 6174 696f 6e20 6f70  al validation op
-0000fc60: 7469 6f6e 7320 6173 206b 6579 2d76 616c  tions as key-val
-0000fc70: 7565 2070 6169 7273 2c20 6465 6661 756c  ue pairs, defaul
-0000fc80: 7473 2074 6f20 607b 7d60 2e0a 2020 2020  ts to `{}`..    
-0000fc90: 2020 2020 2020 2020 2020 2020 2a20 6b65              * ke
-0000fca0: 7920 6072 756e 5f76 616c 6964 6174 696f  y `run_validatio
-0000fcb0: 6e60 2062 6f6f 6c65 616e 2076 616c 7565  n` boolean value
-0000fcc0: 2c20 7365 7420 746f 2060 4661 6c73 6560  , set to `False`
-0000fcd0: 2074 6f20 736b 6970 2076 616c 6964 6174   to skip validat
-0000fce0: 696f 6e20 7465 6d70 6f72 6172 696c 7920  ion temporarily 
-0000fcf0: 6f6e 2069 6e67 6573 7469 6f6e 2e0a 2020  on ingestion..  
-0000fd00: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
-0000fd10: 6b65 7920 6073 6176 655f 7265 706f 7274  key `save_report
-0000fd20: 6020 626f 6f6c 6561 6e20 7661 6c75 652c  ` boolean value,
-0000fd30: 2073 6574 2074 6f20 6046 616c 7365 6020   set to `False` 
-0000fd40: 746f 2073 6b69 7020 7570 6c6f 6164 206f  to skip upload o
-0000fd50: 6620 7468 6520 7661 6c69 6461 7469 6f6e  f the validation
-0000fd60: 2072 6570 6f72 7420 746f 2048 6f70 7377   report to Hopsw
-0000fd70: 6f72 6b73 2e0a 2020 2020 2020 2020 2020  orks..          
-0000fd80: 2020 2020 2020 2a20 6b65 7920 6067 655f        * key `ge_
-0000fd90: 7661 6c69 6461 7465 5f6b 7761 7267 7360  validate_kwargs`
-0000fda0: 2061 2064 6963 7469 6f6e 6172 7920 636f   a dictionary co
-0000fdb0: 6e74 6169 6e69 6e67 206b 7761 7267 7320  ntaining kwargs 
-0000fdc0: 666f 7220 7468 6520 7661 6c69 6461 7465  for the validate
-0000fdd0: 206d 6574 686f 6420 6f66 2047 7265 6174   method of Great
-0000fde0: 2045 7870 6563 7461 7469 6f6e 732e 0a0a   Expectations...
-0000fdf0: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
-0000fe00: 730a 2020 2020 2020 2020 2020 2020 2860  s.            (`
-0000fe10: 4a6f 6260 2c20 6056 616c 6964 6174 696f  Job`, `Validatio
-0000fe20: 6e52 6570 6f72 7460 2920 4120 7475 706c  nReport`) A tupl
-0000fe30: 6520 7769 7468 206a 6f62 2069 6e66 6f72  e with job infor
-0000fe40: 6d61 7469 6f6e 2069 6620 7079 7468 6f6e  mation if python
-0000fe50: 2065 6e67 696e 6520 6973 2075 7365 6420   engine is used 
-0000fe60: 616e 6420 7468 6520 7661 6c69 6461 7469  and the validati
-0000fe70: 6f6e 2072 6570 6f72 7420 6966 2076 616c  on report if val
-0000fe80: 6964 6174 696f 6e20 6973 2065 6e61 626c  idation is enabl
-0000fe90: 6564 2e0a 2020 2020 2020 2020 2222 220a  ed..        """.
-0000fea0: 2020 2020 2020 2020 6665 6174 7572 655f          feature_
-0000feb0: 6461 7461 6672 616d 6520 3d20 656e 6769  dataframe = engi
-0000fec0: 6e65 2e67 6574 5f69 6e73 7461 6e63 6528  ne.get_instance(
-0000fed0: 292e 636f 6e76 6572 745f 746f 5f64 6566  ).convert_to_def
-0000fee0: 6175 6c74 5f64 6174 6166 7261 6d65 2866  ault_dataframe(f
-0000fef0: 6561 7475 7265 7329 0a0a 2020 2020 2020  eatures)..      
-0000ff00: 2020 6a6f 622c 2067 655f 7265 706f 7274    job, ge_report
-0000ff10: 203d 2073 656c 662e 5f66 6561 7475 7265   = self._feature
-0000ff20: 5f67 726f 7570 5f65 6e67 696e 652e 696e  _group_engine.in
-0000ff30: 7365 7274 280a 2020 2020 2020 2020 2020  sert(.          
-0000ff40: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000ff50: 2020 2020 6665 6174 7572 655f 6461 7461      feature_data
-0000ff60: 6672 616d 653d 6665 6174 7572 655f 6461  frame=feature_da
-0000ff70: 7461 6672 616d 652c 0a20 2020 2020 2020  taframe,.       
-0000ff80: 2020 2020 206f 7665 7277 7269 7465 3d6f       overwrite=o
-0000ff90: 7665 7277 7269 7465 2c0a 2020 2020 2020  verwrite,.      
-0000ffa0: 2020 2020 2020 6f70 6572 6174 696f 6e3d        operation=
-0000ffb0: 6f70 6572 6174 696f 6e2c 0a20 2020 2020  operation,.     
-0000ffc0: 2020 2020 2020 2073 746f 7261 6765 3d73         storage=s
-0000ffd0: 746f 7261 6765 2e6c 6f77 6572 2829 2069  torage.lower() i
-0000ffe0: 6620 7374 6f72 6167 6520 6973 206e 6f74  f storage is not
-0000fff0: 204e 6f6e 6520 656c 7365 204e 6f6e 652c   None else None,
-00010000: 0a20 2020 2020 2020 2020 2020 2077 7269  .            wri
-00010010: 7465 5f6f 7074 696f 6e73 3d77 7269 7465  te_options=write
-00010020: 5f6f 7074 696f 6e73 2c0a 2020 2020 2020  _options,.      
-00010030: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
-00010040: 5f6f 7074 696f 6e73 3d76 616c 6964 6174  _options=validat
-00010050: 696f 6e5f 6f70 7469 6f6e 730a 2020 2020  ion_options.    
-00010060: 2020 2020 2020 2020 6966 2076 616c 6964          if valid
-00010070: 6174 696f 6e5f 6f70 7469 6f6e 7320 6973  ation_options is
-00010080: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
-00010090: 2020 2020 2020 656c 7365 207b 2273 6176        else {"sav
-000100a0: 655f 7265 706f 7274 223a 2054 7275 657d  e_report": True}
-000100b0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-000100c0: 2020 2020 2069 6620 6765 5f72 6570 6f72       if ge_repor
-000100d0: 7420 6973 204e 6f6e 6520 6f72 2067 655f  t is None or ge_
-000100e0: 7265 706f 7274 2e69 6e67 6573 7469 6f6e  report.ingestion
-000100f0: 5f72 6573 756c 7420 3d3d 2022 494e 4745  _result == "INGE
-00010100: 5354 4544 223a 0a20 2020 2020 2020 2020  STED":.         
-00010110: 2020 2073 656c 662e 5f63 6f64 655f 656e     self._code_en
-00010120: 6769 6e65 2e73 6176 655f 636f 6465 2873  gine.save_code(s
-00010130: 656c 6629 0a20 2020 2020 2020 2069 6620  elf).        if 
-00010140: 656e 6769 6e65 2e67 6574 5f74 7970 6528  engine.get_type(
-00010150: 2920 3d3d 2022 7370 6172 6b22 3a0a 2020  ) == "spark":.  
-00010160: 2020 2020 2020 2020 2020 2320 4f6e 6c79            # Only
-00010170: 2063 6f6d 7075 7465 2073 7461 7469 7374   compute statist
-00010180: 6963 7320 6966 2074 6865 2065 6e67 696e  ics if the engin
-00010190: 6520 6973 2053 7061 726b 2c0a 2020 2020  e is Spark,.    
-000101a0: 2020 2020 2020 2020 2320 6966 2050 7974          # if Pyt
-000101b0: 686f 6e2c 2074 6865 2073 7461 7469 7374  hon, the statist
-000101c0: 6963 7320 6172 6520 636f 6d70 7574 6564  ics are computed
-000101d0: 2062 7920 7468 6520 6170 706c 6963 6174   by the applicat
-000101e0: 696f 6e20 646f 696e 6720 7468 6520 696e  ion doing the in
-000101f0: 7365 7274 0a20 2020 2020 2020 2020 2020  sert.           
-00010200: 2073 656c 662e 636f 6d70 7574 655f 7374   self.compute_st
-00010210: 6174 6973 7469 6373 2829 0a0a 2020 2020  atistics()..    
-00010220: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
-00010230: 2020 2020 2020 2020 206a 6f62 2c0a 2020           job,.  
-00010240: 2020 2020 2020 2020 2020 6765 5f72 6570            ge_rep
-00010250: 6f72 742e 746f 5f67 655f 7479 7065 2829  ort.to_ge_type()
-00010260: 2069 6620 6765 5f72 6570 6f72 7420 6973   if ge_report is
-00010270: 206e 6f74 204e 6f6e 6520 656c 7365 204e   not None else N
-00010280: 6f6e 652c 0a20 2020 2020 2020 2029 0a0a  one,.        )..
-00010290: 2020 2020 6465 6620 696e 7365 7274 5f73      def insert_s
-000102a0: 7472 6561 6d28 0a20 2020 2020 2020 2073  tream(.        s
-000102b0: 656c 662c 0a20 2020 2020 2020 2066 6561  elf,.        fea
-000102c0: 7475 7265 733a 2054 7970 6556 6172 2822  tures: TypeVar("
-000102d0: 7079 7370 6172 6b2e 7371 6c2e 4461 7461  pyspark.sql.Data
-000102e0: 4672 616d 6522 292c 2020 2320 6e6f 7161  Frame"),  # noqa
-000102f0: 3a20 4638 3231 0a20 2020 2020 2020 2071  : F821.        q
-00010300: 7565 7279 5f6e 616d 653a 204f 7074 696f  uery_name: Optio
-00010310: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00010320: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
-00010330: 6d6f 6465 3a20 4f70 7469 6f6e 616c 5b73  mode: Optional[s
-00010340: 7472 5d20 3d20 2261 7070 656e 6422 2c0a  tr] = "append",.
-00010350: 2020 2020 2020 2020 6177 6169 745f 7465          await_te
-00010360: 726d 696e 6174 696f 6e3a 204f 7074 696f  rmination: Optio
-00010370: 6e61 6c5b 626f 6f6c 5d20 3d20 4661 6c73  nal[bool] = Fals
-00010380: 652c 0a20 2020 2020 2020 2074 696d 656f  e,.        timeo
-00010390: 7574 3a20 4f70 7469 6f6e 616c 5b69 6e74  ut: Optional[int
-000103a0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-000103b0: 2020 6368 6563 6b70 6f69 6e74 5f64 6972    checkpoint_dir
-000103c0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-000103d0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000103e0: 7772 6974 655f 6f70 7469 6f6e 733a 204f  write_options: O
-000103f0: 7074 696f 6e61 6c5b 4469 6374 5b41 6e79  ptional[Dict[Any
-00010400: 2c20 416e 795d 5d20 3d20 7b7d 2c0a 2020  , Any]] = {},.  
-00010410: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-00010420: 496e 6765 7374 2061 2053 7061 726b 2053  Ingest a Spark S
-00010430: 7472 7563 7475 7265 6420 5374 7265 616d  tructured Stream
-00010440: 696e 6720 4461 7461 6672 616d 6520 746f  ing Dataframe to
-00010450: 2074 6865 206f 6e6c 696e 6520 6665 6174   the online feat
-00010460: 7572 6520 7374 6f72 652e 0a0a 2020 2020  ure store...    
-00010470: 2020 2020 5468 6973 206d 6574 686f 6420      This method 
-00010480: 6372 6561 7465 7320 6120 6c6f 6e67 2072  creates a long r
-00010490: 756e 6e69 6e67 2053 7061 726b 2053 7472  unning Spark Str
-000104a0: 6561 6d69 6e67 2051 7565 7279 2c20 796f  eaming Query, yo
-000104b0: 7520 6361 6e20 636f 6e74 726f 6c20 7468  u can control th
-000104c0: 650a 2020 2020 2020 2020 7465 726d 696e  e.        termin
-000104d0: 6174 696f 6e20 6f66 2074 6865 2071 7565  ation of the que
-000104e0: 7279 2074 6872 6f75 6768 2074 6865 2061  ry through the a
-000104f0: 7267 756d 656e 7473 2e0a 0a20 2020 2020  rguments...     
-00010500: 2020 2049 7420 6973 2070 6f73 7369 626c     It is possibl
-00010510: 6520 746f 2073 746f 7020 7468 6520 7265  e to stop the re
-00010520: 7475 726e 6564 2071 7565 7279 2077 6974  turned query wit
-00010530: 6820 7468 6520 602e 7374 6f70 2829 6020  h the `.stop()` 
-00010540: 616e 6420 6368 6563 6b20 6974 730a 2020  and check its.  
-00010550: 2020 2020 2020 7374 6174 7573 2077 6974        status wit
-00010560: 6820 602e 6973 4163 7469 7665 602e 0a0a  h `.isActive`...
-00010570: 2020 2020 2020 2020 546f 2067 6574 2061          To get a
-00010580: 206c 6973 7420 6f66 2061 6c6c 2061 6374   list of all act
-00010590: 6976 6520 7175 6572 6965 732c 2075 7365  ive queries, use
-000105a0: 3a0a 0a20 2020 2020 2020 2060 6060 7079  :..        ```py
-000105b0: 7468 6f6e 0a20 2020 2020 2020 2073 716d  thon.        sqm
-000105c0: 203d 2073 7061 726b 2e73 7472 6561 6d73   = spark.streams
-000105d0: 0a0a 2020 2020 2020 2020 2320 6765 7420  ..        # get 
-000105e0: 7468 6520 6c69 7374 206f 6620 6163 7469  the list of acti
-000105f0: 7665 2073 7472 6561 6d69 6e67 2071 7565  ve streaming que
-00010600: 7269 6573 0a20 2020 2020 2020 205b 712e  ries.        [q.
-00010610: 6e61 6d65 2066 6f72 2071 2069 6e20 7371  name for q in sq
-00010620: 6d2e 6163 7469 7665 5d0a 2020 2020 2020  m.active].      
-00010630: 2020 6060 600a 0a20 2020 2020 2020 2021    ```..        !
-00010640: 2121 2077 6172 6e69 6e67 2022 456e 6769  !! warning "Engi
-00010650: 6e65 2053 7570 706f 7274 220a 2020 2020  ne Support".    
-00010660: 2020 2020 2020 2020 2a2a 5370 6172 6b20          **Spark 
-00010670: 6f6e 6c79 2a2a 0a0a 2020 2020 2020 2020  only**..        
-00010680: 2020 2020 5374 7265 616d 2069 6e67 6573      Stream inges
-00010690: 7469 6f6e 2075 7369 6e67 2050 616e 6461  tion using Panda
-000106a0: 732f 5079 7468 6f6e 2061 7320 656e 6769  s/Python as engi
-000106b0: 6e65 2069 7320 6375 7272 656e 746c 7920  ne is currently 
-000106c0: 6e6f 7420 7375 7070 6f72 7465 642e 0a20  not supported.. 
-000106d0: 2020 2020 2020 2020 2020 2050 7974 686f             Pytho
-000106e0: 6e2f 5061 6e64 6173 2068 6173 206e 6f20  n/Pandas has no 
-000106f0: 6e6f 7469 6f6e 206f 6620 7374 7265 616d  notion of stream
-00010700: 696e 672e 0a0a 2020 2020 2020 2020 2121  ing...        !!
-00010710: 2120 7761 726e 696e 6720 2244 6174 6120  ! warning "Data 
-00010720: 5661 6c69 6461 7469 6f6e 2053 7570 706f  Validation Suppo
-00010730: 7274 220a 2020 2020 2020 2020 2020 2020  rt".            
-00010740: 6069 6e73 6572 745f 7374 7265 616d 6020  `insert_stream` 
-00010750: 646f 6573 206e 6f74 2070 6572 666f 726d  does not perform
-00010760: 2061 6e79 2064 6174 6120 7661 6c69 6461   any data valida
-00010770: 7469 6f6e 2075 7369 6e67 2047 7265 6174  tion using Great
-00010780: 2045 7870 6563 7461 7469 6f6e 730a 2020   Expectations.  
-00010790: 2020 2020 2020 2020 2020 6576 656e 2077            even w
-000107a0: 6865 6e20 6120 6578 7065 6374 6174 696f  hen a expectatio
-000107b0: 6e20 7375 6974 6520 6973 2061 7474 6163  n suite is attac
-000107c0: 6865 642e 0a0a 2020 2020 2020 2020 2320  hed...        # 
-000107d0: 4172 6775 6d65 6e74 730a 2020 2020 2020  Arguments.      
-000107e0: 2020 2020 2020 6665 6174 7572 6573 3a20        features: 
-000107f0: 4665 6174 7572 6573 2069 6e20 5374 7265  Features in Stre
-00010800: 616d 696e 6720 4461 7461 6672 616d 6520  aming Dataframe 
-00010810: 746f 2062 6520 7361 7665 642e 0a20 2020  to be saved..   
-00010820: 2020 2020 2020 2020 2071 7565 7279 5f6e           query_n
-00010830: 616d 653a 2049 7420 6973 2070 6f73 7369  ame: It is possi
-00010840: 626c 6520 746f 206f 7074 696f 6e61 6c6c  ble to optionall
-00010850: 7920 7370 6563 6966 7920 6120 6e61 6d65  y specify a name
-00010860: 2066 6f72 2074 6865 2071 7565 7279 2074   for the query t
-00010870: 6f0a 2020 2020 2020 2020 2020 2020 2020  o.              
-00010880: 2020 6d61 6b65 2069 7420 6561 7369 6572    make it easier
-00010890: 2074 6f20 7265 636f 676e 6973 6520 696e   to recognise in
-000108a0: 2074 6865 2053 7061 726b 2055 492e 2044   the Spark UI. D
-000108b0: 6566 6175 6c74 7320 746f 2060 4e6f 6e65  efaults to `None
-000108c0: 602e 0a20 2020 2020 2020 2020 2020 206f  `..            o
-000108d0: 7574 7075 745f 6d6f 6465 3a20 5370 6563  utput_mode: Spec
-000108e0: 6966 6965 7320 686f 7720 6461 7461 206f  ifies how data o
-000108f0: 6620 6120 7374 7265 616d 696e 6720 4461  f a streaming Da
-00010900: 7461 4672 616d 652f 4461 7461 7365 7420  taFrame/Dataset 
-00010910: 6973 0a20 2020 2020 2020 2020 2020 2020  is.             
-00010920: 2020 2077 7269 7474 656e 2074 6f20 6120     written to a 
-00010930: 7374 7265 616d 696e 6720 7369 6e6b 2e20  streaming sink. 
-00010940: 2831 2920 6022 6170 7065 6e64 2260 3a20  (1) `"append"`: 
-00010950: 4f6e 6c79 2074 6865 206e 6577 2072 6f77  Only the new row
-00010960: 7320 696e 2074 6865 0a20 2020 2020 2020  s in the.       
-00010970: 2020 2020 2020 2020 2073 7472 6561 6d69           streami
-00010980: 6e67 2044 6174 6146 7261 6d65 2f44 6174  ng DataFrame/Dat
-00010990: 6173 6574 2077 696c 6c20 6265 2077 7269  aset will be wri
-000109a0: 7474 656e 2074 6f20 7468 6520 7369 6e6b  tten to the sink
-000109b0: 2e20 2832 290a 2020 2020 2020 2020 2020  . (2).          
-000109c0: 2020 2020 2020 6022 636f 6d70 6c65 7465        `"complete
-000109d0: 2260 3a20 416c 6c20 7468 6520 726f 7773  "`: All the rows
-000109e0: 2069 6e20 7468 6520 7374 7265 616d 696e   in the streamin
-000109f0: 6720 4461 7461 4672 616d 652f 4461 7461  g DataFrame/Data
-00010a00: 7365 7420 7769 6c6c 2062 650a 2020 2020  set will be.    
-00010a10: 2020 2020 2020 2020 2020 2020 7772 6974              writ
-00010a20: 7465 6e20 746f 2074 6865 2073 696e 6b20  ten to the sink 
-00010a30: 6576 6572 7920 7469 6d65 2074 6865 7265  every time there
-00010a40: 2069 7320 736f 6d65 2075 7064 6174 652e   is some update.
-00010a50: 2028 3329 2060 2275 7064 6174 6522 603a   (3) `"update"`:
-00010a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010a70: 206f 6e6c 7920 7468 6520 726f 7773 2074   only the rows t
-00010a80: 6861 7420 7765 7265 2075 7064 6174 6564  hat were updated
-00010a90: 2069 6e20 7468 6520 7374 7265 616d 696e   in the streamin
-00010aa0: 6720 4461 7461 4672 616d 652f 4461 7461  g DataFrame/Data
-00010ab0: 7365 7420 7769 6c6c 0a20 2020 2020 2020  set will.       
-00010ac0: 2020 2020 2020 2020 2062 6520 7772 6974           be writ
-00010ad0: 7465 6e20 746f 2074 6865 2073 696e 6b20  ten to the sink 
-00010ae0: 6576 6572 7920 7469 6d65 2074 6865 7265  every time there
-00010af0: 2061 7265 2073 6f6d 6520 7570 6461 7465   are some update
-00010b00: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-00010b10: 2020 2049 6620 7468 6520 7175 6572 7920     If the query 
-00010b20: 646f 6573 6ee2 8099 7420 636f 6e74 6169  doesn...t contai
-00010b30: 6e20 6167 6772 6567 6174 696f 6e73 2c20  n aggregations, 
-00010b40: 6974 2077 696c 6c20 6265 2065 7175 6976  it will be equiv
-00010b50: 616c 656e 7420 746f 0a20 2020 2020 2020  alent to.       
-00010b60: 2020 2020 2020 2020 2061 7070 656e 6420           append 
-00010b70: 6d6f 6465 2e20 4465 6661 756c 7473 2074  mode. Defaults t
-00010b80: 6f20 6022 6170 7065 6e64 2260 2e0a 2020  o `"append"`..  
-00010b90: 2020 2020 2020 2020 2020 6177 6169 745f            await_
-00010ba0: 7465 726d 696e 6174 696f 6e3a 2057 6169  termination: Wai
-00010bb0: 7473 2066 6f72 2074 6865 2074 6572 6d69  ts for the termi
-00010bc0: 6e61 7469 6f6e 206f 6620 7468 6973 2071  nation of this q
-00010bd0: 7565 7279 2c20 6569 7468 6572 2062 790a  uery, either by.
-00010be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bf0: 7175 6572 792e 7374 6f70 2829 206f 7220  query.stop() or 
-00010c00: 6279 2061 6e20 6578 6365 7074 696f 6e2e  by an exception.
-00010c10: 2049 6620 7468 6520 7175 6572 7920 6861   If the query ha
-00010c20: 7320 7465 726d 696e 6174 6564 2077 6974  s terminated wit
-00010c30: 6820 616e 0a20 2020 2020 2020 2020 2020  h an.           
-00010c40: 2020 2020 2065 7863 6570 7469 6f6e 2c20       exception, 
-00010c50: 7468 656e 2074 6865 2065 7863 6570 7469  then the excepti
-00010c60: 6f6e 2077 696c 6c20 6265 2074 6872 6f77  on will be throw
-00010c70: 6e2e 2049 6620 7469 6d65 6f75 7420 6973  n. If timeout is
-00010c80: 2073 6574 2c20 6974 0a20 2020 2020 2020   set, it.       
-00010c90: 2020 2020 2020 2020 2072 6574 7572 6e73           returns
-00010ca0: 2077 6865 7468 6572 2074 6865 2071 7565   whether the que
-00010cb0: 7279 2068 6173 2074 6572 6d69 6e61 7465  ry has terminate
-00010cc0: 6420 6f72 206e 6f74 2077 6974 6869 6e20  d or not within 
-00010cd0: 7468 6520 7469 6d65 6f75 740a 2020 2020  the timeout.    
-00010ce0: 2020 2020 2020 2020 2020 2020 7365 636f              seco
-00010cf0: 6e64 732e 2044 6566 6175 6c74 7320 746f  nds. Defaults to
-00010d00: 2060 4661 6c73 6560 2e0a 2020 2020 2020   `False`..      
-00010d10: 2020 2020 2020 7469 6d65 6f75 743a 204f        timeout: O
-00010d20: 6e6c 7920 7265 6c65 7661 6e74 2069 6e20  nly relevant in 
-00010d30: 636f 6d62 696e 6174 696f 6e20 7769 7468  combination with
-00010d40: 2060 6177 6169 745f 7465 726d 696e 6174   `await_terminat
-00010d50: 696f 6e3d 5472 7565 602e 0a20 2020 2020  ion=True`..     
-00010d60: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00010d70: 6c74 7320 746f 2060 4e6f 6e65 602e 0a20  lts to `None`.. 
-00010d80: 2020 2020 2020 2020 2020 2063 6865 636b             check
-00010d90: 706f 696e 745f 6469 723a 2043 6865 636b  point_dir: Check
-00010da0: 706f 696e 7420 6469 7265 6374 6f72 7920  point directory 
-00010db0: 6c6f 6361 7469 6f6e 2e20 5468 6973 2077  location. This w
-00010dc0: 696c 6c20 6265 2075 7365 6420 746f 2061  ill be used to a
-00010dd0: 7320 6120 7265 6665 7265 6e63 6520 746f  s a reference to
-00010de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010df0: 2066 726f 6d20 7768 6572 6520 746f 2072   from where to r
-00010e00: 6573 756d 6520 7468 6520 7374 7265 616d  esume the stream
-00010e10: 696e 6720 6a6f 622e 2049 6620 604e 6f6e  ing job. If `Non
-00010e20: 6560 2074 6865 6e20 6873 6673 2077 696c  e` then hsfs wil
-00010e30: 6c20 636f 6e73 7472 7563 7420 6173 0a20  l construct as. 
-00010e40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00010e50: 696e 7365 7274 5f73 7472 6561 6d5f 2220  insert_stream_" 
-00010e60: 2b20 6f6e 6c69 6e65 5f74 6f70 6963 5f6e  + online_topic_n
-00010e70: 616d 652e 2044 6566 6175 6c74 7320 746f  ame. Defaults to
-00010e80: 2060 4e6f 6e65 602e 0a20 2020 2020 2020   `None`..       
-00010e90: 2020 2020 2020 2020 2077 7269 7465 5f6f           write_o
-00010ea0: 7074 696f 6e73 3a20 4164 6469 7469 6f6e  ptions: Addition
-00010eb0: 616c 2077 7269 7465 206f 7074 696f 6e73  al write options
-00010ec0: 2066 6f72 2053 7061 726b 2061 7320 6b65   for Spark as ke
-00010ed0: 792d 7661 6c75 6520 7061 6972 732e 0a20  y-value pairs.. 
-00010ee0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-00010ef0: 6566 6175 6c74 7320 746f 2060 7b7d 602e  efaults to `{}`.
-00010f00: 0a0a 2020 2020 2020 2020 2320 5265 7475  ..        # Retu
-00010f10: 726e 730a 2020 2020 2020 2020 2020 2020  rns.            
-00010f20: 6053 7472 6561 6d69 6e67 5175 6572 7960  `StreamingQuery`
-00010f30: 3a20 5370 6172 6b20 5374 7275 6374 7572  : Spark Structur
-00010f40: 6564 2053 7472 6561 6d69 6e67 2051 7565  ed Streaming Que
-00010f50: 7279 206f 626a 6563 742e 0a20 2020 2020  ry object..     
-00010f60: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00010f70: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-00010f80: 6e6f 7420 656e 6769 6e65 2e67 6574 5f69  not engine.get_i
-00010f90: 6e73 7461 6e63 6528 292e 6973 5f73 7061  nstance().is_spa
-00010fa0: 726b 5f64 6174 6166 7261 6d65 2866 6561  rk_dataframe(fea
-00010fb0: 7475 7265 7329 0a20 2020 2020 2020 2020  tures).         
-00010fc0: 2020 206f 7220 6e6f 7420 6665 6174 7572     or not featur
-00010fd0: 6573 2e69 7353 7472 6561 6d69 6e67 0a20  es.isStreaming. 
-00010fe0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00010ff0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-00011000: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00011010: 2020 2020 2020 2022 4665 6174 7572 6573         "Features
-00011020: 2068 6176 6520 746f 2062 6520 6120 7374   have to be a st
-00011030: 7265 616d 696e 6720 7479 7065 2073 7061  reaming type spa
-00011040: 726b 2064 6174 6166 7261 6d65 2e20 5573  rk dataframe. Us
-00011050: 6520 6069 6e73 6572 7428 2960 206d 6574  e `insert()` met
-00011060: 686f 6420 696e 7374 6561 642e 220a 2020  hod instead.".  
-00011070: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00011080: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00011090: 2020 2020 2020 2320 6c6f 7765 7220 6361        # lower ca
-000110a0: 7369 6e67 2066 6561 7475 7265 206e 616d  sing feature nam
-000110b0: 6573 0a20 2020 2020 2020 2020 2020 2066  es.            f
-000110c0: 6561 7475 7265 5f64 6174 6166 7261 6d65  eature_dataframe
-000110d0: 203d 2065 6e67 696e 652e 6765 745f 696e   = engine.get_in
-000110e0: 7374 616e 6365 2829 2e63 6f6e 7665 7274  stance().convert
-000110f0: 5f74 6f5f 6465 6661 756c 745f 6461 7461  _to_default_data
-00011100: 6672 616d 6528 0a20 2020 2020 2020 2020  frame(.         
-00011110: 2020 2020 2020 2066 6561 7475 7265 730a         features.
-00011120: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00011130: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-00011140: 6773 2e77 6172 6e28 0a20 2020 2020 2020  gs.warn(.       
-00011150: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
-00011160: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011170: 5374 7265 616d 2069 6e67 6573 7469 6f6e  Stream ingestion
-00011180: 2066 6f72 2066 6561 7475 7265 2067 726f   for feature gro
-00011190: 7570 2060 7b7d 602c 2077 6974 6820 7665  up `{}`, with ve
-000111a0: 7273 696f 6e22 0a20 2020 2020 2020 2020  rsion".         
-000111b0: 2020 2020 2020 2020 2020 2022 2060 7b7d             " `{}
-000111c0: 6020 7769 6c6c 206e 6f74 2063 6f6d 7075  ` will not compu
-000111d0: 7465 2073 7461 7469 7374 6963 732e 220a  te statistics.".
-000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111f0: 292e 666f 726d 6174 2873 656c 662e 5f6e  ).format(self._n
-00011200: 616d 652c 2073 656c 662e 5f76 6572 7369  ame, self._versi
-00011210: 6f6e 292c 0a20 2020 2020 2020 2020 2020  on),.           
-00011220: 2020 2020 2075 7469 6c2e 5374 6174 6973       util.Statis
-00011230: 7469 6373 5761 726e 696e 672c 0a20 2020  ticsWarning,.   
-00011240: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00011250: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00011260: 656c 662e 5f66 6561 7475 7265 5f67 726f  elf._feature_gro
-00011270: 7570 5f65 6e67 696e 652e 696e 7365 7274  up_engine.insert
-00011280: 5f73 7472 6561 6d28 0a20 2020 2020 2020  _stream(.       
-00011290: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-000112a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000112b0: 6561 7475 7265 5f64 6174 6166 7261 6d65  eature_dataframe
-000112c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000112d0: 2020 7175 6572 795f 6e61 6d65 2c0a 2020    query_name,.  
-000112e0: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-000112f0: 7470 7574 5f6d 6f64 652c 0a20 2020 2020  tput_mode,.     
-00011300: 2020 2020 2020 2020 2020 2061 7761 6974             await
-00011310: 5f74 6572 6d69 6e61 7469 6f6e 2c0a 2020  _termination,.  
-00011320: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00011330: 6d65 6f75 742c 0a20 2020 2020 2020 2020  meout,.         
-00011340: 2020 2020 2020 2063 6865 636b 706f 696e         checkpoin
-00011350: 745f 6469 722c 0a20 2020 2020 2020 2020  t_dir,.         
-00011360: 2020 2020 2020 2077 7269 7465 5f6f 7074         write_opt
-00011370: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-00011380: 2020 290a 0a20 2020 2064 6566 2063 6f6d    )..    def com
-00011390: 6d69 745f 6465 7461 696c 7328 0a20 2020  mit_details(.   
-000113a0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000113b0: 2020 2077 616c 6c63 6c6f 636b 5f74 696d     wallclock_tim
-000113c0: 653a 204f 7074 696f 6e61 6c5b 556e 696f  e: Optional[Unio
-000113d0: 6e5b 7374 722c 2069 6e74 2c20 6461 7465  n[str, int, date
-000113e0: 7469 6d65 2c20 6461 7465 5d5d 203d 204e  time, date]] = N
-000113f0: 6f6e 652c 0a20 2020 2020 2020 206c 696d  one,.        lim
-00011400: 6974 3a20 4f70 7469 6f6e 616c 5b69 6e74  it: Optional[int
-00011410: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
-00011420: 0a20 2020 2020 2020 2022 2222 5265 7472  .        """Retr
-00011430: 6965 7665 7320 636f 6d6d 6974 2074 696d  ieves commit tim
-00011440: 656c 696e 6520 666f 7220 7468 6973 2066  eline for this f
-00011450: 6561 7475 7265 2067 726f 7570 2e20 5468  eature group. Th
-00011460: 6973 206d 6574 686f 6420 6361 6e20 6f6e  is method can on
-00011470: 6c79 2062 6520 7573 6564 0a20 2020 2020  ly be used.     
-00011480: 2020 206f 6e20 7469 6d65 2074 7261 7665     on time trave
-00011490: 6c20 656e 6162 6c65 6420 6665 6174 7572  l enabled featur
-000114a0: 6520 6772 6f75 7073 0a0a 2020 2020 2020  e groups..      
-000114b0: 2020 2121 2120 6578 616d 706c 650a 2020    !!! example.  
-000114c0: 2020 2020 2020 2020 2020 6060 6070 7974            ```pyt
-000114d0: 686f 6e0a 2020 2020 2020 2020 2020 2020  hon.            
-000114e0: 2320 636f 6e6e 6563 7420 746f 2074 6865  # connect to the
-000114f0: 2046 6561 7475 7265 2053 746f 7265 0a20   Feature Store. 
-00011500: 2020 2020 2020 2020 2020 2066 7320 3d20             fs = 
-00011510: 2e2e 2e0a 0a20 2020 2020 2020 2020 2020  .....           
-00011520: 2023 2067 6574 2074 6865 2046 6561 7475   # get the Featu
-00011530: 7265 2047 726f 7570 2069 6e73 7461 6e63  re Group instanc
-00011540: 650a 2020 2020 2020 2020 2020 2020 6667  e.            fg
-00011550: 203d 2066 732e 6765 745f 6f72 5f63 7265   = fs.get_or_cre
-00011560: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
-00011570: 7028 2e2e 2e29 0a0a 2020 2020 2020 2020  p(...)..        
-00011580: 2020 2020 636f 6d6d 6974 5f64 6574 6169      commit_detai
-00011590: 6c73 203d 2066 672e 636f 6d6d 6974 5f64  ls = fg.commit_d
-000115a0: 6574 6169 6c73 2829 0a20 2020 2020 2020  etails().       
-000115b0: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
-000115c0: 2020 2320 4172 6775 6d65 6e74 730a 2020    # Arguments.  
-000115d0: 2020 2020 2020 2020 2020 7761 6c6c 636c            wallcl
-000115e0: 6f63 6b5f 7469 6d65 3a20 436f 6d6d 6974  ock_time: Commit
-000115f0: 2064 6574 6169 6c73 2061 7320 6f66 2073   details as of s
-00011600: 7065 6369 6669 6320 706f 696e 7420 696e  pecific point in
-00011610: 2074 696d 652e 2044 6566 6175 6c74 7320   time. Defaults 
-00011620: 746f 2060 4e6f 6e65 602e 0a20 2020 2020  to `None`..     
-00011630: 2020 2020 2020 2020 2020 2020 5374 7269              Stri
-00011640: 6e67 7320 7368 6f75 6c64 2062 6520 666f  ngs should be fo
-00011650: 726d 6174 7465 6420 696e 206f 6e65 206f  rmatted in one o
-00011660: 6620 7468 6520 666f 6c6c 6f77 696e 6720  f the following 
-00011670: 666f 726d 6174 7320 6025 592d 256d 2d25  formats `%Y-%m-%
-00011680: 6460 2c20 6025 592d 256d 2d25 6420 2548  d`, `%Y-%m-%d %H
-00011690: 602c 2060 2559 2d25 6d2d 2564 2025 483a  `, `%Y-%m-%d %H:
-000116a0: 254d 602c 0a20 2020 2020 2020 2020 2020  %M`,.           
-000116b0: 2020 2020 2060 2559 2d25 6d2d 2564 2025       `%Y-%m-%d %
-000116c0: 483a 254d 3a25 5360 2c20 6f72 2060 2559  H:%M:%S`, or `%Y
-000116d0: 2d25 6d2d 2564 2025 483a 254d 3a25 532e  -%m-%d %H:%M:%S.
-000116e0: 2566 602e 0a20 2020 2020 2020 2020 2020  %f`..           
-000116f0: 206c 696d 6974 3a20 4e75 6d62 6572 206f   limit: Number o
-00011700: 6620 636f 6d6d 6974 7320 746f 2072 6574  f commits to ret
-00011710: 7269 6576 652e 2044 6566 6175 6c74 7320  rieve. Defaults 
-00011720: 746f 2060 4e6f 6e65 602e 0a0a 2020 2020  to `None`...    
-00011730: 2020 2020 2320 5265 7475 726e 730a 2020      # Returns.  
-00011740: 2020 2020 2020 2020 2020 6044 6963 745b            `Dict[
-00011750: 7374 722c 2044 6963 745b 7374 722c 2073  str, Dict[str, s
-00011760: 7472 5d5d 602e 2044 6963 7469 6f6e 6172  tr]]`. Dictionar
-00011770: 7920 6f62 6a65 6374 206f 6620 636f 6d6d  y object of comm
-00011780: 6974 206d 6574 6164 6174 6120 7469 6d65  it metadata time
-00011790: 6c69 6e65 2c20 7768 6572 6520 4b65 7920  line, where Key 
-000117a0: 6973 2063 6f6d 6d69 7420 6964 2061 6e64  is commit id and
-000117b0: 2076 616c 7565 0a20 2020 2020 2020 2020   value.         
-000117c0: 2020 2069 7320 6044 6963 745b 7374 722c     is `Dict[str,
-000117d0: 2073 7472 5d60 2077 6974 6820 6b65 7920   str]` with key 
-000117e0: 7661 6c75 6520 7061 6972 7320 6f66 2064  value pairs of d
-000117f0: 6174 6520 636f 6d6d 6974 7465 6420 6f6e  ate committed on
-00011800: 2c20 6e75 6d62 6572 206f 6620 726f 7773  , number of rows
-00011810: 2075 7064 6174 6564 2c20 696e 7365 7274   updated, insert
-00011820: 6564 2061 6e64 2064 656c 6574 6564 2e0a  ed and deleted..
-00011830: 0a20 2020 2020 2020 2023 2052 6169 7365  .        # Raise
-00011840: 730a 2020 2020 2020 2020 2020 2020 6068  s.            `h
-00011850: 7366 732e 636c 6965 6e74 2e65 7863 6570  sfs.client.excep
-00011860: 7469 6f6e 732e 5265 7374 4150 4945 7272  tions.RestAPIErr
-00011870: 6f72 602e 0a20 2020 2020 2020 2020 2020  or`..           
-00011880: 2060 6873 6673 2e63 6c69 656e 742e 6578   `hsfs.client.ex
-00011890: 6365 7074 696f 6e73 2e46 6561 7475 7265  ceptions.Feature
-000118a0: 5374 6f72 6545 7863 6570 7469 6f6e 602e  StoreException`.
-000118b0: 2049 6620 7468 6520 6665 6174 7572 6520   If the feature 
-000118c0: 6772 6f75 7020 646f 6573 206e 6f74 2068  group does not h
-000118d0: 6176 6520 6048 5544 4960 2074 696d 6520  ave `HUDI` time 
-000118e0: 7472 6176 656c 2066 6f72 6d61 740a 2020  travel format.  
-000118f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011900: 2020 7265 7475 726e 2073 656c 662e 5f66    return self._f
-00011910: 6561 7475 7265 5f67 726f 7570 5f65 6e67  eature_group_eng
-00011920: 696e 652e 636f 6d6d 6974 5f64 6574 6169  ine.commit_detai
-00011930: 6c73 2873 656c 662c 2077 616c 6c63 6c6f  ls(self, wallclo
-00011940: 636b 5f74 696d 652c 206c 696d 6974 290a  ck_time, limit).
-00011950: 0a20 2020 2064 6566 2063 6f6d 6d69 745f  .    def commit_
-00011960: 6465 6c65 7465 5f72 6563 6f72 6428 0a20  delete_record(. 
-00011970: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00011980: 2020 2020 2064 656c 6574 655f 6466 3a20       delete_df: 
-00011990: 5479 7065 5661 7228 2270 7973 7061 726b  TypeVar("pyspark
-000119a0: 2e73 716c 2e44 6174 6146 7261 6d65 2229  .sql.DataFrame")
-000119b0: 2c20 2023 206e 6f71 613a 2046 3832 310a  ,  # noqa: F821.
-000119c0: 2020 2020 2020 2020 7772 6974 655f 6f70          write_op
-000119d0: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
-000119e0: 4469 6374 5b41 6e79 2c20 416e 795d 5d20  Dict[Any, Any]] 
-000119f0: 3d20 7b7d 2c0a 2020 2020 293a 0a20 2020  = {},.    ):.   
-00011a00: 2020 2020 2022 2222 4472 6f70 7320 7265       """Drops re
-00011a10: 636f 7264 7320 7072 6573 656e 7420 696e  cords present in
-00011a20: 2074 6865 2070 726f 7669 6465 6420 4461   the provided Da
-00011a30: 7461 4672 616d 6520 616e 6420 636f 6d6d  taFrame and comm
-00011a40: 6974 7320 6974 2061 7320 7570 6461 7465  its it as update
-00011a50: 2074 6f20 7468 6973 0a20 2020 2020 2020   to this.       
-00011a60: 2046 6561 7475 7265 2067 726f 7570 2e20   Feature group. 
-00011a70: 5468 6973 206d 6574 686f 6420 6361 6e20  This method can 
-00011a80: 6f6e 6c79 2062 6520 7573 6564 206f 6e20  only be used on 
-00011a90: 7469 6d65 2074 7261 7665 6c20 656e 6162  time travel enab
-00011aa0: 6c65 6420 6665 6174 7572 6520 6772 6f75  led feature grou
-00011ab0: 7073 0a0a 2020 2020 2020 2020 2320 4172  ps..        # Ar
-00011ac0: 6775 6d65 6e74 730a 2020 2020 2020 2020  guments.        
-00011ad0: 2020 2020 6465 6c65 7465 5f64 663a 2064      delete_df: d
-00011ae0: 6174 6146 7261 6d65 2063 6f6e 7461 696e  ataFrame contain
-00011af0: 696e 6720 7265 636f 7264 7320 746f 2062  ing records to b
-00011b00: 6520 6465 6c65 7465 642e 0a20 2020 2020  e deleted..     
-00011b10: 2020 2020 2020 2077 7269 7465 5f6f 7074         write_opt
-00011b20: 696f 6e73 3a20 5573 6572 2070 726f 7669  ions: User provi
-00011b30: 6465 6420 7772 6974 6520 6f70 7469 6f6e  ded write option
-00011b40: 732e 2044 6566 6175 6c74 7320 746f 2060  s. Defaults to `
-00011b50: 7b7d 602e 0a0a 2020 2020 2020 2020 2320  {}`...        # 
-00011b60: 5261 6973 6573 0a20 2020 2020 2020 2020  Raises.         
-00011b70: 2020 2060 6873 6673 2e63 6c69 656e 742e     `hsfs.client.
-00011b80: 6578 6365 7074 696f 6e73 2e52 6573 7441  exceptions.RestA
-00011b90: 5049 4572 726f 7260 2e0a 2020 2020 2020  PIError`..      
-00011ba0: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
-00011bb0: 6c66 2e5f 6665 6174 7572 655f 6772 6f75  lf._feature_grou
-00011bc0: 705f 656e 6769 6e65 2e63 6f6d 6d69 745f  p_engine.commit_
-00011bd0: 6465 6c65 7465 2873 656c 662c 2064 656c  delete(self, del
-00011be0: 6574 655f 6466 2c20 7772 6974 655f 6f70  ete_df, write_op
-00011bf0: 7469 6f6e 7329 0a0a 2020 2020 6465 6620  tions)..    def 
-00011c00: 6173 5f6f 6628 0a20 2020 2020 2020 2073  as_of(.        s
-00011c10: 656c 662c 0a20 2020 2020 2020 2077 616c  elf,.        wal
-00011c20: 6c63 6c6f 636b 5f74 696d 653a 204f 7074  lclock_time: Opt
-00011c30: 696f 6e61 6c5b 556e 696f 6e5b 7374 722c  ional[Union[str,
-00011c40: 2069 6e74 2c20 6461 7465 7469 6d65 2c20   int, datetime, 
-00011c50: 6461 7465 5d5d 203d 204e 6f6e 652c 0a20  date]] = None,. 
-00011c60: 2020 2020 2020 2065 7863 6c75 6465 5f75         exclude_u
-00011c70: 6e74 696c 3a20 4f70 7469 6f6e 616c 5b55  ntil: Optional[U
-00011c80: 6e69 6f6e 5b73 7472 2c20 696e 742c 2064  nion[str, int, d
-00011c90: 6174 6574 696d 652c 2064 6174 655d 5d20  atetime, date]] 
-00011ca0: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-00011cb0: 2020 2020 2020 2022 2222 4765 7420 5175         """Get Qu
-00011cc0: 6572 7920 6f62 6a65 6374 2074 6f20 7265  ery object to re
-00011cd0: 7472 6965 7665 2061 6c6c 2066 6561 7475  trieve all featu
-00011ce0: 7265 7320 6f66 2074 6865 2067 726f 7570  res of the group
-00011cf0: 2061 7420 6120 706f 696e 7420 696e 2074   at a point in t
-00011d00: 6865 2070 6173 742e 0a0a 2020 2020 2020  he past...      
-00011d10: 2020 5468 6973 206d 6574 686f 6420 7365    This method se
-00011d20: 6c65 6374 7320 616c 6c20 6665 6174 7572  lects all featur
-00011d30: 6573 2069 6e20 7468 6520 6665 6174 7572  es in the featur
-00011d40: 6520 6772 6f75 7020 616e 6420 7265 7475  e group and retu
-00011d50: 726e 7320 6120 5175 6572 7920 6f62 6a65  rns a Query obje
-00011d60: 6374 0a20 2020 2020 2020 2061 7420 7468  ct.        at th
-00011d70: 6520 7370 6563 6966 6965 6420 706f 696e  e specified poin
-00011d80: 7420 696e 2074 696d 652e 204f 7074 696f  t in time. Optio
-00011d90: 6e61 6c6c 792c 2063 6f6d 6d69 7473 2062  nally, commits b
-00011da0: 6566 6f72 6520 6120 7370 6563 6966 6965  efore a specifie
-00011db0: 6420 706f 696e 7420 696e 2074 696d 6520  d point in time 
-00011dc0: 6361 6e20 6265 0a20 2020 2020 2020 2065  can be.        e
-00011dd0: 7863 6c75 6465 6420 6672 6f6d 2074 6865  xcluded from the
-00011de0: 2071 7565 7279 2e20 5468 6520 5175 6572   query. The Quer
-00011df0: 7920 6361 6e20 7468 656e 2065 6974 6865  y can then eithe
-00011e00: 7220 6265 2072 6561 6420 696e 746f 2061  r be read into a
-00011e10: 2044 6174 6166 7261 6d65 0a20 2020 2020   Dataframe.     
-00011e20: 2020 206f 7220 7573 6564 2066 7572 7468     or used furth
-00011e30: 6572 2074 6f20 7065 7266 6f72 6d20 6a6f  er to perform jo
-00011e40: 696e 7320 6f72 2063 6f6e 7374 7275 6374  ins or construct
-00011e50: 2061 2074 7261 696e 696e 6720 6461 7461   a training data
-00011e60: 7365 742e 0a0a 2020 2020 2020 2020 2121  set...        !!
-00011e70: 2120 6578 616d 706c 6520 2252 6561 6469  ! example "Readi
-00011e80: 6e67 2066 6561 7475 7265 7320 6174 2061  ng features at a
-00011e90: 2073 7065 6369 6669 6320 706f 696e 7420   specific point 
-00011ea0: 696e 2074 696d 653a 220a 2020 2020 2020  in time:".      
-00011eb0: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00011ec0: 2020 2020 2020 2020 2020 2020 2320 636f              # co
-00011ed0: 6e6e 6563 7420 746f 2074 6865 2046 6561  nnect to the Fea
-00011ee0: 7475 7265 2053 746f 7265 0a20 2020 2020  ture Store.     
-00011ef0: 2020 2020 2020 2066 7320 3d20 2e2e 2e0a         fs = ....
-00011f00: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
-00011f10: 6574 2074 6865 2046 6561 7475 7265 2047  et the Feature G
-00011f20: 726f 7570 2069 6e73 7461 6e63 650a 2020  roup instance.  
-00011f30: 2020 2020 2020 2020 2020 6667 203d 2066            fg = f
-00011f40: 732e 6765 745f 6f72 5f63 7265 6174 655f  s.get_or_create_
-00011f50: 6665 6174 7572 655f 6772 6f75 7028 2e2e  feature_group(..
-00011f60: 2e29 0a0a 2020 2020 2020 2020 2020 2020  .)..            
-00011f70: 2320 6765 7420 6461 7461 2061 7420 6120  # get data at a 
-00011f80: 7370 6563 6966 6963 2070 6f69 6e74 2069  specific point i
-00011f90: 6e20 7469 6d65 2061 6e64 2073 686f 7720  n time and show 
-00011fa0: 6974 0a20 2020 2020 2020 2020 2020 2066  it.            f
-00011fb0: 672e 6173 5f6f 6628 2232 3032 302d 3130  g.as_of("2020-10
-00011fc0: 2d32 3020 3037 3a33 343a 3131 2229 2e72  -20 07:34:11").r
-00011fd0: 6561 6428 292e 7368 6f77 2829 0a20 2020  ead().show().   
-00011fe0: 2020 2020 2020 2020 2060 6060 0a0a 2020           ```..  
-00011ff0: 2020 2020 2020 2121 2120 6578 616d 706c        !!! exampl
-00012000: 6520 2252 6561 6469 6e67 2063 6f6d 6d69  e "Reading commi
-00012010: 7473 2069 6e63 7265 6d65 6e74 616c 6c79  ts incrementally
-00012020: 2062 6574 7765 656e 2073 7065 6369 6669   between specifi
-00012030: 6564 2070 6f69 6e74 7320 696e 2074 696d  ed points in tim
-00012040: 653a 220a 2020 2020 2020 2020 2020 2020  e:".            
-00012050: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-00012060: 2020 2020 2020 6667 2e61 735f 6f66 2822        fg.as_of("
-00012070: 3230 3230 2d31 302d 3230 2030 373a 3334  2020-10-20 07:34
-00012080: 3a31 3122 2c20 6578 636c 7564 655f 756e  :11", exclude_un
-00012090: 7469 6c3d 2232 3032 302d 3130 2d31 3920  til="2020-10-19 
-000120a0: 3037 3a33 343a 3131 2229 2e72 6561 6428  07:34:11").read(
-000120b0: 292e 7368 6f77 2829 0a20 2020 2020 2020  ).show().       
-000120c0: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
-000120d0: 2020 5468 6520 6669 7273 7420 7061 7261    The first para
-000120e0: 6d65 7465 7220 6973 2069 6e63 6c75 7369  meter is inclusi
-000120f0: 7665 2077 6869 6c65 2074 6865 206c 6174  ve while the lat
-00012100: 7465 7220 6973 2065 7863 6c75 7369 7665  ter is exclusive
-00012110: 2e0a 2020 2020 2020 2020 5468 6174 206d  ..        That m
-00012120: 6561 6e73 2c20 696e 206f 7264 6572 2074  eans, in order t
-00012130: 6f20 7175 6572 7920 6120 7369 6e67 6c65  o query a single
-00012140: 2063 6f6d 6d69 742c 2079 6f75 206e 6565   commit, you nee
-00012150: 6420 746f 2071 7565 7279 2074 6861 7420  d to query that 
-00012160: 636f 6d6d 6974 2074 696d 650a 2020 2020  commit time.    
-00012170: 2020 2020 616e 6420 6578 636c 7564 6520      and exclude 
-00012180: 6576 6572 7974 6869 6e67 206a 7573 7420  everything just 
-00012190: 6265 666f 7265 2074 6865 2063 6f6d 6d69  before the commi
-000121a0: 742e 0a0a 2020 2020 2020 2020 2121 2120  t...        !!! 
-000121b0: 6578 616d 706c 6520 2252 6561 6469 6e67  example "Reading
-000121c0: 206f 6e6c 7920 7468 6520 6368 616e 6765   only the change
-000121d0: 7320 6672 6f6d 2061 2073 696e 676c 6520  s from a single 
-000121e0: 636f 6d6d 6974 220a 2020 2020 2020 2020  commit".        
-000121f0: 2020 2020 6060 6070 7974 686f 6e0a 2020      ```python.  
-00012200: 2020 2020 2020 2020 2020 6667 2e61 735f            fg.as_
-00012210: 6f66 2822 3230 3230 2d31 302d 3230 2030  of("2020-10-20 0
-00012220: 373a 3331 3a33 3822 2c20 6578 636c 7564  7:31:38", exclud
-00012230: 655f 756e 7469 6c3d 2232 3032 302d 3130  e_until="2020-10
-00012240: 2d32 3020 3037 3a33 313a 3337 2229 2e72  -20 07:31:37").r
-00012250: 6561 6428 292e 7368 6f77 2829 0a20 2020  ead().show().   
-00012260: 2020 2020 2020 2020 2060 6060 0a0a 2020           ```..  
-00012270: 2020 2020 2020 5768 656e 206e 6f20 7761        When no wa
-00012280: 6c6c 636c 6f63 6b5f 7469 6d65 2069 7320  llclock_time is 
-00012290: 6769 7665 6e2c 2074 6865 206c 6174 6573  given, the lates
-000122a0: 7420 7374 6174 6520 6f66 2066 6561 7475  t state of featu
-000122b0: 7265 7320 6973 2072 6574 7572 6e65 642e  res is returned.
-000122c0: 204f 7074 696f 6e61 6c6c 792c 2063 6f6d   Optionally, com
-000122d0: 6d69 7473 2062 6566 6f72 650a 2020 2020  mits before.    
-000122e0: 2020 2020 6120 7370 6563 6966 6965 6420      a specified 
-000122f0: 706f 696e 7420 696e 2074 696d 6520 6361  point in time ca
-00012300: 6e20 7374 696c 6c20 6265 2065 7863 6c75  n still be exclu
-00012310: 6465 642e 0a0a 2020 2020 2020 2020 2121  ded...        !!
-00012320: 2120 6578 616d 706c 6520 2252 6561 6469  ! example "Readi
-00012330: 6e67 2074 6865 206c 6174 6573 7420 7374  ng the latest st
-00012340: 6174 6520 6f66 2066 6561 7475 7265 732c  ate of features,
-00012350: 2065 7863 6c75 6469 6e67 2063 6f6d 6d69   excluding commi
-00012360: 7473 2062 6566 6f72 6520 6120 7370 6563  ts before a spec
-00012370: 6966 6965 6420 706f 696e 7420 696e 2074  ified point in t
-00012380: 696d 653a 220a 2020 2020 2020 2020 2020  ime:".          
-00012390: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
-000123a0: 2020 2020 2020 2020 6667 2e61 735f 6f66          fg.as_of
-000123b0: 284e 6f6e 652c 2065 7863 6c75 6465 5f75  (None, exclude_u
-000123c0: 6e74 696c 3d22 3230 3230 2d31 302d 3230  ntil="2020-10-20
-000123d0: 2030 373a 3331 3a33 3822 292e 7265 6164   07:31:38").read
-000123e0: 2829 2e73 686f 7728 290a 2020 2020 2020  ().show().      
-000123f0: 2020 2020 2020 6060 600a 0a20 2020 2020        ```..     
-00012400: 2020 204e 6f74 6520 7468 6174 2074 6865     Note that the
-00012410: 2069 6e74 6572 7661 6c20 7769 6c6c 2062   interval will b
-00012420: 6520 6170 706c 6965 6420 746f 2061 6c6c  e applied to all
-00012430: 206a 6f69 6e73 2069 6e20 7468 6520 7175   joins in the qu
-00012440: 6572 792e 0a20 2020 2020 2020 2049 6620  ery..        If 
-00012450: 796f 7520 7761 6e74 2074 6f20 7175 6572  you want to quer
-00012460: 7920 6469 6666 6572 656e 7420 696e 7465  y different inte
-00012470: 7276 616c 7320 666f 7220 6469 6666 6572  rvals for differ
-00012480: 656e 7420 6665 6174 7572 6520 6772 6f75  ent feature grou
-00012490: 7073 2069 6e0a 2020 2020 2020 2020 7468  ps in.        th
-000124a0: 6520 7175 6572 792c 2079 6f75 2068 6176  e query, you hav
-000124b0: 6520 746f 2061 7070 6c79 2074 6865 6d20  e to apply them 
-000124c0: 696e 2061 206e 6573 7465 6420 6661 7368  in a nested fash
-000124d0: 696f 6e3a 0a20 2020 2020 2020 2021 2121  ion:.        !!!
-000124e0: 2065 7861 6d70 6c65 0a20 2020 2020 2020   example.       
-000124f0: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
-00012500: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
-00012510: 6e65 6374 2074 6f20 7468 6520 4665 6174  nect to the Feat
-00012520: 7572 6520 5374 6f72 650a 2020 2020 2020  ure Store.      
-00012530: 2020 2020 2020 6673 203d 202e 2e2e 0a0a        fs = .....
-00012540: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
-00012550: 7420 7468 6520 4665 6174 7572 6520 4772  t the Feature Gr
-00012560: 6f75 7020 696e 7374 616e 6365 0a20 2020  oup instance.   
-00012570: 2020 2020 2020 2020 2066 6731 203d 2066           fg1 = f
-00012580: 732e 6765 745f 6f72 5f63 7265 6174 655f  s.get_or_create_
-00012590: 6665 6174 7572 655f 6772 6f75 7028 2e2e  feature_group(..
-000125a0: 2e29 0a20 2020 2020 2020 2020 2020 2066  .).            f
-000125b0: 6732 203d 2066 732e 6765 745f 6f72 5f63  g2 = fs.get_or_c
-000125c0: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
-000125d0: 6f75 7028 2e2e 2e29 0a0a 2020 2020 2020  oup(...)..      
-000125e0: 2020 2020 2020 6667 312e 7365 6c65 6374        fg1.select
-000125f0: 5f61 6c6c 2829 2e61 735f 6f66 2822 3230  _all().as_of("20
-00012600: 3230 2d31 302d 3230 222c 2065 7863 6c75  20-10-20", exclu
-00012610: 6465 5f75 6e74 696c 3d22 3230 3230 2d31  de_until="2020-1
-00012620: 302d 3139 2229 0a20 2020 2020 2020 2020  0-19").         
-00012630: 2020 2020 2020 202e 6a6f 696e 2866 6732         .join(fg2
-00012640: 2e73 656c 6563 745f 616c 6c28 292e 6173  .select_all().as
-00012650: 5f6f 6628 2232 3032 302d 3130 2d32 3022  _of("2020-10-20"
-00012660: 2c20 6578 636c 7564 655f 756e 7469 6c3d  , exclude_until=
-00012670: 2232 3032 302d 3130 2d31 3922 2929 0a20  "2020-10-19")). 
-00012680: 2020 2020 2020 2020 2020 2060 6060 0a0a             ```..
-00012690: 2020 2020 2020 2020 4966 2069 6e73 7465          If inste
-000126a0: 6164 2079 6f75 2061 7070 6c79 2061 6e6f  ad you apply ano
-000126b0: 7468 6572 2060 6173 5f6f 6660 2073 656c  ther `as_of` sel
-000126c0: 6563 7469 6f6e 2061 6674 6572 2074 6865  ection after the
-000126d0: 206a 6f69 6e2c 2061 6c6c 0a20 2020 2020   join, all.     
-000126e0: 2020 206a 6f69 6e65 6420 6665 6174 7572     joined featur
-000126f0: 6520 6772 6f75 7073 2077 696c 6c20 6265  e groups will be
-00012700: 2071 7565 7269 6564 2077 6974 6820 7468   queried with th
-00012710: 6973 2069 6e74 6572 7661 6c3a 0a20 2020  is interval:.   
-00012720: 2020 2020 2021 2121 2065 7861 6d70 6c65       !!! example
-00012730: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
-00012740: 7079 7468 6f6e 0a20 2020 2020 2020 2020  python.         
-00012750: 2020 2066 6731 2e73 656c 6563 745f 616c     fg1.select_al
-00012760: 6c28 292e 6173 5f6f 6628 2232 3032 302d  l().as_of("2020-
-00012770: 3130 2d32 3022 2c20 6578 636c 7564 655f  10-20", exclude_
-00012780: 756e 7469 6c3d 2232 3032 302d 3130 2d31  until="2020-10-1
-00012790: 3922 2920 2023 2061 735f 6f66 2069 7320  9")  # as_of is 
-000127a0: 6e6f 7420 6170 706c 6965 640a 2020 2020  not applied.    
-000127b0: 2020 2020 2020 2020 2020 2020 2e6a 6f69              .joi
-000127c0: 6e28 6667 322e 7365 6c65 6374 5f61 6c6c  n(fg2.select_all
-000127d0: 2829 2e61 735f 6f66 2822 3230 3230 2d31  ().as_of("2020-1
-000127e0: 302d 3230 222c 2065 7863 6c75 6465 5f75  0-20", exclude_u
-000127f0: 6e74 696c 3d22 3230 3230 2d31 302d 3135  ntil="2020-10-15
-00012800: 2229 2920 2023 2061 735f 6f66 2069 7320  "))  # as_of is 
-00012810: 6e6f 7420 6170 706c 6965 640a 2020 2020  not applied.    
-00012820: 2020 2020 2020 2020 2020 2020 2e61 735f              .as_
-00012830: 6f66 2822 3230 3230 2d31 302d 3230 222c  of("2020-10-20",
-00012840: 2065 7863 6c75 6465 5f75 6e74 696c 3d22   exclude_until="
-00012850: 3230 3230 2d31 302d 3139 2229 0a20 2020  2020-10-19").   
-00012860: 2020 2020 2020 2020 2060 6060 0a0a 2020           ```..  
-00012870: 2020 2020 2020 2121 2120 7761 726e 696e        !!! warnin
-00012880: 670a 2020 2020 2020 2020 2020 2020 5468  g.            Th
-00012890: 6973 2066 756e 6374 696f 6e20 6f6e 6c79  is function only
-000128a0: 2077 6f72 6b73 2066 6f72 2066 6561 7475   works for featu
-000128b0: 7265 2067 726f 7570 7320 7769 7468 2074  re groups with t
-000128c0: 696d 655f 7472 6176 656c 5f66 6f72 6d61  ime_travel_forma
-000128d0: 743d 2748 5544 4927 2e0a 0a20 2020 2020  t='HUDI'...     
-000128e0: 2020 2021 2121 2077 6172 6e69 6e67 0a20     !!! warning. 
-000128f0: 2020 2020 2020 2020 2020 2045 7863 6c75             Exclu
-00012900: 6469 6e67 2063 6f6d 6d69 7473 2076 6961  ding commits via
-00012910: 2065 7863 6c75 6465 5f75 6e74 696c 2069   exclude_until i
-00012920: 7320 6f6e 6c79 2070 6f73 7369 626c 6520  s only possible 
-00012930: 7769 7468 696e 2074 6865 2072 616e 6765  within the range
-00012940: 206f 6620 7468 6520 4875 6469 2061 6374   of the Hudi act
-00012950: 6976 6520 7469 6d65 6c69 6e65 2e0a 2020  ive timeline..  
-00012960: 2020 2020 2020 2020 2020 4279 2064 6566            By def
-00012970: 6175 6c74 2c20 4875 6469 206b 6565 7073  ault, Hudi keeps
-00012980: 2074 6865 206c 6173 7420 3230 2074 6f20   the last 20 to 
-00012990: 3330 2063 6f6d 6d69 7473 2069 6e20 7468  30 commits in th
-000129a0: 6520 6163 7469 7665 2074 696d 656c 696e  e active timelin
-000129b0: 652e 0a20 2020 2020 2020 2020 2020 2049  e..            I
-000129c0: 6620 796f 7520 6e65 6564 2074 6f20 6b65  f you need to ke
-000129d0: 6570 2061 206c 6f6e 6765 7220 6163 7469  ep a longer acti
-000129e0: 7665 2074 696d 656c 696e 652c 2079 6f75  ve timeline, you
-000129f0: 2063 616e 206f 7665 7277 7269 7465 2074   can overwrite t
-00012a00: 6865 206f 7074 696f 6e73 3a0a 2020 2020  he options:.    
-00012a10: 2020 2020 2020 2020 6068 6f6f 6469 652e          `hoodie.
-00012a20: 6b65 6570 2e6d 696e 2e63 6f6d 6d69 7473  keep.min.commits
-00012a30: 6020 616e 6420 6068 6f6f 6469 652e 6b65  ` and `hoodie.ke
-00012a40: 6570 2e6d 6178 2e63 6f6d 6d69 7473 600a  ep.max.commits`.
-00012a50: 2020 2020 2020 2020 2020 2020 7768 656e              when
-00012a60: 2063 616c 6c69 6e67 2074 6865 2060 696e   calling the `in
-00012a70: 7365 7274 2829 6020 6d65 7468 6f64 2e0a  sert()` method..
-00012a80: 0a20 2020 2020 2020 2023 2041 7267 756d  .        # Argum
-00012a90: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
-00012aa0: 2077 616c 6c63 6c6f 636b 5f74 696d 653a   wallclock_time:
-00012ab0: 2052 6561 6420 6461 7461 2061 7320 6f66   Read data as of
-00012ac0: 2074 6869 7320 706f 696e 7420 696e 2074   this point in t
-00012ad0: 696d 652e 2053 7472 696e 6773 2073 686f  ime. Strings sho
-00012ae0: 756c 6420 6265 2066 6f72 6d61 7474 6564  uld be formatted
-00012af0: 2069 6e20 6f6e 6520 6f66 2074 6865 0a20   in one of the. 
-00012b00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00012b10: 6f6c 6c6f 7769 6e67 2066 6f72 6d61 7473  ollowing formats
-00012b20: 2060 2559 2d25 6d2d 2564 602c 2060 2559   `%Y-%m-%d`, `%Y
-00012b30: 2d25 6d2d 2564 2025 4860 2c20 6025 592d  -%m-%d %H`, `%Y-
-00012b40: 256d 2d25 6420 2548 3a25 4d60 2c20 6f72  %m-%d %H:%M`, or
-00012b50: 2060 2559 2d25 6d2d 2564 2025 483a 254d   `%Y-%m-%d %H:%M
-00012b60: 3a25 5360 2e0a 2020 2020 2020 2020 2020  :%S`..          
-00012b70: 2020 6578 636c 7564 655f 756e 7469 6c3a    exclude_until:
-00012b80: 2045 7863 6c75 6465 2063 6f6d 6d69 7473   Exclude commits
-00012b90: 2075 6e74 696c 2074 6869 7320 706f 696e   until this poin
-00012ba0: 7420 696e 2074 696d 652e 2053 7472 696e  t in time. Strin
-00012bb0: 6720 7368 6f75 6c64 2062 6520 666f 726d  g should be form
-00012bc0: 6174 7465 6420 696e 206f 6e65 206f 6620  atted in one of 
-00012bd0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-00012be0: 2020 2020 666f 6c6c 6f77 696e 6720 666f      following fo
-00012bf0: 726d 6174 7320 6025 592d 256d 2d25 6460  rmats `%Y-%m-%d`
-00012c00: 2c20 6025 592d 256d 2d25 6420 2548 602c  , `%Y-%m-%d %H`,
-00012c10: 2060 2559 2d25 6d2d 2564 2025 483a 254d   `%Y-%m-%d %H:%M
-00012c20: 602c 206f 7220 6025 592d 256d 2d25 6420  `, or `%Y-%m-%d 
-00012c30: 2548 3a25 4d3a 2553 602e 0a0a 2020 2020  %H:%M:%S`...    
-00012c40: 2020 2020 2320 5265 7475 726e 730a 2020      # Returns.  
-00012c50: 2020 2020 2020 2020 2020 6051 7565 7279            `Query
-00012c60: 602e 2054 6865 2071 7565 7279 206f 626a  `. The query obj
-00012c70: 6563 7420 7769 7468 2074 6865 2061 7070  ect with the app
-00012c80: 6c69 6564 2074 696d 6520 7472 6176 656c  lied time travel
-00012c90: 2063 6f6e 6469 7469 6f6e 2e0a 2020 2020   condition..    
-00012ca0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012cb0: 7265 7475 726e 2073 656c 662e 7365 6c65  return self.sele
-00012cc0: 6374 5f61 6c6c 2829 2e61 735f 6f66 2877  ct_all().as_of(w
-00012cd0: 616c 6c63 6c6f 636b 5f74 696d 652c 2065  allclock_time, e
-00012ce0: 7863 6c75 6465 5f75 6e74 696c 290a 0a20  xclude_until).. 
-00012cf0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00012d00: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00012d10: 2020 2020 2020 2064 6174 6166 7261 6d65         dataframe
-00012d20: 3a20 4f70 7469 6f6e 616c 5b0a 2020 2020  : Optional[.    
-00012d30: 2020 2020 2020 2020 556e 696f 6e5b 7064          Union[pd
-00012d40: 2e44 6174 6146 7261 6d65 2c20 5479 7065  .DataFrame, Type
-00012d50: 5661 7228 2270 7973 7061 726b 2e73 716c  Var("pyspark.sql
-00012d60: 2e44 6174 6146 7261 6d65 2229 5d20 2023  .DataFrame")]  #
-00012d70: 206e 6f71 613a 2046 3832 310a 2020 2020   noqa: F821.    
-00012d80: 2020 2020 5d20 3d20 4e6f 6e65 2c0a 2020      ] = None,.  
-00012d90: 2020 2020 2020 6578 7065 6374 6174 696f        expectatio
-00012da0: 6e5f 7375 6974 653a 204f 7074 696f 6e61  n_suite: Optiona
-00012db0: 6c5b 4578 7065 6374 6174 696f 6e53 7569  l[ExpectationSui
-00012dc0: 7465 5d20 3d20 4e6f 6e65 2c0a 2020 2020  te] = None,.    
-00012dd0: 2020 2020 7361 7665 5f72 6570 6f72 743a      save_report:
-00012de0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
-00012df0: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
-00012e00: 2076 616c 6964 6174 696f 6e5f 6f70 7469   validation_opti
-00012e10: 6f6e 733a 204f 7074 696f 6e61 6c5b 4469  ons: Optional[Di
-00012e20: 6374 5b41 6e79 2c20 416e 795d 5d20 3d20  ct[Any, Any]] = 
-00012e30: 7b7d 2c0a 2020 2020 2020 2020 696e 6765  {},.        inge
-00012e40: 7374 696f 6e5f 7265 7375 6c74 3a20 7374  stion_result: st
-00012e50: 7220 3d20 2255 4e4b 4e4f 574e 222c 0a20  r = "UNKNOWN",. 
-00012e60: 2020 2020 2020 2067 655f 7479 7065 3a20         ge_type: 
-00012e70: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-00012e80: 2029 202d 3e20 556e 696f 6e5b 6765 2e63   ) -> Union[ge.c
-00012e90: 6f72 652e 4578 7065 6374 6174 696f 6e53  ore.ExpectationS
-00012ea0: 7569 7465 5661 6c69 6461 7469 6f6e 5265  uiteValidationRe
-00012eb0: 7375 6c74 2c20 5661 6c69 6461 7469 6f6e  sult, Validation
-00012ec0: 5265 706f 7274 2c20 4e6f 6e65 5d3a 0a20  Report, None]:. 
-00012ed0: 2020 2020 2020 2022 2222 5275 6e20 7661         """Run va
-00012ee0: 6c69 6461 7469 6f6e 2062 6173 6564 206f  lidation based o
-00012ef0: 6e20 7468 6520 6174 7461 6368 6564 2065  n the attached e
-00012f00: 7870 6563 7461 7469 6f6e 732e 0a0a 2020  xpectations...  
-00012f10: 2020 2020 2020 5275 6e73 2061 6e79 2065        Runs any e
-00012f20: 7870 6563 7461 7469 6f6e 2061 7474 6163  xpectation attac
-00012f30: 6865 6420 7769 7468 2044 6565 7175 2e20  hed with Deequ. 
-00012f40: 4275 7420 616c 736f 2072 756e 7320 6174  But also runs at
-00012f50: 7461 6368 6564 2047 7265 6174 2045 7870  tached Great Exp
-00012f60: 6563 7461 7469 6f6e 0a20 2020 2020 2020  ectation.       
-00012f70: 2053 7569 7465 732e 0a0a 2020 2020 2020   Suites...      
-00012f80: 2020 2121 2120 6578 616d 706c 650a 2020    !!! example.  
-00012f90: 2020 2020 2020 2020 2020 6060 6070 7974            ```pyt
-00012fa0: 686f 6e0a 2020 2020 2020 2020 2020 2020  hon.            
-00012fb0: 2320 636f 6e6e 6563 7420 746f 2074 6865  # connect to the
-00012fc0: 2046 6561 7475 7265 2053 746f 7265 0a20   Feature Store. 
-00012fd0: 2020 2020 2020 2020 2020 2066 7320 3d20             fs = 
-00012fe0: 2e2e 2e0a 0a20 2020 2020 2020 2020 2020  .....           
-00012ff0: 2023 2067 6574 2066 6561 7475 7265 2067   # get feature g
-00013000: 726f 7570 2069 6e73 7461 6e63 650a 2020  roup instance.  
-00013010: 2020 2020 2020 2020 2020 6667 203d 2066            fg = f
-00013020: 732e 6765 745f 6f72 5f63 7265 6174 655f  s.get_or_create_
-00013030: 6665 6174 7572 655f 6772 6f75 7028 2e2e  feature_group(..
-00013040: 2e29 0a0a 2020 2020 2020 2020 2020 2020  .)..            
-00013050: 6765 5f72 6570 6f72 7420 3d20 6667 2e76  ge_report = fg.v
-00013060: 616c 6964 6174 6528 6466 2c20 7361 7665  alidate(df, save
-00013070: 5f72 6570 6f72 743d 4661 6c73 6529 0a20  _report=False). 
-00013080: 2020 2020 2020 2020 2020 2060 6060 0a0a             ```..
-00013090: 2020 2020 2020 2020 2320 4172 6775 6d65          # Argume
-000130a0: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-000130b0: 6461 7461 6672 616d 653a 2054 6865 2064  dataframe: The d
-000130c0: 6174 6166 7261 6d65 2074 6f20 7275 6e20  ataframe to run 
-000130d0: 7468 6520 6461 7461 2076 616c 6964 6174  the data validat
-000130e0: 696f 6e20 6578 7065 6374 6174 696f 6e73  ion expectations
-000130f0: 2061 6761 696e 7374 2e0a 2020 2020 2020   against..      
-00013100: 2020 2020 2020 6578 7065 6374 6174 696f        expectatio
-00013110: 6e5f 7375 6974 653a 204f 7074 696f 6e61  n_suite: Optiona
-00013120: 6c6c 7920 7072 6f76 6964 6520 616e 2045  lly provide an E
-00013130: 7870 6563 7461 7469 6f6e 2053 7569 7465  xpectation Suite
-00013140: 2074 6f20 6f76 6572 7269 6465 2074 6865   to override the
-00013150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013160: 206f 6e65 2074 6861 7420 6973 2070 6f73   one that is pos
-00013170: 7369 626c 7920 6174 7461 6368 6564 2074  sibly attached t
-00013180: 6f20 7468 6520 6665 6174 7572 6520 6772  o the feature gr
-00013190: 6f75 702e 2054 6869 7320 6973 2075 7365  oup. This is use
-000131a0: 6675 6c20 666f 720a 2020 2020 2020 2020  ful for.        
-000131b0: 2020 2020 2020 2020 7465 7374 696e 6720          testing 
-000131c0: 6e65 7720 4578 7065 6374 6174 696f 6e20  new Expectation 
-000131d0: 7375 6974 6573 2e20 5768 656e 2061 6e20  suites. When an 
-000131e0: 6578 7472 6120 7375 6974 6520 6973 2070  extra suite is p
-000131f0: 726f 7669 6465 642c 2074 6865 2072 6573  rovided, the res
-00013200: 756c 7473 0a20 2020 2020 2020 2020 2020  ults.           
-00013210: 2020 2020 2077 696c 6c20 6e65 7665 7220       will never 
-00013220: 6265 2070 6572 7369 7374 6564 2e20 4465  be persisted. De
-00013230: 6661 756c 7473 2074 6f20 604e 6f6e 6560  faults to `None`
-00013240: 2e0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-00013250: 6c69 6461 7469 6f6e 5f6f 7074 696f 6e73  lidation_options
-00013260: 3a20 4164 6469 7469 6f6e 616c 2076 616c  : Additional val
-00013270: 6964 6174 696f 6e20 6f70 7469 6f6e 7320  idation options 
-00013280: 6173 206b 6579 2d76 616c 7565 2070 6169  as key-value pai
-00013290: 7273 2c20 6465 6661 756c 7473 2074 6f20  rs, defaults to 
-000132a0: 607b 7d60 2e0a 2020 2020 2020 2020 2020  `{}`..          
-000132b0: 2020 2020 2020 2a20 6b65 7920 6072 756e        * key `run
-000132c0: 5f76 616c 6964 6174 696f 6e60 2062 6f6f  _validation` boo
-000132d0: 6c65 616e 2076 616c 7565 2c20 7365 7420  lean value, set 
-000132e0: 746f 2060 4661 6c73 6560 2074 6f20 736b  to `False` to sk
-000132f0: 6970 2076 616c 6964 6174 696f 6e20 7465  ip validation te
-00013300: 6d70 6f72 6172 696c 7920 6f6e 2069 6e67  mporarily on ing
-00013310: 6573 7469 6f6e 2e0a 2020 2020 2020 2020  estion..        
-00013320: 2020 2020 2020 2020 2a20 6b65 7920 6067          * key `g
-00013330: 655f 7661 6c69 6461 7465 5f6b 7761 7267  e_validate_kwarg
-00013340: 7360 2061 2064 6963 7469 6f6e 6172 7920  s` a dictionary 
-00013350: 636f 6e74 6169 6e69 6e67 206b 7761 7267  containing kwarg
-00013360: 7320 666f 7220 7468 6520 7661 6c69 6461  s for the valida
-00013370: 7465 206d 6574 686f 6420 6f66 2047 7265  te method of Gre
-00013380: 6174 2045 7870 6563 7461 7469 6f6e 732e  at Expectations.
-00013390: 0a20 2020 2020 2020 2020 2020 2069 6e67  .            ing
-000133a0: 6573 7469 6f6e 5f72 6573 756c 743a 2053  estion_result: S
-000133b0: 7065 6369 6679 2074 6865 2066 6174 6520  pecify the fate 
-000133c0: 6f66 2074 6865 2061 7373 6f63 6961 7465  of the associate
-000133d0: 6420 6461 7461 2c20 6465 6661 756c 7473  d data, defaults
-000133e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000133f0: 2074 6f20 2255 4e4b 4e4f 574e 222e 2053   to "UNKNOWN". S
-00013400: 7570 706f 7274 6564 206f 7074 696f 6e73  upported options
-00013410: 2061 7265 2020 2255 4e4b 4e4f 574e 222c   are  "UNKNOWN",
-00013420: 2022 494e 4745 5354 4544 222c 2022 5245   "INGESTED", "RE
-00013430: 4a45 4354 4544 222c 0a20 2020 2020 2020  JECTED",.       
-00013440: 2020 2020 2020 2020 2022 4558 5045 5249           "EXPERI
-00013450: 4d45 4e54 222c 2022 4647 5f44 4154 4122  MENT", "FG_DATA"
-00013460: 2e20 5573 6520 2249 4e47 4553 5445 4422  . Use "INGESTED"
-00013470: 206f 7220 2252 454a 4543 5445 4422 2066   or "REJECTED" f
-00013480: 6f72 2076 616c 6964 6174 696f 6e0a 2020  or validation.  
-00013490: 2020 2020 2020 2020 2020 2020 2020 6f66                of
-000134a0: 2044 6174 6146 7261 6d65 7320 746f 2062   DataFrames to b
-000134b0: 6520 696e 7365 7274 6564 2069 6e20 7468  e inserted in th
-000134c0: 6520 4665 6174 7572 6520 4772 6f75 702e  e Feature Group.
-000134d0: 2055 7365 2022 4558 5045 5249 4d45 4e54   Use "EXPERIMENT
-000134e0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000134f0: 2020 666f 7220 7465 7374 696e 6720 616e    for testing an
-00013500: 6420 6465 7665 6c6f 706d 656e 7420 616e  d development an
-00013510: 6420 2246 475f 4441 5441 2220 7768 656e  d "FG_DATA" when
-00013520: 2076 616c 6964 6174 696e 6720 6461 7461   validating data
-00013530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013540: 2061 6c72 6561 6479 2069 6e20 7468 6520   already in the 
-00013550: 4665 6174 7572 6520 4772 6f75 702e 0a20  Feature Group.. 
-00013560: 2020 2020 2020 2020 2020 2073 6176 655f             save_
-00013570: 7265 706f 7274 3a20 5768 6574 6865 7220  report: Whether 
-00013580: 746f 2073 6176 6520 7468 6520 7265 706f  to save the repo
-00013590: 7274 2074 6f20 7468 6520 6261 636b 656e  rt to the backen
-000135a0: 642e 2054 6869 7320 6973 206f 6e6c 7920  d. This is only 
-000135b0: 706f 7373 6962 6c65 2069 6620 7468 6520  possible if the 
-000135c0: 4578 7065 6374 6174 696f 6e20 7375 6974  Expectation suit
-000135d0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000135e0: 2020 6973 2069 6e69 7469 616c 6973 6564    is initialised
-000135f0: 2061 6e64 2061 7474 6163 6865 6420 746f   and attached to
-00013600: 2074 6865 2046 6561 7475 7265 2047 726f   the Feature Gro
-00013610: 7570 2e20 4465 6661 756c 7473 2074 6f20  up. Defaults to 
-00013620: 4661 6c73 652e 0a20 2020 2020 2020 2020  False..         
-00013630: 2020 2067 655f 7479 7065 3a20 5768 6574     ge_type: Whet
-00013640: 6865 7220 746f 2072 6574 7572 6e20 6120  her to return a 
-00013650: 4772 6561 7420 4578 7065 6374 6174 696f  Great Expectatio
-00013660: 6e73 206f 626a 6563 7420 6f72 2048 6f70  ns object or Hop
-00013670: 7377 6f72 6b73 206f 776e 2061 6273 7472  sworks own abstr
-00013680: 6163 7469 6f6e 2e20 4465 6661 756c 7473  action. Defaults
-00013690: 2074 6f20 5472 7565 2e0a 0a20 2020 2020   to True...     
-000136a0: 2020 2023 2052 6574 7572 6e73 0a20 2020     # Returns.   
-000136b0: 2020 2020 2020 2020 2041 2056 616c 6964           A Valid
-000136c0: 6174 696f 6e20 5265 706f 7274 2070 726f  ation Report pro
-000136d0: 6475 6365 6420 6279 2047 7265 6174 2045  duced by Great E
-000136e0: 7870 6563 7461 7469 6f6e 732e 0a20 2020  xpectations..   
-000136f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013700: 2023 2041 6374 6976 6974 7920 6973 206c   # Activity is l
-00013710: 6f67 6765 6420 6f6e 6c79 2069 6620 6120  ogged only if a 
-00013720: 7468 6520 7661 6c69 6461 7469 6f6e 2063  the validation c
-00013730: 6f6e 6365 726e 7320 7468 6520 6665 6174  oncerns the feat
-00013740: 7572 6520 6772 6f75 7020 616e 6420 6e6f  ure group and no
-00013750: 7420 6120 7370 6563 6966 6963 2064 6174  t a specific dat
-00013760: 6166 7261 6d65 0a20 2020 2020 2020 2069  aframe.        i
-00013770: 6620 6461 7461 6672 616d 6520 6973 204e  f dataframe is N
-00013780: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00013790: 2064 6174 6166 7261 6d65 203d 2073 656c   dataframe = sel
-000137a0: 662e 7265 6164 2829 0a20 2020 2020 2020  f.read().       
-000137b0: 2020 2020 2069 6620 696e 6765 7374 696f       if ingestio
-000137c0: 6e5f 7265 7375 6c74 203d 3d20 2255 4e4b  n_result == "UNK
-000137d0: 4e4f 574e 223a 0a20 2020 2020 2020 2020  NOWN":.         
-000137e0: 2020 2020 2020 2069 6e67 6573 7469 6f6e         ingestion
-000137f0: 5f72 6573 756c 7420 3d20 2246 475f 4441  _result = "FG_DA
-00013800: 5441 220a 0a20 2020 2020 2020 2072 6574  TA"..        ret
-00013810: 7572 6e20 7365 6c66 2e5f 6772 6561 745f  urn self._great_
-00013820: 6578 7065 6374 6174 696f 6e5f 656e 6769  expectation_engi
-00013830: 6e65 2e76 616c 6964 6174 6528 0a20 2020  ne.validate(.   
-00013840: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-00013850: 2020 2020 2020 2020 2020 2064 6174 6166             dataf
-00013860: 7261 6d65 3d65 6e67 696e 652e 6765 745f  rame=engine.get_
-00013870: 696e 7374 616e 6365 2829 2e63 6f6e 7665  instance().conve
-00013880: 7274 5f74 6f5f 6465 6661 756c 745f 6461  rt_to_default_da
-00013890: 7461 6672 616d 6528 6461 7461 6672 616d  taframe(datafram
-000138a0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-000138b0: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
-000138c0: 653d 6578 7065 6374 6174 696f 6e5f 7375  e=expectation_su
-000138d0: 6974 652c 0a20 2020 2020 2020 2020 2020  ite,.           
-000138e0: 2073 6176 655f 7265 706f 7274 3d73 6176   save_report=sav
-000138f0: 655f 7265 706f 7274 2c0a 2020 2020 2020  e_report,.      
-00013900: 2020 2020 2020 7661 6c69 6461 7469 6f6e        validation
-00013910: 5f6f 7074 696f 6e73 3d76 616c 6964 6174  _options=validat
-00013920: 696f 6e5f 6f70 7469 6f6e 732c 0a20 2020  ion_options,.   
-00013930: 2020 2020 2020 2020 2069 6e67 6573 7469           ingesti
-00013940: 6f6e 5f72 6573 756c 743d 696e 6765 7374  on_result=ingest
-00013950: 696f 6e5f 7265 7375 6c74 2c0a 2020 2020  ion_result,.    
-00013960: 2020 2020 2020 2020 6765 5f74 7970 653d          ge_type=
-00013970: 6765 5f74 7970 652c 0a20 2020 2020 2020  ge_type,.       
-00013980: 2029 0a0a 2020 2020 6465 6620 636f 6d70   )..    def comp
-00013990: 7574 655f 7374 6174 6973 7469 6373 280a  ute_statistics(.
-000139a0: 2020 2020 2020 2020 7365 6c66 2c20 7761          self, wa
-000139b0: 6c6c 636c 6f63 6b5f 7469 6d65 3a20 4f70  llclock_time: Op
-000139c0: 7469 6f6e 616c 5b55 6e69 6f6e 5b73 7472  tional[Union[str
-000139d0: 2c20 696e 742c 2064 6174 6574 696d 652c  , int, datetime,
-000139e0: 2064 6174 655d 5d20 3d20 4e6f 6e65 0a20   date]] = None. 
-000139f0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-00013a00: 2252 6563 6f6d 7075 7465 2074 6865 2073  "Recompute the s
-00013a10: 7461 7469 7374 6963 7320 666f 7220 7468  tatistics for th
-00013a20: 6520 6665 6174 7572 6520 6772 6f75 7020  e feature group 
-00013a30: 616e 6420 7361 7665 2074 6865 6d20 746f  and save them to
-00013a40: 2074 6865 0a20 2020 2020 2020 2066 6561   the.        fea
-00013a50: 7475 7265 2073 746f 7265 2e0a 0a20 2020  ture store...   
-00013a60: 2020 2020 2053 7461 7469 7374 6963 7320       Statistics 
-00013a70: 6172 6520 6f6e 6c79 2063 6f6d 7075 7465  are only compute
-00013a80: 6420 666f 7220 6461 7461 2069 6e20 7468  d for data in th
-00013a90: 6520 6f66 666c 696e 6520 7374 6f72 6167  e offline storag
-00013aa0: 6520 6f66 2074 6865 2066 6561 7475 7265  e of the feature
-00013ab0: 0a20 2020 2020 2020 2067 726f 7570 2e0a  .        group..
-00013ac0: 0a20 2020 2020 2020 2023 2041 7267 756d  .        # Argum
-00013ad0: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
-00013ae0: 2077 616c 6c63 6c6f 636b 5f74 696d 653a   wallclock_time:
-00013af0: 2049 6620 7370 6563 6966 6965 6420 7769   If specified wi
-00013b00: 6c6c 2072 6563 6f6d 7075 7465 2073 7461  ll recompute sta
-00013b10: 7469 7374 6963 7320 6f6e 0a20 2020 2020  tistics on.     
-00013b20: 2020 2020 2020 2020 2020 2066 6561 7475             featu
-00013b30: 7265 2067 726f 7570 2061 7320 6f66 2073  re group as of s
-00013b40: 7065 6369 6669 6320 706f 696e 7420 696e  pecific point in
-00013b50: 2074 696d 652e 2049 6620 6e6f 7420 7370   time. If not sp
-00013b60: 6563 6966 6965 6420 7468 656e 2077 696c  ecified then wil
-00013b70: 6c20 636f 6d70 7574 6520 7374 6174 6973  l compute statis
-00013b80: 7469 6373 0a20 2020 2020 2020 2020 2020  tics.           
-00013b90: 2020 2020 2061 7320 6f66 206d 6f73 7420       as of most 
-00013ba0: 7265 6365 6e74 2074 696d 6520 6f66 2074  recent time of t
-00013bb0: 6869 7320 6665 6174 7572 6520 6772 6f75  his feature grou
-00013bc0: 702e 2044 6566 6175 6c74 7320 746f 2060  p. Defaults to `
-00013bd0: 4e6f 6e65 602e 2053 7472 696e 6773 2073  None`. Strings s
-00013be0: 686f 756c 640a 2020 2020 2020 2020 2020  hould.          
-00013bf0: 2020 2020 2020 6265 2066 6f72 6d61 7474        be formatt
-00013c00: 6564 2069 6e20 6f6e 6520 6f66 2074 6865  ed in one of the
-00013c10: 2066 6f6c 6c6f 7769 6e67 2066 6f72 6d61   following forma
-00013c20: 7473 2060 2559 2d25 6d2d 2564 602c 2060  ts `%Y-%m-%d`, `
-00013c30: 2559 2d25 6d2d 2564 2025 4860 2c20 6025  %Y-%m-%d %H`, `%
-00013c40: 592d 256d 2d25 6420 2548 3a25 4d60 2c20  Y-%m-%d %H:%M`, 
-00013c50: 6025 592d 256d 2d25 6420 2548 3a25 4d3a  `%Y-%m-%d %H:%M:
-00013c60: 2553 602c 0a20 2020 2020 2020 2020 2020  %S`,.           
-00013c70: 2020 2020 206f 7220 6025 592d 256d 2d25       or `%Y-%m-%
-00013c80: 6420 2548 3a25 4d3a 2553 2e25 6660 2e0a  d %H:%M:%S.%f`..
-00013c90: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
-00013ca0: 6e73 0a20 2020 2020 2020 2020 2020 2060  ns.            `
-00013cb0: 5374 6174 6973 7469 6373 602e 2054 6865  Statistics`. The
-00013cc0: 2073 7461 7469 7374 6963 7320 6d65 7461   statistics meta
-00013cd0: 6461 7461 206f 626a 6563 742e 0a0a 2020  data object...  
-00013ce0: 2020 2020 2020 2320 5261 6973 6573 0a20        # Raises. 
-00013cf0: 2020 2020 2020 2020 2020 2060 6873 6673             `hsfs
-00013d00: 2e63 6c69 656e 742e 6578 6365 7074 696f  .client.exceptio
-00013d10: 6e73 2e52 6573 7441 5049 4572 726f 7260  ns.RestAPIError`
-00013d20: 2e20 556e 6162 6c65 2074 6f20 7065 7273  . Unable to pers
-00013d30: 6973 7420 7468 6520 7374 6174 6973 7469  ist the statisti
-00013d40: 6373 2e0a 2020 2020 2020 2020 2222 220a  cs..        """.
-00013d50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00013d60: 7374 6174 6973 7469 6373 5f63 6f6e 6669  statistics_confi
-00013d70: 672e 656e 6162 6c65 643a 0a20 2020 2020  g.enabled:.     
-00013d80: 2020 2020 2020 2023 2044 6f6e 2774 2072         # Don't r
-00013d90: 6561 6420 7468 6520 6461 7461 6672 616d  ead the datafram
-00013da0: 6520 6865 7265 2c20 746f 2061 766f 6964  e here, to avoid
-00013db0: 2074 7269 6767 6572 696e 6720 6120 7265   triggering a re
-00013dc0: 6164 206f 7065 7261 7469 6f6e 0a20 2020  ad operation.   
-00013dd0: 2020 2020 2020 2020 2023 2066 6f72 2074           # for t
-00013de0: 6865 2050 7974 686f 6e20 656e 6769 6e65  he Python engine
-00013df0: 2e20 5468 6520 5079 7468 6f6e 2065 6e67  . The Python eng
-00013e00: 696e 6520 6973 2067 6f69 6e67 2074 6f20  ine is going to 
-00013e10: 7365 7475 7020 6120 5370 6172 6b20 4a6f  setup a Spark Jo
-00013e20: 620a 2020 2020 2020 2020 2020 2020 2320  b.            # 
-00013e30: 746f 2075 7064 6174 6520 7468 6520 7374  to update the st
-00013e40: 6174 6973 7469 6373 2e0a 0a20 2020 2020  atistics...     
-00013e50: 2020 2020 2020 2066 675f 636f 6d6d 6974         fg_commit
-00013e60: 5f69 6420 3d20 4e6f 6e65 0a20 2020 2020  _id = None.     
-00013e70: 2020 2020 2020 2069 6620 7761 6c6c 636c         if wallcl
-00013e80: 6f63 6b5f 7469 6d65 2069 7320 6e6f 7420  ock_time is not 
-00013e90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00013ea0: 2020 2020 2020 2320 5265 7472 6965 7665        # Retrieve
-00013eb0: 2066 6720 636f 6d6d 6974 2069 6420 7265   fg commit id re
-00013ec0: 6c61 7465 6420 746f 2074 6869 7320 7761  lated to this wa
-00013ed0: 6c6c 2063 6c6f 636b 2074 696d 6520 616e  ll clock time an
-00013ee0: 6420 7265 636f 6d70 7574 6520 7374 6174  d recompute stat
-00013ef0: 6973 7469 6373 2e20 4974 2077 696c 6c20  istics. It will 
-00013f00: 7468 726f 770a 2020 2020 2020 2020 2020  throw.          
-00013f10: 2020 2020 2020 2320 6578 6365 7074 696f        # exceptio
-00013f20: 6e20 6966 2069 7473 206e 6f74 2074 696d  n if its not tim
-00013f30: 6520 7472 6176 656c 2065 6e61 626c 6564  e travel enabled
-00013f40: 2066 6561 7475 7265 2067 726f 7570 2e0a   feature group..
-00013f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f60: 6667 5f63 6f6d 6d69 745f 6964 203d 205b  fg_commit_id = [
-00013f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013f80: 2020 2020 2063 6f6d 6d69 745f 6964 0a20       commit_id. 
-00013f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fa0: 2020 2066 6f72 2063 6f6d 6d69 745f 6964     for commit_id
-00013fb0: 2069 6e20 7365 6c66 2e5f 6665 6174 7572   in self._featur
-00013fc0: 655f 6772 6f75 705f 656e 6769 6e65 2e63  e_group_engine.c
-00013fd0: 6f6d 6d69 745f 6465 7461 696c 7328 0a20  ommit_details(. 
-00013fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ff0: 2020 2020 2020 2073 656c 662c 2077 616c         self, wal
-00014000: 6c63 6c6f 636b 5f74 696d 652c 2031 0a20  lclock_time, 1. 
-00014010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014020: 2020 2029 2e6b 6579 7328 290a 2020 2020     ).keys().    
-00014030: 2020 2020 2020 2020 2020 2020 5d5b 305d              ][0]
-00014040: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00014050: 7475 726e 2073 656c 662e 5f73 7461 7469  turn self._stati
-00014060: 7374 6963 735f 656e 6769 6e65 2e63 6f6d  stics_engine.com
-00014070: 7075 7465 5f73 7461 7469 7374 6963 7328  pute_statistics(
-00014080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014090: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-000140a0: 2020 2020 2020 2066 6561 7475 7265 5f67         feature_g
-000140b0: 726f 7570 5f63 6f6d 6d69 745f 6964 3d66  roup_commit_id=f
-000140c0: 675f 636f 6d6d 6974 5f69 640a 2020 2020  g_commit_id.    
-000140d0: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-000140e0: 675f 636f 6d6d 6974 5f69 6420 6973 206e  g_commit_id is n
-000140f0: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
-00014100: 2020 2020 2020 2020 656c 7365 204e 6f6e          else Non
-00014110: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
-00014120: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00014130: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
-00014140: 6e67 732e 7761 726e 280a 2020 2020 2020  ngs.warn(.      
-00014150: 2020 2020 2020 2020 2020 280a 2020 2020            (.    
-00014160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014170: 2254 6865 2073 7461 7469 7374 6963 7320  "The statistics 
-00014180: 6172 6520 6e6f 7420 656e 6162 6c65 6420  are not enabled 
-00014190: 6f66 2066 6561 7475 7265 2067 726f 7570  of feature group
-000141a0: 2060 7b7d 602c 2077 6974 6820 7665 7273   `{}`, with vers
-000141b0: 696f 6e22 0a20 2020 2020 2020 2020 2020  ion".           
-000141c0: 2020 2020 2020 2020 2022 2060 7b7d 602e           " `{}`.
-000141d0: 204e 6f20 7374 6174 6973 7469 6373 2063   No statistics c
-000141e0: 6f6d 7075 7465 642e 220a 2020 2020 2020  omputed.".      
-000141f0: 2020 2020 2020 2020 2020 292e 666f 726d            ).form
-00014200: 6174 2873 656c 662e 5f6e 616d 652c 2073  at(self._name, s
-00014210: 656c 662e 5f76 6572 7369 6f6e 292c 0a20  elf._version),. 
-00014220: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00014230: 7469 6c2e 5374 6f72 6167 6557 6172 6e69  til.StorageWarni
-00014240: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
-00014250: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
-00014260: 686f 640a 2020 2020 6465 6620 6672 6f6d  hod.    def from
-00014270: 5f72 6573 706f 6e73 655f 6a73 6f6e 2863  _response_json(c
-00014280: 6c73 2c20 6a73 6f6e 5f64 6963 7429 3a0a  ls, json_dict):.
-00014290: 2020 2020 2020 2020 6a73 6f6e 5f64 6563          json_dec
-000142a0: 616d 656c 697a 6564 203d 2068 756d 7073  amelized = humps
-000142b0: 2e64 6563 616d 656c 697a 6528 6a73 6f6e  .decamelize(json
-000142c0: 5f64 6963 7429 0a20 2020 2020 2020 2069  _dict).        i
-000142d0: 6620 6973 696e 7374 616e 6365 286a 736f  f isinstance(jso
-000142e0: 6e5f 6465 6361 6d65 6c69 7a65 642c 2064  n_decamelized, d
-000142f0: 6963 7429 3a0a 2020 2020 2020 2020 2020  ict):.          
-00014300: 2020 6966 2022 7479 7065 2220 696e 206a    if "type" in j
-00014310: 736f 6e5f 6465 6361 6d65 6c69 7a65 643a  son_decamelized:
-00014320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014330: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
-00014340: 645b 2273 7472 6561 6d22 5d20 3d20 280a  d["stream"] = (.
-00014350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014360: 2020 2020 6a73 6f6e 5f64 6563 616d 656c      json_decamel
-00014370: 697a 6564 5b22 7479 7065 225d 203d 3d20  ized["type"] == 
-00014380: 2273 7472 6561 6d46 6561 7475 7265 4772  "streamFeatureGr
-00014390: 6f75 7044 544f 220a 2020 2020 2020 2020  oupDTO".        
-000143a0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000143b0: 2020 2020 2020 5f20 3d20 6a73 6f6e 5f64        _ = json_d
-000143c0: 6563 616d 656c 697a 6564 2e70 6f70 2822  ecamelized.pop("
-000143d0: 7479 7065 222c 204e 6f6e 6529 0a20 2020  type", None).   
-000143e0: 2020 2020 2020 2020 206a 736f 6e5f 6465           json_de
-000143f0: 6361 6d65 6c69 7a65 642e 706f 7028 2276  camelized.pop("v
-00014400: 616c 6964 6174 696f 6e5f 7479 7065 222c  alidation_type",
-00014410: 204e 6f6e 6529 0a20 2020 2020 2020 2020   None).         
-00014420: 2020 2072 6574 7572 6e20 636c 7328 2a2a     return cls(**
-00014430: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
-00014440: 290a 2020 2020 2020 2020 666f 7220 6667  ).        for fg
-00014450: 2069 6e20 6a73 6f6e 5f64 6563 616d 656c   in json_decamel
-00014460: 697a 6564 3a0a 2020 2020 2020 2020 2020  ized:.          
-00014470: 2020 6966 2022 7479 7065 2220 696e 2066    if "type" in f
-00014480: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
-00014490: 2020 2066 675b 2273 7472 6561 6d22 5d20     fg["stream"] 
-000144a0: 3d20 6667 5b22 7479 7065 225d 203d 3d20  = fg["type"] == 
-000144b0: 2273 7472 6561 6d46 6561 7475 7265 4772  "streamFeatureGr
-000144c0: 6f75 7044 544f 220a 2020 2020 2020 2020  oupDTO".        
-000144d0: 2020 2020 5f20 3d20 6667 2e70 6f70 2822      _ = fg.pop("
-000144e0: 7479 7065 222c 204e 6f6e 6529 0a20 2020  type", None).   
-000144f0: 2020 2020 2020 2020 2066 672e 706f 7028           fg.pop(
-00014500: 2276 616c 6964 6174 696f 6e5f 7479 7065  "validation_type
-00014510: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
-00014520: 2072 6574 7572 6e20 5b63 6c73 282a 2a66   return [cls(**f
-00014530: 6729 2066 6f72 2066 6720 696e 206a 736f  g) for fg in jso
-00014540: 6e5f 6465 6361 6d65 6c69 7a65 645d 0a0a  n_decamelized]..
-00014550: 2020 2020 6465 6620 7570 6461 7465 5f66      def update_f
-00014560: 726f 6d5f 7265 7370 6f6e 7365 5f6a 736f  rom_response_jso
-00014570: 6e28 7365 6c66 2c20 6a73 6f6e 5f64 6963  n(self, json_dic
-00014580: 7429 3a0a 2020 2020 2020 2020 6a73 6f6e  t):.        json
-00014590: 5f64 6563 616d 656c 697a 6564 203d 2068  _decamelized = h
-000145a0: 756d 7073 2e64 6563 616d 656c 697a 6528  umps.decamelize(
-000145b0: 6a73 6f6e 5f64 6963 7429 0a20 2020 2020  json_dict).     
-000145c0: 2020 206a 736f 6e5f 6465 6361 6d65 6c69     json_decameli
-000145d0: 7a65 645b 2273 7472 6561 6d22 5d20 3d20  zed["stream"] = 
-000145e0: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
-000145f0: 5b22 7479 7065 225d 203d 3d20 2273 7472  ["type"] == "str
-00014600: 6561 6d46 6561 7475 7265 4772 6f75 7044  eamFeatureGroupD
-00014610: 544f 220a 2020 2020 2020 2020 5f20 3d20  TO".        _ = 
-00014620: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
-00014630: 2e70 6f70 2822 7479 7065 2229 0a20 2020  .pop("type").   
-00014640: 2020 2020 2073 656c 662e 5f5f 696e 6974       self.__init
-00014650: 5f5f 282a 2a6a 736f 6e5f 6465 6361 6d65  __(**json_decame
-00014660: 6c69 7a65 6429 0a20 2020 2020 2020 2072  lized).        r
-00014670: 6574 7572 6e20 7365 6c66 0a0a 2020 2020  eturn self..    
-00014680: 6465 6620 6a73 6f6e 2873 656c 6629 3a0a  def json(self):.
-00014690: 2020 2020 2020 2020 2222 2247 6574 2073          """Get s
-000146a0: 7065 6369 6669 6320 4665 6174 7572 6520  pecific Feature 
-000146b0: 4772 6f75 7020 6d65 7461 6461 7461 2069  Group metadata i
-000146c0: 6e20 6a73 6f6e 2066 6f72 6d61 742e 0a0a  n json format...
-000146d0: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
-000146e0: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
-000146f0: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-00014700: 2020 2020 2020 6667 2e6a 736f 6e28 290a        fg.json().
-00014710: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
-00014720: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00014730: 2020 2020 7265 7475 726e 206a 736f 6e2e      return json.
-00014740: 6475 6d70 7328 7365 6c66 2c20 636c 733d  dumps(self, cls=
-00014750: 7574 696c 2e46 6561 7475 7265 5374 6f72  util.FeatureStor
-00014760: 6545 6e63 6f64 6572 290a 0a20 2020 2064  eEncoder)..    d
-00014770: 6566 2074 6f5f 6469 6374 2873 656c 6629  ef to_dict(self)
-00014780: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
-00014790: 2073 7472 7563 7475 7265 6420 696e 666f   structured info
-000147a0: 2061 626f 7574 2073 7065 6369 6669 6320   about specific 
-000147b0: 4665 6174 7572 6520 4772 6f75 7020 696e  Feature Group in
-000147c0: 2070 7974 686f 6e20 6469 6374 696f 6e61   python dictiona
-000147d0: 7279 2066 6f72 6d61 742e 0a0a 2020 2020  ry format...    
-000147e0: 2020 2020 2121 2120 6578 616d 706c 650a      !!! example.
-000147f0: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
-00014800: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
-00014810: 2020 2320 636f 6e6e 6563 7420 746f 2074    # connect to t
-00014820: 6865 2046 6561 7475 7265 2053 746f 7265  he Feature Store
-00014830: 0a20 2020 2020 2020 2020 2020 2066 7320  .            fs 
-00014840: 3d20 2e2e 2e0a 0a20 2020 2020 2020 2020  = .....         
-00014850: 2020 2023 2067 6574 2074 6865 2046 6561     # get the Fea
-00014860: 7475 7265 2047 726f 7570 2069 6e73 7461  ture Group insta
-00014870: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
-00014880: 6667 203d 2066 732e 6765 745f 6f72 5f63  fg = fs.get_or_c
-00014890: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
-000148a0: 6f75 7028 2e2e 2e29 0a0a 2020 2020 2020  oup(...)..      
-000148b0: 2020 2020 2020 6667 2e74 6f5f 6469 6374        fg.to_dict
-000148c0: 2829 0a20 2020 2020 2020 2020 2020 2060  ().            `
-000148d0: 6060 0a20 2020 2020 2020 2022 2222 0a20  ``.        """. 
-000148e0: 2020 2020 2020 2066 675f 6d65 7461 5f64         fg_meta_d
-000148f0: 6963 7420 3d20 7b0a 2020 2020 2020 2020  ict = {.        
-00014900: 2020 2020 2269 6422 3a20 7365 6c66 2e5f      "id": self._
-00014910: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00014920: 226e 616d 6522 3a20 7365 6c66 2e5f 6e61  "name": self._na
-00014930: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-00014940: 2276 6572 7369 6f6e 223a 2073 656c 662e  "version": self.
-00014950: 5f76 6572 7369 6f6e 2c0a 2020 2020 2020  _version,.      
-00014960: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00014970: 6f6e 223a 2073 656c 662e 5f64 6573 6372  on": self._descr
-00014980: 6970 7469 6f6e 2c0a 2020 2020 2020 2020  iption,.        
-00014990: 2020 2020 226f 6e6c 696e 6545 6e61 626c      "onlineEnabl
-000149a0: 6564 223a 2073 656c 662e 5f6f 6e6c 696e  ed": self._onlin
-000149b0: 655f 656e 6162 6c65 642c 0a20 2020 2020  e_enabled,.     
-000149c0: 2020 2020 2020 2022 7469 6d65 5472 6176         "timeTrav
-000149d0: 656c 466f 726d 6174 223a 2073 656c 662e  elFormat": self.
-000149e0: 5f74 696d 655f 7472 6176 656c 5f66 6f72  _time_travel_for
-000149f0: 6d61 742c 0a20 2020 2020 2020 2020 2020  mat,.           
-00014a00: 2022 6665 6174 7572 6573 223a 2073 656c   "features": sel
-00014a10: 662e 5f66 6561 7475 7265 732c 0a20 2020  f._features,.   
-00014a20: 2020 2020 2020 2020 2022 6665 6174 7572           "featur
-00014a30: 6573 746f 7265 4964 223a 2073 656c 662e  estoreId": self.
-00014a40: 5f66 6561 7475 7265 5f73 746f 7265 5f69  _feature_store_i
-00014a50: 642c 0a20 2020 2020 2020 2020 2020 2022  d,.            "
-00014a60: 7479 7065 223a 2022 6361 6368 6564 4665  type": "cachedFe
-00014a70: 6174 7572 6567 726f 7570 4454 4f22 0a20  aturegroupDTO". 
-00014a80: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00014a90: 7420 7365 6c66 2e5f 7374 7265 616d 0a20  t self._stream. 
-00014aa0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-00014ab0: 2273 7472 6561 6d46 6561 7475 7265 4772  "streamFeatureGr
-00014ac0: 6f75 7044 544f 222c 0a20 2020 2020 2020  oupDTO",.       
-00014ad0: 2020 2020 2022 7374 6174 6973 7469 6373       "statistics
-00014ae0: 436f 6e66 6967 223a 2073 656c 662e 5f73  Config": self._s
-00014af0: 7461 7469 7374 6963 735f 636f 6e66 6967  tatistics_config
-00014b00: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
-00014b10: 7665 6e74 5469 6d65 223a 2073 656c 662e  ventTime": self.
-00014b20: 6576 656e 745f 7469 6d65 2c0a 2020 2020  event_time,.    
-00014b30: 2020 2020 2020 2020 2265 7870 6563 7461          "expecta
-00014b40: 7469 6f6e 5375 6974 6522 3a20 7365 6c66  tionSuite": self
-00014b50: 2e5f 6578 7065 6374 6174 696f 6e5f 7375  ._expectation_su
-00014b60: 6974 652c 0a20 2020 2020 2020 2020 2020  ite,.           
-00014b70: 2022 7061 7265 6e74 7322 3a20 7365 6c66   "parents": self
-00014b80: 2e5f 7061 7265 6e74 732c 0a20 2020 2020  ._parents,.     
-00014b90: 2020 207d 0a20 2020 2020 2020 2069 6620     }.        if 
-00014ba0: 7365 6c66 2e5f 7374 7265 616d 3a0a 2020  self._stream:.  
-00014bb0: 2020 2020 2020 2020 2020 6667 5f6d 6574            fg_met
-00014bc0: 615f 6469 6374 5b22 6465 6c74 6153 7472  a_dict["deltaStr
-00014bd0: 6561 6d65 724a 6f62 436f 6e66 225d 203d  eamerJobConf"] =
-00014be0: 2073 656c 662e 5f64 656c 7461 7374 7265   self._deltastre
-00014bf0: 616d 6572 5f6a 6f62 636f 6e66 0a20 2020  amer_jobconf.   
-00014c00: 2020 2020 2072 6574 7572 6e20 6667 5f6d       return fg_m
-00014c10: 6574 615f 6469 6374 0a0a 2020 2020 6465  eta_dict..    de
-00014c20: 6620 5f67 6574 5f74 6162 6c65 5f6e 616d  f _get_table_nam
-00014c30: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00014c40: 2072 6574 7572 6e20 7365 6c66 2e66 6561   return self.fea
-00014c50: 7475 7265 5f73 746f 7265 5f6e 616d 6520  ture_store_name 
-00014c60: 2b20 222e 2220 2b20 7365 6c66 2e6e 616d  + "." + self.nam
-00014c70: 6520 2b20 225f 2220 2b20 7374 7228 7365  e + "_" + str(se
-00014c80: 6c66 2e76 6572 7369 6f6e 290a 0a20 2020  lf.version)..   
-00014c90: 2064 6566 205f 6765 745f 6f6e 6c69 6e65   def _get_online
-00014ca0: 5f74 6162 6c65 5f6e 616d 6528 7365 6c66  _table_name(self
-00014cb0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00014cc0: 6e20 7365 6c66 2e6e 616d 6520 2b20 225f  n self.name + "_
-00014cd0: 2220 2b20 7374 7228 7365 6c66 2e76 6572  " + str(self.ver
-00014ce0: 7369 6f6e 290a 0a20 2020 2064 6566 2067  sion)..    def g
-00014cf0: 6574 5f63 6f6d 706c 6578 5f66 6561 7475  et_complex_featu
-00014d00: 7265 7328 7365 6c66 293a 0a20 2020 2020  res(self):.     
-00014d10: 2020 2022 2222 5265 7475 726e 7320 7468     """Returns th
-00014d20: 6520 6e61 6d65 7320 6f66 2061 6c6c 2066  e names of all f
-00014d30: 6561 7475 7265 7320 7769 7468 2061 2063  eatures with a c
-00014d40: 6f6d 706c 6578 2064 6174 6120 7479 7065  omplex data type
-00014d50: 2069 6e20 7468 6973 0a20 2020 2020 2020   in this.       
-00014d60: 2066 6561 7475 7265 2067 726f 7570 2e0a   feature group..
-00014d70: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
-00014d80: 6d70 6c65 0a20 2020 2020 2020 2020 2020  mple.           
-00014d90: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
-00014da0: 2020 2020 2020 2063 6f6d 706c 6578 5f64         complex_d
-00014db0: 7479 7065 5f66 6561 7475 7265 7320 3d20  type_features = 
-00014dc0: 6667 2e67 6574 5f63 6f6d 706c 6578 5f66  fg.get_complex_f
-00014dd0: 6561 7475 7265 7328 290a 2020 2020 2020  eatures().      
-00014de0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-00014df0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-00014e00: 7475 726e 205b 662e 6e61 6d65 2066 6f72  turn [f.name for
-00014e10: 2066 2069 6e20 7365 6c66 2e66 6561 7475   f in self.featu
-00014e20: 7265 7320 6966 2066 2e69 735f 636f 6d70  res if f.is_comp
-00014e30: 6c65 7828 295d 0a0a 2020 2020 6465 6620  lex()]..    def 
-00014e40: 5f67 6574 5f65 6e63 6f64 6564 5f61 7672  _get_encoded_avr
-00014e50: 6f5f 7363 6865 6d61 2873 656c 6629 3a0a  o_schema(self):.
-00014e60: 2020 2020 2020 2020 636f 6d70 6c65 785f          complex_
-00014e70: 6665 6174 7572 6573 203d 2073 656c 662e  features = self.
-00014e80: 6765 745f 636f 6d70 6c65 785f 6665 6174  get_complex_feat
-00014e90: 7572 6573 2829 0a20 2020 2020 2020 2073  ures().        s
-00014ea0: 6368 656d 6120 3d20 6a73 6f6e 2e6c 6f61  chema = json.loa
-00014eb0: 6473 2873 656c 662e 6176 726f 5f73 6368  ds(self.avro_sch
-00014ec0: 656d 6129 0a0a 2020 2020 2020 2020 666f  ema)..        fo
-00014ed0: 7220 6669 656c 6420 696e 2073 6368 656d  r field in schem
-00014ee0: 615b 2266 6965 6c64 7322 5d3a 0a20 2020  a["fields"]:.   
-00014ef0: 2020 2020 2020 2020 2069 6620 6669 656c           if fiel
-00014f00: 645b 226e 616d 6522 5d20 696e 2063 6f6d  d["name"] in com
-00014f10: 706c 6578 5f66 6561 7475 7265 733a 0a20  plex_features:. 
-00014f20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00014f30: 6965 6c64 5b22 7479 7065 225d 203d 205b  ield["type"] = [
-00014f40: 226e 756c 6c22 2c20 2262 7974 6573 225d  "null", "bytes"]
-00014f50: 0a0a 2020 2020 2020 2020 7363 6865 6d61  ..        schema
-00014f60: 5f73 203d 206a 736f 6e2e 6475 6d70 7328  _s = json.dumps(
-00014f70: 7363 6865 6d61 290a 2020 2020 2020 2020  schema).        
-00014f80: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00014f90: 2061 7672 6f2e 7363 6865 6d61 2e70 6172   avro.schema.par
-00014fa0: 7365 2873 6368 656d 615f 7329 0a20 2020  se(schema_s).   
-00014fb0: 2020 2020 2065 7863 6570 7420 6176 726f       except avro
-00014fc0: 2e73 6368 656d 612e 5363 6865 6d61 5061  .schema.SchemaPa
-00014fd0: 7273 6545 7863 6570 7469 6f6e 2061 7320  rseException as 
-00014fe0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00014ff0: 6169 7365 2046 6561 7475 7265 5374 6f72  aise FeatureStor
-00015000: 6545 7863 6570 7469 6f6e 2822 4661 696c  eException("Fail
-00015010: 6564 2074 6f20 636f 6e73 7472 7563 7420  ed to construct 
-00015020: 4176 726f 2053 6368 656d 613a 207b 7d22  Avro Schema: {}"
-00015030: 2e66 6f72 6d61 7428 6529 290a 2020 2020  .format(e)).    
-00015040: 2020 2020 7265 7475 726e 2073 6368 656d      return schem
-00015050: 615f 730a 0a20 2020 2064 6566 205f 6765  a_s..    def _ge
-00015060: 745f 6665 6174 7572 655f 6176 726f 5f73  t_feature_avro_s
-00015070: 6368 656d 6128 7365 6c66 2c20 6665 6174  chema(self, feat
-00015080: 7572 655f 6e61 6d65 293a 0a20 2020 2020  ure_name):.     
-00015090: 2020 2066 6f72 2066 6965 6c64 2069 6e20     for field in 
-000150a0: 6a73 6f6e 2e6c 6f61 6473 2873 656c 662e  json.loads(self.
-000150b0: 6176 726f 5f73 6368 656d 6129 5b22 6669  avro_schema)["fi
-000150c0: 656c 6473 225d 3a0a 2020 2020 2020 2020  elds"]:.        
-000150d0: 2020 2020 6966 2066 6965 6c64 5b22 6e61      if field["na
-000150e0: 6d65 225d 203d 3d20 6665 6174 7572 655f  me"] == feature_
-000150f0: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
-00015100: 2020 2020 2020 7265 7475 726e 206a 736f        return jso
-00015110: 6e2e 6475 6d70 7328 6669 656c 645b 2274  n.dumps(field["t
-00015120: 7970 6522 5d29 0a0a 2020 2020 4070 726f  ype"])..    @pro
-00015130: 7065 7274 790a 2020 2020 6465 6620 6964  perty.    def id
-00015140: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00015150: 2222 2246 6561 7475 7265 2067 726f 7570  """Feature group
-00015160: 2069 642e 2222 220a 2020 2020 2020 2020   id.""".        
-00015170: 7265 7475 726e 2073 656c 662e 5f69 640a  return self._id.
-00015180: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00015190: 2020 2064 6566 206e 616d 6528 7365 6c66     def name(self
-000151a0: 293a 0a20 2020 2020 2020 2022 2222 4e61  ):.        """Na
-000151b0: 6d65 206f 6620 7468 6520 6665 6174 7572  me of the featur
-000151c0: 6520 6772 6f75 702e 2222 220a 2020 2020  e group.""".    
-000151d0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000151e0: 5f6e 616d 650a 0a20 2020 2040 7072 6f70  _name..    @prop
-000151f0: 6572 7479 0a20 2020 2064 6566 2076 6572  erty.    def ver
-00015200: 7369 6f6e 2873 656c 6629 3a0a 2020 2020  sion(self):.    
-00015210: 2020 2020 2222 2256 6572 7369 6f6e 206e      """Version n
-00015220: 756d 6265 7220 6f66 2074 6865 2066 6561  umber of the fea
-00015230: 7475 7265 2067 726f 7570 2e22 2222 0a20  ture group.""". 
-00015240: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00015250: 6c66 2e5f 7665 7273 696f 6e0a 0a20 2020  lf._version..   
-00015260: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00015270: 6566 2064 6573 6372 6970 7469 6f6e 2873  ef description(s
-00015280: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00015290: 2244 6573 6372 6970 7469 6f6e 206f 6620  "Description of 
-000152a0: 7468 6520 6665 6174 7572 6520 6772 6f75  the feature grou
-000152b0: 7020 636f 6e74 656e 7473 2e22 2222 0a20  p contents.""". 
-000152c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000152d0: 6c66 2e5f 6465 7363 7269 7074 696f 6e0a  lf._description.
-000152e0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-000152f0: 2020 2064 6566 2066 6561 7475 7265 7328     def features(
-00015300: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00015310: 2222 5363 6865 6d61 2069 6e66 6f72 6d61  ""Schema informa
-00015320: 7469 6f6e 2e22 2222 0a20 2020 2020 2020  tion.""".       
-00015330: 2072 6574 7572 6e20 7365 6c66 2e5f 6665   return self._fe
-00015340: 6174 7572 6573 0a0a 2020 2020 4070 726f  atures..    @pro
-00015350: 7065 7274 790a 2020 2020 6465 6620 6f6e  perty.    def on
-00015360: 6c69 6e65 5f65 6e61 626c 6564 2873 656c  line_enabled(sel
-00015370: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
-00015380: 6574 7469 6e67 2069 6620 7468 6520 6665  etting if the fe
-00015390: 6174 7572 6520 6772 6f75 7020 6973 2061  ature group is a
-000153a0: 7661 696c 6162 6c65 2069 6e20 6f6e 6c69  vailable in onli
-000153b0: 6e65 2073 746f 7261 6765 2e22 2222 0a20  ne storage.""". 
-000153c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000153d0: 6c66 2e5f 6f6e 6c69 6e65 5f65 6e61 626c  lf._online_enabl
-000153e0: 6564 0a0a 2020 2020 4070 726f 7065 7274  ed..    @propert
-000153f0: 790a 2020 2020 6465 6620 7469 6d65 5f74  y.    def time_t
-00015400: 7261 7665 6c5f 666f 726d 6174 2873 656c  ravel_format(sel
-00015410: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
-00015420: 6574 7469 6e67 206f 6620 7468 6520 6665  etting of the fe
-00015430: 6174 7572 6520 6772 6f75 7020 7469 6d65  ature group time
-00015440: 2074 7261 7665 6c20 666f 726d 6174 2e22   travel format."
-00015450: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00015460: 6e20 7365 6c66 2e5f 7469 6d65 5f74 7261  n self._time_tra
-00015470: 7665 6c5f 666f 726d 6174 0a0a 2020 2020  vel_format..    
-00015480: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00015490: 6620 7061 7274 6974 696f 6e5f 6b65 7928  f partition_key(
-000154a0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000154b0: 2222 4c69 7374 206f 6620 6665 6174 7572  ""List of featur
-000154c0: 6573 2062 7569 6c64 696e 6720 7468 6520  es building the 
-000154d0: 7061 7274 6974 696f 6e20 6b65 792e 2222  partition key.""
-000154e0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-000154f0: 2073 656c 662e 5f70 6172 7469 7469 6f6e   self._partition
-00015500: 5f6b 6579 0a0a 2020 2020 4070 726f 7065  _key..    @prope
-00015510: 7274 790a 2020 2020 6465 6620 6875 6469  rty.    def hudi
-00015520: 5f70 7265 636f 6d62 696e 655f 6b65 7928  _precombine_key(
-00015530: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00015540: 2222 4665 6174 7572 6520 6e61 6d65 2074  ""Feature name t
-00015550: 6861 7420 6973 2074 6865 2068 7564 6920  hat is the hudi 
-00015560: 7072 6563 6f6d 6269 6e65 206b 6579 2e22  precombine key."
-00015570: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00015580: 6e20 7365 6c66 2e5f 6875 6469 5f70 7265  n self._hudi_pre
-00015590: 636f 6d62 696e 655f 6b65 790a 0a20 2020  combine_key..   
-000155a0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-000155b0: 6566 2066 6561 7475 7265 5f73 746f 7265  ef feature_store
-000155c0: 5f69 6428 7365 6c66 293a 0a20 2020 2020  _id(self):.     
-000155d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000155e0: 6665 6174 7572 655f 7374 6f72 655f 6964  feature_store_id
-000155f0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00015600: 2020 2020 6465 6620 6665 6174 7572 655f      def feature_
-00015610: 7374 6f72 655f 6e61 6d65 2873 656c 6629  store_name(self)
-00015620: 3a0a 2020 2020 2020 2020 2222 224e 616d  :.        """Nam
-00015630: 6520 6f66 2074 6865 2066 6561 7475 7265  e of the feature
-00015640: 2073 746f 7265 2069 6e20 7768 6963 6820   store in which 
-00015650: 7468 6520 6665 6174 7572 6520 6772 6f75  the feature grou
-00015660: 7020 6973 206c 6f63 6174 6564 2e22 2222  p is located."""
-00015670: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00015680: 7365 6c66 2e5f 6665 6174 7572 655f 7374  self._feature_st
-00015690: 6f72 655f 6e61 6d65 0a0a 2020 2020 4070  ore_name..    @p
-000156a0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-000156b0: 6372 6561 746f 7228 7365 6c66 293a 0a20  creator(self):. 
-000156c0: 2020 2020 2020 2022 2222 5573 6572 6e61         """Userna
-000156d0: 6d65 206f 6620 7468 6520 6372 6561 746f  me of the creato
-000156e0: 722e 2222 220a 2020 2020 2020 2020 7265  r.""".        re
-000156f0: 7475 726e 2073 656c 662e 5f63 7265 6174  turn self._creat
-00015700: 6f72 0a0a 2020 2020 4070 726f 7065 7274  or..    @propert
-00015710: 790a 2020 2020 6465 6620 6372 6561 7465  y.    def create
-00015720: 6428 7365 6c66 293a 0a20 2020 2020 2020  d(self):.       
-00015730: 2022 2222 5469 6d65 7374 616d 7020 7768   """Timestamp wh
-00015740: 656e 2074 6865 2066 6561 7475 7265 2067  en the feature g
-00015750: 726f 7570 2077 6173 2063 7265 6174 6564  roup was created
-00015760: 2e22 2222 0a20 2020 2020 2020 2072 6574  .""".        ret
-00015770: 7572 6e20 7365 6c66 2e5f 6372 6561 7465  urn self._create
-00015780: 640a 0a20 2020 2040 7072 6f70 6572 7479  d..    @property
-00015790: 0a20 2020 2064 6566 2073 7562 6a65 6374  .    def subject
-000157a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000157b0: 2222 2253 7562 6a65 6374 206f 6620 7468  """Subject of th
-000157c0: 6520 6665 6174 7572 6520 6772 6f75 702e  e feature group.
-000157d0: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-000157e0: 656c 662e 5f73 7562 6a65 6374 2069 7320  elf._subject is 
-000157f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00015800: 2020 2320 6361 6368 6520 7468 6520 7363    # cache the sc
-00015810: 6865 6d61 0a20 2020 2020 2020 2020 2020  hema.           
-00015820: 2073 656c 662e 5f73 7562 6a65 6374 203d   self._subject =
-00015830: 2073 656c 662e 5f66 6561 7475 7265 5f67   self._feature_g
-00015840: 726f 7570 5f65 6e67 696e 652e 6765 745f  roup_engine.get_
-00015850: 7375 626a 6563 7428 7365 6c66 290a 2020  subject(self).  
-00015860: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00015870: 662e 5f73 7562 6a65 6374 0a0a 2020 2020  f._subject..    
-00015880: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00015890: 6620 6176 726f 5f73 6368 656d 6128 7365  f avro_schema(se
-000158a0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-000158b0: 4176 726f 2073 6368 656d 6120 7265 7072  Avro schema repr
-000158c0: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
-000158d0: 6520 6665 6174 7572 6520 6772 6f75 702e  e feature group.
-000158e0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-000158f0: 726e 2073 656c 662e 7375 626a 6563 745b  rn self.subject[
-00015900: 2273 6368 656d 6122 5d0a 0a20 2020 2040  "schema"]..    @
-00015910: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-00015920: 2073 7472 6561 6d28 7365 6c66 293a 0a20   stream(self):. 
-00015930: 2020 2020 2020 2022 2222 5768 6574 6865         """Whethe
-00015940: 7220 746f 2065 6e61 626c 6520 7265 616c  r to enable real
-00015950: 2074 696d 6520 7374 7265 616d 2077 7269   time stream wri
-00015960: 7469 6e67 2063 6170 6162 696c 6974 6965  ting capabilitie
-00015970: 732e 2222 220a 2020 2020 2020 2020 7265  s.""".        re
-00015980: 7475 726e 2073 656c 662e 5f73 7472 6561  turn self._strea
-00015990: 6d0a 0a20 2020 2040 7072 6f70 6572 7479  m..    @property
-000159a0: 0a20 2020 2064 6566 2070 6172 656e 7473  .    def parents
-000159b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000159c0: 2222 2250 6172 656e 7420 6665 6174 7572  """Parent featur
-000159d0: 6520 6772 6f75 7073 2061 7320 6f72 6967  e groups as orig
-000159e0: 696e 206f 6620 7468 6520 6461 7461 2069  in of the data i
-000159f0: 6e20 7468 6520 6375 7272 656e 7420 6665  n the current fe
-00015a00: 6174 7572 6520 6772 6f75 702e 0a20 2020  ature group..   
-00015a10: 2020 2020 2054 6869 7320 6973 2070 6172       This is par
-00015a20: 7420 6f66 2065 7870 6c69 6369 7420 7072  t of explicit pr
-00015a30: 6f76 656e 616e 6365 2222 220a 2020 2020  ovenance""".    
-00015a40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00015a50: 5f70 6172 656e 7473 0a0a 2020 2020 4076  _parents..    @v
-00015a60: 6572 7369 6f6e 2e73 6574 7465 720a 2020  ersion.setter.  
-00015a70: 2020 6465 6620 7665 7273 696f 6e28 7365    def version(se
-00015a80: 6c66 2c20 7665 7273 696f 6e29 3a0a 2020  lf, version):.  
-00015a90: 2020 2020 2020 7365 6c66 2e5f 7665 7273        self._vers
-00015aa0: 696f 6e20 3d20 7665 7273 696f 6e0a 0a20  ion = version.. 
-00015ab0: 2020 2040 6465 7363 7269 7074 696f 6e2e     @description.
-00015ac0: 7365 7474 6572 0a20 2020 2064 6566 2064  setter.    def d
-00015ad0: 6573 6372 6970 7469 6f6e 2873 656c 662c  escription(self,
-00015ae0: 206e 6577 5f64 6573 6372 6970 7469 6f6e   new_description
-00015af0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00015b00: 5f64 6573 6372 6970 7469 6f6e 203d 206e  _description = n
-00015b10: 6577 5f64 6573 6372 6970 7469 6f6e 0a0a  ew_description..
-00015b20: 2020 2020 4066 6561 7475 7265 732e 7365      @features.se
-00015b30: 7474 6572 0a20 2020 2064 6566 2066 6561  tter.    def fea
-00015b40: 7475 7265 7328 7365 6c66 2c20 6e65 775f  tures(self, new_
-00015b50: 6665 6174 7572 6573 293a 0a20 2020 2020  features):.     
-00015b60: 2020 2073 656c 662e 5f66 6561 7475 7265     self._feature
-00015b70: 7320 3d20 6e65 775f 6665 6174 7572 6573  s = new_features
-00015b80: 0a0a 2020 2020 4074 696d 655f 7472 6176  ..    @time_trav
-00015b90: 656c 5f66 6f72 6d61 742e 7365 7474 6572  el_format.setter
-00015ba0: 0a20 2020 2064 6566 2074 696d 655f 7472  .    def time_tr
-00015bb0: 6176 656c 5f66 6f72 6d61 7428 7365 6c66  avel_format(self
-00015bc0: 2c20 6e65 775f 7469 6d65 5f74 7261 7665  , new_time_trave
-00015bd0: 6c5f 666f 726d 6174 293a 0a20 2020 2020  l_format):.     
-00015be0: 2020 2073 656c 662e 5f74 696d 655f 7472     self._time_tr
-00015bf0: 6176 656c 5f66 6f72 6d61 7420 3d20 6e65  avel_format = ne
-00015c00: 775f 7469 6d65 5f74 7261 7665 6c5f 666f  w_time_travel_fo
-00015c10: 726d 6174 0a0a 2020 2020 4070 6172 7469  rmat..    @parti
-00015c20: 7469 6f6e 5f6b 6579 2e73 6574 7465 720a  tion_key.setter.
-00015c30: 2020 2020 6465 6620 7061 7274 6974 696f      def partitio
-00015c40: 6e5f 6b65 7928 7365 6c66 2c20 6e65 775f  n_key(self, new_
-00015c50: 7061 7274 6974 696f 6e5f 6b65 7929 3a0a  partition_key):.
-00015c60: 2020 2020 2020 2020 7365 6c66 2e5f 7061          self._pa
-00015c70: 7274 6974 696f 6e5f 6b65 7920 3d20 5b70  rtition_key = [p
-00015c80: 6b2e 6c6f 7765 7228 2920 666f 7220 706b  k.lower() for pk
-00015c90: 2069 6e20 6e65 775f 7061 7274 6974 696f   in new_partitio
-00015ca0: 6e5f 6b65 795d 0a0a 2020 2020 4068 7564  n_key]..    @hud
-00015cb0: 695f 7072 6563 6f6d 6269 6e65 5f6b 6579  i_precombine_key
-00015cc0: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00015cd0: 6875 6469 5f70 7265 636f 6d62 696e 655f  hudi_precombine_
-00015ce0: 6b65 7928 7365 6c66 2c20 6875 6469 5f70  key(self, hudi_p
-00015cf0: 7265 636f 6d62 696e 655f 6b65 7929 3a0a  recombine_key):.
-00015d00: 2020 2020 2020 2020 7365 6c66 2e5f 6875          self._hu
-00015d10: 6469 5f70 7265 636f 6d62 696e 655f 6b65  di_precombine_ke
-00015d20: 7920 3d20 6875 6469 5f70 7265 636f 6d62  y = hudi_precomb
-00015d30: 696e 655f 6b65 792e 6c6f 7765 7228 290a  ine_key.lower().
-00015d40: 0a20 2020 2040 6f6e 6c69 6e65 5f65 6e61  .    @online_ena
-00015d50: 626c 6564 2e73 6574 7465 720a 2020 2020  bled.setter.    
-00015d60: 6465 6620 6f6e 6c69 6e65 5f65 6e61 626c  def online_enabl
-00015d70: 6564 2873 656c 662c 206e 6577 5f6f 6e6c  ed(self, new_onl
-00015d80: 696e 655f 656e 6162 6c65 6429 3a0a 2020  ine_enabled):.  
-00015d90: 2020 2020 2020 7365 6c66 2e5f 6f6e 6c69        self._onli
-00015da0: 6e65 5f65 6e61 626c 6564 203d 206e 6577  ne_enabled = new
-00015db0: 5f6f 6e6c 696e 655f 656e 6162 6c65 640a  _online_enabled.
-00015dc0: 0a20 2020 2040 7374 7265 616d 2e73 6574  .    @stream.set
-00015dd0: 7465 720a 2020 2020 6465 6620 7374 7265  ter.    def stre
-00015de0: 616d 2873 656c 662c 2073 7472 6561 6d29  am(self, stream)
-00015df0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00015e00: 7374 7265 616d 203d 2073 7472 6561 6d0a  stream = stream.
-00015e10: 0a20 2020 2040 7061 7265 6e74 732e 7365  .    @parents.se
-00015e20: 7474 6572 0a20 2020 2064 6566 2070 6172  tter.    def par
-00015e30: 656e 7473 2873 656c 662c 206e 6577 5f70  ents(self, new_p
-00015e40: 6172 656e 7473 293a 0a20 2020 2020 2020  arents):.       
-00015e50: 2073 656c 662e 5f70 6172 656e 7473 203d   self._parents =
-00015e60: 206e 6577 5f70 6172 656e 7473 0a0a 0a63   new_parents...c
-00015e70: 6c61 7373 2045 7874 6572 6e61 6c46 6561  lass ExternalFea
-00015e80: 7475 7265 4772 6f75 7028 4665 6174 7572  tureGroup(Featur
-00015e90: 6547 726f 7570 4261 7365 293a 0a20 2020  eGroupBase):.   
-00015ea0: 2045 5854 4552 4e41 4c5f 4645 4154 5552   EXTERNAL_FEATUR
-00015eb0: 455f 4752 4f55 5020 3d20 224f 4e5f 4445  E_GROUP = "ON_DE
-00015ec0: 4d41 4e44 5f46 4541 5455 5245 5f47 524f  MAND_FEATURE_GRO
-00015ed0: 5550 220a 2020 2020 454e 5449 5459 5f54  UP".    ENTITY_T
-00015ee0: 5950 4520 3d20 2266 6561 7475 7265 6772  YPE = "featuregr
-00015ef0: 6f75 7073 220a 0a20 2020 2064 6566 205f  oups"..    def _
-00015f00: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00015f10: 2073 656c 662c 0a20 2020 2020 2020 2073   self,.        s
-00015f20: 746f 7261 6765 5f63 6f6e 6e65 6374 6f72  torage_connector
-00015f30: 2c0a 2020 2020 2020 2020 7175 6572 793d  ,.        query=
-00015f40: 4e6f 6e65 2c0a 2020 2020 2020 2020 6461  None,.        da
-00015f50: 7461 5f66 6f72 6d61 743d 4e6f 6e65 2c0a  ta_format=None,.
-00015f60: 2020 2020 2020 2020 7061 7468 3d4e 6f6e          path=Non
-00015f70: 652c 0a20 2020 2020 2020 206f 7074 696f  e,.        optio
-00015f80: 6e73 3d7b 7d2c 0a20 2020 2020 2020 206e  ns={},.        n
-00015f90: 616d 653d 4e6f 6e65 2c0a 2020 2020 2020  ame=None,.      
-00015fa0: 2020 7665 7273 696f 6e3d 4e6f 6e65 2c0a    version=None,.
-00015fb0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00015fc0: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 2020  ion=None,.      
-00015fd0: 2020 7072 696d 6172 795f 6b65 793d 4e6f    primary_key=No
-00015fe0: 6e65 2c0a 2020 2020 2020 2020 6665 6174  ne,.        feat
-00015ff0: 7572 6573 746f 7265 5f69 643d 4e6f 6e65  urestore_id=None
-00016000: 2c0a 2020 2020 2020 2020 6665 6174 7572  ,.        featur
-00016010: 6573 746f 7265 5f6e 616d 653d 4e6f 6e65  estore_name=None
-00016020: 2c0a 2020 2020 2020 2020 6372 6561 7465  ,.        create
-00016030: 643d 4e6f 6e65 2c0a 2020 2020 2020 2020  d=None,.        
-00016040: 6372 6561 746f 723d 4e6f 6e65 2c0a 2020  creator=None,.  
-00016050: 2020 2020 2020 6964 3d4e 6f6e 652c 0a20        id=None,. 
-00016060: 2020 2020 2020 2066 6561 7475 7265 733d         features=
-00016070: 4e6f 6e65 2c0a 2020 2020 2020 2020 6c6f  None,.        lo
-00016080: 6361 7469 6f6e 3d4e 6f6e 652c 0a20 2020  cation=None,.   
-00016090: 2020 2020 2073 7461 7469 7374 6963 735f       statistics_
-000160a0: 636f 6e66 6967 3d4e 6f6e 652c 0a20 2020  config=None,.   
-000160b0: 2020 2020 2065 7665 6e74 5f74 696d 653d       event_time=
-000160c0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6578  None,.        ex
-000160d0: 7065 6374 6174 696f 6e5f 7375 6974 653d  pectation_suite=
-000160e0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6872  None,.        hr
-000160f0: 6566 3d4e 6f6e 652c 0a20 2020 2029 3a0a  ef=None,.    ):.
-00016100: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-00016110: 5f5f 696e 6974 5f5f 2866 6561 7475 7265  __init__(feature
-00016120: 7374 6f72 655f 6964 2c20 6c6f 6361 7469  store_id, locati
-00016130: 6f6e 2c20 6576 656e 745f 7469 6d65 3d65  on, event_time=e
-00016140: 7665 6e74 5f74 696d 6529 0a20 2020 2020  vent_time).     
-00016150: 2020 2073 656c 662e 5f66 6561 7475 7265     self._feature
-00016160: 5f73 746f 7265 5f6e 616d 6520 3d20 6665  _store_name = fe
-00016170: 6174 7572 6573 746f 7265 5f6e 616d 650a  aturestore_name.
-00016180: 2020 2020 2020 2020 7365 6c66 2e5f 6465          self._de
-00016190: 7363 7269 7074 696f 6e20 3d20 6465 7363  scription = desc
-000161a0: 7269 7074 696f 6e0a 2020 2020 2020 2020  ription.        
-000161b0: 7365 6c66 2e5f 6372 6561 7465 6420 3d20  self._created = 
-000161c0: 6372 6561 7465 640a 2020 2020 2020 2020  created.        
-000161d0: 7365 6c66 2e5f 6372 6561 746f 7220 3d20  self._creator = 
-000161e0: 7573 6572 2e55 7365 722e 6672 6f6d 5f72  user.User.from_r
-000161f0: 6573 706f 6e73 655f 6a73 6f6e 2863 7265  esponse_json(cre
-00016200: 6174 6f72 290a 2020 2020 2020 2020 7365  ator).        se
-00016210: 6c66 2e5f 7665 7273 696f 6e20 3d20 7665  lf._version = ve
-00016220: 7273 696f 6e0a 2020 2020 2020 2020 7365  rsion.        se
-00016230: 6c66 2e5f 6e61 6d65 203d 206e 616d 650a  lf._name = name.
-00016240: 2020 2020 2020 2020 7365 6c66 2e5f 7175          self._qu
-00016250: 6572 7920 3d20 7175 6572 790a 2020 2020  ery = query.    
-00016260: 2020 2020 7365 6c66 2e5f 6461 7461 5f66      self._data_f
-00016270: 6f72 6d61 7420 3d20 6461 7461 5f66 6f72  ormat = data_for
-00016280: 6d61 742e 7570 7065 7228 2920 6966 2064  mat.upper() if d
-00016290: 6174 615f 666f 726d 6174 2065 6c73 6520  ata_format else 
-000162a0: 4e6f 6e65 0a20 2020 2020 2020 2073 656c  None.        sel
-000162b0: 662e 5f70 6174 6820 3d20 7061 7468 0a20  f._path = path. 
-000162c0: 2020 2020 2020 2073 656c 662e 5f69 6420         self._id 
-000162d0: 3d20 6964 0a20 2020 2020 2020 2073 656c  = id.        sel
-000162e0: 662e 5f65 7870 6563 7461 7469 6f6e 5f73  f._expectation_s
-000162f0: 7569 7465 203d 2065 7870 6563 7461 7469  uite = expectati
-00016300: 6f6e 5f73 7569 7465 0a0a 2020 2020 2020  on_suite..      
-00016310: 2020 7365 6c66 2e5f 6665 6174 7572 6573    self._features
-00016320: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00016330: 2066 6561 7475 7265 2e46 6561 7475 7265   feature.Feature
-00016340: 2e66 726f 6d5f 7265 7370 6f6e 7365 5f6a  .from_response_j
-00016350: 736f 6e28 6665 6174 2920 6966 2069 7369  son(feat) if isi
-00016360: 6e73 7461 6e63 6528 6665 6174 2c20 6469  nstance(feat, di
-00016370: 6374 2920 656c 7365 2066 6561 740a 2020  ct) else feat.  
-00016380: 2020 2020 2020 2020 2020 666f 7220 6665            for fe
-00016390: 6174 2069 6e20 2866 6561 7475 7265 7320  at in (features 
-000163a0: 6f72 205b 5d29 0a20 2020 2020 2020 205d  or []).        ]
-000163b0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-000163c0: 6665 6174 7572 655f 6772 6f75 705f 656e  feature_group_en
-000163d0: 6769 6e65 203d 2028 0a20 2020 2020 2020  gine = (.       
-000163e0: 2020 2020 2065 7874 6572 6e61 6c5f 6665       external_fe
-000163f0: 6174 7572 655f 6772 6f75 705f 656e 6769  ature_group_engi
-00016400: 6e65 2e45 7874 6572 6e61 6c46 6561 7475  ne.ExternalFeatu
-00016410: 7265 4772 6f75 7045 6e67 696e 6528 6665  reGroupEngine(fe
-00016420: 6174 7572 6573 746f 7265 5f69 6429 0a20  aturestore_id). 
-00016430: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00016440: 2020 6966 2073 656c 662e 5f69 643a 0a20    if self._id:. 
-00016450: 2020 2020 2020 2020 2020 2023 2047 6f74             # Got
-00016460: 2066 726f 6d20 486f 7073 776f 726b 732c   from Hopsworks,
-00016470: 2064 6573 6572 6961 6c69 7a65 2066 6561   deserialize fea
-00016480: 7475 7265 7320 616e 6420 7374 6f72 6167  tures and storag
-00016490: 6520 636f 6e6e 6563 746f 720a 2020 2020  e connector.    
-000164a0: 2020 2020 2020 2020 7365 6c66 2e5f 6665          self._fe
-000164b0: 6174 7572 6573 203d 2028 0a20 2020 2020  atures = (.     
-000164c0: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
-000164d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000164e0: 2066 6561 7475 7265 2e46 6561 7475 7265   feature.Feature
-000164f0: 2e66 726f 6d5f 7265 7370 6f6e 7365 5f6a  .from_response_j
-00016500: 736f 6e28 6665 6174 290a 2020 2020 2020  son(feat).      
-00016510: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00016520: 2069 7369 6e73 7461 6e63 6528 6665 6174   isinstance(feat
-00016530: 2c20 6469 6374 290a 2020 2020 2020 2020  , dict).        
-00016540: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00016550: 2066 6561 740a 2020 2020 2020 2020 2020   feat.          
-00016560: 2020 2020 2020 2020 2020 666f 7220 6665            for fe
-00016570: 6174 2069 6e20 6665 6174 7572 6573 0a20  at in features. 
-00016580: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00016590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000165a0: 2069 6620 6665 6174 7572 6573 0a20 2020   if features.   
-000165b0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000165c0: 6520 4e6f 6e65 0a20 2020 2020 2020 2020  e None.         
-000165d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000165e0: 2073 656c 662e 7072 696d 6172 795f 6b65   self.primary_ke
-000165f0: 7920 3d20 280a 2020 2020 2020 2020 2020  y = (.          
-00016600: 2020 2020 2020 5b66 6561 742e 6e61 6d65        [feat.name
-00016610: 2066 6f72 2066 6561 7420 696e 2073 656c   for feat in sel
-00016620: 662e 5f66 6561 7475 7265 7320 6966 2066  f._features if f
-00016630: 6561 742e 7072 696d 6172 7920 6973 2054  eat.primary is T
-00016640: 7275 655d 0a20 2020 2020 2020 2020 2020  rue].           
-00016650: 2020 2020 2069 6620 7365 6c66 2e5f 6665       if self._fe
-00016660: 6174 7572 6573 0a20 2020 2020 2020 2020  atures.         
-00016670: 2020 2020 2020 2065 6c73 6520 5b5d 0a20         else []. 
-00016680: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00016690: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-000166a0: 6174 6973 7469 6373 5f63 6f6e 6669 6720  atistics_config 
-000166b0: 3d20 7374 6174 6973 7469 6373 5f63 6f6e  = statistics_con
-000166c0: 6669 670a 2020 2020 2020 2020 2020 2020  fig.            
-000166d0: 7365 6c66 2e65 7870 6563 7461 7469 6f6e  self.expectation
-000166e0: 5f73 7569 7465 203d 2065 7870 6563 7461  _suite = expecta
-000166f0: 7469 6f6e 5f73 7569 7465 0a0a 2020 2020  tion_suite..    
-00016700: 2020 2020 2020 2020 7365 6c66 2e5f 6f70          self._op
-00016710: 7469 6f6e 7320 3d20 280a 2020 2020 2020  tions = (.      
-00016720: 2020 2020 2020 2020 2020 7b6f 7074 696f            {optio
-00016730: 6e5b 226e 616d 6522 5d3a 206f 7074 696f  n["name"]: optio
-00016740: 6e5b 2276 616c 7565 225d 2066 6f72 206f  n["value"] for o
-00016750: 7074 696f 6e20 696e 206f 7074 696f 6e73  ption in options
-00016760: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00016770: 2020 6966 206f 7074 696f 6e73 0a20 2020    if options.   
-00016780: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00016790: 6520 4e6f 6e65 0a20 2020 2020 2020 2020  e None.         
-000167a0: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
-000167b0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000167c0: 656c 662e 7072 696d 6172 795f 6b65 7920  elf.primary_key 
-000167d0: 3d20 7072 696d 6172 795f 6b65 790a 2020  = primary_key.  
-000167e0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000167f0: 7461 7469 7374 6963 735f 636f 6e66 6967  tatistics_config
-00016800: 203d 2073 7461 7469 7374 6963 735f 636f   = statistics_co
-00016810: 6e66 6967 0a20 2020 2020 2020 2020 2020  nfig.           
-00016820: 2073 656c 662e 6578 7065 6374 6174 696f   self.expectatio
-00016830: 6e5f 7375 6974 6520 3d20 6578 7065 6374  n_suite = expect
-00016840: 6174 696f 6e5f 7375 6974 650a 2020 2020  ation_suite.    
-00016850: 2020 2020 2020 2020 7365 6c66 2e5f 6665          self._fe
-00016860: 6174 7572 6573 203d 2066 6561 7475 7265  atures = feature
-00016870: 730a 2020 2020 2020 2020 2020 2020 7365  s.            se
-00016880: 6c66 2e5f 6f70 7469 6f6e 7320 3d20 6f70  lf._options = op
-00016890: 7469 6f6e 730a 0a20 2020 2020 2020 2069  tions..        i
-000168a0: 6620 7374 6f72 6167 655f 636f 6e6e 6563  f storage_connec
-000168b0: 746f 7220 6973 206e 6f74 204e 6f6e 6520  tor is not None 
-000168c0: 616e 6420 6973 696e 7374 616e 6365 2873  and isinstance(s
-000168d0: 746f 7261 6765 5f63 6f6e 6e65 6374 6f72  torage_connector
-000168e0: 2c20 6469 6374 293a 0a20 2020 2020 2020  , dict):.       
-000168f0: 2020 2020 2073 656c 662e 5f73 746f 7261       self._stora
-00016900: 6765 5f63 6f6e 6e65 6374 6f72 203d 2073  ge_connector = s
-00016910: 632e 5374 6f72 6167 6543 6f6e 6e65 6374  c.StorageConnect
-00016920: 6f72 2e66 726f 6d5f 7265 7370 6f6e 7365  or.from_response
-00016930: 5f6a 736f 6e28 0a20 2020 2020 2020 2020  _json(.         
-00016940: 2020 2020 2020 2073 746f 7261 6765 5f63         storage_c
-00016950: 6f6e 6e65 6374 6f72 0a20 2020 2020 2020  onnector.       
-00016960: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
-00016970: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00016980: 2073 656c 662e 5f73 746f 7261 6765 5f63   self._storage_c
-00016990: 6f6e 6e65 6374 6f72 203d 2073 746f 7261  onnector = stora
-000169a0: 6765 5f63 6f6e 6e65 6374 6f72 0a0a 2020  ge_connector..  
-000169b0: 2020 2020 2020 7365 6c66 2e65 7870 6563        self.expec
-000169c0: 7461 7469 6f6e 5f73 7569 7465 203d 2065  tation_suite = e
-000169d0: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-000169e0: 0a20 2020 2020 2020 2073 656c 662e 5f68  .        self._h
-000169f0: 7265 6620 3d20 6872 6566 0a0a 2020 2020  ref = href..    
-00016a00: 6465 6620 7361 7665 2873 656c 6629 3a0a  def save(self):.
-00016a10: 2020 2020 2020 2020 2222 2250 6572 7369          """Persi
-00016a20: 7374 2074 6865 206d 6574 6164 6174 6120  st the metadata 
-00016a30: 666f 7220 7468 6973 2065 7874 6572 6e61  for this externa
-00016a40: 6c20 6665 6174 7572 6520 6772 6f75 702e  l feature group.
-00016a50: 0a0a 2020 2020 2020 2020 5769 7468 6f75  ..        Withou
-00016a60: 7420 6361 6c6c 696e 6720 7468 6973 206d  t calling this m
-00016a70: 6574 686f 642c 2079 6f75 7220 6665 6174  ethod, your feat
-00016a80: 7572 6520 6772 6f75 7020 7769 6c6c 206f  ure group will o
-00016a90: 6e6c 7920 6578 6973 740a 2020 2020 2020  nly exist.      
-00016aa0: 2020 696e 2079 6f75 7220 5079 7468 6f6e    in your Python
-00016ab0: 204b 6572 6e65 6c2c 2062 7574 206e 6f74   Kernel, but not
-00016ac0: 2069 6e20 486f 7073 776f 726b 732e 0a0a   in Hopsworks...
-00016ad0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-00016ae0: 6e0a 2020 2020 2020 2020 7175 6572 7920  n.        query 
-00016af0: 3d20 2253 454c 4543 5420 2a20 4652 4f4d  = "SELECT * FROM
-00016b00: 2073 616c 6573 220a 0a20 2020 2020 2020   sales"..       
-00016b10: 2066 6720 3d20 6665 6174 7572 655f 7374   fg = feature_st
-00016b20: 6f72 652e 6372 6561 7465 5f65 7874 6572  ore.create_exter
-00016b30: 6e61 6c5f 6665 6174 7572 655f 6772 6f75  nal_feature_grou
-00016b40: 7028 6e61 6d65 3d22 7361 6c65 7322 2c0a  p(name="sales",.
-00016b50: 2020 2020 2020 2020 2020 2020 7665 7273              vers
-00016b60: 696f 6e3d 312c 0a20 2020 2020 2020 2020  ion=1,.         
-00016b70: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
-00016b80: 5068 7973 6963 616c 2073 686f 7020 7361  Physical shop sa
-00016b90: 6c65 7320 6665 6174 7572 6573 222c 0a20  les features",. 
-00016ba0: 2020 2020 2020 2020 2020 2071 7565 7279             query
-00016bb0: 3d71 7565 7279 2c0a 2020 2020 2020 2020  =query,.        
-00016bc0: 2020 2020 7374 6f72 6167 655f 636f 6e6e      storage_conn
-00016bd0: 6563 746f 723d 636f 6e6e 6563 746f 722c  ector=connector,
-00016be0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00016bf0: 6d61 7279 5f6b 6579 3d5b 2773 735f 7374  mary_key=['ss_st
-00016c00: 6f72 655f 736b 275d 2c0a 2020 2020 2020  ore_sk'],.      
-00016c10: 2020 2020 2020 6576 656e 745f 7469 6d65        event_time
-00016c20: 3d27 7361 6c65 5f64 6174 6527 0a20 2020  ='sale_date'.   
-00016c30: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00016c40: 6667 2e73 6176 6528 290a 2020 2020 2020  fg.save().      
-00016c50: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
-00016c60: 6c66 2e5f 6665 6174 7572 655f 6772 6f75  lf._feature_grou
-00016c70: 705f 656e 6769 6e65 2e73 6176 6528 7365  p_engine.save(se
-00016c80: 6c66 290a 2020 2020 2020 2020 7365 6c66  lf).        self
-00016c90: 2e5f 636f 6465 5f65 6e67 696e 652e 7361  ._code_engine.sa
-00016ca0: 7665 5f63 6f64 6528 7365 6c66 290a 0a20  ve_code(self).. 
-00016cb0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00016cc0: 7461 7469 7374 6963 735f 636f 6e66 6967  tatistics_config
-00016cd0: 2e65 6e61 626c 6564 3a0a 2020 2020 2020  .enabled:.      
-00016ce0: 2020 2020 2020 7365 6c66 2e5f 7374 6174        self._stat
-00016cf0: 6973 7469 6373 5f65 6e67 696e 652e 636f  istics_engine.co
-00016d00: 6d70 7574 655f 7374 6174 6973 7469 6373  mpute_statistics
-00016d10: 2873 656c 6629 0a0a 2020 2020 6465 6620  (self)..    def 
-00016d20: 7265 6164 2873 656c 662c 2064 6174 6166  read(self, dataf
-00016d30: 7261 6d65 5f74 7970 653d 2264 6566 6175  rame_type="defau
-00016d40: 6c74 2229 3a0a 2020 2020 2020 2020 2222  lt"):.        ""
-00016d50: 2247 6574 2074 6865 2066 6561 7475 7265  "Get the feature
-00016d60: 2067 726f 7570 2061 7320 6120 4461 7461   group as a Data
-00016d70: 4672 616d 652e 0a0a 2020 2020 2020 2020  Frame...        
-00016d80: 2121 2120 6578 616d 706c 650a 2020 2020  !!! example.    
-00016d90: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-00016da0: 6e0a 2020 2020 2020 2020 2020 2020 2320  n.            # 
-00016db0: 636f 6e6e 6563 7420 746f 2074 6865 2046  connect to the F
-00016dc0: 6561 7475 7265 2053 746f 7265 0a20 2020  eature Store.   
-00016dd0: 2020 2020 2020 2020 2066 7320 3d20 2e2e           fs = ..
-00016de0: 2e0a 0a20 2020 2020 2020 2020 2020 2023  ...            #
-00016df0: 2067 6574 2074 6865 2046 6561 7475 7265   get the Feature
-00016e00: 2047 726f 7570 2069 6e73 7461 6e63 650a   Group instance.
-00016e10: 2020 2020 2020 2020 2020 2020 6667 203d              fg =
-00016e20: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
-00016e30: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
-00016e40: 2e2e 2e29 0a0a 2020 2020 2020 2020 2020  ...)..          
-00016e50: 2020 6466 203d 2066 672e 7265 6164 2829    df = fg.read()
-00016e60: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
-00016e70: 0a0a 2020 2020 2020 2020 2121 2120 7761  ..        !!! wa
-00016e80: 726e 696e 6720 2245 6e67 696e 6520 5375  rning "Engine Su
-00016e90: 7070 6f72 7422 0a20 2020 2020 2020 2020  pport".         
-00016ea0: 2020 202a 2a53 7061 726b 206f 6e6c 792a     **Spark only*
-00016eb0: 2a0a 0a20 2020 2020 2020 2020 2020 2052  *..            R
-00016ec0: 6561 6469 6e67 2061 6e20 4578 7465 726e  eading an Extern
-00016ed0: 616c 2046 6561 7475 7265 2047 726f 7570  al Feature Group
-00016ee0: 2064 6972 6563 746c 7920 696e 746f 2061   directly into a
-00016ef0: 2050 616e 6461 7320 4461 7461 6672 616d   Pandas Datafram
-00016f00: 6520 7573 696e 670a 2020 2020 2020 2020  e using.        
-00016f10: 2020 2020 5079 7468 6f6e 2f50 616e 6461      Python/Panda
-00016f20: 7320 6173 2045 6e67 696e 6520 6973 206e  s as Engine is n
-00016f30: 6f74 2073 7570 706f 7274 6564 2c20 686f  ot supported, ho
-00016f40: 7765 7665 722c 2079 6f75 2063 616e 2075  wever, you can u
-00016f50: 7365 2074 6865 0a20 2020 2020 2020 2020  se the.         
-00016f60: 2020 2051 7565 7279 2041 5049 2074 6f20     Query API to 
-00016f70: 6372 6561 7465 2046 6561 7475 7265 2056  create Feature V
-00016f80: 6965 7773 2f54 7261 696e 696e 6720 4461  iews/Training Da
-00016f90: 7461 2063 6f6e 7461 696e 696e 6720 4578  ta containing Ex
-00016fa0: 7465 726e 616c 0a20 2020 2020 2020 2020  ternal.         
-00016fb0: 2020 2046 6561 7475 7265 2047 726f 7570     Feature Group
-00016fc0: 732e 0a0a 2020 2020 2020 2020 2320 4172  s...        # Ar
-00016fd0: 6775 6d65 6e74 730a 2020 2020 2020 2020  guments.        
-00016fe0: 2020 2020 6461 7461 6672 616d 655f 7479      dataframe_ty
-00016ff0: 7065 3a20 7374 722c 206f 7074 696f 6e61  pe: str, optiona
-00017000: 6c2e 2050 6f73 7369 626c 6520 7661 6c75  l. Possible valu
-00017010: 6573 2061 7265 2060 2264 6566 6175 6c74  es are `"default
-00017020: 2260 2c20 6022 7370 6172 6b22 602c 0a20  "`, `"spark"`,. 
-00017030: 2020 2020 2020 2020 2020 2020 2020 2060                 `
-00017040: 2270 616e 6461 7322 602c 2060 226e 756d  "pandas"`, `"num
-00017050: 7079 2260 206f 7220 6022 7079 7468 6f6e  py"` or `"python
-00017060: 2260 2c20 6465 6661 756c 7473 2074 6f20  "`, defaults to 
-00017070: 6022 6465 6661 756c 7422 602e 0a0a 2020  `"default"`...  
-00017080: 2020 2020 2020 2320 5265 7475 726e 730a        # Returns.
-00017090: 2020 2020 2020 2020 2020 2020 6044 6174              `Dat
-000170a0: 6146 7261 6d65 603a 2054 6865 2073 7061  aFrame`: The spa
-000170b0: 726b 2064 6174 6166 7261 6d65 2063 6f6e  rk dataframe con
-000170c0: 7461 696e 696e 6720 7468 6520 6665 6174  taining the feat
-000170d0: 7572 6520 6461 7461 2e0a 2020 2020 2020  ure data..      
-000170e0: 2020 2020 2020 6070 7973 7061 726b 2e44        `pyspark.D
-000170f0: 6174 6146 7261 6d65 602e 2041 2053 7061  ataFrame`. A Spa
-00017100: 726b 2044 6174 6146 7261 6d65 2e0a 2020  rk DataFrame..  
-00017110: 2020 2020 2020 2020 2020 6070 616e 6461            `panda
-00017120: 732e 4461 7461 4672 616d 6560 2e20 4120  s.DataFrame`. A 
-00017130: 5061 6e64 6173 2044 6174 6146 7261 6d65  Pandas DataFrame
-00017140: 2e0a 2020 2020 2020 2020 2020 2020 606e  ..            `n
-00017150: 756d 7079 2e6e 6461 7272 6179 602e 2041  umpy.ndarray`. A
-00017160: 2074 776f 2d64 696d 656e 7369 6f6e 616c   two-dimensional
-00017170: 204e 756d 7079 2061 7272 6179 2e0a 2020   Numpy array..  
-00017180: 2020 2020 2020 2020 2020 606c 6973 7460            `list`
-00017190: 2e20 4120 7477 6f2d 6469 6d65 6e73 696f  . A two-dimensio
-000171a0: 6e61 6c20 5079 7468 6f6e 206c 6973 742e  nal Python list.
-000171b0: 0a0a 2020 2020 2020 2020 2320 5261 6973  ..        # Rais
-000171c0: 6573 0a20 2020 2020 2020 2020 2020 2060  es.            `
-000171d0: 6873 6673 2e63 6c69 656e 742e 6578 6365  hsfs.client.exce
-000171e0: 7074 696f 6e73 2e52 6573 7441 5049 4572  ptions.RestAPIEr
-000171f0: 726f 7260 2e0a 2020 2020 2020 2020 2222  ror`..        ""
-00017200: 220a 2020 2020 2020 2020 656e 6769 6e65  ".        engine
-00017210: 2e67 6574 5f69 6e73 7461 6e63 6528 292e  .get_instance().
-00017220: 7365 745f 6a6f 625f 6772 6f75 7028 0a20  set_job_group(. 
-00017230: 2020 2020 2020 2020 2020 2022 4665 7463             "Fetc
-00017240: 6869 6e67 2046 6561 7475 7265 2067 726f  hing Feature gro
-00017250: 7570 222c 0a20 2020 2020 2020 2020 2020  up",.           
-00017260: 2022 4765 7474 696e 6720 6665 6174 7572   "Getting featur
-00017270: 6520 6772 6f75 703a 207b 7d20 6672 6f6d  e group: {} from
-00017280: 2074 6865 2066 6561 7475 7265 7374 6f72   the featurestor
-00017290: 6520 7b7d 222e 666f 726d 6174 280a 2020  e {}".format(.  
-000172a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000172b0: 6c66 2e5f 6e61 6d65 2c20 7365 6c66 2e5f  lf._name, self._
-000172c0: 6665 6174 7572 655f 7374 6f72 655f 6e61  feature_store_na
-000172d0: 6d65 0a20 2020 2020 2020 2020 2020 2029  me.            )
-000172e0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-000172f0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00017300: 7365 6c65 6374 5f61 6c6c 2829 2e72 6561  select_all().rea
-00017310: 6428 6461 7461 6672 616d 655f 7479 7065  d(dataframe_type
-00017320: 3d64 6174 6166 7261 6d65 5f74 7970 6529  =dataframe_type)
-00017330: 0a0a 2020 2020 6465 6620 7368 6f77 2873  ..    def show(s
-00017340: 656c 662c 206e 293a 0a20 2020 2020 2020  elf, n):.       
-00017350: 2022 2222 5368 6f77 2074 6865 2066 6972   """Show the fir
-00017360: 7374 206e 2072 6f77 7320 6f66 2074 6865  st n rows of the
-00017370: 2066 6561 7475 7265 2067 726f 7570 2e0a   feature group..
-00017380: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
-00017390: 6d70 6c65 0a20 2020 2020 2020 2020 2020  mple.           
-000173a0: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
-000173b0: 2020 2020 2020 2023 2063 6f6e 6e65 6374         # connect
-000173c0: 2074 6f20 7468 6520 4665 6174 7572 6520   to the Feature 
-000173d0: 5374 6f72 650a 2020 2020 2020 2020 2020  Store.          
-000173e0: 2020 6673 203d 202e 2e2e 0a0a 2020 2020    fs = .....    
-000173f0: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
-00017400: 6520 4665 6174 7572 6520 4772 6f75 7020  e Feature Group 
-00017410: 696e 7374 616e 6365 0a20 2020 2020 2020  instance.       
-00017420: 2020 2020 2066 6720 3d20 6673 2e67 6574       fg = fs.get
-00017430: 5f6f 725f 6372 6561 7465 5f66 6561 7475  _or_create_featu
-00017440: 7265 5f67 726f 7570 282e 2e2e 290a 0a20  re_group(...).. 
-00017450: 2020 2020 2020 2020 2020 2066 672e 7368             fg.sh
-00017460: 6f77 2835 290a 2020 2020 2020 2020 2020  ow(5).          
-00017470: 2020 6060 600a 2020 2020 2020 2020 2222    ```.        ""
-00017480: 220a 2020 2020 2020 2020 656e 6769 6e65  ".        engine
-00017490: 2e67 6574 5f69 6e73 7461 6e63 6528 292e  .get_instance().
-000174a0: 7365 745f 6a6f 625f 6772 6f75 7028 0a20  set_job_group(. 
-000174b0: 2020 2020 2020 2020 2020 2022 4665 7463             "Fetc
-000174c0: 6869 6e67 2046 6561 7475 7265 2067 726f  hing Feature gro
-000174d0: 7570 222c 0a20 2020 2020 2020 2020 2020  up",.           
-000174e0: 2022 4765 7474 696e 6720 6665 6174 7572   "Getting featur
-000174f0: 6520 6772 6f75 703a 207b 7d20 6672 6f6d  e group: {} from
-00017500: 2074 6865 2066 6561 7475 7265 7374 6f72   the featurestor
-00017510: 6520 7b7d 222e 666f 726d 6174 280a 2020  e {}".format(.  
-00017520: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00017530: 6c66 2e5f 6e61 6d65 2c20 7365 6c66 2e5f  lf._name, self._
-00017540: 6665 6174 7572 655f 7374 6f72 655f 6e61  feature_store_na
-00017550: 6d65 0a20 2020 2020 2020 2020 2020 2029  me.            )
-00017560: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00017570: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00017580: 7365 6c65 6374 5f61 6c6c 2829 2e73 686f  select_all().sho
-00017590: 7728 6e29 0a0a 2020 2020 4063 6c61 7373  w(n)..    @class
-000175a0: 6d65 7468 6f64 0a20 2020 2064 6566 2066  method.    def f
-000175b0: 726f 6d5f 7265 7370 6f6e 7365 5f6a 736f  rom_response_jso
-000175c0: 6e28 636c 732c 206a 736f 6e5f 6469 6374  n(cls, json_dict
-000175d0: 293a 0a20 2020 2020 2020 206a 736f 6e5f  ):.        json_
-000175e0: 6465 6361 6d65 6c69 7a65 6420 3d20 6875  decamelized = hu
-000175f0: 6d70 732e 6465 6361 6d65 6c69 7a65 286a  mps.decamelize(j
-00017600: 736f 6e5f 6469 6374 290a 2020 2020 2020  son_dict).      
-00017610: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00017620: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
-00017630: 2c20 6469 6374 293a 0a20 2020 2020 2020  , dict):.       
-00017640: 2020 2020 205f 203d 206a 736f 6e5f 6465       _ = json_de
-00017650: 6361 6d65 6c69 7a65 642e 706f 7028 226f  camelized.pop("o
-00017660: 6e6c 696e 655f 746f 7069 635f 6e61 6d65  nline_topic_name
-00017670: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
-00017680: 2020 2020 205f 203d 206a 736f 6e5f 6465       _ = json_de
-00017690: 6361 6d65 6c69 7a65 642e 706f 7028 2274  camelized.pop("t
-000176a0: 7970 6522 2c20 4e6f 6e65 290a 2020 2020  ype", None).    
-000176b0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-000176c0: 6c73 282a 2a6a 736f 6e5f 6465 6361 6d65  ls(**json_decame
-000176d0: 6c69 7a65 6429 0a20 2020 2020 2020 2066  lized).        f
-000176e0: 6f72 2066 6720 696e 206a 736f 6e5f 6465  or fg in json_de
-000176f0: 6361 6d65 6c69 7a65 643a 0a20 2020 2020  camelized:.     
-00017700: 2020 2020 2020 205f 203d 2066 672e 706f         _ = fg.po
-00017710: 7028 226f 6e6c 696e 655f 746f 7069 635f  p("online_topic_
-00017720: 6e61 6d65 222c 204e 6f6e 6529 0a20 2020  name", None).   
-00017730: 2020 2020 2020 2020 205f 203d 2066 672e           _ = fg.
-00017740: 706f 7028 2274 7970 6522 2c20 4e6f 6e65  pop("type", None
-00017750: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00017760: 205b 636c 7328 2a2a 6667 2920 666f 7220   [cls(**fg) for 
-00017770: 6667 2069 6e20 6a73 6f6e 5f64 6563 616d  fg in json_decam
-00017780: 656c 697a 6564 5d0a 0a20 2020 2064 6566  elized]..    def
-00017790: 2075 7064 6174 655f 6672 6f6d 5f72 6573   update_from_res
-000177a0: 706f 6e73 655f 6a73 6f6e 2873 656c 662c  ponse_json(self,
-000177b0: 206a 736f 6e5f 6469 6374 293a 0a20 2020   json_dict):.   
-000177c0: 2020 2020 206a 736f 6e5f 6465 6361 6d65       json_decame
-000177d0: 6c69 7a65 6420 3d20 6875 6d70 732e 6465  lized = humps.de
-000177e0: 6361 6d65 6c69 7a65 286a 736f 6e5f 6469  camelize(json_di
-000177f0: 6374 290a 2020 2020 2020 2020 6966 2022  ct).        if "
-00017800: 7479 7065 2220 696e 206a 736f 6e5f 6465  type" in json_de
-00017810: 6361 6d65 6c69 7a65 643a 0a20 2020 2020  camelized:.     
-00017820: 2020 2020 2020 205f 203d 206a 736f 6e5f         _ = json_
-00017830: 6465 6361 6d65 6c69 7a65 642e 706f 7028  decamelized.pop(
-00017840: 2274 7970 6522 290a 2020 2020 2020 2020  "type").        
-00017850: 7365 6c66 2e5f 5f69 6e69 745f 5f28 2a2a  self.__init__(**
-00017860: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
-00017870: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00017880: 2073 656c 660a 0a20 2020 2064 6566 206a   self..    def j
-00017890: 736f 6e28 7365 6c66 293a 0a20 2020 2020  son(self):.     
-000178a0: 2020 2072 6574 7572 6e20 6a73 6f6e 2e64     return json.d
-000178b0: 756d 7073 2873 656c 662c 2063 6c73 3d75  umps(self, cls=u
-000178c0: 7469 6c2e 4665 6174 7572 6553 746f 7265  til.FeatureStore
-000178d0: 456e 636f 6465 7229 0a0a 2020 2020 6465  Encoder)..    de
-000178e0: 6620 746f 5f64 6963 7428 7365 6c66 293a  f to_dict(self):
-000178f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00017900: 7b0a 2020 2020 2020 2020 2020 2020 2269  {.            "i
-00017910: 6422 3a20 7365 6c66 2e5f 6964 2c0a 2020  d": self._id,.  
-00017920: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-00017930: 3a20 7365 6c66 2e5f 6e61 6d65 2c0a 2020  : self._name,.  
-00017940: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00017950: 6970 7469 6f6e 223a 2073 656c 662e 5f64  iption": self._d
-00017960: 6573 6372 6970 7469 6f6e 2c0a 2020 2020  escription,.    
-00017970: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
-00017980: 223a 2073 656c 662e 5f76 6572 7369 6f6e  ": self._version
-00017990: 2c0a 2020 2020 2020 2020 2020 2020 2266  ,.            "f
-000179a0: 6561 7475 7265 7322 3a20 7365 6c66 2e5f  eatures": self._
-000179b0: 6665 6174 7572 6573 2c0a 2020 2020 2020  features,.      
-000179c0: 2020 2020 2020 2266 6561 7475 7265 7374        "featurest
-000179d0: 6f72 6549 6422 3a20 7365 6c66 2e5f 6665  oreId": self._fe
-000179e0: 6174 7572 655f 7374 6f72 655f 6964 2c0a  ature_store_id,.
-000179f0: 2020 2020 2020 2020 2020 2020 2271 7565              "que
-00017a00: 7279 223a 2073 656c 662e 5f71 7565 7279  ry": self._query
-00017a10: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
-00017a20: 6174 6146 6f72 6d61 7422 3a20 7365 6c66  ataFormat": self
-00017a30: 2e5f 6461 7461 5f66 6f72 6d61 742c 0a20  ._data_format,. 
-00017a40: 2020 2020 2020 2020 2020 2022 7061 7468             "path
-00017a50: 223a 2073 656c 662e 5f70 6174 682c 0a20  ": self._path,. 
-00017a60: 2020 2020 2020 2020 2020 2022 6f70 7469             "opti
-00017a70: 6f6e 7322 3a20 5b7b 226e 616d 6522 3a20  ons": [{"name": 
-00017a80: 6b2c 2022 7661 6c75 6522 3a20 767d 2066  k, "value": v} f
-00017a90: 6f72 206b 2c20 7620 696e 2073 656c 662e  or k, v in self.
-00017aa0: 5f6f 7074 696f 6e73 2e69 7465 6d73 2829  _options.items()
-00017ab0: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
-00017ac0: 2073 656c 662e 5f6f 7074 696f 6e73 0a20   self._options. 
-00017ad0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-00017ae0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00017af0: 2020 2273 746f 7261 6765 436f 6e6e 6563    "storageConnec
-00017b00: 746f 7222 3a20 7365 6c66 2e5f 7374 6f72  tor": self._stor
-00017b10: 6167 655f 636f 6e6e 6563 746f 722e 746f  age_connector.to
-00017b20: 5f64 6963 7428 292c 0a20 2020 2020 2020  _dict(),.       
-00017b30: 2020 2020 2022 7479 7065 223a 2022 6f6e       "type": "on
-00017b40: 4465 6d61 6e64 4665 6174 7572 6567 726f  DemandFeaturegro
-00017b50: 7570 4454 4f22 2c0a 2020 2020 2020 2020  upDTO",.        
-00017b60: 2020 2020 2273 7461 7469 7374 6963 7343      "statisticsC
-00017b70: 6f6e 6669 6722 3a20 7365 6c66 2e5f 7374  onfig": self._st
-00017b80: 6174 6973 7469 6373 5f63 6f6e 6669 672c  atistics_config,
-00017b90: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
-00017ba0: 656e 7454 696d 6522 3a20 7365 6c66 2e5f  entTime": self._
-00017bb0: 6576 656e 745f 7469 6d65 2c0a 2020 2020  event_time,.    
-00017bc0: 2020 2020 2020 2020 2265 7870 6563 7461          "expecta
-00017bd0: 7469 6f6e 5375 6974 6522 3a20 7365 6c66  tionSuite": self
-00017be0: 2e5f 6578 7065 6374 6174 696f 6e5f 7375  ._expectation_su
-00017bf0: 6974 652c 0a20 2020 2020 2020 207d 0a0a  ite,.        }..
-00017c00: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00017c10: 2020 6465 6620 6964 2873 656c 6629 3a0a    def id(self):.
-00017c20: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00017c30: 656c 662e 5f69 640a 0a20 2020 2040 7072  elf._id..    @pr
-00017c40: 6f70 6572 7479 0a20 2020 2064 6566 206e  operty.    def n
-00017c50: 616d 6528 7365 6c66 293a 0a20 2020 2020  ame(self):.     
-00017c60: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00017c70: 6e61 6d65 0a0a 2020 2020 4070 726f 7065  name..    @prope
-00017c80: 7274 790a 2020 2020 6465 6620 7665 7273  rty.    def vers
-00017c90: 696f 6e28 7365 6c66 293a 0a20 2020 2020  ion(self):.     
-00017ca0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00017cb0: 7665 7273 696f 6e0a 0a20 2020 2040 7072  version..    @pr
-00017cc0: 6f70 6572 7479 0a20 2020 2064 6566 2064  operty.    def d
-00017cd0: 6573 6372 6970 7469 6f6e 2873 656c 6629  escription(self)
-00017ce0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00017cf0: 2073 656c 662e 5f64 6573 6372 6970 7469   self._descripti
-00017d00: 6f6e 0a0a 2020 2020 4070 726f 7065 7274  on..    @propert
-00017d10: 790a 2020 2020 6465 6620 6665 6174 7572  y.    def featur
-00017d20: 6573 2873 656c 6629 3a0a 2020 2020 2020  es(self):.      
-00017d30: 2020 7265 7475 726e 2073 656c 662e 5f66    return self._f
-00017d40: 6561 7475 7265 730a 0a20 2020 2040 7072  eatures..    @pr
-00017d50: 6f70 6572 7479 0a20 2020 2064 6566 2071  operty.    def q
-00017d60: 7565 7279 2873 656c 6629 3a0a 2020 2020  uery(self):.    
-00017d70: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00017d80: 5f71 7565 7279 0a0a 2020 2020 4070 726f  _query..    @pro
-00017d90: 7065 7274 790a 2020 2020 6465 6620 6461  perty.    def da
-00017da0: 7461 5f66 6f72 6d61 7428 7365 6c66 293a  ta_format(self):
-00017db0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00017dc0: 7365 6c66 2e5f 6461 7461 5f66 6f72 6d61  self._data_forma
-00017dd0: 740a 0a20 2020 2040 7072 6f70 6572 7479  t..    @property
-00017de0: 0a20 2020 2064 6566 2070 6174 6828 7365  .    def path(se
-00017df0: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-00017e00: 7572 6e20 7365 6c66 2e5f 7061 7468 0a0a  urn self._path..
-00017e10: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00017e20: 2020 6465 6620 6f70 7469 6f6e 7328 7365    def options(se
-00017e30: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-00017e40: 7572 6e20 7365 6c66 2e5f 6f70 7469 6f6e  urn self._option
-00017e50: 730a 0a20 2020 2040 7072 6f70 6572 7479  s..    @property
-00017e60: 0a20 2020 2064 6566 2073 746f 7261 6765  .    def storage
-00017e70: 5f63 6f6e 6e65 6374 6f72 2873 656c 6629  _connector(self)
-00017e80: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00017e90: 2073 656c 662e 5f73 746f 7261 6765 5f63   self._storage_c
-00017ea0: 6f6e 6e65 6374 6f72 0a0a 2020 2020 4070  onnector..    @p
-00017eb0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00017ec0: 6372 6561 746f 7228 7365 6c66 293a 0a20  creator(self):. 
-00017ed0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00017ee0: 6c66 2e5f 6372 6561 746f 720a 0a20 2020  lf._creator..   
-00017ef0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00017f00: 6566 2063 7265 6174 6564 2873 656c 6629  ef created(self)
-00017f10: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00017f20: 2073 656c 662e 5f63 7265 6174 6564 0a0a   self._created..
-00017f30: 2020 2020 4076 6572 7369 6f6e 2e73 6574      @version.set
-00017f40: 7465 720a 2020 2020 6465 6620 7665 7273  ter.    def vers
-00017f50: 696f 6e28 7365 6c66 2c20 7665 7273 696f  ion(self, versio
-00017f60: 6e29 3a0a 2020 2020 2020 2020 7365 6c66  n):.        self
-00017f70: 2e5f 7665 7273 696f 6e20 3d20 7665 7273  ._version = vers
-00017f80: 696f 6e0a 0a20 2020 2040 6465 7363 7269  ion..    @descri
-00017f90: 7074 696f 6e2e 7365 7474 6572 0a20 2020  ption.setter.   
-00017fa0: 2064 6566 2064 6573 6372 6970 7469 6f6e   def description
-00017fb0: 2873 656c 662c 206e 6577 5f64 6573 6372  (self, new_descr
-00017fc0: 6970 7469 6f6e 293a 0a20 2020 2020 2020  iption):.       
-00017fd0: 2073 656c 662e 5f64 6573 6372 6970 7469   self._descripti
-00017fe0: 6f6e 203d 206e 6577 5f64 6573 6372 6970  on = new_descrip
-00017ff0: 7469 6f6e 0a0a 2020 2020 4066 6561 7475  tion..    @featu
-00018000: 7265 732e 7365 7474 6572 0a20 2020 2064  res.setter.    d
-00018010: 6566 2066 6561 7475 7265 7328 7365 6c66  ef features(self
-00018020: 2c20 6e65 775f 6665 6174 7572 6573 293a  , new_features):
-00018030: 0a20 2020 2020 2020 2073 656c 662e 5f66  .        self._f
-00018040: 6561 7475 7265 7320 3d20 6e65 775f 6665  eatures = new_fe
-00018050: 6174 7572 6573 0a0a 2020 2020 4070 726f  atures..    @pro
-00018060: 7065 7274 790a 2020 2020 6465 6620 6665  perty.    def fe
-00018070: 6174 7572 655f 7374 6f72 655f 6e61 6d65  ature_store_name
-00018080: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00018090: 2222 224e 616d 6520 6f66 2074 6865 2066  """Name of the f
-000180a0: 6561 7475 7265 2073 746f 7265 2069 6e20  eature store in 
-000180b0: 7768 6963 6820 7468 6520 6665 6174 7572  which the featur
-000180c0: 6520 6772 6f75 7020 6973 206c 6f63 6174  e group is locat
-000180d0: 6564 2e22 2222 0a20 2020 2020 2020 2072  ed.""".        r
-000180e0: 6574 7572 6e20 7365 6c66 2e5f 6665 6174  eturn self._feat
-000180f0: 7572 655f 7374 6f72 655f 6e61 6d65 0a0a  ure_store_name..
-00018100: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00018110: 2020 6465 6620 6665 6174 7572 655f 7374    def feature_st
-00018120: 6f72 655f 6964 2873 656c 6629 3a0a 2020  ore_id(self):.  
-00018130: 2020 2020 2020 2222 2249 6420 6f66 2074        """Id of t
-00018140: 6865 2066 6561 7475 7265 2073 746f 7265  he feature store
-00018150: 2069 6e20 7768 6963 6820 7468 6520 6665   in which the fe
-00018160: 6174 7572 6520 6772 6f75 7020 6973 206c  ature group is l
-00018170: 6f63 6174 6564 2e22 2222 0a20 2020 2020  ocated.""".     
-00018180: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00018190: 6665 6174 7572 655f 7374 6f72 655f 6964  feature_store_id
-000181a0: 0a                                       .
+0000b330: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
+0000b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b350: 2020 2022 5072 6f76 6964 696e 6720 6576     "Providing ev
+0000b360: 656e 745f 7469 6d65 2061 7320 6120 7369  ent_time as a si
+0000b370: 6e67 6c65 2d65 6c65 6d65 6e74 206c 6973  ngle-element lis
+0000b380: 7420 6973 2064 6570 7265 6361 7465 6422  t is deprecated"
+0000b390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b3a0: 2020 2020 202b 2022 2061 6e64 2077 696c       + " and wil
+0000b3b0: 6c20 6265 2064 726f 7070 6564 2069 6e20  l be dropped in 
+0000b3c0: 6675 7475 7265 2076 6572 7369 6f6e 732e  future versions.
+0000b3d0: 2050 726f 7669 6465 2074 6865 2066 6561   Provide the fea
+0000b3e0: 7475 7265 5f6e 616d 6520 7374 7269 6e67  ture_name string
+0000b3f0: 2069 6e73 7465 6164 2e22 2c0a 2020 2020   instead.",.    
+0000b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b410: 4465 7072 6563 6174 696f 6e57 6172 6e69  DeprecationWarni
+0000b420: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
+0000b430: 2020 2020 2020 2020 7374 6163 6b6c 6576          stacklev
+0000b440: 656c 3d32 2c0a 2020 2020 2020 2020 2020  el=2,.          
+0000b450: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000b460: 2020 2020 2020 2020 7365 6c66 2e5f 6576          self._ev
+0000b470: 656e 745f 7469 6d65 203d 2066 6561 7475  ent_time = featu
+0000b480: 7265 5f6e 616d 655b 305d 0a20 2020 2020  re_name[0].     
+0000b490: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000b4a0: 6e0a 0a20 2020 2020 2020 2072 6169 7365  n..        raise
+0000b4b0: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+0000b4c0: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
+0000b4d0: 7469 6d65 206d 7573 7420 6265 2061 2073  time must be a s
+0000b4e0: 7472 696e 6720 636f 7272 6573 706f 6e64  tring correspond
+0000b4f0: 696e 6720 746f 2061 6e20 6578 6973 7469  ing to an existi
+0000b500: 6e67 2066 6561 7475 7265 206e 616d 6520  ng feature name 
+0000b510: 6f66 2074 6865 2046 6561 7475 7265 2047  of the Feature G
+0000b520: 726f 7570 2e22 0a20 2020 2020 2020 2029  roup.".        )
+0000b530: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0000b540: 2020 2020 6465 6620 6c6f 6361 7469 6f6e      def location
+0000b550: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000b560: 7265 7475 726e 2073 656c 662e 5f6c 6f63  return self._loc
+0000b570: 6174 696f 6e0a 0a20 2020 2040 7072 6f70  ation..    @prop
+0000b580: 6572 7479 0a20 2020 2064 6566 2065 7870  erty.    def exp
+0000b590: 6563 7461 7469 6f6e 5f73 7569 7465 280a  ectation_suite(.
+0000b5a0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000b5b0: 2020 2920 2d3e 204f 7074 696f 6e61 6c5b    ) -> Optional[
+0000b5c0: 4578 7065 6374 6174 696f 6e53 7569 7465  ExpectationSuite
+0000b5d0: 5d3a 0a20 2020 2020 2020 2022 2222 4578  ]:.        """Ex
+0000b5e0: 7065 6374 6174 696f 6e20 5375 6974 6520  pectation Suite 
+0000b5f0: 636f 6e66 6967 7572 6174 696f 6e20 6f62  configuration ob
+0000b600: 6a65 6374 2064 6566 696e 696e 6720 7468  ject defining th
+0000b610: 6520 7365 7474 696e 6773 2066 6f72 0a20  e settings for. 
+0000b620: 2020 2020 2020 2064 6174 6120 7661 6c69         data vali
+0000b630: 6461 7469 6f6e 206f 6620 7468 6520 6665  dation of the fe
+0000b640: 6174 7572 6520 6772 6f75 702e 2222 220a  ature group.""".
+0000b650: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000b660: 656c 662e 5f65 7870 6563 7461 7469 6f6e  elf._expectation
+0000b670: 5f73 7569 7465 0a0a 2020 2020 4065 7870  _suite..    @exp
+0000b680: 6563 7461 7469 6f6e 5f73 7569 7465 2e73  ectation_suite.s
+0000b690: 6574 7465 720a 2020 2020 6465 6620 6578  etter.    def ex
+0000b6a0: 7065 6374 6174 696f 6e5f 7375 6974 6528  pectation_suite(
+0000b6b0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000b6c0: 2020 2020 2020 2065 7870 6563 7461 7469         expectati
+0000b6d0: 6f6e 5f73 7569 7465 3a20 556e 696f 6e5b  on_suite: Union[
+0000b6e0: 0a20 2020 2020 2020 2020 2020 2045 7870  .            Exp
+0000b6f0: 6563 7461 7469 6f6e 5375 6974 652c 2067  ectationSuite, g
+0000b700: 652e 636f 7265 2e45 7870 6563 7461 7469  e.core.Expectati
+0000b710: 6f6e 5375 6974 652c 2064 6963 742c 204e  onSuite, dict, N
+0000b720: 6f6e 650a 2020 2020 2020 2020 5d2c 0a20  one.        ],. 
+0000b730: 2020 2029 3a0a 2020 2020 2020 2020 6966     ):.        if
+0000b740: 2069 7369 6e73 7461 6e63 6528 6578 7065   isinstance(expe
+0000b750: 6374 6174 696f 6e5f 7375 6974 652c 2045  ctation_suite, E
+0000b760: 7870 6563 7461 7469 6f6e 5375 6974 6529  xpectationSuite)
+0000b770: 3a0a 2020 2020 2020 2020 2020 2020 746d  :.            tm
+0000b780: 705f 6578 7065 6374 6174 696f 6e5f 7375  p_expectation_su
+0000b790: 6974 6520 3d20 6578 7065 6374 6174 696f  ite = expectatio
+0000b7a0: 6e5f 7375 6974 652e 746f 5f6a 736f 6e5f  n_suite.to_json_
+0000b7b0: 6469 6374 2829 0a20 2020 2020 2020 2020  dict().         
+0000b7c0: 2020 2074 6d70 5f65 7870 6563 7461 7469     tmp_expectati
+0000b7d0: 6f6e 5f73 7569 7465 5b22 6665 6174 7572  on_suite["featur
+0000b7e0: 6567 726f 7570 5f69 6422 5d20 3d20 7365  egroup_id"] = se
+0000b7f0: 6c66 2e5f 6964 0a20 2020 2020 2020 2020  lf._id.         
+0000b800: 2020 2074 6d70 5f65 7870 6563 7461 7469     tmp_expectati
+0000b810: 6f6e 5f73 7569 7465 5b22 6665 6174 7572  on_suite["featur
+0000b820: 6573 746f 7265 5f69 6422 5d20 3d20 7365  estore_id"] = se
+0000b830: 6c66 2e5f 6665 6174 7572 655f 7374 6f72  lf._feature_stor
+0000b840: 655f 6964 0a20 2020 2020 2020 2020 2020  e_id.           
+0000b850: 2073 656c 662e 5f65 7870 6563 7461 7469   self._expectati
+0000b860: 6f6e 5f73 7569 7465 203d 2045 7870 6563  on_suite = Expec
+0000b870: 7461 7469 6f6e 5375 6974 6528 2a2a 746d  tationSuite(**tm
+0000b880: 705f 6578 7065 6374 6174 696f 6e5f 7375  p_expectation_su
+0000b890: 6974 6529 0a20 2020 2020 2020 2065 6c69  ite).        eli
+0000b8a0: 6620 6973 696e 7374 616e 6365 2865 7870  f isinstance(exp
+0000b8b0: 6563 7461 7469 6f6e 5f73 7569 7465 2c20  ectation_suite, 
+0000b8c0: 6765 2e63 6f72 652e 6578 7065 6374 6174  ge.core.expectat
+0000b8d0: 696f 6e5f 7375 6974 652e 4578 7065 6374  ion_suite.Expect
+0000b8e0: 6174 696f 6e53 7569 7465 293a 0a20 2020  ationSuite):.   
+0000b8f0: 2020 2020 2020 2020 2073 656c 662e 5f65           self._e
+0000b900: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
+0000b910: 203d 2045 7870 6563 7461 7469 6f6e 5375   = ExpectationSu
+0000b920: 6974 6528 0a20 2020 2020 2020 2020 2020  ite(.           
+0000b930: 2020 2020 202a 2a65 7870 6563 7461 7469       **expectati
+0000b940: 6f6e 5f73 7569 7465 2e74 6f5f 6a73 6f6e  on_suite.to_json
+0000b950: 5f64 6963 7428 292c 0a20 2020 2020 2020  _dict(),.       
+0000b960: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+0000b970: 5f73 746f 7265 5f69 643d 7365 6c66 2e5f  _store_id=self._
+0000b980: 6665 6174 7572 655f 7374 6f72 655f 6964  feature_store_id
+0000b990: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b9a0: 2020 6665 6174 7572 655f 6772 6f75 705f    feature_group_
+0000b9b0: 6964 3d73 656c 662e 5f69 642c 0a20 2020  id=self._id,.   
+0000b9c0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000b9d0: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+0000b9e0: 6365 2865 7870 6563 7461 7469 6f6e 5f73  ce(expectation_s
+0000b9f0: 7569 7465 2c20 6469 6374 293a 0a20 2020  uite, dict):.   
+0000ba00: 2020 2020 2020 2020 2074 6d70 5f65 7870           tmp_exp
+0000ba10: 6563 7461 7469 6f6e 5f73 7569 7465 203d  ectation_suite =
+0000ba20: 2065 7870 6563 7461 7469 6f6e 5f73 7569   expectation_sui
+0000ba30: 7465 2e63 6f70 7928 290a 2020 2020 2020  te.copy().      
+0000ba40: 2020 2020 2020 746d 705f 6578 7065 6374        tmp_expect
+0000ba50: 6174 696f 6e5f 7375 6974 655b 2266 6561  ation_suite["fea
+0000ba60: 7475 7265 5f73 746f 7265 5f69 6422 5d20  ture_store_id"] 
+0000ba70: 3d20 7365 6c66 2e5f 6665 6174 7572 655f  = self._feature_
+0000ba80: 7374 6f72 655f 6964 0a20 2020 2020 2020  store_id.       
+0000ba90: 2020 2020 2074 6d70 5f65 7870 6563 7461       tmp_expecta
+0000baa0: 7469 6f6e 5f73 7569 7465 5b22 6665 6174  tion_suite["feat
+0000bab0: 7572 655f 6772 6f75 705f 6964 225d 203d  ure_group_id"] =
+0000bac0: 2073 656c 662e 5f69 640a 2020 2020 2020   self._id.      
+0000bad0: 2020 2020 2020 7365 6c66 2e5f 6578 7065        self._expe
+0000bae0: 6374 6174 696f 6e5f 7375 6974 6520 3d20  ctation_suite = 
+0000baf0: 4578 7065 6374 6174 696f 6e53 7569 7465  ExpectationSuite
+0000bb00: 282a 2a74 6d70 5f65 7870 6563 7461 7469  (**tmp_expectati
+0000bb10: 6f6e 5f73 7569 7465 290a 2020 2020 2020  on_suite).      
+0000bb20: 2020 656c 6966 2065 7870 6563 7461 7469    elif expectati
+0000bb30: 6f6e 5f73 7569 7465 2069 7320 4e6f 6e65  on_suite is None
+0000bb40: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000bb50: 6c66 2e5f 6578 7065 6374 6174 696f 6e5f  lf._expectation_
+0000bb60: 7375 6974 6520 3d20 4e6f 6e65 0a20 2020  suite = None.   
+0000bb70: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000bb80: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+0000bb90: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+0000bba0: 2020 2020 2020 2020 2254 6865 2061 7267          "The arg
+0000bbb0: 756d 656e 7420 6065 7870 6563 7461 7469  ument `expectati
+0000bbc0: 6f6e 5f73 7569 7465 6020 6861 7320 746f  on_suite` has to
+0000bbd0: 2062 6520 604e 6f6e 6560 206f 6620 7479   be `None` of ty
+0000bbe0: 7065 2060 4578 7065 6374 6174 696f 6e53  pe `ExpectationS
+0000bbf0: 7569 7465 6020 6f72 2060 6469 6374 602c  uite` or `dict`,
+0000bc00: 2062 7574 2069 7320 6f66 2074 7970 653a   but is of type:
+0000bc10: 2060 7b7d 6022 2e66 6f72 6d61 7428 0a20   `{}`".format(. 
+0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc30: 2020 2074 7970 6528 6578 7065 6374 6174     type(expectat
+0000bc40: 696f 6e5f 7375 6974 6529 0a20 2020 2020  ion_suite).     
+0000bc50: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000bc60: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000bc70: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000bc80: 6620 6f6e 6c69 6e65 5f65 6e61 626c 6564  f online_enabled
+0000bc90: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000bca0: 2222 2253 6574 7469 6e67 2069 6620 7468  """Setting if th
+0000bcb0: 6520 6665 6174 7572 6520 6772 6f75 7020  e feature group 
+0000bcc0: 6973 2061 7661 696c 6162 6c65 2069 6e20  is available in 
+0000bcd0: 6f6e 6c69 6e65 2073 746f 7261 6765 2e22  online storage."
+0000bce0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0000bcf0: 6e20 7365 6c66 2e5f 6f6e 6c69 6e65 5f65  n self._online_e
+0000bd00: 6e61 626c 6564 0a0a 2020 2020 406f 6e6c  nabled..    @onl
+0000bd10: 696e 655f 656e 6162 6c65 642e 7365 7474  ine_enabled.sett
+0000bd20: 6572 0a20 2020 2064 6566 206f 6e6c 696e  er.    def onlin
+0000bd30: 655f 656e 6162 6c65 6428 7365 6c66 2c20  e_enabled(self, 
+0000bd40: 6f6e 6c69 6e65 5f65 6e61 626c 6564 293a  online_enabled):
+0000bd50: 0a20 2020 2020 2020 2073 656c 662e 5f6f  .        self._o
+0000bd60: 6e6c 696e 655f 656e 6162 6c65 6420 3d20  nline_enabled = 
+0000bd70: 6f6e 6c69 6e65 5f65 6e61 626c 6564 0a0a  online_enabled..
+0000bd80: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000bd90: 2020 6465 6620 7375 626a 6563 7428 7365    def subject(se
+0000bda0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000bdb0: 5375 626a 6563 7420 6f66 2074 6865 2066  Subject of the f
+0000bdc0: 6561 7475 7265 2067 726f 7570 2e22 2222  eature group."""
+0000bdd0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000bde0: 2e5f 7375 626a 6563 7420 6973 204e 6f6e  ._subject is Non
+0000bdf0: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
+0000be00: 2063 6163 6865 2074 6865 2073 6368 656d   cache the schem
+0000be10: 610a 2020 2020 2020 2020 2020 2020 7365  a.            se
+0000be20: 6c66 2e5f 7375 626a 6563 7420 3d20 7365  lf._subject = se
+0000be30: 6c66 2e5f 6665 6174 7572 655f 6772 6f75  lf._feature_grou
+0000be40: 705f 656e 6769 6e65 2e67 6574 5f73 7562  p_engine.get_sub
+0000be50: 6a65 6374 2873 656c 6629 0a20 2020 2020  ject(self).     
+0000be60: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+0000be70: 7375 626a 6563 740a 0a20 2020 2040 7072  subject..    @pr
+0000be80: 6f70 6572 7479 0a20 2020 2064 6566 2061  operty.    def a
+0000be90: 7672 6f5f 7363 6865 6d61 2873 656c 6629  vro_schema(self)
+0000bea0: 3a0a 2020 2020 2020 2020 2222 2241 7672  :.        """Avr
+0000beb0: 6f20 7363 6865 6d61 2072 6570 7265 7365  o schema represe
+0000bec0: 6e74 6174 696f 6e20 6f66 2074 6865 2066  ntation of the f
+0000bed0: 6561 7475 7265 2067 726f 7570 2e22 2222  eature group."""
+0000bee0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000bef0: 7365 6c66 2e73 7562 6a65 6374 5b22 7363  self.subject["sc
+0000bf00: 6865 6d61 225d 0a0a 2020 2020 6465 6620  hema"]..    def 
+0000bf10: 6765 745f 636f 6d70 6c65 785f 6665 6174  get_complex_feat
+0000bf20: 7572 6573 2873 656c 6629 3a0a 2020 2020  ures(self):.    
+0000bf30: 2020 2020 2222 2252 6574 7572 6e73 2074      """Returns t
+0000bf40: 6865 206e 616d 6573 206f 6620 616c 6c20  he names of all 
+0000bf50: 6665 6174 7572 6573 2077 6974 6820 6120  features with a 
+0000bf60: 636f 6d70 6c65 7820 6461 7461 2074 7970  complex data typ
+0000bf70: 6520 696e 2074 6869 730a 2020 2020 2020  e in this.      
+0000bf80: 2020 6665 6174 7572 6520 6772 6f75 702e    feature group.
+0000bf90: 0a0a 2020 2020 2020 2020 2121 2120 6578  ..        !!! ex
+0000bfa0: 616d 706c 650a 2020 2020 2020 2020 2020  ample.          
+0000bfb0: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
+0000bfc0: 2020 2020 2020 2020 636f 6d70 6c65 785f          complex_
+0000bfd0: 6474 7970 655f 6665 6174 7572 6573 203d  dtype_features =
+0000bfe0: 2066 672e 6765 745f 636f 6d70 6c65 785f   fg.get_complex_
+0000bff0: 6665 6174 7572 6573 2829 0a20 2020 2020  features().     
+0000c000: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+0000c010: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+0000c020: 6574 7572 6e20 5b66 2e6e 616d 6520 666f  eturn [f.name fo
+0000c030: 7220 6620 696e 2073 656c 662e 6665 6174  r f in self.feat
+0000c040: 7572 6573 2069 6620 662e 6973 5f63 6f6d  ures if f.is_com
+0000c050: 706c 6578 2829 5d0a 0a20 2020 2064 6566  plex()]..    def
+0000c060: 205f 6765 745f 656e 636f 6465 645f 6176   _get_encoded_av
+0000c070: 726f 5f73 6368 656d 6128 7365 6c66 293a  ro_schema(self):
+0000c080: 0a20 2020 2020 2020 2063 6f6d 706c 6578  .        complex
+0000c090: 5f66 6561 7475 7265 7320 3d20 7365 6c66  _features = self
+0000c0a0: 2e67 6574 5f63 6f6d 706c 6578 5f66 6561  .get_complex_fea
+0000c0b0: 7475 7265 7328 290a 2020 2020 2020 2020  tures().        
+0000c0c0: 7363 6865 6d61 203d 206a 736f 6e2e 6c6f  schema = json.lo
+0000c0d0: 6164 7328 7365 6c66 2e61 7672 6f5f 7363  ads(self.avro_sc
+0000c0e0: 6865 6d61 290a 0a20 2020 2020 2020 2066  hema)..        f
+0000c0f0: 6f72 2066 6965 6c64 2069 6e20 7363 6865  or field in sche
+0000c100: 6d61 5b22 6669 656c 6473 225d 3a0a 2020  ma["fields"]:.  
+0000c110: 2020 2020 2020 2020 2020 6966 2066 6965            if fie
+0000c120: 6c64 5b22 6e61 6d65 225d 2069 6e20 636f  ld["name"] in co
+0000c130: 6d70 6c65 785f 6665 6174 7572 6573 3a0a  mplex_features:.
+0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c150: 6669 656c 645b 2274 7970 6522 5d20 3d20  field["type"] = 
+0000c160: 5b22 6e75 6c6c 222c 2022 6279 7465 7322  ["null", "bytes"
+0000c170: 5d0a 0a20 2020 2020 2020 2073 6368 656d  ]..        schem
+0000c180: 615f 7320 3d20 6a73 6f6e 2e64 756d 7073  a_s = json.dumps
+0000c190: 2873 6368 656d 6129 0a20 2020 2020 2020  (schema).       
+0000c1a0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000c1b0: 2020 6176 726f 2e73 6368 656d 612e 7061    avro.schema.pa
+0000c1c0: 7273 6528 7363 6865 6d61 5f73 290a 2020  rse(schema_s).  
+0000c1d0: 2020 2020 2020 6578 6365 7074 2061 7672        except avr
+0000c1e0: 6f2e 7363 6865 6d61 2e53 6368 656d 6150  o.schema.SchemaP
+0000c1f0: 6172 7365 4578 6365 7074 696f 6e20 6173  arseException as
+0000c200: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+0000c210: 7261 6973 6520 4665 6174 7572 6553 746f  raise FeatureSto
+0000c220: 7265 4578 6365 7074 696f 6e28 2246 6169  reException("Fai
+0000c230: 6c65 6420 746f 2063 6f6e 7374 7275 6374  led to construct
+0000c240: 2041 7672 6f20 5363 6865 6d61 3a20 7b7d   Avro Schema: {}
+0000c250: 222e 666f 726d 6174 2865 2929 0a20 2020  ".format(e)).   
+0000c260: 2020 2020 2072 6574 7572 6e20 7363 6865       return sche
+0000c270: 6d61 5f73 0a0a 2020 2020 6465 6620 5f67  ma_s..    def _g
+0000c280: 6574 5f66 6561 7475 7265 5f61 7672 6f5f  et_feature_avro_
+0000c290: 7363 6865 6d61 2873 656c 662c 2066 6561  schema(self, fea
+0000c2a0: 7475 7265 5f6e 616d 6529 3a0a 2020 2020  ture_name):.    
+0000c2b0: 2020 2020 666f 7220 6669 656c 6420 696e      for field in
+0000c2c0: 206a 736f 6e2e 6c6f 6164 7328 7365 6c66   json.loads(self
+0000c2d0: 2e61 7672 6f5f 7363 6865 6d61 295b 2266  .avro_schema)["f
+0000c2e0: 6965 6c64 7322 5d3a 0a20 2020 2020 2020  ields"]:.       
+0000c2f0: 2020 2020 2069 6620 6669 656c 645b 226e       if field["n
+0000c300: 616d 6522 5d20 3d3d 2066 6561 7475 7265  ame"] == feature
+0000c310: 5f6e 616d 653a 0a20 2020 2020 2020 2020  _name:.         
+0000c320: 2020 2020 2020 2072 6574 7572 6e20 6a73         return js
+0000c330: 6f6e 2e64 756d 7073 2866 6965 6c64 5b22  on.dumps(field["
+0000c340: 7479 7065 225d 290a 0a0a 636c 6173 7320  type"])...class 
+0000c350: 4665 6174 7572 6547 726f 7570 2846 6561  FeatureGroup(Fea
+0000c360: 7475 7265 4772 6f75 7042 6173 6529 3a0a  tureGroupBase):.
+0000c370: 2020 2020 4341 4348 4544 5f46 4541 5455      CACHED_FEATU
+0000c380: 5245 5f47 524f 5550 203d 2022 4341 4348  RE_GROUP = "CACH
+0000c390: 4544 5f46 4541 5455 5245 5f47 524f 5550  ED_FEATURE_GROUP
+0000c3a0: 220a 2020 2020 5354 5245 414d 5f46 4541  ".    STREAM_FEA
+0000c3b0: 5455 5245 5f47 524f 5550 203d 2022 5354  TURE_GROUP = "ST
+0000c3c0: 5245 414d 5f46 4541 5455 5245 5f47 524f  REAM_FEATURE_GRO
+0000c3d0: 5550 220a 2020 2020 454e 5449 5459 5f54  UP".    ENTITY_T
+0000c3e0: 5950 4520 3d20 2266 6561 7475 7265 6772  YPE = "featuregr
+0000c3f0: 6f75 7073 220a 0a20 2020 2064 6566 205f  oups"..    def _
+0000c400: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0000c410: 2073 656c 662c 0a20 2020 2020 2020 206e   self,.        n
+0000c420: 616d 652c 0a20 2020 2020 2020 2076 6572  ame,.        ver
+0000c430: 7369 6f6e 2c0a 2020 2020 2020 2020 6665  sion,.        fe
+0000c440: 6174 7572 6573 746f 7265 5f69 642c 0a20  aturestore_id,. 
+0000c450: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+0000c460: 6f6e 3d22 222c 0a20 2020 2020 2020 2070  on="",.        p
+0000c470: 6172 7469 7469 6f6e 5f6b 6579 3d4e 6f6e  artition_key=Non
+0000c480: 652c 0a20 2020 2020 2020 2070 7269 6d61  e,.        prima
+0000c490: 7279 5f6b 6579 3d4e 6f6e 652c 0a20 2020  ry_key=None,.   
+0000c4a0: 2020 2020 2068 7564 695f 7072 6563 6f6d       hudi_precom
+0000c4b0: 6269 6e65 5f6b 6579 3d4e 6f6e 652c 0a20  bine_key=None,. 
+0000c4c0: 2020 2020 2020 2066 6561 7475 7265 7374         featurest
+0000c4d0: 6f72 655f 6e61 6d65 3d4e 6f6e 652c 0a20  ore_name=None,. 
+0000c4e0: 2020 2020 2020 2063 7265 6174 6564 3d4e         created=N
+0000c4f0: 6f6e 652c 0a20 2020 2020 2020 2063 7265  one,.        cre
+0000c500: 6174 6f72 3d4e 6f6e 652c 0a20 2020 2020  ator=None,.     
+0000c510: 2020 2069 643d 4e6f 6e65 2c0a 2020 2020     id=None,.    
+0000c520: 2020 2020 6665 6174 7572 6573 3d4e 6f6e      features=Non
+0000c530: 652c 0a20 2020 2020 2020 206c 6f63 6174  e,.        locat
+0000c540: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 2020  ion=None,.      
+0000c550: 2020 6f6e 6c69 6e65 5f65 6e61 626c 6564    online_enabled
+0000c560: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+0000c570: 7469 6d65 5f74 7261 7665 6c5f 666f 726d  time_travel_form
+0000c580: 6174 3d4e 6f6e 652c 0a20 2020 2020 2020  at=None,.       
+0000c590: 2073 7461 7469 7374 6963 735f 636f 6e66   statistics_conf
+0000c5a0: 6967 3d4e 6f6e 652c 0a20 2020 2020 2020  ig=None,.       
+0000c5b0: 206f 6e6c 696e 655f 746f 7069 635f 6e61   online_topic_na
+0000c5c0: 6d65 3d4e 6f6e 652c 0a20 2020 2020 2020  me=None,.       
+0000c5d0: 2065 7665 6e74 5f74 696d 653d 4e6f 6e65   event_time=None
+0000c5e0: 2c0a 2020 2020 2020 2020 7374 7265 616d  ,.        stream
+0000c5f0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+0000c600: 6578 7065 6374 6174 696f 6e5f 7375 6974  expectation_suit
+0000c610: 653d 4e6f 6e65 2c0a 2020 2020 2020 2020  e=None,.        
+0000c620: 7061 7265 6e74 733d 4e6f 6e65 2c0a 2020  parents=None,.  
+0000c630: 2020 2020 2020 6872 6566 3d4e 6f6e 652c        href=None,
+0000c640: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0000c650: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+0000c660: 280a 2020 2020 2020 2020 2020 2020 6665  (.            fe
+0000c670: 6174 7572 6573 746f 7265 5f69 642c 0a20  aturestore_id,. 
+0000c680: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
+0000c690: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+0000c6a0: 2065 7665 6e74 5f74 696d 653d 6576 656e   event_time=even
+0000c6b0: 745f 7469 6d65 2c0a 2020 2020 2020 2020  t_time,.        
+0000c6c0: 2020 2020 6f6e 6c69 6e65 5f65 6e61 626c      online_enabl
+0000c6d0: 6564 3d6f 6e6c 696e 655f 656e 6162 6c65  ed=online_enable
+0000c6e0: 642c 0a20 2020 2020 2020 2020 2020 2069  d,.            i
+0000c6f0: 643d 6964 2c0a 2020 2020 2020 2020 2020  d=id,.          
+0000c700: 2020 6578 7065 6374 6174 696f 6e5f 7375    expectation_su
+0000c710: 6974 653d 6578 7065 6374 6174 696f 6e5f  ite=expectation_
+0000c720: 7375 6974 652c 0a20 2020 2020 2020 2020  suite,.         
+0000c730: 2020 206f 6e6c 696e 655f 746f 7069 635f     online_topic_
+0000c740: 6e61 6d65 3d6f 6e6c 696e 655f 746f 7069  name=online_topi
+0000c750: 635f 6e61 6d65 2c0a 2020 2020 2020 2020  c_name,.        
+0000c760: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000c770: 5f66 6561 7475 7265 5f73 746f 7265 5f6e  _feature_store_n
+0000c780: 616d 6520 3d20 6665 6174 7572 6573 746f  ame = featuresto
+0000c790: 7265 5f6e 616d 650a 2020 2020 2020 2020  re_name.        
+0000c7a0: 7365 6c66 2e5f 6465 7363 7269 7074 696f  self._descriptio
+0000c7b0: 6e20 3d20 6465 7363 7269 7074 696f 6e0a  n = description.
+0000c7c0: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
+0000c7d0: 6561 7465 6420 3d20 6372 6561 7465 640a  eated = created.
+0000c7e0: 2020 2020 2020 2020 7365 6c66 2e5f 6372          self._cr
+0000c7f0: 6561 746f 7220 3d20 7573 6572 2e55 7365  eator = user.Use
+0000c800: 722e 6672 6f6d 5f72 6573 706f 6e73 655f  r.from_response_
+0000c810: 6a73 6f6e 2863 7265 6174 6f72 290a 2020  json(creator).  
+0000c820: 2020 2020 2020 7365 6c66 2e5f 7665 7273        self._vers
+0000c830: 696f 6e20 3d20 7665 7273 696f 6e0a 2020  ion = version.  
+0000c840: 2020 2020 2020 7365 6c66 2e5f 6e61 6d65        self._name
+0000c850: 203d 206e 616d 650a 2020 2020 2020 2020   = name.        
+0000c860: 7365 6c66 2e5f 6665 6174 7572 6573 203d  self._features =
+0000c870: 205b 0a20 2020 2020 2020 2020 2020 2066   [.            f
+0000c880: 6561 7475 7265 2e46 6561 7475 7265 2e66  eature.Feature.f
+0000c890: 726f 6d5f 7265 7370 6f6e 7365 5f6a 736f  rom_response_jso
+0000c8a0: 6e28 6665 6174 2920 6966 2069 7369 6e73  n(feat) if isins
+0000c8b0: 7461 6e63 6528 6665 6174 2c20 6469 6374  tance(feat, dict
+0000c8c0: 2920 656c 7365 2066 6561 740a 2020 2020  ) else feat.    
+0000c8d0: 2020 2020 2020 2020 666f 7220 6665 6174          for feat
+0000c8e0: 2069 6e20 2866 6561 7475 7265 7320 6f72   in (features or
+0000c8f0: 205b 5d29 0a20 2020 2020 2020 205d 0a0a   []).        ]..
+0000c900: 2020 2020 2020 2020 7365 6c66 2e5f 7469          self._ti
+0000c910: 6d65 5f74 7261 7665 6c5f 666f 726d 6174  me_travel_format
+0000c920: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+0000c930: 2074 696d 655f 7472 6176 656c 5f66 6f72   time_travel_for
+0000c940: 6d61 742e 7570 7065 7228 2920 6966 2074  mat.upper() if t
+0000c950: 696d 655f 7472 6176 656c 5f66 6f72 6d61  ime_travel_forma
+0000c960: 7420 6973 206e 6f74 204e 6f6e 6520 656c  t is not None el
+0000c970: 7365 204e 6f6e 650a 2020 2020 2020 2020  se None.        
+0000c980: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000c990: 5f73 7472 6561 6d20 3d20 7374 7265 616d  _stream = stream
+0000c9a0: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
+0000c9b0: 6172 656e 7473 203d 2070 6172 656e 7473  arents = parents
+0000c9c0: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
+0000c9d0: 656c 7461 7374 7265 616d 6572 5f6a 6f62  eltastreamer_job
+0000c9e0: 636f 6e66 203d 204e 6f6e 650a 0a20 2020  conf = None..   
+0000c9f0: 2020 2020 2073 656c 662e 5f62 6163 6b66       self._backf
+0000ca00: 696c 6c5f 6a6f 6220 3d20 4e6f 6e65 0a0a  ill_job = None..
+0000ca10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000ca20: 5f69 643a 0a20 2020 2020 2020 2020 2020  _id:.           
+0000ca30: 2023 2069 6e69 7469 616c 697a 6564 2062   # initialized b
+0000ca40: 7920 6261 636b 656e 640a 2020 2020 2020  y backend.      
+0000ca50: 2020 2020 2020 7365 6c66 2e70 7269 6d61        self.prima
+0000ca60: 7279 5f6b 6579 203d 205b 0a20 2020 2020  ry_key = [.     
+0000ca70: 2020 2020 2020 2020 2020 2066 6561 742e             feat.
+0000ca80: 6e61 6d65 2066 6f72 2066 6561 7420 696e  name for feat in
+0000ca90: 2073 656c 662e 5f66 6561 7475 7265 7320   self._features 
+0000caa0: 6966 2066 6561 742e 7072 696d 6172 7920  if feat.primary 
+0000cab0: 6973 2054 7275 650a 2020 2020 2020 2020  is True.        
+0000cac0: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+0000cad0: 2020 7365 6c66 2e5f 7061 7274 6974 696f    self._partitio
+0000cae0: 6e5f 6b65 7920 3d20 5b0a 2020 2020 2020  n_key = [.      
+0000caf0: 2020 2020 2020 2020 2020 6665 6174 2e6e            feat.n
+0000cb00: 616d 6520 666f 7220 6665 6174 2069 6e20  ame for feat in 
+0000cb10: 7365 6c66 2e5f 6665 6174 7572 6573 2069  self._features i
+0000cb20: 6620 6665 6174 2e70 6172 7469 7469 6f6e  f feat.partition
+0000cb30: 2069 7320 5472 7565 0a20 2020 2020 2020   is True.       
+0000cb40: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+0000cb50: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+0000cb60: 2020 2020 2020 2020 7469 6d65 5f74 7261          time_tra
+0000cb70: 7665 6c5f 666f 726d 6174 2069 7320 6e6f  vel_format is no
+0000cb80: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
+0000cb90: 2020 2020 2020 2061 6e64 2074 696d 655f         and time_
+0000cba0: 7472 6176 656c 5f66 6f72 6d61 742e 7570  travel_format.up
+0000cbb0: 7065 7228 2920 3d3d 2022 4855 4449 220a  per() == "HUDI".
+0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbd0: 616e 6420 7365 6c66 2e5f 6665 6174 7572  and self._featur
+0000cbe0: 6573 0a20 2020 2020 2020 2020 2020 2029  es.            )
+0000cbf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000cc00: 2020 2320 6875 6469 2070 7265 636f 6d62    # hudi precomb
+0000cc10: 696e 6520 6b65 7920 6973 2061 6c77 6179  ine key is alway
+0000cc20: 7320 6120 7369 6e67 6c65 2066 6561 7475  s a single featu
+0000cc30: 7265 0a20 2020 2020 2020 2020 2020 2020  re.             
+0000cc40: 2020 2073 656c 662e 5f68 7564 695f 7072     self._hudi_pr
+0000cc50: 6563 6f6d 6269 6e65 5f6b 6579 203d 205b  ecombine_key = [
+0000cc60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cc70: 2020 2020 2066 6561 742e 6e61 6d65 0a20       feat.name. 
+0000cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc90: 2020 2066 6f72 2066 6561 7420 696e 2073     for feat in s
+0000cca0: 656c 662e 5f66 6561 7475 7265 730a 2020  elf._features.  
+0000ccb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ccc0: 2020 6966 2066 6561 742e 6875 6469 5f70    if feat.hudi_p
+0000ccd0: 7265 636f 6d62 696e 655f 6b65 7920 6973  recombine_key is
+0000cce0: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+0000ccf0: 2020 2020 2020 5d5b 305d 0a20 2020 2020        ][0].     
+0000cd00: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000cd10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000cd20: 662e 5f68 7564 695f 7072 6563 6f6d 6269  f._hudi_precombi
+0000cd30: 6e65 5f6b 6579 203d 204e 6f6e 650a 0a20  ne_key = None.. 
+0000cd40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000cd50: 7374 6174 6973 7469 6373 5f63 6f6e 6669  statistics_confi
+0000cd60: 6720 3d20 7374 6174 6973 7469 6373 5f63  g = statistics_c
+0000cd70: 6f6e 6669 670a 0a20 2020 2020 2020 2065  onfig..        e
+0000cd80: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000cd90: 2023 2069 6e69 7469 616c 697a 6564 2062   # initialized b
+0000cda0: 7920 7573 6572 0a20 2020 2020 2020 2020  y user.         
+0000cdb0: 2020 2023 2066 6f72 2070 7974 686f 6e20     # for python 
+0000cdc0: 656e 6769 6e65 2077 6520 616c 7761 7973  engine we always
+0000cdd0: 2075 7365 2073 7472 6561 6d20 6665 6174   use stream feat
+0000cde0: 7572 6520 6772 6f75 700a 2020 2020 2020  ure group.      
+0000cdf0: 2020 2020 2020 6966 2065 6e67 696e 652e        if engine.
+0000ce00: 6765 745f 7479 7065 2829 203d 3d20 2270  get_type() == "p
+0000ce10: 7974 686f 6e22 3a0a 2020 2020 2020 2020  ython":.        
+0000ce20: 2020 2020 2020 2020 7365 6c66 2e5f 7374          self._st
+0000ce30: 7265 616d 203d 2054 7275 650a 2020 2020  ream = True.    
+0000ce40: 2020 2020 2020 2020 2320 666f 7220 7374          # for st
+0000ce50: 7265 616d 2066 6561 7475 7265 2067 726f  ream feature gro
+0000ce60: 7570 2074 696d 6520 7472 6176 656c 2066  up time travel f
+0000ce70: 6f72 6d61 7420 6973 2061 6c77 6179 7320  ormat is always 
+0000ce80: 4855 4449 0a20 2020 2020 2020 2020 2020  HUDI.           
+0000ce90: 2069 6620 7365 6c66 2e5f 7374 7265 616d   if self._stream
+0000cea0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ceb0: 2020 6578 7065 6374 6564 5f66 6f72 6d61    expected_forma
+0000cec0: 7420 3d20 2248 5544 4922 0a20 2020 2020  t = "HUDI".     
+0000ced0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000cee0: 6c66 2e5f 7469 6d65 5f74 7261 7665 6c5f  lf._time_travel_
+0000cef0: 666f 726d 6174 2021 3d20 6578 7065 6374  format != expect
+0000cf00: 6564 5f66 6f72 6d61 743a 0a20 2020 2020  ed_format:.     
+0000cf10: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000cf20: 6172 6e69 6e67 732e 7761 726e 280a 2020  arnings.warn(.  
+0000cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf40: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+0000cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf60: 2020 2020 2254 6865 2070 726f 7669 6465      "The provide
+0000cf70: 6420 7469 6d65 2074 7261 7665 6c20 666f  d time travel fo
+0000cf80: 726d 6174 2060 7b7d 6020 6861 7320 6265  rmat `{}` has be
+0000cf90: 656e 206f 7665 7277 7269 7474 656e 2022  en overwritten "
+0000cfa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cfb0: 2020 2020 2020 2020 2020 2020 2022 6265               "be
+0000cfc0: 6361 7573 6520 5374 7265 616d 2065 6e61  cause Stream ena
+0000cfd0: 626c 6564 2066 6561 7475 7265 2067 726f  bled feature gro
+0000cfe0: 7570 7320 6f6e 6c79 2073 7570 706f 7274  ups only support
+0000cff0: 2060 7b7d 6022 0a20 2020 2020 2020 2020   `{}`".         
+0000d000: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000d010: 2e66 6f72 6d61 7428 7365 6c66 2e5f 7469  .format(self._ti
+0000d020: 6d65 5f74 7261 7665 6c5f 666f 726d 6174  me_travel_format
+0000d030: 2c20 6578 7065 6374 6564 5f66 6f72 6d61  , expected_forma
+0000d040: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
+0000d050: 2020 2020 2020 2020 2020 2020 7574 696c              util
+0000d060: 2e46 6561 7475 7265 4772 6f75 7057 6172  .FeatureGroupWar
+0000d070: 6e69 6e67 2c0a 2020 2020 2020 2020 2020  ning,.          
+0000d080: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0a0: 7365 6c66 2e5f 7469 6d65 5f74 7261 7665  self._time_trave
+0000d0b0: 6c5f 666f 726d 6174 203d 2065 7870 6563  l_format = expec
+0000d0c0: 7465 645f 666f 726d 6174 0a0a 2020 2020  ted_format..    
+0000d0d0: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
+0000d0e0: 6d61 7279 5f6b 6579 203d 2070 7269 6d61  mary_key = prima
+0000d0f0: 7279 5f6b 6579 0a20 2020 2020 2020 2020  ry_key.         
+0000d100: 2020 2073 656c 662e 7061 7274 6974 696f     self.partitio
+0000d110: 6e5f 6b65 7920 3d20 7061 7274 6974 696f  n_key = partitio
+0000d120: 6e5f 6b65 790a 2020 2020 2020 2020 2020  n_key.          
+0000d130: 2020 7365 6c66 2e5f 6875 6469 5f70 7265    self._hudi_pre
+0000d140: 636f 6d62 696e 655f 6b65 7920 3d20 280a  combine_key = (.
+0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d160: 6875 6469 5f70 7265 636f 6d62 696e 655f  hudi_precombine_
+0000d170: 6b65 792e 6c6f 7765 7228 290a 2020 2020  key.lower().    
+0000d180: 2020 2020 2020 2020 2020 2020 6966 2068              if h
+0000d190: 7564 695f 7072 6563 6f6d 6269 6e65 5f6b  udi_precombine_k
+0000d1a0: 6579 2069 7320 6e6f 7420 4e6f 6e65 0a20  ey is not None. 
+0000d1b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000d1c0: 6e64 2073 656c 662e 5f74 696d 655f 7472  nd self._time_tr
+0000d1d0: 6176 656c 5f66 6f72 6d61 7420 6973 206e  avel_format is n
+0000d1e0: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+0000d1f0: 2020 2020 2020 2020 616e 6420 7365 6c66          and self
+0000d200: 2e5f 7469 6d65 5f74 7261 7665 6c5f 666f  ._time_travel_fo
+0000d210: 726d 6174 203d 3d20 2248 5544 4922 0a20  rmat == "HUDI". 
+0000d220: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000d230: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
+0000d240: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000d250: 2020 2073 656c 662e 7374 6174 6973 7469     self.statisti
+0000d260: 6373 5f63 6f6e 6669 6720 3d20 7374 6174  cs_config = stat
+0000d270: 6973 7469 6373 5f63 6f6e 6669 670a 0a20  istics_config.. 
+0000d280: 2020 2020 2020 2073 656c 662e 5f66 6561         self._fea
+0000d290: 7475 7265 5f67 726f 7570 5f65 6e67 696e  ture_group_engin
+0000d2a0: 6520 3d20 6665 6174 7572 655f 6772 6f75  e = feature_grou
+0000d2b0: 705f 656e 6769 6e65 2e46 6561 7475 7265  p_engine.Feature
+0000d2c0: 4772 6f75 7045 6e67 696e 6528 0a20 2020  GroupEngine(.   
+0000d2d0: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+0000d2e0: 7374 6f72 655f 6964 0a20 2020 2020 2020  store_id.       
+0000d2f0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+0000d300: 5f68 7265 6620 3d20 6872 6566 0a0a 2020  _href = href..  
+0000d310: 2020 2020 2020 2320 6361 6368 6520 666f        # cache fo
+0000d320: 7220 6f70 7469 6d69 7a65 6420 7772 6974  r optimized writ
+0000d330: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
+0000d340: 5f6b 6166 6b61 5f70 726f 6475 6365 7220  _kafka_producer 
+0000d350: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+0000d360: 656c 662e 5f66 6561 7475 7265 5f77 7269  elf._feature_wri
+0000d370: 7465 7273 203d 204e 6f6e 650a 2020 2020  ters = None.    
+0000d380: 2020 2020 7365 6c66 2e5f 7772 6974 6572      self._writer
+0000d390: 203d 204e 6f6e 650a 0a20 2020 2064 6566   = None..    def
+0000d3a0: 2072 6561 6428 0a20 2020 2020 2020 2073   read(.        s
+0000d3b0: 656c 662c 0a20 2020 2020 2020 2077 616c  elf,.        wal
+0000d3c0: 6c63 6c6f 636b 5f74 696d 653a 204f 7074  lclock_time: Opt
+0000d3d0: 696f 6e61 6c5b 556e 696f 6e5b 7374 722c  ional[Union[str,
+0000d3e0: 2069 6e74 2c20 6461 7465 7469 6d65 2c20   int, datetime, 
+0000d3f0: 6461 7465 5d5d 203d 204e 6f6e 652c 0a20  date]] = None,. 
+0000d400: 2020 2020 2020 206f 6e6c 696e 653a 204f         online: O
+0000d410: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+0000d420: 4661 6c73 652c 0a20 2020 2020 2020 2064  False,.        d
+0000d430: 6174 6166 7261 6d65 5f74 7970 653a 204f  ataframe_type: O
+0000d440: 7074 696f 6e61 6c5b 7374 725d 203d 2022  ptional[str] = "
+0000d450: 6465 6661 756c 7422 2c0a 2020 2020 2020  default",.      
+0000d460: 2020 7265 6164 5f6f 7074 696f 6e73 3a20    read_options: 
+0000d470: 4f70 7469 6f6e 616c 5b64 6963 745d 203d  Optional[dict] =
+0000d480: 207b 7d2c 0a20 2020 2029 3a0a 2020 2020   {},.    ):.    
+0000d490: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000d4a0: 5265 6164 2074 6865 2066 6561 7475 7265  Read the feature
+0000d4b0: 2067 726f 7570 2069 6e74 6f20 6120 6461   group into a da
+0000d4c0: 7461 6672 616d 652e 0a0a 2020 2020 2020  taframe...      
+0000d4d0: 2020 5265 6164 7320 7468 6520 6665 6174    Reads the feat
+0000d4e0: 7572 6520 6772 6f75 7020 6279 2064 6566  ure group by def
+0000d4f0: 6175 6c74 2066 726f 6d20 7468 6520 6f66  ault from the of
+0000d500: 666c 696e 6520 7374 6f72 6167 6520 6173  fline storage as
+0000d510: 2053 7061 726b 2044 6174 6146 7261 6d65   Spark DataFrame
+0000d520: 0a20 2020 2020 2020 206f 6e20 486f 7073  .        on Hops
+0000d530: 776f 726b 7320 616e 6420 4461 7461 6272  works and Databr
+0000d540: 6963 6b73 2c20 616e 6420 6173 2050 616e  icks, and as Pan
+0000d550: 6461 7320 6461 7461 6672 616d 6520 6f6e  das dataframe on
+0000d560: 2041 5753 2053 6167 656d 616b 6572 2061   AWS Sagemaker a
+0000d570: 6e64 2070 7572 650a 2020 2020 2020 2020  nd pure.        
+0000d580: 5079 7468 6f6e 2065 6e76 6972 6f6e 6d65  Python environme
+0000d590: 6e74 732e 0a0a 2020 2020 2020 2020 5365  nts...        Se
+0000d5a0: 7420 606f 6e6c 696e 6560 2074 6f20 6054  t `online` to `T
+0000d5b0: 7275 6560 2074 6f20 7265 6164 2066 726f  rue` to read fro
+0000d5c0: 6d20 7468 6520 6f6e 6c69 6e65 2073 746f  m the online sto
+0000d5d0: 7261 6765 2c20 6f72 2063 6861 6e67 650a  rage, or change.
+0000d5e0: 2020 2020 2020 2020 6064 6174 6166 7261          `datafra
+0000d5f0: 6d65 5f74 7970 6560 2074 6f20 7265 6164  me_type` to read
+0000d600: 2061 7320 6120 6469 6666 6572 656e 7420   as a different 
+0000d610: 666f 726d 6174 2e0a 0a20 2020 2020 2020  format...       
+0000d620: 2021 2121 2065 7861 6d70 6c65 2022 5265   !!! example "Re
+0000d630: 6164 2066 6561 7475 7265 2067 726f 7570  ad feature group
+0000d640: 2061 7320 6f66 206c 6174 6573 7420 7374   as of latest st
+0000d650: 6174 653a 220a 2020 2020 2020 2020 2020  ate:".          
+0000d660: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
+0000d670: 2020 2020 2020 2020 2320 636f 6e6e 6563          # connec
+0000d680: 7420 746f 2074 6865 2046 6561 7475 7265  t to the Feature
+0000d690: 2053 746f 7265 0a20 2020 2020 2020 2020   Store.         
+0000d6a0: 2020 2066 7320 3d20 2e2e 2e0a 0a20 2020     fs = .....   
+0000d6b0: 2020 2020 2020 2020 2023 2067 6574 2074           # get t
+0000d6c0: 6865 2046 6561 7475 7265 2047 726f 7570  he Feature Group
+0000d6d0: 2069 6e73 7461 6e63 650a 2020 2020 2020   instance.      
+0000d6e0: 2020 2020 2020 6667 203d 2066 732e 6765        fg = fs.ge
+0000d6f0: 745f 6f72 5f63 7265 6174 655f 6665 6174  t_or_create_feat
+0000d700: 7572 655f 6772 6f75 7028 2e2e 2e29 0a20  ure_group(...). 
+0000d710: 2020 2020 2020 2020 2020 2066 672e 7265             fg.re
+0000d720: 6164 2829 0a20 2020 2020 2020 2020 2020  ad().           
+0000d730: 2060 6060 0a0a 2020 2020 2020 2020 2121   ```..        !!
+0000d740: 2120 6578 616d 706c 6520 2252 6561 6420  ! example "Read 
+0000d750: 6665 6174 7572 6520 6772 6f75 7020 6173  feature group as
+0000d760: 206f 6620 7370 6563 6966 6963 2070 6f69   of specific poi
+0000d770: 6e74 2069 6e20 7469 6d65 3a22 0a20 2020  nt in time:".   
+0000d780: 2020 2020 2020 2020 2060 6060 7079 7468           ```pyth
+0000d790: 6f6e 0a20 2020 2020 2020 2020 2020 2066  on.            f
+0000d7a0: 6720 3d20 6673 2e67 6574 5f6f 725f 6372  g = fs.get_or_cr
+0000d7b0: 6561 7465 5f66 6561 7475 7265 5f67 726f  eate_feature_gro
+0000d7c0: 7570 282e 2e2e 290a 2020 2020 2020 2020  up(...).        
+0000d7d0: 2020 2020 6667 2e72 6561 6428 2232 3032      fg.read("202
+0000d7e0: 302d 3130 2d32 3020 3037 3a33 343a 3131  0-10-20 07:34:11
+0000d7f0: 2229 0a20 2020 2020 2020 2020 2020 2060  ").            `
+0000d800: 6060 0a0a 2020 2020 2020 2020 2320 4172  ``..        # Ar
+0000d810: 6775 6d65 6e74 730a 2020 2020 2020 2020  guments.        
+0000d820: 2020 2020 7761 6c6c 636c 6f63 6b5f 7469      wallclock_ti
+0000d830: 6d65 3a20 4966 2073 7065 6369 6669 6564  me: If specified
+0000d840: 2077 696c 6c20 7265 7472 6965 7665 2066   will retrieve f
+0000d850: 6561 7475 7265 2067 726f 7570 2061 7320  eature group as 
+0000d860: 6f66 2073 7065 6369 6669 6320 706f 696e  of specific poin
+0000d870: 7420 696e 2074 696d 652e 2044 6566 6175  t in time. Defau
+0000d880: 6c74 7320 746f 2060 4e6f 6e65 602e 0a20  lts to `None`.. 
+0000d890: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+0000d8a0: 6620 6e6f 7420 7370 6563 6966 6965 642c  f not specified,
+0000d8b0: 2077 696c 6c20 7265 7475 726e 2061 7320   will return as 
+0000d8c0: 6f66 206d 6f73 7420 7265 6365 6e74 2074  of most recent t
+0000d8d0: 696d 652e 0a20 2020 2020 2020 2020 2020  ime..           
+0000d8e0: 2020 2020 2053 7472 696e 6773 2073 686f       Strings sho
+0000d8f0: 756c 6420 6265 2066 6f72 6d61 7474 6564  uld be formatted
+0000d900: 2069 6e20 6f6e 6520 6f66 2074 6865 2066   in one of the f
+0000d910: 6f6c 6c6f 7769 6e67 2066 6f72 6d61 7473  ollowing formats
+0000d920: 2060 2559 2d25 6d2d 2564 602c 2060 2559   `%Y-%m-%d`, `%Y
+0000d930: 2d25 6d2d 2564 2025 4860 2c20 6025 592d  -%m-%d %H`, `%Y-
+0000d940: 256d 2d25 6420 2548 3a25 4d60 2c20 6025  %m-%d %H:%M`, `%
+0000d950: 592d 256d 2d25 6420 2548 3a25 4d3a 2553  Y-%m-%d %H:%M:%S
+0000d960: 602c 0a20 2020 2020 2020 2020 2020 2020  `,.             
+0000d970: 2020 206f 7220 6025 592d 256d 2d25 6420     or `%Y-%m-%d 
+0000d980: 2548 3a25 4d3a 2553 2e25 6660 2e0a 2020  %H:%M:%S.%f`..  
+0000d990: 2020 2020 2020 2020 2020 6f6e 6c69 6e65            online
+0000d9a0: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+0000d9b0: 2e20 4966 2060 5472 7565 6020 7265 6164  . If `True` read
+0000d9c0: 2066 726f 6d20 6f6e 6c69 6e65 2066 6561   from online fea
+0000d9d0: 7475 7265 2073 746f 7265 2c20 6465 6661  ture store, defa
+0000d9e0: 756c 7473 0a20 2020 2020 2020 2020 2020  ults.           
+0000d9f0: 2020 2020 2074 6f20 6046 616c 7365 602e       to `False`.
+0000da00: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000da10: 6166 7261 6d65 5f74 7970 653a 2073 7472  aframe_type: str
+0000da20: 2c20 6f70 7469 6f6e 616c 2e20 506f 7373  , optional. Poss
+0000da30: 6962 6c65 2076 616c 7565 7320 6172 6520  ible values are 
+0000da40: 6022 6465 6661 756c 7422 602c 2060 2273  `"default"`, `"s
+0000da50: 7061 726b 2260 2c0a 2020 2020 2020 2020  park"`,.        
+0000da60: 2020 2020 2020 2020 6022 7061 6e64 6173          `"pandas
+0000da70: 2260 2c20 6022 6e75 6d70 7922 6020 6f72  "`, `"numpy"` or
+0000da80: 2060 2270 7974 686f 6e22 602c 2064 6566   `"python"`, def
+0000da90: 6175 6c74 7320 746f 2060 2264 6566 6175  aults to `"defau
+0000daa0: 6c74 2260 2e0a 2020 2020 2020 2020 2020  lt"`..          
+0000dab0: 2020 7265 6164 5f6f 7074 696f 6e73 3a20    read_options: 
+0000dac0: 4164 6469 7469 6f6e 616c 206f 7074 696f  Additional optio
+0000dad0: 6e73 2061 7320 6b65 792f 7661 6c75 6520  ns as key/value 
+0000dae0: 7061 6972 7320 746f 2070 6173 7320 746f  pairs to pass to
+0000daf0: 2074 6865 2065 7865 6375 7469 6f6e 2065   the execution e
+0000db00: 6e67 696e 652e 0a20 2020 2020 2020 2020  ngine..         
+0000db10: 2020 2020 2020 2046 6f72 2073 7061 726b         For spark
+0000db20: 2065 6e67 696e 653a 2044 6963 7469 6f6e   engine: Diction
+0000db30: 6172 7920 6f66 2072 6561 6420 6f70 7469  ary of read opti
+0000db40: 6f6e 7320 666f 7220 5370 6172 6b2e 0a20  ons for Spark.. 
+0000db50: 2020 2020 2020 2020 2020 2020 2020 2046                 F
+0000db60: 6f72 2070 7974 686f 6e20 656e 6769 6e65  or python engine
+0000db70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000db80: 2020 2a20 6b65 7920 6022 6869 7665 5f63    * key `"hive_c
+0000db90: 6f6e 6669 6722 6020 746f 2070 6173 7320  onfig"` to pass 
+0000dba0: 6120 6469 6374 696f 6e61 7279 206f 6620  a dictionary of 
+0000dbb0: 6869 7665 206f 7220 7465 7a20 636f 6e66  hive or tez conf
+0000dbc0: 6967 7572 6174 696f 6e73 2e0a 2020 2020  igurations..    
+0000dbd0: 2020 2020 2020 2020 2020 2020 2020 466f                Fo
+0000dbe0: 7220 6578 616d 706c 653a 2060 7b22 6869  r example: `{"hi
+0000dbf0: 7665 5f63 6f6e 6669 6722 3a20 7b22 6869  ve_config": {"hi
+0000dc00: 7665 2e74 657a 2e63 7075 2e76 636f 7265  ve.tez.cpu.vcore
+0000dc10: 7322 3a20 322c 2022 7465 7a2e 6772 6f75  s": 2, "tez.grou
+0000dc20: 7069 6e67 2e73 706c 6974 2d63 6f75 6e74  ping.split-count
+0000dc30: 223a 2022 3322 7d7d 600a 2020 2020 2020  ": "3"}}`.      
+0000dc40: 2020 2020 2020 2020 2020 2a20 6b65 7920            * key 
+0000dc50: 6022 7061 6e64 6173 5f74 7970 6573 2260  `"pandas_types"`
+0000dc60: 2061 6e64 2076 616c 7565 2060 5472 7565   and value `True
+0000dc70: 6020 746f 2072 6574 7269 6576 6520 636f  ` to retrieve co
+0000dc80: 6c75 6d6e 7320 6173 2050 616e 6461 7320  lumns as Pandas 
+0000dc90: 6e75 6c6c 6162 6c65 2074 7970 6573 0a20  nullable types. 
+0000dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcb0: 2072 6174 6865 7220 7468 616e 206e 756d   rather than num
+0000dcc0: 7079 2f6f 626a 6563 7428 7374 7269 6e67  py/object(string
+0000dcd0: 2920 7479 7065 7320 2865 7870 6572 696d  ) types (experim
+0000dce0: 656e 7461 6c29 2e0a 2020 2020 2020 2020  ental)..        
+0000dcf0: 2020 2020 2020 2020 2020 2873 6565 2068            (see h
+0000dd00: 7474 7073 3a2f 2f70 616e 6461 732e 7079  ttps://pandas.py
+0000dd10: 6461 7461 2e6f 7267 2f64 6f63 732f 7573  data.org/docs/us
+0000dd20: 6572 5f67 7569 6465 2f69 6e74 6567 6572  er_guide/integer
+0000dd30: 5f6e 612e 6874 6d6c 292e 0a20 2020 2020  _na.html)..     
+0000dd40: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+0000dd50: 6c74 7320 746f 2060 7b7d 602e 0a0a 2020  lts to `{}`...  
+0000dd60: 2020 2020 2020 2320 5265 7475 726e 730a        # Returns.
+0000dd70: 2020 2020 2020 2020 2020 2020 6044 6174              `Dat
+0000dd80: 6146 7261 6d65 603a 2054 6865 2073 7061  aFrame`: The spa
+0000dd90: 726b 2064 6174 6166 7261 6d65 2063 6f6e  rk dataframe con
+0000dda0: 7461 696e 696e 6720 7468 6520 6665 6174  taining the feat
+0000ddb0: 7572 6520 6461 7461 2e0a 2020 2020 2020  ure data..      
+0000ddc0: 2020 2020 2020 6070 7973 7061 726b 2e44        `pyspark.D
+0000ddd0: 6174 6146 7261 6d65 602e 2041 2053 7061  ataFrame`. A Spa
+0000dde0: 726b 2044 6174 6146 7261 6d65 2e0a 2020  rk DataFrame..  
+0000ddf0: 2020 2020 2020 2020 2020 6070 616e 6461            `panda
+0000de00: 732e 4461 7461 4672 616d 6560 2e20 4120  s.DataFrame`. A 
+0000de10: 5061 6e64 6173 2044 6174 6146 7261 6d65  Pandas DataFrame
+0000de20: 2e0a 2020 2020 2020 2020 2020 2020 606e  ..            `n
+0000de30: 756d 7079 2e6e 6461 7272 6179 602e 2041  umpy.ndarray`. A
+0000de40: 2074 776f 2d64 696d 656e 7369 6f6e 616c   two-dimensional
+0000de50: 204e 756d 7079 2061 7272 6179 2e0a 2020   Numpy array..  
+0000de60: 2020 2020 2020 2020 2020 606c 6973 7460            `list`
+0000de70: 2e20 4120 7477 6f2d 6469 6d65 6e73 696f  . A two-dimensio
+0000de80: 6e61 6c20 5079 7468 6f6e 206c 6973 742e  nal Python list.
+0000de90: 0a0a 2020 2020 2020 2020 2320 5261 6973  ..        # Rais
+0000dea0: 6573 0a20 2020 2020 2020 2020 2020 2060  es.            `
+0000deb0: 6873 6673 2e63 6c69 656e 742e 6578 6365  hsfs.client.exce
+0000dec0: 7074 696f 6e73 2e52 6573 7441 5049 4572  ptions.RestAPIEr
+0000ded0: 726f 7260 2e20 4e6f 2064 6174 6120 6973  ror`. No data is
+0000dee0: 2061 7661 696c 6162 6c65 2066 6f72 2066   available for f
+0000def0: 6561 7475 7265 2067 726f 7570 2077 6974  eature group wit
+0000df00: 6820 7468 6973 2063 6f6d 6d69 7420 6461  h this commit da
+0000df10: 7465 2c20 4966 2074 696d 6520 7472 6176  te, If time trav
+0000df20: 656c 2065 6e61 626c 6564 2e0a 2020 2020  el enabled..    
+0000df30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000df40: 656e 6769 6e65 2e67 6574 5f69 6e73 7461  engine.get_insta
+0000df50: 6e63 6528 292e 7365 745f 6a6f 625f 6772  nce().set_job_gr
+0000df60: 6f75 7028 0a20 2020 2020 2020 2020 2020  oup(.           
+0000df70: 2022 4665 7463 6869 6e67 2046 6561 7475   "Fetching Featu
+0000df80: 7265 2067 726f 7570 222c 0a20 2020 2020  re group",.     
+0000df90: 2020 2020 2020 2022 4765 7474 696e 6720         "Getting 
+0000dfa0: 6665 6174 7572 6520 6772 6f75 703a 207b  feature group: {
+0000dfb0: 7d20 6672 6f6d 2074 6865 2066 6561 7475  } from the featu
+0000dfc0: 7265 7374 6f72 6520 7b7d 222e 666f 726d  restore {}".form
+0000dfd0: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+0000dfe0: 2020 2020 7365 6c66 2e5f 6e61 6d65 2c20      self._name, 
+0000dff0: 7365 6c66 2e5f 6665 6174 7572 655f 7374  self._feature_st
+0000e000: 6f72 655f 6e61 6d65 0a20 2020 2020 2020  ore_name.       
+0000e010: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+0000e020: 290a 2020 2020 2020 2020 6966 2077 616c  ).        if wal
+0000e030: 6c63 6c6f 636b 5f74 696d 653a 0a20 2020  lclock_time:.   
+0000e040: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000e050: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000e060: 2020 7365 6c66 2e73 656c 6563 745f 616c    self.select_al
+0000e070: 6c28 290a 2020 2020 2020 2020 2020 2020  l().            
+0000e080: 2020 2020 2e61 735f 6f66 2877 616c 6c63      .as_of(wallc
+0000e090: 6c6f 636b 5f74 696d 6529 0a20 2020 2020  lock_time).     
+0000e0a0: 2020 2020 2020 2020 2020 202e 7265 6164             .read
+0000e0b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000e0c0: 2020 2020 2020 6f6e 6c69 6e65 2c0a 2020        online,.  
+0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0e0: 2020 6461 7461 6672 616d 655f 7479 7065    dataframe_type
+0000e0f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e100: 2020 2020 2020 7265 6164 5f6f 7074 696f        read_optio
+0000e110: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+0000e120: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000e130: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
+0000e140: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000e150: 7475 726e 2073 656c 662e 7365 6c65 6374  turn self.select
+0000e160: 5f61 6c6c 2829 2e72 6561 6428 0a20 2020  _all().read(.   
+0000e170: 2020 2020 2020 2020 2020 2020 206f 6e6c               onl
+0000e180: 696e 652c 0a20 2020 2020 2020 2020 2020  ine,.           
+0000e190: 2020 2020 2064 6174 6166 7261 6d65 5f74       dataframe_t
+0000e1a0: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
+0000e1b0: 2020 2020 2072 6561 645f 6f70 7469 6f6e       read_option
+0000e1c0: 732c 0a20 2020 2020 2020 2020 2020 2029  s,.            )
+0000e1d0: 0a0a 2020 2020 6465 6620 7265 6164 5f63  ..    def read_c
+0000e1e0: 6861 6e67 6573 280a 2020 2020 2020 2020  hanges(.        
+0000e1f0: 7365 6c66 2c0a 2020 2020 2020 2020 7374  self,.        st
+0000e200: 6172 745f 7761 6c6c 636c 6f63 6b5f 7469  art_wallclock_ti
+0000e210: 6d65 3a20 556e 696f 6e5b 7374 722c 2069  me: Union[str, i
+0000e220: 6e74 2c20 6461 7465 7469 6d65 2c20 6461  nt, datetime, da
+0000e230: 7465 5d2c 0a20 2020 2020 2020 2065 6e64  te],.        end
+0000e240: 5f77 616c 6c63 6c6f 636b 5f74 696d 653a  _wallclock_time:
+0000e250: 2055 6e69 6f6e 5b73 7472 2c20 696e 742c   Union[str, int,
+0000e260: 2064 6174 6574 696d 652c 2064 6174 655d   datetime, date]
+0000e270: 2c0a 2020 2020 2020 2020 7265 6164 5f6f  ,.        read_o
+0000e280: 7074 696f 6e73 3a20 4f70 7469 6f6e 616c  ptions: Optional
+0000e290: 5b64 6963 745d 203d 207b 7d2c 0a20 2020  [dict] = {},.   
+0000e2a0: 2029 3a0a 2020 2020 2020 2020 2222 2252   ):.        """R
+0000e2b0: 6561 6473 2075 7064 6174 6573 206f 6620  eads updates of 
+0000e2c0: 7468 6973 2066 6561 7475 7265 2074 6861  this feature tha
+0000e2d0: 7420 6f63 6375 7272 6564 2062 6574 7765  t occurred betwe
+0000e2e0: 656e 2073 7065 6369 6669 6564 2070 6f69  en specified poi
+0000e2f0: 6e74 7320 696e 2074 696d 652e 0a0a 2020  nts in time...  
+0000e300: 2020 2020 2020 2121 2120 7761 726e 696e        !!! warnin
+0000e310: 6720 2244 6570 7265 6361 7465 6422 0a20  g "Deprecated". 
+0000e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e330: 2020 2060 7265 6164 5f63 6861 6e67 6573     `read_changes
+0000e340: 6020 6d65 7468 6f64 2069 7320 6465 7072  ` method is depr
+0000e350: 6563 6174 6564 2e20 5573 650a 2020 2020  ecated. Use.    
+0000e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e370: 6061 735f 6f66 2865 6e64 5f77 616c 6c63  `as_of(end_wallc
+0000e380: 6c6f 636b 5f74 696d 652c 2065 7863 6c75  lock_time, exclu
+0000e390: 6465 5f75 6e74 696c 3d73 7461 7274 5f77  de_until=start_w
+0000e3a0: 616c 6c63 6c6f 636b 5f74 696d 6529 2e72  allclock_time).r
+0000e3b0: 6561 6428 7265 6164 5f6f 7074 696f 6e73  ead(read_options
+0000e3c0: 3d72 6561 645f 6f70 7469 6f6e 7329 600a  =read_options)`.
+0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3e0: 2020 2020 696e 7374 6561 642e 0a0a 2020      instead...  
+0000e3f0: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
+0000e400: 696f 6e20 6f6e 6c79 2077 6f72 6b73 206f  ion only works o
+0000e410: 6e20 6665 6174 7572 6520 6772 6f75 7073  n feature groups
+0000e420: 2077 6974 6820 6048 5544 4960 2074 696d   with `HUDI` tim
+0000e430: 6520 7472 6176 656c 2066 6f72 6d61 742e  e travel format.
+0000e440: 0a0a 2020 2020 2020 2020 2320 4172 6775  ..        # Argu
+0000e450: 6d65 6e74 730a 2020 2020 2020 2020 2020  ments.          
+0000e460: 2020 7374 6172 745f 7761 6c6c 636c 6f63    start_wallcloc
+0000e470: 6b5f 7469 6d65 3a20 5374 6172 7420 7469  k_time: Start ti
+0000e480: 6d65 206f 6620 7468 6520 7469 6d65 2074  me of the time t
+0000e490: 7261 7665 6c20 7175 6572 792e 2053 7472  ravel query. Str
+0000e4a0: 696e 6773 2073 686f 756c 6420 6265 2066  ings should be f
+0000e4b0: 6f72 6d61 7474 6564 2069 6e20 6f6e 6520  ormatted in one 
+0000e4c0: 6f66 2074 6865 2066 6f6c 6c6f 7769 6e67  of the following
+0000e4d0: 2066 6f72 6d61 7473 2060 2559 2d25 6d2d   formats `%Y-%m-
+0000e4e0: 2564 602c 2060 2559 2d25 6d2d 2564 2025  %d`, `%Y-%m-%d %
+0000e4f0: 4860 2c20 6025 592d 256d 2d25 6420 2548  H`, `%Y-%m-%d %H
+0000e500: 3a25 4d60 2c0a 2020 2020 2020 2020 2020  :%M`,.          
+0000e510: 2020 2020 2020 6025 592d 256d 2d25 6420        `%Y-%m-%d 
+0000e520: 2548 3a25 4d3a 2553 602c 206f 7220 6025  %H:%M:%S`, or `%
+0000e530: 592d 256d 2d25 6420 2548 3a25 4d3a 2553  Y-%m-%d %H:%M:%S
+0000e540: 2e25 6660 2e0a 2020 2020 2020 2020 2020  .%f`..          
+0000e550: 2020 656e 645f 7761 6c6c 636c 6f63 6b5f    end_wallclock_
+0000e560: 7469 6d65 3a20 456e 6420 7469 6d65 206f  time: End time o
+0000e570: 6620 7468 6520 7469 6d65 2074 7261 7665  f the time trave
+0000e580: 6c20 7175 6572 792e 2053 7472 696e 6773  l query. Strings
+0000e590: 2073 686f 756c 6420 6265 2066 6f72 6d61   should be forma
+0000e5a0: 7474 6564 2069 6e20 6f6e 6520 6f66 2074  tted in one of t
+0000e5b0: 6865 2066 6f6c 6c6f 7769 6e67 2066 6f72  he following for
+0000e5c0: 6d61 7473 2060 2559 2d25 6d2d 2564 602c  mats `%Y-%m-%d`,
+0000e5d0: 2060 2559 2d25 6d2d 2564 2025 4860 2c20   `%Y-%m-%d %H`, 
+0000e5e0: 6025 592d 256d 2d25 6420 2548 3a25 4d60  `%Y-%m-%d %H:%M`
+0000e5f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e600: 2020 6025 592d 256d 2d25 6420 2548 3a25    `%Y-%m-%d %H:%
+0000e610: 4d3a 2553 602c 206f 7220 6025 592d 256d  M:%S`, or `%Y-%m
+0000e620: 2d25 6420 2548 3a25 4d3a 2553 2e25 6660  -%d %H:%M:%S.%f`
+0000e630: 2e0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000e640: 6164 5f6f 7074 696f 6e73 3a20 4164 6469  ad_options: Addi
+0000e650: 7469 6f6e 616c 206f 7074 696f 6e73 2061  tional options a
+0000e660: 7320 6b65 792f 7661 6c75 6520 7061 6972  s key/value pair
+0000e670: 7320 746f 2070 6173 7320 746f 2074 6865  s to pass to the
+0000e680: 2065 7865 6375 7469 6f6e 2065 6e67 696e   execution engin
+0000e690: 652e 0a20 2020 2020 2020 2020 2020 2020  e..             
+0000e6a0: 2020 2046 6f72 2073 7061 726b 2065 6e67     For spark eng
+0000e6b0: 696e 653a 2044 6963 7469 6f6e 6172 7920  ine: Dictionary 
+0000e6c0: 6f66 2072 6561 6420 6f70 7469 6f6e 7320  of read options 
+0000e6d0: 666f 7220 5370 6172 6b2e 0a20 2020 2020  for Spark..     
+0000e6e0: 2020 2020 2020 2020 2020 2046 6f72 2070             For p
+0000e6f0: 7974 686f 6e20 656e 6769 6e65 3a0a 2020  ython engine:.  
+0000e700: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+0000e710: 6b65 7920 6022 6869 7665 5f63 6f6e 6669  key `"hive_confi
+0000e720: 6722 6020 746f 2070 6173 7320 6120 6469  g"` to pass a di
+0000e730: 6374 696f 6e61 7279 206f 6620 6869 7665  ctionary of hive
+0000e740: 206f 7220 7465 7a20 636f 6e66 6967 7572   or tez configur
+0000e750: 6174 696f 6e73 2e0a 2020 2020 2020 2020  ations..        
+0000e760: 2020 2020 2020 2020 2020 466f 7220 6578            For ex
+0000e770: 616d 706c 653a 2060 7b22 6869 7665 5f63  ample: `{"hive_c
+0000e780: 6f6e 6669 6722 3a20 7b22 6869 7665 2e74  onfig": {"hive.t
+0000e790: 657a 2e63 7075 2e76 636f 7265 7322 3a20  ez.cpu.vcores": 
+0000e7a0: 322c 2022 7465 7a2e 6772 6f75 7069 6e67  2, "tez.grouping
+0000e7b0: 2e73 706c 6974 2d63 6f75 6e74 223a 2022  .split-count": "
+0000e7c0: 3322 7d7d 600a 2020 2020 2020 2020 2020  3"}}`.          
+0000e7d0: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+0000e7e0: 6f20 607b 7d60 2e0a 0a20 2020 2020 2020  o `{}`...       
+0000e7f0: 2023 2052 6574 7572 6e73 0a20 2020 2020   # Returns.     
+0000e800: 2020 2020 2020 2060 4461 7461 4672 616d         `DataFram
+0000e810: 6560 2e20 5468 6520 7370 6172 6b20 6461  e`. The spark da
+0000e820: 7461 6672 616d 6520 636f 6e74 6169 6e69  taframe containi
+0000e830: 6e67 2074 6865 2069 6e63 7265 6d65 6e74  ng the increment
+0000e840: 616c 2063 6861 6e67 6573 206f 660a 2020  al changes of.  
+0000e850: 2020 2020 2020 2020 2020 6665 6174 7572            featur
+0000e860: 6520 6461 7461 2e0a 0a20 2020 2020 2020  e data...       
+0000e870: 2023 2052 6169 7365 730a 2020 2020 2020   # Raises.      
+0000e880: 2020 2020 2020 6068 7366 732e 636c 6965        `hsfs.clie
+0000e890: 6e74 2e65 7863 6570 7469 6f6e 732e 5265  nt.exceptions.Re
+0000e8a0: 7374 4150 4945 7272 6f72 602e 2020 4e6f  stAPIError`.  No
+0000e8b0: 2064 6174 6120 6973 2061 7661 696c 6162   data is availab
+0000e8c0: 6c65 2066 6f72 2066 6561 7475 7265 2067  le for feature g
+0000e8d0: 726f 7570 2077 6974 6820 7468 6973 2063  roup with this c
+0000e8e0: 6f6d 6d69 7420 6461 7465 2e0a 2020 2020  ommit date..    
+0000e8f0: 2020 2020 2020 2020 6068 7366 732e 636c          `hsfs.cl
+0000e900: 6965 6e74 2e65 7863 6570 7469 6f6e 732e  ient.exceptions.
+0000e910: 4665 6174 7572 6553 746f 7265 4578 6365  FeatureStoreExce
+0000e920: 7074 696f 6e60 2e20 4966 2074 6865 2066  ption`. If the f
+0000e930: 6561 7475 7265 2067 726f 7570 2064 6f65  eature group doe
+0000e940: 7320 6e6f 7420 6861 7665 2060 4855 4449  s not have `HUDI
+0000e950: 6020 7469 6d65 2074 7261 7665 6c20 666f  ` time travel fo
+0000e960: 726d 6174 0a20 2020 2020 2020 2022 2222  rmat.        """
+0000e970: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000e980: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
+0000e990: 6c66 2e73 656c 6563 745f 616c 6c28 290a  lf.select_all().
+0000e9a0: 2020 2020 2020 2020 2020 2020 2e70 756c              .pul
+0000e9b0: 6c5f 6368 616e 6765 7328 7374 6172 745f  l_changes(start_
+0000e9c0: 7761 6c6c 636c 6f63 6b5f 7469 6d65 2c20  wallclock_time, 
+0000e9d0: 656e 645f 7761 6c6c 636c 6f63 6b5f 7469  end_wallclock_ti
+0000e9e0: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+0000e9f0: 2e72 6561 6428 4661 6c73 652c 2022 6465  .read(False, "de
+0000ea00: 6661 756c 7422 2c20 7265 6164 5f6f 7074  fault", read_opt
+0000ea10: 696f 6e73 290a 2020 2020 2020 2020 290a  ions).        ).
+0000ea20: 0a20 2020 2064 6566 2073 686f 7728 7365  .    def show(se
+0000ea30: 6c66 2c20 6e3a 2069 6e74 2c20 6f6e 6c69  lf, n: int, onli
+0000ea40: 6e65 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ne: Optional[boo
+0000ea50: 6c5d 203d 2046 616c 7365 293a 0a20 2020  l] = False):.   
+0000ea60: 2020 2020 2022 2222 5368 6f77 2074 6865       """Show the
+0000ea70: 2066 6972 7374 2060 6e60 2072 6f77 7320   first `n` rows 
+0000ea80: 6f66 2074 6865 2066 6561 7475 7265 2067  of the feature g
+0000ea90: 726f 7570 2e0a 0a20 2020 2020 2020 2021  roup...        !
+0000eaa0: 2121 2065 7861 6d70 6c65 0a20 2020 2020  !! example.     
+0000eab0: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+0000eac0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+0000ead0: 6f6e 6e65 6374 2074 6f20 7468 6520 4665  onnect to the Fe
+0000eae0: 6174 7572 6520 5374 6f72 650a 2020 2020  ature Store.    
+0000eaf0: 2020 2020 2020 2020 6673 203d 202e 2e2e          fs = ...
+0000eb00: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000eb10: 6765 7420 7468 6520 4665 6174 7572 6520  get the Feature 
+0000eb20: 4772 6f75 7020 696e 7374 616e 6365 0a20  Group instance. 
+0000eb30: 2020 2020 2020 2020 2020 2066 6720 3d20             fg = 
+0000eb40: 6673 2e67 6574 5f6f 725f 6372 6561 7465  fs.get_or_create
+0000eb50: 5f66 6561 7475 7265 5f67 726f 7570 282e  _feature_group(.
+0000eb60: 2e2e 290a 0a20 2020 2020 2020 2020 2020  ..)..           
+0000eb70: 2023 206d 616b 6520 6120 7175 6572 7920   # make a query 
+0000eb80: 616e 6420 7368 6f77 2074 6f70 2035 2072  and show top 5 r
+0000eb90: 6f77 730a 2020 2020 2020 2020 2020 2020  ows.            
+0000eba0: 6667 2e73 656c 6563 7428 5b27 6461 7465  fg.select(['date
+0000ebb0: 272c 2777 6565 6b6c 795f 7361 6c65 7327  ','weekly_sales'
+0000ebc0: 2c27 6973 5f68 6f6c 6964 6179 275d 292e  ,'is_holiday']).
+0000ebd0: 7368 6f77 2835 290a 2020 2020 2020 2020  show(5).        
+0000ebe0: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
+0000ebf0: 2023 2041 7267 756d 656e 7473 0a20 2020   # Arguments.   
+0000ec00: 2020 2020 2020 2020 206e 3a20 696e 742e           n: int.
+0000ec10: 204e 756d 6265 7220 6f66 2072 6f77 7320   Number of rows 
+0000ec20: 746f 2073 686f 772e 0a20 2020 2020 2020  to show..       
+0000ec30: 2020 2020 206f 6e6c 696e 653a 2062 6f6f       online: boo
+0000ec40: 6c2c 206f 7074 696f 6e61 6c2e 2049 6620  l, optional. If 
+0000ec50: 6054 7275 6560 2072 6561 6420 6672 6f6d  `True` read from
+0000ec60: 206f 6e6c 696e 6520 6665 6174 7572 6520   online feature 
+0000ec70: 7374 6f72 652c 2064 6566 6175 6c74 730a  store, defaults.
+0000ec80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec90: 746f 2060 4661 6c73 6560 2e0a 2020 2020  to `False`..    
+0000eca0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000ecb0: 656e 6769 6e65 2e67 6574 5f69 6e73 7461  engine.get_insta
+0000ecc0: 6e63 6528 292e 7365 745f 6a6f 625f 6772  nce().set_job_gr
+0000ecd0: 6f75 7028 0a20 2020 2020 2020 2020 2020  oup(.           
+0000ece0: 2022 4665 7463 6869 6e67 2046 6561 7475   "Fetching Featu
+0000ecf0: 7265 2067 726f 7570 222c 0a20 2020 2020  re group",.     
+0000ed00: 2020 2020 2020 2022 4765 7474 696e 6720         "Getting 
+0000ed10: 6665 6174 7572 6520 6772 6f75 703a 207b  feature group: {
+0000ed20: 7d20 6672 6f6d 2074 6865 2066 6561 7475  } from the featu
+0000ed30: 7265 7374 6f72 6520 7b7d 222e 666f 726d  restore {}".form
+0000ed40: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+0000ed50: 2020 2020 7365 6c66 2e5f 6e61 6d65 2c20      self._name, 
+0000ed60: 7365 6c66 2e5f 6665 6174 7572 655f 7374  self._feature_st
+0000ed70: 6f72 655f 6e61 6d65 0a20 2020 2020 2020  ore_name.       
+0000ed80: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+0000ed90: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000eda0: 2073 656c 662e 7365 6c65 6374 5f61 6c6c   self.select_all
+0000edb0: 2829 2e73 686f 7728 6e2c 206f 6e6c 696e  ().show(n, onlin
+0000edc0: 6529 0a0a 2020 2020 6465 6620 7361 7665  e)..    def save
+0000edd0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000ede0: 2020 2020 2020 2020 6665 6174 7572 6573          features
+0000edf0: 3a20 556e 696f 6e5b 0a20 2020 2020 2020  : Union[.       
+0000ee00: 2020 2020 2070 642e 4461 7461 4672 616d       pd.DataFram
+0000ee10: 652c 0a20 2020 2020 2020 2020 2020 2054  e,.            T
+0000ee20: 7970 6556 6172 2822 7079 7370 6172 6b2e  ypeVar("pyspark.
+0000ee30: 7371 6c2e 4461 7461 4672 616d 6522 292c  sql.DataFrame"),
+0000ee40: 2020 2320 6e6f 7161 3a20 4638 3231 0a20    # noqa: F821. 
+0000ee50: 2020 2020 2020 2020 2020 2054 7970 6556             TypeV
+0000ee60: 6172 2822 7079 7370 6172 6b2e 5244 4422  ar("pyspark.RDD"
+0000ee70: 292c 2020 2320 6e6f 7161 3a20 4638 3231  ),  # noqa: F821
+0000ee80: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
+0000ee90: 6e64 6172 7261 792c 0a20 2020 2020 2020  ndarray,.       
+0000eea0: 2020 2020 204c 6973 745b 6c69 7374 5d2c       List[list],
+0000eeb0: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
+0000eec0: 2020 2020 7772 6974 655f 6f70 7469 6f6e      write_option
+0000eed0: 733a 204f 7074 696f 6e61 6c5b 4469 6374  s: Optional[Dict
+0000eee0: 5b41 6e79 2c20 416e 795d 5d20 3d20 7b7d  [Any, Any]] = {}
+0000eef0: 2c0a 2020 2020 2020 2020 7661 6c69 6461  ,.        valida
+0000ef00: 7469 6f6e 5f6f 7074 696f 6e73 3a20 4f70  tion_options: Op
+0000ef10: 7469 6f6e 616c 5b44 6963 745b 416e 792c  tional[Dict[Any,
+0000ef20: 2041 6e79 5d5d 203d 207b 7d2c 0a20 2020   Any]] = {},.   
+0000ef30: 2029 3a0a 2020 2020 2020 2020 2222 2250   ):.        """P
+0000ef40: 6572 7369 7374 2074 6865 206d 6574 6164  ersist the metad
+0000ef50: 6174 6120 616e 6420 6d61 7465 7269 616c  ata and material
+0000ef60: 697a 6520 7468 6520 6665 6174 7572 6520  ize the feature 
+0000ef70: 6772 6f75 7020 746f 2074 6865 2066 6561  group to the fea
+0000ef80: 7475 7265 2073 746f 7265 2e0a 0a20 2020  ture store...   
+0000ef90: 2020 2020 2021 2121 2077 6172 6e69 6e67       !!! warning
+0000efa0: 2022 4465 7072 6563 6174 6564 220a 2020   "Deprecated".  
+0000efb0: 2020 2020 2020 2020 2020 6073 6176 6560            `save`
+0000efc0: 206d 6574 686f 6420 6973 2064 6570 7265   method is depre
+0000efd0: 6361 7465 642e 2055 7365 2074 6865 2060  cated. Use the `
+0000efe0: 696e 7365 7274 6020 6d65 7468 6f64 2069  insert` method i
+0000eff0: 6e73 7465 6164 2e0a 0a20 2020 2020 2020  nstead...       
+0000f000: 2043 616c 6c69 6e67 2060 7361 7665 6020   Calling `save` 
+0000f010: 6372 6561 7465 7320 7468 6520 6d65 7461  creates the meta
+0000f020: 6461 7461 2066 6f72 2074 6865 2066 6561  data for the fea
+0000f030: 7475 7265 2067 726f 7570 2069 6e20 7468  ture group in th
+0000f040: 6520 6665 6174 7572 6520 7374 6f72 650a  e feature store.
+0000f050: 2020 2020 2020 2020 616e 6420 7772 6974          and writ
+0000f060: 6573 2074 6865 2073 7065 6369 6669 6564  es the specified
+0000f070: 2060 6665 6174 7572 6573 6020 6461 7461   `features` data
+0000f080: 6672 616d 6520 6173 2066 6561 7475 7265  frame as feature
+0000f090: 2067 726f 7570 2074 6f20 7468 650a 2020   group to the.  
+0000f0a0: 2020 2020 2020 6f6e 6c69 6e65 2f6f 6666        online/off
+0000f0b0: 6c69 6e65 2066 6561 7475 7265 2073 746f  line feature sto
+0000f0c0: 7265 2061 7320 7370 6563 6966 6965 642e  re as specified.
+0000f0d0: 0a20 2020 2020 2020 2042 7920 6465 6661  .        By defa
+0000f0e0: 756c 742c 2074 6869 7320 7772 6974 6573  ult, this writes
+0000f0f0: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
+0000f100: 7570 2074 6f20 7468 6520 6f66 666c 696e  up to the offlin
+0000f110: 6520 7374 6f72 6167 652c 2061 6e64 2069  e storage, and i
+0000f120: 660a 2020 2020 2020 2020 606f 6e6c 696e  f.        `onlin
+0000f130: 655f 656e 6162 6c65 6460 2066 6f72 2074  e_enabled` for t
+0000f140: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
+0000f150: 2c20 616c 736f 2074 6f20 7468 6520 6f6e  , also to the on
+0000f160: 6c69 6e65 2066 6561 7475 7265 2073 746f  line feature sto
+0000f170: 7265 2e0a 2020 2020 2020 2020 5468 6520  re..        The 
+0000f180: 6066 6561 7475 7265 7360 2064 6174 6166  `features` dataf
+0000f190: 7261 6d65 2063 616e 2062 6520 6120 5370  rame can be a Sp
+0000f1a0: 6172 6b20 4461 7461 4672 616d 6520 6f72  ark DataFrame or
+0000f1b0: 2052 4444 2c20 6120 5061 6e64 6173 2044   RDD, a Pandas D
+0000f1c0: 6174 6146 7261 6d65 2c0a 2020 2020 2020  ataFrame,.      
+0000f1d0: 2020 6f72 2061 2074 776f 2d64 696d 656e    or a two-dimen
+0000f1e0: 7369 6f6e 616c 204e 756d 7079 2061 7272  sional Numpy arr
+0000f1f0: 6179 206f 7220 6120 7477 6f2d 6469 6d65  ay or a two-dime
+0000f200: 6e73 696f 6e61 6c20 5079 7468 6f6e 206e  nsional Python n
+0000f210: 6573 7465 6420 6c69 7374 2e0a 2020 2020  ested list..    
+0000f220: 2020 2020 2320 4172 6775 6d65 6e74 730a      # Arguments.
+0000f230: 2020 2020 2020 2020 2020 2020 6665 6174              feat
+0000f240: 7572 6573 3a20 5175 6572 792c 2044 6174  ures: Query, Dat
+0000f250: 6146 7261 6d65 2c20 5244 442c 204e 6461  aFrame, RDD, Nda
+0000f260: 7272 6179 2c20 6c69 7374 2e20 4665 6174  rray, list. Feat
+0000f270: 7572 6573 2074 6f20 6265 2073 6176 6564  ures to be saved
+0000f280: 2e0a 2020 2020 2020 2020 2020 2020 7772  ..            wr
+0000f290: 6974 655f 6f70 7469 6f6e 733a 2041 6464  ite_options: Add
+0000f2a0: 6974 696f 6e61 6c20 7772 6974 6520 6f70  itional write op
+0000f2b0: 7469 6f6e 7320 6173 206b 6579 2d76 616c  tions as key-val
+0000f2c0: 7565 2070 6169 7273 2c20 6465 6661 756c  ue pairs, defaul
+0000f2d0: 7473 2074 6f20 607b 7d60 2e0a 2020 2020  ts to `{}`..    
+0000f2e0: 2020 2020 2020 2020 2020 2020 5768 656e              When
+0000f2f0: 2075 7369 6e67 2074 6865 2060 7079 7468   using the `pyth
+0000f300: 6f6e 6020 656e 6769 6e65 2c20 7772 6974  on` engine, writ
+0000f310: 655f 6f70 7469 6f6e 7320 6361 6e20 636f  e_options can co
+0000f320: 6e74 6169 6e20 7468 650a 2020 2020 2020  ntain the.      
+0000f330: 2020 2020 2020 2020 2020 666f 6c6c 6f77            follow
+0000f340: 696e 6720 656e 7472 6965 733a 0a20 2020  ing entries:.   
+0000f350: 2020 2020 2020 2020 2020 2020 202a 206b               * k
+0000f360: 6579 2060 7370 6172 6b60 2061 6e64 2076  ey `spark` and v
+0000f370: 616c 7565 2061 6e20 6f62 6a65 6374 206f  alue an object o
+0000f380: 6620 7479 7065 0a20 2020 2020 2020 2020  f type.         
+0000f390: 2020 2020 2020 205b 6873 6673 2e63 6f72         [hsfs.cor
+0000f3a0: 652e 6a6f 625f 636f 6e66 6967 7572 6174  e.job_configurat
+0000f3b0: 696f 6e2e 4a6f 6243 6f6e 6669 6775 7261  ion.JobConfigura
+0000f3c0: 7469 6f6e 5d28 2e2e 2f6a 6f62 5f63 6f6e  tion](../job_con
+0000f3d0: 6669 6775 7261 7469 6f6e 290a 2020 2020  figuration).    
+0000f3e0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+0000f3f0: 2063 6f6e 6669 6775 7265 2074 6865 2048   configure the H
+0000f400: 6f70 7377 6f72 6b73 204a 6f62 2075 7365  opsworks Job use
+0000f410: 6420 746f 2077 7269 7465 2064 6174 6120  d to write data 
+0000f420: 696e 746f 2074 6865 0a20 2020 2020 2020  into the.       
+0000f430: 2020 2020 2020 2020 2020 2066 6561 7475             featu
+0000f440: 7265 2067 726f 7570 2e0a 2020 2020 2020  re group..      
+0000f450: 2020 2020 2020 2020 2020 2a20 6b65 7920            * key 
+0000f460: 6077 6169 745f 666f 725f 6a6f 6260 2061  `wait_for_job` a
+0000f470: 6e64 2076 616c 7565 2060 5472 7565 6020  nd value `True` 
+0000f480: 6f72 2060 4661 6c73 6560 2074 6f20 636f  or `False` to co
+0000f490: 6e66 6967 7572 650a 2020 2020 2020 2020  nfigure.        
+0000f4a0: 2020 2020 2020 2020 2020 7768 6574 6865            whethe
+0000f4b0: 7220 6f72 206e 6f74 2074 6f20 7468 6520  r or not to the 
+0000f4c0: 7361 7665 2063 616c 6c20 7368 6f75 6c64  save call should
+0000f4d0: 2072 6574 7572 6e20 6f6e 6c79 0a20 2020   return only.   
+0000f4e0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000f4f0: 6674 6572 2074 6865 2048 6f70 7377 6f72  fter the Hopswor
+0000f500: 6b73 204a 6f62 2068 6173 2066 696e 6973  ks Job has finis
+0000f510: 6865 642e 2042 7920 6465 6661 756c 7420  hed. By default 
+0000f520: 6974 2077 6169 7473 2e0a 2020 2020 2020  it waits..      
+0000f530: 2020 2020 2020 2020 2020 2a20 6b65 7920            * key 
+0000f540: 6073 7461 7274 5f6f 6666 6c69 6e65 5f62  `start_offline_b
+0000f550: 6163 6b66 696c 6c60 2061 6e64 2076 616c  ackfill` and val
+0000f560: 7565 2060 5472 7565 6020 6f72 2060 4661  ue `True` or `Fa
+0000f570: 6c73 6560 2074 6f20 636f 6e66 6967 7572  lse` to configur
+0000f580: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000f590: 2020 2020 7768 6574 6865 7220 6f72 206e      whether or n
+0000f5a0: 6f74 2074 6f20 7374 6172 7420 7468 6520  ot to start the 
+0000f5b0: 6261 636b 6669 6c6c 206a 6f62 2074 6f20  backfill job to 
+0000f5c0: 7772 6974 6520 6461 7461 2074 6f20 7468  write data to th
+0000f5d0: 6520 6f66 666c 696e 650a 2020 2020 2020  e offline.      
+0000f5e0: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
+0000f5f0: 6167 652e 2042 7920 6465 6661 756c 7420  age. By default 
+0000f600: 7468 6520 6261 636b 6669 6c6c 206a 6f62  the backfill job
+0000f610: 2067 6574 7320 7374 6172 7465 6420 696d   gets started im
+0000f620: 6d65 6469 6174 656c 792e 0a20 2020 2020  mediately..     
+0000f630: 2020 2020 2020 2020 2020 202a 206b 6579             * key
+0000f640: 2060 696e 7465 726e 616c 5f6b 6166 6b61   `internal_kafka
+0000f650: 6020 616e 6420 7661 6c75 6520 6054 7275  ` and value `Tru
+0000f660: 6560 206f 7220 6046 616c 7365 6020 696e  e` or `False` in
+0000f670: 2063 6173 6520 796f 7520 6573 7461 626c   case you establ
+0000f680: 6973 6865 640a 2020 2020 2020 2020 2020  ished.          
+0000f690: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
+0000f6a0: 7669 7479 2066 726f 6d20 796f 7520 5079  vity from you Py
+0000f6b0: 7468 6f6e 2065 6e76 6972 6f6e 6d65 6e74  thon environment
+0000f6c0: 2074 6f20 7468 6520 696e 7465 726e 616c   to the internal
+0000f6d0: 2061 6476 6572 7469 7365 640a 2020 2020   advertised.    
+0000f6e0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0000f6f0: 7374 656e 6572 7320 6f66 2074 6865 2048  steners of the H
+0000f700: 6f70 7377 6f72 6b73 204b 6166 6b61 2043  opsworks Kafka C
+0000f710: 6c75 7374 6572 2e20 4465 6661 756c 7473  luster. Defaults
+0000f720: 2074 6f20 6046 616c 7365 6020 616e 640a   to `False` and.
+0000f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f740: 2020 7769 6c6c 2075 7365 2065 7874 6572    will use exter
+0000f750: 6e61 6c20 6c69 7374 656e 6572 7320 7768  nal listeners wh
+0000f760: 656e 2063 6f6e 6e65 6374 696e 6720 6672  en connecting fr
+0000f770: 6f6d 206f 7574 7369 6465 206f 6620 486f  om outside of Ho
+0000f780: 7073 776f 726b 732e 0a20 2020 2020 2020  psworks..       
+0000f790: 2020 2020 2076 616c 6964 6174 696f 6e5f       validation_
+0000f7a0: 6f70 7469 6f6e 733a 2041 6464 6974 696f  options: Additio
+0000f7b0: 6e61 6c20 7661 6c69 6461 7469 6f6e 206f  nal validation o
+0000f7c0: 7074 696f 6e73 2061 7320 6b65 792d 7661  ptions as key-va
+0000f7d0: 6c75 6520 7061 6972 732c 2064 6566 6175  lue pairs, defau
+0000f7e0: 6c74 7320 746f 2060 7b7d 602e 0a20 2020  lts to `{}`..   
+0000f7f0: 2020 2020 2020 2020 2020 2020 202a 206b               * k
+0000f800: 6579 2060 7275 6e5f 7661 6c69 6461 7469  ey `run_validati
+0000f810: 6f6e 6020 626f 6f6c 6561 6e20 7661 6c75  on` boolean valu
+0000f820: 652c 2073 6574 2074 6f20 6046 616c 7365  e, set to `False
+0000f830: 6020 746f 2073 6b69 7020 7661 6c69 6461  ` to skip valida
+0000f840: 7469 6f6e 2074 656d 706f 7261 7269 6c79  tion temporarily
+0000f850: 206f 6e20 696e 6765 7374 696f 6e2e 0a20   on ingestion.. 
+0000f860: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+0000f870: 206b 6579 2060 7361 7665 5f72 6570 6f72   key `save_repor
+0000f880: 7460 2062 6f6f 6c65 616e 2076 616c 7565  t` boolean value
+0000f890: 2c20 7365 7420 746f 2060 4661 6c73 6560  , set to `False`
+0000f8a0: 2074 6f20 736b 6970 2075 706c 6f61 6420   to skip upload 
+0000f8b0: 6f66 2074 6865 2076 616c 6964 6174 696f  of the validatio
+0000f8c0: 6e20 7265 706f 7274 2074 6f20 486f 7073  n report to Hops
+0000f8d0: 776f 726b 732e 0a20 2020 2020 2020 2020  works..         
+0000f8e0: 2020 2020 2020 202a 206b 6579 2060 6765         * key `ge
+0000f8f0: 5f76 616c 6964 6174 655f 6b77 6172 6773  _validate_kwargs
+0000f900: 6020 6120 6469 6374 696f 6e61 7279 2063  ` a dictionary c
+0000f910: 6f6e 7461 696e 696e 6720 6b77 6172 6773  ontaining kwargs
+0000f920: 2066 6f72 2074 6865 2076 616c 6964 6174   for the validat
+0000f930: 6520 6d65 7468 6f64 206f 6620 4772 6561  e method of Grea
+0000f940: 7420 4578 7065 6374 6174 696f 6e73 2e0a  t Expectations..
+0000f950: 0a20 2020 2020 2020 2023 2052 6574 7572  .        # Retur
+0000f960: 6e73 0a20 2020 2020 2020 2020 2020 2060  ns.            `
+0000f970: 4a6f 6260 3a20 5768 656e 2075 7369 6e67  Job`: When using
+0000f980: 2074 6865 2060 7079 7468 6f6e 6020 656e   the `python` en
+0000f990: 6769 6e65 2c20 6974 2072 6574 7572 6e73  gine, it returns
+0000f9a0: 2074 6865 2048 6f70 7377 6f72 6b73 204a   the Hopsworks J
+0000f9b0: 6f62 0a20 2020 2020 2020 2020 2020 2020  ob.             
+0000f9c0: 2020 2074 6861 7420 7761 7320 6c61 756e     that was laun
+0000f9d0: 6368 6564 2074 6f20 696e 6765 7374 2074  ched to ingest t
+0000f9e0: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
+0000f9f0: 2064 6174 612e 0a0a 2020 2020 2020 2020   data...        
+0000fa00: 2320 5261 6973 6573 0a20 2020 2020 2020  # Raises.       
+0000fa10: 2020 2020 2060 6873 6673 2e63 6c69 656e       `hsfs.clien
+0000fa20: 742e 6578 6365 7074 696f 6e73 2e52 6573  t.exceptions.Res
+0000fa30: 7441 5049 4572 726f 7260 2e20 556e 6162  tAPIError`. Unab
+0000fa40: 6c65 2074 6f20 6372 6561 7465 2066 6561  le to create fea
+0000fa50: 7475 7265 2067 726f 7570 2e0a 2020 2020  ture group..    
+0000fa60: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000fa70: 6665 6174 7572 655f 6461 7461 6672 616d  feature_datafram
+0000fa80: 6520 3d20 656e 6769 6e65 2e67 6574 5f69  e = engine.get_i
+0000fa90: 6e73 7461 6e63 6528 292e 636f 6e76 6572  nstance().conver
+0000faa0: 745f 746f 5f64 6566 6175 6c74 5f64 6174  t_to_default_dat
+0000fab0: 6166 7261 6d65 2866 6561 7475 7265 7329  aframe(features)
+0000fac0: 0a0a 2020 2020 2020 2020 7573 6572 5f76  ..        user_v
+0000fad0: 6572 7369 6f6e 203d 2073 656c 662e 5f76  ersion = self._v
+0000fae0: 6572 7369 6f6e 0a0a 2020 2020 2020 2020  ersion..        
+0000faf0: 2320 6667 5f6a 6f62 2069 7320 7573 6564  # fg_job is used
+0000fb00: 206f 6e6c 7920 6966 2074 6865 2070 7974   only if the pyt
+0000fb10: 686f 6e20 656e 6769 6e65 2069 7320 7573  hon engine is us
+0000fb20: 6564 0a20 2020 2020 2020 2066 675f 6a6f  ed.        fg_jo
+0000fb30: 622c 2067 655f 7265 706f 7274 203d 2073  b, ge_report = s
+0000fb40: 656c 662e 5f66 6561 7475 7265 5f67 726f  elf._feature_gro
+0000fb50: 7570 5f65 6e67 696e 652e 7361 7665 280a  up_engine.save(.
+0000fb60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fb70: 2c20 6665 6174 7572 655f 6461 7461 6672  , feature_datafr
+0000fb80: 616d 652c 2077 7269 7465 5f6f 7074 696f  ame, write_optio
+0000fb90: 6e73 2c20 7661 6c69 6461 7469 6f6e 5f6f  ns, validation_o
+0000fba0: 7074 696f 6e73 0a20 2020 2020 2020 2029  ptions.        )
+0000fbb0: 0a20 2020 2020 2020 2069 6620 6765 5f72  .        if ge_r
+0000fbc0: 6570 6f72 7420 6973 204e 6f6e 6520 6f72  eport is None or
+0000fbd0: 2067 655f 7265 706f 7274 2e69 6e67 6573   ge_report.inges
+0000fbe0: 7469 6f6e 5f72 6573 756c 7420 3d3d 2022  tion_result == "
+0000fbf0: 494e 4745 5354 4544 223a 0a20 2020 2020  INGESTED":.     
+0000fc00: 2020 2020 2020 2073 656c 662e 5f63 6f64         self._cod
+0000fc10: 655f 656e 6769 6e65 2e73 6176 655f 636f  e_engine.save_co
+0000fc20: 6465 2873 656c 6629 0a0a 2020 2020 2020  de(self)..      
+0000fc30: 2020 6966 2073 656c 662e 7374 6174 6973    if self.statis
+0000fc40: 7469 6373 5f63 6f6e 6669 672e 656e 6162  tics_config.enab
+0000fc50: 6c65 6420 616e 6420 656e 6769 6e65 2e67  led and engine.g
+0000fc60: 6574 5f74 7970 6528 2920 3d3d 2022 7370  et_type() == "sp
+0000fc70: 6172 6b22 3a0a 2020 2020 2020 2020 2020  ark":.          
+0000fc80: 2020 2320 4f6e 6c79 2063 6f6d 7075 7465    # Only compute
+0000fc90: 2073 7461 7469 7374 6963 7320 6966 2074   statistics if t
+0000fca0: 6865 2065 6e67 696e 6520 6973 2053 7061  he engine is Spa
+0000fcb0: 726b 2e0a 2020 2020 2020 2020 2020 2020  rk..            
+0000fcc0: 2320 466f 7220 5079 7468 6f6e 2065 6e67  # For Python eng
+0000fcd0: 696e 652c 2074 6865 2063 6f6d 7075 7461  ine, the computa
+0000fce0: 7469 6f6e 2068 6170 7065 6e73 2069 6e20  tion happens in 
+0000fcf0: 7468 6520 486f 7073 776f 726b 7320 6170  the Hopsworks ap
+0000fd00: 706c 6963 6174 696f 6e0a 2020 2020 2020  plication.      
+0000fd10: 2020 2020 2020 7365 6c66 2e5f 7374 6174        self._stat
+0000fd20: 6973 7469 6373 5f65 6e67 696e 652e 636f  istics_engine.co
+0000fd30: 6d70 7574 655f 7374 6174 6973 7469 6373  mpute_statistics
+0000fd40: 2873 656c 662c 2066 6561 7475 7265 5f64  (self, feature_d
+0000fd50: 6174 6166 7261 6d65 290a 2020 2020 2020  ataframe).      
+0000fd60: 2020 6966 2075 7365 725f 7665 7273 696f    if user_versio
+0000fd70: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+0000fd80: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
+0000fd90: 7761 726e 280a 2020 2020 2020 2020 2020  warn(.          
+0000fda0: 2020 2020 2020 224e 6f20 7665 7273 696f        "No versio
+0000fdb0: 6e20 7072 6f76 6964 6564 2066 6f72 2063  n provided for c
+0000fdc0: 7265 6174 696e 6720 6665 6174 7572 6520  reating feature 
+0000fdd0: 6772 6f75 7020 607b 7d60 2c20 696e 6372  group `{}`, incr
+0000fde0: 656d 656e 7465 6420 7665 7273 696f 6e20  emented version 
+0000fdf0: 746f 2060 7b7d 602e 222e 666f 726d 6174  to `{}`.".format
+0000fe00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000fe10: 2020 2020 2020 7365 6c66 2e5f 6e61 6d65        self._name
+0000fe20: 2c20 7365 6c66 2e5f 7665 7273 696f 6e0a  , self._version.
+0000fe30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe40: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000fe50: 2020 2075 7469 6c2e 5665 7273 696f 6e57     util.VersionW
+0000fe60: 6172 6e69 6e67 2c0a 2020 2020 2020 2020  arning,.        
+0000fe70: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+0000fe80: 7475 726e 2028 0a20 2020 2020 2020 2020  turn (.         
+0000fe90: 2020 2066 675f 6a6f 622c 0a20 2020 2020     fg_job,.     
+0000fea0: 2020 2020 2020 2067 655f 7265 706f 7274         ge_report
+0000feb0: 2e74 6f5f 6765 5f74 7970 6528 2920 6966  .to_ge_type() if
+0000fec0: 2067 655f 7265 706f 7274 2069 7320 6e6f   ge_report is no
+0000fed0: 7420 4e6f 6e65 2065 6c73 6520 4e6f 6e65  t None else None
+0000fee0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+0000fef0: 2064 6566 2069 6e73 6572 7428 0a20 2020   def insert(.   
+0000ff00: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000ff10: 2020 2066 6561 7475 7265 733a 2055 6e69     features: Uni
+0000ff20: 6f6e 5b0a 2020 2020 2020 2020 2020 2020  on[.            
+0000ff30: 7064 2e44 6174 6146 7261 6d65 2c0a 2020  pd.DataFrame,.  
+0000ff40: 2020 2020 2020 2020 2020 5479 7065 5661            TypeVa
+0000ff50: 7228 2270 7973 7061 726b 2e73 716c 2e44  r("pyspark.sql.D
+0000ff60: 6174 6146 7261 6d65 2229 2c20 2023 206e  ataFrame"),  # n
+0000ff70: 6f71 613a 2046 3832 310a 2020 2020 2020  oqa: F821.      
+0000ff80: 2020 2020 2020 5479 7065 5661 7228 2270        TypeVar("p
+0000ff90: 7973 7061 726b 2e52 4444 2229 2c20 2023  yspark.RDD"),  #
+0000ffa0: 206e 6f71 613a 2046 3832 310a 2020 2020   noqa: F821.    
+0000ffb0: 2020 2020 2020 2020 6e70 2e6e 6461 7272          np.ndarr
+0000ffc0: 6179 2c0a 2020 2020 2020 2020 2020 2020  ay,.            
+0000ffd0: 4c69 7374 5b6c 6973 745d 2c0a 2020 2020  List[list],.    
+0000ffe0: 2020 2020 5d2c 0a20 2020 2020 2020 206f      ],.        o
+0000fff0: 7665 7277 7269 7465 3a20 4f70 7469 6f6e  verwrite: Option
+00010000: 616c 5b62 6f6f 6c5d 203d 2046 616c 7365  al[bool] = False
+00010010: 2c0a 2020 2020 2020 2020 6f70 6572 6174  ,.        operat
+00010020: 696f 6e3a 204f 7074 696f 6e61 6c5b 7374  ion: Optional[st
+00010030: 725d 203d 2022 7570 7365 7274 222c 0a20  r] = "upsert",. 
+00010040: 2020 2020 2020 2073 746f 7261 6765 3a20         storage: 
+00010050: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00010060: 4e6f 6e65 2c0a 2020 2020 2020 2020 7772  None,.        wr
+00010070: 6974 655f 6f70 7469 6f6e 733a 204f 7074  ite_options: Opt
+00010080: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
+00010090: 416e 795d 5d20 3d20 7b7d 2c0a 2020 2020  Any]] = {},.    
+000100a0: 2020 2020 7661 6c69 6461 7469 6f6e 5f6f      validation_o
+000100b0: 7074 696f 6e73 3a20 4f70 7469 6f6e 616c  ptions: Optional
+000100c0: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
+000100d0: 203d 207b 7d2c 0a20 2020 2020 2020 2073   = {},.        s
+000100e0: 6176 655f 636f 6465 3a20 4f70 7469 6f6e  ave_code: Option
+000100f0: 616c 5b62 6f6f 6c5d 203d 2054 7275 652c  al[bool] = True,
+00010100: 0a20 2020 2029 202d 3e20 5475 706c 655b  .    ) -> Tuple[
+00010110: 4f70 7469 6f6e 616c 5b4a 6f62 5d2c 204f  Optional[Job], O
+00010120: 7074 696f 6e61 6c5b 5661 6c69 6461 7469  ptional[Validati
+00010130: 6f6e 5265 706f 7274 5d5d 3a0a 2020 2020  onReport]]:.    
+00010140: 2020 2020 2222 2250 6572 7369 7374 2074      """Persist t
+00010150: 6865 206d 6574 6164 6174 6120 616e 6420  he metadata and 
+00010160: 6d61 7465 7269 616c 697a 6520 7468 6520  materialize the 
+00010170: 6665 6174 7572 6520 6772 6f75 7020 746f  feature group to
+00010180: 2074 6865 2066 6561 7475 7265 2073 746f   the feature sto
+00010190: 7265 0a20 2020 2020 2020 206f 7220 696e  re.        or in
+000101a0: 7365 7274 2064 6174 6120 6672 6f6d 2061  sert data from a
+000101b0: 2064 6174 6166 7261 6d65 2069 6e74 6f20   dataframe into 
+000101c0: 7468 6520 6578 6973 7469 6e67 2066 6561  the existing fea
+000101d0: 7475 7265 2067 726f 7570 2e0a 0a20 2020  ture group...   
+000101e0: 2020 2020 2049 6e63 7265 6d65 6e74 616c       Incremental
+000101f0: 6c79 2069 6e73 6572 7420 6461 7461 2074  ly insert data t
+00010200: 6f20 6120 6665 6174 7572 6520 6772 6f75  o a feature grou
+00010210: 7020 6f72 206f 7665 7277 7269 7465 2061  p or overwrite a
+00010220: 6c6c 2020 6461 7461 2063 6f6e 7461 696e  ll  data contain
+00010230: 6564 2069 6e20 7468 6520 6665 6174 7572  ed in the featur
+00010240: 6520 6772 6f75 702e 2042 790a 2020 2020  e group. By.    
+00010250: 2020 2020 6465 6661 756c 742c 2074 6865      default, the
+00010260: 2064 6174 6120 6973 2069 6e73 6572 7465   data is inserte
+00010270: 6420 696e 746f 2074 6865 206f 6666 6c69  d into the offli
+00010280: 6e65 2073 746f 7261 6765 2061 7320 7765  ne storage as we
+00010290: 6c6c 2061 7320 7468 6520 6f6e 6c69 6e65  ll as the online
+000102a0: 2073 746f 7261 6765 2069 6620 7468 6520   storage if the 
+000102b0: 6665 6174 7572 6520 6772 6f75 7020 6973  feature group is
+000102c0: 0a20 2020 2020 2020 2060 6f6e 6c69 6e65  .        `online
+000102d0: 5f65 6e61 626c 6564 3d54 7275 6560 2e20  _enabled=True`. 
+000102e0: 546f 2069 6e73 6572 7420 6f6e 6c79 2069  To insert only i
+000102f0: 6e74 6f20 7468 6520 6f6e 6c69 6e65 206f  nto the online o
+00010300: 7220 6f66 666c 696e 6520 7374 6f72 6167  r offline storag
+00010310: 6520 7365 7420 6073 746f 7261 6765 3d22  e set `storage="
+00010320: 6f6e 6c69 6e65 2260 206f 720a 2020 2020  online"` or.    
+00010330: 2020 2020 6073 746f 7261 6765 3d22 6f66      `storage="of
+00010340: 666c 696e 6522 6020 7265 7370 6563 7469  fline"` respecti
+00010350: 7665 6c79 2e0a 0a20 2020 2020 2020 2054  vely...        T
+00010360: 6865 2060 6665 6174 7572 6573 6020 6461  he `features` da
+00010370: 7461 6672 616d 6520 6361 6e20 6265 2061  taframe can be a
+00010380: 2053 7061 726b 2044 6174 6146 7261 6d65   Spark DataFrame
+00010390: 206f 7220 5244 442c 2061 2050 616e 6461   or RDD, a Panda
+000103a0: 7320 4461 7461 4672 616d 652c 0a20 2020  s DataFrame,.   
+000103b0: 2020 2020 206f 7220 6120 7477 6f2d 6469       or a two-di
+000103c0: 6d65 6e73 696f 6e61 6c20 4e75 6d70 7920  mensional Numpy 
+000103d0: 6172 7261 7920 6f72 2061 2074 776f 2d64  array or a two-d
+000103e0: 696d 656e 7369 6f6e 616c 2050 7974 686f  imensional Pytho
+000103f0: 6e20 6e65 7374 6564 206c 6973 742e 0a20  n nested list.. 
+00010400: 2020 2020 2020 2049 6620 7374 6174 6973         If statis
+00010410: 7469 6373 2061 7265 2065 6e61 626c 6564  tics are enabled
+00010420: 2c20 7374 6174 6973 7469 6373 2061 7265  , statistics are
+00010430: 2072 6563 6f6d 7075 7465 6420 666f 7220   recomputed for 
+00010440: 7468 6520 656e 7469 7265 2066 6561 7475  the entire featu
+00010450: 7265 0a20 2020 2020 2020 2067 726f 7570  re.        group
+00010460: 2e0a 2020 2020 2020 2020 4966 2066 6561  ..        If fea
+00010470: 7475 7265 2067 726f 7570 2773 2074 696d  ture group's tim
+00010480: 6520 7472 6176 656c 2066 6f72 6d61 7420  e travel format 
+00010490: 6973 2060 4855 4449 6020 7468 656e 2060  is `HUDI` then `
+000104a0: 6f70 6572 6174 696f 6e60 2061 7267 756d  operation` argum
+000104b0: 656e 7420 6361 6e20 6265 0a20 2020 2020  ent can be.     
+000104c0: 2020 2065 6974 6865 7220 6069 6e73 6572     either `inser
+000104d0: 7460 206f 7220 6075 7073 6572 7460 2e0a  t` or `upsert`..
+000104e0: 0a20 2020 2020 2020 2049 6620 6665 6174  .        If feat
+000104f0: 7572 6520 6772 6f75 7020 646f 6573 6e27  ure group doesn'
+00010500: 7420 6578 6973 7473 2020 7468 6520 696e  t exists  the in
+00010510: 7365 7274 206d 6574 686f 6420 7769 6c6c  sert method will
+00010520: 2063 7265 6174 6520 7468 6520 6e65 6365   create the nece
+00010530: 7373 6172 7920 6d65 7461 6461 7461 2074  ssary metadata t
+00010540: 6865 2066 6972 7374 2074 696d 6520 6974  he first time it
+00010550: 2069 730a 2020 2020 2020 2020 696e 766f   is.        invo
+00010560: 6b65 6420 616e 6420 7772 6974 6573 2074  ked and writes t
+00010570: 6865 2073 7065 6369 6669 6564 2060 6665  he specified `fe
+00010580: 6174 7572 6573 6020 6461 7461 6672 616d  atures` datafram
+00010590: 6520 6173 2066 6561 7475 7265 2067 726f  e as feature gro
+000105a0: 7570 2074 6f20 7468 6520 6f6e 6c69 6e65  up to the online
+000105b0: 2f6f 6666 6c69 6e65 2066 6561 7475 7265  /offline feature
+000105c0: 2073 746f 7265 2e0a 0a20 2020 2020 2020   store...       
+000105d0: 2021 2121 2065 7861 6d70 6c65 2022 5570   !!! example "Up
+000105e0: 7365 7274 206e 6577 2066 6561 7475 7265  sert new feature
+000105f0: 2064 6174 6120 7769 7468 2074 696d 6520   data with time 
+00010600: 7472 6176 656c 2066 6f72 6d61 7420 6048  travel format `H
+00010610: 5544 4960 220a 2020 2020 2020 2020 2020  UDI`".          
+00010620: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
+00010630: 2020 2020 2020 2020 2320 636f 6e6e 6563          # connec
+00010640: 7420 746f 2074 6865 2046 6561 7475 7265  t to the Feature
+00010650: 2053 746f 7265 0a20 2020 2020 2020 2020   Store.         
+00010660: 2020 2066 7320 3d20 2e2e 2e0a 0a20 2020     fs = .....   
+00010670: 2020 2020 2020 2020 2066 6720 3d20 6673           fg = fs
+00010680: 2e67 6574 5f6f 725f 6372 6561 7465 5f66  .get_or_create_f
+00010690: 6561 7475 7265 5f67 726f 7570 280a 2020  eature_group(.  
+000106a0: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+000106b0: 6d65 3d27 6269 7463 6f69 6e5f 7072 6963  me='bitcoin_pric
+000106c0: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+000106d0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
+000106e0: 2742 6974 636f 696e 2070 7269 6365 2061  'Bitcoin price a
+000106f0: 6767 7265 6761 7465 6420 666f 7220 6461  ggregated for da
+00010700: 7973 272c 0a20 2020 2020 2020 2020 2020  ys',.           
+00010710: 2020 2020 2076 6572 7369 6f6e 3d31 2c0a       version=1,.
+00010720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010730: 7072 696d 6172 795f 6b65 793d 5b27 756e  primary_key=['un
+00010740: 6978 275d 2c0a 2020 2020 2020 2020 2020  ix'],.          
+00010750: 2020 2020 2020 6f6e 6c69 6e65 5f65 6e61        online_ena
+00010760: 626c 6564 3d54 7275 652c 0a20 2020 2020  bled=True,.     
+00010770: 2020 2020 2020 2020 2020 2065 7665 6e74             event
+00010780: 5f74 696d 653d 2775 6e69 7827 0a20 2020  _time='unix'.   
+00010790: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+000107a0: 2020 2020 2020 2020 6667 2e69 6e73 6572          fg.inser
+000107b0: 7428 6466 5f62 6974 636f 696e 5f70 726f  t(df_bitcoin_pro
+000107c0: 6365 7373 6564 290a 2020 2020 2020 2020  cessed).        
+000107d0: 2020 2020 6060 600a 0a20 2020 2020 2020      ```..       
+000107e0: 2021 2121 2065 7861 6d70 6c65 2022 4173   !!! example "As
+000107f0: 796e 6320 696e 7365 7274 220a 2020 2020  ync insert".    
+00010800: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+00010810: 6e0a 2020 2020 2020 2020 2020 2020 2320  n.            # 
+00010820: 636f 6e6e 6563 7420 746f 2074 6865 2046  connect to the F
+00010830: 6561 7475 7265 2053 746f 7265 0a20 2020  eature Store.   
+00010840: 2020 2020 2020 2020 2066 7320 3d20 2e2e           fs = ..
+00010850: 2e0a 0a20 2020 2020 2020 2020 2020 2066  ...            f
+00010860: 6731 203d 2066 732e 6765 745f 6f72 5f63  g1 = fs.get_or_c
+00010870: 7265 6174 655f 6665 6174 7572 655f 6772  reate_feature_gr
+00010880: 6f75 7028 0a20 2020 2020 2020 2020 2020  oup(.           
+00010890: 2020 2020 206e 616d 653d 2766 6561 7475       name='featu
+000108a0: 7265 5f67 726f 7570 5f6e 616d 6531 272c  re_group_name1',
+000108b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000108c0: 2064 6573 6372 6970 7469 6f6e 3d27 4465   description='De
+000108d0: 7363 7269 7074 696f 6e20 6f66 2074 6865  scription of the
+000108e0: 2066 6972 7374 2046 4727 2c0a 2020 2020   first FG',.    
+000108f0: 2020 2020 2020 2020 2020 2020 7665 7273              vers
+00010900: 696f 6e3d 312c 0a20 2020 2020 2020 2020  ion=1,.         
+00010910: 2020 2020 2020 2070 7269 6d61 7279 5f6b         primary_k
+00010920: 6579 3d5b 2775 6e69 7827 5d2c 0a20 2020  ey=['unix'],.   
+00010930: 2020 2020 2020 2020 2020 2020 206f 6e6c               onl
+00010940: 696e 655f 656e 6162 6c65 643d 5472 7565  ine_enabled=True
+00010950: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010960: 2020 6576 656e 745f 7469 6d65 3d27 756e    event_time='un
+00010970: 6978 270a 2020 2020 2020 2020 2020 2020  ix'.            
+00010980: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+00010990: 6173 796e 6320 696e 7365 7274 696f 6e20  async insertion 
+000109a0: 696e 206f 7264 6572 206e 6f74 2074 6f20  in order not to 
+000109b0: 7761 6974 2074 696c 6c20 6669 6e69 7368  wait till finish
+000109c0: 206f 6620 7468 6520 6a6f 620a 2020 2020   of the job.    
+000109d0: 2020 2020 2020 2020 6667 2e69 6e73 6572          fg.inser
+000109e0: 7428 6466 5f66 6f72 5f66 6731 2c20 7772  t(df_for_fg1, wr
+000109f0: 6974 655f 6f70 7469 6f6e 733d 7b22 7761  ite_options={"wa
+00010a00: 6974 5f66 6f72 5f6a 6f62 2220 3a20 4661  it_for_job" : Fa
+00010a10: 6c73 657d 290a 0a20 2020 2020 2020 2020  lse})..         
+00010a20: 2020 2066 6732 203d 2066 732e 6765 745f     fg2 = fs.get_
+00010a30: 6f72 5f63 7265 6174 655f 6665 6174 7572  or_create_featur
+00010a40: 655f 6772 6f75 7028 0a20 2020 2020 2020  e_group(.       
+00010a50: 2020 2020 2020 2020 206e 616d 653d 2766           name='f
+00010a60: 6561 7475 7265 5f67 726f 7570 5f6e 616d  eature_group_nam
+00010a70: 6532 272c 0a20 2020 2020 2020 2020 2020  e2',.           
+00010a80: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00010a90: 3d27 4465 7363 7269 7074 696f 6e20 6f66  ='Description of
+00010aa0: 2074 6865 2073 6563 6f6e 6420 4647 272c   the second FG',
+00010ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010ac0: 2076 6572 7369 6f6e 3d31 2c0a 2020 2020   version=1,.    
+00010ad0: 2020 2020 2020 2020 2020 2020 7072 696d              prim
+00010ae0: 6172 795f 6b65 793d 5b27 756e 6978 275d  ary_key=['unix']
+00010af0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010b00: 2020 6f6e 6c69 6e65 5f65 6e61 626c 6564    online_enabled
+00010b10: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00010b20: 2020 2020 2020 2065 7665 6e74 5f74 696d         event_tim
+00010b30: 653d 2775 6e69 7827 0a20 2020 2020 2020  e='unix'.       
+00010b40: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00010b50: 2020 2066 672e 696e 7365 7274 2864 665f     fg.insert(df_
+00010b60: 666f 725f 6667 3229 0a20 2020 2020 2020  for_fg2).       
+00010b70: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
+00010b80: 2020 2320 4172 6775 6d65 6e74 730a 2020    # Arguments.  
+00010b90: 2020 2020 2020 2020 2020 6665 6174 7572            featur
+00010ba0: 6573 3a20 4461 7461 4672 616d 652c 2052  es: DataFrame, R
+00010bb0: 4444 2c20 4e64 6172 7261 792c 206c 6973  DD, Ndarray, lis
+00010bc0: 742e 2046 6561 7475 7265 7320 746f 2062  t. Features to b
+00010bd0: 6520 7361 7665 642e 0a20 2020 2020 2020  e saved..       
+00010be0: 2020 2020 206f 7665 7277 7269 7465 3a20       overwrite: 
+00010bf0: 4472 6f70 2061 6c6c 2064 6174 6120 696e  Drop all data in
+00010c00: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
+00010c10: 7570 2062 6566 6f72 650a 2020 2020 2020  up before.      
+00010c20: 2020 2020 2020 2020 2020 696e 7365 7274            insert
+00010c30: 696e 6720 6e65 7720 6461 7461 2e20 5468  ing new data. Th
+00010c40: 6973 2064 6f65 7320 6e6f 7420 6166 6665  is does not affe
+00010c50: 6374 206d 6574 6164 6174 612c 2064 6566  ct metadata, def
+00010c60: 6175 6c74 7320 746f 2046 616c 7365 2e0a  aults to False..
+00010c70: 2020 2020 2020 2020 2020 2020 6f70 6572              oper
+00010c80: 6174 696f 6e3a 2041 7061 6368 6520 4875  ation: Apache Hu
+00010c90: 6469 206f 7065 7261 7469 6f6e 2074 7970  di operation typ
+00010ca0: 6520 6022 696e 7365 7274 2260 206f 7220  e `"insert"` or 
+00010cb0: 6022 7570 7365 7274 2260 2e0a 2020 2020  `"upsert"`..    
+00010cc0: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+00010cd0: 756c 7473 2074 6f20 6022 7570 7365 7274  ults to `"upsert
+00010ce0: 2260 2e0a 2020 2020 2020 2020 2020 2020  "`..            
+00010cf0: 7374 6f72 6167 653a 204f 7665 7277 7269  storage: Overwri
+00010d00: 7465 2064 6566 6175 6c74 2062 6568 6176  te default behav
+00010d10: 696f 7572 2c20 7772 6974 6520 746f 206f  iour, write to o
+00010d20: 6666 6c69 6e65 0a20 2020 2020 2020 2020  ffline.         
+00010d30: 2020 2020 2020 2073 746f 7261 6765 206f         storage o
+00010d40: 6e6c 7920 7769 7468 2060 226f 6666 6c69  nly with `"offli
+00010d50: 6e65 2260 206f 7220 6f6e 6c69 6e65 206f  ne"` or online o
+00010d60: 6e6c 7920 7769 7468 2060 226f 6e6c 696e  nly with `"onlin
+00010d70: 6522 602c 2064 6566 6175 6c74 730a 2020  e"`, defaults.  
+00010d80: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00010d90: 2060 4e6f 6e65 602e 0a20 2020 2020 2020   `None`..       
+00010da0: 2020 2020 2077 7269 7465 5f6f 7074 696f       write_optio
+00010db0: 6e73 3a20 4164 6469 7469 6f6e 616c 2077  ns: Additional w
+00010dc0: 7269 7465 206f 7074 696f 6e73 2061 7320  rite options as 
+00010dd0: 6b65 792d 7661 6c75 6520 7061 6972 732c  key-value pairs,
+00010de0: 2064 6566 6175 6c74 7320 746f 2060 7b7d   defaults to `{}
+00010df0: 602e 0a20 2020 2020 2020 2020 2020 2020  `..             
+00010e00: 2020 2057 6865 6e20 7573 696e 6720 7468     When using th
+00010e10: 6520 6070 7974 686f 6e60 2065 6e67 696e  e `python` engin
+00010e20: 652c 2077 7269 7465 5f6f 7074 696f 6e73  e, write_options
+00010e30: 2063 616e 2063 6f6e 7461 696e 2074 6865   can contain the
+00010e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010e50: 2066 6f6c 6c6f 7769 6e67 2065 6e74 7269   following entri
+00010e60: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00010e70: 2020 2020 2a20 6b65 7920 6073 7061 726b      * key `spark
+00010e80: 6020 616e 6420 7661 6c75 6520 616e 206f  ` and value an o
+00010e90: 626a 6563 7420 6f66 2074 7970 650a 2020  bject of type.  
+00010ea0: 2020 2020 2020 2020 2020 2020 2020 5b68                [h
+00010eb0: 7366 732e 636f 7265 2e6a 6f62 5f63 6f6e  sfs.core.job_con
+00010ec0: 6669 6775 7261 7469 6f6e 2e4a 6f62 436f  figuration.JobCo
+00010ed0: 6e66 6967 7572 6174 696f 6e5d 282e 2e2f  nfiguration](../
+00010ee0: 6a6f 625f 636f 6e66 6967 7572 6174 696f  job_configuratio
+00010ef0: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
+00010f00: 2020 2020 2074 6f20 636f 6e66 6967 7572       to configur
+00010f10: 6520 7468 6520 486f 7073 776f 726b 7320  e the Hopsworks 
+00010f20: 4a6f 6220 7573 6564 2074 6f20 7772 6974  Job used to writ
+00010f30: 6520 6461 7461 2069 6e74 6f20 7468 650a  e data into the.
+00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f50: 2020 6665 6174 7572 6520 6772 6f75 702e    feature group.
+00010f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f70: 202a 206b 6579 2060 7761 6974 5f66 6f72   * key `wait_for
+00010f80: 5f6a 6f62 6020 616e 6420 7661 6c75 6520  _job` and value 
+00010f90: 6054 7275 6560 206f 7220 6046 616c 7365  `True` or `False
+00010fa0: 6020 746f 2063 6f6e 6669 6775 7265 0a20  ` to configure. 
+00010fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fc0: 2077 6865 7468 6572 206f 7220 6e6f 7420   whether or not 
+00010fd0: 746f 2074 6865 2069 6e73 6572 7420 6361  to the insert ca
+00010fe0: 6c6c 2073 686f 756c 6420 7265 7475 726e  ll should return
+00010ff0: 206f 6e6c 790a 2020 2020 2020 2020 2020   only.          
+00011000: 2020 2020 2020 2020 6166 7465 7220 7468          after th
+00011010: 6520 486f 7073 776f 726b 7320 4a6f 6220  e Hopsworks Job 
+00011020: 6861 7320 6669 6e69 7368 6564 2e20 4279  has finished. By
+00011030: 2064 6566 6175 6c74 2069 7420 7761 6974   default it wait
+00011040: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+00011050: 2020 202a 206b 6579 2060 7374 6172 745f     * key `start_
+00011060: 6f66 666c 696e 655f 6261 636b 6669 6c6c  offline_backfill
+00011070: 6020 616e 6420 7661 6c75 6520 6054 7275  ` and value `Tru
+00011080: 6560 206f 7220 6046 616c 7365 6020 746f  e` or `False` to
+00011090: 2063 6f6e 6669 6775 7265 0a20 2020 2020   configure.     
+000110a0: 2020 2020 2020 2020 2020 2020 2077 6865               whe
+000110b0: 7468 6572 206f 7220 6e6f 7420 746f 2073  ther or not to s
+000110c0: 7461 7274 2074 6865 2062 6163 6b66 696c  tart the backfil
+000110d0: 6c20 6a6f 6220 746f 2077 7269 7465 2064  l job to write d
+000110e0: 6174 6120 746f 2074 6865 206f 6666 6c69  ata to the offli
+000110f0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+00011100: 2020 2020 2073 746f 7261 6765 2e20 4279       storage. By
+00011110: 2064 6566 6175 6c74 2074 6865 2062 6163   default the bac
+00011120: 6b66 696c 6c20 6a6f 6220 6765 7473 2073  kfill job gets s
+00011130: 7461 7274 6564 2069 6d6d 6564 6961 7465  tarted immediate
+00011140: 6c79 2e0a 2020 2020 2020 2020 2020 2020  ly..            
+00011150: 2020 2020 2a20 6b65 7920 6069 6e74 6572      * key `inter
+00011160: 6e61 6c5f 6b61 666b 6160 2061 6e64 2076  nal_kafka` and v
+00011170: 616c 7565 2060 5472 7565 6020 6f72 2060  alue `True` or `
+00011180: 4661 6c73 6560 2069 6e20 6361 7365 2079  False` in case y
+00011190: 6f75 2065 7374 6162 6c69 7368 6564 0a20  ou established. 
+000111a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111b0: 2063 6f6e 6e65 6374 6976 6974 7920 6672   connectivity fr
+000111c0: 6f6d 2079 6f75 2050 7974 686f 6e20 656e  om you Python en
+000111d0: 7669 726f 6e6d 656e 7420 746f 2074 6865  vironment to the
+000111e0: 2069 6e74 6572 6e61 6c20 6164 7665 7274   internal advert
+000111f0: 6973 6564 0a20 2020 2020 2020 2020 2020  ised.           
+00011200: 2020 2020 2020 206c 6973 7465 6e65 7273         listeners
+00011210: 206f 6620 7468 6520 486f 7073 776f 726b   of the Hopswork
+00011220: 7320 4b61 666b 6120 436c 7573 7465 722e  s Kafka Cluster.
+00011230: 2044 6566 6175 6c74 7320 746f 2060 4661   Defaults to `Fa
+00011240: 6c73 6560 2061 6e64 0a20 2020 2020 2020  lse` and.       
+00011250: 2020 2020 2020 2020 2020 2077 696c 6c20             will 
+00011260: 7573 6520 6578 7465 726e 616c 206c 6973  use external lis
+00011270: 7465 6e65 7273 2077 6865 6e20 636f 6e6e  teners when conn
+00011280: 6563 7469 6e67 2066 726f 6d20 6f75 7473  ecting from outs
+00011290: 6964 6520 6f66 2048 6f70 7377 6f72 6b73  ide of Hopsworks
+000112a0: 2e0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+000112b0: 6c69 6461 7469 6f6e 5f6f 7074 696f 6e73  lidation_options
+000112c0: 3a20 4164 6469 7469 6f6e 616c 2076 616c  : Additional val
+000112d0: 6964 6174 696f 6e20 6f70 7469 6f6e 7320  idation options 
+000112e0: 6173 206b 6579 2d76 616c 7565 2070 6169  as key-value pai
+000112f0: 7273 2c20 6465 6661 756c 7473 2074 6f20  rs, defaults to 
+00011300: 607b 7d60 2e0a 2020 2020 2020 2020 2020  `{}`..          
+00011310: 2020 2020 2020 2a20 6b65 7920 6072 756e        * key `run
+00011320: 5f76 616c 6964 6174 696f 6e60 2062 6f6f  _validation` boo
+00011330: 6c65 616e 2076 616c 7565 2c20 7365 7420  lean value, set 
+00011340: 746f 2060 4661 6c73 6560 2074 6f20 736b  to `False` to sk
+00011350: 6970 2076 616c 6964 6174 696f 6e20 7465  ip validation te
+00011360: 6d70 6f72 6172 696c 7920 6f6e 2069 6e67  mporarily on ing
+00011370: 6573 7469 6f6e 2e0a 2020 2020 2020 2020  estion..        
+00011380: 2020 2020 2020 2020 2a20 6b65 7920 6073          * key `s
+00011390: 6176 655f 7265 706f 7274 6020 626f 6f6c  ave_report` bool
+000113a0: 6561 6e20 7661 6c75 652c 2073 6574 2074  ean value, set t
+000113b0: 6f20 6046 616c 7365 6020 746f 2073 6b69  o `False` to ski
+000113c0: 7020 7570 6c6f 6164 206f 6620 7468 6520  p upload of the 
+000113d0: 7661 6c69 6461 7469 6f6e 2072 6570 6f72  validation repor
+000113e0: 7420 746f 2048 6f70 7377 6f72 6b73 2e0a  t to Hopsworks..
+000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011400: 2a20 6b65 7920 6067 655f 7661 6c69 6461  * key `ge_valida
+00011410: 7465 5f6b 7761 7267 7360 2061 2064 6963  te_kwargs` a dic
+00011420: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
+00011430: 6e67 206b 7761 7267 7320 666f 7220 7468  ng kwargs for th
+00011440: 6520 7661 6c69 6461 7465 206d 6574 686f  e validate metho
+00011450: 6420 6f66 2047 7265 6174 2045 7870 6563  d of Great Expec
+00011460: 7461 7469 6f6e 732e 0a20 2020 2020 2020  tations..       
+00011470: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
+00011480: 6665 7463 685f 6578 7065 6374 6174 696f  fetch_expectatio
+00011490: 6e5f 7375 6974 6560 2061 2062 6f6f 6c65  n_suite` a boole
+000114a0: 616e 2076 616c 7565 2c20 6279 2064 6566  an value, by def
+000114b0: 6175 6c74 2060 5472 7565 602c 2074 6f20  ault `True`, to 
+000114c0: 636f 6e74 726f 6c20 7768 6574 6865 7220  control whether 
+000114d0: 7468 6520 6578 7065 6374 6174 696f 6e0a  the expectation.
+000114e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114f0: 2020 2073 7569 7465 206f 6620 7468 6520     suite of the 
+00011500: 6665 6174 7572 6520 6772 6f75 7020 7368  feature group sh
+00011510: 6f75 6c64 2062 6520 6665 7463 6865 6420  ould be fetched 
+00011520: 6265 666f 7265 2065 7665 7279 2069 6e73  before every ins
+00011530: 6572 742e 0a20 2020 2020 2020 2020 2020  ert..           
+00011540: 2073 6176 655f 636f 6465 3a20 5768 656e   save_code: When
+00011550: 2072 756e 6e69 6e67 2048 5346 5320 6f6e   running HSFS on
+00011560: 2048 6f70 7377 6f72 6b73 206f 7220 4461   Hopsworks or Da
+00011570: 7461 6272 6963 6b73 2c20 4853 4653 2063  tabricks, HSFS c
+00011580: 616e 2073 6176 6520 7468 6520 636f 6465  an save the code
+00011590: 2f6e 6f74 6562 6f6f 6b20 7573 6564 2074  /notebook used t
+000115a0: 6f20 6372 6561 7465 0a20 2020 2020 2020  o create.       
+000115b0: 2020 2020 2020 2020 2074 6865 2066 6561           the fea
+000115c0: 7475 7265 2067 726f 7570 206f 7220 7573  ture group or us
+000115d0: 6564 2074 6f20 696e 7365 7274 2064 6174  ed to insert dat
+000115e0: 6120 746f 2069 742e 2057 6865 6e20 6361  a to it. When ca
+000115f0: 6c6c 696e 6720 7468 6520 6069 6e73 6572  lling the `inser
+00011600: 7460 206d 6574 686f 6420 7265 7065 6174  t` method repeat
+00011610: 6564 6c79 0a20 2020 2020 2020 2020 2020  edly.           
+00011620: 2020 2020 2077 6974 6820 736d 616c 6c20       with small 
+00011630: 6261 7463 6865 7320 6f66 2064 6174 612c  batches of data,
+00011640: 2074 6869 7320 6361 6e20 736c 6f77 2064   this can slow d
+00011650: 6f77 6e20 7468 6520 7772 6974 6573 2e20  own the writes. 
+00011660: 5573 6520 7468 6973 206f 7074 696f 6e20  Use this option 
+00011670: 746f 2074 7572 6e20 6f66 6620 7361 7669  to turn off savi
+00011680: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
+00011690: 2020 2063 6f64 652e 2044 6566 6175 6c74     code. Default
+000116a0: 7320 746f 2060 5472 7565 602e 0a0a 2020  s to `True`...  
+000116b0: 2020 2020 2020 2320 5265 7475 726e 730a        # Returns.
+000116c0: 2020 2020 2020 2020 2020 2020 2860 4a6f              (`Jo
+000116d0: 6260 2c20 6056 616c 6964 6174 696f 6e52  b`, `ValidationR
+000116e0: 6570 6f72 7460 2920 4120 7475 706c 6520  eport`) A tuple 
+000116f0: 7769 7468 206a 6f62 2069 6e66 6f72 6d61  with job informa
+00011700: 7469 6f6e 2069 6620 7079 7468 6f6e 2065  tion if python e
+00011710: 6e67 696e 6520 6973 2075 7365 6420 616e  ngine is used an
+00011720: 6420 7468 6520 7661 6c69 6461 7469 6f6e  d the validation
+00011730: 2072 6570 6f72 7420 6966 2076 616c 6964   report if valid
+00011740: 6174 696f 6e20 6973 2065 6e61 626c 6564  ation is enabled
+00011750: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00011760: 2020 2020 2020 6665 6174 7572 655f 6461        feature_da
+00011770: 7461 6672 616d 6520 3d20 656e 6769 6e65  taframe = engine
+00011780: 2e67 6574 5f69 6e73 7461 6e63 6528 292e  .get_instance().
+00011790: 636f 6e76 6572 745f 746f 5f64 6566 6175  convert_to_defau
+000117a0: 6c74 5f64 6174 6166 7261 6d65 2866 6561  lt_dataframe(fea
+000117b0: 7475 7265 7329 0a0a 2020 2020 2020 2020  tures)..        
+000117c0: 6a6f 622c 2067 655f 7265 706f 7274 203d  job, ge_report =
+000117d0: 2073 656c 662e 5f66 6561 7475 7265 5f67   self._feature_g
+000117e0: 726f 7570 5f65 6e67 696e 652e 696e 7365  roup_engine.inse
+000117f0: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
+00011800: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00011810: 2020 6665 6174 7572 655f 6461 7461 6672    feature_datafr
+00011820: 616d 653d 6665 6174 7572 655f 6461 7461  ame=feature_data
+00011830: 6672 616d 652c 0a20 2020 2020 2020 2020  frame,.         
+00011840: 2020 206f 7665 7277 7269 7465 3d6f 7665     overwrite=ove
+00011850: 7277 7269 7465 2c0a 2020 2020 2020 2020  rwrite,.        
+00011860: 2020 2020 6f70 6572 6174 696f 6e3d 6f70      operation=op
+00011870: 6572 6174 696f 6e2c 0a20 2020 2020 2020  eration,.       
+00011880: 2020 2020 2073 746f 7261 6765 3d73 746f       storage=sto
+00011890: 7261 6765 2e6c 6f77 6572 2829 2069 6620  rage.lower() if 
+000118a0: 7374 6f72 6167 6520 6973 206e 6f74 204e  storage is not N
+000118b0: 6f6e 6520 656c 7365 204e 6f6e 652c 0a20  one else None,. 
+000118c0: 2020 2020 2020 2020 2020 2077 7269 7465             write
+000118d0: 5f6f 7074 696f 6e73 3d77 7269 7465 5f6f  _options=write_o
+000118e0: 7074 696f 6e73 2c0a 2020 2020 2020 2020  ptions,.        
+000118f0: 2020 2020 7661 6c69 6461 7469 6f6e 5f6f      validation_o
+00011900: 7074 696f 6e73 3d7b 2273 6176 655f 7265  ptions={"save_re
+00011910: 706f 7274 223a 2054 7275 652c 202a 2a76  port": True, **v
+00011920: 616c 6964 6174 696f 6e5f 6f70 7469 6f6e  alidation_option
+00011930: 737d 2c0a 2020 2020 2020 2020 290a 2020  s},.        ).  
+00011940: 2020 2020 2020 6966 2073 6176 655f 636f        if save_co
+00011950: 6465 2061 6e64 2028 0a20 2020 2020 2020  de and (.       
+00011960: 2020 2020 2067 655f 7265 706f 7274 2069       ge_report i
+00011970: 7320 4e6f 6e65 206f 7220 6765 5f72 6570  s None or ge_rep
+00011980: 6f72 742e 696e 6765 7374 696f 6e5f 7265  ort.ingestion_re
+00011990: 7375 6c74 203d 3d20 2249 4e47 4553 5445  sult == "INGESTE
+000119a0: 4422 0a20 2020 2020 2020 2029 3a0a 2020  D".        ):.  
+000119b0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000119c0: 636f 6465 5f65 6e67 696e 652e 7361 7665  code_engine.save
+000119d0: 5f63 6f64 6528 7365 6c66 290a 0a20 2020  _code(self)..   
+000119e0: 2020 2020 2069 6620 656e 6769 6e65 2e67       if engine.g
+000119f0: 6574 5f74 7970 6528 2920 3d3d 2022 7370  et_type() == "sp
+00011a00: 6172 6b22 3a0a 2020 2020 2020 2020 2020  ark":.          
+00011a10: 2020 2320 4f6e 6c79 2063 6f6d 7075 7465    # Only compute
+00011a20: 2073 7461 7469 7374 6963 7320 6966 2074   statistics if t
+00011a30: 6865 2065 6e67 696e 6520 6973 2053 7061  he engine is Spa
+00011a40: 726b 2c0a 2020 2020 2020 2020 2020 2020  rk,.            
+00011a50: 2320 6966 2050 7974 686f 6e2c 2074 6865  # if Python, the
+00011a60: 2073 7461 7469 7374 6963 7320 6172 6520   statistics are 
+00011a70: 636f 6d70 7574 6564 2062 7920 7468 6520  computed by the 
+00011a80: 6170 706c 6963 6174 696f 6e20 646f 696e  application doin
+00011a90: 6720 7468 6520 696e 7365 7274 0a20 2020  g the insert.   
+00011aa0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00011ab0: 6d70 7574 655f 7374 6174 6973 7469 6373  mpute_statistics
+00011ac0: 2829 0a0a 2020 2020 2020 2020 7265 7475  ()..        retu
+00011ad0: 726e 2028 0a20 2020 2020 2020 2020 2020  rn (.           
+00011ae0: 206a 6f62 2c0a 2020 2020 2020 2020 2020   job,.          
+00011af0: 2020 6765 5f72 6570 6f72 742e 746f 5f67    ge_report.to_g
+00011b00: 655f 7479 7065 2829 2069 6620 6765 5f72  e_type() if ge_r
+00011b10: 6570 6f72 7420 6973 206e 6f74 204e 6f6e  eport is not Non
+00011b20: 6520 656c 7365 204e 6f6e 652c 0a20 2020  e else None,.   
+00011b30: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00011b40: 6d75 6c74 695f 7061 7274 5f69 6e73 6572  multi_part_inser
+00011b50: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
+00011b60: 0a20 2020 2020 2020 2066 6561 7475 7265  .        feature
+00011b70: 733a 2055 6e69 6f6e 5b0a 2020 2020 2020  s: Union[.      
+00011b80: 2020 2020 2020 7064 2e44 6174 6146 7261        pd.DataFra
+00011b90: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00011ba0: 5479 7065 5661 7228 2270 7973 7061 726b  TypeVar("pyspark
+00011bb0: 2e73 716c 2e44 6174 6146 7261 6d65 2229  .sql.DataFrame")
+00011bc0: 2c20 2023 206e 6f71 613a 2046 3832 310a  ,  # noqa: F821.
+00011bd0: 2020 2020 2020 2020 2020 2020 5479 7065              Type
+00011be0: 5661 7228 2270 7973 7061 726b 2e52 4444  Var("pyspark.RDD
+00011bf0: 2229 2c20 2023 206e 6f71 613a 2046 3832  "),  # noqa: F82
+00011c00: 310a 2020 2020 2020 2020 2020 2020 6e70  1.            np
+00011c10: 2e6e 6461 7272 6179 2c0a 2020 2020 2020  .ndarray,.      
+00011c20: 2020 2020 2020 4c69 7374 5b6c 6973 745d        List[list]
+00011c30: 2c0a 2020 2020 2020 2020 5d20 3d20 4e6f  ,.        ] = No
+00011c40: 6e65 2c0a 2020 2020 2020 2020 6f76 6572  ne,.        over
+00011c50: 7772 6974 653a 204f 7074 696f 6e61 6c5b  write: Optional[
+00011c60: 626f 6f6c 5d20 3d20 4661 6c73 652c 0a20  bool] = False,. 
+00011c70: 2020 2020 2020 206f 7065 7261 7469 6f6e         operation
+00011c80: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00011c90: 3d20 2275 7073 6572 7422 2c0a 2020 2020  = "upsert",.    
+00011ca0: 2020 2020 7374 6f72 6167 653a 204f 7074      storage: Opt
+00011cb0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00011cc0: 652c 0a20 2020 2020 2020 2077 7269 7465  e,.        write
+00011cd0: 5f6f 7074 696f 6e73 3a20 4f70 7469 6f6e  _options: Option
+00011ce0: 616c 5b44 6963 745b 7374 722c 2041 6e79  al[Dict[str, Any
+00011cf0: 5d5d 203d 207b 7d2c 0a20 2020 2020 2020  ]] = {},.       
+00011d00: 2076 616c 6964 6174 696f 6e5f 6f70 7469   validation_opti
+00011d10: 6f6e 733a 204f 7074 696f 6e61 6c5b 4469  ons: Optional[Di
+00011d20: 6374 5b73 7472 2c20 416e 795d 5d20 3d20  ct[str, Any]] = 
+00011d30: 7b7d 2c0a 2020 2020 2920 2d3e 2055 6e69  {},.    ) -> Uni
+00011d40: 6f6e 5b0a 2020 2020 2020 2020 5475 706c  on[.        Tupl
+00011d50: 655b 4f70 7469 6f6e 616c 5b4a 6f62 5d2c  e[Optional[Job],
+00011d60: 204f 7074 696f 6e61 6c5b 5661 6c69 6461   Optional[Valida
+00011d70: 7469 6f6e 5265 706f 7274 5d5d 2c0a 2020  tionReport]],.  
+00011d80: 2020 2020 2020 6665 6174 7572 655f 6772        feature_gr
+00011d90: 6f75 705f 7772 6974 6572 2e46 6561 7475  oup_writer.Featu
+00011da0: 7265 4772 6f75 7057 7269 7465 722c 0a20  reGroupWriter,. 
+00011db0: 2020 205d 3a0a 2020 2020 2020 2020 2222     ]:.        ""
+00011dc0: 2247 6574 2046 6561 7475 7265 4772 6f75  "Get FeatureGrou
+00011dd0: 7057 7269 7465 7220 666f 7220 6f70 7469  pWriter for opti
+00011de0: 6d69 7a65 6420 6d75 6c74 6920 7061 7274  mized multi part
+00011df0: 2069 6e73 6572 7473 206f 7220 6361 6c6c   inserts or call
+00011e00: 2074 6869 7320 6d65 7468 6f64 0a20 2020   this method.   
+00011e10: 2020 2020 2074 6f20 7374 6172 7420 6d61       to start ma
+00011e20: 6e75 616c 206d 756c 7469 2070 6172 7420  nual multi part 
+00011e30: 6f70 7469 6d69 7a65 6420 696e 7365 7274  optimized insert
+00011e40: 732e 0a0a 2020 2020 2020 2020 496e 2075  s...        In u
+00011e50: 7365 2063 6173 6573 2077 6865 7265 2076  se cases where v
+00011e60: 6572 7920 736d 616c 6c20 6261 7463 6865  ery small batche
+00011e70: 7320 2831 2074 6f20 3130 3030 2920 726f  s (1 to 1000) ro
+00011e80: 7773 2070 6572 2044 6174 6166 7261 6d65  ws per Dataframe
+00011e90: 206e 6565 640a 2020 2020 2020 2020 746f   need.        to
+00011ea0: 2062 6520 7772 6974 7465 6e20 746f 2074   be written to t
+00011eb0: 6865 2066 6561 7475 7265 2073 746f 7265  he feature store
+00011ec0: 2072 6570 6561 7465 646c 792c 2069 7420   repeatedly, it 
+00011ed0: 6d69 6768 7420 6265 2069 6e65 6666 6963  might be ineffic
+00011ee0: 6965 6e74 2074 6f20 7573 650a 2020 2020  ient to use.    
+00011ef0: 2020 2020 7468 6520 7374 616e 6461 7264      the standard
+00011f00: 2060 6665 6174 7572 655f 6772 6f75 702e   `feature_group.
+00011f10: 696e 7365 7274 2829 6020 6d65 7468 6f64  insert()` method
+00011f20: 2061 7320 6974 2070 6572 666f 726d 7320   as it performs 
+00011f30: 736f 6d65 2062 6163 6b67 726f 756e 640a  some background.
+00011f40: 2020 2020 2020 2020 6163 7469 6f6e 7320          actions 
+00011f50: 746f 2075 7064 6174 6520 7468 6520 6d65  to update the me
+00011f60: 7461 6461 7461 206f 6620 7468 6520 6665  tadata of the fe
+00011f70: 6174 7572 6520 6772 6f75 7020 6f62 6a65  ature group obje
+00011f80: 6374 2066 6972 7374 2e0a 0a20 2020 2020  ct first...     
+00011f90: 2020 2046 6f72 2074 6865 7365 2063 6173     For these cas
+00011fa0: 6573 2c20 7468 6520 6665 6174 7572 6520  es, the feature 
+00011fb0: 6772 6f75 7020 7072 6f76 6964 6573 2074  group provides t
+00011fc0: 6865 2060 6d75 6c74 695f 7061 7274 5f69  he `multi_part_i
+00011fd0: 6e73 6572 7460 2041 5049 2c0a 2020 2020  nsert` API,.    
+00011fe0: 2020 2020 7768 6963 6820 6973 206f 7074      which is opt
+00011ff0: 696d 697a 6564 2066 6f72 2077 7269 7469  imized for writi
+00012000: 6e67 206d 616e 7920 736d 616c 6c20 4461  ng many small Da
+00012010: 7461 6672 616d 6573 2061 6674 6572 2061  taframes after a
+00012020: 6e6f 7468 6572 2e0a 0a20 2020 2020 2020  nother...       
+00012030: 2054 6865 7265 2061 7265 2074 776f 2077   There are two w
+00012040: 6179 7320 746f 2075 7365 2074 6869 7320  ays to use this 
+00012050: 4150 493a 0a20 2020 2020 2020 2021 2121  API:.        !!!
+00012060: 2065 7861 6d70 6c65 2022 5079 7468 6f6e   example "Python
+00012070: 2043 6f6e 7465 7874 204d 616e 6167 6572   Context Manager
+00012080: 220a 2020 2020 2020 2020 2020 2020 5573  ".            Us
+00012090: 696e 6720 7468 6520 5079 7468 6f6e 2060  ing the Python `
+000120a0: 7769 7468 6020 7379 6e74 6178 2079 6f75  with` syntax you
+000120b0: 2063 616e 2061 6371 7569 7265 2061 2046   can acquire a F
+000120c0: 6561 7475 7265 4772 6f75 7057 7269 7465  eatureGroupWrite
+000120d0: 720a 2020 2020 2020 2020 2020 2020 6f62  r.            ob
+000120e0: 6a65 6374 2074 6861 7420 696d 706c 656d  ject that implem
+000120f0: 656e 7473 2074 6865 2073 616d 6520 606d  ents the same `m
+00012100: 756c 7469 5f70 6172 745f 696e 7365 7274  ulti_part_insert
+00012110: 6020 4150 492e 0a20 2020 2020 2020 2020  ` API..         
+00012120: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+00012130: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+00012140: 5f67 726f 7570 203d 2066 732e 6765 745f  _group = fs.get_
+00012150: 6f72 5f63 7265 6174 655f 6665 6174 7572  or_create_featur
+00012160: 655f 6772 6f75 7028 2266 675f 6e61 6d65  e_group("fg_name
+00012170: 222c 2076 6572 7369 6f6e 3d31 290a 0a20  ", version=1).. 
+00012180: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00012190: 6665 6174 7572 655f 6772 6f75 702e 6d75  feature_group.mu
+000121a0: 6c74 695f 7061 7274 5f69 6e73 6572 7428  lti_part_insert(
+000121b0: 2920 6173 2077 7269 7465 723a 0a20 2020  ) as writer:.   
+000121c0: 2020 2020 2020 2020 2020 2020 2023 2072               # r
+000121d0: 756e 2069 6e73 6572 7473 2069 6e20 6120  un inserts in a 
+000121e0: 6c6f 6f70 3a0a 2020 2020 2020 2020 2020  loop:.          
+000121f0: 2020 2020 2020 7768 696c 6520 6c6f 6f70        while loop
+00012200: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012210: 2020 2020 2020 736d 616c 6c5f 6261 7463        small_batc
+00012220: 685f 6466 203d 202e 2e2e 0a20 2020 2020  h_df = ....     
+00012230: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00012240: 7269 7465 722e 6d75 6c74 695f 7061 7274  riter.multi_part
+00012250: 5f69 6e73 6572 7428 736d 616c 6c5f 6261  _insert(small_ba
+00012260: 7463 685f 6466 290a 2020 2020 2020 2020  tch_df).        
+00012270: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
+00012280: 2020 2020 5468 6520 7772 6974 6572 2062      The writer b
+00012290: 6174 6368 6573 2074 6865 2073 6d61 6c6c  atches the small
+000122a0: 2044 6174 6166 7261 6d65 7320 616e 6420   Dataframes and 
+000122b0: 7472 616e 736d 6974 7320 7468 656d 2074  transmits them t
+000122c0: 6f20 486f 7073 776f 726b 730a 2020 2020  o Hopsworks.    
+000122d0: 2020 2020 2020 2020 6566 6669 6369 656e          efficien
+000122e0: 746c 792e 0a20 2020 2020 2020 2020 2020  tly..           
+000122f0: 2057 6865 6e20 6578 6974 696e 6720 7468   When exiting th
+00012300: 6520 636f 6e74 6578 742c 2074 6865 2066  e context, the f
+00012310: 6561 7475 7265 2067 726f 7570 2077 7269  eature group wri
+00012320: 7465 7220 6973 2073 7572 6520 746f 2065  ter is sure to e
+00012330: 7869 740a 2020 2020 2020 2020 2020 2020  xit.            
+00012340: 6f6e 6c79 206f 6e63 6520 616c 6c20 7468  only once all th
+00012350: 6520 726f 7773 2068 6176 6520 6265 656e  e rows have been
+00012360: 2074 7261 6e73 6d69 7474 6564 2e0a 0a20   transmitted... 
+00012370: 2020 2020 2020 2021 2121 2065 7861 6d70         !!! examp
+00012380: 6c65 2022 4d75 6c74 6920 7061 7274 2069  le "Multi part i
+00012390: 6e73 6572 7420 7769 7468 206d 616e 7561  nsert with manua
+000123a0: 6c20 636f 6e74 6578 7420 6d61 6e61 6765  l context manage
+000123b0: 6d65 6e74 220a 2020 2020 2020 2020 2020  ment".          
+000123c0: 2020 496e 7374 6561 6420 6f66 206c 6574    Instead of let
+000123d0: 7469 6e67 2050 7974 686f 6e20 6861 6e64  ting Python hand
+000123e0: 6c65 2074 6865 2065 6e74 6572 696e 6720  le the entering 
+000123f0: 616e 6420 6578 6974 696e 6720 6f66 2074  and exiting of t
+00012400: 6865 0a20 2020 2020 2020 2020 2020 206d  he.            m
+00012410: 756c 7469 2070 6172 7420 696e 7365 7274  ulti part insert
+00012420: 2063 6f6e 7465 7874 2c20 796f 7520 6361   context, you ca
+00012430: 6e20 7374 6172 7420 616e 6420 6669 6e61  n start and fina
+00012440: 6c69 7a65 2074 6865 2063 6f6e 7465 7874  lize the context
+00012450: 0a20 2020 2020 2020 2020 2020 206d 616e  .            man
+00012460: 7561 6c6c 792e 0a20 2020 2020 2020 2020  ually..         
+00012470: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+00012480: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+00012490: 5f67 726f 7570 203d 2066 732e 6765 745f  _group = fs.get_
+000124a0: 6f72 5f63 7265 6174 655f 6665 6174 7572  or_create_featur
+000124b0: 655f 6772 6f75 7028 2266 675f 6e61 6d65  e_group("fg_name
+000124c0: 222c 2076 6572 7369 6f6e 3d31 290a 0a20  ", version=1).. 
+000124d0: 2020 2020 2020 2020 2020 2077 6869 6c65             while
+000124e0: 206c 6f6f 703a 0a20 2020 2020 2020 2020   loop:.         
+000124f0: 2020 2020 2020 2073 6d61 6c6c 5f62 6174         small_bat
+00012500: 6368 5f64 6620 3d20 2e2e 2e0a 2020 2020  ch_df = ....    
+00012510: 2020 2020 2020 2020 2020 2020 6665 6174              feat
+00012520: 7572 655f 6772 6f75 702e 6d75 6c74 695f  ure_group.multi_
+00012530: 7061 7274 5f69 6e73 6572 7428 736d 616c  part_insert(smal
+00012540: 6c5f 6261 7463 685f 6466 290a 0a20 2020  l_batch_df)..   
+00012550: 2020 2020 2020 2020 2023 2049 4d50 4f52           # IMPOR
+00012560: 5441 4e54 3a20 6669 6e61 6c69 7a65 2074  TANT: finalize t
+00012570: 6865 206d 756c 7469 2070 6172 7420 696e  he multi part in
+00012580: 7365 7274 2074 6f20 6d61 6b65 2073 7572  sert to make sur
+00012590: 6520 616c 6c20 726f 7773 0a20 2020 2020  e all rows.     
+000125a0: 2020 2020 2020 2023 2068 6176 6520 6265         # have be
+000125b0: 656e 2074 7261 6e73 6d69 7474 6564 0a20  en transmitted. 
+000125c0: 2020 2020 2020 2020 2020 2066 6561 7475             featu
+000125d0: 7265 5f67 726f 7570 2e66 696e 616c 697a  re_group.finaliz
+000125e0: 655f 6d75 6c74 695f 7061 7274 5f69 6e73  e_multi_part_ins
+000125f0: 6572 7428 290a 2020 2020 2020 2020 2020  ert().          
+00012600: 2020 6060 600a 2020 2020 2020 2020 2020    ```.          
+00012610: 2020 4e6f 7465 2074 6861 7420 7468 6520    Note that the 
+00012620: 6669 7273 7420 6361 6c6c 2074 6f20 606d  first call to `m
+00012630: 756c 7469 5f70 6172 745f 696e 7365 7274  ulti_part_insert
+00012640: 6020 696e 6974 6961 7465 7320 7468 6520  ` initiates the 
+00012650: 636f 6e74 6578 740a 2020 2020 2020 2020  context.        
+00012660: 2020 2020 616e 6420 6265 2073 7572 6520      and be sure 
+00012670: 746f 2066 696e 616c 697a 6520 6974 2e20  to finalize it. 
+00012680: 5468 6520 6066 696e 616c 697a 655f 6d75  The `finalize_mu
+00012690: 6c74 695f 7061 7274 5f69 6e73 6572 7460  lti_part_insert`
+000126a0: 2069 7320 610a 2020 2020 2020 2020 2020   is a.          
+000126b0: 2020 626c 6f63 6b69 6e67 2063 616c 6c20    blocking call 
+000126c0: 7468 6174 2072 6574 7572 6e73 206f 6e63  that returns onc
+000126d0: 6520 616c 6c20 726f 7773 2068 6176 6520  e all rows have 
+000126e0: 6265 656e 2074 7261 6e73 6d69 7474 6564  been transmitted
+000126f0: 2e0a 0a20 2020 2020 2020 2020 2020 204f  ...            O
+00012700: 6e63 6520 796f 7520 6172 6520 646f 6e65  nce you are done
+00012710: 2077 6974 6820 7468 6520 6d75 6c74 6920   with the multi 
+00012720: 7061 7274 2069 6e73 6572 742c 2069 7420  part insert, it 
+00012730: 6973 2067 6f6f 6420 7072 6163 7469 6365  is good practice
+00012740: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
+00012750: 7374 6172 7420 7468 6520 6261 636b 6669  start the backfi
+00012760: 6c6c 206a 6f62 2069 6e20 6f72 6465 7220  ll job in order 
+00012770: 746f 2077 7269 7465 2074 6865 2064 6174  to write the dat
+00012780: 6120 746f 2074 6865 206f 6666 6c69 6e65  a to the offline
+00012790: 0a20 2020 2020 2020 2020 2020 2073 746f  .            sto
+000127a0: 7261 6765 3a0a 2020 2020 2020 2020 2020  rage:.          
+000127b0: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
+000127c0: 2020 2020 2020 2020 6665 6174 7572 655f          feature_
+000127d0: 6772 6f75 702e 6261 636b 6669 6c6c 5f6a  group.backfill_j
+000127e0: 6f62 2e72 756e 2861 7761 6974 5f74 6572  ob.run(await_ter
+000127f0: 6d69 6e61 7469 6f6e 3d54 7275 6529 0a20  mination=True). 
+00012800: 2020 2020 2020 2020 2020 2060 6060 0a0a             ```..
+00012810: 2020 2020 2020 2020 2320 4172 6775 6d65          # Argume
+00012820: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
+00012830: 6665 6174 7572 6573 3a20 4461 7461 4672  features: DataFr
+00012840: 616d 652c 2052 4444 2c20 4e64 6172 7261  ame, RDD, Ndarra
+00012850: 792c 206c 6973 742e 2046 6561 7475 7265  y, list. Feature
+00012860: 7320 746f 2062 6520 7361 7665 642e 0a20  s to be saved.. 
+00012870: 2020 2020 2020 2020 2020 206f 7665 7277             overw
+00012880: 7269 7465 3a20 4472 6f70 2061 6c6c 2064  rite: Drop all d
+00012890: 6174 6120 696e 2074 6865 2066 6561 7475  ata in the featu
+000128a0: 7265 2067 726f 7570 2062 6566 6f72 650a  re group before.
+000128b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128c0: 696e 7365 7274 696e 6720 6e65 7720 6461  inserting new da
+000128d0: 7461 2e20 5468 6973 2064 6f65 7320 6e6f  ta. This does no
+000128e0: 7420 6166 6665 6374 206d 6574 6164 6174  t affect metadat
+000128f0: 612c 2064 6566 6175 6c74 7320 746f 2046  a, defaults to F
+00012900: 616c 7365 2e0a 2020 2020 2020 2020 2020  alse..          
+00012910: 2020 6f70 6572 6174 696f 6e3a 2041 7061    operation: Apa
+00012920: 6368 6520 4875 6469 206f 7065 7261 7469  che Hudi operati
+00012930: 6f6e 2074 7970 6520 6022 696e 7365 7274  on type `"insert
+00012940: 2260 206f 7220 6022 7570 7365 7274 2260  "` or `"upsert"`
+00012950: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012960: 2020 4465 6661 756c 7473 2074 6f20 6022    Defaults to `"
+00012970: 7570 7365 7274 2260 2e0a 2020 2020 2020  upsert"`..      
+00012980: 2020 2020 2020 7374 6f72 6167 653a 204f        storage: O
+00012990: 7665 7277 7269 7465 2064 6566 6175 6c74  verwrite default
+000129a0: 2062 6568 6176 696f 7572 2c20 7772 6974   behaviour, writ
+000129b0: 6520 746f 206f 6666 6c69 6e65 0a20 2020  e to offline.   
+000129c0: 2020 2020 2020 2020 2020 2020 2073 746f               sto
+000129d0: 7261 6765 206f 6e6c 7920 7769 7468 2060  rage only with `
+000129e0: 226f 6666 6c69 6e65 2260 206f 7220 6f6e  "offline"` or on
+000129f0: 6c69 6e65 206f 6e6c 7920 7769 7468 2060  line only with `
+00012a00: 226f 6e6c 696e 6522 602c 2064 6566 6175  "online"`, defau
+00012a10: 6c74 730a 2020 2020 2020 2020 2020 2020  lts.            
+00012a20: 2020 2020 746f 2060 4e6f 6e65 602e 0a20      to `None`.. 
+00012a30: 2020 2020 2020 2020 2020 2077 7269 7465             write
+00012a40: 5f6f 7074 696f 6e73 3a20 4164 6469 7469  _options: Additi
+00012a50: 6f6e 616c 2077 7269 7465 206f 7074 696f  onal write optio
+00012a60: 6e73 2061 7320 6b65 792d 7661 6c75 6520  ns as key-value 
+00012a70: 7061 6972 732c 2064 6566 6175 6c74 7320  pairs, defaults 
+00012a80: 746f 2060 7b7d 602e 0a20 2020 2020 2020  to `{}`..       
+00012a90: 2020 2020 2020 2020 2057 6865 6e20 7573           When us
+00012aa0: 696e 6720 7468 6520 6070 7974 686f 6e60  ing the `python`
+00012ab0: 2065 6e67 696e 652c 2077 7269 7465 5f6f   engine, write_o
+00012ac0: 7074 696f 6e73 2063 616e 2063 6f6e 7461  ptions can conta
+00012ad0: 696e 2074 6865 0a20 2020 2020 2020 2020  in the.         
+00012ae0: 2020 2020 2020 2066 6f6c 6c6f 7769 6e67         following
+00012af0: 2065 6e74 7269 6573 3a0a 2020 2020 2020   entries:.      
+00012b00: 2020 2020 2020 2020 2020 2a20 6b65 7920            * key 
+00012b10: 6073 7061 726b 6020 616e 6420 7661 6c75  `spark` and valu
+00012b20: 6520 616e 206f 626a 6563 7420 6f66 2074  e an object of t
+00012b30: 7970 650a 2020 2020 2020 2020 2020 2020  ype.            
+00012b40: 2020 2020 5b68 7366 732e 636f 7265 2e6a      [hsfs.core.j
+00012b50: 6f62 5f63 6f6e 6669 6775 7261 7469 6f6e  ob_configuration
+00012b60: 2e4a 6f62 436f 6e66 6967 7572 6174 696f  .JobConfiguratio
+00012b70: 6e5d 282e 2e2f 6a6f 625f 636f 6e66 6967  n](../job_config
+00012b80: 7572 6174 696f 6e29 0a20 2020 2020 2020  uration).       
+00012b90: 2020 2020 2020 2020 2020 2074 6f20 636f             to co
+00012ba0: 6e66 6967 7572 6520 7468 6520 486f 7073  nfigure the Hops
+00012bb0: 776f 726b 7320 4a6f 6220 7573 6564 2074  works Job used t
+00012bc0: 6f20 7772 6974 6520 6461 7461 2069 6e74  o write data int
+00012bd0: 6f20 7468 650a 2020 2020 2020 2020 2020  o the.          
+00012be0: 2020 2020 2020 2020 6665 6174 7572 6520          feature 
+00012bf0: 6772 6f75 702e 0a20 2020 2020 2020 2020  group..         
+00012c00: 2020 2020 2020 202a 206b 6579 2060 7761         * key `wa
+00012c10: 6974 5f66 6f72 5f6a 6f62 6020 616e 6420  it_for_job` and 
+00012c20: 7661 6c75 6520 6054 7275 6560 206f 7220  value `True` or 
+00012c30: 6046 616c 7365 6020 746f 2063 6f6e 6669  `False` to confi
+00012c40: 6775 7265 0a20 2020 2020 2020 2020 2020  gure.           
+00012c50: 2020 2020 2020 2077 6865 7468 6572 206f         whether o
+00012c60: 7220 6e6f 7420 746f 2074 6865 2069 6e73  r not to the ins
+00012c70: 6572 7420 6361 6c6c 2073 686f 756c 6420  ert call should 
+00012c80: 7265 7475 726e 206f 6e6c 790a 2020 2020  return only.    
+00012c90: 2020 2020 2020 2020 2020 2020 2020 6166                af
+00012ca0: 7465 7220 7468 6520 486f 7073 776f 726b  ter the Hopswork
+00012cb0: 7320 4a6f 6220 6861 7320 6669 6e69 7368  s Job has finish
+00012cc0: 6564 2e20 4279 2064 6566 6175 6c74 2069  ed. By default i
+00012cd0: 7420 7761 6974 732e 0a20 2020 2020 2020  t waits..       
+00012ce0: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
+00012cf0: 7374 6172 745f 6f66 666c 696e 655f 6261  start_offline_ba
+00012d00: 636b 6669 6c6c 6020 616e 6420 7661 6c75  ckfill` and valu
+00012d10: 6520 6054 7275 6560 206f 7220 6046 616c  e `True` or `Fal
+00012d20: 7365 6020 746f 2063 6f6e 6669 6775 7265  se` to configure
+00012d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012d40: 2020 2077 6865 7468 6572 206f 7220 6e6f     whether or no
+00012d50: 7420 746f 2073 7461 7274 2074 6865 2062  t to start the b
+00012d60: 6163 6b66 696c 6c20 6a6f 6220 746f 2077  ackfill job to w
+00012d70: 7269 7465 2064 6174 6120 746f 2074 6865  rite data to the
+00012d80: 206f 6666 6c69 6e65 0a20 2020 2020 2020   offline.       
+00012d90: 2020 2020 2020 2020 2020 2073 746f 7261             stora
+00012da0: 6765 2e20 4279 2064 6566 6175 6c74 2074  ge. By default t
+00012db0: 6865 2062 6163 6b66 696c 6c20 6a6f 6220  he backfill job 
+00012dc0: 646f 6573 206e 6f74 2067 6574 2073 7461  does not get sta
+00012dd0: 7274 6564 2061 7574 6f6d 6174 6963 616c  rted automatical
+00012de0: 6c79 0a20 2020 2020 2020 2020 2020 2020  ly.             
+00012df0: 2020 2020 2066 6f72 206d 756c 7469 2070       for multi p
+00012e00: 6172 7420 696e 7365 7274 732e 0a20 2020  art inserts..   
+00012e10: 2020 2020 2020 2020 2020 2020 202a 206b               * k
+00012e20: 6579 2060 696e 7465 726e 616c 5f6b 6166  ey `internal_kaf
+00012e30: 6b61 6020 616e 6420 7661 6c75 6520 6054  ka` and value `T
+00012e40: 7275 6560 206f 7220 6046 616c 7365 6020  rue` or `False` 
+00012e50: 696e 2063 6173 6520 796f 7520 6573 7461  in case you esta
+00012e60: 626c 6973 6865 640a 2020 2020 2020 2020  blished.        
+00012e70: 2020 2020 2020 2020 2020 636f 6e6e 6563            connec
+00012e80: 7469 7669 7479 2066 726f 6d20 796f 7520  tivity from you 
+00012e90: 5079 7468 6f6e 2065 6e76 6972 6f6e 6d65  Python environme
+00012ea0: 6e74 2074 6f20 7468 6520 696e 7465 726e  nt to the intern
+00012eb0: 616c 2061 6476 6572 7469 7365 640a 2020  al advertised.  
+00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ed0: 6c69 7374 656e 6572 7320 6f66 2074 6865  listeners of the
+00012ee0: 2048 6f70 7377 6f72 6b73 204b 6166 6b61   Hopsworks Kafka
+00012ef0: 2043 6c75 7374 6572 2e20 4465 6661 756c   Cluster. Defaul
+00012f00: 7473 2074 6f20 6046 616c 7365 6020 616e  ts to `False` an
+00012f10: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+00012f20: 2020 2020 7769 6c6c 2075 7365 2065 7874      will use ext
+00012f30: 6572 6e61 6c20 6c69 7374 656e 6572 7320  ernal listeners 
+00012f40: 7768 656e 2063 6f6e 6e65 6374 696e 6720  when connecting 
+00012f50: 6672 6f6d 206f 7574 7369 6465 206f 6620  from outside of 
+00012f60: 486f 7073 776f 726b 732e 0a20 2020 2020  Hopsworks..     
+00012f70: 2020 2020 2020 2076 616c 6964 6174 696f         validatio
+00012f80: 6e5f 6f70 7469 6f6e 733a 2041 6464 6974  n_options: Addit
+00012f90: 696f 6e61 6c20 7661 6c69 6461 7469 6f6e  ional validation
+00012fa0: 206f 7074 696f 6e73 2061 7320 6b65 792d   options as key-
+00012fb0: 7661 6c75 6520 7061 6972 732c 2064 6566  value pairs, def
+00012fc0: 6175 6c74 7320 746f 2060 7b7d 602e 0a20  aults to `{}`.. 
+00012fd0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+00012fe0: 206b 6579 2060 7275 6e5f 7661 6c69 6461   key `run_valida
+00012ff0: 7469 6f6e 6020 626f 6f6c 6561 6e20 7661  tion` boolean va
+00013000: 6c75 652c 2073 6574 2074 6f20 6046 616c  lue, set to `Fal
+00013010: 7365 6020 746f 2073 6b69 7020 7661 6c69  se` to skip vali
+00013020: 6461 7469 6f6e 2074 656d 706f 7261 7269  dation temporari
+00013030: 6c79 206f 6e20 696e 6765 7374 696f 6e2e  ly on ingestion.
+00013040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013050: 202a 206b 6579 2060 7361 7665 5f72 6570   * key `save_rep
+00013060: 6f72 7460 2062 6f6f 6c65 616e 2076 616c  ort` boolean val
+00013070: 7565 2c20 7365 7420 746f 2060 4661 6c73  ue, set to `Fals
+00013080: 6560 2074 6f20 736b 6970 2075 706c 6f61  e` to skip uploa
+00013090: 6420 6f66 2074 6865 2076 616c 6964 6174  d of the validat
+000130a0: 696f 6e20 7265 706f 7274 2074 6f20 486f  ion report to Ho
+000130b0: 7073 776f 726b 732e 0a20 2020 2020 2020  psworks..       
+000130c0: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
+000130d0: 6765 5f76 616c 6964 6174 655f 6b77 6172  ge_validate_kwar
+000130e0: 6773 6020 6120 6469 6374 696f 6e61 7279  gs` a dictionary
+000130f0: 2063 6f6e 7461 696e 696e 6720 6b77 6172   containing kwar
+00013100: 6773 2066 6f72 2074 6865 2076 616c 6964  gs for the valid
+00013110: 6174 6520 6d65 7468 6f64 206f 6620 4772  ate method of Gr
+00013120: 6561 7420 4578 7065 6374 6174 696f 6e73  eat Expectations
+00013130: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013140: 2020 2a20 6b65 7920 6066 6574 6368 5f65    * key `fetch_e
+00013150: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
+00013160: 6020 6120 626f 6f6c 6561 6e20 7661 6c75  ` a boolean valu
+00013170: 652c 2062 7920 6465 6661 756c 7420 6046  e, by default `F
+00013180: 616c 7365 6020 666f 7220 6d75 6c74 6920  alse` for multi 
+00013190: 7061 7274 2069 6e73 6572 7473 2c0a 2020  part inserts,.  
+000131a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131b0: 2074 6f20 636f 6e74 726f 6c20 7768 6574   to control whet
+000131c0: 6865 7220 7468 6520 6578 7065 6374 6174  her the expectat
+000131d0: 696f 6e20 7375 6974 6520 6f66 2074 6865  ion suite of the
+000131e0: 2066 6561 7475 7265 2067 726f 7570 2073   feature group s
+000131f0: 686f 756c 6420 6265 2066 6574 6368 6564  hould be fetched
+00013200: 2062 6566 6f72 6520 6576 6572 7920 696e   before every in
+00013210: 7365 7274 2e0a 0a20 2020 2020 2020 2023  sert...        #
+00013220: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00013230: 2020 2020 2028 604a 6f62 602c 2060 5661       (`Job`, `Va
+00013240: 6c69 6461 7469 6f6e 5265 706f 7274 6029  lidationReport`)
+00013250: 2041 2074 7570 6c65 2077 6974 6820 6a6f   A tuple with jo
+00013260: 6220 696e 666f 726d 6174 696f 6e20 6966  b information if
+00013270: 2070 7974 686f 6e20 656e 6769 6e65 2069   python engine i
+00013280: 7320 7573 6564 2061 6e64 2074 6865 2076  s used and the v
+00013290: 616c 6964 6174 696f 6e20 7265 706f 7274  alidation report
+000132a0: 2069 6620 7661 6c69 6461 7469 6f6e 2069   if validation i
+000132b0: 7320 656e 6162 6c65 642e 0a20 2020 2020  s enabled..     
+000132c0: 2020 2020 2020 2060 4665 6174 7572 6547         `FeatureG
+000132d0: 726f 7570 5772 6974 6572 6020 5768 656e  roupWriter` When
+000132e0: 2075 7365 6420 6173 2061 2063 6f6e 7465   used as a conte
+000132f0: 7874 206d 616e 6167 6572 2077 6974 6820  xt manager with 
+00013300: 5079 7468 6f6e 2060 7769 7468 6020 7374  Python `with` st
+00013310: 6174 656d 656e 742e 0a20 2020 2020 2020  atement..       
+00013320: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
+00013330: 662e 5f6d 756c 7469 5f70 6172 745f 696e  f._multi_part_in
+00013340: 7365 7274 203d 2054 7275 650a 2020 2020  sert = True.    
+00013350: 2020 2020 6d75 6c74 695f 7061 7274 5f77      multi_part_w
+00013360: 7269 7465 7220 3d20 6665 6174 7572 655f  riter = feature_
+00013370: 6772 6f75 705f 7772 6974 6572 2e46 6561  group_writer.Fea
+00013380: 7475 7265 4772 6f75 7057 7269 7465 7228  tureGroupWriter(
+00013390: 7365 6c66 290a 2020 2020 2020 2020 6966  self).        if
+000133a0: 2066 6561 7475 7265 7320 6973 204e 6f6e   features is Non
+000133b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000133c0: 6574 7572 6e20 6d75 6c74 695f 7061 7274  eturn multi_part
+000133d0: 5f77 7269 7465 720a 2020 2020 2020 2020  _writer.        
+000133e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000133f0: 2020 2320 676f 2074 6872 6f75 6768 2077    # go through w
+00013400: 7269 7465 7220 746f 2061 766f 6964 2073  riter to avoid s
+00013410: 6574 7469 6e67 206d 756c 7469 2069 6e73  etting multi ins
+00013420: 6572 7420 6465 6661 756c 7473 2061 6761  ert defaults aga
+00013430: 696e 0a20 2020 2020 2020 2020 2020 2072  in.            r
+00013440: 6574 7572 6e20 6d75 6c74 695f 7061 7274  eturn multi_part
+00013450: 5f77 7269 7465 722e 696e 7365 7274 280a  _writer.insert(.
+00013460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013470: 6665 6174 7572 6573 2c0a 2020 2020 2020  features,.      
+00013480: 2020 2020 2020 2020 2020 6f76 6572 7772            overwr
+00013490: 6974 652c 0a20 2020 2020 2020 2020 2020  ite,.           
+000134a0: 2020 2020 206f 7065 7261 7469 6f6e 2c0a       operation,.
+000134b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134c0: 7374 6f72 6167 652c 0a20 2020 2020 2020  storage,.       
+000134d0: 2020 2020 2020 2020 2077 7269 7465 5f6f           write_o
+000134e0: 7074 696f 6e73 2c0a 2020 2020 2020 2020  ptions,.        
+000134f0: 2020 2020 2020 2020 7661 6c69 6461 7469          validati
+00013500: 6f6e 5f6f 7074 696f 6e73 2c0a 2020 2020  on_options,.    
+00013510: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00013520: 6566 2066 696e 616c 697a 655f 6d75 6c74  ef finalize_mult
+00013530: 695f 7061 7274 5f69 6e73 6572 7428 7365  i_part_insert(se
+00013540: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00013550: 4669 6e61 6c69 7a65 7320 616e 6420 6578  Finalizes and ex
+00013560: 6974 7320 7468 6520 6d75 6c74 6920 7061  its the multi pa
+00013570: 7274 2069 6e73 6572 7420 636f 6e74 6578  rt insert contex
+00013580: 7420 6f70 656e 6564 2062 7920 606d 756c  t opened by `mul
+00013590: 7469 5f70 6172 745f 696e 7365 7274 600a  ti_part_insert`.
+000135a0: 2020 2020 2020 2020 696e 2061 2062 6c6f          in a blo
+000135b0: 636b 696e 6720 6661 7368 696f 6e20 6f6e  cking fashion on
+000135c0: 6365 2061 6c6c 2072 6f77 7320 6861 7665  ce all rows have
+000135d0: 2062 6565 6e20 7472 616e 736d 6974 7465   been transmitte
+000135e0: 642e 0a0a 2020 2020 2020 2020 2121 2120  d...        !!! 
+000135f0: 6578 616d 706c 6520 224d 756c 7469 2070  example "Multi p
+00013600: 6172 7420 696e 7365 7274 2077 6974 6820  art insert with 
+00013610: 6d61 6e75 616c 2063 6f6e 7465 7874 206d  manual context m
+00013620: 616e 6167 656d 656e 7422 0a20 2020 2020  anagement".     
+00013630: 2020 2020 2020 2049 6e73 7465 6164 206f         Instead o
+00013640: 6620 6c65 7474 696e 6720 5079 7468 6f6e  f letting Python
+00013650: 2068 616e 646c 6520 7468 6520 656e 7465   handle the ente
+00013660: 7269 6e67 2061 6e64 2065 7869 7469 6e67  ring and exiting
+00013670: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
+00013680: 2020 2020 6d75 6c74 6920 7061 7274 2069      multi part i
+00013690: 6e73 6572 7420 636f 6e74 6578 742c 2079  nsert context, y
+000136a0: 6f75 2063 616e 2073 7461 7274 2061 6e64  ou can start and
+000136b0: 2066 696e 616c 697a 6520 7468 6520 636f   finalize the co
+000136c0: 6e74 6578 740a 2020 2020 2020 2020 2020  ntext.          
+000136d0: 2020 6d61 6e75 616c 6c79 2e0a 2020 2020    manually..    
+000136e0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+000136f0: 6e0a 2020 2020 2020 2020 2020 2020 6665  n.            fe
+00013700: 6174 7572 655f 6772 6f75 7020 3d20 6673  ature_group = fs
+00013710: 2e67 6574 5f6f 725f 6372 6561 7465 5f66  .get_or_create_f
+00013720: 6561 7475 7265 5f67 726f 7570 2822 6667  eature_group("fg
+00013730: 5f6e 616d 6522 2c20 7665 7273 696f 6e3d  _name", version=
+00013740: 3129 0a0a 2020 2020 2020 2020 2020 2020  1)..            
+00013750: 7768 696c 6520 6c6f 6f70 3a0a 2020 2020  while loop:.    
+00013760: 2020 2020 2020 2020 2020 2020 736d 616c              smal
+00013770: 6c5f 6261 7463 685f 6466 203d 202e 2e2e  l_batch_df = ...
+00013780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013790: 2066 6561 7475 7265 5f67 726f 7570 2e6d   feature_group.m
+000137a0: 756c 7469 5f70 6172 745f 696e 7365 7274  ulti_part_insert
+000137b0: 2873 6d61 6c6c 5f62 6174 6368 5f64 6629  (small_batch_df)
+000137c0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+000137d0: 494d 504f 5254 414e 543a 2066 696e 616c  IMPORTANT: final
+000137e0: 697a 6520 7468 6520 6d75 6c74 6920 7061  ize the multi pa
+000137f0: 7274 2069 6e73 6572 7420 746f 206d 616b  rt insert to mak
+00013800: 6520 7375 7265 2061 6c6c 2072 6f77 730a  e sure all rows.
+00013810: 2020 2020 2020 2020 2020 2020 2320 6861              # ha
+00013820: 7665 2062 6565 6e20 7472 616e 736d 6974  ve been transmit
+00013830: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
+00013840: 6665 6174 7572 655f 6772 6f75 702e 6669  feature_group.fi
+00013850: 6e61 6c69 7a65 5f6d 756c 7469 5f70 6172  nalize_multi_par
+00013860: 745f 696e 7365 7274 2829 0a20 2020 2020  t_insert().     
+00013870: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+00013880: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
+00013890: 2074 6865 2066 6972 7374 2063 616c 6c20   the first call 
+000138a0: 746f 2060 6d75 6c74 695f 7061 7274 5f69  to `multi_part_i
+000138b0: 6e73 6572 7460 2069 6e69 7469 6174 6573  nsert` initiates
+000138c0: 2074 6865 2063 6f6e 7465 7874 0a20 2020   the context.   
+000138d0: 2020 2020 2020 2020 2061 6e64 2062 6520           and be 
+000138e0: 7375 7265 2074 6f20 6669 6e61 6c69 7a65  sure to finalize
+000138f0: 2069 742e 2054 6865 2060 6669 6e61 6c69   it. The `finali
+00013900: 7a65 5f6d 756c 7469 5f70 6172 745f 696e  ze_multi_part_in
+00013910: 7365 7274 6020 6973 2061 0a20 2020 2020  sert` is a.     
+00013920: 2020 2020 2020 2062 6c6f 636b 696e 6720         blocking 
+00013930: 6361 6c6c 2074 6861 7420 7265 7475 726e  call that return
+00013940: 7320 6f6e 6365 2061 6c6c 2072 6f77 7320  s once all rows 
+00013950: 6861 7665 2062 6565 6e20 7472 616e 736d  have been transm
+00013960: 6974 7465 642e 0a20 2020 2020 2020 2022  itted..        "
+00013970: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
+00013980: 6c66 2e5f 6b61 666b 615f 7072 6f64 7563  lf._kafka_produc
+00013990: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
+000139a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000139b0: 2e5f 6b61 666b 615f 7072 6f64 7563 6572  ._kafka_producer
+000139c0: 2e66 6c75 7368 2829 0a20 2020 2020 2020  .flush().       
+000139d0: 2020 2020 2073 656c 662e 5f6b 6166 6b61       self._kafka
+000139e0: 5f70 726f 6475 6365 7220 3d20 4e6f 6e65  _producer = None
+000139f0: 0a20 2020 2020 2020 2073 656c 662e 5f66  .        self._f
+00013a00: 6561 7475 7265 5f77 7269 7465 7273 203d  eature_writers =
+00013a10: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+00013a20: 6c66 2e5f 7772 6974 6572 203d 204e 6f6e  lf._writer = Non
+00013a30: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
+00013a40: 6d75 6c74 695f 7061 7274 5f69 6e73 6572  multi_part_inser
+00013a50: 7420 3d20 4661 6c73 650a 0a20 2020 2064  t = False..    d
+00013a60: 6566 2069 6e73 6572 745f 7374 7265 616d  ef insert_stream
+00013a70: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00013a80: 2020 2020 2020 2020 6665 6174 7572 6573          features
+00013a90: 3a20 5479 7065 5661 7228 2270 7973 7061  : TypeVar("pyspa
+00013aa0: 726b 2e73 716c 2e44 6174 6146 7261 6d65  rk.sql.DataFrame
+00013ab0: 2229 2c20 2023 206e 6f71 613a 2046 3832  "),  # noqa: F82
+00013ac0: 310a 2020 2020 2020 2020 7175 6572 795f  1.        query_
+00013ad0: 6e61 6d65 3a20 4f70 7469 6f6e 616c 5b73  name: Optional[s
+00013ae0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00013af0: 2020 2020 6f75 7470 7574 5f6d 6f64 653a      output_mode:
+00013b00: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00013b10: 2022 6170 7065 6e64 222c 0a20 2020 2020   "append",.     
+00013b20: 2020 2061 7761 6974 5f74 6572 6d69 6e61     await_termina
+00013b30: 7469 6f6e 3a20 4f70 7469 6f6e 616c 5b62  tion: Optional[b
+00013b40: 6f6f 6c5d 203d 2046 616c 7365 2c0a 2020  ool] = False,.  
+00013b50: 2020 2020 2020 7469 6d65 6f75 743a 204f        timeout: O
+00013b60: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00013b70: 6f6e 652c 0a20 2020 2020 2020 2063 6865  one,.        che
+00013b80: 636b 706f 696e 745f 6469 723a 204f 7074  ckpoint_dir: Opt
+00013b90: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00013ba0: 652c 0a20 2020 2020 2020 2077 7269 7465  e,.        write
+00013bb0: 5f6f 7074 696f 6e73 3a20 4f70 7469 6f6e  _options: Option
+00013bc0: 616c 5b44 6963 745b 416e 792c 2041 6e79  al[Dict[Any, Any
+00013bd0: 5d5d 203d 207b 7d2c 0a20 2020 2029 3a0a  ]] = {},.    ):.
+00013be0: 2020 2020 2020 2020 2222 2249 6e67 6573          """Inges
+00013bf0: 7420 6120 5370 6172 6b20 5374 7275 6374  t a Spark Struct
+00013c00: 7572 6564 2053 7472 6561 6d69 6e67 2044  ured Streaming D
+00013c10: 6174 6166 7261 6d65 2074 6f20 7468 6520  ataframe to the 
+00013c20: 6f6e 6c69 6e65 2066 6561 7475 7265 2073  online feature s
+00013c30: 746f 7265 2e0a 0a20 2020 2020 2020 2054  tore...        T
+00013c40: 6869 7320 6d65 7468 6f64 2063 7265 6174  his method creat
+00013c50: 6573 2061 206c 6f6e 6720 7275 6e6e 696e  es a long runnin
+00013c60: 6720 5370 6172 6b20 5374 7265 616d 696e  g Spark Streamin
+00013c70: 6720 5175 6572 792c 2079 6f75 2063 616e  g Query, you can
+00013c80: 2063 6f6e 7472 6f6c 2074 6865 0a20 2020   control the.   
+00013c90: 2020 2020 2074 6572 6d69 6e61 7469 6f6e       termination
+00013ca0: 206f 6620 7468 6520 7175 6572 7920 7468   of the query th
+00013cb0: 726f 7567 6820 7468 6520 6172 6775 6d65  rough the argume
+00013cc0: 6e74 732e 0a0a 2020 2020 2020 2020 4974  nts...        It
+00013cd0: 2069 7320 706f 7373 6962 6c65 2074 6f20   is possible to 
+00013ce0: 7374 6f70 2074 6865 2072 6574 7572 6e65  stop the returne
+00013cf0: 6420 7175 6572 7920 7769 7468 2074 6865  d query with the
+00013d00: 2060 2e73 746f 7028 2960 2061 6e64 2063   `.stop()` and c
+00013d10: 6865 636b 2069 7473 0a20 2020 2020 2020  heck its.       
+00013d20: 2073 7461 7475 7320 7769 7468 2060 2e69   status with `.i
+00013d30: 7341 6374 6976 6560 2e0a 0a20 2020 2020  sActive`...     
+00013d40: 2020 2054 6f20 6765 7420 6120 6c69 7374     To get a list
+00013d50: 206f 6620 616c 6c20 6163 7469 7665 2071   of all active q
+00013d60: 7565 7269 6573 2c20 7573 653a 0a0a 2020  ueries, use:..  
+00013d70: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+00013d80: 2020 2020 2020 2020 7371 6d20 3d20 7370          sqm = sp
+00013d90: 6172 6b2e 7374 7265 616d 730a 0a20 2020  ark.streams..   
+00013da0: 2020 2020 2023 2067 6574 2074 6865 206c       # get the l
+00013db0: 6973 7420 6f66 2061 6374 6976 6520 7374  ist of active st
+00013dc0: 7265 616d 696e 6720 7175 6572 6965 730a  reaming queries.
+00013dd0: 2020 2020 2020 2020 5b71 2e6e 616d 6520          [q.name 
+00013de0: 666f 7220 7120 696e 2073 716d 2e61 6374  for q in sqm.act
+00013df0: 6976 655d 0a20 2020 2020 2020 2060 6060  ive].        ```
+00013e00: 0a0a 2020 2020 2020 2020 2121 2120 7761  ..        !!! wa
+00013e10: 726e 696e 6720 2245 6e67 696e 6520 5375  rning "Engine Su
+00013e20: 7070 6f72 7422 0a20 2020 2020 2020 2020  pport".         
+00013e30: 2020 202a 2a53 7061 726b 206f 6e6c 792a     **Spark only*
+00013e40: 2a0a 0a20 2020 2020 2020 2020 2020 2053  *..            S
+00013e50: 7472 6561 6d20 696e 6765 7374 696f 6e20  tream ingestion 
+00013e60: 7573 696e 6720 5061 6e64 6173 2f50 7974  using Pandas/Pyt
+00013e70: 686f 6e20 6173 2065 6e67 696e 6520 6973  hon as engine is
+00013e80: 2063 7572 7265 6e74 6c79 206e 6f74 2073   currently not s
+00013e90: 7570 706f 7274 6564 2e0a 2020 2020 2020  upported..      
+00013ea0: 2020 2020 2020 5079 7468 6f6e 2f50 616e        Python/Pan
+00013eb0: 6461 7320 6861 7320 6e6f 206e 6f74 696f  das has no notio
+00013ec0: 6e20 6f66 2073 7472 6561 6d69 6e67 2e0a  n of streaming..
+00013ed0: 0a20 2020 2020 2020 2021 2121 2077 6172  .        !!! war
+00013ee0: 6e69 6e67 2022 4461 7461 2056 616c 6964  ning "Data Valid
+00013ef0: 6174 696f 6e20 5375 7070 6f72 7422 0a20  ation Support". 
+00013f00: 2020 2020 2020 2020 2020 2060 696e 7365             `inse
+00013f10: 7274 5f73 7472 6561 6d60 2064 6f65 7320  rt_stream` does 
+00013f20: 6e6f 7420 7065 7266 6f72 6d20 616e 7920  not perform any 
+00013f30: 6461 7461 2076 616c 6964 6174 696f 6e20  data validation 
+00013f40: 7573 696e 6720 4772 6561 7420 4578 7065  using Great Expe
+00013f50: 6374 6174 696f 6e73 0a20 2020 2020 2020  ctations.       
+00013f60: 2020 2020 2065 7665 6e20 7768 656e 2061       even when a
+00013f70: 2065 7870 6563 7461 7469 6f6e 2073 7569   expectation sui
+00013f80: 7465 2069 7320 6174 7461 6368 6564 2e0a  te is attached..
+00013f90: 0a20 2020 2020 2020 2023 2041 7267 756d  .        # Argum
+00013fa0: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
+00013fb0: 2066 6561 7475 7265 733a 2046 6561 7475   features: Featu
+00013fc0: 7265 7320 696e 2053 7472 6561 6d69 6e67  res in Streaming
+00013fd0: 2044 6174 6166 7261 6d65 2074 6f20 6265   Dataframe to be
+00013fe0: 2073 6176 6564 2e0a 2020 2020 2020 2020   saved..        
+00013ff0: 2020 2020 7175 6572 795f 6e61 6d65 3a20      query_name: 
+00014000: 4974 2069 7320 706f 7373 6962 6c65 2074  It is possible t
+00014010: 6f20 6f70 7469 6f6e 616c 6c79 2073 7065  o optionally spe
+00014020: 6369 6679 2061 206e 616d 6520 666f 7220  cify a name for 
+00014030: 7468 6520 7175 6572 7920 746f 0a20 2020  the query to.   
+00014040: 2020 2020 2020 2020 2020 2020 206d 616b               mak
+00014050: 6520 6974 2065 6173 6965 7220 746f 2072  e it easier to r
+00014060: 6563 6f67 6e69 7365 2069 6e20 7468 6520  ecognise in the 
+00014070: 5370 6172 6b20 5549 2e20 4465 6661 756c  Spark UI. Defaul
+00014080: 7473 2074 6f20 604e 6f6e 6560 2e0a 2020  ts to `None`..  
+00014090: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+000140a0: 5f6d 6f64 653a 2053 7065 6369 6669 6573  _mode: Specifies
+000140b0: 2068 6f77 2064 6174 6120 6f66 2061 2073   how data of a s
+000140c0: 7472 6561 6d69 6e67 2044 6174 6146 7261  treaming DataFra
+000140d0: 6d65 2f44 6174 6173 6574 2069 730a 2020  me/Dataset is.  
+000140e0: 2020 2020 2020 2020 2020 2020 2020 7772                wr
+000140f0: 6974 7465 6e20 746f 2061 2073 7472 6561  itten to a strea
+00014100: 6d69 6e67 2073 696e 6b2e 2028 3129 2060  ming sink. (1) `
+00014110: 2261 7070 656e 6422 603a 204f 6e6c 7920  "append"`: Only 
+00014120: 7468 6520 6e65 7720 726f 7773 2069 6e20  the new rows in 
+00014130: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00014140: 2020 2020 7374 7265 616d 696e 6720 4461      streaming Da
+00014150: 7461 4672 616d 652f 4461 7461 7365 7420  taFrame/Dataset 
+00014160: 7769 6c6c 2062 6520 7772 6974 7465 6e20  will be written 
+00014170: 746f 2074 6865 2073 696e 6b2e 2028 3229  to the sink. (2)
+00014180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014190: 2060 2263 6f6d 706c 6574 6522 603a 2041   `"complete"`: A
+000141a0: 6c6c 2074 6865 2072 6f77 7320 696e 2074  ll the rows in t
+000141b0: 6865 2073 7472 6561 6d69 6e67 2044 6174  he streaming Dat
+000141c0: 6146 7261 6d65 2f44 6174 6173 6574 2077  aFrame/Dataset w
+000141d0: 696c 6c20 6265 0a20 2020 2020 2020 2020  ill be.         
+000141e0: 2020 2020 2020 2077 7269 7474 656e 2074         written t
+000141f0: 6f20 7468 6520 7369 6e6b 2065 7665 7279  o the sink every
+00014200: 2074 696d 6520 7468 6572 6520 6973 2073   time there is s
+00014210: 6f6d 6520 7570 6461 7465 2e20 2833 2920  ome update. (3) 
+00014220: 6022 7570 6461 7465 2260 3a0a 2020 2020  `"update"`:.    
+00014230: 2020 2020 2020 2020 2020 2020 6f6e 6c79              only
+00014240: 2074 6865 2072 6f77 7320 7468 6174 2077   the rows that w
+00014250: 6572 6520 7570 6461 7465 6420 696e 2074  ere updated in t
+00014260: 6865 2073 7472 6561 6d69 6e67 2044 6174  he streaming Dat
+00014270: 6146 7261 6d65 2f44 6174 6173 6574 2077  aFrame/Dataset w
+00014280: 696c 6c0a 2020 2020 2020 2020 2020 2020  ill.            
+00014290: 2020 2020 6265 2077 7269 7474 656e 2074      be written t
+000142a0: 6f20 7468 6520 7369 6e6b 2065 7665 7279  o the sink every
+000142b0: 2074 696d 6520 7468 6572 6520 6172 6520   time there are 
+000142c0: 736f 6d65 2075 7064 6174 6573 2e0a 2020  some updates..  
+000142d0: 2020 2020 2020 2020 2020 2020 2020 4966                If
+000142e0: 2074 6865 2071 7565 7279 2064 6f65 736e   the query doesn
+000142f0: e280 9974 2063 6f6e 7461 696e 2061 6767  ...t contain agg
+00014300: 7265 6761 7469 6f6e 732c 2069 7420 7769  regations, it wi
+00014310: 6c6c 2062 6520 6571 7569 7661 6c65 6e74  ll be equivalent
+00014320: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
+00014330: 2020 2020 6170 7065 6e64 206d 6f64 652e      append mode.
+00014340: 2044 6566 6175 6c74 7320 746f 2060 2261   Defaults to `"a
+00014350: 7070 656e 6422 602e 0a20 2020 2020 2020  ppend"`..       
+00014360: 2020 2020 2061 7761 6974 5f74 6572 6d69       await_termi
+00014370: 6e61 7469 6f6e 3a20 5761 6974 7320 666f  nation: Waits fo
+00014380: 7220 7468 6520 7465 726d 696e 6174 696f  r the terminatio
+00014390: 6e20 6f66 2074 6869 7320 7175 6572 792c  n of this query,
+000143a0: 2065 6974 6865 7220 6279 0a20 2020 2020   either by.     
+000143b0: 2020 2020 2020 2020 2020 2071 7565 7279             query
+000143c0: 2e73 746f 7028 2920 6f72 2062 7920 616e  .stop() or by an
+000143d0: 2065 7863 6570 7469 6f6e 2e20 4966 2074   exception. If t
+000143e0: 6865 2071 7565 7279 2068 6173 2074 6572  he query has ter
+000143f0: 6d69 6e61 7465 6420 7769 7468 2061 6e0a  minated with an.
+00014400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014410: 6578 6365 7074 696f 6e2c 2074 6865 6e20  exception, then 
+00014420: 7468 6520 6578 6365 7074 696f 6e20 7769  the exception wi
+00014430: 6c6c 2062 6520 7468 726f 776e 2e20 4966  ll be thrown. If
+00014440: 2074 696d 656f 7574 2069 7320 7365 742c   timeout is set,
+00014450: 2069 740a 2020 2020 2020 2020 2020 2020   it.            
+00014460: 2020 2020 7265 7475 726e 7320 7768 6574      returns whet
+00014470: 6865 7220 7468 6520 7175 6572 7920 6861  her the query ha
+00014480: 7320 7465 726d 696e 6174 6564 206f 7220  s terminated or 
+00014490: 6e6f 7420 7769 7468 696e 2074 6865 2074  not within the t
+000144a0: 696d 656f 7574 0a20 2020 2020 2020 2020  imeout.         
+000144b0: 2020 2020 2020 2073 6563 6f6e 6473 2e20         seconds. 
+000144c0: 4465 6661 756c 7473 2074 6f20 6046 616c  Defaults to `Fal
+000144d0: 7365 602e 0a20 2020 2020 2020 2020 2020  se`..           
+000144e0: 2074 696d 656f 7574 3a20 4f6e 6c79 2072   timeout: Only r
+000144f0: 656c 6576 616e 7420 696e 2063 6f6d 6269  elevant in combi
+00014500: 6e61 7469 6f6e 2077 6974 6820 6061 7761  nation with `awa
+00014510: 6974 5f74 6572 6d69 6e61 7469 6f6e 3d54  it_termination=T
+00014520: 7275 6560 2e0a 2020 2020 2020 2020 2020  rue`..          
+00014530: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+00014540: 6f20 604e 6f6e 6560 2e0a 2020 2020 2020  o `None`..      
+00014550: 2020 2020 2020 6368 6563 6b70 6f69 6e74        checkpoint
+00014560: 5f64 6972 3a20 4368 6563 6b70 6f69 6e74  _dir: Checkpoint
+00014570: 2064 6972 6563 746f 7279 206c 6f63 6174   directory locat
+00014580: 696f 6e2e 2054 6869 7320 7769 6c6c 2062  ion. This will b
+00014590: 6520 7573 6564 2074 6f20 6173 2061 2072  e used to as a r
+000145a0: 6566 6572 656e 6365 2074 6f0a 2020 2020  eference to.    
+000145b0: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
+000145c0: 2077 6865 7265 2074 6f20 7265 7375 6d65   where to resume
+000145d0: 2074 6865 2073 7472 6561 6d69 6e67 206a   the streaming j
+000145e0: 6f62 2e20 4966 2060 4e6f 6e65 6020 7468  ob. If `None` th
+000145f0: 656e 2068 7366 7320 7769 6c6c 2063 6f6e  en hsfs will con
+00014600: 7374 7275 6374 2061 730a 2020 2020 2020  struct as.      
+00014610: 2020 2020 2020 2020 2020 2269 6e73 6572            "inser
+00014620: 745f 7374 7265 616d 5f22 202b 206f 6e6c  t_stream_" + onl
+00014630: 696e 655f 746f 7069 635f 6e61 6d65 2e20  ine_topic_name. 
+00014640: 4465 6661 756c 7473 2074 6f20 604e 6f6e  Defaults to `Non
+00014650: 6560 2e0a 2020 2020 2020 2020 2020 2020  e`..            
+00014660: 2020 2020 7772 6974 655f 6f70 7469 6f6e      write_option
+00014670: 733a 2041 6464 6974 696f 6e61 6c20 7772  s: Additional wr
+00014680: 6974 6520 6f70 7469 6f6e 7320 666f 7220  ite options for 
+00014690: 5370 6172 6b20 6173 206b 6579 2d76 616c  Spark as key-val
+000146a0: 7565 2070 6169 7273 2e0a 2020 2020 2020  ue pairs..      
+000146b0: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+000146c0: 7473 2074 6f20 607b 7d60 2e0a 0a20 2020  ts to `{}`...   
+000146d0: 2020 2020 2023 2052 6574 7572 6e73 0a20       # Returns. 
+000146e0: 2020 2020 2020 2020 2020 2060 5374 7265             `Stre
+000146f0: 616d 696e 6751 7565 7279 603a 2053 7061  amingQuery`: Spa
+00014700: 726b 2053 7472 7563 7475 7265 6420 5374  rk Structured St
+00014710: 7265 616d 696e 6720 5175 6572 7920 6f62  reaming Query ob
+00014720: 6a65 6374 2e0a 2020 2020 2020 2020 2222  ject..        ""
+00014730: 220a 2020 2020 2020 2020 6966 2028 0a20  ".        if (. 
+00014740: 2020 2020 2020 2020 2020 206e 6f74 2065             not e
+00014750: 6e67 696e 652e 6765 745f 696e 7374 616e  ngine.get_instan
+00014760: 6365 2829 2e69 735f 7370 6172 6b5f 6461  ce().is_spark_da
+00014770: 7461 6672 616d 6528 6665 6174 7572 6573  taframe(features
+00014780: 290a 2020 2020 2020 2020 2020 2020 6f72  ).            or
+00014790: 206e 6f74 2066 6561 7475 7265 732e 6973   not features.is
+000147a0: 5374 7265 616d 696e 670a 2020 2020 2020  Streaming.      
+000147b0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+000147c0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+000147d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000147e0: 2020 2246 6561 7475 7265 7320 6861 7665    "Features have
+000147f0: 2074 6f20 6265 2061 2073 7472 6561 6d69   to be a streami
+00014800: 6e67 2074 7970 6520 7370 6172 6b20 6461  ng type spark da
+00014810: 7461 6672 616d 652e 2055 7365 2060 696e  taframe. Use `in
+00014820: 7365 7274 2829 6020 6d65 7468 6f64 2069  sert()` method i
+00014830: 6e73 7465 6164 2e22 0a20 2020 2020 2020  nstead.".       
+00014840: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
+00014850: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00014860: 2023 206c 6f77 6572 2063 6173 696e 6720   # lower casing 
+00014870: 6665 6174 7572 6520 6e61 6d65 730a 2020  feature names.  
+00014880: 2020 2020 2020 2020 2020 6665 6174 7572            featur
+00014890: 655f 6461 7461 6672 616d 6520 3d20 656e  e_dataframe = en
+000148a0: 6769 6e65 2e67 6574 5f69 6e73 7461 6e63  gine.get_instanc
+000148b0: 6528 292e 636f 6e76 6572 745f 746f 5f64  e().convert_to_d
+000148c0: 6566 6175 6c74 5f64 6174 6166 7261 6d65  efault_dataframe
+000148d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000148e0: 2020 6665 6174 7572 6573 0a20 2020 2020    features.     
+000148f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00014900: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+00014910: 726e 280a 2020 2020 2020 2020 2020 2020  rn(.            
+00014920: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
+00014930: 2020 2020 2020 2020 2020 2253 7472 6561            "Strea
+00014940: 6d20 696e 6765 7374 696f 6e20 666f 7220  m ingestion for 
+00014950: 6665 6174 7572 6520 6772 6f75 7020 607b  feature group `{
+00014960: 7d60 2c20 7769 7468 2076 6572 7369 6f6e  }`, with version
+00014970: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00014980: 2020 2020 2020 2220 607b 7d60 2077 696c        " `{}` wil
+00014990: 6c20 6e6f 7420 636f 6d70 7574 6520 7374  l not compute st
+000149a0: 6174 6973 7469 6373 2e22 0a20 2020 2020  atistics.".     
+000149b0: 2020 2020 2020 2020 2020 2029 2e66 6f72             ).for
+000149c0: 6d61 7428 7365 6c66 2e5f 6e61 6d65 2c20  mat(self._name, 
+000149d0: 7365 6c66 2e5f 7665 7273 696f 6e29 2c0a  self._version),.
+000149e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149f0: 7574 696c 2e53 7461 7469 7374 6963 7357  util.StatisticsW
+00014a00: 6172 6e69 6e67 2c0a 2020 2020 2020 2020  arning,.        
+00014a10: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+00014a20: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00014a30: 6665 6174 7572 655f 6772 6f75 705f 656e  feature_group_en
+00014a40: 6769 6e65 2e69 6e73 6572 745f 7374 7265  gine.insert_stre
+00014a50: 616d 280a 2020 2020 2020 2020 2020 2020  am(.            
+00014a60: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00014a70: 2020 2020 2020 2020 2020 6665 6174 7572            featur
+00014a80: 655f 6461 7461 6672 616d 652c 0a20 2020  e_dataframe,.   
+00014a90: 2020 2020 2020 2020 2020 2020 2071 7565               que
+00014aa0: 7279 5f6e 616d 652c 0a20 2020 2020 2020  ry_name,.       
+00014ab0: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+00014ac0: 6d6f 6465 2c0a 2020 2020 2020 2020 2020  mode,.          
+00014ad0: 2020 2020 2020 6177 6169 745f 7465 726d        await_term
+00014ae0: 696e 6174 696f 6e2c 0a20 2020 2020 2020  ination,.       
+00014af0: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+00014b00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014b10: 2020 6368 6563 6b70 6f69 6e74 5f64 6972    checkpoint_dir
+00014b20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014b30: 2020 7772 6974 655f 6f70 7469 6f6e 732c    write_options,
+00014b40: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00014b50: 2020 2020 6465 6620 636f 6d6d 6974 5f64      def commit_d
+00014b60: 6574 6169 6c73 280a 2020 2020 2020 2020  etails(.        
+00014b70: 7365 6c66 2c0a 2020 2020 2020 2020 7761  self,.        wa
+00014b80: 6c6c 636c 6f63 6b5f 7469 6d65 3a20 4f70  llclock_time: Op
+00014b90: 7469 6f6e 616c 5b55 6e69 6f6e 5b73 7472  tional[Union[str
+00014ba0: 2c20 696e 742c 2064 6174 6574 696d 652c  , int, datetime,
+00014bb0: 2064 6174 655d 5d20 3d20 4e6f 6e65 2c0a   date]] = None,.
+00014bc0: 2020 2020 2020 2020 6c69 6d69 743a 204f          limit: O
+00014bd0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
+00014be0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+00014bf0: 2020 2020 2222 2252 6574 7269 6576 6573      """Retrieves
+00014c00: 2063 6f6d 6d69 7420 7469 6d65 6c69 6e65   commit timeline
+00014c10: 2066 6f72 2074 6869 7320 6665 6174 7572   for this featur
+00014c20: 6520 6772 6f75 702e 2054 6869 7320 6d65  e group. This me
+00014c30: 7468 6f64 2063 616e 206f 6e6c 7920 6265  thod can only be
+00014c40: 2075 7365 640a 2020 2020 2020 2020 6f6e   used.        on
+00014c50: 2074 696d 6520 7472 6176 656c 2065 6e61   time travel ena
+00014c60: 626c 6564 2066 6561 7475 7265 2067 726f  bled feature gro
+00014c70: 7570 730a 0a20 2020 2020 2020 2021 2121  ups..        !!!
+00014c80: 2065 7861 6d70 6c65 0a20 2020 2020 2020   example.       
+00014c90: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
+00014ca0: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
+00014cb0: 6e65 6374 2074 6f20 7468 6520 4665 6174  nect to the Feat
+00014cc0: 7572 6520 5374 6f72 650a 2020 2020 2020  ure Store.      
+00014cd0: 2020 2020 2020 6673 203d 202e 2e2e 0a0a        fs = .....
+00014ce0: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
+00014cf0: 7420 7468 6520 4665 6174 7572 6520 4772  t the Feature Gr
+00014d00: 6f75 7020 696e 7374 616e 6365 0a20 2020  oup instance.   
+00014d10: 2020 2020 2020 2020 2066 6720 3d20 6673           fg = fs
+00014d20: 2e67 6574 5f6f 725f 6372 6561 7465 5f66  .get_or_create_f
+00014d30: 6561 7475 7265 5f67 726f 7570 282e 2e2e  eature_group(...
+00014d40: 290a 0a20 2020 2020 2020 2020 2020 2063  )..            c
+00014d50: 6f6d 6d69 745f 6465 7461 696c 7320 3d20  ommit_details = 
+00014d60: 6667 2e63 6f6d 6d69 745f 6465 7461 696c  fg.commit_detail
+00014d70: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00014d80: 6060 600a 0a20 2020 2020 2020 2023 2041  ```..        # A
+00014d90: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
+00014da0: 2020 2020 2077 616c 6c63 6c6f 636b 5f74       wallclock_t
+00014db0: 696d 653a 2043 6f6d 6d69 7420 6465 7461  ime: Commit deta
+00014dc0: 696c 7320 6173 206f 6620 7370 6563 6966  ils as of specif
+00014dd0: 6963 2070 6f69 6e74 2069 6e20 7469 6d65  ic point in time
+00014de0: 2e20 4465 6661 756c 7473 2074 6f20 604e  . Defaults to `N
+00014df0: 6f6e 6560 2e0a 2020 2020 2020 2020 2020  one`..          
+00014e00: 2020 2020 2020 2053 7472 696e 6773 2073         Strings s
+00014e10: 686f 756c 6420 6265 2066 6f72 6d61 7474  hould be formatt
+00014e20: 6564 2069 6e20 6f6e 6520 6f66 2074 6865  ed in one of the
+00014e30: 2066 6f6c 6c6f 7769 6e67 2066 6f72 6d61   following forma
+00014e40: 7473 2060 2559 2d25 6d2d 2564 602c 2060  ts `%Y-%m-%d`, `
+00014e50: 2559 2d25 6d2d 2564 2025 4860 2c20 6025  %Y-%m-%d %H`, `%
+00014e60: 592d 256d 2d25 6420 2548 3a25 4d60 2c0a  Y-%m-%d %H:%M`,.
+00014e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e80: 6025 592d 256d 2d25 6420 2548 3a25 4d3a  `%Y-%m-%d %H:%M:
+00014e90: 2553 602c 206f 7220 6025 592d 256d 2d25  %S`, or `%Y-%m-%
+00014ea0: 6420 2548 3a25 4d3a 2553 2e25 6660 2e0a  d %H:%M:%S.%f`..
+00014eb0: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
+00014ec0: 743a 204e 756d 6265 7220 6f66 2063 6f6d  t: Number of com
+00014ed0: 6d69 7473 2074 6f20 7265 7472 6965 7665  mits to retrieve
+00014ee0: 2e20 4465 6661 756c 7473 2074 6f20 604e  . Defaults to `N
+00014ef0: 6f6e 6560 2e0a 0a20 2020 2020 2020 2023  one`...        #
+00014f00: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00014f10: 2020 2020 2060 4469 6374 5b73 7472 2c20       `Dict[str, 
+00014f20: 4469 6374 5b73 7472 2c20 7374 725d 5d60  Dict[str, str]]`
+00014f30: 2e20 4469 6374 696f 6e61 7279 206f 626a  . Dictionary obj
+00014f40: 6563 7420 6f66 2063 6f6d 6d69 7420 6d65  ect of commit me
+00014f50: 7461 6461 7461 2074 696d 656c 696e 652c  tadata timeline,
+00014f60: 2077 6865 7265 204b 6579 2069 7320 636f   where Key is co
+00014f70: 6d6d 6974 2069 6420 616e 6420 7661 6c75  mmit id and valu
+00014f80: 650a 2020 2020 2020 2020 2020 2020 6973  e.            is
+00014f90: 2060 4469 6374 5b73 7472 2c20 7374 725d   `Dict[str, str]
+00014fa0: 6020 7769 7468 206b 6579 2076 616c 7565  ` with key value
+00014fb0: 2070 6169 7273 206f 6620 6461 7465 2063   pairs of date c
+00014fc0: 6f6d 6d69 7474 6564 206f 6e2c 206e 756d  ommitted on, num
+00014fd0: 6265 7220 6f66 2072 6f77 7320 7570 6461  ber of rows upda
+00014fe0: 7465 642c 2069 6e73 6572 7465 6420 616e  ted, inserted an
+00014ff0: 6420 6465 6c65 7465 642e 0a0a 2020 2020  d deleted...    
+00015000: 2020 2020 2320 5261 6973 6573 0a20 2020      # Raises.   
+00015010: 2020 2020 2020 2020 2060 6873 6673 2e63           `hsfs.c
+00015020: 6c69 656e 742e 6578 6365 7074 696f 6e73  lient.exceptions
+00015030: 2e52 6573 7441 5049 4572 726f 7260 2e0a  .RestAPIError`..
+00015040: 2020 2020 2020 2020 2020 2020 6068 7366              `hsf
+00015050: 732e 636c 6965 6e74 2e65 7863 6570 7469  s.client.excepti
+00015060: 6f6e 732e 4665 6174 7572 6553 746f 7265  ons.FeatureStore
+00015070: 4578 6365 7074 696f 6e60 2e20 4966 2074  Exception`. If t
+00015080: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
+00015090: 2064 6f65 7320 6e6f 7420 6861 7665 2060   does not have `
+000150a0: 4855 4449 6020 7469 6d65 2074 7261 7665  HUDI` time trave
+000150b0: 6c20 666f 726d 6174 0a20 2020 2020 2020  l format.       
+000150c0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+000150d0: 7572 6e20 7365 6c66 2e5f 6665 6174 7572  urn self._featur
+000150e0: 655f 6772 6f75 705f 656e 6769 6e65 2e63  e_group_engine.c
+000150f0: 6f6d 6d69 745f 6465 7461 696c 7328 7365  ommit_details(se
+00015100: 6c66 2c20 7761 6c6c 636c 6f63 6b5f 7469  lf, wallclock_ti
+00015110: 6d65 2c20 6c69 6d69 7429 0a0a 2020 2020  me, limit)..    
+00015120: 6465 6620 636f 6d6d 6974 5f64 656c 6574  def commit_delet
+00015130: 655f 7265 636f 7264 280a 2020 2020 2020  e_record(.      
+00015140: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00015150: 6465 6c65 7465 5f64 663a 2054 7970 6556  delete_df: TypeV
+00015160: 6172 2822 7079 7370 6172 6b2e 7371 6c2e  ar("pyspark.sql.
+00015170: 4461 7461 4672 616d 6522 292c 2020 2320  DataFrame"),  # 
+00015180: 6e6f 7161 3a20 4638 3231 0a20 2020 2020  noqa: F821.     
+00015190: 2020 2077 7269 7465 5f6f 7074 696f 6e73     write_options
+000151a0: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
+000151b0: 416e 792c 2041 6e79 5d5d 203d 207b 7d2c  Any, Any]] = {},
+000151c0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+000151d0: 2222 2244 726f 7073 2072 6563 6f72 6473  """Drops records
+000151e0: 2070 7265 7365 6e74 2069 6e20 7468 6520   present in the 
+000151f0: 7072 6f76 6964 6564 2044 6174 6146 7261  provided DataFra
+00015200: 6d65 2061 6e64 2063 6f6d 6d69 7473 2069  me and commits i
+00015210: 7420 6173 2075 7064 6174 6520 746f 2074  t as update to t
+00015220: 6869 730a 2020 2020 2020 2020 4665 6174  his.        Feat
+00015230: 7572 6520 6772 6f75 702e 2054 6869 7320  ure group. This 
+00015240: 6d65 7468 6f64 2063 616e 206f 6e6c 7920  method can only 
+00015250: 6265 2075 7365 6420 6f6e 2074 696d 6520  be used on time 
+00015260: 7472 6176 656c 2065 6e61 626c 6564 2066  travel enabled f
+00015270: 6561 7475 7265 2067 726f 7570 732e 0a0a  eature groups...
+00015280: 2020 2020 2020 2020 2320 4172 6775 6d65          # Argume
+00015290: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
+000152a0: 6465 6c65 7465 5f64 663a 2064 6174 6146  delete_df: dataF
+000152b0: 7261 6d65 2063 6f6e 7461 696e 696e 6720  rame containing 
+000152c0: 7265 636f 7264 7320 746f 2062 6520 6465  records to be de
+000152d0: 6c65 7465 642e 0a20 2020 2020 2020 2020  leted..         
+000152e0: 2020 2077 7269 7465 5f6f 7074 696f 6e73     write_options
+000152f0: 3a20 5573 6572 2070 726f 7669 6465 6420  : User provided 
+00015300: 7772 6974 6520 6f70 7469 6f6e 732e 2044  write options. D
+00015310: 6566 6175 6c74 7320 746f 2060 7b7d 602e  efaults to `{}`.
+00015320: 0a0a 2020 2020 2020 2020 2320 5261 6973  ..        # Rais
+00015330: 6573 0a20 2020 2020 2020 2020 2020 2060  es.            `
+00015340: 6873 6673 2e63 6c69 656e 742e 6578 6365  hsfs.client.exce
+00015350: 7074 696f 6e73 2e52 6573 7441 5049 4572  ptions.RestAPIEr
+00015360: 726f 7260 2e0a 2020 2020 2020 2020 2222  ror`..        ""
+00015370: 220a 2020 2020 2020 2020 7365 6c66 2e5f  ".        self._
+00015380: 6665 6174 7572 655f 6772 6f75 705f 656e  feature_group_en
+00015390: 6769 6e65 2e63 6f6d 6d69 745f 6465 6c65  gine.commit_dele
+000153a0: 7465 2873 656c 662c 2064 656c 6574 655f  te(self, delete_
+000153b0: 6466 2c20 7772 6974 655f 6f70 7469 6f6e  df, write_option
+000153c0: 7329 0a0a 2020 2020 6465 6620 6173 5f6f  s)..    def as_o
+000153d0: 6628 0a20 2020 2020 2020 2073 656c 662c  f(.        self,
+000153e0: 0a20 2020 2020 2020 2077 616c 6c63 6c6f  .        wallclo
+000153f0: 636b 5f74 696d 653a 204f 7074 696f 6e61  ck_time: Optiona
+00015400: 6c5b 556e 696f 6e5b 7374 722c 2069 6e74  l[Union[str, int
+00015410: 2c20 6461 7465 7469 6d65 2c20 6461 7465  , datetime, date
+00015420: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+00015430: 2020 2065 7863 6c75 6465 5f75 6e74 696c     exclude_until
+00015440: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
+00015450: 5b73 7472 2c20 696e 742c 2064 6174 6574  [str, int, datet
+00015460: 696d 652c 2064 6174 655d 5d20 3d20 4e6f  ime, date]] = No
+00015470: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+00015480: 2020 2022 2222 4765 7420 5175 6572 7920     """Get Query 
+00015490: 6f62 6a65 6374 2074 6f20 7265 7472 6965  object to retrie
+000154a0: 7665 2061 6c6c 2066 6561 7475 7265 7320  ve all features 
+000154b0: 6f66 2074 6865 2067 726f 7570 2061 7420  of the group at 
+000154c0: 6120 706f 696e 7420 696e 2074 6865 2070  a point in the p
+000154d0: 6173 742e 0a0a 2020 2020 2020 2020 5468  ast...        Th
+000154e0: 6973 206d 6574 686f 6420 7365 6c65 6374  is method select
+000154f0: 7320 616c 6c20 6665 6174 7572 6573 2069  s all features i
+00015500: 6e20 7468 6520 6665 6174 7572 6520 6772  n the feature gr
+00015510: 6f75 7020 616e 6420 7265 7475 726e 7320  oup and returns 
+00015520: 6120 5175 6572 7920 6f62 6a65 6374 0a20  a Query object. 
+00015530: 2020 2020 2020 2061 7420 7468 6520 7370         at the sp
+00015540: 6563 6966 6965 6420 706f 696e 7420 696e  ecified point in
+00015550: 2074 696d 652e 204f 7074 696f 6e61 6c6c   time. Optionall
+00015560: 792c 2063 6f6d 6d69 7473 2062 6566 6f72  y, commits befor
+00015570: 6520 6120 7370 6563 6966 6965 6420 706f  e a specified po
+00015580: 696e 7420 696e 2074 696d 6520 6361 6e20  int in time can 
+00015590: 6265 0a20 2020 2020 2020 2065 7863 6c75  be.        exclu
+000155a0: 6465 6420 6672 6f6d 2074 6865 2071 7565  ded from the que
+000155b0: 7279 2e20 5468 6520 5175 6572 7920 6361  ry. The Query ca
+000155c0: 6e20 7468 656e 2065 6974 6865 7220 6265  n then either be
+000155d0: 2072 6561 6420 696e 746f 2061 2044 6174   read into a Dat
+000155e0: 6166 7261 6d65 0a20 2020 2020 2020 206f  aframe.        o
+000155f0: 7220 7573 6564 2066 7572 7468 6572 2074  r used further t
+00015600: 6f20 7065 7266 6f72 6d20 6a6f 696e 7320  o perform joins 
+00015610: 6f72 2063 6f6e 7374 7275 6374 2061 2074  or construct a t
+00015620: 7261 696e 696e 6720 6461 7461 7365 742e  raining dataset.
+00015630: 0a0a 2020 2020 2020 2020 2121 2120 6578  ..        !!! ex
+00015640: 616d 706c 6520 2252 6561 6469 6e67 2066  ample "Reading f
+00015650: 6561 7475 7265 7320 6174 2061 2073 7065  eatures at a spe
+00015660: 6369 6669 6320 706f 696e 7420 696e 2074  cific point in t
+00015670: 696d 653a 220a 2020 2020 2020 2020 2020  ime:".          
+00015680: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
+00015690: 2020 2020 2020 2020 2320 636f 6e6e 6563          # connec
+000156a0: 7420 746f 2074 6865 2046 6561 7475 7265  t to the Feature
+000156b0: 2053 746f 7265 0a20 2020 2020 2020 2020   Store.         
+000156c0: 2020 2066 7320 3d20 2e2e 2e0a 0a20 2020     fs = .....   
+000156d0: 2020 2020 2020 2020 2023 2067 6574 2074           # get t
+000156e0: 6865 2046 6561 7475 7265 2047 726f 7570  he Feature Group
+000156f0: 2069 6e73 7461 6e63 650a 2020 2020 2020   instance.      
+00015700: 2020 2020 2020 6667 203d 2066 732e 6765        fg = fs.ge
+00015710: 745f 6f72 5f63 7265 6174 655f 6665 6174  t_or_create_feat
+00015720: 7572 655f 6772 6f75 7028 2e2e 2e29 0a0a  ure_group(...)..
+00015730: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
+00015740: 7420 6461 7461 2061 7420 6120 7370 6563  t data at a spec
+00015750: 6966 6963 2070 6f69 6e74 2069 6e20 7469  ific point in ti
+00015760: 6d65 2061 6e64 2073 686f 7720 6974 0a20  me and show it. 
+00015770: 2020 2020 2020 2020 2020 2066 672e 6173             fg.as
+00015780: 5f6f 6628 2232 3032 302d 3130 2d32 3020  _of("2020-10-20 
+00015790: 3037 3a33 343a 3131 2229 2e72 6561 6428  07:34:11").read(
+000157a0: 292e 7368 6f77 2829 0a20 2020 2020 2020  ).show().       
+000157b0: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
+000157c0: 2020 2121 2120 6578 616d 706c 6520 2252    !!! example "R
+000157d0: 6561 6469 6e67 2063 6f6d 6d69 7473 2069  eading commits i
+000157e0: 6e63 7265 6d65 6e74 616c 6c79 2062 6574  ncrementally bet
+000157f0: 7765 656e 2073 7065 6369 6669 6564 2070  ween specified p
+00015800: 6f69 6e74 7320 696e 2074 696d 653a 220a  oints in time:".
+00015810: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
+00015820: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
+00015830: 2020 6667 2e61 735f 6f66 2822 3230 3230    fg.as_of("2020
+00015840: 2d31 302d 3230 2030 373a 3334 3a31 3122  -10-20 07:34:11"
+00015850: 2c20 6578 636c 7564 655f 756e 7469 6c3d  , exclude_until=
+00015860: 2232 3032 302d 3130 2d31 3920 3037 3a33  "2020-10-19 07:3
+00015870: 343a 3131 2229 2e72 6561 6428 292e 7368  4:11").read().sh
+00015880: 6f77 2829 0a20 2020 2020 2020 2020 2020  ow().           
+00015890: 2060 6060 0a0a 2020 2020 2020 2020 5468   ```..        Th
+000158a0: 6520 6669 7273 7420 7061 7261 6d65 7465  e first paramete
+000158b0: 7220 6973 2069 6e63 6c75 7369 7665 2077  r is inclusive w
+000158c0: 6869 6c65 2074 6865 206c 6174 7465 7220  hile the latter 
+000158d0: 6973 2065 7863 6c75 7369 7665 2e0a 2020  is exclusive..  
+000158e0: 2020 2020 2020 5468 6174 206d 6561 6e73        That means
+000158f0: 2c20 696e 206f 7264 6572 2074 6f20 7175  , in order to qu
+00015900: 6572 7920 6120 7369 6e67 6c65 2063 6f6d  ery a single com
+00015910: 6d69 742c 2079 6f75 206e 6565 6420 746f  mit, you need to
+00015920: 2071 7565 7279 2074 6861 7420 636f 6d6d   query that comm
+00015930: 6974 2074 696d 650a 2020 2020 2020 2020  it time.        
+00015940: 616e 6420 6578 636c 7564 6520 6576 6572  and exclude ever
+00015950: 7974 6869 6e67 206a 7573 7420 6265 666f  ything just befo
+00015960: 7265 2074 6865 2063 6f6d 6d69 742e 0a0a  re the commit...
+00015970: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
+00015980: 706c 6520 2252 6561 6469 6e67 206f 6e6c  ple "Reading onl
+00015990: 7920 7468 6520 6368 616e 6765 7320 6672  y the changes fr
+000159a0: 6f6d 2061 2073 696e 676c 6520 636f 6d6d  om a single comm
+000159b0: 6974 220a 2020 2020 2020 2020 2020 2020  it".            
+000159c0: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
+000159d0: 2020 2020 2020 6667 2e61 735f 6f66 2822        fg.as_of("
+000159e0: 3230 3230 2d31 302d 3230 2030 373a 3331  2020-10-20 07:31
+000159f0: 3a33 3822 2c20 6578 636c 7564 655f 756e  :38", exclude_un
+00015a00: 7469 6c3d 2232 3032 302d 3130 2d32 3020  til="2020-10-20 
+00015a10: 3037 3a33 313a 3337 2229 2e72 6561 6428  07:31:37").read(
+00015a20: 292e 7368 6f77 2829 0a20 2020 2020 2020  ).show().       
+00015a30: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
+00015a40: 2020 5768 656e 206e 6f20 7761 6c6c 636c    When no wallcl
+00015a50: 6f63 6b5f 7469 6d65 2069 7320 6769 7665  ock_time is give
+00015a60: 6e2c 2074 6865 206c 6174 6573 7420 7374  n, the latest st
+00015a70: 6174 6520 6f66 2066 6561 7475 7265 7320  ate of features 
+00015a80: 6973 2072 6574 7572 6e65 642e 204f 7074  is returned. Opt
+00015a90: 696f 6e61 6c6c 792c 2063 6f6d 6d69 7473  ionally, commits
+00015aa0: 2062 6566 6f72 650a 2020 2020 2020 2020   before.        
+00015ab0: 6120 7370 6563 6966 6965 6420 706f 696e  a specified poin
+00015ac0: 7420 696e 2074 696d 6520 6361 6e20 7374  t in time can st
+00015ad0: 696c 6c20 6265 2065 7863 6c75 6465 642e  ill be excluded.
+00015ae0: 0a0a 2020 2020 2020 2020 2121 2120 6578  ..        !!! ex
+00015af0: 616d 706c 6520 2252 6561 6469 6e67 2074  ample "Reading t
+00015b00: 6865 206c 6174 6573 7420 7374 6174 6520  he latest state 
+00015b10: 6f66 2066 6561 7475 7265 732c 2065 7863  of features, exc
+00015b20: 6c75 6469 6e67 2063 6f6d 6d69 7473 2062  luding commits b
+00015b30: 6566 6f72 6520 6120 7370 6563 6966 6965  efore a specifie
+00015b40: 6420 706f 696e 7420 696e 2074 696d 653a  d point in time:
+00015b50: 220a 2020 2020 2020 2020 2020 2020 6060  ".            ``
+00015b60: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+00015b70: 2020 2020 6667 2e61 735f 6f66 284e 6f6e      fg.as_of(Non
+00015b80: 652c 2065 7863 6c75 6465 5f75 6e74 696c  e, exclude_until
+00015b90: 3d22 3230 3230 2d31 302d 3230 2030 373a  ="2020-10-20 07:
+00015ba0: 3331 3a33 3822 292e 7265 6164 2829 2e73  31:38").read().s
+00015bb0: 686f 7728 290a 2020 2020 2020 2020 2020  how().          
+00015bc0: 2020 6060 600a 0a20 2020 2020 2020 204e    ```..        N
+00015bd0: 6f74 6520 7468 6174 2074 6865 2069 6e74  ote that the int
+00015be0: 6572 7661 6c20 7769 6c6c 2062 6520 6170  erval will be ap
+00015bf0: 706c 6965 6420 746f 2061 6c6c 206a 6f69  plied to all joi
+00015c00: 6e73 2069 6e20 7468 6520 7175 6572 792e  ns in the query.
+00015c10: 0a20 2020 2020 2020 2049 6620 796f 7520  .        If you 
+00015c20: 7761 6e74 2074 6f20 7175 6572 7920 6469  want to query di
+00015c30: 6666 6572 656e 7420 696e 7465 7276 616c  fferent interval
+00015c40: 7320 666f 7220 6469 6666 6572 656e 7420  s for different 
+00015c50: 6665 6174 7572 6520 6772 6f75 7073 2069  feature groups i
+00015c60: 6e0a 2020 2020 2020 2020 7468 6520 7175  n.        the qu
+00015c70: 6572 792c 2079 6f75 2068 6176 6520 746f  ery, you have to
+00015c80: 2061 7070 6c79 2074 6865 6d20 696e 2061   apply them in a
+00015c90: 206e 6573 7465 6420 6661 7368 696f 6e3a   nested fashion:
+00015ca0: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
+00015cb0: 6d70 6c65 0a20 2020 2020 2020 2020 2020  mple.           
+00015cc0: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
+00015cd0: 2020 2020 2020 2023 2063 6f6e 6e65 6374         # connect
+00015ce0: 2074 6f20 7468 6520 4665 6174 7572 6520   to the Feature 
+00015cf0: 5374 6f72 650a 2020 2020 2020 2020 2020  Store.          
+00015d00: 2020 6673 203d 202e 2e2e 0a0a 2020 2020    fs = .....    
+00015d10: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
+00015d20: 6520 4665 6174 7572 6520 4772 6f75 7020  e Feature Group 
+00015d30: 696e 7374 616e 6365 0a20 2020 2020 2020  instance.       
+00015d40: 2020 2020 2066 6731 203d 2066 732e 6765       fg1 = fs.ge
+00015d50: 745f 6f72 5f63 7265 6174 655f 6665 6174  t_or_create_feat
+00015d60: 7572 655f 6772 6f75 7028 2e2e 2e29 0a20  ure_group(...). 
+00015d70: 2020 2020 2020 2020 2020 2066 6732 203d             fg2 =
+00015d80: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
+00015d90: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
+00015da0: 2e2e 2e29 0a0a 2020 2020 2020 2020 2020  ...)..          
+00015db0: 2020 6667 312e 7365 6c65 6374 5f61 6c6c    fg1.select_all
+00015dc0: 2829 2e61 735f 6f66 2822 3230 3230 2d31  ().as_of("2020-1
+00015dd0: 302d 3230 222c 2065 7863 6c75 6465 5f75  0-20", exclude_u
+00015de0: 6e74 696c 3d22 3230 3230 2d31 302d 3139  ntil="2020-10-19
+00015df0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00015e00: 2020 202e 6a6f 696e 2866 6732 2e73 656c     .join(fg2.sel
+00015e10: 6563 745f 616c 6c28 292e 6173 5f6f 6628  ect_all().as_of(
+00015e20: 2232 3032 302d 3130 2d32 3022 2c20 6578  "2020-10-20", ex
+00015e30: 636c 7564 655f 756e 7469 6c3d 2232 3032  clude_until="202
+00015e40: 302d 3130 2d31 3922 2929 0a20 2020 2020  0-10-19")).     
+00015e50: 2020 2020 2020 2060 6060 0a0a 2020 2020         ```..    
+00015e60: 2020 2020 4966 2069 6e73 7465 6164 2079      If instead y
+00015e70: 6f75 2061 7070 6c79 2061 6e6f 7468 6572  ou apply another
+00015e80: 2060 6173 5f6f 6660 2073 656c 6563 7469   `as_of` selecti
+00015e90: 6f6e 2061 6674 6572 2074 6865 206a 6f69  on after the joi
+00015ea0: 6e2c 2061 6c6c 0a20 2020 2020 2020 206a  n, all.        j
+00015eb0: 6f69 6e65 6420 6665 6174 7572 6520 6772  oined feature gr
+00015ec0: 6f75 7073 2077 696c 6c20 6265 2071 7565  oups will be que
+00015ed0: 7269 6564 2077 6974 6820 7468 6973 2069  ried with this i
+00015ee0: 6e74 6572 7661 6c3a 0a20 2020 2020 2020  nterval:.       
+00015ef0: 2021 2121 2065 7861 6d70 6c65 0a20 2020   !!! example.   
+00015f00: 2020 2020 2020 2020 2060 6060 7079 7468           ```pyth
+00015f10: 6f6e 0a20 2020 2020 2020 2020 2020 2066  on.            f
+00015f20: 6731 2e73 656c 6563 745f 616c 6c28 292e  g1.select_all().
+00015f30: 6173 5f6f 6628 2232 3032 302d 3130 2d32  as_of("2020-10-2
+00015f40: 3022 2c20 6578 636c 7564 655f 756e 7469  0", exclude_unti
+00015f50: 6c3d 2232 3032 302d 3130 2d31 3922 2920  l="2020-10-19") 
+00015f60: 2023 2061 735f 6f66 2069 7320 6e6f 7420   # as_of is not 
+00015f70: 6170 706c 6965 640a 2020 2020 2020 2020  applied.        
+00015f80: 2020 2020 2020 2020 2e6a 6f69 6e28 6667          .join(fg
+00015f90: 322e 7365 6c65 6374 5f61 6c6c 2829 2e61  2.select_all().a
+00015fa0: 735f 6f66 2822 3230 3230 2d31 302d 3230  s_of("2020-10-20
+00015fb0: 222c 2065 7863 6c75 6465 5f75 6e74 696c  ", exclude_until
+00015fc0: 3d22 3230 3230 2d31 302d 3135 2229 2920  ="2020-10-15")) 
+00015fd0: 2023 2061 735f 6f66 2069 7320 6e6f 7420   # as_of is not 
+00015fe0: 6170 706c 6965 640a 2020 2020 2020 2020  applied.        
+00015ff0: 2020 2020 2020 2020 2e61 735f 6f66 2822          .as_of("
+00016000: 3230 3230 2d31 302d 3230 222c 2065 7863  2020-10-20", exc
+00016010: 6c75 6465 5f75 6e74 696c 3d22 3230 3230  lude_until="2020
+00016020: 2d31 302d 3139 2229 0a20 2020 2020 2020  -10-19").       
+00016030: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
+00016040: 2020 2121 2120 7761 726e 696e 670a 2020    !!! warning.  
+00016050: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+00016060: 756e 6374 696f 6e20 6f6e 6c79 2077 6f72  unction only wor
+00016070: 6b73 2066 6f72 2066 6561 7475 7265 2067  ks for feature g
+00016080: 726f 7570 7320 7769 7468 2074 696d 655f  roups with time_
+00016090: 7472 6176 656c 5f66 6f72 6d61 743d 2748  travel_format='H
+000160a0: 5544 4927 2e0a 0a20 2020 2020 2020 2021  UDI'...        !
+000160b0: 2121 2077 6172 6e69 6e67 0a20 2020 2020  !! warning.     
+000160c0: 2020 2020 2020 2045 7863 6c75 6469 6e67         Excluding
+000160d0: 2063 6f6d 6d69 7473 2076 6961 2065 7863   commits via exc
+000160e0: 6c75 6465 5f75 6e74 696c 2069 7320 6f6e  lude_until is on
+000160f0: 6c79 2070 6f73 7369 626c 6520 7769 7468  ly possible with
+00016100: 696e 2074 6865 2072 616e 6765 206f 6620  in the range of 
+00016110: 7468 6520 4875 6469 2061 6374 6976 6520  the Hudi active 
+00016120: 7469 6d65 6c69 6e65 2e0a 2020 2020 2020  timeline..      
+00016130: 2020 2020 2020 4279 2064 6566 6175 6c74        By default
+00016140: 2c20 4875 6469 206b 6565 7073 2074 6865  , Hudi keeps the
+00016150: 206c 6173 7420 3230 2074 6f20 3330 2063   last 20 to 30 c
+00016160: 6f6d 6d69 7473 2069 6e20 7468 6520 6163  ommits in the ac
+00016170: 7469 7665 2074 696d 656c 696e 652e 0a20  tive timeline.. 
+00016180: 2020 2020 2020 2020 2020 2049 6620 796f             If yo
+00016190: 7520 6e65 6564 2074 6f20 6b65 6570 2061  u need to keep a
+000161a0: 206c 6f6e 6765 7220 6163 7469 7665 2074   longer active t
+000161b0: 696d 656c 696e 652c 2079 6f75 2063 616e  imeline, you can
+000161c0: 206f 7665 7277 7269 7465 2074 6865 206f   overwrite the o
+000161d0: 7074 696f 6e73 3a0a 2020 2020 2020 2020  ptions:.        
+000161e0: 2020 2020 6068 6f6f 6469 652e 6b65 6570      `hoodie.keep
+000161f0: 2e6d 696e 2e63 6f6d 6d69 7473 6020 616e  .min.commits` an
+00016200: 6420 6068 6f6f 6469 652e 6b65 6570 2e6d  d `hoodie.keep.m
+00016210: 6178 2e63 6f6d 6d69 7473 600a 2020 2020  ax.commits`.    
+00016220: 2020 2020 2020 2020 7768 656e 2063 616c          when cal
+00016230: 6c69 6e67 2074 6865 2060 696e 7365 7274  ling the `insert
+00016240: 2829 6020 6d65 7468 6f64 2e0a 0a20 2020  ()` method...   
+00016250: 2020 2020 2023 2041 7267 756d 656e 7473       # Arguments
+00016260: 0a20 2020 2020 2020 2020 2020 2077 616c  .            wal
+00016270: 6c63 6c6f 636b 5f74 696d 653a 2052 6561  lclock_time: Rea
+00016280: 6420 6461 7461 2061 7320 6f66 2074 6869  d data as of thi
+00016290: 7320 706f 696e 7420 696e 2074 696d 652e  s point in time.
+000162a0: 2053 7472 696e 6773 2073 686f 756c 6420   Strings should 
+000162b0: 6265 2066 6f72 6d61 7474 6564 2069 6e20  be formatted in 
+000162c0: 6f6e 6520 6f66 2074 6865 0a20 2020 2020  one of the.     
+000162d0: 2020 2020 2020 2020 2020 2066 6f6c 6c6f             follo
+000162e0: 7769 6e67 2066 6f72 6d61 7473 2060 2559  wing formats `%Y
+000162f0: 2d25 6d2d 2564 602c 2060 2559 2d25 6d2d  -%m-%d`, `%Y-%m-
+00016300: 2564 2025 4860 2c20 6025 592d 256d 2d25  %d %H`, `%Y-%m-%
+00016310: 6420 2548 3a25 4d60 2c20 6f72 2060 2559  d %H:%M`, or `%Y
+00016320: 2d25 6d2d 2564 2025 483a 254d 3a25 5360  -%m-%d %H:%M:%S`
+00016330: 2e0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+00016340: 636c 7564 655f 756e 7469 6c3a 2045 7863  clude_until: Exc
+00016350: 6c75 6465 2063 6f6d 6d69 7473 2075 6e74  lude commits unt
+00016360: 696c 2074 6869 7320 706f 696e 7420 696e  il this point in
+00016370: 2074 696d 652e 2053 7472 696e 6720 7368   time. String sh
+00016380: 6f75 6c64 2062 6520 666f 726d 6174 7465  ould be formatte
+00016390: 6420 696e 206f 6e65 206f 6620 7468 650a  d in one of the.
+000163a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000163b0: 666f 6c6c 6f77 696e 6720 666f 726d 6174  following format
+000163c0: 7320 6025 592d 256d 2d25 6460 2c20 6025  s `%Y-%m-%d`, `%
+000163d0: 592d 256d 2d25 6420 2548 602c 2060 2559  Y-%m-%d %H`, `%Y
+000163e0: 2d25 6d2d 2564 2025 483a 254d 602c 206f  -%m-%d %H:%M`, o
+000163f0: 7220 6025 592d 256d 2d25 6420 2548 3a25  r `%Y-%m-%d %H:%
+00016400: 4d3a 2553 602e 0a0a 2020 2020 2020 2020  M:%S`...        
+00016410: 2320 5265 7475 726e 730a 2020 2020 2020  # Returns.      
+00016420: 2020 2020 2020 6051 7565 7279 602e 2054        `Query`. T
+00016430: 6865 2071 7565 7279 206f 626a 6563 7420  he query object 
+00016440: 7769 7468 2074 6865 2061 7070 6c69 6564  with the applied
+00016450: 2074 696d 6520 7472 6176 656c 2063 6f6e   time travel con
+00016460: 6469 7469 6f6e 2e0a 2020 2020 2020 2020  dition..        
+00016470: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00016480: 726e 2073 656c 662e 7365 6c65 6374 5f61  rn self.select_a
+00016490: 6c6c 2829 2e61 735f 6f66 2877 616c 6c63  ll().as_of(wallc
+000164a0: 6c6f 636b 5f74 696d 652c 2065 7863 6c75  lock_time, exclu
+000164b0: 6465 5f75 6e74 696c 290a 0a20 2020 2064  de_until)..    d
+000164c0: 6566 2063 6f6d 7075 7465 5f73 7461 7469  ef compute_stati
+000164d0: 7374 6963 7328 0a20 2020 2020 2020 2073  stics(.        s
+000164e0: 656c 662c 2077 616c 6c63 6c6f 636b 5f74  elf, wallclock_t
+000164f0: 696d 653a 204f 7074 696f 6e61 6c5b 556e  ime: Optional[Un
+00016500: 696f 6e5b 7374 722c 2069 6e74 2c20 6461  ion[str, int, da
+00016510: 7465 7469 6d65 2c20 6461 7465 5d5d 203d  tetime, date]] =
+00016520: 204e 6f6e 650a 2020 2020 293a 0a20 2020   None.    ):.   
+00016530: 2020 2020 2022 2222 5265 636f 6d70 7574       """Recomput
+00016540: 6520 7468 6520 7374 6174 6973 7469 6373  e the statistics
+00016550: 2066 6f72 2074 6865 2066 6561 7475 7265   for the feature
+00016560: 2067 726f 7570 2061 6e64 2073 6176 6520   group and save 
+00016570: 7468 656d 2074 6f20 7468 650a 2020 2020  them to the.    
+00016580: 2020 2020 6665 6174 7572 6520 7374 6f72      feature stor
+00016590: 652e 0a0a 2020 2020 2020 2020 5374 6174  e...        Stat
+000165a0: 6973 7469 6373 2061 7265 206f 6e6c 7920  istics are only 
+000165b0: 636f 6d70 7574 6564 2066 6f72 2064 6174  computed for dat
+000165c0: 6120 696e 2074 6865 206f 6666 6c69 6e65  a in the offline
+000165d0: 2073 746f 7261 6765 206f 6620 7468 6520   storage of the 
+000165e0: 6665 6174 7572 650a 2020 2020 2020 2020  feature.        
+000165f0: 6772 6f75 702e 0a0a 2020 2020 2020 2020  group...        
+00016600: 2320 4172 6775 6d65 6e74 730a 2020 2020  # Arguments.    
+00016610: 2020 2020 2020 2020 7761 6c6c 636c 6f63          wallcloc
+00016620: 6b5f 7469 6d65 3a20 4966 2073 7065 6369  k_time: If speci
+00016630: 6669 6564 2077 696c 6c20 7265 636f 6d70  fied will recomp
+00016640: 7574 6520 7374 6174 6973 7469 6373 206f  ute statistics o
+00016650: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00016660: 2020 6665 6174 7572 6520 6772 6f75 7020    feature group 
+00016670: 6173 206f 6620 7370 6563 6966 6963 2070  as of specific p
+00016680: 6f69 6e74 2069 6e20 7469 6d65 2e20 4966  oint in time. If
+00016690: 206e 6f74 2073 7065 6369 6669 6564 2074   not specified t
+000166a0: 6865 6e20 7769 6c6c 2063 6f6d 7075 7465  hen will compute
+000166b0: 2073 7461 7469 7374 6963 730a 2020 2020   statistics.    
+000166c0: 2020 2020 2020 2020 2020 2020 6173 206f              as o
+000166d0: 6620 6d6f 7374 2072 6563 656e 7420 7469  f most recent ti
+000166e0: 6d65 206f 6620 7468 6973 2066 6561 7475  me of this featu
+000166f0: 7265 2067 726f 7570 2e20 4465 6661 756c  re group. Defaul
+00016700: 7473 2074 6f20 604e 6f6e 6560 2e20 5374  ts to `None`. St
+00016710: 7269 6e67 7320 7368 6f75 6c64 0a20 2020  rings should.   
+00016720: 2020 2020 2020 2020 2020 2020 2062 6520               be 
+00016730: 666f 726d 6174 7465 6420 696e 206f 6e65  formatted in one
+00016740: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
+00016750: 6720 666f 726d 6174 7320 6025 592d 256d  g formats `%Y-%m
+00016760: 2d25 6460 2c20 6025 592d 256d 2d25 6420  -%d`, `%Y-%m-%d 
+00016770: 2548 602c 2060 2559 2d25 6d2d 2564 2025  %H`, `%Y-%m-%d %
+00016780: 483a 254d 602c 2060 2559 2d25 6d2d 2564  H:%M`, `%Y-%m-%d
+00016790: 2025 483a 254d 3a25 5360 2c0a 2020 2020   %H:%M:%S`,.    
+000167a0: 2020 2020 2020 2020 2020 2020 6f72 2060              or `
+000167b0: 2559 2d25 6d2d 2564 2025 483a 254d 3a25  %Y-%m-%d %H:%M:%
+000167c0: 532e 2566 602e 0a0a 2020 2020 2020 2020  S.%f`...        
+000167d0: 2320 5265 7475 726e 730a 2020 2020 2020  # Returns.      
+000167e0: 2020 2020 2020 6053 7461 7469 7374 6963        `Statistic
+000167f0: 7360 2e20 5468 6520 7374 6174 6973 7469  s`. The statisti
+00016800: 6373 206d 6574 6164 6174 6120 6f62 6a65  cs metadata obje
+00016810: 6374 2e0a 0a20 2020 2020 2020 2023 2052  ct...        # R
+00016820: 6169 7365 730a 2020 2020 2020 2020 2020  aises.          
+00016830: 2020 6068 7366 732e 636c 6965 6e74 2e65    `hsfs.client.e
+00016840: 7863 6570 7469 6f6e 732e 5265 7374 4150  xceptions.RestAP
+00016850: 4945 7272 6f72 602e 2055 6e61 626c 6520  IError`. Unable 
+00016860: 746f 2070 6572 7369 7374 2074 6865 2073  to persist the s
+00016870: 7461 7469 7374 6963 732e 0a20 2020 2020  tatistics..     
+00016880: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00016890: 6620 7365 6c66 2e73 7461 7469 7374 6963  f self.statistic
+000168a0: 735f 636f 6e66 6967 2e65 6e61 626c 6564  s_config.enabled
+000168b0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+000168c0: 446f 6e27 7420 7265 6164 2074 6865 2064  Don't read the d
+000168d0: 6174 6166 7261 6d65 2068 6572 652c 2074  ataframe here, t
+000168e0: 6f20 6176 6f69 6420 7472 6967 6765 7269  o avoid triggeri
+000168f0: 6e67 2061 2072 6561 6420 6f70 6572 6174  ng a read operat
+00016900: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00016910: 2320 666f 7220 7468 6520 5079 7468 6f6e  # for the Python
+00016920: 2065 6e67 696e 652e 2054 6865 2050 7974   engine. The Pyt
+00016930: 686f 6e20 656e 6769 6e65 2069 7320 676f  hon engine is go
+00016940: 696e 6720 746f 2073 6574 7570 2061 2053  ing to setup a S
+00016950: 7061 726b 204a 6f62 0a20 2020 2020 2020  park Job.       
+00016960: 2020 2020 2023 2074 6f20 7570 6461 7465       # to update
+00016970: 2074 6865 2073 7461 7469 7374 6963 732e   the statistics.
+00016980: 0a0a 2020 2020 2020 2020 2020 2020 6667  ..            fg
+00016990: 5f63 6f6d 6d69 745f 6964 203d 204e 6f6e  _commit_id = Non
+000169a0: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+000169b0: 2077 616c 6c63 6c6f 636b 5f74 696d 6520   wallclock_time 
+000169c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000169d0: 2020 2020 2020 2020 2020 2020 2023 2052               # R
+000169e0: 6574 7269 6576 6520 6667 2063 6f6d 6d69  etrieve fg commi
+000169f0: 7420 6964 2072 656c 6174 6564 2074 6f20  t id related to 
+00016a00: 7468 6973 2077 616c 6c20 636c 6f63 6b20  this wall clock 
+00016a10: 7469 6d65 2061 6e64 2072 6563 6f6d 7075  time and recompu
+00016a20: 7465 2073 7461 7469 7374 6963 732e 2049  te statistics. I
+00016a30: 7420 7769 6c6c 2074 6872 6f77 0a20 2020  t will throw.   
+00016a40: 2020 2020 2020 2020 2020 2020 2023 2065               # e
+00016a50: 7863 6570 7469 6f6e 2069 6620 6974 7320  xception if its 
+00016a60: 6e6f 7420 7469 6d65 2074 7261 7665 6c20  not time travel 
+00016a70: 656e 6162 6c65 6420 6665 6174 7572 6520  enabled feature 
+00016a80: 6772 6f75 702e 0a20 2020 2020 2020 2020  group..         
+00016a90: 2020 2020 2020 2066 675f 636f 6d6d 6974         fg_commit
+00016aa0: 5f69 6420 3d20 5b0a 2020 2020 2020 2020  _id = [.        
+00016ab0: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
+00016ac0: 6974 5f69 640a 2020 2020 2020 2020 2020  it_id.          
+00016ad0: 2020 2020 2020 2020 2020 666f 7220 636f            for co
+00016ae0: 6d6d 6974 5f69 6420 696e 2073 656c 662e  mmit_id in self.
+00016af0: 5f66 6561 7475 7265 5f67 726f 7570 5f65  _feature_group_e
+00016b00: 6e67 696e 652e 636f 6d6d 6974 5f64 6574  ngine.commit_det
+00016b10: 6169 6c73 280a 2020 2020 2020 2020 2020  ails(.          
+00016b20: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016b30: 6c66 2c20 7761 6c6c 636c 6f63 6b5f 7469  lf, wallclock_ti
+00016b40: 6d65 2c20 310a 2020 2020 2020 2020 2020  me, 1.          
+00016b50: 2020 2020 2020 2020 2020 292e 6b65 7973            ).keys
+00016b60: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00016b70: 2020 205d 5b30 5d0a 0a20 2020 2020 2020     ][0]..       
+00016b80: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00016b90: 2e5f 7374 6174 6973 7469 6373 5f65 6e67  ._statistics_eng
+00016ba0: 696e 652e 636f 6d70 7574 655f 7374 6174  ine.compute_stat
+00016bb0: 6973 7469 6373 280a 2020 2020 2020 2020  istics(.        
+00016bc0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00016bd0: 2020 2020 2020 2020 2020 2020 2020 6665                fe
+00016be0: 6174 7572 655f 6772 6f75 705f 636f 6d6d  ature_group_comm
+00016bf0: 6974 5f69 643d 6667 5f63 6f6d 6d69 745f  it_id=fg_commit_
+00016c00: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
+00016c10: 2020 2069 6620 6667 5f63 6f6d 6d69 745f     if fg_commit_
+00016c20: 6964 2069 7320 6e6f 7420 4e6f 6e65 0a20  id is not None. 
+00016c30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00016c40: 6c73 6520 4e6f 6e65 2c0a 2020 2020 2020  lse None,.      
+00016c50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00016c60: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00016c70: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
+00016c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016c90: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00016ca0: 2020 2020 2020 2022 5468 6520 7374 6174         "The stat
+00016cb0: 6973 7469 6373 2061 7265 206e 6f74 2065  istics are not e
+00016cc0: 6e61 626c 6564 206f 6620 6665 6174 7572  nabled of featur
+00016cd0: 6520 6772 6f75 7020 607b 7d60 2c20 7769  e group `{}`, wi
+00016ce0: 7468 2076 6572 7369 6f6e 220a 2020 2020  th version".    
+00016cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d00: 2220 607b 7d60 2e20 4e6f 2073 7461 7469  " `{}`. No stati
+00016d10: 7374 6963 7320 636f 6d70 7574 6564 2e22  stics computed."
+00016d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016d30: 2029 2e66 6f72 6d61 7428 7365 6c66 2e5f   ).format(self._
+00016d40: 6e61 6d65 2c20 7365 6c66 2e5f 7665 7273  name, self._vers
+00016d50: 696f 6e29 2c0a 2020 2020 2020 2020 2020  ion),.          
+00016d60: 2020 2020 2020 7574 696c 2e53 746f 7261        util.Stora
+00016d70: 6765 5761 726e 696e 672c 0a20 2020 2020  geWarning,.     
+00016d80: 2020 2020 2020 2029 0a0a 2020 2020 4063         )..    @c
+00016d90: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00016da0: 6566 2066 726f 6d5f 7265 7370 6f6e 7365  ef from_response
+00016db0: 5f6a 736f 6e28 636c 732c 206a 736f 6e5f  _json(cls, json_
+00016dc0: 6469 6374 293a 0a20 2020 2020 2020 206a  dict):.        j
+00016dd0: 736f 6e5f 6465 6361 6d65 6c69 7a65 6420  son_decamelized 
+00016de0: 3d20 6875 6d70 732e 6465 6361 6d65 6c69  = humps.decameli
+00016df0: 7a65 286a 736f 6e5f 6469 6374 290a 2020  ze(json_dict).  
+00016e00: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00016e10: 6e63 6528 6a73 6f6e 5f64 6563 616d 656c  nce(json_decamel
+00016e20: 697a 6564 2c20 6469 6374 293a 0a20 2020  ized, dict):.   
+00016e30: 2020 2020 2020 2020 2069 6620 2274 7970           if "typ
+00016e40: 6522 2069 6e20 6a73 6f6e 5f64 6563 616d  e" in json_decam
+00016e50: 656c 697a 6564 3a0a 2020 2020 2020 2020  elized:.        
+00016e60: 2020 2020 2020 2020 6a73 6f6e 5f64 6563          json_dec
+00016e70: 616d 656c 697a 6564 5b22 7374 7265 616d  amelized["stream
+00016e80: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
+00016e90: 2020 2020 2020 2020 2020 206a 736f 6e5f             json_
+00016ea0: 6465 6361 6d65 6c69 7a65 645b 2274 7970  decamelized["typ
+00016eb0: 6522 5d20 3d3d 2022 7374 7265 616d 4665  e"] == "streamFe
+00016ec0: 6174 7572 6547 726f 7570 4454 4f22 0a20  atureGroupDTO". 
+00016ed0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00016ee0: 0a20 2020 2020 2020 2020 2020 205f 203d  .            _ =
+00016ef0: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
+00016f00: 642e 706f 7028 2274 7970 6522 2c20 4e6f  d.pop("type", No
+00016f10: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
+00016f20: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
+00016f30: 2e70 6f70 2822 7661 6c69 6461 7469 6f6e  .pop("validation
+00016f40: 5f74 7970 6522 2c20 4e6f 6e65 290a 2020  _type", None).  
+00016f50: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00016f60: 2063 6c73 282a 2a6a 736f 6e5f 6465 6361   cls(**json_deca
+00016f70: 6d65 6c69 7a65 6429 0a20 2020 2020 2020  melized).       
+00016f80: 2066 6f72 2066 6720 696e 206a 736f 6e5f   for fg in json_
+00016f90: 6465 6361 6d65 6c69 7a65 643a 0a20 2020  decamelized:.   
+00016fa0: 2020 2020 2020 2020 2069 6620 2274 7970           if "typ
+00016fb0: 6522 2069 6e20 6667 3a0a 2020 2020 2020  e" in fg:.      
+00016fc0: 2020 2020 2020 2020 2020 6667 5b22 7374            fg["st
+00016fd0: 7265 616d 225d 203d 2066 675b 2274 7970  ream"] = fg["typ
+00016fe0: 6522 5d20 3d3d 2022 7374 7265 616d 4665  e"] == "streamFe
+00016ff0: 6174 7572 6547 726f 7570 4454 4f22 0a20  atureGroupDTO". 
+00017000: 2020 2020 2020 2020 2020 205f 203d 2066             _ = f
+00017010: 672e 706f 7028 2274 7970 6522 2c20 4e6f  g.pop("type", No
+00017020: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
+00017030: 6667 2e70 6f70 2822 7661 6c69 6461 7469  fg.pop("validati
+00017040: 6f6e 5f74 7970 6522 2c20 4e6f 6e65 290a  on_type", None).
+00017050: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+00017060: 636c 7328 2a2a 6667 2920 666f 7220 6667  cls(**fg) for fg
+00017070: 2069 6e20 6a73 6f6e 5f64 6563 616d 656c   in json_decamel
+00017080: 697a 6564 5d0a 0a20 2020 2064 6566 2075  ized]..    def u
+00017090: 7064 6174 655f 6672 6f6d 5f72 6573 706f  pdate_from_respo
+000170a0: 6e73 655f 6a73 6f6e 2873 656c 662c 206a  nse_json(self, j
+000170b0: 736f 6e5f 6469 6374 293a 0a20 2020 2020  son_dict):.     
+000170c0: 2020 206a 736f 6e5f 6465 6361 6d65 6c69     json_decameli
+000170d0: 7a65 6420 3d20 6875 6d70 732e 6465 6361  zed = humps.deca
+000170e0: 6d65 6c69 7a65 286a 736f 6e5f 6469 6374  melize(json_dict
+000170f0: 290a 2020 2020 2020 2020 6a73 6f6e 5f64  ).        json_d
+00017100: 6563 616d 656c 697a 6564 5b22 7374 7265  ecamelized["stre
+00017110: 616d 225d 203d 206a 736f 6e5f 6465 6361  am"] = json_deca
+00017120: 6d65 6c69 7a65 645b 2274 7970 6522 5d20  melized["type"] 
+00017130: 3d3d 2022 7374 7265 616d 4665 6174 7572  == "streamFeatur
+00017140: 6547 726f 7570 4454 4f22 0a20 2020 2020  eGroupDTO".     
+00017150: 2020 205f 203d 206a 736f 6e5f 6465 6361     _ = json_deca
+00017160: 6d65 6c69 7a65 642e 706f 7028 2274 7970  melized.pop("typ
+00017170: 6522 290a 2020 2020 2020 2020 7365 6c66  e").        self
+00017180: 2e5f 5f69 6e69 745f 5f28 2a2a 6a73 6f6e  .__init__(**json
+00017190: 5f64 6563 616d 656c 697a 6564 290a 2020  _decamelized).  
+000171a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000171b0: 660a 0a20 2020 2064 6566 206a 736f 6e28  f..    def json(
+000171c0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+000171d0: 2222 4765 7420 7370 6563 6966 6963 2046  ""Get specific F
+000171e0: 6561 7475 7265 2047 726f 7570 206d 6574  eature Group met
+000171f0: 6164 6174 6120 696e 206a 736f 6e20 666f  adata in json fo
+00017200: 726d 6174 2e0a 0a20 2020 2020 2020 2021  rmat...        !
+00017210: 2121 2065 7861 6d70 6c65 0a20 2020 2020  !! example.     
+00017220: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+00017230: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
+00017240: 6a73 6f6e 2829 0a20 2020 2020 2020 2020  json().         
+00017250: 2020 2060 6060 0a20 2020 2020 2020 2022     ```.        "
+00017260: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00017270: 6e20 6a73 6f6e 2e64 756d 7073 2873 656c  n json.dumps(sel
+00017280: 662c 2063 6c73 3d75 7469 6c2e 4665 6174  f, cls=util.Feat
+00017290: 7572 6553 746f 7265 456e 636f 6465 7229  ureStoreEncoder)
+000172a0: 0a0a 2020 2020 6465 6620 746f 5f64 6963  ..    def to_dic
+000172b0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+000172c0: 2022 2222 4765 7420 7374 7275 6374 7572   """Get structur
+000172d0: 6564 2069 6e66 6f20 6162 6f75 7420 7370  ed info about sp
+000172e0: 6563 6966 6963 2046 6561 7475 7265 2047  ecific Feature G
+000172f0: 726f 7570 2069 6e20 7079 7468 6f6e 2064  roup in python d
+00017300: 6963 7469 6f6e 6172 7920 666f 726d 6174  ictionary format
+00017310: 2e0a 0a20 2020 2020 2020 2021 2121 2065  ...        !!! e
+00017320: 7861 6d70 6c65 0a20 2020 2020 2020 2020  xample.         
+00017330: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+00017340: 2020 2020 2020 2020 2023 2063 6f6e 6e65           # conne
+00017350: 6374 2074 6f20 7468 6520 4665 6174 7572  ct to the Featur
+00017360: 6520 5374 6f72 650a 2020 2020 2020 2020  e Store.        
+00017370: 2020 2020 6673 203d 202e 2e2e 0a0a 2020      fs = .....  
+00017380: 2020 2020 2020 2020 2020 2320 6765 7420            # get 
+00017390: 7468 6520 4665 6174 7572 6520 4772 6f75  the Feature Grou
+000173a0: 7020 696e 7374 616e 6365 0a20 2020 2020  p instance.     
+000173b0: 2020 2020 2020 2066 6720 3d20 6673 2e67         fg = fs.g
+000173c0: 6574 5f6f 725f 6372 6561 7465 5f66 6561  et_or_create_fea
+000173d0: 7475 7265 5f67 726f 7570 282e 2e2e 290a  ture_group(...).
+000173e0: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
+000173f0: 746f 5f64 6963 7428 290a 2020 2020 2020  to_dict().      
+00017400: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00017410: 2020 2222 220a 2020 2020 2020 2020 6667    """.        fg
+00017420: 5f6d 6574 615f 6469 6374 203d 207b 0a20  _meta_dict = {. 
+00017430: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
+00017440: 2073 656c 662e 5f69 642c 0a20 2020 2020   self._id,.     
+00017450: 2020 2020 2020 2022 6e61 6d65 223a 2073         "name": s
+00017460: 656c 662e 5f6e 616d 652c 0a20 2020 2020  elf._name,.     
+00017470: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
+00017480: 3a20 7365 6c66 2e5f 7665 7273 696f 6e2c  : self._version,
+00017490: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
+000174a0: 7363 7269 7074 696f 6e22 3a20 7365 6c66  scription": self
+000174b0: 2e5f 6465 7363 7269 7074 696f 6e2c 0a20  ._description,. 
+000174c0: 2020 2020 2020 2020 2020 2022 6f6e 6c69             "onli
+000174d0: 6e65 456e 6162 6c65 6422 3a20 7365 6c66  neEnabled": self
+000174e0: 2e5f 6f6e 6c69 6e65 5f65 6e61 626c 6564  ._online_enabled
+000174f0: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
+00017500: 696d 6554 7261 7665 6c46 6f72 6d61 7422  imeTravelFormat"
+00017510: 3a20 7365 6c66 2e5f 7469 6d65 5f74 7261  : self._time_tra
+00017520: 7665 6c5f 666f 726d 6174 2c0a 2020 2020  vel_format,.    
+00017530: 2020 2020 2020 2020 2266 6561 7475 7265          "feature
+00017540: 7322 3a20 7365 6c66 2e5f 6665 6174 7572  s": self._featur
+00017550: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00017560: 2266 6561 7475 7265 7374 6f72 6549 6422  "featurestoreId"
+00017570: 3a20 7365 6c66 2e5f 6665 6174 7572 655f  : self._feature_
+00017580: 7374 6f72 655f 6964 2c0a 2020 2020 2020  store_id,.      
+00017590: 2020 2020 2020 2274 7970 6522 3a20 2263        "type": "c
+000175a0: 6163 6865 6446 6561 7475 7265 6772 6f75  achedFeaturegrou
+000175b0: 7044 544f 220a 2020 2020 2020 2020 2020  pDTO".          
+000175c0: 2020 6966 206e 6f74 2073 656c 662e 5f73    if not self._s
+000175d0: 7472 6561 6d0a 2020 2020 2020 2020 2020  tream.          
+000175e0: 2020 656c 7365 2022 7374 7265 616d 4665    else "streamFe
+000175f0: 6174 7572 6547 726f 7570 4454 4f22 2c0a  atureGroupDTO",.
+00017600: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
+00017610: 7469 7374 6963 7343 6f6e 6669 6722 3a20  tisticsConfig": 
+00017620: 7365 6c66 2e5f 7374 6174 6973 7469 6373  self._statistics
+00017630: 5f63 6f6e 6669 672c 0a20 2020 2020 2020  _config,.       
+00017640: 2020 2020 2022 6576 656e 7454 696d 6522       "eventTime"
+00017650: 3a20 7365 6c66 2e65 7665 6e74 5f74 696d  : self.event_tim
+00017660: 652c 0a20 2020 2020 2020 2020 2020 2022  e,.            "
+00017670: 6578 7065 6374 6174 696f 6e53 7569 7465  expectationSuite
+00017680: 223a 2073 656c 662e 5f65 7870 6563 7461  ": self._expecta
+00017690: 7469 6f6e 5f73 7569 7465 2c0a 2020 2020  tion_suite,.    
+000176a0: 2020 2020 2020 2020 2270 6172 656e 7473          "parents
+000176b0: 223a 2073 656c 662e 5f70 6172 656e 7473  ": self._parents
+000176c0: 2c0a 2020 2020 2020 2020 7d0a 2020 2020  ,.        }.    
+000176d0: 2020 2020 6966 2073 656c 662e 5f73 7472      if self._str
+000176e0: 6561 6d3a 0a20 2020 2020 2020 2020 2020  eam:.           
+000176f0: 2066 675f 6d65 7461 5f64 6963 745b 2264   fg_meta_dict["d
+00017700: 656c 7461 5374 7265 616d 6572 4a6f 6243  eltaStreamerJobC
+00017710: 6f6e 6622 5d20 3d20 7365 6c66 2e5f 6465  onf"] = self._de
+00017720: 6c74 6173 7472 6561 6d65 725f 6a6f 6263  ltastreamer_jobc
+00017730: 6f6e 660a 2020 2020 2020 2020 7265 7475  onf.        retu
+00017740: 726e 2066 675f 6d65 7461 5f64 6963 740a  rn fg_meta_dict.
+00017750: 0a20 2020 2064 6566 205f 6765 745f 7461  .    def _get_ta
+00017760: 626c 655f 6e61 6d65 2873 656c 6629 3a0a  ble_name(self):.
+00017770: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00017780: 656c 662e 6665 6174 7572 655f 7374 6f72  elf.feature_stor
+00017790: 655f 6e61 6d65 202b 2022 2e22 202b 2073  e_name + "." + s
+000177a0: 656c 662e 6e61 6d65 202b 2022 5f22 202b  elf.name + "_" +
+000177b0: 2073 7472 2873 656c 662e 7665 7273 696f   str(self.versio
+000177c0: 6e29 0a0a 2020 2020 6465 6620 5f67 6574  n)..    def _get
+000177d0: 5f6f 6e6c 696e 655f 7461 626c 655f 6e61  _online_table_na
+000177e0: 6d65 2873 656c 6629 3a0a 2020 2020 2020  me(self):.      
+000177f0: 2020 7265 7475 726e 2073 656c 662e 6e61    return self.na
+00017800: 6d65 202b 2022 5f22 202b 2073 7472 2873  me + "_" + str(s
+00017810: 656c 662e 7665 7273 696f 6e29 0a0a 2020  elf.version)..  
+00017820: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00017830: 6465 6620 6964 2873 656c 6629 3a0a 2020  def id(self):.  
+00017840: 2020 2020 2020 2222 2246 6561 7475 7265        """Feature
+00017850: 2067 726f 7570 2069 642e 2222 220a 2020   group id.""".  
+00017860: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00017870: 662e 5f69 640a 0a20 2020 2040 7072 6f70  f._id..    @prop
+00017880: 6572 7479 0a20 2020 2064 6566 206e 616d  erty.    def nam
+00017890: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000178a0: 2022 2222 4e61 6d65 206f 6620 7468 6520   """Name of the 
+000178b0: 6665 6174 7572 6520 6772 6f75 702e 2222  feature group.""
+000178c0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+000178d0: 2073 656c 662e 5f6e 616d 650a 0a20 2020   self._name..   
+000178e0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+000178f0: 6566 2076 6572 7369 6f6e 2873 656c 6629  ef version(self)
+00017900: 3a0a 2020 2020 2020 2020 2222 2256 6572  :.        """Ver
+00017910: 7369 6f6e 206e 756d 6265 7220 6f66 2074  sion number of t
+00017920: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
+00017930: 2e22 2222 0a20 2020 2020 2020 2072 6574  .""".        ret
+00017940: 7572 6e20 7365 6c66 2e5f 7665 7273 696f  urn self._versio
+00017950: 6e0a 0a20 2020 2040 7072 6f70 6572 7479  n..    @property
+00017960: 0a20 2020 2064 6566 2064 6573 6372 6970  .    def descrip
+00017970: 7469 6f6e 2873 656c 6629 3a0a 2020 2020  tion(self):.    
+00017980: 2020 2020 2222 2244 6573 6372 6970 7469      """Descripti
+00017990: 6f6e 206f 6620 7468 6520 6665 6174 7572  on of the featur
+000179a0: 6520 6772 6f75 7020 636f 6e74 656e 7473  e group contents
+000179b0: 2e22 2222 0a20 2020 2020 2020 2072 6574  .""".        ret
+000179c0: 7572 6e20 7365 6c66 2e5f 6465 7363 7269  urn self._descri
+000179d0: 7074 696f 6e0a 0a20 2020 2040 7072 6f70  ption..    @prop
+000179e0: 6572 7479 0a20 2020 2064 6566 2066 6561  erty.    def fea
+000179f0: 7475 7265 7328 7365 6c66 293a 0a20 2020  tures(self):.   
+00017a00: 2020 2020 2022 2222 5363 6865 6d61 2069       """Schema i
+00017a10: 6e66 6f72 6d61 7469 6f6e 2e22 2222 0a20  nformation.""". 
+00017a20: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00017a30: 6c66 2e5f 6665 6174 7572 6573 0a0a 2020  lf._features..  
+00017a40: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00017a50: 6465 6620 7469 6d65 5f74 7261 7665 6c5f  def time_travel_
+00017a60: 666f 726d 6174 2873 656c 6629 3a0a 2020  format(self):.  
+00017a70: 2020 2020 2020 2222 2253 6574 7469 6e67        """Setting
+00017a80: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
+00017a90: 6772 6f75 7020 7469 6d65 2074 7261 7665  group time trave
+00017aa0: 6c20 666f 726d 6174 2e22 2222 0a20 2020  l format.""".   
+00017ab0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00017ac0: 2e5f 7469 6d65 5f74 7261 7665 6c5f 666f  ._time_travel_fo
+00017ad0: 726d 6174 0a0a 2020 2020 4070 726f 7065  rmat..    @prope
+00017ae0: 7274 790a 2020 2020 6465 6620 7061 7274  rty.    def part
+00017af0: 6974 696f 6e5f 6b65 7928 7365 6c66 293a  ition_key(self):
+00017b00: 0a20 2020 2020 2020 2022 2222 4c69 7374  .        """List
+00017b10: 206f 6620 6665 6174 7572 6573 2062 7569   of features bui
+00017b20: 6c64 696e 6720 7468 6520 7061 7274 6974  lding the partit
+00017b30: 696f 6e20 6b65 792e 2222 220a 2020 2020  ion key.""".    
+00017b40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00017b50: 5f70 6172 7469 7469 6f6e 5f6b 6579 0a0a  _partition_key..
+00017b60: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00017b70: 2020 6465 6620 6875 6469 5f70 7265 636f    def hudi_preco
+00017b80: 6d62 696e 655f 6b65 7928 7365 6c66 293a  mbine_key(self):
+00017b90: 0a20 2020 2020 2020 2022 2222 4665 6174  .        """Feat
+00017ba0: 7572 6520 6e61 6d65 2074 6861 7420 6973  ure name that is
+00017bb0: 2074 6865 2068 7564 6920 7072 6563 6f6d   the hudi precom
+00017bc0: 6269 6e65 206b 6579 2e22 2222 0a20 2020  bine key.""".   
+00017bd0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00017be0: 2e5f 6875 6469 5f70 7265 636f 6d62 696e  ._hudi_precombin
+00017bf0: 655f 6b65 790a 0a20 2020 2040 7072 6f70  e_key..    @prop
+00017c00: 6572 7479 0a20 2020 2064 6566 2066 6561  erty.    def fea
+00017c10: 7475 7265 5f73 746f 7265 5f69 6428 7365  ture_store_id(se
+00017c20: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+00017c30: 7572 6e20 7365 6c66 2e5f 6665 6174 7572  urn self._featur
+00017c40: 655f 7374 6f72 655f 6964 0a0a 2020 2020  e_store_id..    
+00017c50: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00017c60: 6620 6665 6174 7572 655f 7374 6f72 655f  f feature_store_
+00017c70: 6e61 6d65 2873 656c 6629 3a0a 2020 2020  name(self):.    
+00017c80: 2020 2020 2222 224e 616d 6520 6f66 2074      """Name of t
+00017c90: 6865 2066 6561 7475 7265 2073 746f 7265  he feature store
+00017ca0: 2069 6e20 7768 6963 6820 7468 6520 6665   in which the fe
+00017cb0: 6174 7572 6520 6772 6f75 7020 6973 206c  ature group is l
+00017cc0: 6f63 6174 6564 2e22 2222 0a20 2020 2020  ocated.""".     
+00017cd0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00017ce0: 6665 6174 7572 655f 7374 6f72 655f 6e61  feature_store_na
+00017cf0: 6d65 0a0a 2020 2020 4070 726f 7065 7274  me..    @propert
+00017d00: 790a 2020 2020 6465 6620 6372 6561 746f  y.    def creato
+00017d10: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+00017d20: 2022 2222 5573 6572 6e61 6d65 206f 6620   """Username of 
+00017d30: 7468 6520 6372 6561 746f 722e 2222 220a  the creator.""".
+00017d40: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00017d50: 656c 662e 5f63 7265 6174 6f72 0a0a 2020  elf._creator..  
+00017d60: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00017d70: 6465 6620 6372 6561 7465 6428 7365 6c66  def created(self
+00017d80: 293a 0a20 2020 2020 2020 2022 2222 5469  ):.        """Ti
+00017d90: 6d65 7374 616d 7020 7768 656e 2074 6865  mestamp when the
+00017da0: 2066 6561 7475 7265 2067 726f 7570 2077   feature group w
+00017db0: 6173 2063 7265 6174 6564 2e22 2222 0a20  as created.""". 
+00017dc0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00017dd0: 6c66 2e5f 6372 6561 7465 640a 0a20 2020  lf._created..   
+00017de0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00017df0: 6566 2073 7472 6561 6d28 7365 6c66 293a  ef stream(self):
+00017e00: 0a20 2020 2020 2020 2022 2222 5768 6574  .        """Whet
+00017e10: 6865 7220 746f 2065 6e61 626c 6520 7265  her to enable re
+00017e20: 616c 2074 696d 6520 7374 7265 616d 2077  al time stream w
+00017e30: 7269 7469 6e67 2063 6170 6162 696c 6974  riting capabilit
+00017e40: 6965 732e 2222 220a 2020 2020 2020 2020  ies.""".        
+00017e50: 7265 7475 726e 2073 656c 662e 5f73 7472  return self._str
+00017e60: 6561 6d0a 0a20 2020 2040 7072 6f70 6572  eam..    @proper
+00017e70: 7479 0a20 2020 2064 6566 2070 6172 656e  ty.    def paren
+00017e80: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
+00017e90: 2020 2222 2250 6172 656e 7420 6665 6174    """Parent feat
+00017ea0: 7572 6520 6772 6f75 7073 2061 7320 6f72  ure groups as or
+00017eb0: 6967 696e 206f 6620 7468 6520 6461 7461  igin of the data
+00017ec0: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
+00017ed0: 6665 6174 7572 6520 6772 6f75 702e 0a20  feature group.. 
+00017ee0: 2020 2020 2020 2054 6869 7320 6973 2070         This is p
+00017ef0: 6172 7420 6f66 2065 7870 6c69 6369 7420  art of explicit 
+00017f00: 7072 6f76 656e 616e 6365 2222 220a 2020  provenance""".  
+00017f10: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00017f20: 662e 5f70 6172 656e 7473 0a0a 2020 2020  f._parents..    
+00017f30: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00017f40: 6620 6261 636b 6669 6c6c 5f6a 6f62 2873  f backfill_job(s
+00017f50: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00017f60: 2247 6574 2074 6865 204a 6f62 206f 626a  "Get the Job obj
+00017f70: 6563 7420 7265 6665 7265 6e63 6520 666f  ect reference fo
+00017f80: 7220 7468 6520 6261 636b 6669 6c6c 206a  r the backfill j
+00017f90: 6f62 2066 6f72 2074 6869 730a 2020 2020  ob for this.    
+00017fa0: 2020 2020 4665 6174 7572 6520 4772 6f75      Feature Grou
+00017fb0: 702e 2222 220a 2020 2020 2020 2020 6966  p.""".        if
+00017fc0: 2073 656c 662e 5f62 6163 6b66 696c 6c5f   self._backfill_
+00017fd0: 6a6f 6220 6973 204e 6f6e 653a 0a20 2020  job is None:.   
+00017fe0: 2020 2020 2020 2020 206a 6f62 5f6e 616d           job_nam
+00017ff0: 6520 3d20 227b 6667 5f6e 616d 657d 5f7b  e = "{fg_name}_{
+00018000: 7665 7273 696f 6e7d 5f6f 6666 6c69 6e65  version}_offline
+00018010: 5f66 675f 6261 636b 6669 6c6c 222e 666f  _fg_backfill".fo
+00018020: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+00018030: 2020 2020 2020 6667 5f6e 616d 653d 7365        fg_name=se
+00018040: 6c66 2e5f 6e61 6d65 2c20 7665 7273 696f  lf._name, versio
+00018050: 6e3d 7365 6c66 2e5f 7665 7273 696f 6e0a  n=self._version.
+00018060: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00018070: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00018080: 6261 636b 6669 6c6c 5f6a 6f62 203d 206a  backfill_job = j
+00018090: 6f62 5f61 7069 2e4a 6f62 4170 6928 292e  ob_api.JobApi().
+000180a0: 6765 7428 6a6f 625f 6e61 6d65 290a 2020  get(job_name).  
+000180b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000180c0: 662e 5f62 6163 6b66 696c 6c5f 6a6f 620a  f._backfill_job.
+000180d0: 0a20 2020 2040 7665 7273 696f 6e2e 7365  .    @version.se
+000180e0: 7474 6572 0a20 2020 2064 6566 2076 6572  tter.    def ver
+000180f0: 7369 6f6e 2873 656c 662c 2076 6572 7369  sion(self, versi
+00018100: 6f6e 293a 0a20 2020 2020 2020 2073 656c  on):.        sel
+00018110: 662e 5f76 6572 7369 6f6e 203d 2076 6572  f._version = ver
+00018120: 7369 6f6e 0a0a 2020 2020 4064 6573 6372  sion..    @descr
+00018130: 6970 7469 6f6e 2e73 6574 7465 720a 2020  iption.setter.  
+00018140: 2020 6465 6620 6465 7363 7269 7074 696f    def descriptio
+00018150: 6e28 7365 6c66 2c20 6e65 775f 6465 7363  n(self, new_desc
+00018160: 7269 7074 696f 6e29 3a0a 2020 2020 2020  ription):.      
+00018170: 2020 7365 6c66 2e5f 6465 7363 7269 7074    self._descript
+00018180: 696f 6e20 3d20 6e65 775f 6465 7363 7269  ion = new_descri
+00018190: 7074 696f 6e0a 0a20 2020 2040 6665 6174  ption..    @feat
+000181a0: 7572 6573 2e73 6574 7465 720a 2020 2020  ures.setter.    
+000181b0: 6465 6620 6665 6174 7572 6573 2873 656c  def features(sel
+000181c0: 662c 206e 6577 5f66 6561 7475 7265 7329  f, new_features)
+000181d0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+000181e0: 6665 6174 7572 6573 203d 206e 6577 5f66  features = new_f
+000181f0: 6561 7475 7265 730a 0a20 2020 2040 7469  eatures..    @ti
+00018200: 6d65 5f74 7261 7665 6c5f 666f 726d 6174  me_travel_format
+00018210: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
+00018220: 7469 6d65 5f74 7261 7665 6c5f 666f 726d  time_travel_form
+00018230: 6174 2873 656c 662c 206e 6577 5f74 696d  at(self, new_tim
+00018240: 655f 7472 6176 656c 5f66 6f72 6d61 7429  e_travel_format)
+00018250: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00018260: 7469 6d65 5f74 7261 7665 6c5f 666f 726d  time_travel_form
+00018270: 6174 203d 206e 6577 5f74 696d 655f 7472  at = new_time_tr
+00018280: 6176 656c 5f66 6f72 6d61 740a 0a20 2020  avel_format..   
+00018290: 2040 7061 7274 6974 696f 6e5f 6b65 792e   @partition_key.
+000182a0: 7365 7474 6572 0a20 2020 2064 6566 2070  setter.    def p
+000182b0: 6172 7469 7469 6f6e 5f6b 6579 2873 656c  artition_key(sel
+000182c0: 662c 206e 6577 5f70 6172 7469 7469 6f6e  f, new_partition
+000182d0: 5f6b 6579 293a 0a20 2020 2020 2020 2073  _key):.        s
+000182e0: 656c 662e 5f70 6172 7469 7469 6f6e 5f6b  elf._partition_k
+000182f0: 6579 203d 205b 706b 2e6c 6f77 6572 2829  ey = [pk.lower()
+00018300: 2066 6f72 2070 6b20 696e 206e 6577 5f70   for pk in new_p
+00018310: 6172 7469 7469 6f6e 5f6b 6579 5d0a 0a20  artition_key].. 
+00018320: 2020 2040 6875 6469 5f70 7265 636f 6d62     @hudi_precomb
+00018330: 696e 655f 6b65 792e 7365 7474 6572 0a20  ine_key.setter. 
+00018340: 2020 2064 6566 2068 7564 695f 7072 6563     def hudi_prec
+00018350: 6f6d 6269 6e65 5f6b 6579 2873 656c 662c  ombine_key(self,
+00018360: 2068 7564 695f 7072 6563 6f6d 6269 6e65   hudi_precombine
+00018370: 5f6b 6579 293a 0a20 2020 2020 2020 2073  _key):.        s
+00018380: 656c 662e 5f68 7564 695f 7072 6563 6f6d  elf._hudi_precom
+00018390: 6269 6e65 5f6b 6579 203d 2068 7564 695f  bine_key = hudi_
+000183a0: 7072 6563 6f6d 6269 6e65 5f6b 6579 2e6c  precombine_key.l
+000183b0: 6f77 6572 2829 0a0a 2020 2020 4073 7472  ower()..    @str
+000183c0: 6561 6d2e 7365 7474 6572 0a20 2020 2064  eam.setter.    d
+000183d0: 6566 2073 7472 6561 6d28 7365 6c66 2c20  ef stream(self, 
+000183e0: 7374 7265 616d 293a 0a20 2020 2020 2020  stream):.       
+000183f0: 2073 656c 662e 5f73 7472 6561 6d20 3d20   self._stream = 
+00018400: 7374 7265 616d 0a0a 2020 2020 4070 6172  stream..    @par
+00018410: 656e 7473 2e73 6574 7465 720a 2020 2020  ents.setter.    
+00018420: 6465 6620 7061 7265 6e74 7328 7365 6c66  def parents(self
+00018430: 2c20 6e65 775f 7061 7265 6e74 7329 3a0a  , new_parents):.
+00018440: 2020 2020 2020 2020 7365 6c66 2e5f 7061          self._pa
+00018450: 7265 6e74 7320 3d20 6e65 775f 7061 7265  rents = new_pare
+00018460: 6e74 730a 0a0a 636c 6173 7320 4578 7465  nts...class Exte
+00018470: 726e 616c 4665 6174 7572 6547 726f 7570  rnalFeatureGroup
+00018480: 2846 6561 7475 7265 4772 6f75 7042 6173  (FeatureGroupBas
+00018490: 6529 3a0a 2020 2020 4558 5445 524e 414c  e):.    EXTERNAL
+000184a0: 5f46 4541 5455 5245 5f47 524f 5550 203d  _FEATURE_GROUP =
+000184b0: 2022 4f4e 5f44 454d 414e 445f 4645 4154   "ON_DEMAND_FEAT
+000184c0: 5552 455f 4752 4f55 5022 0a20 2020 2045  URE_GROUP".    E
+000184d0: 4e54 4954 595f 5459 5045 203d 2022 6665  NTITY_TYPE = "fe
+000184e0: 6174 7572 6567 726f 7570 7322 0a0a 2020  aturegroups"..  
+000184f0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00018500: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00018510: 2020 2020 2020 7374 6f72 6167 655f 636f        storage_co
+00018520: 6e6e 6563 746f 722c 0a20 2020 2020 2020  nnector,.       
+00018530: 2071 7565 7279 3d4e 6f6e 652c 0a20 2020   query=None,.   
+00018540: 2020 2020 2064 6174 615f 666f 726d 6174       data_format
+00018550: 3d4e 6f6e 652c 0a20 2020 2020 2020 2070  =None,.        p
+00018560: 6174 683d 4e6f 6e65 2c0a 2020 2020 2020  ath=None,.      
+00018570: 2020 6f70 7469 6f6e 733d 7b7d 2c0a 2020    options={},.  
+00018580: 2020 2020 2020 6e61 6d65 3d4e 6f6e 652c        name=None,
+00018590: 0a20 2020 2020 2020 2076 6572 7369 6f6e  .        version
+000185a0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2064  =None,.        d
+000185b0: 6573 6372 6970 7469 6f6e 3d4e 6f6e 652c  escription=None,
+000185c0: 0a20 2020 2020 2020 2070 7269 6d61 7279  .        primary
+000185d0: 5f6b 6579 3d4e 6f6e 652c 0a20 2020 2020  _key=None,.     
+000185e0: 2020 2066 6561 7475 7265 7374 6f72 655f     featurestore_
+000185f0: 6964 3d4e 6f6e 652c 0a20 2020 2020 2020  id=None,.       
+00018600: 2066 6561 7475 7265 7374 6f72 655f 6e61   featurestore_na
+00018610: 6d65 3d4e 6f6e 652c 0a20 2020 2020 2020  me=None,.       
+00018620: 2063 7265 6174 6564 3d4e 6f6e 652c 0a20   created=None,. 
+00018630: 2020 2020 2020 2063 7265 6174 6f72 3d4e         creator=N
+00018640: 6f6e 652c 0a20 2020 2020 2020 2069 643d  one,.        id=
+00018650: 4e6f 6e65 2c0a 2020 2020 2020 2020 6665  None,.        fe
+00018660: 6174 7572 6573 3d4e 6f6e 652c 0a20 2020  atures=None,.   
+00018670: 2020 2020 206c 6f63 6174 696f 6e3d 4e6f       location=No
+00018680: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+00018690: 6973 7469 6373 5f63 6f6e 6669 673d 4e6f  istics_config=No
+000186a0: 6e65 2c0a 2020 2020 2020 2020 6576 656e  ne,.        even
+000186b0: 745f 7469 6d65 3d4e 6f6e 652c 0a20 2020  t_time=None,.   
+000186c0: 2020 2020 2065 7870 6563 7461 7469 6f6e       expectation
+000186d0: 5f73 7569 7465 3d4e 6f6e 652c 0a20 2020  _suite=None,.   
+000186e0: 2020 2020 206f 6e6c 696e 655f 656e 6162       online_enab
+000186f0: 6c65 643d 4661 6c73 652c 0a20 2020 2020  led=False,.     
+00018700: 2020 2068 7265 663d 4e6f 6e65 2c0a 2020     href=None,.  
+00018710: 2020 2020 2020 6f6e 6c69 6e65 5f74 6f70        online_top
+00018720: 6963 5f6e 616d 653d 4e6f 6e65 2c0a 2020  ic_name=None,.  
+00018730: 2020 293a 0a20 2020 2020 2020 2073 7570    ):.        sup
+00018740: 6572 2829 2e5f 5f69 6e69 745f 5f28 0a20  er().__init__(. 
+00018750: 2020 2020 2020 2020 2020 2066 6561 7475             featu
+00018760: 7265 7374 6f72 655f 6964 2c0a 2020 2020  restore_id,.    
+00018770: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
+00018780: 2c0a 2020 2020 2020 2020 2020 2020 6576  ,.            ev
+00018790: 656e 745f 7469 6d65 3d65 7665 6e74 5f74  ent_time=event_t
+000187a0: 696d 652c 0a20 2020 2020 2020 2020 2020  ime,.           
+000187b0: 206f 6e6c 696e 655f 656e 6162 6c65 643d   online_enabled=
+000187c0: 6f6e 6c69 6e65 5f65 6e61 626c 6564 2c0a  online_enabled,.
+000187d0: 2020 2020 2020 2020 2020 2020 6964 3d69              id=i
+000187e0: 642c 0a20 2020 2020 2020 2020 2020 2065  d,.            e
+000187f0: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
+00018800: 3d65 7870 6563 7461 7469 6f6e 5f73 7569  =expectation_sui
+00018810: 7465 2c0a 2020 2020 2020 2020 2020 2020  te,.            
+00018820: 6f6e 6c69 6e65 5f74 6f70 6963 5f6e 616d  online_topic_nam
+00018830: 653d 6f6e 6c69 6e65 5f74 6f70 6963 5f6e  e=online_topic_n
+00018840: 616d 652c 0a20 2020 2020 2020 2029 0a0a  ame,.        )..
+00018850: 2020 2020 2020 2020 7365 6c66 2e5f 6665          self._fe
+00018860: 6174 7572 655f 7374 6f72 655f 6e61 6d65  ature_store_name
+00018870: 203d 2066 6561 7475 7265 7374 6f72 655f   = featurestore_
+00018880: 6e61 6d65 0a20 2020 2020 2020 2073 656c  name.        sel
+00018890: 662e 5f64 6573 6372 6970 7469 6f6e 203d  f._description =
+000188a0: 2064 6573 6372 6970 7469 6f6e 0a20 2020   description.   
+000188b0: 2020 2020 2073 656c 662e 5f63 7265 6174       self._creat
+000188c0: 6564 203d 2063 7265 6174 6564 0a20 2020  ed = created.   
+000188d0: 2020 2020 2073 656c 662e 5f63 7265 6174       self._creat
+000188e0: 6f72 203d 2075 7365 722e 5573 6572 2e66  or = user.User.f
+000188f0: 726f 6d5f 7265 7370 6f6e 7365 5f6a 736f  rom_response_jso
+00018900: 6e28 6372 6561 746f 7229 0a20 2020 2020  n(creator).     
+00018910: 2020 2073 656c 662e 5f76 6572 7369 6f6e     self._version
+00018920: 203d 2076 6572 7369 6f6e 0a20 2020 2020   = version.     
+00018930: 2020 2073 656c 662e 5f6e 616d 6520 3d20     self._name = 
+00018940: 6e61 6d65 0a20 2020 2020 2020 2073 656c  name.        sel
+00018950: 662e 5f71 7565 7279 203d 2071 7565 7279  f._query = query
+00018960: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
+00018970: 6174 615f 666f 726d 6174 203d 2064 6174  ata_format = dat
+00018980: 615f 666f 726d 6174 2e75 7070 6572 2829  a_format.upper()
+00018990: 2069 6620 6461 7461 5f66 6f72 6d61 7420   if data_format 
+000189a0: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
+000189b0: 2020 7365 6c66 2e5f 7061 7468 203d 2070    self._path = p
+000189c0: 6174 680a 0a20 2020 2020 2020 2073 656c  ath..        sel
+000189d0: 662e 5f66 6561 7475 7265 7320 3d20 5b0a  f._features = [.
+000189e0: 2020 2020 2020 2020 2020 2020 6665 6174              feat
+000189f0: 7572 652e 4665 6174 7572 652e 6672 6f6d  ure.Feature.from
+00018a00: 5f72 6573 706f 6e73 655f 6a73 6f6e 2866  _response_json(f
+00018a10: 6561 7429 2069 6620 6973 696e 7374 616e  eat) if isinstan
+00018a20: 6365 2866 6561 742c 2064 6963 7429 2065  ce(feat, dict) e
+00018a30: 6c73 6520 6665 6174 0a20 2020 2020 2020  lse feat.       
+00018a40: 2020 2020 2066 6f72 2066 6561 7420 696e       for feat in
+00018a50: 2028 6665 6174 7572 6573 206f 7220 5b5d   (features or []
+00018a60: 290a 2020 2020 2020 2020 5d0a 0a20 2020  ).        ]..   
+00018a70: 2020 2020 2073 656c 662e 5f66 6561 7475       self._featu
+00018a80: 7265 5f67 726f 7570 5f65 6e67 696e 6520  re_group_engine 
+00018a90: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00018aa0: 6578 7465 726e 616c 5f66 6561 7475 7265  external_feature
+00018ab0: 5f67 726f 7570 5f65 6e67 696e 652e 4578  _group_engine.Ex
+00018ac0: 7465 726e 616c 4665 6174 7572 6547 726f  ternalFeatureGro
+00018ad0: 7570 456e 6769 6e65 2866 6561 7475 7265  upEngine(feature
+00018ae0: 7374 6f72 655f 6964 290a 2020 2020 2020  store_id).      
+00018af0: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
+00018b00: 7365 6c66 2e5f 6964 3a0a 2020 2020 2020  self._id:.      
+00018b10: 2020 2020 2020 2320 476f 7420 6672 6f6d        # Got from
+00018b20: 2048 6f70 7377 6f72 6b73 2c20 6465 7365   Hopsworks, dese
+00018b30: 7269 616c 697a 6520 6665 6174 7572 6573  rialize features
+00018b40: 2061 6e64 2073 746f 7261 6765 2063 6f6e   and storage con
+00018b50: 6e65 6374 6f72 0a20 2020 2020 2020 2020  nector.         
+00018b60: 2020 2073 656c 662e 5f66 6561 7475 7265     self._feature
+00018b70: 7320 3d20 280a 2020 2020 2020 2020 2020  s = (.          
+00018b80: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00018b90: 2020 2020 2020 2020 2020 2020 6665 6174              feat
+00018ba0: 7572 652e 4665 6174 7572 652e 6672 6f6d  ure.Feature.from
+00018bb0: 5f72 6573 706f 6e73 655f 6a73 6f6e 2866  _response_json(f
+00018bc0: 6561 7429 0a20 2020 2020 2020 2020 2020  eat).           
+00018bd0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+00018be0: 7374 616e 6365 2866 6561 742c 2064 6963  stance(feat, dic
+00018bf0: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+00018c00: 2020 2020 2020 2065 6c73 6520 6665 6174         else feat
+00018c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018c20: 2020 2020 2066 6f72 2066 6561 7420 696e       for feat in
+00018c30: 2066 6561 7475 7265 730a 2020 2020 2020   features.      
+00018c40: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00018c50: 2020 2020 2020 2020 2020 2020 6966 2066              if f
+00018c60: 6561 7475 7265 730a 2020 2020 2020 2020  eatures.        
+00018c70: 2020 2020 2020 2020 656c 7365 204e 6f6e          else Non
+00018c80: 650a 2020 2020 2020 2020 2020 2020 290a  e.            ).
+00018c90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018ca0: 2e70 7269 6d61 7279 5f6b 6579 203d 2028  .primary_key = (
+00018cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018cc0: 205b 6665 6174 2e6e 616d 6520 666f 7220   [feat.name for 
+00018cd0: 6665 6174 2069 6e20 7365 6c66 2e5f 6665  feat in self._fe
+00018ce0: 6174 7572 6573 2069 6620 6665 6174 2e70  atures if feat.p
+00018cf0: 7269 6d61 7279 2069 7320 5472 7565 5d0a  rimary is True].
+00018d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d10: 6966 2073 656c 662e 5f66 6561 7475 7265  if self._feature
+00018d20: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00018d30: 2020 656c 7365 205b 5d0a 2020 2020 2020    else [].      
+00018d40: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00018d50: 2020 2020 7365 6c66 2e73 7461 7469 7374      self.statist
+00018d60: 6963 735f 636f 6e66 6967 203d 2073 7461  ics_config = sta
+00018d70: 7469 7374 6963 735f 636f 6e66 6967 0a0a  tistics_config..
+00018d80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018d90: 2e5f 6f70 7469 6f6e 7320 3d20 280a 2020  ._options = (.  
+00018da0: 2020 2020 2020 2020 2020 2020 2020 7b6f                {o
+00018db0: 7074 696f 6e5b 226e 616d 6522 5d3a 206f  ption["name"]: o
+00018dc0: 7074 696f 6e5b 2276 616c 7565 225d 2066  ption["value"] f
+00018dd0: 6f72 206f 7074 696f 6e20 696e 206f 7074  or option in opt
+00018de0: 696f 6e73 7d0a 2020 2020 2020 2020 2020  ions}.          
+00018df0: 2020 2020 2020 6966 206f 7074 696f 6e73        if options
+00018e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018e10: 2065 6c73 6520 4e6f 6e65 0a20 2020 2020   else None.     
+00018e20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00018e30: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00018e40: 2020 2073 656c 662e 7072 696d 6172 795f     self.primary_
+00018e50: 6b65 7920 3d20 7072 696d 6172 795f 6b65  key = primary_ke
+00018e60: 790a 2020 2020 2020 2020 2020 2020 7365  y.            se
+00018e70: 6c66 2e73 7461 7469 7374 6963 735f 636f  lf.statistics_co
+00018e80: 6e66 6967 203d 2073 7461 7469 7374 6963  nfig = statistic
+00018e90: 735f 636f 6e66 6967 0a20 2020 2020 2020  s_config.       
+00018ea0: 2020 2020 2073 656c 662e 5f66 6561 7475       self._featu
+00018eb0: 7265 7320 3d20 6665 6174 7572 6573 0a20  res = features. 
+00018ec0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018ed0: 5f6f 7074 696f 6e73 203d 206f 7074 696f  _options = optio
+00018ee0: 6e73 0a0a 2020 2020 2020 2020 6966 2073  ns..        if s
+00018ef0: 746f 7261 6765 5f63 6f6e 6e65 6374 6f72  torage_connector
+00018f00: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+00018f10: 2069 7369 6e73 7461 6e63 6528 7374 6f72   isinstance(stor
+00018f20: 6167 655f 636f 6e6e 6563 746f 722c 2064  age_connector, d
+00018f30: 6963 7429 3a0a 2020 2020 2020 2020 2020  ict):.          
+00018f40: 2020 7365 6c66 2e5f 7374 6f72 6167 655f    self._storage_
+00018f50: 636f 6e6e 6563 746f 7220 3d20 7363 2e53  connector = sc.S
+00018f60: 746f 7261 6765 436f 6e6e 6563 746f 722e  torageConnector.
+00018f70: 6672 6f6d 5f72 6573 706f 6e73 655f 6a73  from_response_js
+00018f80: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00018f90: 2020 2020 7374 6f72 6167 655f 636f 6e6e      storage_conn
+00018fa0: 6563 746f 720a 2020 2020 2020 2020 2020  ector.          
+00018fb0: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
+00018fc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00018fd0: 6c66 2e5f 7374 6f72 6167 655f 636f 6e6e  lf._storage_conn
+00018fe0: 6563 746f 7220 3d20 7374 6f72 6167 655f  ector = storage_
+00018ff0: 636f 6e6e 6563 746f 720a 0a20 2020 2020  connector..     
+00019000: 2020 2073 656c 662e 5f68 7265 6620 3d20     self._href = 
+00019010: 6872 6566 0a0a 2020 2020 6465 6620 7361  href..    def sa
+00019020: 7665 2873 656c 6629 3a0a 2020 2020 2020  ve(self):.      
+00019030: 2020 2222 2250 6572 7369 7374 2074 6865    """Persist the
+00019040: 206d 6574 6164 6174 6120 666f 7220 7468   metadata for th
+00019050: 6973 2065 7874 6572 6e61 6c20 6665 6174  is external feat
+00019060: 7572 6520 6772 6f75 702e 0a0a 2020 2020  ure group...    
+00019070: 2020 2020 5769 7468 6f75 7420 6361 6c6c      Without call
+00019080: 696e 6720 7468 6973 206d 6574 686f 642c  ing this method,
+00019090: 2079 6f75 7220 6665 6174 7572 6520 6772   your feature gr
+000190a0: 6f75 7020 7769 6c6c 206f 6e6c 7920 6578  oup will only ex
+000190b0: 6973 740a 2020 2020 2020 2020 696e 2079  ist.        in y
+000190c0: 6f75 7220 5079 7468 6f6e 204b 6572 6e65  our Python Kerne
+000190d0: 6c2c 2062 7574 206e 6f74 2069 6e20 486f  l, but not in Ho
+000190e0: 7073 776f 726b 732e 0a0a 2020 2020 2020  psworks...      
+000190f0: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
+00019100: 2020 2020 7175 6572 7920 3d20 2253 454c      query = "SEL
+00019110: 4543 5420 2a20 4652 4f4d 2073 616c 6573  ECT * FROM sales
+00019120: 220a 0a20 2020 2020 2020 2066 6720 3d20  "..        fg = 
+00019130: 6665 6174 7572 655f 7374 6f72 652e 6372  feature_store.cr
+00019140: 6561 7465 5f65 7874 6572 6e61 6c5f 6665  eate_external_fe
+00019150: 6174 7572 655f 6772 6f75 7028 6e61 6d65  ature_group(name
+00019160: 3d22 7361 6c65 7322 2c0a 2020 2020 2020  ="sales",.      
+00019170: 2020 2020 2020 7665 7273 696f 6e3d 312c        version=1,
+00019180: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+00019190: 6372 6970 7469 6f6e 3d22 5068 7973 6963  cription="Physic
+000191a0: 616c 2073 686f 7020 7361 6c65 7320 6665  al shop sales fe
+000191b0: 6174 7572 6573 222c 0a20 2020 2020 2020  atures",.       
+000191c0: 2020 2020 2071 7565 7279 3d71 7565 7279       query=query
+000191d0: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
+000191e0: 6f72 6167 655f 636f 6e6e 6563 746f 723d  orage_connector=
+000191f0: 636f 6e6e 6563 746f 722c 0a20 2020 2020  connector,.     
+00019200: 2020 2020 2020 2070 7269 6d61 7279 5f6b         primary_k
+00019210: 6579 3d5b 2773 735f 7374 6f72 655f 736b  ey=['ss_store_sk
+00019220: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
+00019230: 6576 656e 745f 7469 6d65 3d27 7361 6c65  event_time='sale
+00019240: 5f64 6174 6527 0a20 2020 2020 2020 2029  _date'.        )
+00019250: 0a0a 2020 2020 2020 2020 6667 2e73 6176  ..        fg.sav
+00019260: 6528 290a 2020 2020 2020 2020 2222 220a  e().        """.
+00019270: 2020 2020 2020 2020 7365 6c66 2e5f 6665          self._fe
+00019280: 6174 7572 655f 6772 6f75 705f 656e 6769  ature_group_engi
+00019290: 6e65 2e73 6176 6528 7365 6c66 290a 2020  ne.save(self).  
+000192a0: 2020 2020 2020 7365 6c66 2e5f 636f 6465        self._code
+000192b0: 5f65 6e67 696e 652e 7361 7665 5f63 6f64  _engine.save_cod
+000192c0: 6528 7365 6c66 290a 0a20 2020 2020 2020  e(self)..       
+000192d0: 2069 6620 7365 6c66 2e73 7461 7469 7374   if self.statist
+000192e0: 6963 735f 636f 6e66 6967 2e65 6e61 626c  ics_config.enabl
+000192f0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+00019300: 7365 6c66 2e5f 7374 6174 6973 7469 6373  self._statistics
+00019310: 5f65 6e67 696e 652e 636f 6d70 7574 655f  _engine.compute_
+00019320: 7374 6174 6973 7469 6373 2873 656c 6629  statistics(self)
+00019330: 0a0a 2020 2020 6465 6620 696e 7365 7274  ..    def insert
+00019340: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00019350: 2020 2020 2020 2020 6665 6174 7572 6573          features
+00019360: 3a20 556e 696f 6e5b 0a20 2020 2020 2020  : Union[.       
+00019370: 2020 2020 2070 642e 4461 7461 4672 616d       pd.DataFram
+00019380: 652c 0a20 2020 2020 2020 2020 2020 2054  e,.            T
+00019390: 7970 6556 6172 2822 7079 7370 6172 6b2e  ypeVar("pyspark.
+000193a0: 7371 6c2e 4461 7461 4672 616d 6522 292c  sql.DataFrame"),
+000193b0: 2020 2320 6e6f 7161 3a20 4638 3231 0a20    # noqa: F821. 
+000193c0: 2020 2020 2020 2020 2020 2054 7970 6556             TypeV
+000193d0: 6172 2822 7079 7370 6172 6b2e 5244 4422  ar("pyspark.RDD"
+000193e0: 292c 2020 2320 6e6f 7161 3a20 4638 3231  ),  # noqa: F821
+000193f0: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
+00019400: 6e64 6172 7261 792c 0a20 2020 2020 2020  ndarray,.       
+00019410: 2020 2020 204c 6973 745b 6c69 7374 5d2c       List[list],
+00019420: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
+00019430: 2020 2020 7772 6974 655f 6f70 7469 6f6e      write_option
+00019440: 733a 204f 7074 696f 6e61 6c5b 4469 6374  s: Optional[Dict
+00019450: 5b73 7472 2c20 416e 795d 5d20 3d20 7b7d  [str, Any]] = {}
+00019460: 2c0a 2020 2020 2020 2020 7661 6c69 6461  ,.        valida
+00019470: 7469 6f6e 5f6f 7074 696f 6e73 3a20 4f70  tion_options: Op
+00019480: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
+00019490: 2041 6e79 5d5d 203d 207b 7d2c 0a20 2020   Any]] = {},.   
+000194a0: 2020 2020 2073 6176 655f 636f 6465 3a20       save_code: 
+000194b0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+000194c0: 2054 7275 652c 0a20 2020 2029 202d 3e20   True,.    ) -> 
+000194d0: 5475 706c 655b 4f70 7469 6f6e 616c 5b4a  Tuple[Optional[J
+000194e0: 6f62 5d2c 204f 7074 696f 6e61 6c5b 5661  ob], Optional[Va
+000194f0: 6c69 6461 7469 6f6e 5265 706f 7274 5d5d  lidationReport]]
+00019500: 3a0a 2020 2020 2020 2020 6665 6174 7572  :.        featur
+00019510: 655f 6461 7461 6672 616d 6520 3d20 656e  e_dataframe = en
+00019520: 6769 6e65 2e67 6574 5f69 6e73 7461 6e63  gine.get_instanc
+00019530: 6528 292e 636f 6e76 6572 745f 746f 5f64  e().convert_to_d
+00019540: 6566 6175 6c74 5f64 6174 6166 7261 6d65  efault_dataframe
+00019550: 2866 6561 7475 7265 7329 0a0a 2020 2020  (features)..    
+00019560: 2020 2020 6a6f 622c 2067 655f 7265 706f      job, ge_repo
+00019570: 7274 203d 2073 656c 662e 5f66 6561 7475  rt = self._featu
+00019580: 7265 5f67 726f 7570 5f65 6e67 696e 652e  re_group_engine.
+00019590: 696e 7365 7274 280a 2020 2020 2020 2020  insert(.        
+000195a0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000195b0: 2020 2020 2020 6665 6174 7572 655f 6461        feature_da
+000195c0: 7461 6672 616d 653d 6665 6174 7572 655f  taframe=feature_
+000195d0: 6461 7461 6672 616d 652c 0a20 2020 2020  dataframe,.     
+000195e0: 2020 2020 2020 2077 7269 7465 5f6f 7074         write_opt
+000195f0: 696f 6e73 3d77 7269 7465 5f6f 7074 696f  ions=write_optio
+00019600: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+00019610: 7661 6c69 6461 7469 6f6e 5f6f 7074 696f  validation_optio
+00019620: 6e73 3d7b 2273 6176 655f 7265 706f 7274  ns={"save_report
+00019630: 223a 2054 7275 652c 202a 2a76 616c 6964  ": True, **valid
+00019640: 6174 696f 6e5f 6f70 7469 6f6e 737d 2c0a  ation_options},.
+00019650: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00019660: 2020 2069 6620 7361 7665 5f63 6f64 6520     if save_code 
+00019670: 616e 6420 280a 2020 2020 2020 2020 2020  and (.          
+00019680: 2020 6765 5f72 6570 6f72 7420 6973 204e    ge_report is N
+00019690: 6f6e 6520 6f72 2067 655f 7265 706f 7274  one or ge_report
+000196a0: 2e69 6e67 6573 7469 6f6e 5f72 6573 756c  .ingestion_resul
+000196b0: 7420 3d3d 2022 494e 4745 5354 4544 220a  t == "INGESTED".
+000196c0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+000196d0: 2020 2020 2020 2073 656c 662e 5f63 6f64         self._cod
+000196e0: 655f 656e 6769 6e65 2e73 6176 655f 636f  e_engine.save_co
+000196f0: 6465 2873 656c 6629 0a0a 2020 2020 2020  de(self)..      
+00019700: 2020 6966 2073 656c 662e 7374 6174 6973    if self.statis
+00019710: 7469 6373 5f63 6f6e 6669 672e 656e 6162  tics_config.enab
+00019720: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
+00019730: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
+00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019750: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00019760: 2020 2020 2020 2253 7461 7469 7374 6963        "Statistic
+00019770: 7320 6172 6520 6e6f 7420 636f 6d70 7574  s are not comput
+00019780: 6564 2066 6f72 2069 6e73 6572 7469 6f6e  ed for insertion
+00019790: 2074 6f20 6f6e 6c69 6e65 2065 6e61 626c   to online enabl
+000197a0: 6564 2065 7874 6572 6e61 6c20 6665 6174  ed external feat
+000197b0: 7572 6520 6772 6f75 7020 607b 7d60 2c20  ure group `{}`, 
+000197c0: 7769 7468 2076 6572 7369 6f6e 220a 2020  with version".  
+000197d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197e0: 2020 2220 607b 7d60 2e20 4361 6c6c 2060    " `{}`. Call `
+000197f0: 636f 6d70 7574 655f 7374 6174 6973 7469  compute_statisti
+00019800: 6373 6020 6578 706c 6963 6974 6c79 2074  cs` explicitly t
+00019810: 6f20 636f 6d70 7574 6520 7374 6174 6973  o compute statis
+00019820: 7469 6373 206f 7665 7220 7468 6520 6461  tics over the da
+00019830: 7461 2069 6e20 7468 6520 6578 7465 726e  ta in the extern
+00019840: 616c 2073 746f 7261 6765 2073 7973 7465  al storage syste
+00019850: 6d2e 220a 2020 2020 2020 2020 2020 2020  m.".            
+00019860: 2020 2020 292e 666f 726d 6174 2873 656c      ).format(sel
+00019870: 662e 5f6e 616d 652c 2073 656c 662e 5f76  f._name, self._v
+00019880: 6572 7369 6f6e 292c 0a20 2020 2020 2020  ersion),.       
+00019890: 2020 2020 2020 2020 2075 7469 6c2e 5374           util.St
+000198a0: 6f72 6167 6557 6172 6e69 6e67 2c0a 2020  orageWarning,.  
+000198b0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000198c0: 2020 2020 2072 6574 7572 6e20 280a 2020       return (.  
+000198d0: 2020 2020 2020 2020 2020 6a6f 622c 0a20            job,. 
+000198e0: 2020 2020 2020 2020 2020 2067 655f 7265             ge_re
+000198f0: 706f 7274 2e74 6f5f 6765 5f74 7970 6528  port.to_ge_type(
+00019900: 2920 6966 2067 655f 7265 706f 7274 2069  ) if ge_report i
+00019910: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+00019920: 4e6f 6e65 2c0a 2020 2020 2020 2020 290a  None,.        ).
+00019930: 0a20 2020 2064 6566 2072 6561 6428 0a20  .    def read(. 
+00019940: 2020 2020 2020 2073 656c 662c 2064 6174         self, dat
+00019950: 6166 7261 6d65 5f74 7970 653a 204f 7074  aframe_type: Opt
+00019960: 696f 6e61 6c5b 7374 725d 203d 2022 6465  ional[str] = "de
+00019970: 6661 756c 7422 2c20 6f6e 6c69 6e65 3a20  fault", online: 
+00019980: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+00019990: 2046 616c 7365 0a20 2020 2029 3a0a 2020   False.    ):.  
+000199a0: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
+000199b0: 2066 6561 7475 7265 2067 726f 7570 2061   feature group a
+000199c0: 7320 6120 4461 7461 4672 616d 652e 0a0a  s a DataFrame...
+000199d0: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
+000199e0: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
+000199f0: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
+00019a00: 2020 2020 2020 2320 636f 6e6e 6563 7420        # connect 
+00019a10: 746f 2074 6865 2046 6561 7475 7265 2053  to the Feature S
+00019a20: 746f 7265 0a20 2020 2020 2020 2020 2020  tore.           
+00019a30: 2066 7320 3d20 2e2e 2e0a 0a20 2020 2020   fs = .....     
+00019a40: 2020 2020 2020 2023 2067 6574 2074 6865         # get the
+00019a50: 2046 6561 7475 7265 2047 726f 7570 2069   Feature Group i
+00019a60: 6e73 7461 6e63 650a 2020 2020 2020 2020  nstance.        
+00019a70: 2020 2020 6667 203d 2066 732e 6765 745f      fg = fs.get_
+00019a80: 6f72 5f63 7265 6174 655f 6665 6174 7572  or_create_featur
+00019a90: 655f 6772 6f75 7028 2e2e 2e29 0a0a 2020  e_group(...)..  
+00019aa0: 2020 2020 2020 2020 2020 6466 203d 2066            df = f
+00019ab0: 672e 7265 6164 2829 0a20 2020 2020 2020  g.read().       
+00019ac0: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
+00019ad0: 2020 2121 2120 7761 726e 696e 6720 2245    !!! warning "E
+00019ae0: 6e67 696e 6520 5375 7070 6f72 7422 0a20  ngine Support". 
+00019af0: 2020 2020 2020 2020 2020 202a 2a53 7061             **Spa
+00019b00: 726b 206f 6e6c 792a 2a0a 0a20 2020 2020  rk only**..     
+00019b10: 2020 2020 2020 2052 6561 6469 6e67 2061         Reading a
+00019b20: 6e20 4578 7465 726e 616c 2046 6561 7475  n External Featu
+00019b30: 7265 2047 726f 7570 2064 6972 6563 746c  re Group directl
+00019b40: 7920 696e 746f 2061 2050 616e 6461 7320  y into a Pandas 
+00019b50: 4461 7461 6672 616d 6520 7573 696e 670a  Dataframe using.
+00019b60: 2020 2020 2020 2020 2020 2020 5079 7468              Pyth
+00019b70: 6f6e 2f50 616e 6461 7320 6173 2045 6e67  on/Pandas as Eng
+00019b80: 696e 6520 6973 206e 6f74 2073 7570 706f  ine is not suppo
+00019b90: 7274 6564 2c20 686f 7765 7665 722c 2079  rted, however, y
+00019ba0: 6f75 2063 616e 2075 7365 2074 6865 0a20  ou can use the. 
+00019bb0: 2020 2020 2020 2020 2020 2051 7565 7279             Query
+00019bc0: 2041 5049 2074 6f20 6372 6561 7465 2046   API to create F
+00019bd0: 6561 7475 7265 2056 6965 7773 2f54 7261  eature Views/Tra
+00019be0: 696e 696e 6720 4461 7461 2063 6f6e 7461  ining Data conta
+00019bf0: 696e 696e 6720 4578 7465 726e 616c 0a20  ining External. 
+00019c00: 2020 2020 2020 2020 2020 2046 6561 7475             Featu
+00019c10: 7265 2047 726f 7570 732e 0a0a 2020 2020  re Groups...    
+00019c20: 2020 2020 2320 4172 6775 6d65 6e74 730a      # Arguments.
+00019c30: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00019c40: 6672 616d 655f 7479 7065 3a20 7374 722c  frame_type: str,
+00019c50: 206f 7074 696f 6e61 6c2e 2050 6f73 7369   optional. Possi
+00019c60: 626c 6520 7661 6c75 6573 2061 7265 2060  ble values are `
+00019c70: 2264 6566 6175 6c74 2260 2c20 6022 7370  "default"`, `"sp
+00019c80: 6172 6b22 602c 0a20 2020 2020 2020 2020  ark"`,.         
+00019c90: 2020 2020 2020 2060 2270 616e 6461 7322         `"pandas"
+00019ca0: 602c 2060 226e 756d 7079 2260 206f 7220  `, `"numpy"` or 
+00019cb0: 6022 7079 7468 6f6e 2260 2c20 6465 6661  `"python"`, defa
+00019cc0: 756c 7473 2074 6f20 6022 6465 6661 756c  ults to `"defaul
+00019cd0: 7422 602e 0a20 2020 2020 2020 2020 2020  t"`..           
+00019ce0: 206f 6e6c 696e 653a 2062 6f6f 6c2c 206f   online: bool, o
+00019cf0: 7074 696f 6e61 6c2e 2049 6620 6054 7275  ptional. If `Tru
+00019d00: 6560 2072 6561 6420 6672 6f6d 206f 6e6c  e` read from onl
+00019d10: 696e 6520 6665 6174 7572 6520 7374 6f72  ine feature stor
+00019d20: 652c 2064 6566 6175 6c74 730a 2020 2020  e, defaults.    
+00019d30: 2020 2020 2020 2020 2020 2020 746f 2060              to `
+00019d40: 4661 6c73 6560 2e0a 0a20 2020 2020 2020  False`...       
+00019d50: 2023 2052 6574 7572 6e73 0a20 2020 2020   # Returns.     
+00019d60: 2020 2020 2020 2060 4461 7461 4672 616d         `DataFram
+00019d70: 6560 3a20 5468 6520 7370 6172 6b20 6461  e`: The spark da
+00019d80: 7461 6672 616d 6520 636f 6e74 6169 6e69  taframe containi
+00019d90: 6e67 2074 6865 2066 6561 7475 7265 2064  ng the feature d
+00019da0: 6174 612e 0a20 2020 2020 2020 2020 2020  ata..           
+00019db0: 2060 7079 7370 6172 6b2e 4461 7461 4672   `pyspark.DataFr
+00019dc0: 616d 6560 2e20 4120 5370 6172 6b20 4461  ame`. A Spark Da
+00019dd0: 7461 4672 616d 652e 0a20 2020 2020 2020  taFrame..       
+00019de0: 2020 2020 2060 7061 6e64 6173 2e44 6174       `pandas.Dat
+00019df0: 6146 7261 6d65 602e 2041 2050 616e 6461  aFrame`. A Panda
+00019e00: 7320 4461 7461 4672 616d 652e 0a20 2020  s DataFrame..   
+00019e10: 2020 2020 2020 2020 2060 6e75 6d70 792e           `numpy.
+00019e20: 6e64 6172 7261 7960 2e20 4120 7477 6f2d  ndarray`. A two-
+00019e30: 6469 6d65 6e73 696f 6e61 6c20 4e75 6d70  dimensional Nump
+00019e40: 7920 6172 7261 792e 0a20 2020 2020 2020  y array..       
+00019e50: 2020 2020 2060 6c69 7374 602e 2041 2074       `list`. A t
+00019e60: 776f 2d64 696d 656e 7369 6f6e 616c 2050  wo-dimensional P
+00019e70: 7974 686f 6e20 6c69 7374 2e0a 0a20 2020  ython list...   
+00019e80: 2020 2020 2023 2052 6169 7365 730a 2020       # Raises.  
+00019e90: 2020 2020 2020 2020 2020 6068 7366 732e            `hsfs.
+00019ea0: 636c 6965 6e74 2e65 7863 6570 7469 6f6e  client.exception
+00019eb0: 732e 5265 7374 4150 4945 7272 6f72 602e  s.RestAPIError`.
+00019ec0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00019ed0: 2020 2020 2069 6620 656e 6769 6e65 2e67       if engine.g
+00019ee0: 6574 5f74 7970 6528 2920 3d3d 2022 7079  et_type() == "py
+00019ef0: 7468 6f6e 2220 616e 6420 6e6f 7420 6f6e  thon" and not on
+00019f00: 6c69 6e65 3a0a 2020 2020 2020 2020 2020  line:.          
+00019f10: 2020 7261 6973 6520 4665 6174 7572 6553    raise FeatureS
+00019f20: 746f 7265 4578 6365 7074 696f 6e28 0a20  toreException(. 
+00019f30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00019f40: 5265 6164 696e 6720 616e 2045 7874 6572  Reading an Exter
+00019f50: 6e61 6c20 4665 6174 7572 6520 4772 6f75  nal Feature Grou
+00019f60: 7020 6469 7265 6374 6c79 2069 6e74 6f20  p directly into 
+00019f70: 6120 5061 6e64 6173 2044 6174 6166 7261  a Pandas Datafra
+00019f80: 6d65 2075 7369 6e67 2022 0a20 2020 2020  me using ".     
+00019f90: 2020 2020 2020 2020 2020 202b 2022 5079             + "Py
+00019fa0: 7468 6f6e 2f50 616e 6461 7320 6173 2045  thon/Pandas as E
+00019fb0: 6e67 696e 6520 6672 6f6d 2074 6865 2065  ngine from the e
+00019fc0: 7874 6572 6e61 6c20 7374 6f72 6167 6520  xternal storage 
+00019fd0: 7379 7374 656d 2022 0a20 2020 2020 2020  system ".       
+00019fe0: 2020 2020 2020 2020 202b 2022 6973 206e           + "is n
+00019ff0: 6f74 2073 7570 706f 7274 6564 2c20 686f  ot supported, ho
+0001a000: 7765 7665 722c 2069 6620 7468 6520 6665  wever, if the fe
+0001a010: 6174 7572 6520 6772 6f75 7020 6973 206f  ature group is o
+0001a020: 6e6c 696e 6520 656e 6162 6c65 642c 2079  nline enabled, y
+0001a030: 6f75 2063 616e 2072 6561 6420 220a 2020  ou can read ".  
+0001a040: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001a050: 2266 726f 6d20 6f6e 6c69 6e65 2073 746f  "from online sto
+0001a060: 7261 6765 206f 7220 796f 7520 6361 6e20  rage or you can 
+0001a070: 7573 6520 7468 6520 220a 2020 2020 2020  use the ".      
+0001a080: 2020 2020 2020 2020 2020 2b20 2251 7565            + "Que
+0001a090: 7279 2041 5049 2074 6f20 6372 6561 7465  ry API to create
+0001a0a0: 2046 6561 7475 7265 2056 6965 7773 2f54   Feature Views/T
+0001a0b0: 7261 696e 696e 6720 4461 7461 2063 6f6e  raining Data con
+0001a0c0: 7461 696e 696e 6720 4578 7465 726e 616c  taining External
+0001a0d0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0001a0e0: 2020 202b 2022 4665 6174 7572 6520 4772     + "Feature Gr
+0001a0f0: 6f75 7073 2e22 0a20 2020 2020 2020 2020  oups.".         
+0001a100: 2020 2029 0a20 2020 2020 2020 2065 6e67     ).        eng
+0001a110: 696e 652e 6765 745f 696e 7374 616e 6365  ine.get_instance
+0001a120: 2829 2e73 6574 5f6a 6f62 5f67 726f 7570  ().set_job_group
+0001a130: 280a 2020 2020 2020 2020 2020 2020 2246  (.            "F
+0001a140: 6574 6368 696e 6720 4665 6174 7572 6520  etching Feature 
+0001a150: 6772 6f75 7022 2c0a 2020 2020 2020 2020  group",.        
+0001a160: 2020 2020 2247 6574 7469 6e67 2066 6561      "Getting fea
+0001a170: 7475 7265 2067 726f 7570 3a20 7b7d 2066  ture group: {} f
+0001a180: 726f 6d20 7468 6520 6665 6174 7572 6573  rom the features
+0001a190: 746f 7265 207b 7d22 2e66 6f72 6d61 7428  tore {}".format(
+0001a1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a1b0: 2073 656c 662e 5f6e 616d 652c 2073 656c   self._name, sel
+0001a1c0: 662e 5f66 6561 7475 7265 5f73 746f 7265  f._feature_store
+0001a1d0: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
+0001a1e0: 2020 292c 0a20 2020 2020 2020 2029 0a20    ),.        ). 
+0001a1f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001a200: 6c66 2e73 656c 6563 745f 616c 6c28 292e  lf.select_all().
+0001a210: 7265 6164 2864 6174 6166 7261 6d65 5f74  read(dataframe_t
+0001a220: 7970 653d 6461 7461 6672 616d 655f 7479  ype=dataframe_ty
+0001a230: 7065 2c20 6f6e 6c69 6e65 3d6f 6e6c 696e  pe, online=onlin
+0001a240: 6529 0a0a 2020 2020 6465 6620 7368 6f77  e)..    def show
+0001a250: 2873 656c 662c 206e 293a 0a20 2020 2020  (self, n):.     
+0001a260: 2020 2022 2222 5368 6f77 2074 6865 2066     """Show the f
+0001a270: 6972 7374 206e 2072 6f77 7320 6f66 2074  irst n rows of t
+0001a280: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
+0001a290: 2e0a 0a20 2020 2020 2020 2021 2121 2065  ...        !!! e
+0001a2a0: 7861 6d70 6c65 0a20 2020 2020 2020 2020  xample.         
+0001a2b0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+0001a2c0: 2020 2020 2020 2020 2023 2063 6f6e 6e65           # conne
+0001a2d0: 6374 2074 6f20 7468 6520 4665 6174 7572  ct to the Featur
+0001a2e0: 6520 5374 6f72 650a 2020 2020 2020 2020  e Store.        
+0001a2f0: 2020 2020 6673 203d 202e 2e2e 0a0a 2020      fs = .....  
+0001a300: 2020 2020 2020 2020 2020 2320 6765 7420            # get 
+0001a310: 7468 6520 4665 6174 7572 6520 4772 6f75  the Feature Grou
+0001a320: 7020 696e 7374 616e 6365 0a20 2020 2020  p instance.     
+0001a330: 2020 2020 2020 2066 6720 3d20 6673 2e67         fg = fs.g
+0001a340: 6574 5f6f 725f 6372 6561 7465 5f66 6561  et_or_create_fea
+0001a350: 7475 7265 5f67 726f 7570 282e 2e2e 290a  ture_group(...).
+0001a360: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
+0001a370: 7368 6f77 2835 290a 2020 2020 2020 2020  show(5).        
+0001a380: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
+0001a390: 2222 220a 2020 2020 2020 2020 656e 6769  """.        engi
+0001a3a0: 6e65 2e67 6574 5f69 6e73 7461 6e63 6528  ne.get_instance(
+0001a3b0: 292e 7365 745f 6a6f 625f 6772 6f75 7028  ).set_job_group(
+0001a3c0: 0a20 2020 2020 2020 2020 2020 2022 4665  .            "Fe
+0001a3d0: 7463 6869 6e67 2046 6561 7475 7265 2067  tching Feature g
+0001a3e0: 726f 7570 222c 0a20 2020 2020 2020 2020  roup",.         
+0001a3f0: 2020 2022 4765 7474 696e 6720 6665 6174     "Getting feat
+0001a400: 7572 6520 6772 6f75 703a 207b 7d20 6672  ure group: {} fr
+0001a410: 6f6d 2074 6865 2066 6561 7475 7265 7374  om the featurest
+0001a420: 6f72 6520 7b7d 222e 666f 726d 6174 280a  ore {}".format(.
+0001a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a440: 7365 6c66 2e5f 6e61 6d65 2c20 7365 6c66  self._name, self
+0001a450: 2e5f 6665 6174 7572 655f 7374 6f72 655f  ._feature_store_
+0001a460: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
+0001a470: 2029 2c0a 2020 2020 2020 2020 290a 2020   ),.        ).  
+0001a480: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001a490: 662e 7365 6c65 6374 5f61 6c6c 2829 2e73  f.select_all().s
+0001a4a0: 686f 7728 6e29 0a0a 2020 2020 4063 6c61  how(n)..    @cla
+0001a4b0: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+0001a4c0: 2066 726f 6d5f 7265 7370 6f6e 7365 5f6a   from_response_j
+0001a4d0: 736f 6e28 636c 732c 206a 736f 6e5f 6469  son(cls, json_di
+0001a4e0: 6374 293a 0a20 2020 2020 2020 206a 736f  ct):.        jso
+0001a4f0: 6e5f 6465 6361 6d65 6c69 7a65 6420 3d20  n_decamelized = 
+0001a500: 6875 6d70 732e 6465 6361 6d65 6c69 7a65  humps.decamelize
+0001a510: 286a 736f 6e5f 6469 6374 290a 2020 2020  (json_dict).    
+0001a520: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0001a530: 6528 6a73 6f6e 5f64 6563 616d 656c 697a  e(json_decameliz
+0001a540: 6564 2c20 6469 6374 293a 0a20 2020 2020  ed, dict):.     
+0001a550: 2020 2020 2020 205f 203d 206a 736f 6e5f         _ = json_
+0001a560: 6465 6361 6d65 6c69 7a65 642e 706f 7028  decamelized.pop(
+0001a570: 2274 7970 6522 2c20 4e6f 6e65 290a 2020  "type", None).  
+0001a580: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001a590: 2063 6c73 282a 2a6a 736f 6e5f 6465 6361   cls(**json_deca
+0001a5a0: 6d65 6c69 7a65 6429 0a20 2020 2020 2020  melized).       
+0001a5b0: 2066 6f72 2066 6720 696e 206a 736f 6e5f   for fg in json_
+0001a5c0: 6465 6361 6d65 6c69 7a65 643a 0a20 2020  decamelized:.   
+0001a5d0: 2020 2020 2020 2020 205f 203d 2066 672e           _ = fg.
+0001a5e0: 706f 7028 2274 7970 6522 2c20 4e6f 6e65  pop("type", None
+0001a5f0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0001a600: 205b 636c 7328 2a2a 6667 2920 666f 7220   [cls(**fg) for 
+0001a610: 6667 2069 6e20 6a73 6f6e 5f64 6563 616d  fg in json_decam
+0001a620: 656c 697a 6564 5d0a 0a20 2020 2064 6566  elized]..    def
+0001a630: 2075 7064 6174 655f 6672 6f6d 5f72 6573   update_from_res
+0001a640: 706f 6e73 655f 6a73 6f6e 2873 656c 662c  ponse_json(self,
+0001a650: 206a 736f 6e5f 6469 6374 293a 0a20 2020   json_dict):.   
+0001a660: 2020 2020 206a 736f 6e5f 6465 6361 6d65       json_decame
+0001a670: 6c69 7a65 6420 3d20 6875 6d70 732e 6465  lized = humps.de
+0001a680: 6361 6d65 6c69 7a65 286a 736f 6e5f 6469  camelize(json_di
+0001a690: 6374 290a 2020 2020 2020 2020 6966 2022  ct).        if "
+0001a6a0: 7479 7065 2220 696e 206a 736f 6e5f 6465  type" in json_de
+0001a6b0: 6361 6d65 6c69 7a65 643a 0a20 2020 2020  camelized:.     
+0001a6c0: 2020 2020 2020 205f 203d 206a 736f 6e5f         _ = json_
+0001a6d0: 6465 6361 6d65 6c69 7a65 642e 706f 7028  decamelized.pop(
+0001a6e0: 2274 7970 6522 290a 2020 2020 2020 2020  "type").        
+0001a6f0: 7365 6c66 2e5f 5f69 6e69 745f 5f28 2a2a  self.__init__(**
+0001a700: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
+0001a710: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0001a720: 2073 656c 660a 0a20 2020 2064 6566 206a   self..    def j
+0001a730: 736f 6e28 7365 6c66 293a 0a20 2020 2020  son(self):.     
+0001a740: 2020 2072 6574 7572 6e20 6a73 6f6e 2e64     return json.d
+0001a750: 756d 7073 2873 656c 662c 2063 6c73 3d75  umps(self, cls=u
+0001a760: 7469 6c2e 4665 6174 7572 6553 746f 7265  til.FeatureStore
+0001a770: 456e 636f 6465 7229 0a0a 2020 2020 6465  Encoder)..    de
+0001a780: 6620 746f 5f64 6963 7428 7365 6c66 293a  f to_dict(self):
+0001a790: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001a7a0: 7b0a 2020 2020 2020 2020 2020 2020 2269  {.            "i
+0001a7b0: 6422 3a20 7365 6c66 2e5f 6964 2c0a 2020  d": self._id,.  
+0001a7c0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+0001a7d0: 3a20 7365 6c66 2e5f 6e61 6d65 2c0a 2020  : self._name,.  
+0001a7e0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+0001a7f0: 6970 7469 6f6e 223a 2073 656c 662e 5f64  iption": self._d
+0001a800: 6573 6372 6970 7469 6f6e 2c0a 2020 2020  escription,.    
+0001a810: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
+0001a820: 223a 2073 656c 662e 5f76 6572 7369 6f6e  ": self._version
+0001a830: 2c0a 2020 2020 2020 2020 2020 2020 2266  ,.            "f
+0001a840: 6561 7475 7265 7322 3a20 7365 6c66 2e5f  eatures": self._
+0001a850: 6665 6174 7572 6573 2c0a 2020 2020 2020  features,.      
+0001a860: 2020 2020 2020 2266 6561 7475 7265 7374        "featurest
+0001a870: 6f72 6549 6422 3a20 7365 6c66 2e5f 6665  oreId": self._fe
+0001a880: 6174 7572 655f 7374 6f72 655f 6964 2c0a  ature_store_id,.
+0001a890: 2020 2020 2020 2020 2020 2020 2271 7565              "que
+0001a8a0: 7279 223a 2073 656c 662e 5f71 7565 7279  ry": self._query
+0001a8b0: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
+0001a8c0: 6174 6146 6f72 6d61 7422 3a20 7365 6c66  ataFormat": self
+0001a8d0: 2e5f 6461 7461 5f66 6f72 6d61 742c 0a20  ._data_format,. 
+0001a8e0: 2020 2020 2020 2020 2020 2022 7061 7468             "path
+0001a8f0: 223a 2073 656c 662e 5f70 6174 682c 0a20  ": self._path,. 
+0001a900: 2020 2020 2020 2020 2020 2022 6f70 7469             "opti
+0001a910: 6f6e 7322 3a20 5b7b 226e 616d 6522 3a20  ons": [{"name": 
+0001a920: 6b2c 2022 7661 6c75 6522 3a20 767d 2066  k, "value": v} f
+0001a930: 6f72 206b 2c20 7620 696e 2073 656c 662e  or k, v in self.
+0001a940: 5f6f 7074 696f 6e73 2e69 7465 6d73 2829  _options.items()
+0001a950: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
+0001a960: 2073 656c 662e 5f6f 7074 696f 6e73 0a20   self._options. 
+0001a970: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+0001a980: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0001a990: 2020 2273 746f 7261 6765 436f 6e6e 6563    "storageConnec
+0001a9a0: 746f 7222 3a20 7365 6c66 2e5f 7374 6f72  tor": self._stor
+0001a9b0: 6167 655f 636f 6e6e 6563 746f 722e 746f  age_connector.to
+0001a9c0: 5f64 6963 7428 292c 0a20 2020 2020 2020  _dict(),.       
+0001a9d0: 2020 2020 2022 7479 7065 223a 2022 6f6e       "type": "on
+0001a9e0: 4465 6d61 6e64 4665 6174 7572 6567 726f  DemandFeaturegro
+0001a9f0: 7570 4454 4f22 2c0a 2020 2020 2020 2020  upDTO",.        
+0001aa00: 2020 2020 2273 7461 7469 7374 6963 7343      "statisticsC
+0001aa10: 6f6e 6669 6722 3a20 7365 6c66 2e5f 7374  onfig": self._st
+0001aa20: 6174 6973 7469 6373 5f63 6f6e 6669 672c  atistics_config,
+0001aa30: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
+0001aa40: 656e 7454 696d 6522 3a20 7365 6c66 2e5f  entTime": self._
+0001aa50: 6576 656e 745f 7469 6d65 2c0a 2020 2020  event_time,.    
+0001aa60: 2020 2020 2020 2020 2265 7870 6563 7461          "expecta
+0001aa70: 7469 6f6e 5375 6974 6522 3a20 7365 6c66  tionSuite": self
+0001aa80: 2e5f 6578 7065 6374 6174 696f 6e5f 7375  ._expectation_su
+0001aa90: 6974 652c 0a20 2020 2020 2020 2020 2020  ite,.           
+0001aaa0: 2022 6f6e 6c69 6e65 456e 6162 6c65 6422   "onlineEnabled"
+0001aab0: 3a20 7365 6c66 2e5f 6f6e 6c69 6e65 5f65  : self._online_e
+0001aac0: 6e61 626c 6564 2c0a 2020 2020 2020 2020  nabled,.        
+0001aad0: 7d0a 0a20 2020 2040 7072 6f70 6572 7479  }..    @property
+0001aae0: 0a20 2020 2064 6566 2069 6428 7365 6c66  .    def id(self
+0001aaf0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+0001ab00: 6e20 7365 6c66 2e5f 6964 0a0a 2020 2020  n self._id..    
+0001ab10: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0001ab20: 6620 6e61 6d65 2873 656c 6629 3a0a 2020  f name(self):.  
+0001ab30: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001ab40: 662e 5f6e 616d 650a 0a20 2020 2040 7072  f._name..    @pr
+0001ab50: 6f70 6572 7479 0a20 2020 2064 6566 2076  operty.    def v
+0001ab60: 6572 7369 6f6e 2873 656c 6629 3a0a 2020  ersion(self):.  
+0001ab70: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001ab80: 662e 5f76 6572 7369 6f6e 0a0a 2020 2020  f._version..    
+0001ab90: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0001aba0: 6620 6465 7363 7269 7074 696f 6e28 7365  f description(se
+0001abb0: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+0001abc0: 7572 6e20 7365 6c66 2e5f 6465 7363 7269  urn self._descri
+0001abd0: 7074 696f 6e0a 0a20 2020 2040 7072 6f70  ption..    @prop
+0001abe0: 6572 7479 0a20 2020 2064 6566 2066 6561  erty.    def fea
+0001abf0: 7475 7265 7328 7365 6c66 293a 0a20 2020  tures(self):.   
+0001ac00: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0001ac10: 2e5f 6665 6174 7572 6573 0a0a 2020 2020  ._features..    
+0001ac20: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0001ac30: 6620 7175 6572 7928 7365 6c66 293a 0a20  f query(self):. 
+0001ac40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001ac50: 6c66 2e5f 7175 6572 790a 0a20 2020 2040  lf._query..    @
+0001ac60: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0001ac70: 2064 6174 615f 666f 726d 6174 2873 656c   data_format(sel
+0001ac80: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+0001ac90: 726e 2073 656c 662e 5f64 6174 615f 666f  rn self._data_fo
+0001aca0: 726d 6174 0a0a 2020 2020 4070 726f 7065  rmat..    @prope
+0001acb0: 7274 790a 2020 2020 6465 6620 7061 7468  rty.    def path
+0001acc0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001acd0: 7265 7475 726e 2073 656c 662e 5f70 6174  return self._pat
+0001ace0: 680a 0a20 2020 2040 7072 6f70 6572 7479  h..    @property
+0001acf0: 0a20 2020 2064 6566 206f 7074 696f 6e73  .    def options
+0001ad00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001ad10: 7265 7475 726e 2073 656c 662e 5f6f 7074  return self._opt
+0001ad20: 696f 6e73 0a0a 2020 2020 4070 726f 7065  ions..    @prope
+0001ad30: 7274 790a 2020 2020 6465 6620 7374 6f72  rty.    def stor
+0001ad40: 6167 655f 636f 6e6e 6563 746f 7228 7365  age_connector(se
+0001ad50: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+0001ad60: 7572 6e20 7365 6c66 2e5f 7374 6f72 6167  urn self._storag
+0001ad70: 655f 636f 6e6e 6563 746f 720a 0a20 2020  e_connector..   
+0001ad80: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+0001ad90: 6566 2063 7265 6174 6f72 2873 656c 6629  ef creator(self)
+0001ada0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0001adb0: 2073 656c 662e 5f63 7265 6174 6f72 0a0a   self._creator..
+0001adc0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0001add0: 2020 6465 6620 6372 6561 7465 6428 7365    def created(se
+0001ade0: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+0001adf0: 7572 6e20 7365 6c66 2e5f 6372 6561 7465  urn self._create
+0001ae00: 640a 0a20 2020 2040 7665 7273 696f 6e2e  d..    @version.
+0001ae10: 7365 7474 6572 0a20 2020 2064 6566 2076  setter.    def v
+0001ae20: 6572 7369 6f6e 2873 656c 662c 2076 6572  ersion(self, ver
+0001ae30: 7369 6f6e 293a 0a20 2020 2020 2020 2073  sion):.        s
+0001ae40: 656c 662e 5f76 6572 7369 6f6e 203d 2076  elf._version = v
+0001ae50: 6572 7369 6f6e 0a0a 2020 2020 4064 6573  ersion..    @des
+0001ae60: 6372 6970 7469 6f6e 2e73 6574 7465 720a  cription.setter.
+0001ae70: 2020 2020 6465 6620 6465 7363 7269 7074      def descript
+0001ae80: 696f 6e28 7365 6c66 2c20 6e65 775f 6465  ion(self, new_de
+0001ae90: 7363 7269 7074 696f 6e29 3a0a 2020 2020  scription):.    
+0001aea0: 2020 2020 7365 6c66 2e5f 6465 7363 7269      self._descri
+0001aeb0: 7074 696f 6e20 3d20 6e65 775f 6465 7363  ption = new_desc
+0001aec0: 7269 7074 696f 6e0a 0a20 2020 2040 6665  ription..    @fe
+0001aed0: 6174 7572 6573 2e73 6574 7465 720a 2020  atures.setter.  
+0001aee0: 2020 6465 6620 6665 6174 7572 6573 2873    def features(s
+0001aef0: 656c 662c 206e 6577 5f66 6561 7475 7265  elf, new_feature
+0001af00: 7329 3a0a 2020 2020 2020 2020 7365 6c66  s):.        self
+0001af10: 2e5f 6665 6174 7572 6573 203d 206e 6577  ._features = new
+0001af20: 5f66 6561 7475 7265 730a 0a20 2020 2040  _features..    @
+0001af30: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0001af40: 2066 6561 7475 7265 5f73 746f 7265 5f6e   feature_store_n
+0001af50: 616d 6528 7365 6c66 293a 0a20 2020 2020  ame(self):.     
+0001af60: 2020 2022 2222 4e61 6d65 206f 6620 7468     """Name of th
+0001af70: 6520 6665 6174 7572 6520 7374 6f72 6520  e feature store 
+0001af80: 696e 2077 6869 6368 2074 6865 2066 6561  in which the fea
+0001af90: 7475 7265 2067 726f 7570 2069 7320 6c6f  ture group is lo
+0001afa0: 6361 7465 642e 2222 220a 2020 2020 2020  cated.""".      
+0001afb0: 2020 7265 7475 726e 2073 656c 662e 5f66    return self._f
+0001afc0: 6561 7475 7265 5f73 746f 7265 5f6e 616d  eature_store_nam
+0001afd0: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
+0001afe0: 0a20 2020 2064 6566 2066 6561 7475 7265  .    def feature
+0001aff0: 5f73 746f 7265 5f69 6428 7365 6c66 293a  _store_id(self):
+0001b000: 0a20 2020 2020 2020 2022 2222 4964 206f  .        """Id o
+0001b010: 6620 7468 6520 6665 6174 7572 6520 7374  f the feature st
+0001b020: 6f72 6520 696e 2077 6869 6368 2074 6865  ore in which the
+0001b030: 2066 6561 7475 7265 2067 726f 7570 2069   feature group i
+0001b040: 7320 6c6f 6361 7465 642e 2222 220a 2020  s located.""".  
+0001b050: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001b060: 662e 5f66 6561 7475 7265 5f73 746f 7265  f._feature_store
+0001b070: 5f69 640a                                _id.
```

### Comparing `hsfs-3.1.1rc4/hsfs/feature_group_commit.py` & `hsfs-3.2.0rc0/hsfs/feature_group_commit.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/feature_store.py` & `hsfs-3.2.0rc0/hsfs/feature_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,14 +508,18 @@
                 `"exact_uniqueness"` to compute uniqueness, distinctness and entropy.
                 The values should be booleans indicating the setting. To fully turn off
                 statistics computation pass `statistics_config=False`. Defaults to
                 `None` and will compute only descriptive statistics.
             event_time: Optionally, provide the name of the feature containing the event
                 time for the features in this feature group. If event_time is set
                 the feature group can be used for point-in-time joins. Defaults to `None`.
+
+                !!!note "Event time data type restriction"
+                    The supported data types for the event time column are: `timestamp`, `date` and `bigint`.
+
             stream: Optionally, Define whether the feature group should support real time stream writing capabilities.
                 Stream enabled Feature Groups have unified single API for writing streaming features transparently
                 to both online and offline store.
             expectation_suite: Optionally, attach an expectation suite to the feature
                 group which dataframes should be validated against upon insertion.
                 Defaults to `None`.
             parents: Optionally, Define the parents of this feature group as the
@@ -619,14 +623,18 @@
                 `None` and will compute only descriptive statistics.
             expectation_suite: Optionally, attach an expectation suite to the feature
                 group which dataframes should be validated against upon insertion.
                 Defaults to `None`.
             event_time: Optionally, provide the name of the feature containing the event
                 time for the features in this feature group. If event_time is set
                 the feature group can be used for point-in-time joins. Defaults to `None`.
+
+                !!!note "Event time data type restriction"
+                    The supported data types for the event time column are: `timestamp`, `date` and `bigint`.
+
             stream: Optionally, Define whether the feature group should support real time stream writing capabilities.
                 Stream enabled Feature Groups have unified single API for writing streaming features transparently
                 to both online and offline store.
             parents: Optionally, Define the parents of this feature group as the
                 origin where the data is coming from.
 
         # Returns
@@ -726,14 +734,18 @@
                 `"exact_uniqueness"` to compute uniqueness, distinctness and entropy.
                 The values should be booleans indicating the setting. To fully turn off
                 statistics computation pass `statistics_config=False`. Defaults to
                 `None` and will compute only descriptive statistics.
             event_time: Optionally, provide the name of the feature containing the event
                 time for the features in this feature group. If event_time is set
                 the feature group can be used for point-in-time joins. Defaults to `None`.
+
+                !!!note "Event time data type restriction"
+                    The supported data types for the event time column are: `timestamp`, `date` and `bigint`.
+
             expectation_suite: Optionally, attach an expectation suite to the feature
                 group which dataframes should be validated against upon insertion.
                 Defaults to `None`.
 
         # Returns
             `ExternalFeatureGroup`. The external feature group metadata object.
         """
@@ -768,14 +780,15 @@
         primary_key: Optional[List[str]] = [],
         features: Optional[List[feature.Feature]] = [],
         statistics_config: Optional[Union[StatisticsConfig, bool, dict]] = None,
         event_time: Optional[str] = None,
         expectation_suite: Optional[
             Union[expectation_suite.ExpectationSuite, ge.core.ExpectationSuite]
         ] = None,
+        online_enabled: Optional[bool] = False,
     ):
         """Create a external feature group metadata object.
 
         !!! example
             ```python
             # connect to the Feature Store
             fs = ...
@@ -792,14 +805,37 @@
             ```
 
         !!! note "Lazy"
             This method is lazy and does not persist any metadata in the
             feature store on its own. To persist the feature group metadata in the feature store,
             call the `save()` method.
 
+        You can enable online storage for external feature groups, however, the sync from the
+        external storage to Hopsworks online storage needs to be done manually:
+
+        ```python
+        external_fg = fs.create_external_feature_group(
+                    name="sales",
+                    version=1,
+                    description="Physical shop sales features",
+                    query=query,
+                    storage_connector=connector,
+                    primary_key=['ss_store_sk'],
+                    event_time='sale_date',
+                    online_enabled=True
+                    )
+        external_fg.save()
+
+        # read from external storage and filter data to sync to online
+        df = external_fg.read().filter(external_fg.customer_status == "active")
+
+        # insert to online storage
+        external_fg.insert(df)
+        ```
+
         # Arguments
             name: Name of the external feature group to create.
             storage_connector: the storage connector to use to establish connectivity
                 with the data source.
             query: A string containing a SQL query valid for the target data source.
                 the query will be used to pull data from the data sources when the
                 feature group is used.
@@ -831,17 +867,23 @@
                 `"exact_uniqueness"` to compute uniqueness, distinctness and entropy.
                 The values should be booleans indicating the setting. To fully turn off
                 statistics computation pass `statistics_config=False`. Defaults to
                 `None` and will compute only descriptive statistics.
             event_time: Optionally, provide the name of the feature containing the event
                 time for the features in this feature group. If event_time is set
                 the feature group can be used for point-in-time joins. Defaults to `None`.
+
+                !!!note "Event time data type restriction"
+                    The supported data types for the event time column are: `timestamp`, `date` and `bigint`.
+
             expectation_suite: Optionally, attach an expectation suite to the feature
                 group which dataframes should be validated against upon insertion.
                 Defaults to `None`.
+            online_enabled: Define whether it should be possible to sync the feature group to
+                the online feature store for low latency access, defaults to `False`.
 
         # Returns
             `ExternalFeatureGroup`. The external feature group metadata object.
         """
         return feature_group.ExternalFeatureGroup(
             name=name,
             query=query,
@@ -854,14 +896,15 @@
             primary_key=primary_key,
             featurestore_id=self._id,
             featurestore_name=self._name,
             features=features,
             statistics_config=statistics_config,
             event_time=event_time,
             expectation_suite=expectation_suite,
+            online_enabled=online_enabled,
         )
 
     def create_training_dataset(
         self,
         name: str,
         version: Optional[int] = None,
         description: Optional[str] = "",
```

### Comparing `hsfs-3.1.1rc4/hsfs/feature_view.py` & `hsfs-3.2.0rc0/hsfs/feature_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,15 @@
         """
         return self._feature_view_engine.update(self)
 
     def init_serving(
         self,
         training_dataset_version: Optional[int] = None,
         external: Optional[bool] = None,
+        options: Optional[dict] = None,
     ):
         """Initialise feature view to retrieve feature vector from online feature store.
 
         !!! example
             ```python
             # get feature store instance
             fs = ...
@@ -191,34 +192,37 @@
                 are fetched from training dataset and applied to the feature vector.
             external: boolean, optional. If set to True, the connection to the
                 online feature store is established using the same host as
                 for the `host` parameter in the [`hsfs.connection()`](connection_api.md#connection) method.
                 If set to False, the online feature store storage connector is used which relies on the private IP.
                 Defaults to True if connection to Hopsworks is established from external environment (e.g AWS
                 Sagemaker or Google Colab), otherwise to False.
+            options: Additional options as key/value pairs for configuring online serving engine.
+                * key: kwargs of SqlAlchemy engine creation (See: https://docs.sqlalchemy.org/en/20/core/engines.html#sqlalchemy.create_engine).
+                  For example: `{"pool_size": 10}`
         """
 
         if training_dataset_version is None:
             training_dataset_version = 1
             warnings.warn(
                 "No training dataset version was provided to initialise serving. Defaulting to version 1.",
                 util.VersionWarning,
             )
 
         # initiate single vector server
         self._single_vector_server = vector_server.VectorServer(
             self._featurestore_id, self._features, training_dataset_version
         )
-        self._single_vector_server.init_serving(self, False, external)
+        self._single_vector_server.init_serving(self, False, external, options=options)
 
         # initiate batch vector server
         self._batch_vectors_server = vector_server.VectorServer(
             self._featurestore_id, self._features, training_dataset_version
         )
-        self._batch_vectors_server.init_serving(self, True, external)
+        self._batch_vectors_server.init_serving(self, True, external, options=options)
 
         # initiate batch scoring server
         self.init_batch_scoring(training_dataset_version)
 
     def init_batch_scoring(
         self,
         training_dataset_version: Optional[int] = None,
@@ -302,15 +306,17 @@
     def get_feature_vector(
         self,
         entry: Dict[str, Any],
         passed_features: Optional[Dict[str, Any]] = {},
         external: Optional[bool] = None,
     ):
         """Returns assembled feature vector from online feature store.
-
+            Call [`feature_view.init_serving`](#init_serving) before this method if the following configurations are needed.
+              1. The training dataset version of the transformation statistics
+              2. Additional configurations of online serving engine
         !!! warning "Missing primary key entries"
             If the provided primary key `entry` can't be found in one or more of the feature groups
             used by this feature view the call to this method will raise an exception.
 
         !!! example
             ```python
             # get feature store instance
@@ -369,15 +375,17 @@
     def get_feature_vectors(
         self,
         entry: List[Dict[str, Any]],
         passed_features: Optional[List[Dict[str, Any]]] = {},
         external: Optional[bool] = None,
     ):
         """Returns assembled feature vectors in batches from online feature store.
-
+            Call [`feature_view.init_serving`](#init_serving) before this method if the following configurations are needed.
+              1. The training dataset version of the transformation statistics
+              2. Additional configurations of online serving engine
         !!! warning "Missing primary key entries"
             If any of the provided primary key elements in `entry` can't be found in any
             of the feature groups, no feature vector for that primary key value will be
             returned.
             If it can be found in at least one but not all feature groups used by
             this feature view the call to this method will raise an exception.
```

### Comparing `hsfs-3.1.1rc4/hsfs/ge_expectation.py` & `hsfs-3.2.0rc0/hsfs/ge_expectation.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/ge_validation_result.py` & `hsfs-3.2.0rc0/hsfs/ge_validation_result.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/split_statistics.py` & `hsfs-3.2.0rc0/hsfs/split_statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/statistics.py` & `hsfs-3.2.0rc0/hsfs/statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/statistics_config.py` & `hsfs-3.2.0rc0/hsfs/statistics_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/storage_connector.py` & `hsfs-3.2.0rc0/hsfs/storage_connector.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/tag.py` & `hsfs-3.2.0rc0/hsfs/tag.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/training_dataset.py` & `hsfs-3.2.0rc0/hsfs/training_dataset.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/training_dataset_feature.py` & `hsfs-3.2.0rc0/hsfs/training_dataset_feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/training_dataset_split.py` & `hsfs-3.2.0rc0/hsfs/training_dataset_split.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/transformation_function.py` & `hsfs-3.2.0rc0/hsfs/transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/transformation_function_attached.py` & `hsfs-3.2.0rc0/hsfs/transformation_function_attached.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/user.py` & `hsfs-3.2.0rc0/hsfs/user.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/util.py` & `hsfs-3.2.0rc0/hsfs/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     name = name.lower()
     if name.endswith(FEATURE_STORE_NAME_SUFFIX):
         return name
     else:
         return name + FEATURE_STORE_NAME_SUFFIX
 
 
-def create_mysql_engine(online_conn, external):
+def create_mysql_engine(online_conn, external, options=None):
     online_options = online_conn.spark_options()
     # Here we are replacing the first part of the string returned by Hopsworks,
     # jdbc:mysql:// with the sqlalchemy one + username and password
     # useSSL and allowPublicKeyRetrieval are not valid properties for the pymysql driver
     # to use SSL we'll have to something like this:
     # ssl_args = {'ssl_ca': ca_path}
     # engine = create_engine("mysql+pymysql://<user>:<pass>@<addr>/<schema>", connect_args=ssl_args)
@@ -92,17 +92,22 @@
             + ":"
             + online_options["password"]
             + "@",
         )
         .replace("useSSL=false&", "")
         .replace("?allowPublicKeyRetrieval=true", "")
     )
-
+    if options is not None and not isinstance(options, dict):
+        raise TypeError("`options` should be a `dict` type.")
+    if not options:
+        options = {"pool_recycle": 3600}
+    elif "pool_recycle" not in options:
+        options["pool_recycle"] = 3600
     # default connection pool size kept by engine is 5
-    sql_alchemy_engine = create_engine(sql_alchemy_conn_str, pool_recycle=3600)
+    sql_alchemy_engine = create_engine(sql_alchemy_conn_str, **options)
     return sql_alchemy_engine
 
 
 def check_timestamp_format_from_date_string(input_date):
     date_format_patterns = {
         r"^([0-9]{4})([0-9]{2})([0-9]{2})$": "%Y%m%d",
         r"^([0-9]{4})([0-9]{2})([0-9]{2})([0-9]{2})$": "%Y%m%d%H",
```

### Comparing `hsfs-3.1.1rc4/hsfs/validation_report.py` & `hsfs-3.2.0rc0/hsfs/validation_report.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.1.1rc4/hsfs/version.py` & `hsfs-3.2.0rc0/hsfs/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.1.1rc4"
+__version__ = "3.2.0rc0"
```

### Comparing `hsfs-3.1.1rc4/hsfs.egg-info/PKG-INFO` & `hsfs-3.2.0rc0/hsfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.1.1rc4
+Version: 3.2.0rc0
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.1.1rc4
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc0
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.1.1rc4 Summary: HSFS: An
+Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc0 Summary: HSFS: An
 environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api Author: Hopsworks
 AB Author-email: moritz@logicalclocks.com License: Apache License 2.0 Download-
-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.1.1rc4
+URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc0
 Description: # Hopsworks Feature Store
   [Hopsworks_Community] [Hopsworks_Feature_Store_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.1.1rc4/hsfs.egg-info/SOURCES.txt` & `hsfs-3.2.0rc0/hsfs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 hsfs/code.py
 hsfs/connection.py
 hsfs/decorators.py
 hsfs/expectation_suite.py
 hsfs/feature.py
 hsfs/feature_group.py
 hsfs/feature_group_commit.py
+hsfs/feature_group_writer.py
 hsfs/feature_store.py
 hsfs/feature_view.py
 hsfs/ge_expectation.py
 hsfs/ge_validation_result.py
 hsfs/split_statistics.py
 hsfs/statistics.py
 hsfs/statistics_config.py
```

### Comparing `hsfs-3.1.1rc4/hsfs.egg-info/requires.txt` & `hsfs-3.2.0rc0/hsfs.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 PyMySQL[rsa]
-avro==1.10.2
+avro==1.11.0
 boto3
 furl
 great_expectations==0.14.12
 markupsafe<2.1.0
 mock
 numpy
 pandas<2.0.0,>=1.2.0
```

### Comparing `hsfs-3.1.1rc4/setup.py` & `hsfs-3.2.0rc0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         "requests",
         "furl",
         "boto3",
         "pandas>=1.2.0,<2.0.0",
         "numpy",
         "pyjks",
         "mock",
-        "avro==1.10.2",
+        "avro==1.11.0",
         "sqlalchemy",
         "PyMySQL[rsa]",
         "great_expectations==0.14.12",
         "markupsafe<2.1.0",  # GE issue 1: jinja2==2.11.3, pulls in markupsafe 2.1.0 which is not compatible with jinja2==2.11.3.
         "tzlocal",
     ],
     extras_require={
```

