# Comparing `tmp/mosaicml-cli-0.4.0a4.tar.gz` & `tmp/mosaicml-cli-0.4.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.0a4.tar", last modified: Thu Apr 27 22:51:24 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.4.0a5.tar", last modified: Wed May  3 00:12:03 2023, max compression
```

## Comparing `mosaicml-cli-0.4.0a4.tar` & `mosaicml-cli-0.4.0a5.tar`

### file list

```diff
@@ -1,193 +1,195 @@
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.378729 mosaicml-cli-0.4.0a4/
--rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-27 22:51:24.378381 mosaicml-cli-0.4.0a4/PKG-INFO
--rw-r--r--   0 anna       (501) staff       (20)     7199 2023-04-27 22:42:06.000000 mosaicml-cli-0.4.0a4/README.md
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.333880 mosaicml-cli-0.4.0a4/mcli/
--rw-r--r--   0 anna       (501) staff       (20)       54 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.334604 mosaicml-cli-0.4.0a4/mcli/api/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.335406 mosaicml-cli-0.4.0a4/mcli/api/cluster/
--rw-r--r--   0 anna       (501) staff       (20)      134 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/cluster/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4141 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.336058 mosaicml-cli-0.4.0a4/mcli/api/engine/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/engine/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)    25914 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/engine/engine.py
--rw-r--r--   0 anna       (501) staff       (20)    10685 2023-04-27 22:33:58.000000 mosaicml-cli-0.4.0a4/mcli/api/exceptions.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.338595 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/
--rw-r--r--   0 anna       (501) staff       (20)     1023 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3421 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     3311 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     3586 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 anna       (501) staff       (20)     6111 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     1052 2023-04-27 22:33:58.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_ping_inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     1136 2023-04-27 22:33:58.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_predict_inference_deployment.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.339181 mosaicml-cli-0.4.0a4/mcli/api/mint/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/mint/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     7005 2023-04-27 22:33:58.000000 mosaicml-cli-0.4.0a4/mcli/api/mint/shell.py
--rw-r--r--   0 anna       (501) staff       (20)     2489 2023-04-27 22:33:58.000000 mosaicml-cli-0.4.0a4/mcli/api/mint/tty.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.340445 mosaicml-cli-0.4.0a4/mcli/api/model/
--rw-r--r--   0 anna       (501) staff       (20)     1114 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/api/model/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     5735 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/api/model/cluster_details.py
--rw-r--r--   0 anna       (501) staff       (20)     2987 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/api/model/inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)    10439 2023-04-27 22:42:24.000000 mosaicml-cli-0.4.0a4/mcli/api/model/run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.343528 mosaicml-cli-0.4.0a4/mcli/api/runs/
--rw-r--r--   0 anna       (501) staff       (20)     1199 2023-04-26 20:08:55.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2750 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_create_run.py
--rw-r--r--   0 anna       (501) staff       (20)     4143 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     8371 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 anna       (501) staff       (20)    10912 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     5141 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_start_run.py
--rw-r--r--   0 anna       (501) staff       (20)     5329 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     3937 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 anna       (501) staff       (20)    10619 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.343920 mosaicml-cli-0.4.0a4/mcli/api/schema/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/schema/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      636 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.345032 mosaicml-cli-0.4.0a4/mcli/api/secrets/
--rw-r--r--   0 anna       (501) staff       (20)      309 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/secrets/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2365 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 anna       (501) staff       (20)     2998 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     3697 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     2354 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/typing_future.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.345598 mosaicml-cli-0.4.0a4/mcli/api/users/
--rw-r--r--   0 anna       (501) staff       (20)      139 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/users/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2694 2023-04-27 22:33:37.000000 mosaicml-cli-0.4.0a4/mcli/api/users/api_get_users.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.346310 mosaicml-cli-0.4.0a4/mcli/cli/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/__init__.py
--rwxr-xr-x   0 anna       (501) staff       (20)     6436 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/cli/cli.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.347102 mosaicml-cli-0.4.0a4/mcli/cli/common/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/common/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2670 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 anna       (501) staff       (20)     7331 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.347528 mosaicml-cli-0.4.0a4/mcli/cli/m_connect/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1541 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.348347 mosaicml-cli-0.4.0a4/mcli/cli/m_create/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_create/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2385 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_create/m_create.py
--rw-r--r--   0 anna       (501) staff       (20)    16874 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.349324 mosaicml-cli-0.4.0a4/mcli/cli/m_delete/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6098 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_delete/delete.py
--rw-r--r--   0 anna       (501) staff       (20)     5380 2023-04-27 22:34:27.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.349780 mosaicml-cli-0.4.0a4/mcli/cli/m_deploy/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3896 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.350792 mosaicml-cli-0.4.0a4/mcli/cli/m_describe/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4367 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     9702 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     1860 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.353345 mosaicml-cli-0.4.0a4/mcli/cli/m_get/
--rw-r--r--   0 anna       (501) staff       (20)      467 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6226 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/clusters.py
--rw-r--r--   0 anna       (501) staff       (20)     6452 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/display.py
--rw-r--r--   0 anna       (501) staff       (20)     5467 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     4796 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/m_get.py
--rw-r--r--   0 anna       (501) staff       (20)     9517 2023-04-26 20:19:58.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/runs.py
--rw-r--r--   0 anna       (501) staff       (20)     2189 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     1580 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/users.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.354132 mosaicml-cli-0.4.0a4/mcli/cli/m_init/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_init/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4115 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_init/m_init.py
--rw-r--r--   0 anna       (501) staff       (20)    13963 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_init/m_init_kube.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.355198 mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     9005 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 anna       (501) staff       (20)    44284 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/kube_config.py
--rw-r--r--   0 anna       (501) staff       (20)     9321 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.355625 mosaicml-cli-0.4.0a4/mcli/cli/m_log/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_log/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)    10260 2023-04-27 22:45:47.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.356137 mosaicml-cli-0.4.0a4/mcli/cli/m_ping/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1732 2023-04-27 22:33:58.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.356625 mosaicml-cli-0.4.0a4/mcli/cli/m_predict/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.357275 mosaicml-cli-0.4.0a4/mcli/cli/m_root/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_root/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      536 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.357702 mosaicml-cli-0.4.0a4/mcli/cli/m_run/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_run/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     8099 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.359487 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2973 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 anna       (501) staff       (20)     1802 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 anna       (501) staff       (20)     1940 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 anna       (501) staff       (20)     1421 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 anna       (501) staff       (20)      881 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.360038 mosaicml-cli-0.4.0a4/mcli/cli/m_stop/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3847 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.360835 mosaicml-cli-0.4.0a4/mcli/cli/m_util/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_util/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      797 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_util/m_util.py
--rw-r--r--   0 anna       (501) staff       (20)     6837 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_util/util.py
--rw-r--r--   0 anna       (501) staff       (20)    12743 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.362829 mosaicml-cli-0.4.0a4/mcli/models/
--rw-r--r--   0 anna       (501) staff       (20)     1047 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/models/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2103 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/models/gpu_type.py
--rw-r--r--   0 anna       (501) staff       (20)    11810 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/models/inference_deployment_config.py
--rw-r--r--   0 anna       (501) staff       (20)      427 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/models/mcli_cluster.py
--rw-r--r--   0 anna       (501) staff       (20)      563 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/models/mcli_envvar.py
--rw-r--r--   0 anna       (501) staff       (20)     6156 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/models/mcli_secret.py
--rw-r--r--   0 anna       (501) staff       (20)    19299 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/models/run_config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.363211 mosaicml-cli-0.4.0a4/mcli/objects/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/objects/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.365733 mosaicml-cli-0.4.0a4/mcli/objects/secrets/
--rw-r--r--   0 anna       (501) staff       (20)     1090 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.367642 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1646 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/base.py
--rw-r--r--   0 anna       (501) staff       (20)     2244 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 anna       (501) staff       (20)     2408 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 anna       (501) staff       (20)     6377 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 anna       (501) staff       (20)     3858 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 anna       (501) staff       (20)     3001 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 anna       (501) staff       (20)     5342 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 anna       (501) staff       (20)      783 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 anna       (501) staff       (20)     1017 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/env_var.py
--rw-r--r--   0 anna       (501) staff       (20)      556 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/gcp.py
--rw-r--r--   0 anna       (501) staff       (20)     1267 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/mounted.py
--rw-r--r--   0 anna       (501) staff       (20)      967 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/oci.py
--rw-r--r--   0 anna       (501) staff       (20)      961 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/s3.py
--rw-r--r--   0 anna       (501) staff       (20)     1718 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.368132 mosaicml-cli-0.4.0a4/mcli/proto/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/proto/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1477 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.368536 mosaicml-cli-0.4.0a4/mcli/sdk/
--rw-r--r--   0 anna       (501) staff       (20)     1099 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/sdk/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.375028 mosaicml-cli-0.4.0a4/mcli/utils/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     5306 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_cli.py
--rw-r--r--   0 anna       (501) staff       (20)     6073 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_config.py
--rw-r--r--   0 anna       (501) staff       (20)      740 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_date.py
--rw-r--r--   0 anna       (501) staff       (20)    10453 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_docker.py
--rw-r--r--   0 anna       (501) staff       (20)     2225 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_epilog.py
--rw-r--r--   0 anna       (501) staff       (20)    10774 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_interactive.py
--rw-r--r--   0 anna       (501) staff       (20)     4527 2023-04-27 22:43:58.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_logging.py
--rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 anna       (501) staff       (20)     6614 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_pypi.py
--rw-r--r--   0 anna       (501) staff       (20)     3115 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_rich.py
--rw-r--r--   0 anna       (501) staff       (20)     4307 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_run_status.py
--rw-r--r--   0 anna       (501) staff       (20)     4350 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 anna       (501) staff       (20)     1103 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_spinner.py
--rw-r--r--   0 anna       (501) staff       (20)    10751 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_string_functions.py
--rw-r--r--   0 anna       (501) staff       (20)     1677 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_types.py
--rw-r--r--   0 anna       (501) staff       (20)     1001 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_yaml.py
--rw-r--r--   0 anna       (501) staff       (20)     3887 2023-04-27 22:49:49.000000 mosaicml-cli-0.4.0a4/mcli/version.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.376085 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/
--rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-27 22:51:24.000000 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 anna       (501) staff       (20)     4708 2023-04-27 22:51:24.000000 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anna       (501) staff       (20)        1 2023-04-27 22:51:24.000000 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anna       (501) staff       (20)       75 2023-04-27 22:51:24.000000 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 anna       (501) staff       (20)     1546 2023-04-27 22:51:24.000000 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 anna       (501) staff       (20)        5 2023-04-27 22:51:24.000000 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 anna       (501) staff       (20)    31087 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/pyproject.toml
--rw-r--r--   0 anna       (501) staff       (20)       38 2023-04-27 22:51:24.378935 mosaicml-cli-0.4.0a4/setup.cfg
--rw-r--r--   0 anna       (501) staff       (20)     2965 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/setup.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.377298 mosaicml-cli-0.4.0a4/tests/
--rw-r--r--   0 anna       (501) staff       (20)     5991 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/tests/test_config.py
--rw-r--r--   0 anna       (501) staff       (20)       62 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/tests/test_simple.py
--rw-r--r--   0 anna       (501) staff       (20)     6116 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/tests/test_upgrade.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.859705 mosaicml-cli-0.4.0a5/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      698 2023-05-03 00:12:03.859367 mosaicml-cli-0.4.0a5/PKG-INFO
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7199 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/README.md
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.811890 mosaicml-cli-0.4.0a5/mcli/
+-rw-r--r--   0 tylerlee   (502) staff       (20)       54 2022-03-04 18:07:55.000000 mosaicml-cli-0.4.0a5/mcli/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.814143 mosaicml-cli-0.4.0a5/mcli/api/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/api/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.814981 mosaicml-cli-0.4.0a5/mcli/api/cluster/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      134 2022-11-02 22:22:14.000000 mosaicml-cli-0.4.0a5/mcli/api/cluster/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4216 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.815445 mosaicml-cli-0.4.0a5/mcli/api/engine/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/api/engine/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    25914 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/api/engine/engine.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10685 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/api/exceptions.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.817896 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1023 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3427 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3311 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3586 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6117 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1294 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_ping_inference_deployment.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1596 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_predict_inference_deployment.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.818625 mosaicml-cli-0.4.0a5/mcli/api/mint/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a5/mcli/api/mint/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7005 2023-05-03 00:02:41.000000 mosaicml-cli-0.4.0a5/mcli/api/mint/shell.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2489 2023-05-03 00:02:41.000000 mosaicml-cli-0.4.0a5/mcli/api/mint/tty.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.819597 mosaicml-cli-0.4.0a5/mcli/api/model/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1114 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/api/model/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6290 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/model/cluster_details.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2992 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10439 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/api/model/run.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.822357 mosaicml-cli-0.4.0a5/mcli/api/runs/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1199 2023-04-25 23:51:33.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2750 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4143 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     8371 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10912 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5141 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5329 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3937 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10619 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.822976 mosaicml-cli-0.4.0a5/mcli/api/schema/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/api/schema/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      636 2022-08-23 15:11:52.000000 mosaicml-cli-0.4.0a5/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.824437 mosaicml-cli-0.4.0a5/mcli/api/secrets/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      309 2022-09-23 17:32:12.000000 mosaicml-cli-0.4.0a5/mcli/api/secrets/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2365 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a5/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2998 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a5/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3697 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a5/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2354 2022-03-24 04:29:23.000000 mosaicml-cli-0.4.0a5/mcli/api/typing_future.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.825075 mosaicml-cli-0.4.0a5/mcli/api/users/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      139 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a5/mcli/api/users/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2694 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a5/mcli/api/users/api_get_users.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.825570 mosaicml-cli-0.4.0a5/mcli/cli/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.0a5/mcli/cli/__init__.py
+-rwxr-xr-x   0 tylerlee   (502) staff       (20)     6436 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/cli.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.826347 mosaicml-cli-0.4.0a5/mcli/cli/common/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a5/mcli/cli/common/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2670 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     7331 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.826925 mosaicml-cli-0.4.0a5/mcli/cli/m_connect/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1541 2023-04-21 23:37:59.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.828039 mosaicml-cli-0.4.0a5/mcli/cli/m_create/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2385 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    16874 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.828886 mosaicml-cli-0.4.0a5/mcli/cli/m_delete/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6098 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5380 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.829268 mosaicml-cli-0.4.0a5/mcli/cli/m_deploy/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3896 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.830275 mosaicml-cli-0.4.0a5/mcli/cli/m_describe/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-01-26 00:46:18.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4367 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     9702 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1860 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.832541 mosaicml-cli-0.4.0a5/mcli/cli/m_get/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      467 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6226 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6452 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/display.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5467 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4796 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     9517 2023-04-26 01:33:20.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/runs.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2189 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1580 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_get/users.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.833224 mosaicml-cli-0.4.0a5/mcli/cli/m_init/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4115 2023-04-27 21:32:19.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_init/m_init.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    13963 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_init/m_init_kube.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.833972 mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     9005 2023-05-03 00:02:41.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    44284 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/kube_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     9321 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.834313 mosaicml-cli-0.4.0a5/mcli/cli/m_log/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10260 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.834747 mosaicml-cli-0.4.0a5/mcli/cli/m_ping/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2343 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.835087 mosaicml-cli-0.4.0a5/mcli/cli/m_predict/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2684 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.835551 mosaicml-cli-0.4.0a5/mcli/cli/m_root/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      536 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.836120 mosaicml-cli-0.4.0a5/mcli/cli/m_run/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     8099 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.837627 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2973 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1802 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1940 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1421 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      881 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.838038 mosaicml-cli-0.4.0a5/mcli/cli/m_stop/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3847 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.838582 mosaicml-cli-0.4.0a5/mcli/cli/m_util/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-08-10 05:32:44.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      797 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6837 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/cli/m_util/util.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    12743 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/config.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.840315 mosaicml-cli-0.4.0a5/mcli/models/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1047 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/models/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2103 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/models/gpu_type.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    11816 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      427 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/models/mcli_cluster.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      563 2022-09-13 15:17:57.000000 mosaicml-cli-0.4.0a5/mcli/models/mcli_envvar.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6156 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/models/mcli_secret.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    19547 2023-05-03 00:07:06.000000 mosaicml-cli-0.4.0a5/mcli/models/run_config.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.840611 mosaicml-cli-0.4.0a5/mcli/objects/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a5/mcli/objects/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.842490 mosaicml-cli-0.4.0a5/mcli/objects/secrets/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1090 2022-12-07 21:26:59.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.844126 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1646 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2244 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2408 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6377 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3858 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3001 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5342 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      783 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1017 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      556 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1267 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      967 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/oci.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      961 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/s3.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1718 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.844424 mosaicml-cli-0.4.0a5/mcli/proto/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/proto/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1477 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.844668 mosaicml-cli-0.4.0a5/mcli/sdk/
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1099 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/sdk/__init__.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.850357 mosaicml-cli-0.4.0a5/mcli/utils/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.0a5/mcli/utils/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5306 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_cli.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6073 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      740 2022-09-27 01:25:02.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_date.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10453 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_docker.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2225 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_epilog.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10774 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_interactive.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4527 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_logging.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2160 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6614 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_pypi.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3115 2023-03-15 17:23:44.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_rich.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4307 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_run_status.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4350 2022-03-30 16:04:08.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1103 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_spinner.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)    10751 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1677 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_types.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1001 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a5/mcli/utils/utils_yaml.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     3887 2023-05-03 00:08:44.000000 mosaicml-cli-0.4.0a5/mcli/version.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.854904 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/
+-rw-r--r--   0 tylerlee   (502) staff       (20)      698 2023-05-03 00:12:03.000000 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tylerlee   (502) staff       (20)     4744 2023-05-03 00:12:03.000000 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)        1 2023-05-03 00:12:03.000000 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)       75 2023-05-03 00:12:03.000000 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)     1565 2023-05-03 00:12:03.000000 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)        5 2023-05-03 00:12:03.000000 mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 tylerlee   (502) staff       (20)    31087 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a5/pyproject.toml
+-rw-r--r--   0 tylerlee   (502) staff       (20)       38 2023-05-03 00:12:03.859925 mosaicml-cli-0.4.0a5/setup.cfg
+-rw-r--r--   0 tylerlee   (502) staff       (20)     2991 2023-05-03 00:11:27.000000 mosaicml-cli-0.4.0a5/setup.py
+drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-05-03 00:12:03.858363 mosaicml-cli-0.4.0a5/tests/
+-rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.0a5/tests/__init__.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)      618 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/tests/conftest.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     5991 2023-05-03 00:07:01.000000 mosaicml-cli-0.4.0a5/tests/test_config.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)       62 2022-03-03 05:25:48.000000 mosaicml-cli-0.4.0a5/tests/test_simple.py
+-rw-r--r--   0 tylerlee   (502) staff       (20)     6116 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a5/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.0a4/PKG-INFO` & `mosaicml-cli-0.4.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.0a4
+Version: 0.4.0a5
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.0a4/README.md` & `mosaicml-cli-0.4.0a5/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.4.0a5/mcli/api/cluster/api_get_clusters.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,19 @@
     allowMultinode
     allowedInstances {{
       name
       gpuType
       gpusPerNode
       gpuNums
       numNodes
+      nodes {{
+        name
+        isAlive
+        isSchedulable
+      }}
     }}
   }}
 }}"""
 QUERY_UTILIZATION = f"""
 query GetClusters(${VARIABLE_DATA_NAME}: GetClustersInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
```

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/engine/engine.py` & `mosaicml-cli-0.4.0a5/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/exceptions.py` & `mosaicml-cli-0.4.0a5/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,18 @@
     ...
 
 
 def create_inference_deployment(deployment: Union[InferenceDeploymentConfig, FinalInferenceDeploymentConfig],
                                 timeout: Optional[float] = 10,
                                 future: bool = False) -> Union[InferenceDeployment, Future[InferenceDeployment]]:
     """Launch a inference deployment in the MosaicML platform
+
     The provided :class:`deploy <mcli.models.inference_deployment_config.InferenceDeploymentConfig>` must contain
     enough information to fully detail the inference deployment
+    
     Args:
         deployment: A fully-configured inference deployment to launch. The deployment will be queued and persisted
             in the deployment database.
         timeout: Time, in seconds, in which the call should complete. If the deployment creation
             takes too long, a TimeoutError will be raised. If ``future`` is ``True``, this
             value will be ignored.
         future: Return the output as a :type concurrent.futures.Future:. If True, the
```

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_get_inference_deployment_logs.py` & `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,17 @@
     gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[List[str]] = None,
     timeout: Optional[float] = 10,
     future: bool = False,
 ):
     """List inference deployments that have been launched in the MosaicML platform
+
     The returned list will contain all of the details stored about the requested deployments.
+    
     Arguments:
         deployments: List of inference deployments on which to get information
         clusters: List of clusters to filter inference deployments. This can be a list of str or
             :type Cluster: objects. Only deployments submitted to these clusters will be
             returned.
         before: Only inference deployments created strictly before this time will be returned. This
             can be a str in ISO 8601 format(e.g 2023-03-31T12:23:04.34+05:30)
```

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_ping_inference_deployment.py` & `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_ping_inference_deployment.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """ Ping a InferenceDeployment """
 from __future__ import annotations
 
-from typing import Optional
+from typing import Optional, Union
 
 import requests
 from requests import Response
 
 from mcli.api.model.inference_deployment import InferenceDeployment
 
 __all__ = ['ping_inference_deployment']
 
 
 def ping_inference_deployment(
-    deployment: InferenceDeployment,
+    deployment: Union[InferenceDeployment, str],
     timeout: Optional[float] = 10,
 ) -> dict:
     """Pings an inference deployment that has been launched in the MosaicML platform
     and returns the status of the deployment. The deployment must have a '/ping' endpoint
     defined.
     Arguments:
