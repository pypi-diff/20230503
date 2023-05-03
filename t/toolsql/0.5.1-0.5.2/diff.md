# Comparing `tmp/toolsql-0.5.1.tar.gz` & `tmp/toolsql-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolsql-0.5.1.tar", last modified: Sat Apr 15 22:59:01 2023, max compression
+gzip compressed data, was "toolsql-0.5.2.tar", last modified: Wed May  3 18:28:20 2023, max compression
```

## Comparing `toolsql-0.5.1.tar` & `toolsql-0.5.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0       97 2023-01-27 20:52:41.456006 toolsql-0.5.1/.gitignore
--rw-r--r--   0        0        0     1084 2022-12-07 18:42:43.242114 toolsql-0.5.1/LICENSE
--rw-r--r--   0        0        0     4659 2023-04-11 15:37:42.827266 toolsql-0.5.1/README.md
--rw-r--r--   0        0        0        0 2022-12-07 18:42:43.251690 toolsql-0.5.1/py.typed
--rw-r--r--   0        0        0      649 2023-04-15 22:58:00.373193 toolsql-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      263 2023-01-21 18:52:09.694776 toolsql-0.5.1/tests/README.md
--rw-r--r--   0        0        0        0 2023-01-22 21:52:27.654376 toolsql-0.5.1/tests/conf/__init__.py
--rw-r--r--   0        0        0     1670 2023-01-28 01:59:10.345388 toolsql-0.5.1/tests/conf/conf_db_configs.py
--rw-r--r--   0        0        0     2120 2023-04-15 22:57:06.210871 toolsql-0.5.1/tests/conf/conf_helpers.py
--rw-r--r--   0        0        0     8392 2023-03-01 01:29:02.029340 toolsql-0.5.1/tests/conf/conf_tables.py
--rw-r--r--   0        0        0       62 2023-01-22 21:48:58.241419 toolsql-0.5.1/tests/conf/conf_write_queries.py
--rw-r--r--   0        0        0     4511 2023-02-03 00:06:54.451338 toolsql-0.5.1/tests/conftest.py
--rw-r--r--   0        0        0     2432 2023-03-05 03:27:04.199101 toolsql-0.5.1/tests/test_aggregations.py
--rw-r--r--   0        0        0     2220 2023-02-13 08:03:37.896687 toolsql-0.5.1/tests/test_column_expressions.py
--rw-r--r--   0        0        0     2084 2023-03-01 07:37:14.269608 toolsql-0.5.1/tests/test_dbms_metadata.py
--rw-r--r--   0        0        0     5206 2023-03-05 03:26:24.446611 toolsql-0.5.1/tests/test_delete.py
--rw-r--r--   0        0        0     2526 2023-03-05 07:24:19.484344 toolsql-0.5.1/tests/test_exceptions.py
--rw-r--r--   0        0        0    14606 2023-03-05 04:37:15.341481 toolsql-0.5.1/tests/test_insert.py
--rw-r--r--   0        0        0     1242 2023-03-01 07:35:46.632270 toolsql-0.5.1/tests/test_multicolumn_indices.py
--rw-r--r--   0        0        0     1075 2023-03-05 03:27:08.232652 toolsql-0.5.1/tests/test_renaming_results.py
--rw-r--r--   0        0        0    12107 2023-03-05 03:28:04.000994 toolsql-0.5.1/tests/test_select.py
--rw-r--r--   0        0        0     2003 2023-02-12 01:16:45.228226 toolsql-0.5.1/tests/test_summary.py
--rw-r--r--   0        0        0     8908 2023-03-06 02:50:19.508898 toolsql-0.5.1/tests/test_transactions.py
--rw-r--r--   0        0        0     3478 2023-03-05 03:30:56.862706 toolsql-0.5.1/tests/test_update.py
--rw-r--r--   0        0        0      233 2023-04-15 22:58:34.081963 toolsql-0.5.1/toolsql/__init__.py
--rw-r--r--   0        0        0       51 2023-04-11 15:27:03.745564 toolsql-0.5.1/toolsql/dbs/__init__.py
--rw-r--r--   0        0        0        1 2023-01-25 07:09:40.611833 toolsql-0.5.1/toolsql/dbs/db_classes/__init__.py
--rw-r--r--   0        0        0     4877 2023-04-12 01:43:17.868464 toolsql-0.5.1/toolsql/dbs/db_classes/abstract_db.py
--rw-r--r--   0        0        0    18537 2023-04-12 01:44:57.604428 toolsql-0.5.1/toolsql/dbs/db_classes/postgresql_db.py
--rw-r--r--   0        0        0     9519 2023-04-12 01:45:09.168973 toolsql-0.5.1/toolsql/dbs/db_classes/sqlite_db.py
--rw-r--r--   0        0        0     1251 2023-02-12 00:58:17.129402 toolsql-0.5.1/toolsql/dbs/db_utils.py
--rw-r--r--   0        0        0      560 2023-04-11 15:36:56.187104 toolsql-0.5.1/toolsql/dbs/login_utils.py
--rw-r--r--   0        0        0       84 2023-01-30 03:42:00.561041 toolsql-0.5.1/toolsql/drivers/__init__.py
--rw-r--r--   0        0        0      149 2023-02-02 22:58:21.072982 toolsql-0.5.1/toolsql/drivers/conn_utils/__init__.py
--rw-r--r--   0        0        0     1618 2023-03-19 18:55:10.095445 toolsql-0.5.1/toolsql/drivers/conn_utils/conn_attributes.py
--rw-r--r--   0        0        0     1986 2023-04-12 00:38:59.125862 toolsql-0.5.1/toolsql/drivers/conn_utils/connect_utils.py
--rw-r--r--   0        0        0      953 2023-02-03 05:07:04.778141 toolsql-0.5.1/toolsql/drivers/conn_utils/db_config_utils.py
--rw-r--r--   0        0        0     4853 2023-03-06 02:50:00.401901 toolsql-0.5.1/toolsql/drivers/conn_utils/transaction_utils.py
--rw-r--r--   0        0        0     1833 2023-03-27 19:30:33.769865 toolsql-0.5.1/toolsql/drivers/conn_utils/uri_utils.py
--rw-r--r--   0        0        0        0 2023-01-19 23:23:14.797191 toolsql-0.5.1/toolsql/drivers/driver_classes/__init__.py
--rw-r--r--   0        0        0     3437 2023-04-11 15:48:57.844239 toolsql-0.5.1/toolsql/drivers/driver_classes/abstract_driver.py
--rw-r--r--   0        0        0     1686 2023-03-22 00:04:08.425756 toolsql-0.5.1/toolsql/drivers/driver_classes/aiosqlite_driver.py
--rw-r--r--   0        0        0     6947 2023-04-12 00:38:35.826888 toolsql-0.5.1/toolsql/drivers/driver_classes/connectorx_driver.py
--rw-r--r--   0        0        0     4133 2023-04-11 15:55:51.938956 toolsql-0.5.1/toolsql/drivers/driver_classes/dbapi_driver.py
--rw-r--r--   0        0        0     3878 2023-03-27 19:32:22.818512 toolsql-0.5.1/toolsql/drivers/driver_classes/psycopg_driver.py
--rw-r--r--   0        0        0     2290 2023-03-22 00:03:41.799839 toolsql-0.5.1/toolsql/drivers/driver_classes/sqlite3_driver.py
--rw-r--r--   0        0        0     3968 2023-02-11 22:48:18.364943 toolsql-0.5.1/toolsql/drivers/driver_utils.py
--rw-r--r--   0        0        0       92 2023-02-03 19:35:08.076396 toolsql-0.5.1/toolsql/executors/__init__.py
--rw-r--r--   0        0        0      127 2023-01-30 03:14:58.462588 toolsql-0.5.1/toolsql/executors/ddl_executors/__init__.py
--rw-r--r--   0        0        0     2153 2023-02-01 21:30:22.128642 toolsql-0.5.1/toolsql/executors/ddl_executors/alter_executors.py
--rw-r--r--   0        0        0     2161 2023-03-28 18:58:28.379011 toolsql-0.5.1/toolsql/executors/ddl_executors/create_executors.py
--rw-r--r--   0        0        0     1153 2023-03-28 18:19:02.990162 toolsql-0.5.1/toolsql/executors/ddl_executors/drop_executors.py
--rw-r--r--   0        0        0     4105 2023-04-12 01:56:12.421844 toolsql-0.5.1/toolsql/executors/ddl_executors/metadata_executors.py
--rw-r--r--   0        0        0      128 2023-01-30 03:15:43.131090 toolsql-0.5.1/toolsql/executors/dml_executors/__init__.py
--rw-r--r--   0        0        0     2584 2023-03-28 19:49:02.476403 toolsql-0.5.1/toolsql/executors/dml_executors/delete_executors.py
--rw-r--r--   0        0        0     3409 2023-03-21 23:26:17.745727 toolsql-0.5.1/toolsql/executors/dml_executors/insert_executors.py
--rw-r--r--   0        0        0    19701 2023-04-12 01:58:15.422563 toolsql-0.5.1/toolsql/executors/dml_executors/select_executors.py
--rw-r--r--   0        0        0     2843 2023-02-12 04:21:29.361650 toolsql-0.5.1/toolsql/executors/dml_executors/update_executors.py
--rw-r--r--   0        0        0       59 2023-02-26 07:01:46.454118 toolsql-0.5.1/toolsql/executors/summary_executors/__init__.py
--rw-r--r--   0        0        0     3424 2023-03-28 18:23:04.706576 toolsql-0.5.1/toolsql/executors/summary_executors/summary_prints.py
--rw-r--r--   0        0        0     2201 2023-02-12 02:23:37.024146 toolsql-0.5.1/toolsql/executors/summary_executors/summary_usage.py
--rw-r--r--   0        0        0      102 2023-02-26 22:29:04.008347 toolsql-0.5.1/toolsql/formats/__init__.py
--rw-r--r--   0        0        0     4144 2023-04-11 15:35:31.235749 toolsql-0.5.1/toolsql/formats/encoding_format_utils.py
--rw-r--r--   0        0        0     2045 2023-04-11 15:35:17.654255 toolsql-0.5.1/toolsql/formats/json_format_utils.py
--rw-r--r--   0        0        0     5533 2023-04-11 15:35:06.683633 toolsql-0.5.1/toolsql/formats/row_format_utils.py
--rw-r--r--   0        0        0        0 2023-02-01 00:04:45.871374 toolsql-0.5.1/toolsql/py.typed
--rw-r--r--   0        0        0       61 2023-01-27 04:00:11.947543 toolsql-0.5.1/toolsql/schemas/__init__.py
--rw-r--r--   0        0        0     4240 2023-02-26 21:30:57.707911 toolsql-0.5.1/toolsql/schemas/datatype_utils.py
--rw-r--r--   0        0        0     5427 2023-03-28 20:11:21.623102 toolsql-0.5.1/toolsql/schemas/shorthand_utils.py
--rw-r--r--   0        0        0      147 2023-03-05 04:53:25.455675 toolsql-0.5.1/toolsql/spec/__init__.py
--rw-r--r--   0        0        0     1184 2023-03-05 07:23:00.086051 toolsql-0.5.1/toolsql/spec/exceptions.py
--rw-r--r--   0        0        0     2130 2023-03-06 07:52:30.415917 toolsql-0.5.1/toolsql/spec/typedata.py
--rw-r--r--   0        0        0      148 2023-03-27 21:12:23.119118 toolsql-0.5.1/toolsql/spec/typedefs/__init__.py
--rw-r--r--   0        0        0      234 2023-01-25 21:23:06.637935 toolsql-0.5.1/toolsql/spec/typedefs/dataset_types.py
--rw-r--r--   0        0        0     1504 2023-02-12 00:16:22.417559 toolsql-0.5.1/toolsql/spec/typedefs/driver_types.py
--rw-r--r--   0        0        0      109 2023-03-27 20:31:11.573302 toolsql-0.5.1/toolsql/spec/typedefs/permission_types.py
--rw-r--r--   0        0        0     3931 2023-03-16 07:48:08.417256 toolsql-0.5.1/toolsql/spec/typedefs/schema_types.py
--rw-r--r--   0        0        0     5568 2023-04-11 15:36:02.595008 toolsql-0.5.1/toolsql/spec/typedefs/statement_types.py
--rw-r--r--   0        0        0     2645 2023-04-11 15:34:42.673529 toolsql-0.5.1/toolsql/spec/typeguards.py
--rw-r--r--   0        0        0      125 2023-02-03 22:03:30.312085 toolsql-0.5.1/toolsql/statements/__init__.py
--rw-r--r--   0        0        0       96 2023-01-30 01:01:07.284310 toolsql-0.5.1/toolsql/statements/ddl_statements/__init__.py
--rw-r--r--   0        0        0     2631 2023-02-01 20:55:53.683307 toolsql-0.5.1/toolsql/statements/ddl_statements/alter_statements.py
--rw-r--r--   0        0        0     7916 2023-03-01 07:30:44.368247 toolsql-0.5.1/toolsql/statements/ddl_statements/create_statements.py
--rw-r--r--   0        0        0      636 2023-02-01 20:52:53.962533 toolsql-0.5.1/toolsql/statements/ddl_statements/drop_statements.py
--rw-r--r--   0        0        0      132 2023-01-30 01:01:54.106030 toolsql-0.5.1/toolsql/statements/dml_statements/__init__.py
--rw-r--r--   0        0        0     1712 2023-02-13 08:35:53.659371 toolsql-0.5.1/toolsql/statements/dml_statements/delete_statements.py
--rw-r--r--   0        0        0     6978 2023-02-27 06:35:28.865971 toolsql-0.5.1/toolsql/statements/dml_statements/insert_statements.py
--rw-r--r--   0        0        0     4472 2023-02-13 08:35:08.066374 toolsql-0.5.1/toolsql/statements/dml_statements/select_statements.py
--rw-r--r--   0        0        0     3280 2023-02-13 08:35:26.310154 toolsql-0.5.1/toolsql/statements/dml_statements/update_statements.py
--rw-r--r--   0        0        0    13142 2023-03-07 06:06:56.187816 toolsql-0.5.1/toolsql/statements/statement_utils.py
--rw-r--r--   0        0        0     1509 2023-02-04 01:31:44.402064 toolsql-0.5.1/toolsql/statements/summary_statements.py
--rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 toolsql-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-01-27 20:52:41.456006 toolsql-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1084 2022-12-07 18:42:43.242114 toolsql-0.5.2/LICENSE
+-rw-r--r--   0        0        0     4659 2023-04-11 15:37:42.827266 toolsql-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2022-12-07 18:42:43.251690 toolsql-0.5.2/py.typed
+-rw-r--r--   0        0        0      649 2023-04-15 22:58:00.373193 toolsql-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      263 2023-01-21 18:52:09.694776 toolsql-0.5.2/tests/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 21:52:27.654376 toolsql-0.5.2/tests/conf/__init__.py
+-rw-r--r--   0        0        0     1670 2023-01-28 01:59:10.345388 toolsql-0.5.2/tests/conf/conf_db_configs.py
+-rw-r--r--   0        0        0     2120 2023-04-15 22:57:06.210871 toolsql-0.5.2/tests/conf/conf_helpers.py
+-rw-r--r--   0        0        0     8392 2023-03-01 01:29:02.029340 toolsql-0.5.2/tests/conf/conf_tables.py
+-rw-r--r--   0        0        0       62 2023-01-22 21:48:58.241419 toolsql-0.5.2/tests/conf/conf_write_queries.py
+-rw-r--r--   0        0        0     4511 2023-02-03 00:06:54.451338 toolsql-0.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     2432 2023-03-05 03:27:04.199101 toolsql-0.5.2/tests/test_aggregations.py
+-rw-r--r--   0        0        0     2220 2023-02-13 08:03:37.896687 toolsql-0.5.2/tests/test_column_expressions.py
+-rw-r--r--   0        0        0     2084 2023-03-01 07:37:14.269608 toolsql-0.5.2/tests/test_dbms_metadata.py
+-rw-r--r--   0        0        0     5206 2023-03-05 03:26:24.446611 toolsql-0.5.2/tests/test_delete.py
+-rw-r--r--   0        0        0     2526 2023-03-05 07:24:19.484344 toolsql-0.5.2/tests/test_exceptions.py
+-rw-r--r--   0        0        0    14606 2023-03-05 04:37:15.341481 toolsql-0.5.2/tests/test_insert.py
+-rw-r--r--   0        0        0     1242 2023-03-01 07:35:46.632270 toolsql-0.5.2/tests/test_multicolumn_indices.py
+-rw-r--r--   0        0        0     1075 2023-03-05 03:27:08.232652 toolsql-0.5.2/tests/test_renaming_results.py
+-rw-r--r--   0        0        0    12107 2023-03-05 03:28:04.000994 toolsql-0.5.2/tests/test_select.py
+-rw-r--r--   0        0        0     2003 2023-02-12 01:16:45.228226 toolsql-0.5.2/tests/test_summary.py
+-rw-r--r--   0        0        0     8908 2023-03-06 02:50:19.508898 toolsql-0.5.2/tests/test_transactions.py
+-rw-r--r--   0        0        0     3478 2023-03-05 03:30:56.862706 toolsql-0.5.2/tests/test_update.py
+-rw-r--r--   0        0        0      233 2023-04-27 21:58:36.961295 toolsql-0.5.2/toolsql/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-11 15:27:03.745564 toolsql-0.5.2/toolsql/dbs/__init__.py
+-rw-r--r--   0        0        0        1 2023-01-25 07:09:40.611833 toolsql-0.5.2/toolsql/dbs/db_classes/__init__.py
+-rw-r--r--   0        0        0     4877 2023-04-12 01:43:17.868464 toolsql-0.5.2/toolsql/dbs/db_classes/abstract_db.py
+-rw-r--r--   0        0        0    19071 2023-04-27 21:02:35.060364 toolsql-0.5.2/toolsql/dbs/db_classes/postgresql_db.py
+-rw-r--r--   0        0        0     9559 2023-04-27 20:53:47.906206 toolsql-0.5.2/toolsql/dbs/db_classes/sqlite_db.py
+-rw-r--r--   0        0        0     1251 2023-02-12 00:58:17.129402 toolsql-0.5.2/toolsql/dbs/db_utils.py
+-rw-r--r--   0        0        0      920 2023-04-27 20:38:29.627687 toolsql-0.5.2/toolsql/dbs/login_utils.py
+-rw-r--r--   0        0        0       84 2023-01-30 03:42:00.561041 toolsql-0.5.2/toolsql/drivers/__init__.py
+-rw-r--r--   0        0        0      149 2023-02-02 22:58:21.072982 toolsql-0.5.2/toolsql/drivers/conn_utils/__init__.py
+-rw-r--r--   0        0        0     1618 2023-03-19 18:55:10.095445 toolsql-0.5.2/toolsql/drivers/conn_utils/conn_attributes.py
+-rw-r--r--   0        0        0     1986 2023-04-12 00:38:59.125862 toolsql-0.5.2/toolsql/drivers/conn_utils/connect_utils.py
+-rw-r--r--   0        0        0      953 2023-02-03 05:07:04.778141 toolsql-0.5.2/toolsql/drivers/conn_utils/db_config_utils.py
+-rw-r--r--   0        0        0     4853 2023-03-06 02:50:00.401901 toolsql-0.5.2/toolsql/drivers/conn_utils/transaction_utils.py
+-rw-r--r--   0        0        0     1833 2023-03-27 19:30:33.769865 toolsql-0.5.2/toolsql/drivers/conn_utils/uri_utils.py
+-rw-r--r--   0        0        0        0 2023-01-19 23:23:14.797191 toolsql-0.5.2/toolsql/drivers/driver_classes/__init__.py
+-rw-r--r--   0        0        0     3437 2023-04-11 15:48:57.844239 toolsql-0.5.2/toolsql/drivers/driver_classes/abstract_driver.py
+-rw-r--r--   0        0        0     1686 2023-03-22 00:04:08.425756 toolsql-0.5.2/toolsql/drivers/driver_classes/aiosqlite_driver.py
+-rw-r--r--   0        0        0     6947 2023-04-12 00:38:35.826888 toolsql-0.5.2/toolsql/drivers/driver_classes/connectorx_driver.py
+-rw-r--r--   0        0        0     4133 2023-04-11 15:55:51.938956 toolsql-0.5.2/toolsql/drivers/driver_classes/dbapi_driver.py
+-rw-r--r--   0        0        0     3878 2023-03-27 19:32:22.818512 toolsql-0.5.2/toolsql/drivers/driver_classes/psycopg_driver.py
+-rw-r--r--   0        0        0     2290 2023-03-22 00:03:41.799839 toolsql-0.5.2/toolsql/drivers/driver_classes/sqlite3_driver.py
+-rw-r--r--   0        0        0     3968 2023-02-11 22:48:18.364943 toolsql-0.5.2/toolsql/drivers/driver_utils.py
+-rw-r--r--   0        0        0       92 2023-02-03 19:35:08.076396 toolsql-0.5.2/toolsql/executors/__init__.py
+-rw-r--r--   0        0        0      127 2023-01-30 03:14:58.462588 toolsql-0.5.2/toolsql/executors/ddl_executors/__init__.py
+-rw-r--r--   0        0        0     2153 2023-02-01 21:30:22.128642 toolsql-0.5.2/toolsql/executors/ddl_executors/alter_executors.py
+-rw-r--r--   0        0        0     2504 2023-04-27 01:37:34.473367 toolsql-0.5.2/toolsql/executors/ddl_executors/create_executors.py
+-rw-r--r--   0        0        0     1153 2023-03-28 18:19:02.990162 toolsql-0.5.2/toolsql/executors/ddl_executors/drop_executors.py
+-rw-r--r--   0        0        0     4105 2023-04-12 01:56:12.421844 toolsql-0.5.2/toolsql/executors/ddl_executors/metadata_executors.py
+-rw-r--r--   0        0        0      128 2023-01-30 03:15:43.131090 toolsql-0.5.2/toolsql/executors/dml_executors/__init__.py
+-rw-r--r--   0        0        0     2584 2023-03-28 19:49:02.476403 toolsql-0.5.2/toolsql/executors/dml_executors/delete_executors.py
+-rw-r--r--   0        0        0     3409 2023-03-21 23:26:17.745727 toolsql-0.5.2/toolsql/executors/dml_executors/insert_executors.py
+-rw-r--r--   0        0        0    19701 2023-04-12 01:58:15.422563 toolsql-0.5.2/toolsql/executors/dml_executors/select_executors.py
+-rw-r--r--   0        0        0     2843 2023-02-12 04:21:29.361650 toolsql-0.5.2/toolsql/executors/dml_executors/update_executors.py
+-rw-r--r--   0        0        0       59 2023-02-26 07:01:46.454118 toolsql-0.5.2/toolsql/executors/summary_executors/__init__.py
+-rw-r--r--   0        0        0     3424 2023-03-28 18:23:04.706576 toolsql-0.5.2/toolsql/executors/summary_executors/summary_prints.py
+-rw-r--r--   0        0        0     2201 2023-02-12 02:23:37.024146 toolsql-0.5.2/toolsql/executors/summary_executors/summary_usage.py
+-rw-r--r--   0        0        0      102 2023-02-26 22:29:04.008347 toolsql-0.5.2/toolsql/formats/__init__.py
+-rw-r--r--   0        0        0     4144 2023-04-11 15:35:31.235749 toolsql-0.5.2/toolsql/formats/encoding_format_utils.py
+-rw-r--r--   0        0        0     2045 2023-04-11 15:35:17.654255 toolsql-0.5.2/toolsql/formats/json_format_utils.py
+-rw-r--r--   0        0        0     5533 2023-04-11 15:35:06.683633 toolsql-0.5.2/toolsql/formats/row_format_utils.py
+-rw-r--r--   0        0        0        0 2023-02-01 00:04:45.871374 toolsql-0.5.2/toolsql/py.typed
+-rw-r--r--   0        0        0       61 2023-01-27 04:00:11.947543 toolsql-0.5.2/toolsql/schemas/__init__.py
+-rw-r--r--   0        0        0     4240 2023-02-26 21:30:57.707911 toolsql-0.5.2/toolsql/schemas/datatype_utils.py
+-rw-r--r--   0        0        0     5576 2023-04-27 20:46:22.127450 toolsql-0.5.2/toolsql/schemas/shorthand_utils.py
+-rw-r--r--   0        0        0      147 2023-03-05 04:53:25.455675 toolsql-0.5.2/toolsql/spec/__init__.py
+-rw-r--r--   0        0        0     1184 2023-03-05 07:23:00.086051 toolsql-0.5.2/toolsql/spec/exceptions.py
+-rw-r--r--   0        0        0     2130 2023-03-06 07:52:30.415917 toolsql-0.5.2/toolsql/spec/typedata.py
+-rw-r--r--   0        0        0      148 2023-03-27 21:12:23.119118 toolsql-0.5.2/toolsql/spec/typedefs/__init__.py
+-rw-r--r--   0        0        0      234 2023-01-25 21:23:06.637935 toolsql-0.5.2/toolsql/spec/typedefs/dataset_types.py
+-rw-r--r--   0        0        0     1504 2023-02-12 00:16:22.417559 toolsql-0.5.2/toolsql/spec/typedefs/driver_types.py
+-rw-r--r--   0        0        0      109 2023-03-27 20:31:11.573302 toolsql-0.5.2/toolsql/spec/typedefs/permission_types.py
+-rw-r--r--   0        0        0     4031 2023-04-27 20:45:29.560935 toolsql-0.5.2/toolsql/spec/typedefs/schema_types.py
+-rw-r--r--   0        0        0     5568 2023-04-11 15:36:02.595008 toolsql-0.5.2/toolsql/spec/typedefs/statement_types.py
+-rw-r--r--   0        0        0     2645 2023-04-11 15:34:42.673529 toolsql-0.5.2/toolsql/spec/typeguards.py
+-rw-r--r--   0        0        0      125 2023-02-03 22:03:30.312085 toolsql-0.5.2/toolsql/statements/__init__.py
+-rw-r--r--   0        0        0       96 2023-01-30 01:01:07.284310 toolsql-0.5.2/toolsql/statements/ddl_statements/__init__.py
+-rw-r--r--   0        0        0     2631 2023-02-01 20:55:53.683307 toolsql-0.5.2/toolsql/statements/ddl_statements/alter_statements.py
+-rw-r--r--   0        0        0     8586 2023-04-27 20:52:25.616132 toolsql-0.5.2/toolsql/statements/ddl_statements/create_statements.py
+-rw-r--r--   0        0        0      636 2023-02-01 20:52:53.962533 toolsql-0.5.2/toolsql/statements/ddl_statements/drop_statements.py
+-rw-r--r--   0        0        0      132 2023-01-30 01:01:54.106030 toolsql-0.5.2/toolsql/statements/dml_statements/__init__.py
+-rw-r--r--   0        0        0     1712 2023-02-13 08:35:53.659371 toolsql-0.5.2/toolsql/statements/dml_statements/delete_statements.py
+-rw-r--r--   0        0        0     6978 2023-02-27 06:35:28.865971 toolsql-0.5.2/toolsql/statements/dml_statements/insert_statements.py
+-rw-r--r--   0        0        0     4472 2023-02-13 08:35:08.066374 toolsql-0.5.2/toolsql/statements/dml_statements/select_statements.py
+-rw-r--r--   0        0        0     3280 2023-02-13 08:35:26.310154 toolsql-0.5.2/toolsql/statements/dml_statements/update_statements.py
+-rw-r--r--   0        0        0    13253 2023-04-27 05:59:35.674096 toolsql-0.5.2/toolsql/statements/statement_utils.py
+-rw-r--r--   0        0        0     1509 2023-02-04 01:31:44.402064 toolsql-0.5.2/toolsql/statements/summary_statements.py
+-rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 toolsql-0.5.2/PKG-INFO
```

### Comparing `toolsql-0.5.1/LICENSE` & `toolsql-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/README.md` & `toolsql-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/pyproject.toml` & `toolsql-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/conf/conf_db_configs.py` & `toolsql-0.5.2/tests/conf/conf_db_configs.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/conf/conf_helpers.py` & `toolsql-0.5.2/tests/conf/conf_helpers.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/conf/conf_tables.py` & `toolsql-0.5.2/tests/conf/conf_tables.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/conftest.py` & `toolsql-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/test_aggregations.py` & `toolsql-0.5.2/tests/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/test_column_expressions.py` & `toolsql-0.5.2/tests/test_column_expressions.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/test_dbms_metadata.py` & `toolsql-0.5.2/tests/test_dbms_metadata.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/test_delete.py` & `toolsql-0.5.2/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/test_exceptions.py` & `toolsql-0.5.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/test_insert.py` & `toolsql-0.5.2/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/test_multicolumn_indices.py` & `toolsql-0.5.2/tests/test_multicolumn_indices.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/test_renaming_results.py` & `toolsql-0.5.2/tests/test_renaming_results.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/test_select.py` & `toolsql-0.5.2/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/test_summary.py` & `toolsql-0.5.2/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/test_transactions.py` & `toolsql-0.5.2/tests/test_transactions.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/tests/test_update.py` & `toolsql-0.5.2/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/dbs/db_classes/abstract_db.py` & `toolsql-0.5.2/toolsql/dbs/db_classes/abstract_db.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/dbs/db_classes/postgresql_db.py` & `toolsql-0.5.2/toolsql/dbs/db_classes/postgresql_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import os
 import typing
 
 from toolsql import executors
 from toolsql import spec
 from toolsql import statements
 from . import abstract_db
 
