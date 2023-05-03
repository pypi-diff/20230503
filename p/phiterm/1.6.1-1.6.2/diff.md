# Comparing `tmp/phiterm-1.6.1.tar.gz` & `tmp/phiterm-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiterm-1.6.1.tar", last modified: Tue Apr 18 15:39:39 2023, max compression
+gzip compressed data, was "phiterm-1.6.2.tar", last modified: Wed May  3 15:16:00 2023, max compression
```

## Comparing `phiterm-1.6.1.tar` & `phiterm-1.6.2.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.585495 phiterm-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-18 15:39:18.000000 phiterm-1.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 15:39:39.585495 phiterm-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 15:39:18.000000 phiterm-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/aws/aws_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/cli_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/dx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/dx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/dx/dx_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/gcp/gcp_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/gcp/gke/gke_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/k8s/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/wf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/wf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/wf/wf_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35058 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/ws/ws_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/conf/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/conf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/conf/phi_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/databox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/databox/databox_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/docker/docker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/enums/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/tbd_k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/tbd_k8s_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/tbd_k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/tbd_phi_k8s_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/local/local_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/release/release_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/release/release_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/release/ws_releases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/schemas/user_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/schemas/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.569496 phiterm-1.6.1/phiterm/tbd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/tbd/backend_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/backend_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/backend_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/backend_api/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/backend_api/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/backend_api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/backend_api/workspace_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.581495 phiterm-1.6.1/phiterm/tbd/tbd_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_zones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.581495 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gke/gke_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gke/gke_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/phi_gcp_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.581495 phiterm-1.6.1/phiterm/tbd/tbd_old_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_old_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_old_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_old_api/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_old_api/kubectl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.581495 phiterm-1.6.1/phiterm/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.581495 phiterm-1.6.1/phiterm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/cli_auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/ws_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.581495 phiterm-1.6.1/phiterm/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workflow/wf_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workflow/wf_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workflow/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.585495 phiterm-1.6.1/phiterm/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/phi_ws_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/ws_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/ws_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    40282 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/ws_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/ws_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/ws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 15:39:39.000000 phiterm-1.6.1/phiterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-18 15:39:39.000000 phiterm-1.6.1/phiterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:39:39.000000 phiterm-1.6.1/phiterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 15:39:39.000000 phiterm-1.6.1/phiterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-18 15:39:39.000000 phiterm-1.6.1/phiterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 15:39:39.000000 phiterm-1.6.1/phiterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-18 15:39:18.000000 phiterm-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:39:39.585495 phiterm-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 15:39:18.000000 phiterm-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.585495 phiterm-1.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-18 15:39:18.000000 phiterm-1.6.1/tests/test_backend_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.010510 phiterm-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-03 15:15:40.000000 phiterm-1.6.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 15:16:00.006509 phiterm-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-03 15:15:40.000000 phiterm-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.990508 phiterm-1.6.2/phiterm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/aws/aws_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/cli_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/dx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/dx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/dx/dx_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/gcp/gcp_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/gcp/gke/gke_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/k8s/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/wf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/wf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/wf/wf_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35062 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/ws/ws_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/conf/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/conf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/conf/phi_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/databox/databox_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/docker/docker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/enums/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/tbd_k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/tbd_k8s_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/tbd_k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/tbd_phi_k8s_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/local/local_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/release/release_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/release/release_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/release/ws_releases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/schemas/user_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/schemas/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.990508 phiterm-1.6.2/phiterm/tbd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.002509 phiterm-1.6.2/phiterm/tbd/backend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/backend_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/backend_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/backend_api/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/backend_api/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/backend_api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/backend_api/workspace_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.002509 phiterm-1.6.2/phiterm/tbd/tbd_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.002509 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gke/gke_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gke/gke_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/phi_gcp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.002509 phiterm-1.6.2/phiterm/tbd/tbd_old_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_old_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_old_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_old_api/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_old_api/kubectl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.002509 phiterm-1.6.2/phiterm/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.006509 phiterm-1.6.2/phiterm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/cli_auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/ws_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.006509 phiterm-1.6.2/phiterm/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workflow/wf_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workflow/wf_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workflow/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.006509 phiterm-1.6.2/phiterm/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/phi_ws_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/ws_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/ws_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40288 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/ws_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/ws_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/ws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.990508 phiterm-1.6.2/phiterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 15:15:59.000000 phiterm-1.6.2/phiterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-03 15:15:59.000000 phiterm-1.6.2/phiterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:15:59.000000 phiterm-1.6.2/phiterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 15:15:59.000000 phiterm-1.6.2/phiterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-03 15:15:59.000000 phiterm-1.6.2/phiterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 15:15:59.000000 phiterm-1.6.2/phiterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-03 15:15:40.000000 phiterm-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:16:00.010510 phiterm-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-03 15:15:40.000000 phiterm-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.006509 phiterm-1.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 15:15:40.000000 phiterm-1.6.2/tests/test_backend_api.py
```

### Comparing `phiterm-1.6.1/LICENSE.md` & `phiterm-1.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/api/client.py` & `phiterm-1.6.2/phiterm/api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/api/routes.py` & `phiterm-1.6.2/phiterm/api/routes.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/api/user.py` & `phiterm-1.6.2/phiterm/api/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/api/workspace.py` & `phiterm-1.6.2/phiterm/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/aws/aws_operator.py` & `phiterm-1.6.2/phiterm/aws/aws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/cli/cli_app.py` & `phiterm-1.6.2/phiterm/cli/cli_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 cli_app = typer.Typer(
     help="""\b
 Phidata is a toolkit for building data products as code.
 \b
 Get started:
 1. Run `phi init` to init phidata on this machine
-2. Run `phi ws init` to create a new workspace
+2. Run `phi ws create` to create a new workspace
 3. Run `phi ws setup` to setup an existing workspace
 4. Run `phi ws up` to deploy the active workspace
 5. Run `phi ws down` to shutdown the active workspace
 """,
     no_args_is_help=True,
     add_completion=False,
     invoke_without_command=True,
```

### Comparing `phiterm-1.6.1/phiterm/cli/cli_operator.py` & `phiterm-1.6.2/phiterm/cli/cli_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
     # Authenticate user
     if login:
         auth_success = authenticate_user()
 
     if phi_conf is not None:
         print_info("Phidata is initialized. Next steps:\n")
-        print_info(" 1. Run `phi ws init` to create a new workspace")
+        print_info(" 1. Run `phi ws create` to create a new workspace")
         print_info(" 2. Run `phi ws setup` to setup an existing workspace")
         print_info(" 3. Run `phi ws up -dr` to dry-run workspace deploy")
         print_info(" 4. Run `phi ws up` to deploy the workspace")
     return True
 
 
 def sign_in_using_cli() -> bool:
```

### Comparing `phiterm-1.6.1/phiterm/cli/dx/dx_app.py` & `phiterm-1.6.2/phiterm/cli/dx/dx_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/cli/gcp/gcp_app.py` & `phiterm-1.6.2/phiterm/cli/gcp/gcp_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/cli/gcp/gke/gke_app.py` & `phiterm-1.6.2/phiterm/cli/gcp/gke/gke_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/cli/k8s/k8s_app.py` & `phiterm-1.6.2/phiterm/cli/k8s/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/cli/wf/wf_app.py` & `phiterm-1.6.2/phiterm/cli/wf/wf_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/cli/ws/ws_app.py` & `phiterm-1.6.2/phiterm/cli/ws/ws_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 ):
     """\b
     Creates a new workspace in the current directory using the selected starter template
     [default: ml-app]
 
     \b
     Examples:
-    $ phi ws init            -> Create a new workspace
-    $ phi ws init -ws ml     -> Create a workspace named data using the default starter template (aws)
+    $ phi ws create            -> Create a new workspace
+    $ phi ws create -ws ml     -> Create a workspace named data using the default starter template (aws)
     """
     from phiterm.workspace.ws_operator import (
         create_new_workspace,
         initialize_workspace,
     )
 
     if print_debug_log:
```

### Comparing `phiterm-1.6.1/phiterm/conf/auth.py` & `phiterm-1.6.2/phiterm/conf/auth.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/conf/constants.py` & `phiterm-1.6.2/phiterm/conf/constants.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/conf/phi_conf.py` & `phiterm-1.6.2/phiterm/conf/phi_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
         Notes:
         * ws_name is the only required argument.
         * This function does not call self.save_config(). call it from the parent.
 
         This function is called from 5 places:
         1. During `phi login` when active/available workspaces are requested from the api.
-        2. During `phi ws init` when a new workspace is created on the users machine.
+        2. During `phi ws create` when a new workspace is created on the users machine.
         3. When the user already has a local workspace on their machine
             and adds the ws manually using `phi ws setup`
             (possible after running `phi init -r` which deletes the config)
         4. Whenever ws config, creds or data needs to be refreshed. This function is called with just the `ws_name` arg
         5. When active or available workspaces are updated, this function is called from the
             @active_ws_name.setter and @available_ws.setter with the ws_name and ws_schema
         """
@@ -446,15 +446,15 @@
 
     def print_to_cli(self):
         if self.user:
             print_heading(f"User: {self.user.email}")
         if self.active_ws_name:
             print_heading(f"\nActive workspace: {self.active_ws_name}\n")
         else:
-            print_info("* No active workspace, run `phi ws init` to create one")
+            print_info("* No active workspace, run `phi ws create` to create one")
         # if len(self._ws_data_map) > 0:
         #     print_heading("Available workspaces:\n")
         #     c = 1
         #     for k, v in self._ws_data_map.items():
         #         print_info(f"  {c}. Name: {v.ws_name}")
         #         print_info(f"     Dir: {v.ws_root_path}")
         #         if v.ws_schema:
```

### Comparing `phiterm-1.6.1/phiterm/databox/databox_operator.py` & `phiterm-1.6.2/phiterm/databox/databox_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/docker/docker_operator.py` & `phiterm-1.6.2/phiterm/docker/docker_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/enums/user.py` & `phiterm-1.6.2/phiterm/enums/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/k8s/k8s_operator.py` & `phiterm-1.6.2/phiterm/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/k8s/tbd_k8s_operator.py` & `phiterm-1.6.2/phiterm/k8s/tbd_k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/k8s/tbd_k8s_ops.py` & `phiterm-1.6.2/phiterm/k8s/tbd_k8s_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/k8s/tbd_k8s_utils.py` & `phiterm-1.6.2/phiterm/k8s/tbd_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/k8s/tbd_phi_k8s_data.py` & `phiterm-1.6.2/phiterm/k8s/tbd_phi_k8s_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/local/local_operator.py` & `phiterm-1.6.2/phiterm/local/local_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/release/release_schemas.py` & `phiterm-1.6.2/phiterm/release/release_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/release/ws_releases.py` & `phiterm-1.6.2/phiterm/release/ws_releases.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/schemas/user.py` & `phiterm-1.6.2/phiterm/schemas/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/schemas/user_schemas.py` & `phiterm-1.6.2/phiterm/schemas/user_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/schemas/workspace.py` & `phiterm-1.6.2/phiterm/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/backend_api/api_client.py` & `phiterm-1.6.2/phiterm/tbd/backend_api/api_client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/backend_api/api_utils.py` & `phiterm-1.6.2/phiterm/tbd/backend_api/api_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/backend_api/auth_api.py` & `phiterm-1.6.2/phiterm/tbd/backend_api/auth_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/backend_api/workspace_api.py` & `phiterm-1.6.2/phiterm/tbd/backend_api/workspace_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_enums.py` & `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_operator.py` & `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_schemas.py` & `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_utils.py` & `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_zones.py` & `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_zones.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gke/gke_operator.py` & `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gke/gke_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gke/gke_utils.py` & `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gke/gke_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/tbd_gcp/phi_gcp_data.py` & `phiterm-1.6.2/phiterm/tbd/tbd_gcp/phi_gcp_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py` & `phiterm-1.6.2/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/tbd_old_api/client.py` & `phiterm-1.6.2/phiterm/tbd/tbd_old_api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/tbd_old_api/gcp.py` & `phiterm-1.6.2/phiterm/tbd/tbd_old_api/gcp.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/tbd/tbd_old_api/kubectl.py` & `phiterm-1.6.2/phiterm/tbd/tbd_old_api/kubectl.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/utils/cli_auth_server.py` & `phiterm-1.6.2/phiterm/utils/cli_auth_server.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/utils/cli_console.py` & `phiterm-1.6.2/phiterm/utils/cli_console.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 def print_generic_error_msg() -> None:
     console.print("Something went wrong, please try again", style=error_style)
 
 
 def log_ws_not_available_msg():
     logger.warning("No active workspace")
     logger.warning("Set a workspace as active using `phi set [ws_name]`")
-    logger.warning("Or run `phi ws init` to create a new workspace")
+    logger.warning("Or run `phi ws create` to create a new workspace")
 
 
 def log_network_error_msg() -> None:
     logger.debug("NetworkError. Could not reach phidata servers.")
 
 
 def log_server_error_msg() -> None:
@@ -93,15 +93,15 @@
 
 def log_auth_error_msg() -> None:
     logger.debug("AuthError: could not authenticate, please run `phi auth` again")
 
 
 def print_active_workspace_not_available() -> None:
     print_warning("No active workspace")
-    print_warning("Run `phi ws init` to create a new workspace")
+    print_warning("Run `phi ws create` to create a new workspace")
     print_warning(
         "Run `phi ws setup` from an existing workspace directory to setup the workspace"
     )
     print_warning("Or set an existing workspace as active using `phi set [ws_name]`")
 
 
 def print_available_workspaces(avl_ws_list) -> None:
```

### Comparing `phiterm-1.6.1/phiterm/utils/common.py` & `phiterm-1.6.2/phiterm/utils/common.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/utils/dttm.py` & `phiterm-1.6.2/phiterm/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/utils/enums.py` & `phiterm-1.6.2/phiterm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/utils/filesystem.py` & `phiterm-1.6.2/phiterm/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/utils/git.py` & `phiterm-1.6.2/phiterm/utils/git.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/utils/load_env.py` & `phiterm-1.6.2/phiterm/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/utils/log.py` & `phiterm-1.6.2/phiterm/utils/log.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/utils/pyproject.py` & `phiterm-1.6.2/phiterm/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/utils/ws_filter.py` & `phiterm-1.6.2/phiterm/utils/ws_filter.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/workflow/wf_operator.py` & `phiterm-1.6.2/phiterm/workflow/wf_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/workflow/wf_utils.py` & `phiterm-1.6.2/phiterm/workflow/wf_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/workspace/phi_ws_data.py` & `phiterm-1.6.2/phiterm/workspace/phi_ws_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         loaded_config: WorkspaceConfig = load_workspace(ws_root_path=self.ws_root_path)
 
         # Update cached_ws_config
         self.cached_ws_config = loaded_config
         self.cached_ws_config.workspace_root_path = self.ws_root_path
         self.cached_ws_config.workspace_config_file_path = self.ws_config_file_path
 
-        logger.debug("WorkspaceConfig:\n{}".format(self.cached_ws_config.args))
+        logger.debug("WorkspaceConfig: {}".format(self.cached_ws_config.args))
         return self.cached_ws_config
 
     ######################################################
     ## Print functions
     ######################################################
 
     def print_to_cli(self):
```

### Comparing `phiterm-1.6.1/phiterm/workspace/ws_enums.py` & `phiterm-1.6.2/phiterm/workspace/ws_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/workspace/ws_loader.py` & `phiterm-1.6.2/phiterm/workspace/ws_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,29 +53,34 @@
         logger.debug(f"--^^-- Loading workspace from: {config_dir_path}")
         workspace_config_objects = {}
         config_files = config_dir_path.rglob("*.py")
         for _config_file in config_files:
             if _config_file.name == "__init__.py":
                 continue
             logger.debug(f"Reading file: {_config_file}")
+            parent_dir = _config_file.parent.name
+            if parent_dir in ("resources", "tests"):
+                logger.debug(f"Skipping file in {parent_dir}")
+                continue
             try:
                 python_objects = get_python_objects_from_module(_config_file)
                 for obj_name, obj in python_objects.items():
                     _type_name = obj.__class__.__name__
                     if _type_name in [
                         "WorkspaceSettings",
                         "DockerConfig",
                         "K8sConfig",
                         "AwsConfig",
                     ]:
                         workspace_config_objects[obj_name] = obj
             except Exception as e:
+                logger.warning(f"Error in {_config_file}: {e}")
                 pass
 
-        logger.debug(f"workspace_config_objects: {workspace_config_objects}")
+        # logger.debug(f"workspace_config_objects: {workspace_config_objects}")
         for obj_name, obj in workspace_config_objects.items():
             _obj_type = obj.__class__.__name__
             logger.debug(f"Adding {obj_name}: | Type: {_obj_type}")
             if _obj_type == "WorkspaceSettings":
                 ws_config.ws_settings = obj
                 try:
                     ws_config.default_env = obj.dev_env
```

### Comparing `phiterm-1.6.1/phiterm/workspace/ws_operator.py` & `phiterm-1.6.2/phiterm/workspace/ws_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     )
     create_new_workspace(ws_name_inp_raw, template)
 
 
 def initialize_workspace() -> None:
     """Initialize a phidata workspace.
 