-        deployment: Inference deployment to ping for a status check
+        deployment:(InferenceDeployment | str): The deployment to check the status of. Can be
+            either an InferenceDeployment or a string which is of the form https://<the deployment dns>.
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised.
     Raises:
         HTTPError: If pinging the endpoint fails
     """
-    resp: Response = requests.get(url=f'https://{deployment.public_dns}/ping', timeout=timeout)
+    base_url = f'https://{deployment.public_dns}' if isinstance(deployment, InferenceDeployment) else deployment
+    resp: Response = requests.get(url=f'{base_url}/ping', timeout=timeout)
     if resp.ok:
         return resp.json()
     else:
         resp.raise_for_status()
         return {}
```

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.4.0a5/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 """ Predict on an Inference Deployment """
 from __future__ import annotations
 
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 import requests
 from requests import Response
 
+from mcli import config
 from mcli.api.model.inference_deployment import InferenceDeployment
 
 __all__ = ['predict']
 
 
 def predict(
-    deployment: InferenceDeployment,
+    deployment: Union[InferenceDeployment, str],
     inputs: Dict[str, Any],
     timeout: Optional[float] = 20,
 ) -> dict:
-    """Sends input to \'/infer\' endpoint of an inference deployment on the MosaicML
+    """Sends input to \'/predict\' endpoint of an inference deployment on the MosaicML
     platform. Runs prediction on input and returns output produced by the model.
     Arguments:
-        deployment: Inference deployment to send input to
+        deployment (InferenceDeployment | str): The deployment to make a prediction with.
+            Can be either an InferenceDeployment object to send or a string which is of
+            the form https://<the deployment dns>.
         input: Input data to run prediction on in the form of dictionary
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised.
     Raises:
         HTTPError: If sending the request to the endpoint fails
     """