@@ -29,25 +30,34 @@
 
 
 class PostgresqlDb(abstract_db.AbstractDb):
     @classmethod
     def create_db(cls, db_config: spec.DBConfig) -> None:
         import subprocess
 
+        format_config: dict[str, typing.Any] = db_config.copy()  # type: ignore
+        if format_config.get('owner') is None:
+            format_config['owner'] = format_config.get('username')
+
         template = (
             'createdb'
             ' --owner={owner}'
             ' --host={hostname}'
             ' --port={port}'
             ' --username={username}'
-            ' --password={password}'
             ' {database}'
         )
-        cmd = template.format(**db_config)
-        subprocess.call(cmd)
+        cmd = template.format(**format_config)
+        password = db_config.get('password')
+        if password is None or password == '':
+            env = None
+        else:
+            env = os.environ.copy()
+            env['PGPASSWORD'] = password
+        subprocess.call(cmd.split(' '), env=env)
 
     @classmethod
     def get_table_names(
         cls,
         conn: spec.Connection,
         *,
         permission: spec.TablePermission = 'read',
@@ -145,14 +155,17 @@
         for raw_column in raw_columns:
             raw_column['primary'] = raw_column['name'] in primary_keys
 
             # TODO
             raw_column['index'] = raw_column['name'] in indexed_single_columns
             raw_column['unique'] = raw_column['name'] in unique_single_columns
 
+            # TODO
+            raw_column['autoincrement'] = False
+
             # TODO: support more datatypes for default values
             if raw_column['default'] is not None:
                 default = raw_column['default']
                 if default[0] == "'" and default[-1] == "'":
                     raw_column['default'] = default.strip("'")
                 elif default.endswith('::text'):
                     raw_column['default'] = default.split('::text')[0].strip(
@@ -255,14 +268,17 @@
         for raw_column in raw_columns:
             raw_column['primary'] = raw_column['name'] in primary_keys
 
             # TODO
             raw_column['index'] = raw_column['name'] in indexed_single_columns
             raw_column['unique'] = raw_column['name'] in unique_single_columns
 
+            # TODO
+            raw_column['autoincrement'] = False
+
         return {
             'name': table_name,
             'description': None,
             'columns': raw_columns,  # type: ignore
             'indices': [],
             'constraints': [],
         }
```

### Comparing `toolsql-0.5.1/toolsql/dbs/db_classes/sqlite_db.py` & `toolsql-0.5.2/toolsql/dbs/db_classes/sqlite_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,14 +120,15 @@
                 'name': name,
                 'type': type,
                 'nullable': not not_null,
                 'default': default,
                 'primary': primary,
                 'index': name in indexed_single_columns,
                 'unique': name in unique_single_columns,
+                'autoincrement': False,
                 'description': None,
             }
             columns.append(column)
 
         if len(unique_multi_columns) > 0:
             raise NotImplementedError('multicolumn_indices')
```

### Comparing `toolsql-0.5.1/toolsql/dbs/db_utils.py` & `toolsql-0.5.2/toolsql/dbs/db_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/dbs/login_utils.py` & `toolsql-0.5.2/toolsql/dbs/login_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 from __future__ import annotations
 
+import os
+
 import toolsql
 
 
 def login(db_config: toolsql.DBConfig) -> None:
     """connect to db using interactive shell"""
 
     import subprocess
 
+    env = os.environ.copy()
     if db_config['dbms'] == 'sqlite':
         path = db_config.get('path')
         if path is None:
             raise Exception('no path specified for sqlite database')
         cmd = ['sqlite3', path]
 
     elif db_config['dbms'] == 'postgresql':
-        raise NotImplementedError()
+        template = (
+            'psql'
+            ' --host={hostname}'
+            ' --port={port}'
+            ' --username={username}'
+            ' {database}'
+        )
+        cmd = template.format(**db_config).split(' ')
+        password = db_config.get('password')
+        if password is not None:
+            env['PGPASSWORD'] = password
 
     else:
         raise Exception('invalid dbms: ' + str(db_config['dbms']))
 
-    subprocess.call(cmd)
+    subprocess.call(cmd, env=env)
```

### Comparing `toolsql-0.5.1/toolsql/drivers/conn_utils/conn_attributes.py` & `toolsql-0.5.2/toolsql/drivers/conn_utils/conn_attributes.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/drivers/conn_utils/connect_utils.py` & `toolsql-0.5.2/toolsql/drivers/conn_utils/connect_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/drivers/conn_utils/db_config_utils.py` & `toolsql-0.5.2/toolsql/drivers/conn_utils/db_config_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/drivers/conn_utils/transaction_utils.py` & `toolsql-0.5.2/toolsql/drivers/conn_utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/drivers/conn_utils/uri_utils.py` & `toolsql-0.5.2/toolsql/drivers/conn_utils/uri_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/drivers/driver_classes/abstract_driver.py` & `toolsql-0.5.2/toolsql/drivers/driver_classes/abstract_driver.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/drivers/driver_classes/aiosqlite_driver.py` & `toolsql-0.5.2/toolsql/drivers/driver_classes/aiosqlite_driver.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/drivers/driver_classes/connectorx_driver.py` & `toolsql-0.5.2/toolsql/drivers/driver_classes/connectorx_driver.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/drivers/driver_classes/dbapi_driver.py` & `toolsql-0.5.2/toolsql/drivers/driver_classes/dbapi_driver.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/drivers/driver_classes/psycopg_driver.py` & `toolsql-0.5.2/toolsql/drivers/driver_classes/psycopg_driver.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/drivers/driver_classes/sqlite3_driver.py` & `toolsql-0.5.2/toolsql/drivers/driver_classes/sqlite3_driver.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/drivers/driver_utils.py` & `toolsql-0.5.2/toolsql/drivers/driver_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/executors/ddl_executors/alter_executors.py` & `toolsql-0.5.2/toolsql/executors/ddl_executors/alter_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/executors/ddl_executors/create_executors.py` & `toolsql-0.5.2/toolsql/executors/ddl_executors/create_executors.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,29 +37,37 @@
         )
         for sql in sqls:
             conn.execute(sql)
 
 
 def create_db(
     *,
-    db_schema: spec.DBSchema,
+    db_schema: spec.DBSchema | None = None,
     db_config: spec.DBConfig,
     db_only: bool = False,
     if_not_exists: bool = False,
     confirm: bool = False,
+    verbose: bool = False,
 ) -> None:
 
     if not confirm:
         raise Exception('must use confirm=True to modify database')
 
     # create database itself
     if not metadata_executors.does_db_exist(db_config):
