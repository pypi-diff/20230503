# Comparing `tmp/fugue-0.8.3.dev1.tar.gz` & `tmp/fugue-0.8.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugue-0.8.3.dev1.tar", last modified: Wed Mar 29 04:22:27 2023, max compression
+gzip compressed data, was "fugue-0.8.4.dev1.tar", last modified: Wed May  3 06:43:09 2023, max compression
```

## Comparing `fugue-0.8.3.dev1.tar` & `fugue-0.8.4.dev1.tar`

### file list

```diff
@@ -1,324 +1,323 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.672648 fugue-0.8.3.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-03-29 04:22:27.672648 fugue-0.8.3.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.648648 fugue-0.8.3.dev1/fugue/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.648648 fugue-0.8.3.dev1/fugue/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/_utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/_utils/interfaceless.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/_utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.648648 fugue-0.8.3.dev1/fugue/bag/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/bag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/bag/array_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/bag/bag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.648648 fugue-0.8.3.dev1/fugue/collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/collections/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/collections/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/collections/yielded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.648648 fugue-0.8.3.dev1/fugue/column/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/column/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/column/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/column/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.652648 fugue-0.8.3.dev1/fugue/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataframe/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataframe/array_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataframe/arrow_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataframe/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataframe/dataframe_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataframe/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataframe/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataframe/iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataframe/pandas_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataframe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.652648 fugue-0.8.3.dev1/fugue/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataset/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.652648 fugue-0.8.3.dev1/fugue/execution/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/execution/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/execution/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/execution/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/execution/native_execution_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.652648 fugue-0.8.3.dev1/fugue/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.652648 fugue-0.8.3.dev1/fugue/extensions/_builtins/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/_builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/_builtins/creators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/_builtins/outputters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/_builtins/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.652648 fugue-0.8.3.dev1/fugue/extensions/creator/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/creator/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/creator/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.652648 fugue-0.8.3.dev1/fugue/extensions/outputter/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/outputter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/outputter/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/outputter/outputter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.652648 fugue-0.8.3.dev1/fugue/extensions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/processor/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/processor/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.652648 fugue-0.8.3.dev1/fugue/extensions/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/transformer/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/transformer/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/extensions/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.652648 fugue-0.8.3.dev1/fugue/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/rpc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/rpc/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.656648 fugue-0.8.3.dev1/fugue/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/sql/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/sql/_visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/sql/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/sql/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.656648 fugue-0.8.3.dev1/fugue/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/workflow/_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/workflow/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/workflow/_workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/workflow/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/workflow/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/workflow/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.648648 fugue-0.8.3.dev1/fugue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-03-29 04:22:27.000000 fugue-0.8.3.dev1/fugue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-03-29 04:22:27.000000 fugue-0.8.3.dev1/fugue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 04:22:27.000000 fugue-0.8.3.dev1/fugue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-29 04:22:27.000000 fugue-0.8.3.dev1/fugue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-29 04:22:27.000000 fugue-0.8.3.dev1/fugue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-29 04:22:27.000000 fugue-0.8.3.dev1/fugue.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.656648 fugue-0.8.3.dev1/fugue_contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_contrib/contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.656648 fugue-0.8.3.dev1/fugue_contrib/seaborn/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_contrib/seaborn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.656648 fugue-0.8.3.dev1/fugue_contrib/viz/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_contrib/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_contrib/viz/_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.656648 fugue-0.8.3.dev1/fugue_dask/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_dask/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_dask/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_dask/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_dask/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    18309 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_dask/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_dask/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_dask/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.656648 fugue-0.8.3.dev1/fugue_duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_duckdb/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_duckdb/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_duckdb/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_duckdb/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    20479 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_duckdb/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_duckdb/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_duckdb/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.656648 fugue-0.8.3.dev1/fugue_ibis/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ibis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ibis/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ibis/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ibis/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.660648 fugue-0.8.3.dev1/fugue_ibis/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ibis/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ibis/execution/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ibis/execution/pandas_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ibis/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ibis/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.660648 fugue-0.8.3.dev1/fugue_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_notebook/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.660648 fugue-0.8.3.dev1/fugue_notebook/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_notebook/nbextension/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_notebook/nbextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_notebook/nbextension/description.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_notebook/nbextension/main.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.660648 fugue-0.8.3.dev1/fugue_polars/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_polars/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_polars/polars_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_polars/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.660648 fugue-0.8.3.dev1/fugue_ray/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ray/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.660648 fugue-0.8.3.dev1/fugue_ray/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ray/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ray/_utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ray/_utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ray/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ray/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ray/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_ray/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.660648 fugue-0.8.3.dev1/fugue_spark/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_spark/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.660648 fugue-0.8.3.dev1/fugue_spark/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_spark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_spark/_utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_spark/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_spark/_utils/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9367 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_spark/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    32034 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_spark/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_spark/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_spark/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.660648 fugue-0.8.3.dev1/fugue_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.660648 fugue-0.8.3.dev1/fugue_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_test/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_test/bag_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    75791 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_test/builtin_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    18994 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_test/dataframe_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    52798 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_test/execution_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_test/ibis_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.660648 fugue-0.8.3.dev1/fugue_version/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/fugue_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-29 04:22:27.672648 fugue-0.8.3.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.664648 fugue-0.8.3.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.664648 fugue-0.8.3.dev1/tests/fugue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.664648 fugue-0.8.3.dev1/tests/fugue/bag/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/bag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/bag/test_array_bag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.664648 fugue-0.8.3.dev1/tests/fugue/collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/collections/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/collections/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.664648 fugue-0.8.3.dev1/tests/fugue/column/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/column/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/column/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/column/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.664648 fugue-0.8.3.dev1/tests/fugue/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/dataframe/test_array_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/dataframe/test_arrow_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/dataframe/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/dataframe/test_dataframe_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/dataframe/test_dataframes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/dataframe/test_function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/dataframe/test_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/dataframe/test_pandas_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/dataframe/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.664648 fugue-0.8.3.dev1/tests/fugue/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/execution/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/execution/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/execution/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/execution/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/execution/test_naive_execution_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.664648 fugue-0.8.3.dev1/tests/fugue/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.664648 fugue-0.8.3.dev1/tests/fugue/extensions/creator/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/extensions/creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/extensions/creator/test_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.664648 fugue-0.8.3.dev1/tests/fugue/extensions/outputter/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/extensions/outputter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/extensions/outputter/test_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.664648 fugue-0.8.3.dev1/tests/fugue/extensions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/extensions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/extensions/processor/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/extensions/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.664648 fugue-0.8.3.dev1/tests/fugue/extensions/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/extensions/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/extensions/transformer/test_convert_cotransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/extensions/transformer/test_convert_output_cotransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/extensions/transformer/test_convert_output_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/extensions/transformer/test_convert_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.664648 fugue-0.8.3.dev1/tests/fugue/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/rpc/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/rpc/test_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/rpc/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.668648 fugue-0.8.3.dev1/tests/fugue/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/sql/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/sql/test_visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/sql/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    23329 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/sql/test_workflow_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/test_interfaceless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.668648 fugue-0.8.3.dev1/tests/fugue/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/utils/test_interfaceless.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/utils/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/utils/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.668648 fugue-0.8.3.dev1/tests/fugue/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/workflow/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/workflow/test_runtime_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/workflow/test_workflow_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue/workflow/test_workflow_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.668648 fugue-0.8.3.dev1/tests/fugue_dask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_dask/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_dask/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_dask/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_dask/test_importless.py
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_dask/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_dask/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.668648 fugue-0.8.3.dev1/tests/fugue_duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_duckdb/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_duckdb/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_duckdb/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_duckdb/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_duckdb/test_importless.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_duckdb/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.668648 fugue-0.8.3.dev1/tests/fugue_ibis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ibis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.668648 fugue-0.8.3.dev1/tests/fugue_ibis/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ibis/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ibis/mock/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ibis/mock/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ibis/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ibis/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ibis/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ibis/test_importless.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ibis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.668648 fugue-0.8.3.dev1/tests/fugue_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.668648 fugue-0.8.3.dev1/tests/fugue_polars/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_polars/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_polars/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_polars/test_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.672648 fugue-0.8.3.dev1/tests/fugue_ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ray/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ray/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ray/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_ray/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.672648 fugue-0.8.3.dev1/tests/fugue_spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_spark/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_spark/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_spark/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_spark/test_importless.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_spark/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 04:22:27.672648 fugue-0.8.3.dev1/tests/fugue_spark/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_spark/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_spark/utils/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_spark/utils/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-03-29 04:20:21.000000 fugue-0.8.3.dev1/tests/fugue_spark/utils/test_partition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.099465 fugue-0.8.4.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-03 06:43:09.099465 fugue-0.8.4.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.075465 fugue-0.8.4.dev1/fugue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.075465 fugue-0.8.4.dev1/fugue/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/interfaceless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.075465 fugue-0.8.4.dev1/fugue/bag/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/bag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/bag/array_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/bag/bag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.075465 fugue-0.8.4.dev1/fugue/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/collections/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/collections/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/collections/yielded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/column/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/column/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/column/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/column/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/array_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/arrow_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/dataframe_iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/pandas_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataset/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/execution/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/execution/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/execution/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/execution/native_execution_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/extensions/_builtins/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/_builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/_builtins/creators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/_builtins/outputters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/_builtins/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/extensions/creator/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/creator/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/creator/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/extensions/outputter/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/outputter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/outputter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/outputter/outputter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/extensions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/processor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/processor/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/extensions/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/transformer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/transformer/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/rpc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/rpc/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/sql/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/sql/_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/sql/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/sql/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.075465 fugue-0.8.4.dev1/fugue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-03 06:43:08.000000 fugue-0.8.4.dev1/fugue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-05-03 06:43:09.000000 fugue-0.8.4.dev1/fugue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:43:08.000000 fugue-0.8.4.dev1/fugue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-03 06:43:08.000000 fugue-0.8.4.dev1/fugue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-03 06:43:08.000000 fugue-0.8.4.dev1/fugue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 06:43:08.000000 fugue-0.8.4.dev1/fugue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue_contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_contrib/contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue_contrib/seaborn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_contrib/seaborn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue_contrib/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_contrib/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_contrib/viz/_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18309 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue_duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20479 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue_ibis/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_ibis/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/execution/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/execution/pandas_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_notebook/nbextension/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_notebook/nbextension/description.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_notebook/nbextension/main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_polars/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_polars/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_polars/polars_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_polars/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_ray/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_ray/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/_utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/_utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_spark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/_utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/_utils/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31733 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_test/bag_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75748 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_test/builtin_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_test/dataframe_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50559 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_test/execution_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_test/ibis_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-03 06:43:09.099465 fugue-0.8.4.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/tests/fugue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/tests/fugue/bag/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/bag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/bag/test_array_bag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/collections/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/collections/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/column/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/column/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/column/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/column/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_array_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_arrow_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_dataframe_iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_pandas_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/execution/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/execution/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/execution/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/execution/test_ibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/execution/test_naive_execution_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/extensions/creator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/creator/test_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/extensions/outputter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/outputter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/outputter/test_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/extensions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/processor/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/extensions/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_cotransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_output_cotransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_output_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/rpc/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/rpc/test_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/rpc/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/sql/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/sql/test_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/sql/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23329 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/sql/test_workflow_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/test_interfaceless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/utils/test_interfaceless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/utils/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/utils/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/workflow/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/workflow/test_runtime_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/workflow/test_workflow_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/workflow/test_workflow_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/test_ibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/test_importless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/test_ibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/test_importless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_ibis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_ibis/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/mock/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/mock/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/test_importless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_polars/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_polars/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_polars/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_polars/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ray/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ray/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ray/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ray/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.099465 fugue-0.8.4.dev1/tests/fugue_spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/test_ibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/test_importless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.099465 fugue-0.8.4.dev1/tests/fugue_spark/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/utils/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/utils/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/utils/test_partition.py
```

### Comparing `fugue-0.8.3.dev1/LICENSE` & `fugue-0.8.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/PKG-INFO` & `fugue-0.8.4.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.3.dev1
+Version: 0.8.4.dev1
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
         
