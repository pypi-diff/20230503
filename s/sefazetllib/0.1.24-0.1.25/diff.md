# Comparing `tmp/sefazetllib-0.1.24.tar.gz` & `tmp/sefazetllib-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sefazetllib-0.1.24.tar", max compression
+gzip compressed data, was "sefazetllib-0.1.25.tar", max compression
```

## Comparing `sefazetllib-0.1.24.tar` & `sefazetllib-0.1.25.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    10349 2023-03-22 02:02:06.498182 sefazetllib-0.1.24/LICENSE
--rw-r--r--   0        0        0     2537 2023-04-13 13:05:41.916016 sefazetllib-0.1.24/pyproject.toml
--rw-r--r--   0        0        0     3264 2023-04-09 18:51:54.608430 sefazetllib-0.1.24/README.md
--rw-r--r--   0        0        0      137 2023-03-22 11:22:30.166093 sefazetllib-0.1.24/sefazetllib/__init__.py
--rw-r--r--   0        0        0     1716 2023-03-22 11:35:33.508530 sefazetllib-0.1.24/sefazetllib/Builder.py
--rw-r--r--   0        0        0       53 2023-03-22 11:18:45.691953 sefazetllib-0.1.24/sefazetllib/config/__init__.py
--rw-r--r--   0        0        0     2415 2023-03-28 02:16:14.475807 sefazetllib-0.1.24/sefazetllib/config/CustomLogging.py
--rw-r--r--   0        0        0       37 2023-03-22 02:03:33.079166 sefazetllib-0.1.24/sefazetllib/etl/__init__.py
--rw-r--r--   0        0        0     8363 2023-03-28 02:16:14.477806 sefazetllib-0.1.24/sefazetllib/etl/ETL.py
--rw-r--r--   0        0        0      279 2023-03-22 11:23:55.081767 sefazetllib-0.1.24/sefazetllib/extract/__init__.py
--rw-r--r--   0        0        0      729 2023-03-22 11:35:33.511528 sefazetllib-0.1.24/sefazetllib/extract/Extract.py
--rw-r--r--   0        0        0     2047 2023-03-22 11:35:33.512538 sefazetllib-0.1.24/sefazetllib/extract/ExtractLocal.py
--rw-r--r--   0        0        0     2552 2023-03-24 02:29:17.874836 sefazetllib-0.1.24/sefazetllib/extract/ExtractS3.py
--rw-r--r--   0        0        0     2600 2023-03-22 11:24:35.794185 sefazetllib-0.1.24/sefazetllib/extract/ExtractSQL.py
--rw-r--r--   0        0        0     2351 2023-03-22 11:35:33.515528 sefazetllib-0.1.24/sefazetllib/extract/ExtractStorage.py
--rw-r--r--   0        0        0       91 2023-03-22 02:17:48.512311 sefazetllib-0.1.24/sefazetllib/factory/__init__.py
--rw-r--r--   0        0        0      967 2023-03-22 11:35:33.517536 sefazetllib-0.1.24/sefazetllib/factory/Factory.py
--rw-r--r--   0        0        0      272 2023-03-22 11:24:56.091205 sefazetllib-0.1.24/sefazetllib/factory/platform/__init__.py
--rw-r--r--   0        0        0      137 2023-03-22 11:27:14.887522 sefazetllib-0.1.24/sefazetllib/factory/platform/database/__init__.py
--rw-r--r--   0        0        0      749 2023-03-22 11:35:33.520527 sefazetllib-0.1.24/sefazetllib/factory/platform/database/MySQL.py
--rw-r--r--   0        0        0      814 2023-03-22 11:28:00.370816 sefazetllib-0.1.24/sefazetllib/factory/platform/database/PostgresSQL.py
--rw-r--r--   0        0        0      380 2023-03-22 11:25:06.491132 sefazetllib-0.1.24/sefazetllib/factory/platform/DatabasePlatform.py
--rw-r--r--   0        0        0      198 2023-03-22 11:28:08.380181 sefazetllib-0.1.24/sefazetllib/factory/platform/dataframe/__init__.py
--rw-r--r--   0        0        0      272 2023-03-22 11:35:33.522527 sefazetllib-0.1.24/sefazetllib/factory/platform/dataframe/Default.py
--rw-r--r--   0        0        0     1854 2023-03-22 11:35:33.523528 sefazetllib-0.1.24/sefazetllib/factory/platform/dataframe/Pandas.py
--rw-r--r--   0        0        0     4220 2023-04-08 00:24:55.746715 sefazetllib-0.1.24/sefazetllib/factory/platform/dataframe/Spark.py
--rw-r--r--   0        0        0      297 2023-03-22 11:35:33.518538 sefazetllib-0.1.24/sefazetllib/factory/platform/Platform.py
--rw-r--r--   0        0        0     1077 2023-03-22 11:27:04.493215 sefazetllib-0.1.24/sefazetllib/factory/platform/PlatformFactory.py
--rw-r--r--   0        0        0      234 2023-03-22 11:35:33.533527 sefazetllib-0.1.24/sefazetllib/load/__init__.py
--rw-r--r--   0        0        0      711 2023-03-22 11:35:33.526527 sefazetllib-0.1.24/sefazetllib/load/Load.py
--rw-r--r--   0        0        0     2077 2023-03-22 11:35:33.528526 sefazetllib-0.1.24/sefazetllib/load/LoadLocal.py
--rw-r--r--   0        0        0     2372 2023-03-22 11:35:33.529528 sefazetllib-0.1.24/sefazetllib/load/LoadS3.py
--rw-r--r--   0        0        0     2835 2023-03-22 11:35:33.531566 sefazetllib-0.1.24/sefazetllib/load/LoadSQL.py
--rw-r--r--   0        0        0     2261 2023-03-22 11:35:33.532526 sefazetllib-0.1.24/sefazetllib/load/LoadStorage.py
--rw-r--r--   0        0        0      201 2023-03-22 02:12:37.861367 sefazetllib-0.1.24/sefazetllib/transform/__init__.py
--rw-r--r--   0        0        0     1523 2023-03-22 02:15:28.119480 sefazetllib-0.1.24/sefazetllib/transform/MinMaxLineTransform.py
--rw-r--r--   0        0        0     4445 2023-04-08 00:24:55.749710 sefazetllib-0.1.24/sefazetllib/transform/QuartileTransform.py
--rw-r--r--   0        0        0      577 2023-03-22 11:35:33.535526 sefazetllib-0.1.24/sefazetllib/transform/Transform.py
--rw-r--r--   0        0        0       46 2023-03-22 02:08:23.799891 sefazetllib-0.1.24/sefazetllib/utils/__init__.py
--rw-r--r--   0        0        0      161 2023-03-22 02:03:33.166061 sefazetllib-0.1.24/sefazetllib/utils/key/__init__.py
--rw-r--r--   0        0        0      339 2023-03-22 11:35:33.536528 sefazetllib-0.1.24/sefazetllib/utils/key/DefaultKey.py
--rw-r--r--   0        0        0      419 2023-03-22 11:35:33.537527 sefazetllib-0.1.24/sefazetllib/utils/key/Key.py
--rw-r--r--   0        0        0      775 2023-03-22 11:35:33.538526 sefazetllib-0.1.24/sefazetllib/utils/key/SurrogateKey.py
--rw-r--r--   0        0        0      234 2023-03-22 02:03:33.178225 sefazetllib-0.1.24/sefazetllib/utils/partition/__init__.py
--rw-r--r--   0        0        0     2172 2023-03-22 11:21:12.190698 sefazetllib-0.1.24/sefazetllib/utils/partition/DatePartition.py
--rw-r--r--   0        0        0      652 2023-03-22 11:21:29.374214 sefazetllib-0.1.24/sefazetllib/utils/partition/IncrementalRangePartition.py
--rw-r--r--   0        0        0      447 2023-03-22 11:35:33.539526 sefazetllib-0.1.24/sefazetllib/utils/partition/Partition.py
--rw-r--r--   0        0        0      112 2023-03-22 11:35:33.543527 sefazetllib-0.1.24/sefazetllib/validate/__init__.py
--rw-r--r--   0        0        0     7817 2023-04-13 01:29:36.832013 sefazetllib-0.1.24/sefazetllib/validate/DataValidate.py
--rw-r--r--   0        0        0      122 2023-03-22 11:35:33.542530 sefazetllib-0.1.24/sefazetllib/validate/Validate.py
--rw-r--r--   0        0        0     3675 2023-04-13 13:05:41.918016 sefazetllib-0.1.24/sefazetllibcli/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 01:29:36.835022 sefazetllib-0.1.24/sefazetllibcli/config/__init__.py
--rw-r--r--   0        0        0     1153 2023-04-13 01:29:36.839029 sefazetllib-0.1.24/sefazetllibcli/config/logging.py
--rw-r--r--   0        0        0      188 2023-04-13 01:29:36.841551 sefazetllib-0.1.24/sefazetllibcli/errors/__init__.py
--rw-r--r--   0        0        0       78 2023-04-13 01:29:36.842562 sefazetllib-0.1.24/sefazetllibcli/errors/method_not_implemented.py
--rw-r--r--   0        0        0       54 2023-04-13 01:29:36.843561 sefazetllib-0.1.24/sefazetllibcli/errors/unsupported_file_extension.py
--rw-r--r--   0        0        0       90 2023-04-13 01:29:36.845560 sefazetllib-0.1.24/sefazetllibcli/errors/variable_processing_error.py
--rw-r--r--   0        0        0        0 2023-04-13 01:29:36.846578 sefazetllib-0.1.24/sefazetllibcli/generators/__init__.py
--rw-r--r--   0        0        0     6071 2023-04-13 01:29:36.847561 sefazetllib-0.1.24/sefazetllibcli/generators/etl_generator.py
--rw-r--r--   0        0        0      908 2023-04-13 01:29:36.848399 sefazetllib-0.1.24/sefazetllibcli/generators/generator.py
--rw-r--r--   0        0        0      390 2023-04-13 01:29:36.848399 sefazetllib-0.1.24/sefazetllibcli/templates/etl_template
--rw-r--r--   0        0        0        0 2023-04-13 01:29:36.848399 sefazetllib-0.1.24/sefazetllibcli/usecases/__init__.py
--rw-r--r--   0        0        0      533 2023-04-13 01:29:36.848399 sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/__init__.py
--rw-r--r--   0        0        0     3582 2023-04-13 01:29:36.848399 sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_etl_variable.py
--rw-r--r--   0        0        0     1158 2023-04-13 01:29:36.848399 sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_extract_variable.py
--rw-r--r--   0        0        0     1014 2023-04-13 01:29:36.848399 sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_imports_variable.py
--rw-r--r--   0        0        0     1174 2023-04-13 01:29:36.863428 sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_key_variable.py
--rw-r--r--   0        0        0     1140 2023-04-13 01:29:36.863428 sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_load_variable.py
--rw-r--r--   0        0        0     1640 2023-04-13 01:29:36.863428 sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_partition_variable.py
--rw-r--r--   0        0        0     2148 2023-04-13 01:29:36.863428 sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
--rw-r--r--   0        0        0     1106 2023-04-13 01:29:36.863428 sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_validate_variable.py
--rw-r--r--   0        0        0      963 2023-04-13 01:29:36.863428 sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_variable.py
--rw-r--r--   0        0        0      101 2023-04-13 01:29:36.879071 sefazetllib-0.1.24/sefazetllibcli/usecases/replace_template/__init__.py
--rw-r--r--   0        0        0      996 2023-04-13 01:29:36.879071 sefazetllib-0.1.24/sefazetllibcli/usecases/replace_template/replace_etl_template.py
--rw-r--r--   0        0        0     1724 2023-04-13 01:29:36.879071 sefazetllib-0.1.24/sefazetllibcli/usecases/replace_template/replace_template.py
--rw-r--r--   0        0        0       33 2023-04-13 01:29:36.890996 sefazetllib-0.1.24/sefazetllibcli/utils/__init__.py
--rw-r--r--   0        0        0     3744 2023-04-13 01:29:36.892995 sefazetllib-0.1.24/sefazetllibcli/utils/parse_etl.py
--rw-r--r--   0        0        0     4975 1970-01-01 00:00:00.000000 sefazetllib-0.1.24/setup.py
--rw-r--r--   0        0        0     4934 1970-01-01 00:00:00.000000 sefazetllib-0.1.24/PKG-INFO
+-rw-r--r--   0        0        0    10349 2023-03-22 02:02:06.498182 sefazetllib-0.1.25/LICENSE
+-rw-r--r--   0        0        0     2537 2023-05-03 17:55:22.825376 sefazetllib-0.1.25/pyproject.toml
+-rw-r--r--   0        0        0     3264 2023-04-09 18:51:54.608430 sefazetllib-0.1.25/README.md
+-rw-r--r--   0        0        0      137 2023-03-22 11:22:30.166093 sefazetllib-0.1.25/sefazetllib/__init__.py
+-rw-r--r--   0        0        0     1716 2023-03-22 11:35:33.508530 sefazetllib-0.1.25/sefazetllib/Builder.py
+-rw-r--r--   0        0        0       53 2023-03-22 11:18:45.691953 sefazetllib-0.1.25/sefazetllib/config/__init__.py
+-rw-r--r--   0        0        0     2415 2023-03-28 02:16:14.475807 sefazetllib-0.1.25/sefazetllib/config/CustomLogging.py
+-rw-r--r--   0        0        0       37 2023-03-22 02:03:33.079166 sefazetllib-0.1.25/sefazetllib/etl/__init__.py
+-rw-r--r--   0        0        0     8363 2023-03-28 02:16:14.477806 sefazetllib-0.1.25/sefazetllib/etl/ETL.py
+-rw-r--r--   0        0        0      279 2023-03-22 11:23:55.081767 sefazetllib-0.1.25/sefazetllib/extract/__init__.py
+-rw-r--r--   0        0        0      729 2023-03-22 11:35:33.511528 sefazetllib-0.1.25/sefazetllib/extract/Extract.py
+-rw-r--r--   0        0        0     2047 2023-03-22 11:35:33.512538 sefazetllib-0.1.25/sefazetllib/extract/ExtractLocal.py
+-rw-r--r--   0        0        0     2552 2023-03-24 02:29:17.874836 sefazetllib-0.1.25/sefazetllib/extract/ExtractS3.py
+-rw-r--r--   0        0        0     2600 2023-03-22 11:24:35.794185 sefazetllib-0.1.25/sefazetllib/extract/ExtractSQL.py
+-rw-r--r--   0        0        0     2351 2023-03-22 11:35:33.515528 sefazetllib-0.1.25/sefazetllib/extract/ExtractStorage.py
+-rw-r--r--   0        0        0       91 2023-03-22 02:17:48.512311 sefazetllib-0.1.25/sefazetllib/factory/__init__.py
+-rw-r--r--   0        0        0      967 2023-03-22 11:35:33.517536 sefazetllib-0.1.25/sefazetllib/factory/Factory.py
+-rw-r--r--   0        0        0      272 2023-03-22 11:24:56.091205 sefazetllib-0.1.25/sefazetllib/factory/platform/__init__.py
+-rw-r--r--   0        0        0      136 2023-05-03 17:55:22.831406 sefazetllib-0.1.25/sefazetllib/factory/platform/database/__init__.py
+-rw-r--r--   0        0        0      749 2023-03-22 11:35:33.520527 sefazetllib-0.1.25/sefazetllib/factory/platform/database/MySQL.py
+-rw-r--r--   0        0        0     4156 2023-05-03 17:55:22.828363 sefazetllib-0.1.25/sefazetllib/factory/platform/database/PostgreSQL.py
+-rw-r--r--   0        0        0      380 2023-03-22 11:25:06.491132 sefazetllib-0.1.25/sefazetllib/factory/platform/DatabasePlatform.py
+-rw-r--r--   0        0        0      198 2023-03-22 11:28:08.380181 sefazetllib-0.1.25/sefazetllib/factory/platform/dataframe/__init__.py
+-rw-r--r--   0        0        0      272 2023-03-22 11:35:33.522527 sefazetllib-0.1.25/sefazetllib/factory/platform/dataframe/Default.py
+-rw-r--r--   0        0        0     1854 2023-03-22 11:35:33.523528 sefazetllib-0.1.25/sefazetllib/factory/platform/dataframe/Pandas.py
+-rw-r--r--   0        0        0     4594 2023-05-03 17:55:22.833399 sefazetllib-0.1.25/sefazetllib/factory/platform/dataframe/Spark.py
+-rw-r--r--   0        0        0      297 2023-03-22 11:35:33.518538 sefazetllib-0.1.25/sefazetllib/factory/platform/Platform.py
+-rw-r--r--   0        0        0     1077 2023-03-22 11:27:04.493215 sefazetllib-0.1.25/sefazetllib/factory/platform/PlatformFactory.py
+-rw-r--r--   0        0        0      234 2023-03-22 11:35:33.533527 sefazetllib-0.1.25/sefazetllib/load/__init__.py
+-rw-r--r--   0        0        0      711 2023-03-22 11:35:33.526527 sefazetllib-0.1.25/sefazetllib/load/Load.py
+-rw-r--r--   0        0        0     2077 2023-03-22 11:35:33.528526 sefazetllib-0.1.25/sefazetllib/load/LoadLocal.py
+-rw-r--r--   0        0        0     2458 2023-05-03 17:55:22.834392 sefazetllib-0.1.25/sefazetllib/load/LoadS3.py
+-rw-r--r--   0        0        0     7164 2023-05-03 17:55:22.836392 sefazetllib-0.1.25/sefazetllib/load/LoadSQL.py
+-rw-r--r--   0        0        0     2261 2023-03-22 11:35:33.532526 sefazetllib-0.1.25/sefazetllib/load/LoadStorage.py
+-rw-r--r--   0        0        0      201 2023-03-22 02:12:37.861367 sefazetllib-0.1.25/sefazetllib/transform/__init__.py
+-rw-r--r--   0        0        0     1523 2023-03-22 02:15:28.119480 sefazetllib-0.1.25/sefazetllib/transform/MinMaxLineTransform.py
+-rw-r--r--   0        0        0     4445 2023-04-08 00:24:55.749710 sefazetllib-0.1.25/sefazetllib/transform/QuartileTransform.py
+-rw-r--r--   0        0        0      577 2023-03-22 11:35:33.535526 sefazetllib-0.1.25/sefazetllib/transform/Transform.py
+-rw-r--r--   0        0        0       46 2023-03-22 02:08:23.799891 sefazetllib-0.1.25/sefazetllib/utils/__init__.py
+-rw-r--r--   0        0        0      161 2023-03-22 02:03:33.166061 sefazetllib-0.1.25/sefazetllib/utils/key/__init__.py
+-rw-r--r--   0        0        0      339 2023-03-22 11:35:33.536528 sefazetllib-0.1.25/sefazetllib/utils/key/DefaultKey.py
+-rw-r--r--   0        0        0      419 2023-03-22 11:35:33.537527 sefazetllib-0.1.25/sefazetllib/utils/key/Key.py
+-rw-r--r--   0        0        0      775 2023-03-22 11:35:33.538526 sefazetllib-0.1.25/sefazetllib/utils/key/SurrogateKey.py
+-rw-r--r--   0        0        0      234 2023-03-22 02:03:33.178225 sefazetllib-0.1.25/sefazetllib/utils/partition/__init__.py
+-rw-r--r--   0        0        0     2172 2023-03-22 11:21:12.190698 sefazetllib-0.1.25/sefazetllib/utils/partition/DatePartition.py
+-rw-r--r--   0        0        0      652 2023-03-22 11:21:29.374214 sefazetllib-0.1.25/sefazetllib/utils/partition/IncrementalRangePartition.py
+-rw-r--r--   0        0        0      447 2023-03-22 11:35:33.539526 sefazetllib-0.1.25/sefazetllib/utils/partition/Partition.py
+-rw-r--r--   0        0        0      112 2023-03-22 11:35:33.543527 sefazetllib-0.1.25/sefazetllib/validate/__init__.py
+-rw-r--r--   0        0        0     7817 2023-05-03 17:55:22.840469 sefazetllib-0.1.25/sefazetllib/validate/DataValidate.py
+-rw-r--r--   0        0        0      122 2023-03-22 11:35:33.542530 sefazetllib-0.1.25/sefazetllib/validate/Validate.py
+-rw-r--r--   0        0        0     3675 2023-05-03 17:55:22.841468 sefazetllib-0.1.25/sefazetllibcli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 17:55:22.846732 sefazetllib-0.1.25/sefazetllibcli/config/__init__.py
+-rw-r--r--   0        0        0     1153 2023-05-03 17:55:22.848772 sefazetllib-0.1.25/sefazetllibcli/config/logging.py
+-rw-r--r--   0        0        0      188 2023-05-03 17:55:22.850781 sefazetllib-0.1.25/sefazetllibcli/errors/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-03 17:55:22.852785 sefazetllib-0.1.25/sefazetllibcli/errors/method_not_implemented.py
+-rw-r--r--   0        0        0       54 2023-05-03 17:55:22.855787 sefazetllib-0.1.25/sefazetllibcli/errors/unsupported_file_extension.py
+-rw-r--r--   0        0        0       90 2023-05-03 17:55:22.859397 sefazetllib-0.1.25/sefazetllibcli/errors/variable_processing_error.py
+-rw-r--r--   0        0        0        0 2023-05-03 17:55:22.863453 sefazetllib-0.1.25/sefazetllibcli/generators/__init__.py
+-rw-r--r--   0        0        0     6071 2023-05-03 17:55:22.866434 sefazetllib-0.1.25/sefazetllibcli/generators/etl_generator.py
+-rw-r--r--   0        0        0      908 2023-05-03 17:55:22.867422 sefazetllib-0.1.25/sefazetllibcli/generators/generator.py
+-rw-r--r--   0        0        0      390 2023-05-03 17:55:22.870098 sefazetllib-0.1.25/sefazetllibcli/templates/etl_template
+-rw-r--r--   0        0        0        0 2023-05-03 17:55:22.871111 sefazetllib-0.1.25/sefazetllibcli/usecases/__init__.py
+-rw-r--r--   0        0        0      533 2023-05-03 17:55:22.874111 sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/__init__.py
+-rw-r--r--   0        0        0     3582 2023-05-03 17:55:22.875119 sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_etl_variable.py
+-rw-r--r--   0        0        0     1158 2023-05-03 17:55:22.876120 sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_extract_variable.py
+-rw-r--r--   0        0        0     1014 2023-05-03 17:55:22.878655 sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_imports_variable.py
+-rw-r--r--   0        0        0     1174 2023-05-03 17:55:22.879699 sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_key_variable.py
+-rw-r--r--   0        0        0     1140 2023-05-03 17:55:22.880699 sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_load_variable.py
+-rw-r--r--   0        0        0     1640 2023-05-03 17:55:22.881700 sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_partition_variable.py
+-rw-r--r--   0        0        0     2148 2023-05-03 17:55:22.883701 sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
+-rw-r--r--   0        0        0     1106 2023-05-03 17:55:22.885700 sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_validate_variable.py
+-rw-r--r--   0        0        0      963 2023-05-03 17:55:22.888826 sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_variable.py
+-rw-r--r--   0        0        0      101 2023-05-03 17:55:22.894836 sefazetllib-0.1.25/sefazetllibcli/usecases/replace_template/__init__.py
+-rw-r--r--   0        0        0      996 2023-05-03 17:55:22.896797 sefazetllib-0.1.25/sefazetllibcli/usecases/replace_template/replace_etl_template.py
+-rw-r--r--   0        0        0     1724 2023-05-03 17:55:22.899329 sefazetllib-0.1.25/sefazetllibcli/usecases/replace_template/replace_template.py
+-rw-r--r--   0        0        0       33 2023-05-03 17:55:22.901426 sefazetllib-0.1.25/sefazetllibcli/utils/__init__.py
+-rw-r--r--   0        0        0     3744 2023-05-03 17:55:22.902437 sefazetllib-0.1.25/sefazetllibcli/utils/parse_etl.py
+-rw-r--r--   0        0        0     4975 1970-01-01 00:00:00.000000 sefazetllib-0.1.25/setup.py
+-rw-r--r--   0        0        0     4934 1970-01-01 00:00:00.000000 sefazetllib-0.1.25/PKG-INFO
```

### Comparing `sefazetllib-0.1.24/LICENSE` & `sefazetllib-0.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/pyproject.toml` & `sefazetllib-0.1.25/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sefazetllib"
-version = "0.1.24"
+version = "0.1.25"
 description = "sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines."
 license = "Apache-2.0"
 authors = ["Felipe Gochi <felipe.gochi@elogroup.com.br>"]
 maintainers = [
     "Bruno Santos <bruno.santos@elogroup.com.br>",
     "Felipe Alcantara <felipe.alcantara@elogroup.com.br>",
     "Felipe Gochi <felipe.gochi@elogroup.com.br>",
```

### Comparing `sefazetllib-0.1.24/README.md` & `sefazetllib-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/Builder.py` & `sefazetllib-0.1.25/sefazetllib/Builder.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/config/CustomLogging.py` & `sefazetllib-0.1.25/sefazetllib/config/CustomLogging.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/etl/ETL.py` & `sefazetllib-0.1.25/sefazetllib/etl/ETL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/extract/Extract.py` & `sefazetllib-0.1.25/sefazetllib/extract/Extract.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/extract/ExtractLocal.py` & `sefazetllib-0.1.25/sefazetllib/extract/ExtractLocal.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/extract/ExtractS3.py` & `sefazetllib-0.1.25/sefazetllib/extract/ExtractS3.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/extract/ExtractSQL.py` & `sefazetllib-0.1.25/sefazetllib/extract/ExtractSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/extract/ExtractStorage.py` & `sefazetllib-0.1.25/sefazetllib/extract/ExtractStorage.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/factory/Factory.py` & `sefazetllib-0.1.25/sefazetllib/factory/Factory.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/factory/platform/database/MySQL.py` & `sefazetllib-0.1.25/sefazetllib/factory/platform/database/MySQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/factory/platform/dataframe/Pandas.py` & `sefazetllib-0.1.25/sefazetllib/factory/platform/dataframe/Pandas.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/factory/platform/dataframe/Spark.py` & `sefazetllib-0.1.25/sefazetllib/factory/platform/dataframe/Spark.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pyspark.sql import SparkSession
 from pyspark.sql.functions import (
+    col,
     current_date,
     lit,
     monotonically_increasing_id,
     xxhash64,
 )
 from pyspark.sql.types import StructType
 
@@ -15,36 +16,60 @@
     def __init__(self, name="Spark Job", configs=[]) -> None:
         self.name = name
         session = SparkSession.builder.appName(name)
         if configs != []:
             for config in configs:
                 session = session.config(*config)
         self.session = session.getOrCreate()
+        checkpoint_dir = "/tmp/checkpoint"
+        self.session.sparkContext.setCheckpointDir(checkpoint_dir)
 
     def __get_key_method(self, name):
         return {
             "SurrogateKey": xxhash64,
             "IncrementalKey": monotonically_increasing_id,
         }[name]
 
     def __define_properties(self, df, type_format, url, properties):
         if type_format == "jdbc":
             properties.pop("operation", None)
+            properties["url"] = url
+
         return df.options(**properties)
 
     def __define_load(self, df, type_format, url):
         if type_format == "jdbc":
             return df.load()
         return df.load(url)
 
     def __define_save(self, df, type_format, url):
         if type_format == "jdbc":
             return df.save()
         return df.save(url)
 
+    def columns_to_upper(self, df):
+        return df.select([col(c).alias(c.upper()) for c in df.columns])
+
+    def checkpoint(self, df):
+        return df.checkpoint()
+
+    def select_columns(self, df, columns):
+        return df.select(*columns)
+
+    def join(self, left, right, keys, how):
+        if isinstance(keys, list):
+            left_key, right_key = keys
+        else:
+            left_key = right_key = keys
+
+        return left.join(right, left[left_key] == right[right_key], how)
+
+    def union_by_name(self, left, right):
+        return left.unionByName(right)
+
     def read(self, **kwargs):
         type_format = kwargs["file_format"]
         url = kwargs["url"]
         format_properties = kwargs["format_properties"]
         optional = kwargs["optional"]
         columns = kwargs["columns"]
         duplicates = kwargs["duplicates"]
@@ -63,15 +88,15 @@
             if duplicates:
                 df = df.dropDuplicates()
             return df
 
         except Exception as e:
             if not optional:
                 logger.error("The 'optional' attribute is set to False. Error: %s", e)
-                raise
+                raise Exception("erro dentro do SPARK", str(e))
             schema = StructType([])
             df = self.session.createDataFrame([], schema)
             for cols in columns:
                 df = df.withColumn(cols, lit(None))
             return df
 
     def load(self, **kwargs):
@@ -80,54 +105,40 @@
         key = kwargs["key"]
         columns = kwargs["columns"]
         duplicates = kwargs["duplicates"]
         type_format = kwargs["file_format"]
         format_properties = kwargs["format_properties"]
         url = kwargs["url"]
         mode = kwargs["mode"]
+        load_date = kwargs["load_date"]
+
+        df_writer = df
 
-        if key.name is not None:
-            sk_name = key.name
+        if load_date:
+            df_writer = df_writer.withColumn("DAT_CARGA", current_date())
 
-        key.setMethod(self.__get_key_method(type(key).__name__))
+        if hasattr(key, "name"):  
+            if key.name is not None:
+                sk_name = key.name
 
-        df_writer = df.withColumn("DAT_CARGA", current_date()).withColumn(
-            sk_name, key.get()
-        )
+            key.setMethod(self.__get_key_method(type(key).__name__))
+            df_writer = df_writer.withColumn(sk_name, key.get())
 
         if bool(columns):
-            df_writer = df_writer.select(sk_name, *columns, "DAT_CARGA")
+            df_writer = df_writer.select(list(set([sk_name, *columns, "DAT_CARGA"])))
 
         if duplicates:
             df_writer = df_writer.dropDuplicates()
 
-        if (
-            "operation" in format_properties
-            and format_properties["operation"] == "upsert"
-        ):
-            df_old = self.read(
-                format=type_format,
-                url=url,
-                format_properties={**format_properties},
-                optional=True,
-                columns=df_writer.columns,
-                duplicates=duplicates,
-            ).drop("DAT_CARGA")
-
-            df_writer = df_writer.join(df_old, sk_name, "full")
-
-            for column in columns:
-                df_writer = df_writer.drop(df_old[column])
-
         writer_format = df_writer.write.format(type_format)
 
         if bool(format_properties):
             writer_format = self.__define_properties(
                 writer_format, type_format, url, format_properties
             )
 
         if mode is not None:
             writer_format = writer_format.mode(mode)
 
-        self.__define_save(writer_format, type_format, url)
+        self.__define_save(writer_format, type_format, url) 
 
         return df_writer
```

### Comparing `sefazetllib-0.1.24/sefazetllib/factory/platform/PlatformFactory.py` & `sefazetllib-0.1.25/sefazetllib/factory/platform/PlatformFactory.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/load/Load.py` & `sefazetllib-0.1.25/sefazetllib/load/Load.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/load/LoadLocal.py` & `sefazetllib-0.1.25/sefazetllib/load/LoadLocal.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/load/LoadS3.py` & `sefazetllib-0.1.25/sefazetllib/load/LoadS3.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     schema: str = field(default="")
     entity: str = field(default="")
     mode: str = field(default="")
     df_writer: Any = field(default="")
     duplicates: bool = field(default=False)
     key: Key = field(default=DefaultKey())
     columns: List = field(default_factory=list)
+    load_date: bool = field(default=True)
 
     def build_connection_string(self):
         self.url = f"s3a://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
         return self.url
 
     def execute(self, **kwargs):
         if isinstance(self.platform, Default):
@@ -62,9 +63,10 @@
                 key=self.key,
                 columns=self.columns,
                 duplicates=self.duplicates,
                 file_format=self.file_format,
                 format_properties=self.format_properties,
                 url=url,
                 mode=self.mode,
+                load_date=self.load_date,
             ),
         )