+        if verbose:
+            print('creating', db_config['dbms'], 'database')
         db_class = dbs.get_db_class(db_config=db_config)
         db_class.create_db(db_config=db_config)
-    if db_only:
+    else:
+        if verbose:
+            print(db_config['dbms'], 'database already exists')
+        if not if_not_exists:
+            raise Exception(db_config['dbms'] + ' database already exists')
+    if db_only or db_schema is None:
         return
 
     # create database tables
     if isinstance(db_config, dict):
         dialect = db_config.get('dbms')
     elif isinstance(db_config, str):
         dialect = drivers.get_conn_dialect(db_config)
```

### Comparing `toolsql-0.5.1/toolsql/executors/ddl_executors/drop_executors.py` & `toolsql-0.5.2/toolsql/executors/ddl_executors/drop_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/executors/ddl_executors/metadata_executors.py` & `toolsql-0.5.2/toolsql/executors/ddl_executors/metadata_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/executors/dml_executors/delete_executors.py` & `toolsql-0.5.2/toolsql/executors/dml_executors/delete_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/executors/dml_executors/insert_executors.py` & `toolsql-0.5.2/toolsql/executors/dml_executors/insert_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/executors/dml_executors/select_executors.py` & `toolsql-0.5.2/toolsql/executors/dml_executors/select_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/executors/dml_executors/update_executors.py` & `toolsql-0.5.2/toolsql/executors/dml_executors/update_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/executors/summary_executors/summary_prints.py` & `toolsql-0.5.2/toolsql/executors/summary_executors/summary_prints.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/executors/summary_executors/summary_usage.py` & `toolsql-0.5.2/toolsql/executors/summary_executors/summary_usage.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/formats/encoding_format_utils.py` & `toolsql-0.5.2/toolsql/formats/encoding_format_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/formats/json_format_utils.py` & `toolsql-0.5.2/toolsql/formats/json_format_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/formats/row_format_utils.py` & `toolsql-0.5.2/toolsql/formats/row_format_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/schemas/datatype_utils.py` & `toolsql-0.5.2/toolsql/schemas/datatype_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/schemas/shorthand_utils.py` & `toolsql-0.5.2/toolsql/schemas/shorthand_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,14 +128,18 @@
     if name is None:
         raise Exception('column name not specified')
 
     primary = column.get('primary')
     if primary is None:
         primary = False
 
