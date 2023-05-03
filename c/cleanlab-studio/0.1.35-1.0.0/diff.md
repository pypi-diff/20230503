# Comparing `tmp/cleanlab-studio-0.1.35.tar.gz` & `tmp/cleanlab-studio-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-0.1.35.tar", last modified: Wed Apr 19 20:25:52 2023, max compression
+gzip compressed data, was "cleanlab-studio-1.0.0.tar", last modified: Wed May  3 02:00:04 2023, max compression
```

## Comparing `cleanlab-studio-0.1.35.tar` & `cleanlab-studio-1.0.0.tar`

### file list

```diff
@@ -1,70 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:52.718254 cleanlab-studio-0.1.35/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-19 20:25:52.718254 cleanlab-studio-0.1.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:52.698255 cleanlab-studio-0.1.35/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:52.702255 cleanlab-studio-0.1.35/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:52.706255 cleanlab-studio-0.1.35/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:52.706255 cleanlab-studio-0.1.35/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:52.710255 cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/schema_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12412 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/upload_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:52.710255 cleanlab-studio-0.1.35/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:52.714254 cleanlab-studio-0.1.35/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:52.714254 cleanlab-studio-0.1.35/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:52.698255 cleanlab-studio-0.1.35/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-19 20:25:52.000000 cleanlab-studio-0.1.35/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-19 20:25:52.000000 cleanlab-studio-0.1.35/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:25:52.000000 cleanlab-studio-0.1.35/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 20:25:52.000000 cleanlab-studio-0.1.35/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-19 20:25:52.000000 cleanlab-studio-0.1.35/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 20:25:52.000000 cleanlab-studio-0.1.35/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:25:52.718254 cleanlab-studio-0.1.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:52.714254 cleanlab-studio-0.1.35/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/tests/bench.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:52.714254 cleanlab-studio-0.1.35/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/tests/commands/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:52.718254 cleanlab-studio-0.1.35/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/tests/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/tests/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/tests/datasets/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/tests/datasets/test_excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/tests/datasets/test_json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-19 20:25:24.000000 cleanlab-studio-0.1.35/tests/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.917315 cleanlab-studio-1.0.0/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.925315 cleanlab-studio-1.0.0/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.925315 cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.925315 cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.925315 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/schema_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/upload_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.925315 cleanlab-studio-1.0.0/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.925315 cleanlab-studio-1.0.0/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/studio/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.921315 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-03 02:00:04.000000 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-03 02:00:04.000000 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:00:04.000000 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 02:00:04.000000 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-03 02:00:04.000000 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-03 02:00:04.000000 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/bench.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/datasets/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/datasets/test_excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/datasets/test_json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/datasets/utils.py
```

### Comparing `cleanlab-studio-0.1.35/LICENSE` & `cleanlab-studio-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/api_service.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/api_service.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/classes/dataset.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,11 +60,13 @@
         """Preprocesses record value.
         Operations performed:
             - Cast datetimes to strings
 
         :param record_value: record value to preprocess
         :return: preprocessed record value
         """
-        if isinstance(record_value, (datetime.date, datetime.time, datetime.datetime, pd.Timestamp)):
+        if isinstance(
+            record_value, (datetime.date, datetime.time, datetime.datetime, pd.Timestamp)
+        ):
             return record_value.isoformat()
 
         return record_value
```

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/cleanset/download.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from cleanlab_studio.cli import click_helpers
 from cleanlab_studio.cli import util
 from cleanlab_studio.cli.cleanset.download_helpers import combine_fields_with_dataset
 from cleanlab_studio.cli.click_helpers import log, progress
 from cleanlab_studio.cli.decorators import previous_state, auth_config
 from cleanlab_studio.cli.decorators.auth_config import AuthConfig
 from cleanlab_studio.cli.decorators.previous_state import PreviousState
-from cleanlab_studio.cli.settings import CleanlabSettings
-from cleanlab_studio.cli.types import IDType, RecordType, DatasetFileExtension
+from cleanlab_studio.cli.types import RecordType, DatasetFileExtension
+from cleanlab_studio.internal.settings import CleanlabSettings
 
 
 @click.command(help="download Cleanlab columns")
 @click.option(
     "--id",
     type=str,
     prompt=True,
```

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/click_helpers.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/helpers.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/image_utils.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/image_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     FeatureType,
     MEDIA_FEATURE_TYPES,
     Schema,
 )
 from cleanlab_studio.cli.types import Modality
 from cleanlab_studio.cli.util import dump_json
 from cleanlab_studio.errors import ColumnMismatchError, EmptyDatasetError