-    resp: Response = requests.post(url=f'https://{deployment.public_dns}/predict', timeout=timeout, json=inputs)
+    conf = config.MCLIConfig.load_config(safe=True)
+    api_key = conf.api_key
+    headers = {
+        'authorization': api_key,
+    }
+    base_url = f'https://{deployment.public_dns}' if isinstance(deployment, InferenceDeployment) else deployment
+    resp: Response = requests.post(url=f'{base_url}/predict', timeout=timeout, json=inputs, headers=headers)
     if resp.ok:
         return resp.json()
     else:
         resp.raise_for_status()
         return {}
```

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/mint/shell.py` & `mosaicml-cli-0.4.0a5/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/mint/tty.py` & `mosaicml-cli-0.4.0a5/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/model/__init__.py` & `mosaicml-cli-0.4.0a5/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.4.0a5/mcli/api/model/cluster_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,32 +90,50 @@
         ],
                    active_by_user=[ClusterUtilizationByRun.from_mapi_response(i) for i in response['activeByUser']],
                    queued_by_user=[ClusterUtilizationByRun.from_mapi_response(i) for i in response['queuedByUser']],
                    anonymize_users=response['anonymizeUsers'])
 
 
 @dataclass
+class Node:
+    """Node on an instance for a cluster
+    """
+    name: str
+    is_alive: bool
+    is_schedulable: bool
+
+    @classmethod
+    def from_mapi_response(cls, response: Dict[str, Any]) -> Node:
+        check_response(response, {'name', 'isAlive', 'isSchedulable'})
+        return cls(name=response['name'], is_alive=response['isAlive'], is_schedulable=response['isSchedulable'])
+
+
+@dataclass
 @functools.total_ordering
 class Instance:
     """Instance of a cluster
     """
     name: str
     gpu_type: str
     gpus: int
     nodes: int
     gpu_nums: List[int] = field(default_factory=list)
+    node_details: List[Node] = field(default_factory=list)
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> Instance:
-        check_response(response, {'name', 'gpusPerNode', 'numNodes', 'gpuType', 'gpuNums'})
-        return cls(name=response['name'],
-                   gpu_type=response['gpuType'],
-                   gpus=response['gpusPerNode'],
-                   nodes=response['numNodes'],
-                   gpu_nums=response['gpuNums'])
+        check_response(response, {'name', 'gpusPerNode', 'numNodes', 'gpuType', 'gpuNums', 'nodes'})
+        return cls(
+            name=response['name'],
+            gpu_type=response['gpuType'],
+            gpus=response['gpusPerNode'],
+            nodes=response['numNodes'],
+            gpu_nums=response['gpuNums'],
+            node_details=[Node.from_mapi_response(i) for i in response.get('nodes', [])],
+        )
 
     def __lt__(self, other: Instance):
         if self.gpu_type.lower() == 'none':
             return True
         return self.gpu_type < other.gpu_type
```

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.4.0a5/mcli/api/model/inference_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from mcli.api.schema.generic_model import DeserializableModel, convert_datetime
 from mcli.models.inference_deployment_config import FinalInferenceDeploymentConfig, InferenceDeploymentConfig
 
 
 @dataclass
 class InferenceDeployment(DeserializableModel):
     """A deployment that has been launched on the MosaicML Cloud
+    
     Args:
         deployment_uid (`str`): Unique identifier for the deployment
         name (`str`): User-defined name of the deployment
         status (:class:`~mcli.utils.utils_deployment_status.DeploymentStatus`): Status of the deployment
         at a moment in time
         created_at (`datetime`): Date and time when the deployment was created
         updated_at (`datetime`): Date and time when the deployment was last updated
```

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/model/run.py` & `mosaicml-cli-0.4.0a5/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/runs/__init__.py` & `mosaicml-cli-0.4.0a5/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.4.0a5/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.4.0a5/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.4.0a5/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.4.0a5/mcli/api/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.4.0a5/mcli/api/runs/api_start_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.4.0a5/mcli/api/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.4.0a5/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.4.0a5/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.4.0a5/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.4.0a5/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.4.0a5/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.4.0a5/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/typing_future.py` & `mosaicml-cli-0.4.0a5/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.4.0a5/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/cli.py` & `mosaicml-cli-0.4.0a5/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.4.0a5/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.4.0a5/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_get/display.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_get/users.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_init/m_init_kube.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_init/m_init_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/kube_config.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/kube_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_interactive/m_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_log/m_log.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_predict/m_predict.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,75 @@
-""" mcli ping entrypoint """
+"""mcli predict entrypoint"""
 import argparse
 import logging
 from pprint import pprint
-from typing import Optional
+from typing import Any, Dict, Optional, Union
+
+import validators
+import yaml
 
 from mcli.api.exceptions import MAPIException
+from mcli.api.model.inference_deployment import InferenceDeployment
 from mcli.cli.common.deployment_filters import get_deployments_with_filters
-from mcli.sdk import ping_inference_deployment
+from mcli.sdk import predict
 from mcli.utils.utils_logging import FAIL, err_console
 
 logger = logging.getLogger(__name__)
 
 
-def ping(
-    deployment_name: Optional[str] = None,
+def predict_cli(
+    inputs: Dict[str, Any],
+    deployment: Optional[str] = None,
     **kwargs,
 ) -> int:
     del kwargs
     try:
-        name_filter = [deployment_name] if deployment_name else None
-        deployments = get_deployments_with_filters(name_filter=name_filter, latest=True)
-
-        if len(deployments) == 0:
-            if not deployment_name:
-                err_console.print("No inference deployments found.")
-            else:
-                err_console.log(f'No inference deployment foung with name {deployment_name}.')
-            return 1
-
-        resp = ping_inference_deployment(deployments[0])
-        print(f'{deployments[0].name}\'s status:')
+        deployment_obj_or_url: Union[InferenceDeployment, Optional[str]] = deployment
+        if not deployment_obj_or_url or not validators.url(deployment):
+            # if a url is not passed in then lookup the deployment and get the name
+            name_filter = [deployment] if deployment else None
+            deployment_objs = get_deployments_with_filters(name_filter=name_filter, latest=True)
+            if len(deployment_objs) == 0:
+                if not deployment:
+                    err_console.print("No inference deployments found.")
+                else:
+                    err_console.print(f'No inference deployment found with name {deployment}.')
+                return 1
+
+            deployment_obj_or_url = deployment_objs[0]
+
+        resp = predict(deployment_obj_or_url, inputs=inputs)
+        name_or_url = deployment_obj_or_url if isinstance(deployment_obj_or_url, str) else deployment_obj_or_url.name
+        print(f'{name_or_url}\'s prediction results:')
         pprint(resp)
         return 0
     except RuntimeError as e:
         logger.error(f'{FAIL} {e}')
         return 1
-    except (MAPIException) as e:
+    except MAPIException as e:
         logger.error(f'{FAIL} {e}')
         return 1
 
 
-def add_ping_parser(subparser: argparse._SubParsersAction):
-    ping_parser: argparse.ArgumentParser = subparser.add_parser(
-        'ping',
-        help='Ping a inference deployment in the MosaicML platform for health metrics',
+def add_predict_parser(subparser: argparse._SubParsersAction):
+    predict_parser: argparse.ArgumentParser = subparser.add_parser(
+        'predict',
+        help='Run prediction on a model in the MosaicML Cloud with given inputs. Returns forward pass result',
+    )
+    predict_parser.add_argument('deployment',
+                                metavar='DEPLOYMENT',
+                                nargs='?',
+                                help='The name or url of the deployment to run inference on')
+
+    predict_parser.add_argument(
+        '--input',
+        '--inputs',
+        '-i',
+        dest='inputs',
+        required=True,
+        nargs="?",
+        type=yaml.safe_load,
+        metavar='INPUT',
+        help='Input values to run forward pass on. Input values must be JSON-serializable and have string keys.',
     )
-    ping_parser.add_argument(
-        'deployment_name',
-        metavar='DEPLOYMENT',
-        nargs='?',
-        help='The name of the inference deployment. If not provided, will return the metrics of the latest deployment')
 
-    ping_parser.set_defaults(func=ping)
+    predict_parser.set_defaults(func=predict_cli)
```

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_run/m_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/cli/m_util/util.py` & `mosaicml-cli-0.4.0a5/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/config.py` & `mosaicml-cli-0.4.0a5/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/models/__init__.py` & `mosaicml-cli-0.4.0a5/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/models/gpu_type.py` & `mosaicml-cli-0.4.0a5/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.4.0a5/mcli/models/inference_deployment_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,17 @@
             'inferenceDeploymentInput': translated_input,
         }
 
 
 @dataclass
 class InferenceDeploymentConfig(BaseSubmissionConfig):
     """A deployment configuration for the MosaicML Cloud
