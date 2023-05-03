# Comparing `tmp/mosaicml-cli-0.4.0a3.tar.gz` & `tmp/mosaicml-cli-0.4.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.0a3.tar", last modified: Tue Apr 25 22:15:59 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.4.0a4.tar", last modified: Thu Apr 27 22:51:24 2023, max compression
```

## Comparing `mosaicml-cli-0.4.0a3.tar` & `mosaicml-cli-0.4.0a4.tar`

### file list

```diff
@@ -1,194 +1,193 @@
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.880574 mosaicml-cli-0.4.0a3/
--rw-r--r--   0 tylerlee   (502) staff       (20)      698 2023-04-25 22:15:59.880238 mosaicml-cli-0.4.0a3/PKG-INFO
--rw-r--r--   0 tylerlee   (502) staff       (20)     7173 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/README.md
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.816949 mosaicml-cli-0.4.0a3/mcli/
--rw-r--r--   0 tylerlee   (502) staff       (20)       54 2022-03-04 18:07:55.000000 mosaicml-cli-0.4.0a3/mcli/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.817643 mosaicml-cli-0.4.0a3/mcli/api/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/api/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.818303 mosaicml-cli-0.4.0a3/mcli/api/cluster/
--rw-r--r--   0 tylerlee   (502) staff       (20)      134 2022-11-02 22:22:14.000000 mosaicml-cli-0.4.0a3/mcli/api/cluster/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4141 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.818765 mosaicml-cli-0.4.0a3/mcli/api/engine/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/api/engine/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    24296 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/api/engine/engine.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10685 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/api/exceptions.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.820795 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/
--rw-r--r--   0 tylerlee   (502) staff       (20)      879 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3421 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3311 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6111 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1052 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_ping_inference_deployment.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1134 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_predict_inference_deployment.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.821557 mosaicml-cli-0.4.0a3/mcli/api/mint/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a3/mcli/api/mint/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     7005 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/api/mint/shell.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2489 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/api/mint/tty.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.822601 mosaicml-cli-0.4.0a3/mcli/api/model/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1114 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/api/model/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5735 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/api/model/cluster_details.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2987 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/model/inference_deployment.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     7814 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/api/model/run.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.826673 mosaicml-cli-0.4.0a3/mcli/api/runs/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1199 2023-04-25 21:57:35.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2750 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_create_run.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3926 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     7971 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10427 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4910 2023-04-25 21:57:35.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_start_run.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5099 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3937 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10619 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.827258 mosaicml-cli-0.4.0a3/mcli/api/schema/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/api/schema/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      636 2022-08-23 15:11:52.000000 mosaicml-cli-0.4.0a3/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.828612 mosaicml-cli-0.4.0a3/mcli/api/secrets/
--rw-r--r--   0 tylerlee   (502) staff       (20)      309 2022-09-23 17:32:12.000000 mosaicml-cli-0.4.0a3/mcli/api/secrets/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2365 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a3/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2998 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3697 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2354 2022-03-24 04:29:23.000000 mosaicml-cli-0.4.0a3/mcli/api/typing_future.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.829239 mosaicml-cli-0.4.0a3/mcli/api/users/
--rw-r--r--   0 tylerlee   (502) staff       (20)      139 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a3/mcli/api/users/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2694 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a3/mcli/api/users/api_get_users.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.829697 mosaicml-cli-0.4.0a3/mcli/cli/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.0a3/mcli/cli/__init__.py
--rwxr-xr-x   0 tylerlee   (502) staff       (20)     6384 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/cli.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.830456 mosaicml-cli-0.4.0a3/mcli/cli/common/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a3/mcli/cli/common/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2670 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6950 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.830808 mosaicml-cli-0.4.0a3/mcli/cli/m_connect/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-16 23:57:15.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1541 2023-04-21 23:37:59.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.831512 mosaicml-cli-0.4.0a3/mcli/cli/m_create/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_create/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2385 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_create/m_create.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    16874 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.832204 mosaicml-cli-0.4.0a3/mcli/cli/m_delete/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6098 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_delete/delete.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5600 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.832528 mosaicml-cli-0.4.0a3/mcli/cli/m_deploy/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3896 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.833341 mosaicml-cli-0.4.0a3/mcli/cli/m_describe/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-01-26 00:46:18.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4367 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10262 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1860 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.835576 mosaicml-cli-0.4.0a3/mcli/cli/m_get/
--rw-r--r--   0 tylerlee   (502) staff       (20)      467 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6226 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/clusters.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6452 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/display.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5467 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4506 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/m_get.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     9517 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/runs.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2189 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/secrets.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1580 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_get/users.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.836382 mosaicml-cli-0.4.0a3/mcli/cli/m_init/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_init/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4113 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_init/m_init.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    13963 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_init/m_init_kube.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.837226 mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     9005 2023-04-21 14:41:49.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    44284 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/kube_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     9321 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.837584 mosaicml-cli-0.4.0a3/mcli/cli/m_log/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_log/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6803 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.837850 mosaicml-cli-0.4.0a3/mcli/cli/m_ping/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1742 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.838142 mosaicml-cli-0.4.0a3/mcli/cli/m_predict/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2160 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.838479 mosaicml-cli-0.4.0a3/mcli/cli/m_root/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_root/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      536 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.838785 mosaicml-cli-0.4.0a3/mcli/cli/m_run/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_run/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     8099 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.840460 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2973 2023-04-12 22:48:07.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1802 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1940 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1421 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      881 2023-02-03 22:45:38.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.840859 mosaicml-cli-0.4.0a3/mcli/cli/m_stop/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-10-04 23:53:41.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3847 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.841486 mosaicml-cli-0.4.0a3/mcli/cli/m_util/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-08-10 05:32:44.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_util/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      797 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_util/m_util.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6837 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/cli/m_util/util.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    12743 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/config.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.846583 mosaicml-cli-0.4.0a3/mcli/models/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1047 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/models/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2103 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/models/gpu_type.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    11810 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/models/inference_deployment_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      427 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/models/mcli_cluster.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      563 2022-09-13 15:17:57.000000 mosaicml-cli-0.4.0a3/mcli/models/mcli_envvar.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6156 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/models/mcli_secret.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    19299 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/models/run_config.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.847461 mosaicml-cli-0.4.0a3/mcli/objects/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a3/mcli/objects/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.853218 mosaicml-cli-0.4.0a3/mcli/objects/secrets/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1090 2022-12-07 21:26:59.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.858225 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-06-22 01:15:31.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1646 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/base.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2244 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2408 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6377 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3858 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3001 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5342 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      783 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1017 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/env_var.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      556 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/gcp.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1267 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/mounted.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      967 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/oci.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      961 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/s3.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1718 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.859425 mosaicml-cli-0.4.0a3/mcli/proto/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/proto/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1477 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.860194 mosaicml-cli-0.4.0a3/mcli/sdk/
--rw-r--r--   0 tylerlee   (502) staff       (20)     1068 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/sdk/__init__.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.871833 mosaicml-cli-0.4.0a3/mcli/utils/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.0a3/mcli/utils/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5306 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_cli.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6073 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      740 2022-09-27 01:25:02.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_date.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10453 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_docker.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2225 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_epilog.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10774 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_interactive.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4130 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_logging.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     2160 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6614 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_pypi.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3115 2023-03-15 17:23:44.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_rich.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4307 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_run_status.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     4350 2022-03-30 16:04:08.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1103 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_spinner.py
--rw-r--r--   0 tylerlee   (502) staff       (20)    10751 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_string_functions.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1677 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_types.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     1001 2022-03-09 05:57:25.000000 mosaicml-cli-0.4.0a3/mcli/utils/utils_yaml.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     3886 2023-04-25 22:13:08.000000 mosaicml-cli-0.4.0a3/mcli/version.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.875457 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/
--rw-r--r--   0 tylerlee   (502) staff       (20)      698 2023-04-25 22:15:59.000000 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 tylerlee   (502) staff       (20)     4676 2023-04-25 22:15:59.000000 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)        1 2023-04-25 22:15:59.000000 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)       75 2023-04-25 22:15:59.000000 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)     1546 2023-04-25 22:15:59.000000 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)        5 2023-04-25 22:15:59.000000 mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 tylerlee   (502) staff       (20)    31087 2023-04-25 21:22:56.000000 mosaicml-cli-0.4.0a3/pyproject.toml
--rw-r--r--   0 tylerlee   (502) staff       (20)       38 2023-04-25 22:15:59.880775 mosaicml-cli-0.4.0a3/setup.cfg
--rw-r--r--   0 tylerlee   (502) staff       (20)     2965 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/setup.py
-drwxr-xr-x   0 tylerlee   (502) staff       (20)        0 2023-04-25 22:15:59.879176 mosaicml-cli-0.4.0a3/tests/
--rw-r--r--   0 tylerlee   (502) staff       (20)        0 2022-02-08 05:39:24.000000 mosaicml-cli-0.4.0a3/tests/__init__.py
--rw-r--r--   0 tylerlee   (502) staff       (20)      618 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/tests/conftest.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     5991 2023-04-25 22:12:56.000000 mosaicml-cli-0.4.0a3/tests/test_config.py
--rw-r--r--   0 tylerlee   (502) staff       (20)       62 2022-03-03 05:25:48.000000 mosaicml-cli-0.4.0a3/tests/test_simple.py
--rw-r--r--   0 tylerlee   (502) staff       (20)     6116 2023-03-17 00:12:11.000000 mosaicml-cli-0.4.0a3/tests/test_upgrade.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.378729 mosaicml-cli-0.4.0a4/
+-rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-27 22:51:24.378381 mosaicml-cli-0.4.0a4/PKG-INFO
+-rw-r--r--   0 anna       (501) staff       (20)     7199 2023-04-27 22:42:06.000000 mosaicml-cli-0.4.0a4/README.md
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.333880 mosaicml-cli-0.4.0a4/mcli/
+-rw-r--r--   0 anna       (501) staff       (20)       54 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.334604 mosaicml-cli-0.4.0a4/mcli/api/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.335406 mosaicml-cli-0.4.0a4/mcli/api/cluster/
+-rw-r--r--   0 anna       (501) staff       (20)      134 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/cluster/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4141 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.336058 mosaicml-cli-0.4.0a4/mcli/api/engine/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/engine/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)    25914 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/engine/engine.py
+-rw-r--r--   0 anna       (501) staff       (20)    10685 2023-04-27 22:33:58.000000 mosaicml-cli-0.4.0a4/mcli/api/exceptions.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.338595 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/
+-rw-r--r--   0 anna       (501) staff       (20)     1023 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3421 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)     3311 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     3586 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 anna       (501) staff       (20)     6111 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     1052 2023-04-27 22:33:58.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_ping_inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)     1136 2023-04-27 22:33:58.000000 mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_predict_inference_deployment.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.339181 mosaicml-cli-0.4.0a4/mcli/api/mint/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/mint/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     7005 2023-04-27 22:33:58.000000 mosaicml-cli-0.4.0a4/mcli/api/mint/shell.py
+-rw-r--r--   0 anna       (501) staff       (20)     2489 2023-04-27 22:33:58.000000 mosaicml-cli-0.4.0a4/mcli/api/mint/tty.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.340445 mosaicml-cli-0.4.0a4/mcli/api/model/
+-rw-r--r--   0 anna       (501) staff       (20)     1114 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/api/model/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     5735 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/api/model/cluster_details.py
+-rw-r--r--   0 anna       (501) staff       (20)     2987 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 anna       (501) staff       (20)    10439 2023-04-27 22:42:24.000000 mosaicml-cli-0.4.0a4/mcli/api/model/run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.343528 mosaicml-cli-0.4.0a4/mcli/api/runs/
+-rw-r--r--   0 anna       (501) staff       (20)     1199 2023-04-26 20:08:55.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2750 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 anna       (501) staff       (20)     4143 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     8371 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 anna       (501) staff       (20)    10912 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     5141 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 anna       (501) staff       (20)     5329 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     3937 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 anna       (501) staff       (20)    10619 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.343920 mosaicml-cli-0.4.0a4/mcli/api/schema/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/schema/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      636 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.345032 mosaicml-cli-0.4.0a4/mcli/api/secrets/
+-rw-r--r--   0 anna       (501) staff       (20)      309 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/secrets/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2365 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 anna       (501) staff       (20)     2998 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     3697 2023-04-26 22:07:45.000000 mosaicml-cli-0.4.0a4/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     2354 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/typing_future.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.345598 mosaicml-cli-0.4.0a4/mcli/api/users/
+-rw-r--r--   0 anna       (501) staff       (20)      139 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/api/users/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2694 2023-04-27 22:33:37.000000 mosaicml-cli-0.4.0a4/mcli/api/users/api_get_users.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.346310 mosaicml-cli-0.4.0a4/mcli/cli/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/__init__.py
+-rwxr-xr-x   0 anna       (501) staff       (20)     6436 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/cli/cli.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.347102 mosaicml-cli-0.4.0a4/mcli/cli/common/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/common/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2670 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 anna       (501) staff       (20)     7331 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.347528 mosaicml-cli-0.4.0a4/mcli/cli/m_connect/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1541 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.348347 mosaicml-cli-0.4.0a4/mcli/cli/m_create/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2385 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 anna       (501) staff       (20)    16874 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.349324 mosaicml-cli-0.4.0a4/mcli/cli/m_delete/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6098 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 anna       (501) staff       (20)     5380 2023-04-27 22:34:27.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.349780 mosaicml-cli-0.4.0a4/mcli/cli/m_deploy/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3896 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.350792 mosaicml-cli-0.4.0a4/mcli/cli/m_describe/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4367 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     9702 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     1860 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.353345 mosaicml-cli-0.4.0a4/mcli/cli/m_get/
+-rw-r--r--   0 anna       (501) staff       (20)      467 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     6226 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 anna       (501) staff       (20)     6452 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/display.py
+-rw-r--r--   0 anna       (501) staff       (20)     5467 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 anna       (501) staff       (20)     4796 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 anna       (501) staff       (20)     9517 2023-04-26 20:19:58.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/runs.py
+-rw-r--r--   0 anna       (501) staff       (20)     2189 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 anna       (501) staff       (20)     1580 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_get/users.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.354132 mosaicml-cli-0.4.0a4/mcli/cli/m_init/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     4115 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_init/m_init.py
+-rw-r--r--   0 anna       (501) staff       (20)    13963 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_init/m_init_kube.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.355198 mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     9005 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 anna       (501) staff       (20)    44284 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/kube_config.py
+-rw-r--r--   0 anna       (501) staff       (20)     9321 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.355625 mosaicml-cli-0.4.0a4/mcli/cli/m_log/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)    10260 2023-04-27 22:45:47.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.356137 mosaicml-cli-0.4.0a4/mcli/cli/m_ping/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1732 2023-04-27 22:33:58.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.356625 mosaicml-cli-0.4.0a4/mcli/cli/m_predict/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.357275 mosaicml-cli-0.4.0a4/mcli/cli/m_root/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      536 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.357702 mosaicml-cli-0.4.0a4/mcli/cli/m_run/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     8099 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.359487 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2973 2023-04-18 18:35:37.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 anna       (501) staff       (20)     1802 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 anna       (501) staff       (20)     1940 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 anna       (501) staff       (20)     1421 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 anna       (501) staff       (20)      881 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.360038 mosaicml-cli-0.4.0a4/mcli/cli/m_stop/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     3847 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.360835 mosaicml-cli-0.4.0a4/mcli/cli/m_util/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)      797 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 anna       (501) staff       (20)     6837 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/cli/m_util/util.py
+-rw-r--r--   0 anna       (501) staff       (20)    12743 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.362829 mosaicml-cli-0.4.0a4/mcli/models/
+-rw-r--r--   0 anna       (501) staff       (20)     1047 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/models/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     2103 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/models/gpu_type.py
+-rw-r--r--   0 anna       (501) staff       (20)    11810 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 anna       (501) staff       (20)      427 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/models/mcli_cluster.py
+-rw-r--r--   0 anna       (501) staff       (20)      563 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/models/mcli_envvar.py
+-rw-r--r--   0 anna       (501) staff       (20)     6156 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/models/mcli_secret.py
+-rw-r--r--   0 anna       (501) staff       (20)    19299 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/models/run_config.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.363211 mosaicml-cli-0.4.0a4/mcli/objects/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/objects/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.365733 mosaicml-cli-0.4.0a4/mcli/objects/secrets/
+-rw-r--r--   0 anna       (501) staff       (20)     1090 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.367642 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1646 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 anna       (501) staff       (20)     2244 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 anna       (501) staff       (20)     2408 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 anna       (501) staff       (20)     6377 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 anna       (501) staff       (20)     3858 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 anna       (501) staff       (20)     3001 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 anna       (501) staff       (20)     5342 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 anna       (501) staff       (20)      783 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 anna       (501) staff       (20)     1017 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 anna       (501) staff       (20)      556 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 anna       (501) staff       (20)     1267 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 anna       (501) staff       (20)      967 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/oci.py
+-rw-r--r--   0 anna       (501) staff       (20)      961 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/s3.py
+-rw-r--r--   0 anna       (501) staff       (20)     1718 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.368132 mosaicml-cli-0.4.0a4/mcli/proto/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/proto/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     1477 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.368536 mosaicml-cli-0.4.0a4/mcli/sdk/
+-rw-r--r--   0 anna       (501) staff       (20)     1099 2023-04-27 22:34:02.000000 mosaicml-cli-0.4.0a4/mcli/sdk/__init__.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.375028 mosaicml-cli-0.4.0a4/mcli/utils/
+-rw-r--r--   0 anna       (501) staff       (20)        0 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/__init__.py
+-rw-r--r--   0 anna       (501) staff       (20)     5306 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_cli.py
+-rw-r--r--   0 anna       (501) staff       (20)     6073 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_config.py
+-rw-r--r--   0 anna       (501) staff       (20)      740 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_date.py
+-rw-r--r--   0 anna       (501) staff       (20)    10453 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_docker.py
+-rw-r--r--   0 anna       (501) staff       (20)     2225 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_epilog.py
+-rw-r--r--   0 anna       (501) staff       (20)    10774 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_interactive.py
+-rw-r--r--   0 anna       (501) staff       (20)     4527 2023-04-27 22:43:58.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_logging.py
+-rw-r--r--   0 anna       (501) staff       (20)     2160 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 anna       (501) staff       (20)     6614 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_pypi.py
+-rw-r--r--   0 anna       (501) staff       (20)     3115 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_rich.py
+-rw-r--r--   0 anna       (501) staff       (20)     4307 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_run_status.py
+-rw-r--r--   0 anna       (501) staff       (20)     4350 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 anna       (501) staff       (20)     1103 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_spinner.py
+-rw-r--r--   0 anna       (501) staff       (20)    10751 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 anna       (501) staff       (20)     1677 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_types.py
+-rw-r--r--   0 anna       (501) staff       (20)     1001 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/mcli/utils/utils_yaml.py
+-rw-r--r--   0 anna       (501) staff       (20)     3887 2023-04-27 22:49:49.000000 mosaicml-cli-0.4.0a4/mcli/version.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.376085 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/
+-rw-r--r--   0 anna       (501) staff       (20)      698 2023-04-27 22:51:24.000000 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 anna       (501) staff       (20)     4708 2023-04-27 22:51:24.000000 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 anna       (501) staff       (20)        1 2023-04-27 22:51:24.000000 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 anna       (501) staff       (20)       75 2023-04-27 22:51:24.000000 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 anna       (501) staff       (20)     1546 2023-04-27 22:51:24.000000 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 anna       (501) staff       (20)        5 2023-04-27 22:51:24.000000 mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 anna       (501) staff       (20)    31087 2023-04-24 22:56:44.000000 mosaicml-cli-0.4.0a4/pyproject.toml
+-rw-r--r--   0 anna       (501) staff       (20)       38 2023-04-27 22:51:24.378935 mosaicml-cli-0.4.0a4/setup.cfg
+-rw-r--r--   0 anna       (501) staff       (20)     2965 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/setup.py
+drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-27 22:51:24.377298 mosaicml-cli-0.4.0a4/tests/
+-rw-r--r--   0 anna       (501) staff       (20)     5991 2023-04-27 22:33:50.000000 mosaicml-cli-0.4.0a4/tests/test_config.py
+-rw-r--r--   0 anna       (501) staff       (20)       62 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/tests/test_simple.py
+-rw-r--r--   0 anna       (501) staff       (20)     6116 2023-04-18 01:44:55.000000 mosaicml-cli-0.4.0a4/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.0a3/PKG-INFO` & `mosaicml-cli-0.4.0a4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.0a3
+Version: 0.4.0a4
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.0a3/README.md` & `mosaicml-cli-0.4.0a4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -131,21 +131,21 @@
 - To exit the virtual environment later on: `$ deactivate`
 - To get back into your virtual environment: `$ source venv/bin/activate`
 
 ## Running against mcloud as a developer
 
 There are currently 6 MCLI Modes. To use a mode other than the default `PROD`, set your local environment variable `MCLI_MODE` or specify the mode when you run MCLI commands (e.g. `MCLI_MODE=DEV mcli get runs`)
 