@@ -159,15 +159,15 @@
         *   **polars**: to support Polars DataFrames and extensions using Polars.
         *   **ibis**: to enable Ibis for Fugue workflows, read [details](https://fugue-tutorials.readthedocs.io/tutorials/integrations/backends/ibis.html).
         *   **cpp_sql_parser**: to enable the CPP antlr parser for Fugue SQL. It can be 50+ times faster than the pure Python parser. For the main Python versions and platforms, there is already pre-built binaries, but for the remaining, it needs a C++ compiler to build on the fly.
         
         For example a common use case is:
         
         ```bash
-        pip install fugue[duckdb,spark]
+        pip install "fugue[duckdb,spark]"
         ```
         
         Note if you already installed Spark or DuckDB independently, Fugue is able to automatically use them without installing the extras.
         
         ## [Getting Started](https://fugue-tutorials.readthedocs.io/)
         
         The best way to get started with Fugue is to work through the 10 minute tutorials:
```

### Comparing `fugue-0.8.3.dev1/README.md` & `fugue-0.8.4.dev1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 *   **polars**: to support Polars DataFrames and extensions using Polars.
 *   **ibis**: to enable Ibis for Fugue workflows, read [details](https://fugue-tutorials.readthedocs.io/tutorials/integrations/backends/ibis.html).
 *   **cpp_sql_parser**: to enable the CPP antlr parser for Fugue SQL. It can be 50+ times faster than the pure Python parser. For the main Python versions and platforms, there is already pre-built binaries, but for the remaining, it needs a C++ compiler to build on the fly.
 
 For example a common use case is:
 
 ```bash
-pip install fugue[duckdb,spark]
+pip install "fugue[duckdb,spark]"
 ```
 
 Note if you already installed Spark or DuckDB independently, Fugue is able to automatically use them without installing the extras.
 
 ## [Getting Started](https://fugue-tutorials.readthedocs.io/)
 
 The best way to get started with Fugue is to work through the 10 minute tutorials:
```

### Comparing `fugue-0.8.3.dev1/fugue/__init__.py` & `fugue-0.8.4.dev1/fugue/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/_utils/display.py` & `fugue-0.8.4.dev1/fugue/_utils/display.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/_utils/exception.py` & `fugue-0.8.4.dev1/fugue/_utils/exception.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/_utils/interfaceless.py` & `fugue-0.8.4.dev1/fugue/_utils/interfaceless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/_utils/io.py` & `fugue-0.8.4.dev1/fugue/_utils/io.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import pathlib
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 import fs as pfs
 import pandas as pd
-from fs.errors import FileExpected
-from fugue.dataframe import LocalBoundedDataFrame, LocalDataFrame, PandasDataFrame
 from triad.collections.dict import ParamDict
 from triad.collections.fs import FileSystem
 from triad.collections.schema import Schema
 from triad.utils.assertion import assert_or_throw
 
+from fugue.dataframe import LocalBoundedDataFrame, LocalDataFrame, PandasDataFrame
+
 
 class FileParser(object):
     def __init__(self, path: str, format_hint: Optional[str] = None):
         last = len(path)
         has_glob = False
         self._orig_format_hint = format_hint
         for i in range(len(path)):
@@ -267,115 +267,26 @@
         return pdf, None
     if isinstance(columns, list):  # column names
         return pdf[columns], None
     schema = Schema(columns)
     return pdf[schema.names], schema
 
 
-def _save_avro(df: LocalDataFrame, p: FileParser, **kwargs: Any):
-    """Save pandas dataframe as avro.
-    If providing your own schema, the usage of schema argument is preferred
-
-    :param schema: Avro Schema determines dtypes saved
-    """
-    import pandavro as pdx
-
-    kw = ParamDict(kwargs)
-
-    # pandavro defaults
-    schema = None
-    append = False
-    times_as_micros = True
-
-    if "schema" in kw:
-        schema = kw["schema"]
-        del kw["schema"]
-
-    if "append" in kw:
-        append = kw["append"]  # default is overwrite (False) instead of append (True)
-        del kw["append"]
-
-    if "times_as_micros" in kw:
-        times_as_micros = kw["times_as_micros"]
-        del kw["times_as_micros"]
-
-    pdf = df.as_pandas()
-    pdx.to_avro(
-        p.uri, pdf, schema=schema, append=append, times_as_micros=times_as_micros, **kw
-    )
-
-
-def _load_avro(
-    p: FileParser, columns: Any = None, **kwargs: Any
-) -> Tuple[pd.DataFrame, Any]:
-    path = p.uri
-    try:
-        pdf = _load_single_avro(path, **kwargs)
-    except (IsADirectoryError, PermissionError, FileExpected):
-        fs = FileSystem()
-        pdf = pd.concat(
-            [
-                _load_single_avro(
-                    pfs.path.combine(path, pfs.path.basename(x.path)), **kwargs
-                )
-                for x in fs.opendir(path).glob("*.avro")
-            ]
-        )
-
-    if columns is None:
-        return pdf, None
-    if isinstance(columns, list):  # column names
-        return pdf[columns], None
-
-    schema = Schema(columns)
-
-    # Return created DataFrame
-    return pdf[schema.names], schema
-
-
-def _load_single_avro(path: str, **kwargs: Any) -> pd.DataFrame:
-    from fastavro import reader
-
-    kw = ParamDict(kwargs)
-    process_record = None
-    if "process_record" in kw:
-        process_record = kw["process_record"]
-        del kw["process_record"]
-
-    fs = FileSystem()
-    with fs.openbin(path) as fp:
-        # Configure Avro reader
-        avro_reader = reader(fp)
-        # Load records in memory
-        if process_record:
-            records = [process_record(r) for r in avro_reader]
-
-        else:
-            records = list(avro_reader)
-
-        # Populate pandas.DataFrame with records
-        return pd.DataFrame.from_records(records)
-
-
 _FORMAT_MAP: Dict[str, str] = {
     ".csv": "csv",
     ".csv.gz": "csv",
     ".parquet": "parquet",
     ".json": "json",
     ".json.gz": "json",
-    ".avro": "avro",
-    ".avro.gz": "avro",
 }
 
 _FORMAT_LOAD: Dict[str, Callable[..., Tuple[pd.DataFrame, Any]]] = {
     "csv": _load_csv,
     "parquet": _load_parquet,
     "json": _load_json,
-    "avro": _load_avro,
 }
 
 _FORMAT_SAVE: Dict[str, Callable] = {
     "csv": _save_csv,
     "parquet": _save_parquet,
     "json": _save_json,
-    "avro": _save_avro,
 }
```

### Comparing `fugue-0.8.3.dev1/fugue/api.py` & `fugue-0.8.4.dev1/fugue/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/bag/array_bag.py` & `fugue-0.8.4.dev1/fugue/bag/array_bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/bag/bag.py` & `fugue-0.8.4.dev1/fugue/bag/bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/collections/partition.py` & `fugue-0.8.4.dev1/fugue/collections/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/collections/sql.py` & `fugue-0.8.4.dev1/fugue/collections/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/collections/yielded.py` & `fugue-0.8.4.dev1/fugue/collections/yielded.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/column/expressions.py` & `fugue-0.8.4.dev1/fugue/column/expressions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/column/functions.py` & `fugue-0.8.4.dev1/fugue/column/functions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/column/sql.py` & `fugue-0.8.4.dev1/fugue/column/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/constants.py` & `fugue-0.8.4.dev1/fugue/constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/dataframe/__init__.py` & `fugue-0.8.4.dev1/fugue/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/dataframe/api.py` & `fugue-0.8.4.dev1/fugue/dataframe/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/dataframe/array_dataframe.py` & `fugue-0.8.4.dev1/fugue/dataframe/array_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/dataframe/arrow_dataframe.py` & `fugue-0.8.4.dev1/fugue/dataframe/arrow_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         data = self.native.take([0]).to_pydict()
         return {k: v[0] for k, v in data.items()}
 
     def count(self) -> int:
         return self.native.shape[0]
 
     def as_pandas(self) -> pd.DataFrame:
-        return self.native.to_pandas()
+        return self.native.to_pandas(use_threads=False, date_as_object=False)
 
     def head(
         self, n: int, columns: Optional[List[str]] = None
     ) -> LocalBoundedDataFrame:
         adf = self.native if columns is None else self.native.select(columns)
         n = min(n, self.count())
         if n == 0:
```

### Comparing `fugue-0.8.3.dev1/fugue/dataframe/dataframe.py` & `fugue-0.8.4.dev1/fugue/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/dataframe/dataframe_iterable_dataframe.py` & `fugue-0.8.4.dev1/fugue/dataframe/dataframe_iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/dataframe/dataframes.py` & `fugue-0.8.4.dev1/fugue/dataframe/dataframes.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/dataframe/function_wrapper.py` & `fugue-0.8.4.dev1/fugue/dataframe/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/dataframe/iterable_dataframe.py` & `fugue-0.8.4.dev1/fugue/dataframe/iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/dataframe/pandas_dataframe.py` & `fugue-0.8.4.dev1/fugue/dataframe/pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/dataframe/utils.py` & `fugue-0.8.4.dev1/fugue/dataframe/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             d2 = df2.as_pandas()
         if not check_order:
             d1 = d1.sort_values(df1.columns)
             d2 = d2.sort_values(df1.columns)
         d1 = d1.reset_index(drop=True)
         d2 = d2.reset_index(drop=True)
         pd.testing.assert_frame_equal(
-            d1, d2, check_less_precise=digits, check_dtype=False
+            d1, d2, rtol=0, atol=10 ** (-digits), check_dtype=False, check_exact=False
         )
         return True
     except AssertionError:
         if throw:
             raise
         return False
```

### Comparing `fugue-0.8.3.dev1/fugue/dataset/api.py` & `fugue-0.8.4.dev1/fugue/dataset/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/dataset/dataset.py` & `fugue-0.8.4.dev1/fugue/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/dev.py` & `fugue-0.8.4.dev1/fugue/dev.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/exceptions.py` & `fugue-0.8.4.dev1/fugue/exceptions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/execution/api.py` & `fugue-0.8.4.dev1/fugue/execution/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/execution/execution_engine.py` & `fugue-0.8.4.dev1/fugue/execution/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/execution/factory.py` & `fugue-0.8.4.dev1/fugue/execution/factory.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/execution/native_execution_engine.py` & `fugue-0.8.4.dev1/fugue/execution/native_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/__init__.py` & `fugue-0.8.4.dev1/fugue/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/_builtins/__init__.py` & `fugue-0.8.4.dev1/fugue/extensions/_builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/_builtins/creators.py` & `fugue-0.8.4.dev1/fugue/extensions/_builtins/creators.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/_builtins/outputters.py` & `fugue-0.8.4.dev1/fugue/extensions/_builtins/outputters.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/_builtins/processors.py` & `fugue-0.8.4.dev1/fugue/extensions/_builtins/processors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/_utils.py` & `fugue-0.8.4.dev1/fugue/extensions/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/context.py` & `fugue-0.8.4.dev1/fugue/extensions/context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/creator/convert.py` & `fugue-0.8.4.dev1/fugue/extensions/creator/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/creator/creator.py` & `fugue-0.8.4.dev1/fugue/extensions/creator/creator.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/outputter/convert.py` & `fugue-0.8.4.dev1/fugue/extensions/outputter/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/outputter/outputter.py` & `fugue-0.8.4.dev1/fugue/extensions/outputter/outputter.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/processor/convert.py` & `fugue-0.8.4.dev1/fugue/extensions/processor/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/processor/processor.py` & `fugue-0.8.4.dev1/fugue/extensions/processor/processor.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/transformer/convert.py` & `fugue-0.8.4.dev1/fugue/extensions/transformer/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/extensions/transformer/transformer.py` & `fugue-0.8.4.dev1/fugue/extensions/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/plugins.py` & `fugue-0.8.4.dev1/fugue/plugins.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/registry.py` & `fugue-0.8.4.dev1/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/rpc/base.py` & `fugue-0.8.4.dev1/fugue/rpc/base.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/rpc/flask.py` & `fugue-0.8.4.dev1/fugue/rpc/flask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/sql/_utils.py` & `fugue-0.8.4.dev1/fugue/sql/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/sql/_visitors.py` & `fugue-0.8.4.dev1/fugue/sql/_visitors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/sql/api.py` & `fugue-0.8.4.dev1/fugue/sql/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/sql/workflow.py` & `fugue-0.8.4.dev1/fugue/sql/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/workflow/_checkpoint.py` & `fugue-0.8.4.dev1/fugue/workflow/_checkpoint.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/workflow/_tasks.py` & `fugue-0.8.4.dev1/fugue/workflow/_tasks.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/workflow/_workflow_context.py` & `fugue-0.8.4.dev1/fugue/workflow/_workflow_context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/workflow/api.py` & `fugue-0.8.4.dev1/fugue/workflow/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/workflow/module.py` & `fugue-0.8.4.dev1/fugue/workflow/module.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue/workflow/workflow.py` & `fugue-0.8.4.dev1/fugue/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue.egg-info/PKG-INFO` & `fugue-0.8.4.dev1/fugue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.3.dev1
+Version: 0.8.4.dev1
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
         
@@ -159,15 +159,15 @@
         *   **polars**: to support Polars DataFrames and extensions using Polars.
         *   **ibis**: to enable Ibis for Fugue workflows, read [details](https://fugue-tutorials.readthedocs.io/tutorials/integrations/backends/ibis.html).
         *   **cpp_sql_parser**: to enable the CPP antlr parser for Fugue SQL. It can be 50+ times faster than the pure Python parser. For the main Python versions and platforms, there is already pre-built binaries, but for the remaining, it needs a C++ compiler to build on the fly.
         
         For example a common use case is:
         
         ```bash
-        pip install fugue[duckdb,spark]
+        pip install "fugue[duckdb,spark]"
         ```
         
         Note if you already installed Spark or DuckDB independently, Fugue is able to automatically use them without installing the extras.
         
         ## [Getting Started](https://fugue-tutorials.readthedocs.io/)
         
         The best way to get started with Fugue is to work through the 10 minute tutorials:
```

### Comparing `fugue-0.8.3.dev1/fugue.egg-info/SOURCES.txt` & `fugue-0.8.4.dev1/fugue.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,14 @@
 fugue_spark/_utils/__init__.py
 fugue_spark/_utils/convert.py
 fugue_spark/_utils/io.py
 fugue_spark/_utils/partition.py
 fugue_sql/__init__.py
 fugue_sql/exceptions.py
 fugue_test/__init__.py
-fugue_test/_utils.py
 fugue_test/bag_suite.py
 fugue_test/builtin_suite.py
 fugue_test/dataframe_suite.py
 fugue_test/execution_suite.py
 fugue_test/ibis_suite.py
 fugue_version/__init__.py
 tests/__init__.py
```

### Comparing `fugue-0.8.3.dev1/fugue.egg-info/requires.txt` & `fugue-0.8.4.dev1/fugue.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-triad>=0.8.4
+triad>=0.8.6
 adagio>=0.2.4
-qpd>=0.4.0
+qpd>=0.4.1
 fugue-sql-antlr>=0.1.6
 pyarrow>=0.15.1
-pandas<2,>=1.2.0
+pandas>=1.2.0
 sqlglot
 jinja2
 
 [all]
 fugue-sql-antlr[cpp]>=0.1.6
 pyspark
 ray[data]>=2.0.0
@@ -27,15 +27,15 @@
 dask[dataframe,distributed]>=2022.9.0
 ibis-framework>=3.2.0
 
 [cpp_sql_parser]
 fugue-sql-antlr[cpp]>=0.1.6
 
 [dask]
-qpd[dask]>=0.4.0
+qpd[dask]>=0.4.1
 
 [dask:python_version < "3.8"]
 dask[dataframe,distributed]
 
 [dask:python_version >= "3.8"]
 dask[dataframe,distributed]>=2022.9.0
```

### Comparing `fugue-0.8.3.dev1/fugue_contrib/seaborn/__init__.py` & `fugue-0.8.4.dev1/fugue_contrib/seaborn/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_contrib/viz/__init__.py` & `fugue-0.8.4.dev1/fugue_contrib/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_contrib/viz/_ext.py` & `fugue-0.8.4.dev1/fugue_contrib/viz/_ext.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_dask/_io.py` & `fugue-0.8.4.dev1/fugue_dask/_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import fs as pfs
 from dask import dataframe as dd
 from fugue._utils.io import FileParser, _get_single_files
-from fugue._utils.io import _load_avro as _pd_load_avro
-from fugue._utils.io import _save_avro
 from triad.collections.dict import ParamDict
 from triad.collections.fs import FileSystem
 from triad.collections.schema import Schema
 from triad.utils.assertion import assert_or_throw
 
 from fugue_dask.dataframe import DaskDataFrame
 
@@ -149,29 +147,18 @@
         return pdf, None
     if isinstance(columns, list):  # column names
         return pdf[columns], None
     schema = Schema(columns)
     return pdf[schema.names], schema
 
 
-def _load_avro(
-    p: FileParser, columns: Any = None, **kwargs: Any
-) -> Tuple[dd.DataFrame, Any]:
-    # TODO: change this hacky implementation!
-    pdf, schema = _pd_load_avro(p, columns, **kwargs)
-
-    return dd.from_pandas(pdf, npartitions=4), schema
-
-
 _FORMAT_LOAD: Dict[str, Callable[..., Tuple[dd.DataFrame, Any]]] = {
     "csv": _load_csv,
     "parquet": _load_parquet,
     "json": _load_json,
-    "avro": _load_avro,
 }
 
 _FORMAT_SAVE: Dict[str, Callable] = {
     "csv": _save_csv,
     "parquet": _save_parquet,
     "json": _save_json,
-    "avro": _save_avro,
 }
```

### Comparing `fugue-0.8.3.dev1/fugue_dask/_utils.py` & `fugue-0.8.4.dev1/fugue_dask/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_dask/dataframe.py` & `fugue-0.8.4.dev1/fugue_dask/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_dask/execution_engine.py` & `fugue-0.8.4.dev1/fugue_dask/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_dask/ibis_engine.py` & `fugue-0.8.4.dev1/fugue_dask/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_dask/registry.py` & `fugue-0.8.4.dev1/fugue_dask/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_duckdb/_io.py` & `fugue-0.8.4.dev1/fugue_duckdb/_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_duckdb/_utils.py` & `fugue-0.8.4.dev1/fugue_duckdb/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_duckdb/dask.py` & `fugue-0.8.4.dev1/fugue_duckdb/dask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_duckdb/dataframe.py` & `fugue-0.8.4.dev1/fugue_duckdb/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_duckdb/execution_engine.py` & `fugue-0.8.4.dev1/fugue_duckdb/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_duckdb/ibis_engine.py` & `fugue-0.8.4.dev1/fugue_duckdb/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_duckdb/registry.py` & `fugue-0.8.4.dev1/fugue_duckdb/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_ibis/_utils.py` & `fugue-0.8.4.dev1/fugue_ibis/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_ibis/dataframe.py` & `fugue-0.8.4.dev1/fugue_ibis/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_ibis/execution/ibis_engine.py` & `fugue-0.8.4.dev1/fugue_ibis/execution/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_ibis/execution/pandas_backend.py` & `fugue-0.8.4.dev1/fugue_ibis/execution/pandas_backend.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_ibis/execution_engine.py` & `fugue-0.8.4.dev1/fugue_ibis/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_ibis/extensions.py` & `fugue-0.8.4.dev1/fugue_ibis/extensions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_notebook/__init__.py` & `fugue-0.8.4.dev1/fugue_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_notebook/env.py` & `fugue-0.8.4.dev1/fugue_notebook/env.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_notebook/nbextension/main.js` & `fugue-0.8.4.dev1/fugue_notebook/nbextension/main.js`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_polars/_utils.py` & `fugue-0.8.4.dev1/fugue_polars/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_polars/polars_dataframe.py` & `fugue-0.8.4.dev1/fugue_polars/polars_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     def peek_array(self) -> List[Any]:
         self.assert_not_empty()
         return list(self._native.row(0))
 
     def peek_dict(self) -> Dict[str, Any]:
         self.assert_not_empty()
-        return dict(zip(self._native.columns, self._native.row(0)))
+        return self._native.row(0, named=True)
 
     def count(self) -> int:
         return self.native.shape[0]
 
     def as_pandas(self) -> pd.DataFrame:
         return self.native.to_pandas()
```

### Comparing `fugue-0.8.3.dev1/fugue_polars/registry.py` & `fugue-0.8.4.dev1/fugue_polars/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_ray/_constants.py` & `fugue-0.8.4.dev1/fugue_ray/_constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_ray/_utils/cluster.py` & `fugue-0.8.4.dev1/fugue_ray/_utils/cluster.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_ray/_utils/dataframe.py` & `fugue-0.8.4.dev1/fugue_ray/_utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_ray/_utils/io.py` & `fugue-0.8.4.dev1/fugue_ray/_utils/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import pathlib
 from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 import pyarrow as pa
 import ray.data as rd
 from fugue import ExecutionEngine
-from fugue._utils.io import FileParser, load_df, save_df
+from fugue._utils.io import FileParser, save_df
 from fugue.collections.partition import PartitionSpec
 from fugue.dataframe import DataFrame
 from fugue_ray.dataframe import RayDataFrame
 from pyarrow import csv as pacsv
 from pyarrow import json as pajson
 from ray.data.datasource import FileExtensionFilter
 from triad.collections import Schema
@@ -45,16 +45,14 @@
         else:
             fp = [FileParser(u, format_hint) for u in uri]
         fmts = list(set(f.file_format for f in fp))  # noqa: C401
         assert_or_throw(
             len(fmts) == 1, NotImplementedError("can't support multiple formats")
         )
         fmt = fmts[0]
-        if fmt == "avro":  # TODO: remove avro support
-            return load_df(uri, format_hint=format_hint, columns=columns, **kwargs)
         files = [f.uri for f in fp]
         return self._loads[fmt](files, columns, **kwargs)
 
     def save_df(
         self,
         df: RayDataFrame,
         uri: str,
@@ -71,15 +69,15 @@
                 self._fs.remove(uri)
             except Exception:
                 try:
                     self._fs.removetree(uri)
                 except Exception:  # pragma: no cover
                     pass
         p = FileParser(uri, format_hint)
-        if not force_single and p.file_format != "avro":
+        if not force_single:
             df = self._prepartition(df, partition_spec=partition_spec)
 
             self._saves[p.file_format](df=df, uri=p.uri, **kwargs)
         else:
             ldf = df.as_local()
             self._fs.makedirs(os.path.dirname(uri), recreate=True)
             save_df(ldf, uri, format_hint=format_hint, mode=mode, fs=self._fs, **kwargs)
```

### Comparing `fugue-0.8.3.dev1/fugue_ray/dataframe.py` & `fugue-0.8.4.dev1/fugue_ray/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_ray/execution_engine.py` & `fugue-0.8.4.dev1/fugue_ray/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_ray/registry.py` & `fugue-0.8.4.dev1/fugue_ray/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_spark/_utils/convert.py` & `fugue-0.8.4.dev1/fugue_spark/_utils/convert.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 from typing import Any, Iterable, List, Tuple
 
+import cloudpickle
+import pandas as pd
 import pyarrow as pa
 import pyspark.sql as ps
 import pyspark.sql.types as pt
-
-try:  # pyspark < 3
-    from pyspark.sql.types import from_arrow_type, to_arrow_type  # type: ignore
-
-    # https://issues.apache.org/jira/browse/SPARK-29041
-    pt._acceptable_types[pt.BinaryType] = (bytearray, bytes)  # type: ignore  # pragma: no cover  # noqa: E501  # pylint: disable=line-too-long
-except ImportError:  # pyspark >=3
-    from pyspark.sql.pandas.types import from_arrow_type, to_arrow_type
-
 from pyarrow.types import is_list, is_struct, is_timestamp
+from pyspark.sql.pandas.types import from_arrow_type, to_arrow_type
 from triad.collections import Schema
 from triad.utils.assertion import assert_arg_not_none, assert_or_throw
 from triad.utils.pyarrow import TRIAD_DEFAULT_TIMESTAMP
 from triad.utils.schema import quote_name
 
 
 def to_spark_schema(obj: Any) -> pt.StructType:
@@ -109,14 +103,30 @@
     else:
         for row in rows:
             data = row.asDict(recursive=True)
             r = [data[n] for n in schema.names]
             yield r
 
 
+def to_pandas(df: ps.DataFrame) -> pd.DataFrame:
+    if pd.__version__ < "2" or not any(
+        isinstance(x.dataType, (pt.TimestampType, pt.TimestampNTZType))
+        for x in df.schema.fields
+    ):
+        return df.toPandas()
+
+    def serialize(dfs):  # pragma: no cover
+        for df in dfs:
+            data = cloudpickle.dumps(df)
+            yield pd.DataFrame([[data]], columns=["data"])
+
+    sdf = df.mapInPandas(serialize, schema="data binary")
+    return pd.concat(cloudpickle.loads(x.data) for x in sdf.collect())
+
+
 # TODO: the following function always set nullable to true,
 # but should we use field.nullable?
 def _to_arrow_type(dt: pt.DataType) -> pa.DataType:
     if isinstance(dt, pt.TimestampType):
         return TRIAD_DEFAULT_TIMESTAMP
     if isinstance(dt, pt.StructType):
         fields = [
```

### Comparing `fugue-0.8.3.dev1/fugue_spark/_utils/io.py` & `fugue-0.8.4.dev1/fugue_spark/_utils/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     def __init__(self, spark_session: SparkSession, fs: FileSystem):
         self._session = spark_session
         self._fs = fs
         self._loads: Dict[str, Callable[..., DataFrame]] = {
             "csv": self._load_csv,
             "parquet": self._load_parquet,
             "json": self._load_json,
-            "avro": self._load_avro,
         }
 
     def load_df(
         self,
         uri: Union[str, List[str]],
         format_hint: Optional[str] = None,
         columns: Any = None,
@@ -132,19 +131,7 @@
         reader.options(**kwargs)
         if columns is None:
             return SparkDataFrame(reader.load(p))
         if isinstance(columns, list):  # column names
             return SparkDataFrame(reader.load(p))[columns]
         schema = Schema(columns)
         return SparkDataFrame(reader.load(p)[schema.names], schema)
-
-    def _load_avro(self, p: List[str], columns: Any = None, **kwargs: Any) -> DataFrame:
-        reader = self._session.read.format(
-            "avro"
-        )  # avro is an external data source that has built-in support since spark 2.4
-        reader.options(**kwargs)
-        if columns is None:
-            return SparkDataFrame(reader.load(p))
-        if isinstance(columns, list):  # column names
-            return SparkDataFrame(reader.load(p))[columns]
-        schema = Schema(columns)
-        return SparkDataFrame(reader.load(p)[schema.names], schema)
```

### Comparing `fugue-0.8.3.dev1/fugue_spark/_utils/partition.py` & `fugue-0.8.4.dev1/fugue_spark/_utils/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_spark/dataframe.py` & `fugue-0.8.4.dev1/fugue_spark/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,20 @@
     is_bounded,
     is_df,
     is_empty,
     is_local,
     rename,
     select_columns,
 )
-from fugue_spark._utils.convert import to_cast_expression, to_schema, to_type_safe_input
+from fugue_spark._utils.convert import (
+    to_cast_expression,
+    to_pandas,
+    to_schema,
+    to_type_safe_input,
+)
 
 
 class SparkDataFrame(DataFrame):
     """DataFrame that wraps Spark DataFrame. Please also read
     |DataFrameTutorial| to understand this Fugue concept
 
     :param df: :class:`spark:pyspark.sql.DataFrame`
@@ -90,15 +95,15 @@
         return True
 
     def as_local_bounded(self) -> LocalBoundedDataFrame:
         if any(pa.types.is_nested(t) for t in self.schema.types):
             data = list(to_type_safe_input(self.native.collect(), self.schema))
             res: LocalBoundedDataFrame = ArrayDataFrame(data, self.schema)
         else:
-            res = PandasDataFrame(self.native.toPandas(), self.schema)
+            res = PandasDataFrame(self.as_pandas(), self.schema)
         if self.has_metadata:
             res.reset_metadata(self.metadata)
         return res
 
     @property
     def num_partitions(self) -> int:
         return _spark_num_partitions(self.native)
@@ -122,15 +127,15 @@
         return self._select_cols(cols)
 
     def _select_cols(self, cols: List[Any]) -> DataFrame:
         schema = self.schema.extract(cols)
         return SparkDataFrame(self.native[schema.names])
 
     def as_pandas(self) -> pd.DataFrame:
-        return self.native.toPandas()
+        return to_pandas(self.native)
 
     def rename(self, columns: Dict[str, str]) -> DataFrame:
         try:
             self.schema.rename(columns)
         except Exception as e:
             raise FugueDataFrameOperationError from e
         return SparkDataFrame(_rename_spark_dataframe(self.native, columns))
@@ -210,15 +215,15 @@
 @is_local.candidate(lambda df: isinstance(df, ps.DataFrame))
 def _spark_df_is_local(df: ps.DataFrame) -> bool:
     return False
 
 
 @as_local_bounded.candidate(lambda df: isinstance(df, ps.DataFrame))
 def _spark_df_as_local(df: ps.DataFrame) -> pd.DataFrame:
-    return df.toPandas()
+    return to_pandas(df)
 
 
 @get_column_names.candidate(lambda df: isinstance(df, ps.DataFrame))
 def _get_spark_df_columns(df: ps.DataFrame) -> List[Any]:
     return df.columns
 
 
@@ -260,15 +265,15 @@
     n: int,
     columns: Optional[List[str]] = None,
     as_fugue: bool = False,
 ) -> pd.DataFrame:
     if columns is not None:
         df = df[columns]
     res = df.limit(n)
-    return SparkDataFrame(res).as_local() if as_fugue else res.toPandas()
+    return SparkDataFrame(res).as_local() if as_fugue else to_pandas(res)
 
 
 def _rename_spark_dataframe(df: ps.DataFrame, names: Dict[str, Any]) -> ps.DataFrame:
     cols: List[ps.Column] = []
     for f in df.schema:
         c = col(f.name)
         if f.name in names:
```

### Comparing `fugue-0.8.3.dev1/fugue_spark/execution_engine.py` & `fugue-0.8.4.dev1/fugue_spark/execution_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Type, Union
 from uuid import uuid4
 
 import pandas as pd
 import pyarrow as pa
-import pyspark
 import pyspark.sql as ps
 from pyspark import StorageLevel
 from pyspark.rdd import RDD
 from pyspark.sql import SparkSession
 from pyspark.sql.functions import broadcast, col, lit, row_number
 from pyspark.sql.window import Window
 from triad import FileSystem, IndexedOrderedDict, ParamDict, Schema, SerializableRLock
@@ -39,19 +38,15 @@
     PandasDataFrame,
 )
 from fugue.dataframe.arrow_dataframe import _build_empty_arrow
 from fugue.dataframe.utils import get_join_schemas
 from fugue.exceptions import FugueDataFrameInitError
 from fugue.execution.execution_engine import ExecutionEngine, MapEngine, SQLEngine
 
-from ._constants import (
-    FUGUE_SPARK_CONF_USE_PANDAS_UDF,
-    FUGUE_SPARK_DEFAULT_CONF,
-    _IS_SPARK_2,
-)
+from ._constants import FUGUE_SPARK_CONF_USE_PANDAS_UDF, FUGUE_SPARK_DEFAULT_CONF
 from ._utils.convert import to_schema, to_spark_schema, to_type_safe_input
 from ._utils.io import SparkIO
 from ._utils.partition import even_repartition, hash_repartition, rand_repartition
 from .dataframe import SparkDataFrame
 
 _TO_SPARK_JOIN_MAP: Dict[str, str] = {
     "inner": "inner",
@@ -99,18 +94,14 @@
 class SparkMapEngine(MapEngine):
     @property
     def is_distributed(self) -> bool:
         return True
 
     def _should_use_pandas_udf(self, schema: Schema) -> bool:
         possible = hasattr(ps.DataFrame, "mapInPandas")  # must be new version of Spark
-        if pyspark.__version__ < "3":  # pragma: no cover
-            possible &= self.execution_engine.conf.get(
-                "spark.sql.execution.arrow.enabled", False
-            )
         # else:  # this condition seems to be unnecessary
         #    possible &= self.execution_engine.conf.get(
         #        "spark.sql.execution.arrow.pyspark.enabled", False
         #    )
         enabled = self.execution_engine.conf.get_or_throw(
             FUGUE_SPARK_CONF_USE_PANDAS_UDF, bool
         )
@@ -719,22 +710,22 @@
                 assert_or_throw(
                     schema is None,
                     ValueError("schema must be None when df is a DataFrame"),
                 )
                 if isinstance(df, SparkDataFrame):
                     return df
                 if isinstance(df, ArrowDataFrame):
-                    raw_df: Any = df.as_array() if _IS_SPARK_2 else df.as_pandas()
+                    raw_df: Any = df.as_pandas()
                     sdf = self.spark_session.createDataFrame(
                         raw_df, to_spark_schema(df.schema)
                     )
                     return SparkDataFrame(sdf, df.schema)
                 if isinstance(df, (ArrayDataFrame, IterableDataFrame)):
                     adf = ArrowDataFrame(df.as_array(type_safe=False), df.schema)
-                    raw_df = adf.as_array() if _IS_SPARK_2 else adf.as_pandas()
+                    raw_df = adf.as_pandas()
                     sdf = self.spark_session.createDataFrame(
                         raw_df, to_spark_schema(df.schema)
                     )
                     return SparkDataFrame(sdf, df.schema)
                 if any(pa.types.is_struct(t) for t in df.schema.types):
                     sdf = self.spark_session.createDataFrame(
                         df.as_array(type_safe=True), to_spark_schema(df.schema)
```

### Comparing `fugue-0.8.3.dev1/fugue_spark/ibis_engine.py` & `fugue-0.8.4.dev1/fugue_spark/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_spark/registry.py` & `fugue-0.8.4.dev1/fugue_spark/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_test/bag_suite.py` & `fugue-0.8.4.dev1/fugue_test/bag_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/fugue_test/builtin_suite.py` & `fugue-0.8.4.dev1/fugue_test/builtin_suite.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 from fugue.exceptions import (
     FugueInterfacelessError,
     FugueWorkflowCompileError,
     FugueWorkflowCompileValidationError,
     FugueWorkflowError,
     FugueWorkflowRuntimeValidationError,
 )
-from fugue_test._utils import _is_spark2
 
 
 class BuiltInTests(object):
     """Workflow level general test suite. It is a more general end to end
     test suite than :class:`~fugue_test.execution_suite.ExecutionEngineTests`.
     Any new :class:`~fugue.execution.execution_engine.ExecutionEngine`
     should also pass this test suite.
@@ -1312,20 +1311,21 @@
                 b.partition(by="c").save(path3, fmt="parquet", single=False)
             dag.run(self.engine)
             assert FileSystem().isdir(path3)
             assert FileSystem().isdir(os.path.join(path3, "c=6"))
             assert FileSystem().isdir(os.path.join(path3, "c=2"))
             # TODO: in test below, once issue #288 is fixed, use dag.load
             #  instead of pd.read_parquet
+            pdf = pd.read_parquet(path3).sort_values("a").reset_index(drop=True)
+            pdf["c"] = pdf["c"].astype(int)
             pd.testing.assert_frame_equal(
-                pd.read_parquet(path3).sort_values("a").reset_index(drop=True),
-                pd.DataFrame({"c": pd.Categorical([6, 2]), "a": [1, 7]}).reset_index(
-                    drop=True
-                ),
+                pdf,
+                pd.DataFrame({"c": [6, 2], "a": [1, 7]}).reset_index(drop=True),
                 check_like=True,
+                check_dtype=False,
             )
 
         def test_save_and_use(self):
             path = os.path.join(self.tmpdir, "a")
             with FugueWorkflow() as dag:
                 b = dag.df([[6, 1], [2, 7]], "c:int,a:long")
                 c = b.save_and_use(path, fmt="parquet")
@@ -1671,17 +1671,15 @@
                 """,
                     as_fugue=False,
                     as_local=True,
                 )
                 assert not isinstance(sdf4, DataFrame)
                 assert fa.is_local(sdf4)
 
-        @pytest.mark.skipif(
-            _is_spark2() or os.name == "nt", reason="Skip Spark<3 or Windows"
-        )
+        @pytest.mark.skipif(os.name == "nt", reason="Skip Windows")
         def test_any_column_name(self):
 
             f_parquet = os.path.join(str(self.tmpdir), "a.parquet")
             f_csv = os.path.join(str(self.tmpdir), "a.csv")
 
             # schema: *,`c *`:long
             def tr(df: pd.DataFrame) -> pd.DataFrame:
```

### Comparing `fugue-0.8.3.dev1/fugue_test/dataframe_suite.py` & `fugue-0.8.4.dev1/fugue_test/dataframe_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,33 +411,37 @@
             assert [["a", 1.1], ["b", 2.0], ["c", None]] == fi.as_array(
                 ndf, type_safe=True
             )
             assert fi.get_schema(ndf) == "a:str,b:double"
 
             # str -> date
             df = self.df(
-                [["1", "2020-01-01"], ["2", "2020-01-02 01:02:03"], ["3", None]],
+                [["1", "2020-01-01"], ["2", "2020-01-02"], ["3", None]],
                 "a:str,b:str",
             )
             ndf = fi.alter_columns(df, "b:date,a:int", as_fugue=True)
             assert [
                 [1, date(2020, 1, 1)],
                 [2, date(2020, 1, 2)],
                 [3, None],
             ] == fi.as_array(ndf, type_safe=True)
             assert fi.get_schema(ndf) == "a:int,b:date"
 
             # str -> datetime
             df = self.df(
-                [["1", "2020-01-01"], ["2", "2020-01-02 01:02:03"], ["3", None]],
+                [
+                    ["1", "2020-01-01 01:02:03"],
+                    ["2", "2020-01-02 01:02:03"],
+                    ["3", None],
+                ],
                 "a:str,b:str",
             )
             ndf = fi.alter_columns(df, "b:datetime,a:int", as_fugue=True)
             assert [
-                [1, datetime(2020, 1, 1)],
+                [1, datetime(2020, 1, 1, 1, 2, 3)],
                 [2, datetime(2020, 1, 2, 1, 2, 3)],
                 [3, None],
             ] == fi.as_array(ndf, type_safe=True)
             assert fi.get_schema(ndf) == "a:int,b:datetime"
 
         def test_alter_columns_invalid(self):
             # invalid conversion
```

### Comparing `fugue-0.8.3.dev1/fugue_test/execution_suite.py` & `fugue-0.8.4.dev1/fugue_test/execution_suite.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     PandasDataFrame,
     PartitionSpec,
     register_default_sql_engine,
 )
 from fugue.column import all_cols, col, lit
 from fugue.dataframe.utils import _df_eq as df_eq
 from fugue.execution.native_execution_engine import NativeExecutionEngine
-from fugue_test._utils import skip_spark2
 
 
 class ExecutionEngineTests(object):
     """ExecutionEngine level general test suite.
     Any new :class:`~fugue.execution.execution_engine.ExecutionEngine`
     should pass this test suite.
     """
@@ -1084,55 +1083,14 @@
             fa.save(a, f1, engine=native)
             fa.save(b, f2, engine=native)
             c = fa.load(
                 [f1, f2], format_hint="parquet", columns=["a", "c"], as_fugue=True
             )
             df_eq(c, [[1, 6], [7, 2], [8, 4]], "a:long,c:int", throw=True)
 
-        @skip_spark2
-        def test_save_single_and_load_avro(self):
-            # TODO: switch to c:int,a:long when we can preserve schema to avro
-            e = self.engine
-            b = ArrayDataFrame([[6, 1], [2, 7]], "c:long,a:long")
-            path = os.path.join(self.tmpdir, "a", "b")
-            e.fs.makedirs(path, recreate=True)
-            # over write folder with single file
-            fa.save(b, path, format_hint="avro", force_single=True)
-            assert e.fs.isfile(path)
-            c = fa.load(path, format_hint="avro", columns=["a", "c"], as_fugue=True)
-            df_eq(c, [[1, 6], [7, 2]], "a:long,c:long", throw=True)
-
-            # overwirte single with folder (if applicable)
-            b = ArrayDataFrame([[60, 1], [20, 7]], "c:long,a:long")
-            fa.save(b, path, format_hint="avro", mode="overwrite")
-            c = fa.load(path, format_hint="avro", columns=["a", "c"], as_fugue=True)
-            df_eq(c, [[1, 60], [7, 20]], "a:long,c:long", throw=True)
-
-        @skip_spark2
-        def test_save_and_load_avro(self):
-            # TODO: switch to c:int,a:long when we can preserve schema to avro
-            b = ArrayDataFrame([[6, 1], [2, 7]], "c:long,a:long")
-            path = os.path.join(self.tmpdir, "a", "b")
-            fa.save(b, path, format_hint="avro")
-            c = fa.load(path, format_hint="avro", columns=["a", "c"], as_fugue=True)
-            df_eq(c, [[1, 6], [7, 2]], "a:long,c:long", throw=True)
-
-        @skip_spark2
-        def test_load_avro_folder(self):
-            # TODO: switch to c:int,a:long when we can preserve schema to avro
-            native = NativeExecutionEngine()
-            a = ArrayDataFrame([[6, 1]], "c:long,a:long")
-            b = ArrayDataFrame([[2, 7], [4, 8]], "c:long,a:long")
-            path = os.path.join(self.tmpdir, "a", "b")
-            fa.save(a, os.path.join(path, "a.avro"), engine=native)
-            fa.save(b, os.path.join(path, "b.avro"), engine=native)
-            FileSystem().touch(os.path.join(path, "_SUCCESS"))
-            c = fa.load(path, format_hint="avro", columns=["a", "c"], as_fugue=True)
-            df_eq(c, [[1, 6], [7, 2], [8, 4]], "a:long,c:long", throw=True)
-
         def test_save_single_and_load_csv(self):
             e = self.engine
             b = ArrayDataFrame([[6.1, 1.1], [2.1, 7.1]], "c:double,a:double")
             path = os.path.join(self.tmpdir, "a", "b")
             e.fs.makedirs(path, recreate=True)
             # over write folder with single file
             fa.save(b, path, format_hint="csv", header=True, force_single=True)
```

### Comparing `fugue-0.8.3.dev1/fugue_test/ibis_suite.py` & `fugue-0.8.4.dev1/fugue_test/ibis_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/setup.cfg` & `fugue-0.8.4.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/setup.py` & `fugue-0.8.4.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,30 +27,30 @@
     long_description_content_type="text/markdown",
     license="Apache-2.0",
     author="The Fugue Development Team",
     author_email="hello@fugue.ai",
     keywords="distributed spark dask sql dsl domain specific language",
     url="http://github.com/fugue-project/fugue",
     install_requires=[
-        "triad>=0.8.4",
+        "triad>=0.8.6",
         "adagio>=0.2.4",
-        "qpd>=0.4.0",
+        "qpd>=0.4.1",
         "fugue-sql-antlr>=0.1.6",
         "pyarrow>=0.15.1",
-        "pandas>=1.2.0,<2",
+        "pandas>=1.2.0",
         "sqlglot",
         "jinja2",
     ],
     extras_require={
         "cpp_sql_parser": ["fugue-sql-antlr[cpp]>=0.1.6"],
         "spark": ["pyspark"],
         "dask": [
             "dask[distributed,dataframe]; python_version < '3.8'",
             "dask[distributed,dataframe]>=2022.9.0; python_version >= '3.8'",
-            "qpd[dask]>=0.4.0",
+            "qpd[dask]>=0.4.1",
         ],
         "ray": ["ray[data]>=2.0.0", "duckdb>=0.5.0", "pyarrow>=6.0.1"],
         "duckdb": [
             "duckdb>=0.5.0",
             "pyarrow>=6.0.1",
             "numpy",
         ],
```

### Comparing `fugue-0.8.3.dev1/tests/fugue/bag/test_array_bag.py` & `fugue-0.8.4.dev1/tests/fugue/bag/test_array_bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/collections/test_partition.py` & `fugue-0.8.4.dev1/tests/fugue/collections/test_partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/collections/test_sql.py` & `fugue-0.8.4.dev1/tests/fugue/collections/test_sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/column/test_expressions.py` & `fugue-0.8.4.dev1/tests/fugue/column/test_expressions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/column/test_functions.py` & `fugue-0.8.4.dev1/tests/fugue/column/test_functions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/column/test_sql.py` & `fugue-0.8.4.dev1/tests/fugue/column/test_sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/dataframe/test_array_dataframe.py` & `fugue-0.8.4.dev1/tests/fugue/dataframe/test_array_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/dataframe/test_arrow_dataframe.py` & `fugue-0.8.4.dev1/tests/fugue/dataframe/test_arrow_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/dataframe/test_dataframe.py` & `fugue-0.8.4.dev1/tests/fugue/dataframe/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/dataframe/test_dataframe_iterable_dataframe.py` & `fugue-0.8.4.dev1/tests/fugue/dataframe/test_dataframe_iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/dataframe/test_dataframes.py` & `fugue-0.8.4.dev1/tests/fugue/dataframe/test_dataframes.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/dataframe/test_function_wrapper.py` & `fugue-0.8.4.dev1/tests/fugue/dataframe/test_function_wrapper.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/dataframe/test_iterable_dataframe.py` & `fugue-0.8.4.dev1/tests/fugue/dataframe/test_iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/dataframe/test_pandas_dataframe.py` & `fugue-0.8.4.dev1/tests/fugue/dataframe/test_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/dataframe/test_utils.py` & `fugue-0.8.4.dev1/tests/fugue/dataframe/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     assert _schema_eq(s1, s2)
 
 
 def test_df_eq():
     df1 = ArrayDataFrame([[0, 100.0, "a"]], "a:int,b:double,c:str")
     df2 = ArrayDataFrame([[0, 100.001, "a"]], "a:int,b:double,c:str")
     assert df_eq(df1, df1)
-    assert df_eq(df1, df2, digits=4)
+    assert df_eq(df1, df2, digits=2)
     # precision
     assert not df_eq(df1, df2, digits=6)
     # no content
     assert df_eq(df1, df2, digits=6, check_content=False)
     raises(AssertionError, lambda: df_eq(df1, df2, throw=True))
 
     df1 = ArrayDataFrame([[100.0, "a"]], "a:double,b:str")
```

### Comparing `fugue-0.8.3.dev1/tests/fugue/execution/test_api.py` & `fugue-0.8.4.dev1/tests/fugue/execution/test_api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/execution/test_execution_engine.py` & `fugue-0.8.4.dev1/tests/fugue/execution/test_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/execution/test_factory.py` & `fugue-0.8.4.dev1/tests/fugue/execution/test_factory.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/execution/test_ibis.py` & `fugue-0.8.4.dev1/tests/fugue/execution/test_ibis.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/execution/test_naive_execution_engine.py` & `fugue-0.8.4.dev1/tests/fugue/execution/test_naive_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/extensions/creator/__init__.py` & `fugue-0.8.4.dev1/tests/fugue/extensions/creator/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/extensions/creator/test_convert.py` & `fugue-0.8.4.dev1/tests/fugue/extensions/creator/test_convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/extensions/outputter/__init__.py` & `fugue-0.8.4.dev1/tests/fugue/extensions/outputter/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/extensions/outputter/test_convert.py` & `fugue-0.8.4.dev1/tests/fugue/extensions/outputter/test_convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/extensions/processor/__init__.py` & `fugue-0.8.4.dev1/tests/fugue/extensions/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/extensions/processor/test_convert.py` & `fugue-0.8.4.dev1/tests/fugue/extensions/processor/test_convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/extensions/test_utils.py` & `fugue-0.8.4.dev1/tests/fugue/extensions/test_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/extensions/transformer/test_convert_cotransformer.py` & `fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_cotransformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/extensions/transformer/test_convert_output_cotransformer.py` & `fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_output_cotransformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/extensions/transformer/test_convert_output_transformer.py` & `fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_output_transformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/extensions/transformer/test_convert_transformer.py` & `fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_transformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/rpc/test_base.py` & `fugue-0.8.4.dev1/tests/fugue/rpc/test_base.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/rpc/test_flask.py` & `fugue-0.8.4.dev1/tests/fugue/rpc/test_flask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/rpc/test_func.py` & `fugue-0.8.4.dev1/tests/fugue/rpc/test_func.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/sql/test_utils.py` & `fugue-0.8.4.dev1/tests/fugue/sql/test_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/sql/test_visitors.py` & `fugue-0.8.4.dev1/tests/fugue/sql/test_visitors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/sql/test_workflow.py` & `fugue-0.8.4.dev1/tests/fugue/sql/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/sql/test_workflow_parse.py` & `fugue-0.8.4.dev1/tests/fugue/sql/test_workflow_parse.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/test_interfaceless.py` & `fugue-0.8.4.dev1/tests/fugue/test_interfaceless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/utils/test_interfaceless.py` & `fugue-0.8.4.dev1/tests/fugue/utils/test_interfaceless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/workflow/test_module.py` & `fugue-0.8.4.dev1/tests/fugue/workflow/test_module.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/workflow/test_runtime_exception.py` & `fugue-0.8.4.dev1/tests/fugue/workflow/test_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/workflow/test_workflow.py` & `fugue-0.8.4.dev1/tests/fugue/workflow/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/workflow/test_workflow_determinism.py` & `fugue-0.8.4.dev1/tests/fugue/workflow/test_workflow_determinism.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue/workflow/test_workflow_parallel.py` & `fugue-0.8.4.dev1/tests/fugue/workflow/test_workflow_parallel.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_dask/test_dataframe.py` & `fugue-0.8.4.dev1/tests/fugue_dask/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_dask/test_execution_engine.py` & `fugue-0.8.4.dev1/tests/fugue_dask/test_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_dask/test_importless.py` & `fugue-0.8.4.dev1/tests/fugue_dask/test_importless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_dask/test_io.py` & `fugue-0.8.4.dev1/tests/fugue_dask/test_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -113,62 +113,7 @@
     actual = load_df(path)
     df_eq(actual, [[1, 2, 3]], "a:long,b:long,c:long")
     actual = load_df(path, columns=["b", "a"])
     df_eq(actual, [[2, "1"]], "b:int,a:str")
     actual = load_df(path, columns="b:str,a:int")
     df_eq(actual, [["2", 1]], "b:str,a:int")
     raises(KeyError, lambda: load_df(path, columns="bb:str,a:int"))
-
-
-@mark.skip(reason="Unable to test due to spark jars not being downloaded properly")
-def test_avro_io(tmpdir):
-    df1 = DaskDataFrame([["1", 2, 3]], "a:str,b:int,c:long")
-    path = os.path.join(tmpdir, "a.avro")
-    save_df(df1, path)
-    actual = load_df(path)
-
-    df_eq(actual, [["1", 2, 3]], "a:str,b:long,c:long")
-    actual = load_df(path, columns=["a", "b"])
-    df_eq(actual, [["1", 3]], "a:str,b:long")
-
-    actual = load_df(path, columns="a:str,b:int,c:long")
-    df_eq(actual, [["1", 2, 3]], "a:str,b:int,c:long")
-
-    actual = load_df(path, columns=["b", "c"], infer_schema=True)
-    df_eq(actual, [[2, 3]], "b:long,c:long")
-
-    # provide schema and columns -> throw error
-    raises(
-        Exception,
-        lambda: save_df(
-            path,
-            columns="a:str,b:int,c:long",
-            schema={
-                "type": "record",
-                "name": "Root",
-                "fields": [
-                    {"name": "station", "type": "string"},
-                    {"name": "time", "type": "long"},
-                    {"name": "temp", "type": "int"},
-                ],
-            },
-        ),
-    )
-
-    # provide schema and infer_schema is True -> throw error
-    raises(
-        Exception,
-        lambda: save_df(
-            path,
-            columns=None,
-            schema={
-                "type": "record",
-                "name": "Root",
-                "fields": [
-                    {"name": "station", "type": "string"},
-                    {"name": "time", "type": "long"},
-                    {"name": "temp", "type": "int"},
-                ],
-            },
-            infer_schema=True,
-        ),
-    )
```

### Comparing `fugue-0.8.3.dev1/tests/fugue_dask/test_sql.py` & `fugue-0.8.4.dev1/tests/fugue_dask/test_sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_duckdb/test_dask.py` & `fugue-0.8.4.dev1/tests/fugue_duckdb/test_dask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_duckdb/test_dataframe.py` & `fugue-0.8.4.dev1/tests/fugue_duckdb/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_duckdb/test_execution_engine.py` & `fugue-0.8.4.dev1/tests/fugue_duckdb/test_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_duckdb/test_ibis.py` & `fugue-0.8.4.dev1/tests/fugue_duckdb/test_ibis.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_duckdb/test_importless.py` & `fugue-0.8.4.dev1/tests/fugue_duckdb/test_importless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_duckdb/test_utils.py` & `fugue-0.8.4.dev1/tests/fugue_duckdb/test_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_ibis/mock/dataframe.py` & `fugue-0.8.4.dev1/tests/fugue_ibis/mock/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_ibis/mock/execution_engine.py` & `fugue-0.8.4.dev1/tests/fugue_ibis/mock/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_ibis/test_dataframe.py` & `fugue-0.8.4.dev1/tests/fugue_ibis/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_ibis/test_execution_engine.py` & `fugue-0.8.4.dev1/tests/fugue_ibis/test_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_ibis/test_extensions.py` & `fugue-0.8.4.dev1/tests/fugue_ibis/test_extensions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_ibis/test_utils.py` & `fugue-0.8.4.dev1/tests/fugue_ibis/test_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_polars/test_dataframe.py` & `fugue-0.8.4.dev1/tests/fugue_polars/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_polars/test_transform.py` & `fugue-0.8.4.dev1/tests/fugue_polars/test_transform.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 import pandas as pd
 
 import fugue.api as fa
 
 
 def test_transform_common():
     def tr1(df: pl.DataFrame) -> pl.DataFrame:
-        tdf = df.with_column(pl.lit(1, pl.Int32()).alias("b"))
+        tdf = df.with_columns(pl.lit(1, pl.Int32()).alias("b"))
         return tdf
 
     def tr2(dfs: Iterable[pl.DataFrame]) -> Iterator[pl.DataFrame]:
         for df in dfs:
-            tdf = df.with_column(pl.lit(1, pl.Int32()).alias("b"))
+            tdf = df.with_columns(pl.lit(1, pl.Int32()).alias("b"))
             yield tdf
 
     for tr in [tr1, tr2]:
         df = fa.as_fugue_df([[0], [1]], schema="a:int")
         fdf = fa.transform(df, tr, schema="a:int,b:int", as_fugue=True)
         assert fdf.schema == "a:int,b:int"
         assert fdf.as_array() == [[0, 1], [1, 1]]
@@ -46,15 +46,15 @@
         fdf = fa.transform(df, tr, schema="a:int,b:int", as_fugue=True)
         assert fdf.schema == "a:int,b:int"
         assert fdf.as_array() == [[0, 1], [1, 1]]
 
 
 def test_transform_empty_result():
     def tr1(df: pl.DataFrame) -> pl.DataFrame:
-        tdf = df.with_column(pl.lit(1, pl.Int32()).alias("b"))
+        tdf = df.with_columns(pl.lit(1, pl.Int32()).alias("b"))
         return tdf.head(0)
 
     def tr2(dfs: Iterable[pl.DataFrame]) -> Iterator[pl.DataFrame]:
         for _ in []:
             yield None
 
     def tr3(dfs: Iterable[pl.DataFrame]) -> Iterator[pl.DataFrame]:
@@ -65,20 +65,20 @@
         fdf = fa.transform(df, tr, schema="a:int,b:int", as_fugue=True)
         assert fdf.schema == "a:int,b:int"
         assert fdf.as_array() == []
 
 
 def test_polars_on_engines():
     def tr1(df: pl.DataFrame) -> pl.DataFrame:
-        tdf = df.with_column(pl.lit(1, pl.Int32()).alias("c"))
+        tdf = df.with_columns(pl.lit(1, pl.Int32()).alias("c"))
         return tdf
 
     def tr2(dfs: Iterable[pl.DataFrame]) -> Iterator[pl.DataFrame]:
         for df in dfs:
-            tdf = df.with_column(pl.lit(1, pl.Int32()).alias("c"))
+            tdf = df.with_columns(pl.lit(1, pl.Int32()).alias("c"))
             yield tdf
 
     def test(engine):
         for tr in [tr1, tr2]:
             with fa.engine_context(engine):
                 df = fa.as_fugue_df(
                     [["a", datetime(2022, 1, 1)], ["b", datetime(2022, 1, 2)]],
```

### Comparing `fugue-0.8.3.dev1/tests/fugue_ray/test_dataframe.py` & `fugue-0.8.4.dev1/tests/fugue_ray/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_ray/test_execution_engine.py` & `fugue-0.8.4.dev1/tests/fugue_ray/test_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_ray/test_registry.py` & `fugue-0.8.4.dev1/tests/fugue_ray/test_registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_ray/test_utils.py` & `fugue-0.8.4.dev1/tests/fugue_ray/test_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_spark/test_dataframe.py` & `fugue-0.8.4.dev1/tests/fugue_spark/test_dataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,14 @@
         engine = SparkExecutionEngine(session)
         return engine.to_df(data, schema=schema)
 
     def test_alter_columns_invalid(self):
         # TODO: Spark will silently cast invalid data to nulls without exceptions
         pass
 
-    def test_map_type(self):
-        if pyspark.__version__ >= "3":
-            return super().test_map_type()
-
 
 class NativeSparkDataFrameTests(DataFrameTests.NativeTests):
     @pytest.fixture(autouse=True)
     def init_session(self, spark_session):
         self.spark_session = spark_session
 
     def df(self, data: Any = None, schema: Any = None):
@@ -51,18 +47,14 @@
     def test_not_local(self):
         assert not fi.is_local(self.df([], "a:int,b:str"))
 
     def test_alter_columns_invalid(self):
         # TODO: Spark will silently cast invalid data to nulls without exceptions
         pass
 
-    def test_map_type(self):
-        if pyspark.__version__ >= "3":
-            return super().test_map_type()
-
 
 def test_init(spark_session):
     sdf = spark_session.createDataFrame([["a", 1]])
     df = SparkDataFrame(sdf, "a:str,b:double")
     assert [["a", 1.0]] == df.as_array()
     assert [["a", 1.0]] == df.as_pandas().values.tolist()
     assert not df.is_local
```

### Comparing `fugue-0.8.3.dev1/tests/fugue_spark/test_execution_engine.py` & `fugue-0.8.4.dev1/tests/fugue_spark/test_execution_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     LocalDataFrameIterableDataFrame,
     PandasDataFrame,
 )
 from fugue.dataframe.utils import _df_eq as df_eq
 from fugue.extensions.transformer import Transformer, transformer
 from fugue.plugins import infer_execution_engine
 from fugue.workflow.workflow import FugueWorkflow
+from fugue_spark._utils.convert import to_pandas
 from fugue_spark.dataframe import SparkDataFrame
 from fugue_spark.execution_engine import SparkExecutionEngine
 from fugue_test.builtin_suite import BuiltInTests
 from fugue_test.execution_suite import ExecutionEngineTests
 
 
 class SparkExecutionEngineTests(ExecutionEngineTests.Tests):
@@ -122,15 +123,14 @@
         df = self.spark_session.createDataFrame(pd.DataFrame([[0]], columns=["a"]))
         assert isinstance(infer_execution_engine([df]), SparkSession)
 
         fdf = SparkDataFrame(df)
         assert isinstance(infer_execution_engine([fdf]), SparkSession)
 
 
-@pytest.mark.skipif(pyspark.__version__ < "3", reason="pyspark < 3")
 class SparkExecutionEnginePandasUDFTests(ExecutionEngineTests.Tests):
     @pytest.fixture(autouse=True)
     def init_session(self, spark_session):
         self.spark_session = spark_session
 
     def make_engine(self):
         session = SparkSession.builder.getOrCreate()
@@ -308,25 +308,25 @@
 
         # schema:*
         def f1(df: pd.DataFrame) -> pd.DataFrame:
             return df.sort_values("b").head(1)
 
         result = transform(sdf, f1, partition=dict(by=["a"]), engine=self.engine)
         assert isinstance(result, SDataFrame)
-        assert result.toPandas().sort_values(["a"]).values.tolist() == [[0, 0], [1, 1]]
+        assert to_pandas(result).sort_values(["a"]).values.tolist() == [[0, 0], [1, 1]]
 
     def test_annotation_1(self):
         def m_c(engine: SparkExecutionEngine) -> ps.DataFrame:
             return engine.spark_session.createDataFrame([[0]], "a:long")
 
         def m_p(engine: SparkExecutionEngine, df: ps.DataFrame) -> ps.DataFrame:
             return df
 
         def m_o(engine: SparkExecutionEngine, df: ps.DataFrame) -> None:
-            assert 1 == df.toPandas().shape[0]
+            assert 1 == to_pandas(df).shape[0]
 
         with FugueWorkflow() as dag:
             df = dag.create(m_c).process(m_p)
             df.assert_eq(dag.df([[0]], "a:long"))
             df.output(m_o)
         dag.run(self.engine)
 
@@ -336,15 +336,15 @@
 
         def m_p(session: SparkSession, df: ps.DataFrame) -> ps.DataFrame:
             assert isinstance(session, SparkSession)
             return df
 
         def m_o(session: SparkSession, df: ps.DataFrame) -> None:
             assert isinstance(session, SparkSession)
-            assert 1 == df.toPandas().shape[0]
+            assert 1 == to_pandas(df).shape[0]
 
         with FugueWorkflow() as dag:
             df = dag.create(m_c).process(m_p)
             df.assert_eq(dag.df([[0]], "a:long"))
             df.output(m_o)
         dag.run(self.engine)
```

### Comparing `fugue-0.8.3.dev1/tests/fugue_spark/test_ibis.py` & `fugue-0.8.4.dev1/tests/fugue_spark/test_ibis.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_spark/test_importless.py` & `fugue-0.8.4.dev1/tests/fugue_spark/test_importless.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from fugue import FugueWorkflow, transform
-from fugue import fsql
-from pyspark.sql import SparkSession, DataFrame
 import pandas as pd
+from pyspark.sql import DataFrame, SparkSession
 
+from fugue import FugueWorkflow, fsql, transform
+from fugue_spark._utils.convert import to_pandas
 from fugue_spark.registry import _is_sparksql
 
 
 def test_importless(spark_session):
     for engine in [spark_session, "spark"]:
         dag = FugueWorkflow()
         dag.df([[0]], "a:int").show()
@@ -37,8 +37,8 @@
 def test_transform_from_sparksql(spark_session):
     # schema: *
     def t(df: pd.DataFrame) -> pd.DataFrame:
         return df
 
     res = transform(("sparksql", "SELECT 1 AS a, 'b' AS aa"), t)
     assert isinstance(res, DataFrame)  # engine inference
-    assert res.toPandas().to_dict("records") == [{"a": 1, "aa": "b"}]
+    assert to_pandas(res).to_dict("records") == [{"a": 1, "aa": "b"}]
```

### Comparing `fugue-0.8.3.dev1/tests/fugue_spark/test_sql.py` & `fugue-0.8.4.dev1/tests/fugue_spark/test_sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.3.dev1/tests/fugue_spark/utils/test_convert.py` & `fugue-0.8.4.dev1/tests/fugue_spark/utils/test_convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pyspark
 from fugue_spark._utils.convert import (
     to_cast_expression,
     to_schema,
     to_select_expression,
     to_spark_schema,
 )
 from pytest import raises
@@ -49,21 +48,20 @@
             )
         ]
     )
     df = spark_session.createDataFrame([[[("a", 1), ("b", 2)]]], schema)
     assert to_schema(df) == "name:[{nest_name:str,nest_value:int}]"
     assert to_spark_schema("name:[{nest_name:str,nest_value:int}]") == schema
 
-    if pyspark.__version__ >= "3":
-        schema = StructType(
-            [StructField("a", MapType(StringType(), IntegerType(), True), True)],
-        )
-        df = spark_session.createDataFrame([[{"x": 1}], [{"y": 2}]], schema)
-        assert to_schema(df) == "a:<str,int>"
-        assert to_spark_schema("a:<str,int>") == schema
+    schema = StructType(
+        [StructField("a", MapType(StringType(), IntegerType(), True), True)],
+    )
+    df = spark_session.createDataFrame([[{"x": 1}], [{"y": 2}]], schema)
+    assert to_schema(df) == "a:<str,int>"
+    assert to_spark_schema("a:<str,int>") == schema
 
 
 def test_to_cast_expression():
     # length mismatch
     raises(ValueError, lambda: to_cast_expression("a:int,b:int", "a:int", False))
     assert (False, ["a", "b"]) == to_cast_expression(
         "a:int,b:int", "a:int,b:int", False
```

### Comparing `fugue-0.8.3.dev1/tests/fugue_spark/utils/test_io.py` & `fugue-0.8.4.dev1/tests/fugue_spark/utils/test_io.py`

 * *Files 11% similar despite different names*

```diff
@@ -101,31 +101,14 @@
     actual = si.load_df(path, columns=["b", "a"])
     df_eq(actual, [[2, "1"]], "b:int,a:str")
     actual = si.load_df(path, columns="b:str,a:int")
     df_eq(actual, [["2", 1]], "b:str,a:int")
     raises(Exception, lambda: si.load_df(path, columns="bb:str,a:int"))
 
 
-def test_avro_io(tmpdir, spark_session):
-    if spark_session.version < "3.0.0":
-        return
-    fs = FileSystem()
-    si = SparkIO(spark_session, fs)
-    df1 = _df([["1", 2, 3]], "a:str,b:int,c:long")
-    path = os.path.join(tmpdir, "a.avro")
-    si.save_df(df1, path)
-    actual = si.load_df(path)
-    df_eq(actual, [["1", 2, 3]], "a:str,b:int,c:long")
-    actual = si.load_df(path, columns=["b", "a"])
-    df_eq(actual, [[2, "1"]], "b:int,a:str")
-    actual = si.load_df(path, columns="b:str,a:int")
-    df_eq(actual, [["2", 1]], "b:str,a:int")
-    raises(Exception, lambda: si.load_df(path, columns="bb:str,a:int"))
-
-
 def test_save_with_partition(tmpdir, spark_session):
     si = SparkIO(spark_session, FileSystem())
     df1 = _df([["1", 2, 3]], "a:str,b:int,c:long")
     path = os.path.join(tmpdir, "a.parquet")
     si.save_df(df1, path, partition_spec=PartitionSpec(num=2))
     actual = si.load_df(path, columns=["b", "a"])
     df_eq(actual, [[2, "1"]], "b:int,a:str")
```

### Comparing `fugue-0.8.3.dev1/tests/fugue_spark/utils/test_partition.py` & `fugue-0.8.4.dev1/tests/fugue_spark/utils/test_partition.py`

 * *Files identical despite different names*