```

### Comparing `sefazetllib-0.1.24/sefazetllib/load/LoadSQL.py` & `sefazetllib-0.1.25/sefazetllib/load/LoadStorage.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,67 @@
 from typing import Any, Dict, List
 
 from sefazetllib.Builder import Builder, field
 from sefazetllib.factory.platform.dataframe.Default import Default
 from sefazetllib.factory.platform.Platform import Platform
-from sefazetllib.factory.platform.PlatformFactory import PlatformFactory
 from sefazetllib.load.Load import Load
 from sefazetllib.utils.key import DefaultKey, Key
 
 
 @Builder
-class LoadSQL(Load):
+class LoadStorage(Load):
     platform: Platform = field(default=Default())
-    format: str = field(default="jdbc")
-    operator: str = field(default=":")
-    host: str = field(default="")
-    port: int = field(default=0)
-    database: str = field(default="")
-    instance: str = field(default="")
-    driver: str = field(default="")
-    schema: str = field(default="")
-    table: str = field(default="")
-    authentication: Dict[str, Any] = field(default_factory=dict)
-    url: str = field(default="")
+    file_format: str = field(default="")
+    format_properties: Dict[str, Any] = field(default_factory=dict)
     reference: str = field(default="")
-    df_writer: Any = field(default="")
+    url: str = field(default="")
+    repository: str = field(default="")
+    layer: str = field(default="")
+    schema: str = field(default="")
+    entity: str = field(default="")
     mode: str = field(default="")