-| Mode       | Used By         | MAPI Endpoint                            | Use cases                                              | API Key                                                    |
-| ---------- | --------------- | ---------------------------------------- | ------------------------------------------------------ | ---------------------------------------------------------- |
-| `PROD`     | Default         | https://api.mosaicml.com/graphql         | Demos, simulating customer behavior, integration tests | Create one [here](https://cloud.mosaicml.com/account#)     |
-| `INTERNAL` | Internal users  | https://api.mosaicml.com/graphql         | Internal/alpha features in a prod environment          | Create one [here](https://cloud.mosaicml.com/account#)     |
-| `STAGING`  | Developers only | https://staging.api.mosaicml.com/graphql | Test changes queued for prod release                   | Testing api key                                            |
-| `DEV`      | Developers only | https://dev.api.mosaicml.com/graphql     | Test against dev branch of mcloud                      | Create one [here](https://dev.cloud.mosaicml.com/account#) |
-| `LOCAL`    | Developers only | http://localhost:3001/graphql            | Test local mcloud changes                              | Testing api key                                            |
+| Mode       | Used By         | MAPI Endpoint                            | Use cases                                              | API Key                                                      |
+| ---------- | --------------- | ---------------------------------------- | ------------------------------------------------------ | ------------------------------------------------------------ | --- |
+| `PROD`     | Default         | https://api.mosaicml.com/graphql         | Demos, simulating customer behavior, integration tests | Create one [here](https://console.mosaicml.com/account#)     |     |
+| `INTERNAL` | Internal users  | https://api.mosaicml.com/graphql         | Internal/alpha features in a prod environment          | Create one [here](https://console.mosaicml.com/account#)     |
+| `STAGING`  | Developers only | https://staging.api.mosaicml.com/graphql | Test changes queued for prod release                   | Testing api key                                              |
+| `DEV`      | Developers only | https://dev.api.mosaicml.com/graphql     | Test against dev branch of mcloud                      | Create one [here](https://dev.console.mosaicml.com/account#) |
+| `LOCAL`    | Developers only | http://localhost:3001/graphql            | Test local mcloud changes                              | Testing api key                                              |
 
 Note for almost all of these modes, you need to set an api key to talk to MAPI:
 
 ```bash
 mcli set api-key <value>
 ```
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.4.0a4/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/engine/engine.py` & `mosaicml-cli-0.4.0a4/mcli/api/engine/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -677,7 +677,50 @@
 
 def get_return_response(response, future: bool = False, timeout: Optional[float] = 10.0):
     if future:
         return response
 
     timeout = get_timeout(default_timeout=timeout)
     return response.result(timeout=timeout)