+    autoincrement = column.get('autoincrement')
+    if autoincrement is None:
+        autoincrement = False
+
     nullable = column.get('nullable')
     if nullable is None:
         nullable = not primary
 
     column_type = column.get('type')
     if column_type is None:
         raise Exception('column type not specified')
@@ -170,10 +174,11 @@
         'default': default,
         'index': index,
         'name': name,
         'nullable': nullable,
         'primary': primary,
         'type': column_type,
         'unique': unique,
+        'autoincrement': autoincrement,
         'description': column.get('description'),
     }
```

### Comparing `toolsql-0.5.1/toolsql/spec/exceptions.py` & `toolsql-0.5.2/toolsql/spec/exceptions.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/spec/typedata.py` & `toolsql-0.5.2/toolsql/spec/typedata.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/spec/typedefs/driver_types.py` & `toolsql-0.5.2/toolsql/spec/typedefs/driver_types.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/spec/typedefs/schema_types.py` & `toolsql-0.5.2/toolsql/spec/typedefs/schema_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,25 +57,27 @@
     default: typing.Any  # default value
     index: bool  # whether to create an index for column
     name: str  # name of table, usually specified in TableSpec
     nullable: bool  # for whether column can be null
     primary: bool  # for use as primary key
     type: ColumntypeShorthand
     unique: bool  # for creating unique index
