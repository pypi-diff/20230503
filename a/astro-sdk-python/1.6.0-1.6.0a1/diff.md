# Comparing `tmp/astro-sdk-python-1.6.0.tar.gz` & `tmp/astro-sdk-python-1.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-sdk-python-1.6.0.tar", last modified: Wed May  3 19:09:09 2023, max compression
+gzip compressed data, was "astro-sdk-python-1.6.0a1.tar", last modified: Fri Apr 21 19:05:24 2023, max compression
```

## Comparing `astro-sdk-python-1.6.0.tar` & `astro-sdk-python-1.6.0a1.tar`

### file list

```diff
@@ -1,94 +1,93 @@
-lrwxr-xr-x   0        0        0        0 2023-05-03 19:08:50.470633 astro-sdk-python-1.6.0/LICENSE -> ../LICENSE
--rw-r--r--   0        0        0     8344 2023-05-03 19:08:50.470633 astro-sdk-python-1.6.0/README.md
--rw-r--r--   0        0        0     5401 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      685 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/airflow/__init__.py
--rw-r--r--   0        0        0     1605 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/airflow/datasets.py
--rw-r--r--   0        0        0     2256 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/constants.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/custom_backend/__init__.py
--rw-r--r--   0        0        0     2187 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/custom_backend/astro_custom_backend.py
--rw-r--r--   0        0        0     3915 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/custom_backend/serializer.py
--rw-r--r--   0        0        0     1876 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/databases/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/databases/aws/__init__.py
--rw-r--r--   0        0        0    18189 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/databases/aws/redshift.py
--rw-r--r--   0        0        0    37127 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/databases/base.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/databases/databricks/__init__.py
--rw-r--r--   0        0        0     7247 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/databases/databricks/api_utils.py
--rw-r--r--   0        0        0    17788 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/databases/databricks/delta.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/databases/databricks/load_file/__init__.py
--rw-r--r--   0        0        0      720 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2
--rw-r--r--   0        0        0      647 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2
--rw-r--r--   0        0        0      913 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2
--rw-r--r--   0        0        0      512 2023-05-03 19:08:50.486633 astro-sdk-python-1.6.0/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2
--rw-r--r--   0        0        0     6368 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/databases/databricks/load_file/load_file_job.py
--rw-r--r--   0        0        0      880 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/databases/databricks/load_file/load_file_python_code_generator.py
--rw-r--r--   0        0        0     2687 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/databases/databricks/load_options.py
--rw-r--r--   0        0        0     6181 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/databases/duckdb.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/databases/google/__init__.py
--rw-r--r--   0        0        0    26823 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/databases/google/bigquery.py
--rw-r--r--   0        0        0    17049 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/databases/mssql.py
--rw-r--r--   0        0        0     9267 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/databases/mysql.py
--rw-r--r--   0        0        0    10678 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/databases/postgres.py
--rw-r--r--   0        0        0    42201 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/databases/snowflake.py
--rw-r--r--   0        0        0     6508 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/databases/sqlite.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/dataframes/__init__.py
--rw-r--r--   0        0        0     4116 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/dataframes/load_options.py
--rw-r--r--   0        0        0     2356 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/dataframes/pandas.py
--rw-r--r--   0        0        0     1267 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/exceptions.py
--rw-r--r--   0        0        0     1096 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/__init__.py
--rw-r--r--   0        0        0    10151 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/base.py
--rw-r--r--   0        0        0     1535 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/locations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/locations/amazon/__init__.py
--rw-r--r--   0        0        0     3605 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/locations/amazon/s3.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/locations/azure/__init__.py
--rw-r--r--   0        0        0     5867 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/locations/azure/wasb.py
--rw-r--r--   0        0        0     6601 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/locations/base.py
--rw-r--r--   0        0        0     2374 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/locations/ftp.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/locations/google/__init__.py
--rw-r--r--   0        0        0     4420 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/locations/google/gcs.py
--rw-r--r--   0        0        0     5006 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/locations/google/gdrive.py
--rw-r--r--   0        0        0     1303 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/locations/http.py
--rw-r--r--   0        0        0     1531 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/locations/local.py
--rw-r--r--   0        0        0     3267 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/locations/sftp.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/operators/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/operators/files.py
--rw-r--r--   0        0        0     2576 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/types/__init__.py
--rw-r--r--   0        0        0     1504 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/types/base.py
--rw-r--r--   0        0        0     1900 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/types/csv.py
--rw-r--r--   0        0        0     2197 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/types/json.py
--rw-r--r--   0        0        0     3652 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/types/ndjson.py
--rw-r--r--   0        0        0     2848 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/files/types/parquet.py
--rw-r--r--   0        0        0      700 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/lineage/__init__.py
--rw-r--r--   0        0        0     4264 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/lineage/facets.py
--rw-r--r--   0        0        0     3910 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/options.py
--rw-r--r--   0        0        0     1117 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/query_modifier.py
--rw-r--r--   0        0        0     3869 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/settings.py
--rw-r--r--   0        0        0     3194 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/__init__.py
--rw-r--r--   0        0        0     7857 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/append.py
--rw-r--r--   0        0        0    18419 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/base_decorator.py
--rw-r--r--   0        0        0      334 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/base_operator.py
--rw-r--r--   0        0        0    12688 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/cleanup.py
--rw-r--r--   0        0        0     7870 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/data_validations/check_column.py
--rw-r--r--   0        0        0     3696 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/data_validations/check_table.py
--rw-r--r--   0        0        0    15362 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/dataframe.py
--rw-r--r--   0        0        0     1435 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/drop.py
--rw-r--r--   0        0        0     2693 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/export_file.py
--rw-r--r--   0        0        0     2715 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/export_table_to_file.py
--rw-r--r--   0        0        0     7035 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/export_to_file.py
--rw-r--r--   0        0        0    17274 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/load_file.py
--rw-r--r--   0        0        0     8824 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/merge.py
--rw-r--r--   0        0        0     9898 2023-05-03 19:08:50.490633 astro-sdk-python-1.6.0/src/astro/sql/operators/raw_sql.py
--rw-r--r--   0        0        0     7393 2023-05-03 19:08:50.494633 astro-sdk-python-1.6.0/src/astro/sql/operators/transform.py
--rw-r--r--   0        0        0      880 2023-05-03 19:08:50.494633 astro-sdk-python-1.6.0/src/astro/sql/operators/upstream_task_mixin.py
--rw-r--r--   0        0        0      160 2023-05-03 19:08:50.494633 astro-sdk-python-1.6.0/src/astro/sql/table.py
--rw-r--r--   0        0        0     8747 2023-05-03 19:08:50.494633 astro-sdk-python-1.6.0/src/astro/table.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.494633 astro-sdk-python-1.6.0/src/astro/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 19:08:50.494633 astro-sdk-python-1.6.0/src/astro/utils/compat/__init__.py
--rw-r--r--   0        0        0      359 2023-05-03 19:08:50.494633 astro-sdk-python-1.6.0/src/astro/utils/compat/functools.py
--rw-r--r--   0        0        0      843 2023-05-03 19:08:50.494633 astro-sdk-python-1.6.0/src/astro/utils/compat/typing.py
--rw-r--r--   0        0        0     2022 2023-05-03 19:08:50.494633 astro-sdk-python-1.6.0/src/astro/utils/dataframe.py
--rw-r--r--   0        0        0     1581 2023-05-03 19:08:50.494633 astro-sdk-python-1.6.0/src/astro/utils/load.py
--rw-r--r--   0        0        0     2790 2023-05-03 19:08:50.494633 astro-sdk-python-1.6.0/src/astro/utils/path.py
--rw-r--r--   0        0        0     4025 2023-05-03 19:08:50.494633 astro-sdk-python-1.6.0/src/astro/utils/table.py
--rw-r--r--   0        0        0    13464 1970-01-01 00:00:00.000000 astro-sdk-python-1.6.0/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-04-21 19:05:11.619546 astro-sdk-python-1.6.0a1/LICENSE -> ../LICENSE
+-rw-r--r--   0        0        0     8344 2023-04-21 19:05:11.619546 astro-sdk-python-1.6.0a1/README.md
+-rw-r--r--   0        0        0     5313 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/pyproject.toml
+-rw-r--r--   0        0        0      687 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/airflow/__init__.py
+-rw-r--r--   0        0        0     1605 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/airflow/datasets.py
+-rw-r--r--   0        0        0     2018 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/constants.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/custom_backend/__init__.py
+-rw-r--r--   0        0        0     2187 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/custom_backend/astro_custom_backend.py
+-rw-r--r--   0        0        0     3915 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/custom_backend/serializer.py
+-rw-r--r--   0        0        0     1876 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/aws/__init__.py
+-rw-r--r--   0        0        0    18189 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/aws/redshift.py
+-rw-r--r--   0        0        0    37127 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/base.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/__init__.py
+-rw-r--r--   0        0        0     7247 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/api_utils.py
+-rw-r--r--   0        0        0    17788 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/delta.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/__init__.py
+-rw-r--r--   0        0        0      720 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2
+-rw-r--r--   0        0        0      647 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2
+-rw-r--r--   0        0        0      913 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2
+-rw-r--r--   0        0        0      512 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2
+-rw-r--r--   0        0        0     6287 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/load_file_job.py
+-rw-r--r--   0        0        0      880 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/load_file_python_code_generator.py
+-rw-r--r--   0        0        0     2687 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_options.py
+-rw-r--r--   0        0        0     6181 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/duckdb.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/google/__init__.py
+-rw-r--r--   0        0        0    26823 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/google/bigquery.py
+-rw-r--r--   0        0        0    17049 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/databases/mssql.py
+-rw-r--r--   0        0        0    10678 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/databases/postgres.py
+-rw-r--r--   0        0        0    42201 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/databases/snowflake.py
+-rw-r--r--   0        0        0     6508 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/databases/sqlite.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/dataframes/__init__.py
+-rw-r--r--   0        0        0     4116 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/dataframes/load_options.py
+-rw-r--r--   0        0        0     1977 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/dataframes/pandas.py
+-rw-r--r--   0        0        0     1137 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/exceptions.py
+-rw-r--r--   0        0        0     1096 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/__init__.py
+-rw-r--r--   0        0        0    10151 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/base.py
+-rw-r--r--   0        0        0     1535 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/amazon/__init__.py
+-rw-r--r--   0        0        0     3605 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/amazon/s3.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/azure/__init__.py
+-rw-r--r--   0        0        0     4290 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/azure/wasb.py
+-rw-r--r--   0        0        0     6355 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/base.py
+-rw-r--r--   0        0        0     2374 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/ftp.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/google/__init__.py
+-rw-r--r--   0        0        0     4420 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/google/gcs.py
+-rw-r--r--   0        0        0     5006 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/google/gdrive.py
+-rw-r--r--   0        0        0     1303 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/http.py
+-rw-r--r--   0        0        0     1531 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/local.py
+-rw-r--r--   0        0        0     3267 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/sftp.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/operators/__init__.py
+-rw-r--r--   0        0        0     1595 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/operators/files.py
+-rw-r--r--   0        0        0     2576 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/__init__.py
+-rw-r--r--   0        0        0     1504 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/base.py
+-rw-r--r--   0        0        0     1900 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/csv.py
+-rw-r--r--   0        0        0     2197 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/json.py
+-rw-r--r--   0        0        0     3652 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/ndjson.py
+-rw-r--r--   0        0        0     2848 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/parquet.py
+-rw-r--r--   0        0        0      700 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/lineage/__init__.py
+-rw-r--r--   0        0        0     4264 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/lineage/facets.py
+-rw-r--r--   0        0        0     3910 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/options.py
+-rw-r--r--   0        0        0     1117 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/query_modifier.py
+-rw-r--r--   0        0        0     3791 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/settings.py
+-rw-r--r--   0        0        0     3194 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/__init__.py
+-rw-r--r--   0        0        0     7857 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/append.py
+-rw-r--r--   0        0        0    18379 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/base_decorator.py
+-rw-r--r--   0        0        0      334 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/base_operator.py
+-rw-r--r--   0        0        0    11280 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/cleanup.py
+-rw-r--r--   0        0        0     7870 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/data_validations/check_column.py
+-rw-r--r--   0        0        0     3696 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/data_validations/check_table.py
+-rw-r--r--   0        0        0    15366 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/dataframe.py
+-rw-r--r--   0        0        0     1435 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/drop.py
+-rw-r--r--   0        0        0     2693 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_file.py
+-rw-r--r--   0        0        0     2715 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_table_to_file.py
+-rw-r--r--   0        0        0     7035 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_to_file.py
+-rw-r--r--   0        0        0    17274 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/load_file.py
+-rw-r--r--   0        0        0     8824 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/merge.py
+-rw-r--r--   0        0        0     9902 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/raw_sql.py
+-rw-r--r--   0        0        0     7401 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/transform.py
+-rw-r--r--   0        0        0      880 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/upstream_task_mixin.py
+-rw-r--r--   0        0        0      160 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/table.py
+-rw-r--r--   0        0        0     8098 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/table.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/compat/__init__.py
+-rw-r--r--   0        0        0      359 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/compat/functools.py
+-rw-r--r--   0        0        0      843 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/compat/typing.py
+-rw-r--r--   0        0        0     2022 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/dataframe.py
+-rw-r--r--   0        0        0     1581 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/load.py
+-rw-r--r--   0        0        0     2790 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/path.py
+-rw-r--r--   0        0        0     4025 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/table.py
+-rw-r--r--   0        0        0    13316 1970-01-01 00:00:00.000000 astro-sdk-python-1.6.0a1/PKG-INFO
```

### Comparing `astro-sdk-python-1.6.0/README.md` & `astro-sdk-python-1.6.0a1/README.md`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/pyproject.toml` & `astro-sdk-python-1.6.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -94,18 +94,14 @@
 databricks = ["databricks-cli",
     "apache-airflow-providers-databricks"]
 
 mssql = [
     "apache-airflow-providers-microsoft-mssql>=3.2",
 ]
 
-mysql = [
-    "apache-airflow-providers-mysql",
-]
-
 duckdb = [
     "airflow-provider-duckdb>=0.0.2",
 ]
 
 all = [
     "apache-airflow-providers-amazon",
     "apache-airflow-providers-google>=6.4.0",
@@ -125,15 +121,14 @@
     "s3fs",
     "protobuf<=3.20", # Google bigquery client require protobuf <= 3.20.0. We can remove the limitation when this limitation is removed
     "openlineage-airflow>=0.17.0",
     "apache-airflow-providers-microsoft-azure",
     "azure-storage-blob",
     "apache-airflow-providers-microsoft-mssql>=3.2",
     "airflow-provider-duckdb>=0.0.2",
-    "apache-airflow-providers-mysql"
 ]
 doc = [
     "myst-parser>=0.17",
     "sphinx>=4.4.0",
     "sphinx-autoapi==2.0.0", # Multiple FileType class (same name) import is broken in sphinx-autoapi 2.0.1
     "sphinx-rtd-theme"
 ]
```