-    This function is called by `phi ws init` to create a new workspace.
+    This function is called by `phi ws create` to create a new workspace.
     """
     phi_conf: Optional[PhiConf] = PhiConf.get_saved_conf()
     if not phi_conf:
         print_conf_not_available_msg()
         return
 
     print_heading("New phidata workspace")
@@ -217,15 +217,15 @@
     1.4 Check if this is the active workspace or if it needs to be set as active
     1.5 Check if remote origin is available
 
     2. Create or Update WorkspaceSchema
     If a ws_schema exists for this workspace, this workspace has been setup before
     2.1 Create WorkspaceSchema for a NEWLY CREATED WORKSPACE
         If ws_schema is None, this is a NEWLY CREATED WORKSPACE.
-        i.e. A new workspace was created using create_new_workspace() <- which is called using `phi ws init`.
+        i.e. A new workspace was created using create_new_workspace() <- which is called using `phi ws create`.
         This ws does not have a ws_schema, make an api call to create one.
         If the api call returns None, then we could not create the workspace.
     2.2 Update WorkspaceSchema if ws_schema exists
     2.3 Set as active if needed
     2.4 Refresh PhiWsData
 
     3. Complete Workspace setup
@@ -962,15 +962,15 @@
 #
 #     # Check if we can create the workspace in the current dir
 #     current_dir: Path = Path("../../workspace").resolve()
 #     logger.debug(f"current_dir: {current_dir}")
 #     ws_root_path: Path = current_dir.joinpath(ws_to_clone.name)
 #     if ws_root_path.exists():
 #         logger.error(
-#             f"{ws_root_path} already exists, please choose another directory to clone or delete the existing dir and run `phi ws init` again"
+#             f"{ws_root_path} already exists, please choose another directory to clone or delete the existing dir and run `phi ws create` again"
 #         )
 #         return
 #
 #     print_info(f"Creating {str(ws_root_path)}")
 #     # Clone the workspace repo in ws_root_path
 #     repo_to_clone = ws_to_clone.git_url
 #     _cloned_git_repo: git.Repo = git.Repo.clone_from(
```

### Comparing `phiterm-1.6.1/phiterm/workspace/ws_schemas.py` & `phiterm-1.6.2/phiterm/workspace/ws_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/phiterm/workspace/ws_utils.py` & `phiterm-1.6.2/phiterm/workspace/ws_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,35 +126,35 @@
     #         False,
     #         "Version control provider not available. Please run `phi init -r` to initialize phi",
     #     )
 
     if ws_data is None:
         return (
             False,
-            "WorkspaceSchema not yet registered with Phidata. Please run `phi ws init` to create a new workspace or `phi ws setup` for an existing workspace",
+            "WorkspaceSchema not yet registered with Phidata. Please run `phi ws create` to create a new workspace or `phi ws setup` for an existing workspace",
         )
 
     # Validate WorkspaceSchema Directory
     ws_root_path: Optional[Path] = ws_data.ws_root_path
     if ws_root_path is None or not ws_root_path.exists() or not ws_root_path.is_dir():
         return (
             False,
-            "The WorkspaceSchema directory is not available or invalid.\n\tTo create a new workspace, run `phi ws init`.\n\tFor an existing workspace, run `phi ws setup` from the workspace directory",
+            "The WorkspaceSchema directory is not available or invalid.\n\tTo create a new workspace, run `phi ws create`.\n\tFor an existing workspace, run `phi ws setup` from the workspace directory",
         )
 
     # Validate WorkspaceSchema Config Exists (we will validate the contents later)
     ws_config_file_path: Optional[Path] = ws_data.ws_config_file_path
     if (
         ws_config_file_path is None
         or not ws_config_file_path.exists()
         or not ws_config_file_path.is_file()
     ):
         return (
             False,
-            "WorkspaceSchema config is not available or invalid. Please run `phi ws init` to create a new workspace or `phi ws setup` for an existing workspace",
+            "WorkspaceSchema config is not available or invalid. Please run `phi ws create` to create a new workspace or `phi ws setup` for an existing workspace",
         )
 
     # Validate that the workspace is registered with phidata
     if ws_data is not None and ws_data.ws_schema is None:
         return (
             False,
             "WorkspaceSchema not registered with phidata. Please run `phi ws setup` from the workspace dir",
```

### Comparing `phiterm-1.6.1/phiterm.egg-info/SOURCES.txt` & `phiterm-1.6.2/phiterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.1/pyproject.toml` & `phiterm-1.6.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phiterm"
-version = "1.6.1"
+version = "1.6.2"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
```