+
+
+def convert_plural_future_to_singleton(
+    future: Future[List[ModelT]],
+    error_message: Optional[str] = None,
+) -> Future[ModelT]:
+    """Convert a future for a list of models to a future for a single model
+
+    This is useful if you know that the query will only return one result, but
+    you want to use the same code to handle both cases.
+
+    Args:
+        future: A future that will resolve to a list of models
+        error_message: The error message to use if the plural future resolves to
+            an empty list. If None, no error will be raised. This is used can be used
+            resolvers that do not raise an error if nothing is found (eg getRuns)
+
+    Returns:
+        A future that will resolve to a single model
+
+    Raises:
+        MAPIException: If the plural future resolves to an empty list
+    """
+    future_obj: Future[ModelT] = Future()
+
+    def callback(f: Future[List[ModelT]]) -> None:
+        try:
+            res = f.result()
+        except Exception as e:  # pylint: disable=broad-except
+            # Propagate any exception to the new future
+            future_obj.set_exception(e)
+        else:
+            if res:
+                future_obj.set_result(res[0])
+
+            else:
+                # Most mapi mutation resolvers will raise their own error, this is for
+                # resolvers that do not raise an error if nothing is found (eg getRuns)
+                msg = error_message or 'No results found'
+                future_obj.set_exception(MAPIException(status=HTTPStatus.NOT_FOUND, message=msg))
+
+    future.add_done_callback(callback)
+    return future_obj
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/exceptions.py` & `mosaicml-cli-0.4.0a4/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """ API calls for deployment management """
 from mcli.api.inference_deployments.api_create_inference_deployment import create_inference_deployment
 from mcli.api.inference_deployments.api_delete_inference_deployments import delete_inference_deployments