+
     Values in here are not yet validated and some required values may be missing.
+    
     Args:
         name (`Optional[str]`): User-defined name of the deployment
         gpu_type (`Optional[str]`): GPU type (optional if only one gpu type for your cluster)
         gpu_num (`Optional[int]`): Number of GPUs
         cluster (`Optional[str]`): Cluster to use (optional if you only have one)
         image (`Optional[str]`): Docker image (e.g. `mosaicml/composer`)
         command (`str`): Command to use when a deployment starts
```

### Comparing `mosaicml-cli-0.4.0a4/mcli/models/mcli_envvar.py` & `mosaicml-cli-0.4.0a5/mcli/models/mcli_envvar.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/models/mcli_secret.py` & `mosaicml-cli-0.4.0a5/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/models/run_config.py` & `mosaicml-cli-0.4.0a5/mcli/models/run_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 MAX_RUN_NAME_LENGTH = MAX_KUBERNETES_LENGTH - RUN_CONFIG_UID_LENGTH - 1  # -1 for the dash
 DEFAULT_PRIORITY_NAME = 'medium'
 
 
 class SchedulingConfig(TypedDict, total=False):
     """Typed dictionary for nested scheduling configurations"""
     priority: Optional[str]
+    resumable: Optional[bool]
+    max_retries: Optional[int]
 
 
 class ComputeConfig(TypedDict, total=False):
     """Typed dictionary for nested compute requests"""
     cluster: Optional[str]
     instance: Optional[str]
     nodes: Optional[int]
