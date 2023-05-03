# Comparing `tmp/codalab-1.6.2.tar.gz` & `tmp/codalab-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/codalab-1.6.2.tar", last modified: Tue Mar 21 19:18:26 2023, max compression
+gzip compressed data, was "dist/codalab-1.6.3.tar", last modified: Wed May  3 06:01:34 2023, max compression
```

## Comparing `codalab-1.6.2.tar` & `codalab-1.6.3.tar`

### file list

```diff
@@ -1,191 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-21 18:50:42.000000 codalab-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-21 19:18:26.000000 codalab-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-21 18:50:42.000000 codalab-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bin/bundle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bin/cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bin/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bin/ws_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab/bundles/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bundles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bundles/dataset_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bundles/derived_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bundles/make_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bundles/named_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bundles/private_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bundles/program_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bundles/run_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/bundles/uploaded_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27650 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/client/json_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab/lib/beam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/beam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/beam/blobstorageuploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/beam/filesystems.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/beam/mockblobstoragefilesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/beam/streamingzipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/bundle_action.py
--rw-r--r--   0 runner    (1001) docker     (123)   175230 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/bundle_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/bundle_fuse.py
--rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/bundle_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    17635 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/bundle_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/canonicalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    21487 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/codalab_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/completers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/crypt_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18423 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/editor_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/emailer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/interactive_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/metadata_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/metadata_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/path_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/print_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/profiling_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/server_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/spec_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/telemetry_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/ui_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/unicode_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25561 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/upload_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    47933 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/worksheet_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/lib/zip_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   133917 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/model/bundle_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/model/mysql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/model/orm_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/model/sqlite_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21321 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/model/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/model/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/model/worker_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/objects/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/objects/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/objects/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/objects/metadata_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/objects/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/objects/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/objects/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/objects/worksheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab/rest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/bundle_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    59093 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    31534 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/interpret.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/worksheet_block_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    20603 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/rest/worksheets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/server/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/server/authenticated_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    51850 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/server/bundle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/server/cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/server/json_api_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    35051 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/server/oauth2_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/server/rest_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/server/worker_info_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/bundle_service_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/bundle_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    30942 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/docker_image_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18090 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/download_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/fsm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/image_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/noop_image_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/pyjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/rest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab/worker/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/runtime/kubernetes_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/singularity_image_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/state_committer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/tar_file_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/tar_subdir_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/un_gzip_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/un_tar_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/upload_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    40004 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/worker_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)    36035 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/worker_run_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker/worker_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab/worker_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker_manager/aws_batch_worker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker_manager/azure_batch_worker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker_manager/kubernetes_worker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker_manager/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker_manager/slurm_batch_worker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab/worker_manager/worker_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-21 19:18:26.000000 codalab-1.6.2/codalab.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    40133 2023-03-21 18:50:42.000000 codalab-1.6.2/codalab_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/docker_config/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/docker_config/compose_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/compose_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/compose_files/docker-compose.dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/compose_files/docker-compose.ssl.yml
--rw-r--r--   0 runner    (1001) docker     (123)    23444 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/compose_files/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/docker_config/compose_files/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/compose_files/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/compose_files/files/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/compose_files/files/nginx.conf.ssl
--rwxr-xr-x   0 runner    (1001) docker     (123)     5213 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/compose_files/files/wait-for-it.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/docker_config/dockerfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/dockerfiles/Dockerfile.default-cpu
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/dockerfiles/Dockerfile.default-gpu
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/dockerfiles/Dockerfile.frontend
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/dockerfiles/Dockerfile.server
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/dockerfiles/Dockerfile.worker
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/docker_config/dockerfiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-21 18:50:42.000000 codalab-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-21 18:50:42.000000 codalab-1.6.2/rc
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-21 18:50:42.000000 codalab-1.6.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:26.000000 codalab-1.6.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 18:50:42.000000 codalab-1.6.2/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35824 2023-03-21 18:50:42.000000 codalab-1.6.2/scripts/competitiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-21 18:50:42.000000 codalab-1.6.2/scripts/create-root-user.py
--rw-r--r--   0 runner    (1001) docker     (123)    26218 2023-03-21 18:50:42.000000 codalab-1.6.2/scripts/create_sample_worksheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-21 18:50:42.000000 codalab-1.6.2/scripts/gen-cli-docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-03-21 18:50:42.000000 codalab-1.6.2/scripts/gen-rest-docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-21 18:50:42.000000 codalab-1.6.2/scripts/initialize-azurite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-03-21 18:50:42.000000 codalab-1.6.2/scripts/send-email-notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-03-21 18:50:42.000000 codalab-1.6.2/scripts/test_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-03-21 18:50:42.000000 codalab-1.6.2/scripts/upload-mlcomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-21 19:18:26.000000 codalab-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-03-21 18:50:42.000000 codalab-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 05:28:40.000000 codalab-1.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-03 06:01:34.000000 codalab-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-03 05:28:40.000000 codalab-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bin/bundle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bin/cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bin/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bin/ws_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab/bundles/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bundles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bundles/dataset_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bundles/derived_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bundles/make_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bundles/named_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bundles/private_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bundles/program_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bundles/run_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/bundles/uploaded_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27650 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/client/json_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab/lib/beam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/beam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/beam/blobstorageuploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/beam/filesystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/beam/mockblobstoragefilesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/beam/streamingzipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/bundle_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)   175230 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/bundle_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/bundle_fuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/bundle_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17635 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/bundle_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/canonicalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21487 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/codalab_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/completers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/crypt_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18423 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/editor_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/emailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/interactive_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/metadata_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/metadata_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/path_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/print_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/profiling_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/spec_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/telemetry_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/ui_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/unicode_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25672 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/upload_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47933 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/worksheet_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/lib/zip_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135134 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/model/bundle_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/model/mysql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/model/orm_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/model/sqlite_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21321 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/model/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/model/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/model/worker_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/objects/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/objects/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/objects/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/objects/metadata_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/objects/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/objects/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/objects/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/objects/worksheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/bundle_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59039 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31534 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/interpret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/worksheet_block_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20603 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/rest/worksheets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/server/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/server/authenticated_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51893 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/server/bundle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/server/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/server/json_api_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35051 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/server/oauth2_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/server/rest_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/server/worker_info_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/bundle_service_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/bundle_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30942 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/docker_image_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18090 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/download_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/fsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/image_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/noop_image_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/pyjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab/worker/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/runtime/kubernetes_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/singularity_image_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/state_committer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/tar_file_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/tar_subdir_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/un_gzip_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/un_tar_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/upload_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40065 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/worker_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36035 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/worker_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker/worker_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab/worker_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker_manager/aws_batch_worker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker_manager/azure_batch_worker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker_manager/kubernetes_worker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker_manager/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker_manager/slurm_batch_worker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab/worker_manager/worker_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 06:01:34.000000 codalab-1.6.3/codalab.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40133 2023-05-03 05:28:40.000000 codalab-1.6.3/codalab_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/docker_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/docker_config/compose_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/compose_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/compose_files/docker-compose.dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/compose_files/docker-compose.ssl.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    23444 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/compose_files/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/docker_config/compose_files/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/compose_files/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/compose_files/files/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/compose_files/files/nginx.conf.ssl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5213 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/compose_files/files/wait-for-it.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/docker_config/dockerfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/dockerfiles/Dockerfile.default-cpu
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/dockerfiles/Dockerfile.default-gpu
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/dockerfiles/Dockerfile.frontend
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/dockerfiles/Dockerfile.server
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/dockerfiles/Dockerfile.worker
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/docker_config/dockerfiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-03 05:28:40.000000 codalab-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-03 05:28:40.000000 codalab-1.6.3/rc
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-03 05:28:40.000000 codalab-1.6.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:01:34.000000 codalab-1.6.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 05:28:40.000000 codalab-1.6.3/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35824 2023-05-03 05:28:40.000000 codalab-1.6.3/scripts/competitiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-03 05:28:40.000000 codalab-1.6.3/scripts/create-root-user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26218 2023-05-03 05:28:40.000000 codalab-1.6.3/scripts/create_sample_worksheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-03 05:28:40.000000 codalab-1.6.3/scripts/gen-cli-docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-05-03 05:28:40.000000 codalab-1.6.3/scripts/gen-rest-docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-03 05:28:40.000000 codalab-1.6.3/scripts/initialize-azurite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-03 05:28:40.000000 codalab-1.6.3/scripts/send-email-notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-05-03 05:28:40.000000 codalab-1.6.3/scripts/test_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-05-03 05:28:40.000000 codalab-1.6.3/scripts/upload-mlcomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-03 06:01:34.000000 codalab-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-03 05:28:40.000000 codalab-1.6.3/setup.py
```

### Comparing `codalab-1.6.2/PKG-INFO` & `codalab-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: codalab
-Version: 1.6.2
+Version: 1.6.3
 Summary: CLI for CodaLab, a platform for reproducible computation
 Home-page: https://github.com/codalab/codalab-worksheets
 Author: CodaLab
 Author-email: codalab.worksheets@gmail.com
 License: Apache License 2.0
 Description: Visit https://worksheets.codalab.org/ or setup your own server by following the instructions in the documentation (https://codalab-worksheets.readthedocs.io/en/latest/Server-Setup).
 Keywords: codalab reproducible computation worksheets competitions