-    key: Key = field(default=DefaultKey())
-    columns: List[str] = field(default_factory=list)
-    operation: bool = field(default=False)
-    optional: bool = field(default=False)
+    df_writer: Any = field(default="")
     duplicates: bool = field(default=False)
-
-    def __build_properties(self):
-        return {
-            "operation": self.operation,
-            "database": self.database,
-            "driver": self.driver,
-            "user": self.authentication["user"],
-            "password": self.authentication["password"],
-            "dbtable": self.table,
-            "url": self.url,
-        }
+    key: Key = field(default=DefaultKey())
+    columns: List = field(default_factory=list)
+    protocol: str = field(default="")
 
     def build_connection_string(self):
-        platform_db = PlatformFactory(self.database).create(
-            name="get url jdbc",
-        )
-        self.url = platform_db.get_url(
-            format=self.format,
-            operator=self.operator,
-            database=self.database,
-            host=self.host,
-            instance=self.instance,
-            schema=self.schema,
-            port=self.port,
-        )
-
-        self.table = platform_db.get_table_name(table=self.table, schema=self.schema)
+        self.url = f"{self.protocol}://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
+        return self.url
 
     def execute(self, **kwargs):
         if isinstance(self.platform, Default):
             self.setPlatform(kwargs["platform"])
 