+from mcli.api.inference_deployments.api_get_inference_deployment_logs import get_inference_deployment_logs
 from mcli.api.inference_deployments.api_get_inference_deployments import get_inference_deployments
 from mcli.api.inference_deployments.api_ping_inference_deployment import ping_inference_deployment
 from mcli.api.inference_deployments.api_predict_inference_deployment import predict
 from mcli.api.model.inference_deployment import InferenceDeployment
 from mcli.models import InferenceDeploymentConfig
 
 __all__ = [
     "InferenceDeployment",
     "InferenceDeploymentConfig",
     "create_inference_deployment",
     "delete_inference_deployments",
     "get_inference_deployments",
     "ping_inference_deployment",
+    "get_inference_deployment_logs",
     "predict",
 ]
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_ping_inference_deployment.py` & `mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_ping_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.4.0a4/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,13 +22,13 @@
         deployment: Inference deployment to send input to
         input: Input data to run prediction on in the form of dictionary
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised.
     Raises:
         HTTPError: If sending the request to the endpoint fails
     """
-    resp: Response = requests.post(url=f'https://{deployment.public_dns}/infer', timeout=timeout, json=inputs)
+    resp: Response = requests.post(url=f'https://{deployment.public_dns}/predict', timeout=timeout, json=inputs)
     if resp.ok:
         return resp.json()
     else:
         resp.raise_for_status()
         return {}
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/mint/shell.py` & `mosaicml-cli-0.4.0a4/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/mint/tty.py` & `mosaicml-cli-0.4.0a4/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/model/__init__.py` & `mosaicml-cli-0.4.0a4/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.4.0a4/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.4.0a4/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/model/run.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_run/m_run.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,227 +1,274 @@
-""" GraphQL representation of MCLIJob"""
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-from datetime import datetime
+""" mcli run Entrypoint """
+import argparse
+import logging
+import textwrap
 from http import HTTPStatus
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Optional
 
-from mcli.api.exceptions import MAPIException
-from mcli.api.schema.generic_model import DeserializableModel, convert_datetime
-from mcli.models.run_config import FinalRunConfig, RunConfig
+from mcli.api.exceptions import MAPIException, cli_error_handler
+from mcli.api.runs import create_run, delete_runs
+from mcli.api.runs.api_watch_run import EpilogSpinner as CloudEpilogSpinner
+from mcli.config import MCLIConfig
+from mcli.models.run_config import VALID_OPTIMIZATION_LEVELS
+from mcli.sdk import Run, RunConfig, follow_run_logs, get_run, start_run, wait_for_run_status
+from mcli.utils.utils_epilog import CommonLog
+from mcli.utils.utils_logging import INFO, OK
 from mcli.utils.utils_run_status import RunStatus
+from mcli.utils.utils_spinner import console_status
 
+logger = logging.getLogger(__name__)
 
-@dataclass
-class Node(DeserializableModel):
-    """Node linked to a run
-    """
-
-    rank: int
-    name: str
-
-    @classmethod
-    def from_mapi_response(cls, response: Dict[str, Any]) -> Node:
-        return Node(rank=response.get('rank', 0), name=response.get('name', 'Unknown'))
-
-    def to_dict(self):
-        return {"rank": str(self.rank), "name": self.name}
-
-
-@dataclass
-class Run(DeserializableModel):
-    """A run that has been launched on the MosaicML platform
-
-    Args:
-        run_uid (`str`): Unique identifier for the run
-        name (`str`): User-defined name of the run
-        status (:class:`~mcli.utils.utils_run_status.RunStatus`): Status of the run at a moment in time
-        created_at (`datetime`): Date and time when the run was created
-        updated_at (`datetime`): Date and time when the run was last updated
-        config (:class:`~mcli.models.run_config.RunConfig`): The
-            :class:`run configuration <mcli.models.run_config.RunConfig>` that was used to launch to the run
-
-        started_at (`Optional[datetime]`): Date and time when the run entered
-            the `STARTED` :class:`~mcli.utils.utils_run_status.RunStatus`
-        completed_at (`Optional[datetime]`): Date and time when the run entered
-            the `COMPLETED` :class:`~mcli.utils.utils_run_status.RunStatus`
-    """
-
-    run_uid: str
-    name: str
-    status: RunStatus
-    created_at: datetime
-    updated_at: datetime
-    config: FinalRunConfig
-    created_by: str
-
-    started_at: Optional[datetime] = None
-    completed_at: Optional[datetime] = None
-    reason: Optional[str] = None
-    nodes: List[Node] = field(default_factory=list)
-    submitted_config: Optional[RunConfig] = None
-    metadata: Optional[Dict[str, Any]] = None
-    last_attempt_id: Optional[str] = None
-
-    _required_properties: Tuple[str] = tuple([
-        'id',
-        'name',
-        'status',
-        'createdAt',
-        'updatedAt',
-        'runInput',
-        'createdByEmail',
-    ])
-
-    def clone(
-        self,
-        name: Optional[str] = None,
-        image: Optional[str] = None,
-        cluster: Optional[str] = None,
-        instance: Optional[str] = None,
-        nodes: Optional[int] = None,
-        gpu_type: Optional[str] = None,
-        gpus: Optional[int] = None,
-        priority: Optional[str] = None,
-    ) -> Run:
-        """
-        Submits a new run with the same configuration as this run
 
-        Args:
-            name (str): Override the name of the run
-            image (str): Override the image of the run
-            cluster (str): Override the cluster of the run
-            instance (str): Override the instance of the run
-            nodes (int): Override the number of nodes of the run
-            gpu_type (str): Override the GPU type of the run
-            gpus (int): Override the number of GPUs of the run
-            priority (str): Override the priority of the run
+def print_help(**kwargs) -> int:
+    del kwargs
+    mock_parser = argparse.ArgumentParser()
+    _configure_parser(mock_parser)
+    mock_parser.print_help()
+    return 1
 
-        Returns:
-            New :class:`~mcli.api.model.run.Run` object
-        """
-        # pylint: disable-next=import-outside-toplevel
-        from mcli.api.runs import create_run
 
-        submitted_config = self.submitted_config
-        if submitted_config is None:
-            refreshed_run = self.refresh()
-            submitted_config = refreshed_run.submitted_config
-
-        if not submitted_config:
-            raise MAPIException(
-                HTTPStatus.INTERNAL_SERVER_ERROR,
-                f'Could not find the submitted run config for run {self.name}',
-            )
-
-        if name:
-            submitted_config.name = name
-        if image:
-            submitted_config.image = image
-        if cluster:
-            submitted_config.compute['cluster'] = cluster
-        if instance:
-            submitted_config.compute['instance'] = instance
-        if nodes is not None:
-            submitted_config.compute['nodes'] = nodes
-        if gpu_type:
-            submitted_config.compute['gpu_type'] = gpu_type
-        if gpus is not None:
-            submitted_config.compute['gpus'] = gpus
-        if priority:
-            submitted_config.scheduling['priority'] = priority
+def follow_run(run: Run) -> int:
+    final_config = run.config
+    last_status: Optional[RunStatus] = None
 
-        return create_run(submitted_config)
+    with CloudEpilogSpinner(run, RunStatus.RUNNING) as watcher:
+        run = watcher.follow()
+        last_status = run.status
 
-    def refresh(self) -> Run:
-        """
-        Refreshes the data on the run object
+    # Wait timed out
+    common_log = CommonLog(logger)
+    if last_status is None:
+        common_log.log_timeout()
+        return 0
+    elif last_status == RunStatus.FAILED_PULL:
+        common_log.log_pod_failed_pull(run.name, final_config.image)
+        with console_status('Deleting failed run...'):
+            delete_runs([run])
+        return 1
+    elif last_status == RunStatus.FAILED:
+        common_log.log_pod_failed(run.name)
+        return 1
+    elif last_status.before(RunStatus.RUNNING):
+        common_log.log_unknown_did_not_start()
+        logger.debug(last_status)
+        return 1
 
-        Returns:
-            Refreshed :class:`~mcli.api.model.run.Run` object
-        """
-        # pylint: disable-next=import-outside-toplevel
-        from mcli.api.runs import get_run
+    logger.info(f'{OK} Run [cyan]{run.name}[/] started')
+    logger.info(f'{INFO} Following run logs. Press Ctrl+C to quit.\n')
 
-        return get_run(self)
+    end = ''
+    for line in follow_run_logs(run, rank=0):
+        print(line, end=end)
+    if not end:
+        print('')
 
-    def stop(self) -> Run:
-        """
-        Stops the run
+    wait_for_run_status(run, status=RunStatus.COMPLETED, timeout=10)
 
-        Returns:
-            Stopped :class:`~mcli.api.model.run.Run` object
-        """
-        # pylint: disable-next=import-outside-toplevel
-        from mcli.api.runs import stop_run
+    return 0
 
-        return stop_run(self)
 
-    def delete(self) -> Run:
-        """
-        Deletes the run
+def finish_run(run: Run, follow: bool, restarted: bool = False) -> int:
+    if not follow:
+        log_cmd = f'mcli logs {run.name}'
+        message = f"""
+        {OK} Run [cyan]{run.name}[/] {'re' if restarted else ''}submitted.
 
-        Returns:
-            Deleted :class:`~mcli.api.model.run.Run` object
-        """
-        # pylint: disable-next=import-outside-toplevel
-        from mcli.api.runs import delete_run
-        return delete_run(self)
-
-    def update_metadata(self, metadata: Dict[str, Any]) -> Run:
-        """
-        Updates the run's metadata
-    
-        Args:
-            metadata (`Dict[str, Any]`): The metadata to update the run with. This will be merged with
-                the existing metadata. Keys not specified in this dictionary will not be modified.
+        To see the run\'s status, use:
 
-        Returns:
-            Updated :class:`~mcli.api.model.run.Run` object
-        """
-        # pylint: disable-next=import-outside-toplevel
-        from mcli.api.runs import update_run_metadata
+        [bold]mcli get runs[/]
 
-        return update_run_metadata(self, metadata)
+        To see the run\'s logs, use:
 
