# Comparing `tmp/flytekit-1.6.0b0.tar.gz` & `tmp/flytekit-1.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.6.0b0.tar", last modified: Wed Apr 19 20:54:19 2023, max compression
+gzip compressed data, was "flytekit-1.6.0b1.tar", last modified: Wed May  3 04:47:56 2023, max compression
```

## Comparing `flytekit-1.6.0b0.tar` & `flytekit-1.6.0b1.tar`

### file list

```diff
@@ -1,244 +1,244 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-19 20:54:16.000000 flytekit-1.6.0b0/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28007 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.370920 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    27156 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.370920 flytekit-1.6.0b0/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    35808 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    30894 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    35772 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17439 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    45827 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    75336 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    37762 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/stats/taggable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.378920 flytekit-1.6.0b0/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.378920 flytekit-1.6.0b0/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.378920 flytekit-1.6.0b0/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    82901 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44333 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-19 20:54:16.000000 flytekit-1.6.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.004263 flytekit-1.6.0b1/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-03 04:47:53.000000 flytekit-1.6.0b1/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.004263 flytekit-1.6.0b1/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.004263 flytekit-1.6.0b1/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.008263 flytekit-1.6.0b1/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.008263 flytekit-1.6.0b1/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28007 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.008263 flytekit-1.6.0b1/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.008263 flytekit-1.6.0b1/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.008263 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29387 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.008263 flytekit-1.6.0b1/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    35938 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31110 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36193 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45827 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75520 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37762 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.012263 flytekit-1.6.0b1/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/interfaces/stats/taggable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.016264 flytekit-1.6.0b1/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82901 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44333 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.004263 flytekit-1.6.0b1/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-03 04:47:55.000000 flytekit-1.6.0b1/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-03 04:47:55.000000 flytekit-1.6.0b1/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:47:55.000000 flytekit-1.6.0b1/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-03 04:47:55.000000 flytekit-1.6.0b1/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-03 04:47:55.000000 flytekit-1.6.0b1/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 04:47:55.000000 flytekit-1.6.0b1/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-03 04:47:44.000000 flytekit-1.6.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-03 04:47:56.020264 flytekit-1.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-03 04:47:53.000000 flytekit-1.6.0b1/setup.py
```

### Comparing `flytekit-1.6.0b0/LICENSE` & `flytekit-1.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/MANIFEST.in` & `flytekit-1.6.0b1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/PKG-INFO` & `flytekit-1.6.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b1 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.0b0/README.md` & `flytekit-1.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/__init__.py` & `flytekit-1.6.0b1/flytekit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,15 @@
 from flytekit.core.resources import Resources
 from flytekit.core.schedule import CronSchedule, FixedRate
 from flytekit.core.task import Secret, reference_task, task
 from flytekit.core.workflow import ImperativeWorkflow as Workflow
 from flytekit.core.workflow import WorkflowFailurePolicy, reference_workflow, workflow
 from flytekit.deck import Deck
 from flytekit.extras import pytorch, sklearn, tensorflow
+from flytekit.image_spec import ImageSpec
 from flytekit.loggers import logger
 from flytekit.models.common import Annotations, AuthRole, Labels
 from flytekit.models.core.execution import WorkflowExecutionPhase
 from flytekit.models.core.types import BlobType
 from flytekit.models.documentation import Description, Documentation, SourceCode
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
@@ -236,15 +237,15 @@
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.6.0b0"
+__version__ = "1.6.0b1"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
```

### Comparing `flytekit-1.6.0b0/flytekit/bin/entrypoint.py` & `flytekit-1.6.0b1/flytekit/bin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/clients/auth/auth_client.py` & `flytekit-1.6.0b1/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/clients/auth/authenticator.py` & `flytekit-1.6.0b1/flytekit/clients/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/clients/auth/keyring.py` & `flytekit-1.6.0b1/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/clients/auth/token_client.py` & `flytekit-1.6.0b1/flytekit/clients/auth/token_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/clients/auth_helper.py` & `flytekit-1.6.0b1/flytekit/clients/auth_helper.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/clients/friendly.py` & `flytekit-1.6.0b1/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.6.0b1/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.6.0b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/clients/helpers.py` & `flytekit-1.6.0b1/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/clients/raw.py` & `flytekit-1.6.0b1/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/clis/flyte_cli/main.py` & `flytekit-1.6.0b1/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/clis/helpers.py` & `flytekit-1.6.0b1/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/backfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import typing
 from datetime import datetime, timedelta
 
-import click
+import rich_click as click
 
 from flytekit.clis.sdk_in_container.helpers import get_and_save_remote_with_click_context
 from flytekit.clis.sdk_in_container.run import DateTimeType, DurationParamType
 
 _backfill_help = """
 The backfill command generates and registers a new workflow based on the input launchplan to run an
 automated backfill. The workflow can be managed using the Flyte UI and can be canceled, relaunched, and recovered.
 
-- ``launchplan`` refers to the name of the Launchplan
-- ``launchplan_version`` is optional and should be a valid version for a Launchplan version.
+    - ``launchplan`` refers to the name of the Launchplan
+    - ``launchplan_version`` is optional and should be a valid version for a Launchplan version.
 """
 
 
 def resolve_backfill_window(
     from_date: datetime = None,
     to_date: datetime = None,
     backfill_window: timedelta = None,
@@ -164,15 +164,16 @@
             launchplan_version=launchplan_version,
             execution_name=execution_name,
             version=version,
             dry_run=dry_run,
             execute=execute,
             parallel=parallel,
         )
-        if entity:
-            console_url = remote.generate_console_url(entity)
-            if execute:
-                click.secho(f"\n Execution launched {console_url} to see execution in the console.", fg="green")
-                return
-            click.secho(f"\n Workflow registered at {console_url}", fg="green")
+        if dry_run:
+            return
+        console_url = remote.generate_console_url(entity)
+        if execute:
+            click.secho(f"\n Execution launched {console_url} to see execution in the console.", fg="green")
+            return
+        click.secho(f"\n Workflow registered at {console_url}", fg="green")
     except StopIteration as e:
         click.secho(f"{e.value}", fg="red")
```

### Comparing `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import pathlib
 import typing
 
-import click
+import rich_click as click
 from typing_extensions import OrderedDict
 
 from flytekit.clis.sdk_in_container.constants import CTX_MODULE, CTX_PROJECT_ROOT
 from flytekit.clis.sdk_in_container.run import RUN_LEVEL_PARAMS_KEY, get_entities_in_file, load_naive_entity
 from flytekit.configuration import ImageConfig, SerializationSettings
 from flytekit.core.base_task import PythonTask
 from flytekit.core.workflow import PythonFunctionWorkflow
```

### Comparing `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import click as _click
+import rich_click as _click
 
 CTX_PROJECT = "project"
 CTX_DOMAIN = "domain"
 CTX_VERSION = "version"
 CTX_TEST = "test"
 CTX_PACKAGES = "pkgs"
 CTX_NOTIFICATIONS = "notifications"
```

### Comparing `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import replace
 from typing import Optional
 
-import click
+import rich_click as click
 
 from flytekit.clis.sdk_in_container.constants import CTX_CONFIG_FILE
 from flytekit.configuration import Config, ImageConfig, get_config_file
 from flytekit.loggers import cli_logger
 from flytekit.remote.remote import FlyteRemote
 
 FLYTE_REMOTE_INSTANCE_KEY = "flyte_remote"