```

### Comparing `codalab-1.6.2/README.md` & `codalab-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/bin/bundle_manager.py` & `codalab-1.6.3/codalab/bin/bundle_manager.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/bin/server.py` & `codalab-1.6.3/codalab/bin/server.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/bin/ws_server.py` & `codalab-1.6.3/codalab/bin/ws_server.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/bundles/__init__.py` & `codalab-1.6.3/codalab/bundles/__init__.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/bundles/derived_bundle.py` & `codalab-1.6.3/codalab/bundles/derived_bundle.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/bundles/make_bundle.py` & `codalab-1.6.3/codalab/bundles/make_bundle.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/bundles/named_bundle.py` & `codalab-1.6.3/codalab/bundles/named_bundle.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/bundles/private_bundle.py` & `codalab-1.6.3/codalab/bundles/private_bundle.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/bundles/run_bundle.py` & `codalab-1.6.3/codalab/bundles/run_bundle.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/bundles/uploaded_bundle.py` & `codalab-1.6.3/codalab/bundles/uploaded_bundle.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/client/json_api_client.py` & `codalab-1.6.3/codalab/client/json_api_client.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/common.py` & `codalab-1.6.3/codalab/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     AZURE_BLOB_ACCOUNT_KEY,
     AZURE_BLOB_CONTAINER_NAME,
     AZURE_BLOB_HTTP_ENDPOINT,
 )
 
 # Increment this on master when ready to cut a release.
 # http://semver.org/