+    autoincrement: Literal[False, True, 'strict']
 
 
 class ColumnSchema(TypedDict):
     description: NotRequired[str | None]
     default: typing.Any  # default value
     index: bool  # whether to create an index for column
     name: str  # name of table, usually specified in TableSpec
     nullable: bool  # for whether column can be null
     primary: bool  # for use as primary key
     type: Columntype
     unique: bool  # for creating unique index
+    autoincrement: Literal[False, True, 'strict']
     #
     # in near future
     # on_delete: DeleteOption  # what to do when foreign key deleted
     # fk_column: str  # column name
     # fk_table: str  # table name
     #
     # possible in future
```

### Comparing `toolsql-0.5.1/toolsql/spec/typedefs/statement_types.py` & `toolsql-0.5.2/toolsql/spec/typedefs/statement_types.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/spec/typeguards.py` & `toolsql-0.5.2/toolsql/spec/typeguards.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/statements/ddl_statements/alter_statements.py` & `toolsql-0.5.2/toolsql/statements/ddl_statements/alter_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/statements/ddl_statements/create_statements.py` & `toolsql-0.5.2/toolsql/statements/ddl_statements/create_statements.py`

 * *Files 9% similar despite different names*

```diff
@@ -77,14 +77,31 @@
         dialect,
     )
     line = column['name'] + ' ' + columntype.upper()
 
     if column['primary'] and not composite_primary_key:
         line = line + ' PRIMARY KEY'
 