+from cleanlab_studio.internal.types import JSONDict
 from cleanlab_studio.version import MAX_SCHEMA_VERSION, MIN_SCHEMA_VERSION, SCHEMA_VERSION
 
 
 def _find_best_matching_column(target_column: str, columns: List[str]) -> Optional[str]:
     """
     Find the column from `columns` that is the closest match to the `target_col`.
     If no columns are likely, pick the first column of `columns`
@@ -57,36 +58,27 @@
 
     if len(poss) > 0:  # pick first possibility
         return poss[0]
     else:
         return columns[0]
 
 
-def load_schema(filepath: str) -> Schema:
+def load_schema(filepath: str) -> JSONDict:
     with open(filepath, "r") as f:
-        schema_dict = json.load(f)
-        schema: Schema = Schema.create(
-            metadata=schema_dict["metadata"],
-            fields=schema_dict["fields"],
-            version=schema_dict["version"],
-        )
-        return schema
+        schema_dict: JSONDict = json.load(f)
+        return schema_dict
 
 
-def validate_schema(schema: Schema, columns: Collection[str]) -> None:
+def validate_schema(schema: Schema) -> None:
     """
     Checks that:
     (1) all schema column names are strings
-    (2) all schema columns exist in the dataset columns
-    (3) all schema column types are recognized
-
+    (2) all schema column types are recognized
     Note that schema initialization already checks that all keys are present and that fields are valid.
-
     :param schema:
-    :param columns: full list of columns in dataset
     :return: raises a ValueError if any checks fail
     """
 
     # check schema version validity
     schema_version = schema.version
     if (
         semver.VersionInfo.parse(MIN_SCHEMA_VERSION).compare(schema_version) == 1
@@ -96,22 +88,16 @@
             "A new schema should be generated using 'cleanlab dataset schema generate'"
         )
     elif semver.VersionInfo.parse(MAX_SCHEMA_VERSION).compare(schema_version) == -1:
         raise ValueError(
             "CLI is not up to date with your schema version. Run 'pip install --upgrade cleanlab-studio'."
         )
 
-    schema_columns = set(schema.fields)
-    columns = set(columns)
     metadata = schema.metadata
 
-    ## Check that the dataset has all columns specified in the schema
-    if not schema_columns.issubset(columns):
-        raise ValueError(f"Dataset is missing schema columns: {schema_columns - columns}")
-
     # Advanced validation checks: this should be aligned with ConfirmSchema's validate() function
     ## Check that specified ID column has the feature_type 'identifier'
     id_column_name = metadata.id_column
     id_column_spec_feature_type = schema.fields[id_column_name].feature_type
     if id_column_spec_feature_type != FeatureType.identifier:
         raise ValueError(
             f"ID column field {id_column_name} must have feature type: 'identifier', but has"
@@ -400,26 +386,26 @@
 
     assert id_column is not None
 
     metadata: Dict[str, Optional[str]] = dict(id_column=id_column, modality=modality, name=name)
     return Schema.create(metadata=metadata, fields=fields_dict, version=SCHEMA_VERSION)
 
 
-def save_schema(schema: Schema, filename: Optional[str]) -> None:
+def save_schema(schema: JSONDict, filename: Optional[str]) -> None:
     """
 
     :param schema:
     :param filename: filename to save schema with
     :return:
     """
     if filename == "":
         filename = "schema.json"
     if filename:
         progress(f"Writing schema to {filename}...")
-        dump_json(filename, schema.to_dict())
+        dump_json(filename, schema)
         success("Saved.")
     else:
         info("Schema was not saved.")
 
 
 def get_dataset_filepath_columns(
     dataset: Union[Dataset[IO[bytes]], Dataset[IO[str]]], schema: Schema
```

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/schema_types.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/schema_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/upload_helpers.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/dataset/upload_types.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/upload_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
-from cleanlab_studio.cli.api_service import validate_api_key
 from cleanlab_studio.cli.click_helpers import abort
-from cleanlab_studio.cli.settings import CleanlabSettings
+from cleanlab_studio.internal.api import validate_api_key
+from cleanlab_studio.internal.settings import CleanlabSettings
 from typing import Optional
 
 
 class AuthConfig:
     def __init__(self) -> None:
         self.api_key: Optional[str] = None
```

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import click
 import json
 import os
-from cleanlab_studio.cli.settings import CleanlabSettings
 from cleanlab_studio.cli.types import CommandState
+from cleanlab_studio.internal.settings import CleanlabSettings
 from typing import Dict, Any, Optional
 
 FILENAME = "state.json"
 
 
 class PreviousState:
     def __init__(self) -> None:
```

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/login/login.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/login/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from cleanlab_studio.cli.api_service import validate_api_key
 from cleanlab_studio.cli.click_helpers import *
 from cleanlab_studio.cli.decorators.previous_state import PreviousState
-from cleanlab_studio.cli.settings import CleanlabSettings
 from cleanlab_studio.cli.decorators import previous_state
+from cleanlab_studio.internal.settings import CleanlabSettings
 import click
 
 
 @click.command(help="authentication for Cleanlab Studio")
 @click.option(
     "--key",
     "--k",
```

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/main.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import subprocess
 
 from cleanlab_studio.cli import api_service
 from cleanlab_studio.cli.click_helpers import abort
 from cleanlab_studio.cli.dataset.commands import dataset
 from cleanlab_studio.cli.cleanset.commands import cleanset
 from cleanlab_studio.cli.login.login import login
-from cleanlab_studio.cli.settings import CleanlabSettings
+from cleanlab_studio.internal.settings import CleanlabSettings
 from cleanlab_studio.version import __version__
 
 
 @click.group()
 @click.pass_context
 def cli(ctx: click.Context) -> None:
     if ctx.invoked_subcommand == "version":
```

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/settings.py` & `cleanlab-studio-1.0.0/cleanlab_studio/internal/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
-from typing import Optional, Dict, Any
+from typing import Optional
 import semver
 
 from cleanlab_studio.version import SETTINGS_VERSION, MIN_SETTINGS_VERSION, MAX_SETTINGS_VERSION
-from cleanlab_studio.cli.types import CleanlabSettingsDict
+from cleanlab_studio.internal.types import CleanlabSettingsDict
 
 
 class CleanlabSettings:
     def __init__(self, version: Optional[str], api_key: Optional[str]):
         self.version = version
         self.api_key = api_key
```

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/types.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio/cli/util.py` & `cleanlab-studio-1.0.0/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab-studio-1.0.0/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 cleanlab_studio.egg-info/entry_points.txt
 cleanlab_studio.egg-info/requires.txt
 cleanlab_studio.egg-info/top_level.txt
 cleanlab_studio/cli/__init__.py
 cleanlab_studio/cli/api_service.py
 cleanlab_studio/cli/click_helpers.py
 cleanlab_studio/cli/main.py
-cleanlab_studio/cli/settings.py
 cleanlab_studio/cli/types.py
 cleanlab_studio/cli/util.py
 cleanlab_studio/cli/classes/__init__.py
 cleanlab_studio/cli/classes/csv_dataset.py
 cleanlab_studio/cli/classes/dataset.py
 cleanlab_studio/cli/classes/excel_dataset.py
 cleanlab_studio/cli/classes/json_dataset.py
@@ -27,29 +26,41 @@
 cleanlab_studio/cli/cleanset/commands.py
 cleanlab_studio/cli/cleanset/download.py
 cleanlab_studio/cli/cleanset/download_helpers.py
 cleanlab_studio/cli/dataset/__init__.py
 cleanlab_studio/cli/dataset/commands.py
 cleanlab_studio/cli/dataset/helpers.py
 cleanlab_studio/cli/dataset/image_utils.py
-cleanlab_studio/cli/dataset/schema.py
 cleanlab_studio/cli/dataset/schema_helpers.py
 cleanlab_studio/cli/dataset/schema_types.py
 cleanlab_studio/cli/dataset/upload.py
 cleanlab_studio/cli/dataset/upload_helpers.py
 cleanlab_studio/cli/dataset/upload_types.py
 cleanlab_studio/cli/decorators/__init__.py
 cleanlab_studio/cli/decorators/auth_config.py
 cleanlab_studio/cli/decorators/previous_state.py
 cleanlab_studio/cli/login/__init__.py
 cleanlab_studio/cli/login/login.py
 cleanlab_studio/internal/__init__.py
+cleanlab_studio/internal/settings.py
+cleanlab_studio/internal/types.py
+cleanlab_studio/internal/upload_helpers.py
+cleanlab_studio/internal/util.py
+cleanlab_studio/internal/api/__init__.py
+cleanlab_studio/internal/api/api.py
+cleanlab_studio/internal/dataset_source/__init__.py
+cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+cleanlab_studio/internal/dataset_source/dataset_source.py
+cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+cleanlab_studio/studio/__init__.py
+cleanlab_studio/studio/studio.py
+cleanlab_studio/studio/upload.py
 tests/__init__.py
 tests/bench.py
-tests/commands/__init__.py
-tests/commands/test_schema.py
 tests/datasets/__init__.py
 tests/datasets/constants.py
 tests/datasets/test_csv_dataset.py
 tests/datasets/test_excel_dataset.py
 tests/datasets/test_json_dataset.py
 tests/datasets/utils.py
```

### Comparing `cleanlab-studio-0.1.35/setup.py` & `cleanlab-studio-1.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         "pyexcel>=0.7.0",
         "pyexcel-xls>=0.7.0",
         "pyexcel-xlsx>=0.6.0",
         "requests>=2.27.1",
         "tqdm>=4.64.0",
         "ijson>=3.1.4",
         "jsonstreams>=0.6.0",
-        "semver>=2.13.0",
+        "semver>=2.13.0,<3.0.0",
         "Pillow>=9.2.0",
         "openpyxl==3.0.10",
         "validators>=0.20.0",
     ],
     entry_points="""
         [console_scripts]
         cleanlab=cleanlab_studio.cli:main
```

### Comparing `cleanlab-studio-0.1.35/tests/bench.py` & `cleanlab-studio-1.0.0/tests/bench.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/tests/datasets/test_csv_dataset.py` & `cleanlab-studio-1.0.0/tests/datasets/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/tests/datasets/test_excel_dataset.py` & `cleanlab-studio-1.0.0/tests/datasets/test_excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/tests/datasets/test_json_dataset.py` & `cleanlab-studio-1.0.0/tests/datasets/test_json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-0.1.35/tests/datasets/utils.py` & `cleanlab-studio-1.0.0/tests/datasets/utils.py`

 * *Files identical despite different names*

