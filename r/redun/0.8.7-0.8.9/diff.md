# Comparing `tmp/redun-0.8.7.tar.gz` & `tmp/redun-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/redun-0.8.7.tar", last modified: Fri Mar 11 19:38:15 2022, max compression
+gzip compressed data, was "dist/redun-0.8.9.tar", last modified: Wed May 18 15:49:22 2022, max compression
```

## Comparing `redun-0.8.7.tar` & `redun-0.8.9.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 19:38:15.000000 redun-0.8.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 19:38:15.000000 redun-0.8.7/bin/
--rwxr-xr-x   0 root         (0) root         (0)      402 2022-03-11 19:11:04.000000 redun-0.8.7/bin/redun
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 19:38:15.000000 redun-0.8.7/redun/
--rw-r--r--   0 root         (0) root         (0)     2665 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tags.py
--rw-r--r--   0 root         (0) root         (0)     4765 2022-03-11 19:11:04.000000 redun-0.8.7/redun/glue.py
--rw-r--r--   0 root         (0) root         (0)    11044 2022-03-11 19:11:04.000000 redun-0.8.7/redun/expression.py
--rw-r--r--   0 root         (0) root         (0)    33536 2022-03-11 19:11:04.000000 redun-0.8.7/redun/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 19:38:15.000000 redun-0.8.7/redun/contrib/
--rw-r--r--   0 root         (0) root         (0)     1783 2022-03-11 19:11:04.000000 redun-0.8.7/redun/contrib/spark_helpers.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-11 19:11:04.000000 redun-0.8.7/redun/contrib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3031 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tools.py
--rw-r--r--   0 root         (0) root         (0)    40595 2022-03-11 19:11:04.000000 redun-0.8.7/redun/file.py
--rw-r--r--   0 root         (0) root         (0)     7251 2022-03-11 19:11:04.000000 redun-0.8.7/redun/handle.py
--rw-r--r--   0 root         (0) root         (0)    11414 2022-03-11 19:11:04.000000 redun-0.8.7/redun/utils.py
--rw-r--r--   0 root         (0) root         (0)     2424 2022-03-11 19:11:04.000000 redun-0.8.7/redun/hashing.py
--rw-r--r--   0 root         (0) root         (0)     6165 2022-03-11 19:11:04.000000 redun-0.8.7/redun/promise.py
--rw-r--r--   0 root         (0) root         (0)   107618 2022-03-11 19:11:04.000000 redun-0.8.7/redun/cli.py
--rw-r--r--   0 root         (0) root         (0)     7397 2022-03-11 19:11:04.000000 redun-0.8.7/redun/scripting.py
--rw-r--r--   0 root         (0) root         (0)      375 2022-03-11 19:11:04.000000 redun-0.8.7/redun/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 19:38:15.000000 redun-0.8.7/redun/tests/
--rw-r--r--   0 root         (0) root         (0)     2583 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_namespace.py
--rw-r--r--   0 root         (0) root         (0)      804 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_typing.py
--rw-r--r--   0 root         (0) root         (0)     6084 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     4124 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_value.py
--rw-r--r--   0 root         (0) root         (0)     2586 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_value_store.py
--rw-r--r--   0 root         (0) root         (0)     4448 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     5680 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_expression.py
--rw-r--r--   0 root         (0) root         (0)     7402 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_promise.py
--rw-r--r--   0 root         (0) root         (0)    10595 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_partial_task.py
--rw-r--r--   0 root         (0) root         (0)    10589 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/utils.py
--rw-r--r--   0 root         (0) root         (0)    11643 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_script.py
--rw-r--r--   0 root         (0) root         (0)     5358 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     2649 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_bcoding.py
--rw-r--r--   0 root         (0) root         (0)    20178 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_handle.py
--rw-r--r--   0 root         (0) root         (0)     7218 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_repos.py
--rw-r--r--   0 root         (0) root         (0)     4107 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_process_executor.py
--rw-r--r--   0 root         (0) root         (0)    14184 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_scheduler_subrun.py
--rw-r--r--   0 root         (0) root         (0)     2436 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_s3.py
--rw-r--r--   0 root         (0) root         (0)    12701 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_tags.py
--rw-r--r--   0 root         (0) root         (0)     8585 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_type_registry.py
--rw-r--r--   0 root         (0) root         (0)     7045 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)    12753 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_aws_glue.py
--rw-r--r--   0 root         (0) root         (0)    16449 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 19:38:15.000000 redun-0.8.7/redun/tests/scripts/
--rw-r--r--   0 root         (0) root         (0)     2008 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/scripts/workflow_subrun_process_executor.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22826 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_dataflow.py
--rw-r--r--   0 root         (0) root         (0)      495 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/task_test_helpers.py
--rw-r--r--   0 root         (0) root         (0)    51440 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_aws_batch.py
--rw-r--r--   0 root         (0) root         (0)     2506 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_uri_parsing.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      500 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_hashing.py
--rw-r--r--   0 root         (0) root         (0)     4423 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_logging.py
--rw-r--r--   0 root         (0) root         (0)    19230 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_file.py
--rw-r--r--   0 root         (0) root         (0)    13693 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_serializers.py
--rw-r--r--   0 root         (0) root         (0)     3545 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_args.py
--rw-r--r--   0 root         (0) root         (0)    51098 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     7325 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_functools.py
--rw-r--r--   0 root         (0) root         (0)     3476 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_static_analysis.py
--rw-r--r--   0 root         (0) root         (0)     2605 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_db_utils.py
--rw-r--r--   0 root         (0) root         (0)    36427 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     3814 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_limits.py
--rw-r--r--   0 root         (0) root         (0)     2442 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_executors.py
--rw-r--r--   0 root         (0) root         (0)    30442 2022-03-11 19:11:04.000000 redun-0.8.7/redun/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    19028 2022-03-11 19:11:04.000000 redun-0.8.7/redun/value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 19:38:15.000000 redun-0.8.7/redun/backends/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 19:38:15.000000 redun-0.8.7/redun/backends/db/
--rw-r--r--   0 root         (0) root         (0)    44907 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/dataflow.py
--rw-r--r--   0 root         (0) root         (0)    17960 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/query.py
--rw-r--r--   0 root         (0) root         (0)     2051 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 19:38:15.000000 redun-0.8.7/redun/backends/db/alembic/
--rw-r--r--   0 root         (0) root         (0)     2259 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/alembic/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 19:38:15.000000 redun-0.8.7/redun/backends/db/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)    11198 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/alembic/versions/806f5dcb11bf_initial_schema.py
--rw-r--r--   0 root         (0) root         (0)     2137 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/alembic/versions/cc4f663817b6_add_tag_models.py
--rw-r--r--   0 root         (0) root         (0)     3017 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/alembic/versions/30ffbaee18cd_add_task_version_and_backfill_companion_values.py
--rw-r--r--   0 root         (0) root         (0)     3258 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/alembic/versions/cd2d53191748_make_job_execution_id_non_nullable.py
--rw-r--r--   0 root         (0) root         (0)     1482 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/alembic/versions/d4af139b6f53_add_job_execution_id.py
--rw-r--r--   0 root         (0) root         (0)     1500 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/alembic/versions/647c510a77b1_add_evaluation_model.py
--rw-r--r--   0 root         (0) root         (0)     2742 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/alembic/versions/71ec303c90e4_add_id_indexes.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12453 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/serializers.py
--rw-r--r--   0 root         (0) root         (0)    81063 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3717 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/base.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1631 2022-03-11 19:11:04.000000 redun-0.8.7/redun/backends/value_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 19:38:15.000000 redun-0.8.7/redun/executors/
--rw-r--r--   0 root         (0) root         (0)     6915 2022-03-11 19:11:04.000000 redun-0.8.7/redun/executors/aws_utils.py
--rw-r--r--   0 root         (0) root         (0)     1788 2022-03-11 19:11:04.000000 redun-0.8.7/redun/executors/glue_oneshot.py.txt
--rw-r--r--   0 root         (0) root         (0)     5567 2022-03-11 19:11:04.000000 redun-0.8.7/redun/executors/local.py
--rw-r--r--   0 root         (0) root         (0)     3587 2022-03-11 19:11:04.000000 redun-0.8.7/redun/executors/base.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-11 19:11:04.000000 redun-0.8.7/redun/executors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25436 2022-03-11 19:11:04.000000 redun-0.8.7/redun/executors/aws_glue.py
--rw-r--r--   0 root         (0) root         (0)    54262 2022-03-11 19:11:04.000000 redun-0.8.7/redun/executors/aws_batch.py
--rw-r--r--   0 root         (0) root         (0)      718 2022-03-11 19:11:04.000000 redun-0.8.7/redun/__init__.py
--rw-r--r--   0 root         (0) root         (0)      359 2022-03-11 19:11:04.000000 redun-0.8.7/redun/namespace.py
--rw-r--r--   0 root         (0) root         (0)     7581 2022-03-11 19:11:04.000000 redun-0.8.7/redun/bcoding.py
--rw-r--r--   0 root         (0) root         (0)     6991 2022-03-11 19:11:04.000000 redun-0.8.7/redun/functools.py
--rw-r--r--   0 root         (0) root         (0)     7258 2022-03-11 19:11:04.000000 redun-0.8.7/redun/job_array.py
--rw-r--r--   0 root         (0) root         (0)    75021 2022-03-11 19:11:04.000000 redun-0.8.7/redun/scheduler.py
--rw-r--r--   0 root         (0) root         (0)      188 2022-03-11 19:11:04.000000 redun-0.8.7/redun/pytest.py
--rw-r--r--   0 root         (0) root         (0)     1780 2022-03-11 19:11:04.000000 redun-0.8.7/redun/db_utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-11 19:11:04.000000 redun-0.8.7/redun/py.typed
--rw-r--r--   0 root         (0) root         (0)     4163 2022-03-11 19:11:04.000000 redun-0.8.7/redun/config.py
--rw-r--r--   0 root         (0) root         (0)     3125 2022-03-11 19:11:04.000000 redun-0.8.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-11 19:38:15.000000 redun-0.8.7/redun.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-11 19:38:15.000000 redun-0.8.7/redun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2974 2022-03-11 19:38:15.000000 redun-0.8.7/redun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      217 2022-03-11 19:38:15.000000 redun-0.8.7/redun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-03-11 19:38:15.000000 redun-0.8.7/redun.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-11 19:17:47.000000 redun-0.8.7/redun.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)     1875 2022-03-11 19:38:15.000000 redun-0.8.7/redun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11358 2022-03-11 19:11:04.000000 redun-0.8.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      217 2022-03-11 19:38:15.000000 redun-0.8.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      101 2022-03-11 19:11:04.000000 redun-0.8.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      150 2022-03-11 19:11:04.000000 redun-0.8.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1875 2022-03-11 19:38:15.000000 redun-0.8.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17728 2022-03-11 19:11:04.000000 redun-0.8.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 15:49:22.000000 redun-0.8.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 15:49:22.000000 redun-0.8.9/bin/
+-rwxr-xr-x   0 root         (0) root         (0)      402 2022-05-18 15:20:09.000000 redun-0.8.9/bin/redun
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 15:49:22.000000 redun-0.8.9/redun/
+-rw-r--r--   0 root         (0) root         (0)     2665 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tags.py
+-rw-r--r--   0 root         (0) root         (0)     4765 2022-05-18 15:20:09.000000 redun-0.8.9/redun/glue.py
+-rw-r--r--   0 root         (0) root         (0)    11044 2022-05-18 15:20:09.000000 redun-0.8.9/redun/expression.py
+-rw-r--r--   0 root         (0) root         (0)    33536 2022-05-18 15:20:09.000000 redun-0.8.9/redun/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 15:49:22.000000 redun-0.8.9/redun/contrib/
+-rw-r--r--   0 root         (0) root         (0)     1783 2022-05-18 15:20:09.000000 redun-0.8.9/redun/contrib/spark_helpers.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-05-18 15:20:09.000000 redun-0.8.9/redun/contrib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3031 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tools.py
+-rw-r--r--   0 root         (0) root         (0)    43689 2022-05-18 15:20:09.000000 redun-0.8.9/redun/file.py
+-rw-r--r--   0 root         (0) root         (0)     7251 2022-05-18 15:20:09.000000 redun-0.8.9/redun/handle.py
+-rw-r--r--   0 root         (0) root         (0)    11414 2022-05-18 15:20:09.000000 redun-0.8.9/redun/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2022-05-18 15:20:09.000000 redun-0.8.9/redun/hashing.py
+-rw-r--r--   0 root         (0) root         (0)     6792 2022-05-18 15:20:09.000000 redun-0.8.9/redun/promise.py
+-rw-r--r--   0 root         (0) root         (0)   107560 2022-05-18 15:20:09.000000 redun-0.8.9/redun/cli.py
+-rw-r--r--   0 root         (0) root         (0)     7296 2022-05-18 15:20:09.000000 redun-0.8.9/redun/scripting.py
+-rw-r--r--   0 root         (0) root         (0)      375 2022-05-18 15:20:09.000000 redun-0.8.9/redun/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 15:49:22.000000 redun-0.8.9/redun/tests/
+-rw-r--r--   0 root         (0) root         (0)     2583 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_namespace.py
+-rw-r--r--   0 root         (0) root         (0)      804 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_typing.py
+-rw-r--r--   0 root         (0) root         (0)     6084 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_value.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_value_store.py
+-rw-r--r--   0 root         (0) root         (0)     4448 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_expression.py
+-rw-r--r--   0 root         (0) root         (0)     8310 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_promise.py
+-rw-r--r--   0 root         (0) root         (0)    10595 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_partial_task.py
+-rw-r--r--   0 root         (0) root         (0)    10589 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11643 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_script.py
+-rw-r--r--   0 root         (0) root         (0)     5358 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     2649 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_bcoding.py
+-rw-r--r--   0 root         (0) root         (0)    20178 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_handle.py
+-rw-r--r--   0 root         (0) root         (0)     7218 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_repos.py
+-rw-r--r--   0 root         (0) root         (0)     4107 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)    14178 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_scheduler_subrun.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_s3.py
+-rw-r--r--   0 root         (0) root         (0)    12701 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_tags.py
+-rw-r--r--   0 root         (0) root         (0)     8585 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_type_registry.py
+-rw-r--r--   0 root         (0) root         (0)     7045 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12101 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_aws_glue.py
+-rw-r--r--   0 root         (0) root         (0)    16449 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 15:49:22.000000 redun-0.8.9/redun/tests/scripts/
+-rw-r--r--   0 root         (0) root         (0)     2008 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/scripts/workflow_subrun_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22826 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_dataflow.py
+-rw-r--r--   0 root         (0) root         (0)      495 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/task_test_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    69025 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_aws_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_uri_parsing.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      500 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_hashing.py
+-rw-r--r--   0 root         (0) root         (0)     4423 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_logging.py
+-rw-r--r--   0 root         (0) root         (0)    20168 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_file.py
+-rw-r--r--   0 root         (0) root         (0)    13693 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_serializers.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_args.py
+-rw-r--r--   0 root         (0) root         (0)    52192 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     7265 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_functools.py
+-rw-r--r--   0 root         (0) root         (0)     3476 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_static_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_db_utils.py
+-rw-r--r--   0 root         (0) root         (0)    39000 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_limits.py
+-rw-r--r--   0 root         (0) root         (0)     2442 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_executors.py
+-rw-r--r--   0 root         (0) root         (0)    30442 2022-05-18 15:20:09.000000 redun-0.8.9/redun/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    19028 2022-05-18 15:20:09.000000 redun-0.8.9/redun/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 15:49:22.000000 redun-0.8.9/redun/backends/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 15:49:22.000000 redun-0.8.9/redun/backends/db/
+-rw-r--r--   0 root         (0) root         (0)    44907 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/dataflow.py
+-rw-r--r--   0 root         (0) root         (0)    17960 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/query.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 15:49:22.000000 redun-0.8.9/redun/backends/db/alembic/
+-rw-r--r--   0 root         (0) root         (0)     2259 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/alembic/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 15:49:22.000000 redun-0.8.9/redun/backends/db/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)    11198 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/alembic/versions/806f5dcb11bf_initial_schema.py
+-rw-r--r--   0 root         (0) root         (0)     2137 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/alembic/versions/cc4f663817b6_add_tag_models.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/alembic/versions/30ffbaee18cd_add_task_version_and_backfill_companion_values.py
+-rw-r--r--   0 root         (0) root         (0)     3258 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/alembic/versions/cd2d53191748_make_job_execution_id_non_nullable.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/alembic/versions/d4af139b6f53_add_job_execution_id.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/alembic/versions/647c510a77b1_add_evaluation_model.py
+-rw-r--r--   0 root         (0) root         (0)     2742 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/alembic/versions/71ec303c90e4_add_id_indexes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12453 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/serializers.py
+-rw-r--r--   0 root         (0) root         (0)    81063 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3717 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/base.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1631 2022-05-18 15:20:09.000000 redun-0.8.9/redun/backends/value_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 15:49:22.000000 redun-0.8.9/redun/executors/
+-rw-r--r--   0 root         (0) root         (0)     8490 2022-05-18 15:20:09.000000 redun-0.8.9/redun/executors/aws_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2022-05-18 15:20:09.000000 redun-0.8.9/redun/executors/glue_oneshot.py.txt
+-rw-r--r--   0 root         (0) root         (0)     5773 2022-05-18 15:20:09.000000 redun-0.8.9/redun/executors/local.py
+-rw-r--r--   0 root         (0) root         (0)     3587 2022-05-18 15:20:09.000000 redun-0.8.9/redun/executors/base.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-05-18 15:20:09.000000 redun-0.8.9/redun/executors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25506 2022-05-18 15:20:09.000000 redun-0.8.9/redun/executors/aws_glue.py
+-rw-r--r--   0 root         (0) root         (0)    58909 2022-05-18 15:20:09.000000 redun-0.8.9/redun/executors/aws_batch.py
+-rw-r--r--   0 root         (0) root         (0)      592 2022-05-18 15:20:09.000000 redun-0.8.9/redun/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      359 2022-05-18 15:20:09.000000 redun-0.8.9/redun/namespace.py
+-rw-r--r--   0 root         (0) root         (0)     7581 2022-05-18 15:20:09.000000 redun-0.8.9/redun/bcoding.py
+-rw-r--r--   0 root         (0) root         (0)     6991 2022-05-18 15:20:09.000000 redun-0.8.9/redun/functools.py
+-rw-r--r--   0 root         (0) root         (0)     7258 2022-05-18 15:20:09.000000 redun-0.8.9/redun/job_array.py
+-rw-r--r--   0 root         (0) root         (0)    79372 2022-05-18 15:20:09.000000 redun-0.8.9/redun/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)      188 2022-05-18 15:20:09.000000 redun-0.8.9/redun/pytest.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2022-05-18 15:20:09.000000 redun-0.8.9/redun/db_utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-05-18 15:20:09.000000 redun-0.8.9/redun/py.typed
+-rw-r--r--   0 root         (0) root         (0)     4163 2022-05-18 15:20:09.000000 redun-0.8.9/redun/config.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2022-05-18 15:20:10.000000 redun-0.8.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-18 15:49:22.000000 redun-0.8.9/redun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-18 15:49:22.000000 redun-0.8.9/redun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2974 2022-05-18 15:49:22.000000 redun-0.8.9/redun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      225 2022-05-18 15:49:22.000000 redun-0.8.9/redun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2022-05-18 15:49:22.000000 redun-0.8.9/redun.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-18 15:26:36.000000 redun-0.8.9/redun.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1875 2022-05-18 15:49:22.000000 redun-0.8.9/redun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11358 2022-05-18 15:20:09.000000 redun-0.8.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      257 2022-05-18 15:49:22.000000 redun-0.8.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      101 2022-05-18 15:20:09.000000 redun-0.8.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      150 2022-05-18 15:20:09.000000 redun-0.8.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1875 2022-05-18 15:49:22.000000 redun-0.8.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17738 2022-05-18 15:20:09.000000 redun-0.8.9/README.md
```

### Comparing `redun-0.8.7/redun/tags.py` & `redun-0.8.9/redun/tags.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/glue.py` & `redun-0.8.9/redun/glue.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/expression.py` & `redun-0.8.9/redun/expression.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/task.py` & `redun-0.8.9/redun/task.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/contrib/spark_helpers.py` & `redun-0.8.9/redun/contrib/spark_helpers.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tools.py` & `redun-0.8.9/redun/tools.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/file.py` & `redun-0.8.9/redun/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import abc
 import glob