-CODALAB_VERSION = '1.6.2'
+CODALAB_VERSION = '1.6.3'
 BINARY_PLACEHOLDER = '<binary>'
 URLOPEN_TIMEOUT_SECONDS = int(os.environ.get('CODALAB_URLOPEN_TIMEOUT_SECONDS', 5 * 60))
 
 # Silence verbose log outputs from certain libraries
 logger = logging.getLogger('azure.core.pipeline.policies.http_logging_policy')
 logger.setLevel(logging.WARNING)
 logger = logging.getLogger('azure.storage.blob')
```

### Comparing `codalab-1.6.2/codalab/lib/beam/blobstorageuploader.py` & `codalab-1.6.3/codalab/lib/beam/blobstorageuploader.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/beam/filesystems.py` & `codalab-1.6.3/codalab/lib/beam/filesystems.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/beam/mockblobstoragefilesystem.py` & `codalab-1.6.3/codalab/lib/beam/mockblobstoragefilesystem.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/beam/streamingzipfile.py` & `codalab-1.6.3/codalab/lib/beam/streamingzipfile.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/bundle_action.py` & `codalab-1.6.3/codalab/lib/bundle_action.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/bundle_cli.py` & `codalab-1.6.3/codalab/lib/bundle_cli.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/bundle_fuse.py` & `codalab-1.6.3/codalab/lib/bundle_fuse.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/bundle_store.py` & `codalab-1.6.3/codalab/lib/bundle_store.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/bundle_util.py` & `codalab-1.6.3/codalab/lib/bundle_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/canonicalize.py` & `codalab-1.6.3/codalab/lib/canonicalize.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/cli_util.py` & `codalab-1.6.3/codalab/lib/cli_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/codalab_manager.py` & `codalab-1.6.3/codalab/lib/codalab_manager.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/completers.py` & `codalab-1.6.3/codalab/lib/completers.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/crypt_util.py` & `codalab-1.6.3/codalab/lib/crypt_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/download_manager.py` & `codalab-1.6.3/codalab/lib/download_manager.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/editor_util.py` & `codalab-1.6.3/codalab/lib/editor_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/emailer.py` & `codalab-1.6.3/codalab/lib/emailer.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/file_util.py` & `codalab-1.6.3/codalab/lib/file_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/formatting.py` & `codalab-1.6.3/codalab/lib/formatting.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/interactive_session.py` & `codalab-1.6.3/codalab/lib/interactive_session.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/metadata_defaults.py` & `codalab-1.6.3/codalab/lib/metadata_defaults.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/metadata_util.py` & `codalab-1.6.3/codalab/lib/metadata_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/path_util.py` & `codalab-1.6.3/codalab/lib/path_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/print_util.py` & `codalab-1.6.3/codalab/lib/print_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/profiling_util.py` & `codalab-1.6.3/codalab/lib/profiling_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/server_util.py` & `codalab-1.6.3/codalab/lib/server_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/spec_util.py` & `codalab-1.6.3/codalab/lib/spec_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/telemetry_util.py` & `codalab-1.6.3/codalab/lib/telemetry_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/ui_actions.py` & `codalab-1.6.3/codalab/lib/ui_actions.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/upload_manager.py` & `codalab-1.6.3/codalab/lib/upload_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,16 +361,19 @@
         ).upload_to_bundle_store(bundle, source, git, unpack)
 
     def has_contents(self, bundle):
         # TODO: make this non-fs-specific.
         return os.path.exists(self._bundle_store.get_bundle_location(bundle.uuid))
 
     def cleanup_existing_contents(self, bundle):
-        data_size = self._bundle_model.get_bundle_metadata(bundle.uuid, 'data_size')[bundle.uuid]
-        removed = self._bundle_store.cleanup(bundle.uuid, dry_run=False)
+        data_size = int(
+            self._bundle_model.get_bundle_metadata([bundle.uuid], 'data_size')[bundle.uuid]
+        )
+        bundle_location = self._bundle_store.get_bundle_location(bundle.uuid)
+        removed = self._bundle_store.cleanup(bundle_location, dry_run=False)
         bundle_update = {'metadata': {'data_size': 0}}
         self._bundle_model.update_bundle(bundle, bundle_update)
         if removed:
             self._bundle_model.increment_user_disk_used(bundle.owner_id, -data_size)
 
     def get_bundle_sas_token(self, path, **kwargs):
         """
```

### Comparing `codalab-1.6.2/codalab/lib/worksheet_util.py` & `codalab-1.6.3/codalab/lib/worksheet_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/lib/zip_util.py` & `codalab-1.6.3/codalab/lib/zip_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/model/bundle_model.py` & `codalab-1.6.3/codalab/model/bundle_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,26 +64,36 @@
 from codalab.worker.worker_run_state import RunStage
 from typing import Any, List
 
 logger = logging.getLogger(__name__)
 
 SEARCH_KEYWORD_REGEX = re.compile('^([\.\w/]*)=(.*)$')
 SEARCH_RESULTS_LIMIT = 10
+EDU_USER_REGEXES = re.compile('@[\w\.-]+\.(edu|edu\.[a-z]{2}|ac\.[a-z]{2})$')
 
 
 def str_key_dict(row):
     """
     row comes out of an element of a database query.
     For some versions of SqlAlchemy, the keys are of type sqlalchemy.sql.elements.quoted_name,
     which cannot be serialized to JSON.
     This function converts the keys to strings.
     """
     return dict((str(k), v) for k, v in row.items())
 
 
+def is_academic_email(email):
+    """
+    This is a basic function that can be used to compare the email domain suffix with a list of academic email domains.
+    Academic emails typically have domains such as "yy.edu" or "xyz.edu.xx" (where "edu" is followed by a country code).
+    """
+    email_suffix = EDU_USER_REGEXES.findall(email.lower())
+    return len(email_suffix) > 0
+
+
 @dataclass
 class Join:
     """
     Class that stores data for joins used in final SQL query in search_bundles.
     By default, becomes an inner join. Becomes left outer join if left_outer_join is True.
 
     """
@@ -218,24 +228,23 @@
         Fetch a single metadata value from the bundles referenced
         by the given uuids.
         Return {uuid: metadata_value}
         """
         if len(uuids) == 0:
             return []
         with self.engine.begin() as connection:
-            rows = connection.execute(
-                select(
-                    [cl_bundle_metadata.c.bundle_uuid, cl_bundle_metadata.c.metadata_value]
-                ).where(
-                    and_(
-                        cl_bundle_metadata.c.metadata_key == metadata_key,
-                        cl_bundle_metadata.c.bundle_uuid.in_(uuids),
-                    )
+            query = select(
+                [cl_bundle_metadata.c.bundle_uuid, cl_bundle_metadata.c.metadata_value]
+            ).where(
+                and_(
+                    cl_bundle_metadata.c.metadata_key == metadata_key,
+                    cl_bundle_metadata.c.bundle_uuid.in_(uuids),
                 )
-            ).fetchall()
+            )
+            rows = connection.execute(query).fetchall()
             return dict((row.bundle_uuid, row.metadata_value) for row in rows)
 
     def get_owner_ids(self, table, uuids):
         """
         Fetch the owners of the given uuids (for either bundles or worksheets).
         Return {uuid: ..., owner_id: ...}
         """
@@ -997,20 +1006,29 @@
             'last_updated': int(time.time()),
             'time': worker_run.container_time_total,
             'time_user': worker_run.container_time_user,
             'time_system': worker_run.container_time_system,
             'remote': worker_run.remote,
             'cpu_usage': cpu_usage,
             'memory_usage': memory_usage,
+            'data_size': worker_run.disk_utilization,
         }
 
-        # Increment user time as we go to ensure user doesn't go over time quota.
-        if user_id == self.root_user_id and hasattr(bundle.metadata, 'time'):
-            time_increment = worker_run.container_time_total - bundle.metadata.time
+        # Increment user time and disk as we go to ensure user doesn't go over quota.
+        # time increment is the change in running time for this bundle since the last checkin.
+        # disk increment is the change in disk quota used for this bundle since the last checkin.
+        if user_id == self.root_user_id:
+            time_increment = worker_run.container_time_total
+            if hasattr(bundle.metadata, 'time'):
+                time_increment -= bundle.metadata.time
             self.increment_user_time_used(bundle.owner_id, time_increment)