-        sk_name = f"SK_{self.table}"
-        if "/" in self.table:
-            table = self.table.split("/")[1]
-            sk_name = f"SK_{table}"
-
-        self.build_connection_string()
-
-        return self.reference, self.platform.load(
-            df=self.df_writer,
-            sk_name=sk_name,
-            key=self.key,
-            columns=self.columns,
-            duplicates=self.duplicates,
-            format=self.format,
-            format_properties=self.__build_properties(),
-            url=None,
-            mode=self.mode,
+        if self.repository == "":
+            self.setRepository(kwargs["repository"])
+
+        url = self.build_connection_string()
+
+        if kwargs:
+            args = kwargs["args"]
+            if args.loadRepository:
+                self.setRepository(args.loadRepository)
+
+            if args.loadUrl:
+                url = args.loadUrl
+
+        sk_name = f"SK_{self.entity}"
+        if "/" in self.entity:
+            entity = self.entity.split("/")[1]
+            sk_name = f"SK_{entity}"
+
+        return (
+            self.reference,
+            self.platform.load(
+                df=self.df_writer,
+                sk_name=sk_name,
+                key=self.key,
+                columns=self.columns,
+                duplicates=self.duplicates,
+                file_format=self.file_format,
+                format_properties=self.format_properties,
+                url=url,
+                mode=self.mode,
+            ),
         )
```

### Comparing `sefazetllib-0.1.24/sefazetllib/transform/MinMaxLineTransform.py` & `sefazetllib-0.1.25/sefazetllib/transform/MinMaxLineTransform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/transform/QuartileTransform.py` & `sefazetllib-0.1.25/sefazetllib/transform/QuartileTransform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/transform/Transform.py` & `sefazetllib-0.1.25/sefazetllib/transform/Transform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/utils/key/SurrogateKey.py` & `sefazetllib-0.1.25/sefazetllib/utils/key/SurrogateKey.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/utils/partition/DatePartition.py` & `sefazetllib-0.1.25/sefazetllib/utils/partition/DatePartition.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/utils/partition/IncrementalRangePartition.py` & `sefazetllib-0.1.25/sefazetllib/utils/partition/IncrementalRangePartition.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllib/validate/DataValidate.py` & `sefazetllib-0.1.25/sefazetllib/validate/DataValidate.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/__init__.py` & `sefazetllib-0.1.25/sefazetllibcli/__init__.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/config/logging.py` & `sefazetllib-0.1.25/sefazetllibcli/config/logging.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/generators/etl_generator.py` & `sefazetllib-0.1.25/sefazetllibcli/generators/etl_generator.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/generators/generator.py` & `sefazetllib-0.1.25/sefazetllibcli/generators/generator.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/__init__.py` & `sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_etl_variable.py` & `sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_etl_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_extract_variable.py` & `sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_extract_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_imports_variable.py` & `sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_imports_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_key_variable.py` & `sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_key_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_load_variable.py` & `sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_load_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_partition_variable.py` & `sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_partition_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_transforms_variable.py` & `sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_transforms_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_validate_variable.py` & `sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_validate_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/usecases/process_variable/process_variable.py` & `sefazetllib-0.1.25/sefazetllibcli/usecases/process_variable/process_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/usecases/replace_template/replace_etl_template.py` & `sefazetllib-0.1.25/sefazetllibcli/usecases/replace_template/replace_etl_template.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/usecases/replace_template/replace_template.py` & `sefazetllib-0.1.25/sefazetllibcli/usecases/replace_template/replace_template.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/sefazetllibcli/utils/parse_etl.py` & `sefazetllib-0.1.25/sefazetllibcli/utils/parse_etl.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.24/setup.py` & `sefazetllib-0.1.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
  'pyyaml>=6.0,<7.0']
 
 entry_points = \
 {'console_scripts': ['sefazetllib = sefazetllibcli:cli']}
 
 setup_kwargs = {
     'name': 'sefazetllib',
-    'version': '0.1.24',
+    'version': '0.1.25',
     'description': 'sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.',
     'long_description': '# sefazetllib\n\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n---\n\n**Documentation**: [https://main.d32to2oidohzrl.amplifyapp.com/](https://main.d32to2oidohzrl.amplifyapp.com/)\n\n**Source code**: [AWS CodeCommit](https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1)\n\n---\n\n**sefazetllib** is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.\n\n## Features\n\n- Easy to use and understand library for constructing ETL/ELT pipelines.\n- Compatibility with popular data processing frameworks, such as [pandas](https://pandas.pydata.org/) and [PySpark](https://spark.apache.org/).\n- Support for file formats such as CSV and Parquet.\n- Provides the ability to extract, transform and load data with customizable configurations.\n\n## Requirements\n\n**sefazetllib** requires the following to run:\n\n- [Python](https://www.python.org/) 3.7.1+\n- [pandas](https://pandas.pydata.org/) 1.3+\n- [PyArrow](https://arrow.apache.org/) 6.0+\n- [PySpark](https://spark.apache.org/) 3.0+\n- [PyDeequ](https://pydeequ.readthedocs.io/) 1.0+\n- [Boto3](https://github.com/boto/boto3) 1.24+\n\n## Installation\n\nUse [pip](https://pip.pypa.io/en/stable/) to install **sefazetllib**:\n\n```bash\npip install sefazetllib\n```\n\n## Usage\n\nHere is an example of how to use the **sefazetllib**:\n\n```Python\nfrom typing import Tuple\n\nfrom pandas import DataFrame\n\nfrom sefazetllib import Builder\nfrom sefazetllib.etl import ETL\nfrom sefazetllib.extract import ExtractLocal\nfrom sefazetllib.factory.platform import PlatformFactory\nfrom sefazetllib.load import LoadLocal\nfrom sefazetllib.transform import Transform\nfrom sefazetllib.utils.key import SurrogateKey\n\n\n@Builder\nclass TestingDataFrame(Transform):\n    def execute(self) -> Tuple[str, DataFrame]:\n        return (\n            "dataframe",\n            DataFrame(\n                [["tom", 10], ["nick", 15], ["juli", 14]], columns=["Name", "Age"]\n            ),\n        )\n\n\n(\n    ETL()\n    .setPlatform(PlatformFactory("Pandas").create(name="test_pandas"))\n    .transform(TestingDataFrame)\n    .load(\n        LoadLocal()\n        .setFileFormat("parquet")\n        .setEntity("load_test")\n        .setMode("overwrite")\n        .setReference("dataframe")\n        .setDuplicates(True)\n        .setKey(SurrogateKey().setColumns(["Name", "Age"]).setDistribute(False))\n    )\n    .extract(\n        ExtractLocal()\n        .setFileFormat("parquet")\n        .setUrl("load_test.parquet")\n        .setReference("extract_test")\n    )\n)\n```\n\n## Testing\n\nTo run the unit tests, run the following command:\n\n```bash\npy -m unittest tests/main.py -v\n```\n\n## License\n\n**sefazetllib** is released under the [Apache-2.0](/LICENSE).\n',
     'author': 'Felipe Gochi',
     'author_email': 'felipe.gochi@elogroup.com.br',
     'maintainer': 'Bruno Santos',
     'maintainer_email': 'bruno.santos@elogroup.com.br',
     'url': 'https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1',
```

### Comparing `sefazetllib-0.1.24/PKG-INFO` & `sefazetllib-0.1.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sefazetllib
-Version: 0.1.24
+Version: 0.1.25
 Summary: sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.
 Home-page: https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1
 License: Apache-2.0
 Author: Felipe Gochi
 Author-email: felipe.gochi@elogroup.com.br
 Maintainer: Bruno Santos
 Maintainer-email: bruno.santos@elogroup.com.br
```