+    if column['autoincrement']:
+        if column['autoincrement'] == 'strict':
+            if dialect == 'postgresql':
+                line = line + ' GENERATED ALWAYS AS IDENTITY'
+            elif dialect == 'sqlite':
+                line = line + ' AUTOINCREMENT'
+            else:
+                raise Exception('invalid dialect: ' + str(dialect))
+        else:
+            if dialect == 'postgresql':
+                line = line + ' GENERATED BY DEFAULT AS IDENTITY'
+            elif dialect == 'sqlite':
+                # this is already default behavior
+                pass
+            else:
+                raise Exception('invalid dialect: ' + str(dialect))
+
     if not column['nullable']:
         line = line + ' NOT NULL'
 
     if column['unique']:
         line = line + ' UNIQUE'
 
     if column['default'] is not None:
```

### Comparing `toolsql-0.5.1/toolsql/statements/ddl_statements/drop_statements.py` & `toolsql-0.5.2/toolsql/statements/ddl_statements/drop_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/statements/dml_statements/delete_statements.py` & `toolsql-0.5.2/toolsql/statements/dml_statements/delete_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/statements/dml_statements/insert_statements.py` & `toolsql-0.5.2/toolsql/statements/dml_statements/insert_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/statements/dml_statements/select_statements.py` & `toolsql-0.5.2/toolsql/statements/dml_statements/select_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/statements/dml_statements/update_statements.py` & `toolsql-0.5.2/toolsql/statements/dml_statements/update_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/toolsql/statements/statement_utils.py` & `toolsql-0.5.2/toolsql/statements/statement_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,14 +324,17 @@
 
                 subclauses.append(column_name + symbol + placeholder)
                 parameters.append(column_value)
 
     if where_in is not None:
         for column_name, column_value in where_in.items():
 
+            if len(column_value) == 0:
+                raise Exception('cannot use WHERE IN with empty list')
+
             # convert hex to binary
             if (
                 column_types is not None
                 and column_types.get(column_name) in spec.binary_columntypes
             ):
                 column_value = [
                     _convert_hex_to_bytes(subvalue) for subvalue in column_value
```

### Comparing `toolsql-0.5.1/toolsql/statements/summary_statements.py` & `toolsql-0.5.2/toolsql/statements/summary_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.1/PKG-INFO` & `toolsql-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolsql
-Version: 0.5.1
+Version: 0.5.2
 Summary: toolsql is an async+sync sql builder+executor for sqlite+postgres
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: typing_extensions>=4.2.0
 Requires-Dist: toolstr >=0.9.1, <0.10
 Requires-Dist: polars >=0.17.2, <0.18
 Requires-Dist: aiosqlite >=0.18.0, <0.19
```