+        disk_increment = worker_run.disk_utilization
+        if hasattr(bundle.metadata, 'data_size'):
+            disk_increment -= bundle.metadata.data_size
+        self.increment_user_disk_used(bundle.owner_id, disk_increment)
 
         if worker_run.docker_image is not None:
             metadata_update['docker_image'] = worker_run.docker_image
 
         if worker_run.bundle_profile_stats is not None:
             metadata_update['time_preparing'] = worker_run.bundle_profile_stats[RunStage.PREPARING][
                 'elapsed'
@@ -1081,14 +1099,16 @@
         failure_message, exitcode = worker_run.failure_message, worker_run.exitcode
         if failure_message is None and exitcode is not None and exitcode != 0:
             failure_message = 'Exit code %d' % exitcode
 
         if user_id == self.root_user_id:
             time_increment = worker_run.container_time_total - bundle.metadata.time
             self.increment_user_time_used(bundle.owner_id, time_increment)
+        disk_increment = worker_run.disk_utilization - bundle.metadata.data_size
+        self.increment_user_disk_used(bundle.owner_id, disk_increment)
 
         # Build metadata
         metadata = {}
         if failure_message is not None:
             metadata['failure_message'] = failure_message
         if exitcode is not None:
             metadata['exitcode'] = exitcode
@@ -1107,63 +1127,68 @@
         metadata = bundle.metadata.to_dict()
         failure_message = metadata.get('failure_message', None)
         exitcode = metadata.get('exitcode', 0)
         state = State.FAILED if failure_message or exitcode else State.READY
         if failure_message and 'Kill requested' in failure_message:
             state = State.KILLED
 
-        worker = self.get_bundle_worker(bundle.uuid)
-
-        if worker['shared_file_system']:
-            # TODO(Ashwin): fix for --link.
-            self.update_disk_metadata(bundle, bundle_location)
-
         metadata = {'run_status': 'Finished', 'last_updated': int(time.time())}
 
         with self.engine.begin() as connection:
             self.update_bundle(bundle, {'state': state, 'metadata': metadata}, connection)
             connection.execute(
                 cl_worker_run.delete().where(cl_worker_run.c.run_uuid == bundle.uuid)
             )
 
     # ==========================================================================
     # Bundle state machine helper functions
     # ==========================================================================
 
-    def update_disk_metadata(self, bundle, bundle_location, enforce_disk_quota=False):
+    def get_data_size(self, bundle_location):
         """
-        Computes the disk use and data hash of the given bundle.
-        Updates the database rows for the bundle and user with the new disk use
+        Returns data_size (in bytes) of bundle at bundle_location
         """
         dirs_and_files = None
         if os.path.isdir(bundle_location):
             dirs_and_files = path_util.recursive_ls(bundle_location)
         else:
             dirs_and_files = [], [bundle_location]
 
         # TODO(Ashwin): make this non-fs specific
-        data_size = path_util.get_size(bundle_location, dirs_and_files)
+        return path_util.get_size(bundle_location, dirs_and_files)
+
+    def enforce_disk_quota(self, bundle, bundle_location):
+        """
+        Throws an error if saving bundle will cause user to go over disk quota left.
+        """
+        data_size = self.get_data_size(bundle_location)
+        disk_left = self.get_user_disk_quota_left(bundle.owner_id)
+        if data_size > disk_left:
+            raise UsageError(
+                "Can't save bundle, bundle size %s greater than user's disk quota left: %s"
+                % (data_size, disk_left)
+            )
+
+    def update_disk_metadata(self, bundle, bundle_location):
+        """
+        Update user's disk used with the size of the new bundle.
+
+        Only used by bundle_manager when creating make bundles.
+        """
+        data_size = self.get_data_size(bundle_location)
         try:
             if 'data_size' in bundle.metadata.__dict__:
                 current_data_size = bundle.metadata.data_size
             else:
                 current_data_size = int(
                     self.get_bundle_metadata([bundle.uuid], 'data_size')[bundle.uuid]
                 )
         except Exception:
             current_data_size = 0
         disk_increment = data_size - current_data_size
-        if enforce_disk_quota:
-            disk_left = self.get_user_disk_quota_left(bundle.owner_id)
-            if disk_increment > disk_left:
-                raise UsageError(
-                    "Can't save bundle, bundle size %s greater than user's disk quota left: %s"
-                    % (data_size, disk_left)
-                )
-
         bundle_update = {'metadata': {'data_size': data_size}}
         self.update_bundle(bundle, bundle_update)
         self.increment_user_disk_used(bundle.owner_id, disk_increment)
 
     def bundle_checkin(self, bundle, worker_run, user_id, worker_id):
         """
         Updates the database tables with the most recent bundle information from worker
@@ -2456,26 +2481,27 @@
         :param email:
         :param first_name:
         :param last_name:
         :param password:
         :param affiliation:
         :return: (new integer user ID, verification key to send)
         """
+
         with self.engine.begin() as connection:
             now = datetime.datetime.utcnow()
             user_id = user_id or '0x%s' % uuid4().hex
 
             time_quota = (
                 self.default_user_info['edu_time_quota']
-                if email.endswith(".edu")
+                if is_academic_email(email)
                 else self.default_user_info['time_quota']
             )
             disk_quota = (
                 self.default_user_info['edu_disk_quota']
-                if email.endswith(".edu")
+                if is_academic_email(email)
                 else self.default_user_info['disk_quota']
             )
 
             connection.execute(
                 cl_user.insert().values(
                     {
                         "user_id": user_id,
@@ -2753,14 +2779,19 @@
     def get_user_time_quota_left(self, user_id, user_info=None):
         if not user_info:
             user_info = self.get_user_info(user_id)
         time_quota = user_info['time_quota']
         time_used = user_info['time_used']
         return time_quota - time_used
 
+    def get_user_disk_quota_left(self, user_id, user_info=None):
+        if not user_info:
+            user_info = self.get_user_info(user_id)
+        return user_info['disk_quota'] - user_info['disk_used']
+
     def get_user_parallel_run_quota_left(self, user_id, user_info=None):
         if not user_info:
             user_info = self.get_user_info(user_id)
         parallel_run_quota = user_info['parallel_run_quota']
         with self.engine.begin() as connection:
             # Get all the runs belonging to this user whose workers are not personal workers
             # of the user themselves
@@ -2778,19 +2809,14 @@
 
     def update_user_last_login(self, user_id):
         """
         Update user's last login date to now.
         """
         self.update_user_info({'user_id': user_id, 'last_login': datetime.datetime.utcnow()})
 
-    def get_user_disk_quota_left(self, user_id, user_info=None):
-        if not user_info:
-            user_info = self.get_user_info(user_id)
-        return user_info['disk_quota'] - user_info['disk_used']
-
     # ===========================================================================
     # OAuth-related methods follow!
     # ===========================================================================
 
     def _create_default_clients(self):
         DEFAULT_CLIENTS = [
             ('codalab_cli_client', 'CodaLab CLI'),
```

### Comparing `codalab-1.6.2/codalab/model/mysql_model.py` & `codalab-1.6.3/codalab/model/mysql_model.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/model/orm_object.py` & `codalab-1.6.3/codalab/model/orm_object.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/model/sqlite_model.py` & `codalab-1.6.3/codalab/model/sqlite_model.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/model/tables.py` & `codalab-1.6.3/codalab/model/tables.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/model/worker_model.py` & `codalab-1.6.3/codalab/model/worker_model.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/objects/bundle.py` & `codalab-1.6.3/codalab/objects/bundle.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/objects/dependency.py` & `codalab-1.6.3/codalab/objects/dependency.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/objects/metadata.py` & `codalab-1.6.3/codalab/objects/metadata.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/objects/metadata_spec.py` & `codalab-1.6.3/codalab/objects/metadata_spec.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/objects/oauth2.py` & `codalab-1.6.3/codalab/objects/oauth2.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/objects/permission.py` & `codalab-1.6.3/codalab/objects/permission.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/objects/user.py` & `codalab-1.6.3/codalab/objects/user.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/objects/worksheet.py` & `codalab-1.6.3/codalab/objects/worksheet.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/rest/account.py` & `codalab-1.6.3/codalab/rest/account.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/rest/bundle_actions.py` & `codalab-1.6.3/codalab/rest/bundle_actions.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/rest/bundles.py` & `codalab-1.6.3/codalab/rest/bundles.py`

 * *Files 1% similar despite different names*

```diff
@@ -589,15 +589,15 @@
     error_msg = query_get_type(str, 'error_msg', default=None)
 
     bundle = local.model.get_bundle(bundle_uuid)
     bundle_location = local.bundle_store.get_bundle_location(bundle.uuid)  # get blob storage url
     logging.info(f"_update_bundle_location, bundle_location is {bundle_location}")
 
     if success:
-        local.model.update_disk_metadata(bundle, bundle_location, enforce_disk_quota=True)
+        local.model.enforce_disk_quota(bundle, bundle_location)
         local.model.update_bundle(
             bundle, {'state': state_on_success},
         )
     else:  # If the upload failed, cleanup the uploaded file and update bundle state
         local.model.update_bundle(
             bundle, {'state': state_on_failure, 'metadata': {'failure_message': error_msg},},
         )
@@ -1161,15 +1161,15 @@
                 git=query_get_bool('git', default=False),
                 unpack=query_get_bool('unpack', default=True),
                 use_azure_blob_beta=use_azure_blob_beta,
                 destination_bundle_store=store,
             )
             bundle_link_url = getattr(bundle.metadata, "link_url", None)
             bundle_location = bundle_link_url or local.bundle_store.get_bundle_location(bundle.uuid)
-            local.model.update_disk_metadata(bundle, bundle_location, enforce_disk_quota=True)
+            local.model.enforce_disk_quota(bundle, bundle_location)
 
     except UsageError as err:
         # This is a user error (most likely disk quota overuser) so raise a client HTTP error
         if local.upload_manager.has_contents(bundle):
             local.upload_manager.cleanup_existing_contents(bundle)
         msg = "Upload failed: %s" % err
         local.model.update_bundle(
```

### Comparing `codalab-1.6.2/codalab/rest/cli.py` & `codalab-1.6.3/codalab/rest/cli.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/rest/groups.py` & `codalab-1.6.3/codalab/rest/groups.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/rest/help.py` & `codalab-1.6.3/codalab/rest/help.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/rest/interpret.py` & `codalab-1.6.3/codalab/rest/interpret.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/rest/oauth2.py` & `codalab-1.6.3/codalab/rest/oauth2.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/rest/schemas.py` & `codalab-1.6.3/codalab/rest/schemas.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/rest/users.py` & `codalab-1.6.3/codalab/rest/users.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/rest/util.py` & `codalab-1.6.3/codalab/rest/util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/rest/workers.py` & `codalab-1.6.3/codalab/rest/workers.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,23 +46,32 @@
     )
 
     messages = []
     for run in request.json["runs"]:
         try:
             worker_run = BundleCheckinState.from_dict(run)
             bundle = local.model.get_bundle(worker_run.uuid)
-            local.model.bundle_checkin(bundle, worker_run, request.user.user_id, worker_id)
+            local.model.bundle_checkin(
+                bundle, worker_run, request.user.user_id, worker_id,
+            )
 
             if local.model.get_user_time_quota_left(bundle.owner_id) <= 0:
                 # Then, user has gone over their time quota and we kill the job.
                 kill_message = (
                     'Kill requested: User time quota exceeded. To apply for more quota, please visit the following link: '
                     'https://codalab-worksheets.readthedocs.io/en/latest/FAQ/#how-do-i-request-more-disk-quota-or-time-quota'
                 )
                 messages.append({'type': 'kill', 'uuid': bundle.uuid, 'kill_message': kill_message})
+            elif local.model.get_user_disk_quota_left(bundle.owner_id) <= 0:
+                # Then, user has gone over their disk quota and we kill the job.
+                kill_message = (
+                    'Kill requested: User disk quota exceeded. To apply for more quota, please visit the following link: '
+                    'https://codalab-worksheets.readthedocs.io/en/latest/FAQ/#how-do-i-request-more-disk-quota-or-time-quota'
+                )
+                messages.append({'type': 'kill', 'uuid': bundle.uuid, 'kill_message': kill_message})
         except Exception as e:
             logger.info("Exception in REST checkin: {}".format(e))
 
     with closing(local.worker_model.start_listening(socket_id)) as sock:
         messages.append(local.worker_model.get_json_message(sock, WAIT_TIME_SECS))
     response.content_type = 'application/json'
     return json.dumps(messages)
```

### Comparing `codalab-1.6.2/codalab/rest/worksheet_block_schemas.py` & `codalab-1.6.3/codalab/rest/worksheet_block_schemas.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/rest/worksheets.py` & `codalab-1.6.3/codalab/rest/worksheets.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/server/auth.py` & `codalab-1.6.3/codalab/server/auth.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/server/authenticated_plugin.py` & `codalab-1.6.3/codalab/server/authenticated_plugin.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/server/bundle_manager.py` & `codalab-1.6.3/codalab/server/bundle_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,16 @@
                     else:
                         os.mkdir(path)
                         for dependency_path, child_path in deps:
                             path_util.copy(dependency_path, child_path, follow_symlinks=False)
 
             # update the bundle location since we already change is_dir field
             bundle_location = bundle_link_url or self._bundle_store.get_bundle_location(bundle.uuid)
-            self._model.update_disk_metadata(bundle, bundle_location, enforce_disk_quota=True)
+            self._model.enforce_disk_quota(bundle, bundle_location)
+            self._model.update_disk_metadata(bundle, bundle_location)
             logger.info('Finished making bundle %s', bundle.uuid)
             self._model.update_bundle(bundle, {'state': State.READY})
         except Exception as e:
             logger.info('Failing bundle %s: %s', bundle.uuid, str(e))
             self._model.update_bundle(
                 bundle,
                 {
```

### Comparing `codalab-1.6.2/codalab/server/cookie.py` & `codalab-1.6.3/codalab/server/cookie.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/server/json_api_plugin.py` & `codalab-1.6.3/codalab/server/json_api_plugin.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/server/oauth2_provider.py` & `codalab-1.6.3/codalab/server/oauth2_provider.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/server/rest_server.py` & `codalab-1.6.3/codalab/server/rest_server.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/server/worker_info_accessor.py` & `codalab-1.6.3/codalab/server/worker_info_accessor.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/bundle_service_client.py` & `codalab-1.6.3/codalab/worker/bundle_service_client.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/bundle_state.py` & `codalab-1.6.3/codalab/worker/bundle_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -275,29 +275,31 @@
         state,  # type: State
         remote,  # type: str
         exitcode,  # type: Optional[str]
         failure_message,  # type: Optional[str]
         bundle_profile_stats,  # type: dict
         cpu_usage,  # type: float
         memory_usage,  # type: int
+        disk_utilization,  # type: int
     ):
         self.uuid = uuid
         self.run_status = run_status
         self.bundle_start_time = bundle_start_time
         self.container_time_total = container_time_total
         self.container_time_user = container_time_user
         self.container_time_system = container_time_system
         self.docker_image = docker_image
         self.state = state
         self.remote = remote
         self.exitcode = exitcode
         self.failure_message = failure_message
+        self.bundle_profile_stats = bundle_profile_stats
         self.cpu_usage = cpu_usage
         self.memory_usage = memory_usage
-        self.bundle_profile_stats = bundle_profile_stats
+        self.disk_utilization = disk_utilization
 
     @classmethod
     def from_dict(cls, dct):
         return cls(
             uuid=dct['uuid'],
             run_status=dct['run_status'],
             bundle_start_time=dct['bundle_start_time'],
@@ -305,17 +307,18 @@
             container_time_user=dct['container_time_user'],
             container_time_system=dct['container_time_system'],
             docker_image=dct['docker_image'],
             state=dct['state'],
             remote=dct['remote'],
             exitcode=dct['exitcode'],
             failure_message=dct['failure_message'],
+            bundle_profile_stats=dct.get('bundle_profile_stats'),
             cpu_usage=dct.get('cpu_usage'),
             memory_usage=dct.get('memory_usage'),
-            bundle_profile_stats=dct.get('bundle_profile_stats'),
+            disk_utilization=dct.get('disk_utilization'),
         )
 
     @property
     def as_dict(self):
         return generic_to_dict(self)
```

### Comparing `codalab-1.6.2/codalab/worker/dependency_manager.py` & `codalab-1.6.3/codalab/worker/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/docker_image_manager.py` & `codalab-1.6.3/codalab/worker/docker_image_manager.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/docker_utils.py` & `codalab-1.6.3/codalab/worker/docker_utils.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/download_util.py` & `codalab-1.6.3/codalab/worker/download_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/file_util.py` & `codalab-1.6.3/codalab/worker/file_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/fsm.py` & `codalab-1.6.3/codalab/worker/fsm.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/image_manager.py` & `codalab-1.6.3/codalab/worker/image_manager.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/main.py` & `codalab-1.6.3/codalab/worker/main.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/pyjson.py` & `codalab-1.6.3/codalab/worker/pyjson.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/reader.py` & `codalab-1.6.3/codalab/worker/reader.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/rest_client.py` & `codalab-1.6.3/codalab/worker/rest_client.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/runtime/__init__.py` & `codalab-1.6.3/codalab/worker/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/runtime/kubernetes_runtime.py` & `codalab-1.6.3/codalab/worker/runtime/kubernetes_runtime.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/singularity_image_manager.py` & `codalab-1.6.3/codalab/worker/singularity_image_manager.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/state_committer.py` & `codalab-1.6.3/codalab/worker/state_committer.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/tar_file_stream.py` & `codalab-1.6.3/codalab/worker/tar_file_stream.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/tar_subdir_stream.py` & `codalab-1.6.3/codalab/worker/tar_subdir_stream.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/un_gzip_stream.py` & `codalab-1.6.3/codalab/worker/un_gzip_stream.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/un_tar_directory.py` & `codalab-1.6.3/codalab/worker/un_tar_directory.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/upload_util.py` & `codalab-1.6.3/codalab/worker/upload_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/worker.py` & `codalab-1.6.3/codalab/worker/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -645,14 +645,15 @@
                 state=RunStage.WORKER_STATE_TO_SERVER_STATE[run_state.stage],
                 remote=self.id,
                 exitcode=run_state.exitcode,
                 failure_message=run_state.failure_message,
                 bundle_profile_stats=run_state.bundle_profile_stats,
                 cpu_usage=run_state.cpu_usage,
                 memory_usage=run_state.memory_usage,
+                disk_utilization=run_state.disk_utilization,
             )
             for run_state in self.runs.values()
         ]
 
     @property
     def free_disk_bytes(self):
         """
```

### Comparing `codalab-1.6.2/codalab/worker/worker_monitoring.py` & `codalab-1.6.3/codalab/worker/worker_monitoring.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/worker_run_state.py` & `codalab-1.6.3/codalab/worker/worker_run_state.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker/worker_thread.py` & `codalab-1.6.3/codalab/worker/worker_thread.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker_manager/aws_batch_worker_manager.py` & `codalab-1.6.3/codalab/worker_manager/aws_batch_worker_manager.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker_manager/azure_batch_worker_manager.py` & `codalab-1.6.3/codalab/worker_manager/azure_batch_worker_manager.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker_manager/kubernetes_worker_manager.py` & `codalab-1.6.3/codalab/worker_manager/kubernetes_worker_manager.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker_manager/main.py` & `codalab-1.6.3/codalab/worker_manager/main.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker_manager/slurm_batch_worker_manager.py` & `codalab-1.6.3/codalab/worker_manager/slurm_batch_worker_manager.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab/worker_manager/worker_manager.py` & `codalab-1.6.3/codalab/worker_manager/worker_manager.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab.egg-info/PKG-INFO` & `codalab-1.6.3/codalab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: codalab
-Version: 1.6.2
+Version: 1.6.3
 Summary: CLI for CodaLab, a platform for reproducible computation
 Home-page: https://github.com/codalab/codalab-worksheets
 Author: CodaLab
 Author-email: codalab.worksheets@gmail.com
 License: Apache License 2.0
 Description: Visit https://worksheets.codalab.org/ or setup your own server by following the instructions in the documentation (https://codalab-worksheets.readthedocs.io/en/latest/Server-Setup).
 Keywords: codalab reproducible computation worksheets competitions
```

### Comparing `codalab-1.6.2/codalab.egg-info/SOURCES.txt` & `codalab-1.6.3/codalab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/codalab.egg-info/requires.txt` & `codalab-1.6.3/codalab.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-apache-beam[azure]==2.36.0
+apache-beam[azure]==2.38.0
 cachetools<5,>=3.1.0
 google-apitools<0.5.32,>=0.5.31
 google-auth<3,>=1.18.0
 bottle==0.12.20
 docker==4.3.0
 marshmallow-jsonapi==0.15.1
 marshmallow==2.15.1
```

### Comparing `codalab-1.6.2/codalab_service.py` & `codalab-1.6.3/codalab_service.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/docker_config/compose_files/docker-compose.dev.yml` & `codalab-1.6.3/docker_config/compose_files/docker-compose.dev.yml`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/docker_config/compose_files/docker-compose.yml` & `codalab-1.6.3/docker_config/compose_files/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/docker_config/compose_files/files/nginx.conf` & `codalab-1.6.3/docker_config/compose_files/files/nginx.conf`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/docker_config/compose_files/files/nginx.conf.ssl` & `codalab-1.6.3/docker_config/compose_files/files/nginx.conf.ssl`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/docker_config/compose_files/files/wait-for-it.sh` & `codalab-1.6.3/docker_config/compose_files/files/wait-for-it.sh`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/docker_config/dockerfiles/Dockerfile.default-cpu` & `codalab-1.6.3/docker_config/dockerfiles/Dockerfile.default-cpu`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/docker_config/dockerfiles/Dockerfile.default-gpu` & `codalab-1.6.3/docker_config/dockerfiles/Dockerfile.default-gpu`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/docker_config/dockerfiles/Dockerfile.server` & `codalab-1.6.3/docker_config/dockerfiles/Dockerfile.server`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/docker_config/dockerfiles/Dockerfile.worker` & `codalab-1.6.3/docker_config/dockerfiles/Dockerfile.worker`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/rc` & `codalab-1.6.3/rc`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/requirements.txt` & `codalab-1.6.3/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-apache-beam[azure]==2.36.0
+apache-beam[azure]==2.38.0
 
 # GCP requirements for apache-beam. Note: when upgrading
 # apache-beam, make sure these requirements are also upgraded
 # accordingly according to Beam's GCP requirements
 # (https://github.com/apache/beam/blob/master/sdks/python/setup.py).
 cachetools>=3.1.0,<5
 google-apitools>=0.5.31,<0.5.32
```

### Comparing `codalab-1.6.2/scripts/competitiond.py` & `codalab-1.6.3/scripts/competitiond.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/scripts/create-root-user.py` & `codalab-1.6.3/scripts/create-root-user.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/scripts/create_sample_worksheet.py` & `codalab-1.6.3/scripts/create_sample_worksheet.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/scripts/gen-cli-docs.py` & `codalab-1.6.3/scripts/gen-cli-docs.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/scripts/gen-rest-docs.py` & `codalab-1.6.3/scripts/gen-rest-docs.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/scripts/send-email-notifications.py` & `codalab-1.6.3/scripts/send-email-notifications.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/scripts/test_util.py` & `codalab-1.6.3/scripts/test_util.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/scripts/upload-mlcomp.py` & `codalab-1.6.3/scripts/upload-mlcomp.py`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/setup.cfg` & `codalab-1.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `codalab-1.6.2/setup.py` & `codalab-1.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 import setuptools
 import sys
 
 
 # should match codalab/common.py#CODALAB_VERSION
-CODALAB_VERSION = "1.6.2"
+CODALAB_VERSION = "1.6.3"
 
 
 class Install(install):
     _WARNING_TEMPLATE = (
         '\n\n\033[1m\033[93mWarning! CodaLab was installed at {}, which is not\n'
         'one of the following paths in $PATH:\n\n{}\n\nConsider adding {} to $PATH\n'
         'to use the CodaLab CLI. You can do this by {}\033[0m\n\n'
```