### Comparing `astro-sdk-python-1.6.0/src/astro/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A decorator that allows users to run SQL queries natively in Airflow."""
 
-__version__ = "1.6.0"
+__version__ = "1.6.0a1"
 
 
 # This is needed to allow Airflow to pick up specific metadata fields it needs
 # for certain features. We recognize it's a bit unclean to define these in
 # multiple places, but at this point it's the only workaround if you'd like
 # your custom conn type to show up in the Airflow UI.
 def get_provider_info() -> dict:
```

### Comparing `astro-sdk-python-1.6.0/src/astro/airflow/datasets.py` & `astro-sdk-python-1.6.0a1/src/astro/airflow/datasets.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/constants.py` & `astro-sdk-python-1.6.0a1/src/astro/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import sys
 from enum import Enum
 
 # typing.Literal was only introduced in Python 3.8, and we support Python 3.7
 if sys.version_info >= (3, 8):
-    from typing import Any, Literal
+    from typing import Literal
 else:
     from typing_extensions import Literal
 
 DEFAULT_SCHEMA = "tmp_astro"
 DEFAULT_CHUNK_SIZE = 1000000
 PYPI_PROJECT_NAME = "astro-sdk-python"
 
@@ -40,36 +40,26 @@
     NDJSON = "ndjson"
     PARQUET = "parquet"
     # [END filetypes]
 
     def __str__(self) -> str:
         return self.value
 