@@ -249,14 +251,17 @@
                 value = EnvVarTranslation.to_mapi(value)
             elif field_name == 'integrations':
                 value = IntegrationTranslation.to_mapi(value)
             elif field_name == "scheduling":
                 value = SchedulingTranslation.to_mapi(value)
             elif field_name == "compute":
                 value = ComputeTranslation.to_mapi(value)
+            elif field_name == "parameters":
+                # parameters should be passed as-is, explicitly
+                pass
             elif field_name == "gpu_type" and not value:
                 continue
             elif field_name == "cluster" and not value:
                 continue
             elif field_name == "platform":
                 continue
             elif isinstance(value, dict):
@@ -363,36 +368,36 @@
             integrations_list.append(translated_integration)
         return integrations_list
 
 
 class SchedulingTranslation(Translation[SchedulingConfig, Dict[str, Any]]):
     """Translate scheduling configs to and from MAPI"""
 
+    translations = {
+        "maxRetries": "max_retries",
+    }
+
     @classmethod
     def from_mapi(cls, value: Dict[str, Any]) -> SchedulingConfig:
-        extracted: SchedulingConfig = {'priority': None}
-        for k, v in value.items():
-            if k == 'priority':
-                extracted['priority'] = v
+        extracted = SchedulingConfig(**{cls.translations.get(k, k): v for k, v in value.items() if k != "priorityInt"})
         return extracted
 
     @classmethod
     def to_mapi(cls, value: SchedulingConfig) -> Dict[str, Any]:
-        processed: Dict[str, Any] = {}
-        for k, v in value.items():
-            if v is not None:
-                processed[k] = v
+        inv = {v: k for k, v in cls.translations.items()}
+        processed = {inv.get(k, k): v for k, v in value.items() if v is not None}
         return processed
 
 
 class ComputeTranslation(Translation[ComputeConfig, Dict[str, Any]]):
     """Translate compute configs to and from MAPI"""
 
     translations = {
         "gpuType": "gpu_type",
+        "nodeNames": "node_names",
     }
 
     @classmethod
     def from_mapi(cls, value: Dict[str, Any]) -> ComputeConfig:
         extracted = ComputeConfig(**{cls.translations.get(k, k): v for k, v in value.items()})
         return extracted
```

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.4.0a5/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.4.0a5/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/sdk/__init__.py` & `mosaicml-cli-0.4.0a5/mcli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_cli.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_config.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_date.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_docker.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_logging.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_rich.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_types.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.4.0a5/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/mcli/version.py` & `mosaicml-cli-0.4.0a5/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = "0.4.0a4"
+__version__ = "0.4.0a5"
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.0a4
+Version: 0.4.0a5
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -143,10 +143,12 @@
 mcli/utils/utils_yaml.py
 mosaicml_cli.egg-info/PKG-INFO
 mosaicml_cli.egg-info/SOURCES.txt
 mosaicml_cli.egg-info/dependency_links.txt
 mosaicml_cli.egg-info/entry_points.txt
 mosaicml_cli.egg-info/requires.txt
 mosaicml_cli.egg-info/top_level.txt
+tests/__init__.py
+tests/conftest.py
 tests/test_config.py
 tests/test_simple.py
 tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.4.0a5/mosaicml_cli.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,46 +6,47 @@
 prompt_toolkit>=3.0.29
 protobuf>=4.22.0
 pyyaml>=5.4.1
 questionary>=1.10.0
 rich>=10.16.2
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
+validators>=0.20.0
 
 [all]
-sphinxcontrib-katex>=0.8.6
-isort>=5.9.3
-sphinx-argparse>=0.3.1
-yapf>=0.33.0
-sphinxcontrib-images>=0.9.4
-sphinxcontrib-qthelp>=1.0.3
 sphinx-design
-sphinxcontrib-serializinghtml>=1.1.5
-toml>=0.10.2
-sphinxcontrib-applehelp>=1.0.2
-sphinx-copybutton>=0.5.0
-pre-commit>=2.17.0
+pytest-cov>=4.0.0
+sphinxemoji>=0.2.0
 sphinx-markdown-tables>=0.0.15
-sphinxext-opengraph>=0.6.1
+sphinxcontrib-applehelp>=1.0.2
+sphinx_external_toc>=0.3.0
+radon>=5.1.0
 sphinxcontrib-jsmath>=1.0.1
-pylint>=2.12.2
-sphinxcontrib-htmlhelp>=2.0.0
-sphinxemoji>=0.2.0
-sphinx-panels>=0.6.0
-sphinx-rtd-theme>=1.0.0
-sphinxcontrib-devhelp>=1.0.2
+yapf>=0.33.0
 furo>=2022.3.4
-pytest>=6.2.5
-radon>=5.1.0
+sphinxcontrib-serializinghtml>=1.1.5
+sphinx-panels>=0.6.0
+sphinx-argparse>=0.3.1
+sphinxcontrib-katex>=0.8.6
+pylint>=2.12.2
 pytest-mock>=3.7.0
-myst-parser>=0.16.1
-pyright>=1.1.256
 sphinx>=4.4.0
-sphinx_external_toc>=0.3.0
-pytest-cov>=4.0.0
+sphinxcontrib-qthelp>=1.0.3
+isort>=5.9.3
+pytest>=6.2.5
+sphinx-copybutton>=0.5.0
+sphinxcontrib-devhelp>=1.0.2
+pre-commit>=2.17.0
+sphinxcontrib-images>=0.9.4
+sphinxext-opengraph>=0.6.1
+pyright>=1.1.256
+myst-parser>=0.16.1
+sphinx-rtd-theme>=1.0.0
+toml>=0.10.2
+sphinxcontrib-htmlhelp>=2.0.0
 
 [dev]
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright>=1.1.256
 pytest-cov>=4.0.0
```

### Comparing `mosaicml-cli-0.4.0a4/pyproject.toml` & `mosaicml-cli-0.4.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/setup.py` & `mosaicml-cli-0.4.0a5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     'prompt_toolkit>=3.0.29',
     'protobuf>=4.22.0',
     'pyyaml>=5.4.1',
     'questionary>=1.10.0',
     'rich>=10.16.2',
     'ruamel.yaml>=0.17.21',
     'typing_extensions>=4.0.1',
+    'validators>=0.20.0',
 ]
 
 extra_deps = {}
 
 extra_deps['dev'] = [
     'isort>=5.9.3',
     'pre-commit>=2.17.0',
```

### Comparing `mosaicml-cli-0.4.0a4/tests/test_config.py` & `mosaicml-cli-0.4.0a5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a4/tests/test_upgrade.py` & `mosaicml-cli-0.4.0a5/tests/test_upgrade.py`

 * *Files identical despite different names*