+import io
 import os
 import shutil
+import threading
 from shlex import quote
 from typing import (
     IO,
     TYPE_CHECKING,
     Any,
     Dict,
     Generic,
@@ -29,14 +31,18 @@
 from redun.value import Value
 
 # Don't require pyspark to be installed locally except for type checking.
 if TYPE_CHECKING:
     import pandas
     import pyspark
 
+# Thread-local storage is used for thread-specific s3 clients.
+_local = threading.local()
+
+# Global singletons for Filesystems.
 _proto2filesystem_class: Dict[str, Type["FileSystem"]] = {}
 
 
 def register_filesystem(cls: Type["FileSystem"]) -> Type["FileSystem"]:
     _proto2filesystem_class[cls.name] = cls
     return cls
 
@@ -59,16 +65,30 @@
     """
     if not proto:
         assert url, "Must give url or proto as argument."
         proto = get_proto(url)
     return _proto2filesystem_class[proto]
 
 
-def open_file(url: str, mode: str = "r") -> IO:
-    return get_filesystem(url=url).open(url, mode=mode)
+def open_file(url: str, mode: str = "r", encoding: Optional[str] = None, **kwargs: Any) -> IO:
+    """
+    Open a file stream.
+
+    Parameters
+    ----------
+    url : str
+        Url or path of file to open.
+    mode : str
+        Stream mode for reading or writing ('r', 'w', 'b', 'a').
+    encoding : str
+        Text encoding (e.g. 'utf-8') to use when read or writing.
+    **kwargs
+        Additional arguments for the underlying file stream. They are Filesystem-specific.
+    """
+    return get_filesystem(url=url).open(url, mode=mode, encoding=encoding, **kwargs)
 
 
 def glob_file(pattern: str) -> List[str]:
     return get_filesystem(url=pattern).glob(pattern)
 
 
 _filesystem_instances: Dict[Type, "FileSystem"] = {}
@@ -88,17 +108,45 @@
 class FileSystem(abc.ABC):
     """
     Base class filesystem access.
     """
 
     name: str = "base"
 
-    def open(self, path: str, mode: str) -> IO:
+    def open(self, path: str, mode: str, encoding: Optional[str] = None, **kwargs: Any) -> IO:
         """
-        Open a file stream for path with mode ('r', 'w', 'b').
+        Open a file stream from the filesystem.
+
+        Parameters
+        ----------
+        path : str
+            Url or path of file to open.
+        mode : str
+            Stream mode for reading or writing ('r', 'w', 'b', 'a').
+        encoding : str
+            Text encoding (e.g. 'utf-8') to use when read or writing.
+        **kwargs
+            Additional arguments for the underlying file stream. They are Filesystem-specific.
+        """
+        if encoding:
+            if "b" in mode:
+                raise ValueError("Binary mode 'b' cannot be used with encoding.")
+            mode += "b"
+
+        stream = self._open(path, mode, **kwargs)
+
+        if encoding:
+            # Perform encoding/decoding, if specified.
+            stream = io.TextIOWrapper(stream, encoding)
+
+        return stream
+
+    def _open(self, path: str, mode: str, **kwargs: Any) -> IO:
+        """
+        Private open method for subclasses to implement.
         """
         pass
 
     def exists(self, path: str) -> bool:
         """
         Returns True if path exists on filesystem.
         """
@@ -184,23 +232,23 @@
         Automatically create the directory for path.
         """
         dirname = os.path.dirname(path)
         if dirname and not os.path.exists(dirname):
             os.makedirs(dirname)
         return dirname
 
-    def open(self, path: str, mode: str) -> IO:
+    def _open(self, path: str, mode: str, **kwargs: Any) -> IO:
         """
         Open a file stream for path with mode ('r', 'w', 'b').
         """
         # Auto create the directory if needed.
         if "w" in mode or "a" in mode:
             self._ensure_dir(path)
 
-        return open(path, mode)
+        return open(path, mode, **kwargs)
 
     def exists(self, path: str) -> bool:
         """
         Returns True if path exists on filesystem.
         """
         return os.path.exists(path)
 
@@ -303,23 +351,23 @@
         """
         Automatically create the directory for path.
         """
         dirname = os.path.dirname(path)
         self.fs.makedirs(dirname, exist_ok=True)
         return dirname
 
-    def open(self, path: str, mode: str) -> IO:
+    def _open(self, path: str, mode: str, **kwargs: Any) -> IO:
         """
         Open a file stream for path with mode ('r', 'w', 'b').
         """
         # Auto create the directory if needed.
         if "w" in mode or "a" in mode:
             self._ensure_dir(path)
 
-        return self.fs.open(path, mode)
+        return self.fs.open(path, mode, **kwargs)
 
     def exists(self, path: str) -> bool:
         """
         Returns True if path exists on filesystem.
         """
         return self.fs.exists(path)
 
@@ -425,17 +473,41 @@
 class S3FileSystem(FileSystem):
     """
     FileSystem methods for a AWS S3.
     """
 
     name = "s3"
 
-    def __init__(self):
-        self.s3 = s3fs.S3FileSystem(anon=False)
-        self.s3_raw = boto3.client("s3")
+    @property
+    def s3(self) -> s3fs.S3FileSystem:
+        # Maintain a client per thread, since s3fs is not thread-safe.
+        # Double check pid since fork can clone thread-local storage.
+        pid = getattr(_local, "pid", None)
+        if pid != os.getpid():
+            _local.pid = os.getpid()
+            client = None
+        else:
+            client = getattr(_local, "s3", None)
+        if not client:
+            client = _local.s3 = s3fs.S3FileSystem(anon=False)
+        return client
+
+    @property
+    def s3_raw(self) -> Any:
+        # Maintain a client per thread, since boto is not thread-safe.
+        # Double check pid since fork can clone thread-local storage.
+        pid = getattr(_local, "pid", None)
+        if pid != os.getpid():
+            _local.pid = os.getpid()
+            client = None
+        else:
+            client = getattr(_local, "s3_raw", None)
+        if not client:
+            client = _local.s3_raw = boto3.client("s3")
+        return client
 
     def exists(self, path: str) -> bool:
         """
         Returns True if path exists in filesystem.
         """
         try:
             # We call head_object ourselves so that we can avoid getting stale
@@ -456,16 +528,16 @@
     def remove(self, path: str) -> None:
         try:
             self.s3.rm(path)
         except FileNotFoundError:
             # It it not an error to try to remove a non-existent File.
             pass
 
-    def open(self, path: str, mode: str) -> IO:
-        return self.s3.open(path, mode)
+    def _open(self, path: str, mode: str, **kwargs: Any) -> IO:
+        return self.s3.open(path, mode, **kwargs)
 
     def mkdir(self, path: str) -> None:
         # s3fs mkdir only creates buckets, so we just touch this key
         if not self.exists(path):
             self.s3.touch(path)
 
     def rmdir(self, path: str, recursive: bool = False) -> None:
@@ -556,44 +628,60 @@
 
     def exists(self) -> bool:
         return self.filesystem.exists(self.path)
 
     def remove(self) -> None:
         return self.filesystem.remove(self.path)
 
-    def open(self, mode: str = "r") -> IO:
+    def open(self, mode: str = "r", encoding: Optional[str] = None, **kwargs: Any) -> IO:
+        """
+        Open a file stream.
+
+        Parameters
+        ----------
+        mode : str
+            Stream mode for reading or writing ('r', 'w', 'b', 'a').
+        encoding : str
+            Text encoding (e.g. 'utf-8') to use when read or writing.
+        **kwargs
+            Additional arguments for the underlying file stream. They are Filesystem-specific.
+        """
+
         def close():
             original_close()
             self.update_hash()
 
             # Restore original close. This way double closing doesn't trigger
             # unnecessary hashing.
             self.stream.close = original_close
 
-        self.stream = self.filesystem.open(self.path, mode)
+        self.stream = self.filesystem.open(self.path, mode, encoding=encoding, **kwargs)
+
         original_close = self.stream.close
         self.stream.close = close  # type: ignore
 
         return self.stream
 
     def touch(self, time: Union[Tuple[int, int], Tuple[float, float], None] = None) -> None:
         self.filesystem.touch(self.path, time)
 
-    def read(self, mode: str = "r") -> Union[str, bytes]:
-        with self.open(mode=mode) as infile:
+    def read(self, mode: str = "r", encoding: Optional[str] = None) -> Union[str, bytes]:
+        with self.open(mode=mode, encoding=encoding) as infile:
             data = infile.read()
         return data
 
     def readlines(self, mode: str = "r") -> List[Union[str, bytes]]:
         with self.open(mode=mode) as infile:
             data = infile.readlines()
         return data
 
-    def write(self, data: Union[str, bytes], mode: str = "w") -> None:
-        with self.open(mode) as out:
+    def write(
+        self, data: Union[str, bytes], mode: str = "w", encoding: Optional[str] = None
+    ) -> None:
+        with self.open(mode=mode, encoding=encoding) as out:
             out.write(data)
 
     def copy_to(self, dest_file: "File", skip_if_exists: bool = False) -> "File":
         if skip_if_exists and dest_file.exists():
             return dest_file
 
         self.filesystem.copy(self.path, dest_file.path)
```

### Comparing `redun-0.8.7/redun/handle.py` & `redun-0.8.9/redun/handle.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/utils.py` & `redun-0.8.9/redun/utils.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/hashing.py` & `redun-0.8.9/redun/hashing.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/promise.py` & `redun-0.8.9/redun/promise.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Generic, List, Optional, Sequence, TypeVar, cast
+from typing import Any, Callable, Generic, List, Optional, Sequence, TypeVar, cast
 
 S = TypeVar("S")
 T = TypeVar("T")
 
 
 class Promise(Generic[T]):
     """
@@ -182,7 +182,30 @@
             subpromise.then(make_then(i), fail)
 
         if len(results) == 0:
             # Special case for when we are given no subpromises.
             promise.do_resolve(cast(List[T], results))
 
         return promise
+
+
+def wait_promises(subpromises: List[Promise[T]]) -> Promise[List[Promise[T]]]:
+    """
+    Wait for all promises to finish (either fulfill or reject).
+    """
+    promise: Promise[List[Promise[T]]] = Promise()
+    num_done = 0
+
+    def done(result_or_error: Any) -> None:
+        nonlocal num_done
+        num_done += 1
+        if num_done == len(subpromises):
+            promise.do_resolve(subpromises)
+
+    for subpromise in subpromises:
+        subpromise.then(done, done)
+
+    if len(subpromises) == 0:
+        # Special case for when we are given no subpromises.
+        promise.do_resolve([])
+
+    return promise
```

### Comparing `redun-0.8.7/redun/cli.py` & `redun-0.8.9/redun/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,17 +67,16 @@
 from redun.backends.db.serializers import RecordSerializer
 from redun.config import Config, create_config_section
 from redun.executors.aws_batch import (
     BATCH_LOG_GROUP,
     AWSBatchExecutor,
     aws_describe_jobs,
     format_log_stream_event,
-    iter_log_stream,
 )
-from redun.executors.aws_utils import extract_tar
+from redun.executors.aws_utils import extract_tar, iter_log_stream
 from redun.file import File as BaseFile
 from redun.job_array import AWS_ARRAY_VAR
 from redun.logging import log_levels, logger
 from redun.scheduler import DryRunResult, ErrorValue, Scheduler, Traceback, get_task_registry
 from redun.tags import (
     ANY_VALUE,
     DOC_KEY,
@@ -910,17 +909,16 @@
 def format_tags(tags: List[Tag], max_length: int = 50) -> str:
     """
     Format a set of tags.
     """
     if not tags:
         return ""
 
-    tags = sorted(tags, key=lambda tag: (tag.key, tag.value))
     tag_list = ", ".join(
-        format_tag_key_value(tag.key, tag.value, max_length=max_length) for tag in tags
+        sorted(format_tag_key_value(tag.key, tag.value, max_length=max_length) for tag in tags)
     )
     return f"({tag_list})"
 
 
 def get_default_execution_tags() -> List[Tuple[str, Any]]:
     """
     Get default tags for the Execution.
```

### Comparing `redun-0.8.7/redun/scripting.py` & `redun-0.8.9/redun/scripting.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,26 +169,24 @@
     This task correctly implements reactivity to changing inputs and outputs.
     `script_task()` alone is unable to implement such reactivity because its
     only argument is a shell script string and its output is the stdout.
     Thus, the ultimate input and output files of the script are accessed
     outside the usual redun detection mechanisms (task arguments
     and return values).
 
-    To achieve the correct reactivity, `script_task()` is called with
-    `cached=False`, in order to force it to always execute when called.
+    To achieve the correct reactivity, `script_task()` is special-cased in the Scheduler
+    to not use caching, in order to force it to always execute when called.
     Additionally, `_script()` is configured with `check_valid="shallow"` to
     skip execution of its child tasks, `script_task()` and `postprocess_script()`,
     if its previous outputs are still valid (i.e. not altered or deleted).
     """
     # Note: inputs are an argument just for reactivity sake.
     # They have already been incorporated into the command.
-    # Use cache=False to force rerunning script_task since it can't react
-    # to invalidation of its output.
     return postprocess_script(
-        script_task.options(cache=False, **task_options)(command), outputs, temp_path=temp_path
+        script_task.options(**task_options)(command), outputs, temp_path=temp_path
     )
 
 
 @task(name="postprocess_script", namespace="redun", version="1")
 def postprocess_script(result: Any, outputs: Any, temp_path: Optional[str] = None) -> Any:
     """
     Postprocess the results of a script task.
```

### Comparing `redun-0.8.7/redun/tests/test_namespace.py` & `redun-0.8.9/redun/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_typing.py` & `redun-0.8.9/redun/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/conftest.py` & `redun-0.8.9/redun/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_value.py` & `redun-0.8.9/redun/tests/test_value.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_value_store.py` & `redun-0.8.9/redun/tests/test_value_store.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_config.py` & `redun-0.8.9/redun/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_expression.py` & `redun-0.8.9/redun/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_promise.py` & `redun-0.8.9/redun/tests/test_promise.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest.mock import Mock
 
 import pytest
 
-from redun.promise import Promise
+from redun.promise import Promise, wait_promises
 
 
 def test_resolve() -> None:
     """
     Promise constructor should resolve values.
     """
     promise: Promise[int] = Promise(lambda resolve, reject: resolve(10))
@@ -323,7 +323,37 @@
 
     promises = Promise.all([promise1, promise2])
 
     mock = Mock()
     promises.then(None, mock)
 
     mock.assert_called_with(error)
+
+
+def test_wait_promises() -> None:
+    """
+    wait_promises() should wait for all subpromises regardless of success or failure.
+    """
+
+    def good():
+        return Promise(lambda resolve, reject: resolve(10))
+
+    def bad():
+        return Promise(lambda resolve, reject: reject(ValueError("boom")))
+
+    top = wait_promises([good(), good(), good()])
+    promises = top.value
+    assert [promise.value for promise in promises] == [10, 10, 10]
+
+    top = wait_promises([good(), bad(), good()])
+    promises = top.value
+    assert promises[0].value == 10
+    assert isinstance(promises[1].error, ValueError)
+    assert promises[2].value == 10
+
+    a: Promise[int] = Promise()
+    top = wait_promises([good(), bad(), a])
+    a.do_resolve(20)
+    promises = top.value
+    assert promises[0].value == 10
+    assert isinstance(promises[1].error, ValueError)
+    assert promises[2].value == 20
```

### Comparing `redun-0.8.7/redun/tests/test_partial_task.py` & `redun-0.8.9/redun/tests/test_partial_task.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/utils.py` & `redun-0.8.9/redun/tests/utils.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_script.py` & `redun-0.8.9/redun/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_errors.py` & `redun-0.8.9/redun/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_bcoding.py` & `redun-0.8.9/redun/tests/test_bcoding.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_handle.py` & `redun-0.8.9/redun/tests/test_handle.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_repos.py` & `redun-0.8.9/redun/tests/test_repos.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_process_executor.py` & `redun-0.8.9/redun/tests/test_process_executor.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_scheduler_subrun.py` & `redun-0.8.9/redun/tests/test_scheduler_subrun.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
 def test_subrun_cached():
     """Subrun "wrapper" task is cached"""
     task_calls = []
 
     @task(cache=False)
     def foo(x):
         task_calls.append("foo")
-        return x ** 2
+        return x**2
 
     @task()
     def local_main(x):
         task_calls.append("local_main")
         return subrun(foo(x), executor="default")
 
     scheduler = Scheduler()
@@ -313,15 +313,15 @@
 def test_subrun_root_task_cached():
     """_subrun_root_task is cached by default.  This test disables caching for all other tasks."""
     task_calls = []
 
     @task(cache=False)
     def foo(x):
         task_calls.append("foo")
-        return x ** 2
+        return x**2
 
     @task(cache=False)
     def local_main(x):
         task_calls.append("local_main")
         return subrun(foo(x), executor="default")
 
     scheduler = Scheduler()
@@ -341,15 +341,15 @@
 def test_subrun_root_task_disabled_cached():
     """Invoker of subrun disables caching so _subrun_root_task is no longer cached."""
     task_calls = []
 
     @task(cache=False)
     def foo(x):
         task_calls.append("foo")
-        return x ** 2
+        return x**2
 
     @task(cache=False)
     def local_main(x):
         task_calls.append("local_main")
         return subrun(foo(x), executor="default", cache=False)  # disable caching
 
     scheduler = Scheduler()
```

### Comparing `redun-0.8.7/redun/tests/test_s3.py` & `redun-0.8.9/redun/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_tags.py` & `redun-0.8.9/redun/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_type_registry.py` & `redun-0.8.9/redun/tests/test_type_registry.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_utils.py` & `redun-0.8.9/redun/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_aws_glue.py` & `redun-0.8.9/redun/tests/test_aws_glue.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 import re
 import zipfile
 from typing import Any, Dict
 from unittest.mock import Mock, patch
 
 import boto3
 import moto
-import pytest
 from moto.glue.responses import GlueResponse
 
-import redun.executors.aws_glue as redun_glue
 from redun import File, task
 from redun.config import Config
 from redun.executors.aws_glue import AWSGlueExecutor, get_redun_lib_files, package_redun_lib
 from redun.executors.aws_utils import create_zip, get_aws_client
 from redun.scheduler import Job
 from redun.tests.utils import mock_s3, mock_scheduler, use_tempdir, wait_until
 from redun.utils import pickle_dumps
@@ -210,30 +208,14 @@
     assert executor.aws_region == "pangea"
     assert executor.role == "overlord"
     assert executor.interval == 1.0
     assert executor.code_package["includes"] == ["*.txt"]
     assert executor.debug is False
 
 
-# This has a permissions error when running as pytest
-@pytest.mark.skip(reason="permissions")
-def test_error_logs() -> None:
-    """
-    Tests errors can be found in logs. Runs on an actual Glue output.
-    """
-    job_id = "jr_4eee8443c9e37797a96dc1c790843ecc6552ff34f648b6faff2f76ac07b9e4cc"
-    log_group = "/aws-glue/jobs/error"
-
-    output = list(redun_glue.get_error_logs(job_id, log_group))
-    assert output == [
-        '2021-06-30 14:18:34.523000  Exception in thread "main"',
-        "2021-06-30 14:18:34.523000  java.io.FileNotFoundException: File --task does not exist",
-    ]
-
-
 @use_tempdir
 def test_redun_lib_files() -> None:
     """
     We should be able to create a zip archive of the redun library.
     """
     lib_files = list(get_redun_lib_files())
     assert len(lib_files) > 0
```

### Comparing `redun-0.8.7/redun/tests/test_tasks.py` & `redun-0.8.9/redun/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/scripts/workflow_subrun_process_executor.py` & `redun-0.8.9/redun/tests/scripts/workflow_subrun_process_executor.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_dataflow.py` & `redun-0.8.9/redun/tests/test_dataflow.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_aws_batch.py` & `redun-0.8.9/redun/tests/test_aws_batch.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     SUCCEEDED,
     AWSBatchError,
     AWSBatchExecutor,
     batch_submit,
     get_batch_job_name,
     get_hash_from_job_name,
     get_job_definition,
+    get_or_create_job_definition,
     iter_batch_job_log_lines,
     iter_batch_job_logs,
     make_job_def_name,
     parse_task_error,
     submit_task,
 )
 from redun.executors.aws_utils import (
@@ -87,22 +88,22 @@
 @patch("redun.executors.aws_batch.get_job_definition")
 def test_required_job_def_name(get_job_definition_mock, _) -> None:
     """
     Confirm that job_def_name is required when autocreate_job is False.
     """
     # A job_def_name is required when autocreate is False.
     with pytest.raises(AssertionError):
-        batch_submit(["command"], "queue", "image", autocreate_job=False)
+        batch_submit({"command": ["ls"]}, "queue", "image", autocreate_job=False)
 
     # When the required job_def_name is supplied, an error should be raised if a matching
     # definition cannot be found.
     get_job_definition_mock.return_value = {}
     with pytest.raises(ValueError):
         batch_submit(
-            ["command"], "queue", "image", job_def_name="NONEXISTENT", autocreate_job=False
+            {"command": ["ls"]}, "queue", "image", job_def_name="NONEXISTENT", autocreate_job=False
         )
 
 
 @pytest.mark.parametrize("array,suffix", [(False, ""), (True, "-array")])
 def test_get_hash_from_job_name(array, suffix) -> None:
     """
     Returns the Job hash from a AWS Batch job name.
@@ -113,14 +114,317 @@
     assert job_name.startswith(prefix)
     assert job_name.endswith(suffix)
 
     job_hash2 = get_hash_from_job_name(job_name)
     assert job_hash2 == job_hash
 
 
+@patch("redun.executors.aws_utils.get_aws_client")
+@patch("redun.executors.aws_batch.get_job_definition")
+def test_get_or_create_job_definition(get_job_definition_mock, get_aws_client_mock) -> None:
+    """
+    Confirm that jobs are correctly fetched or created.
+    """
+
+    get_aws_client_mock.return_value.register_job_definition.return_value = {"jobId": "new-job"}
+
+    # 1. Jobs get created
+    get_job_definition_mock.return_value = {}
+    result = get_or_create_job_definition(
+        job_def_name="test-jd", image="an-image:latest", role="aRole"
+    )
+
+    assert result == {"jobId": "new-job"}
+    get_aws_client_mock.return_value.register_job_definition.assert_called_with(
+        jobDefinitionName="test-jd",
+        type="container",
+        containerProperties={
+            "command": ["ls"],
+            "image": "an-image:latest",
+            "vcpus": 1,
+            "memory": 4,
+            "jobRoleArn": "aRole",
+            "environment": [],
+            "mountPoints": [],
+            "volumes": [],
+            "resourceRequirements": [],
+            "ulimits": [],
+            "privileged": False,
+        },
+    )
+
+    # 2a. Identical jobs are not recreated
+    get_aws_client_mock.return_value.register_job_definition.reset_mock()
+    get_job_definition_mock.return_value = {
+        "jobDefinitionName": "test-jd2",
+        "type": "container",
+        "containerProperties": {
+            "command": ["ls"],
+            "image": "an-image:latest",
+            "vcpus": 1,
+            "memory": 4,
+            "jobRoleArn": "aRole",
+            "environment": [],
+            "mountPoints": [],
+            "volumes": [],
+            "resourceRequirements": [],
+            "ulimits": [],
+            "privileged": False,
+        },
+    }
+    get_or_create_job_definition(job_def_name="test-jd2", image="an-image:latest", role="aRole")
+    get_aws_client_mock.return_value.register_job_definition.assert_not_called()
+
+    # 2.b. resource differences are ignored on single node
+    get_aws_client_mock.return_value.register_job_definition.reset_mock()
+    get_or_create_job_definition(
+        job_def_name="test-jd2b",
+        image="an-image:latest",
+        role="aRole",
+        vcpus=2,
+        memory=8,
+    )
+    get_aws_client_mock.return_value.register_job_definition.assert_not_called()
+
+    # 3. Extra keys are ignored
+    get_aws_client_mock.return_value.register_job_definition.reset_mock()
+    get_job_definition_mock.return_value = {
+        "extraneous_key": "ignored",
+        "jobDefinitionName": "test-jd3",
+        "type": "container",
+        "containerProperties": {
+            "command": ["ls"],
+            "image": "an-image:latest",
+            "vcpus": 1,
+            "memory": 4,
+            "jobRoleArn": "aRole",
+            "environment": [],
+            "mountPoints": [],
+            "volumes": [],
+            "resourceRequirements": [],
+            "ulimits": [],
+            "privileged": False,
+        },
+    }
+    get_or_create_job_definition(job_def_name="test-jd3", image="an-image:latest", role="aRole")
+    get_aws_client_mock.return_value.register_job_definition.assert_not_called()
+
+    # 4. Important differences trigger recreation
+    # 4.a. job type
+    get_aws_client_mock.return_value.register_job_definition.reset_mock()
+    get_job_definition_mock.return_value = {
+        "jobDefinitionName": "test-jd4a",
+        "type": "other",
+        "containerProperties": {
+            "command": ["ls"],
+            "image": "an-image:latest",
+            "vcpus": 2,
+            "memory": 4,
+            "jobRoleArn": "aRole",
+            "environment": [],
+            "mountPoints": [],
+            "volumes": [],
+            "resourceRequirements": [],
+            "ulimits": [],
+            "privileged": False,
+        },
+    }
+    get_or_create_job_definition(job_def_name="test-jd4a", image="an-image:latest", role="aRole")
+    assert result == {"jobId": "new-job"}
+    get_aws_client_mock.return_value.register_job_definition.assert_called_with(
+        jobDefinitionName="test-jd4a",
+        type="container",
+        containerProperties={
+            "command": ["ls"],
+            "image": "an-image:latest",
+            "vcpus": 1,
+            "memory": 4,
+            "jobRoleArn": "aRole",
+            "environment": [],
+            "mountPoints": [],
+            "volumes": [],
+            "resourceRequirements": [],
+            "ulimits": [],
+            "privileged": False,
+        },
+    )
+
+    # 4.b. num_nodes
+    get_aws_client_mock.return_value.register_job_definition.reset_mock()
+    get_job_definition_mock.return_value = {
+        "jobDefinitionName": "test-jd4b",
+        "type": "container",
+        "containerProperties": {
+            "command": ["ls"],
+            "image": "an-image:latest",
+            "vcpus": 2,
+            "memory": 4,
+            "jobRoleArn": "aRole",
+            "environment": [],
+            "mountPoints": [],
+            "volumes": [],
+            "resourceRequirements": [],
+            "ulimits": [],
+            "privileged": False,
+        },
+    }
+    get_or_create_job_definition(
+        job_def_name="test-jd4b", image="an-image:latest", role="aRole", num_nodes=3
+    )
+    multinode_job = {
+        "jobDefinitionName": "test-jd4b",
+        "type": "multinode",
+        "nodeProperties": {
+            "mainNode": 0,
+            "numNodes": 3,
+            "nodeRangeProperties": [
+                {
+                    "container": {
+                        "command": ["ls"],
+                        "image": "an-image:latest",
+                        "vcpus": 1,
+                        "memory": 4,
+                        "jobRoleArn": "aRole",
+                        "environment": [],
+                        "mountPoints": [],
+                        "volumes": [],
+                        "resourceRequirements": [],
+                        "ulimits": [],
+                        "privileged": False,
+                    },
+                    "targetNodes": "0",
+                },
+                {
+                    "container": {
+                        "command": ["ls"],
+                        "image": "an-image:latest",
+                        "vcpus": 1,
+                        "memory": 4,
+                        "jobRoleArn": "aRole",
+                        "environment": [],
+                        "mountPoints": [],
+                        "volumes": [],
+                        "resourceRequirements": [],
+                        "ulimits": [],
+                        "privileged": False,
+                    },
+                    "targetNodes": "1:",
+                },
+            ],
+        },
+    }
+    get_aws_client_mock.return_value.register_job_definition.assert_called_with(**multinode_job)
+
+    # 4c. Multinode resource definitions do not trigger changes
+    get_aws_client_mock.return_value.register_job_definition.reset_mock()
+    get_job_definition_mock.return_value = multinode_job
+    get_or_create_job_definition(
+        job_def_name="test-jd4b",
+        image="an-image:latest",
+        role="aRole",
+        num_nodes=3,
+        vcpus=2,
+        memory=8,
+    )
+    get_aws_client_mock.return_value.register_job_definition.assert_not_called()
+
+
+@patch("redun.executors.aws_utils.get_aws_client")
+@patch("redun.executors.aws_batch.get_or_create_job_definition")
+def test_job_submit_resources(get_or_create_job_definition_mock, get_aws_client_mock) -> None:
+    """
+    Confirm that resource overrides are properly applied.
+    """
+
+    get_or_create_job_definition_mock.return_value = {"jobDefinitionArn": "test-jd-arn"}
+
+    # 1. Single node
+    batch_submit(
+        batch_job_args={"containerOverrides": {"command": ["test_command"]}, "user": "user-test"},
+        job_name="test",
+        queue="test_queue",
+        image="test_image",
+        vcpus=4,
+        memory=8,
+        gpus=2,
+    )
+
+    # Check that the resources are applied but the custom commands are specifically not touched.
+    get_aws_client_mock.return_value.submit_job.assert_called_with(
+        jobName="test",
+        jobQueue="test_queue",
+        jobDefinition="test-jd-arn",
+        retryStrategy={"attempts": 1},
+        containerOverrides={
+            "command": ["test_command"],
+            "vcpus": 4,
+            "memory": 8192,
+            "resourceRequirements": [{"type": "GPU", "value": "2"}],
+        },
+        propagateTags=True,
+        user="user-test",
+    )
+
+    # 2. multi-node
+    get_aws_client_mock.return_value.submit_job.reset_mock()
+    batch_submit(
+        batch_job_args={
+            "nodeOverrides": {
+                "nodePropertyOverrides": [
+                    {
+                        "targetNodes": "0",
+                        "containerOverrides": {"command": ["command_rank_0"]},
+                    },
+                    {
+                        "targetNodes": "1:",
+                        "containerOverrides": {"command": ["command_rank_1"]},
+                    },
+                ],
+            }
+        },
+        job_name="test",
+        queue="test_queue",
+        image="test_image",
+        vcpus=4,
+        memory=8,
+        gpus=2,
+    )
+
+    # Check that the resources are applied but the custom commands are specifically not touched.
+    get_aws_client_mock.return_value.submit_job.assert_called_with(
+        jobName="test",
+        jobQueue="test_queue",
+        jobDefinition="test-jd-arn",
+        retryStrategy={"attempts": 1},
+        nodeOverrides={
+            "nodePropertyOverrides": [
+                {
+                    "targetNodes": "0",
+                    "containerOverrides": {
+                        "command": ["command_rank_0"],
+                        "vcpus": 4,
+                        "memory": 8192,
+                        "resourceRequirements": [{"type": "GPU", "value": "2"}],
+                    },
+                },
+                {
+                    "targetNodes": "1:",
+                    "containerOverrides": {
+                        "command": ["command_rank_1"],
+                        "vcpus": 4,
+                        "memory": 8192,
+                        "resourceRequirements": [{"type": "GPU", "value": "2"}],
+                    },
+                },
+            ]
+        },
+        propagateTags=True,
+    )
+
+
 def test_batch_tags(scheduler: Scheduler) -> None:
     """
     Executor should be able to determine batch tags for a batch job.
     """
     # Setup executor.
     config = Config(
         {
@@ -274,42 +578,150 @@
 
     # Input files should be made.
     assert File("s3://example-bucket/redun/jobs/eval_hash/input").exists()
     [code_file] = list(Dir("s3://example-bucket/redun/code"))
 
     # We should have submitted a job to AWS Batch.
     redun.executors.aws_batch.batch_submit.assert_called_with(
-        [
-            "redun",
-            "--check-version",
-            REDUN_REQUIRED_VERSION,
-            "oneshot",
-            expected_load_module,
-            "--code",
-            code_file.path,
-            "--input",
-            "s3://example-bucket/redun/jobs/eval_hash/input",
-            "--output",
-            "s3://example-bucket/redun/jobs/eval_hash/output",
-            "--error",
-            "s3://example-bucket/redun/jobs/eval_hash/error",
-            a_task.name,
-        ],
+        {
+            "containerOverrides": {
+                "command": [
+                    "redun",
+                    "--check-version",
+                    REDUN_REQUIRED_VERSION,
+                    "oneshot",
+                    expected_load_module,
+                    "--code",
+                    code_file.path,
+                    "--input",
+                    "s3://example-bucket/redun/jobs/eval_hash/input",
+                    "--error",
+                    "s3://example-bucket/redun/jobs/eval_hash/error",
+                    a_task.name,
+                    "--output",
+                    "s3://example-bucket/redun/jobs/eval_hash/output",
+                ]
+            }
+        },
         "queue",
         image="my-image",
         job_def_suffix="-redun-jd",
         job_name="batch-job-eval_hash",
         array_size=0,
         aws_region="us-west-2",
     )
 
 
 @use_tempdir
 @mock_s3
 @patch("redun.executors.aws_batch.batch_submit")
+def test_submit_multinode_task(batch_submit_mock):
+    job_id = "123"
+    image = "my-image"
+    queue = "queue"
+    s3_scratch_prefix = "s3://example-bucket/redun/"
+
+    client = boto3.client("s3", region_name="us-east-1")
+    client.create_bucket(Bucket="example-bucket")
+
+    redun.executors.aws_batch.batch_submit.return_value = {"jobId": "batch-job-id"}
+
+    # Create example workflow script to be packaged.
+    File("workflow.py").write(
+        """
+@task()
+def task1(x):
+    return x + 10
+    """
+    )
+
+    job = Job(task1())
+    job.id = job_id
+    job.eval_hash = "eval_hash"
+    code_file = package_code(s3_scratch_prefix)
+    resp = submit_task(
+        image,
+        queue,
+        s3_scratch_prefix,
+        job,
+        task1,
+        args=[10],
+        kwargs={},
+        code_file=code_file,
+        job_options={"num_nodes": 4},
+    )
+
+    # We should get a AWS Batch job id back.
+    assert resp["jobId"] == "batch-job-id"
+
+    # Input files should be made.
+    assert File("s3://example-bucket/redun/jobs/eval_hash/input").exists()
+    [code_file] = list(Dir("s3://example-bucket/redun/code"))
+
+    # We should have submitted a job to AWS Batch.
+    redun.executors.aws_batch.batch_submit.assert_called_with(
+        {
+            "nodeOverrides": {
+                "nodePropertyOverrides": [
+                    {
+                        "targetNodes": "0",
+                        "containerOverrides": {
+                            "command": [
+                                "redun",
+                                "--check-version",
+                                REDUN_REQUIRED_VERSION,
+                                "oneshot",
+                                "redun.tests.test_aws_batch",
+                                "--code",
+                                code_file.path,
+                                "--input",
+                                "s3://example-bucket/redun/jobs/eval_hash/input",
+                                "--error",
+                                "s3://example-bucket/redun/jobs/eval_hash/error",
+                                task1.name,
+                                "--output",
+                                "s3://example-bucket/redun/jobs/eval_hash/output",
+                            ]
+                        },
+                    },
+                    {
+                        "targetNodes": "1:",
+                        "containerOverrides": {
+                            "command": [
+                                "redun",
+                                "--check-version",
+                                REDUN_REQUIRED_VERSION,
+                                "oneshot",
+                                "redun.tests.test_aws_batch",
+                                "--code",
+                                code_file.path,
+                                "--input",
+                                "s3://example-bucket/redun/jobs/eval_hash/input",
+                                "--error",
+                                "s3://example-bucket/redun/jobs/eval_hash/error",
+                                task1.name,
+                            ]
+                        },
+                    },
+                ],
+            }
+        },
+        "queue",
+        image="my-image",
+        job_def_suffix="-redun-jd",
+        job_name="batch-job-eval_hash",
+        array_size=0,
+        aws_region="us-west-2",
+        num_nodes=4,
+    )
+
+
+@use_tempdir
+@mock_s3
+@patch("redun.executors.aws_batch.batch_submit")
 def test_submit_task_deep_file(batch_submit_mock):
     """
     Executor should be able to submit a task defined in a deeply nested file path.
     """
     job_id = "123"
     image = "my-image"
     queue = "queue"
@@ -353,32 +765,36 @@
 
     # Input files should be made.
     assert File("s3://example-bucket/redun/jobs/eval_hash/input").exists()
     [code_file] = list(Dir("s3://example-bucket/redun/code"))
 
     # We should have submitted a job to AWS Batch.
     redun.executors.aws_batch.batch_submit.assert_called_with(
-        [
-            "redun",
-            "--check-version",
-            REDUN_REQUIRED_VERSION,
-            "oneshot",
-            "workflow",
-            "--import-path",
-            "path/to",
-            "--code",
-            code_file.path,
-            "--input",
-            "s3://example-bucket/redun/jobs/eval_hash/input",
-            "--output",
-            "s3://example-bucket/redun/jobs/eval_hash/output",
-            "--error",
-            "s3://example-bucket/redun/jobs/eval_hash/error",
-            "task1",
-        ],
+        {
+            "containerOverrides": {
+                "command": [
+                    "redun",
+                    "--check-version",
+                    REDUN_REQUIRED_VERSION,
+                    "oneshot",
+                    "workflow",
+                    "--import-path",
+                    "path/to",
+                    "--code",
+                    code_file.path,
+                    "--input",
+                    "s3://example-bucket/redun/jobs/eval_hash/input",
+                    "--error",
+                    "s3://example-bucket/redun/jobs/eval_hash/error",
+                    "task1",
+                    "--output",
+                    "s3://example-bucket/redun/jobs/eval_hash/output",
+                ]
+            }
+        },
         "queue",
         image="my-image",
         job_def_suffix="-redun-jd",
         job_name="batch-job-eval_hash",
         array_size=0,
         aws_region="us-west-2",
     )
@@ -602,111 +1018,185 @@
     iter_batch_job_status_mock.return_value = iter([])
     parse_task_logs_mock.return_value = []
 
     scheduler = mock_scheduler()
     executor = mock_executor(scheduler)
     executor.start()
 
-    batch_submit_mock.return_value = {
-        "jobId": batch_job_id,
-    }
-
-    # Submit redun job that will succeed.
-    expr = task1(10)
-    job = Job(expr)
-    job.task = task1
-    job.eval_hash = "eval_hash"
-    executor.submit(job, [10], {})
+    try:
+        batch_submit_mock.return_value = {
+            "jobId": batch_job_id,
+        }
 
-    # Let job get stale so job arrayer actually submits it.
-    wait_until(lambda: executor.arrayer.num_pending == 0)
+        # Submit redun job that will succeed.
+        expr = task1(10)
+        job = Job(expr)
+        job.task = task1
+        job.eval_hash = "eval_hash"
+        executor.submit(job, [10], {})
+
+        # Let job get stale so job arrayer actually submits it.
+        wait_until(lambda: executor.arrayer.num_pending == 0)
+
+        # Ensure job options were passed correctly.
+        assert batch_submit_mock.call_args
+        assert batch_submit_mock.call_args[1] == {
+            "image": "my-image",
+            "job_name": "redun-job-eval_hash",
+            "job_def_suffix": "-redun-jd",
+            "array_size": 0,
+            "vcpus": 1,
+            "gpus": 0,
+            "memory": 4,
+            "role": None,
+            "retries": 1,
+            "aws_region": "us-west-2",
+            "num_nodes": None,
+            "batch_tags": {
+                "redun_aws_user": "alice",
+                "redun_execution_id": "",
+                "redun_job_id": job.id,
+                "redun_project": "",
+                "redun_task_name": "task1",
+            },
+        }
 
-    # Ensure job options were passed correctly.
-    assert batch_submit_mock.call_args
-    assert batch_submit_mock.call_args[1] == {
-        "image": "my-image",
-        "job_name": "redun-job-eval_hash",
-        "job_def_suffix": "-redun-jd",
-        "array_size": 0,
-        "vcpus": 1,
-        "gpus": 0,
-        "memory": 4,
-        "role": None,
-        "retries": 1,
-        "aws_region": "us-west-2",
-        "batch_tags": {
-            "redun_aws_user": "alice",
-            "redun_execution_id": "",
-            "redun_job_id": job.id,
-            "redun_project": "",
-            "redun_task_name": "task1",
-        },
-    }
+        batch_submit_mock.return_value = {
+            "jobId": batch_job2_id,
+        }
 
-    batch_submit_mock.return_value = {
-        "jobId": batch_job2_id,
-    }
+        # Submit redun job that will fail.
+        expr2 = task1.options(memory=8)("a")
+        job2 = Job(expr2)
+        job2.task = task1
+        job2.eval_hash = "eval_hash2"
+        executor.submit(job2, ["a"], {})
+
+        # Let job get stale so job arrayer actually submits it.
+        wait_until(lambda: executor.arrayer.num_pending == 0)
+
+        # Ensure job options were passed correctly.
+        assert batch_submit_mock.call_args[1] == {
+            "image": "my-image",
+            "job_name": "redun-job-eval_hash2",
+            "job_def_suffix": "-redun-jd",
+            "array_size": 0,
+            "vcpus": 1,
+            "gpus": 0,
+            "memory": 8,
+            "role": None,
+            "retries": 1,
+            "aws_region": "us-west-2",
+            "num_nodes": None,
+            "batch_tags": {
+                "redun_aws_user": "alice",
+                "redun_execution_id": "",
+                "redun_job_id": job2.id,
+                "redun_project": "",
+                "redun_task_name": "task1",
+            },
+        }
 
-    # Submit redun job that will fail.
-    expr2 = task1.options(memory=8)("a")
-    job2 = Job(expr2)
-    job2.task = task1
-    job2.eval_hash = "eval_hash2"
-    executor.submit(job2, ["a"], {})
+        # Simulate AWS Batch completing job.
+        output_file = File("s3://example-bucket/redun/jobs/eval_hash/output")
+        output_file.write(pickle_dumps(task1.func(10)), mode="wb")
+
+        # Simulate AWS Batch failing.
+        error = ValueError("Boom")
+        error_file = File("s3://example-bucket/redun/jobs/eval_hash2/error")
+        error_file.write(pickle_dumps((error, Traceback.from_error(error))), mode="wb")
+
+        iter_batch_job_status_mock.return_value = iter(
+            [
+                {
+                    "jobId": batch_job_id,
+                    "status": SUCCEEDED,
+                    "container": {"logStreamName": "log1"},
+                },
+                {"jobId": batch_job2_id, "status": FAILED, "container": {"logStreamName": "log2"}},
+            ]
+        )
 
-    # Let job get stale so job arrayer actually submits it.
-    wait_until(lambda: executor.arrayer.num_pending == 0)
+        scheduler.batch_wait([job.id, job2.id])
+        executor.stop()
 
-    # Ensure job options were passed correctly.
-    assert batch_submit_mock.call_args[1] == {
-        "image": "my-image",
-        "job_name": "redun-job-eval_hash2",
-        "job_def_suffix": "-redun-jd",
-        "array_size": 0,
-        "vcpus": 1,
-        "gpus": 0,
-        "memory": 8,
-        "role": None,
-        "retries": 1,
-        "aws_region": "us-west-2",
-        "batch_tags": {
-            "redun_aws_user": "alice",
-            "redun_execution_id": "",
-            "redun_job_id": job2.id,
-            "redun_project": "",
-            "redun_task_name": "task1",
-        },
-    }
+        # Job results and errors should be sent back to scheduler.
+        assert scheduler.job_results[job.id] == 20
+        assert isinstance(scheduler.job_errors[job2.id], ValueError)
+
+        # Assert job tags.
+        job.job_tags == [("aws_batch_job", "batch-job-id"), ("aws_log_stream", "log1")]
+        job.job_tags == [("aws_batch_job", "batch-job2-id"), ("aws_log_stream", "log2")]
+    finally:
+        # Ensure executor threads stop before continuing.
+        executor.stop()
 
-    # Simulate AWS Batch completing job.
-    output_file = File("s3://example-bucket/redun/jobs/eval_hash/output")
-    output_file.write(pickle_dumps(task1.func(10)), mode="wb")
 
-    # Simulate AWS Batch failing.
-    error = ValueError("Boom")
-    error_file = File("s3://example-bucket/redun/jobs/eval_hash2/error")
-    error_file.write(pickle_dumps((error, Traceback.from_error(error))), mode="wb")
+@mock_s3
+@patch("redun.executors.aws_utils.get_aws_user", return_value="alice")
+@patch("redun.executors.aws_batch.parse_task_logs")
+@patch("redun.executors.aws_batch.iter_batch_job_status")
+@patch("redun.executors.aws_batch.batch_submit")
+def test_executor_multinode(
+    batch_submit_mock, iter_batch_job_status_mock, parse_task_logs_mock, get_aws_user_mock
+) -> None:
+    """
+    Ensure that we can submit job to AWSBatchExecutor.
+    """
+    batch_job_id = "batch-job-id"
 
-    iter_batch_job_status_mock.return_value = iter(
-        [
-            {"jobId": batch_job_id, "status": SUCCEEDED, "container": {"logStreamName": "log1"}},
-            {"jobId": batch_job2_id, "status": FAILED, "container": {"logStreamName": "log2"}},
-        ]
-    )
+    # Setup AWS Batch mocks.
+    iter_batch_job_status_mock.return_value = iter([])
+    parse_task_logs_mock.return_value = []
 
-    scheduler.batch_wait([job.id, job2.id])
-    executor.stop()
+    scheduler = mock_scheduler()
+    executor = mock_executor(scheduler)
+    executor.start()
 
-    # Job results and errors should be sent back to scheduler.
-    assert scheduler.job_results[job.id] == 20
-    assert isinstance(scheduler.job_errors[job2.id], ValueError)
+    try:
+        batch_submit_mock.return_value = {
+            "jobId": batch_job_id,
+        }
 
-    # Assert job tags.
-    job.job_tags == [("aws_batch_job", "batch-job-id"), ("aws_log_stream", "log1")]
-    job.job_tags == [("aws_batch_job", "batch-job2-id"), ("aws_log_stream", "log2")]
+        # Submit redun job that will succeed.
+        expr = task1.options(num_nodes=4)(10)
+        job = Job(expr)
+        job.task = task1
+        job.eval_hash = "eval_hash"
+        executor.submit(job, [10], {})
+
+        # Let job get stale so job arrayer actually submits it.
+        wait_until(lambda: executor.arrayer.num_pending == 0)
+
+        # Ensure job options were passed correctly.
+        assert batch_submit_mock.call_args
+        assert batch_submit_mock.call_args[1] == {
+            "image": "my-image",
+            "job_name": "redun-job-eval_hash",
+            "job_def_suffix": "-redun-jd",
+            "array_size": 0,
+            "vcpus": 1,
+            "gpus": 0,
+            "memory": 4,
+            "role": None,
+            "retries": 1,
+            "aws_region": "us-west-2",
+            "num_nodes": 4,
+            "batch_tags": {
+                "redun_aws_user": "alice",
+                "redun_execution_id": "",
+                "redun_job_id": job.id,
+                "redun_project": "",
+                "redun_task_name": "task1",
+            },
+        }
+        job.job_tags == [("aws_batch_job", "batch-job-id#0"), ("aws_log_stream", "log1")]
+    finally:
+        # Ensure executor threads stop before continuing.
+        executor.stop()
 
 
 @mock_s3
 @patch("redun.executors.aws_utils.get_aws_user", return_value="alice")
 @patch("redun.executors.aws_batch.parse_task_logs")
 @patch("redun.executors.aws_batch.iter_local_job_status")
 @patch("redun.executors.aws_batch.run_docker")
@@ -727,71 +1217,81 @@
     parse_task_logs_mock.return_value = []
 
     # Setup redun mocks.
     scheduler = mock_scheduler()
     executor = mock_executor(scheduler, debug=True)
     executor.start()
 
-    run_docker_mock.return_value = batch_job_id
-
-    # Submit redun job that will succeed.
-    expr = task1(10)
-    job = Job(expr)
-    job.task = task1
-    job.eval_hash = "eval_hash"
-    executor.submit(job, [10], {})
-
-    # Let job get stale so job arrayer actually submits it.
-    wait_until(lambda: executor.arrayer.num_pending == 0)
-
-    # Ensure job options were passed correctly.
-    assert run_docker_mock.call_args[1] == {
-        "image": "my-image",
-    }
-
-    run_docker_mock.reset_mock()
-    run_docker_mock.return_value = batch_job2_id
+    try:
+        run_docker_mock.return_value = batch_job_id
 
-    # Hand create Job and submit.
-    expr2 = task1("a")
-    job2 = Job(expr2)
-    job2.task = task1
-    job2.eval_hash = "eval_hash2"
-    executor.submit(job2, ["a"], {})
-
-    # Let job get stale so job arrayer actually submits it.
-    wait_until(lambda: executor.arrayer.num_pending == 0)
-
-    # Ensure job options were passed correctly.
-    assert run_docker_mock.call_args[1] == {
-        "image": "my-image",
-    }
+        # Submit redun job that will succeed.
+        expr = task1(10)
+        job = Job(expr)
+        job.task = task1
+        job.eval_hash = "eval_hash"
+        executor.submit(job, [10], {})
+
+        # Let job get stale so job arrayer actually submits it.
+        wait_until(lambda: executor.arrayer.num_pending == 0)
+
+        # Ensure job options were passed correctly.
+        assert run_docker_mock.call_args[1] == {
+            "image": "my-image",
+            "gpus": 0,
+            "memory": 4,
+            "vcpus": 1,
+        }
 
-    # Simulate output file created by job.
-    output_file = File("s3://example-bucket/redun/jobs/eval_hash/output")
-    output_file.write(pickle_dumps(task1.func(10)), mode="wb")
+        run_docker_mock.reset_mock()
+        run_docker_mock.return_value = batch_job2_id
 
-    # Simulate AWS Batch failing.
-    error = ValueError("Boom")
-    error_file = File("s3://example-bucket/redun/jobs/eval_hash2/error")
-    error_file.write(pickle_dumps((error, Traceback.from_error(error))), mode="wb")
+        # Hand create Job and submit.
+        expr2 = task1("a")
+        job2 = Job(expr2)
+        job2.task = task1
+        job2.eval_hash = "eval_hash2"
+        executor.submit(job2, ["a"], {})
+
+        # Let job get stale so job arrayer actually submits it.
+        wait_until(lambda: executor.arrayer.num_pending == 0)
+
+        # Ensure job options were passed correctly.
+        assert run_docker_mock.call_args[1] == {
+            "image": "my-image",
+            "gpus": 0,
+            "memory": 4,
+            "vcpus": 1,
+        }
 
-    iter_local_job_status_mock.return_value = iter(
-        [
-            {"jobId": batch_job_id, "status": SUCCEEDED, "logs": ""},
-            {"jobId": batch_job2_id, "status": FAILED, "logs": ""},
-        ]
-    )
+        # Simulate output file created by job.
+        output_file = File("s3://example-bucket/redun/jobs/eval_hash/output")
+        output_file.write(pickle_dumps(task1.func(10)), mode="wb")
+
+        # Simulate AWS Batch failing.
+        error = ValueError("Boom")
+        error_file = File("s3://example-bucket/redun/jobs/eval_hash2/error")
+        error_file.write(pickle_dumps((error, Traceback.from_error(error))), mode="wb")
+
+        iter_local_job_status_mock.return_value = iter(
+            [
+                {"jobId": batch_job_id, "status": SUCCEEDED, "logs": ""},
+                {"jobId": batch_job2_id, "status": FAILED, "logs": ""},
+            ]
+        )
 
-    scheduler.batch_wait([job.id, job2.id])
-    executor.stop()
+        scheduler.batch_wait([job.id, job2.id])
 
-    # Job results and errors should be sent back to scheduler.
-    assert scheduler.job_results[job.id] == 20
-    assert isinstance(scheduler.job_errors[job2.id], ValueError)
+        # Job results and errors should be sent back to scheduler.
+        assert scheduler.job_results[job.id] == 20
+        assert isinstance(scheduler.job_errors[job2.id], ValueError)
+
+    finally:
+        # Ensure executor threads stop before continuing.
+        executor.stop()
 
 
 @mock_s3
 @patch("redun.executors.aws_utils.get_aws_user", return_value="alice")
 @patch("redun.executors.aws_batch.parse_task_logs")
 @patch("redun.executors.aws_batch.iter_batch_job_status")
 @patch("redun.executors.aws_batch.batch_submit")
@@ -944,14 +1444,17 @@
     # Let job get stale so job arrayer actually submits it
     wait_until(lambda: executor.arrayer.num_pending == 0)
 
     # Ensure job options were passed correctly.
     assert run_docker_mock.call_args[1] == {
         "image": "my-image",
         "interactive": True,
+        "gpus": 0,
+        "memory": 4,
+        "vcpus": 1,
     }
 
     # Cleanly stop executor.
     executor.stop()
 
 
 @mock_s3
@@ -1032,16 +1535,17 @@
         "one": "carrots:1",
         "two": "carrots:2",
     }
 
 
 @mock_s3
 @patch("redun.executors.aws_utils.get_aws_user", return_value="alice")
+@patch("redun.executors.aws_batch.iter_local_job_status")
 @patch("redun.executors.aws_utils.package_code")
-def test_code_packaging(package_code_mock, get_aws_user_mock) -> None:
+def test_code_packaging(package_code_mock, iter_local_job_status_mock, get_aws_user_mock) -> None:
     """
     Ensure that code packaging only happens on first submission.
     """
     package_code_mock.return_value = "s3://fake-bucket/code.tar.gz"
 
     scheduler = mock_scheduler()
     executor = mock_executor(scheduler, debug=True, code_package=True)
@@ -1072,15 +1576,16 @@
     assert package_code_mock.call_count == 1
 
     executor.stop()
 
 
 @mock_s3
 @patch("redun.executors.aws_utils.get_aws_user", return_value="alice")
-def test_inflight_join_disabled_in_debug(get_aws_user_mock) -> None:
+@patch("redun.executors.aws_batch.iter_local_job_status")
+def test_inflight_join_disabled_in_debug(iter_local_job_status_mock, get_aws_user_mock) -> None:
     """
     Ensure that debug=True disables inflight job gathering as it is unnecessary.
     """
     scheduler = mock_scheduler()
     executor = mock_executor(scheduler, debug=True)
     executor.start()
```

### Comparing `redun-0.8.7/redun/tests/test_uri_parsing.py` & `redun-0.8.9/redun/tests/test_uri_parsing.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_logging.py` & `redun-0.8.9/redun/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_file.py` & `redun-0.8.9/redun/tests/test_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,45 @@
     assert file.copy_to(file2) == file2
     assert file2.read() == "hello2"
 
     assert file.size() == 6
 
 
 @use_tempdir
+def test_encoding() -> None:
+    """
+    File read/write/open should support encodings.
+    """
+    text = "hello \u1F600"
+
+    # Read and write utf-8.
+    file = File("hello.txt")
+    file.write(text, encoding="utf-8")
+    assert file.read(encoding="utf-8") == text
+    assert file.read("rb") == b"hello \xe1\xbd\xa00"
+
+    # Read and write utf-16.
+    file2 = File("hello.txt")
+    file2.write(text, encoding="utf-16")
+    assert file2.read(encoding="utf-16") == text
+    assert file2.read("rb") == b"\xff\xfeh\x00e\x00l\x00l\x00o\x00 \x00`\x1f0\x00"
+
+    # Ensure File context can use encoding.
+    with file.open(mode="w", encoding="utf-8") as out:
+        out.write(text)
+
+    with file.open(mode="r", encoding="utf-8") as infile:
+        assert infile.read() == text
+
+    # Binary mode cannot be used with encoding.
+    with pytest.raises(ValueError, match="encoding"):
+        file.open(mode="rb", encoding="utf-8")
+
+
+@use_tempdir
 def test_dir_api() -> None:
 
     dir = Dir("hi")
     assert dir.rel_path(os.getcwd()) == ".."
 
     assert not dir.exists()
     dir.mkdir()
```

### Comparing `redun-0.8.7/redun/tests/test_serializers.py` & `redun-0.8.9/redun/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_args.py` & `redun-0.8.9/redun/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_cli.py` & `redun-0.8.9/redun/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1651,14 +1651,64 @@
     # Update a tag.
     output = run_command(client, ["redun", "tag", "update", execution.id, "env=prod2"])
     output = run_command(client, ["redun", "tag", "list", "env=prod2"])
     assert "Exec " in output
 
 
 @use_tempdir
+def test_cli_log_tags_order() -> None:
+    """
+    redun log entries should have tags sorted in a stable way, even if their values are not
+    comparable directly.
+    """
+    file = File("workflow.py")
+    file.write(
+        """
+from redun import task
+from redun.scheduler import apply_tags
+
+redun_namespace = 'test'
+
+@task()
+def example1():
+    return apply_tags(
+        42,
+        execution_tags=[("key", {"b": 1}), ("key", {"a": 2})]
+    )
+
+@task()
+def example2():
+    return apply_tags(
+        42,
+        execution_tags=[("key", {"c": 2}), ("key", {"c": 1})]
+    )
+
+"""
+    )
+
+    # Run example workflow.
+    client = RedunClient()
+    client.execute(["redun", "run", "workflow.py", "example1"])
+    client.execute(["redun", "run", "workflow.py", "example2"])
+
+    lines = run_command(client, ["redun", "log"]).split("\n")
+
+    assert_match_lines(
+        [
+            r"Recent executions:",
+            r"",
+            r"Exec.*key={\"c\": 1}, key={\"c\": 2}.*",
+            r"Exec.*key={\"a\": 2}, key={\"b\": 1}.*",
+            r"",
+        ],
+        lines,
+    )
+
+
+@use_tempdir
 def test_cli_log_files() -> None:
     """
     cli should support querying for files.
     """
     file = File("workflow.py")
     file.write(
         """
```

### Comparing `redun-0.8.7/redun/tests/test_functools.py` & `redun-0.8.9/redun/tests/test_functools.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,27 +74,24 @@
 
     @task()
     def subtask(name, interval):
         time.sleep(interval)
         calls.append(name)
         return name
 
-    assert (
-        scheduler.run(
-            seq(
-                [
-                    subtask(1, 0.2),
-                    subtask(2, 0.1),
-                    subtask(3, 0.01),
-                    subtask(4, 0.01),
-                ]
-            )
+    assert scheduler.run(
+        seq(
+            [
+                subtask(1, 0.2),
+                subtask(2, 0.1),
+                subtask(3, 0.01),
+                subtask(4, 0.01),
+            ]
         )
-        == [1, 2, 3, 4]
-    )
+    ) == [1, 2, 3, 4]
     assert calls == [1, 2, 3, 4]
 
     assert scheduler.run(seq([])) == []
     assert scheduler.run(seq([10])) == [10]
     assert scheduler.run(seq([subtask(1, 0)])) == [1]
```

### Comparing `redun-0.8.7/redun/tests/test_static_analysis.py` & `redun-0.8.9/redun/tests/test_static_analysis.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_db_utils.py` & `redun-0.8.9/redun/tests/test_db_utils.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_scheduler.py` & `redun-0.8.9/redun/tests/test_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,28 @@
 from sqlalchemy.orm import Session
 
 from redun import Scheduler, task
 from redun.backends.db import Execution, RedunBackendDb
 from redun.config import Config
 from redun.expression import SchedulerExpression
 from redun.promise import Promise
-from redun.scheduler import DryRunResult, Frame, Job, Task, Traceback, catch, cond, scheduler_task
+from redun.scheduler import (
+    DryRunResult,
+    Frame,
+    Job,
+    Task,
+    Traceback,
+    catch,
+    catch_all,
+    cond,
+    scheduler_task,
+)
 from redun.task import PartialTask, SchedulerTask
 from redun.tests.utils import assert_match_lines, use_tempdir
+from redun.utils import map_nested_value
 from redun.value import Value, get_type_registry
 
 
 def test_simple(scheduler: Scheduler) -> None:
     """
     A single task should execute.
     """
@@ -1334,14 +1345,77 @@
         calls.append("deep2")
         return 2
 
     assert scheduler.run(catch(faulty(), ZeroDivisionError, recover)) == 2
     assert calls == ["faulty", "recover", "deep", "deep2"]
 
 
+def test_catch_all(scheduler: Scheduler) -> None:
+    """
+    Catch expression should handle exceptions.
+    """
+
+    @task
+    def throw(error: Exception) -> None:
+        raise error
+
+    @task
+    def good(x=10):
+        return x
+
+    @task
+    def bad(message="boom"):
+        raise ValueError(message)
+
+    @task
+    def recover(results):
+        return map_nested_value(
+            lambda result: (0 if isinstance(result, Exception) else result), results
+        )
+
+    # All subtasks succeed.
+    assert scheduler.run(catch_all([good(1), good(2), good(3)], ValueError, recover)) == [1, 2, 3]
+
+    # Failed tasks should be caught.
+    assert scheduler.run(catch_all([good(4), bad(), good(5)], ValueError, recover)) == [4, 0, 5]
+    assert scheduler.run(catch_all([good(6), bad(), bad(), good(7)], ValueError, recover)) == [
+        6,
+        0,
+        0,
+        7,
+    ]
+
+    # We should be able to catch multiple error classes.
+    assert scheduler.run(
+        catch_all(
+            [throw(KeyError()), throw(ValueError()), good()], (KeyError, ValueError), recover
+        )
+    ) == [0, 0, 10]
+
+    # Without a recovery, errors should reraise.
+    with pytest.raises(ValueError):
+        scheduler.run(catch_all([good(), bad(), good()]))
+
+    # Different error_class should pass through.
+    with pytest.raises(ValueError):
+        scheduler.run(catch_all([good(), bad(), good()], ZeroDivisionError, recover))
+
+    # Different error_class should pass through, even if others are caught.
+    with pytest.raises(ValueError):
+        scheduler.run(
+            catch_all([throw(KeyError()), throw(ValueError()), good()], KeyError, recover)
+        )
+
+    # Any kind of nested value should work.
+    assert scheduler.run(catch_all([good(8), [bad(), {"a": good(9)}]], ValueError, recover)) == [
+        8,
+        [0, {"a": 9}],
+    ]
+
+
 def test_config_args(scheduler: Scheduler) -> None:
     """
     Config_args should not contribute to the eval_hash.
     """
 
     @task(config_args=["x", "z"])
     def task1(x: int, y: int, z: str = "hello") -> int:
@@ -1424,7 +1498,36 @@
 
     @task
     def main2(x: List[int] = [add(1, 2)]) -> List[int]:
         # Default argument might contain an expression within a nested value (e.g. list).
         return x
 
     assert scheduler.run(main2()) == [3]
+
+
+def test_job_clear(scheduler: Scheduler) -> None:
+    """
+    Job clean up should occur correctly even when child jobs fail.
+
+    https://insitro.atlassian.net/browse/DE-4645
+    """
+
+    @task
+    def child(x: int) -> int:
+        if x == 2:
+            raise ValueError("raised by child")
+        return x
+
+    @task
+    def child2(x: int) -> int:
+        return x
+
+    @task
+    def parent(n: int) -> List[int]:
+        return [child2(child(i)) for i in range(n)]
+
+    @task
+    def main(n: int) -> List[int]:
+        return parent(n)
+
+    with pytest.raises(ValueError, match="raised by child"):
+        scheduler.run(main(10))
```

### Comparing `redun-0.8.7/redun/tests/test_limits.py` & `redun-0.8.9/redun/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_executors.py` & `redun-0.8.9/redun/tests/test_executors.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/tests/test_db.py` & `redun-0.8.9/redun/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/value.py` & `redun-0.8.9/redun/value.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/db/dataflow.py` & `redun-0.8.9/redun/backends/db/dataflow.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/db/query.py` & `redun-0.8.9/redun/backends/db/query.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/db/alembic.ini` & `redun-0.8.9/redun/backends/db/alembic.ini`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/db/alembic/env.py` & `redun-0.8.9/redun/backends/db/alembic/env.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/db/alembic/versions/806f5dcb11bf_initial_schema.py` & `redun-0.8.9/redun/backends/db/alembic/versions/806f5dcb11bf_initial_schema.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/db/alembic/versions/cc4f663817b6_add_tag_models.py` & `redun-0.8.9/redun/backends/db/alembic/versions/cc4f663817b6_add_tag_models.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/db/alembic/versions/30ffbaee18cd_add_task_version_and_backfill_companion_values.py` & `redun-0.8.9/redun/backends/db/alembic/versions/30ffbaee18cd_add_task_version_and_backfill_companion_values.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/db/alembic/versions/cd2d53191748_make_job_execution_id_non_nullable.py` & `redun-0.8.9/redun/backends/db/alembic/versions/cd2d53191748_make_job_execution_id_non_nullable.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/db/alembic/versions/d4af139b6f53_add_job_execution_id.py` & `redun-0.8.9/redun/backends/db/alembic/versions/d4af139b6f53_add_job_execution_id.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/db/alembic/versions/647c510a77b1_add_evaluation_model.py` & `redun-0.8.9/redun/backends/db/alembic/versions/647c510a77b1_add_evaluation_model.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/db/alembic/versions/71ec303c90e4_add_id_indexes.py` & `redun-0.8.9/redun/backends/db/alembic/versions/71ec303c90e4_add_id_indexes.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/db/serializers.py` & `redun-0.8.9/redun/backends/db/serializers.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/db/__init__.py` & `redun-0.8.9/redun/backends/db/__init__.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/base.py` & `redun-0.8.9/redun/backends/base.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/backends/value_store.py` & `redun-0.8.9/redun/backends/value_store.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/executors/aws_utils.py` & `redun-0.8.9/redun/executors/aws_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import pickle
 import shlex
 import tarfile
 import tempfile
 import threading
 import zipfile
-from typing import Any, Dict, Iterable, List, NamedTuple, Optional, Set, Tuple, Union
+from typing import Any, Dict, Iterable, Iterator, List, NamedTuple, Optional, Set, Tuple, Union
 
 import boto3
 
 from redun.file import File
 from redun.hashing import hash_stream
 from redun.scheduler import Job
 
@@ -225,7 +225,58 @@
     if not job.task.script:
         with output_file.open("rb") as infile:
             result = pickle.load(infile)
     else:
         result = [0, output_file.read(mode="rb")]  # TODO: Get real exitcode.
 
     return result
+
+
+def iter_log_stream(
+    log_group_name: str,
+    log_stream: str,
+    limit: Optional[int] = None,
+    reverse: bool = False,
+    required: bool = True,
+    aws_region: str = DEFAULT_AWS_REGION,
+) -> Iterator[dict]:
+    """
+    Iterate through the events of logStream.
+    """
+    logs_client = get_aws_client("logs", aws_region=aws_region)
+    try:
+        response = logs_client.get_log_events(
+            logGroupName=log_group_name,
+            logStreamName=log_stream,
+            startFromHead=not reverse,
+            # boto API does not allow passing None, so we must fully exclude the parameter.
+            **{"limit": limit} if limit else {},
+        )
+    except logs_client.exceptions.ResourceNotFoundException as error:
+        if required:
+            # If logs are required, raise an error.
+            raise error
+        else:
+            return
+
+    while True:
+        events = response["events"]
+
+        # If no events, we are at the end of the stream.
+        if not events:
+            break
+
+        if reverse:
+            events = reversed(events)
+        yield from events
+
+        if not reverse:
+            next_token = response["nextForwardToken"]
+        else:
+            next_token = response["nextBackwardToken"]
+        response = logs_client.get_log_events(
+            logGroupName=log_group_name,
+            logStreamName=log_stream,
+            nextToken=next_token,
+            # boto API does not allow passing None, so we must fully exclude the parameter.
+            **{"limit": limit} if limit else {},
+        )
```

### Comparing `redun-0.8.7/redun/executors/glue_oneshot.py.txt` & `redun-0.8.9/redun/executors/glue_oneshot.py.txt`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/executors/local.py` & `redun-0.8.9/redun/executors/local.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,18 @@
     # Available local executor modes.
     MODES = [THREAD_MODE, PROCESS_MODE]
     _OLD2NEW_MODES = {
         "threads": THREAD_MODE,
         "processes": PROCESS_MODE,
     }
     START_METHODS = ["fork", "spawn", "forkserver"]
+    # start_method fork is not reliable on Mac OS X. So we use forkserver as
+    # a safe common default.
+    # https://bugs.python.org/issue33725
+    DEFAULT_START_METHOD = "forkserver"
 
     def __init__(
         self,
         name: str,
         scheduler: Optional["Scheduler"] = None,
         config=None,
         mode: str = THREAD_MODE,
@@ -65,15 +69,15 @@
 
         self.max_workers = config.getint("max_workers", 20)
         self.mode = config.get("mode", mode)
         # Autoconvert deprecated modes.
         self.mode = self._OLD2NEW_MODES.get(self.mode, self.mode)
         assert self.mode in self.MODES, f"Unknown mode: {self.mode}"
 
-        self.start_method = config.get("start_method", "fork")
+        self.start_method = config.get("start_method", self.DEFAULT_START_METHOD)
         assert (
             self.start_method in self.START_METHODS
         ), f"Unknown start_method: {self.start_method}"
 
         # Pools.
         self._thread_executor: Optional[ThreadPoolExecutor] = None
         self._process_executor: Optional[ProcessPoolExecutor] = None
```

### Comparing `redun-0.8.7/redun/executors/base.py` & `redun-0.8.9/redun/executors/base.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/executors/aws_glue.py` & `redun-0.8.9/redun/executors/aws_glue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import datetime
 import json
 import os
 import pickle
 import tempfile
 import threading
 import time
 from collections import OrderedDict, deque
@@ -28,15 +27,22 @@
     success=["SUCCEEDED"],
     failure=["FAILED", "ERROR"],
     stopped=["STOPPED"],
     timeout=["TIMEOUT"],
 )
 
 # These packages are needed for the redun lib to work on glue.
-DEFAULT_ADDITIONAL_PYTHON_MODULES = "alembic,mako,promise,sqlalchemy"
+# Versions should remain up to date with setup.py
+DEFAULT_ADDITIONAL_PYTHON_MODULES = [
+    "alembic>=1.4",
+    "mako",
+    "promise",
+    "s3fs>=2021.11.1",
+    "sqlalchemy>=1.3.17or<2",  # Don't use commas as AWS won't parse them.
+]
 
 
 def get_spark_history_dir(s3_scratch_prefix: str) -> str:
     """
     Returns s3 scratch path for Spark UI monitoring files.
     """
     return os.path.join(s3_scratch_prefix, "glue", "spark_history")
@@ -90,42 +96,43 @@
 
 def get_or_create_glue_job_definition(
     script_location: str,
     role: str,
     temp_dir: str,
     extra_py_files: str,
     spark_history_dir: str,
-    additional_python_modules: str = DEFAULT_ADDITIONAL_PYTHON_MODULES,
+    additional_python_modules: List[str] = DEFAULT_ADDITIONAL_PYTHON_MODULES,
     aws_region: str = aws_utils.DEFAULT_AWS_REGION,
 ) -> str:
     """
     Gets or creates an AWS Glue Job.
     """
     client = aws_utils.get_aws_client("glue", aws_region=aws_region)
 
     # Define job definition.
     glue_job_def = dict(
         Description=f"Redun oneshot glue job {aws_utils.REDUN_REQUIRED_VERSION}",
         Role=role,
         ExecutionProperty={
-            "MaxConcurrentRuns": 1000,  # account-max value.
-        },
+            "MaxConcurrentRuns": 1000,
+        },  # account-max value.
         Command={
             "Name": "glueetl",
             "ScriptLocation": script_location,
             "PythonVersion": "3",
         },
         DefaultArguments={
             "--TempDir": temp_dir,
             "--enable-s3-parquet-optimized-committer": "true",
             "--extra-py-files": extra_py_files,
-            "--additional-python-modules": additional_python_modules,
+            "--additional-python-modules": ",".join(additional_python_modules),
             "--job-bookmark-option": "job-bookmark-disable",
             "--job-language": "python",
             "--enable-spark-ui": "true",
+            "--enable-job-insights": "true",
             "--spark-event-logs-path": spark_history_dir,
         },
         MaxRetries=0,
         NumberOfWorkers=2,  # Jobs will override this, so set to minimum value.
         WorkerType="Standard",
         GlueVersion="3.0",
         Timeout=2880,
@@ -344,62 +351,63 @@
         return None, False
 
     def _process_job_status(self, job: dict) -> None:
         assert self.scheduler
 
         error: Optional[Exception] = None
         error_traceback: Optional[Traceback] = None
+        result: Optional[Any] = None
+        redun_job = self.running_glue_jobs.get(job["Id"])
+        assert redun_job
 
         if job["JobRunState"] in GLUE_JOB_STATUSES.success:
-            redun_job = self.running_glue_jobs.pop(job["Id"])
             result, exists = self._get_job_output(redun_job, check_valid=False)
             if exists:
-                self.scheduler.done_job(redun_job, result)
+                error = None
             else:
                 error = FileNotFoundError(
                     aws_utils.get_job_scratch_file(
                         self.s3_scratch_prefix, redun_job, aws_utils.S3_SCRATCH_OUTPUT
                     )
                 )
                 error_traceback = None
 
         elif job["JobRunState"] in GLUE_JOB_STATUSES.stopped:
-            redun_job = self.running_glue_jobs.pop(job["Id"])
             error = AWSGlueJobStoppedError("Job stopped by user.")
-            self.scheduler.reject_job(redun_job, error)
 
         elif job["JobRunState"] in GLUE_JOB_STATUSES.failure:
-            redun_job = self.running_glue_jobs.pop(job["Id"])
-            error, error_traceback = parse_task_error(self.s3_scratch_prefix, redun_job, job)
-
-            if not self.debug:
-                logs = ["*** CloudWatch logs for AWS Glue job {}:\n".format(job["Id"])]
-                logs.extend(
-                    get_error_logs(
-                        job_id=job["Id"],
-                        log_group_name=job["LogGroupName"] + "/error",
-                        aws_region=self.aws_region,
-                        max_results=100,
-                    )
-                )
-                if len(logs) > 100:
-                    logs.extend(["-----\n", "*** Logs truncated to last 100 errors ***\n"])
 
-                error_traceback.logs = logs
+            # Errors may not be unpicklable out of the Glue environment, so use CloudWatch
+            # job insights to get a traceback.
+            if self.debug:
+                error, error_traceback = parse_task_error(self.s3_scratch_prefix, redun_job, job)
+            else:
+                error = AWSGlueError("Glue job failed: see log info.")
+                error_traceback = Traceback.from_error(error)
 
-            self.scheduler.reject_job(redun_job, error, error_traceback=error_traceback)
+                error_traceback.logs = get_job_insight_traceback(
+                    job_id=job["Id"],
+                    log_group_name=job["LogGroupName"],
+                    aws_region=self.aws_region,
+                    max_results=100,
+                )
 
         elif job["JobRunState"] in GLUE_JOB_STATUSES.timeout:
-            redun_job = self.running_glue_jobs.pop(job["Id"])
-
             error = AWSGlueJobTimeoutError(job.get("ErrorMessage", ""))
             error_traceback = Traceback.from_error(error)
 
+        # Job is still running
+        else:
+            return
+
+        self.running_glue_jobs.pop(job["Id"])
         if error:
             self.scheduler.reject_job(redun_job, error, error_traceback=error_traceback)
+        else:
+            self.scheduler.done_job(redun_job, result)
 
     def _get_job_options(self, job: Job) -> dict:
         """
         Determines task options for a job.
         """
         assert job.task
 
@@ -550,16 +558,16 @@
         "--task": a_task.fullname,
         "--error": error_path,
         "--job-hash": job.eval_hash,
     }
 
     # Comma separated string of Python modules to be installed with pip before job start.
     if job_options.get("additional_libs"):
-        glue_args["--additional-python-modules"] = (
-            DEFAULT_ADDITIONAL_PYTHON_MODULES + "," + ",".join(job_options["additional_libs"])
+        glue_args["--additional-python-modules"] = ",".join(
+            DEFAULT_ADDITIONAL_PYTHON_MODULES + job_options["additional_libs"]
         )
 
     # Extra python and data files are specified as comma separated strings.
     # Files are first copied to S3, as Glue requires them to be there.
 
     # Extra py files will be in an importable location at job start.
     # They can be either importable zip files, or .py source files.
@@ -632,44 +640,48 @@
         )
         error = AWSGlueError(message)
         error_traceback = Traceback.from_error(error)
 
     return error, error_traceback
 
 
-def get_error_logs(
+def get_job_insight_traceback(
     job_id: str,
     log_group_name: str,
     aws_region: str = aws_utils.DEFAULT_AWS_REGION,
     max_results=200,
-) -> Iterator[str]:
+) -> List[str]:
     """
-    Gets error lines from a log group.
+    Gets the traceback from AWS' Glue Job insights.
     """
-    logs_client = aws_utils.get_aws_client("logs", aws_region=aws_region)
-    paginator = logs_client.get_paginator("filter_log_events")
+    log_lines = aws_utils.iter_log_stream(
+        log_group_name=f"{log_group_name}/logs-v2",
+        log_stream=f"{job_id}-job-insights-rca-driver",
+        limit=max_results,
+        reverse=False,
+        required=False,
+        aws_region=aws_region,
+    )
 
-    try:
-        for response in paginator.paginate(
-            logGroupName=log_group_name,
-            logStreamNamePrefix=job_id,
-            filterPattern="?ERROR ?Error ?error ?Exception ?exception ?WARN",
-            PaginationConfig={"MaxItems": max_results},
-        ):
-
-            events = response["events"]
-            while events:
-                event = events.pop(0)
-                timestamp = str(datetime.datetime.fromtimestamp(event["timestamp"] / 1000))
-                yield "{timestamp}  {message}".format(
-                    timestamp=timestamp, message=event["message"]
+    if not log_lines:
+        return ["No job insights found. See AWS Glue GUI online."]
+
+    traceback = []
+    for line in log_lines:
+        message = line.get("message")
+        if message and "Failure Reason" in message:
+            # Message looks like "ERROR GlueException... [Glue Exception Analysis] {DICT we want}".
+            try:
+                traceback.extend(
+                    json.loads(message[message.index("{") :])["Failure Reason"].split("\n")
                 )
+            except Exception:
+                continue
 
-    except logs_client.exceptions.ResourceNotFoundException:
-        return None
+    return traceback
 
 
 class AWSGlueError(Exception):
     pass
 
 
 class AWSGlueJobTimeoutError(Exception):
```

### Comparing `redun-0.8.7/redun/executors/aws_batch.py` & `redun-0.8.9/redun/executors/aws_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import datetime
 import json
 import logging
 import os
 import pickle
 import re
 import subprocess
@@ -125,54 +126,113 @@
 @lru_cache(maxsize=200)
 def get_or_create_job_definition(
     job_def_name: str,
     image: str,
     command: List[str] = ["ls"],
     memory: int = 4,
     vcpus: int = 1,
+    num_nodes: Optional[int] = None,
+    shared_memory: Optional[int] = None,
     role: Optional[str] = None,
     aws_region: str = aws_utils.DEFAULT_AWS_REGION,
     privileged: bool = False,
 ) -> dict:
     """
-    Returns a job definition with the specified requirements.
+    Returns a job definition with the specified requirements. Although the resource requirements
+    provided are used when creating a job, they are specifically excluded from creating new
+    job definitions.
 
     Either an existing active job definition is used or a new one is created.
+
+    num_nodes - if present, create a multi-node batch job.
     """
     batch_client = aws_utils.get_aws_client("batch", aws_region=aws_region)
 
     # Get default IAM role.
     if role is None:
         caller_id = aws_utils.get_aws_client("sts", aws_region=aws_region).get_caller_identity()
         account_num = caller_id["Account"]
         role = "arn:aws:iam::%d:role/ecsTaskExecutionRole" % int(account_num)
 
+    existing_job_def = get_job_definition(job_def_name, batch_client=batch_client)
+
     container_props = {
         "command": command,
         "image": image,
         "vcpus": vcpus,
         "memory": memory,
         "jobRoleArn": role,
         "environment": [],
         "mountPoints": [],
         "volumes": [],
         "resourceRequirements": [],
         "ulimits": [],
         "privileged": privileged,
     }
-    existing_job_def = get_job_definition(job_def_name, batch_client=batch_client)
+    if shared_memory is not None:
+        container_props["linuxParameters"] = {"sharedMemorySize": int(shared_memory * 1024)}
+
+    if num_nodes is None:
+        # Single-node job type
+
+        job_details = {"type": "container", "containerProperties": container_props}
+
+    else:
+        # Multi-node job type
+        node_properties = {
+            "mainNode": 0,
+            "numNodes": num_nodes,
+            "nodeRangeProperties": [
+                # Create two identical node groups, so we can tell only the main node to provide
+                # outputs.
+                {
+                    "container": container_props,
+                    "targetNodes": "0",
+                },
+                {
+                    "container": container_props,
+                    "targetNodes": "1:",
+                },
+            ],
+        }
+
+        job_details = {"type": "multinode", "nodeProperties": node_properties}
+
+    # We override resource properties, so create sanitized versions of both job definitions to
+    # compare them
+    no_resource_container_properties = {
+        "vcpus": "any_vcpus",
+        "memory": "any_memory",
+        "resourceRequirements": ["any_requirements"],
+    }
+
+    def sanitize_job_def(job_def: Dict) -> Dict:
+        """Overwrite the resource properties with redactions."""
+        result = copy.deepcopy(job_def)
+        result["containerProperties"] = result.get("containerProperties", {}).update(
+            no_resource_container_properties
+        )
+        node_range = result.get("nodeProperties", {}).get("nodeRangeProperties", [{}, {}])
+        node_range[0].get("container", {}).update(no_resource_container_properties)
+        node_range[1].get("container", {}).update(no_resource_container_properties)
+        result["nodeRangeProperties"] = node_range
+        return result
+
     if existing_job_def:
-        existing_container_props = existing_job_def.get("containerProperties", {})
-        if existing_container_props == container_props:
+        # If there's an existing job with no interesting variations, we can use it.
+        sanitized_existing_job_def = sanitize_job_def(existing_job_def)
+        sanitized_job_details = sanitize_job_def(job_details)
+
+        if all(
+            [sanitized_existing_job_def.get(k, {}) == v for k, v in sanitized_job_details.items()]
+        ):
             return existing_job_def
 
-    # register job definition
-    job_def = batch_client.register_job_definition(
-        jobDefinitionName=job_def_name, type="container", containerProperties=container_props
-    )
+    job_def = batch_client.register_job_definition(jobDefinitionName=job_def_name, **job_details)
+
     return job_def
 
 
 def make_job_def_name(image_name: str, job_def_suffix: str = "-jd") -> str:
     """
     Autogenerate a job definition name from an image name.
     """
@@ -184,75 +244,145 @@
     # For Job definition name, enter a unique name for your job definition. Up to 128 letters
     # (uppercase and lowercase), numbers, hyphens, and underscores are allowed.
     job_def_prefix = re.sub("[^A-Za-z_0-9-]", "", image_name)[: 128 - len(job_def_suffix)]
     job_def_name = job_def_prefix + job_def_suffix
     return job_def_name
 
 
-def batch_submit(
+def create_job_override_command(
     command: List[str],
+    command_output_suffix: Optional[List[str]] = None,
+    num_nodes: Optional[int] = None,
+) -> Dict[str, Any]:
+    """Format the command into the form needed for the AWS Batch `submit_job` API.
+
+    command: A list of tokens comprising the command
+    command_output_suffix: Tokens to add to the end of the command to actually trigger output
+        to get written.
+    num_nodes: If `None`, this is a single-node job. If not `None`, a multi-node job.
+
+    Returns a dictionary to be passed to `submit_job` as kwargs."""
+    batch_job_args: Dict[str, Any] = {}
+
+    # Multi-node jobs use node overrides.
+    if command_output_suffix is None:
+        command_output_suffix = []
+
+    if num_nodes is None:
+        # Single-node jobs override the container.
+        batch_job_args["containerOverrides"] = {"command": command + command_output_suffix}
+    else:
+
+        # Make a shallow copy so we can suppress output on these nodes
+        node_overrides = [
+            {
+                "targetNodes": "0",
+                "containerOverrides": {"command": command + command_output_suffix},
+            },
+            {"targetNodes": "1:", "containerOverrides": {"command": command}},
+        ]
+
+        batch_job_args["nodeOverrides"] = {"nodePropertyOverrides": node_overrides}
+
+    return batch_job_args
+
+
+def batch_submit(
+    batch_job_args: dict,
     queue: str,
     image: str,
     job_def_name: Optional[str] = None,
     job_def_suffix: str = "-jd",
     job_name: str = "batch-job",
     array_size: int = 0,
     memory: int = 4,
     vcpus: int = 1,
     gpus: int = 0,
+    num_nodes: Optional[int] = None,
+    shared_memory: Optional[int] = None,
     retries: int = 1,
     role: Optional[str] = None,
     aws_region: str = aws_utils.DEFAULT_AWS_REGION,
     privileged: bool = False,
     autocreate_job: bool = True,
     timeout: Optional[int] = None,
     batch_tags: Optional[Dict[str, str]] = None,
     propagate_tags: bool = True,
 ) -> Dict[str, Any]:
+    """Actually perform job submission to AWS batch. Create or retrieve the job definition, then
+    use it to submit the job.
 
+    batch_job_args : dict
+        These are passed as kwargs to the `submit_job` API. Generally, it must configure the
+        commands to be run by setting node or container overrides. This function will modify
+        the provided dictionary, at a minimum applying overrides for the resource requirements
+        stated by other arguments to this function.
+    """
     batch_client = aws_utils.get_aws_client("batch", aws_region=aws_region)
 
     # Get or create job definition. If autocreate_job is disabled, then we require a job_def_name
     # to be present and lookup the job by name. If autocreate_job is enabled, then we will create
     # a job if an existing one matching job def name and required properties cannot be found.
     if not autocreate_job:
         assert job_def_name
         job_def = get_job_definition(job_def_name, aws_region=aws_region)
         if not job_def:
             raise ValueError(f"No job with name {job_def_name} was found.")
     else:
         job_def_name = job_def_name or make_job_def_name(image, job_def_suffix)
         job_def = get_or_create_job_definition(
-            job_def_name, image, role=role, aws_region=aws_region, privileged=privileged
+            job_def_name,
+            image,
+            role=role,
+            aws_region=aws_region,
+            privileged=privileged,
+            num_nodes=num_nodes,
+            shared_memory=shared_memory,
         )
 
-    # Container overrides for this job.
-    container_overrides = {"vcpus": vcpus, "memory": int(memory * 1024), "command": command}
-    if gpus > 0:
-        container_overrides["resourceRequirements"] = [{"type": "GPU", "value": str(gpus)}]
+    def apply_resources(container_properties: Dict) -> None:
+        """Modify the provided dictionary of container properties to apply requested resources"""
 
-    batch_job_args: dict = {
-        "propagateTags": propagate_tags,
-    }
+        # Switch units, redun configs are in GB but AWS uses MB.
+        memory_mb = int(memory * 1024)
+
+        container_properties.update({"vcpus": vcpus, "memory": memory_mb})
+        if gpus > 0:
+            container_properties["resourceRequirements"] = [{"type": "GPU", "value": str(gpus)}]
+
+    if "containerOverrides" in batch_job_args:
+        apply_resources(batch_job_args["containerOverrides"])
+
+    if "nodeOverrides" in batch_job_args:
+        for node in batch_job_args["nodeOverrides"]["nodePropertyOverrides"]:
+            apply_resources(node["containerOverrides"])
+
+    batch_job_args["propagateTags"] = propagate_tags
     if array_size > 0:
         batch_job_args["arrayProperties"] = {"size": array_size}
+        if num_nodes is not None:
+            raise ValueError("Cannot combine array jobs and multi-node jobs.")
     if timeout:
         batch_job_args["timeout"] = {"attemptDurationSeconds": timeout}
     if batch_tags:
         batch_job_args["tags"] = batch_tags
 
     # Submit to batch.
     batch_run = batch_client.submit_job(
         jobName=job_name,
         jobQueue=queue,
         jobDefinition=job_def["jobDefinitionArn"],
-        containerOverrides=container_overrides,
         retryStrategy={"attempts": retries},
         **batch_job_args,
     )
+
+    # For multi-node jobs, the rank 0 job id is sufficient for monitoring.
+    if num_nodes is not None:
+        batch_run["jobId"] = f"{batch_run['jobId']}#0"
+
     return batch_run
 
 
 def is_ec2_instance() -> bool:
     """
     Returns True if this process is running on an EC2 instance.
 
@@ -268,14 +398,18 @@
 def run_docker(
     command: List[str],
     image: str,
     array_index: int = -1,
     volumes: Optional[Iterable[Tuple[str, str]]] = None,
     interactive: bool = True,
     cleanup: bool = False,
+    memory: int = 4,
+    vcpus: int = 1,
+    gpus: int = 0,
+    shared_memory: Optional[int] = None,
 ) -> str:
     """
     volumes: a list of ('host', 'container') path pairs for volume mouting.
     """
     # Add AWS credentials to environment for docker command.
     env = dict(os.environ)
     if not is_ec2_instance():
@@ -305,14 +439,21 @@
 
     # Volume mounting args.
     if not volumes:
         volumes = []
     for host, container in volumes:
         common_args.extend(["-v", f"{host}:{container}"])
 
+    common_args.extend([f"--memory={memory}g", f"--cpus={vcpus}"])
+    if gpus:
+        # We can't easily assign a single gpu so we make all available if any GPUs are required.
+        common_args.extend(["--gpus", "all"])
+    if shared_memory is not None:
+        common_args.append(f"--shm-size={shared_memory}g")
+
     common_args.append(image)
     common_args.extend(command)
 
     if interactive:
         # Adding this flag is necessary to prevent docker from hijacking the terminal and modifying
         # the tty settings. One of the modifications it makes when it hijacks the terminal is to
         # change the behavior of line endings which means output(like from logging) will be
@@ -375,30 +516,32 @@
     """
     Returns AWS Batch-specific job options from general job options.
     """
     keys = [
         "vcpus",
         "gpus",
         "memory",
+        "shared_memory",
         "role",
         "retries",
         "privileged",
         "job_def_name",
         "autocreate_job",
         "timeout",
         "batch_tags",
+        "num_nodes",
     ]
     return {key: job_options[key] for key in keys if key in job_options}
 
 
 def get_docker_job_options(job_options: dict) -> dict:
     """
     Returns Docker-specific job options from general job options.
     """
-    keys = ["volumes", "interactive"]
+    keys = ["vcpus", "memory", "gpus", "shared_memory", "volumes", "interactive"]
     return {key: job_options[key] for key in keys if key in job_options}
 
 
 def submit_task(
     image: str,
     queue: str,
     s3_scratch_prefix: str,
@@ -467,53 +610,66 @@
             "oneshot",
             a_task.load_module,
         ]
         + import_args
         + code_arg
         + array_arg
         + cache_arg
-        + ["--input", input_path, "--output", output_path, "--error", error_path, a_task.fullname]
+        + ["--input", input_path, "--error", error_path, a_task.fullname]
     )
+    command_output_suffix = [
+        "--output",
+        output_path,
+    ]
 
     if not debug:
         if array_uuid:
             job_hash = array_uuid
         else:
             assert job.eval_hash
             job_hash = job.eval_hash
 
         # Submit to AWS Batch.
         job_name = get_batch_job_name(
             job_options.get("job_name_prefix", "batch-job"), job_hash, array=bool(array_size)
         )
 
+        job_batch_options = get_batch_job_options(job_options)
+        job_batch_args = create_job_override_command(
+            command=command,
+            command_output_suffix=command_output_suffix,
+            num_nodes=job_batch_options.get("num_nodes", None),
+        )
+
         result = batch_submit(
-            command,
+            job_batch_args,
             queue,
             image=image,
             job_name=job_name,
             job_def_suffix="-redun-jd",
             aws_region=aws_region,
             array_size=array_size,
-            **get_batch_job_options(job_options),
+            **job_batch_options,
         )
     else:
         # Submit to local Docker.
         # This loop only runs if array_size > 0
         result = {"jobId": [], "redun_job_id": []}
         for i in range(array_size):
             container_id = run_docker(
                 command, image=image, array_index=i, **get_docker_job_options(job_options)
             )
             result["jobId"].append(container_id)
             result["redun_job_id"].append(job.id)
 
         # Otherwise, submit one non-array job
         if not array_size:
-            container_id = run_docker(command, image=image, **get_docker_job_options(job_options))
+            container_id = run_docker(
+                command + command_output_suffix, image=image, **get_docker_job_options(job_options)
+            )
             result = {"jobId": container_id, "redun_job_id": job.id}
     return result
 
 
 def submit_command(
     image: str,
     queue: str,
@@ -575,23 +731,30 @@
     if not debug:
         # Submit to AWS Batch.
         assert job.eval_hash
         job_name = get_batch_job_name(
             job_options.get("job_name_prefix", "batch-job"), job.eval_hash
         )
 
+        job_batch_options = get_batch_job_options(job_options)
+        job_batch_args = create_job_override_command(
+            command=shell_command,
+            command_output_suffix=None,
+            num_nodes=job_batch_options.get("num_nodes", None),
+        )
+
         # Submit to AWS Batch.
         return batch_submit(
-            shell_command,
+            job_batch_args,
             queue,
             image=image,
             job_name=job_name,
             job_def_suffix="-redun-jd",
             aws_region=aws_region,
-            **get_batch_job_options(job_options),
+            **job_batch_options,
         )
     else:
         # Submit to local Docker.
         container_id = run_docker(
             shell_command, image=image, **get_docker_job_options(job_options)
         )
         return {"jobId": container_id, "redun_job_id": job.id}
@@ -703,65 +866,14 @@
         else:
             pending_run = 0
 
         if pending_truncate > 0 and pending_run > pending_truncate:
             break
 
 
-def iter_log_stream(
-    log_group_name: str,
-    log_stream: str,
-    limit: Optional[int] = None,
-    reverse: bool = False,
-    required: bool = True,
-    aws_region: str = aws_utils.DEFAULT_AWS_REGION,
-) -> Iterator[dict]:
-    """
-    Iterate through the events of logStream.
-    """
-    logs_client = aws_utils.get_aws_client("logs", aws_region=aws_region)
-    try:
-        response = logs_client.get_log_events(
-            logGroupName=log_group_name,
-            logStreamName=log_stream,
-            startFromHead=not reverse,
-            # boto API does not allow passing None, so we must fully exclude the parameter.
-            **{"limit": limit} if limit else {},
-        )
-    except logs_client.exceptions.ResourceNotFoundException as error:
-        if required:
-            # If logs are required, raise an error.
-            raise error
-        else:
-            return
-
-    while True:
-        events = response["events"]
-
-        # If no events, we are at the end of the stream.
-        if not events:
-            break
-
-        if reverse:
-            events = reversed(events)
-        yield from events
-
-        if not reverse:
-            next_token = response["nextForwardToken"]
-        else:
-            next_token = response["nextBackwardToken"]
-        response = logs_client.get_log_events(
-            logGroupName=log_group_name,
-            logStreamName=log_stream,
-            nextToken=next_token,
-            # boto API does not allow passing None, so we must fully exclude the parameter.
-            **{"limit": limit} if limit else {},
-        )
-
-
 def format_log_stream_event(event: dict) -> str:
     """
     Format a logStream event as a line.
     """
     timestamp = str(datetime.datetime.fromtimestamp(event["timestamp"] / 1000))
     return "{timestamp}  {message}".format(timestamp=timestamp, message=event["message"])
 
@@ -778,20 +890,20 @@
     Iterate through the log events of an AWS Batch job.
     """
     # Get job's log stream.
     job = next(aws_describe_jobs([job_id], aws_region=aws_region), None)
     if not job:
         # Job is no longer present in AWS API. Return no logs.
         return
-    log_stream = job["container"].get("logStreamName")
+    log_stream = job.get("container", {}).get("logStreamName")
     if not log_stream:
         # No log stream is present. Return no logs.
         return
 
-    yield from iter_log_stream(
+    yield from aws_utils.iter_log_stream(
         log_group_name=log_group_name,
         log_stream=log_stream,
         limit=limit,
         reverse=reverse,
         required=required,
         aws_region=aws_region,
     )
@@ -887,14 +999,15 @@
         self.default_task_options = {
             "vcpus": config.getint("vcpus", 1),
             "gpus": config.getint("gpus", 0),
             "memory": config.getint("memory", 4),
             "retries": config.getint("retries", 1),
             "role": config.get("role"),
             "job_name_prefix": config.get("job_name_prefix", "redun-job"),
+            "num_nodes": config.getint("num_nodes", None),
         }
         if config.get("batch_tags"):
             self.default_task_options["batch_tags"] = json.loads(config.get("batch_tags"))
         self.use_default_batch_tags = config.getboolean("default_batch_tags", True)
 
         self.is_running = False
         # We use an OrderedDict in order to retain submission order.
```

### Comparing `redun-0.8.7/redun/bcoding.py` & `redun-0.8.9/redun/bcoding.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/functools.py` & `redun-0.8.9/redun/functools.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/job_array.py` & `redun-0.8.9/redun/job_array.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/scheduler.py` & `redun-0.8.9/redun/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,28 +49,30 @@
     derive_expression,
     get_lazy_operation,
     quote,
 )
 from redun.handle import Handle
 from redun.hashing import hash_eval, hash_struct
 from redun.logging import logger as _logger
-from redun.promise import Promise
+from redun.promise import Promise, wait_promises
 from redun.tags import parse_tag_value
 from redun.task import Task, TaskRegistry, get_task_registry, scheduler_task, task
 from redun.utils import format_table, iter_nested_value, map_nested_value, trim_string
 from redun.value import TypeError as RedunTypeError
 from redun.value import Value, get_type_registry
 
 # Globals.
 _local = threading.local()
 
 # Constants.
 JOB_ACTION_WIDTH = 6  # Width of job action in logs.
 
 Result = TypeVar("Result")
+T = TypeVar("T")
+S = TypeVar("S")
 
 
 def settrace_patch(tracefunc: Any) -> None:
     """
     Monkey patch for recording whether debugger REPL is active or not.
 
     sys.settrace() is called by debuggers such as pdb whenever the debugger
@@ -381,17 +383,14 @@
         self.kwargs = None
         self.eval_args = None
         self.result_promise = None
         self.result = None
         self.job_tags.clear()
         self.execution_tags.clear()
         self.value_tags.clear()
-
-        for child_job in self.child_jobs:
-            child_job.parent_job = None
         self.child_jobs.clear()
 
 
 def get_backend_from_config(backend_config: Optional[SectionProxy] = None) -> RedunBackend:
     """
     Parses a redun :class:`redun.backends.base.RedunBackend` from a config object.
     """
@@ -1146,16 +1145,21 @@
         # Preprocess arguments before sending them to task function.
         args, kwargs = job.eval_args
         args, kwargs = self.preprocess_args(job, args, kwargs)
 
         # Check cache using eval_hash as key.
         job.eval_hash, job.args_hash = self.get_eval_hash(job.task, args, kwargs)
 
+        # HACK: This is a workaround introduced by DE-4761. See the ticket for
+        # notes on how script_task could be redesigned to remove the need for
+        # this special-casing.
+        is_script_task = job.task_name == "redun.script_task"
+
         call_hash: Optional[str]
-        if self.use_cache and job.get_option("cache", True):
+        if self.use_cache and job.get_option("cache", True) and not is_script_task:
             result, job.was_cached, call_hash = self.get_cache(
                 job,
                 job.eval_hash,
                 job.task.hash,
                 job.args_hash,
                 check_valid=job.get_option("check_valid", "full"),
             )
@@ -1924,14 +1928,119 @@
         cached_expr, is_cached = scheduler.backend.get_eval_cache(eval_hash)
         if is_cached:
             return scheduler.evaluate(cached_expr, parent_job=parent_job).catch(promise_catch)
 
     return scheduler.evaluate(expr, parent_job=parent_job).then(on_success, promise_catch)
 
 
+@scheduler_task(namespace="redun", version="1")
+def catch_all(
+    scheduler: Scheduler,
+    parent_job: Job,
+    sexpr: SchedulerExpression,
+    exprs: T,
+    error_class: Union[None, Exception, Tuple[Exception, ...]] = None,
+    recover: Optional[Task[Callable[..., S]]] = None,
+) -> Promise[Union[T, S]]:
+    """
+    Catch all exceptions that occur in the nested value `exprs`.
+
+    This task works similar to `catch`, except it takes multiple
+    expressions within a nested value (e.g. a list, set, dict, etc).
+    Any exceptions raised by the expressions are caught and processed only after
+    all expressions succeed or fail. For example, this can be useful in large
+    fanouts where the user wants to avoid one small error stopping the whole
+    workflow immediately. Consider the following code:
+
+    .. code-block:: python
+
+        @task
+        def divider(denom):
+            return 1.0 / denom
+
+        @task
+        def recover(values):
+            nerrors = sum(1 for value in values if isinstance(value, Exception))
+            raise Exception(f"{nerrors} error(s) occurred.")
+
+        @task
+        def main():
+            result catch_all([divider(1), divider(0), divider(2)], ZeroDivisionError, recover)
+
+    Each of the expressions in the list `[divider(1), divider(0), divider(2)]`
+    will be allowed to finish before the exceptions are processed by `recover`. If
+    there are no exceptions, the evaluated list is returned. If there are any
+    exceptions, the list is passed to `recover`, where it will contain each
+    successful result or Exception. `recover` then has the opportunity to process
+    all errors together. In the example above, the total number of errors is
+    reraised.
+
+    Parameters
+    ----------
+    exprs:
+        A nested value (list, set, dict, tuple, NamedTuple) of expressions to evaluate.
+    error_class: Union[Exception, Tuple[Expression, ...]]
+        An Exception or Exceptions to catch.
+    recover: Task
+        A task to call if any errors occurs. It will be called with the nested
+        value containing both successful results and errors.
+    """
+
+    def postprocess(pending_terms):
+        # Gather all errors.
+        errors = [promise.error for promise in pending_terms if promise.is_rejected]
+
+        if errors:
+            if not recover:
+                # By default, just reraise the first error.
+                raise errors[0]
+            else:
+
+                def do_recover(error_class_recover):
+                    error_class, recover = error_class_recover
+                    if all(isinstance(error, error_class) for error in errors):
+                        return scheduler.evaluate(
+                            recover(map_nested_value(resolve_term, pending_expr)),
+                            parent_job=parent_job,
+                        )
+                    else:
+                        # By default, just reraise first non-matching error.
+                        raise next(error for error in errors if not isinstance(error, error_class))
+
+                # Evaluate error_class and recover in case they're Expressions.
+                return scheduler.evaluate((error_class, recover), parent_job=parent_job).then(
+                    do_recover
+                )
+        else:
+            # Return the evaluated nested value.
+            return map_nested_value(resolve_term, pending_expr)
+
+    def resolve_term(value):
+        # Replace a Promise with its return value or its error.
+        if isinstance(value, Promise):
+            if value.is_fulfilled:
+                return value.value
+            else:
+                return value.error
+        else:
+            # Regular values (non-Promises) pass through unchanged.
+            return value
+
+    pending_terms = []
+
+    def eval_term(value):
+        # Evaluate one term and track its promise in pending_terms.
+        promise = scheduler.evaluate(value, parent_job=parent_job)
+        pending_terms.append(promise)
+        return promise
+
+    pending_expr = map_nested_value(eval_term, exprs)
+    return wait_promises(pending_terms).then(postprocess)
+
+
 @scheduler_task(namespace="redun")
 def apply_tags(
     scheduler: Scheduler,
     parent_job: Job,
     sexpr: SchedulerExpression,
     value: Any,
     tags: List[Tuple[str, Any]] = [],
```

### Comparing `redun-0.8.7/redun/db_utils.py` & `redun-0.8.9/redun/db_utils.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun/config.py` & `redun-0.8.9/redun/config.py`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/setup.py` & `redun-0.8.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     "alembic>=1.4",
     "boto3>=1.16.63",
     "botocore>=1.22.8",
     "gcsfs>=2021.4.0",
     "s3fs>=2021.11.1",
     "sqlalchemy>=1.3.17,<2",
     "python-dateutil>=2.8",
+    # If updating this list, check executors/aws_glue.py stays up to date with
+    # packages needed to run in the glue environment.
 ]
 
-extras = {
-    "glue": ["pandas", "pyarrow"],
-}
+extras = {"glue": ["pandas", "pyarrow", "pyspark"]}
 
 if REQUIRE_POSTGRES:
     requirements.append(PSYCOPG2_VERSION)
 else:
     extras["postgres"] = [PSYCOPG2_VERSION]
```

### Comparing `redun-0.8.7/redun.egg-info/SOURCES.txt` & `redun-0.8.9/redun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/redun.egg-info/PKG-INFO` & `redun-0.8.9/redun.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redun
-Version: 0.8.7
+Version: 0.8.9
 Summary: Yet another redundant workflow engine.
 Home-page: https://github.com/insitro/redun/
 Author: Matt Rasmussen
 Author-email: rasmus@insitro.com
 License: UNKNOWN
 Description: 
         redun aims to be a more expressive and efficient workflow framework, built on
```

### Comparing `redun-0.8.7/LICENSE` & `redun-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `redun-0.8.7/PKG-INFO` & `redun-0.8.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redun
-Version: 0.8.7
+Version: 0.8.9
 Summary: Yet another redundant workflow engine.
 Home-page: https://github.com/insitro/redun/
 Author: Matt Rasmussen
 Author-email: rasmus@insitro.com
 License: UNKNOWN
 Description: 
         redun aims to be a more expressive and efficient workflow framework, built on
```

### Comparing `redun-0.8.7/README.md` & `redun-0.8.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <img src="docs/source/redun.svg" width="200"/>
 
 *yet another redundant workflow engine*
 
-**redun** aims to be a more expressive and efficient workflow framework, built on top of the popular Python programming language. It takes the somewhat contrarian view that writing dataflows directly is unnecessarily restrictive, and by doing so we lose abstractions we have come to rely on in most modern high-level languages (control flow, compositiblity, recursion, high order functions, etc). redun's key insight is that workflows can be expressed as [lazy expressions](#whats-the-trick), that are then evaluated by a scheduler which performs automatic parallelization, caching, and data provenance logging.
+**redun** aims to be a more expressive and efficient workflow framework, built on top of the popular Python programming language. It takes the somewhat contrarian view that writing dataflows directly is unnecessarily restrictive, and by doing so we lose abstractions we have come to rely on in most modern high-level languages (control flow, composability, recursion, high order functions, etc). redun's key insight is that workflows can be expressed as [lazy expressions](#whats-the-trick), which are then evaluated by a scheduler that performs automatic parallelization, caching, and data provenance logging.
 
 redun's key features are:
 
 - Workflows are defined by lazy expressions that when evaluated emit dynamic directed acyclic graphs (DAGs), enabling complex data flows.
 - Incremental computation that is reactive to both data changes as well as code changes.
 - Workflow tasks can be executed on a variety of compute backend (threads, processes, AWS batch jobs, Spark jobs, etc). 
-- Data changes are detected for in memory values as well as external data sources such as files and object stores using file hashing.
-- Code changes are detected by hashing individual Python functions and comparing against historical call graph recordings.
+- Data changes are detected for in-memory values as well as external data sources such as files and object stores using file hashing.
+- Code changes are detected by hashing individual Python functions and comparing them against historical call graph recordings.
 - Past intermediate results are cached centrally and reused across workflows.
 - Past call graphs can be used as a data lineage record and can be queried for debugging and auditing.
 
-See the [original blog post](https://insitro.medium.com/when-data-science-goes-with-the-flow-insitro-introduces-redun-8b06b707a14b), [documenation](https://insitro.github.io/redun/design.html), [tutorial](examples/README.md), and [influences](https://insitro.github.io/redun/design.html#influences) for more.
+See the [original blog post](https://insitro.medium.com/when-data-science-goes-with-the-flow-insitro-introduces-redun-8b06b707a14b), [documentation](https://insitro.github.io/redun/design.html), [tutorial](examples/README.md), and [influences](https://insitro.github.io/redun/design.html#influences) for more.
 
-*About the name:* The name "redun" is self deprecating (there are [A LOT](https://github.com/pditommaso/awesome-pipeline) of workflow engines), but it is also a reference to its original inspiration, the [redo](https://apenwarr.ca/log/20101214) build system.
+*About the name:* The name "redun" is self-deprecating (there are [A LOT](https://github.com/pditommaso/awesome-pipeline) of workflow engines), but it is also a reference to its original inspiration, the [redo](https://apenwarr.ca/log/20101214) build system.
 
 ## Install
 
 ```sh
 pip install redun
 ```
 
@@ -249,15 +249,15 @@
         c_file_2 = <dfa3aba7> File(path=prog.c, hash=dfa3aba7)
 
       c_file_2 <-- argument of <74cceb4e> make_prog(prog_path, c_files)
                <-- argument of <45400ab5> make(files)
                <-- origin
 ```
 
-This output shows the original `link` task source code responsible for creating the program `prog`, as well as the full derivation, denoted "upstream dataflow". See the full example for a [deeper explanation](examples/02_compile#data-provenance-for-files) of this output. To understand more about the data structure that powers these kind of queries, see [call graphs](https://insitro.github.io/redun/design.html#call-graphs).
+This output shows the original `link` task source code responsible for creating the program `prog`, as well as the full derivation, denoted "upstream dataflow". See the full example for a [deeper explanation](examples/02_compile#data-provenance-for-files) of this output. To understand more about the data structure that powers these kinds of queries, see [call graphs](https://insitro.github.io/redun/design.html#call-graphs).
 
 We can change one of the input files, such as `lib.c`, and rerun the workflow. Due to redun's automatic incremental compute, only the minimal tasks are rerun:
 
 ```
 redun run make.py make
 
 [redun] redun :: version 0.4.15
@@ -280,15 +280,15 @@
 [redun] | redun.examples.compile.link            0       0       0       0       2       2
 [redun] | redun.examples.compile.make            0       0       0       0       1       1
 [redun] | redun.examples.compile.make_prog       0       0       0       0       2       2
 [redun]
 [File(path=prog, hash=2f43c23c), File(path=prog2, hash=b4537ad7)]
 ```
 
-Notice, two of the compile jobs are cached (`prog.c` and `prog2.c`), but compiling the library `lib.c` and the downstream link steps correctly rerun.
+Notice, two of the compile jobs are cached (`prog.c` and `prog2.c`), but compiling the library `lib.c` and the downstream link steps are correctly rerun.
 
 Check out the [examples](examples/) for more example workflows and features of redun. Also, see the [design notes](https://insitro.github.io/redun/design.html) for more information on redun's design.
 
 ## Mixed compute backends
 
 In the above example, each task ran in its own thread. However, more generally each task can run in its own process, Docker container, [AWS Batch job](examples/05_aws_batch), or [Spark job](examples/aws_glue). With [minimal configuration](examples/05_aws_batch/.redun/redun.ini), users can lightly annotate where they would like each task to run. redun will automatically handle the data and code movement as well as backend scheduling:
 
@@ -320,12 +320,12 @@
 
 <img width="800" src="examples/02_compile/images/expression-graph.svg">
 
 For a more in-depth walk-through, see the [scheduler tutorial](examples/03_scheduler).
 
 ## Why not another workflow engine?
 
-redun focuses on making multi-domain scientific pipelines easy to develop and deploy. The automatic parallelism, caching, code and data reactivity, as well as data provenance features makes it a great fit for such work. However, redun does not attempt to solve all possible workflow problems, so it's perfectly reasonable to supplement it with other tools. For example, while redun provides a very expressive way to define [task parallelism](https://en.wikipedia.org/wiki/Task_parallelism), it does not attempt to perform the kind of fine-grain [data parallelism](https://en.wikipedia.org/wiki/Data_parallelism) more commonly provided by Spark or Dask. Fortunately, redun does not perform any "dirty tricks" (e.g. complex static analysis or call stack manipulation), and so we have found it possible to safely combine redun with other frameworks (e.g. pyspark, pytorch, Dask, etc) to achieve the benefits of each tool.
+redun focuses on making multi-domain scientific pipelines easy to develop and deploy. The automatic parallelism, caching, code, and data reactivity, as well as data provenance features, make it a great fit for such work. However, redun does not attempt to solve all possible workflow problems, so it's perfectly reasonable to supplement it with other tools. For example, while redun provides a very expressive way to define [task parallelism](https://en.wikipedia.org/wiki/Task_parallelism), it does not attempt to perform the kind of fine-grain [data parallelism](https://en.wikipedia.org/wiki/Data_parallelism) more commonly provided by Spark or Dask. Fortunately, redun does not perform any "dirty tricks" (e.g. complex static analysis or call stack manipulation), and so we have found it possible to safely combine redun with other frameworks (e.g. pyspark, pytorch, Dask, etc) to achieve the benefits of each tool.
 
-Lastly, redun does not provide its own compute cluster, but instead builds upon other systems that do, such as cloud provider services for batch Docker jobs or Spark jobs.
+Lastly, redun does not provide its own compute cluster but instead builds upon other systems that do, such as cloud provider services for batch Docker jobs or Spark jobs.
 
 For more details on how redun compares to other related ideas, see the [influences](https://insitro.github.io/redun/design.html#influences) section.
```

