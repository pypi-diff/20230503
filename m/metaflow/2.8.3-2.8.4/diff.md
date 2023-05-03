# Comparing `tmp/metaflow-2.8.3.tar.gz` & `tmp/metaflow-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-2.8.3.tar", last modified: Wed Apr 12 18:52:36 2023, max compression
+gzip compressed data, was "metaflow-2.8.4.tar", last modified: Wed May  3 03:04:27 2023, max compression
```

## Comparing `metaflow-2.8.3.tar` & `metaflow-2.8.4.tar`

### file list

```diff
@@ -1,331 +1,334 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-12 18:52:25.000000 metaflow-2.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 18:52:25.000000 metaflow-2.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-12 18:52:36.890292 metaflow-2.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-12 18:52:25.000000 metaflow-2.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.866292 metaflow-2.8.3/metaflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/R.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.866292 metaflow-2.8.3/metaflow/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/_vendor/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/_bashcomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/_termui_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/_textwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/_unicodefun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/_winconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/_vendor/v3_5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/_vendor/v3_5/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_5/zipp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/_vendor/v3_6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/_vendor/v3_6/zipp.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63753 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/client/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/client/filecache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31039 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cmd/configure_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cmd/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cmd/tutorials_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cmd/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/cmd_with_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.870292 metaflow-2.8.3/metaflow/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/content_addressed_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/datastore_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/datastore_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/flow_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/datastore/task_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/event_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/extension_support/
--rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/extension_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/extension_support/_empty_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/extension_support/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/extension_support/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/extension_support/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/flowspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/includefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metadata/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metadata/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metaflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metaflow_config_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metaflow_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metaflow_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/metaflow_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/mflog/
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/mflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/mflog/mflog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/mflog/save_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/mflog/save_logs_periodically.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/mflog/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/multicore_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30229 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/airflow_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/airflow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/plugins/airflow/plumbing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/plumbing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/plumbing/set_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.874292 metaflow-2.8.3/metaflow/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/sensors/base_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/sensors/external_task_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/airflow/sensors/s3_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/argo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/argo/argo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    58089 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/argo/argo_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    17737 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/argo/argo_workflows_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/argo/argo_workflows_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/argo/process_input_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/aws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16118 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/batch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/batch/batch_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23960 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/batch/batch_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15590 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/batch/batch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/secrets_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/dynamo_db_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/event_bridge_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/production_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/schedule_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/set_batch_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42073 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/azure/azure_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/azure/azure_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/azure/azure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/azure/blob_service_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/azure/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.878292 metaflow-2.8.3/metaflow/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/convert_to_native_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/renderer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_modules/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/card_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/component_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/cards/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/catch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/conda/batch_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/conda/conda_step_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/datastores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datastores/azure_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datastores/gs_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datastores/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datastores/s3_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62975 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/s3/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/s3/s3op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/s3/s3tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/datatools/s3/s3util.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/debug_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/debug_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.882292 metaflow-2.8.3/metaflow/plugins/env_escape/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/client_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/env_escape/communication/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/communication/bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/communication/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/communication/socket_bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/communication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/test_lib_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/data_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/exception_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/override_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/env_escape/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/environment_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/frameworks/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/gcp/gs_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/gcp/gs_storage_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/gcp/gs_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/gcp/gs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/gcp/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17409 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/metadata/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/metadata/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/package_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/parallel_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/project_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/resources_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/retry_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/secrets/inline_secrets_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/secrets/secrets_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/storage_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/tag_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/test_unbounded_foreach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/plugins/timeout_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/procpoll.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/pylint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/sidecar/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/sidecar/sidecar_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/sidecar/sidecar_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/sidecar/sidecar_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tagging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.862292 metaflow-2.8.3/metaflow/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/tutorials/00-helloworld/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/00-helloworld/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/00-helloworld/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.886292 metaflow-2.8.3/metaflow/tutorials/01-playlist/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/01-playlist/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/01-playlist/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/01-playlist/playlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/01-playlist/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/02-statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/02-statistics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/02-statistics/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/02-statistics/stats.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/02-statistics/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/03-playlist-redux/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/03-playlist-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/03-playlist-redux/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/04-playlist-plus/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/04-playlist-plus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/04-playlist-plus/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/hello-cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/06-statistics-redux/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/06-statistics-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/06-statistics-redux/stats.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/07-worldview/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/07-worldview/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/07-worldview/worldview.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.890292 metaflow-2.8.3/metaflow/tutorials/08-autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/08-autopilot/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/tutorials/08-autopilot/autopilot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/unbounded_foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-12 18:52:25.000000 metaflow-2.8.3/metaflow/vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:52:36.866292 metaflow-2.8.3/metaflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-12 18:52:36.000000 metaflow-2.8.3/metaflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10861 2023-04-12 18:52:36.000000 metaflow-2.8.3/metaflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:52:36.000000 metaflow-2.8.3/metaflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 18:52:36.000000 metaflow-2.8.3/metaflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 18:52:36.000000 metaflow-2.8.3/metaflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 18:52:36.000000 metaflow-2.8.3/metaflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 18:52:36.890292 metaflow-2.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-12 18:52:25.000000 metaflow-2.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.333938 metaflow-2.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-03 03:04:13.000000 metaflow-2.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-03 03:04:13.000000 metaflow-2.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-03 03:04:27.333938 metaflow-2.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-03 03:04:13.000000 metaflow-2.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.305938 metaflow-2.8.4/metaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/R.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.309938 metaflow-2.8.4/metaflow/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.309938 metaflow-2.8.4/metaflow/_vendor/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/_bashcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/_unicodefun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.309938 metaflow-2.8.4/metaflow/_vendor/v3_5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.309938 metaflow-2.8.4/metaflow/_vendor/v3_5/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_5/zipp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.309938 metaflow-2.8.4/metaflow/_vendor/v3_6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.313938 metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_6/typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/_vendor/v3_6/zipp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.313938 metaflow-2.8.4/metaflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68712 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/client/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/client/filecache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.313938 metaflow-2.8.4/metaflow/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31039 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/cmd/configure_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/cmd/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/cmd/tutorials_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/cmd/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/cmd_with_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.313938 metaflow-2.8.4/metaflow/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/datastore/content_addressed_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/datastore/datastore_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/datastore/datastore_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/datastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/datastore/flow_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/datastore/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/datastore/task_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/event_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.313938 metaflow-2.8.4/metaflow/extension_support/
+-rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/extension_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/extension_support/_empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/extension_support/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/extension_support/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/extension_support/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/flowspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/includefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.313938 metaflow-2.8.4/metaflow/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/metadata/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/metadata/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/metaflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/metaflow_config_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/metaflow_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/metaflow_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/metaflow_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.317938 metaflow-2.8.4/metaflow/mflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/mflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/mflog/mflog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/mflog/save_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/mflog/save_logs_periodically.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/mflog/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/multicore_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.317938 metaflow-2.8.4/metaflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.317938 metaflow-2.8.4/metaflow/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31282 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/airflow/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/airflow/airflow_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/airflow/airflow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/airflow/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/airflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/airflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.317938 metaflow-2.8.4/metaflow/plugins/airflow/plumbing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/airflow/plumbing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/airflow/plumbing/set_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.317938 metaflow-2.8.4/metaflow/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/airflow/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/airflow/sensors/base_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/airflow/sensors/external_task_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/airflow/sensors/s3_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.317938 metaflow-2.8.4/metaflow/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/argo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/argo/argo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/argo/argo_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96242 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/argo/argo_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/argo/argo_workflows_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/argo/argo_workflows_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/argo/process_input_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.317938 metaflow-2.8.4/metaflow/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/aws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.321938 metaflow-2.8.4/metaflow/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16114 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/batch/batch_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/batch/batch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/batch/batch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.321938 metaflow-2.8.4/metaflow/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.321938 metaflow-2.8.4/metaflow/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/step_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/step_functions/dynamo_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/step_functions/event_bridge_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/step_functions/production_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/step_functions/schedule_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/step_functions/set_batch_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/step_functions/step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/step_functions/step_functions_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/step_functions/step_functions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/aws/step_functions/step_functions_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.321938 metaflow-2.8.4/metaflow/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/azure/azure_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/azure/azure_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/azure/azure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/azure/blob_service_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/azure/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.321938 metaflow-2.8.4/metaflow/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.321938 metaflow-2.8.4/metaflow/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.321938 metaflow-2.8.4/metaflow/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/chevron/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/chevron/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/chevron/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/chevron/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/convert_to_native_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/renderer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_modules/test_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/card_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/component_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/cards/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/catch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.321938 metaflow-2.8.4/metaflow/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/conda/batch_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/conda/conda_step_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.325938 metaflow-2.8.4/metaflow/plugins/datastores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/datastores/azure_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/datastores/gs_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/datastores/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/datastores/s3_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.325938 metaflow-2.8.4/metaflow/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/datatools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/datatools/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.325938 metaflow-2.8.4/metaflow/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/datatools/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62975 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/datatools/s3/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/datatools/s3/s3op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/datatools/s3/s3tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/datatools/s3/s3util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/debug_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/debug_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.325938 metaflow-2.8.4/metaflow/plugins/env_escape/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/client_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.325938 metaflow-2.8.4/metaflow/plugins/env_escape/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/communication/bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/communication/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/communication/socket_bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/communication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.325938 metaflow-2.8.4/metaflow/plugins/env_escape/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.325938 metaflow-2.8.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.325938 metaflow-2.8.4/metaflow/plugins/env_escape/configurations/test_lib_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/data_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/exception_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/override_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/env_escape/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/environment_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/events_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.325938 metaflow-2.8.4/metaflow/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/frameworks/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.325938 metaflow-2.8.4/metaflow/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/gcp/gs_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/gcp/gs_storage_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/gcp/gs_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/gcp/gs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/gcp/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.325938 metaflow-2.8.4/metaflow/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13314 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/kubernetes/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/kubernetes/kubernetes_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/kubernetes/kubernetes_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19331 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/kubernetes/kubernetes_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26188 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/kubernetes/kubernetes_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.329938 metaflow-2.8.4/metaflow/plugins/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/metadata/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/metadata/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/package_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/parallel_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/project_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/resources_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/retry_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.329938 metaflow-2.8.4/metaflow/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/secrets/inline_secrets_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/secrets/secrets_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/storage_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/tag_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/test_unbounded_foreach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/plugins/timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/procpoll.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/pylint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.329938 metaflow-2.8.4/metaflow/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/sidecar/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/sidecar/sidecar_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/sidecar/sidecar_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/sidecar/sidecar_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tagging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.305938 metaflow-2.8.4/metaflow/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.329938 metaflow-2.8.4/metaflow/tutorials/00-helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/00-helloworld/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/00-helloworld/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.329938 metaflow-2.8.4/metaflow/tutorials/01-playlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/01-playlist/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/01-playlist/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/01-playlist/playlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/01-playlist/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.329938 metaflow-2.8.4/metaflow/tutorials/02-statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/02-statistics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/02-statistics/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/02-statistics/stats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/02-statistics/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.329938 metaflow-2.8.4/metaflow/tutorials/03-playlist-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/03-playlist-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/03-playlist-redux/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.329938 metaflow-2.8.4/metaflow/tutorials/04-playlist-plus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/04-playlist-plus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/04-playlist-plus/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.333938 metaflow-2.8.4/metaflow/tutorials/05-hello-cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/05-hello-cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/05-hello-cloud/hello-cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.333938 metaflow-2.8.4/metaflow/tutorials/06-statistics-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/06-statistics-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/06-statistics-redux/stats.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.333938 metaflow-2.8.4/metaflow/tutorials/07-worldview/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/07-worldview/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/07-worldview/worldview.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.333938 metaflow-2.8.4/metaflow/tutorials/08-autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/08-autopilot/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/tutorials/08-autopilot/autopilot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/unbounded_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-03 03:04:13.000000 metaflow-2.8.4/metaflow/vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:04:27.309938 metaflow-2.8.4/metaflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-03 03:04:27.000000 metaflow-2.8.4/metaflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-03 03:04:27.000000 metaflow-2.8.4/metaflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 03:04:27.000000 metaflow-2.8.4/metaflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 03:04:27.000000 metaflow-2.8.4/metaflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 03:04:27.000000 metaflow-2.8.4/metaflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 03:04:27.000000 metaflow-2.8.4/metaflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-03 03:04:27.333938 metaflow-2.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-03 03:04:13.000000 metaflow-2.8.4/setup.py
```

### Comparing `metaflow-2.8.3/LICENSE` & `metaflow-2.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/PKG-INFO` & `metaflow-2.8.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow
-Version: 2.8.3
+Version: 2.8.4
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
```

### Comparing `metaflow-2.8.3/README.md` & `metaflow-2.8.4/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/R.py` & `metaflow-2.8.4/metaflow/R.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/__init__.py` & `metaflow-2.8.4/metaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/__init__.py` & `metaflow-2.8.4/metaflow/_vendor/click/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/_bashcomplete.py` & `metaflow-2.8.4/metaflow/_vendor/click/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/_compat.py` & `metaflow-2.8.4/metaflow/_vendor/click/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/_termui_impl.py` & `metaflow-2.8.4/metaflow/_vendor/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/_textwrap.py` & `metaflow-2.8.4/metaflow/_vendor/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/_unicodefun.py` & `metaflow-2.8.4/metaflow/_vendor/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/_winconsole.py` & `metaflow-2.8.4/metaflow/_vendor/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/core.py` & `metaflow-2.8.4/metaflow/_vendor/click/core.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/decorators.py` & `metaflow-2.8.4/metaflow/_vendor/click/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/exceptions.py` & `metaflow-2.8.4/metaflow/_vendor/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/formatting.py` & `metaflow-2.8.4/metaflow/_vendor/click/formatting.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/globals.py` & `metaflow-2.8.4/metaflow/_vendor/click/globals.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/parser.py` & `metaflow-2.8.4/metaflow/_vendor/click/parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/termui.py` & `metaflow-2.8.4/metaflow/_vendor/click/termui.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/testing.py` & `metaflow-2.8.4/metaflow/_vendor/click/testing.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/types.py` & `metaflow-2.8.4/metaflow/_vendor/click/types.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/click/utils.py` & `metaflow-2.8.4/metaflow/_vendor/click/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/v3_5/importlib_metadata/__init__.py` & `metaflow-2.8.4/metaflow/_vendor/v3_5/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/v3_5/importlib_metadata/_compat.py` & `metaflow-2.8.4/metaflow/_vendor/v3_5/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/v3_5/zipp.py` & `metaflow-2.8.4/metaflow/_vendor/v3_5/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/__init__.py` & `metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py` & `metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_collections.py` & `metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_compat.py` & `metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_functools.py` & `metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py` & `metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_meta.py` & `metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/v3_6/importlib_metadata/_text.py` & `metaflow-2.8.4/metaflow/_vendor/v3_6/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/v3_6/typing_extensions.py` & `metaflow-2.8.4/metaflow/_vendor/v3_6/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/_vendor/v3_6/zipp.py` & `metaflow-2.8.4/metaflow/_vendor/v3_6/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/cli.py` & `metaflow-2.8.4/metaflow/cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/cli_args.py` & `metaflow-2.8.4/metaflow/cli_args.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/client/core.py` & `metaflow-2.8.4/metaflow/client/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 from __future__ import print_function
-from datetime import datetime
+
+import json
 import os
 import tarfile
-import json
-from io import BytesIO
 from collections import namedtuple
+from datetime import datetime
+from io import BytesIO
 from itertools import chain
-from typing import (
-    Any,
-    Dict,
-    FrozenSet,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
-)
+from typing import Any, Dict, FrozenSet, Iterable, List, Optional, Tuple
 
-from metaflow.metaflow_environment import MetaflowEnvironment
 from metaflow.current import current
+from metaflow.events import Trigger
 from metaflow.exception import (
-    MetaflowNotFound,
-    MetaflowNamespaceMismatch,
     MetaflowInternalError,
+    MetaflowInvalidPathspec,
+    MetaflowNamespaceMismatch,
+    MetaflowNotFound,
 )
 from metaflow.includefile import IncludedFile
 from metaflow.metaflow_config import DEFAULT_METADATA, MAX_ATTEMPTS
+from metaflow.metaflow_environment import MetaflowEnvironment
 from metaflow.plugins import ENVIRONMENTS, METADATA_PROVIDERS
 from metaflow.unbounded_foreach import CONTROL_TASK_TAG
-from metaflow.util import cached_property, resolve_identity, to_unicode, is_stringish
+from metaflow.util import cached_property, is_stringish, resolve_identity, to_unicode
 
-from .filecache import FileCache
 from .. import INFO_FILE
+from .filecache import FileCache
 
 try:
     # python2
     import cPickle as pickle
 except:  # noqa E722
     # python3
     import pickle
@@ -286,31 +281,46 @@
             # NOTE: It is possible that no attempt exists, but we can't
             # distinguish between "attempt will happen" and "no such
             # attempt exists".
 
         if pathspec:
             ids = pathspec.split("/")
 
+            if self._NAME == "flow" and len(ids) != 1:
+                raise MetaflowInvalidPathspec("Expects Flow('FlowName')")
+            elif self._NAME == "run" and len(ids) != 2:
+                raise MetaflowInvalidPathspec("Expects Run('FlowName/RunID')")
+            elif self._NAME == "step" and len(ids) != 3:
+                raise MetaflowInvalidPathspec("Expects Step('FlowName/RunID/StepName')")
+            elif self._NAME == "task" and len(ids) != 4:
+                raise MetaflowInvalidPathspec(
+                    "Expects Task('FlowName/RunID/StepName/TaskID')"
+                )
+            elif self._NAME == "artifact" and len(ids) != 5:
+                raise MetaflowInvalidPathspec(
+                    "Expects DataArtifact('FlowName/RunID/StepName/TaskID/ArtifactName')"
+                )
+
             self.id = ids[-1]
             self._pathspec = pathspec
             self._object = self._get_object(*ids)
         else:
             self._object = _object
             self._pathspec = pathspec
 
-        if self._NAME in ("flow", "task"):
-            self.id = str(self._object[self._NAME + "_id"])
-        elif self._NAME == "run":
-            self.id = str(self._object["run_number"])
-        elif self._NAME == "step":
-            self.id = str(self._object["step_name"])
-        elif self._NAME == "artifact":
-            self.id = str(self._object["name"])
-        else:
-            raise MetaflowInternalError(msg="Unknown type: %s" % self._NAME)
+            if self._NAME in ("flow", "task"):
+                self.id = str(self._object[self._NAME + "_id"])
+            elif self._NAME == "run":
+                self.id = str(self._object["run_number"])
+            elif self._NAME == "step":
+                self.id = str(self._object["step_name"])
+            elif self._NAME == "artifact":
+                self.id = str(self._object["name"])
+            else:
+                raise MetaflowInternalError(msg="Unknown type: %s" % self._NAME)
 
         self._created_at = datetime.fromtimestamp(self._object["ts_epoch"] / 1000.0)
 
         self._tags = frozenset(
             chain(self._object.get("system_tags") or [], self._object.get("tags") or [])
         )
         self._user_tags = frozenset(self._object.get("tags") or [])
@@ -336,15 +346,16 @@
 
         Returns
         -------
         Iterable[MetaflowObject]
             Iterator over all children
         """
         query_filter = {}
-        # skip namespace filtering if _namespace_check is False
+
+        # skip namespace filtering if _namespace_check is unset.
         if self._namespace_check and current_namespace:
             query_filter = {"any_tags": current_namespace}
 
         unfiltered_children = self._metaflow.metadata.get_object(
             self._NAME,
             _CLASSES[self._CHILD_CLASS]._NAME,
             query_filter,
@@ -471,14 +482,68 @@
         Returns
         -------
         bool
             True if the child exists or False otherwise
         """
         return bool(self._get_child(id))
 
+    def _unpickle_284(self, data):
+        if len(data) != 3:
+            raise MetaflowInternalError(
+                "Unexpected size of array: {}".format(len(data))
+            )
+        pathspec, attempt, namespace_check = data
+        self.__init__(
+            pathspec=pathspec, attempt=attempt, _namespace_check=namespace_check
+        )
+
+    _UNPICKLE_FUNC = {"2.8.4": _unpickle_284}
+
+    def __setstate__(self, state):
+        """
+        This function is used during the unpickling operation.
+        More info here https://docs.python.org/3/library/pickle.html#object.__setstate__
+        """
+        if "version" in state and "data" in state:
+            version = state["version"]
+            if version not in self._UNPICKLE_FUNC:
+                # this happens when an object pickled using a newer version of Metaflow is
+                # being un-pickled using an older version of Metaflow
+                raise MetaflowInternalError(
+                    "Unpickling this object requires a Metaflow version greater than or equal to {}".format(
+                        version
+                    )
+                )
+            self._UNPICKLE_FUNC[version](self, state["data"])
+        else:
+            # For backward compatibility: handles pickled objects that were serialized without a __getstate__ override
+            self.__init__(
+                pathspec=state.get("_pathspec", None),
+                attempt=state.get("_attempt", None),
+                _namespace_check=state.get("_namespace_check", True),
+            )
+
+    def __getstate__(self):
+        """
+        This function is used during the pickling operation.
+        More info here https://docs.python.org/3/library/pickle.html#object.__getstate__
+
+        This function is not forward compatible i.e., if this object (or any of the objects deriving
+        from this object) are pickled (serialized) in a later version of Metaflow, it may not be possible
+        to unpickle (deserialize) them in a previous version of Metaflow.
+        """
+        return {
+            "version": "2.8.4",
+            "data": [
+                self.pathspec,
+                self._attempt,
+                self._namespace_check,
+            ],
+        }
+
     @property
     def tags(self) -> FrozenSet[str]:
         """
         Tags associated with this object.
 
         Tags can be user defined or system defined. This returns all tags associated
         with the object.
@@ -675,15 +740,15 @@
     def __repr__(self):
         return str(self)
 
 
 class MetaflowCode(object):
     """
     Snapshot of the code used to execute this `Run`. Instantiate the object through
-    `Run(...).code` (if all steps are executed remotely) or `Task(...).code` for an
+    `Run(...).code` (if any step is executed remotely) or `Task(...).code` for an
     individual task. The code package is the same for all steps of a `Run`.
 
     `MetaflowCode` includes a package of the user-defined `FlowSpec` class and supporting
     files, as well as a snapshot of the Metaflow library itself.
 
     Currently, `MetaflowCode` objects are stored only for `Run`s that have at least one `Step`
     executing outside the user's local environment.
@@ -899,14 +964,20 @@
         Returns
         -------
         datetime
             Creation time
         """
         return self.created_at
 
+    def __getstate__(self):
+        return super(DataArtifact, self).__getstate__()
+
+    def __setstate__(self, state):
+        super(DataArtifact, self).__setstate__(state)
+
 
 class Task(MetaflowObject):
     """
     A `Task` represents an execution of a `Step`.
 
     It contains all `DataArtifact` objects produced by the task as
     well as metadata related to execution.
@@ -1444,14 +1515,20 @@
             filecache = FileCache()
         attempt = self.current_attempt
 
         return filecache.get_log_size(
             ds_type, ds_root, stream, attempt, *self.path_components
         )
 
+    def __getstate__(self):
+        return super(Task, self).__getstate__()
+
+    def __setstate__(self, state):
+        super(Task, self).__setstate__(state)
+
 
 class Step(MetaflowObject):
     """
     A `Step` represents a user-defined step, that is, a method annotated with the `@step` decorator.
 
     It contains `Task` objects associated with the step, that is, all executions of the
     `Step`. The step may contain multiple `Task`s in the case of a foreach step.
@@ -1561,14 +1638,20 @@
                         yield child
 
     def __iter__(self):
         children = super(Step, self).__iter__()
         for t in children:
             yield t
 
+    def __getstate__(self):
+        return super(Step, self).__getstate__()
+
+    def __setstate__(self, state):
+        super(Step, self).__setstate__(state)
+
     @property
     def finished_at(self) -> Optional[datetime]:
         """
         Returns the datetime object of when the step finished (successfully or not).
 
         A step is considered finished when all the tasks that belong to it have
         finished. This call will return None if the step has not finished
@@ -1654,24 +1737,31 @@
         """
         return self._filtered_children(*tags)
 
     @property
     def code(self) -> Optional[MetaflowCode]:
         """
         Returns the MetaflowCode object for this run, if present.
-
-        Not all runs save their code so this call may return None in those cases.
+        Code is packed if atleast one `Step` runs remotely, else None is returned.
 
         Returns
         -------
         MetaflowCode, optional
             Code package for this run
         """
-        if "start" in self:
-            return self["start"].task.code
+        # Note that this can be quite slow in the edge-case where the codepackage is only available
+        # for the last step on the list. Steps are reverse-ordered, so the worst-case scenario is
+        # if the start step executes remotely and every step after that is remote.
+        #
+        # TODO: A more optimized way of figuring out if a run has remote steps (and thus a codepackage) available.
+        # This might require changes to the metadata-service as well.
+        for step in self:
+            code = step.task.code
+            if code:
+                return code
 
     @property
     def data(self) -> Optional[MetaflowData]:
         """
         Returns a container of data artifacts produced by this run.
 
         You can access data produced by this run as follows:
@@ -1874,14 +1964,38 @@
         final_user_tags = self._metaflow.metadata.mutate_user_tags_for_run(
             flow_id, self.id, tags_to_remove=tags_to_remove, tags_to_add=tags_to_add
         )
         # refresh Run object with the latest tags
         self._user_tags = frozenset(final_user_tags)
         self._tags = frozenset([*self._user_tags, *self._system_tags])
 
+    def __getstate__(self):
+        return super(Run, self).__getstate__()
+
+    def __setstate__(self, state):
+        super(Run, self).__setstate__(state)
+
+    @property
+    def trigger(self) -> Optional[Trigger]:
+        """
+        Returns a container of events that triggered this run.
+
+        This returns None if the run was not triggered by any events.
+
+        Returns
+        -------
+        Trigger, optional
+            Container of triggering events
+        """
+        if "start" in self:
+            meta = self["start"].task.metadata_dict.get("execution-triggers")
+            if meta:
+                return Trigger(json.loads(meta))
+        return None
+
 
 class Flow(MetaflowObject):
     """
     A Flow represents all existing flows with a certain name, in other words,
     classes derived from `FlowSpec`. A container of `Run` objects.
 
     Attributes
@@ -1945,14 +2059,20 @@
         Returns
         -------
         Iterable[Run]
             Iterator over `Run` objects in this flow.
         """
         return self._filtered_children(*tags)
 
+    def __getstate__(self):
+        return super(Flow, self).__getstate__()
+
+    def __setstate__(self, state):
+        super(Flow, self).__setstate__(state)
+
 
 class Metaflow(object):
     """
     Entry point to all objects in the Metaflow universe.
 
     This object can be used to list all the flows present either through the explicit property
     or by iterating over this object.
```

### Comparing `metaflow-2.8.3/metaflow/client/filecache.py` & `metaflow-2.8.4/metaflow/client/filecache.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/cmd/configure_cmd.py` & `metaflow-2.8.4/metaflow/cmd/configure_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/cmd/main_cli.py` & `metaflow-2.8.4/metaflow/cmd/main_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/cmd/tutorials_cmd.py` & `metaflow-2.8.4/metaflow/cmd/tutorials_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/cmd_with_io.py` & `metaflow-2.8.4/metaflow/cmd_with_io.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/current.py` & `metaflow-2.8.4/metaflow/current.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 import os
 from typing import Any, Optional
 
 from metaflow.metaflow_config import TEMPDIR
 
 Parallel = namedtuple("Parallel", ["main_ip", "num_nodes", "node_index"])
 
+# Can add this if we are ok with 3.5.2+
+# if typing.TYPE_CHECKING:
+#     from metaflow.client.core import Run, Task
+
 
 class Current(object):
     def __init__(self):
         self._flow_name = None
         self._run_id = None
         self._step_name = None
         self._task_id = None
@@ -79,57 +83,57 @@
         -------
         bool
             True if called inside a run, False otherwise.
         """
         return self._is_running
 
     @property
-    def flow_name(self) -> str:
+    def flow_name(self) -> Optional[str]:
         """
         The name of the currently executing flow.
 
         Returns
         -------
-        str
+        str, optional
             Flow name.
         """
         return self._flow_name
 
     @property
-    def run_id(self) -> str:
+    def run_id(self) -> Optional[str]:
         """
         The run ID of the currently executing run.
 
         Returns
         -------
-        str
+        str, optional
             Run ID.
         """
         return self._run_id
 
     @property
-    def step_name(self) -> str:
+    def step_name(self) -> Optional[str]:
         """
         The name of the currently executing step.
 
         Returns
         -------
-        str
+        str, optional
             Step name.
         """
         return self._step_name
 
     @property
-    def task_id(self) -> str:
+    def task_id(self) -> Optional[str]:
         """
         The task ID of the currently executing task.
 
         Returns
         -------
-        str
+        str, optional
             Task ID.
         """
         return self._task_id
 
     @property
     def retry_count(self) -> int:
         """
@@ -163,40 +167,81 @@
         -------
         str, optional
             Run ID of the original run.
         """
         return self._origin_run_id
 
     @property
-    def pathspec(self) -> str:
+    def pathspec(self) -> Optional[str]:
         """
-        Pathspec of the current run, i.e. a unique
+        Pathspec of the current task, i.e. a unique
         identifier of the current task. The returned
         string follows this format:
         ```
         {flow_name}/{run_id}/{step_name}/{task_id}
         ```
 
+        This is a shorthand to `current.task.pathspec`.
+
         Returns
         -------
-        str
+        str, optional
             Pathspec.
         """
 
         pathspec_components = (
             self._flow_name,
             self._run_id,
             self._step_name,
             self._task_id,
         )
         if any(v is None for v in pathspec_components):
             return None
         return "/".join(pathspec_components)
 
     @property
+    def task(self) -> Optional["Task"]:
+        """
+        Task object of the current task.
+
+        Returns
+        -------
+        Task, optional
+            Current task.
+        """
+        from metaflow import Task  # Prevent circular dependency
+
+        pathspec_components = (
+            self._flow_name,
+            self._run_id,
+            self._step_name,
+            self._task_id,
+        )
+        if any(v is None for v in pathspec_components):
+            return None
+        return Task("/".join(pathspec_components), _namespace_check=False)
+
+    @property
+    def run(self) -> Optional["Run"]:
+        """
+        Run object of the current run.
+
+        Returns
+        -------
+        Run, optional
+            Current run.
+        """
+        from metaflow import Run  # Prevent circular dependency
+
+        pathspec_components = (self._flow_name, self._run_id)
+        if any(v is None for v in pathspec_components):
+            return None
+        return Run("/".join(pathspec_components), _namespace_check=False)
+
+    @property
     def namespace(self) -> str:
         """
         The current namespace.
 
         Returns
         -------
         str
@@ -230,22 +275,22 @@
         [Legacy function - do not use]
 
         Access tags through the Run object instead.
         """
         return self._tags
 
     @property
-    def tempdir(self) -> str:
+    def tempdir(self) -> Optional[str]:
         """
-        Currently configured temp dir.
+        Currently configured temporary directory.
 
         Returns
         -------
-        str
-            temp dir.
+        str, optional
+            Temporary director.
         """
         return self._tempdir
 
 
 # instantiate the Current singleton. This will be populated
 # by task.MetaflowTask before a task is executed.
 current = Current()
```

### Comparing `metaflow-2.8.3/metaflow/datastore/content_addressed_store.py` & `metaflow-2.8.4/metaflow/datastore/content_addressed_store.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/datastore/datastore_set.py` & `metaflow-2.8.4/metaflow/datastore/datastore_set.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/datastore/datastore_storage.py` & `metaflow-2.8.4/metaflow/datastore/datastore_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/datastore/flow_datastore.py` & `metaflow-2.8.4/metaflow/datastore/flow_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/datastore/task_datastore.py` & `metaflow-2.8.4/metaflow/datastore/task_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/debug.py` & `metaflow-2.8.4/metaflow/debug.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/decorators.py` & `metaflow-2.8.4/metaflow/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/event_logger.py` & `metaflow-2.8.4/metaflow/event_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/exception.py` & `metaflow-2.8.4/metaflow/exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,21 @@
     headline = "Object not in the current namespace"
 
     def __init__(self, namespace):
         msg = "Object not in namespace '%s'" % namespace
         super(MetaflowNamespaceMismatch, self).__init__(msg)
 
 
+class MetaflowInvalidPathspec(MetaflowException):
+    headline = "Invalid pathspec"
+
+    def __init__(self, msg):
+        super(MetaflowInvalidPathspec, self).__init__(msg)
+
+
 class MetaflowInternalError(MetaflowException):
     headline = "Internal error"
 
 
 class MetaflowTaggingError(MetaflowException):
     headline = "Tagging error"
```

### Comparing `metaflow-2.8.3/metaflow/extension_support/__init__.py` & `metaflow-2.8.4/metaflow/extension_support/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/extension_support/cmd.py` & `metaflow-2.8.4/metaflow/extension_support/cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/extension_support/integrations.py` & `metaflow-2.8.4/metaflow/extension_support/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/extension_support/plugins.py` & `metaflow-2.8.4/metaflow/extension_support/plugins.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/flowspec.py` & `metaflow-2.8.4/metaflow/flowspec.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/graph.py` & `metaflow-2.8.4/metaflow/graph.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/includefile.py` & `metaflow-2.8.4/metaflow/includefile.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/integrations.py` & `metaflow-2.8.4/metaflow/integrations.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 # these aliases in the toplevel file.
 
 # It follows a similar pattern to plugins so that the these integration aliases can be
 # turned on and off and avoid exposing things that are not necessarily needed/wanted.
 
 from metaflow.extension_support.integrations import process_integration_aliases
 
-# To enable an alias `metaflow.alias.get_s3_client` to
+# To enable an alias `metaflow.integrations.get_s3_client` to
 # `metaflow.plugins.aws.aws_client.get_aws_client`, use the following:
 #
 # ALIASES_DESC = [("get_s3_client", ".plugins.aws.aws_client.get_aws_client")]
 #
 # ALIASES_DESC is a list of tuples:
 #  - name: name of the integration alias
 #  - obj: object it points to
 #
+ALIASES_DESC = [("ArgoEvent", ".plugins.argo.argo_events.ArgoEvent")]
+
 # Aliases can be enabled or disabled through configuration or extensions:
 #  - ENABLED_INTEGRATION_ALIAS: list of alias names to enable.
 #  - TOGGLE_INTEGRATION_ALIAS: if ENABLED_INTEGRATION_ALIAS is not set anywhere
 #    (environment variable, configuration or extensions), list of integration aliases
 #    to toggle (+<name> or <name> enables, -<name> disables) to build
 #    ENABLED_INTEGRATION_ALIAS from the concatenation of the names in
 #    ALIASES_DESC (concatenation of the names here as well as in the extensions).
```

### Comparing `metaflow-2.8.3/metaflow/lint.py` & `metaflow-2.8.4/metaflow/lint.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/metadata/heartbeat.py` & `metaflow-2.8.4/metaflow/metadata/heartbeat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/metadata/metadata.py` & `metaflow-2.8.4/metaflow/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/metadata/util.py` & `metaflow-2.8.4/metaflow/metadata/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/metaflow_config.py` & `metaflow-2.8.4/metaflow/metaflow_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -282,14 +282,24 @@
 # Toggle for trying to fetch EC2 instance metadata
 KUBERNETES_FETCH_EC2_METADATA = from_conf("KUBERNETES_FETCH_EC2_METADATA", False)
 
 ARGO_WORKFLOWS_KUBERNETES_SECRETS = from_conf("ARGO_WORKFLOWS_KUBERNETES_SECRETS", "")
 ARGO_WORKFLOWS_ENV_VARS_TO_SKIP = from_conf("ARGO_WORKFLOWS_ENV_VARS_TO_SKIP", "")
 
 ##
+# Argo Events Configuration
+##
+ARGO_EVENTS_SERVICE_ACCOUNT = from_conf("ARGO_EVENTS_SERVICE_ACCOUNT")
+ARGO_EVENTS_EVENT_BUS = from_conf("ARGO_EVENTS_EVENT_BUS", "default")
+ARGO_EVENTS_EVENT_SOURCE = from_conf("ARGO_EVENTS_EVENT_SOURCE")
+ARGO_EVENTS_EVENT = from_conf("ARGO_EVENTS_EVENT")
+ARGO_EVENTS_WEBHOOK_URL = from_conf("ARGO_EVENTS_WEBHOOK_URL")
+
+
+##
 # Airflow Configuration
 ##
 # This configuration sets `startup_timeout_seconds` in airflow's KubernetesPodOperator.
 AIRFLOW_KUBERNETES_STARTUP_TIMEOUT_SECONDS = from_conf(
     "AIRFLOW_KUBERNETES_STARTUP_TIMEOUT_SECONDS", 60 * 60
 )
 # This configuration sets `kubernetes_conn_id` in airflow's KubernetesPodOperator.