-    @classmethod
-    def from_mapi_response(cls, response: Dict[str, Any]) -> Run:
-        missing = set(cls._required_properties) - set(response)
-        if missing:
-            raise MAPIException(
-                status=HTTPStatus.BAD_REQUEST,
-                message=f'Missing required key(s) in response to deserialize Run object: {", ".join(missing)}',
-            )
-
-        started_at = None
-        if response['startedAt'] is not None:
-            started_at = convert_datetime(response['startedAt'])
-
-        completed_at = None
-        if response['completedAt'] is not None:
-            completed_at = convert_datetime(response['completedAt'])
-
-        args = {
-            'run_uid': response['id'],
-            'name': response['name'],
-            'created_at': convert_datetime(response['createdAt']),
-            'started_at': started_at,
-            'completed_at': completed_at,
-            'updated_at': convert_datetime(response['updatedAt']),
-            'status': RunStatus.from_string(response['status']),
-            'created_by': response['createdByEmail'],
-            'config': FinalRunConfig.from_mapi_response(response['runInput']),
-            'nodes': [Node.from_mapi_response(n) for n in response.get('nodes', [])],
-            'reason': response['reason'],
-        }
-
-        details = response.get('details', {})
-        if details:
-            submitted_run_input = details.get('originalRunInput')
-            args['submitted_config'] = RunConfig.from_mapi_response(
-                submitted_run_input) if submitted_run_input is not None else None
-
-            args['metadata'] = details.get('metadata')
-            args['last_attempt_id'] = details.get('lastExecutionId')
-
-        return cls(**args)
+        [bold]{log_cmd}[/]
+        """
+        logger.info(textwrap.dedent(message).strip())
+        return 0
+    else:
+        return follow_run(run)
+
+
+# pylint: disable-next=too-many-statements
+@cli_error_handler('mcli run')
+def run_entrypoint(
+    file: Optional[str] = None,
+    restart_run: Optional[str] = None,
+    clone: Optional[str] = None,
+    follow: bool = True,
+    override_cluster: Optional[str] = None,
+    override_gpu_type: Optional[str] = None,
+    override_gpu_num: Optional[int] = None,
+    override_image: Optional[str] = None,
+    override_name: Optional[str] = None,
+    override_optimization_level: Optional[int] = None,
+    override_priority: Optional[str] = None,
+    override_nodes: Optional[int] = None,
+    override_instance: Optional[str] = None,
+    **kwargs,
+) -> int:
+    del kwargs
+
+    if file:
+        run_config = RunConfig.from_file(path=file)
+    elif clone:
+        run = get_run(clone)
+        if run.submitted_config is None:
+            raise MAPIException(HTTPStatus.NOT_FOUND, f"Could not retrieve configuration from run {clone}")
+        run_config = run.submitted_config
+    elif restart_run:
+        with console_status('Restarting run...'):
+            run = start_run(restart_run, timeout=None)
+
+        return finish_run(run, follow, restarted=True)
+
+    else:
+        return print_help()
+
+    # command line overrides
+    # only supports basic format for now and not structured params
+    if override_cluster is not None:
+        run_config.compute['cluster'] = override_cluster
+
+    if override_gpu_type is not None:
+        run_config.compute['gpu_type'] = override_gpu_type
+
+    if override_gpu_num is not None:
+        run_config.compute['gpus'] = override_gpu_num
+
+    if override_image is not None:
+        run_config.image = override_image
+
+    if override_name is not None:
+        run_config.name = override_name
+
+    if override_optimization_level is not None:
+        run_config.optimization_level = override_optimization_level
+
+    if override_priority is not None:
+        run_config.scheduling['priority'] = override_priority
+
+    if override_instance is not None:
+        run_config.compute['instance'] = override_instance
+
+    if override_nodes is not None:
+        run_config.compute['nodes'] = override_nodes
+
+    with console_status('Submitting run...'):
+        run = create_run(run=run_config, timeout=None)
+
+    return finish_run(run, follow)
+
+
+def add_run_argparser(subparser: argparse._SubParsersAction) -> None:
+    run_parser: argparse.ArgumentParser = subparser.add_parser(
+        'run',
+        aliases=['r'],
+        help='Launch a run in the MosaicML platform',
+    )
+    run_parser.set_defaults(func=run_entrypoint)
+    _configure_parser(run_parser)
+
+
+def _configure_parser(parser: argparse.ArgumentParser):
+    parser.add_argument(
+        '-f',
+        '--file',
+        dest='file',
+        help='File from which to load arguments.',
+    )
+
+    parser.add_argument(
+        '-r',
+        '--restart',
+        dest='restart_run',
+        help='Previously stopped run to start again',
+    )
+
+    parser.add_argument(
+        '--clone',
+        dest='clone',
+        help='Copy the run config from an existing run',
+    )
+
+    parser.add_argument(
+        '--priority',
+        dest='override_priority',
+        help='Priority level at which runs should be submitted. For low priority runs, '
+        'use "low" and for high priority runs use "high" '
+        '(default None)',
+    )
+
+    parser.add_argument(
+        '--no-follow',
+        action='store_false',
+        dest='follow',
+        default=False,
+        help='Do not automatically try to follow the run\'s logs. This is the default behavior',
+    )
+
+    parser.add_argument('--follow',
+                        action='store_true',
+                        dest='follow',
+                        default=False,
+                        help='Follow the logs of an in-progress run.')
+
+    parser.add_argument(
+        '--cluster',
+        '--platform',
+        dest='override_cluster',
+        help='Optional override for MCLI cluster',
+    )
+
+    parser.add_argument(
+        '--gpu-type',
+        dest='override_gpu_type',
+        help='Optional override for GPU type. Valid GPU type depend on'
+        ' the cluster and GPU number requested',
+    )
+
+    parser.add_argument(
+        '--gpus',
+        type=int,
+        dest='override_gpu_num',
+        help='Optional override for number of GPUs. Valid GPU numbers '
+        'depend on the cluster and GPU type',
+    )
+
+    parser.add_argument(
+        '--image',
+        dest='override_image',
+        help='Optional override for docker image',
+    )
+
+    parser.add_argument(
+        '--name',
+        '--run-name',
+        dest='override_name',
+        help='Optional override for run name',
+    )
+
+    parser.add_argument(
+        '--nodes',
+        type=int,
+        dest='override_nodes',
+        help='Optional override for number of nodes. '
+        'Valid node numbers depend on the cluster and instance type',
+    )
+
+    parser.add_argument(
+        '--instance',
+        dest='override_instance',
+        help='Optional override for instance type',
+    )
+
+    conf = MCLIConfig.load_config(safe=True)
+    if conf.internal:
+        parser.add_argument(
+            '-o',
+            '--optimization_level',
+            dest='override_optimization_level',
+            choices=VALID_OPTIMIZATION_LEVELS,
+            type=int,
+            help='Optimization level for auto-optimization agent. '
+            '0 to disable, 1 for safe system-level speedups, 2 for optimal speed at same accuracy, '
+            '3 for optimal accuracy at same speed',
+        )
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/runs/__init__.py` & `mosaicml-cli-0.4.0a4/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.4.0a4/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.4.0a4/mcli/api/runs/api_delete_runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ Delete a run. """
 from __future__ import annotations
 
 from concurrent.futures import Future
-from typing import List, Optional, Union, overload
+from typing import List, Optional, Union, cast, overload
 
 from typing_extensions import Literal
 
-from mcli.api.engine.engine import get_return_response, run_plural_mapi_request
+from mcli.api.engine.engine import convert_plural_future_to_singleton, get_return_response, run_plural_mapi_request
 from mcli.api.model.run import Run
 from mcli.config import MCLIConfig
 
 __all__ = ['delete_runs']
 
 QUERY_FUNCTION = 'deleteRuns'
 VARIABLE_DATA_NAME = 'getRunsData'
@@ -56,15 +56,21 @@
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the :type Run: output, use ``return_value.result()``
             with an optional ``timeout`` argument.
 
     Returns:
         A :type Run: for the run that was deleted
     """
-    return delete_runs([run], timeout=timeout, future=future)[0]  # type: ignore
+    runs = cast(Union[List[str], List[Run]], [run])
+
+    if future:
+        res = delete_runs(runs=runs, timeout=None, future=True)
+        return convert_plural_future_to_singleton(res)
+
+    return delete_runs(runs=runs, timeout=timeout, future=False)[0]
 
 
 @overload
 def delete_runs(runs: Union[List[str], List[Run]],
                 timeout: Optional[float] = 10,
                 future: Literal[False] = False) -> List[Run]:
     ...
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.4.0a4/mcli/api/runs/api_get_run_logs.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     cfg = MCLIConfig.load_config(safe=True)
     if cfg.user_id:
         filters['entity'] = {
             'userIds': [cfg.user_id],
         }
 
     variables = {VARIABLE_DATA_NAME: filters}
-    for message in _get_logs(QUERY, variables):
+    for message in _get_logs(QUERY, variables, QUERY_FUNCTION):
         if not future:
             try:
                 yield message.result(timeout)
             except StopAsyncIteration:
                 break
         else:
             yield message
@@ -167,51 +167,56 @@
     cfg = MCLIConfig.load_config(safe=True)
     if cfg.user_id:
         filters['entity'] = {
             'userIds': [cfg.user_id],
         }
 
     variables = {VARIABLE_DATA_NAME: filters}
-    for message in _get_logs(QUERY, variables):
+    for message in _get_logs(QUERY, variables, QUERY_FUNCTION):
         if not future:
             try:
                 yield message.result(timeout)
             except StopAsyncIteration:
                 break
         else:
             yield message
 
 
-def _get_logs(query: str, variables: Dict[str, Any]) -> Generator[Future[str], None, None]:
+def _get_logs(query: str, variables: Dict[str, Any], return_key: str) -> Generator[Future[str], None, None]:
 
     gql_query = gql.gql(query)
     connection = MAPIConnection.get_current_connection()
-    decoder = LogsDecoder()
+    decoder = LogsDecoder(return_key=return_key)
 
     for message in connection.subscribe(
             query=gql_query,
             variables=variables,
             callback=decoder.parse_message,
             retry_callback=decoder.update_offset,
     ):
         yield message
 
 
 class LogsDecoder(MessageDecoder):
     """Decode log messages and update read offset
     """
 
+    def __init__(self, return_key: str):
+        self.return_key = return_key
+        super().__init__()
+
     def update_offset(self, variables: Dict[str, Any]) -> Dict[str, Any]:
-        variables['getRunLogsInput']['offset'] = self.num_bytes_read
+        if self.return_key == "getRunLogs":
+            variables['getRunLogsInput']['offset'] = self.num_bytes_read
+        else:
+            variables['getInferenceDeploymentLogsInput']['offset'] = self.num_bytes_read
         return variables
 
     def parse_message(self, data: Dict[str, str]) -> str:
         """Get the next message from the GraphQL logging subscription
         """
-
         # Convert from base64 string to a bytestring
-        b64_message = data['getRunLogs']
-
+        b64_message = data['getRunLogs'] if self.return_key == "getRunLogs" else data['getInferenceDeploymentLogs']
         b64_bytes = b64_message.encode('utf8')
         message_bytes = base64.b64decode(b64_bytes)
 
         return self.decode(message_bytes)
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.4.0a4/mcli/api/runs/api_get_runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """get_runs SDK for MAPI"""
 from __future__ import annotations
 
 from concurrent.futures import Future
 from datetime import datetime
 from http import HTTPStatus
-from typing import List, Optional, Union, overload
+from typing import List, Optional, Union, cast, overload
 
 from typing_extensions import Literal
 
-from mcli.api.engine.engine import get_return_response, run_paginated_mapi_request, run_plural_mapi_request
+from mcli.api.engine.engine import (convert_plural_future_to_singleton, get_return_response, run_paginated_mapi_request,
+                                    run_plural_mapi_request)
 from mcli.api.exceptions import MAPIException
 from mcli.api.model.run import Run
 from mcli.config import MCLIConfig
 from mcli.models.gpu_type import GPUType
 from mcli.models.mcli_cluster import Cluster
 from mcli.utils.utils_run_status import RunStatus
 
@@ -43,24 +44,31 @@
     name
     status
     createdAt
     startedAt
     completedAt
     updatedAt
     reason
-    nodes {{
-        rank
-        name
-    }}
     createdByEmail
     runInput
     details {{
         originalRunInput
         metadata
         lastExecutionId
+        lifecycle {{
+            executionIndex
+            status
+            startTime
+            endTime
+            reason
+        }}
+        nodes {{
+            rank
+            name
+        }}
     }}
   }}
 }}
 """
 QUERY_FUNCTION_PAGINATED = 'getRunsPaginated'
 VARIABLE_DATA_NAME_PAGINATED = 'getRunsPaginatedData'
 QUERY_PAGINATED = f"""
@@ -126,17 +134,25 @@
             argument. To get the list of runs, use ``return_value.result()``
             with an optional ``timeout`` argument.
         include_details: If true, will fetch detailed information like run input for each run.
 
     Raises:
         MAPIException: If connecting to MAPI, raised when a MAPI communication error occurs
     """