-    def serialize(self) -> dict[str, Any]:
-        return {
-            "value": self.value,
-        }
-
-    @staticmethod
-    def deserialize(data: dict[str, Any], _: int):
-        return FileType(data["value"])
-
 
 class Database(Enum):
     # [START database]
     POSTGRES = "postgres"
     POSTGRESQL = "postgres"
     SQLITE = "sqlite"
     DELTA = "delta"
     BIGQUERY = "bigquery"
     SNOWFLAKE = "snowflake"
     REDSHIFT = "redshift"
     MSSQL = "mssql"
     DUCKDB = "duckdb"
-    MYSQL = "mysql"
     # [END database]
 
     def __str__(self) -> str:
         return self.value
 
 
 class DatabricksLoadMode(str, Enum):
```

### Comparing `astro-sdk-python-1.6.0/src/astro/custom_backend/astro_custom_backend.py` & `astro-sdk-python-1.6.0a1/src/astro/custom_backend/astro_custom_backend.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/custom_backend/serializer.py` & `astro-sdk-python-1.6.0a1/src/astro/custom_backend/serializer.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/aws/redshift.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/aws/redshift.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/base.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/databricks/api_utils.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/api_utils.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/databricks/delta.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/delta.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/databricks/load_file/load_file_job.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/load_file_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,15 @@
 )
 from astro.databases.databricks.load_options import DeltaLoadOptions
 from astro.files import File
 from astro.table import BaseTable
 
 cwd = pathlib.Path(__file__).parent
 
