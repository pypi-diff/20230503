# Comparing `tmp/dbt-athena-community-1.4.3.tar.gz` & `tmp/dbt-athena-community-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-athena-community-1.4.3.tar", last modified: Mon Apr 17 14:02:16 2023, max compression
+gzip compressed data, was "dbt-athena-community-1.4.4.tar", last modified: Wed May  3 08:00:02 2023, max compression
```

## Comparing `dbt-athena-community-1.4.3.tar` & `dbt-athena-community-1.4.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.566805 dbt-athena-community-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-04-17 14:02:16.566805 dbt-athena-community-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19331 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/adapters/athena/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30215 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/adapters/athena/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.558805 dbt-athena-community-1.4.3/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.558805 dbt-athena-community-1.4.3/dbt/include/athena/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.558805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.558805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/table/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.562805 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.566805 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/ddl_data_type.sql
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/profile_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/dbt/include/athena/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:02:16.566805 dbt-athena-community-1.4.3/dbt_athena_community.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-04-17 14:02:16.000000 dbt-athena-community-1.4.3/dbt_athena_community.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-17 14:02:16.000000 dbt-athena-community-1.4.3/dbt_athena_community.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:02:16.000000 dbt-athena-community-1.4.3/dbt_athena_community.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 14:02:16.000000 dbt-athena-community-1.4.3/dbt_athena_community.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 14:02:16.000000 dbt-athena-community-1.4.3/dbt_athena_community.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:02:16.566805 dbt-athena-community-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-17 14:02:02.000000 dbt-athena-community-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.408949 dbt-athena-community-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21963 2023-05-03 08:00:02.408949 dbt-athena-community-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21719 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.400949 dbt-athena-community-1.4.4/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.400949 dbt-athena-community-1.4.4/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/adapters/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31197 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/adapters/athena/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.400949 dbt-athena-community-1.4.4/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.400949 dbt-athena-community-1.4.4/dbt/include/athena/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.400949 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.400949 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/table/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.404950 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/snapshots/snapshot.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.408949 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/ddl_data_type.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/profile_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/dbt/include/athena/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 08:00:02.408949 dbt-athena-community-1.4.4/dbt_athena_community.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21963 2023-05-03 08:00:02.000000 dbt-athena-community-1.4.4/dbt_athena_community.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-03 08:00:02.000000 dbt-athena-community-1.4.4/dbt_athena_community.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 08:00:02.000000 dbt-athena-community-1.4.4/dbt_athena_community.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-03 08:00:02.000000 dbt-athena-community-1.4.4/dbt_athena_community.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-03 08:00:02.000000 dbt-athena-community-1.4.4/dbt_athena_community.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 08:00:02.408949 dbt-athena-community-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-03 07:59:50.000000 dbt-athena-community-1.4.4/setup.py
```

### Comparing `dbt-athena-community-1.4.3/LICENSE.txt` & `dbt-athena-community-1.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/PKG-INFO` & `dbt-athena-community-1.4.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-athena-community
-Version: 1.4.3
+Version: 1.4.4
 Summary: The athena adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-athena/dbt-athena
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/dbt-athena-long.png" />
@@ -63,34 +63,39 @@
 
 Notes:
 - Take note of your AWS region code (e.g. `us-west-2` or `eu-west-2`, etc.).
 - You can also use [AWS Glue](https://docs.aws.amazon.com/athena/latest/ug/glue-athena.html) to create and manage Athena databases.
 
 ### Credentials
 
-This plugin does not accept any credentials directly. Instead, [credentials are determined automatically](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3` conventions and
-stored login info. You can configure the AWS profile name to use via `aws_profile_name`. Checkout DBT profile configuration below for details.
+Credentials can be passed directly to the adapter, or they can be [determined automatically](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3` conventions.
+You can either:
+- configure `aws_access_key_id` and `aws_secret_access_key`
+- configure `aws_profile_name` to match a profile defined in your AWS credentials file
+Checkout DBT profile configuration below for details.
 
 ### Configuring your profile
 
 A dbt profile can be configured to run against AWS Athena using the following configuration:
 
-| Option           | Description                                                                    | Required? | Example                                  |
-|------------------|--------------------------------------------------------------------------------|-----------|------------------------------------------|
-| s3_staging_dir   | S3 location to store Athena query results and metadata                         | Required  | `s3://bucket/dbt/`                       |
-| s3_data_dir      | Prefix for storing tables, if different from the connection's `s3_staging_dir` | Optional  | `s3://bucket2/dbt/`                      |
-| s3_data_naming   | How to generate table paths in `s3_data_dir`                                   | Optional  | `schema_table_unique`                    |
-| region_name      | AWS region of your Athena instance                                             | Required  | `eu-west-1`                              |
-| schema           | Specify the schema (Athena database) to build models into (lowercase **only**) | Required  | `dbt`                                    |
-| database         | Specify the database (Data catalog) to build models into (lowercase **only**)  | Required  | `awsdatacatalog`                         |
-| poll_interval    | Interval in seconds to use for polling the status of query results in Athena   | Optional  | `5`                                      |
-| aws_profile_name | Profile to use from your AWS shared credentials file.                          | Optional  | `my-profile`                             |
-| work_group       | Identifier of Athena workgroup                                                 | Optional  | `my-custom-workgroup`                    |
-| num_retries      | Number of times to retry a failing query                                       | Optional  | `3`                                      |
-| lf_tags          | Default lf tags to apply to any database created by dbt                        | Optional  | `{"origin": "dbt", "team": "analytics"}` |
+| Option                | Description                                                                    | Required? | Example                                    |
+|-----------------------|--------------------------------------------------------------------------------|-----------|--------------------------------------------|
+| s3_staging_dir        | S3 location to store Athena query results and metadata                         | Required  | `s3://bucket/dbt/`                         |
+| s3_data_dir           | Prefix for storing tables, if different from the connection's `s3_staging_dir` | Optional  | `s3://bucket2/dbt/`                        |
+| s3_data_naming        | How to generate table paths in `s3_data_dir`                                   | Optional  | `schema_table_unique`                      |
+| region_name           | AWS region of your Athena instance                                             | Required  | `eu-west-1`                                |
+| schema                | Specify the schema (Athena database) to build models into (lowercase **only**) | Required  | `dbt`                                      |
+| database              | Specify the database (Data catalog) to build models into (lowercase **only**)  | Required  | `awsdatacatalog`                           |
+| poll_interval         | Interval in seconds to use for polling the status of query results in Athena   | Optional  | `5`                                        |
+| aws_access_key_id     | Access key ID of the user performing requests.                                 | Optional  | `AKIAIOSFODNN7EXAMPLE`                     |
+| aws_secret_access_key | Secret access key of the user performing requests                              | Optional  | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` |
+| aws_profile_name      | Profile to use from your AWS shared credentials file.                          | Optional  | `my-profile`                               |
+| work_group            | Identifier of Athena workgroup                                                 | Optional  | `my-custom-workgroup`                      |
+| num_retries           | Number of times to retry a failing query                                       | Optional  | `3`                                        |
+| lf_tags               | Default lf tags to apply to any database created by dbt                        | Optional  | `{"origin": "dbt", "team": "analytics"}`   |
 
 **Example profiles.yml entry:**
 ```yaml
 athena:
   target: dev
   outputs:
     dev:
@@ -218,15 +223,39 @@
 Iceberg supports bucketing as hidden partitions, therefore use the `partitioned_by` config to add specific bucketing conditions.
 
 Iceberg supports several table formats for data : `PARQUET`, `AVRO` and `ORC`.
 
 It is possible to use iceberg in an incremental fashion, specifically 2 strategies are supported:
 * `append`: new records are appended to the table, this can lead to duplicates
 * `merge`: must be used in combination with `unique_key` and it's only available with Engine version 3.
-   It performs an upsert, new record are added, and record already existing are updated
+   It performs an upsert, new record are added, and record already existing are updated. If
+   `delete_condition` is provided in the model config, it can also delete records based on the
+   provided condition (SQL condition). You can use any column of the incremental table (`src`) or
+   the final table (`target`). You must prefix the column by the name of the table to prevent
+   `Column is ambiguous` error.
+
+```sql
+{{ config(
+    materialized='incremental',
+    table_type='iceberg',
+    incremental_strategy='merge',
+    unique_key='user_id',
+    delete_condition="src.status != 'active' and target.my_date < now() - interval '2' year"
+    format='parquet',
+) }}
+
+SELECT
+	'A' AS user_id,
+	'pi' AS name,
+	'active' AS status,
+	17.89 AS cost,
+	1 AS quantity,
+	100000000 AS quantity_big,
+	current_date AS my_date
+```
 
 ### High available table materialization
 The current implementation of the table materialization can lead to downtime, as target table is dropped and re-created.
 To have the less destructive behavior it's possible to use `table='table_hive_ha'` materialization.
 **table_hive_ha** leverage the table versions feature of glue catalog, creating a tmp table and swapping
 the target table to the location of the tmp table.
 This materialization is only available for `table_type=hive` and requires using unique locations.
@@ -381,76 +410,41 @@
   See https://github.com/dbt-athena/dbt-athena/issues/103 for more details.
 
 * Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
 
 
 ## Contributing
 
-This connector works with Python from 3.7 to 3.11.
-
-### Getting started
-
-In order to start developing on this adapter clone the repo and run this make command (see [Makefile](Makefile)) :
-
-```bash
-make setup
-```
-
-It will :
-1. Install all dependencies.
-2. Install pre-commit hooks.
-3. Generate your `.env` file
-
-Next, adjust `.env` file by configuring the environment variables to match your Athena development environment.
-
-### Running tests
-
-We have 2 different types of testing:
-* **unit testing**: you can run this type of tests running `make unit_test`
-* **functional testing**: you must have an AWS account with Athena setup in order to launch this type of tests and have a `.env` file in place with the right values.
-  You can run this type of tests running `make functional_test`
-
-All type of tests can be run using `make`:
-```bash
-make test
-```
-
-### Pull Request
-
-* Create a commit with your changes and push them to a
-  [fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo).
-* Create a [pull request on
-  Github](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
-* Pull request title and message (and PR title and description) must adhere to
-  [conventionalcommits](https://www.conventionalcommits.org).
-* Pull request body should describe _motivation_.
-
-
-## Resources
-* [Athena CREATE TABLE AS](https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html)
-* [dbt-labs/dbt-core](https://github.com/dbt-labs/dbt-core)
-* [laughingman7743/PyAthena](https://github.com/laughingman7743/PyAthena)
+See [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to this project.
 
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nicor88"><img src="https://avatars.githubusercontent.com/u/6278547?v=4?s=100" width="100px;" alt="nicor88"/><br /><sub><b>nicor88</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=nicor88" title="Code">💻</a> <a href="#maintenance-nicor88" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nicor88"><img src="https://avatars.githubusercontent.com/u/6278547?v=4?s=100" width="100px;" alt="nicor88"/><br /><sub><b>nicor88</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=nicor88" title="Code">💻</a> <a href="#maintenance-nicor88" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Anicor88" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://jessedobbelae.re"><img src="https://avatars.githubusercontent.com/u/1352979?v=4?s=100" width="100px;" alt="Jesse Dobbelaere"/><br /><sub><b>Jesse Dobbelaere</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ajessedobbelaere" title="Bug reports">🐛</a> <a href="#maintenance-jessedobbelaere" title="Maintenance">🚧</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/lemiffe"><img src="https://avatars.githubusercontent.com/u/7487772?v=4?s=100" width="100px;" alt="Lemiffe"/><br /><sub><b>Lemiffe</b></sub></a><br /><a href="#design-lemiffe" title="Design">🎨</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Jrmyy"><img src="https://avatars.githubusercontent.com/u/9251353?v=4?s=100" width="100px;" alt="Jérémy Guiselin"/><br /><sub><b>Jérémy Guiselin</b></sub></a><br /><a href="#maintenance-Jrmyy" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Jrmyy"><img src="https://avatars.githubusercontent.com/u/9251353?v=4?s=100" width="100px;" alt="Jérémy Guiselin"/><br /><sub><b>Jérémy Guiselin</b></sub></a><br /><a href="#maintenance-Jrmyy" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/commits?author=Jrmyy" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3AJrmyy" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tomme"><img src="https://avatars.githubusercontent.com/u/932895?v=4?s=100" width="100px;" alt="Tom"/><br /><sub><b>Tom</b></sub></a><br /><a href="#maintenance-Tomme" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/commits?author=Tomme" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/mattiamatrix"><img src="https://avatars.githubusercontent.com/u/5013654?v=4?s=100" width="100px;" alt="Mattia"/><br /><sub><b>Mattia</b></sub></a><br /><a href="#maintenance-mattiamatrix" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Gatsby-Lee"><img src="https://avatars.githubusercontent.com/u/22950880?v=4?s=100" width="100px;" alt="Gatsby Lee"/><br /><sub><b>Gatsby Lee</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3AGatsby-Lee" title="Bug reports">🐛</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BrechtDeVlieger"><img src="https://avatars.githubusercontent.com/u/12074972?v=4?s=100" width="100px;" alt="BrechtDeVlieger"/><br /><sub><b>BrechtDeVlieger</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3ABrechtDeVlieger" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/aartaria"><img src="https://avatars.githubusercontent.com/u/10273710?v=4?s=100" width="100px;" alt="Andrea Artaria"/><br /><sub><b>Andrea Artaria</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Aaartaria" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/maiarareinaldo"><img src="https://avatars.githubusercontent.com/u/72740386?v=4?s=100" width="100px;" alt="Maiara Reinaldo"/><br /><sub><b>Maiara Reinaldo</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Amaiarareinaldo" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/henriblancke"><img src="https://avatars.githubusercontent.com/u/1708162?v=4?s=100" width="100px;" alt="Henri Blancke"/><br /><sub><b>Henri Blancke</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=henriblancke" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ahenriblancke" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/svdimchenko"><img src="https://avatars.githubusercontent.com/u/39801237?v=4?s=100" width="100px;" alt="Serhii Dimchenko"/><br /><sub><b>Serhii Dimchenko</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=svdimchenko" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Asvdimchenko" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.4.3 Summary: The
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.4.4 Summary: The
 athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
 dbt-athena/dbt-athena Description-Content-Type: text/markdown License-File:
 LICENSE.txt
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
    dbt-athena-long.png] [https://badge.fury.io/py/dbt-athena-community.svg]
                 [https://img.shields.io/badge/%20imports-isort-
     %231674b1?style=flat&labelColor=ef8336] [https://img.shields.io/badge/
@@ -30,55 +30,59 @@
 athena/dbt-athena.git` ### Prerequisites To start, you will need an S3 bucket,
 for instance `my-bucket` and an Athena database: ```sql CREATE DATABASE IF NOT
 EXISTS analytics_dev COMMENT 'Analytics models generated by dbt (development)'
 LOCATION 's3://my-bucket/' WITH DBPROPERTIES ('creator'='Foo Bar',
 'email'='foo@bar.com'); ``` Notes: - Take note of your AWS region code (e.g.
 `us-west-2` or `eu-west-2`, etc.). - You can also use [AWS Glue](https://
 docs.aws.amazon.com/athena/latest/ug/glue-athena.html) to create and manage
-Athena databases. ### Credentials This plugin does not accept any credentials
-directly. Instead, [credentials are determined automatically](https://
-boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based
-on `aws cli`/`boto3` conventions and stored login info. You can configure the
-AWS profile name to use via `aws_profile_name`. Checkout DBT profile
-configuration below for details. ### Configuring your profile A dbt profile can
-be configured to run against AWS Athena using the following configuration: |
-Option | Description | Required? | Example | |------------------|--------------
-------------------------------------------------------------------|-----------
-|------------------------------------------| | s3_staging_dir | S3 location to
+Athena databases. ### Credentials Credentials can be passed directly to the
+adapter, or they can be [determined automatically](https://boto3.amazonaws.com/
+v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3`
+conventions. You can either: - configure `aws_access_key_id` and
+`aws_secret_access_key` - configure `aws_profile_name` to match a profile
+defined in your AWS credentials file Checkout DBT profile configuration below
+for details. ### Configuring your profile A dbt profile can be configured to
+run against AWS Athena using the following configuration: | Option |
+Description | Required? | Example | |-----------------------|------------------
+--------------------------------------------------------------|-----------|----
+----------------------------------------| | s3_staging_dir | S3 location to
 store Athena query results and metadata | Required | `s3://bucket/dbt/` | |
 s3_data_dir | Prefix for storing tables, if different from the connection's
 `s3_staging_dir` | Optional | `s3://bucket2/dbt/` | | s3_data_naming | How to
 generate table paths in `s3_data_dir` | Optional | `schema_table_unique` | |
 region_name | AWS region of your Athena instance | Required | `eu-west-1` | |
 schema | Specify the schema (Athena database) to build models into (lowercase
 **only**) | Required | `dbt` | | database | Specify the database (Data catalog)
 to build models into (lowercase **only**) | Required | `awsdatacatalog` | |
 poll_interval | Interval in seconds to use for polling the status of query
-results in Athena | Optional | `5` | | aws_profile_name | Profile to use from
-your AWS shared credentials file. | Optional | `my-profile` | | work_group |
-Identifier of Athena workgroup | Optional | `my-custom-workgroup` | |
-num_retries | Number of times to retry a failing query | Optional | `3` | |
-lf_tags | Default lf tags to apply to any database created by dbt | Optional |
-`{"origin": "dbt", "team": "analytics"}` | **Example profiles.yml entry:**
-```yaml athena: target: dev outputs: dev: type: athena s3_staging_dir: s3://
-athena-query-results/dbt/ s3_data_dir: s3://your_s3_bucket/dbt/ s3_data_naming:
-schema_table region_name: eu-west-1 schema: dbt database: awsdatacatalog
-aws_profile_name: my-profile work_group: my-workgroup lf_tags: origin: dbt
-team: analytics ``` _Additional information_ * `threads` is supported *
-`database` and `catalog` can be used interchangeably ## Models ### Table
-Configuration * `external_location` (`default=none`) * If set, the full S3 path
-in which the table will be saved. (Does not work with Iceberg table). *
-`partitioned_by` (`default=none`) * An array list of columns by which the table
-will be partitioned * Limited to creation of 100 partitions (_currently_) *
-`bucketed_by` (`default=none`) * An array list of columns to bucket data,
-ignored if using Iceberg * `bucket_count` (`default=none`) * The number of
-buckets for bucketing your data, ignored if using Iceberg * `table_type`
-(`default='hive'`) * The type of table * Supports `hive` or `iceberg` *
-`format` (`default='parquet'`) * The data format for the table * Supports
-`ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
+results in Athena | Optional | `5` | | aws_access_key_id | Access key ID of the
+user performing requests. | Optional | `AKIAIOSFODNN7EXAMPLE` | |
+aws_secret_access_key | Secret access key of the user performing requests |
+Optional | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` | | aws_profile_name |
+Profile to use from your AWS shared credentials file. | Optional | `my-profile`
+| | work_group | Identifier of Athena workgroup | Optional | `my-custom-
+workgroup` | | num_retries | Number of times to retry a failing query |
+Optional | `3` | | lf_tags | Default lf tags to apply to any database created
+by dbt | Optional | `{"origin": "dbt", "team": "analytics"}` | **Example
+profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type: athena
+s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
+your_s3_bucket/dbt/ s3_data_naming: schema_table region_name: eu-west-1 schema:
+dbt database: awsdatacatalog aws_profile_name: my-profile work_group: my-
+workgroup lf_tags: origin: dbt team: analytics ``` _Additional information_ *
+`threads` is supported * `database` and `catalog` can be used interchangeably
+## Models ### Table Configuration * `external_location` (`default=none`) * If
+set, the full S3 path in which the table will be saved. (Does not work with
+Iceberg table). * `partitioned_by` (`default=none`) * An array list of columns
+by which the table will be partitioned * Limited to creation of 100 partitions
+(_currently_) * `bucketed_by` (`default=none`) * An array list of columns to
+bucket data, ignored if using Iceberg * `bucket_count` (`default=none`) * The
+number of buckets for bucketing your data, ignored if using Iceberg *
+`table_type` (`default='hive'`) * The type of table * Supports `hive` or
+`iceberg` * `format` (`default='parquet'`) * The data format for the table *
+Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
 (`default=none`) * The compression type to use for any storage format that
 allows compression to be specified. To see which options are available, check
 out [CREATE TABLE AS][create-table-as] * `field_delimiter` (`default=none`) *
 Custom field delimiter, for when format is set to `TEXTFILE` *
 `table_properties`: table properties to add to the table, valid for Iceberg
 only * `lf_tags` (`default=none`) * lf tags to associate with the table *
 format: `{"tag1": "value1", "tag2": "value2"}` * `lf_tags_columns`
@@ -121,42 +125,52 @@
 partitions, therefore use the `partitioned_by` config to add specific bucketing
 conditions. Iceberg supports several table formats for data : `PARQUET`, `AVRO`
 and `ORC`. It is possible to use iceberg in an incremental fashion,
 specifically 2 strategies are supported: * `append`: new records are appended
 to the table, this can lead to duplicates * `merge`: must be used in
 combination with `unique_key` and it's only available with Engine version 3. It
 performs an upsert, new record are added, and record already existing are
-updated ### High available table materialization The current implementation of
-the table materialization can lead to downtime, as target table is dropped and
-re-created. To have the less destructive behavior it's possible to use
-`table='table_hive_ha'` materialization. **table_hive_ha** leverage the table
-versions feature of glue catalog, creating a tmp table and swapping the target
-table to the location of the tmp table. This materialization is only available
-for `table_type=hive` and requires using unique locations. ``` {{ config
-( materialized='table_hive_ha', format='parquet', partition_by=['status'],
-s3_data_naming='table_unique' ) }} select 'a' as user_id, 'pi' as user_name,
-'active' as status union all select 'b' as user_id, 'sh' as user_name,
-'disabled' as status ``` By default, the materialization keeps the last 4 table
-versions, you can change it that setting `versions_to_keep`. #### Known issues
-* When swapping from a table with partitions to a table without (and the other
-way around), there could be a little downtime. In case high performances are
-needed consider bucketing instead of partitions * By default, Glue "duplicate"
-the versions internally, so the last 2 versions of a table point to the same
-location * It's recommended to have versions_to_keep>= 4, as this will avoid to
-have the older location removed * The macro athena__end_of_time needs to be
-overwritten by the user if using Athena v3 since it requires a precision
-parameter for timestamps ## Snapshots The adapter supports snapshot
-materialization. It supports both timestamp and check strategy. To create a
-snapshot create a snapshot file in the snapshots directory. If directory does
-not exist create one. ### Timestamp strategy To use the timestamp strategy
-refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
-strategy-recommended) ### Check strategy To use the check strategy refer to the
-[dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
-Hard-deletes The materialization also supports invalidating hard deletes. Check
-the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
+updated. If `delete_condition` is provided in the model config, it can also
+delete records based on the provided condition (SQL condition). You can use any
+column of the incremental table (`src`) or the final table (`target`). You must
+prefix the column by the name of the table to prevent `Column is ambiguous`
+error. ```sql {{ config( materialized='incremental', table_type='iceberg',
+incremental_strategy='merge', unique_key='user_id',
+delete_condition="src.status != 'active' and target.my_date < now() - interval
+'2' year" format='parquet', ) }} SELECT 'A' AS user_id, 'pi' AS name, 'active'
+AS status, 17.89 AS cost, 1 AS quantity, 100000000 AS quantity_big,
+current_date AS my_date ``` ### High available table materialization The
+current implementation of the table materialization can lead to downtime, as
+target table is dropped and re-created. To have the less destructive behavior
+it's possible to use `table='table_hive_ha'` materialization. **table_hive_ha**
+leverage the table versions feature of glue catalog, creating a tmp table and
+swapping the target table to the location of the tmp table. This
+materialization is only available for `table_type=hive` and requires using
+unique locations. ``` {{ config( materialized='table_hive_ha',
+format='parquet', partition_by=['status'], s3_data_naming='table_unique' ) }}
+select 'a' as user_id, 'pi' as user_name, 'active' as status union all select
+'b' as user_id, 'sh' as user_name, 'disabled' as status ``` By default, the
+materialization keeps the last 4 table versions, you can change it that setting
+`versions_to_keep`. #### Known issues * When swapping from a table with
+partitions to a table without (and the other way around), there could be a
+little downtime. In case high performances are needed consider bucketing
+instead of partitions * By default, Glue "duplicate" the versions internally,
+so the last 2 versions of a table point to the same location * It's recommended
+to have versions_to_keep>= 4, as this will avoid to have the older location
+removed * The macro athena__end_of_time needs to be overwritten by the user if
+using Athena v3 since it requires a precision parameter for timestamps ##
+Snapshots The adapter supports snapshot materialization. It supports both
+timestamp and check strategy. To create a snapshot create a snapshot file in
+the snapshots directory. If directory does not exist create one. ### Timestamp
+strategy To use the timestamp strategy refer to the [dbt docs](https://
+docs.getdbt.com/docs/build/snapshots#timestamp-strategy-recommended) ### Check
+strategy To use the check strategy refer to the [dbt docs](https://
+docs.getdbt.com/docs/build/snapshots#check-strategy) ### Hard-deletes The
+materialization also supports invalidating hard deletes. Check the [docs]
+(https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
 understand usage. ### Working example seed file -
 employent_indicators_november_2022_csv_tables.csv ```
 Series_reference,Period,Data_value,Suppressed MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803, MEIM.S1WA,1999.06,65792, MEIM.S1WA,1999.07,66194,
 MEIM.S1WA,1999.08,67259, MEIM.S1WA,1999.09,69691, MEIM.S1WA,1999.1,72475,
 MEIM.S1WA,1999.11,79263, MEIM.S1WA,1999.12,86540, MEIM.S1WA,2000.01,82552,
 MEIM.S1WA,2000.02,81709, MEIM.S1WA,2000.03,84126, MEIM.S1WA,2000.04,77089,
@@ -180,37 +194,24 @@
 the incremental model. * Tables, schemas and database should only be lowercase
 * In order to avoid potential conflicts, make sure [`dbt-athena-adapter`]
 (https://github.com/Tomme/dbt-athena) is not installed in the target
 environment. See https://github.com/dbt-athena/dbt-athena/issues/103 for more
 details. * Snapshot does not support dropping columns from the source table. If
 you drop a column make sure to drop the column from the snapshot as well.
 Another workaround is to NULL the column in the snapshot definition to preserve
-history ## Contributing This connector works with Python from 3.7 to 3.11. ###
-Getting started In order to start developing on this adapter clone the repo and
-run this make command (see [Makefile](Makefile)) : ```bash make setup ``` It
-will : 1. Install all dependencies. 2. Install pre-commit hooks. 3. Generate
-your `.env` file Next, adjust `.env` file by configuring the environment
-variables to match your Athena development environment. ### Running tests We
-have 2 different types of testing: * **unit testing**: you can run this type of
-tests running `make unit_test` * **functional testing**: you must have an AWS
-account with Athena setup in order to launch this type of tests and have a
-`.env` file in place with the right values. You can run this type of tests
-running `make functional_test` All type of tests can be run using `make`:
-```bash make test ``` ### Pull Request * Create a commit with your changes and
-push them to a [fork](https://docs.github.com/en/get-started/quickstart/fork-a-
-repo). * Create a [pull request on Github](https://docs.github.com/en/github/
-collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-
-requests/creating-a-pull-request-from-a-fork). * Pull request title and message
-(and PR title and description) must adhere to [conventionalcommits](https://
-www.conventionalcommits.org). * Pull request body should describe _motivation_.
-## Resources * [Athena CREATE TABLE AS](https://docs.aws.amazon.com/athena/
-latest/ug/create-table-as.html) * [dbt-labs/dbt-core](https://github.com/dbt-
-labs/dbt-core) * [laughingman7743/PyAthena](https://github.com/laughingman7743/
-PyAthena) ## Contributors â¨ Thanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)):
-    [nicor88]          [Jesse       [Lemiffe] [JÃ©rÃ©my_Guisel      [Tom]       [Mattia]
-     nicor88         Dobbelaere]     Lemiffe   JÃ©rÃ©my_Guisel       Tom         Mattia
-    ð» ð�Jesse_Dobbelaere    ð¨       ð§         ð§ ð�  ð§
-                      ð ð§
+history ## Contributing See [CONTRIBUTING](CONTRIBUTING.md) for more
+information on how to contribute to this project. ## Contributors â¨ Thanks
+goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
+en/emoji-key)):
+        [nicor88]               [Jesse       [Lemiffe]  [JÃ©rÃ©my_Guiselin      [Tom]       [Mattia] [Gatsby
+         nicor88              Dobbelaere]     Lemiffe    JÃ©rÃ©my_Guiselin       Tom         Mattia    Lee]
+      ð» ð§ ð�Jesse_Dobbelaere    ð¨    ð§ ð» �    ð§ ð�  ð� Gatsby
+                               ð ð§                                                           Lee
+                                                                                                           ð
+      [BrechtDeVlieger]    [Andrea_Artaria]   [Maiara     [Henri_Blancke]          [Serhii
+       BrechtDeVlieger      Andrea_Artaria   Reinaldo]     Henri_Blancke         Dimchenko]
+             ð            ð     Maiara         ð» ðSerhii_Dimchenko
+                                             Reinaldo                             ð» ð
+                                               ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `dbt-athena-community-1.4.3/README.md` & `dbt-athena-community-1.4.4/dbt_athena_community.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: dbt-athena-community
+Version: 1.4.4
+Summary: The athena adapter plugin for dbt (data build tool)
+Home-page: https://github.com/dbt-athena/dbt-athena
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 <p align="center">
     <img src="https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/dbt-athena-long.png" />
     <a href="https://pypi.org/project/dbt-athena-community/"><img src="https://badge.fury.io/py/dbt-athena-community.svg" /></a>
     <a href="https://pycqa.github.io/isort/"><img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" /></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
     <a href="https://pepy.tech/project/dbt-athena-community"><img src="https://pepy.tech/badge/dbt-athena-community/month" /></a>
 </p>
@@ -55,34 +63,39 @@
 
 Notes:
 - Take note of your AWS region code (e.g. `us-west-2` or `eu-west-2`, etc.).
 - You can also use [AWS Glue](https://docs.aws.amazon.com/athena/latest/ug/glue-athena.html) to create and manage Athena databases.
 
 ### Credentials
 
-This plugin does not accept any credentials directly. Instead, [credentials are determined automatically](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3` conventions and
-stored login info. You can configure the AWS profile name to use via `aws_profile_name`. Checkout DBT profile configuration below for details.
+Credentials can be passed directly to the adapter, or they can be [determined automatically](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3` conventions.
+You can either:
+- configure `aws_access_key_id` and `aws_secret_access_key`
+- configure `aws_profile_name` to match a profile defined in your AWS credentials file
+Checkout DBT profile configuration below for details.
 
 ### Configuring your profile
 
 A dbt profile can be configured to run against AWS Athena using the following configuration:
 
-| Option           | Description                                                                    | Required? | Example                                  |
-|------------------|--------------------------------------------------------------------------------|-----------|------------------------------------------|
-| s3_staging_dir   | S3 location to store Athena query results and metadata                         | Required  | `s3://bucket/dbt/`                       |
-| s3_data_dir      | Prefix for storing tables, if different from the connection's `s3_staging_dir` | Optional  | `s3://bucket2/dbt/`                      |
-| s3_data_naming   | How to generate table paths in `s3_data_dir`                                   | Optional  | `schema_table_unique`                    |
-| region_name      | AWS region of your Athena instance                                             | Required  | `eu-west-1`                              |
-| schema           | Specify the schema (Athena database) to build models into (lowercase **only**) | Required  | `dbt`                                    |
-| database         | Specify the database (Data catalog) to build models into (lowercase **only**)  | Required  | `awsdatacatalog`                         |
-| poll_interval    | Interval in seconds to use for polling the status of query results in Athena   | Optional  | `5`                                      |
-| aws_profile_name | Profile to use from your AWS shared credentials file.                          | Optional  | `my-profile`                             |
-| work_group       | Identifier of Athena workgroup                                                 | Optional  | `my-custom-workgroup`                    |
-| num_retries      | Number of times to retry a failing query                                       | Optional  | `3`                                      |
-| lf_tags          | Default lf tags to apply to any database created by dbt                        | Optional  | `{"origin": "dbt", "team": "analytics"}` |
+| Option                | Description                                                                    | Required? | Example                                    |
+|-----------------------|--------------------------------------------------------------------------------|-----------|--------------------------------------------|
+| s3_staging_dir        | S3 location to store Athena query results and metadata                         | Required  | `s3://bucket/dbt/`                         |
+| s3_data_dir           | Prefix for storing tables, if different from the connection's `s3_staging_dir` | Optional  | `s3://bucket2/dbt/`                        |
+| s3_data_naming        | How to generate table paths in `s3_data_dir`                                   | Optional  | `schema_table_unique`                      |
+| region_name           | AWS region of your Athena instance                                             | Required  | `eu-west-1`                                |
+| schema                | Specify the schema (Athena database) to build models into (lowercase **only**) | Required  | `dbt`                                      |
+| database              | Specify the database (Data catalog) to build models into (lowercase **only**)  | Required  | `awsdatacatalog`                           |
+| poll_interval         | Interval in seconds to use for polling the status of query results in Athena   | Optional  | `5`                                        |
+| aws_access_key_id     | Access key ID of the user performing requests.                                 | Optional  | `AKIAIOSFODNN7EXAMPLE`                     |
+| aws_secret_access_key | Secret access key of the user performing requests                              | Optional  | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` |
+| aws_profile_name      | Profile to use from your AWS shared credentials file.                          | Optional  | `my-profile`                               |
+| work_group            | Identifier of Athena workgroup                                                 | Optional  | `my-custom-workgroup`                      |
+| num_retries           | Number of times to retry a failing query                                       | Optional  | `3`                                        |
+| lf_tags               | Default lf tags to apply to any database created by dbt                        | Optional  | `{"origin": "dbt", "team": "analytics"}`   |
 
 **Example profiles.yml entry:**
 ```yaml
 athena:
   target: dev
   outputs:
     dev:
@@ -210,15 +223,39 @@
 Iceberg supports bucketing as hidden partitions, therefore use the `partitioned_by` config to add specific bucketing conditions.
 
 Iceberg supports several table formats for data : `PARQUET`, `AVRO` and `ORC`.
 
 It is possible to use iceberg in an incremental fashion, specifically 2 strategies are supported:
 * `append`: new records are appended to the table, this can lead to duplicates
 * `merge`: must be used in combination with `unique_key` and it's only available with Engine version 3.
-   It performs an upsert, new record are added, and record already existing are updated
+   It performs an upsert, new record are added, and record already existing are updated. If
+   `delete_condition` is provided in the model config, it can also delete records based on the
+   provided condition (SQL condition). You can use any column of the incremental table (`src`) or
+   the final table (`target`). You must prefix the column by the name of the table to prevent
+   `Column is ambiguous` error.
+
+```sql
+{{ config(
+    materialized='incremental',
+    table_type='iceberg',
+    incremental_strategy='merge',
+    unique_key='user_id',
+    delete_condition="src.status != 'active' and target.my_date < now() - interval '2' year"
+    format='parquet',
+) }}
+
+SELECT
+	'A' AS user_id,
+	'pi' AS name,
+	'active' AS status,
+	17.89 AS cost,
+	1 AS quantity,
+	100000000 AS quantity_big,
+	current_date AS my_date
+```
 
 ### High available table materialization
 The current implementation of the table materialization can lead to downtime, as target table is dropped and re-created.
 To have the less destructive behavior it's possible to use `table='table_hive_ha'` materialization.
 **table_hive_ha** leverage the table versions feature of glue catalog, creating a tmp table and swapping
 the target table to the location of the tmp table.
 This materialization is only available for `table_type=hive` and requires using unique locations.
@@ -373,76 +410,41 @@
   See https://github.com/dbt-athena/dbt-athena/issues/103 for more details.
 
 * Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
 
 
 ## Contributing
 
-This connector works with Python from 3.7 to 3.11.
-
-### Getting started
-
-In order to start developing on this adapter clone the repo and run this make command (see [Makefile](Makefile)) :
-
-```bash
-make setup
-```
-
-It will :
-1. Install all dependencies.
-2. Install pre-commit hooks.
-3. Generate your `.env` file
-
-Next, adjust `.env` file by configuring the environment variables to match your Athena development environment.
-
-### Running tests
-
-We have 2 different types of testing:
-* **unit testing**: you can run this type of tests running `make unit_test`
-* **functional testing**: you must have an AWS account with Athena setup in order to launch this type of tests and have a `.env` file in place with the right values.
-  You can run this type of tests running `make functional_test`
-
-All type of tests can be run using `make`:
-```bash
-make test
-```
-
-### Pull Request
-
-* Create a commit with your changes and push them to a
-  [fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo).
-* Create a [pull request on
-  Github](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
-* Pull request title and message (and PR title and description) must adhere to
-  [conventionalcommits](https://www.conventionalcommits.org).
-* Pull request body should describe _motivation_.
-
-
-## Resources
-* [Athena CREATE TABLE AS](https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html)
-* [dbt-labs/dbt-core](https://github.com/dbt-labs/dbt-core)
-* [laughingman7743/PyAthena](https://github.com/laughingman7743/PyAthena)
+See [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to this project.
 
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nicor88"><img src="https://avatars.githubusercontent.com/u/6278547?v=4?s=100" width="100px;" alt="nicor88"/><br /><sub><b>nicor88</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=nicor88" title="Code">💻</a> <a href="#maintenance-nicor88" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nicor88"><img src="https://avatars.githubusercontent.com/u/6278547?v=4?s=100" width="100px;" alt="nicor88"/><br /><sub><b>nicor88</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=nicor88" title="Code">💻</a> <a href="#maintenance-nicor88" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Anicor88" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://jessedobbelae.re"><img src="https://avatars.githubusercontent.com/u/1352979?v=4?s=100" width="100px;" alt="Jesse Dobbelaere"/><br /><sub><b>Jesse Dobbelaere</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ajessedobbelaere" title="Bug reports">🐛</a> <a href="#maintenance-jessedobbelaere" title="Maintenance">🚧</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/lemiffe"><img src="https://avatars.githubusercontent.com/u/7487772?v=4?s=100" width="100px;" alt="Lemiffe"/><br /><sub><b>Lemiffe</b></sub></a><br /><a href="#design-lemiffe" title="Design">🎨</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Jrmyy"><img src="https://avatars.githubusercontent.com/u/9251353?v=4?s=100" width="100px;" alt="Jérémy Guiselin"/><br /><sub><b>Jérémy Guiselin</b></sub></a><br /><a href="#maintenance-Jrmyy" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Jrmyy"><img src="https://avatars.githubusercontent.com/u/9251353?v=4?s=100" width="100px;" alt="Jérémy Guiselin"/><br /><sub><b>Jérémy Guiselin</b></sub></a><br /><a href="#maintenance-Jrmyy" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/commits?author=Jrmyy" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3AJrmyy" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tomme"><img src="https://avatars.githubusercontent.com/u/932895?v=4?s=100" width="100px;" alt="Tom"/><br /><sub><b>Tom</b></sub></a><br /><a href="#maintenance-Tomme" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/commits?author=Tomme" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/mattiamatrix"><img src="https://avatars.githubusercontent.com/u/5013654?v=4?s=100" width="100px;" alt="Mattia"/><br /><sub><b>Mattia</b></sub></a><br /><a href="#maintenance-mattiamatrix" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Gatsby-Lee"><img src="https://avatars.githubusercontent.com/u/22950880?v=4?s=100" width="100px;" alt="Gatsby Lee"/><br /><sub><b>Gatsby Lee</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3AGatsby-Lee" title="Bug reports">🐛</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BrechtDeVlieger"><img src="https://avatars.githubusercontent.com/u/12074972?v=4?s=100" width="100px;" alt="BrechtDeVlieger"/><br /><sub><b>BrechtDeVlieger</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3ABrechtDeVlieger" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/aartaria"><img src="https://avatars.githubusercontent.com/u/10273710?v=4?s=100" width="100px;" alt="Andrea Artaria"/><br /><sub><b>Andrea Artaria</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Aaartaria" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/maiarareinaldo"><img src="https://avatars.githubusercontent.com/u/72740386?v=4?s=100" width="100px;" alt="Maiara Reinaldo"/><br /><sub><b>Maiara Reinaldo</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Amaiarareinaldo" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/henriblancke"><img src="https://avatars.githubusercontent.com/u/1708162?v=4?s=100" width="100px;" alt="Henri Blancke"/><br /><sub><b>Henri Blancke</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=henriblancke" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ahenriblancke" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/svdimchenko"><img src="https://avatars.githubusercontent.com/u/39801237?v=4?s=100" width="100px;" alt="Serhii Dimchenko"/><br /><sub><b>Serhii Dimchenko</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=svdimchenko" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Asvdimchenko" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,7 +1,11 @@
+Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.4.4 Summary: The
+athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
+dbt-athena/dbt-athena Description-Content-Type: text/markdown License-File:
+LICENSE.txt
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
    dbt-athena-long.png] [https://badge.fury.io/py/dbt-athena-community.svg]
                 [https://img.shields.io/badge/%20imports-isort-
     %231674b1?style=flat&labelColor=ef8336] [https://img.shields.io/badge/
  code%20style-black-000000.svg] [https://pepy.tech/badge/dbt-athena-community/
                                     month]
 ## Features * Supports dbt version `1.4.*` * Supports [Seeds][seeds] *
@@ -26,55 +30,59 @@
 athena/dbt-athena.git` ### Prerequisites To start, you will need an S3 bucket,
 for instance `my-bucket` and an Athena database: ```sql CREATE DATABASE IF NOT
 EXISTS analytics_dev COMMENT 'Analytics models generated by dbt (development)'
 LOCATION 's3://my-bucket/' WITH DBPROPERTIES ('creator'='Foo Bar',
 'email'='foo@bar.com'); ``` Notes: - Take note of your AWS region code (e.g.
 `us-west-2` or `eu-west-2`, etc.). - You can also use [AWS Glue](https://
 docs.aws.amazon.com/athena/latest/ug/glue-athena.html) to create and manage
-Athena databases. ### Credentials This plugin does not accept any credentials
-directly. Instead, [credentials are determined automatically](https://
-boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based
-on `aws cli`/`boto3` conventions and stored login info. You can configure the
-AWS profile name to use via `aws_profile_name`. Checkout DBT profile
-configuration below for details. ### Configuring your profile A dbt profile can
-be configured to run against AWS Athena using the following configuration: |
-Option | Description | Required? | Example | |------------------|--------------
-------------------------------------------------------------------|-----------
-|------------------------------------------| | s3_staging_dir | S3 location to
+Athena databases. ### Credentials Credentials can be passed directly to the
+adapter, or they can be [determined automatically](https://boto3.amazonaws.com/
+v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3`
+conventions. You can either: - configure `aws_access_key_id` and
+`aws_secret_access_key` - configure `aws_profile_name` to match a profile
+defined in your AWS credentials file Checkout DBT profile configuration below
+for details. ### Configuring your profile A dbt profile can be configured to
+run against AWS Athena using the following configuration: | Option |
+Description | Required? | Example | |-----------------------|------------------
+--------------------------------------------------------------|-----------|----
+----------------------------------------| | s3_staging_dir | S3 location to
 store Athena query results and metadata | Required | `s3://bucket/dbt/` | |
 s3_data_dir | Prefix for storing tables, if different from the connection's
 `s3_staging_dir` | Optional | `s3://bucket2/dbt/` | | s3_data_naming | How to
 generate table paths in `s3_data_dir` | Optional | `schema_table_unique` | |
 region_name | AWS region of your Athena instance | Required | `eu-west-1` | |
 schema | Specify the schema (Athena database) to build models into (lowercase
 **only**) | Required | `dbt` | | database | Specify the database (Data catalog)
 to build models into (lowercase **only**) | Required | `awsdatacatalog` | |
 poll_interval | Interval in seconds to use for polling the status of query
-results in Athena | Optional | `5` | | aws_profile_name | Profile to use from
-your AWS shared credentials file. | Optional | `my-profile` | | work_group |
-Identifier of Athena workgroup | Optional | `my-custom-workgroup` | |
-num_retries | Number of times to retry a failing query | Optional | `3` | |
-lf_tags | Default lf tags to apply to any database created by dbt | Optional |
-`{"origin": "dbt", "team": "analytics"}` | **Example profiles.yml entry:**
-```yaml athena: target: dev outputs: dev: type: athena s3_staging_dir: s3://
-athena-query-results/dbt/ s3_data_dir: s3://your_s3_bucket/dbt/ s3_data_naming:
-schema_table region_name: eu-west-1 schema: dbt database: awsdatacatalog
-aws_profile_name: my-profile work_group: my-workgroup lf_tags: origin: dbt
-team: analytics ``` _Additional information_ * `threads` is supported *
-`database` and `catalog` can be used interchangeably ## Models ### Table
-Configuration * `external_location` (`default=none`) * If set, the full S3 path
-in which the table will be saved. (Does not work with Iceberg table). *
-`partitioned_by` (`default=none`) * An array list of columns by which the table
-will be partitioned * Limited to creation of 100 partitions (_currently_) *
-`bucketed_by` (`default=none`) * An array list of columns to bucket data,
-ignored if using Iceberg * `bucket_count` (`default=none`) * The number of
-buckets for bucketing your data, ignored if using Iceberg * `table_type`
-(`default='hive'`) * The type of table * Supports `hive` or `iceberg` *
-`format` (`default='parquet'`) * The data format for the table * Supports
-`ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
+results in Athena | Optional | `5` | | aws_access_key_id | Access key ID of the
+user performing requests. | Optional | `AKIAIOSFODNN7EXAMPLE` | |
+aws_secret_access_key | Secret access key of the user performing requests |
+Optional | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` | | aws_profile_name |
+Profile to use from your AWS shared credentials file. | Optional | `my-profile`
+| | work_group | Identifier of Athena workgroup | Optional | `my-custom-
+workgroup` | | num_retries | Number of times to retry a failing query |
+Optional | `3` | | lf_tags | Default lf tags to apply to any database created
+by dbt | Optional | `{"origin": "dbt", "team": "analytics"}` | **Example
+profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type: athena
+s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
+your_s3_bucket/dbt/ s3_data_naming: schema_table region_name: eu-west-1 schema:
+dbt database: awsdatacatalog aws_profile_name: my-profile work_group: my-
+workgroup lf_tags: origin: dbt team: analytics ``` _Additional information_ *
+`threads` is supported * `database` and `catalog` can be used interchangeably
+## Models ### Table Configuration * `external_location` (`default=none`) * If
+set, the full S3 path in which the table will be saved. (Does not work with
+Iceberg table). * `partitioned_by` (`default=none`) * An array list of columns
+by which the table will be partitioned * Limited to creation of 100 partitions
+(_currently_) * `bucketed_by` (`default=none`) * An array list of columns to
+bucket data, ignored if using Iceberg * `bucket_count` (`default=none`) * The
+number of buckets for bucketing your data, ignored if using Iceberg *
+`table_type` (`default='hive'`) * The type of table * Supports `hive` or
+`iceberg` * `format` (`default='parquet'`) * The data format for the table *
+Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
 (`default=none`) * The compression type to use for any storage format that
 allows compression to be specified. To see which options are available, check
 out [CREATE TABLE AS][create-table-as] * `field_delimiter` (`default=none`) *
 Custom field delimiter, for when format is set to `TEXTFILE` *
 `table_properties`: table properties to add to the table, valid for Iceberg
 only * `lf_tags` (`default=none`) * lf tags to associate with the table *
 format: `{"tag1": "value1", "tag2": "value2"}` * `lf_tags_columns`
@@ -117,42 +125,52 @@
 partitions, therefore use the `partitioned_by` config to add specific bucketing
 conditions. Iceberg supports several table formats for data : `PARQUET`, `AVRO`
 and `ORC`. It is possible to use iceberg in an incremental fashion,
 specifically 2 strategies are supported: * `append`: new records are appended
 to the table, this can lead to duplicates * `merge`: must be used in
 combination with `unique_key` and it's only available with Engine version 3. It
 performs an upsert, new record are added, and record already existing are
-updated ### High available table materialization The current implementation of
-the table materialization can lead to downtime, as target table is dropped and
-re-created. To have the less destructive behavior it's possible to use
-`table='table_hive_ha'` materialization. **table_hive_ha** leverage the table
-versions feature of glue catalog, creating a tmp table and swapping the target
-table to the location of the tmp table. This materialization is only available
-for `table_type=hive` and requires using unique locations. ``` {{ config
-( materialized='table_hive_ha', format='parquet', partition_by=['status'],
-s3_data_naming='table_unique' ) }} select 'a' as user_id, 'pi' as user_name,
-'active' as status union all select 'b' as user_id, 'sh' as user_name,
-'disabled' as status ``` By default, the materialization keeps the last 4 table
-versions, you can change it that setting `versions_to_keep`. #### Known issues
-* When swapping from a table with partitions to a table without (and the other
-way around), there could be a little downtime. In case high performances are
-needed consider bucketing instead of partitions * By default, Glue "duplicate"
-the versions internally, so the last 2 versions of a table point to the same
-location * It's recommended to have versions_to_keep>= 4, as this will avoid to
-have the older location removed * The macro athena__end_of_time needs to be
-overwritten by the user if using Athena v3 since it requires a precision
-parameter for timestamps ## Snapshots The adapter supports snapshot
-materialization. It supports both timestamp and check strategy. To create a
-snapshot create a snapshot file in the snapshots directory. If directory does
-not exist create one. ### Timestamp strategy To use the timestamp strategy
-refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
-strategy-recommended) ### Check strategy To use the check strategy refer to the
-[dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
-Hard-deletes The materialization also supports invalidating hard deletes. Check
-the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
+updated. If `delete_condition` is provided in the model config, it can also
+delete records based on the provided condition (SQL condition). You can use any
+column of the incremental table (`src`) or the final table (`target`). You must
+prefix the column by the name of the table to prevent `Column is ambiguous`
+error. ```sql {{ config( materialized='incremental', table_type='iceberg',
+incremental_strategy='merge', unique_key='user_id',
+delete_condition="src.status != 'active' and target.my_date < now() - interval
+'2' year" format='parquet', ) }} SELECT 'A' AS user_id, 'pi' AS name, 'active'
+AS status, 17.89 AS cost, 1 AS quantity, 100000000 AS quantity_big,
+current_date AS my_date ``` ### High available table materialization The
+current implementation of the table materialization can lead to downtime, as
+target table is dropped and re-created. To have the less destructive behavior
+it's possible to use `table='table_hive_ha'` materialization. **table_hive_ha**
+leverage the table versions feature of glue catalog, creating a tmp table and
+swapping the target table to the location of the tmp table. This
+materialization is only available for `table_type=hive` and requires using
+unique locations. ``` {{ config( materialized='table_hive_ha',
+format='parquet', partition_by=['status'], s3_data_naming='table_unique' ) }}
+select 'a' as user_id, 'pi' as user_name, 'active' as status union all select
+'b' as user_id, 'sh' as user_name, 'disabled' as status ``` By default, the
+materialization keeps the last 4 table versions, you can change it that setting
+`versions_to_keep`. #### Known issues * When swapping from a table with
+partitions to a table without (and the other way around), there could be a
+little downtime. In case high performances are needed consider bucketing
+instead of partitions * By default, Glue "duplicate" the versions internally,
+so the last 2 versions of a table point to the same location * It's recommended
+to have versions_to_keep>= 4, as this will avoid to have the older location
+removed * The macro athena__end_of_time needs to be overwritten by the user if
+using Athena v3 since it requires a precision parameter for timestamps ##
+Snapshots The adapter supports snapshot materialization. It supports both
+timestamp and check strategy. To create a snapshot create a snapshot file in
+the snapshots directory. If directory does not exist create one. ### Timestamp
+strategy To use the timestamp strategy refer to the [dbt docs](https://
+docs.getdbt.com/docs/build/snapshots#timestamp-strategy-recommended) ### Check
+strategy To use the check strategy refer to the [dbt docs](https://
+docs.getdbt.com/docs/build/snapshots#check-strategy) ### Hard-deletes The
+materialization also supports invalidating hard deletes. Check the [docs]
+(https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
 understand usage. ### Working example seed file -
 employent_indicators_november_2022_csv_tables.csv ```
 Series_reference,Period,Data_value,Suppressed MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803, MEIM.S1WA,1999.06,65792, MEIM.S1WA,1999.07,66194,
 MEIM.S1WA,1999.08,67259, MEIM.S1WA,1999.09,69691, MEIM.S1WA,1999.1,72475,
 MEIM.S1WA,1999.11,79263, MEIM.S1WA,1999.12,86540, MEIM.S1WA,2000.01,82552,
 MEIM.S1WA,2000.02,81709, MEIM.S1WA,2000.03,84126, MEIM.S1WA,2000.04,77089,
@@ -176,37 +194,24 @@
 the incremental model. * Tables, schemas and database should only be lowercase
 * In order to avoid potential conflicts, make sure [`dbt-athena-adapter`]
 (https://github.com/Tomme/dbt-athena) is not installed in the target
 environment. See https://github.com/dbt-athena/dbt-athena/issues/103 for more
 details. * Snapshot does not support dropping columns from the source table. If
 you drop a column make sure to drop the column from the snapshot as well.
 Another workaround is to NULL the column in the snapshot definition to preserve
-history ## Contributing This connector works with Python from 3.7 to 3.11. ###
-Getting started In order to start developing on this adapter clone the repo and
-run this make command (see [Makefile](Makefile)) : ```bash make setup ``` It
-will : 1. Install all dependencies. 2. Install pre-commit hooks. 3. Generate
-your `.env` file Next, adjust `.env` file by configuring the environment
-variables to match your Athena development environment. ### Running tests We
-have 2 different types of testing: * **unit testing**: you can run this type of
-tests running `make unit_test` * **functional testing**: you must have an AWS
-account with Athena setup in order to launch this type of tests and have a
-`.env` file in place with the right values. You can run this type of tests
-running `make functional_test` All type of tests can be run using `make`:
-```bash make test ``` ### Pull Request * Create a commit with your changes and
-push them to a [fork](https://docs.github.com/en/get-started/quickstart/fork-a-
-repo). * Create a [pull request on Github](https://docs.github.com/en/github/
-collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-
-requests/creating-a-pull-request-from-a-fork). * Pull request title and message
-(and PR title and description) must adhere to [conventionalcommits](https://
-www.conventionalcommits.org). * Pull request body should describe _motivation_.
-## Resources * [Athena CREATE TABLE AS](https://docs.aws.amazon.com/athena/
-latest/ug/create-table-as.html) * [dbt-labs/dbt-core](https://github.com/dbt-
-labs/dbt-core) * [laughingman7743/PyAthena](https://github.com/laughingman7743/
-PyAthena) ## Contributors â¨ Thanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)):
-    [nicor88]          [Jesse       [Lemiffe] [JÃ©rÃ©my_Guisel      [Tom]       [Mattia]
-     nicor88         Dobbelaere]     Lemiffe   JÃ©rÃ©my_Guisel       Tom         Mattia
-    ð» ð�Jesse_Dobbelaere    ð¨       ð§         ð§ ð�  ð§
-                      ð ð§
+history ## Contributing See [CONTRIBUTING](CONTRIBUTING.md) for more
+information on how to contribute to this project. ## Contributors â¨ Thanks
+goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
+en/emoji-key)):
+        [nicor88]               [Jesse       [Lemiffe]  [JÃ©rÃ©my_Guiselin      [Tom]       [Mattia] [Gatsby
+         nicor88              Dobbelaere]     Lemiffe    JÃ©rÃ©my_Guiselin       Tom         Mattia    Lee]
+      ð» ð§ ð�Jesse_Dobbelaere    ð¨    ð§ ð» �    ð§ ð�  ð� Gatsby
+                               ð ð§                                                           Lee
+                                                                                                           ð
+      [BrechtDeVlieger]    [Andrea_Artaria]   [Maiara     [Henri_Blancke]          [Serhii
+       BrechtDeVlieger      Andrea_Artaria   Reinaldo]     Henri_Blancke         Dimchenko]
+             ð            ð     Maiara         ð» ðSerhii_Dimchenko
+                                             Reinaldo                             ð» ð
+                                               ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `dbt-athena-community-1.4.3/dbt/adapters/athena/__init__.py` & `dbt-athena-community-1.4.4/dbt/adapters/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/dbt/adapters/athena/column.py` & `dbt-athena-community-1.4.4/dbt/adapters/athena/column.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/dbt/adapters/athena/connections.py` & `dbt-athena-community-1.4.4/dbt/adapters/athena/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 @dataclass
 class AthenaCredentials(Credentials):
     s3_staging_dir: str
     region_name: str
     endpoint_url: Optional[str] = None
     work_group: Optional[str] = None
     aws_profile_name: Optional[str] = None
+    aws_access_key_id: Optional[str] = None
+    aws_secret_access_key: Optional[str] = None
     poll_interval: float = 1.0
     _ALIASES = {"catalog": "database"}
     num_retries: Optional[int] = 5
     s3_data_dir: Optional[str] = None
     s3_data_naming: Optional[str] = "schema_table_unique"
     lf_tags: Optional[Dict[str, str]] = None
 
@@ -62,14 +64,16 @@
             "s3_staging_dir",
             "work_group",
             "region_name",
             "database",
             "schema",
             "poll_interval",
             "aws_profile_name",
+            "aws_access_key_id",
+            "aws_secret_access_key",
             "endpoint_url",
             "s3_data_dir",
             "s3_data_naming",
             "lf_tags",
         )
```

### Comparing `dbt-athena-community-1.4.3/dbt/adapters/athena/impl.py` & `dbt-athena-community-1.4.4/dbt/adapters/athena/impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 from threading import Lock
 from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, Union
 from urllib.parse import urlparse
 from uuid import uuid4
 
 import agate
 from botocore.exceptions import ClientError
+from mypy_boto3_athena.type_defs import DataCatalogTypeDef
 
 from dbt.adapters.athena import AthenaConnectionManager
 from dbt.adapters.athena.column import AthenaColumn
 from dbt.adapters.athena.config import get_boto3_config
 from dbt.adapters.athena.relation import (
     AthenaRelation,
     AthenaSchemaSearchMap,
     TableType,
 )
-from dbt.adapters.athena.utils import clean_sql_comment
+from dbt.adapters.athena.utils import clean_sql_comment, get_catalog_id
 from dbt.adapters.base import available
 from dbt.adapters.base.relation import BaseRelation, InformationSchema
 from dbt.adapters.sql import SQLAdapter
 from dbt.contracts.graph.manifest import Manifest
 from dbt.contracts.graph.nodes import CompiledNode
 from dbt.events import AdapterLogger
 from dbt.exceptions import DbtRuntimeError
@@ -187,30 +188,36 @@
     @available
     def s3_table_location(
         self,
         s3_data_dir: Optional[str],
         s3_data_naming: str,
         schema_name: str,
         table_name: str,
+        s3_path_table_part: Optional[str] = None,
         external_location: Optional[str] = None,
         is_temporary_table: bool = False,
     ) -> str:
         """
         Returns either a UUID or database/table prefix for storing a table,
         depending on the value of s3_table
         """
         if external_location and not is_temporary_table:
             return external_location.rstrip("/")
 
+        if not s3_path_table_part:
+            s3_path_table_part = table_name
+
         mapping = {
             "uuid": path.join(self.s3_table_prefix(s3_data_dir), str(uuid4())),
-            "table": path.join(self.s3_table_prefix(s3_data_dir), table_name),
-            "table_unique": path.join(self.s3_table_prefix(s3_data_dir), table_name, str(uuid4())),
-            "schema_table": path.join(self.s3_table_prefix(s3_data_dir), schema_name, table_name),
-            "schema_table_unique": path.join(self.s3_table_prefix(s3_data_dir), schema_name, table_name, str(uuid4())),
+            "table": path.join(self.s3_table_prefix(s3_data_dir), s3_path_table_part),
+            "table_unique": path.join(self.s3_table_prefix(s3_data_dir), s3_path_table_part, str(uuid4())),
+            "schema_table": path.join(self.s3_table_prefix(s3_data_dir), schema_name, s3_path_table_part),
+            "schema_table_unique": path.join(
+                self.s3_table_prefix(s3_data_dir), schema_name, s3_path_table_part, str(uuid4())
+            ),
         }
         table_location = mapping.get(s3_data_naming)
 
         if table_location is None:
             raise ValueError(f"Unknown value for s3_data_naming: {s3_data_naming}")
 
         return table_location
@@ -276,15 +283,17 @@
         table_name: str,
         table: agate.Table,
     ) -> str:
         conn = self.connections.get_thread_connection()
         client = conn.handle
 
         # TODO: consider using the workgroup default location when configured
-        s3_location = self.s3_table_location(s3_data_dir, s3_data_naming, database_name, table_name, external_location)
+        s3_location = self.s3_table_location(
+            s3_data_dir, s3_data_naming, database_name, table_name, external_location=external_location
+        )
         bucket, prefix = self._parse_s3_path(s3_location)
 
         file_name = f"{table_name}.csv"
         object_name = path.join(prefix, file_name)
 
         with boto3_client_lock:
             s3_client = client.session.client("s3", region_name=client.region_name, config=get_boto3_config())
@@ -373,15 +382,15 @@
         )
 
     def _get_one_table_for_catalog(self, table: dict, database: str) -> list:
         table_catalog = {
             "table_database": database,
             "table_schema": table["DatabaseName"],
             "table_name": table["Name"],
-            "table_type": self.relation_type_map[table["TableType"]].value,
+            "table_type": self.relation_type_map[table.get("TableType", "EXTERNAL_TABLE")].value,
             "table_comment": table.get("Parameters", {}).get("comment", table.get("Description", "")),
         }
         return [
             {
                 **table_catalog,
                 **{
                     "column_name": col["Name"],
@@ -395,27 +404,36 @@
 
     def _get_one_catalog(
         self,
         information_schema: InformationSchema,
         schemas: Dict[str, Optional[Set[str]]],
         manifest: Manifest,
     ) -> agate.Table:
+        data_catalog = self._get_data_catalog(information_schema.path.database)
+        catalog_id = get_catalog_id(data_catalog)
         conn = self.connections.get_thread_connection()
         client = conn.handle
-
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
 
         catalog = []
         paginator = glue_client.get_paginator("get_tables")
         for schema, relations in schemas.items():
-            for page in paginator.paginate(DatabaseName=schema, MaxResults=100):
+            kwargs = {
+                "DatabaseName": schema,
+                "MaxResults": 100,
+            }
+            # If the catalog is `awsdatacatalog` we don't need to pass CatalogId as boto3 infers it from the account Id.
+            if catalog_id:
+                kwargs["CatalogId"] = catalog_id
+
+            for page in paginator.paginate(**kwargs):
                 for table in page["TableList"]:
                     if table["Name"] in relations:
-                        catalog.extend(self._get_one_table_for_catalog(table, conn.credentials.database))
+                        catalog.extend(self._get_one_table_for_catalog(table, information_schema.path.database))
 
         table = agate.Table.from_object(catalog)
         filtered_table = self._catalog_filter_table(table, manifest)
         return self._join_catalog_table_owners(filtered_table, manifest)
 
     def _get_catalog_schemas(self, manifest: Manifest) -> AthenaSchemaSearchMap:
         info_schema_name_map = AthenaSchemaSearchMap()
@@ -424,35 +442,34 @@
             manifest.sources.values(),
         )
         for node in nodes:
             relation = self.Relation.create_from(self.config, node)
             info_schema_name_map.add(relation)
         return info_schema_name_map
 
-    def _get_data_catalog(self, catalog_name):
-        conn = self.connections.get_thread_connection()
-        client = conn.handle
-        with boto3_client_lock:
-            athena_client = client.session.client("athena", region_name=client.region_name, config=get_boto3_config())
-
-        response = athena_client.get_data_catalog(Name=catalog_name)
-        return response["DataCatalog"]
-
-    def list_relations_without_caching(
-        self,
-        schema_relation: AthenaRelation,
-    ) -> List[BaseRelation]:
-        catalog_id = None
-        if schema_relation.database is not None and schema_relation.database.lower() != "awsdatacatalog":
-            data_catalog = self._get_data_catalog(schema_relation.database.lower())
-            # For non-Glue Data Catalogs, use the original Athena query against INFORMATION_SCHEMA approach
-            if data_catalog["Type"] != "GLUE":
-                return super().list_relations_without_caching(schema_relation)
+    def _get_data_catalog(self, database: str) -> Optional[DataCatalogTypeDef]:
+        if database:
+            conn = self.connections.get_thread_connection()
+            client = conn.handle
+            if database.lower() == "awsdatacatalog":
+                with boto3_client_lock:
+                    sts = client.session.client("sts", region_name=client.region_name, config=get_boto3_config())
+                catalog_id = sts.get_caller_identity()["Account"]
+                return {"Name": database, "Type": "GLUE", "Parameters": {"catalog-id": catalog_id}}
             else:
-                catalog_id = data_catalog["Parameters"]["catalog-id"]
+                with boto3_client_lock:
+                    athena = client.session.client("athena", region_name=client.region_name, config=get_boto3_config())
+                return athena.get_data_catalog(Name=database)["DataCatalog"]
+
+    def list_relations_without_caching(self, schema_relation: AthenaRelation) -> List[BaseRelation]:
+        data_catalog = self._get_data_catalog(schema_relation.database)
+        catalog_id = get_catalog_id(data_catalog)
+        if data_catalog and data_catalog["Type"] != "GLUE":
+            # For non-Glue Data Catalogs, use the original Athena query against INFORMATION_SCHEMA approach
+            return super().list_relations_without_caching(schema_relation)
 
         conn = self.connections.get_thread_connection()
         client = conn.handle
         with boto3_client_lock:
             glue_client = client.session.client("glue", region_name=client.region_name, config=get_boto3_config())
         paginator = glue_client.get_paginator("get_tables")
```

### Comparing `dbt-athena-community-1.4.3/dbt/adapters/athena/query_headers.py` & `dbt-athena-community-1.4.4/dbt/adapters/athena/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/dbt/adapters/athena/relation.py` & `dbt-athena-community-1.4.4/dbt/adapters/athena/relation.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     identifier: bool = True
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class AthenaRelation(BaseRelation):
     quote_character: str = '"'  # Presto quote character
     include_policy: Policy = field(default_factory=lambda: AthenaIncludePolicy())
+    s3_path_table_part: Optional[str] = None
 
     def render_hive(self):
         """
         Render relation with Hive format. Athena uses Hive format for some DDL statements.
 
         See:
         - https://aws.amazon.com/athena/faqs/ "Q: How do I create tables and schemas for my data on Amazon S3?"
```

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/persist_docs.sql` & `dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/macros/adapters/relation.sql` & `dbt-athena-community-1.4.4/dbt/include/athena/macros/adapters/relation.sql`

 * *Files 23% similar despite different names*

```diff
@@ -16,7 +16,13 @@
 
 {% macro set_table_classification(relation) -%}
   {%- set format = config.get('format', default='parquet') -%}
   {% call statement('set_table_classification', auto_begin=False) -%}
     alter table {{ relation.render_hive() }} set tblproperties ('classification' = '{{ format }}')
   {%- endcall %}
 {%- endmacro %}
+
+{% macro athena__rename_relation(from_relation, to_relation) %}
+  {% call statement('rename_relation') -%}
+    alter table {{ from_relation.render_hive() }} rename to `{{ to_relation.schema }}`.`{{ to_relation.identifier }}`
+  {%- endcall %}
+{%- endmacro %}
```

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql` & `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/helpers.sql` & `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/incremental.sql` & `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/incremental.sql`

 * *Files 2% similar despite different names*

```diff
@@ -43,27 +43,28 @@
       {% do drop_relation(tmp_relation) %}
     {% endif %}
     {% do run_query(create_table_as(True, tmp_relation, sql)) %}
     {% set build_sql = incremental_insert(on_schema_change, tmp_relation, target_relation, existing_relation) %}
     {% do to_drop.append(tmp_relation) %}
   {% elif strategy == 'merge' and table_type == 'iceberg' %}
     {% set unique_key = config.get('unique_key') %}
+    {% set delete_condition = config.get('delete_condition') %}
     {% set empty_unique_key -%}
       Merge strategy must implement unique_key as a single column or a list of columns.
     {%- endset %}
     {% if unique_key is none %}
       {% do exceptions.raise_compiler_error(empty_unique_key) %}
     {% endif %}
 
     {% set tmp_relation = make_temp_relation(target_relation) %}
     {% if tmp_relation is not none %}
       {% do drop_relation(tmp_relation) %}
     {% endif %}
     {% do run_query(create_table_as(True, tmp_relation, sql)) %}
-    {% set build_sql = iceberg_merge(on_schema_change, tmp_relation, target_relation, unique_key, existing_relation) %}
+    {% set build_sql = iceberg_merge(on_schema_change, tmp_relation, target_relation, unique_key, existing_relation, delete_condition) %}
     {% do to_drop.append(tmp_relation) %}
   {% endif %}
 
   {% call statement("main") %}
     {{ build_sql }}
   {% endcall %}
```

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/table/create_table_as.sql` & `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/table/create_table_as.sql`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,21 @@
   {%- set s3_data_dir = config.get('s3_data_dir', default=target.s3_data_dir) -%}
   {%- set s3_data_naming = config.get('s3_data_naming', default=target.s3_data_naming) -%}
   {%- set extra_table_properties = config.get('table_properties', default=none) -%}
 
   {%- set location_property = 'external_location' -%}
   {%- set partition_property = 'partitioned_by' -%}
   {%- set work_group_output_location_enforced = adapter.is_work_group_output_location_enforced() -%}
-  {%- set location = adapter.s3_table_location(s3_data_dir, s3_data_naming, relation.schema, relation.identifier, external_location, temporary) -%}
+  {%- set location = adapter.s3_table_location(s3_data_dir,
+                                               s3_data_naming,
+                                               relation.schema,
+                                               relation.identifier,
+                                               relation.s3_path_table_part,
+                                               external_location,
+                                               temporary) -%}
 
   {%- if materialized == 'table_hive_ha' -%}
     {%- set location = location.replace('__ha', '') -%}
   {%- endif %}
 
   {%- if table_type == 'iceberg' -%}
     {%- set location_property = 'location' -%}
@@ -44,15 +50,15 @@
 
   {% do adapter.delete_from_s3(location) %}
 
   create table {{ relation }}
   with (
     table_type='{{ table_type }}',
     is_external={%- if table_type == 'iceberg' -%}false{%- else -%}true{%- endif %},
-  {%- if not work_group_output_location_enforced -%}
+  {%- if not work_group_output_location_enforced or table_type == 'iceberg' -%}
     {{ location_property }}='{{ location }}',
   {%- endif %}
   {%- if partitioned_by is not none %}
     {{ partition_property }}=ARRAY{{ partitioned_by | tojson | replace('\"', '\'') }},
   {%- endif %}
   {%- if bucketed_by is not none %}
     bucketed_by=ARRAY{{ bucketed_by | tojson | replace('\"', '\'') }},
```

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql` & `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/table/table_hive_ha.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/seeds/helpers.sql` & `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/seeds/helpers.sql`

 * *Files 5% similar despite different names*

```diff
@@ -38,34 +38,34 @@
   {%- set lf_tags_columns = config.get('lf_tags_columns', default=none) -%}
   {%- set column_override = config.get('column_types', {}) -%}
   {%- set quote_seed_column = config.get('quote_columns', None) -%}
   {%- set s3_data_dir = config.get('s3_data_dir', default=target.s3_data_dir) -%}
   {%- set s3_data_naming = config.get('s3_data_naming', target.s3_data_naming) -%}
   {%- set external_location = config.get('external_location', default=none) -%}
 
-  {%- set s3_location = adapter.upload_seed_to_s3(
+  {%- set tmp_s3_location = adapter.upload_seed_to_s3(
     s3_data_dir,
     s3_data_naming,
     external_location,
     model.schema,
-    model.name,
+    model.name + "__dbt_tmp",
     agate_table,
   ) -%}
 
   -- create tmp relation
   {%- set tmp_relation = api.Relation.create(
-    identifier=model.name + "_tmp",
+    identifier=identifier + "__dbt_tmp",
     schema=model.schema,
     database=model.database,
     type='table'
   ) -%}
 
   -- create target relation
   {%- set relation = api.Relation.create(
-    identifier=model.name,
+    identifier=identifier,
     schema=model.schema,
     database=model.database,
     type='table'
   ) -%}
 
   -- drop tmp relation if exists
   {{ drop_relation(tmp_relation) }}
@@ -74,15 +74,15 @@
     create external table {{ tmp_relation.render_hive() }} (
         {%- for col_name in agate_table.column_names -%}
             {%- set column_name = (col_name | string) -%}
             {{ adapter.quote_seed_column(column_name, quote_seed_column) }} string {%- if not loop.last -%}, {% endif -%}
         {%- endfor -%}
     )
     row format serde 'org.apache.hadoop.hive.serde2.OpenCSVSerde'
-    location '{{ s3_location }}'
+    location '{{ tmp_s3_location }}'
     tblproperties (
       'skip.header.line.count'='1'
     )
   {% endset %}
 
   -- casting to type string is not allowed needs to be varchar
   {% set sql %}
@@ -115,15 +115,15 @@
     {{ sql_table }}
   {%- endcall %}
 
   -- drop tmp table
   {{ drop_relation(tmp_relation) }}
 
   -- delete csv file from s3
-  {% do adapter.delete_from_s3(s3_location) %}
+  {% do adapter.delete_from_s3(tmp_s3_location) %}
 
   {% if lf_tags is not none or lf_tags_columns is not none %}
     {{ adapter.add_lf_tags(model.schema, identifier, lf_tags, lf_tags_columns) }}
   {% endif %}
 
   {{ return(sql_table) }}
 {% endmacro %}
```

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/macros/materializations/snapshots/snapshot.sql` & `dbt-athena-community-1.4.4/dbt/include/athena/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/datediff.sql` & `dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/macros/utils/ddl_data_type.sql` & `dbt-athena-community-1.4.4/dbt/include/athena/macros/utils/ddl_data_type.sql`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/dbt/include/athena/profile_template.yml` & `dbt-athena-community-1.4.4/dbt/include/athena/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/dbt_athena_community.egg-info/PKG-INFO` & `dbt-athena-community-1.4.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: dbt-athena-community
-Version: 1.4.3
-Summary: The athena adapter plugin for dbt (data build tool)
-Home-page: https://github.com/dbt-athena/dbt-athena
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <p align="center">
     <img src="https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/dbt-athena-long.png" />
     <a href="https://pypi.org/project/dbt-athena-community/"><img src="https://badge.fury.io/py/dbt-athena-community.svg" /></a>
     <a href="https://pycqa.github.io/isort/"><img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" /></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" /></a>
     <a href="https://pepy.tech/project/dbt-athena-community"><img src="https://pepy.tech/badge/dbt-athena-community/month" /></a>
 </p>
@@ -63,34 +55,39 @@
 
 Notes:
 - Take note of your AWS region code (e.g. `us-west-2` or `eu-west-2`, etc.).
 - You can also use [AWS Glue](https://docs.aws.amazon.com/athena/latest/ug/glue-athena.html) to create and manage Athena databases.
 
 ### Credentials
 
-This plugin does not accept any credentials directly. Instead, [credentials are determined automatically](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3` conventions and
-stored login info. You can configure the AWS profile name to use via `aws_profile_name`. Checkout DBT profile configuration below for details.
+Credentials can be passed directly to the adapter, or they can be [determined automatically](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3` conventions.
+You can either:
+- configure `aws_access_key_id` and `aws_secret_access_key`
+- configure `aws_profile_name` to match a profile defined in your AWS credentials file
+Checkout DBT profile configuration below for details.
 
 ### Configuring your profile
 
 A dbt profile can be configured to run against AWS Athena using the following configuration:
 
-| Option           | Description                                                                    | Required? | Example                                  |
-|------------------|--------------------------------------------------------------------------------|-----------|------------------------------------------|
-| s3_staging_dir   | S3 location to store Athena query results and metadata                         | Required  | `s3://bucket/dbt/`                       |
-| s3_data_dir      | Prefix for storing tables, if different from the connection's `s3_staging_dir` | Optional  | `s3://bucket2/dbt/`                      |
-| s3_data_naming   | How to generate table paths in `s3_data_dir`                                   | Optional  | `schema_table_unique`                    |
-| region_name      | AWS region of your Athena instance                                             | Required  | `eu-west-1`                              |
-| schema           | Specify the schema (Athena database) to build models into (lowercase **only**) | Required  | `dbt`                                    |
-| database         | Specify the database (Data catalog) to build models into (lowercase **only**)  | Required  | `awsdatacatalog`                         |
-| poll_interval    | Interval in seconds to use for polling the status of query results in Athena   | Optional  | `5`                                      |
-| aws_profile_name | Profile to use from your AWS shared credentials file.                          | Optional  | `my-profile`                             |
-| work_group       | Identifier of Athena workgroup                                                 | Optional  | `my-custom-workgroup`                    |
-| num_retries      | Number of times to retry a failing query                                       | Optional  | `3`                                      |
-| lf_tags          | Default lf tags to apply to any database created by dbt                        | Optional  | `{"origin": "dbt", "team": "analytics"}` |
+| Option                | Description                                                                    | Required? | Example                                    |
+|-----------------------|--------------------------------------------------------------------------------|-----------|--------------------------------------------|
+| s3_staging_dir        | S3 location to store Athena query results and metadata                         | Required  | `s3://bucket/dbt/`                         |
+| s3_data_dir           | Prefix for storing tables, if different from the connection's `s3_staging_dir` | Optional  | `s3://bucket2/dbt/`                        |
+| s3_data_naming        | How to generate table paths in `s3_data_dir`                                   | Optional  | `schema_table_unique`                      |
+| region_name           | AWS region of your Athena instance                                             | Required  | `eu-west-1`                                |
+| schema                | Specify the schema (Athena database) to build models into (lowercase **only**) | Required  | `dbt`                                      |
+| database              | Specify the database (Data catalog) to build models into (lowercase **only**)  | Required  | `awsdatacatalog`                           |
+| poll_interval         | Interval in seconds to use for polling the status of query results in Athena   | Optional  | `5`                                        |
+| aws_access_key_id     | Access key ID of the user performing requests.                                 | Optional  | `AKIAIOSFODNN7EXAMPLE`                     |
+| aws_secret_access_key | Secret access key of the user performing requests                              | Optional  | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` |
+| aws_profile_name      | Profile to use from your AWS shared credentials file.                          | Optional  | `my-profile`                               |
+| work_group            | Identifier of Athena workgroup                                                 | Optional  | `my-custom-workgroup`                      |
+| num_retries           | Number of times to retry a failing query                                       | Optional  | `3`                                        |
+| lf_tags               | Default lf tags to apply to any database created by dbt                        | Optional  | `{"origin": "dbt", "team": "analytics"}`   |
 
 **Example profiles.yml entry:**
 ```yaml
 athena:
   target: dev
   outputs:
     dev:
@@ -218,15 +215,39 @@
 Iceberg supports bucketing as hidden partitions, therefore use the `partitioned_by` config to add specific bucketing conditions.
 
 Iceberg supports several table formats for data : `PARQUET`, `AVRO` and `ORC`.
 
 It is possible to use iceberg in an incremental fashion, specifically 2 strategies are supported:
 * `append`: new records are appended to the table, this can lead to duplicates
 * `merge`: must be used in combination with `unique_key` and it's only available with Engine version 3.
-   It performs an upsert, new record are added, and record already existing are updated
+   It performs an upsert, new record are added, and record already existing are updated. If
+   `delete_condition` is provided in the model config, it can also delete records based on the
+   provided condition (SQL condition). You can use any column of the incremental table (`src`) or
+   the final table (`target`). You must prefix the column by the name of the table to prevent
+   `Column is ambiguous` error.
+
+```sql
+{{ config(
+    materialized='incremental',
+    table_type='iceberg',
+    incremental_strategy='merge',
+    unique_key='user_id',
+    delete_condition="src.status != 'active' and target.my_date < now() - interval '2' year"
+    format='parquet',
+) }}
+
+SELECT
+	'A' AS user_id,
+	'pi' AS name,
+	'active' AS status,
+	17.89 AS cost,
+	1 AS quantity,
+	100000000 AS quantity_big,
+	current_date AS my_date
+```
 
 ### High available table materialization
 The current implementation of the table materialization can lead to downtime, as target table is dropped and re-created.
 To have the less destructive behavior it's possible to use `table='table_hive_ha'` materialization.
 **table_hive_ha** leverage the table versions feature of glue catalog, creating a tmp table and swapping
 the target table to the location of the tmp table.
 This materialization is only available for `table_type=hive` and requires using unique locations.
@@ -381,76 +402,41 @@
   See https://github.com/dbt-athena/dbt-athena/issues/103 for more details.
 
 * Snapshot does not support dropping columns from the source table. If you drop a column make sure to drop the column from the snapshot as well. Another workaround is to NULL the column in the snapshot definition to preserve history
 
 
 ## Contributing
 
-This connector works with Python from 3.7 to 3.11.
-
-### Getting started
-
-In order to start developing on this adapter clone the repo and run this make command (see [Makefile](Makefile)) :
-
-```bash
-make setup
-```
-
-It will :
-1. Install all dependencies.
-2. Install pre-commit hooks.
-3. Generate your `.env` file
-
-Next, adjust `.env` file by configuring the environment variables to match your Athena development environment.
-
-### Running tests
-
-We have 2 different types of testing:
-* **unit testing**: you can run this type of tests running `make unit_test`
-* **functional testing**: you must have an AWS account with Athena setup in order to launch this type of tests and have a `.env` file in place with the right values.
-  You can run this type of tests running `make functional_test`
-
-All type of tests can be run using `make`:
-```bash
-make test
-```
-
-### Pull Request
-
-* Create a commit with your changes and push them to a
-  [fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo).
-* Create a [pull request on
-  Github](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
-* Pull request title and message (and PR title and description) must adhere to
-  [conventionalcommits](https://www.conventionalcommits.org).
-* Pull request body should describe _motivation_.
-
-
-## Resources
-* [Athena CREATE TABLE AS](https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html)
-* [dbt-labs/dbt-core](https://github.com/dbt-labs/dbt-core)
-* [laughingman7743/PyAthena](https://github.com/laughingman7743/PyAthena)
+See [CONTRIBUTING](CONTRIBUTING.md) for more information on how to contribute to this project.
 
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nicor88"><img src="https://avatars.githubusercontent.com/u/6278547?v=4?s=100" width="100px;" alt="nicor88"/><br /><sub><b>nicor88</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=nicor88" title="Code">💻</a> <a href="#maintenance-nicor88" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nicor88"><img src="https://avatars.githubusercontent.com/u/6278547?v=4?s=100" width="100px;" alt="nicor88"/><br /><sub><b>nicor88</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=nicor88" title="Code">💻</a> <a href="#maintenance-nicor88" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Anicor88" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://jessedobbelae.re"><img src="https://avatars.githubusercontent.com/u/1352979?v=4?s=100" width="100px;" alt="Jesse Dobbelaere"/><br /><sub><b>Jesse Dobbelaere</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ajessedobbelaere" title="Bug reports">🐛</a> <a href="#maintenance-jessedobbelaere" title="Maintenance">🚧</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/lemiffe"><img src="https://avatars.githubusercontent.com/u/7487772?v=4?s=100" width="100px;" alt="Lemiffe"/><br /><sub><b>Lemiffe</b></sub></a><br /><a href="#design-lemiffe" title="Design">🎨</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Jrmyy"><img src="https://avatars.githubusercontent.com/u/9251353?v=4?s=100" width="100px;" alt="Jérémy Guiselin"/><br /><sub><b>Jérémy Guiselin</b></sub></a><br /><a href="#maintenance-Jrmyy" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Jrmyy"><img src="https://avatars.githubusercontent.com/u/9251353?v=4?s=100" width="100px;" alt="Jérémy Guiselin"/><br /><sub><b>Jérémy Guiselin</b></sub></a><br /><a href="#maintenance-Jrmyy" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/commits?author=Jrmyy" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3AJrmyy" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Tomme"><img src="https://avatars.githubusercontent.com/u/932895?v=4?s=100" width="100px;" alt="Tom"/><br /><sub><b>Tom</b></sub></a><br /><a href="#maintenance-Tomme" title="Maintenance">🚧</a> <a href="https://github.com/dbt-athena/dbt-athena/commits?author=Tomme" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/mattiamatrix"><img src="https://avatars.githubusercontent.com/u/5013654?v=4?s=100" width="100px;" alt="Mattia"/><br /><sub><b>Mattia</b></sub></a><br /><a href="#maintenance-mattiamatrix" title="Maintenance">🚧</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Gatsby-Lee"><img src="https://avatars.githubusercontent.com/u/22950880?v=4?s=100" width="100px;" alt="Gatsby Lee"/><br /><sub><b>Gatsby Lee</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3AGatsby-Lee" title="Bug reports">🐛</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/BrechtDeVlieger"><img src="https://avatars.githubusercontent.com/u/12074972?v=4?s=100" width="100px;" alt="BrechtDeVlieger"/><br /><sub><b>BrechtDeVlieger</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3ABrechtDeVlieger" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/aartaria"><img src="https://avatars.githubusercontent.com/u/10273710?v=4?s=100" width="100px;" alt="Andrea Artaria"/><br /><sub><b>Andrea Artaria</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Aaartaria" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/maiarareinaldo"><img src="https://avatars.githubusercontent.com/u/72740386?v=4?s=100" width="100px;" alt="Maiara Reinaldo"/><br /><sub><b>Maiara Reinaldo</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Amaiarareinaldo" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/henriblancke"><img src="https://avatars.githubusercontent.com/u/1708162?v=4?s=100" width="100px;" alt="Henri Blancke"/><br /><sub><b>Henri Blancke</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=henriblancke" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Ahenriblancke" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/svdimchenko"><img src="https://avatars.githubusercontent.com/u/39801237?v=4?s=100" width="100px;" alt="Serhii Dimchenko"/><br /><sub><b>Serhii Dimchenko</b></sub></a><br /><a href="https://github.com/dbt-athena/dbt-athena/commits?author=svdimchenko" title="Code">💻</a> <a href="https://github.com/dbt-athena/dbt-athena/issues?q=author%3Asvdimchenko" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,11 +1,7 @@
-Metadata-Version: 2.1 Name: dbt-athena-community Version: 1.4.3 Summary: The
-athena adapter plugin for dbt (data build tool) Home-page: https://github.com/
-dbt-athena/dbt-athena Description-Content-Type: text/markdown License-File:
-LICENSE.txt
  [https://raw.githubusercontent.com/dbt-athena/dbt-athena/main/static/images/
    dbt-athena-long.png] [https://badge.fury.io/py/dbt-athena-community.svg]
                 [https://img.shields.io/badge/%20imports-isort-
     %231674b1?style=flat&labelColor=ef8336] [https://img.shields.io/badge/
  code%20style-black-000000.svg] [https://pepy.tech/badge/dbt-athena-community/
                                     month]
 ## Features * Supports dbt version `1.4.*` * Supports [Seeds][seeds] *
@@ -30,55 +26,59 @@
 athena/dbt-athena.git` ### Prerequisites To start, you will need an S3 bucket,
 for instance `my-bucket` and an Athena database: ```sql CREATE DATABASE IF NOT
 EXISTS analytics_dev COMMENT 'Analytics models generated by dbt (development)'
 LOCATION 's3://my-bucket/' WITH DBPROPERTIES ('creator'='Foo Bar',
 'email'='foo@bar.com'); ``` Notes: - Take note of your AWS region code (e.g.
 `us-west-2` or `eu-west-2`, etc.). - You can also use [AWS Glue](https://
 docs.aws.amazon.com/athena/latest/ug/glue-athena.html) to create and manage
-Athena databases. ### Credentials This plugin does not accept any credentials
-directly. Instead, [credentials are determined automatically](https://
-boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) based
-on `aws cli`/`boto3` conventions and stored login info. You can configure the
-AWS profile name to use via `aws_profile_name`. Checkout DBT profile
-configuration below for details. ### Configuring your profile A dbt profile can
-be configured to run against AWS Athena using the following configuration: |
-Option | Description | Required? | Example | |------------------|--------------
-------------------------------------------------------------------|-----------
-|------------------------------------------| | s3_staging_dir | S3 location to
+Athena databases. ### Credentials Credentials can be passed directly to the
+adapter, or they can be [determined automatically](https://boto3.amazonaws.com/
+v1/documentation/api/latest/guide/credentials.html) based on `aws cli`/`boto3`
+conventions. You can either: - configure `aws_access_key_id` and
+`aws_secret_access_key` - configure `aws_profile_name` to match a profile
+defined in your AWS credentials file Checkout DBT profile configuration below
+for details. ### Configuring your profile A dbt profile can be configured to
+run against AWS Athena using the following configuration: | Option |
+Description | Required? | Example | |-----------------------|------------------
+--------------------------------------------------------------|-----------|----
+----------------------------------------| | s3_staging_dir | S3 location to
 store Athena query results and metadata | Required | `s3://bucket/dbt/` | |
 s3_data_dir | Prefix for storing tables, if different from the connection's
 `s3_staging_dir` | Optional | `s3://bucket2/dbt/` | | s3_data_naming | How to
 generate table paths in `s3_data_dir` | Optional | `schema_table_unique` | |
 region_name | AWS region of your Athena instance | Required | `eu-west-1` | |
 schema | Specify the schema (Athena database) to build models into (lowercase
 **only**) | Required | `dbt` | | database | Specify the database (Data catalog)
 to build models into (lowercase **only**) | Required | `awsdatacatalog` | |
 poll_interval | Interval in seconds to use for polling the status of query
-results in Athena | Optional | `5` | | aws_profile_name | Profile to use from
-your AWS shared credentials file. | Optional | `my-profile` | | work_group |
-Identifier of Athena workgroup | Optional | `my-custom-workgroup` | |
-num_retries | Number of times to retry a failing query | Optional | `3` | |
-lf_tags | Default lf tags to apply to any database created by dbt | Optional |
-`{"origin": "dbt", "team": "analytics"}` | **Example profiles.yml entry:**
-```yaml athena: target: dev outputs: dev: type: athena s3_staging_dir: s3://
-athena-query-results/dbt/ s3_data_dir: s3://your_s3_bucket/dbt/ s3_data_naming:
-schema_table region_name: eu-west-1 schema: dbt database: awsdatacatalog
-aws_profile_name: my-profile work_group: my-workgroup lf_tags: origin: dbt
-team: analytics ``` _Additional information_ * `threads` is supported *
-`database` and `catalog` can be used interchangeably ## Models ### Table
-Configuration * `external_location` (`default=none`) * If set, the full S3 path
-in which the table will be saved. (Does not work with Iceberg table). *
-`partitioned_by` (`default=none`) * An array list of columns by which the table
-will be partitioned * Limited to creation of 100 partitions (_currently_) *
-`bucketed_by` (`default=none`) * An array list of columns to bucket data,
-ignored if using Iceberg * `bucket_count` (`default=none`) * The number of
-buckets for bucketing your data, ignored if using Iceberg * `table_type`
-(`default='hive'`) * The type of table * Supports `hive` or `iceberg` *
-`format` (`default='parquet'`) * The data format for the table * Supports
-`ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
+results in Athena | Optional | `5` | | aws_access_key_id | Access key ID of the
+user performing requests. | Optional | `AKIAIOSFODNN7EXAMPLE` | |
+aws_secret_access_key | Secret access key of the user performing requests |
+Optional | `wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY` | | aws_profile_name |
+Profile to use from your AWS shared credentials file. | Optional | `my-profile`
+| | work_group | Identifier of Athena workgroup | Optional | `my-custom-
+workgroup` | | num_retries | Number of times to retry a failing query |
+Optional | `3` | | lf_tags | Default lf tags to apply to any database created
+by dbt | Optional | `{"origin": "dbt", "team": "analytics"}` | **Example
+profiles.yml entry:** ```yaml athena: target: dev outputs: dev: type: athena
+s3_staging_dir: s3://athena-query-results/dbt/ s3_data_dir: s3://
+your_s3_bucket/dbt/ s3_data_naming: schema_table region_name: eu-west-1 schema:
+dbt database: awsdatacatalog aws_profile_name: my-profile work_group: my-
+workgroup lf_tags: origin: dbt team: analytics ``` _Additional information_ *
+`threads` is supported * `database` and `catalog` can be used interchangeably
+## Models ### Table Configuration * `external_location` (`default=none`) * If
+set, the full S3 path in which the table will be saved. (Does not work with
+Iceberg table). * `partitioned_by` (`default=none`) * An array list of columns
+by which the table will be partitioned * Limited to creation of 100 partitions
+(_currently_) * `bucketed_by` (`default=none`) * An array list of columns to
+bucket data, ignored if using Iceberg * `bucket_count` (`default=none`) * The
+number of buckets for bucketing your data, ignored if using Iceberg *
+`table_type` (`default='hive'`) * The type of table * Supports `hive` or
+`iceberg` * `format` (`default='parquet'`) * The data format for the table *
+Supports `ORC`, `PARQUET`, `AVRO`, `JSON`, `TEXTFILE` * `write_compression`
 (`default=none`) * The compression type to use for any storage format that
 allows compression to be specified. To see which options are available, check
 out [CREATE TABLE AS][create-table-as] * `field_delimiter` (`default=none`) *
 Custom field delimiter, for when format is set to `TEXTFILE` *
 `table_properties`: table properties to add to the table, valid for Iceberg
 only * `lf_tags` (`default=none`) * lf tags to associate with the table *
 format: `{"tag1": "value1", "tag2": "value2"}` * `lf_tags_columns`
@@ -121,42 +121,52 @@
 partitions, therefore use the `partitioned_by` config to add specific bucketing
 conditions. Iceberg supports several table formats for data : `PARQUET`, `AVRO`
 and `ORC`. It is possible to use iceberg in an incremental fashion,
 specifically 2 strategies are supported: * `append`: new records are appended
 to the table, this can lead to duplicates * `merge`: must be used in
 combination with `unique_key` and it's only available with Engine version 3. It
 performs an upsert, new record are added, and record already existing are
-updated ### High available table materialization The current implementation of
-the table materialization can lead to downtime, as target table is dropped and
-re-created. To have the less destructive behavior it's possible to use
-`table='table_hive_ha'` materialization. **table_hive_ha** leverage the table
-versions feature of glue catalog, creating a tmp table and swapping the target
-table to the location of the tmp table. This materialization is only available
-for `table_type=hive` and requires using unique locations. ``` {{ config
-( materialized='table_hive_ha', format='parquet', partition_by=['status'],
-s3_data_naming='table_unique' ) }} select 'a' as user_id, 'pi' as user_name,
-'active' as status union all select 'b' as user_id, 'sh' as user_name,
-'disabled' as status ``` By default, the materialization keeps the last 4 table
-versions, you can change it that setting `versions_to_keep`. #### Known issues
-* When swapping from a table with partitions to a table without (and the other
-way around), there could be a little downtime. In case high performances are
-needed consider bucketing instead of partitions * By default, Glue "duplicate"
-the versions internally, so the last 2 versions of a table point to the same
-location * It's recommended to have versions_to_keep>= 4, as this will avoid to
-have the older location removed * The macro athena__end_of_time needs to be
-overwritten by the user if using Athena v3 since it requires a precision
-parameter for timestamps ## Snapshots The adapter supports snapshot
-materialization. It supports both timestamp and check strategy. To create a
-snapshot create a snapshot file in the snapshots directory. If directory does
-not exist create one. ### Timestamp strategy To use the timestamp strategy
-refer to the [dbt docs](https://docs.getdbt.com/docs/build/snapshots#timestamp-
-strategy-recommended) ### Check strategy To use the check strategy refer to the
-[dbt docs](https://docs.getdbt.com/docs/build/snapshots#check-strategy) ###
-Hard-deletes The materialization also supports invalidating hard deletes. Check
-the [docs](https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
+updated. If `delete_condition` is provided in the model config, it can also
+delete records based on the provided condition (SQL condition). You can use any
+column of the incremental table (`src`) or the final table (`target`). You must
+prefix the column by the name of the table to prevent `Column is ambiguous`
+error. ```sql {{ config( materialized='incremental', table_type='iceberg',
+incremental_strategy='merge', unique_key='user_id',
+delete_condition="src.status != 'active' and target.my_date < now() - interval
+'2' year" format='parquet', ) }} SELECT 'A' AS user_id, 'pi' AS name, 'active'
+AS status, 17.89 AS cost, 1 AS quantity, 100000000 AS quantity_big,
+current_date AS my_date ``` ### High available table materialization The
+current implementation of the table materialization can lead to downtime, as
+target table is dropped and re-created. To have the less destructive behavior
+it's possible to use `table='table_hive_ha'` materialization. **table_hive_ha**
+leverage the table versions feature of glue catalog, creating a tmp table and
+swapping the target table to the location of the tmp table. This
+materialization is only available for `table_type=hive` and requires using
+unique locations. ``` {{ config( materialized='table_hive_ha',
+format='parquet', partition_by=['status'], s3_data_naming='table_unique' ) }}
+select 'a' as user_id, 'pi' as user_name, 'active' as status union all select
+'b' as user_id, 'sh' as user_name, 'disabled' as status ``` By default, the
+materialization keeps the last 4 table versions, you can change it that setting
+`versions_to_keep`. #### Known issues * When swapping from a table with
+partitions to a table without (and the other way around), there could be a
+little downtime. In case high performances are needed consider bucketing
+instead of partitions * By default, Glue "duplicate" the versions internally,
+so the last 2 versions of a table point to the same location * It's recommended
+to have versions_to_keep>= 4, as this will avoid to have the older location
+removed * The macro athena__end_of_time needs to be overwritten by the user if
+using Athena v3 since it requires a precision parameter for timestamps ##
+Snapshots The adapter supports snapshot materialization. It supports both
+timestamp and check strategy. To create a snapshot create a snapshot file in
+the snapshots directory. If directory does not exist create one. ### Timestamp
+strategy To use the timestamp strategy refer to the [dbt docs](https://
+docs.getdbt.com/docs/build/snapshots#timestamp-strategy-recommended) ### Check
+strategy To use the check strategy refer to the [dbt docs](https://
+docs.getdbt.com/docs/build/snapshots#check-strategy) ### Hard-deletes The
+materialization also supports invalidating hard deletes. Check the [docs]
+(https://docs.getdbt.com/docs/build/snapshots#hard-deletes-opt-in) to
 understand usage. ### Working example seed file -
 employent_indicators_november_2022_csv_tables.csv ```
 Series_reference,Period,Data_value,Suppressed MEIM.S1WA,1999.04,80267,
 MEIM.S1WA,1999.05,70803, MEIM.S1WA,1999.06,65792, MEIM.S1WA,1999.07,66194,
 MEIM.S1WA,1999.08,67259, MEIM.S1WA,1999.09,69691, MEIM.S1WA,1999.1,72475,
 MEIM.S1WA,1999.11,79263, MEIM.S1WA,1999.12,86540, MEIM.S1WA,2000.01,82552,
 MEIM.S1WA,2000.02,81709, MEIM.S1WA,2000.03,84126, MEIM.S1WA,2000.04,77089,
@@ -180,37 +190,24 @@
 the incremental model. * Tables, schemas and database should only be lowercase
 * In order to avoid potential conflicts, make sure [`dbt-athena-adapter`]
 (https://github.com/Tomme/dbt-athena) is not installed in the target
 environment. See https://github.com/dbt-athena/dbt-athena/issues/103 for more
 details. * Snapshot does not support dropping columns from the source table. If
 you drop a column make sure to drop the column from the snapshot as well.
 Another workaround is to NULL the column in the snapshot definition to preserve
-history ## Contributing This connector works with Python from 3.7 to 3.11. ###
-Getting started In order to start developing on this adapter clone the repo and
-run this make command (see [Makefile](Makefile)) : ```bash make setup ``` It
-will : 1. Install all dependencies. 2. Install pre-commit hooks. 3. Generate
-your `.env` file Next, adjust `.env` file by configuring the environment
-variables to match your Athena development environment. ### Running tests We
-have 2 different types of testing: * **unit testing**: you can run this type of
-tests running `make unit_test` * **functional testing**: you must have an AWS
-account with Athena setup in order to launch this type of tests and have a
-`.env` file in place with the right values. You can run this type of tests
-running `make functional_test` All type of tests can be run using `make`:
-```bash make test ``` ### Pull Request * Create a commit with your changes and
-push them to a [fork](https://docs.github.com/en/get-started/quickstart/fork-a-
-repo). * Create a [pull request on Github](https://docs.github.com/en/github/
-collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-
-requests/creating-a-pull-request-from-a-fork). * Pull request title and message
-(and PR title and description) must adhere to [conventionalcommits](https://
-www.conventionalcommits.org). * Pull request body should describe _motivation_.
-## Resources * [Athena CREATE TABLE AS](https://docs.aws.amazon.com/athena/
-latest/ug/create-table-as.html) * [dbt-labs/dbt-core](https://github.com/dbt-
-labs/dbt-core) * [laughingman7743/PyAthena](https://github.com/laughingman7743/
-PyAthena) ## Contributors â¨ Thanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)):
-    [nicor88]          [Jesse       [Lemiffe] [JÃ©rÃ©my_Guisel      [Tom]       [Mattia]
-     nicor88         Dobbelaere]     Lemiffe   JÃ©rÃ©my_Guisel       Tom         Mattia
-    ð» ð�Jesse_Dobbelaere    ð¨       ð§         ð§ ð�  ð§
-                      ð ð§
+history ## Contributing See [CONTRIBUTING](CONTRIBUTING.md) for more
+information on how to contribute to this project. ## Contributors â¨ Thanks
+goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
+en/emoji-key)):
+        [nicor88]               [Jesse       [Lemiffe]  [JÃ©rÃ©my_Guiselin      [Tom]       [Mattia] [Gatsby
+         nicor88              Dobbelaere]     Lemiffe    JÃ©rÃ©my_Guiselin       Tom         Mattia    Lee]
+      ð» ð§ ð�Jesse_Dobbelaere    ð¨    ð§ ð» �    ð§ ð�  ð� Gatsby
+                               ð ð§                                                           Lee
+                                                                                                           ð
+      [BrechtDeVlieger]    [Andrea_Artaria]   [Maiara     [Henri_Blancke]          [Serhii
+       BrechtDeVlieger      Andrea_Artaria   Reinaldo]     Henri_Blancke         Dimchenko]
+             ð            ð     Maiara         ð» ðSerhii_Dimchenko
+                                             Reinaldo                             ð» ð
+                                               ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `dbt-athena-community-1.4.3/dbt_athena_community.egg-info/SOURCES.txt` & `dbt-athena-community-1.4.4/dbt_athena_community.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/pyproject.toml` & `dbt-athena-community-1.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt-athena-community-1.4.3/setup.py` & `dbt-athena-community-1.4.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,12 +46,13 @@
     long_description_content_type="text/markdown",
     url="https://github.com/dbt-athena/dbt-athena",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         # In order to control dbt-core version and package version
         "boto3~=1.26",
-        "dbt-core~=1.4.5",
-        "pyathena~=2.24",
+        "boto3-stubs[athena,glue,lakeformation,sts]~=1.26",
+        "dbt-core~=1.4.6",
+        "pyathena~=2.25",
         "tenacity~=8.2",
     ],
 )
```