```

### Comparing `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/init.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import click
+import rich_click as click
 from cookiecutter.main import cookiecutter
 
 
 @click.command("init")
 @click.option(
     "--template",
     default="simple-example",
```

### Comparing `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import click
+import rich_click as click
 
 from flytekit.clis.sdk_in_container.helpers import get_and_save_remote_with_click_context
 from flytekit.models.launch_plan import LaunchPlanState
 
 _launchplan_help = """
 The launchplan command activates or deactivates a specified or the latest version of the launchplan.
 If ``--activate`` is chosen then the previous version of the launchplan will be deactivated.
```

### Comparing `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-import click
+import rich_click as click
 
 from flytekit.clis.helpers import display_help_with_error
 from flytekit.clis.sdk_in_container import constants
 from flytekit.configuration import (
     DEFAULT_RUNTIME_PYTHON_INTERPRETER,
     FastSerializationSettings,
     ImageConfig,
```

### Comparing `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 
-import click
 import grpc
+import rich_click as click
 from google.protobuf.json_format import MessageToJson
 
 from flytekit import configuration
 from flytekit.clis.sdk_in_container.backfill import backfill
 from flytekit.clis.sdk_in_container.build import build
 from flytekit.clis.sdk_in_container.constants import CTX_CONFIG_FILE, CTX_PACKAGES, CTX_VERBOSE
 from flytekit.clis.sdk_in_container.init import init
@@ -70,15 +70,15 @@
     if isinstance(e, grpc.RpcError):
         pretty_print_grpc_error(e)
         return
 
     click.secho(f"Failed with Unknown Exception {type(e)} Reason: {e}", fg="red")  # noqa
 
 
-class ErrorHandlingCommand(click.Group):
+class ErrorHandlingCommand(click.RichGroup):
     def invoke(self, ctx: click.Context) -> typing.Any:
         try:
             return super().invoke(ctx)
         except Exception as e:
             if CTX_VERBOSE in ctx.obj and ctx.obj[CTX_VERBOSE]:
                 print("Verbose mode on")
                 raise e
```

### Comparing `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import typing
 
-import click
+import rich_click as click
 
 from flytekit.clis.helpers import display_help_with_error
 from flytekit.clis.sdk_in_container import constants
 from flytekit.clis.sdk_in_container.helpers import get_and_save_remote_with_click_context, patch_image_config
 from flytekit.configuration import ImageConfig
 from flytekit.configuration.default_images import DefaultImages
 from flytekit.loggers import cli_logger
```

### Comparing `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import logging
 import os
 import pathlib
 import typing
 from dataclasses import dataclass
 from typing import cast
 
-import click
+import rich_click as click
+import yaml
 from dataclasses_json import DataClassJsonMixin
 from pytimeparse import parse
 from typing_extensions import get_args
 
 from flytekit import BlobType, Literal, Scalar
 from flytekit.clis.sdk_in_container.constants import (
     CTX_CONFIG_FILE,
@@ -51,18 +52,14 @@
 
 def remove_prefix(text, prefix):
     if text.startswith(prefix):
         return text[len(prefix) :]
     return text
 
 
-class JsonParamType(click.ParamType):
-    name = "json object"
-
-
 @dataclass
 class Directory(object):
     dir_path: str
     local_file: typing.Optional[pathlib.Path] = None
     local: bool = True
 
 
@@ -130,14 +127,41 @@
         self, value: typing.Any, param: typing.Optional[click.Parameter], ctx: typing.Optional[click.Context]
     ) -> typing.Any:
         if value is None:
             raise click.BadParameter("None value cannot be converted to a Duration type.")
         return datetime.timedelta(seconds=parse(value))
 
 
+class JsonParamType(click.ParamType):
+    name = "json object OR json/yaml file path"
+
+    def convert(
+        self, value: typing.Any, param: typing.Optional[click.Parameter], ctx: typing.Optional[click.Context]
+    ) -> typing.Any:
+        if value is None:
+            raise click.BadParameter("None value cannot be converted to a Json type.")
+        if type(value) == dict or type(value) == list:
+            return value
+        try:
+            return json.loads(value)
+        except Exception:  # noqa
+            try:
+                # We failed to load the json, so we'll try to load it as a file
+                if os.path.exists(value):
+                    # if the value is a yaml file, we'll try to load it as yaml
+                    if value.endswith(".yaml") or value.endswith(".yml"):
+                        with open(value, "r") as f:
+                            return yaml.safe_load(f)
+                    with open(value, "r") as f:
+                        return json.load(f)
+                raise
+            except json.JSONDecodeError as e:
+                raise click.BadParameter(f"parameter {param} should be a valid json object, {value}, error: {e}")
+
+
 @dataclass
 class DefaultConverter(object):
     click_type: click.ParamType
     primitive_type: typing.Optional[str] = None
     scalar_type: typing.Optional[str] = None
 
     def convert(self, value: typing.Any, python_type_hint: typing.Optional[typing.Type] = None) -> Scalar:
@@ -295,85 +319,116 @@
                 python_val = converter._click_type.convert(value, param, ctx)
                 literal = converter.convert_to_literal(ctx, param, python_val)
                 return Literal(scalar=Scalar(union=Union(literal, variant)))
             except (Exception or AttributeError) as e:
                 logging.debug(f"Failed to convert python type {python_type} to literal type {variant}", e)
         raise ValueError(f"Failed to convert python type {self._python_type} to literal type {lt}")
 
+    def convert_to_list(
+        self, ctx: typing.Optional[click.Context], param: typing.Optional[click.Parameter], value: list
+    ) -> Literal:
+        """
+        Convert a python list into a Flyte Literal
+        """
+        if not value:
+            raise click.BadParameter("Expected non-empty list")
+        if not isinstance(value, list):
+            raise click.BadParameter(f"Expected json list '[...]', parsed value is {type(value)}")
+        converter = FlyteLiteralConverter(
+            ctx,
+            self._flyte_ctx,
+            self._literal_type.collection_type,
+            type(value[0]),
+            self._create_upload_fn,
+        )
+        lt = Literal(collection=LiteralCollection([]))
+        for v in value:
+            click_val = converter._click_type.convert(v, param, ctx)
+            lt.collection.literals.append(converter.convert_to_literal(ctx, param, click_val))
+        return lt
+
+    def convert_to_map(
+        self, ctx: typing.Optional[click.Context], param: typing.Optional[click.Parameter], value: dict
+    ) -> Literal:
+        """
+        Convert a python dict into a Flyte Literal.
+        It is assumed that the click parameter type is a JsonParamType. The map is also assumed to be univariate.
+        """
+        if not value:
+            raise click.BadParameter("Expected non-empty dict")
+        if not isinstance(value, dict):
+            raise click.BadParameter(f"Expected json dict '{{...}}', parsed value is {type(value)}")
+        converter = FlyteLiteralConverter(
+            ctx,
+            self._flyte_ctx,
+            self._literal_type.map_value_type,
+            type(value[list(value.keys())[0]]),
+            self._create_upload_fn,
+        )
+        lt = Literal(map=LiteralMap({}))
+        for k, v in value.items():
+            click_val = converter._click_type.convert(v, param, ctx)
+            lt.map.literals[k] = converter.convert_to_literal(ctx, param, click_val)
+        return lt
+
+    def convert_to_struct(
+        self,
+        ctx: typing.Optional[click.Context],
+        param: typing.Optional[click.Parameter],
+        value: typing.Union[dict, typing.Any],
+    ) -> Literal:
+        """
+        Convert the loaded json object to a Flyte Literal struct type.
+        """
+        if type(value) != self._python_type:
+            o = cast(DataClassJsonMixin, self._python_type).from_json(json.dumps(value))
+        else:
+            o = value
+        return TypeEngine.to_literal(self._flyte_ctx, o, self._python_type, self._literal_type)
+
     def convert_to_literal(
         self, ctx: typing.Optional[click.Context], param: typing.Optional[click.Parameter], value: typing.Any
     ) -> Literal:
         if self._literal_type.structured_dataset_type:
             return self.convert_to_structured_dataset(ctx, param, value)
 
         if self._literal_type.blob:
             return self.convert_to_blob(ctx, param, value)
 
         if self._literal_type.collection_type:
-            python_value = json.loads(value) if isinstance(value, str) else value
-            if not isinstance(python_value, list):
-                raise click.BadParameter(f"Expected json list '[...]', parsed value is {type(python_value)}")
-            converter = FlyteLiteralConverter(
-                ctx,
-                self._flyte_ctx,
-                self._literal_type.collection_type,
-                type(python_value[0]),
-                self._create_upload_fn,
-            )
-            lt = Literal(collection=LiteralCollection([]))
-            for v in python_value:
-                click_val = converter._click_type.convert(v, param, ctx)
-                lt.collection.literals.append(converter.convert_to_literal(ctx, param, click_val))
-            return lt
+            return self.convert_to_list(ctx, param, value)
+
         if self._literal_type.map_value_type:
-            python_value = json.loads(value) if isinstance(value, str) else value
-            if not isinstance(python_value, dict):
-                raise click.BadParameter("Expected json map '{}', parsed value is {%s}" % type(python_value))
-            converter = FlyteLiteralConverter(
-                ctx,
-                self._flyte_ctx,
-                self._literal_type.map_value_type,
-                type(python_value[next(iter(python_value))]),
-                self._create_upload_fn,
-            )
-            lt = Literal(map=LiteralMap({}))
-            for k, v in python_value.items():
-                click_val = converter._click_type.convert(v, param, ctx)
-                lt.map.literals[k] = converter.convert_to_literal(ctx, param, click_val)
-            return lt
+            return self.convert_to_map(ctx, param, value)
 
         if self._literal_type.union_type:
             return self.convert_to_union(ctx, param, value)
 
         if self._literal_type.simple or self._literal_type.enum_type:
             if self._literal_type.simple and self._literal_type.simple == SimpleType.STRUCT:
-                if self._python_type == dict:
-                    if type(value) != str:
-                        # The type of default value is dict, so we have to convert it to json string
-                        value = json.dumps(value)
-                    o = json.loads(value)
-                elif type(value) != self._python_type:
-                    o = cast(DataClassJsonMixin, self._python_type).from_json(value)
-                else:
-                    o = value
-                return TypeEngine.to_literal(self._flyte_ctx, o, self._python_type, self._literal_type)
+                return self.convert_to_struct(ctx, param, value)
             return Literal(scalar=self._converter.convert(value, self._python_type))
 
         if self._literal_type.schema:
             raise DeprecationWarning("Schema Types are not supported in pyflyte run. Use StructuredDataset instead.")
 
         raise NotImplementedError(
             f"CLI parsing is not available for Python Type:`{self._python_type}`, LiteralType:`{self._literal_type}`."
         )
 
     def convert(self, ctx, param, value) -> typing.Union[Literal, typing.Any]:
-        lit = self.convert_to_literal(ctx, param, value)
-        if not self._remote:
-            return TypeEngine.to_python_value(self._flyte_ctx, lit, self._python_type)
-        return lit
+        try:
+            lit = self.convert_to_literal(ctx, param, value)
+            if not self._remote:
+                return TypeEngine.to_python_value(self._flyte_ctx, lit, self._python_type)
+            return lit
+        except click.BadParameter:
+            raise
+        except Exception as e:
+            raise click.BadParameter(f"Failed to convert param {param}, {value} to {self._python_type}") from e
 
 
 def to_click_option(
     ctx: click.Context,
     flyte_ctx: FlyteContext,
     input_name: str,
     literal_var: Variable,
@@ -388,14 +443,21 @@
     literal_converter = FlyteLiteralConverter(
         ctx, flyte_ctx, literal_type=literal_var.type, python_type=python_type, get_upload_url_fn=get_upload_url_fn
     )
 
     if literal_converter.is_bool() and not default_val:
         default_val = False
 
+    if literal_var.type.simple == SimpleType.STRUCT:
+        if default_val:
+            if type(default_val) == dict or type(default_val) == list:
+                default_val = json.dumps(default_val)
+            else:
+                default_val = cast(DataClassJsonMixin, default_val).to_json()
+
     return click.Option(
         param_decls=[f"--{input_name}"],
         type=literal_converter.click_type,
         is_flag=literal_converter.is_bool(),
         default=default_val,
         show_default=True,
         required=default_val is None,
@@ -606,15 +668,15 @@
 
         if run_level_params.get("dump_snippet"):
             dump_flyte_remote_snippet(execution, project, domain)
 
     return _run
 
 
-class WorkflowCommand(click.MultiCommand):
+class WorkflowCommand(click.RichGroup):
     """
     click multicommand at the python file layer, subcommands should be all the workflows in the file.
     """
 
     def __init__(self, filename: str, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._filename = pathlib.Path(filename).resolve()
@@ -674,15 +736,15 @@
             params=params,
             callback=run_command(ctx, entity),
             help=f"Run {module}.{exe_entity} in script mode",
         )
         return cmd
 
 
-class RunCommand(click.MultiCommand):
+class RunCommand(click.RichGroup):
     """
     A click command group for registering and executing flyte workflows & tasks in a file.
     """
 
     def __init__(self, *args, **kwargs):
         params = get_workflow_command_base_params()
         super().__init__(*args, params=params, **kwargs)
```

### Comparing `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.6.0b1/flytekit/clis/sdk_in_container/serialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 import typing
 from enum import Enum as _Enum
 
-import click
+import rich_click as click
 
 from flytekit.clis.sdk_in_container import constants
 from flytekit.clis.sdk_in_container.constants import CTX_PACKAGES
 from flytekit.configuration import FastSerializationSettings, ImageConfig, SerializationSettings
 from flytekit.exceptions.scopes import system_entry_point
 from flytekit.tools.fast_registration import fast_package
 from flytekit.tools.repo import serialize_to_folder
@@ -65,15 +65,15 @@
         flytekit_virtualenv_root=flytekit_virtualenv_root,
         python_interpreter=python_interpreter,
     )
 
     serialize_to_folder(pkgs, serialization_settings, local_source_root, folder)
 
 
-@click.group("serialize")
+@click.group("serialize", cls=click.RichGroup)
 @click.option(
     "--image",
     required=False,
     default=lambda: os.environ.get("FLYTE_INTERNAL_IMAGE", ""),
     help="Text tag, for example ``somedocker.com/myimage:someversion123``",
 )
 @click.option(
@@ -120,15 +120,15 @@
         import flytekit
 
         flytekit_install_loc = os.path.abspath(flytekit.__file__)
         ctx.obj[CTX_FLYTEKIT_VIRTUALENV_ROOT] = os.path.dirname(flytekit_install_loc)
         ctx.obj[CTX_PYTHON_INTERPRETER] = sys.executable
 
 
-@click.command("workflows")
+@click.command("workflows", cls=click.RichCommand)
 # For now let's just assume that the directory needs to exist. If you're docker run -v'ing, docker will create the
 # directory for you so it shouldn't be a problem.
 @click.option("-f", "--folder", type=click.Path(exists=True))
 @click.pass_context
 def workflows(ctx, folder=None):
 
     if folder:
@@ -144,21 +144,21 @@
         image=ctx.obj[CTX_IMAGE],
         flytekit_virtualenv_root=ctx.obj[CTX_FLYTEKIT_VIRTUALENV_ROOT],
         python_interpreter=ctx.obj[CTX_PYTHON_INTERPRETER],
         config_file=ctx.obj.get(constants.CTX_CONFIG_FILE, None),
     )
 
 
-@click.group("fast")
+@click.group("fast", cls=click.RichGroup)
 @click.pass_context
 def fast(ctx):
     pass
 
 
-@click.command("workflows")
+@click.command("workflows", cls=click.RichCommand)
 @click.option(
     "--deref-symlinks",
     default=False,
     is_flag=True,
     help="Enables symlink dereferencing when packaging files in fast registration",
 )
 @click.option("-f", "--folder", type=click.Path(exists=True))
```

### Comparing `flytekit-1.6.0b0/flytekit/configuration/__init__.py` & `flytekit-1.6.0b1/flytekit/configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -791,14 +791,15 @@
             version=self.version,
             image_config=self.image_config,
             env=self.env.copy() if self.env else None,
             git_repo=self.git_repo,
             flytekit_virtualenv_root=self.flytekit_virtualenv_root,
             python_interpreter=self.python_interpreter,
             fast_serialization_settings=self.fast_serialization_settings,
+            source_root=self.source_root,
         )
 
     def should_fast_serialize(self) -> bool:
         """
         Whether or not the serialization settings specify that entities should be serialized for fast registration.
         """
         return self.fast_serialization_settings is not None and self.fast_serialization_settings.enabled
@@ -841,14 +842,15 @@
         version: str
         image_config: ImageConfig
         env: Optional[Dict[str, str]] = None
         git_repo: Optional[str] = None
         flytekit_virtualenv_root: Optional[str] = None
         python_interpreter: Optional[str] = None
         fast_serialization_settings: Optional[FastSerializationSettings] = None
+        source_root: Optional[str] = None
 
         def with_fast_serialization_settings(self, fss: fast_serialization_settings) -> SerializationSettings.Builder:
             self.fast_serialization_settings = fss
             return self
 
         def build(self) -> SerializationSettings:
             return SerializationSettings(
@@ -857,8 +859,9 @@
                 version=self.version,
                 image_config=self.image_config,
                 env=self.env,
                 git_repo=self.git_repo,
                 flytekit_virtualenv_root=self.flytekit_virtualenv_root,
                 python_interpreter=self.python_interpreter,
                 fast_serialization_settings=self.fast_serialization_settings,
+                source_root=self.source_root,
             )
```

### Comparing `flytekit-1.6.0b0/flytekit/configuration/default_images.py` & `flytekit-1.6.0b1/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/configuration/feature_flags.py` & `flytekit-1.6.0b1/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/configuration/file.py` & `flytekit-1.6.0b1/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/configuration/internal.py` & `flytekit-1.6.0b1/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/annotation.py` & `flytekit-1.6.0b1/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/base_sql_task.py` & `flytekit-1.6.0b1/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/base_task.py` & `flytekit-1.6.0b1/flytekit/core/base_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     create_task_output,
     extract_obj_name,
     flyte_entity_call_handler,
     translate_inputs_to_literals,
 )
 from flytekit.core.tracker import TrackedInstance
 from flytekit.core.type_engine import TypeEngine, TypeTransformerFailedError
+from flytekit.core.utils import timeit
 from flytekit.deck.deck import Deck
 from flytekit.loggers import logger
 from flytekit.models import dynamic_job as _dynamic_job
 from flytekit.models import interface as _interface_models
 from flytekit.models import literals as _literal_models
 from flytekit.models import task as _task_model
 from flytekit.models.core import workflow as _workflow_model
@@ -529,15 +530,16 @@
                 logger.error(msg)
                 raise type(exc)(msg) from exc
 
             # TODO: Logger should auto inject the current context information to indicate if the task is running within
             #   a workflow or a subworkflow etc
             logger.info(f"Invoking {self.name} with inputs: {native_inputs}")
             try:
-                native_outputs = self.execute(**native_inputs)
+                with timeit("Execute user level code"):
+                    native_outputs = self.execute(**native_inputs)
             except Exception as e:
                 logger.exception(f"Exception when executing {e}")
                 raise e
 
             logger.debug("Task executed successfully in user level")
             # Lets run the post_execute method. This may result in a IgnoreOutputs Exception, which is
             # bubbled up to be handled at the callee layer.
@@ -566,29 +568,30 @@
             else:
                 native_outputs_as_map = {
                     expected_output_names[i]: native_outputs[i] for i, _ in enumerate(native_outputs)
                 }
 
             # We manually construct a LiteralMap here because task inputs and outputs actually violate the assumption
             # built into the IDL that all the values of a literal map are of the same type.
-            literals = {}
-            for i, (k, v) in enumerate(native_outputs_as_map.items()):
-                literal_type = self._outputs_interface[k].type
-                py_type = self.get_type_for_output_var(k, v)
-
-                if isinstance(v, tuple):
-                    raise TypeError(f"Output({k}) in task '{self.name}' received a tuple {v}, instead of {py_type}")
-                try:
-                    literals[k] = TypeEngine.to_literal(exec_ctx, v, py_type, literal_type)
-                except Exception as e:
-                    # only show the name of output key if it's user-defined (by default Flyte names these as "o<n>")
-                    key = k if k != f"o{i}" else i
-                    msg = f"Failed to convert outputs of task '{self.name}' at position {key}:\n  {e}"
-                    logger.error(msg)
-                    raise TypeError(msg) from e
+            with timeit("Translate the output to literals"):
+                literals = {}
+                for i, (k, v) in enumerate(native_outputs_as_map.items()):
+                    literal_type = self._outputs_interface[k].type
+                    py_type = self.get_type_for_output_var(k, v)
+
+                    if isinstance(v, tuple):
+                        raise TypeError(f"Output({k}) in task '{self.name}' received a tuple {v}, instead of {py_type}")
+                    try:
+                        literals[k] = TypeEngine.to_literal(exec_ctx, v, py_type, literal_type)
+                    except Exception as e:
+                        # only show the name of output key if it's user-defined (by default Flyte names these as "o<n>")
+                        key = k if k != f"o{i}" else i
+                        msg = f"Failed to convert outputs of task '{self.name}' at position {key}:\n  {e}"
+                        logger.error(msg)
+                        raise TypeError(msg) from e
 
             if self._disable_deck is False:
                 INPUT = "input"
                 OUTPUT = "output"
 
                 input_deck = Deck(INPUT)
                 for k, v in native_inputs.items():
```

### Comparing `flytekit-1.6.0b0/flytekit/core/checkpointer.py` & `flytekit-1.6.0b1/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/class_based_resolver.py` & `flytekit-1.6.0b1/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/condition.py` & `flytekit-1.6.0b1/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/constants.py` & `flytekit-1.6.0b1/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/container_task.py` & `flytekit-1.6.0b1/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/context_manager.py` & `flytekit-1.6.0b1/flytekit/core/context_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,28 @@
 
     @property
     def default_deck(self) -> Deck:
         from flytekit.deck.deck import Deck
 
         return Deck("default")
 
+    @property
+    def timeline_deck(self) -> "TimeLineDeck":  # type: ignore
+        from flytekit.deck.deck import TimeLineDeck
+
+        time_line_deck = None
+        for deck in self.decks:
+            if isinstance(deck, TimeLineDeck):
+                time_line_deck = deck
+                break
+        if time_line_deck is None:
+            time_line_deck = TimeLineDeck("Timeline")
+
+        return time_line_deck
+
     def __getattr__(self, attr_name: str) -> typing.Any:
         """
         This houses certain task specific context. For example in Spark, it houses the SparkSession, etc
         """
         attr_name = attr_name.upper()
         if self._attrs and attr_name in self._attrs:
             return self._attrs[attr_name]
@@ -721,15 +735,15 @@
 
 
 class FlyteContextManager(object):
     """
     FlyteContextManager manages the execution context within Flytekit. It holds global state of either compilation
     or Execution. It is not thread-safe and can only be run as a single threaded application currently.
     Context's within Flytekit is useful to manage compilation state and execution state. Refer to ``CompilationState``
-    and ``ExecutionState`` for for information. FlyteContextManager provides a singleton stack to manage these contexts.
+    and ``ExecutionState`` for more information. FlyteContextManager provides a singleton stack to manage these contexts.
 
     Typical usage is
 
     .. code-block:: python
 
         FlyteContextManager.initialize()
         with FlyteContextManager.with_context(o) as ctx:
```

### Comparing `flytekit-1.6.0b0/flytekit/core/data_persistence.py` & `flytekit-1.6.0b1/flytekit/core/data_persistence.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from uuid import UUID
 
 import fsspec
 from fsspec.utils import get_protocol
 
 from flytekit import configuration
 from flytekit.configuration import DataConfig
-from flytekit.core.utils import PerformanceTimer
+from flytekit.core.utils import timeit
 from flytekit.exceptions.user import FlyteAssertion
 from flytekit.interfaces.random import random
 from flytekit.loggers import logger
 
 # Refer to https://github.com/fsspec/s3fs/blob/50bafe4d8766c3b2a4e1fc09669cf02fb2d71454/s3fs/core.py#L198
 # for key and secret
 _FSSPEC_S3_KEY_ID = "key"
@@ -287,43 +287,44 @@
     def upload_directory(self, local_path: str, remote_path: str):
         """
         :param Text local_path:
         :param Text remote_path:
         """
         return self.put_data(local_path, remote_path, is_multipart=True)
 
+    @timeit("Download data to local from remote")
     def get_data(self, remote_path: str, local_path: str, is_multipart: bool = False):
         """
         :param remote_path:
         :param local_path:
         :param is_multipart:
         """
         try:
-            with PerformanceTimer(f"Copying ({remote_path} -> {local_path})"):
-                pathlib.Path(local_path).parent.mkdir(parents=True, exist_ok=True)
-                self.get(remote_path, to_path=local_path, recursive=is_multipart)
+            pathlib.Path(local_path).parent.mkdir(parents=True, exist_ok=True)
+            self.get(remote_path, to_path=local_path, recursive=is_multipart)
         except Exception as ex:
             raise FlyteAssertion(
                 f"Failed to get data from {remote_path} to {local_path} (recursive={is_multipart}).\n\n"
                 f"Original exception: {str(ex)}"
             )
 
+    @timeit("Upload data to remote")
     def put_data(self, local_path: Union[str, os.PathLike], remote_path: str, is_multipart: bool = False):
         """
         The implication here is that we're always going to put data to the remote location, so we .remote to ensure
         we don't use the true local proxy if the remote path is a file://
 
         :param local_path:
         :param remote_path:
         :param is_multipart:
         """
         try:
             local_path = str(local_path)
-            with PerformanceTimer(f"Writing ({local_path} -> {remote_path})"):
-                self.put(cast(str, local_path), remote_path, recursive=is_multipart)
+
+            self.put(cast(str, local_path), remote_path, recursive=is_multipart)
         except Exception as ex:
             raise FlyteAssertion(
                 f"Failed to put data from {local_path} to {remote_path} (recursive={is_multipart}).\n\n"
                 f"Original exception: {str(ex)}"
             ) from ex
```

### Comparing `flytekit-1.6.0b0/flytekit/core/docstring.py` & `flytekit-1.6.0b1/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.6.0b1/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/gate.py` & `flytekit-1.6.0b1/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/interface.py` & `flytekit-1.6.0b1/flytekit/core/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/launch_plan.py` & `flytekit-1.6.0b1/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/local_cache.py` & `flytekit-1.6.0b1/flytekit/core/local_cache.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/map_task.py` & `flytekit-1.6.0b1/flytekit/core/map_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from flytekit.core import tracker
 from flytekit.core.base_task import PythonTask, Task, TaskResolverMixin
 from flytekit.core.constants import SdkTaskType
 from flytekit.core.context_manager import ExecutionState, FlyteContext, FlyteContextManager
 from flytekit.core.interface import transform_interface_to_list_interface
 from flytekit.core.python_function_task import PythonFunctionTask
 from flytekit.core.tracker import TrackedInstance
+from flytekit.core.utils import timeit
 from flytekit.exceptions import scopes as exception_scopes
 from flytekit.models.array_job import ArrayJob
 from flytekit.models.interface import Variable
 from flytekit.models.task import Container, K8sPod, Sql
 from flytekit.tools.module_loader import load_object_from_module
 
 
@@ -352,14 +353,15 @@
     But, at runtime this information is lost. To reconstruct this, we use MapTaskResolver that records the "bound vars"
     and then at runtime reconstructs the interface with this knowledge
     """
 
     def name(self) -> str:
         return "MapTaskResolver"
 
+    @timeit("Load map task")
     def load_task(self, loader_args: List[str], max_concurrency: int = 0) -> MapPythonTask:
         """
         Loader args should be of the form
         vars "var1,var2,.." resolver "resolver" [resolver_args]
         """
         _, bound_vars, _, resolver, *resolver_args = loader_args
         logging.info(f"MapTask found task resolver {resolver} and arguments {resolver_args}")
```

### Comparing `flytekit-1.6.0b0/flytekit/core/mock_stats.py` & `flytekit-1.6.0b1/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/node.py` & `flytekit-1.6.0b1/flytekit/core/node.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/node_creation.py` & `flytekit-1.6.0b1/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/notification.py` & `flytekit-1.6.0b1/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/pod_template.py` & `flytekit-1.6.0b1/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/promise.py` & `flytekit-1.6.0b1/flytekit/core/promise.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/python_auto_container.py` & `flytekit-1.6.0b1/flytekit/core/python_auto_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from flytekit.configuration import ImageConfig, SerializationSettings
 from flytekit.core.base_task import PythonTask, TaskMetadata, TaskResolverMixin
 from flytekit.core.context_manager import FlyteContextManager
 from flytekit.core.pod_template import PodTemplate
 from flytekit.core.resources import Resources, ResourceSpec
 from flytekit.core.tracked_abc import FlyteTrackedABC
 from flytekit.core.tracker import TrackedInstance, extract_task_module
-from flytekit.core.utils import _get_container_definition, _serialize_pod_spec
+from flytekit.core.utils import _get_container_definition, _serialize_pod_spec, timeit
 from flytekit.image_spec.image_spec import ImageBuildEngine, ImageSpec
 from flytekit.loggers import logger
 from flytekit.models import task as _task_model
 from flytekit.models.security import Secret, SecurityContext
 
 T = TypeVar("T")
 _PRIMARY_CONTAINER_NAME_FIELD = "primary_container_name"
@@ -177,16 +177,17 @@
             return self._get_container(settings)
 
     def _get_container(self, settings: SerializationSettings) -> _task_model.Container:
         env = {}
         for elem in (settings.env, self.environment):
             if elem:
                 env.update(elem)
-        if isinstance(self.container_image, ImageSpec):
-            self.container_image.source_root = settings.source_root
+        if settings.fast_serialization_settings is None or not settings.fast_serialization_settings.enabled:
+            if isinstance(self.container_image, ImageSpec):
+                self.container_image.source_root = settings.source_root
         return _get_container_definition(
             image=get_registerable_container_image(self.container_image, settings.image_config),
             command=[],
             args=self.get_command(settings=settings),
             data_loading_config=None,
             environment=env,
             storage_request=self.resources.requests.storage,
@@ -223,14 +224,15 @@
     """
     Please see the notes in the TaskResolverMixin as it describes this default behavior.
     """
 
     def name(self) -> str:
         return "DefaultTaskResolver"
 
+    @timeit("Load task")
     def load_task(self, loader_args: List[str]) -> PythonAutoContainerTask:
         _, task_module, _, task_name, *_ = loader_args
 
         task_module = importlib.import_module(name=task_module)  # type: ignore
         task_def = getattr(task_module, task_name)
         return task_def
```

### Comparing `flytekit-1.6.0b0/flytekit/core/python_customized_container_task.py` & `flytekit-1.6.0b1/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/python_function_task.py` & `flytekit-1.6.0b1/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/reference.py` & `flytekit-1.6.0b1/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/reference_entity.py` & `flytekit-1.6.0b1/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/resources.py` & `flytekit-1.6.0b1/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/schedule.py` & `flytekit-1.6.0b1/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/shim_task.py` & `flytekit-1.6.0b1/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/task.py` & `flytekit-1.6.0b1/flytekit/core/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/testing.py` & `flytekit-1.6.0b1/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/tracker.py` & `flytekit-1.6.0b1/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/type_engine.py` & `flytekit-1.6.0b1/flytekit/core/type_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from marshmallow_jsonschema import JSONSchema
 from typing_extensions import Annotated, get_args, get_origin
 
 from flytekit.core.annotation import FlyteAnnotation
 from flytekit.core.context_manager import FlyteContext
 from flytekit.core.hash import HashMethod
 from flytekit.core.type_helpers import load_type_from_tag
+from flytekit.core.utils import timeit
 from flytekit.exceptions import user as user_exceptions
 from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
 from flytekit.models import types as _type_models
 from flytekit.models.annotation import TypeAnnotation as TypeAnnotationModel
 from flytekit.models.core import types as _core_types
 from flytekit.models.literals import (
@@ -829,15 +830,15 @@
         """
         Converts a Literal value with an expected python type into a python value.
         """
         transformer = cls.get_transformer(expected_python_type)
         return transformer.to_python_value(ctx, lv, expected_python_type)
 
     @classmethod
-    def to_html(cls, ctx: FlyteContext, python_val: typing.Any, expected_python_type: Type[T]) -> str:
+    def to_html(cls, ctx: FlyteContext, python_val: typing.Any, expected_python_type: Type[typing.Any]) -> str:
         transformer = cls.get_transformer(expected_python_type)
         if get_origin(expected_python_type) is Annotated:
             expected_python_type, *annotate_args = get_args(expected_python_type)
             from flytekit.deck.renderer import Renderable
 
             for arg in annotate_args:
                 if isinstance(arg, Renderable):
@@ -852,14 +853,15 @@
         variables = {}
         for idx, (var_name, var_type) in enumerate(t.__annotations__.items()):
             literal_type = cls.to_literal_type(var_type)
             variables[var_name] = _interface_models.Variable(type=literal_type, description=f"{idx}")
         return _interface_models.VariableMap(variables=variables)
 
     @classmethod
+    @timeit("Translate literal to python value")
     def literal_map_to_kwargs(
         cls, ctx: FlyteContext, lm: LiteralMap, python_types: typing.Dict[str, type]
     ) -> typing.Dict[str, typing.Any]:
         """
         Given a ``LiteralMap`` (usually an input into a task - intermediate), convert to kwargs for the task
         """
         if len(lm.literals) > len(python_types):
@@ -995,22 +997,25 @@
     def to_literal(self, ctx: FlyteContext, python_val: T, python_type: Type[T], expected: LiteralType) -> Literal:
         if type(python_val) != list:
             raise TypeTransformerFailedError("Expected a list")
 
         if ListTransformer.is_batchable(python_type):
             from flytekit.types.pickle.pickle import BatchSize, FlytePickle
 
-            batchSize = len(python_val)  # default batch size
+            batch_size = len(python_val)  # default batch size
             # parse annotated to get the number of items saved in a pickle file.
             if get_origin(python_type) is Annotated:
                 for annotation in get_args(python_type)[1:]:
                     if isinstance(annotation, BatchSize):
-                        batchSize = annotation.val
+                        batch_size = annotation.val
                         break
-            lit_list = [TypeEngine.to_literal(ctx, python_val[i : i + batchSize], FlytePickle, expected.collection_type) for i in range(0, len(python_val), batchSize)]  # type: ignore
+            if batch_size > 0:
+                lit_list = [TypeEngine.to_literal(ctx, python_val[i : i + batch_size], FlytePickle, expected.collection_type) for i in range(0, len(python_val), batch_size)]  # type: ignore
+            else:
+                lit_list = []
         else:
             t = self.get_sub_type(python_type)
             lit_list = [TypeEngine.to_literal(ctx, x, t, expected.collection_type) for x in python_val]  # type: ignore
         return Literal(collection=LiteralCollection(literals=lit_list))
 
     def to_python_value(self, ctx: FlyteContext, lv: Literal, expected_python_type: Type[T]) -> typing.List[typing.Any]:  # type: ignore
         try:
```

### Comparing `flytekit-1.6.0b0/flytekit/core/type_helpers.py` & `flytekit-1.6.0b1/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/core/utils.py` & `flytekit-1.6.0b1/flytekit/core/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import datetime
 import os as _os
 import shutil as _shutil
 import tempfile as _tempfile
 import time as _time
+from functools import wraps
 from hashlib import sha224 as _sha224
 from pathlib import Path
-from typing import Any, Dict, List, Optional, cast
+from typing import Any, Callable, Dict, List, Optional, cast
 
 from flyteidl.core import tasks_pb2 as _core_task
 from kubernetes.client import ApiClient
 from kubernetes.client.models import V1Container, V1EnvVar, V1ResourceRequirements
 
 from flytekit.core.pod_template import PodTemplate
 from flytekit.loggers import logger
@@ -255,31 +257,71 @@
     def __repr__(self):
         return "Auto-Deleting Tmp Directory @ {}".format(self.name)
 
     def __str__(self):
         return self.__repr__()
 
 
-class PerformanceTimer(object):
-    def __init__(self, context_statement):
+class timeit:
+    """
+    A context manager and a decorator that measures the execution time of the wrapped code block or functions.
+    It will append a timing information to TimeLineDeck. For instance:
+
+    @timeit("Function description")
+    def function()
+
+    with timeit("Wrapped code block description"):
+        # your code
+    """
+
+    def __init__(self, name: str = ""):
         """
-        :param Text context_statement: the statement to log
+        :param name: A string that describes the wrapped code block or function being executed.
         """
-        self._context_statement = context_statement
+        self._name = name
+        self.start_time = None
         self._start_wall_time = None
         self._start_process_time = None
 
+    def __call__(self, func: Callable):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            with self:
+                return func(*args, **kwargs)
+
+        return wrapper
+
     def __enter__(self):
-        logger.info("Entering timed context: {}".format(self._context_statement))
+        self.start_time = datetime.datetime.utcnow()
         self._start_wall_time = _time.perf_counter()
         self._start_process_time = _time.process_time()
+        return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+        """
+        The exception, if any, will propagate outside the context manager, as the purpose of this context manager
+        is solely to measure the execution time of the wrapped code block.
+        """
+        from flytekit.core.context_manager import FlyteContextManager
+
+        end_time = datetime.datetime.utcnow()
         end_wall_time = _time.perf_counter()
         end_process_time = _time.process_time()
+
+        timeline_deck = FlyteContextManager.current_context().user_space_params.timeline_deck
+        timeline_deck.append_time_info(
+            dict(
+                Name=self._name,
+                Start=self.start_time,
+                Finish=end_time,
+                WallTime=end_wall_time - self._start_wall_time,
+                ProcessTime=end_process_time - self._start_process_time,
+            )
+        )
+
         logger.info(
-            "Exiting timed context: {} [Wall Time: {}s, Process Time: {}s]".format(
-                self._context_statement,
+            "{}. [Wall Time: {}s, Process Time: {}s]".format(
+                self._name,
                 end_wall_time - self._start_wall_time,
                 end_process_time - self._start_process_time,
             )
         )
```

### Comparing `flytekit-1.6.0b0/flytekit/core/workflow.py` & `flytekit-1.6.0b1/flytekit/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/deck/html/template.html` & `flytekit-1.6.0b1/flytekit/deck/html/template.html`

 * *Files 1% similar despite different names*

```diff
@@ -49,25 +49,27 @@
 
         #flyte-frame-tabs li.active {
             border-bottom: 4px solid rgb(163, 26, 255);
             color: #333333;
         }
 
         #flyte-frame-container {
-            width: 100%;
+            width: auto;
         }
 
         #flyte-frame-container > div {
-            display: none;
+            display: None;
         }
 
         #flyte-frame-container > div.active {
-            display: block;
+            display: Block;
             padding: 2rem 4rem;
+            width: 100%;
         }
+
     </style>
 
 </head>
 <body>
     <!---{#% autoescape true %#}--->
     <nav id="flyte-frame-nav">
         <ul id="flyte-frame-tabs">
```

### Comparing `flytekit-1.6.0b0/flytekit/deck/renderer.py` & `flytekit-1.6.0b1/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/exceptions/scopes.py` & `flytekit-1.6.0b1/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/exceptions/system.py` & `flytekit-1.6.0b1/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/exceptions/user.py` & `flytekit-1.6.0b1/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/extend/__init__.py` & `flytekit-1.6.0b1/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.6.0b1/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/extras/pytorch/__init__.py` & `flytekit-1.6.0b1/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.6.0b1/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/extras/pytorch/native.py` & `flytekit-1.6.0b1/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/extras/sklearn/__init__.py` & `flytekit-1.6.0b1/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/extras/sklearn/native.py` & `flytekit-1.6.0b1/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/extras/sqlite3/task.py` & `flytekit-1.6.0b1/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/extras/tasks/shell.py` & `flytekit-1.6.0b1/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.6.0b1/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/extras/tensorflow/model.py` & `flytekit-1.6.0b1/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/extras/tensorflow/record.py` & `flytekit-1.6.0b1/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/image_spec/image_spec.py` & `flytekit-1.6.0b1/flytekit/image_spec/image_spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import base64
 import hashlib
 import os
 import sys
 import typing
 from abc import abstractmethod
+from copy import copy
 from dataclasses import dataclass
 from functools import lru_cache
 from typing import List, Optional
 
 import click
 import docker
+import requests
 from dataclasses_json import dataclass_json
 from docker.errors import APIError, ImageNotFound
 
+DOCKER_HUB = "docker.io"
+_F_IMG_ID = "_F_IMG_ID"
+
 
 @dataclass_json
 @dataclass
 class ImageSpec:
     """
     This class is used to specify the docker image that will be used to run the task.
 
     Args:
         name: name of the image.
         python_version: python version of the image.
+        builder: Type of plugin to build the image. Use envd by default.
         source_root: source root of the image.
         env: environment variables of the image.
-        destination_dir: destination directory of the image.
         registry: registry of the image.
         packages: list of python packages to install.
         apt_packages: list of apt packages to install.
         base_image: base image of the image.
     """
 
     name: str = "flytekit"
@@ -48,34 +53,54 @@
         """
         tag = calculate_hash_from_image_spec(self)
         container_image = f"{self.name}:{tag}"
         if self.registry:
             container_image = f"{self.registry}/{container_image}"
         return container_image
 
+    def is_container(self) -> bool:
+        from flytekit.core.context_manager import ExecutionState, FlyteContextManager
+
+        state = FlyteContextManager.current_context().execution_state
+        if state and state.mode and state.mode != ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION:
+            return os.environ.get(_F_IMG_ID) == self.image_name()
+        return True
+
+    @lru_cache
     def exist(self) -> bool:
         """
         Check if the image exists in the registry.
         """
-        client = docker.from_env()
         try:
+            client = docker.from_env()
             if self.registry:
                 client.images.get_registry_data(self.image_name())
             else:
                 client.images.get(self.image_name())
             return True
         except APIError as e:
             if e.response.status_code == 404:
                 return False
-            if e.response.status_code == 403:
-                click.secho("Permission denied. Please login you docker registry first.", fg="red")
-                raise e
-            return False
         except ImageNotFound:
             return False
+        except Exception as e:
+            tag = calculate_hash_from_image_spec(self)
+            # if docker engine is not running locally
+            container_registry = DOCKER_HUB
+            if "/" in self.registry:
+                container_registry = self.registry.split("/")[0]
+            if container_registry == DOCKER_HUB:
+                url = f"https://hub.docker.com/v2/repositories/{self.registry}/{self.name}/tags/{tag}"
+                response = requests.get(url)
+                if response.status_code == 200:
+                    return True
+
+            click.secho(f"Failed to check if the image exists with error : {e}", fg="red")
+            click.secho("Flytekit assumes that the image already exists.", fg="blue")
+            return True
 
     def __hash__(self):
         return hash(self.to_json())
 
 
 class ImageSpecBuilder:
     @abstractmethod
@@ -107,23 +132,24 @@
         if not image_spec.exist():
             click.secho(f"Image {image_spec.image_name()} not found. Building...", fg="blue")
             cls._REGISTRY[image_spec.builder].build_image(image_spec)
         else:
             click.secho(f"Image {image_spec.image_name()} found. Skip building.", fg="blue")
 
 
-@lru_cache(maxsize=None)
+@lru_cache
 def calculate_hash_from_image_spec(image_spec: ImageSpec):
     """
     Calculate the hash from the image spec.
     """
+    # copy the image spec to avoid modifying the original image spec. otherwise, the hash will be different.
+    spec = copy(image_spec)
+    spec.source_root = hash_directory(image_spec.source_root) if image_spec.source_root else b""
     image_spec_bytes = bytes(image_spec.to_json(), "utf-8")
-    source_root_bytes = hash_directory(image_spec.source_root) if image_spec.source_root else b""
-    h = hashlib.md5(image_spec_bytes + source_root_bytes)
-    tag = base64.urlsafe_b64encode(h.digest()).decode("ascii")
+    tag = base64.urlsafe_b64encode(hashlib.md5(image_spec_bytes).digest()).decode("ascii")
     # replace "=" with "." to make it a valid tag
     return tag.replace("=", ".")
 
 
 def hash_directory(path):
     """
     Return the SHA-256 hash of the directory at the given path.
```

### Comparing `flytekit-1.6.0b0/flytekit/interaction/parse_stdin.py` & `flytekit-1.6.0b1/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.6.0b1/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/interfaces/random.py` & `flytekit-1.6.0b1/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/interfaces/stats/client.py` & `flytekit-1.6.0b1/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/interfaces/stats/taggable.py` & `flytekit-1.6.0b1/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/loggers.py` & `flytekit-1.6.0b1/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/admin/common.py` & `flytekit-1.6.0b1/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/admin/task_execution.py` & `flytekit-1.6.0b1/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/admin/workflow.py` & `flytekit-1.6.0b1/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/annotation.py` & `flytekit-1.6.0b1/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/array_job.py` & `flytekit-1.6.0b1/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/common.py` & `flytekit-1.6.0b1/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/core/catalog.py` & `flytekit-1.6.0b1/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/core/compiler.py` & `flytekit-1.6.0b1/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/core/condition.py` & `flytekit-1.6.0b1/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/core/errors.py` & `flytekit-1.6.0b1/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/core/execution.py` & `flytekit-1.6.0b1/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/core/identifier.py` & `flytekit-1.6.0b1/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/core/types.py` & `flytekit-1.6.0b1/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/core/workflow.py` & `flytekit-1.6.0b1/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/documentation.py` & `flytekit-1.6.0b1/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/dynamic_job.py` & `flytekit-1.6.0b1/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/execution.py` & `flytekit-1.6.0b1/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/filters.py` & `flytekit-1.6.0b1/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/interface.py` & `flytekit-1.6.0b1/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/launch_plan.py` & `flytekit-1.6.0b1/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/literals.py` & `flytekit-1.6.0b1/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/matchable_resource.py` & `flytekit-1.6.0b1/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/named_entity.py` & `flytekit-1.6.0b1/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/node_execution.py` & `flytekit-1.6.0b1/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/presto.py` & `flytekit-1.6.0b1/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/project.py` & `flytekit-1.6.0b1/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/qubole.py` & `flytekit-1.6.0b1/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/schedule.py` & `flytekit-1.6.0b1/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/security.py` & `flytekit-1.6.0b1/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/task.py` & `flytekit-1.6.0b1/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/types.py` & `flytekit-1.6.0b1/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/models/workflow_closure.py` & `flytekit-1.6.0b1/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/remote/__init__.py` & `flytekit-1.6.0b1/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/remote/backfill.py` & `flytekit-1.6.0b1/flytekit/remote/backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,26 +64,31 @@
     if schedule.cron_schedule is not None:
         cron_schedule = schedule.cron_schedule
     else:
         raise NotImplementedError("Currently backfilling only supports cron schedules.")
 
     logging.info(f"Generating backfill from {start_date} -> {end_date}. Parallel?[{parallel}]")
     wf = ImperativeWorkflow(name=f"backfill-{for_lp.name}")
+
+    input_name = schedule.kickoff_time_input_arg
     date_iter = croniter(cron_schedule.schedule, start_time=start_date, ret_type=datetime)
     prev_node = None
     actual_start = None
     actual_end = None
     while True:
         next_start_date = date_iter.get_next()
         if not actual_start:
             actual_start = next_start_date
         if next_start_date >= end_date:
             break
         actual_end = next_start_date
-        next_node = wf.add_launch_plan(for_lp, t=next_start_date)
+        inputs = {}
+        if input_name:
+            inputs[input_name] = next_start_date
+        next_node = wf.add_launch_plan(for_lp, **inputs)
         next_node = next_node.with_overrides(
             name=f"b-{next_start_date}", retries=per_node_retries, timeout=per_node_timeout
         )
         if not parallel:
             if prev_node:
                 prev_node.runs_before(next_node)
         prev_node = next_node
```

### Comparing `flytekit-1.6.0b0/flytekit/remote/entities.py` & `flytekit-1.6.0b1/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/remote/executions.py` & `flytekit-1.6.0b1/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/remote/lazy_entity.py` & `flytekit-1.6.0b1/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/remote/remote.py` & `flytekit-1.6.0b1/flytekit/remote/remote.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/remote/remote_callable.py` & `flytekit-1.6.0b1/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/testing/__init__.py` & `flytekit-1.6.0b1/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/tools/fast_registration.py` & `flytekit-1.6.0b1/flytekit/tools/fast_registration.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import tarfile
 import tempfile
 from typing import Optional
 
 import click
 
 from flytekit.core.context_manager import FlyteContextManager
+from flytekit.core.utils import timeit
 from flytekit.tools.ignore import DockerIgnore, GitIgnore, IgnoreGroup, StandardIgnore
 from flytekit.tools.script_mode import tar_strip_file_attributes
 
 FAST_PREFIX = "fast"
 FAST_FILEENDING = ".tar.gz"
 
 
@@ -93,14 +94,15 @@
     :param Text remote_location:
     :param Text identifier:
     :return Text:
     """
     return posixpath.join(remote_location, "{}.{}".format(identifier, "tar.gz"))
 
 
+@timeit("Download distribution")
 def download_distribution(additional_distribution: str, destination: str):
     """
     Downloads a remote code distribution and overwrites any local files.
     :param Text additional_distribution:
     :param os.PathLike destination:
     """
     if not os.path.isdir(destination):
```

### Comparing `flytekit-1.6.0b0/flytekit/tools/ignore.py` & `flytekit-1.6.0b1/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/tools/module_loader.py` & `flytekit-1.6.0b1/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/tools/repo.py` & `flytekit-1.6.0b1/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/tools/script_mode.py` & `flytekit-1.6.0b1/flytekit/tools/script_mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import tarfile
 import tempfile
 import typing
 from pathlib import Path
 
 from flytekit import PythonFunctionTask
 from flytekit.core.tracker import get_full_module_path
-from flytekit.core.workflow import WorkflowBase
+from flytekit.core.workflow import ImperativeWorkflow, WorkflowBase
 
 
 def compress_scripts(source_path: str, destination: str, module_name: str):
     """
     Compresses the single script while maintaining the folder structure for that file.
 
     For example, given the follow file structure:
@@ -88,15 +88,19 @@
         script_file,
         script_file_destination,
     )
 
     # Try to copy other files to destination if tasks or workflows aren't in the same file
     for flyte_entity_name in mod.__dict__:
         flyte_entity = mod.__dict__[flyte_entity_name]
-        if isinstance(flyte_entity, (PythonFunctionTask, WorkflowBase)) and flyte_entity.instantiated_in:
+        if (
+            isinstance(flyte_entity, (PythonFunctionTask, WorkflowBase))
+            and not isinstance(flyte_entity, ImperativeWorkflow)
+            and flyte_entity.instantiated_in
+        ):
             copy_module_to_destination(
                 original_source_path, original_destination_path, flyte_entity.instantiated_in, visited
             )
 
 
 # Takes in a TarInfo and returns the modified TarInfo:
 # https://docs.python.org/3/library/tarfile.html#tarinfo-objects
```

### Comparing `flytekit-1.6.0b0/flytekit/tools/serialize_helpers.py` & `flytekit-1.6.0b1/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/tools/subprocess.py` & `flytekit-1.6.0b1/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/tools/translator.py` & `flytekit-1.6.0b1/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/types/directory/__init__.py` & `flytekit-1.6.0b1/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/types/directory/types.py` & `flytekit-1.6.0b1/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/types/file/__init__.py` & `flytekit-1.6.0b1/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/types/file/file.py` & `flytekit-1.6.0b1/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/types/numpy/ndarray.py` & `flytekit-1.6.0b1/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/types/pickle/pickle.py` & `flytekit-1.6.0b1/flytekit/types/pickle/pickle.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/types/schema/types.py` & `flytekit-1.6.0b1/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/types/schema/types_pandas.py` & `flytekit-1.6.0b1/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/types/structured/__init__.py` & `flytekit-1.6.0b1/flytekit/types/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/types/structured/basic_dfs.py` & `flytekit-1.6.0b1/flytekit/types/structured/basic_dfs.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/types/structured/bigquery.py` & `flytekit-1.6.0b1/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit/types/structured/structured_dataset.py` & `flytekit-1.6.0b1/flytekit/types/structured/structured_dataset.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit.egg-info/PKG-INFO` & `flytekit-1.6.0b1/flytekit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.0b0
+Version: 1.6.0b1
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b1 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.0b0/flytekit.egg-info/SOURCES.txt` & `flytekit-1.6.0b1/flytekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/flytekit.egg-info/requires.txt` & `flytekit-1.6.0b1/flytekit.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -37,10 +37,11 @@
 diskcache>=5.2.1
 cloudpickle>=2.0.0
 cookiecutter>=1.7.3
 numpy
 gitpython
 kubernetes>=12.0.1
 rich
+rich_click
 
 [:python_version < "3.8.0"]
 singledispatchmethod
```

### Comparing `flytekit-1.6.0b0/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.6.0b1/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b0/setup.py` & `flytekit-1.6.0b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.6.0b0"
+__version__ = "1.6.0b1"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
@@ -70,14 +70,15 @@
         "diskcache>=5.2.1",
         "cloudpickle>=2.0.0",
         "cookiecutter>=1.7.3",
         "numpy",
         "gitpython",
         "kubernetes>=12.0.1",
         "rich",
+        "rich_click",
     ],
     extras_require=extras_require,
     scripts=[
         "flytekit_scripts/flytekit_build_image.sh",
         "flytekit_scripts/flytekit_venv",
         "flytekit/bin/entrypoint.py",
     ],
```