-supported_file_locations = [
-    FileLocation.LOCAL,
-    FileLocation.S3,
-    FileLocation.GS,
-    FileLocation.WASB,
-    FileLocation.WASBS,
-]
+supported_file_locations = [FileLocation.LOCAL, FileLocation.S3, FileLocation.GS]
 
 log = logging.getLogger(__file__)
 
 
 def load_file_to_delta(  # noqa: C901
     input_file: File,
     delta_table: BaseTable,
@@ -111,15 +105,15 @@
     if (
         databricks_options.load_mode == DatabricksLoadMode.AUTOLOADER
         and databricks_options.if_exists == "replace"
     ):
         databricks_options.autoloader_load_options["cloudFiles.allowOverwrites"] = "true"
 
     file_path = generate_file(
-        data_source_path=str(dbfs_file_path) if dbfs_file_path else input_file.location.databricks_uri,
+        data_source_path=str(dbfs_file_path) if dbfs_file_path else input_file.path,
         table_name=delta_table.name,
         source_type=str(input_file.location.location_type),
         output_file_path=Path(output_file.name),
         file_type=file_type or "",
         load_options=databricks_options,
     )
     dbfs_file_path = load_file_to_dbfs(
```

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/databricks/load_file/load_file_python_code_generator.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/load_file_python_code_generator.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/databricks/load_options.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/duckdb.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/google/bigquery.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/google/bigquery.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/mssql.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/mssql.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/mysql.py` & `astro-sdk-python-1.6.0a1/src/astro/table.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,237 +1,230 @@
 from __future__ import annotations
 
-import pandas as pd
-import sqlalchemy
-from airflow.exceptions import AirflowException
-from airflow.providers.mysql.hooks.mysql import MySqlHook
-from MySQLdb import OperationalError
-
-from astro.constants import DEFAULT_CHUNK_SIZE, LoadExistStrategy, MergeConflictStrategy
-from astro.databases.base import BaseDatabase
-from astro.options import LoadOptions
-from astro.settings import MYSQL_SCHEMA
-from astro.table import BaseTable, Metadata
-from astro.utils.compat.functools import cached_property
-
-DEFAULT_CONN_ID = MySqlHook.default_conn_name
-
-
-class MysqlDatabase(BaseDatabase):
-    DEFAULT_SCHEMA = MYSQL_SCHEMA
-
-    _create_schema_statement: str = (
-        "CREATE SCHEMA IF NOT EXISTS {} "
-        "DEFAULT CHARACTER SET = 'utf8' DEFAULT COLLATE = "
-        "'utf8_unicode_ci'"
+import random
+import string
+from typing import Any
+
+from attr import define, field, fields_dict
+from sqlalchemy import Column, MetaData
+
+from astro.airflow.datasets import Dataset
+from astro.databases import create_database
+from astro.settings import OPENLINEAGE_EMIT_TEMP_TABLE_EVENT
+
+MAX_TABLE_NAME_LENGTH = 62
+TEMP_PREFIX = "_tmp"
+
+
+@define
+class Metadata:
+    """
+    Contains additional information to access a SQL Table, which is very likely optional and, in some cases, may
+    be database-specific.
+
+    :param schema: A schema name
+    :param database: A database name
+    """
+
+    # This property is used by several databases, including: Postgres, Snowflake and BigQuery ("namespace")
+    schema: str | None = None
+    database: str | None = None
+
+    def is_empty(self) -> bool:
+        """Check if all the fields are None."""
+        return all(getattr(self, field_name) is None for field_name in fields_dict(self.__class__))
+
+
+@define(slots=False)
+class BaseTable:
+    """
+    Base class that has information necessary to access a SQL Table. It is agnostic to the database type.
+    If no name is given, it auto-generates a name for the Table and considers it temporary.
+
+    Temporary tables are prefixed with the prefix TEMP_PREFIX.
+
+    :param name: The name of the database table. If name not provided then it would create a temporary name
+    :param conn_id: The Airflow connection id. This will be used to identify the right database type at the runtime
+    :param metadata: A metadata object which will have database or schema name
+    :param columns: columns which define the database table schema.
+    :sphinx-autoapi-skip:
+    """
+
+    template_fields = ("name",)
+
+    # TODO: discuss alternative names to this class, since it contains metadata as opposed to be the
+    # SQL table itself
+    # Some ideas: TableRef, TableMetadata, TableData, TableDataset
+    name: str = field(default="")
+    conn_id: str = field(default="")
+    # Setting converter allows passing a dictionary to metadata arg
+    metadata: Metadata = field(
+        factory=Metadata,
+        converter=lambda val: Metadata(**val) if isinstance(val, dict) else val,
     )
+    columns: list[Column] = field(factory=list)
+    temp: bool = field(default=False)
 
-    def __init__(
-        self,
-        conn_id: str = DEFAULT_CONN_ID,
-        table: BaseTable | None = None,
-        load_options: LoadOptions | None = None,
-    ):
-        super().__init__(conn_id)
-        self.table = table
-        self.load_options = load_options
-
-    @cached_property
-    def hook(self) -> MySqlHook:
-        """Retrieve Airflow hook to interface with the mysql database."""
-        conn = MySqlHook(mysql_conn_id=self.conn_id).get_connection(self.conn_id)
-        kwargs = {}
-        if conn.schema is None:
-            if (
-                self.table
-                and self.table.metadata
-                and self.table.metadata.database
-                and self.table.metadata.schema
-            ):
-                raise AirflowException(
-                    "You have provided both database and schema in Metadata."
-                    "Enter only schema while connecting to MySQL!"
-                )
-            if (
-                self.table
-                and self.table.metadata
-                and self.table.metadata.database
-                and self.table.metadata.schema is None
-            ):
-                raise AirflowException(
-                    "You have provided database in Metadata.Enter only schema while connecting to MySQL!"
-                )
-            if self.table and self.table.metadata and self.table.metadata.schema:
-                kwargs.update({"schema": self.table.metadata.schema})
-            else:
-                kwargs.update({"schema": self.DEFAULT_SCHEMA})
-        return MySqlHook(mysql_conn_id=self.conn_id, **kwargs)
-
-    def populate_table_metadata(self, table: BaseTable) -> BaseTable:
-        """
-        Given a table, check if the table has metadata.
-        If the metadata is missing, and the database has metadata, assign it to the table.
-        If the table schema was not defined by the end, retrieve the user-defined schema.
-        This method performs the changes in-place and also returns the table.
-        For mysql - schema is synonymous with database.
-
-        :param table: Table to potentially have their metadata changed
-        :return table: Return the modified table
-        """
-        if table.metadata and table.metadata.is_empty() and self.default_metadata:
-            table.metadata = self.default_metadata
-        return table
-
-    @property
-    def default_metadata(self) -> Metadata:
-        """schema and database are synonymous in MySQL"""
-        schema_from_conn = self.hook.get_connection(self.conn_id).schema
-        database = schema_from_conn if schema_from_conn else self.DEFAULT_SCHEMA
-        return Metadata(database=database, schema=database)  # type: ignore
-
-    def load_pandas_dataframe_to_table(
-        self,
-        source_dataframe: pd.DataFrame,
-        target_table: BaseTable,
-        if_exists: LoadExistStrategy = "replace",
-        chunk_size: int = DEFAULT_CHUNK_SIZE,
-    ) -> None:
-        """
-        Create a table with the dataframe's contents.
-        If the table already exists, append or replace the content, depending on the value of `if_exists`.
-
-        :param source_dataframe: Local or remote filepath
-        :param target_table: Table in which the file will be loaded
-        :param if_exists: Strategy to be used in case the target table already exists.
-        :param chunk_size: Specify the number of rows in each batch to be written at a time.
-        """
-        self._assert_not_empty_df(source_dataframe)
-
-        source_dataframe.to_sql(
-            self.get_table_qualified_name(target_table),
-            con=self.sqlalchemy_engine,
-            schema=target_table.metadata.schema,
-            if_exists=if_exists,
-            chunksize=chunk_size,
-            method="multi",
-            index=False,
+    def __attrs_post_init__(self) -> None:
+        if not self.name:
+            self.name = self._create_unique_table_name(TEMP_PREFIX + "_")
+            self.temp = True
+        if self.name.startswith(TEMP_PREFIX):
+            self.temp = True
+
+    # We need this method to pickle Table object, without this we cannot push/pull this object from xcom.
+    def __getstate__(self):
+        return self.__dict__
+
+    def _create_unique_table_name(self, prefix: str = "") -> str:
+        """
+        If a table is instantiated without a name, create a unique table for it.
+        This new name should be compatible with all supported databases.
+        """
+        schema_length = len((self.metadata and self.metadata.schema) or "") + 1
+        prefix_length = len(prefix)
+
+        unique_id = random.choice(string.ascii_lowercase) + "".join(
+            random.choice(string.ascii_lowercase + string.digits)
+            for _ in range(MAX_TABLE_NAME_LENGTH - schema_length - prefix_length)
         )
+        if prefix:
+            unique_id = f"{prefix}{unique_id}"
 
-    @property
-    def sql_type(self) -> str:
-        return "mysql"
-
-    def table_exists(self, table: BaseTable) -> bool:
-        """
-        Check if a table exists in the database
+        return unique_id
 
-        :param table: Details of the table we want to check that exists
+    def create_similar_table(self) -> Table:
         """
-        inspector = sqlalchemy.inspect(self.sqlalchemy_engine)
-
-        schema = None
-        if table and table.metadata:
-            schema = table.metadata.schema
-        return bool(inspector.dialect.has_table(self.connection, table.name, schema=schema))
-
-    def schema_exists(self, schema) -> bool:
+        Create a new table with a unique name but with the same metadata.
         """
-        Checks if a schema exists in the database
-
-        :param schema: DB Schema - a namespace that contains named objects like (tables, functions, etc)
-        """
-        try:
-            schema_result = self.hook.run(
-                "SELECT schema_name FROM information_schema.schemata WHERE "
-                "lower(schema_name) = lower(%(schema_name)s);",
-                parameters={"schema_name": schema.lower()},
-                handler=lambda x: [y[0] for y in x.fetchall()],
-            )
-            return len(schema_result) > 0
-        except OperationalError:
-            return False
+        return Table(  # type: ignore
+            name=self._create_unique_table_name(),
+            conn_id=self.conn_id,
+            metadata=self.metadata,
+        )
 
-    @staticmethod
-    def get_table_qualified_name(table: BaseTable) -> str:
-        """
-        Return the table qualified name.
+    @property
+    def sqlalchemy_metadata(self) -> MetaData:
+        """Return the Sqlalchemy metadata for the given table."""
+        if self.metadata and self.metadata.schema:
+            alchemy_metadata = MetaData(schema=self.metadata.schema)
+        else:
+            alchemy_metadata = MetaData()
+        return alchemy_metadata
 
-        :param table: The table we want to retrieve the qualified name for.
+    @property
+    def row_count(self) -> Any:
         """
-        return table.name
-
-    def merge_table(
-        self,
-        source_table: BaseTable,
-        target_table: BaseTable,
-        source_to_target_columns_map: dict[str, str],
-        target_conflict_columns: list[str],
-        if_conflicts: MergeConflictStrategy = "exception",
-    ) -> None:
+        Return the row count of table.
         """
-        Merge the source table rows into a destination table.
-        The argument `if_conflicts` allows the user to define how to handle conflicts.
+        db = create_database(self.conn_id)
+        return db.row_count(self)
 
-        :param source_table: Contains the rows to be merged to the target_table
-        :param target_table: Contains the destination table in which the rows will be merged
-        :param source_to_target_columns_map: Dict of target_table columns names to source_table columns names
-        :param target_conflict_columns: List of cols where we expect to have a conflict while combining
-        :param if_conflicts: The strategy to be applied if there are conflicts.
-        """
-        statement = (
-            "insert into {target_table}"
-            "({target_columns})  "
-            "select {source_columns} "
-            "from {source_table}  "
-            "on duplicate key update {merge_vals};"
-        )
-
-        source_column_names = list(source_to_target_columns_map.keys())
-        target_column_names = list(source_to_target_columns_map.values())
-
-        target_identifier_enclosure = ""
-        source_identifier_enclosure = ""
-
-        join_conditions = ",".join(
-            [
-                f"{target_table.name}.{target_identifier_enclosure}{t}{target_identifier_enclosure}="
-                f"{source_table.name}.{source_identifier_enclosure}{s}{source_identifier_enclosure}"
-                for s, t in source_to_target_columns_map.items()
-            ]
-        )
-        statement = statement.replace("{merge_vals}", join_conditions)
-
-        statement = statement.format(
-            target_columns=",".join(target_column_names),
-            target_table=target_table.name,
-            source_columns=",".join(source_column_names),
-            source_table=source_table.name,
+    @property
+    def sql_type(self) -> Any:
+        if self.conn_id:
+            return create_database(self.conn_id).sql_type
+
+    def to_json(self):
+        return {
+            "class": "Table",
+            "name": self.name,
+            "metadata": {
+                "schema": self.metadata.schema,
+                "database": self.metadata.database,
+            },
+            "temp": self.temp,
+            "conn_id": self.conn_id,
+        }
+
+    @classmethod
+    def from_json(cls, obj: dict):
+        return Table(
+            name=obj["name"],
+            metadata=Metadata(**obj["metadata"]),
+            temp=obj["temp"],
+            conn_id=obj["conn_id"],
         )
 
-        self.run_sql(sql=statement)
-
-    def openlineage_dataset_name(self, table: BaseTable) -> str:
+    def openlineage_dataset_name(self) -> str:
         """
         Returns the open lineage dataset name as per
         https://github.com/OpenLineage/OpenLineage/blob/main/spec/Naming.md
-        Example: database.schema.table.name
         """
-        schema = self.hook.get_connection(self.conn_id).schema
-        if table.metadata and table.metadata.schema:
-            schema = table.metadata.schema
-        return f"{schema}.{table.name}"
+        database = create_database(self.conn_id)
+        return database.openlineage_dataset_name(table=self)
 
     def openlineage_dataset_namespace(self) -> str:
         """
         Returns the open lineage dataset namespace as per
         https://github.com/OpenLineage/OpenLineage/blob/main/spec/Naming.md
-        Example: mssql://localhost:3306
         """
-        conn = self.hook.get_connection(self.conn_id)
-        return f"{self.sql_type}://{conn.host}:{conn.port}"
+        database = create_database(self.conn_id)
+        return database.openlineage_dataset_namespace()
 
-    def openlineage_dataset_uri(self, table: BaseTable) -> str:
+    def openlineage_dataset_uri(self) -> str:
         """
         Returns the open lineage dataset uri as per
         https://github.com/OpenLineage/OpenLineage/blob/main/spec/Naming.md
         """
-        return f"{self.openlineage_dataset_namespace()}/{self.openlineage_dataset_name(table=table)}"
+        database = create_database(self.conn_id)
+        return f"{database.openlineage_dataset_uri(table=self)}"
+
+    def openlineage_emit_temp_table_event(self):
+        """
+        Based on airflow config ```OPENLINEAGE_EMIT_TEMP_TABLE_EVENT``` value and table type
+        check whether to emit temp table event in openlineage or not
+        """
+        return (not isinstance(self, TempTable)) or (
+            isinstance(self, TempTable) and OPENLINEAGE_EMIT_TEMP_TABLE_EVENT
+        )
+
+
+@define(slots=False)
+class TempTable(BaseTable):
+    """
+    Internal class to represent a Temporary table
+
+    :sphinx-autoapi-skip:
+    """
+
+    temp: bool = field(default=True)
+
+
+@define(slots=False)
+class Table(BaseTable, Dataset):
+    """
+    User-facing class that has information necessary to access a SQL Table. It is agnostic to the database type.
+    If no name is given, it auto-generates a name for the Table and considers it temporary.
+
+    Temporary tables are prefixed with the prefix TEMP_PREFIX.
+
+    :param name: The name of the database table. If name not provided then it would create a temporary name
+    :param conn_id: The Airflow connection id. This will be used to identify the right database type at the runtime
+    :param metadata: A metadata object which will have database or schema name
+    :param columns: columns which define the database table schema.
+    """
+
+    uri: str = field(init=False, eq=False)
+    extra: dict | None = field(init=False, factory=dict)
+
+    def __new__(cls, *args, **kwargs):
+        name = kwargs.get("name") or args and args[0] or ""
+        temp = kwargs.get("temp", False)
+        if temp or (not name or name.startswith("_tmp")):
+            return TempTable(*args, **kwargs)
+        return super().__new__(cls)
+
+    @uri.default
+    def _path_to_dataset_uri(self) -> str:
+        """Build a URI to be passed to Dataset obj introduced in Airflow 2.4"""
+        from urllib.parse import urlencode, urlparse
+
+        path = f"astro://{self.conn_id}@"
+        db_extra = {"table": self.name}
+        if self.metadata.schema:
+            db_extra["schema"] = self.metadata.schema
+        if self.metadata.database:
+            db_extra["database"] = self.metadata.database
+        parsed_url = urlparse(url=path)
+        new_parsed_url = parsed_url._replace(query=urlencode(db_extra))
+        return new_parsed_url.geturl()
```

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/postgres.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/snowflake.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/databases/sqlite.py` & `astro-sdk-python-1.6.0a1/src/astro/databases/sqlite.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/dataframes/load_options.py` & `astro-sdk-python-1.6.0a1/src/astro/dataframes/load_options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/dataframes/pandas.py` & `astro-sdk-python-1.6.0a1/src/astro/dataframes/pandas.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import logging
 from typing import ClassVar
 
 from pandas import DataFrame, read_json
 
 from astro import settings
-from astro.exceptions import AstroSDKConfigError
 
 logger = logging.getLogger(__name__)
 
 
 class PandasDataframe(DataFrame):
     """Pandas-compatible dataframe class that can be serialized and deserialized into XCom by Airflow 2.5"""
 
@@ -18,32 +17,26 @@
 
     def serialize(self):
         # Store in the metadata DB if Dataframe < 100 kb
         df_size = self.memory_usage(deep=True).sum()
         if df_size < (settings.MAX_DATAFRAME_MEMORY_FOR_XCOM_DB * 1024):
             logger.info("Dataframe size: %s bytes. Storing it in Airflow's metadata DB", df_size)
             return {"data": self.to_json()}
-        elif settings.DATAFRAME_STORAGE_CONN_ID is not None:
+        else:
             # Avoid cyclic dependency
             from astro.utils.dataframe import convert_dataframe_to_file
 
             logger.info(
                 "Dataframe size: %s bytes. Storing it in Remote Storage (conn_id: %s | URL: %s)",
                 df_size,
                 settings.DATAFRAME_STORAGE_CONN_ID,
                 settings.DATAFRAME_STORAGE_URL,
             )
             return convert_dataframe_to_file(self).to_json()
 
-        raise AstroSDKConfigError(
-            "Dataframe size exceeds allowed limit for storing in Airflow's metadata DB. "
-            "Airflow config variable AIRFLOW__ASTRO_SDK__XCOM_STORAGE_CONN_ID needs to "
-            "be set for remote storage of the dataframe."
-        )
-
     @staticmethod
     def deserialize(data: dict, version: int):
         if version > 1:
             raise TypeError(f"version > {PandasDataframe.version}")
         if isinstance(data, dict) and data.get("class", "") == "File":
             # Avoid cyclic dependency
             from astro.files import File
```

### Comparing `astro-sdk-python-1.6.0/src/astro/exceptions.py` & `astro-sdk-python-1.6.0a1/src/astro/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,11 +20,7 @@
     Inappropriate argument value (of correct type) or attribute
     not found while running query. while running query
     """
 
 
 class PermissionNotSetError(Exception):
     """Raised if a permission to files present in locations are not accessible"""
-
-
-class AstroSDKConfigError(Exception):
-    """Raised if a configuration parameter required for Astro SDK is not set correctly"""
```

### Comparing `astro-sdk-python-1.6.0/src/astro/files/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/files/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/base.py` & `astro-sdk-python-1.6.0a1/src/astro/files/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/locations/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/locations/amazon/s3.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/amazon/s3.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/locations/base.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,23 +156,14 @@
         """Check if the file exists or not"""
         try:
             with smart_open.open(self.smartopen_uri, mode="r", transport_params=self.transport_params):
                 return True
         except OSError:
             return False
 
-    @property
-    def databricks_uri(self) -> str:
-        """
-        Return a Databricks compatible URI. In most scenarios, it will be self.path. An exception is Microsoft WASB.
-
-        :return: self.path
-        """
-        return self.path
-
     def databricks_auth_settings(self) -> dict:
         """
         Required settings to upload this file into databricks. Only needed for cloud storage systems
         like S3
         :return: A dictionary of settings keys to settings values
         """
         return {}
```

### Comparing `astro-sdk-python-1.6.0/src/astro/files/locations/ftp.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/ftp.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/locations/google/gcs.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/google/gcs.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/locations/google/gdrive.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/google/gdrive.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/locations/http.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/http.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/locations/local.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/local.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/locations/sftp.py` & `astro-sdk-python-1.6.0a1/src/astro/files/locations/sftp.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/operators/files.py` & `astro-sdk-python-1.6.0a1/src/astro/files/operators/files.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/types/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/files/types/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/types/base.py` & `astro-sdk-python-1.6.0a1/src/astro/files/types/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/types/csv.py` & `astro-sdk-python-1.6.0a1/src/astro/files/types/csv.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/types/json.py` & `astro-sdk-python-1.6.0a1/src/astro/files/types/json.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/types/ndjson.py` & `astro-sdk-python-1.6.0a1/src/astro/files/types/ndjson.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/files/types/parquet.py` & `astro-sdk-python-1.6.0a1/src/astro/files/types/parquet.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/lineage/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/lineage/facets.py` & `astro-sdk-python-1.6.0a1/src/astro/lineage/facets.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/options.py` & `astro-sdk-python-1.6.0a1/src/astro/options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/query_modifier.py` & `astro-sdk-python-1.6.0a1/src/astro/query_modifier.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/settings.py` & `astro-sdk-python-1.6.0a1/src/astro/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 SCHEMA = conf.get(SECTION_KEY, "sql_schema", fallback=DEFAULT_SCHEMA)
 POSTGRES_SCHEMA = conf.get(SECTION_KEY, "postgres_default_schema", fallback=SCHEMA)
 BIGQUERY_SCHEMA = conf.get(SECTION_KEY, "bigquery_default_schema", fallback=SCHEMA)
 SNOWFLAKE_SCHEMA = conf.get(SECTION_KEY, "snowflake_default_schema", fallback=SCHEMA)
 REDSHIFT_SCHEMA = conf.get(SECTION_KEY, "redshift_default_schema", fallback=SCHEMA)
 MSSQL_SCHEMA = conf.get(SECTION_KEY, "mssql_default_schema", fallback=SCHEMA)
-MYSQL_SCHEMA = conf.get(SECTION_KEY, "mysql_default_schema", fallback=SCHEMA)
 
 BIGQUERY_SCHEMA_LOCATION = conf.get(
     SECTION_KEY, "bigquery_dataset_location", fallback=DEFAULT_BIGQUERY_SCHEMA_LOCATION
 )
 
 LOAD_FILE_ENABLE_NATIVE_FALLBACK = conf.get(SECTION_KEY, "load_file_enable_native_fallback", fallback=False)
```

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/__init__.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/append.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/append.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/base_decorator.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/base_decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,14 @@
                 self.sql, self.parameters = returned_value
             else:
                 self.sql = returned_value
                 self.parameters = self.parameters or {}
         if self.sql.endswith(".sql"):
             with open(self.sql) as file:
                 self.sql = file.read().replace("\n", " ")
-        self.op_kwargs.pop("sql", None)
 
     def move_function_params_into_sql_params(self, context: dict) -> None:
         """
         Pulls values from the function op_args and op_kwargs and places them into
         parameters for SQLAlchemy to parse
 
         :param context: Airflow's Context dictionary used for rendering templates
```

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/cleanup.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/cleanup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from __future__ import annotations
 
 import time
 from datetime import timedelta
 from typing import Any
 
-from airflow import __version__ as airflow_version
 from airflow.decorators.base import get_unique_task_id
 from airflow.exceptions import AirflowException
 from airflow.models.baseoperator import BaseOperator
 from airflow.models.dagrun import DagRun
-from packaging import version
 
 try:
     # Airflow >= 2.3
     from airflow.models.mappedoperator import MappedOperator
 except ImportError:  # pragma: no cover
     # Airflow < 2.3
     MappedOperator = None
@@ -71,83 +69,54 @@
     :param retries: The number of retries that should be performed before failing the task.
         Very relevant if using a synchronous executor. The default is 3.
     :param retry_delay: Delay between running retries. Very relevant if using a synchronous executor.
         The default is 10s.
     :param run_sync_mode: Whether to wait for the DAG to finish or not. Set to True if you want
         to immediately clean all tables. Note that if you supply anything to `tables_to_cleanup`
         this argument is ignored.
-    :param skip_on_failure: Skip cleanup if any upstream task fails. Useful while debugging failed tasks,
-        to prevent temporary tables upstream from being deleted prematurely. The default is False.
     """
 
     template_fields = ("tables_to_cleanup",)
 
     def __init__(
         self,
         *,
         tables_to_cleanup: list[BaseTable] | None = None,
         task_id: str = "",
         retries: int = 3,
         retry_delay: timedelta = timedelta(seconds=10),
         run_sync_mode: bool = False,
-        skip_on_failure: bool = False,
         **kwargs,
     ):
         self.tables_to_cleanup = tables_to_cleanup or []
         self.run_immediately = run_sync_mode
-        self.skip_on_failure = skip_on_failure
         task_id = task_id or get_unique_task_id("cleanup")
 
         super().__init__(task_id=task_id, retries=retries, retry_delay=retry_delay, **kwargs)
 
     def execute(self, context: Context) -> None:
         self.log.info("Execute Cleanup")
         if not self.tables_to_cleanup:
             # tables not provided, attempt to either immediately run or wait for all other tasks to finish
             if not self.run_immediately:
                 self.wait_for_dag_to_finish(context)
             self.tables_to_cleanup = self.get_all_task_outputs(context=context)
-        if self.skip_on_failure:
-            task_instances = context["dag_run"].get_task_instances()
-            if self._has_task_failed(task_instances=task_instances):
-                return None
         temp_tables = filter_for_temp_tables(self.tables_to_cleanup)
         self.log.info(
             "Tables found for cleanup: %s",
             ",".join([t.name for t in temp_tables]),
         )
         for table in temp_tables:
             self.drop_table(table)
 
     def drop_table(self, table: BaseTable) -> None:
         db = create_database(conn_id=table.conn_id, table=table)
         self.log.info("Dropping table %s", table.name)
         db.drop_table(table)
 
-    def _has_task_failed(self, task_instances: list[TaskInstance]) -> bool:
-        """
-        Given a list of task instances, return True if at least one task has failed.
-
-        :param task_instances:
-        :return: boolean if at least one task besides this one has failed
-        """
-        failed_tasks = [
-            (ti.task_id, ti.state)
-            for ti in task_instances
-            if ti.task_id != self.task_id and ti.state == State.FAILED
-        ]
-        if failed_tasks:
-            self.log.info(
-                "skipping cleanup as the following tasks have failed: %s",
-                failed_tasks,
-            )
-            return True
-        else:
-            return False
-
     def _is_dag_running(self, task_instances: list[TaskInstance]) -> bool:
         """
         Given a list of task instances, determine whether the DAG (minus the current cleanup task) is still
         running.
 
         :param task_instances:
         :return: boolean to show if all tasks besides this one have completed
@@ -213,22 +182,19 @@
         executor: str = conf.get("core", "EXECUTOR")
         if job_id:
             executor = cls._get_executor_from_job_id(job_id) or executor
         return executor in ["SequentialExecutor", "DebugExecutor"]
 
     @staticmethod
     def _get_executor_from_job_id(job_id: int) -> str | None:
-        if version.parse(airflow_version) >= version.parse("2.6"):
-            from airflow.jobs.job import Job
-        else:
-            from airflow.jobs.base_job import BaseJob as Job
+        from airflow.jobs.base_job import BaseJob
         from airflow.utils.session import create_session
 
         with create_session() as session:
-            job = session.get(Job, job_id)
+            job = session.get(BaseJob, job_id)
         return job.executor_class if job else None
 
     def get_all_task_outputs(self, context: Context) -> list[BaseTable]:
         """
         In the scenario where we are not given a list of tasks to follow, we will want to gather all temporary tables
         To prevent scenarios where we grab objects that are not tables, we try to only follow up on SQL operators or
         the dataframe operator, as these are the operators that return temporary tables.
```

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/data_validations/check_column.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/data_validations/check_column.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/data_validations/check_table.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/data_validations/check_table.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/dataframe.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,18 +309,18 @@
     :param multiple_outputs: If set to True, the decorated function's return value will be unrolled to
         multiple XCom values. Dict will unroll to XCom values with its keys as XCom keys. Defaults to False.
     :param conn_id: Connection ID for the database you want to connect to. If you do
         not pass in a value for this object
         we can infer the connection ID from the first table passed into the python_callable function.
         (required if there are no table arguments)
     :param database: Database within the SQL instance you want to access. If left blank we will
-        default to the table.metadata.database in the first Table passed
+        default to the table.metatadata.database in the first Table passed
         to the function (required if there are no table arguments)
     :param schema: Schema within the SQL instance you want to access. If left blank we will
-        default to the table.metadata.schema in the first Table passed to the
+        default to the table.metatadata.schema in the first Table passed to the
         function (required if there are no table arguments)
     :param columns_names_capitalization: determines whether to convert all columns to lowercase/uppercase
         in the resulting dataframe
     :param if_exists: Overwrite when set to "replace" else "append"
     :param kwargs: Any keyword arguments supported by the BaseOperator is supported (e.g ``queue``, ``owner``)
     """
     kwargs.update(
```

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/drop.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/drop.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/export_file.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/export_table_to_file.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_table_to_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/export_to_file.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_to_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/load_file.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/load_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/merge.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/merge.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/raw_sql.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/raw_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,18 +198,18 @@
     :param python_callable: This parameter is filled in automatically when you use the transform function as a
         decorator. This is where the python function gets passed to the wrapping function
     :param conn_id: Connection ID for the database you want to connect to.
         If you do not pass in a value for this object we can infer the connection ID from the first table
         passed into the python_callable function. (required if there are no table arguments)
     :param parameters: parameters to pass into the SQL query
     :param database: Database within the SQL instance you want to access. If left blank we will default to the
-        table.metadata.database in the first Table passed to the function
+        table.metatadata.database in the first Table passed to the function
         (required if there are no table arguments)
     :param schema: Schema within the SQL instance you want to access. If left blank we will default to the
-        table.metadata.schema in the first Table passed to the function
+        table.metatadata.schema in the first Table passed to the function
         (required if there are no table arguments)
     :param handler: Handler function to process the result of the SQL query. For more information please consult
         https://docs.sqlalchemy.org/en/14/core/connections.html#sqlalchemy.engine.Result
     :param results_format: Format of the results returned by the SQL query. Overrides the handler, if provided.
     :param fail_on_empty: If True and a results_format is provided, raises an exception if the query returns no results.
     :param response_size: Used to trim the responses returned to avoid trashing the Airflow DB.
         The default value is -1, which means the response is not changed. Otherwise, if the response is a list,
```

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/transform.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,17 +104,17 @@
     :param python_callable: This parameter is filled in automatically when you use the transform function as a decorator
         This is where the python function gets passed to the wrapping function
     :param conn_id: Connection ID for the database you want to connect to. If you do not pass in a value for this object
         we can infer the connection ID from the first table passed into the python_callable function.
         (required if there are no table arguments)
     :param parameters: parameters to pass into the SQL query
     :param database: Database within the SQL instance you want to access. If left blank we will default to the
-        table.metadata.database in the first Table passed to the function (required if there are no table arguments)
+        table.metatadata.database in the first Table passed to the function (required if there are no table arguments)
     :param schema: Schema within the SQL instance you want to access. If left blank we will default to the
-        table.metadata.schema in the first Table passed to the function (required if there are no table arguments)
+        table.metatadata.schema in the first Table passed to the function (required if there are no table arguments)
     :param kwargs: Any keyword arguments supported by the BaseOperator is supported (e.g ``queue``, ``owner``)
     :return: Transform functions return a ``Table`` object that can be passed to future tasks.
         This table will be either an auto-generated temporary table,
         or will overwrite a table given in the `output_table` parameter.
     """
 
     kwargs.update(
@@ -149,17 +149,17 @@
     :param file_path: File path for the SQL file you would like to parse. Can be an absolute path, or you can use a
         relative path if the `template_searchpath` variable is set in your DAG
     :param conn_id: Connection ID for the database you want to connect to. If you do not pass in a value for this object
         we can infer the connection ID from the first table passed into the python_callable function.
         (required if there are no table arguments)
     :param parameters: parameters to pass into the SQL query
     :param database: Database within the SQL instance you want to access. If left blank we will default to the
-        table.metadata.database in the first Table passed to the function (required if there are no table arguments)
+        table.metatadata.database in the first Table passed to the function (required if there are no table arguments)
     :param schema: Schema within the SQL instance you want to access. If left blank we will default to the
-        table.metadata.schema in the first Table passed to the function (required if there are no table arguments)
+        table.metatadata.schema in the first Table passed to the function (required if there are no table arguments)
     :param kwargs: Any keyword arguments supported by the BaseOperator is supported (e.g ``queue``, ``owner``)
     :return: Transform functions return a ``Table`` object that can be passed to future tasks.
         This table will be either an auto-generated temporary table,
         or will overwrite a table given in the `output_table` parameter.
     """
 
     kwargs.update(
```

### Comparing `astro-sdk-python-1.6.0/src/astro/sql/operators/upstream_task_mixin.py` & `astro-sdk-python-1.6.0a1/src/astro/sql/operators/upstream_task_mixin.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/utils/compat/typing.py` & `astro-sdk-python-1.6.0a1/src/astro/utils/compat/typing.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/utils/dataframe.py` & `astro-sdk-python-1.6.0a1/src/astro/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/utils/load.py` & `astro-sdk-python-1.6.0a1/src/astro/utils/load.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/utils/path.py` & `astro-sdk-python-1.6.0a1/src/astro/utils/path.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/src/astro/utils/table.py` & `astro-sdk-python-1.6.0a1/src/astro/utils/table.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0/PKG-INFO` & `astro-sdk-python-1.6.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-sdk-python
-Version: 1.6.0
+Version: 1.6.0a1
 Summary: Astro SDK allows rapid and clean development of {Extract, Load, Transform} workflows using Python and SQL, powered by Apache Airflow.
 Keywords: airflow,provider,astronomer,sql,decorator,task flow,elt,etl,dag
 Author-email: Astronomer <humans@astronomer.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -40,15 +40,14 @@
 Requires-Dist: s3fs ; extra == "all"
 Requires-Dist: protobuf<=3.20 ; extra == "all"
 Requires-Dist: openlineage-airflow>=0.17.0 ; extra == "all"
 Requires-Dist: apache-airflow-providers-microsoft-azure ; extra == "all"
 Requires-Dist: azure-storage-blob ; extra == "all"
 Requires-Dist: apache-airflow-providers-microsoft-mssql>=3.2 ; extra == "all"
 Requires-Dist: airflow-provider-duckdb>=0.0.2 ; extra == "all"
-Requires-Dist: apache-airflow-providers-mysql ; extra == "all"
 Requires-Dist: apache-airflow-providers-amazon>=5.0.0 ; extra == "amazon"
 Requires-Dist: s3fs ; extra == "amazon"
 Requires-Dist: smart-open[s3]>=5.2.1 ; extra == "amazon"
 Requires-Dist: apache-airflow-providers-microsoft-azure ; extra == "azure"
 Requires-Dist: azure-storage-blob ; extra == "azure"
 Requires-Dist: smart-open[azure]>=5.2.1 ; extra == "azure"
 Requires-Dist: databricks-cli ; extra == "databricks"
@@ -61,15 +60,14 @@
 Requires-Dist: apache-airflow-providers-ftp>=3.0.0 ; extra == "ftp"
 Requires-Dist: smart-open>=5.2.1 ; extra == "ftp"
 Requires-Dist: protobuf<=3.20 ; extra == "google"
 Requires-Dist: apache-airflow-providers-google>=6.4.0 ; extra == "google"
 Requires-Dist: sqlalchemy-bigquery>=1.3.0 ; extra == "google"
 Requires-Dist: smart-open[gcs]>=5.2.1 ; extra == "google"
 Requires-Dist: apache-airflow-providers-microsoft-mssql>=3.2 ; extra == "mssql"
-Requires-Dist: apache-airflow-providers-mysql ; extra == "mysql"
 Requires-Dist: openlineage-airflow>=0.17.0 ; extra == "openlineage"
 Requires-Dist: apache-airflow-providers-postgres ; extra == "postgres"
 Requires-Dist: apache-airflow-providers-sftp>=4.0.0 ; extra == "sftp"
 Requires-Dist: smart-open[ssh]>=5.2.1 ; extra == "sftp"
 Requires-Dist: apache-airflow-providers-snowflake ; extra == "snowflake"
 Requires-Dist: snowflake-sqlalchemy>=1.2.0 ; extra == "snowflake"
 Requires-Dist: snowflake-connector-python[pandas]<3.0.0 ; extra == "snowflake"
@@ -90,15 +88,14 @@
 Provides-Extra: azure
 Provides-Extra: databricks
 Provides-Extra: doc
 Provides-Extra: duckdb
 Provides-Extra: ftp
 Provides-Extra: google
 Provides-Extra: mssql
-Provides-Extra: mysql
 Provides-Extra: openlineage
 Provides-Extra: postgres
 Provides-Extra: sftp
 Provides-Extra: snowflake
 Provides-Extra: tests
 
 <h1 align="center">
```