```

### Comparing `metaflow-2.8.3/metaflow/metaflow_config_funcs.py` & `metaflow-2.8.4/metaflow/metaflow_config_funcs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/metaflow_environment.py` & `metaflow-2.8.4/metaflow/metaflow_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/metaflow_version.py` & `metaflow-2.8.4/metaflow/metaflow_version.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/mflog/__init__.py` & `metaflow-2.8.4/metaflow/mflog/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/mflog/mflog.py` & `metaflow-2.8.4/metaflow/mflog/mflog.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/mflog/save_logs.py` & `metaflow-2.8.4/metaflow/mflog/save_logs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/mflog/save_logs_periodically.py` & `metaflow-2.8.4/metaflow/mflog/save_logs_periodically.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/mflog/tee.py` & `metaflow-2.8.4/metaflow/mflog/tee.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/monitor.py` & `metaflow-2.8.4/metaflow/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,15 @@
     @property
     def value(self):
         return self._value
 
     def serialize(self):
         parent_ser = super(Gauge, self).serialize()
         parent_ser["_value"] = self._value
+        return parent_ser
 
     @classmethod
     def deserialize(cls, metric_name, value):
         g = Gauge(metric_name)
         g.set_value(value.get("_value", 0))
         return g
```

### Comparing `metaflow-2.8.3/metaflow/multicore_utils.py` & `metaflow-2.8.4/metaflow/multicore_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/package.py` & `metaflow-2.8.4/metaflow/package.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/parameters.py` & `metaflow-2.8.4/metaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/__init__.py` & `metaflow-2.8.4/metaflow/plugins/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from metaflow.extension_support.plugins import (
-    process_plugins,
     merge_lists,
+    process_plugins,
     resolve_plugins,
 )
 
 # Add new CLI commands here
 CLIS_DESC = [
     ("package", ".package_cli.cli"),
     ("batch", ".aws.batch.batch_cli.cli"),
@@ -52,14 +52,16 @@
 # Add an entry here if you need a new flow-level annotation. Be
 # careful with the choice of name though - they become top-level
 # imports from the metaflow package.
 FLOW_DECORATORS_DESC = [
     ("conda_base", ".conda.conda_flow_decorator.CondaFlowDecorator"),
     ("schedule", ".aws.step_functions.schedule_decorator.ScheduleDecorator"),
     ("project", ".project_decorator.ProjectDecorator"),
+    ("trigger", ".events_decorator.TriggerDecorator"),
+    ("trigger_on_finish", ".events_decorator.TriggerOnFinishDecorator"),
 ]
 
 # Add environments here
 ENVIRONMENTS_DESC = [("conda", ".conda.conda_environment.CondaEnvironment")]
 
 # Add metadata providers here
 METADATA_PROVIDERS_DESC = [
@@ -133,36 +135,37 @@
 
 SIDECARS.update(LOGGING_SIDECARS)
 SIDECARS.update(MONITOR_SIDECARS)
 
 AWS_CLIENT_PROVIDERS = resolve_plugins("aws_client_provider")
 SECRETS_PROVIDERS = resolve_plugins("secrets_provider")
 
+from .cards.card_modules import MF_EXTERNAL_CARDS
+
 # Cards; due to the way cards were designed, it is harder to make them fit
 # in the resolve_plugins mechanism. This should be OK because it is unlikely that
 # cards will need to be *removed*. No card should be too specific (for example, no
 # card should be something just for Airflow, or Argo or step-functions -- those should
 # be added externally).
 from .cards.card_modules.basic import (
-    DefaultCard,
-    TaskSpecCard,
-    ErrorCard,
     BlankCard,
+    DefaultCard,
     DefaultCardJSON,
+    ErrorCard,
+    TaskSpecCard,
 )
 from .cards.card_modules.test_cards import (
-    TestErrorCard,
-    TestTimeoutCard,
-    TestMockCard,
-    TestPathSpecCard,
     TestEditableCard,
     TestEditableCard2,
+    TestErrorCard,
+    TestMockCard,
     TestNonEditableCard,
+    TestPathSpecCard,
+    TestTimeoutCard,
 )
-from .cards.card_modules import MF_EXTERNAL_CARDS
 
 CARDS = [
     DefaultCard,
     TaskSpecCard,
     ErrorCard,
     BlankCard,
     TestErrorCard,
```

### Comparing `metaflow-2.8.3/metaflow/plugins/airflow/airflow.py` & `metaflow-2.8.4/metaflow/plugins/airflow/airflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,58 +1,57 @@
-from io import BytesIO
 import json
 import os
 import random
 import string
 import sys
 from datetime import datetime, timedelta
-from metaflow.includefile import FilePathClass
+from io import BytesIO
 
 import metaflow.util as util
+from metaflow import current
 from metaflow.decorators import flow_decorators
 from metaflow.exception import MetaflowException
+from metaflow.includefile import FilePathClass
 from metaflow.metaflow_config import (
-    SERVICE_HEADERS,
-    SERVICE_INTERNAL_URL,
-    CARD_S3ROOT,
-    DATASTORE_SYSROOT_S3,
-    DATATOOLS_S3ROOT,
-    KUBERNETES_SERVICE_ACCOUNT,
-    KUBERNETES_SECRETS,
-    AIRFLOW_KUBERNETES_STARTUP_TIMEOUT_SECONDS,
-    AZURE_STORAGE_BLOB_SERVICE_ENDPOINT,
-    DATASTORE_SYSROOT_AZURE,
-    CARD_AZUREROOT,
     AIRFLOW_KUBERNETES_CONN_ID,
     AIRFLOW_KUBERNETES_KUBECONFIG_CONTEXT,
     AIRFLOW_KUBERNETES_KUBECONFIG_FILE,
-    DATASTORE_SYSROOT_GS,
+    AIRFLOW_KUBERNETES_STARTUP_TIMEOUT_SECONDS,
+    AWS_SECRETS_MANAGER_DEFAULT_REGION,
+    AZURE_STORAGE_BLOB_SERVICE_ENDPOINT,
+    CARD_AZUREROOT,
     CARD_GSROOT,
+    CARD_S3ROOT,
+    DATASTORE_SYSROOT_AZURE,
+    DATASTORE_SYSROOT_GS,
+    DATASTORE_SYSROOT_S3,
+    DATATOOLS_S3ROOT,
     DEFAULT_SECRETS_BACKEND_TYPE,
-    AWS_SECRETS_MANAGER_DEFAULT_REGION,
+    KUBERNETES_SECRETS,
+    KUBERNETES_SERVICE_ACCOUNT,
+    S3_ENDPOINT_URL,
+    SERVICE_HEADERS,
+    SERVICE_INTERNAL_URL,
+)
+from metaflow.parameters import (
+    DelayedEvaluationParameter,
+    JSONTypeClass,
+    deploy_time_eval,
 )
-from metaflow.parameters import DelayedEvaluationParameter, deploy_time_eval
-from metaflow.plugins.kubernetes.kubernetes import Kubernetes
 
 # TODO: Move chevron to _vendor
 from metaflow.plugins.cards.card_modules import chevron
+from metaflow.plugins.kubernetes.kubernetes import Kubernetes
 from metaflow.plugins.timeout_decorator import get_run_time_limit_for_task
-from metaflow.util import dict_to_cli_options, get_username, compress_list
-from metaflow.parameters import JSONTypeClass
+from metaflow.util import compress_list, dict_to_cli_options, get_username
 
 from . import airflow_utils
+from .airflow_utils import AIRFLOW_MACROS, TASK_ID_XCOM_KEY, AirflowTask, Workflow
 from .exception import AirflowException
 from .sensors import SUPPORTED_SENSORS
-from .airflow_utils import (
-    TASK_ID_XCOM_KEY,
-    AirflowTask,
-    Workflow,
-    AIRFLOW_MACROS,
-)
-from metaflow import current
 
 AIRFLOW_DEPLOY_TEMPLATE_FILE = os.path.join(os.path.dirname(__file__), "dag.py")
 
 
 class Airflow(object):
     TOKEN_STORAGE_ROOT = "mf.airflow"
 
@@ -379,14 +378,15 @@
             "METAFLOW_AIRFLOW_DAG_RUN_ID": AIRFLOW_MACROS.AIRFLOW_RUN_ID,
             "METAFLOW_AIRFLOW_JOB_ID": AIRFLOW_MACROS.AIRFLOW_JOB_ID,
             "METAFLOW_PRODUCTION_TOKEN": self.production_token,
             "METAFLOW_ATTEMPT_NUMBER": AIRFLOW_MACROS.ATTEMPT,
             # GCP stuff
             "METAFLOW_DATASTORE_SYSROOT_GS": DATASTORE_SYSROOT_GS,
             "METAFLOW_CARD_GSROOT": CARD_GSROOT,
+            "METAFLOW_S3_ENDPOINT_URL": S3_ENDPOINT_URL,
         }
         env[
             "METAFLOW_AZURE_STORAGE_BLOB_SERVICE_ENDPOINT"
         ] = AZURE_STORAGE_BLOB_SERVICE_ENDPOINT
         env["METAFLOW_DATASTORE_SYSROOT_AZURE"] = DATASTORE_SYSROOT_AZURE
         env["METAFLOW_CARD_AZUREROOT"] = CARD_AZUREROOT
         if DEFAULT_SECRETS_BACKEND_TYPE:
@@ -621,16 +621,39 @@
     def _contains_foreach(self):
         for node in self.graph:
             if node.type == "foreach":
                 return True
         return False
 
     def compile(self):
+        if self.flow._flow_decorators.get("trigger") or self.flow._flow_decorators.get(
+            "trigger_on_finish"
+        ):
+            raise AirflowException(
+                "Deploying flows with @trigger or @trigger_on_finish decorator(s) "
+                "to Airflow is not supported currently."
+            )
+
         # Visit every node of the flow and recursively build the state machine.
         def _visit(node, workflow, exit_node=None):
+            kube_deco = dict(
+                [deco for deco in node.decorators if deco.name == "kubernetes"][
+                    0
+                ].attributes
+            )
+            if kube_deco:
+                # Only guard against use_tmpfs and tmpfs_size as these determine if tmpfs is enabled.
+                for attr in ["use_tmpfs", "tmpfs_size"]:
+                    if kube_deco[attr]:
+                        raise AirflowException(
+                            "tmpfs attribute *%s* is currently not supported on Airflow "
+                            "for the @kubernetes decorator on step *%s*"
+                            % (attr, node.name)
+                        )
+
             parent_is_foreach = any(  # Any immediate parent is a foreach node.
                 self.graph[n].type == "foreach" for n in node.in_funcs
             )
             state = AirflowTask(
                 node.name, is_mapper_node=parent_is_foreach
             ).set_operator_args(**self._to_job(node))
             if node.type == "end":
```

### Comparing `metaflow-2.8.3/metaflow/plugins/airflow/airflow_cli.py` & `metaflow-2.8.4/metaflow/plugins/airflow/airflow_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
+import base64
 import os
 import re
 import sys
-import base64
+from hashlib import sha1
+
 from metaflow import current, decorators
 from metaflow._vendor import click
 from metaflow.exception import MetaflowException, MetaflowInternalError
 from metaflow.package import MetaflowPackage
-from hashlib import sha1
-from metaflow.plugins.kubernetes.kubernetes_decorator import KubernetesDecorator
-from metaflow.util import get_username, to_bytes, to_unicode
-
-from .airflow import Airflow
-from .exception import AirflowException, NotSupportedException
-
 from metaflow.plugins.aws.step_functions.production_token import (
     load_token,
     new_token,
     store_token,
 )
+from metaflow.plugins.kubernetes.kubernetes_decorator import KubernetesDecorator
+from metaflow.util import get_username, to_bytes, to_unicode
+
+from .airflow import Airflow
+from .exception import AirflowException, NotSupportedException
 
 
 class IncorrectProductionToken(MetaflowException):
     headline = "Incorrect production token"
 
 
 VALID_NAME = re.compile("[^a-zA-Z0-9_\-\.]")
@@ -368,17 +368,17 @@
                 "Parameter *%s* is specified twice. "
                 "Note that parameter names are "
                 "case-insensitive." % param.name
             )
         seen.add(norm)
         if "default" not in param.kwargs:
             raise MetaflowException(
-                "Parameter *%s* does not have a "
-                "default value. "
+                "Parameter *%s* does not have a default value. "
                 "A default value is required for parameters when deploying flows on Airflow."
+                % param.name
             )
     # check for other compute related decorators.
     _validate_foreach_constraints(graph)
     for node in graph:
         if node.parallel_foreach:
             raise AirflowException(
                 "Deploying flows with @parallel decorator(s) "
```

### Comparing `metaflow-2.8.3/metaflow/plugins/airflow/airflow_decorator.py` & `metaflow-2.8.4/metaflow/plugins/airflow/airflow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/airflow/airflow_utils.py` & `metaflow-2.8.4/metaflow/plugins/airflow/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/airflow/plumbing/set_parameters.py` & `metaflow-2.8.4/metaflow/plugins/airflow/plumbing/set_parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/airflow/sensors/base_sensor.py` & `metaflow-2.8.4/metaflow/plugins/airflow/sensors/base_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/airflow/sensors/external_task_sensor.py` & `metaflow-2.8.4/metaflow/plugins/airflow/sensors/external_task_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/airflow/sensors/s3_sensor.py` & `metaflow-2.8.4/metaflow/plugins/airflow/sensors/s3_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/argo/argo_client.py` & `metaflow-2.8.4/metaflow/plugins/argo/argo_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,22 +8,21 @@
 
 class ArgoClientException(MetaflowException):
     headline = "Argo Client error"
 
 
 class ArgoClient(object):
     def __init__(self, namespace=None):
-
-        self._kubernetes_client = KubernetesClient()
+        self._client = KubernetesClient()
         self._namespace = namespace or "default"
         self._group = "argoproj.io"
         self._version = "v1alpha1"
 
     def get_workflow_template(self, name):
-        client = self._kubernetes_client.get()
+        client = self._client.get()
         try:
             return client.CustomObjectsApi().get_namespaced_custom_object(
                 group=self._group,
                 version=self._version,
                 namespace=self._namespace,
                 plural="workflowtemplates",
                 name=name,
@@ -34,15 +33,15 @@
             raise ArgoClientException(
                 json.loads(e.body)["message"] if e.body is not None else e.reason
             )
 
     def register_workflow_template(self, name, workflow_template):
         # Unfortunately, Kubernetes client does not handle optimistic
         # concurrency control by itself unlike kubectl
-        client = self._kubernetes_client.get()
+        client = self._client.get()
         try:
             workflow_template["metadata"][
                 "resourceVersion"
             ] = client.CustomObjectsApi().get_namespaced_custom_object(
                 group=self._group,
                 version=self._version,
                 namespace=self._namespace,
@@ -84,15 +83,15 @@
             )
         except client.rest.ApiException as e:
             raise ArgoClientException(
                 json.loads(e.body)["message"] if e.body is not None else e.reason
             )
 
     def trigger_workflow_template(self, name, parameters={}):
-        client = self._kubernetes_client.get()
+        client = self._client.get()
         body = {
             "apiVersion": "argoproj.io/v1alpha1",
             "kind": "Workflow",
             "metadata": {"generateName": name + "-"},
             "spec": {
                 "workflowTemplateRef": {"name": name},
                 "arguments": {
@@ -115,15 +114,15 @@
             raise ArgoClientException(
                 json.loads(e.body)["message"] if e.body is not None else e.reason
             )
 
     def schedule_workflow_template(self, name, schedule=None, timezone=None):
         # Unfortunately, Kubernetes client does not handle optimistic
         # concurrency control by itself unlike kubectl
-        client = self._kubernetes_client.get()
+        client = self._client.get()
         body = {
             "apiVersion": "argoproj.io/v1alpha1",
             "kind": "CronWorkflow",
             "metadata": {"name": name},
             "spec": {
                 "suspend": schedule is None,
                 "schedule": schedule,
@@ -177,7 +176,81 @@
                 body=body,
                 name=name,
             )
         except client.rest.ApiException as e:
             raise ArgoClientException(
                 json.loads(e.body)["message"] if e.body is not None else e.reason
             )
+
+    def register_sensor(self, name, sensor=None):
+        if sensor is None:
+            sensor = {}
+        # Unfortunately, Kubernetes client does not handle optimistic
+        # concurrency control by itself unlike kubectl
+        client = self._client.get()
+        if not sensor:
+            sensor["metadata"] = {}
+
+        try:
+            sensor["metadata"][
+                "resourceVersion"
+            ] = client.CustomObjectsApi().get_namespaced_custom_object(
+                group=self._group,
+                version=self._version,
+                namespace=self._namespace,
+                plural="sensors",
+                name=name,
+            )[
+                "metadata"
+            ][
+                "resourceVersion"
+            ]
+        except client.rest.ApiException as e:
+            # Sensor does not exist and we want to add one
+            if e.status == 404:
+                if sensor.get("kind") is None:
+                    return
+                try:
+                    return client.CustomObjectsApi().create_namespaced_custom_object(
+                        group=self._group,
+                        version=self._version,
+                        namespace=self._namespace,
+                        plural="sensors",
+                        body=sensor,
+                    )
+                except client.rest.ApiException as e:
+                    raise ArgoClientException(
+                        json.loads(e.body)["message"]
+                        if e.body is not None
+                        else e.reason
+                    )
+            else:
+                raise ArgoClientException(
+                    json.loads(e.body)["message"] if e.body is not None else e.reason
+                )
+        # Since sensors occupy real resources, delete existing sensor if needed
+        if sensor.get("kind") is None:
+            try:
+                return client.CustomObjectsApi().delete_namespaced_custom_object(
+                    group=self._group,
+                    version=self._version,
+                    namespace=self._namespace,
+                    plural="sensors",
+                    name=name,
+                )
+            except client.rest.ApiException as e:
+                raise ArgoClientException(
+                    json.loads(e.body)["message"] if e.body is not None else e.reason
+                )
+        try:
+            return client.CustomObjectsApi().replace_namespaced_custom_object(
+                group=self._group,
+                version=self._version,
+                namespace=self._namespace,
+                plural="sensors",
+                body=sensor,
+                name=name,
+            )
+        except client.rest.ApiException as e:
+            raise ArgoClientException(
+                json.loads(e.body)["message"] if e.body is not None else e.reason
+            )
```

### Comparing `metaflow-2.8.3/metaflow/plugins/argo/argo_workflows.py` & `metaflow-2.8.4/metaflow/plugins/datatools/s3/s3.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1428 +1,1695 @@
 import json
 import os
-import shlex
+import re
 import sys
-from collections import defaultdict
+import time
+import shutil
+import random
+import subprocess
+from io import RawIOBase, BufferedIOBase
+from itertools import chain, starmap
+from tempfile import mkdtemp, NamedTemporaryFile
+from typing import Dict, Iterable, List, Optional, Tuple, Union, TYPE_CHECKING
 
-from metaflow import current
-from metaflow.decorators import flow_decorators
-from metaflow.exception import MetaflowException
+from metaflow import FlowSpec
+from metaflow.current import current
 from metaflow.metaflow_config import (
-    SERVICE_HEADERS,
-    SERVICE_INTERNAL_URL,
-    CARD_S3ROOT,
-    DATASTORE_SYSROOT_S3,
     DATATOOLS_S3ROOT,
-    DEFAULT_METADATA,
-    KUBERNETES_NAMESPACE,
-    KUBERNETES_NODE_SELECTOR,
-    KUBERNETES_SANDBOX_INIT_SCRIPT,
-    KUBERNETES_SECRETS,
-    KUBERNETES_FETCH_EC2_METADATA,
-    S3_ENDPOINT_URL,
-    AZURE_STORAGE_BLOB_SERVICE_ENDPOINT,
-    DATASTORE_SYSROOT_AZURE,
-    DATASTORE_SYSROOT_GS,
-    CARD_AZUREROOT,
-    CARD_GSROOT,
-    DEFAULT_SECRETS_BACKEND_TYPE,
-    AWS_SECRETS_MANAGER_DEFAULT_REGION,
-    ARGO_WORKFLOWS_KUBERNETES_SECRETS,
-    ARGO_WORKFLOWS_ENV_VARS_TO_SKIP,
+    S3_RETRY_COUNT,
+    S3_TRANSIENT_RETRY_COUNT,
+    TEMPDIR,
+)
+from metaflow.util import (
+    namedtuple_with_defaults,
+    is_stringish,
+    to_bytes,
+    to_unicode,
+    to_fileobj,
+    url_quote,
+    url_unquote,
 )
-from metaflow.mflog import BASH_SAVE_LOGS, bash_capture_logs, export_mflog_env_vars
-from metaflow.parameters import deploy_time_eval
-from metaflow.util import compress_list, dict_to_cli_options, to_camelcase
+from metaflow.exception import MetaflowException
+from metaflow.debug import debug
 
-from .argo_client import ArgoClient
+try:
+    # python2
+    from urlparse import urlparse
+except:
+    # python3
+    from urllib.parse import urlparse
+
+from .s3util import (
+    get_s3_client,
+    read_in_chunks,
+    get_timestamp,
+    TRANSIENT_RETRY_START_LINE,
+    TRANSIENT_RETRY_LINE_CONTENT,
+)
 
+if TYPE_CHECKING:
+    from metaflow.client import Run
 
-class ArgoWorkflowsException(MetaflowException):
-    headline = "Argo Workflows error"
+try:
+    import boto3
+    from boto3.s3.transfer import TransferConfig
+
+    DOWNLOAD_FILE_THRESHOLD = 2 * TransferConfig().multipart_threshold
+    DOWNLOAD_MAX_CHUNK = 2 * 1024 * 1024 * 1024 - 1
+    boto_found = True
+except:
+    boto_found = False
 
 
-class ArgoWorkflowsSchedulingException(MetaflowException):
-    headline = "Argo Workflows scheduling error"
+TEST_INJECT_RETRYABLE_FAILURES = int(
+    os.environ.get("METAFLOW_S3_TEST_RETRYABLE_FAILURES", 0)
+)
 
 
-# List of future enhancements -
-#     1. Configure Argo metrics.
-#     2. Support Argo Events.
-#     3. Support resuming failed workflows within Argo Workflows.
-#     4. Support gang-scheduled clusters for distributed PyTorch/TF - One option is to
-#        use volcano - https://github.com/volcano-sh/volcano/tree/master/example/integrations/argo
-#     5. Support GitOps workflows.
-#     6. Add Metaflow tags to labels/annotations.
-#     7. Support Multi-cluster scheduling - https://github.com/argoproj/argo-workflows/issues/3523#issuecomment-792307297
-#     8. Support for workflow notifications.
-#     9. Support R lang.
-#     10.Ping @savin at slack.outerbounds.co for any feature request.
+def ensure_unicode(x):
+    return None if x is None else to_unicode(x)
 
 
-class ArgoWorkflows(object):
-    def __init__(
-        self,
-        name,
-        graph,
-        flow,
-        code_package_sha,
-        code_package_url,
-        production_token,
-        metadata,
-        flow_datastore,
-        environment,
-        event_logger,
-        monitor,
-        tags=None,
-        namespace=None,
-        username=None,
-        max_workers=None,
-        workflow_timeout=None,
-        workflow_priority=None,
-    ):
-        # Some high-level notes -
-        #
-        # Fail-fast behavior for Argo Workflows - Argo stops
-        # scheduling new steps as soon as it detects that one of the DAG nodes
-        # has failed. After waiting for all the scheduled DAG nodes to run till
-        # completion, Argo with fail the DAG. This implies that after a node
-        # has failed, it may be awhile before the entire DAG is marked as
-        # failed. There is nothing Metaflow can do here for failing even
-        # faster (as of Argo 3.2).
-        #
-        # argo stop` vs `argo terminate` - since we don't currently
-        # rely on any exit handlers, it's safe to either stop or terminate any running
-        # argo workflow deployed through Metaflow. This may not hold true, once we
-        # integrate with Argo Events.
-        #
-        # Currently, an Argo Workflow can only execute entirely within a single
-        # Kubernetes namespace. Multi-cluster / Multi-namespace execution is on the
-        # deck for v3.4 release for Argo Workflows; beyond which point, we will be
-        # able to support them natively.
-        #
-        # Since this implementation generates numerous templates on the fly, please
-        # ensure that your Argo Workflows controller doesn't restrict
-        # templateReferencing.
-
-        self.name = name
-        self.graph = graph
-        self.flow = flow
-        self.code_package_sha = code_package_sha
-        self.code_package_url = code_package_url
-        self.production_token = production_token
-        self.metadata = metadata
-        self.flow_datastore = flow_datastore
-        self.environment = environment
-        self.event_logger = event_logger
-        self.monitor = monitor
-        self.tags = tags
-        self.namespace = namespace
-        self.username = username
-        self.max_workers = max_workers
-        self.workflow_timeout = workflow_timeout
-        self.workflow_priority = workflow_priority
-
-        self.parameters = self._process_parameters()
-        self._workflow_template = self._compile()
-        self._cron = self._get_cron()
+PutValue = Union[RawIOBase, BufferedIOBase, str, bytes]
 
-    def __str__(self):
-        return str(self._workflow_template)
+S3GetObject = namedtuple_with_defaults(
+    "S3GetObject", [("key", str), ("offset", int), ("length", int)]
+)
+S3GetObject.__module__ = __name__
 
-    def deploy(self):
-        try:
-            ArgoClient(namespace=KUBERNETES_NAMESPACE).register_workflow_template(
-                self.name, self._workflow_template.to_json()
-            )
-        except Exception as e:
-            raise ArgoWorkflowsException(str(e))
+S3PutObject = namedtuple_with_defaults(
+    "S3PutObject",
+    [
+        ("key", str),
+        ("value", Optional[PutValue]),
+        ("path", Optional[str]),
+        ("content_type", Optional[str]),
+        ("metadata", Optional[Dict[str, str]]),
+    ],
+    defaults=(None, None, None, None),
+)
+S3PutObject.__module__ = __name__
 
-    @staticmethod
-    def _sanitize(name):
-        # Metaflow allows underscores in node names, which are disallowed in Argo
-        # Workflow template names - so we swap them with hyphens which are not
-        # allowed by Metaflow - guaranteeing uniqueness.
-        return name.replace("_", "-")
+RangeInfo = namedtuple_with_defaults(
+    "RangeInfo",
+    [("total_size", int), ("request_offset", int), ("request_length", int)],
+    defaults=(0, -1),
+)
+RangeInfo.__module__ = __name__
 
-    @classmethod
-    def trigger(cls, name, parameters=None):
-        if parameters is None:
-            parameters = {}
-        try:
-            workflow_template = ArgoClient(
-                namespace=KUBERNETES_NAMESPACE
-            ).get_workflow_template(name)
-        except Exception as e:
-            raise ArgoWorkflowsException(str(e))
-        if workflow_template is None:
-            raise ArgoWorkflowsException(
-                "The workflow *%s* doesn't exist on Argo Workflows in namespace *%s*. "
-                "Please deploy your flow first." % (name, KUBERNETES_NAMESPACE)
-            )
-        else:
-            try:
-                # Check that the workflow was deployed through Metaflow
-                workflow_template["metadata"]["annotations"]["metaflow/owner"]
-            except KeyError as e:
-                raise ArgoWorkflowsException(
-                    "An existing non-metaflow workflow with the same name as "
-                    "*%s* already exists in Argo Workflows. \nPlease modify the "
-                    "name of this flow or delete your existing workflow on Argo "
-                    "Workflows before proceeding." % name
-                )
-        try:
-            return ArgoClient(namespace=KUBERNETES_NAMESPACE).trigger_workflow_template(
-                name, parameters
-            )
-        except Exception as e:
-            raise ArgoWorkflowsException(str(e))
+RANGE_MATCH = re.compile(r"bytes (?P<start>[0-9]+)-(?P<end>[0-9]+)/(?P<total>[0-9]+)")
 
-    def _get_cron(self):
-        schedule = self.flow._flow_decorators.get("schedule")
-        if schedule:
-            # Remove the field "Year" if it exists
-            schedule = schedule[0]
-            return " ".join(schedule.schedule.split()[:5]), schedule.timezone
-        return None
 
-    def schedule(self):
-        try:
-            if self._cron is None:
-                cron, timezone = None, None
-            else:
-                cron, timezone = self._cron
-            ArgoClient(namespace=KUBERNETES_NAMESPACE).schedule_workflow_template(
-                self.name, cron, timezone
-            )
-        except Exception as e:
-            raise ArgoWorkflowsSchedulingException(str(e))
+class MetaflowS3InvalidObject(MetaflowException):
+    headline = "Not a string-like object"
 
-    def trigger_explanation(self):
-        if self._cron:
-            return (
-                "This workflow triggers automatically via the CronWorkflow *%s*."
-                % self.name
-            )
-        else:
-            return "No triggers defined. You need to launch this workflow manually."
 
-    @classmethod
-    def get_existing_deployment(cls, name):
-        workflow_template = ArgoClient(
-            namespace=KUBERNETES_NAMESPACE
-        ).get_workflow_template(name)
-        if workflow_template is not None:
-            try:
-                return (
-                    workflow_template["metadata"]["annotations"]["metaflow/owner"],
-                    workflow_template["metadata"]["annotations"][
-                        "metaflow/production_token"
-                    ],
-                )
-            except KeyError as e:
-                raise ArgoWorkflowsException(
-                    "An existing non-metaflow workflow with the same name as "
-                    "*%s* already exists in Argo Workflows. \nPlease modify the "
-                    "name of this flow or delete your existing workflow on Argo "
-                    "Workflows before proceeding." % name
-                )
-        return None
+class MetaflowS3URLException(MetaflowException):
+    headline = "Invalid address"
 
-    def _process_parameters(self):
-        parameters = []
-        has_schedule = self._get_cron() is not None
-        seen = set()
-        for var, param in self.flow._get_parameters():
-            # Throw an exception if the parameter is specified twice.
-            norm = param.name.lower()
-            if norm in seen:
-                raise MetaflowException(
-                    "Parameter *%s* is specified twice. "
-                    "Note that parameter names are "
-                    "case-insensitive." % param.name
-                )
-            seen.add(norm)
 
-            is_required = param.kwargs.get("required", False)
-            # Throw an exception if a schedule is set for a flow with required
-            # parameters with no defaults. We currently don't have any notion
-            # of data triggers in Argo Workflows.
-
-            # TODO: Support Argo Events for data triggering in the near future.
-            if "default" not in param.kwargs and is_required and has_schedule:
-                raise MetaflowException(
-                    "The parameter *%s* does not have a default and is required. "
-                    "Scheduling such parameters via Argo CronWorkflows is not "
-                    "currently supported." % param.name
-                )
-            value = deploy_time_eval(param.kwargs.get("default"))
-            # If the value is not required and the value is None, we set the value to
-            # the JSON equivalent of None to please argo-workflows.
-            if not is_required or value is not None:
-                value = json.dumps(value)
-            parameters.append(
-                dict(name=param.name, value=value, description=param.kwargs.get("help"))
-            )
-        return parameters
+class MetaflowS3Exception(MetaflowException):
+    headline = "S3 access failed"
 
-    def _compile(self):
-        # This method compiles a Metaflow FlowSpec into Argo WorkflowTemplate
-        #
-        # WorkflowTemplate
-        #   |
-        #    -- WorkflowSpec
-        #         |
-        #          -- Array<Template>
-        #                     |
-        #                      -- DAGTemplate, ContainerTemplate
-        #                           |                  |
-        #                            -- Array<DAGTask> |
-        #                                       |      |
-        #                                        -- Template
-        #
-        # Steps in FlowSpec are represented as DAGTasks.
-        # A DAGTask can reference to -
-        #     a ContainerTemplate (for linear steps..) or
-        #     another DAGTemplate (for nested `foreach`s).
-        #
-        # While we could have very well inlined container templates inside a DAGTask,
-        # unfortunately Argo variable substitution ({{pod.name}}) doesn't work as
-        # expected within DAGTasks
-        # (https://github.com/argoproj/argo-workflows/issues/7432) and we are forced to
-        # generate container templates at the top level (in WorkflowSpec) and maintain
-        # references to them within the DAGTask.
-
-        labels = {"app.kubernetes.io/part-of": "metaflow"}
-
-        annotations = {
-            "metaflow/production_token": self.production_token,
-            "metaflow/owner": self.username,
-            "metaflow/user": "argo-workflows",
-            "metaflow/flow_name": self.flow.name,
-        }
-        if current.get("project_name"):
-            annotations.update(
-                {
-                    "metaflow/project_name": current.project_name,
-                    "metaflow/branch_name": current.branch_name,
-                    "metaflow/project_flow_name": current.project_flow_name,
-                }
-            )
-
-        return (
-            WorkflowTemplate()
-            .metadata(
-                # Workflow Template metadata.
-                ObjectMeta()
-                .name(self.name)
-                # Argo currently only supports Workflow-level namespaces. When v3.4.0
-                # is released, we should be able to support multi-namespace /
-                # multi-cluster scheduling.
-                .namespace(KUBERNETES_NAMESPACE)
-                .label("app.kubernetes.io/name", "metaflow-flow")
-                .label("app.kubernetes.io/part-of", "metaflow")
-                .annotations(annotations)
-            )
-            .spec(
-                WorkflowSpec()
-                # Set overall workflow timeout.
-                .active_deadline_seconds(self.workflow_timeout)
-                # TODO: Allow Argo to optionally archive all workflow execution logs
-                #       It's disabled for now since it requires all Argo installations
-                #       to enable an artifactory repository. If log archival is
-                #       enabled in workflow controller, the logs for this workflow will
-                #       automatically get archived.
-                # .archive_logs()
-                # Don't automount service tokens for now - https://github.com/kubernetes/kubernetes/issues/16779#issuecomment-159656641
-                # TODO: Service account names are currently set in the templates. We
-                #       can specify the default service account name here to reduce
-                #       the size of the generated YAML by a tiny bit.
-                # .automount_service_account_token()
-                # TODO: Support ImagePullSecrets for Argo & Kubernetes
-                # .image_pull_secrets(...)
-                # Limit workflow parallelism
-                .parallelism(self.max_workers)
-                # TODO: Support Prometheus metrics for Argo
-                # .metrics(...)
-                # TODO: Support PodGC and DisruptionBudgets
-                .priority(self.workflow_priority)
-                # Set workflow metadata
-                .workflow_metadata(
-                    Metadata()
-                    .label("app.kubernetes.io/name", "metaflow-run")
-                    .label("app.kubernetes.io/part-of", "metaflow")
-                    .annotations(
-                        {**annotations, **{"metaflow/run_id": "argo-{{workflow.name}}"}}
-                    )
-                    # TODO: Set dynamic labels using labels_from. Ideally, we would
-                    #       want to expose run_id as a label. It's easy to add labels,
-                    #       but very difficult to remove them - let's err on the
-                    #       conservative side and only add labels when we come across
-                    #       use-cases for them.
-                )
-                # Handle parameters
-                .arguments(
-                    Arguments().parameters(
-                        [
-                            Parameter(parameter["name"])
-                            .value(parameter["value"])
-                            .description(parameter.get("description"))
-                            # TODO: Better handle IncludeFile in Argo Workflows UI.
-                            for parameter in self.parameters
-                        ]
-                    )
-                )
-                # Set common pod metadata.
-                .pod_metadata(
-                    Metadata()
-                    .label("app.kubernetes.io/name", "metaflow-task")
-                    .label("app.kubernetes.io/part-of", "metaflow")
-                    .annotations(annotations)
-                )
-                # Set the entrypoint to flow name
-                .entrypoint(self.flow.name)
-                # Top-level DAG template(s)
-                .templates(self._dag_templates())
-                # Container templates
-                .templates(self._container_templates())
-            )
-        )
-
-    # Visit every node and yield the uber DAGTemplate(s).
-    def _dag_templates(self):
-        def _visit(node, exit_node=None, templates=None, dag_tasks=None):
-            # Every for-each node results in a separate subDAG and an equivalent
-            # DAGTemplate rooted at the child of the for-each node. Each DAGTemplate
-            # has a unique name - the top-level DAGTemplate is named as the name of
-            # the flow and the subDAG DAGTemplates are named after the (only) descendant
-            # of the for-each node.
-
-            # Emit if we have reached the end of the sub workflow
-            if dag_tasks is None:
-                dag_tasks = []
-            if templates is None:
-                templates = []
-            if exit_node is not None and exit_node is node.name:
-                return templates, dag_tasks
-
-            if node.name == "start":
-                # Start node has no dependencies.
-                dag_task = DAGTask(self._sanitize(node.name)).template(
-                    self._sanitize(node.name)
-                )
-            elif (
-                node.is_inside_foreach
-                and self.graph[node.in_funcs[0]].type == "foreach"
-            ):
-                # Child of a foreach node needs input-paths as well as split-index
-                # This child is the first node of the sub workflow and has no dependency
-                parameters = [
-                    Parameter("input-paths").value("{{inputs.parameters.input-paths}}"),
-                    Parameter("split-index").value("{{inputs.parameters.split-index}}"),
-                ]
-                dag_task = (
-                    DAGTask(self._sanitize(node.name))
-                    .template(self._sanitize(node.name))
-                    .arguments(Arguments().parameters(parameters))
-                )
-            else:
-                # Every other node needs only input-paths
-                parameters = [
-                    Parameter("input-paths").value(
-                        compress_list(
-                            [
-                                "argo-{{workflow.name}}/%s/{{tasks.%s.outputs.parameters.task-id}}"
-                                % (n, self._sanitize(n))
-                                for n in node.in_funcs
-                            ]
-                        )
-                    )
-                ]
-                dag_task = (
-                    DAGTask(self._sanitize(node.name))
-                    .dependencies(
-                        [self._sanitize(in_func) for in_func in node.in_funcs]
-                    )
-                    .template(self._sanitize(node.name))
-                    .arguments(Arguments().parameters(parameters))
-                )
-            dag_tasks.append(dag_task)
 
-            # End the workflow if we have reached the end of the flow
-            if node.type == "end":
-                return [
-                    Template(self.flow.name).dag(
-                        DAGTemplate().fail_fast().tasks(dag_tasks)
-                    )
-                ] + templates, dag_tasks
-            # For split nodes traverse all the children
-            if node.type == "split":
-                for n in node.out_funcs:
-                    _visit(self.graph[n], node.matching_join, templates, dag_tasks)
-                return _visit(
-                    self.graph[node.matching_join], exit_node, templates, dag_tasks
-                )
-            # For foreach nodes generate a new sub DAGTemplate
-            elif node.type == "foreach":
-                foreach_template_name = self._sanitize(
-                    "%s-foreach-%s"
-                    % (
-                        node.name,
-                        node.foreach_param,
-                    )
-                )
-                foreach_task = (
-                    DAGTask(foreach_template_name)
-                    .dependencies([self._sanitize(node.name)])
-                    .template(foreach_template_name)
-                    .arguments(
-                        Arguments().parameters(
-                            [
-                                Parameter("input-paths").value(
-                                    "argo-{{workflow.name}}/%s/{{tasks.%s.outputs.parameters.task-id}}"
-                                    % (node.name, self._sanitize(node.name))
-                                ),
-                                Parameter("split-index").value("{{item}}"),
-                            ]
-                        )
-                    )
-                    .with_param(
-                        "{{tasks.%s.outputs.parameters.num-splits}}"
-                        % self._sanitize(node.name)
-                    )
-                )
-                dag_tasks.append(foreach_task)
-                templates, dag_tasks_1 = _visit(
-                    self.graph[node.out_funcs[0]], node.matching_join, templates, []
-                )
-                templates.append(
-                    Template(foreach_template_name)
-                    .inputs(
-                        Inputs().parameters(
-                            [Parameter("input-paths"), Parameter("split-index")]
-                        )
-                    )
-                    .outputs(
-                        Outputs().parameters(
-                            [
-                                Parameter("task-id").valueFrom(
-                                    {
-                                        "parameter": "{{tasks.%s.outputs.parameters.task-id}}"
-                                        % self._sanitize(
-                                            self.graph[node.matching_join].in_funcs[0]
-                                        )
-                                    }
-                                )
-                            ]
-                        )
-                    )
-                    .dag(DAGTemplate().fail_fast().tasks(dag_tasks_1))
-                )
-                join_foreach_task = (
-                    DAGTask(self._sanitize(self.graph[node.matching_join].name))
-                    .template(self._sanitize(self.graph[node.matching_join].name))
-                    .dependencies([foreach_template_name])
-                    .arguments(
-                        Arguments().parameters(
-                            [
-                                Parameter("input-paths").value(
-                                    "argo-{{workflow.name}}/%s/{{tasks.%s.outputs.parameters}}"
-                                    % (
-                                        self.graph[node.matching_join].in_funcs[-1],
-                                        foreach_template_name,
-                                    )
-                                )
-                            ]
-                        )
-                    )
-                )
-                dag_tasks.append(join_foreach_task)
-                return _visit(
-                    self.graph[self.graph[node.matching_join].out_funcs[0]],
-                    exit_node,
-                    templates,
-                    dag_tasks,
-                )
-            # For linear nodes continue traversing to the next node
-            if node.type in ("linear", "join", "start"):
-                return _visit(
-                    self.graph[node.out_funcs[0]], exit_node, templates, dag_tasks
-                )
-            else:
-                raise ArgoWorkflowsException(
-                    "Node type *%s* for step *%s* is not currently supported by "
-                    "Argo Workflows." % (node.type, node.name)
-                )
+class MetaflowS3NotFound(MetaflowException):
+    headline = "S3 object not found"
 
-        templates, _ = _visit(node=self.graph["start"])
-        return templates
 
-    # Visit every node and yield ContainerTemplates.
-    def _container_templates(self):
-        try:
-            # Kubernetes is a soft dependency for generating Argo objects.
-            # We can very well remove this dependency for Argo with the downside of
-            # adding a bunch more json bloat classes (looking at you... V1Container)
-            from kubernetes import client as kubernetes_sdk
-        except (NameError, ImportError):
-            raise MetaflowException(
-                "Could not import Python package 'kubernetes'. Install kubernetes "
-                "sdk (https://pypi.org/project/kubernetes/) first."
-            )
-        for node in self.graph:
-            # Resolve entry point for pod container.
-            script_name = os.path.basename(sys.argv[0])
-            executable = self.environment.executable(node.name)
-            # TODO: Support R someday. Quite a few people will be happy.
-            entrypoint = [executable, script_name]
-
-            # The values with curly braces '{{}}' are made available by Argo
-            # Workflows. Unfortunately, there are a few bugs in Argo which prevent
-            # us from accessing these values as liberally as we would like to - e.g,
-            # within inline templates - so we are forced to generate container templates
-            run_id = "argo-{{workflow.name}}"
-
-            # Unfortunately, we don't have any easy access to unique ids that remain
-            # stable across task attempts through Argo Workflows. So, we are forced to
-            # stitch them together ourselves. The task ids are a function of step name,
-            # split index and the parent task id (available from input path name).
-            # Ideally, we would like these task ids to be the same as node name
-            # (modulo retry suffix) on Argo Workflows but that doesn't seem feasible
-            # right now.
-            task_str = node.name + "-{{workflow.creationTimestamp}}"
-            if node.name != "start":
-                task_str += "-{{inputs.parameters.input-paths}}"
-            if any(self.graph[n].type == "foreach" for n in node.in_funcs):
-                task_str += "-{{inputs.parameters.split-index}}"
-            # Generated task_ids need to be non-numeric - see register_task_id in
-            # service.py. We do so by prefixing `t-`
-            task_id_expr = (
-                "export METAFLOW_TASK_ID="
-                "(t-$(echo %s | md5sum | cut -d ' ' -f 1 | tail -c 9))" % task_str
-            )
-            task_id = "$METAFLOW_TASK_ID"
+class MetaflowS3AccessDenied(MetaflowException):
+    headline = "S3 access denied"
 
-            # Resolve retry strategy.
-            (
-                user_code_retries,
-                total_retries,
-                retry_count,
-                minutes_between_retries,
-            ) = self._get_retries(node)
-
-            mflog_expr = export_mflog_env_vars(
-                datastore_type=self.flow_datastore.TYPE,
-                stdout_path="$PWD/.logs/mflog_stdout",
-                stderr_path="$PWD/.logs/mflog_stderr",
-                flow_name=self.flow.name,
-                run_id=run_id,
-                step_name=node.name,
-                task_id=task_id,
-                retry_count=retry_count,
-            )
 
-            init_cmds = " && ".join(
-                [
-                    # For supporting sandboxes, ensure that a custom script is executed
-                    # before anything else is executed. The script is passed in as an
-                    # env var.
-                    '${METAFLOW_INIT_SCRIPT:+eval \\"${METAFLOW_INIT_SCRIPT}\\"}',
-                    "mkdir -p $PWD/.logs",
-                    task_id_expr,
-                    mflog_expr,
-                ]
-                + self.environment.get_package_commands(
-                    self.code_package_url, self.flow_datastore.TYPE
-                )
-            )
-            step_cmds = self.environment.bootstrap_commands(
-                node.name, self.flow_datastore.TYPE
-            )
+class MetaflowS3InvalidRange(MetaflowException):
+    headline = "S3 invalid range"
 
-            input_paths = "{{inputs.parameters.input-paths}}"
 
-            top_opts_dict = {
-                "with": [
-                    decorator.make_decorator_spec()
-                    for decorator in node.decorators
-                    if not decorator.statically_defined
-                ]
-            }
-            # FlowDecorators can define their own top-level options. They are
-            # responsible for adding their own top-level options and values through
-            # the get_top_level_options() hook. See similar logic in runtime.py.
-            for deco in flow_decorators():
-                top_opts_dict.update(deco.get_top_level_options())
-
-            top_level = list(dict_to_cli_options(top_opts_dict)) + [
-                "--quiet",
-                "--metadata=%s" % self.metadata.TYPE,
-                "--environment=%s" % self.environment.TYPE,
-                "--datastore=%s" % self.flow_datastore.TYPE,
-                "--datastore-root=%s" % self.flow_datastore.datastore_root,
-                "--event-logger=%s" % self.event_logger.TYPE,
-                "--monitor=%s" % self.monitor.TYPE,
-                "--no-pylint",
-                "--with=argo_workflows_internal",
-            ]
-
-            if node.name == "start":
-                # Execute `init` before any step of the workflow executes
-                task_id_params = "%s-params" % task_id
-                init = (
-                    entrypoint
-                    + top_level
-                    + [
-                        "init",
-                        "--run-id %s" % run_id,
-                        "--task-id %s" % task_id_params,
-                    ]
-                    + [
-                        # Parameter names can be hyphenated, hence we use
-                        # {{foo.bar['param_name']}}
-                        "--%s={{workflow.parameters.%s}}"
-                        % (parameter["name"], parameter["name"])
-                        for parameter in self.parameters
-                    ]
-                )
-                if self.tags:
-                    init.extend("--tag %s" % tag for tag in self.tags)
-                # if the start step gets retried, we must be careful
-                # not to regenerate multiple parameters tasks. Hence,
-                # we check first if _parameters exists already.
-                exists = entrypoint + [
-                    "dump",
-                    "--max-value-size=0",
-                    "%s/_parameters/%s" % (run_id, task_id_params),
-                ]
-                step_cmds.extend(
-                    [
-                        "if ! %s >/dev/null 2>/dev/null; then %s; fi"
-                        % (" ".join(exists), " ".join(init))
-                    ]
-                )
-                input_paths = "%s/_parameters/%s" % (run_id, task_id_params)
-            elif (
-                node.type == "join"
-                and self.graph[node.split_parents[-1]].type == "foreach"
-            ):
-                # Set aggregated input-paths for a foreach-join
-                input_paths = (
-                    "$(python -m metaflow.plugins.argo.process_input_paths %s)"
-                    % input_paths
-                )
-            step = [
-                "step",
-                node.name,
-                "--run-id %s" % run_id,
-                "--task-id %s" % task_id,
-                "--retry-count %s" % retry_count,
-                "--max-user-code-retries %d" % user_code_retries,
-                "--input-paths %s" % input_paths,
-            ]
-            if any(self.graph[n].type == "foreach" for n in node.in_funcs):
-                # Pass split-index to a foreach task
-                step.append("--split-index {{inputs.parameters.split-index}}")
-            if self.tags:
-                step.extend("--tag %s" % tag for tag in self.tags)
-            if self.namespace is not None:
-                step.append("--namespace=%s" % self.namespace)
-
-            step_cmds.extend([" ".join(entrypoint + top_level + step)])
-
-            cmd_str = "%s; c=$?; %s; exit $c" % (
-                " && ".join([init_cmds, bash_capture_logs(" && ".join(step_cmds))]),
-                BASH_SAVE_LOGS,
-            )
-            cmds = shlex.split('bash -c "%s"' % cmd_str)
+class S3Object(object):
+    """
+    This object represents a path or an object in S3,
+    with an optional local copy.
 
-            # Resolve resource requirements.
-            resources = dict(
-                [deco for deco in node.decorators if deco.name == "kubernetes"][
-                    0
-                ].attributes
-            )
+    `S3Object`s are not instantiated directly, but they are returned
+    by many methods of the `S3` client.
+    """
 
-            if (
-                resources["namespace"]
-                and resources["namespace"] != KUBERNETES_NAMESPACE
-            ):
-                raise ArgoWorkflowsException(
-                    "Multi-namespace Kubernetes execution of flows in Argo Workflows "
-                    "is not currently supported. \nStep *%s* is trying to override the "
-                    "default Kubernetes namespace *%s*."
-                    % (node.name, KUBERNETES_NAMESPACE)
-                )
+    def __init__(
+        self,
+        prefix: str,
+        url: str,
+        path: str,
+        size: Optional[int] = None,
+        content_type: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        range_info: Optional[RangeInfo] = None,
+        last_modified: int = None,
+    ):
+        # all fields of S3Object should return a unicode object
+        prefix, url, path = map(ensure_unicode, (prefix, url, path))
 
-            run_time_limit = [
-                deco for deco in node.decorators if deco.name == "kubernetes"
-            ][0].run_time_limit
-
-            # Resolve @environment decorator. We set three classes of environment
-            # variables -
-            #   (1) User-specified environment variables through @environment
-            #   (2) Metaflow runtime specific environment variables
-            #   (3) @kubernetes, @argo_workflows_internal bookkeeping environment
-            #       variables
-            env = dict(
-                [deco for deco in node.decorators if deco.name == "environment"][
-                    0
-                ].attributes["vars"]
-            )
-            env.update(
-                {
-                    **{
-                        # These values are needed by Metaflow to set it's internal
-                        # state appropriately
-                        "METAFLOW_CODE_URL": self.code_package_url,
-                        "METAFLOW_CODE_SHA": self.code_package_sha,
-                        "METAFLOW_CODE_DS": self.flow_datastore.TYPE,
-                        "METAFLOW_SERVICE_URL": SERVICE_INTERNAL_URL,
-                        "METAFLOW_SERVICE_HEADERS": json.dumps(SERVICE_HEADERS),
-                        "METAFLOW_USER": "argo-workflows",
-                        "METAFLOW_DATASTORE_SYSROOT_S3": DATASTORE_SYSROOT_S3,
-                        "METAFLOW_DATATOOLS_S3ROOT": DATATOOLS_S3ROOT,
-                        "METAFLOW_DEFAULT_DATASTORE": self.flow_datastore.TYPE,
-                        "METAFLOW_DEFAULT_METADATA": DEFAULT_METADATA,
-                        "METAFLOW_CARD_S3ROOT": CARD_S3ROOT,
-                        "METAFLOW_KUBERNETES_WORKLOAD": 1,
-                        "METAFLOW_KUBERNETES_FETCH_EC2_METADATA": KUBERNETES_FETCH_EC2_METADATA,
-                        "METAFLOW_RUNTIME_ENVIRONMENT": "kubernetes",
-                        "METAFLOW_OWNER": self.username,
-                    },
-                    **{
-                        # Some optional values for bookkeeping
-                        "METAFLOW_FLOW_NAME": self.flow.name,
-                        "METAFLOW_STEP_NAME": node.name,
-                        "METAFLOW_RUN_ID": run_id,
-                        # "METAFLOW_TASK_ID": task_id,
-                        "METAFLOW_RETRY_COUNT": retry_count,
-                        "METAFLOW_PRODUCTION_TOKEN": self.production_token,
-                        "ARGO_WORKFLOW_TEMPLATE": self.name,
-                        "ARGO_WORKFLOW_NAME": "{{workflow.name}}",
-                        "ARGO_WORKFLOW_NAMESPACE": KUBERNETES_NAMESPACE,
-                    },
-                    **self.metadata.get_runtime_environment("argo-workflows"),
-                }
+        self._size = size
+        self._url = url
+        self._path = path
+        self._key = None
+        self._content_type = content_type
+        self._last_modified = last_modified
+
+        self._metadata = None
+        if metadata is not None and "metaflow-user-attributes" in metadata:
+            self._metadata = json.loads(metadata["metaflow-user-attributes"])
+
+        if range_info and (
+            range_info.request_length is None or range_info.request_length < 0
+        ):
+            self._range_info = RangeInfo(
+                range_info.total_size, range_info.request_offset, range_info.total_size
             )
-            # add METAFLOW_S3_ENDPOINT_URL
-            env["METAFLOW_S3_ENDPOINT_URL"] = S3_ENDPOINT_URL
-
-            # support Metaflow sandboxes
-            env["METAFLOW_INIT_SCRIPT"] = KUBERNETES_SANDBOX_INIT_SCRIPT
-
-            # secrets stuff
-            env["METAFLOW_DEFAULT_SECRETS_BACKEND_TYPE"] = DEFAULT_SECRETS_BACKEND_TYPE
-            env[
-                "METAFLOW_AWS_SECRETS_MANAGER_DEFAULT_REGION"
-            ] = AWS_SECRETS_MANAGER_DEFAULT_REGION
-
-            # Azure stuff
-            env[
-                "METAFLOW_AZURE_STORAGE_BLOB_SERVICE_ENDPOINT"
-            ] = AZURE_STORAGE_BLOB_SERVICE_ENDPOINT
-            env["METAFLOW_DATASTORE_SYSROOT_AZURE"] = DATASTORE_SYSROOT_AZURE
-            env["METAFLOW_CARD_AZUREROOT"] = CARD_AZUREROOT
-
-            # GCP stuff
-            env["METAFLOW_DATASTORE_SYSROOT_GS"] = DATASTORE_SYSROOT_GS
-            env["METAFLOW_CARD_GSROOT"] = CARD_GSROOT
-
-            metaflow_version = self.environment.get_environment_info()
-            metaflow_version["flow_name"] = self.graph.name
-            metaflow_version["production_token"] = self.production_token
-            env["METAFLOW_VERSION"] = json.dumps(metaflow_version)
-
-            # Set the template inputs and outputs for passing state. Very simply,
-            # the container template takes in input-paths as input and outputs
-            # the task-id (which feeds in as input-paths to the subsequent task).
-            # In addition to that, if the parent of the node under consideration
-            # is a for-each node, then we take the split-index as an additional
-            # input. Analogously, if the node under consideration is a foreach
-            # node, then we emit split cardinality as an extra output. I would like
-            # to thank the designers of Argo Workflows for making this so
-            # straightforward!
-            inputs = []
-            if node.name != "start":
-                inputs.append(Parameter("input-paths"))
-            if any(self.graph[n].type == "foreach" for n in node.in_funcs):
-                # Fetch split-index from parent
-                inputs.append(Parameter("split-index"))
-
-            outputs = []
-            if node.name != "end":
-                outputs = [Parameter("task-id").valueFrom({"path": "/mnt/out/task_id"})]
-            if node.type == "foreach":
-                # Emit split cardinality from foreach task
-                outputs.append(
-                    Parameter("num-splits").valueFrom({"path": "/mnt/out/splits"})
-                )
+        else:
+            self._range_info = range_info
 
-            # It makes no sense to set env vars to None (shows up as "None" string)
-            # Also we skip some env vars (e.g. in case we want to pull them from KUBERNETES_SECRETS)
-            env_vars_to_skip = set(ARGO_WORKFLOWS_ENV_VARS_TO_SKIP.split(","))
-            env = {
-                k: v
-                for k, v in env.items()
-                if v is not None and k not in env_vars_to_skip
-            }
+        if path:
+            self._size = os.stat(self._path).st_size
 
-            # Create a ContainerTemplate for this node. Ideally, we would have
-            # liked to inline this ContainerTemplate and avoid scanning the workflow
-            # twice, but due to issues with variable substitution, we will have to
-            # live with this routine.
-            yield (
-                Template(self._sanitize(node.name))
-                # Set @timeout values
-                .active_deadline_seconds(run_time_limit)
-                # Set service account
-                .service_account_name(resources["service_account"])
-                # Configure template input
-                .inputs(Inputs().parameters(inputs))
-                # Configure template output
-                .outputs(Outputs().parameters(outputs))
-                # Fail fast!
-                .fail_fast()
-                # Set @retry/@catch values
-                .retry_strategy(
-                    times=total_retries,
-                    minutes_between_retries=minutes_between_retries,
-                )
-                .metadata(
-                    ObjectMeta().annotation("metaflow/step_name", node.name)
-                    # Unfortunately, we can't set the task_id since it is generated
-                    # inside the pod. However, it can be inferred from the annotation
-                    # set by argo-workflows - `workflows.argoproj.io/outputs` - refer
-                    # the field 'task-id' in 'parameters'
-                    # .annotation("metaflow/task_id", ...)
-                    .annotation("metaflow/attempt", retry_count)
-                )
-                # Set emptyDir volume for state management
-                .empty_dir_volume("out")
-                # Set node selectors
-                .node_selectors(resources.get("node_selector"))
-                .tolerations(resources.get("tolerations"))
-                # Set container
-                .container(
-                    # TODO: Unify the logic with kubernetes.py
-                    # Important note - Unfortunately, V1Container uses snakecase while
-                    # Argo Workflows uses camel. For most of the attributes, both cases
-                    # are indistinguishable, but unfortunately, not for all - (
-                    # env_from, value_from, etc.) - so we need to handle the conversion
-                    # ourselves using to_camelcase. We need to be vigilant about
-                    # resources attributes in particular where the keys maybe user
-                    # defined.
-                    to_camelcase(
-                        kubernetes_sdk.V1Container(
-                            name=self._sanitize(node.name),
-                            command=cmds,
-                            env=[
-                                kubernetes_sdk.V1EnvVar(name=k, value=str(v))
-                                for k, v in env.items()
-                            ]
-                            # Add environment variables for book-keeping.
-                            # https://argoproj.github.io/argo-workflows/fields/#fields_155
-                            + [
-                                kubernetes_sdk.V1EnvVar(
-                                    name=k,
-                                    value_from=kubernetes_sdk.V1EnvVarSource(
-                                        field_ref=kubernetes_sdk.V1ObjectFieldSelector(
-                                            field_path=str(v)
-                                        )
-                                    ),
-                                )
-                                for k, v in {
-                                    "METAFLOW_KUBERNETES_POD_NAMESPACE": "metadata.namespace",
-                                    "METAFLOW_KUBERNETES_POD_NAME": "metadata.name",
-                                    "METAFLOW_KUBERNETES_POD_ID": "metadata.uid",
-                                    "METAFLOW_KUBERNETES_SERVICE_ACCOUNT_NAME": "spec.serviceAccountName",
-                                    "METAFLOW_KUBERNETES_NODE_IP": "status.hostIP",
-                                }.items()
-                            ],
-                            image=resources["image"],
-                            resources=kubernetes_sdk.V1ResourceRequirements(
-                                requests={
-                                    "cpu": str(resources["cpu"]),
-                                    "memory": "%sM" % str(resources["memory"]),
-                                    "ephemeral-storage": "%sM" % str(resources["disk"]),
-                                },
-                                limits={
-                                    "%s.com/gpu".lower()
-                                    % resources["gpu_vendor"]: str(resources["gpu"])
-                                    for k in [0]
-                                    if resources["gpu"] is not None
-                                },
-                            ),
-                            # Configure secrets
-                            env_from=[
-                                kubernetes_sdk.V1EnvFromSource(
-                                    secret_ref=kubernetes_sdk.V1SecretEnvSource(
-                                        name=str(k),
-                                        # optional=True
-                                    )
-                                )
-                                for k in list(
-                                    []
-                                    if not resources.get("secrets")
-                                    else [resources.get("secrets")]
-                                    if isinstance(resources.get("secrets"), str)
-                                    else resources.get("secrets")
-                                )
-                                + KUBERNETES_SECRETS.split(",")
-                                + ARGO_WORKFLOWS_KUBERNETES_SECRETS.split(",")
-                                if k
-                            ],
-                            # Assign a volume point to pass state to the next task.
-                            volume_mounts=[
-                                kubernetes_sdk.V1VolumeMount(
-                                    name="out", mount_path="/mnt/out"
-                                )
-                            ],
-                        ).to_dict()
-                    )
-                )
-            )
-
-    def _get_retries(self, node):
-        max_user_code_retries = 0
-        max_error_retries = 0
-        minutes_between_retries = "2"
-        for deco in node.decorators:
-            if deco.name == "retry":
-                minutes_between_retries = deco.attributes.get(
-                    "minutes_between_retries", minutes_between_retries
-                )
-            user_code_retries, error_retries = deco.step_task_retry_count()
-            max_user_code_retries = max(max_user_code_retries, user_code_retries)
-            max_error_retries = max(max_error_retries, error_retries)
+        if prefix is None or prefix == url:
+            self._key = url
+            self._prefix = None
+        else:
+            self._key = url[len(prefix.rstrip("/")) + 1 :].rstrip("/")
+            self._prefix = prefix
 
+    @property
+    def exists(self) -> bool:
+        """
+        Does this key correspond to an object in S3?
+
+        Returns
+        -------
+        bool
+            True if this object points at an existing object (file) in S3.
+        """
+        return self._size is not None
+
+    @property
+    def downloaded(self) -> bool:
+        """
+        Has this object been downloaded?
+
+        If True, the contents can be accessed through `path`, `blob`,
+        and `text` properties.
+
+        Returns
+        -------
+        bool
+            True if the contents of this object have been downloaded.
+        """
+        return bool(self._path)
+
+    @property
+    def url(self) -> str:
+        """
+        S3 location of the object
+
+        Returns
+        -------
+        str
+            The S3 location of this object.
+        """
+        return self._url
+
+    @property
+    def prefix(self) -> str:
+        """
+        Prefix requested that matches this object.
+
+        Returns
+        -------
+        str
+            Requested prefix
+        """
+        return self._prefix
+
+    @property
+    def key(self) -> str:
+        """
+        Key corresponds to the key given to the get call that produced
+        this object.
+
+        This may be a full S3 URL or a suffix based on what
+        was requested.
+
+        Returns
+        -------
+        str
+            Key requested.
+        """
+        return self._key
+
+    @property
+    def path(self) -> Optional[str]:
+        """
+        Path to a local temporary file corresponding to the object downloaded.
+
+        This file gets deleted automatically when a S3 scope exits.
+        Returns None if this S3Object has not been downloaded.
+
+        Returns
+        -------
+        str
+            Local path, if the object has been downloaded.
+        """
+        return self._path
+
+    @property
+    def blob(self) -> Optional[bytes]:
+        """
+        Contents of the object as a byte string or None if the
+        object hasn't been downloaded.
+
+        Returns
+        -------
+        bytes
+            Contents of the object as bytes.
+        """
+        if self._path:
+            with open(self._path, "rb") as f:
+                return f.read()
+
+    @property
+    def text(self) -> Optional[str]:
+        """
+        Contents of the object as a string or None if the
+        object hasn't been downloaded.
+
+        The object is assumed to contain UTF-8 encoded data.
+
+        Returns
+        -------
+        str
+            Contents of the object as text.
+        """
+        if self._path:
+            return self.blob.decode("utf-8", errors="replace")
+
+    @property
+    def size(self) -> Optional[int]:
+        """
+        Size of the object in bytes.
+
+        Returns None if the key does not correspond to an object in S3.
+
+        Returns
+        -------
+        int
+            Size of the object in bytes, if the object exists.
+        """
+        return self._size
+
+    @property
+    def has_info(self) -> bool:
+        """
+        Returns true if this `S3Object` contains the content-type MIME header or
+        user-defined metadata.
+
+        If False, this means that `content_type`, `metadata`, `range_info` and
+        `last_modified` will return None.
+
+        Returns
+        -------
+        bool
+            True if additional metadata is available.
+        """
         return (
-            max_user_code_retries,
-            max_user_code_retries + max_error_retries,
-            # {{retries}} is only available if retryStrategy is specified
-            "{{retries}}" if max_user_code_retries + max_error_retries else 0,
-            int(minutes_between_retries),
+            self._content_type is not None
+            or self._metadata is not None
+            or self._range_info is not None
         )
 
-
-# Helper classes to assist with JSON-foo. This can very well replaced with an explicit
-# dependency on argo-workflows Python SDK if this method turns out to be painful.
-# TODO: Autogenerate them, maybe?
-
-
-class WorkflowTemplate(object):
-    # https://argoproj.github.io/argo-workflows/fields/#workflowtemplate
-
-    def __init__(self):
-        tree = lambda: defaultdict(tree)
-        self.payload = tree()
-        self.payload["apiVersion"] = "argoproj.io/v1alpha1"
-        self.payload["kind"] = "WorkflowTemplate"
-
-    def metadata(self, object_meta):
-        self.payload["metadata"] = object_meta.to_json()
-        return self
-
-    def spec(self, workflow_spec):
-        self.payload["spec"] = workflow_spec.to_json()
-        return self
-
-    def to_json(self):
-        return self.payload
+    @property
+    def metadata(self) -> Optional[Dict[str, str]]:
+        """
+        Returns a dictionary of user-defined metadata, or None if no metadata
+        is defined.
+
+        Returns
+        -------
+        Dict
+            User-defined metadata.
+        """
+        return self._metadata
+
+    @property
+    def content_type(self) -> Optional[str]:
+        """
+        Returns the content-type of the S3 object or None if it is not defined.
+
+        Returns
+        -------
+        str
+            Content type or None if the content type is undefined.
+        """
+        return self._content_type
+
+    @property
+    def range_info(self) -> Optional[RangeInfo]:
+        """
+        If the object corresponds to a partially downloaded object, returns
+        information of what was downloaded.
+
+        The returned object has the following fields:
+        - `total_size`: Size of the object in S3.
+        - `request_offset`: The starting offset.
+        - `request_length`: The number of bytes downloaded.
+
+        Returns
+        -------
+        namedtuple
+            An object containing information about the partial download. If
+            the `S3Object` doesn't correspond to a partially downloaded file,
+            returns None.
+        """
+        return self._range_info
+
+    @property
+    def last_modified(self) -> Optional[int]:
+        """
+        Returns the last modified unix timestamp of the object.
+
+        Returns
+        -------
+        int
+            Unix timestamp corresponding to the last modified time.
+        """
+        return self._last_modified
 
     def __str__(self):
-        return json.dumps(self.payload, indent=4)
-
-
-class ObjectMeta(object):
-    # https://argoproj.github.io/argo-workflows/fields/#objectmeta
-
-    def __init__(self):
-        tree = lambda: defaultdict(tree)
-        self.payload = tree()
-
-    def annotation(self, key, value):
-        self.payload["annotations"][key] = str(value)
-        return self
-
-    def annotations(self, annotations):
-        if "annotations" not in self.payload:
-            self.payload["annotations"] = {}
-        self.payload["annotations"].update(annotations)
-        return self
-
-    def generate_name(self, generate_name):
-        self.payload["generateName"] = generate_name
-        return self
-
-    def label(self, key, value):
-        self.payload["labels"][key] = str(value)
-        return self
-
-    def labels(self, labels):
-        if "labels" not in self.payload:
-            self.payload["labels"] = {}
-        self.payload["labels"].update(labels)
-        return self
-
-    def name(self, name):
-        self.payload["name"] = name
-        return self
-
-    def namespace(self, namespace):
-        self.payload["namespace"] = namespace
-        return self
-
-    def to_json(self):
-        return self.payload
-
-    def __str__(self):
-        return json.dumps(self.to_json(), indent=4)
-
-
-class WorkflowSpec(object):
-    # https://argoproj.github.io/argo-workflows/fields/#workflowspec
-    # This object sets all Workflow level properties.
-
-    def __init__(self):
-        tree = lambda: defaultdict(tree)
-        self.payload = tree()
-
-    def active_deadline_seconds(self, active_deadline_seconds):
-        # Overall duration of a workflow in seconds
-        if active_deadline_seconds is not None:
-            self.payload["activeDeadlineSeconds"] = int(active_deadline_seconds)
-        return self
-
-    def automount_service_account_token(self, mount=True):
-        self.payload["automountServiceAccountToken"] = mount
-        return self
-
-    def arguments(self, arguments):
-        self.payload["arguments"] = arguments.to_json()
-        return self
-
-    def archive_logs(self, archive_logs=True):
-        self.payload["archiveLogs"] = archive_logs
-        return self
-
-    def entrypoint(self, entrypoint):
-        self.payload["entrypoint"] = entrypoint
-        return self
-
-    def parallelism(self, parallelism):
-        # Set parallelism at Workflow level
-        self.payload["parallelism"] = int(parallelism)
-        return self
-
-    def pod_metadata(self, metadata):
-        self.payload["podMetadata"] = metadata.to_json()
-        return self
-
-    def priority(self, priority):
-        if priority is not None:
-            self.payload["priority"] = int(priority)
-        return self
-
-    def workflow_metadata(self, workflow_metadata):
-        self.payload["workflowMetadata"] = workflow_metadata.to_json()
-        return self
-
-    def service_account_name(self, service_account_name):
-        # https://argoproj.github.io/argo-workflows/workflow-rbac/
-        self.payload["serviceAccountName"] = service_account_name
-        return self
-
-    def templates(self, templates):
-        if "templates" not in self.payload:
-            self.payload["templates"] = []
-        for template in templates:
-            self.payload["templates"].append(template.to_json())
-        return self
-
-    def to_json(self):
-        return self.payload
-
-    def __str__(self):
-        return json.dumps(self.to_json(), indent=4)
-
-
-class Metadata(object):
-    # https://argoproj.github.io/argo-workflows/fields/#metadata
-
-    def __init__(self):
-        tree = lambda: defaultdict(tree)
-        self.payload = tree()
-
-    def annotation(self, key, value):
-        self.payload["annotations"][key] = str(value)
-        return self
-
-    def annotations(self, annotations):
-        if "annotations" not in self.payload:
-            self.payload["annotations"] = {}
-        self.payload["annotations"].update(annotations)
-        return self
-
-    def label(self, key, value):
-        self.payload["labels"][key] = str(value)
-        return self
+        if self._path:
+            return "<S3Object %s (%d bytes, local)>" % (self._url, self._size)
+        elif self._size:
+            return "<S3Object %s (%d bytes, in S3)>" % (self._url, self._size)
+        else:
+            return "<S3Object %s (object does not exist)>" % self._url
 
-    def labels(self, labels):
-        if "labels" not in self.payload:
-            self.payload["labels"] = {}
-        self.payload["labels"].update(labels)
-        return self
+    def __repr__(self):
+        return str(self)
 
-    def labels_from(self, labels_from):
-        # Only available in workflow_metadata
-        # https://github.com/argoproj/argo-workflows/blob/master/examples/label-value-from-workflow.yaml
-        if "labelsFrom" not in self.payload:
-            self.payload["labelsFrom"] = {}
-        for k, v in labels_from.items():
-            self.payload["labelsFrom"].update({k: {"expression": v}})
-        return self
 
-    def to_json(self):
-        return self.payload
+class S3Client(object):
+    def __init__(self, s3_role_arn=None, s3_session_vars=None, s3_client_params=None):
+        self._s3_client = None
+        self._s3_error = None
+        self._s3_role = s3_role_arn
+        self._s3_session_vars = s3_session_vars
+        self._s3_client_params = s3_client_params
+
+    @property
+    def client(self):
+        if self._s3_client is None:
+            self.reset_client()
+        return self._s3_client
+
+    @property
+    def error(self):
+        if self._s3_error is None:
+            self.reset_client()
+        return self._s3_error
+
+    def reset_client(self):
+        self._s3_client, self._s3_error = get_s3_client(
+            s3_role_arn=self._s3_role,
+            s3_session_vars=self._s3_session_vars,
+            s3_client_params=self._s3_client_params,
+        )
 
-    def __str__(self):
-        return json.dumps(self.to_json(), indent=4)
 
+class S3(object):
+    """
+    The Metaflow S3 client.
+
+    This object manages the connection to S3 and a temporary diretory that is used
+    to download objects. Note that in most cases when the data fits in memory, no local
+    disk IO is needed as operations are cached by the operating system, which makes
+    operations fast as long as there is enough memory available.
+
+    The easiest way is to use this object as a context manager:
+    ```
+    with S3() as s3:
+        data = [obj.blob for obj in s3.get_many(urls)]
+    print(data)
+    ```
+    The context manager takes care of creating and deleting a temporary directory
+    automatically. Without a context manager, you must call `.close()` to delete
+    the directory explicitly:
+    ```
+    s3 = S3()
+    data = [obj.blob for obj in s3.get_many(urls)]
+    s3.close()
+    ```
+    You can customize the location of the temporary directory with `tmproot`. It
+    defaults to the current working directory.
+
+    To make it easier to deal with object locations, the client can be initialized
+    with an S3 path prefix. There are three ways to handle locations:
+
+    1. Use a `metaflow.Run` object or `self`, e.g. `S3(run=self)` which
+       initializes the prefix with the global `DATATOOLS_S3ROOT` path, combined
+       with the current run ID. This mode makes it easy to version data based
+       on the run ID consistently. You can use the `bucket` and `prefix` to
+       override parts of `DATATOOLS_S3ROOT`.
+
+    2. Specify an S3 prefix explicitly with `s3root`,
+       e.g. `S3(s3root='s3://mybucket/some/path')`.
+
+    3. Specify nothing, i.e. `S3()`, in which case all operations require
+       a full S3 url prefixed with `s3://`.
+
+    Parameters
+    ----------
+    tmproot : str, default: '.'
+        Where to store the temporary directory.
+    bucket : str, optional
+        Override the bucket from `DATATOOLS_S3ROOT` when `run` is specified.
+    prefix : str, optional
+        Override the path from `DATATOOLS_S3ROOT` when `run` is specified.
+    run : FlowSpec or Run, optional
+        Derive path prefix from the current or a past run ID, e.g. S3(run=self).
+    s3root : str, optional
+        If `run` is not specified, use this as the S3 prefix.
+    """
 
-class Template(object):
-    # https://argoproj.github.io/argo-workflows/fields/#template
+    @classmethod
+    def get_root_from_config(cls, echo, create_on_absent=True):
+        return DATATOOLS_S3ROOT
 
-    def __init__(self, name):
-        tree = lambda: defaultdict(tree)
-        self.payload = tree()
-        self.payload["name"] = name
+    def __init__(
+        self,
+        tmproot: str = TEMPDIR,
+        bucket: Optional[str] = None,
+        prefix: Optional[str] = None,
+        run: Optional[Union[FlowSpec, "Run"]] = None,
+        s3root: Optional[str] = None,
+        **kwargs
+    ):
+        if not boto_found:
+            raise MetaflowException("You need to install 'boto3' in order to use S3.")
 
-    def active_deadline_seconds(self, active_deadline_seconds):
-        # Overall duration of a pod in seconds, only obeyed for container templates
-        # Used for implementing @timeout.
-        self.payload["activeDeadlineSeconds"] = int(active_deadline_seconds)
-        return self
+        if run:
+            # 1. use a (current) run ID with optional customizations
+            parsed = urlparse(DATATOOLS_S3ROOT)
+            if not bucket:
+                bucket = parsed.netloc
+            if not prefix:
+                prefix = parsed.path
+            if isinstance(run, FlowSpec):
+                if current.is_running_flow:
+                    prefix = os.path.join(prefix, current.flow_name, current.run_id)
+                else:
+                    raise MetaflowS3URLException(
+                        "Initializing S3 with a FlowSpec outside of a running "
+                        "flow is not supported."
+                    )
+            else:
+                prefix = os.path.join(prefix, run.parent.id, run.id)
 
-    def dag(self, dag_template):
-        self.payload["dag"] = dag_template.to_json()
-        return self
+            self._s3root = "s3://%s" % os.path.join(bucket, prefix.strip("/"))
+        elif s3root:
+            # 2. use an explicit S3 prefix
+            parsed = urlparse(to_unicode(s3root))
+            if parsed.scheme != "s3":
+                raise MetaflowS3URLException(
+                    "s3root needs to be an S3 URL prefixed with s3://."
+                )
+            self._s3root = s3root.rstrip("/")
+        else:
+            # 3. use the client only with full URLs
+            self._s3root = None
 
-    def container(self, container):
-        # Luckily this can simply be V1Container and we are spared from writing more
-        # boilerplate - https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Container.md.
-        self.payload["container"] = container
-        return self
+        # Note that providing a role, session vars or client params and a client
+        # will result in the role/session vars/client params being ignored
+        self._s3_role = kwargs.get("role", None)
+        self._s3_session_vars = kwargs.get("session_vars", None)
+        self._s3_client_params = kwargs.get("client_params", None)
+        self._s3_client = kwargs.get(
+            "external_client",
+            S3Client(
+                s3_role_arn=self._s3_role,
+                s3_session_vars=self._s3_session_vars,
+                s3_client_params=self._s3_client_params,
+            ),
+        )
+        self._s3_inject_failures = kwargs.get(
+            "inject_failure_rate", TEST_INJECT_RETRYABLE_FAILURES
+        )
+        self._tmpdir = mkdtemp(dir=tmproot, prefix="metaflow.s3.")
 
-    def inputs(self, inputs):
-        self.payload["inputs"] = inputs.to_json()
+    def __enter__(self) -> "S3":
         return self
 
-    def outputs(self, outputs):
-        self.payload["outputs"] = outputs.to_json()
-        return self
+    def __exit__(self, *args):
+        self.close()
 
-    def fail_fast(self, fail_fast=True):
-        # https://github.com/argoproj/argo-workflows/issues/1442
-        self.payload["failFast"] = fail_fast
-        return self
+    def close(self):
+        """
+        Delete all temporary files downloaded in this context.
+        """
+        try:
+            if not debug.s3client:
+                if self._tmpdir:
+                    shutil.rmtree(self._tmpdir)
+                    self._tmpdir = None
+        except:
+            pass
+
+    def _url(self, key_value):
+        # NOTE: All URLs are handled as Unicode objects (unicode in py2,
+        # string in py3) internally. We expect that all URLs passed to this
+        # class as either Unicode or UTF-8 encoded byte strings. All URLs
+        # returned are Unicode.
+        key = getattr(key_value, "key", key_value)
+        if self._s3root is None:
+            parsed = urlparse(to_unicode(key))
+            if parsed.scheme == "s3" and parsed.path:
+                return key
+            else:
+                if current.is_running_flow:
+                    raise MetaflowS3URLException(
+                        "Specify S3(run=self) when you use S3 inside a running "
+                        "flow. Otherwise you have to use S3 with full "
+                        "s3:// urls."
+                    )
+                else:
+                    raise MetaflowS3URLException(
+                        "Initialize S3 with an 's3root' or 'run' if you don't "
+                        "want to specify full s3:// urls."
+                    )
+        elif key:
+            if key.startswith("s3://"):
+                raise MetaflowS3URLException(
+                    "Don't use absolute S3 URLs when the S3 client is "
+                    "initialized with a prefix. URL: %s" % key
+                )
+            return os.path.join(self._s3root, key)
+        else:
+            return self._s3root
 
-    def metadata(self, metadata):
-        self.payload["metadata"] = metadata.to_json()
-        return self
+    def _url_and_range(self, key_value):
+        url = self._url(key_value)
+        start = getattr(key_value, "offset", None)
+        length = getattr(key_value, "length", None)
+        range_str = None
+        # Range specification are inclusive so getting from offset 500 for 100
+        # bytes will read as bytes=500-599
+        if start is not None or length is not None:
+            if start is None:
+                start = 0
+            if length is None:
+                # Fetch from offset till the end of the file
+                range_str = "bytes=%d-" % start
+            elif length < 0:
+                # Fetch from end; ignore start value here
+                range_str = "bytes=-%d" % (-length)
+            else:
+                # Typical range fetch
+                range_str = "bytes=%d-%d" % (start, start + length - 1)
+        return url, range_str
+
+    def list_paths(self, keys: Optional[Iterable[str]] = None) -> List[S3Object]:
+        """
+        List the next level of paths in S3.
+
+        If multiple keys are specified, listings are done in parallel. The returned
+        S3Objects have `.exists == False` if the path refers to a prefix, not an
+        existing S3 object.
+
+        For instance, if the directory hierarchy is
+        ```
+        a/0.txt
+        a/b/1.txt
+        a/c/2.txt
+        a/d/e/3.txt
+        f/4.txt
+        ```
+        The `list_paths(['a', 'f'])` call returns
+        ```
+        a/0.txt (exists == True)
+        a/b/ (exists == False)
+        a/c/ (exists == False)
+        a/d/ (exists == False)
+        f/4.txt (exists == True)
+        ```
+
+        Parameters
+        ----------
+        keys : Iterable[str], optional
+            List of paths.
+
+        Returns
+        -------
+        List[`S3Object`]
+            S3Objects under the given paths, including prefixes (directories) that
+            do not correspond to leaf objects.
+        """
+
+        def _list(keys):
+            if keys is None:
+                keys = [None]
+            urls = ((self._url(key).rstrip("/") + "/", None) for key in keys)
+            res = self._read_many_files("list", urls)
+            for s3prefix, s3url, size in res:
+                if size:
+                    yield s3prefix, s3url, None, int(size)
+                else:
+                    yield s3prefix, s3url, None, None
+
+        return list(starmap(S3Object, _list(keys)))
+
+    def list_recursive(self, keys: Optional[Iterable[str]] = None) -> List[S3Object]:
+        """
+        List all objects recursively under the given prefixes.
+
+        If multiple keys are specified, listings are done in parallel. All objects
+        returned have `.exists == True` as this call always returns leaf objects.
+
+        For instance, if the directory hierarchy is
+        ```
+        a/0.txt
+        a/b/1.txt
+        a/c/2.txt
+        a/d/e/3.txt
+        f/4.txt
+        ```
+        The `list_paths(['a', 'f'])` call returns
+        ```
+        a/0.txt (exists == True)
+        a/b/1.txt (exists == True)
+        a/c/2.txt (exists == True)
+        a/d/e/3.txt (exists == True)
+        f/4.txt (exists == True)
+        ```
+
+        Parameters
+        ----------
+        keys : Iterable[str], optional
+            List of paths.
+
+        Returns
+        -------
+        List[`S3Object`]
+            S3Objects under the given paths.
+        """
+
+        def _list(keys):
+            if keys is None:
+                keys = [None]
+            res = self._read_many_files(
+                "list", map(self._url_and_range, keys), recursive=True
+            )
+            for s3prefix, s3url, size in res:
+                yield s3prefix, s3url, None, int(size)
 
-    def service_account_name(self, service_account_name):
-        self.payload["serviceAccountName"] = service_account_name
-        return self
+        return list(starmap(S3Object, _list(keys)))
 
-    def retry_strategy(self, times, minutes_between_retries):
-        if times > 0:
-            self.payload["retryStrategy"] = {
-                "retryPolicy": "Always",
-                "limit": times,
-                "backoff": {"duration": "%sm" % minutes_between_retries},
+    def info(self, key: Optional[str] = None, return_missing: bool = False) -> S3Object:
+        """
+        Get metadata about a single object in S3.
+
+        This call makes a single `HEAD` request to S3 which can be
+        much faster than downloading all data with `get`.
+
+        Parameters
+        ----------
+        key : str, optional
+            Object to query. It can be an S3 url or a path suffix.
+        return_missing : bool, default: False
+            If set to True, do not raise an exception for a missing key but
+            return it as an `S3Object` with `.exists == False`.
+
+        Returns
+        -------
+        `S3Object`
+            An S3Object corresponding to the object requested. The object
+            will have `.downloaded == False`.
+        """
+
+        url = self._url(key)
+        src = urlparse(url)
+
+        def _info(s3, tmp):
+            resp = s3.head_object(Bucket=src.netloc, Key=src.path.lstrip('/"'))
+            return {
+                "content_type": resp["ContentType"],
+                "metadata": resp["Metadata"],
+                "size": resp["ContentLength"],
+                "last_modified": get_timestamp(resp["LastModified"]),
             }
-        return self
-
-    def empty_dir_volume(self, name):
-        # Attach an emptyDir volume
-        # https://argoproj.github.io/argo-workflows/empty-dir/
-        if "volumes" not in self.payload:
-            self.payload["volumes"] = []
-        self.payload["volumes"].append({"name": name, "emptyDir": {}})
-        return self
-
-    def node_selectors(self, node_selectors):
-        if "nodeSelector" not in self.payload:
-            self.payload["nodeSelector"] = {}
-        if node_selectors:
-            self.payload["nodeSelector"].update(node_selectors)
-        return self
-
-    def tolerations(self, tolerations):
-        self.payload["tolerations"] = tolerations
-        return self
-
-    def to_json(self):
-        return self.payload
-
-    def __str__(self):
-        return json.dumps(self.payload, indent=4)
-
-
-class Inputs(object):
-    # https://argoproj.github.io/argo-workflows/fields/#inputs
-
-    def __init__(self):
-        tree = lambda: defaultdict(tree)
-        self.payload = tree()
-
-    def parameters(self, parameters):
-        if "parameters" not in self.payload:
-            self.payload["parameters"] = []
-        for parameter in parameters:
-            self.payload["parameters"].append(parameter.to_json())
-        return self
-
-    def to_json(self):
-        return self.payload
-
-    def __str__(self):
-        return json.dumps(self.payload, indent=4)
-
-
-class Outputs(object):
-    # https://argoproj.github.io/argo-workflows/fields/#outputs
-
-    def __init__(self):
-        tree = lambda: defaultdict(tree)
-        self.payload = tree()
-
-    def parameters(self, parameters):
-        if "parameters" not in self.payload:
-            self.payload["parameters"] = []
-        for parameter in parameters:
-            self.payload["parameters"].append(parameter.to_json())
-        return self
-
-    def to_json(self):
-        return self.payload
-
-    def __str__(self):
-        return json.dumps(self.payload, indent=4)
 
+        info_results = None
+        try:
+            _, info_results = self._one_boto_op(_info, url, create_tmp_file=False)
+        except MetaflowS3NotFound:
+            if return_missing:
+                info_results = None
+            else:
+                raise
+        if info_results:
+            return S3Object(
+                self._s3root,
+                url,
+                path=None,
+                size=info_results["size"],
+                content_type=info_results["content_type"],
+                metadata=info_results["metadata"],
+                last_modified=info_results["last_modified"],
+            )
+        return S3Object(self._s3root, url, None)
 
-class Parameter(object):
-    # https://argoproj.github.io/argo-workflows/fields/#parameter
-
-    def __init__(self, name):
-        tree = lambda: defaultdict(tree)
-        self.payload = tree()
-        self.payload["name"] = name
-
-    def value(self, value):
-        self.payload["value"] = value
-        return self
-
-    def default(self, value):
-        self.payload["default"] = value
-        return self
-
-    def valueFrom(self, value_from):
-        self.payload["valueFrom"] = value_from
-        return self
+    def info_many(
+        self, keys: Iterable[str], return_missing: bool = False
+    ) -> List[S3Object]:
+        """
+        Get metadata about many objects in S3 in parallel.
+
+        This call makes a single `HEAD` request to S3 which can be
+        much faster than downloading all data with `get`.
+
+        Parameters
+        ----------
+        keys : Iterable[str]
+            Objects to query. Each key can be an S3 url or a path suffix.
+        return_missing : bool, default: False
+            If set to True, do not raise an exception for a missing key but
+            return it as an `S3Object` with `.exists == False`.
+
+        Returns
+        -------
+        List[`S3Object`]
+            A list of `S3Object`s corresponding to the paths requested. The
+            objects will have `.downloaded == False`.
+        """
 
-    def description(self, description):
-        self.payload["description"] = description
-        return self
+        def _head():
+            from . import s3op
 
-    def to_json(self):
-        return self.payload
+            res = self._read_many_files(
+                "info", map(self._url_and_range, keys), verbose=False, listing=True
+            )
 
-    def __str__(self):
-        return json.dumps(self.payload, indent=4)
+            for s3prefix, s3url, fname in res:
+                if fname:
+                    # We have a metadata file to read from
+                    with open(os.path.join(self._tmpdir, fname), "r") as f:
+                        info = json.load(f)
+                    if info["error"] is not None:
+                        # We have an error, we check if it is a missing file
+                        if info["error"] == s3op.ERROR_URL_NOT_FOUND:
+                            if return_missing:
+                                yield self._s3root, s3url, None
+                            else:
+                                raise MetaflowS3NotFound()
+                        elif info["error"] == s3op.ERROR_URL_ACCESS_DENIED:
+                            raise MetaflowS3AccessDenied()
+                        else:
+                            raise MetaflowS3Exception("Got error: %d" % info["error"])
+                    else:
+                        yield self._s3root, s3url, None, info["size"], info[
+                            "content_type"
+                        ], info["metadata"], None, info["last_modified"]
+                else:
+                    # This should not happen; we should always get a response
+                    # even if it contains an error inside it
+                    raise MetaflowS3Exception("Did not get a response to HEAD")
 
+        return list(starmap(S3Object, _head()))
 
-class DAGTemplate(object):
-    # https://argoproj.github.io/argo-workflows/fields/#dagtemplate
+    def get(
+        self,
+        key: Optional[Union[str, S3GetObject]] = None,
+        return_missing: bool = False,
+        return_info: bool = True,
+    ) -> S3Object:
+        """
+        Get a single object from S3.
+
+        Parameters
+        ----------
+        key : str or `S3GetObject`, optional
+            Object to download. It can be an S3 url, a path suffix, or
+            an `S3GetObject` that defines a range of data to download. If None, or
+            not provided, gets the S3 root.
+        return_missing : bool, default: False
+            If set to True, do not raise an exception for a missing key but
+            return it as an `S3Object` with `.exists == False`.
+        return_info : bool, default: True
+            If set to True, fetch the content-type and user metadata associated
+            with the object at no extra cost, included for symmetry with `get_many`
+
+        Returns
+        -------
+        `S3Object`
+            An S3Object corresponding to the object requested.
+        """
+        url, r = self._url_and_range(key)
+        src = urlparse(url)
+
+        def _download(s3, tmp):
+            if r:
+                resp = s3.get_object(
+                    Bucket=src.netloc, Key=src.path.lstrip("/"), Range=r
+                )
+                # Format is bytes start-end/total; both start and end are inclusive so
+                # a 500 bytes file will be `bytes 0-499/500` for the entire file.
+                range_result = resp["ContentRange"]
+                range_result_match = RANGE_MATCH.match(range_result)
+                if range_result_match is None:
+                    raise RuntimeError(
+                        "Wrong format for ContentRange: %s" % str(range_result)
+                    )
+                range_result = RangeInfo(
+                    int(range_result_match.group("total")),
+                    request_offset=int(range_result_match.group("start")),
+                    request_length=int(range_result_match.group("end"))
+                    - int(range_result_match.group("start"))
+                    + 1,
+                )
+            else:
+                resp = s3.get_object(Bucket=src.netloc, Key=src.path.lstrip("/"))
+                range_result = None
+            sz = resp["ContentLength"]
+            if range_result is None:
+                range_result = RangeInfo(sz, request_offset=0, request_length=sz)
+            if not r and sz > DOWNLOAD_FILE_THRESHOLD:
+                # In this case, it is more efficient to use download_file as it
+                # will download multiple parts in parallel (it does it after
+                # multipart_threshold)
+                s3.download_file(src.netloc, src.path.lstrip("/"), tmp)
+            else:
+                with open(tmp, mode="wb") as t:
+                    read_in_chunks(t, resp["Body"], sz, DOWNLOAD_MAX_CHUNK)
+            if return_info:
+                return {
+                    "content_type": resp["ContentType"],
+                    "metadata": resp["Metadata"],
+                    "range_result": range_result,
+                    "last_modified": get_timestamp(resp["LastModified"]),
+                }
+            return None
 
-    def __init__(self):
-        tree = lambda: defaultdict(tree)
-        self.payload = tree()
+        addl_info = None
+        try:
+            path, addl_info = self._one_boto_op(_download, url)
+        except MetaflowS3NotFound:
+            if return_missing:
+                path = None
+            else:
+                raise
+        if addl_info:
+            return S3Object(
+                self._s3root,
+                url,
+                path,
+                content_type=addl_info["content_type"],
+                metadata=addl_info["metadata"],
+                range_info=addl_info["range_result"],
+                last_modified=addl_info["last_modified"],
+            )
+        return S3Object(self._s3root, url, path)
 
-    def fail_fast(self, fail_fast=True):
-        # https://github.com/argoproj/argo-workflows/issues/1442
-        self.payload["failFast"] = fail_fast
-        return self
+    def get_many(
+        self,
+        keys: Iterable[Union[str, S3GetObject]],
+        return_missing: bool = False,
+        return_info: bool = True,
+    ) -> List[S3Object]:
+        """
+        Get many objects from S3 in parallel.
+
+        Parameters
+        ----------
+        keys : Iterable[str or `S3GetObject`]
+            Objects to download. Each object can be an S3 url, a path suffix, or
+            an `S3GetObject` that defines a range of data to download.
+        return_missing : bool, default: False
+            If set to True, do not raise an exception for a missing key but
+            return it as an `S3Object` with `.exists == False`.
+        return_info : bool, default: True
+            If set to True, fetch the content-type and user metadata associated
+            with the object at no extra cost, included for symmetry with `get_many`.
+
+        Returns
+        -------
+        List[`S3Object`]
+            S3Objects corresponding to the objects requested.
+        """
+
+        def _get():
+            res = self._read_many_files(
+                "get",
+                map(self._url_and_range, keys),
+                allow_missing=return_missing,
+                verify=True,
+                verbose=False,
+                info=return_info,
+                listing=True,
+            )
 
-    def tasks(self, tasks):
-        if "tasks" not in self.payload:
-            self.payload["tasks"] = []
-        for task in tasks:
-            self.payload["tasks"].append(task.to_json())
-        return self
+            for s3prefix, s3url, fname in res:
+                if return_info:
+                    if fname:
+                        # We have a metadata file to read from
+                        with open(
+                            os.path.join(self._tmpdir, "%s_meta" % fname), "r"
+                        ) as f:
+                            info = json.load(f)
+                        range_info = info.get("range_result")
+                        if range_info:
+                            range_info = RangeInfo(
+                                range_info["total"],
+                                request_offset=range_info["start"],
+                                request_length=range_info["end"]
+                                - range_info["start"]
+                                + 1,
+                            )
+                        yield self._s3root, s3url, os.path.join(
+                            self._tmpdir, fname
+                        ), None, info["content_type"], info[
+                            "metadata"
+                        ], range_info, info[
+                            "last_modified"
+                        ]
+                    else:
+                        yield self._s3root, s3prefix, None
+                else:
+                    if fname:
+                        yield self._s3root, s3url, os.path.join(self._tmpdir, fname)
+                    else:
+                        # missing entries per return_missing=True
+                        yield self._s3root, s3prefix, None
+
+        return list(starmap(S3Object, _get()))
+
+    def get_recursive(
+        self, keys: Iterable[str], return_info: bool = False
+    ) -> List[S3Object]:
+        """
+        Get many objects from S3 recursively in parallel.
+
+        Parameters
+        ----------
+        keys : Iterable[str]
+            Prefixes to download recursively. Each prefix can be an S3 url or a path suffix
+            which define the root prefix under which all objects are downloaded.
+        return_info : bool, default: False
+            If set to True, fetch the content-type and user metadata associated
+            with the object.
+
+        Returns
+        -------
+        List[`S3Object`]
+            S3Objects stored under the given prefixes.
+        """
+
+        def _get():
+            res = self._read_many_files(
+                "get",
+                map(self._url_and_range, keys),
+                recursive=True,
+                verify=True,
+                verbose=False,
+                info=return_info,
+                listing=True,
+            )
 
-    def to_json(self):
-        return self.payload
+            for s3prefix, s3url, fname in res:
+                if return_info:
+                    # We have a metadata file to read from
+                    with open(os.path.join(self._tmpdir, "%s_meta" % fname), "r") as f:
+                        info = json.load(f)
+                    range_info = info.get("range_result")
+                    if range_info:
+                        range_info = RangeInfo(
+                            range_info["total"],
+                            request_offset=range_info["start"],
+                            request_length=range_info["end"] - range_info["start"] + 1,
+                        )
+                    yield self._s3root, s3url, os.path.join(
+                        self._tmpdir, fname
+                    ), None, info["content_type"], info["metadata"], range_info, info[
+                        "last_modified"
+                    ]
+                else:
+                    yield s3prefix, s3url, os.path.join(self._tmpdir, fname)
 
-    def __str__(self):
-        return json.dumps(self.payload, indent=4)
+        return list(starmap(S3Object, _get()))
 
+    def get_all(self, return_info: bool = False) -> List[S3Object]:
+        """
+        Get all objects under the prefix set in the `S3` constructor.
+
+        This method requires that the `S3` object is initialized either with `run` or
+        `s3root`.
+
+        Parameters
+        ----------
+        return_info : bool, default: False
+            If set to True, fetch the content-type and user metadata associated
+            with the object.
+
+        Returns
+        -------
+        Iterable[`S3Object`]
+            S3Objects stored under the main prefix.
+        """
+
+        if self._s3root is None:
+            raise MetaflowS3URLException(
+                "Can't get_all() when S3 is initialized without a prefix"
+            )
+        else:
+            return self.get_recursive([None], return_info)
 
-class DAGTask(object):
-    # https://argoproj.github.io/argo-workflows/fields/#dagtask
+    def put(
+        self,
+        key: Union[str, S3PutObject],
+        obj: PutValue,
+        overwrite: bool = True,
+        content_type: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+    ) -> str:
+        """
+        Upload a single object to S3.
+
+        Parameters
+        ----------
+        key : str or `S3PutObject`
+            Object path. It can be an S3 url or a path suffix.
+        obj : bytes or str
+            An object to store in S3. Strings are converted to UTF-8 encoding.
+        overwrite : bool, default: True
+            Overwrite the object if it exists. If set to False, the operation
+            succeeds without uploading anything if the key already exists.
+        content_type : str, optional
+            Optional MIME type for the object.
+        metadata : Dict, optional
+            A JSON-encodable dictionary of additional headers to be stored
+            as metadata with the object.
+
+        Returns
+        -------
+        str
+            URL of the object stored.
+        """
+
+        if isinstance(obj, (RawIOBase, BufferedIOBase)):
+            if not obj.readable() or not obj.seekable():
+                raise MetaflowS3InvalidObject(
+                    "Object corresponding to the key '%s' is not readable or seekable"
+                    % key
+                )
+            blob = obj
+        else:
+            if not is_stringish(obj):
+                raise MetaflowS3InvalidObject(
+                    "Object corresponding to the key '%s' is not a string "
+                    "or a bytes object." % key
+                )
+            blob = to_fileobj(obj)
+        # We override the close functionality to prevent closing of the
+        # file if it is used multiple times when uploading (since upload_fileobj
+        # will/may close it on failure)
+        real_close = blob.close
+        blob.close = lambda: None
+
+        url = self._url(key)
+        src = urlparse(url)
+        extra_args = None
+        if content_type or metadata:
+            extra_args = {}
+            if content_type:
+                extra_args["ContentType"] = content_type
+            if metadata:
+                extra_args["Metadata"] = {
+                    "metaflow-user-attributes": json.dumps(metadata)
+                }
 
-    def __init__(self, name):
-        tree = lambda: defaultdict(tree)
-        self.payload = tree()
-        self.payload["name"] = name
+        def _upload(s3, _):
+            # We make sure we are at the beginning in case we are retrying
+            blob.seek(0)
+            s3.upload_fileobj(
+                blob, src.netloc, src.path.lstrip("/"), ExtraArgs=extra_args
+            )
 
-    def arguments(self, arguments):
-        self.payload["arguments"] = arguments.to_json()
-        return self
+        if overwrite:
+            self._one_boto_op(_upload, url, create_tmp_file=False)
+            real_close()
+            return url
+        else:
 
-    def dependencies(self, dependencies):
-        self.payload["dependencies"] = dependencies
-        return self
+            def _head(s3, _):
+                s3.head_object(Bucket=src.netloc, Key=src.path.lstrip("/"))
 
-    def template(self, template):
-        # Template reference
-        self.payload["template"] = template
-        return self
+            try:
+                self._one_boto_op(_head, url, create_tmp_file=False)
+            except MetaflowS3NotFound:
+                self._one_boto_op(_upload, url, create_tmp_file=False)
+            finally:
+                real_close()
+            return url
 
-    def inline(self, template):
-        # We could have inlined the template here but
-        # https://github.com/argoproj/argo-workflows/issues/7432 prevents us for now.
-        self.payload["inline"] = template.to_json()
-        return self
+    def put_many(
+        self,
+        key_objs: List[Union[Tuple[str, PutValue], S3PutObject]],
+        overwrite: bool = True,
+    ) -> List[Tuple[str, str]]:
+        """
+        Upload many objects to S3.
+
+        Each object to be uploaded can be specified in two ways:
+
+        1. As a `(key, obj)` tuple where `key` is a string specifying
+           the path and `obj` is a string or a bytes object.
+
+        2. As a `S3PutObject` which contains additional metadata to be
+           stored with the object.
+
+        Parameters
+        ----------
+        key_objs : List[(str, str) or `S3PutObject`]
+            List of key-object pairs to upload.
+        overwrite : bool, default : True
+            Overwrite the object if it exists. If set to False, the operation
+            succeeds without uploading anything if the key already exists.
+
+        Returns
+        -------
+        List[(str, str)]
+            List of `(key, url)` pairs corresponding to the objects uploaded.
+        """
+
+        def _store():
+            for key_obj in key_objs:
+                if isinstance(key_obj, tuple):
+                    key = key_obj[0]
+                    obj = key_obj[1]
+                else:
+                    key = key_obj.key
+                    obj = key_obj.value
+                store_info = {
+                    "key": key,
+                    "content_type": getattr(key_obj, "content_type", None),
+                }
+                metadata = getattr(key_obj, "metadata", None)
+                if metadata:
+                    store_info["metadata"] = {
+                        "metaflow-user-attributes": json.dumps(metadata)
+                    }
+                if isinstance(obj, (RawIOBase, BufferedIOBase)):
+                    if not obj.readable() or not obj.seekable():
+                        raise MetaflowS3InvalidObject(
+                            "Object corresponding to the key '%s' is not readable or seekable"
+                            % key
+                        )
+                else:
+                    if not is_stringish(obj):
+                        raise MetaflowS3InvalidObject(
+                            "Object corresponding to the key '%s' is not a string "
+                            "or a bytes object." % key
+                        )
+                    obj = to_fileobj(obj)
+                with NamedTemporaryFile(
+                    dir=self._tmpdir,
+                    delete=False,
+                    mode="wb",
+                    prefix="metaflow.s3.put_many.",
+                ) as tmp:
+                    tmp.write(obj.read())
+                    tmp.close()
+                    yield tmp.name, self._url(key), store_info
 
-    def with_param(self, with_param):
-        self.payload["withParam"] = with_param
-        return self
+        return self._put_many_files(_store(), overwrite)
 
-    def to_json(self):
-        return self.payload
+    def put_files(
+        self,
+        key_paths: List[Union[Tuple[str, PutValue], S3PutObject]],
+        overwrite: bool = True,
+    ) -> List[Tuple[str, str]]:
+        """
+        Upload many local files to S3.
+
+        Each file to be uploaded can be specified in two ways:
+
+        1. As a `(key, path)` tuple where `key` is a string specifying
+           the S3 path and `path` is the path to a local file.
+
+        2. As a `S3PutObject` which contains additional metadata to be
+           stored with the file.
+
+        Parameters
+        ----------
+        key_paths : List[(str, str) or `S3PutObject`]
+            List of files to upload.
+        overwrite : bool, default: True
+            Overwrite the object if it exists. If set to False, the operation
+            succeeds without uploading anything if the key already exists.
+
+        Returns
+        -------
+        List[(str, str)]
+            List of `(key, url)` pairs corresponding to the files uploaded.
+        """
+
+        def _check():
+            for key_path in key_paths:
+                if isinstance(key_path, tuple):
+                    key = key_path[0]
+                    path = key_path[1]
+                else:
+                    key = key_path.key
+                    path = key_path.path
+                store_info = {
+                    "key": key,
+                    "content_type": getattr(key_path, "content_type", None),
+                }
+                metadata = getattr(key_path, "metadata", None)
+                if metadata:
+                    store_info["metadata"] = {
+                        "metaflow-user-attributes": json.dumps(metadata)
+                    }
+                if not os.path.exists(path):
+                    raise MetaflowS3NotFound("Local file not found: %s" % path)
+                yield path, self._url(key), store_info
+
+        return self._put_many_files(_check(), overwrite)
+
+    def _one_boto_op(self, op, url, create_tmp_file=True):
+        error = ""
+        for i in range(S3_RETRY_COUNT + 1):
+            tmp = None
+            if create_tmp_file:
+                tmp = NamedTemporaryFile(
+                    dir=self._tmpdir, prefix="metaflow.s3.one_file.", delete=False
+                )
+            try:
+                side_results = op(self._s3_client.client, tmp.name if tmp else None)
+                return tmp.name if tmp else None, side_results
+            except self._s3_client.error as err:
+                from . import s3op
+
+                error_code = s3op.normalize_client_error(err)
+                if error_code == 404:
+                    raise MetaflowS3NotFound(url)
+                elif error_code == 403:
+                    raise MetaflowS3AccessDenied(url)
+                elif error_code == 416:
+                    raise MetaflowS3InvalidRange(err)
+                elif error_code == "NoSuchBucket":
+                    raise MetaflowS3URLException("Specified S3 bucket doesn't exist.")
+                error = str(err)
+            except Exception as ex:
+                # TODO specific error message for out of disk space
+                error = str(ex)
+            if tmp:
+                os.unlink(tmp.name)
+            self._s3_client.reset_client()
+            # only sleep if retries > 0
+            if S3_RETRY_COUNT > 0:
+                self._jitter_sleep(i)
+        raise MetaflowS3Exception(
+            "S3 operation failed.\n" "Key requested: %s\n" "Error: %s" % (url, error)
+        )
 
-    def __str__(self):
-        return json.dumps(self.payload, indent=4)
+    # add some jitter to make sure retries are not synchronized
+    def _jitter_sleep(self, trynum, multiplier=2):
+        interval = multiplier**trynum + random.randint(0, 10)
+        time.sleep(interval)
+
+    # NOTE: re: _read_many_files and _put_many_files
+    # All file IO is through binary files - we write bytes, we read
+    # bytes. All inputs and outputs from these functions are Unicode.
+    # Conversion between bytes and unicode is done through
+    # and url_unquote.
+    def _read_many_files(self, op, prefixes_and_ranges, **options):
+        prefixes_and_ranges = list(prefixes_and_ranges)
+        with NamedTemporaryFile(
+            dir=self._tmpdir,
+            mode="wb",
+            delete=not debug.s3client,
+            prefix="metaflow.s3.inputs.",
+        ) as inputfile:
+            inputfile.write(
+                b"\n".join(
+                    [
+                        b" ".join([url_quote(prefix)] + ([url_quote(r)] if r else []))
+                        for prefix, r in prefixes_and_ranges
+                    ]
+                )
+            )
+            inputfile.flush()
+            stdout_lines, stderr = self._s3op_with_retries(
+                op, inputs=inputfile.name, **options
+            )
+            if stderr:
+                raise MetaflowS3Exception(
+                    "Getting S3 files failed.\n"
+                    "First prefix requested: %s\n"
+                    "Error: %s" % (prefixes_and_ranges[0], stderr)
+                )
+            else:
+                for line in stdout_lines:
+                    yield tuple(map(url_unquote, line.strip(b"\n").split(b" ")))
 
+    def _put_many_files(self, url_info, overwrite):
+        url_info = list(url_info)
+        url_dicts = [
+            dict(
+                chain([("local", os.path.realpath(local)), ("url", url)], info.items())
+            )
+            for local, url, info in url_info
+        ]
 
-class Arguments(object):
-    # https://argoproj.github.io/argo-workflows/fields/#arguments
+        with NamedTemporaryFile(
+            dir=self._tmpdir,
+            mode="wb",
+            delete=not debug.s3client,
+            prefix="metaflow.s3.put_inputs.",
+        ) as inputfile:
+            lines = [to_bytes(json.dumps(x)) for x in url_dicts]
+            inputfile.write(b"\n".join(lines))
+            inputfile.flush()
+            stdout_lines, stderr = self._s3op_with_retries(
+                "put",
+                inputs=inputfile.name,
+                verbose=False,
+                overwrite=overwrite,
+                listing=True,
+            )
+            if stderr:
+                raise MetaflowS3Exception(
+                    "Uploading S3 files failed.\n"
+                    "First key: %s\n"
+                    "Error: %s" % (url_info[0][2]["key"], stderr)
+                )
+            else:
+                urls = set()
+                for line in stdout_lines:
+                    url, _, _ = map(url_unquote, line.strip(b"\n").split(b" "))
+                    urls.add(url)
+                return [(info["key"], url) for _, url, info in url_info if url in urls]
+
+    def _s3op_with_retries(self, mode, **options):
+        from . import s3op
+
+        # High level note on what this function does:
+        #  - perform s3op (which calls s3op.py in a subprocess to parallelize the
+        #    operation). Typically this operation has several inputs (for example,
+        #    multiple files to get or put)
+        #  - the result of this operation can be either:
+        #    - a known permanent failure (access denied for example) in which case we
+        #      return this failure.
+        #    - a known transient failure (SlowDown for example) in which case we will
+        #      retry *only* the inputs that have this transient failure.
+        #    - an unknown failure (something went wrong but we cannot say if it was
+        #      a known permanent failure or something else). In this case, we retry
+        #      the operation completely.
+        #
+        # There are therefore two retry counts:
+        #  - the transient failure retry count: how many times do we try on known
+        #    transient errors
+        #  - the top-level retry count: how many times do we try on unknown failures
+        #
+        # Note that, if the operation runs out of transient failure retries, it will
+        # count as an "unknown" failure (ie: it will be retried according to the
+        # outer top-level retry count). In other words, you can potentially have
+        # transient_retry_count * retry_count tries).
+        # Finally, if on transient failures, we make NO progress (ie: no input is
+        # successfully processed), that counts as an "unknown" failure.
+        cmdline = [sys.executable, os.path.abspath(s3op.__file__), mode]
+        recursive_get = False
+        for key, value in options.items():
+            key = key.replace("_", "-")
+            if isinstance(value, bool):
+                if value:
+                    if mode == "get" and key == "recursive":
+                        # We make a note of this because for transient retries, we
+                        # don't pass the recursive flag since we already did all the
+                        # listing we needed
+                        recursive_get = True
+                    else:
+                        cmdline.append("--%s" % key)
+                else:
+                    cmdline.append("--no-%s" % key)
+            elif key == "inputs":
+                base_input_filename = value
+            else:
+                cmdline.extend(("--%s" % key, value))
+        if self._s3_role is not None:
+            cmdline.extend(("--s3role", self._s3_role))
+        if self._s3_session_vars is not None:
+            cmdline.extend(("--s3sessionvars", json.dumps(self._s3_session_vars)))
+        if self._s3_client_params is not None:
+            cmdline.extend(("--s3clientparams", json.dumps(self._s3_client_params)))
+
+        def _inject_failure_rate():
+            # list mode does not do retries on transient failures (there is no
+            # SlowDown handling) so we never inject a failure rate
+            if mode == "list":
+                return 0
+            # Otherwise, we cap the failure rate at 90%
+            return min(90, self._s3_inject_failures)
+
+        retry_count = 0  # Number of retries (excluding transient failures)
+        transient_retry_count = 0  # Number of transient retries (per top-level retry)
+        inject_failures = _inject_failure_rate()
+        out_lines = []  # List to contain the lines returned by _s3op_with_retries
+        pending_retries = (
+            []
+        )  # Inputs that need to be retried due to a transient failure
+        loop_count = 0
+        last_ok_count = 0  # Number of inputs that were successful in the last try
+        total_ok_count = 0  # Total number of OK inputs
+
+        def _reset():
+            nonlocal transient_retry_count, inject_failures, out_lines, pending_retries
+            nonlocal loop_count, last_ok_count, total_ok_count
+            transient_retry_count = 0
+            inject_failures = _inject_failure_rate()
+            if mode != "put":
+                # For put, even after retries, we keep around whatever we already
+                # uploaded. This is because uploading with overwrite=False is not
+                # an idempotent operation and so some files could be uploaded during
+                # the first try which we should report back.
+                out_lines = []
+            pending_retries = []
+            loop_count = 0
+            last_ok_count = 0
+            total_ok_count = 0  # Reset to zero even if we keep out_lines
+
+        def _update_out_lines(out_lines, ok_lines, resize=False):
+            if resize:
+                # This is the first time around; we make the list big enough. Typically,
+                # there is nothing in out_lines but in some cases (a retry after a
+                # partial result), there may be stuff in it
+                out_lines.extend([None] * (len(ok_lines) - len(out_lines)))
+            for l in ok_lines:
+                idx, rest = l.split(b" ", maxsplit=1)
+                if rest.decode(encoding="utf-8") != TRANSIENT_RETRY_LINE_CONTENT:
+                    # Update the proper location in the out_lines array; we maintain
+                    # position as if transient retries did not exist. This
+                    # makes sure that order is respected even in the presence of
+                    # transient retries.
+                    out_lines[int(idx.decode(encoding="utf-8"))] = rest
+
+        def try_s3_op(last_ok_count, pending_retries, out_lines, inject_failures):
+            # NOTE: Make sure to update pending_retries and out_lines in place
+            addl_cmdline = []
+            if len(pending_retries) == 0 and recursive_get:
+                # First time around (or after a fatal failure)
+                addl_cmdline = ["--recursive"]
+            with NamedTemporaryFile(
+                dir=self._tmpdir,
+                mode="wb+",
+                delete=not debug.s3client,
+                prefix="metaflow.s3op.stderr.",
+            ) as stderr:
+                with NamedTemporaryFile(
+                    dir=self._tmpdir,
+                    mode="wb",
+                    delete=not debug.s3client,
+                    prefix="metaflow.s3op.transientretry.",
+                ) as tmp_input:
+                    if len(pending_retries) > 0:
+                        # We try a little bit more than the previous success (to still
+                        # be aggressive but not too much). If there is a lot of
+                        # transient errors and we are having issues pushing through
+                        # things, this will shrink more and more until we are doing a
+                        # single operation at a time. If things start going better, it
+                        # will increase by 20% every round.
+                        max_count = min(int(last_ok_count * 1.2), len(pending_retries))
+                        tmp_input.writelines(pending_retries[:max_count])
+                        tmp_input.flush()
+                        debug.s3client_exec(
+                            "Have %d pending; succeeded in %d => trying for %d and "
+                            "leaving %d for the next round"
+                            % (
+                                len(pending_retries),
+                                last_ok_count,
+                                max_count,
+                                len(pending_retries) - max_count,
+                            )
+                        )
+                        del pending_retries[:max_count]
 
-    def __init__(self):
-        tree = lambda: defaultdict(tree)
-        self.payload = tree()
+                        input_filename = tmp_input.name
+                    else:
+                        input_filename = base_input_filename
+
+                    addl_cmdline.extend(["--inputs", input_filename])
+
+                    # Check if we want to inject failures (for testing)
+                    if inject_failures > 0:
+                        addl_cmdline.extend(["--inject-failure", str(inject_failures)])
+                        # Logic here is to have higher and lower failure rates to try to
+                        # exercise as much of the code as possible. The failure rate
+                        # trends towards 0.
+                        if loop_count % 2 == 0:
+                            inject_failures = int(inject_failures / 3)
+                        else:
+                            # We cap at 90 (and not 100) for injection of failures to
+                            # reduce the likelihood of having flaky test. If the
+                            # failure injection rate is too high, this can cause actual
+                            # retries more often and then lead to too many actual
+                            # retries
+                            inject_failures = min(90, int(inject_failures * 1.5))
+                    try:
+                        debug.s3client_exec(cmdline + addl_cmdline)
+                        # Run the operation.
+                        stdout = subprocess.check_output(
+                            cmdline + addl_cmdline,
+                            cwd=self._tmpdir,
+                            stderr=stderr.file,
+                        )
+                        # Here we did not have any error -- transient or otherwise.
+                        ok_lines = stdout.splitlines()
+                        _update_out_lines(out_lines, ok_lines, resize=loop_count == 0)
+                        return (len(ok_lines), 0, inject_failures, None)
+                    except subprocess.CalledProcessError as ex:
+                        if ex.returncode == s3op.ERROR_TRANSIENT:
+                            # In this special case, we failed transiently on *some* of
+                            # the files but not necessarily all. This is typically
+                            # caused by limits on the number of operations that can
+                            # occur per second or some other temporary limitation.
+                            # We will retry only those that we failed on and we will not
+                            # count this as a retry *unless* we are making no forward
+                            # progress. In effect, we consider that as long as *some*
+                            # operations are going through, we should just keep going as
+                            # if it was a single operation.
+                            ok_lines = ex.stdout.splitlines()
+                            stderr.seek(0)
+                            do_output = False
+                            retry_lines = []
+                            for l in stderr:
+                                if do_output:
+                                    retry_lines.append(l)
+                                    continue
+                                if (
+                                    l.decode(encoding="utf-8")
+                                    == "%s\n" % TRANSIENT_RETRY_START_LINE
+                                ):
+                                    # Look for a special marker as the start of the
+                                    # "failed inputs that need to be retried"
+                                    do_output = True
+                            stderr.seek(0)
+                            if do_output is False:
+                                return (
+                                    0,
+                                    0,
+                                    inject_failures,
+                                    "Could not find inputs to retry",
+                                )
+                            else:
+                                _update_out_lines(
+                                    out_lines, ok_lines, resize=loop_count == 0
+                                )
+                                pending_retries.extend(retry_lines)
 
-    def parameters(self, parameters):
-        if "parameters" not in self.payload:
-            self.payload["parameters"] = []
-        for parameter in parameters:
-            self.payload["parameters"].append(parameter.to_json())
-        return self
+                                return (
+                                    len(ok_lines),
+                                    len(retry_lines),
+                                    inject_failures,
+                                    None,
+                                )
 
-    def to_json(self):
-        return self.payload
+                        # Here, this is a "normal" failure that we need to send back up.
+                        # These failures are not retried.
+                        stderr.seek(0)
+                        err_out = stderr.read().decode("utf-8", errors="replace")
+                        stderr.seek(0)
+                        if ex.returncode == s3op.ERROR_URL_NOT_FOUND:
+                            raise MetaflowS3NotFound(err_out)
+                        elif ex.returncode == s3op.ERROR_URL_ACCESS_DENIED:
+                            raise MetaflowS3AccessDenied(err_out)
+                        elif ex.returncode == s3op.ERROR_INVALID_RANGE:
+                            raise MetaflowS3InvalidRange(err_out)
+
+                        # Here, this is some other error that we will retry. We still
+                        # update the successful lines
+                        ok_lines = ex.stdout.splitlines()
+                        _update_out_lines(out_lines, ok_lines, resize=loop_count == 0)
+                        return 0, 0, inject_failures, err_out
 
-    def __str__(self):
-        return json.dumps(self.payload, indent=4)
+        while retry_count <= S3_RETRY_COUNT:
+            (
+                last_ok_count,
+                last_retry_count,
+                inject_failures,
+                err_out,
+            ) = try_s3_op(last_ok_count, pending_retries, out_lines, inject_failures)
+            if err_out or (
+                last_retry_count != 0
+                and (
+                    last_ok_count == 0
+                    or transient_retry_count > S3_TRANSIENT_RETRY_COUNT
+                )
+            ):
+                # We had a fatal failure (err_out is not None)
+                # or we made no progress (last_ok_count is 0)
+                # or we are out of transient retries
+                # so we will restart from scratch (being very conservative)
+                retry_count += 1
+                err_msg = err_out
+                if err_msg is None and last_ok_count == 0:
+                    err_msg = "No progress"
+                if err_msg is None:
+                    err_msg = "Too many transient errors"
+                print(
+                    "S3 non-transient error (attempt #%d): %s" % (retry_count, err_msg)
+                )
+                _reset()
+                if retry_count <= S3_RETRY_COUNT:
+                    self._jitter_sleep(retry_count)
+                continue
+            elif last_retry_count != 0:
+                # During our last try, we did not manage to process everything we wanted
+                # due to a transient failure so we try again.
+                transient_retry_count += 1
+                total_ok_count += last_ok_count
+                print(
+                    "Transient S3 failure (attempt #%d) -- total success: %d, "
+                    "last attempt %d/%d -- remaining: %d"
+                    % (
+                        transient_retry_count,
+                        total_ok_count,
+                        last_ok_count,
+                        last_ok_count + last_retry_count,
+                        len(pending_retries),
+                    )
+                )
+                if inject_failures == 0:
+                    # Don't sleep when we are "faking" the failures
+                    self._jitter_sleep(transient_retry_count)
+
+            loop_count += 1
+            # If we have no more things to try, we break out of the loop.
+            if len(pending_retries) == 0:
+                break
+
+        # At this point, we check out_lines; strip None which can happen for puts that
+        # didn't upload files
+        return [o for o in out_lines if o is not None], err_out
```

### Comparing `metaflow-2.8.3/metaflow/plugins/argo/argo_workflows_cli.py` & `metaflow-2.8.4/metaflow/plugins/argo/argo_workflows_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 import re
 import sys
 from distutils.version import LooseVersion
 from hashlib import sha1
 
 from metaflow import JSONType, current, decorators, parameters
 from metaflow._vendor import click
-from metaflow.metaflow_config import SERVICE_VERSION_CHECK, UI_URL
 from metaflow.exception import MetaflowException, MetaflowInternalError
+from metaflow.metaflow_config import SERVICE_VERSION_CHECK, UI_URL
 from metaflow.package import MetaflowPackage
-from metaflow.plugins.environment_decorator import EnvironmentDecorator
-from metaflow.plugins.kubernetes.kubernetes_decorator import KubernetesDecorator
 
 # TODO: Move production_token to utils
 from metaflow.plugins.aws.step_functions.production_token import (
     load_token,
     new_token,
     store_token,
 )
-from metaflow.util import get_username, to_bytes, to_unicode
+from metaflow.plugins.environment_decorator import EnvironmentDecorator
+from metaflow.plugins.kubernetes.kubernetes_decorator import KubernetesDecorator
 from metaflow.tagging_util import validate_tags
+from metaflow.util import get_username, to_bytes, to_unicode
 
 from .argo_workflows import ArgoWorkflows
 
 VALID_NAME = re.compile("^[a-z0-9]([a-z0-9\.\-]*[a-z0-9])?$")
 
 
 class IncorrectProductionToken(MetaflowException):
@@ -51,15 +51,15 @@
 
 @cli.group(help="Commands related to Argo Workflows.")
 @click.option(
     "--name",
     default=None,
     type=str,
     help="Argo Workflow name. The flow name is used instead if "
-    "this option is not specified",
+    "this option is not specified.",
 )
 @click.pass_obj
 def argo_workflows(obj, name=None):
     check_python_version(obj)
     obj.check(obj.graph, obj.flow, obj.environment, pylint=obj.pylint)
     (
         obj.workflow_name,
@@ -125,26 +125,33 @@
     "--workflow-priority",
     default=None,
     type=int,
     help="Workflow priority as an integer. Workflows with higher priority "
     "are processed first if Argo Workflows controller is configured to process limited "
     "number of workflows in parallel",
 )
+@click.option(
+    "--auto-emit-argo-events/--no-auto-emit-argo-events",
+    default=False,  # TODO: Default to a value from config
+    show_default=True,
+    help="Auto emits Argo Events when the run completes successfully",
+)
 @click.pass_obj
 def create(
     obj,
     tags=None,
     user_namespace=None,
     only_json=False,
     authorize=None,
     generate_new_token=False,
     given_token=None,
     max_workers=None,
     workflow_timeout=None,
     workflow_priority=None,
+    auto_emit_argo_events=False,
 ):
     validate_tags(tags)
 
     obj.echo("Deploying *%s* to Argo Workflows..." % obj.workflow_name, bold=True)
 
     if SERVICE_VERSION_CHECK:
         # TODO: Consider dispelling with this check since it's been 2 years since the
@@ -168,18 +175,20 @@
         token,
         obj.workflow_name,
         tags,
         user_namespace,
         max_workers,
         workflow_timeout,
         workflow_priority,
+        auto_emit_argo_events,
     )
 
     if only_json:
         obj.echo_always(str(flow), err=False, no_bold=True)
+        # TODO: Support echo-ing Argo Events Sensor template
     else:
         flow.deploy()
         obj.echo(
             "Workflow *{workflow_name}* "
             "for flow *{name}* pushed to "
             "Argo Workflows successfully.\n".format(
                 workflow_name=obj.workflow_name, name=current.flow_name
@@ -192,14 +201,16 @@
                 "due to Kubernetes naming conventions\non Argo Workflows. The "
                 "original flow name is stored in the workflow annotation.\n"
             )
         flow.schedule()
         obj.echo("What will trigger execution of the workflow:", bold=True)
         obj.echo(flow.trigger_explanation(), indent=True)
 
+        # TODO: Print events emitted by execution of this flow
+
         # response = ArgoWorkflows.trigger(obj.workflow_name)
         # run_id = "argo-" + response["metadata"]["name"]
 
         # obj.echo(
         #     "Workflow *{name}* triggered on Argo Workflows "
         #     "(run-id *{run_id}*).".format(name=obj.workflow_name, run_id=run_id),
         #     bold=True,
@@ -321,15 +332,23 @@
             )
             obj._is_workflow_name_modified = True
 
     return workflow_name, token_prefix.lower(), is_project
 
 
 def make_flow(
-    obj, token, name, tags, namespace, max_workers, workflow_timeout, workflow_priority
+    obj,
+    token,
+    name,
+    tags,
+    namespace,
+    max_workers,
+    workflow_timeout,
+    workflow_priority,
+    auto_emit_argo_events,
 ):
     # TODO: Make this check less specific to Amazon S3 as we introduce
     #       support for more cloud object stores.
     if obj.flow_datastore.TYPE not in ("azure", "gs", "s3"):
         raise MetaflowException(
             "Argo Workflows requires --datastore=s3 or --datastore=azure or --datastore=gs"
         )
@@ -367,14 +386,15 @@
         obj.monitor,
         tags=tags,
         namespace=namespace,
         max_workers=max_workers,
         username=get_username(),
         workflow_timeout=workflow_timeout,
         workflow_priority=workflow_priority,
+        auto_emit_argo_events=auto_emit_argo_events,
     )
 
 
 # TODO: Unify this method with the one in step_functions_cli.py
 def resolve_token(
     name, token_prefix, obj, authorize, given_token, generate_new_token, is_project
 ):
```

### Comparing `metaflow-2.8.3/metaflow/plugins/argo/process_input_paths.py` & `metaflow-2.8.4/metaflow/plugins/argo/process_input_paths.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import sys
 import re
+import sys
 
 
 def process_input_paths(input_paths):
     # Convert Argo Workflows provided input-paths string to something that Metaflow
     # understands
     #
     # flow/step/[{task-id:foo},{task-id:bar}] => flow/step/:foo,bar
```

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/aws_client.py` & `metaflow-2.8.4/metaflow/plugins/aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/aws_utils.py` & `metaflow-2.8.4/metaflow/plugins/aws/aws_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/batch/batch.py` & `metaflow-2.8.4/metaflow/plugins/aws/batch/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
             )
         if AWS_SECRETS_MANAGER_DEFAULT_REGION is not None:
             job.environment_variable(
                 "METAFLOW_AWS_SECRETS_MANAGER_DEFAULT_REGION",
                 AWS_SECRETS_MANAGER_DEFAULT_REGION,
             )
 
-        tmpfs_enabled = use_tmpfs or (tmpfs_size and use_tmpfs is None)
+        tmpfs_enabled = use_tmpfs or (tmpfs_size and not use_tmpfs)
 
         if tmpfs_enabled and tmpfs_tempdir:
             job.environment_variable("METAFLOW_TEMPDIR", tmpfs_path)
 
         # Skip setting METAFLOW_DATASTORE_SYSROOT_LOCAL because metadata sync between the local user
         # instance and the remote AWS Batch instance assumes metadata is stored in DATASTORE_LOCAL_DIR
         # on the remote AWS Batch instance; this happens when METAFLOW_DATASTORE_SYSROOT_LOCAL
```

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/batch/batch_cli.py` & `metaflow-2.8.4/metaflow/plugins/aws/batch/batch_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/batch/batch_client.py` & `metaflow-2.8.4/metaflow/plugins/aws/batch/batch_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
                 job_definition["containerProperties"]["volumes"].append(
                     {"name": name, "host": {"sourcePath": host_path}}
                 )
                 job_definition["containerProperties"]["mountPoints"].append(
                     {"sourceVolume": name, "containerPath": host_path}
                 )
 
-        if use_tmpfs or (tmpfs_size and use_tmpfs is None):
+        if use_tmpfs or (tmpfs_size and not use_tmpfs):
             if tmpfs_size:
                 if not (isinstance(tmpfs_size, (int, unicode, basestring))):
                     raise BatchJobException(
                         "Invalid tmpfs value: ({}) (should be 0 or greater)".format(
                             tmpfs_size
                         )
                     )
```

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/batch/batch_decorator.py` & `metaflow-2.8.4/metaflow/plugins/aws/batch/batch_decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,15 @@
         # task_finished may run locally if fallback is activated for @catch
         # decorator.
         if "AWS_BATCH_JOB_ID" in os.environ:
             # If `local` metadata is configured, we would need to copy task
             # execution metadata from the AWS Batch container to user's
             # local file system after the user code has finished execution.
             # This happens via datastore as a communication bridge.
-            if self.metadata.TYPE == "local":
+            if hasattr(self, "metadata") and self.metadata.TYPE == "local":
                 # Note that the datastore is *always* Amazon S3 (see
                 # runtime_task_created function).
                 sync_local_metadata_to_datastore(
                     DATASTORE_LOCAL_DIR, self.task_datastore
                 )
 
         try:
```

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py` & `metaflow-2.8.4/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/step_functions/dynamo_db_client.py` & `metaflow-2.8.4/metaflow/plugins/aws/step_functions/dynamo_db_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/step_functions/event_bridge_client.py` & `metaflow-2.8.4/metaflow/plugins/aws/step_functions/event_bridge_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/step_functions/production_token.py` & `metaflow-2.8.4/metaflow/plugins/aws/step_functions/production_token.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/step_functions/schedule_decorator.py` & `metaflow-2.8.4/metaflow/plugins/aws/step_functions/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/step_functions/set_batch_environment.py` & `metaflow-2.8.4/metaflow/plugins/aws/step_functions/set_batch_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions.py` & `metaflow-2.8.4/metaflow/plugins/aws/step_functions/step_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import os
-from collections import defaultdict
-import sys
 import hashlib
 import json
-import time
-import string
+import os
 import random
+import string
+import sys
+import time
 import uuid
+from collections import defaultdict
 
-from metaflow.exception import MetaflowException, MetaflowInternalError
-from metaflow.plugins.aws.batch.batch_decorator import BatchDecorator
-from metaflow.plugins.resources_decorator import ResourcesDecorator
-from metaflow.plugins.retry_decorator import RetryDecorator
-from metaflow.parameters import deploy_time_eval
+from metaflow import R
 from metaflow.decorators import flow_decorators
-from metaflow.util import compress_list, dict_to_cli_options, to_pascalcase
+from metaflow.exception import MetaflowException, MetaflowInternalError
 from metaflow.metaflow_config import (
-    SFN_IAM_ROLE,
     EVENTS_SFN_ACCESS_IAM_ROLE,
+    S3_ENDPOINT_URL,
     SFN_DYNAMO_DB_TABLE,
     SFN_EXECUTION_LOG_GROUP_ARN,
-    S3_ENDPOINT_URL,
+    SFN_IAM_ROLE,
 )
-from metaflow import R
+from metaflow.parameters import deploy_time_eval
+from metaflow.plugins.aws.batch.batch_decorator import BatchDecorator
+from metaflow.plugins.resources_decorator import ResourcesDecorator
+from metaflow.plugins.retry_decorator import RetryDecorator
+from metaflow.util import compress_list, dict_to_cli_options, to_pascalcase
 
-from .step_functions_client import StepFunctionsClient
-from .event_bridge_client import EventBridgeClient
-from ..batch.batch import Batch
 from ..aws_utils import compute_resource_attributes
+from ..batch.batch import Batch
+from .event_bridge_client import EventBridgeClient
+from .step_functions_client import StepFunctionsClient
 
 
 class StepFunctionsException(MetaflowException):
     headline = "AWS Step Functions error"
 
 
 class StepFunctionsSchedulingException(MetaflowException):
@@ -223,14 +223,21 @@
                     "name of this flow or delete your "
                     "existing workflow on AWS Step "
                     "Functions." % name
                 )
         return None
 
     def _compile(self):
+        if self.flow._flow_decorators.get("trigger") or self.flow._flow_decorators.get(
+            "trigger_on_finish"
+        ):
+            raise StepFunctionsException(
+                "Deploying flows with @trigger or @trigger_on_finish decorator(s) "
+                "to AWS Step Functions is not supported currently."
+            )
         # Visit every node of the flow and recursively build the state machine.
         def _visit(node, workflow, exit_node=None):
             if node.parallel_foreach:
                 raise StepFunctionsException(
                     "Deploying flows with @parallel decorator(s) "
                     "to AWS Step Functions is not supported currently."
                 )
```

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions_cli.py` & `metaflow-2.8.4/metaflow/plugins/aws/step_functions/step_functions_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions_client.py` & `metaflow-2.8.4/metaflow/plugins/aws/step_functions/step_functions_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/aws/step_functions/step_functions_decorator.py` & `metaflow-2.8.4/metaflow/plugins/aws/step_functions/step_functions_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/azure/azure_tail.py` & `metaflow-2.8.4/metaflow/plugins/azure/azure_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/azure/azure_utils.py` & `metaflow-2.8.4/metaflow/plugins/azure/azure_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/azure/blob_service_client_factory.py` & `metaflow-2.8.4/metaflow/plugins/azure/blob_service_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/azure/includefile_support.py` & `metaflow-2.8.4/metaflow/plugins/azure/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_cli.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_client.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_datastore.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_decorator.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_modules/__init__.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_modules/base.html` & `metaflow-2.8.4/metaflow/plugins/cards/card_modules/base.html`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_modules/basic.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_modules/basic.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_modules/bundle.css` & `metaflow-2.8.4/metaflow/plugins/cards/card_modules/bundle.css`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_modules/card.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_modules/card.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/main.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_modules/chevron/main.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/renderer.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_modules/chevron/renderer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_modules/chevron/tokenizer.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_modules/chevron/tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_modules/components.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_modules/components.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_modules/convert_to_native_type.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_modules/convert_to_native_type.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_modules/main.js` & `metaflow-2.8.4/metaflow/plugins/cards/card_modules/main.js`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_modules/renderer_tools.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_modules/renderer_tools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_modules/test_cards.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_modules/test_cards.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/card_resolver.py` & `metaflow-2.8.4/metaflow/plugins/cards/card_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/component_serializer.py` & `metaflow-2.8.4/metaflow/plugins/cards/component_serializer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/cards/exception.py` & `metaflow-2.8.4/metaflow/plugins/cards/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/catch_decorator.py` & `metaflow-2.8.4/metaflow/plugins/catch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/conda/__init__.py` & `metaflow-2.8.4/metaflow/plugins/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/conda/batch_bootstrap.py` & `metaflow-2.8.4/metaflow/plugins/conda/batch_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/conda/conda.py` & `metaflow-2.8.4/metaflow/plugins/conda/conda.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/conda/conda_environment.py` & `metaflow-2.8.4/metaflow/plugins/conda/conda_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/conda/conda_flow_decorator.py` & `metaflow-2.8.4/metaflow/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/conda/conda_step_decorator.py` & `metaflow-2.8.4/metaflow/plugins/conda/conda_step_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/datastores/azure_storage.py` & `metaflow-2.8.4/metaflow/plugins/datastores/azure_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/datastores/gs_storage.py` & `metaflow-2.8.4/metaflow/plugins/datastores/gs_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/datastores/local_storage.py` & `metaflow-2.8.4/metaflow/plugins/datastores/local_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/datastores/s3_storage.py` & `metaflow-2.8.4/metaflow/plugins/datastores/s3_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/datatools/__init__.py` & `metaflow-2.8.4/metaflow/plugins/datatools/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/datatools/local.py` & `metaflow-2.8.4/metaflow/plugins/datatools/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/datatools/s3/s3.py` & `metaflow-2.8.4/metaflow/runtime.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1695 +1,1384 @@
-import json
+"""
+Local backend
+
+Execute the flow with a native runtime
+using local / remote processes
+"""
+from __future__ import print_function
 import os
-import re
 import sys
+import fcntl
 import time
-import shutil
-import random
 import subprocess
-from io import RawIOBase, BufferedIOBase
-from itertools import chain, starmap
-from tempfile import mkdtemp, NamedTemporaryFile
-from typing import Dict, Iterable, List, Optional, Tuple, Union, TYPE_CHECKING
-
-from metaflow import FlowSpec
-from metaflow.current import current
-from metaflow.metaflow_config import (
-    DATATOOLS_S3ROOT,
-    S3_RETRY_COUNT,
-    S3_TRANSIENT_RETRY_COUNT,
-    TEMPDIR,
-)
-from metaflow.util import (
-    namedtuple_with_defaults,
-    is_stringish,
-    to_bytes,
-    to_unicode,
-    to_fileobj,
-    url_quote,
-    url_unquote,
-)
-from metaflow.exception import MetaflowException
-from metaflow.debug import debug
-
-try:
-    # python2
-    from urlparse import urlparse
-except:
-    # python3
-    from urllib.parse import urlparse
-
-from .s3util import (
-    get_s3_client,
-    read_in_chunks,
-    get_timestamp,
-    TRANSIENT_RETRY_START_LINE,
-    TRANSIENT_RETRY_LINE_CONTENT,
-)
-
-if TYPE_CHECKING:
-    from metaflow.client import Run
-
-try:
-    import boto3
-    from boto3.s3.transfer import TransferConfig
-
-    DOWNLOAD_FILE_THRESHOLD = 2 * TransferConfig().multipart_threshold
-    DOWNLOAD_MAX_CHUNK = 2 * 1024 * 1024 * 1024 - 1
-    boto_found = True
-except:
-    boto_found = False
-
-
-TEST_INJECT_RETRYABLE_FAILURES = int(
-    os.environ.get("METAFLOW_S3_TEST_RETRYABLE_FAILURES", 0)
+from datetime import datetime
+from io import BytesIO
+from functools import partial
+
+from metaflow.datastore.exceptions import DataException
+
+from . import get_namespace
+from .metadata import MetaDatum
+from .metaflow_config import MAX_ATTEMPTS, UI_URL
+from .exception import (
+    MetaflowException,
+    MetaflowInternalError,
+    METAFLOW_EXIT_DISALLOW_RETRY,
 )
-
-
-def ensure_unicode(x):
-    return None if x is None else to_unicode(x)
-
-
-PutValue = Union[RawIOBase, BufferedIOBase, str, bytes]
-
-S3GetObject = namedtuple_with_defaults(
-    "S3GetObject", [("key", str), ("offset", int), ("length", int)]
+from . import procpoll
+from .datastore import TaskDataStoreSet
+from .debug import debug
+from .decorators import flow_decorators
+from .mflog import mflog, RUNTIME_LOG_SOURCE
+from .util import to_unicode, compress_list, unicode_type
+from .unbounded_foreach import (
+    CONTROL_TASK_TAG,
+    UBF_CONTROL,
+    UBF_TASK,
 )
-S3GetObject.__module__ = __name__
 
-S3PutObject = namedtuple_with_defaults(
-    "S3PutObject",
-    [
-        ("key", str),
-        ("value", Optional[PutValue]),
-        ("path", Optional[str]),
-        ("content_type", Optional[str]),
-        ("metadata", Optional[Dict[str, str]]),
-    ],
-    defaults=(None, None, None, None),
-)
-S3PutObject.__module__ = __name__
+MAX_WORKERS = 16
+MAX_NUM_SPLITS = 100
+MAX_LOG_SIZE = 1024 * 1024
+POLL_TIMEOUT = 1000  # ms
+PROGRESS_INTERVAL = 300  # s
+# The following is a list of the (data) artifacts used by the runtime while
+# executing a flow. These are prefetched during the resume operation by
+# leveraging the TaskDataStoreSet.
+PREFETCH_DATA_ARTIFACTS = ["_foreach_stack", "_task_ok", "_transition"]
+
+# Runtime must use logsource=RUNTIME_LOG_SOURCE for all loglines that it
+# formats according to mflog. See a comment in mflog.__init__
+mflog_msg = partial(mflog.decorate, RUNTIME_LOG_SOURCE)
 
-RangeInfo = namedtuple_with_defaults(
-    "RangeInfo",
-    [("total_size", int), ("request_offset", int), ("request_length", int)],
-    defaults=(0, -1),
-)
-RangeInfo.__module__ = __name__
+# TODO option: output dot graph periodically about execution
 
-RANGE_MATCH = re.compile(r"bytes (?P<start>[0-9]+)-(?P<end>[0-9]+)/(?P<total>[0-9]+)")
-
-
-class MetaflowS3InvalidObject(MetaflowException):
-    headline = "Not a string-like object"
-
-
-class MetaflowS3URLException(MetaflowException):
-    headline = "Invalid address"
-
-
-class MetaflowS3Exception(MetaflowException):
-    headline = "S3 access failed"
 
+class NativeRuntime(object):
+    def __init__(
+        self,
+        flow,
+        graph,
+        flow_datastore,
+        metadata,
+        environment,
+        package,
+        logger,
+        entrypoint,
+        event_logger,
+        monitor,
+        run_id=None,
+        clone_run_id=None,
+        clone_only=False,
+        reentrant=False,
+        clone_steps=None,
+        max_workers=MAX_WORKERS,
+        max_num_splits=MAX_NUM_SPLITS,
+        max_log_size=MAX_LOG_SIZE,
+    ):
 
-class MetaflowS3NotFound(MetaflowException):
-    headline = "S3 object not found"
+        if run_id is None:
+            self._run_id = metadata.new_run_id()
+        else:
+            self._run_id = run_id
+            metadata.register_run_id(run_id)
 
+        self._flow = flow
+        self._graph = graph
+        self._flow_datastore = flow_datastore
+        self._metadata = metadata
+        self._environment = environment
+        self._logger = logger
+        self._max_workers = max_workers
+        self._active_tasks = dict()  # Key: step name;
+        # value: [number of running tasks, number of done tasks]
+        # Special key 0 is total number of running tasks
+        self._active_tasks[0] = 0
+        self._unprocessed_steps = set([n.name for n in self._graph])
+        self._max_num_splits = max_num_splits
+        self._max_log_size = max_log_size
+        self._params_task = None
+        self._entrypoint = entrypoint
+        self.event_logger = event_logger
+        self._monitor = monitor
+
+        self._clone_run_id = clone_run_id
+        self._clone_only = clone_only
+        self._clone_steps = {} if clone_steps is None else clone_steps
+        self._reentrant = reentrant
+
+        self._origin_ds_set = None
+        if clone_run_id:
+            # resume logic
+            # 0. If clone_run_id is specified, attempt to clone all the
+            # successful tasks from the flow with `clone_run_id`. And run the
+            # unsuccessful or not-run steps in the regular fashion.
+            # 1. With _find_origin_task, for every task in the current run, we
+            # find the equivalent task in `clone_run_id` using
+            # pathspec_index=run/step:[index] and verify if this task can be
+            # cloned.
+            # 2. If yes, we fire off a clone-only task which copies the
+            # metadata from the `clone_origin` to pathspec=run/step/task to
+            # mimmick that the resumed run looks like an actual run.
+            # 3. All steps that couldn't be cloned (either unsuccessful or not
+            # run) are run as regular tasks.
+            # Lastly, to improve the performance of the cloning process, we
+            # leverage the TaskDataStoreSet abstraction to prefetch the
+            # entire DAG of `clone_run_id` and relevant data artifacts
+            # (see PREFETCH_DATA_ARTIFACTS) so that the entire runtime can
+            # access the relevant data from cache (instead of going to the datastore
+            # after the first prefetch).
+            logger(
+                "Gathering required information to resume run (this may take a bit of time)..."
+            )
+            self._origin_ds_set = TaskDataStoreSet(
+                flow_datastore,
+                clone_run_id,
+                prefetch_data_artifacts=PREFETCH_DATA_ARTIFACTS,
+            )
+        self._run_queue = []
+        self._poll = procpoll.make_poll()
+        self._workers = {}  # fd -> subprocess mapping
+        self._finished = {}
+        self._is_cloned = {}
+        # NOTE: In case of unbounded foreach, we need the following to schedule
+        # the (sibling) mapper tasks  of the control task (in case of resume);
+        # and ensure that the join tasks runs only if all dependent tasks have
+        # finished.
+        self._control_num_splits = {}  # control_task -> num_splits mapping
+
+        for step in flow:
+            for deco in step.decorators:
+                deco.runtime_init(flow, graph, package, self._run_id)
 
-class MetaflowS3AccessDenied(MetaflowException):
-    headline = "S3 access denied"
+    def _new_task(self, step, input_paths=None, **kwargs):
 
+        if input_paths is None:
+            may_clone = True
+        else:
+            may_clone = all(self._is_cloned[path] for path in input_paths)
 
-class MetaflowS3InvalidRange(MetaflowException):
-    headline = "S3 invalid range"
+        if step in self._clone_steps:
+            may_clone = False
 
+        if step == "_parameters":
+            decos = []
+        else:
+            decos = getattr(self._flow, step).decorators
 
-class S3Object(object):
-    """
-    This object represents a path or an object in S3,
-    with an optional local copy.
+        return Task(
+            self._flow_datastore,
+            self._flow,
+            step,
+            self._run_id,
+            self._metadata,
+            self._environment,
+            self._entrypoint,
+            self.event_logger,
+            self._monitor,
+            input_paths=input_paths,
+            may_clone=may_clone,
+            clone_run_id=self._clone_run_id,
+            clone_only=self._clone_only,
+            reentrant=self._reentrant,
+            origin_ds_set=self._origin_ds_set,
+            decos=decos,
+            logger=self._logger,
+            **kwargs
+        )
 
-    `S3Object`s are not instantiated directly, but they are returned
-    by many methods of the `S3` client.
-    """
+    @property
+    def run_id(self):
+        return self._run_id
 
-    def __init__(
-        self,
-        prefix: str,
-        url: str,
-        path: str,
-        size: Optional[int] = None,
-        content_type: Optional[str] = None,
-        metadata: Optional[Dict[str, str]] = None,
-        range_info: Optional[RangeInfo] = None,
-        last_modified: int = None,
-    ):
-        # all fields of S3Object should return a unicode object
-        prefix, url, path = map(ensure_unicode, (prefix, url, path))
+    def persist_constants(self, task_id=None):
+        task = self._new_task("_parameters", task_id=task_id)
+        if not task.is_cloned:
+            task.persist(self._flow)
+        self._params_task = task.path
+        self._is_cloned[task.path] = task.is_cloned
+
+    def execute(self):
+        run_url = (
+            "%s/%s/%s" % (UI_URL.rstrip("/"), self._flow.name, self._run_id)
+            if UI_URL
+            else None
+        )
 
-        self._size = size
-        self._url = url
-        self._path = path
-        self._key = None
-        self._content_type = content_type
-        self._last_modified = last_modified
-
-        self._metadata = None
-        if metadata is not None and "metaflow-user-attributes" in metadata:
-            self._metadata = json.loads(metadata["metaflow-user-attributes"])
-
-        if range_info and (
-            range_info.request_length is None or range_info.request_length < 0
-        ):
-            self._range_info = RangeInfo(
-                range_info.total_size, range_info.request_offset, range_info.total_size
+        if run_url:
+            self._logger(
+                "Workflow starting (run-id %s), see it in the UI at %s"
+                % (
+                    self._run_id,
+                    run_url,
+                ),
+                system_msg=True,
             )
         else:
-            self._range_info = range_info
+            self._logger(
+                "Workflow starting (run-id %s):" % self._run_id, system_msg=True
+            )
 
-        if path:
-            self._size = os.stat(self._path).st_size
+        self._metadata.start_run_heartbeat(self._flow.name, self._run_id)
 
-        if prefix is None or prefix == url:
-            self._key = url
-            self._prefix = None
+        if self._params_task:
+            self._queue_push("start", {"input_paths": [self._params_task]})
         else:
-            self._key = url[len(prefix.rstrip("/")) + 1 :].rstrip("/")
-            self._prefix = prefix
-
-    @property
-    def exists(self) -> bool:
-        """
-        Does this key correspond to an object in S3?
-
-        Returns
-        -------
-        bool
-            True if this object points at an existing object (file) in S3.
-        """
-        return self._size is not None
-
-    @property
-    def downloaded(self) -> bool:
-        """
-        Has this object been downloaded?
-
-        If True, the contents can be accessed through `path`, `blob`,
-        and `text` properties.
-
-        Returns
-        -------
-        bool
-            True if the contents of this object have been downloaded.
-        """
-        return bool(self._path)
-
-    @property
-    def url(self) -> str:
-        """
-        S3 location of the object
-
-        Returns
-        -------
-        str
-            The S3 location of this object.
-        """
-        return self._url
-
-    @property
-    def prefix(self) -> str:
-        """
-        Prefix requested that matches this object.
-
-        Returns
-        -------
-        str
-            Requested prefix
-        """
-        return self._prefix
+            self._queue_push("start", {})
 
-    @property
-    def key(self) -> str:
-        """
-        Key corresponds to the key given to the get call that produced
-        this object.
-
-        This may be a full S3 URL or a suffix based on what
-        was requested.
-
-        Returns
-        -------
-        str
-            Key requested.
-        """
-        return self._key
+        progress_tstamp = time.time()
+        try:
+            # main scheduling loop
+            exception = None
+            while self._run_queue or self._active_tasks[0] > 0:
+
+                # 1. are any of the current workers finished?
+                finished_tasks = list(self._poll_workers())
+                # 2. push new tasks triggered by the finished tasks to the queue
+                self._queue_tasks(finished_tasks)
+                # 3. if there are available worker slots, pop and start tasks
+                #    from the queue.
+                self._launch_workers()
+
+                if time.time() - progress_tstamp > PROGRESS_INTERVAL:
+                    progress_tstamp = time.time()
+                    tasks_print = ", ".join(
+                        [
+                            "%s (%d running; %d done)" % (k, v[0], v[1])
+                            for k, v in self._active_tasks.items()
+                            if k != 0 and v[0] > 0
+                        ]
+                    )
+                    if self._active_tasks[0] == 0:
+                        msg = "No tasks are running."
+                    else:
+                        if self._active_tasks[0] == 1:
+                            msg = "1 task is running: "
+                        else:
+                            msg = "%d tasks are running: " % self._active_tasks[0]
+                        msg += "%s." % tasks_print
 
-    @property
-    def path(self) -> Optional[str]:
-        """
-        Path to a local temporary file corresponding to the object downloaded.
-
-        This file gets deleted automatically when a S3 scope exits.
-        Returns None if this S3Object has not been downloaded.
-
-        Returns
-        -------
-        str
-            Local path, if the object has been downloaded.
-        """
-        return self._path
+                    self._logger(msg, system_msg=True)
 
-    @property
-    def blob(self) -> Optional[bytes]:
-        """
-        Contents of the object as a byte string or None if the
-        object hasn't been downloaded.
-
-        Returns
-        -------
-        bytes
-            Contents of the object as bytes.
-        """
-        if self._path:
-            with open(self._path, "rb") as f:
-                return f.read()
+                    if len(self._run_queue) == 0:
+                        msg = "No tasks are waiting in the queue."
+                    else:
+                        if len(self._run_queue) == 1:
+                            msg = "1 task is waiting in the queue: "
+                        else:
+                            msg = "%d tasks are waiting in the queue." % len(
+                                self._run_queue
+                            )
 
-    @property
-    def text(self) -> Optional[str]:
-        """
-        Contents of the object as a string or None if the
-        object hasn't been downloaded.
-
-        The object is assumed to contain UTF-8 encoded data.
-
-        Returns
-        -------
-        str
-            Contents of the object as text.
-        """
-        if self._path:
-            return self.blob.decode("utf-8", errors="replace")
+                    self._logger(msg, system_msg=True)
+                    if len(self._unprocessed_steps) > 0:
+                        if len(self._unprocessed_steps) == 1:
+                            msg = "%s step has not started" % (
+                                next(iter(self._unprocessed_steps)),
+                            )
+                        else:
+                            msg = "%d steps have not started: " % len(
+                                self._unprocessed_steps
+                            )
+                            msg += "%s." % ", ".join(self._unprocessed_steps)
+                        self._logger(msg, system_msg=True)
 
-    @property
-    def size(self) -> Optional[int]:
-        """
-        Size of the object in bytes.
-
-        Returns None if the key does not correspond to an object in S3.
-
-        Returns
-        -------
-        int
-            Size of the object in bytes, if the object exists.
-        """
-        return self._size
+        except KeyboardInterrupt as ex:
+            self._logger("Workflow interrupted.", system_msg=True, bad=True)
+            self._killall()
+            exception = ex
+            raise
+        except Exception as ex:
+            self._logger("Workflow failed.", system_msg=True, bad=True)
+            self._killall()
+            exception = ex
+            raise
+        finally:
+            # on finish clean tasks
+            for step in self._flow:
+                for deco in step.decorators:
+                    deco.runtime_finished(exception)
+
+            self._metadata.stop_heartbeat()
+
+        # assert that end was executed and it was successful
+        if ("end", ()) in self._finished:
+            if run_url:
+                self._logger(
+                    "Done! See the run in the UI at %s" % run_url,
+                    system_msg=True,
+                )
+            else:
+                self._logger("Done!", system_msg=True)
+        elif self._clone_only:
+            self._logger(
+                "Clone-only resume complete -- only previously successful steps were "
+                "cloned; no new tasks executed!",
+                system_msg=True,
+            )
+        else:
+            raise MetaflowInternalError(
+                "The *end* step was not successful by the end of flow."
+            )
 
-    @property
-    def has_info(self) -> bool:
-        """
-        Returns true if this `S3Object` contains the content-type MIME header or
-        user-defined metadata.
-
-        If False, this means that `content_type`, `metadata`, `range_info` and
-        `last_modified` will return None.
-
-        Returns
-        -------
-        bool
-            True if additional metadata is available.
-        """
-        return (
-            self._content_type is not None
-            or self._metadata is not None
-            or self._range_info is not None
+    def _killall(self):
+        # If we are here, all children have received a signal and are shutting down.
+        # We want to give them an opportunity to do so and then kill
+        live_workers = set(self._workers.values())
+        now = int(time.time())
+        self._logger(
+            "Terminating %d active tasks..." % len(live_workers),
+            system_msg=True,
+            bad=True,
         )
+        while live_workers and int(time.time()) - now < 5:
+            # While not all workers are dead and we have waited less than 5 seconds
+            live_workers = [worker for worker in live_workers if not worker.clean()]
+        if live_workers:
+            self._logger(
+                "Killing %d remaining tasks after having waited for %d seconds -- "
+                "some tasks may not exit cleanly"
+                % (len(live_workers), int(time.time()) - now),
+                system_msg=True,
+                bad=True,
+            )
+            for worker in live_workers:
+                worker.kill()
+        self._logger("Flushing logs...", system_msg=True, bad=True)
+        # give killed workers a chance to flush their logs to datastore
+        for _ in range(3):
+            list(self._poll_workers())
+
+    # Store the parameters needed for task creation, so that pushing on items
+    # onto the run_queue is an inexpensive operation.
+    def _queue_push(self, step, task_kwargs):
+        self._run_queue.insert(0, (step, task_kwargs))
+        # For foreaches, this will happen multiple time but is ok, becomes a no-op
+        self._unprocessed_steps.discard(step)
+
+    def _queue_pop(self):
+        return self._run_queue.pop() if self._run_queue else (None, {})
+
+    def _queue_task_join(self, task, next_steps):
+        # if the next step is a join, we need to check that
+        # all input tasks for the join have finished before queuing it.
+
+        # CHECK: this condition should be enforced by the linter but
+        # let's assert that the assumption holds
+        if len(next_steps) > 1:
+            msg = (
+                "Step *{step}* transitions to a join and another "
+                "step. The join must be the only transition."
+            )
+            raise MetaflowInternalError(task, msg.format(step=task.step))
+        else:
+            next_step = next_steps[0]
 
-    @property
-    def metadata(self) -> Optional[Dict[str, str]]:
-        """
-        Returns a dictionary of user-defined metadata, or None if no metadata
-        is defined.
-
-        Returns
-        -------
-        Dict
-            User-defined metadata.
-        """
-        return self._metadata
+        unbounded_foreach = not task.results.is_none("_unbounded_foreach")
 
-    @property
-    def content_type(self) -> Optional[str]:
-        """
-        Returns the content-type of the S3 object or None if it is not defined.
-
-        Returns
-        -------
-        str
-            Content type or None if the content type is undefined.
-        """
-        return self._content_type
+        if unbounded_foreach:
+            # Before we queue the join, do some post-processing of runtime state
+            # (_finished, _is_cloned) for the (sibling) mapper tasks.
+            # Update state of (sibling) mapper tasks for control task.
+            if task.ubf_context == UBF_CONTROL:
+                mapper_tasks = task.results.get("_control_mapper_tasks")
+                if not mapper_tasks:
+                    msg = (
+                        "Step *{step}* has a control task which didn't "
+                        "specify the artifact *_control_mapper_tasks* for "
+                        "the subsequent *{join}* step."
+                    )
+                    raise MetaflowInternalError(
+                        msg.format(step=task.step, join=next_steps[0])
+                    )
+                elif not (
+                    isinstance(mapper_tasks, list)
+                    and isinstance(mapper_tasks[0], unicode_type)
+                ):
+                    msg = (
+                        "Step *{step}* has a control task which didn't "
+                        "specify the artifact *_control_mapper_tasks* as a "
+                        "list of strings but instead specified it as {typ} "
+                        "with elements of {elem_typ}."
+                    )
+                    raise MetaflowInternalError(
+                        msg.format(
+                            step=task.step,
+                            typ=type(mapper_tasks),
+                            elem_type=type(mapper_tasks[0]),
+                        )
+                    )
+                num_splits = len(mapper_tasks)
+                self._control_num_splits[task.path] = num_splits
+                if task.is_cloned:
+                    # Add mapper tasks to be cloned.
+                    for i in range(num_splits):
+                        # NOTE: For improved robustness, introduce
+                        # `clone_options` as an enum so that we can force that
+                        # clone must occur for this task.
+                        self._queue_push(
+                            task.step,
+                            {
+                                "input_paths": task.input_paths,
+                                "split_index": str(i),
+                                "ubf_context": UBF_TASK,
+                            },
+                        )
+                else:
+                    # Update _finished since these tasks were successfully
+                    # run elsewhere so that join will be unblocked.
+                    step_name, foreach_stack = task.finished_id
+                    top = foreach_stack[-1]
+                    bottom = list(foreach_stack[:-1])
+                    for i in range(num_splits):
+                        s = tuple(bottom + [top._replace(index=i)])
+                        self._finished[(task.step, s)] = mapper_tasks[i]
+                        self._is_cloned[mapper_tasks[i]] = False
+
+            # Find and check status of control task and retrieve its pathspec
+            # for retrieving unbounded foreach cardinality.
+            step_name, foreach_stack = task.finished_id
+            top = foreach_stack[-1]
+            bottom = list(foreach_stack[:-1])
+            s = tuple(bottom + [top._replace(index=None)])
+
+            # UBF control can also be the first task of the list. Then
+            # it will have index=0 instead of index=None.
+            if task.results.get("_control_task_is_mapper_zero", False):
+                s = tuple(bottom + [top._replace(index=0)])
+            control_path = self._finished.get((task.step, s))
+            if control_path:
+                # Control task was successful.
+                # Additionally check the state of (sibling) mapper tasks as well
+                # (for the sake of resume) before queueing join task.
+                num_splits = self._control_num_splits[control_path]
+                required_tasks = []
+                for i in range(num_splits):
+                    s = tuple(bottom + [top._replace(index=i)])
+                    required_tasks.append(self._finished.get((task.step, s)))
+
+                if all(required_tasks):
+                    # all tasks to be joined are ready. Schedule the next join step.
+                    self._queue_push(
+                        next_step,
+                        {"input_paths": required_tasks, "join_type": "foreach"},
+                    )
+        else:
+            # matching_split is the split-parent of the finished task
+            matching_split = self._graph[self._graph[next_step].split_parents[-1]]
+            step_name, foreach_stack = task.finished_id
+
+            if matching_split.type == "foreach":
+                # next step is a foreach join
+
+                def siblings(foreach_stack):
+                    top = foreach_stack[-1]
+                    bottom = list(foreach_stack[:-1])
+                    for index in range(top.num_splits):
+                        yield tuple(bottom + [top._replace(index=index)])
+
+                # required tasks are all split-siblings of the finished task
+                required_tasks = [
+                    self._finished.get((task.step, s)) for s in siblings(foreach_stack)
+                ]
+                join_type = "foreach"
+            else:
+                # next step is a split
+                # required tasks are all branches joined by the next step
+                required_tasks = [
+                    self._finished.get((step, foreach_stack))
+                    for step in self._graph[next_step].in_funcs
+                ]
+                join_type = "linear"
+
+            if all(required_tasks):
+                # all tasks to be joined are ready. Schedule the next join step.
+                self._queue_push(
+                    next_step, {"input_paths": required_tasks, "join_type": join_type}
+                )
 
-    @property
-    def range_info(self) -> Optional[RangeInfo]:
-        """
-        If the object corresponds to a partially downloaded object, returns
-        information of what was downloaded.
-
-        The returned object has the following fields:
-        - `total_size`: Size of the object in S3.
-        - `request_offset`: The starting offset.
-        - `request_length`: The number of bytes downloaded.
-
-        Returns
-        -------
-        namedtuple
-            An object containing information about the partial download. If
-            the `S3Object` doesn't correspond to a partially downloaded file,
-            returns None.
-        """
-        return self._range_info
+    def _queue_task_foreach(self, task, next_steps):
 
-    @property
-    def last_modified(self) -> Optional[int]:
-        """
-        Returns the last modified unix timestamp of the object.
-
-        Returns
-        -------
-        int
-            Unix timestamp corresponding to the last modified time.
-        """
-        return self._last_modified
+        # CHECK: this condition should be enforced by the linter but
+        # let's assert that the assumption holds
+        if len(next_steps) > 1:
+            msg = (
+                "Step *{step}* makes a foreach split but it defines "
+                "multiple transitions. Specify only one transition "
+                "for foreach."
+            )
+            raise MetaflowInternalError(msg.format(step=task.step))
+        else:
+            next_step = next_steps[0]
 
-    def __str__(self):
-        if self._path:
-            return "<S3Object %s (%d bytes, local)>" % (self._url, self._size)
-        elif self._size:
-            return "<S3Object %s (%d bytes, in S3)>" % (self._url, self._size)
+        unbounded_foreach = not task.results.is_none("_unbounded_foreach")
+        if unbounded_foreach:
+            # Need to push control process related task.
+            ubf_iter_name = task.results.get("_foreach_var")
+            ubf_iter = task.results.get(ubf_iter_name)
+            self._queue_push(
+                next_step,
+                {
+                    "input_paths": [task.path],
+                    "ubf_context": UBF_CONTROL,
+                    "ubf_iter": ubf_iter,
+                },
+            )
         else:
-            return "<S3Object %s (object does not exist)>" % self._url
+            num_splits = task.results["_foreach_num_splits"]
+            if num_splits > self._max_num_splits:
+                msg = (
+                    "Foreach in step *{step}* yielded {num} child steps "
+                    "which is more than the current maximum of {max} "
+                    "children. You can raise the maximum with the "
+                    "--max-num-splits option. "
+                )
+                raise TaskFailed(
+                    task,
+                    msg.format(
+                        step=task.step, num=num_splits, max=self._max_num_splits
+                    ),
+                )
 
-    def __repr__(self):
-        return str(self)
+            # schedule all splits
+            for i in range(num_splits):
+                self._queue_push(
+                    next_step, {"split_index": str(i), "input_paths": [task.path]}
+                )
 
+    def _queue_tasks(self, finished_tasks):
+        # finished tasks include only successful tasks
+        for task in finished_tasks:
+            self._finished[task.finished_id] = task.path
+            self._is_cloned[task.path] = task.is_cloned
+
+            # CHECK: ensure that runtime transitions match with
+            # statically inferred transitions. Make an exception for control
+            # tasks, where we just rely on static analysis since we don't
+            # execute user code.
+            trans = task.results.get("_transition")
+            if trans:
+                next_steps = trans[0]
+                foreach = trans[1]
+            else:
+                next_steps = []
+                foreach = None
+            expected = self._graph[task.step].out_funcs
+            if next_steps != expected:
+                msg = (
+                    "Based on static analysis of the code, step *{step}* "
+                    "was expected to transition to step(s) *{expected}*. "
+                    "However, when the code was executed, self.next() was "
+                    "called with *{actual}*. Make sure there is only one "
+                    "unconditional self.next() call in the end of your "
+                    "step. "
+                )
+                raise MetaflowInternalError(
+                    msg.format(
+                        step=task.step,
+                        expected=", ".join(expected),
+                        actual=", ".join(next_steps),
+                    )
+                )
 
-class S3Client(object):
-    def __init__(self, s3_role_arn=None, s3_session_vars=None, s3_client_params=None):
-        self._s3_client = None
-        self._s3_error = None
-        self._s3_role = s3_role_arn
-        self._s3_session_vars = s3_session_vars
-        self._s3_client_params = s3_client_params
+            # Different transition types require different treatment
+            if any(self._graph[f].type == "join" for f in next_steps):
+                # Next step is a join
+                self._queue_task_join(task, next_steps)
+            elif foreach:
+                # Next step is a foreach child
+                self._queue_task_foreach(task, next_steps)
+            else:
+                # Next steps are normal linear steps
+                for step in next_steps:
+                    self._queue_push(step, {"input_paths": [task.path]})
+
+    def _poll_workers(self):
+        if self._workers:
+            for event in self._poll.poll(POLL_TIMEOUT):
+                worker = self._workers.get(event.fd)
+                if worker:
+                    if event.can_read:
+                        worker.read_logline(event.fd)
+                    if event.is_terminated:
+                        returncode = worker.terminate()
+
+                        for fd in worker.fds():
+                            self._poll.remove(fd)
+                            del self._workers[fd]
+                        step_counts = self._active_tasks[worker.task.step]
+                        step_counts[0] -= 1  # One less task for this step is running
+                        step_counts[1] += 1  # ... and one more completed.
+                        # We never remove from self._active_tasks because it is possible
+                        # for all currently running task for a step to complete but
+                        # for others to still be queued up.
+                        self._active_tasks[0] -= 1
+
+                        task = worker.task
+                        if returncode:
+                            # worker did not finish successfully
+                            if (
+                                worker.cleaned
+                                or returncode == METAFLOW_EXIT_DISALLOW_RETRY
+                            ):
+                                self._logger(
+                                    "This failed task will not be retried.",
+                                    system_msg=True,
+                                )
+                            else:
+                                if (
+                                    task.retries
+                                    < task.user_code_retries + task.error_retries
+                                ):
+                                    self._retry_worker(worker)
+                                else:
+                                    raise TaskFailed(task)
+                        else:
+                            # worker finished successfully
+                            yield task
 
-    @property
-    def client(self):
-        if self._s3_client is None:
-            self.reset_client()
-        return self._s3_client
+    def _launch_workers(self):
+        while self._run_queue and self._active_tasks[0] < self._max_workers:
+            step, task_kwargs = self._queue_pop()
+            # Initialize the task (which can be expensive using remote datastores)
+            # before launching the worker so that cost is amortized over time, instead
+            # of doing it during _queue_push.
+            task = self._new_task(step, **task_kwargs)
+            self._launch_worker(task)
+
+    def _retry_worker(self, worker):
+        worker.task.retries += 1
+        if worker.task.retries >= MAX_ATTEMPTS:
+            # any results with an attempt ID >= MAX_ATTEMPTS will be ignored
+            # by datastore, so running a task with such a retry_could would
+            # be pointless and dangerous
+            raise MetaflowInternalError(
+                "Too many task attempts (%d)! "
+                "MAX_ATTEMPTS exceeded." % worker.task.retries
+            )
 
-    @property
-    def error(self):
-        if self._s3_error is None:
-            self.reset_client()
-        return self._s3_error
-
-    def reset_client(self):
-        self._s3_client, self._s3_error = get_s3_client(
-            s3_role_arn=self._s3_role,
-            s3_session_vars=self._s3_session_vars,
-            s3_client_params=self._s3_client_params,
-        )
+        worker.task.new_attempt()
+        self._launch_worker(worker.task)
 
+    def _launch_worker(self, task):
+        if self._clone_only and not task.is_cloned:
+            # We don't launch a worker here
+            self._logger(
+                "Not executing non-cloned task for step '%s' in clone-only resume"
+                % "/".join([task.flow_name, task.run_id, task.step]),
+                system_msg=True,
+            )
+            return
 
-class S3(object):
-    """
-    The Metaflow S3 client.
+        worker = Worker(task, self._max_log_size)
+        for fd in worker.fds():
+            self._workers[fd] = worker
+            self._poll.add(fd)
+        active_step_counts = self._active_tasks.setdefault(task.step, [0, 0])
 
-    This object manages the connection to S3 and a temporary diretory that is used
-    to download objects. Note that in most cases when the data fits in memory, no local
-    disk IO is needed as operations are cached by the operating system, which makes
-    operations fast as long as there is enough memory available.
-
-    The easiest way is to use this object as a context manager:
-    ```
-    with S3() as s3:
-        data = [obj.blob for obj in s3.get_many(urls)]
-    print(data)
-    ```
-    The context manager takes care of creating and deleting a temporary directory
-    automatically. Without a context manager, you must call `.close()` to delete
-    the directory explicitly:
-    ```
-    s3 = S3()
-    data = [obj.blob for obj in s3.get_many(urls)]
-    s3.close()
-    ```
-    You can customize the location of the temporary directory with `tmproot`. It
-    defaults to the current working directory.
-
-    To make it easier to deal with object locations, the client can be initialized
-    with an S3 path prefix. There are three ways to handle locations:
-
-    1. Use a `metaflow.Run` object or `self`, e.g. `S3(run=self)` which
-       initializes the prefix with the global `DATATOOLS_S3ROOT` path, combined
-       with the current run ID. This mode makes it easy to version data based
-       on the run ID consistently. You can use the `bucket` and `prefix` to
-       override parts of `DATATOOLS_S3ROOT`.
-
-    2. Specify an S3 prefix explicitly with `s3root`,
-       e.g. `S3(s3root='s3://mybucket/some/path')`.
-
-    3. Specify nothing, i.e. `S3()`, in which case all operations require
-       a full S3 url prefixed with `s3://`.
-
-    Parameters
-    ----------
-    tmproot : str, default: '.'
-        Where to store the temporary directory.
-    bucket : str, optional
-        Override the bucket from `DATATOOLS_S3ROOT` when `run` is specified.
-    prefix : str, optional
-        Override the path from `DATATOOLS_S3ROOT` when `run` is specified.
-    run : FlowSpec or Run, optional
-        Derive path prefix from the current or a past run ID, e.g. S3(run=self).
-    s3root : str, optional
-        If `run` is not specified, use this as the S3 prefix.
-    """
+        # We have an additional task for this step running
+        active_step_counts[0] += 1
+
+        # One more task actively running
+        self._active_tasks[0] += 1
 
-    @classmethod
-    def get_root_from_config(cls, echo, create_on_absent=True):
-        return DATATOOLS_S3ROOT
+
+class Task(object):
+    clone_pathspec_mapping = {}
 
     def __init__(
         self,
-        tmproot: str = TEMPDIR,
-        bucket: Optional[str] = None,
-        prefix: Optional[str] = None,
-        run: Optional[Union[FlowSpec, "Run"]] = None,
-        s3root: Optional[str] = None,
-        **kwargs
+        flow_datastore,
+        flow,
+        step,
+        run_id,
+        metadata,
+        environment,
+        entrypoint,
+        event_logger,
+        monitor,
+        input_paths=None,
+        may_clone=False,
+        clone_run_id=None,
+        clone_only=False,
+        reentrant=False,
+        origin_ds_set=None,
+        decos=None,
+        logger=None,
+        # Anything below this is passed as part of kwargs
+        split_index=None,
+        ubf_context=None,
+        ubf_iter=None,
+        join_type=None,
+        task_id=None,
     ):
-        if not boto_found:
-            raise MetaflowException("You need to install 'boto3' in order to use S3.")
 
-        if run:
-            # 1. use a (current) run ID with optional customizations
-            parsed = urlparse(DATATOOLS_S3ROOT)
-            if not bucket:
-                bucket = parsed.netloc
-            if not prefix:
-                prefix = parsed.path
-            if isinstance(run, FlowSpec):
-                if current.is_running_flow:
-                    prefix = os.path.join(prefix, current.flow_name, current.run_id)
-                else:
-                    raise MetaflowS3URLException(
-                        "Initializing S3 with a FlowSpec outside of a running "
-                        "flow is not supported."
+        self.step = step
+        self.flow_name = flow.name
+        self.run_id = run_id
+        self.task_id = None
+        self._path = None
+        self.input_paths = input_paths
+        self.split_index = split_index
+        self.ubf_context = ubf_context
+        self.ubf_iter = ubf_iter
+        self.decos = [] if decos is None else decos
+        self.entrypoint = entrypoint
+        self.environment = environment
+        self.environment_type = self.environment.TYPE
+        self.clone_run_id = clone_run_id
+        self.clone_origin = None
+        self.origin_ds_set = origin_ds_set
+        self.metadata = metadata
+        self.event_logger = event_logger
+        self.monitor = monitor
+
+        self._logger = logger
+
+        self.retries = 0
+        self.user_code_retries = 0
+        self.error_retries = 0
+
+        self.tags = metadata.sticky_tags
+        self.event_logger_type = self.event_logger.TYPE
+        self.monitor_type = monitor.TYPE
+
+        self.metadata_type = metadata.TYPE
+        self.datastore_type = flow_datastore.TYPE
+        self._flow_datastore = flow_datastore
+        self.datastore_sysroot = flow_datastore.datastore_root
+        self._results_ds = None
+
+        origin = None
+        if clone_run_id and may_clone:
+            origin = self._find_origin_task(clone_run_id, join_type)
+        if origin and origin["_task_ok"]:
+            # At this point, we know we are going to clone
+            self._is_cloned = True
+            if reentrant:
+                # A re-entrant clone basically allows multiple concurrent processes
+                # to perform the clone at the same time to the same new run id. Let's
+                # assume two processes A and B both simultaneously calling
+                # `resume --reentrant --run-id XX`.
+                # For each task that is cloned, we want to guarantee that:
+                #   - one and only one of A or B will do the actual cloning
+                #   - the other process (or other processes) will block until the cloning
+                #     is complete.
+                # This ensures that the rest of the clone algorithm can proceed as normal
+                # and also guarantees that we only write once to the datastore and
+                # metadata.
+                #
+                # To accomplish this, we use the cloned task's task-id as the "key" to
+                # synchronize on. We then try to "register" this new task-id (or rather
+                # the full pathspec <run>/<step>/<taskid>) with the metadata service
+                # which will indicate if we actually registered it or if it existed
+                # already. If we did manage to register it, we are the "elected cloner"
+                # in essence and proceed to clone. If we didn't, we just wait to make
+                # sure the task is fully done (ie: the clone is finished).
+                if task_id is not None:
+                    # Sanity check -- this should never happen. We cannot allow
+                    # for explicit task-ids because in the reentrant case, we use the
+                    # cloned task's id as the new task's id.
+                    raise MetaflowInternalError(
+                        "Reentrant clone-only resume does not allow for explicit task-id"
                     )
+
+                # We will use the same task_id as the original task
+                # to use it effectively as a synchronization key
+                clone_task_id = origin.task_id
+                # Make sure the task-id is a non-integer to not clash with task ids
+                # assigned by the metadata provider. If this is an integer, we
+                # add some string to it. It doesn't matter what we add as long as it is
+                # consistent.
+                try:
+                    clone_task_int = int(clone_task_id)
+                    clone_task_id = "resume-%d" % clone_task_int
+                except ValueError:
+                    pass
+
+                # If _get_task_id returns True it means the task already existed, so
+                # we wait for it.
+                self._wait_for_clone = self._get_task_id(clone_task_id)
             else:
-                prefix = os.path.join(prefix, run.parent.id, run.id)
+                self._wait_for_clone = False
+                self._get_task_id(task_id)
 
-            self._s3root = "s3://%s" % os.path.join(bucket, prefix.strip("/"))
-        elif s3root:
-            # 2. use an explicit S3 prefix
-            parsed = urlparse(to_unicode(s3root))
-            if parsed.scheme != "s3":
-                raise MetaflowS3URLException(
-                    "s3root needs to be an S3 URL prefixed with s3://."
-                )
-            self._s3root = s3root.rstrip("/")
+            # Store the mapping from current_pathspec -> origin_pathspec which
+            # will be useful for looking up origin_ds_set in find_origin_task.
+            self.clone_pathspec_mapping[self._path] = origin.pathspec
+            if self.step == "_parameters":
+                # We don't put _parameters on the queue so we either clone it or wait
+                # for it.
+                if not self._wait_for_clone:
+                    # Clone in place without relying on run_queue.
+                    self.new_attempt()
+                    self._ds.clone(origin)
+                    self._ds.done()
+                else:
+                    # TODO: There is a bit of a duplication with the task.py
+                    # clone_only function here
+                    self.log(
+                        "Waiting for clone of _parameters step to occur...",
+                        system_msg=True,
+                    )
+                    while True:
+                        try:
+                            ds = self._flow_datastore.get_task_datastore(
+                                self.run_id, self.step, self.task_id
+                            )
+                            if not ds["_task_ok"]:
+                                raise MetaflowInternalError(
+                                    "Externally cloned _parameters task did not succeed"
+                                )
+                            break
+                        except DataException:
+                            self.log("Sleeping for 5s...", system_msg=True)
+                            # No need to get fancy with the sleep here.
+                            time.sleep(5)
+                    self.log("_parameters clone successful", system_msg=True)
+            else:
+                # For non parameter steps
+                # Store the origin pathspec in clone_origin so this can be run
+                # as a task by the runtime.
+                self.clone_origin = origin.pathspec
+                # Save a call to creating the results_ds since its same as origin.
+                self._results_ds = origin
+                if self._wait_for_clone:
+                    self.log(
+                        "Waiting for the successful cloning of results "
+                        "of a previously run task %s (this may take some time)"
+                        % self.clone_origin,
+                        system_msg=True,
+                    )
+                else:
+                    self.log(
+                        "Cloning results of a previously run task %s"
+                        % self.clone_origin,
+                        system_msg=True,
+                    )
         else:
-            # 3. use the client only with full URLs
-            self._s3root = None
+            self._is_cloned = False
+            if clone_only:
+                # We are done -- we don't proceed to create new task-ids
+                return
+            self._get_task_id(task_id)
+
+        # Open the output datastore only if the task is not being cloned.
+        if not self._is_cloned:
+            self.new_attempt()
+
+            for deco in decos:
+                deco.runtime_task_created(
+                    self._ds,
+                    task_id,
+                    split_index,
+                    input_paths,
+                    self._is_cloned,
+                    ubf_context,
+                )
 
-        # Note that providing a role, session vars or client params and a client
-        # will result in the role/session vars/client params being ignored
-        self._s3_role = kwargs.get("role", None)
-        self._s3_session_vars = kwargs.get("session_vars", None)
-        self._s3_client_params = kwargs.get("client_params", None)
-        self._s3_client = kwargs.get(
-            "external_client",
-            S3Client(
-                s3_role_arn=self._s3_role,
-                s3_session_vars=self._s3_session_vars,
-                s3_client_params=self._s3_client_params,
-            ),
-        )
-        self._s3_inject_failures = kwargs.get(
-            "inject_failure_rate", TEST_INJECT_RETRYABLE_FAILURES
+                # determine the number of retries of this task
+                user_code_retries, error_retries = deco.step_task_retry_count()
+                if user_code_retries is None and error_retries is None:
+                    # This signals the runtime that the task doesn't want any
+                    # retries indifferent to other decorator opinions.
+                    # NOTE: This is needed since we don't statically disallow
+                    # specifying `@retry` in combination with decorators which
+                    # implement `unbounded_foreach` semantics. This allows for
+                    # ergonomic user invocation of `--with retry`; instead
+                    # choosing to specially handle this way in the runtime.
+                    self.user_code_retries = None
+                    self.error_retries = None
+                if (
+                    self.user_code_retries is not None
+                    and self.error_retries is not None
+                ):
+                    self.user_code_retries = max(
+                        self.user_code_retries, user_code_retries
+                    )
+                    self.error_retries = max(self.error_retries, error_retries)
+            if self.user_code_retries is None and self.error_retries is None:
+                self.user_code_retries = 0
+                self.error_retries = 0
+
+    def new_attempt(self):
+        self._ds = self._flow_datastore.get_task_datastore(
+            self.run_id, self.step, self.task_id, attempt=self.retries, mode="w"
         )
-        self._tmpdir = mkdtemp(dir=tmproot, prefix="metaflow.s3.")
+        self._ds.init_task()
 
-    def __enter__(self) -> "S3":
-        return self
+    def log(self, msg, system_msg=False, pid=None, timestamp=True):
+        if pid:
+            prefix = "[%s (pid %s)] " % (self._path, pid)
+        else:
+            prefix = "[%s] " % self._path
 
-    def __exit__(self, *args):
-        self.close()
+        self._logger(msg, head=prefix, system_msg=system_msg, timestamp=timestamp)
+        sys.stdout.flush()
 
-    def close(self):
-        """
-        Delete all temporary files downloaded in this context.
-        """
-        try:
-            if not debug.s3client:
-                if self._tmpdir:
-                    shutil.rmtree(self._tmpdir)
-                    self._tmpdir = None
-        except:
-            pass
-
-    def _url(self, key_value):
-        # NOTE: All URLs are handled as Unicode objects (unicode in py2,
-        # string in py3) internally. We expect that all URLs passed to this
-        # class as either Unicode or UTF-8 encoded byte strings. All URLs
-        # returned are Unicode.
-        key = getattr(key_value, "key", key_value)
-        if self._s3root is None:
-            parsed = urlparse(to_unicode(key))
-            if parsed.scheme == "s3" and parsed.path:
-                return key
-            else:
-                if current.is_running_flow:
-                    raise MetaflowS3URLException(
-                        "Specify S3(run=self) when you use S3 inside a running "
-                        "flow. Otherwise you have to use S3 with full "
-                        "s3:// urls."
-                    )
-                else:
-                    raise MetaflowS3URLException(
-                        "Initialize S3 with an 's3root' or 'run' if you don't "
-                        "want to specify full s3:// urls."
+    def _get_task_id(self, task_id):
+        already_existed = True
+        if self.ubf_context == UBF_CONTROL:
+            [input_path] = self.input_paths
+            run, input_step, input_task = input_path.split("/")
+            # We associate the control task-id to be 1:1 with the split node
+            # where the unbounded-foreach was defined.
+            # We prefer encoding the corresponding split into the task_id of
+            # the control node; so it has access to this information quite
+            # easily. There is anyway a corresponding int id stored in the
+            # metadata backend - so this should be fine.
+            task_id = "control-%s-%s-%s" % (run, input_step, input_task)
+        # Register only regular Metaflow (non control) tasks.
+        if task_id is None:
+            task_id = str(self.metadata.new_task_id(self.run_id, self.step))
+            already_existed = False
+        else:
+            # task_id is preset only by persist_constants() or control tasks.
+            if self.ubf_context == UBF_CONTROL:
+                tags = [CONTROL_TASK_TAG]
+                attempt_id = 0
+                already_existed = not self.metadata.register_task_id(
+                    self.run_id,
+                    self.step,
+                    task_id,
+                    attempt_id,
+                    sys_tags=tags,
+                )
+                # A Task's tags are now those of its ancestral Run, so we are not able
+                # to rely on a task's tags to indicate the presence of a control task
+                # so, on top of adding the tags above, we also add a task metadata
+                # entry indicating that this is a "control task".
+                #
+                # Here we will also add a task metadata entry to indicate "control task".
+                # Within the metaflow repo, the only dependency of such a "control task"
+                # indicator is in the integration test suite (see Step.control_tasks() in
+                # client API).
+                task_metadata_list = [
+                    MetaDatum(
+                        field="internal_task_type",
+                        value=CONTROL_TASK_TAG,
+                        type="internal_task_type",
+                        tags=["attempt_id:{0}".format(attempt_id)],
                     )
-        elif key:
-            if key.startswith("s3://"):
-                raise MetaflowS3URLException(
-                    "Don't use absolute S3 URLs when the S3 client is "
-                    "initialized with a prefix. URL: %s" % key
+                ]
+                self.metadata.register_metadata(
+                    self.run_id, self.step, task_id, task_metadata_list
+                )
+            else:
+                already_existed = not self.metadata.register_task_id(
+                    self.run_id, self.step, task_id, 0
                 )
-            return os.path.join(self._s3root, key)
-        else:
-            return self._s3root
 
-    def _url_and_range(self, key_value):
-        url = self._url(key_value)
-        start = getattr(key_value, "offset", None)
-        length = getattr(key_value, "length", None)
-        range_str = None
-        # Range specification are inclusive so getting from offset 500 for 100
-        # bytes will read as bytes=500-599
-        if start is not None or length is not None:
-            if start is None:
-                start = 0
-            if length is None:
-                # Fetch from offset till the end of the file
-                range_str = "bytes=%d-" % start
-            elif length < 0:
-                # Fetch from end; ignore start value here
-                range_str = "bytes=-%d" % (-length)
+        self.task_id = task_id
+        self._path = "%s/%s/%s" % (self.run_id, self.step, self.task_id)
+        return already_existed
+
+    def _find_origin_task(self, clone_run_id, join_type):
+        if self.step == "_parameters":
+            pathspec = "%s/_parameters[]" % clone_run_id
+            origin = self.origin_ds_set.get_with_pathspec_index(pathspec)
+
+            if origin is None:
+                # This is just for usability: We could rerun the whole flow
+                # if an unknown clone_run_id is provided but probably this is
+                # not what the user intended, so raise a warning
+                raise MetaflowException(
+                    "Resume could not find run id *%s*" % clone_run_id
+                )
             else:
-                # Typical range fetch
-                range_str = "bytes=%d-%d" % (start, start + length - 1)
-        return url, range_str
-
-    def list_paths(self, keys: Optional[Iterable[str]] = None) -> List[S3Object]:
-        """
-        List the next level of paths in S3.
-
-        If multiple keys are specified, listings are done in parallel. The returned
-        S3Objects have `.exists == False` if the path refers to a prefix, not an
-        existing S3 object.
-
-        For instance, if the directory hierarchy is
-        ```
-        a/0.txt
-        a/b/1.txt
-        a/c/2.txt
-        a/d/e/3.txt
-        f/4.txt
-        ```
-        The `list_paths(['a', 'f'])` call returns
-        ```
-        a/0.txt (exists == True)
-        a/b/ (exists == False)
-        a/c/ (exists == False)
-        a/d/ (exists == False)
-        f/4.txt (exists == True)
-        ```
-
-        Parameters
-        ----------
-        keys : Iterable[str], optional
-            List of paths.
-
-        Returns
-        -------
-        List[`S3Object`]
-            S3Objects under the given paths, including prefixes (directories) that
-            do not correspond to leaf objects.
-        """
-
-        def _list(keys):
-            if keys is None:
-                keys = [None]
-            urls = ((self._url(key).rstrip("/") + "/", None) for key in keys)
-            res = self._read_many_files("list", urls)
-            for s3prefix, s3url, size in res:
-                if size:
-                    yield s3prefix, s3url, None, int(size)
-                else:
-                    yield s3prefix, s3url, None, None
+                return origin
+        else:
+            # all inputs must have the same foreach stack, so we can safely
+            # pick the first one
+            parent_pathspec = self.input_paths[0]
+            origin_parent_pathspec = self.clone_pathspec_mapping[parent_pathspec]
+            parent = self.origin_ds_set.get_with_pathspec(origin_parent_pathspec)
+            # Parent should be non-None since only clone the child if the parent
+            # was successfully cloned.
+            foreach_stack = parent["_foreach_stack"]
+            if join_type == "foreach":
+                # foreach-join pops the topmost index
+                index = ",".join(str(s.index) for s in foreach_stack[:-1])
+            elif self.split_index or self.ubf_context == UBF_CONTROL:
+                # foreach-split pushes a new index
+                index = ",".join(
+                    [str(s.index) for s in foreach_stack] + [str(self.split_index)]
+                )
+            else:
+                # all other transitions keep the parent's foreach stack intact
+                index = ",".join(str(s.index) for s in foreach_stack)
+            pathspec = "%s/%s[%s]" % (clone_run_id, self.step, index)
+            return self.origin_ds_set.get_with_pathspec_index(pathspec)
 
-        return list(starmap(S3Object, _list(keys)))
+    @property
+    def path(self):
+        return self._path
 
-    def list_recursive(self, keys: Optional[Iterable[str]] = None) -> List[S3Object]:
-        """
-        List all objects recursively under the given prefixes.
-
-        If multiple keys are specified, listings are done in parallel. All objects
-        returned have `.exists == True` as this call always returns leaf objects.
-
-        For instance, if the directory hierarchy is
-        ```
-        a/0.txt
-        a/b/1.txt
-        a/c/2.txt
-        a/d/e/3.txt
-        f/4.txt
-        ```
-        The `list_paths(['a', 'f'])` call returns
-        ```
-        a/0.txt (exists == True)
-        a/b/1.txt (exists == True)
-        a/c/2.txt (exists == True)
-        a/d/e/3.txt (exists == True)
-        f/4.txt (exists == True)
-        ```
-
-        Parameters
-        ----------
-        keys : Iterable[str], optional
-            List of paths.
-
-        Returns
-        -------
-        List[`S3Object`]
-            S3Objects under the given paths.
-        """
-
-        def _list(keys):
-            if keys is None:
-                keys = [None]
-            res = self._read_many_files(
-                "list", map(self._url_and_range, keys), recursive=True
+    @property
+    def results(self):
+        if self._results_ds:
+            return self._results_ds
+        else:
+            self._results_ds = self._flow_datastore.get_task_datastore(
+                self.run_id, self.step, self.task_id
             )
-            for s3prefix, s3url, size in res:
-                yield s3prefix, s3url, None, int(size)
-
-        return list(starmap(S3Object, _list(keys)))
+            return self._results_ds
 
-    def info(self, key: Optional[str] = None, return_missing: bool = False) -> S3Object:
-        """
-        Get metadata about a single object in S3.
-
-        This call makes a single `HEAD` request to S3 which can be
-        much faster than downloading all data with `get`.
-
-        Parameters
-        ----------
-        key : str, optional
-            Object to query. It can be an S3 url or a path suffix.
-        return_missing : bool, default: False
-            If set to True, do not raise an exception for a missing key but
-            return it as an `S3Object` with `.exists == False`.
-
-        Returns
-        -------
-        `S3Object`
-            An S3Object corresponding to the object requested. The object
-            will have `.downloaded == False`.
-        """
-
-        url = self._url(key)
-        src = urlparse(url)
-
-        def _info(s3, tmp):
-            resp = s3.head_object(Bucket=src.netloc, Key=src.path.lstrip('/"'))
-            return {
-                "content_type": resp["ContentType"],
-                "metadata": resp["Metadata"],
-                "size": resp["ContentLength"],
-                "last_modified": get_timestamp(resp["LastModified"]),
-            }
+    @property
+    def finished_id(self):
+        # note: id is not available before the task has finished
+        return (self.step, tuple(self.results["_foreach_stack"]))
 
-        info_results = None
-        try:
-            _, info_results = self._one_boto_op(_info, url, create_tmp_file=False)
-        except MetaflowS3NotFound:
-            if return_missing:
-                info_results = None
-            else:
-                raise
-        if info_results:
-            return S3Object(
-                self._s3root,
-                url,
-                path=None,
-                size=info_results["size"],
-                content_type=info_results["content_type"],
-                metadata=info_results["metadata"],
-                last_modified=info_results["last_modified"],
-            )
-        return S3Object(self._s3root, url, None)
+    @property
+    def is_cloned(self):
+        return self._is_cloned
 
-    def info_many(
-        self, keys: Iterable[str], return_missing: bool = False
-    ) -> List[S3Object]:
-        """
-        Get metadata about many objects in S3 in parallel.
-
-        This call makes a single `HEAD` request to S3 which can be
-        much faster than downloading all data with `get`.
-
-        Parameters
-        ----------
-        keys : Iterable[str]
-            Objects to query. Each key can be an S3 url or a path suffix.
-        return_missing : bool, default: False
-            If set to True, do not raise an exception for a missing key but
-            return it as an `S3Object` with `.exists == False`.
-
-        Returns
-        -------
-        List[`S3Object`]
-            A list of `S3Object`s corresponding to the paths requested. The
-            objects will have `.downloaded == False`.
-        """
+    @property
+    def wait_for_clone(self):
+        return self._wait_for_clone
 
-        def _head():
-            from . import s3op
+    def persist(self, flow):
+        # this is used to persist parameters before the start step
+        flow._task_ok = flow._success = True
+        flow._foreach_stack = []
+        self._ds.persist(flow)
+        self._ds.done()
 
-            res = self._read_many_files(
-                "info", map(self._url_and_range, keys), verbose=False, listing=True
-            )
+    def save_logs(self, logtype_to_logs):
+        self._ds.save_logs(RUNTIME_LOG_SOURCE, logtype_to_logs)
 
-            for s3prefix, s3url, fname in res:
-                if fname:
-                    # We have a metadata file to read from
-                    with open(os.path.join(self._tmpdir, fname), "r") as f:
-                        info = json.load(f)
-                    if info["error"] is not None:
-                        # We have an error, we check if it is a missing file
-                        if info["error"] == s3op.ERROR_URL_NOT_FOUND:
-                            if return_missing:
-                                yield self._s3root, s3url, None
-                            else:
-                                raise MetaflowS3NotFound()
-                        elif info["error"] == s3op.ERROR_URL_ACCESS_DENIED:
-                            raise MetaflowS3AccessDenied()
-                        else:
-                            raise MetaflowS3Exception("Got error: %d" % info["error"])
-                    else:
-                        yield self._s3root, s3url, None, info["size"], info[
-                            "content_type"
-                        ], info["metadata"], None, info["last_modified"]
-                else:
-                    # This should not happen; we should always get a response
-                    # even if it contains an error inside it
-                    raise MetaflowS3Exception("Did not get a response to HEAD")
+    def save_metadata(self, name, metadata):
+        self._ds.save_metadata({name: metadata})
 
-        return list(starmap(S3Object, _head()))
+    def __str__(self):
+        return " ".join(self._args)
 
-    def get(
-        self,
-        key: Optional[Union[str, S3GetObject]] = None,
-        return_missing: bool = False,
-        return_info: bool = True,
-    ) -> S3Object:
-        """
-        Get a single object from S3.
-
-        Parameters
-        ----------
-        key : str or `S3GetObject`, optional
-            Object to download. It can be an S3 url, a path suffix, or
-            an `S3GetObject` that defines a range of data to download. If None, or
-            not provided, gets the S3 root.
-        return_missing : bool, default: False
-            If set to True, do not raise an exception for a missing key but
-            return it as an `S3Object` with `.exists == False`.
-        return_info : bool, default: True
-            If set to True, fetch the content-type and user metadata associated
-            with the object at no extra cost, included for symmetry with `get_many`
-
-        Returns
-        -------
-        `S3Object`
-            An S3Object corresponding to the object requested.
-        """
-        url, r = self._url_and_range(key)
-        src = urlparse(url)
-
-        def _download(s3, tmp):
-            if r:
-                resp = s3.get_object(
-                    Bucket=src.netloc, Key=src.path.lstrip("/"), Range=r
-                )
-                # Format is bytes start-end/total; both start and end are inclusive so
-                # a 500 bytes file will be `bytes 0-499/500` for the entire file.
-                range_result = resp["ContentRange"]
-                range_result_match = RANGE_MATCH.match(range_result)
-                if range_result_match is None:
-                    raise RuntimeError(
-                        "Wrong format for ContentRange: %s" % str(range_result)
-                    )
-                range_result = RangeInfo(
-                    int(range_result_match.group("total")),
-                    request_offset=int(range_result_match.group("start")),
-                    request_length=int(range_result_match.group("end"))
-                    - int(range_result_match.group("start"))
-                    + 1,
-                )
-            else:
-                resp = s3.get_object(Bucket=src.netloc, Key=src.path.lstrip("/"))
-                range_result = None
-            sz = resp["ContentLength"]
-            if range_result is None:
-                range_result = RangeInfo(sz, request_offset=0, request_length=sz)
-            if not r and sz > DOWNLOAD_FILE_THRESHOLD:
-                # In this case, it is more efficient to use download_file as it
-                # will download multiple parts in parallel (it does it after
-                # multipart_threshold)
-                s3.download_file(src.netloc, src.path.lstrip("/"), tmp)
-            else:
-                with open(tmp, mode="wb") as t:
-                    read_in_chunks(t, resp["Body"], sz, DOWNLOAD_MAX_CHUNK)
-            if return_info:
-                return {
-                    "content_type": resp["ContentType"],
-                    "metadata": resp["Metadata"],
-                    "range_result": range_result,
-                    "last_modified": get_timestamp(resp["LastModified"]),
-                }
-            return None
 
-        addl_info = None
-        try:
-            path, addl_info = self._one_boto_op(_download, url)
-        except MetaflowS3NotFound:
-            if return_missing:
-                path = None
-            else:
-                raise
-        if addl_info:
-            return S3Object(
-                self._s3root,
-                url,
-                path,
-                content_type=addl_info["content_type"],
-                metadata=addl_info["metadata"],
-                range_info=addl_info["range_result"],
-                last_modified=addl_info["last_modified"],
-            )
-        return S3Object(self._s3root, url, path)
+class TaskFailed(MetaflowException):
+    headline = "Step failure"
 
-    def get_many(
-        self,
-        keys: Iterable[Union[str, S3GetObject]],
-        return_missing: bool = False,
-        return_info: bool = True,
-    ) -> List[S3Object]:
-        """
-        Get many objects from S3 in parallel.
-
-        Parameters
-        ----------
-        keys : Iterable[str or `S3GetObject`]
-            Objects to download. Each object can be an S3 url, a path suffix, or
-            an `S3GetObject` that defines a range of data to download.
-        return_missing : bool, default: False
-            If set to True, do not raise an exception for a missing key but
-            return it as an `S3Object` with `.exists == False`.
-        return_info : bool, default: True
-            If set to True, fetch the content-type and user metadata associated
-            with the object at no extra cost, included for symmetry with `get_many`.
-
-        Returns
-        -------
-        List[`S3Object`]
-            S3Objects corresponding to the objects requested.
-        """
-
-        def _get():
-            res = self._read_many_files(
-                "get",
-                map(self._url_and_range, keys),
-                allow_missing=return_missing,
-                verify=True,
-                verbose=False,
-                info=return_info,
-                listing=True,
-            )
+    def __init__(self, task, msg=""):
+        body = "Step *%s* (task-id %s) failed" % (task.step, task.task_id)
+        if msg:
+            body = "%s: %s" % (body, msg)
+        else:
+            body += "."
 
-            for s3prefix, s3url, fname in res:
-                if return_info:
-                    if fname:
-                        # We have a metadata file to read from
-                        with open(
-                            os.path.join(self._tmpdir, "%s_meta" % fname), "r"
-                        ) as f:
-                            info = json.load(f)
-                        range_info = info.get("range_result")
-                        if range_info:
-                            range_info = RangeInfo(
-                                range_info["total"],
-                                request_offset=range_info["start"],
-                                request_length=range_info["end"]
-                                - range_info["start"]
-                                + 1,
-                            )
-                        yield self._s3root, s3url, os.path.join(
-                            self._tmpdir, fname
-                        ), None, info["content_type"], info[
-                            "metadata"
-                        ], range_info, info[
-                            "last_modified"
-                        ]
-                    else:
-                        yield self._s3root, s3prefix, None
-                else:
-                    if fname:
-                        yield self._s3root, s3url, os.path.join(self._tmpdir, fname)
-                    else:
-                        # missing entries per return_missing=True
-                        yield self._s3root, s3prefix, None
+        super(TaskFailed, self).__init__(body)
 
-        return list(starmap(S3Object, _get()))
 
-    def get_recursive(
-        self, keys: Iterable[str], return_info: bool = False
-    ) -> List[S3Object]:
-        """
-        Get many objects from S3 recursively in parallel.
-
-        Parameters
-        ----------
-        keys : Iterable[str]
-            Prefixes to download recursively. Each prefix can be an S3 url or a path suffix
-            which define the root prefix under which all objects are downloaded.
-        return_info : bool, default: False
-            If set to True, fetch the content-type and user metadata associated
-            with the object.
-
-        Returns
-        -------
-        List[`S3Object`]
-            S3Objects stored under the given prefixes.
-        """
-
-        def _get():
-            res = self._read_many_files(
-                "get",
-                map(self._url_and_range, keys),
-                recursive=True,
-                verify=True,
-                verbose=False,
-                info=return_info,
-                listing=True,
-            )
+class TruncatedBuffer(object):
+    def __init__(self, name, maxsize):
+        self.name = name
+        self._maxsize = maxsize
+        self._buffer = BytesIO()
+        self._size = 0
+        self._eof = False
+
+    def write(self, bytedata, system_msg=False):
+        if system_msg:
+            self._buffer.write(bytedata)
+        elif not self._eof:
+            if self._size + len(bytedata) < self._maxsize:
+                self._buffer.write(bytedata)
+                self._size += len(bytedata)
+            else:
+                msg = b"[TRUNCATED - MAXIMUM LOG FILE SIZE REACHED]\n"
+                self._buffer.write(mflog_msg(msg))
+                self._eof = True
 
-            for s3prefix, s3url, fname in res:
-                if return_info:
-                    # We have a metadata file to read from
-                    with open(os.path.join(self._tmpdir, "%s_meta" % fname), "r") as f:
-                        info = json.load(f)
-                    range_info = info.get("range_result")
-                    if range_info:
-                        range_info = RangeInfo(
-                            range_info["total"],
-                            request_offset=range_info["start"],
-                            request_length=range_info["end"] - range_info["start"] + 1,
-                        )
-                    yield self._s3root, s3url, os.path.join(
-                        self._tmpdir, fname
-                    ), None, info["content_type"], info["metadata"], range_info, info[
-                        "last_modified"
-                    ]
-                else:
-                    yield s3prefix, s3url, os.path.join(self._tmpdir, fname)
+    def get_bytes(self):
+        return self._buffer.getvalue()
 
-        return list(starmap(S3Object, _get()))
+    def get_buffer(self):
+        self._buffer.seek(0)
+        return self._buffer
 
-    def get_all(self, return_info: bool = False) -> List[S3Object]:
-        """
-        Get all objects under the prefix set in the `S3` constructor.
-
-        This method requires that the `S3` object is initialized either with `run` or
-        `s3root`.
-
-        Parameters
-        ----------
-        return_info : bool, default: False
-            If set to True, fetch the content-type and user metadata associated
-            with the object.
-
-        Returns
-        -------
-        Iterable[`S3Object`]
-            S3Objects stored under the main prefix.
-        """
-
-        if self._s3root is None:
-            raise MetaflowS3URLException(
-                "Can't get_all() when S3 is initialized without a prefix"
-            )
-        else:
-            return self.get_recursive([None], return_info)
 
-    def put(
-        self,
-        key: Union[str, S3PutObject],
-        obj: PutValue,
-        overwrite: bool = True,
-        content_type: Optional[str] = None,
-        metadata: Optional[Dict[str, str]] = None,
-    ) -> str:
-        """
-        Upload a single object to S3.
-
-        Parameters
-        ----------
-        key : str or `S3PutObject`
-            Object path. It can be an S3 url or a path suffix.
-        obj : bytes or str
-            An object to store in S3. Strings are converted to UTF-8 encoding.
-        overwrite : bool, default: True
-            Overwrite the object if it exists. If set to False, the operation
-            succeeds without uploading anything if the key already exists.
-        content_type : str, optional
-            Optional MIME type for the object.
-        metadata : Dict, optional
-            A JSON-encodable dictionary of additional headers to be stored
-            as metadata with the object.
-
-        Returns
-        -------
-        str
-            URL of the object stored.
-        """
-
-        if isinstance(obj, (RawIOBase, BufferedIOBase)):
-            if not obj.readable() or not obj.seekable():
-                raise MetaflowS3InvalidObject(
-                    "Object corresponding to the key '%s' is not readable or seekable"
-                    % key
-                )
-            blob = obj
-        else:
-            if not is_stringish(obj):
-                raise MetaflowS3InvalidObject(
-                    "Object corresponding to the key '%s' is not a string "
-                    "or a bytes object." % key
-                )
-            blob = to_fileobj(obj)
-        # We override the close functionality to prevent closing of the
-        # file if it is used multiple times when uploading (since upload_fileobj
-        # will/may close it on failure)
-        real_close = blob.close
-        blob.close = lambda: None
-
-        url = self._url(key)
-        src = urlparse(url)
-        extra_args = None
-        if content_type or metadata:
-            extra_args = {}
-            if content_type:
-                extra_args["ContentType"] = content_type
-            if metadata:
-                extra_args["Metadata"] = {
-                    "metaflow-user-attributes": json.dumps(metadata)
-                }
+class CLIArgs(object):
+    """
+    Container to allow decorators modify the command line parameters
+    for step execution in StepDecorator.runtime_step_cli().
+    """
 
-        def _upload(s3, _):
-            # We make sure we are at the beginning in case we are retrying
-            blob.seek(0)
-            s3.upload_fileobj(
-                blob, src.netloc, src.path.lstrip("/"), ExtraArgs=extra_args
-            )
+    def __init__(self, task):
+        self.task = task
+        self.entrypoint = list(task.entrypoint)
+        self.top_level_options = {
+            "quiet": True,
+            "metadata": self.task.metadata_type,
+            "environment": self.task.environment_type,
+            "datastore": self.task.datastore_type,
+            "pylint": False,
+            "event-logger": self.task.event_logger_type,
+            "monitor": self.task.monitor_type,
+            "datastore-root": self.task.datastore_sysroot,
+            "with": [
+                deco.make_decorator_spec()
+                for deco in self.task.decos
+                if not deco.statically_defined
+            ],
+        }
+
+        # FlowDecorators can define their own top-level options. They are
+        # responsible for adding their own top-level options and values through
+        # the get_top_level_options() hook.
+        for deco in flow_decorators():
+            self.top_level_options.update(deco.get_top_level_options())
+
+        self.commands = ["step"]
+        self.command_args = [self.task.step]
+        self.command_options = {
+            "run-id": task.run_id,
+            "task-id": task.task_id,
+            "input-paths": compress_list(task.input_paths),
+            "split-index": task.split_index,
+            "retry-count": task.retries,
+            "max-user-code-retries": task.user_code_retries,
+            "tag": task.tags,
+            "namespace": get_namespace() or "",
+            "ubf-context": task.ubf_context,
+        }
+        self.env = {}
+
+    def get_args(self):
+
+        # TODO: Make one with dict_to_cli_options; see cli_args.py for more detail
+        def _options(mapping):
+            for k, v in mapping.items():
+
+                # None or False arguments are ignored
+                # v needs to be explicitly False, not falsy, e.g. 0 is an acceptable value
+                if v is None or v is False:
+                    continue
+
+                # we need special handling for 'with' since it is a reserved
+                # keyword in Python, so we call it 'decospecs' in click args
+                if k == "decospecs":
+                    k = "with"
+                k = k.replace("_", "-")
+                v = v if isinstance(v, (list, tuple, set)) else [v]
+                for value in v:
+                    yield "--%s" % k
+                    if not isinstance(value, bool):
+                        yield to_unicode(value)
+
+        args = list(self.entrypoint)
+        args.extend(_options(self.top_level_options))
+        args.extend(self.commands)
+        args.extend(self.command_args)
+        args.extend(_options(self.command_options))
+        return args
 
-        if overwrite:
-            self._one_boto_op(_upload, url, create_tmp_file=False)
-            real_close()
-            return url
-        else:
+    def get_env(self):
+        return self.env
 
-            def _head(s3, _):
-                s3.head_object(Bucket=src.netloc, Key=src.path.lstrip("/"))
+    def __str__(self):
+        return " ".join(self.get_args())
 
-            try:
-                self._one_boto_op(_head, url, create_tmp_file=False)
-            except MetaflowS3NotFound:
-                self._one_boto_op(_upload, url, create_tmp_file=False)
-            finally:
-                real_close()
-            return url
 
-    def put_many(
-        self,
-        key_objs: List[Union[Tuple[str, PutValue], S3PutObject]],
-        overwrite: bool = True,
-    ) -> List[Tuple[str, str]]:
-        """
-        Upload many objects to S3.
-
-        Each object to be uploaded can be specified in two ways:
-
-        1. As a `(key, obj)` tuple where `key` is a string specifying
-           the path and `obj` is a string or a bytes object.
-
-        2. As a `S3PutObject` which contains additional metadata to be
-           stored with the object.
-
-        Parameters
-        ----------
-        key_objs : List[(str, str) or `S3PutObject`]
-            List of key-object pairs to upload.
-        overwrite : bool, default : True
-            Overwrite the object if it exists. If set to False, the operation
-            succeeds without uploading anything if the key already exists.
-
-        Returns
-        -------
-        List[(str, str)]
-            List of `(key, url)` pairs corresponding to the objects uploaded.
-        """
-
-        def _store():
-            for key_obj in key_objs:
-                if isinstance(key_obj, tuple):
-                    key = key_obj[0]
-                    obj = key_obj[1]
-                else:
-                    key = key_obj.key
-                    obj = key_obj.value
-                store_info = {
-                    "key": key,
-                    "content_type": getattr(key_obj, "content_type", None),
-                }
-                metadata = getattr(key_obj, "metadata", None)
-                if metadata:
-                    store_info["metadata"] = {
-                        "metaflow-user-attributes": json.dumps(metadata)
-                    }
-                if isinstance(obj, (RawIOBase, BufferedIOBase)):
-                    if not obj.readable() or not obj.seekable():
-                        raise MetaflowS3InvalidObject(
-                            "Object corresponding to the key '%s' is not readable or seekable"
-                            % key
-                        )
-                else:
-                    if not is_stringish(obj):
-                        raise MetaflowS3InvalidObject(
-                            "Object corresponding to the key '%s' is not a string "
-                            "or a bytes object." % key
-                        )
-                    obj = to_fileobj(obj)
-                with NamedTemporaryFile(
-                    dir=self._tmpdir,
-                    delete=False,
-                    mode="wb",
-                    prefix="metaflow.s3.put_many.",
-                ) as tmp:
-                    tmp.write(obj.read())
-                    tmp.close()
-                    yield tmp.name, self._url(key), store_info
+class Worker(object):
+    def __init__(self, task, max_logs_size):
 
-        return self._put_many_files(_store(), overwrite)
+        self.task = task
+        self._proc = self._launch()
 
-    def put_files(
-        self,
-        key_paths: List[Union[Tuple[str, PutValue], S3PutObject]],
-        overwrite: bool = True,
-    ) -> List[Tuple[str, str]]:
-        """
-        Upload many local files to S3.
-
-        Each file to be uploaded can be specified in two ways:
-
-        1. As a `(key, path)` tuple where `key` is a string specifying
-           the S3 path and `path` is the path to a local file.
-
-        2. As a `S3PutObject` which contains additional metadata to be
-           stored with the file.
-
-        Parameters
-        ----------
-        key_paths : List[(str, str) or `S3PutObject`]
-            List of files to upload.
-        overwrite : bool, default: True
-            Overwrite the object if it exists. If set to False, the operation
-            succeeds without uploading anything if the key already exists.
-
-        Returns
-        -------
-        List[(str, str)]
-            List of `(key, url)` pairs corresponding to the files uploaded.
-        """
-
-        def _check():
-            for key_path in key_paths:
-                if isinstance(key_path, tuple):
-                    key = key_path[0]
-                    path = key_path[1]
-                else:
-                    key = key_path.key
-                    path = key_path.path
-                store_info = {
-                    "key": key,
-                    "content_type": getattr(key_path, "content_type", None),
-                }
-                metadata = getattr(key_path, "metadata", None)
-                if metadata:
-                    store_info["metadata"] = {
-                        "metaflow-user-attributes": json.dumps(metadata)
-                    }
-                if not os.path.exists(path):
-                    raise MetaflowS3NotFound("Local file not found: %s" % path)
-                yield path, self._url(key), store_info
-
-        return self._put_many_files(_check(), overwrite)
-
-    def _one_boto_op(self, op, url, create_tmp_file=True):
-        error = ""
-        for i in range(S3_RETRY_COUNT + 1):
-            tmp = None
-            if create_tmp_file:
-                tmp = NamedTemporaryFile(
-                    dir=self._tmpdir, prefix="metaflow.s3.one_file.", delete=False
-                )
-            try:
-                side_results = op(self._s3_client.client, tmp.name if tmp else None)
-                return tmp.name if tmp else None, side_results
-            except self._s3_client.error as err:
-                from . import s3op
-
-                error_code = s3op.normalize_client_error(err)
-                if error_code == 404:
-                    raise MetaflowS3NotFound(url)
-                elif error_code == 403:
-                    raise MetaflowS3AccessDenied(url)
-                elif error_code == 416:
-                    raise MetaflowS3InvalidRange(err)
-                elif error_code == "NoSuchBucket":
-                    raise MetaflowS3URLException("Specified S3 bucket doesn't exist.")
-                error = str(err)
-            except Exception as ex:
-                # TODO specific error message for out of disk space
-                error = str(ex)
-            if tmp:
-                os.unlink(tmp.name)
-            self._s3_client.reset_client()
-            # only sleep if retries > 0
-            if S3_RETRY_COUNT > 0:
-                self._jitter_sleep(i)
-        raise MetaflowS3Exception(
-            "S3 operation failed.\n" "Key requested: %s\n" "Error: %s" % (url, error)
-        )
-
-    # add some jitter to make sure retries are not synchronized
-    def _jitter_sleep(self, trynum, multiplier=2):
-        interval = multiplier**trynum + random.randint(0, 10)
-        time.sleep(interval)
-
-    # NOTE: re: _read_many_files and _put_many_files
-    # All file IO is through binary files - we write bytes, we read
-    # bytes. All inputs and outputs from these functions are Unicode.
-    # Conversion between bytes and unicode is done through
-    # and url_unquote.
-    def _read_many_files(self, op, prefixes_and_ranges, **options):
-        prefixes_and_ranges = list(prefixes_and_ranges)
-        with NamedTemporaryFile(
-            dir=self._tmpdir,
-            mode="wb",
-            delete=not debug.s3client,
-            prefix="metaflow.s3.inputs.",
-        ) as inputfile:
-            inputfile.write(
-                b"\n".join(
-                    [
-                        b" ".join([url_quote(prefix)] + ([url_quote(r)] if r else []))
-                        for prefix, r in prefixes_and_ranges
-                    ]
-                )
+        if task.retries > task.user_code_retries:
+            self.task.log(
+                "Task fallback is starting to handle the failure.",
+                system_msg=True,
+                pid=self._proc.pid,
             )
-            inputfile.flush()
-            stdout_lines, stderr = self._s3op_with_retries(
-                op, inputs=inputfile.name, **options
+        elif not task.is_cloned:
+            suffix = " (retry)." if task.retries else "."
+            self.task.log(
+                "Task is starting" + suffix, system_msg=True, pid=self._proc.pid
             )
-            if stderr:
-                raise MetaflowS3Exception(
-                    "Getting S3 files failed.\n"
-                    "First prefix requested: %s\n"
-                    "Error: %s" % (prefixes_and_ranges[0], stderr)
-                )
-            else:
-                for line in stdout_lines:
-                    yield tuple(map(url_unquote, line.strip(b"\n").split(b" ")))
 
-    def _put_many_files(self, url_info, overwrite):
-        url_info = list(url_info)
-        url_dicts = [
-            dict(
-                chain([("local", os.path.realpath(local)), ("url", url)], info.items())
-            )
-            for local, url, info in url_info
-        ]
+        self._stdout = TruncatedBuffer("stdout", max_logs_size)
+        self._stderr = TruncatedBuffer("stderr", max_logs_size)
 
-        with NamedTemporaryFile(
-            dir=self._tmpdir,
-            mode="wb",
-            delete=not debug.s3client,
-            prefix="metaflow.s3.put_inputs.",
-        ) as inputfile:
-            lines = [to_bytes(json.dumps(x)) for x in url_dicts]
-            inputfile.write(b"\n".join(lines))
-            inputfile.flush()
-            stdout_lines, stderr = self._s3op_with_retries(
-                "put",
-                inputs=inputfile.name,
-                verbose=False,
-                overwrite=overwrite,
-                listing=True,
-            )
-            if stderr:
-                raise MetaflowS3Exception(
-                    "Uploading S3 files failed.\n"
-                    "First key: %s\n"
-                    "Error: %s" % (url_info[0][2]["key"], stderr)
+        self._logs = {
+            self._proc.stderr.fileno(): (self._proc.stderr, self._stderr),
+            self._proc.stdout.fileno(): (self._proc.stdout, self._stdout),
+        }
+
+        self._encoding = sys.stdout.encoding or "UTF-8"
+        self.killed = False  # Killed indicates that the task was forcibly killed
+        # with SIGKILL by the master process.
+        # A killed task is always considered cleaned
+        self.cleaned = False  # A cleaned task is one that is shutting down and has been
+        # noticed by the runtime and queried for its state (whether or
+        # not it is properly shut down)
+
+    def _launch(self):
+        args = CLIArgs(self.task)
+        env = dict(os.environ)
+
+        if self.task.clone_run_id:
+            args.command_options["clone-run-id"] = self.task.clone_run_id
+
+        if self.task.is_cloned and self.task.clone_origin:
+            args.command_options["clone-only"] = self.task.clone_origin
+            # disabling sidecars for cloned tasks due to perf reasons
+            args.top_level_options["event-logger"] = "nullSidecarLogger"
+            args.top_level_options["monitor"] = "nullSidecarMonitor"
+            if self.task.wait_for_clone:
+                args.command_options["clone-wait-only"] = True
+        else:
+            # decorators may modify the CLIArgs object in-place
+            for deco in self.task.decos:
+                deco.runtime_step_cli(
+                    args,
+                    self.task.retries,
+                    self.task.user_code_retries,
+                    self.task.ubf_context,
                 )
-            else:
-                urls = set()
-                for line in stdout_lines:
-                    url, _, _ = map(url_unquote, line.strip(b"\n").split(b" "))
-                    urls.add(url)
-                return [(info["key"], url) for _, url, info in url_info if url in urls]
-
-    def _s3op_with_retries(self, mode, **options):
-        from . import s3op
-
-        # High level note on what this function does:
-        #  - perform s3op (which calls s3op.py in a subprocess to parallelize the
-        #    operation). Typically this operation has several inputs (for example,
-        #    multiple files to get or put)
-        #  - the result of this operation can be either:
-        #    - a known permanent failure (access denied for example) in which case we
-        #      return this failure.
-        #    - a known transient failure (SlowDown for example) in which case we will
-        #      retry *only* the inputs that have this transient failure.
-        #    - an unknown failure (something went wrong but we cannot say if it was
-        #      a known permanent failure or something else). In this case, we retry
-        #      the operation completely.
-        #
-        # There are therefore two retry counts:
-        #  - the transient failure retry count: how many times do we try on known
-        #    transient errors
-        #  - the top-level retry count: how many times do we try on unknown failures
-        #
-        # Note that, if the operation runs out of transient failure retries, it will
-        # count as an "unknown" failure (ie: it will be retried according to the
-        # outer top-level retry count). In other words, you can potentially have
-        # transient_retry_count * retry_count tries).
-        # Finally, if on transient failures, we make NO progress (ie: no input is
-        # successfully processed), that counts as an "unknown" failure.
-        cmdline = [sys.executable, os.path.abspath(s3op.__file__), mode]
-        recursive_get = False
-        for key, value in options.items():
-            key = key.replace("_", "-")
-            if isinstance(value, bool):
-                if value:
-                    if mode == "get" and key == "recursive":
-                        # We make a note of this because for transient retries, we
-                        # don't pass the recursive flag since we already did all the
-                        # listing we needed
-                        recursive_get = True
-                    else:
-                        cmdline.append("--%s" % key)
-                else:
-                    cmdline.append("--no-%s" % key)
-            elif key == "inputs":
-                base_input_filename = value
-            else:
-                cmdline.extend(("--%s" % key, value))
-        if self._s3_role is not None:
-            cmdline.extend(("--s3role", self._s3_role))
-        if self._s3_session_vars is not None:
-            cmdline.extend(("--s3sessionvars", json.dumps(self._s3_session_vars)))
-        if self._s3_client_params is not None:
-            cmdline.extend(("--s3clientparams", json.dumps(self._s3_client_params)))
-
-        def _inject_failure_rate():
-            # list mode does not do retries on transient failures (there is no
-            # SlowDown handling) so we never inject a failure rate
-            if mode == "list":
-                return 0
-            # Otherwise, we cap the failure rate at 90%
-            return min(90, self._s3_inject_failures)
-
-        retry_count = 0  # Number of retries (excluding transient failures)
-        transient_retry_count = 0  # Number of transient retries (per top-level retry)
-        inject_failures = _inject_failure_rate()
-        out_lines = []  # List to contain the lines returned by _s3op_with_retries
-        pending_retries = (
-            []
-        )  # Inputs that need to be retried due to a transient failure
-        loop_count = 0
-        last_ok_count = 0  # Number of inputs that were successful in the last try
-        total_ok_count = 0  # Total number of OK inputs
-
-        def _reset():
-            nonlocal transient_retry_count, inject_failures, out_lines, pending_retries
-            nonlocal loop_count, last_ok_count, total_ok_count
-            transient_retry_count = 0
-            inject_failures = _inject_failure_rate()
-            if mode != "put":
-                # For put, even after retries, we keep around whatever we already
-                # uploaded. This is because uploading with overwrite=False is not
-                # an idempotent operation and so some files could be uploaded during
-                # the first try which we should report back.
-                out_lines = []
-            pending_retries = []
-            loop_count = 0
-            last_ok_count = 0
-            total_ok_count = 0  # Reset to zero even if we keep out_lines
-
-        def _update_out_lines(out_lines, ok_lines, resize=False):
-            if resize:
-                # This is the first time around; we make the list big enough. Typically,
-                # there is nothing in out_lines but in some cases (a retry after a
-                # partial result), there may be stuff in it
-                out_lines.extend([None] * (len(ok_lines) - len(out_lines)))
-            for l in ok_lines:
-                idx, rest = l.split(b" ", maxsplit=1)
-                if rest.decode(encoding="utf-8") != TRANSIENT_RETRY_LINE_CONTENT:
-                    # Update the proper location in the out_lines array; we maintain
-                    # position as if transient retries did not exist. This
-                    # makes sure that order is respected even in the presence of
-                    # transient retries.
-                    out_lines[int(idx.decode(encoding="utf-8"))] = rest
-
-        def try_s3_op(last_ok_count, pending_retries, out_lines, inject_failures):
-            # NOTE: Make sure to update pending_retries and out_lines in place
-            addl_cmdline = []
-            if len(pending_retries) == 0 and recursive_get:
-                # First time around (or after a fatal failure)
-                addl_cmdline = ["--recursive"]
-            with NamedTemporaryFile(
-                dir=self._tmpdir,
-                mode="wb+",
-                delete=not debug.s3client,
-                prefix="metaflow.s3op.stderr.",
-            ) as stderr:
-                with NamedTemporaryFile(
-                    dir=self._tmpdir,
-                    mode="wb",
-                    delete=not debug.s3client,
-                    prefix="metaflow.s3op.transientretry.",
-                ) as tmp_input:
-                    if len(pending_retries) > 0:
-                        # We try a little bit more than the previous success (to still
-                        # be aggressive but not too much). If there is a lot of
-                        # transient errors and we are having issues pushing through
-                        # things, this will shrink more and more until we are doing a
-                        # single operation at a time. If things start going better, it
-                        # will increase by 20% every round.
-                        max_count = min(int(last_ok_count * 1.2), len(pending_retries))
-                        tmp_input.writelines(pending_retries[:max_count])
-                        tmp_input.flush()
-                        debug.s3client_exec(
-                            "Have %d pending; succeeded in %d => trying for %d and "
-                            "leaving %d for the next round"
-                            % (
-                                len(pending_retries),
-                                last_ok_count,
-                                max_count,
-                                len(pending_retries) - max_count,
-                            )
-                        )
-                        del pending_retries[:max_count]
+        env.update(args.get_env())
+        env["PYTHONUNBUFFERED"] = "x"
+        # NOTE bufsize=1 below enables line buffering which is required
+        # by read_logline() below that relies on readline() not blocking
+        # print('running', args)
+        cmdline = args.get_args()
+        debug.subcommand_exec(cmdline)
+        return subprocess.Popen(
+            cmdline,
+            env=env,
+            bufsize=1,
+            stdin=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            stdout=subprocess.PIPE,
+        )
 
-                        input_filename = tmp_input.name
-                    else:
-                        input_filename = base_input_filename
+    def emit_log(self, msg, buf, system_msg=False):
+        if mflog.is_structured(msg):
+            res = mflog.parse(msg)
+            if res:
+                # parsing successful
+                plain = res.msg
+                timestamp = res.utc_tstamp
+                if res.should_persist:
+                    # in special circumstances we may receive structured
+                    # loglines that haven't been properly persisted upstream.
+                    # This is the case if, for example, a task crashes in an external
+                    # system and we retrieve the remaining logs after the crash.
+                    # Those lines are marked with a special tag, should_persist,
+                    # which we process here
+                    buf.write(mflog.unset_should_persist(msg))
+            else:
+                # parsing failed, corrupted logline. Print it as-is
+                timestamp = datetime.utcnow()
+                plain = msg
+        else:
+            # If the line isn't formatted with mflog already, we format it here.
+            plain = msg
+            timestamp = datetime.utcnow()
+            # store unformatted loglines in the buffer that will be
+            # persisted, assuming that all previously formatted loglines have
+            # been already persisted at the source.
+            buf.write(mflog_msg(msg, now=timestamp), system_msg=system_msg)
+        text = plain.strip().decode(self._encoding, errors="replace")
+        self.task.log(
+            text,
+            pid=self._proc.pid,
+            timestamp=mflog.utc_to_local(timestamp),
+            system_msg=system_msg,
+        )
 
-                    addl_cmdline.extend(["--inputs", input_filename])
+    def read_logline(self, fd):
+        fileobj, buf = self._logs[fd]
+        # readline() below should never block thanks to polling and
+        # line buffering. If it does, things will deadlock
+        line = fileobj.readline()
+        if line:
+            self.emit_log(line, buf)
+            return True
+        else:
+            return False
 
-                    # Check if we want to inject failures (for testing)
-                    if inject_failures > 0:
-                        addl_cmdline.extend(["--inject-failure", str(inject_failures)])
-                        # Logic here is to have higher and lower failure rates to try to
-                        # exercise as much of the code as possible. The failure rate
-                        # trends towards 0.
-                        if loop_count % 2 == 0:
-                            inject_failures = int(inject_failures / 3)
-                        else:
-                            # We cap at 90 (and not 100) for injection of failures to
-                            # reduce the likelihood of having flaky test. If the
-                            # failure injection rate is too high, this can cause actual
-                            # retries more often and then lead to too many actual
-                            # retries
-                            inject_failures = min(90, int(inject_failures * 1.5))
-                    try:
-                        debug.s3client_exec(cmdline + addl_cmdline)
-                        # Run the operation.
-                        stdout = subprocess.check_output(
-                            cmdline + addl_cmdline,
-                            cwd=self._tmpdir,
-                            stderr=stderr.file,
-                        )
-                        # Here we did not have any error -- transient or otherwise.
-                        ok_lines = stdout.splitlines()
-                        _update_out_lines(out_lines, ok_lines, resize=loop_count == 0)
-                        return (len(ok_lines), 0, inject_failures, None)
-                    except subprocess.CalledProcessError as ex:
-                        if ex.returncode == s3op.ERROR_TRANSIENT:
-                            # In this special case, we failed transiently on *some* of
-                            # the files but not necessarily all. This is typically
-                            # caused by limits on the number of operations that can
-                            # occur per second or some other temporary limitation.
-                            # We will retry only those that we failed on and we will not
-                            # count this as a retry *unless* we are making no forward
-                            # progress. In effect, we consider that as long as *some*
-                            # operations are going through, we should just keep going as
-                            # if it was a single operation.
-                            ok_lines = ex.stdout.splitlines()
-                            stderr.seek(0)
-                            do_output = False
-                            retry_lines = []
-                            for l in stderr:
-                                if do_output:
-                                    retry_lines.append(l)
-                                    continue
-                                if (
-                                    l.decode(encoding="utf-8")
-                                    == "%s\n" % TRANSIENT_RETRY_START_LINE
-                                ):
-                                    # Look for a special marker as the start of the
-                                    # "failed inputs that need to be retried"
-                                    do_output = True
-                            stderr.seek(0)
-                            if do_output is False:
-                                return (
-                                    0,
-                                    0,
-                                    inject_failures,
-                                    "Could not find inputs to retry",
-                                )
-                            else:
-                                _update_out_lines(
-                                    out_lines, ok_lines, resize=loop_count == 0
-                                )
-                                pending_retries.extend(retry_lines)
+    def fds(self):
+        return (self._proc.stderr.fileno(), self._proc.stdout.fileno())
 
-                                return (
-                                    len(ok_lines),
-                                    len(retry_lines),
-                                    inject_failures,
-                                    None,
-                                )
+    def clean(self):
+        if self.killed:
+            return True
+        if not self.cleaned:
+            for fileobj, buf in self._logs.values():
+                msg = b"[KILLED BY ORCHESTRATOR]\n"
+                self.emit_log(msg, buf, system_msg=True)
+            self.cleaned = True
+        return self._proc.poll() is not None
 
-                        # Here, this is a "normal" failure that we need to send back up.
-                        # These failures are not retried.
-                        stderr.seek(0)
-                        err_out = stderr.read().decode("utf-8", errors="replace")
-                        stderr.seek(0)
-                        if ex.returncode == s3op.ERROR_URL_NOT_FOUND:
-                            raise MetaflowS3NotFound(err_out)
-                        elif ex.returncode == s3op.ERROR_URL_ACCESS_DENIED:
-                            raise MetaflowS3AccessDenied(err_out)
-                        elif ex.returncode == s3op.ERROR_INVALID_RANGE:
-                            raise MetaflowS3InvalidRange(err_out)
-
-                        # Here, this is some other error that we will retry. We still
-                        # update the successful lines
-                        ok_lines = ex.stdout.splitlines()
-                        _update_out_lines(out_lines, ok_lines, resize=loop_count == 0)
-                        return 0, 0, inject_failures, err_out
-
-        while retry_count <= S3_RETRY_COUNT:
-            (
-                last_ok_count,
-                last_retry_count,
-                inject_failures,
-                err_out,
-            ) = try_s3_op(last_ok_count, pending_retries, out_lines, inject_failures)
-            if err_out or (
-                last_retry_count != 0
-                and (
-                    last_ok_count == 0
-                    or transient_retry_count > S3_TRANSIENT_RETRY_COUNT
-                )
-            ):
-                # We had a fatal failure (err_out is not None)
-                # or we made no progress (last_ok_count is 0)
-                # or we are out of transient retries
-                # so we will restart from scratch (being very conservative)
-                retry_count += 1
-                err_msg = err_out
-                if err_msg is None and last_ok_count == 0:
-                    err_msg = "No progress"
-                if err_msg is None:
-                    err_msg = "Too many transient errors"
-                print(
-                    "S3 non-transient error (attempt #%d): %s" % (retry_count, err_msg)
-                )
-                _reset()
-                if retry_count <= S3_RETRY_COUNT:
-                    self._jitter_sleep(retry_count)
-                continue
-            elif last_retry_count != 0:
-                # During our last try, we did not manage to process everything we wanted
-                # due to a transient failure so we try again.
-                transient_retry_count += 1
-                total_ok_count += last_ok_count
-                print(
-                    "Transient S3 failure (attempt #%d) -- total success: %d, "
-                    "last attempt %d/%d -- remaining: %d"
-                    % (
-                        transient_retry_count,
-                        total_ok_count,
-                        last_ok_count,
-                        last_ok_count + last_retry_count,
-                        len(pending_retries),
+    def kill(self):
+        if not self.killed:
+            try:
+                self._proc.kill()
+            except:
+                pass
+            self.cleaned = True
+            self.killed = True
+
+    def terminate(self):
+        # this shouldn't block, since terminate() is called only
+        # after the poller has decided that the worker is dead
+        returncode = self._proc.wait()
+
+        # consume all remaining loglines
+        # we set the file descriptor to be non-blocking, since
+        # the pipe may stay active due to subprocesses launched by
+        # the worker, e.g. sidecars, so we can't rely on EOF. We try to
+        # read just what's available in the pipe buffer
+        for fileobj, buf in self._logs.values():
+            fileno = fileobj.fileno()
+            fcntl.fcntl(fileno, fcntl.F_SETFL, os.O_NONBLOCK)
+            try:
+                while self.read_logline(fileno):
+                    pass
+            except:
+                # ignore "resource temporarily unavailable" etc. errors
+                # caused due to non-blocking. Draining is done on a
+                # best-effort basis.
+                pass
+
+        # Return early if the task is cloned since we don't want to
+        # perform any log collection.
+        if not self.task.is_cloned:
+            self.task.save_metadata(
+                "runtime",
+                {
+                    "return_code": returncode,
+                    "killed": self.killed,
+                    "success": returncode == 0,
+                },
+            )
+            if returncode:
+                if not self.killed:
+                    if returncode == -11:
+                        self.emit_log(
+                            b"Task failed with a segmentation fault.",
+                            self._stderr,
+                            system_msg=True,
+                        )
+                    else:
+                        self.emit_log(b"Task failed.", self._stderr, system_msg=True)
+            else:
+                num = self.task.results["_foreach_num_splits"]
+                if num:
+                    self.task.log(
+                        "Foreach yields %d child steps." % num,
+                        system_msg=True,
+                        pid=self._proc.pid,
                     )
+                self.task.log(
+                    "Task finished successfully.", system_msg=True, pid=self._proc.pid
                 )
-                if inject_failures == 0:
-                    # Don't sleep when we are "faking" the failures
-                    self._jitter_sleep(transient_retry_count)
-
-            loop_count += 1
-            # If we have no more things to try, we break out of the loop.
-            if len(pending_retries) == 0:
-                break
-
-        # At this point, we check out_lines; strip None which can happen for puts that
-        # didn't upload files
-        return [o for o in out_lines if o is not None], err_out
+            self.task.save_logs(
+                {
+                    "stdout": self._stdout.get_buffer(),
+                    "stderr": self._stderr.get_buffer(),
+                }
+            )
+
+        return returncode
+
+    def __str__(self):
+        return "Worker[%d]: %s" % (self._proc.pid, self.task.path)
```

### Comparing `metaflow-2.8.3/metaflow/plugins/datatools/s3/s3op.py` & `metaflow-2.8.4/metaflow/plugins/datatools/s3/s3op.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/datatools/s3/s3tail.py` & `metaflow-2.8.4/metaflow/plugins/datatools/s3/s3tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/datatools/s3/s3util.py` & `metaflow-2.8.4/metaflow/plugins/datatools/s3/s3util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/debug_logger.py` & `metaflow-2.8.4/metaflow/plugins/debug_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/debug_monitor.py` & `metaflow-2.8.4/metaflow/plugins/debug_monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/__init__.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/client.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/client_modules.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/client_modules.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/communication/bytestream.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/communication/bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/communication/channel.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/communication/channel.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/communication/socket_bytestream.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/communication/socket_bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/communication/utils.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/communication/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/consts.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/consts.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/data_transferer.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/data_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/exception_transferer.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/exception_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/override_decorators.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/override_decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/server.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/server.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/stub.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/stub.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/env_escape/utils.py` & `metaflow-2.8.4/metaflow/plugins/env_escape/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/environment_decorator.py` & `metaflow-2.8.4/metaflow/plugins/environment_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/frameworks/pytorch.py` & `metaflow-2.8.4/metaflow/plugins/frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/gcp/gs_storage_client_factory.py` & `metaflow-2.8.4/metaflow/plugins/gcp/gs_storage_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/gcp/gs_tail.py` & `metaflow-2.8.4/metaflow/plugins/gcp/gs_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/gcp/gs_utils.py` & `metaflow-2.8.4/metaflow/plugins/gcp/gs_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/gcp/includefile_support.py` & `metaflow-2.8.4/metaflow/plugins/gcp/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes.py` & `metaflow-2.8.4/metaflow/plugins/kubernetes/kubernetes.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,38 +3,39 @@
 import os
 import shlex
 import time
 
 from metaflow import current, util
 from metaflow.exception import MetaflowException
 from metaflow.metaflow_config import (
-    SERVICE_HEADERS,
-    SERVICE_INTERNAL_URL,
+    ARGO_EVENTS_WEBHOOK_URL,
+    AWS_SECRETS_MANAGER_DEFAULT_REGION,
+    AZURE_STORAGE_BLOB_SERVICE_ENDPOINT,
+    CARD_AZUREROOT,
+    CARD_GSROOT,
     CARD_S3ROOT,
+    DATASTORE_SYSROOT_AZURE,
+    DATASTORE_SYSROOT_GS,
     DATASTORE_SYSROOT_S3,
     DATATOOLS_S3ROOT,
     DEFAULT_AWS_CLIENT_PROVIDER,
     DEFAULT_METADATA,
+    DEFAULT_SECRETS_BACKEND_TYPE,
     KUBERNETES_SANDBOX_INIT_SCRIPT,
     KUBERNETES_FETCH_EC2_METADATA,
     S3_ENDPOINT_URL,
-    AZURE_STORAGE_BLOB_SERVICE_ENDPOINT,
-    DATASTORE_SYSROOT_AZURE,
-    CARD_AZUREROOT,
-    CARD_GSROOT,
-    DATASTORE_SYSROOT_GS,
-    DEFAULT_SECRETS_BACKEND_TYPE,
-    AWS_SECRETS_MANAGER_DEFAULT_REGION,
+    SERVICE_HEADERS,
+    SERVICE_INTERNAL_URL,
 )
 from metaflow.mflog import (
     BASH_SAVE_LOGS,
     bash_capture_logs,
     export_mflog_env_vars,
-    tail_logs,
     get_log_tailer,
+    tail_logs,
 )
 
 from .kubernetes_client import KubernetesClient
 
 # Redirect structured logs to $PWD/.logs/
 LOGS_DIR = "$PWD/.logs"
 STDOUT_FILE = "mflog_stdout"
@@ -145,19 +146,22 @@
         node_selector=None,
         namespace=None,
         cpu=None,
         gpu=None,
         gpu_vendor=None,
         disk=None,
         memory=None,
+        use_tmpfs=None,
+        tmpfs_tempdir=None,
+        tmpfs_size=None,
+        tmpfs_path=None,
         run_time_limit=None,
         env=None,
         tolerations=None,
     ):
-
         if env is None:
             env = {}
 
         job = (
             KubernetesClient()
             .job(
                 generate_name="t-",
@@ -181,14 +185,18 @@
                 gpu=gpu,
                 gpu_vendor=gpu_vendor,
                 timeout_in_seconds=run_time_limit,
                 # Retries are handled by Metaflow runtime
                 retries=0,
                 step_name=step_name,
                 tolerations=tolerations,
+                use_tmpfs=use_tmpfs,
+                tmpfs_tempdir=tmpfs_tempdir,
+                tmpfs_size=tmpfs_size,
+                tmpfs_path=tmpfs_path,
             )
             .environment_variable("METAFLOW_CODE_SHA", code_package_sha)
             .environment_variable("METAFLOW_CODE_URL", code_package_url)
             .environment_variable("METAFLOW_CODE_DS", code_package_ds)
             .environment_variable("METAFLOW_USER", user)
             .environment_variable("METAFLOW_SERVICE_URL", SERVICE_INTERNAL_URL)
             .environment_variable(
@@ -226,21 +234,28 @@
             .environment_variable("METAFLOW_CARD_AZUREROOT", CARD_AZUREROOT)
             .environment_variable("METAFLOW_DATASTORE_SYSROOT_GS", DATASTORE_SYSROOT_GS)
             .environment_variable("METAFLOW_CARD_GSROOT", CARD_GSROOT)
             # support Metaflow sandboxes
             .environment_variable(
                 "METAFLOW_INIT_SCRIPT", KUBERNETES_SANDBOX_INIT_SCRIPT
             )
+            .environment_variable(
+                "METAFLOW_ARGO_EVENTS_WEBHOOK_URL", ARGO_EVENTS_WEBHOOK_URL
+            )
             # Skip setting METAFLOW_DATASTORE_SYSROOT_LOCAL because metadata sync
             # between the local user instance and the remote Kubernetes pod
             # assumes metadata is stored in DATASTORE_LOCAL_DIR on the Kubernetes
             # pod; this happens when METAFLOW_DATASTORE_SYSROOT_LOCAL is NOT set (
             # see get_datastore_root_from_config in datastore/local.py).
         )
 
+        tmpfs_enabled = use_tmpfs or (tmpfs_size and not use_tmpfs)
+        if tmpfs_enabled and tmpfs_tempdir:
+            job.environment_variable("METAFLOW_TEMPDIR", tmpfs_path)
+
         for name, value in env.items():
             job.environment_variable(name, value)
 
         annotations = {
             "metaflow/user": user,
             "metaflow/flow_name": flow_name,
         }
```

### Comparing `metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_cli.py` & `metaflow-2.8.4/metaflow/plugins/kubernetes/kubernetes_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,20 @@
     "--tag", multiple=True, default=None, help="Passed to the top-level 'step'."
 )
 @click.option("--namespace", default=None, help="Passed to the top-level 'step'.")
 @click.option("--retry-count", default=0, help="Passed to the top-level 'step'.")
 @click.option(
     "--max-user-code-retries", default=0, help="Passed to the top-level 'step'."
 )
+@click.option("--use-tmpfs", is_flag=True, help="tmpfs requirement for Kubernetes pod.")
+@click.option(
+    "--tmpfs-tempdir", is_flag=True, help="tmpfs requirement for Kubernetes pod."
+)
+@click.option("--tmpfs-size", help="tmpfs requirement for Kubernetes pod.")
+@click.option("--tmpfs-path", help="tmpfs requirement for Kubernetes pod.")
 @click.option(
     "--run-time-limit",
     default=5 * 24 * 60 * 60,  # Default is set to 5 days
     help="Run time limit in seconds for Kubernetes pod.",
 )
 @click.option(
     "--tolerations",
@@ -104,14 +110,18 @@
     node_selector=None,
     k8s_namespace=None,
     cpu=None,
     disk=None,
     memory=None,
     gpu=None,
     gpu_vendor=None,
+    use_tmpfs=None,
+    tmpfs_tempdir=None,
+    tmpfs_size=None,
+    tmpfs_path=None,
     run_time_limit=None,
     tolerations=None,
     **kwargs
 ):
     def echo(msg, stream="stderr", job_id=None, **kwargs):
         msg = util.to_unicode(msg)
         if job_id:
@@ -211,14 +221,18 @@
                 node_selector=node_selector,
                 namespace=k8s_namespace,
                 cpu=cpu,
                 disk=disk,
                 memory=memory,
                 gpu=gpu,
                 gpu_vendor=gpu_vendor,
+                use_tmpfs=use_tmpfs,
+                tmpfs_tempdir=tmpfs_tempdir,
+                tmpfs_size=tmpfs_size,
+                tmpfs_path=tmpfs_path,
                 run_time_limit=run_time_limit,
                 env=env,
                 tolerations=tolerations,
             )
     except Exception as e:
         traceback.print_exc(chain=False)
         _sync_metadata()
```

### Comparing `metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_client.py` & `metaflow-2.8.4/metaflow/plugins/kubernetes/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_decorator.py` & `metaflow-2.8.4/metaflow/plugins/kubernetes/kubernetes_decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 import platform
 import sys
 
+from metaflow import current
 from metaflow.decorators import StepDecorator
 from metaflow.exception import MetaflowException
 from metaflow.metadata import MetaDatum
 from metaflow.metadata.util import sync_local_metadata_to_datastore
 from metaflow.metaflow_config import (
     DATASTORE_LOCAL_DIR,
     KUBERNETES_CONTAINER_IMAGE,
@@ -61,14 +62,24 @@
         Kubernetes namespace to use when launching pod in Kubernetes.
     secrets : List[str], optional
         Kubernetes secrets to use when launching pod in Kubernetes. These
         secrets are in addition to the ones defined in `METAFLOW_KUBERNETES_SECRETS`
         in Metaflow configuration.
     tolerations : List[str], default: METAFLOW_KUBERNETES_TOLERATIONS
         Kubernetes tolerations to use when launching pod in Kubernetes.
+    use_tmpfs: bool, default: False
+        This enables an explicit tmpfs mount for this step.
+    tmpfs_tempdir: bool, default: True
+        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
+    tmpfs_size: int, optional
+        The value for the size (in MiB) of the tmpfs mount for this step.
+        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
+        memory allocated for this step.
+    tmpfs_path: string, optional
+        Path to tmpfs mount for this step. Defaults to /metaflow_temp.
     """
 
     name = "kubernetes"
     defaults = {
         "cpu": "1",
         "memory": "4096",
         "disk": "10240",
@@ -77,14 +88,18 @@
         "secrets": None,  # e.g., mysecret
         "node_selector": None,  # e.g., kubernetes.io/os=linux
         "namespace": None,
         "gpu": None,  # value of 0 implies that the scheduled node should not have GPUs
         "gpu_vendor": None,
         "tolerations": None,  # e.g., [{"key": "arch", "operator": "Equal", "value": "amd"},
         #                              {"key": "foo", "operator": "Equal", "value": "bar"}]
+        "use_tmpfs": None,
+        "tmpfs_tempdir": True,
+        "tmpfs_size": None,
+        "tmpfs_path": "/metaflow_temp",
     }
     package_url = None
     package_sha = None
     run_time_limit = None
 
     def __init__(self, attributes=None, statically_defined=False):
         super(KubernetesDecorator, self).__init__(attributes, statically_defined)
@@ -146,14 +161,21 @@
         # Assign docker registry URL for the image.
         if not get_docker_registry(self.attributes["image"]):
             if KUBERNETES_CONTAINER_REGISTRY:
                 self.attributes["image"] = "%s/%s" % (
                     KUBERNETES_CONTAINER_REGISTRY.rstrip("/"),
                     self.attributes["image"],
                 )
+        # Check if TmpFS is enabled and set default tmpfs_size if missing.
+        if self.attributes["use_tmpfs"] or (
+            self.attributes["tmpfs_size"] and not self.attributes["use_tmpfs"]
+        ):
+            if not self.attributes["tmpfs_size"]:
+                # default tmpfs behavior - https://man7.org/linux/man-pages/man5/tmpfs.5.html
+                self.attributes["tmpfs_size"] = int(self.attributes["memory"]) // 2
 
     # Refer https://github.com/Netflix/metaflow/blob/master/docs/lifecycle.png
     def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
         # Executing Kubernetes jobs requires a non-local datastore.
         if flow_datastore.TYPE not in ("s3", "azure", "gs"):
             raise KubernetesException(
                 "The *@kubernetes* decorator requires --datastore=s3 or --datastore=azure or --datastore=gs at the moment."
@@ -230,14 +252,25 @@
         ):
             raise KubernetesException(
                 "Invalid GPU value *{}* for step *{step}*; it should be an integer".format(
                     self.attributes["gpu"], step=step
                 )
             )
 
+        if self.attributes["tmpfs_size"]:
+            if not (
+                isinstance(self.attributes["tmpfs_size"], (int, unicode, basestring))
+                and int(self.attributes["tmpfs_size"]) > 0
+            ):
+                raise KubernetesException(
+                    "Invalid tmpfs_size value: *{size}* for step *{step}* (should be an integer greater than 0)".format(
+                        size=self.attributes["tmpfs_size"], step=step
+                    )
+                )
+
     def package_init(self, flow, step_name, environment):
         try:
             # Kubernetes is a soft dependency.
             from kubernetes import client, config
         except (NameError, ImportError):
             raise KubernetesException(
                 "Could not import module 'kubernetes'.\n\nInstall Kubernetes "
@@ -304,14 +337,19 @@
         max_retries,
         ubf_context,
         inputs,
     ):
         self.metadata = metadata
         self.task_datastore = task_datastore
 
+        # current.tempdir reflects the value of METAFLOW_TEMPDIR (the current working
+        # directory by default), or the value of tmpfs_path if tmpfs_tempdir=False.
+        if not self.attributes["tmpfs_tempdir"]:
+            current._update_env({"tempdir": self.attributes["tmpfs_path"]})
+
         # task_pre_step may run locally if fallback is activated for @catch
         # decorator. In that scenario, we skip collecting Kubernetes execution
         # metadata. A rudimentary way to detect non-local execution is to
         # check for the existence of METAFLOW_KUBERNETES_WORKLOAD environment
         # variable.
 
         if "METAFLOW_KUBERNETES_WORKLOAD" in os.environ:
```

### Comparing `metaflow-2.8.3/metaflow/plugins/kubernetes/kubernetes_job.py` & `metaflow-2.8.4/metaflow/plugins/kubernetes/kubernetes_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,19 @@
         #        API. When we ship the AWS Step Functions integration with EKS,
         #        it will hopefully lessen our workload.
         #
         # Note: This implementation ensures that there is only one unique Pod
         # (unique UID) per Metaflow task attempt.
         client = self._client.get()
 
+        # tmpfs variables
+        use_tmpfs = self._kwargs["use_tmpfs"]
+        tmpfs_size = self._kwargs["tmpfs_size"]
+        tmpfs_enabled = use_tmpfs or (tmpfs_size and not use_tmpfs)
+
         self._job = client.V1Job(
             api_version="batch/v1",
             kind="Job",
             metadata=client.V1ObjectMeta(
                 # Annotations are for humans
                 annotations=self._kwargs.get("annotations", {}),
                 # While labels are for Kubernetes
@@ -157,14 +162,22 @@
                                             self._kwargs["gpu"]
                                         )
                                         for k in [0]
                                         # Don't set GPU limits if gpu isn't specified.
                                         if self._kwargs["gpu"] is not None
                                     },
                                 ),
+                                volume_mounts=[
+                                    client.V1VolumeMount(
+                                        mount_path=self._kwargs.get("tmpfs_path"),
+                                        name="tmpfs-ephemeral-volume",
+                                    )
+                                ]
+                                if tmpfs_enabled
+                                else [],
                             )
                         ],
                         node_selector=self._kwargs.get("node_selector"),
                         # TODO (savin): Support image_pull_secrets
                         # image_pull_secrets=?,
                         # TODO (savin): Support preemption policies
                         # preemption_policy=?,
@@ -178,15 +191,26 @@
                         service_account_name=self._kwargs["service_account"],
                         # Terminate the container immediately on SIGTERM
                         termination_grace_period_seconds=0,
                         tolerations=[
                             client.V1Toleration(**toleration)
                             for toleration in self._kwargs.get("tolerations") or []
                         ],
-                        # volumes=?,
+                        volumes=[
+                            client.V1Volume(
+                                name="tmpfs-ephemeral-volume",
+                                empty_dir=client.V1EmptyDirVolumeSource(
+                                    medium="Memory",
+                                    # Add default unit as ours differs from Kubernetes default.
+                                    size_limit="{}Mi".format(tmpfs_size),
+                                ),
+                            )
+                        ]
+                        if tmpfs_enabled
+                        else [],
                         # TODO (savin): Set termination_message_policy
                     ),
                 ),
             ),
         )
         return self
```

### Comparing `metaflow-2.8.3/metaflow/plugins/metadata/local.py` & `metaflow-2.8.4/metaflow/plugins/metadata/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/metadata/service.py` & `metaflow-2.8.4/metaflow/plugins/metadata/service.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/package_cli.py` & `metaflow-2.8.4/metaflow/plugins/package_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/parallel_decorator.py` & `metaflow-2.8.4/metaflow/plugins/parallel_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/project_decorator.py` & `metaflow-2.8.4/metaflow/plugins/project_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/resources_decorator.py` & `metaflow-2.8.4/metaflow/plugins/resources_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/retry_decorator.py` & `metaflow-2.8.4/metaflow/plugins/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/secrets/secrets_decorator.py` & `metaflow-2.8.4/metaflow/plugins/secrets/secrets_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/storage_executor.py` & `metaflow-2.8.4/metaflow/plugins/storage_executor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/tag_cli.py` & `metaflow-2.8.4/metaflow/plugins/tag_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/test_unbounded_foreach_decorator.py` & `metaflow-2.8.4/metaflow/plugins/test_unbounded_foreach_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/plugins/timeout_decorator.py` & `metaflow-2.8.4/metaflow/plugins/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/procpoll.py` & `metaflow-2.8.4/metaflow/procpoll.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/pylint_wrapper.py` & `metaflow-2.8.4/metaflow/pylint_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/sidecar/sidecar.py` & `metaflow-2.8.4/metaflow/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/sidecar/sidecar_messages.py` & `metaflow-2.8.4/metaflow/sidecar/sidecar_messages.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/sidecar/sidecar_subprocess.py` & `metaflow-2.8.4/metaflow/sidecar/sidecar_subprocess.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/sidecar/sidecar_worker.py` & `metaflow-2.8.4/metaflow/sidecar/sidecar_worker.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tagging_util.py` & `metaflow-2.8.4/metaflow/tagging_util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/task.py` & `metaflow-2.8.4/metaflow/task.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/00-helloworld/helloworld.py` & `metaflow-2.8.4/metaflow/tutorials/00-helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/01-playlist/README.md` & `metaflow-2.8.4/metaflow/tutorials/01-playlist/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/01-playlist/movies.csv` & `metaflow-2.8.4/metaflow/tutorials/01-playlist/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/01-playlist/playlist.ipynb` & `metaflow-2.8.4/metaflow/tutorials/01-playlist/playlist.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/01-playlist/playlist.py` & `metaflow-2.8.4/metaflow/tutorials/01-playlist/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/02-statistics/README.md` & `metaflow-2.8.4/metaflow/tutorials/02-statistics/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/02-statistics/movies.csv` & `metaflow-2.8.4/metaflow/tutorials/02-statistics/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/02-statistics/stats.ipynb` & `metaflow-2.8.4/metaflow/tutorials/02-statistics/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/02-statistics/stats.py` & `metaflow-2.8.4/metaflow/tutorials/02-statistics/stats.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/03-playlist-redux/README.md` & `metaflow-2.8.4/metaflow/tutorials/03-playlist-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/03-playlist-redux/playlist.py` & `metaflow-2.8.4/metaflow/tutorials/03-playlist-redux/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/04-playlist-plus/README.md` & `metaflow-2.8.4/metaflow/tutorials/04-playlist-plus/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/04-playlist-plus/playlist.py` & `metaflow-2.8.4/metaflow/tutorials/04-playlist-plus/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/README.md` & `metaflow-2.8.4/metaflow/tutorials/05-hello-cloud/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb` & `metaflow-2.8.4/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/05-hello-cloud/hello-cloud.py` & `metaflow-2.8.4/metaflow/tutorials/05-hello-cloud/hello-cloud.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/06-statistics-redux/README.md` & `metaflow-2.8.4/metaflow/tutorials/06-statistics-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/06-statistics-redux/stats.ipynb` & `metaflow-2.8.4/metaflow/tutorials/06-statistics-redux/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/07-worldview/worldview.ipynb` & `metaflow-2.8.4/metaflow/tutorials/07-worldview/worldview.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/08-autopilot/README.md` & `metaflow-2.8.4/metaflow/tutorials/08-autopilot/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/tutorials/08-autopilot/autopilot.ipynb` & `metaflow-2.8.4/metaflow/tutorials/08-autopilot/autopilot.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/util.py` & `metaflow-2.8.4/metaflow/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow/vendor.py` & `metaflow-2.8.4/metaflow/vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.3/metaflow.egg-info/PKG-INFO` & `metaflow-2.8.4/metaflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow
-Version: 2.8.3
+Version: 2.8.4
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
```

### Comparing `metaflow-2.8.3/metaflow.egg-info/SOURCES.txt` & `metaflow-2.8.4/metaflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 metaflow/cli.py
 metaflow/cli_args.py
 metaflow/cmd_with_io.py
 metaflow/current.py
 metaflow/debug.py
 metaflow/decorators.py
 metaflow/event_logger.py
+metaflow/events.py
 metaflow/exception.py
 metaflow/flowspec.py
 metaflow/graph.py
 metaflow/includefile.py
 metaflow/integrations.py
 metaflow/lint.py
 metaflow/metaflow_config.py
@@ -107,14 +108,15 @@
 metaflow/mflog/save_logs_periodically.py
 metaflow/mflog/tee.py
 metaflow/plugins/__init__.py
 metaflow/plugins/catch_decorator.py
 metaflow/plugins/debug_logger.py
 metaflow/plugins/debug_monitor.py
 metaflow/plugins/environment_decorator.py
+metaflow/plugins/events_decorator.py
 metaflow/plugins/package_cli.py
 metaflow/plugins/parallel_decorator.py
 metaflow/plugins/project_decorator.py
 metaflow/plugins/resources_decorator.py
 metaflow/plugins/retry_decorator.py
 metaflow/plugins/storage_executor.py
 metaflow/plugins/tag_cli.py
@@ -131,14 +133,15 @@
 metaflow/plugins/airflow/plumbing/set_parameters.py
 metaflow/plugins/airflow/sensors/__init__.py
 metaflow/plugins/airflow/sensors/base_sensor.py
 metaflow/plugins/airflow/sensors/external_task_sensor.py
 metaflow/plugins/airflow/sensors/s3_sensor.py
 metaflow/plugins/argo/__init__.py
 metaflow/plugins/argo/argo_client.py
+metaflow/plugins/argo/argo_events.py
 metaflow/plugins/argo/argo_workflows.py
 metaflow/plugins/argo/argo_workflows_cli.py
 metaflow/plugins/argo/argo_workflows_decorator.py
 metaflow/plugins/argo/process_input_paths.py
 metaflow/plugins/aws/__init__.py
 metaflow/plugins/aws/aws_client.py
 metaflow/plugins/aws/aws_utils.py
```

### Comparing `metaflow-2.8.3/setup.py` & `metaflow-2.8.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "2.8.3"
+version = "2.8.4"
 
 setup(
     include_package_data=True,
     name="metaflow",
     version=version,
     description="Metaflow: More Data Science, Less Engineering",
     long_description=open("README.md").read(),
@@ -39,10 +39,9 @@
     entry_points="""
         [console_scripts]
         metaflow=metaflow.cmd.main_cli:start
       """,
     install_requires=[
         "requests",
         "boto3",
-        "pylint",
     ],
 )
```