-    res = get_runs(runs=[run], timeout=timeout, future=future, include_details=include_details)  # type: ignore
+
+    runs = cast(Union[List[str], List[Run]], [run])
+    error_message = f"Run {run.name if isinstance(run, Run) else run} not found"
+
+    if future:
+        res = get_runs(runs=runs, timeout=None, future=True, include_details=include_details)
+        return convert_plural_future_to_singleton(res, error_message)
+
+    res = get_runs(runs=runs, timeout=timeout, future=False, include_details=include_details)
     if not res:
-        raise MAPIException(HTTPStatus.NOT_FOUND, f"Run {run.name if isinstance(run, Run) else run} not found")
+        raise MAPIException(HTTPStatus.NOT_FOUND, error_message)
     return res[0]
 
 
 @overload
 def get_runs(
     runs: Optional[Union[List[str], List[Run]]] = None,
     cluster_names: Optional[Union[List[str], List[Cluster]]] = None,
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.4.0a4/mcli/api/runs/api_start_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ Start a run. """
 from __future__ import annotations
 
 from concurrent.futures import Future
-from typing import List, Optional, Union, overload
+from typing import List, Optional, Union, cast, overload
 
 from typing_extensions import Literal
 
-from mcli.api.engine.engine import get_return_response, run_plural_mapi_request
+from mcli.api.engine.engine import convert_plural_future_to_singleton, get_return_response, run_plural_mapi_request
 from mcli.api.model.run import Run
 from mcli.config import MCLIConfig
 
 __all__ = ['start_runs']
 
 QUERY_FUNCTION = 'startRuns'
 VARIABLE_DATA_NAME = 'getRunsData'
@@ -63,15 +63,21 @@
 
     Returns:
         If future is False:
             Started :class:`~mcli.api.model.run.Run` object
         Otherwise:
             A :class:`~concurrent.futures.Future` for the object
     """
-    return start_runs([run], timeout, future)[0]  # type: ignore
+    runs = cast(Union[List[str], List[Run]], [run])
+
+    if future:
+        res = start_runs(runs=runs, timeout=None, future=True)
+        return convert_plural_future_to_singleton(res)
+
+    return start_runs(runs=runs, timeout=timeout, future=False)[0]
 
 
 @overload
 def start_runs(runs: Union[List[str], List[Run]],
                timeout: Optional[float] = 10,
                future: Literal[False] = False) -> List[Run]:
     ...
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.4.0a4/mcli/api/runs/api_stop_runs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ Stop a run. """
 from __future__ import annotations
 
 from concurrent.futures import Future
-from typing import List, Optional, Union, overload
+from typing import List, Optional, Union, cast, overload
 
 from typing_extensions import Literal
 
-from mcli.api.engine.engine import get_return_response, run_plural_mapi_request
+from mcli.api.engine.engine import convert_plural_future_to_singleton, get_return_response, run_plural_mapi_request
 from mcli.api.model.run import Run
 from mcli.config import MCLIConfig
 
 __all__ = ['stop_runs']
 
 QUERY_FUNCTION = 'stopRuns'
 VARIABLE_DATA_NAME = 'getRunsData'
@@ -65,15 +65,21 @@
 
     Returns:
         If future is False:
             Stopped :class:`~mcli.api.model.run.Run` object
         Otherwise:
             A :class:`~concurrent.futures.Future` for the object
     """
-    return stop_runs([run], timeout, future)[0]  # type: ignore
+    runs = cast(Union[List[str], List[Run]], [run])
+
+    if future:
+        res = stop_runs(runs=runs, timeout=None, future=True)
+        return convert_plural_future_to_singleton(res)
+
+    return stop_runs(runs=runs, timeout=timeout, future=False)[0]
 
 
 @overload
 def stop_runs(runs: Union[List[str], List[Run]],
               timeout: Optional[float] = 10,
               future: Literal[False] = False) -> List[Run]:
     ...
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.4.0a4/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.4.0a4/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.4.0a4/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.4.0a4/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.4.0a4/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.4.0a4/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/typing_future.py` & `mosaicml-cli-0.4.0a4/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.4.0a4/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/cli.py` & `mosaicml-cli-0.4.0a4/mcli/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from mcli.cli.m_root.m_config import m_get_config
 from mcli.cli.m_run.m_run import add_run_argparser
 from mcli.cli.m_set_unset.m_set import add_set_argparser
 from mcli.cli.m_set_unset.m_unset import add_unset_argparser
 from mcli.cli.m_stop.m_stop import add_stop_parser
 from mcli.cli.m_util.m_util import add_util_argparser
 from mcli.config import FeatureFlag, MCLIConfig
-from mcli.utils.utils_cli import MCLIArgumentParser
+from mcli.utils.utils_cli import MCLIArgumentParser, SubmissionType
 from mcli.utils.utils_logging import console_handler
 from mcli.utils.utils_pypi import NeedsUpdateError, check_new_update_available
 from mcli.version import get_formatted_version, print_version
 
 logger = logging.getLogger('mcli')
 logger.setLevel(logging.INFO)
 logger.addHandler(console_handler)
@@ -109,15 +109,15 @@
         kube_interactive_argparser(subparser=subparser)
 
     add_create_argparser(subparser=subparser)
     add_delete_argparser(subparser=subparser)
     add_deploy_argparser(subparser=subparser)
     add_describe_parser(subparser=subparser)
     add_get_argparser(subparser=subparser, is_admin=is_admin)
-    add_log_parser(subparser=subparser)
+    add_log_parser(subparser=subparser, submission_type=SubmissionType.RUN)
     add_ping_parser(subparser=subparser)
     add_predict_parser(subparser=subparser)
     add_run_argparser(subparser=subparser)
     add_stop_parser(subparser=subparser)
     add_util_argparser(subparser=subparser)
     add_set_argparser(subparser=subparser, is_admin=is_admin)
     add_unset_argparser(subparser=subparser, is_admin=is_admin)
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.4.0a4/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.4.0a4/mcli/cli/common/run_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,31 @@
 
 
 def configure_submission_filter_argparser(action: str,
                                           parser: argparse.ArgumentParser,
                                           include_all: bool = True,
                                           submission_type: SubmissionType = SubmissionType.RUN):
 
-    parser.add_argument(
-        dest='name_filter',
-        nargs='*',
-        metavar=submission_type.value.upper(),
-        default=None,
-        help=f'String or glob of the name(s) of the {submission_type.value}(s) to {action}',
-    )
+    if submission_type == SubmissionType.DEPLOYMENT:
+        parser.add_argument(
+            '--name',
+            dest='name_filter',
+            nargs='*',
+            metavar=submission_type.value.upper(),
+            default=None,
+            help=f'String or glob of the name(s) of the {submission_type.value}(s) to {action}',
+        )
+    else:
+        parser.add_argument(
+            dest='name_filter',
+            nargs='*',
+            metavar=submission_type.value.upper(),
+            default=None,
+            help=f'String or glob of the name(s) of the {submission_type.value}(s) to {action}',
+        )
 
     parser.add_argument(
         '-c',
         '--cluster',
         '-p',
         '--platform',
         dest='cluster_filter',
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_delete/m_delete.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,22 +42,20 @@
     CLIExample(example='mcli delete runs --all', description='Delete all runs (Please be careful!)'),
 ]
 
 _deployments_description = Description("""
 Delete a deployment or set of deployments by name.
 """)
 
-_deployments_example_simple = CLIExample(example='mcli delete deployment deployment-name',
+_deployments_example_simple = CLIExample(example='mcli delete deployment --name deployment-name',
                                          description='Delete a specific deployment')
-_deployments_example_all = CLIExample(example='mcli delete deployment --all',
-                                      description='Delete all deployments (Please be careful!)')
 
-_deployments_examples = [_deployments_example_all, _deployments_example_simple]
+_deployments_examples = [_deployments_example_simple]
 
-_all_examples = [_secret_example_all, _run_example_simple, _run_example_status, _deployments_example_all]
+_all_examples = [_secret_example_all, _run_example_simple, _run_example_status]
 
 
 def delete(parser, **kwargs) -> int:
     del kwargs
     parser.print_help()
     return 0
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_describe/describe_runs.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from dataclasses import asdict, dataclass
 from enum import Enum
 from typing import Any, Dict, Generator, List, Optional, Tuple, TypeVar
 
 from rich.table import Table
 
 from mcli.api.exceptions import cli_error_handler
-from mcli.api.model.run import Node, Run
+from mcli.api.model.run import Node, Run, RunLifecycle
 from mcli.cli.m_get.display import (MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, create_vertical_display_table,
                                     format_timestamp)
 from mcli.models.run_config import DEFAULT_PRIORITY_NAME, ComputeConfig
 from mcli.sdk import get_run
-from mcli.utils.utils_logging import FormatString, console, format_string, print_timedelta
+from mcli.utils.utils_logging import FormatString, console, format_string, print_timedelta, seconds_to_str
 
 logger = logging.getLogger(__name__)
 
 DISPLAY_RUN_STATUSES = ['PENDING', 'RUNNING', 'COMPLETED']
 
 
 class DisplayRunStatus(Enum):
@@ -35,32 +35,21 @@
     GPU_TYPE = 'gpu_type'
     GPU_NUM = 'gpu_num'
     CPUS = 'cpus'
     IMAGE = 'image'
     PRIORITY = 'priority'
 
 
-class DescribeRunLifecycleColumns(Enum):
-    STATUS = 'status'
-    START_TIME = 'start_time'
-    END_TIME = 'end_time'
-    DURATION = 'duration'
-
-
 class DescribeRunOriginalInputColumns(Enum):
     SUBMITTED_CONFIG = 'submitted_config'
 
 
 RUN_DETAIL_DISPLAY_NAMES = ['Run Name', 'Run ID', 'Last Attempt ID', 'Cluster', 'Image', 'GPU Type', 'GPU Num']
 
-RUN_LIFECYCLE_DISPLAY_NAMES = [
-    'Start Time',
-    'End Time',
-    'Duration',
-]
+RUN_LIFECYCLE_DISPLAY_NAMES = ['Status', 'Reached At', 'Duration', 'Reason']
 RUN_NODES_DISPLAY_NAMES = ['Node Name']
 SUBMITTED_CONFIG = ['Run Config']
 
 
 @dataclass
 class DescribeRunDetailDisplayItem(MCLIDisplayItem):
     """Tuple that extracts detailed run data for display purposes"""
@@ -89,18 +78,19 @@
 
         return DescribeRunDetailDisplayItem(**extracted)
 
 
 @dataclass
 class DescribeRunLifecycleDisplayItem(MCLIDisplayItem):
     """Tuple that extracts run data for run lifecycle display purposes"""
+    attempt: str
     status: str
-    start_time: str
-    end_time: str
+    reached_at: str
     duration: str
+    reason: str
 
 
 @dataclass
 class DescribeRunMetadataDisplayItem(MCLIDisplayItem):
     """Tuple that extracts run metadata for display purposes"""
 
     key: str
@@ -133,29 +123,43 @@
             item = DescribeRunDetailDisplayItem.from_run(model)
             yield item
 
 
 class MCLIDescribeRunLifecycleDisplay(MCLIGetDisplay):
     """ Horizontal table view of run lifecycle """
 
-    def __init__(self, models: List[Run]):
-        self.model = models[0]
+    def __init__(self, model: List[RunLifecycle]):
+        self.model = model
+        self.include_reason_in_display = any(m.reason for m in model)
 
     @property
     def custom_column_names(self) -> List[str]:
-        return RUN_LIFECYCLE_DISPLAY_NAMES
+        if self.include_reason_in_display:
+            return RUN_LIFECYCLE_DISPLAY_NAMES
+        else:
+            return RUN_LIFECYCLE_DISPLAY_NAMES[:-1]
 
     def __iter__(self) -> Generator[DescribeRunLifecycleDisplayItem, None, None]:
-        for e in DisplayRunStatus:
-            item = format_run_status(e.value, self.model)
-            yield item
+        last_index: Optional[int] = None
+        for e in self.model:
+            duration = ''
+            if e.started_at and e.ended_at:
+                duration = print_timedelta(e.ended_at - e.started_at)
+            yield DescribeRunLifecycleDisplayItem(
+                attempt=str(e.attempt_id) if last_index != e.attempt_id else '',
+                status=e.status.display_name,
+                reached_at=format_timestamp(e.started_at),
+                duration=duration,
+                reason=e.reason or '',
+            )
+            last_index = e.attempt_id
 
     @property
     def index_label(self) -> str:
-        return 'status'
+        return 'attempt'
 
 
 class MCLIDescribeRunMetadataDisplay(MCLIGetDisplay):
     """ Vertical table view of run metadata """
 
     def __init__(self, metadata: Dict[str, Any]):
         self.columns = sorted(metadata.keys())
@@ -236,35 +240,14 @@
     def to_table(self) -> Table:
         data = {self.display_names.get(k, k.capitalize()): str(v) for k, v in asdict(self).items() if v is not None}
         columns = list(data.keys())
         values = [tuple(data.values())]
         return create_vertical_display_table(data=values, columns=columns)
 
 
-# Run lifecycle
-def format_run_status(status: str, run: Run) -> DescribeRunLifecycleDisplayItem:
-    if status == DisplayRunStatus.PENDING.value:
-        duration = print_timedelta(run.started_at - run.created_at) if run.started_at and run.created_at else '-'
-        return DescribeRunLifecycleDisplayItem(status=status,
-                                               start_time=format_timestamp(run.created_at),
-                                               end_time=format_timestamp(run.started_at),
-                                               duration=duration)
-    elif status == DisplayRunStatus.RUNNING.value:
-        duration = print_timedelta(run.completed_at - run.started_at) if run.completed_at and run.started_at else '-'
-        return DescribeRunLifecycleDisplayItem(status=status,
-                                               start_time=format_timestamp(run.started_at),
-                                               end_time=format_timestamp(run.completed_at),
-                                               duration=duration)
-    else:
-        return DescribeRunLifecycleDisplayItem(status=status,
-                                               start_time='--',
-                                               end_time=format_timestamp(run.completed_at),
-                                               duration='')
-
-
 @cli_error_handler("mcli describe run")
 def describe_run(run_name: str, output: OutputDisplay = OutputDisplay.TABLE, **kwargs):
     """
     Fetches more details of a Run
     """
     del kwargs
 
@@ -280,17 +263,21 @@
     print(format_string('Compute Requests', FormatString.BOLD))
     compute_display = DescribeComputeRequests.from_run(run)
     console.print(compute_display.to_table())
     print()
 
     # Run lifecycle section
     print(format_string('Run Lifecycle', FormatString.BOLD))
-    lifecycle_display = MCLIDescribeRunLifecycleDisplay([run])
+    lifecycle_display = MCLIDescribeRunLifecycleDisplay(run.lifecycle)
     lifecycle_display.print(output)
     print()
+    print(f'Total Attempts: {run.attempts:,}')
+    print(f'Total time spent in Pending: {seconds_to_str(run.cumulative_pending_time)}')
+    print(f'Total time spent in Running: {seconds_to_str(run.cumulative_running_time)}')
+    print()
 
     if run.metadata:
         print(format_string('Run Metadata', FormatString.BOLD))
         metadata_display = MCLIDescribeRunMetadataDisplay(run.metadata)
         metadata_display.print(output)
         print()
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_get/display.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_get/m_get.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from typing import List, Optional
 
 from mcli import config
 from mcli.cli.m_get import cli_get_secrets, get_clusters, get_users
 from mcli.cli.m_get.display import OutputDisplay
 from mcli.cli.m_get.inference_deployments import get_deployments_argparser
 from mcli.cli.m_get.runs import get_runs_argparser
+from mcli.cli.m_log.m_log import add_log_parser
 from mcli.models.mcli_secret import SecretType
+from mcli.utils.utils_cli import SubmissionType
 
 
 def get_entrypoint(parser, **kwargs) -> int:
     del kwargs
     parser.print_help()
     return 0
 
@@ -87,14 +89,18 @@
                                 dest='include_ids',
                                 default=config.ADMIN_MODE,
                                 help='Include the secret ids in the output')
     runs_parser = get_runs_argparser(subparsers)
     add_common_arguments(runs_parser)
     deployments_parser = get_deployments_argparser(subparsers)
     add_common_arguments(deployments_parser)
+    deployment_details_parsers = deployments_parser.add_subparsers(title='Deployment Details')
+
+    # mcli get run logs
+    add_log_parser(deployment_details_parsers, SubmissionType.DEPLOYMENT)
 
     return parser
 
 
 def add_get_argparser(subparser: argparse._SubParsersAction,
                       is_admin: bool = False,
                       parents: Optional[List[argparse.ArgumentParser]] = None) -> argparse.ArgumentParser:
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_get/users.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_init/m_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from mcli.utils.utils_interactive import secret_prompt
 from mcli.utils.utils_logging import OK
 from mcli.utils.utils_string_functions import validate_api_plaintext
 
 logger = logging.getLogger(__name__)
 
 DOCS_URL = 'https://mcli.docs.mosaicml.com'
-ACCOUNT_URL = 'https://cloud.mosaicml.com/account'
+ACCOUNT_URL = 'https://console.mosaicml.com/account'
 
 
 def initialize_mcli_config() -> MCLIConfig:
     """Initialize the MCLI config directory and file, if necessary
 
     Returns:
         True if MCLI needed to be initialized. False if initialization was already done.
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_init/m_init_kube.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_init/m_init_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/kube_config.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/kube_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_interactive/m_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_ping/m_ping.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,13 +42,13 @@
 
 def add_ping_parser(subparser: argparse._SubParsersAction):
     ping_parser: argparse.ArgumentParser = subparser.add_parser(
         'ping',
         help='Ping a inference deployment in the MosaicML platform for health metrics',
     )
     ping_parser.add_argument(
-        'inference_deployment_name',
+        'deployment_name',
         metavar='DEPLOYMENT',
         nargs='?',
         help='The name of the inference deployment. If not provided, will return the metrics of the latest deployment')
 
     ping_parser.set_defaults(func=ping)
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/cli/m_util/util.py` & `mosaicml-cli-0.4.0a4/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/config.py` & `mosaicml-cli-0.4.0a4/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/models/__init__.py` & `mosaicml-cli-0.4.0a4/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/models/gpu_type.py` & `mosaicml-cli-0.4.0a4/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.4.0a4/mcli/models/inference_deployment_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/models/mcli_envvar.py` & `mosaicml-cli-0.4.0a4/mcli/models/mcli_envvar.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/models/mcli_secret.py` & `mosaicml-cli-0.4.0a4/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/models/run_config.py` & `mosaicml-cli-0.4.0a4/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.4.0a4/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.4.0a4/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/sdk/__init__.py` & `mosaicml-cli-0.4.0a4/mcli/sdk/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 # pyright: reportUnusedImport=false
 # pylint: disable=useless-import-alias, disable=reimported
 
 from mcli.api.cluster import get_clusters
 from mcli.api.exceptions import MAPIException
 from mcli.api.inference_deployments import (InferenceDeployment, InferenceDeploymentConfig, create_inference_deployment,
-                                            delete_inference_deployments, get_inference_deployments,
-                                            ping_inference_deployment, predict)
+                                            delete_inference_deployments, get_inference_deployment_logs,
+                                            get_inference_deployments, ping_inference_deployment, predict)
 from mcli.api.runs import (FinalRunConfig, Run, RunConfig, RunStatus, create_run, delete_run, delete_runs,
                            follow_run_logs, get_run, get_run_logs, get_runs, start_run, start_runs, stop_run, stop_runs,
                            update_run_metadata, wait_for_run_status, watch_run_status)
 from mcli.api.secrets import create_secret, delete_secrets, get_secrets
 from mcli.cli.m_init.m_init import initialize
 from mcli.cli.m_set_unset.api_key import set_api_key
 from mcli.config import FeatureFlag, MCLIConfig
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_cli.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_config.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_date.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_docker.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_logging.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utils for logging"""
 import logging
 import textwrap
 from datetime import timedelta
 from enum import Enum
-from typing import List
+from typing import List, Union
 
 from rich import print as rprint
 from rich.console import Console
 from rich.highlighter import NullHighlighter
 from rich.logging import RichHandler
 from rich.tree import Tree
 from yaml.representer import SafeRepresenter
@@ -104,28 +104,44 @@
 
     text = ' '.join([strip(line) for line in text.splitlines() if strip(line) != ''])
     wrapped = textwrap.wrap(text, console.width - 2 * indent)
     block = textwrap.indent('\n'.join(wrapped), prefix=marker * indent)
     return block
 
 
-def print_timedelta(delta: timedelta):
-    # strftime cannot be used with timedelta
+def set_indent(text: str, indent: int, marker: str = ' ') -> str:
+    return textwrap.indent(textwrap.dedent(text), prefix=marker * indent)
 
-    seconds = delta.total_seconds()
+
+def seconds_to_str(seconds: Union[int, float]) -> str:
+    """Converts seconds to a human-readable string
+
+    Args:
+        seconds: Number of seconds
+
+    Returns:
+        Human-readable string
+    """
     if seconds < 60:
         return f'{int(seconds)}s'
     elif seconds < 3600:
         return f'{int(seconds/60)}min'
     elif seconds < 24 * 3600:
         return f'{int(seconds/3600)}hr'
     else:
         return f'{int(seconds/3600/24)}d'
 
 
+def print_timedelta(delta: timedelta) -> str:
+    # strftime cannot be used with timedelta
+
+    seconds = delta.total_seconds()
+    return seconds_to_str(seconds)
+
+
 def str_presenter(dumper: SafeRepresenter, data: str):
     """Converts multiline data into |\n<data>
     This is useful for displaying Run.command.
     """
     data = data.strip()
     if len(data.splitlines()) > 1:  # check for multiline string
         return dumper.represent_scalar('tag:yaml.org,2002:str', data, style='|')
```

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_rich.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_types.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.4.0a4/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/mcli/version.py` & `mosaicml-cli-0.4.0a4/mcli/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,13 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = "0.4.0a3"
+__version__ = "0.4.0a4"
+
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.0a3
+Version: 0.4.0a4
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 mcli/api/cluster/__init__.py
 mcli/api/cluster/api_get_clusters.py
 mcli/api/engine/__init__.py
 mcli/api/engine/engine.py
 mcli/api/inference_deployments/__init__.py
 mcli/api/inference_deployments/api_create_inference_deployment.py
 mcli/api/inference_deployments/api_delete_inference_deployments.py
+mcli/api/inference_deployments/api_get_inference_deployment_logs.py
 mcli/api/inference_deployments/api_get_inference_deployments.py
 mcli/api/inference_deployments/api_ping_inference_deployment.py
 mcli/api/inference_deployments/api_predict_inference_deployment.py
 mcli/api/mint/__init__.py
 mcli/api/mint/shell.py
 mcli/api/mint/tty.py
 mcli/api/model/__init__.py
@@ -142,12 +143,10 @@
 mcli/utils/utils_yaml.py
 mosaicml_cli.egg-info/PKG-INFO
 mosaicml_cli.egg-info/SOURCES.txt
 mosaicml_cli.egg-info/dependency_links.txt
 mosaicml_cli.egg-info/entry_points.txt
 mosaicml_cli.egg-info/requires.txt
 mosaicml_cli.egg-info/top_level.txt
-tests/__init__.py
-tests/conftest.py
 tests/test_config.py
 tests/test_simple.py
 tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.0a3/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.4.0a4/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -8,44 +8,44 @@
 pyyaml>=5.4.1
 questionary>=1.10.0
 rich>=10.16.2
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 
 [all]
-sphinxemoji>=0.2.0
-myst-parser>=0.16.1
-radon>=5.1.0
-pytest>=6.2.5
-pre-commit>=2.17.0
-sphinx_external_toc>=0.3.0
-sphinx-copybutton>=0.5.0
-pytest-mock>=3.7.0
-sphinx>=4.4.0
-pyright>=1.1.256
-sphinx-design
-sphinx-markdown-tables>=0.0.15
-sphinxcontrib-serializinghtml>=1.1.5
-sphinxcontrib-jsmath>=1.0.1
-sphinxcontrib-qthelp>=1.0.3
-toml>=0.10.2
-sphinx-panels>=0.6.0
-sphinxcontrib-images>=0.9.4
 sphinxcontrib-katex>=0.8.6
 isort>=5.9.3
-pytest-cov>=4.0.0
-sphinx-rtd-theme>=1.0.0
-sphinxcontrib-applehelp>=1.0.2
-sphinxcontrib-htmlhelp>=2.0.0
 sphinx-argparse>=0.3.1
 yapf>=0.33.0
-pylint>=2.12.2
+sphinxcontrib-images>=0.9.4
+sphinxcontrib-qthelp>=1.0.3
+sphinx-design
+sphinxcontrib-serializinghtml>=1.1.5
+toml>=0.10.2
+sphinxcontrib-applehelp>=1.0.2
+sphinx-copybutton>=0.5.0
+pre-commit>=2.17.0
+sphinx-markdown-tables>=0.0.15
 sphinxext-opengraph>=0.6.1
-furo>=2022.3.4
+sphinxcontrib-jsmath>=1.0.1
+pylint>=2.12.2
+sphinxcontrib-htmlhelp>=2.0.0
+sphinxemoji>=0.2.0
+sphinx-panels>=0.6.0
+sphinx-rtd-theme>=1.0.0
 sphinxcontrib-devhelp>=1.0.2
+furo>=2022.3.4
+pytest>=6.2.5
+radon>=5.1.0
+pytest-mock>=3.7.0
+myst-parser>=0.16.1
+pyright>=1.1.256
+sphinx>=4.4.0
+sphinx_external_toc>=0.3.0
+pytest-cov>=4.0.0
 
 [dev]
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright>=1.1.256
 pytest-cov>=4.0.0
```

### Comparing `mosaicml-cli-0.4.0a3/pyproject.toml` & `mosaicml-cli-0.4.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/setup.py` & `mosaicml-cli-0.4.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/tests/test_config.py` & `mosaicml-cli-0.4.0a4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.0a3/tests/test_upgrade.py` & `mosaicml-cli-0.4.0a4/tests/test_upgrade.py`

 * *Files identical despite different names*

