# Comparing `tmp/google-cloud-spanner-3.8.0.tar.gz` & `tmp/google-cloud-spanner-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/google-cloud-spanner-3.8.0.tar", last modified: Mon Aug 16 07:09:38 2021, max compression
+gzip compressed data, was "dist/google-cloud-spanner-3.9.0.tar", last modified: Mon Aug 30 20:24:30 2021, max compression
```

## Comparing `google-cloud-spanner-3.8.0.tar` & `google-cloud-spanner-3.9.0.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.697450 google-cloud-spanner-3.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     8494 2021-08-16 07:09:38.697450 google-cloud-spanner-3.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     7638 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.665466 google-cloud-spanner-3.8.0/google/
--rw-rw-r--   0 root         (0)     1003      172 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.669464 google-cloud-spanner-3.8.0/google/cloud/
--rw-rw-r--   0 root         (0)     1003      172 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/__init__.py
--rw-rw-r--   0 root         (0)     1003     1562 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.669464 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/
--rw-rw-r--   0 root         (0)     1003     3673 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4788 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       96 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.669464 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.669464 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/
--rw-rw-r--   0 root         (0)     1003      765 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/__init__.py
--rw-rw-r--   0 root         (0)     1003    84933 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/async_client.py
--rw-rw-r--   0 root         (0)     1003    93200 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/client.py
--rw-rw-r--   0 root         (0)     1003    21820 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.669464 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/
--rw-rw-r--   0 root         (0)     1003     1185 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    19591 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/base.py
--rw-rw-r--   0 root         (0)     1003    37162 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    37947 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.669464 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/types/
--rw-rw-r--   0 root         (0)     1003     2563 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    22963 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/types/backup.py
--rw-rw-r--   0 root         (0)     1003     3279 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003    29110 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/types/spanner_database_admin.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.669464 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/
--rw-rw-r--   0 root         (0)     1003     2061 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3072 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       96 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.673462 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.673462 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/
--rw-rw-r--   0 root         (0)     1003      765 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/__init__.py
--rw-rw-r--   0 root         (0)     1003    55808 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/async_client.py
--rw-rw-r--   0 root         (0)     1003    63065 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/client.py
--rw-rw-r--   0 root         (0)     1003    11502 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.673462 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/
--rw-rw-r--   0 root         (0)     1003     1185 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14030 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/base.py
--rw-rw-r--   0 root         (0)     1003    28912 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    29481 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.673462 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/types/
--rw-rw-r--   0 root         (0)     1003     1403 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    19361 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/types/spanner_instance_admin.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.677460 google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/
--rw-rw-r--   0 root         (0)     1003     3275 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/__init__.py
--rw-rw-r--   0 root         (0)     1003     5462 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/_helpers.py
--rw-rw-r--   0 root         (0)     1003     2740 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/checksum.py
--rw-rw-r--   0 root         (0)     1003    14963 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/connection.py
--rw-rw-r--   0 root         (0)     1003    17589 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/cursor.py
--rw-rw-r--   0 root         (0)     1003     2408 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/exceptions.py
--rw-rw-r--   0 root         (0)     1003    17016 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/parse_utils.py
--rw-rw-r--   0 root         (0)     1003     7486 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/parser.py
--rw-rw-r--   0 root         (0)     1003     3146 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/types.py
--rw-rw-r--   0 root         (0)     1003     4500 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/utils.py
--rw-rw-r--   0 root         (0)     1003      721 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.681458 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/
--rw-rw-r--   0 root         (0)     1003     4502 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10330 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/_helpers.py
--rw-rw-r--   0 root         (0)     1003     2011 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/_opentelemetry_tracing.py
--rw-rw-r--   0 root         (0)     1003    11271 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/backup.py
--rw-rw-r--   0 root         (0)     1003     7182 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/batch.py
--rw-rw-r--   0 root         (0)     1003    14202 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/client.py
--rw-rw-r--   0 root         (0)     1003    44970 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/database.py
--rw-rw-r--   0 root         (0)     1003     4138 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003    24366 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/instance.py
--rw-rw-r--   0 root         (0)     1003     6251 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/keyset.py
--rw-rw-r--   0 root         (0)     1003     2414 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/param_types.py
--rw-rw-r--   0 root         (0)     1003    18260 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/pool.py
--rw-rw-r--   0 root         (0)     1003       81 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.681458 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.681458 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/
--rw-rw-r--   0 root         (0)     1003      741 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/__init__.py
--rw-rw-r--   0 root         (0)     1003    60943 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/async_client.py
--rw-rw-r--   0 root         (0)     1003    67967 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/client.py
--rw-rw-r--   0 root         (0)     1003     5670 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.681458 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/transports/
--rw-rw-r--   0 root         (0)     1003     1131 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    17431 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/transports/base.py
--rw-rw-r--   0 root         (0)     1003    33705 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34392 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    15670 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/session.py
--rw-rw-r--   0 root         (0)     1003    23524 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/snapshot.py
--rw-rw-r--   0 root         (0)     1003    10950 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/streamed.py
--rw-rw-r--   0 root         (0)     1003     3784 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/table.py
--rw-rw-r--   0 root         (0)     1003    14414 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/transaction.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.685456 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/
--rw-rw-r--   0 root         (0)     1003     2440 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2517 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/commit_response.py
--rw-rw-r--   0 root         (0)     1003     6810 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/keys.py
--rw-rw-r--   0 root         (0)     1003     6448 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/mutation.py
--rw-rw-r--   0 root         (0)     1003     6575 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/query_plan.py
--rw-rw-r--   0 root         (0)     1003    11025 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/result_set.py
--rw-rw-r--   0 root         (0)     1003    42609 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/spanner.py
--rw-rw-r--   0 root         (0)     1003    23127 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/transaction.py
--rw-rw-r--   0 root         (0)     1003     4118 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/type.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.685456 google-cloud-spanner-3.8.0/google_cloud_spanner.egg-info/
--rw-r--r--   0 root         (0)     1003     8494 2021-08-16 07:09:38.000000 google-cloud-spanner-3.8.0/google_cloud_spanner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     6361 2021-08-16 07:09:38.000000 google-cloud-spanner-3.8.0/google_cloud_spanner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2021-08-16 07:09:38.000000 google-cloud-spanner-3.8.0/google_cloud_spanner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2021-08-16 07:09:38.000000 google-cloud-spanner-3.8.0/google_cloud_spanner.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2021-08-16 07:09:38.000000 google-cloud-spanner-3.8.0/google_cloud_spanner.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      292 2021-08-16 07:09:38.000000 google-cloud-spanner-3.8.0/google_cloud_spanner.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2021-08-16 07:09:38.000000 google-cloud-spanner-3.8.0/google_cloud_spanner.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2021-08-16 07:09:38.701448 google-cloud-spanner-3.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3313 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.685456 google-cloud-spanner-3.8.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/__init__.py
--rw-rw-r--   0 root         (0)     1003     3631 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/_fixtures.py
--rw-rw-r--   0 root         (0)     1003     2123 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/_helpers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.689454 google-cloud-spanner-3.8.0/tests/system/
--rw-rw-r--   0 root         (0)     1003        0 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/__init__.py
--rw-rw-r--   0 root         (0)     1003     3739 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/_helpers.py
--rw-rw-r--   0 root         (0)     1003     2985 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/_sample_data.py
--rw-rw-r--   0 root         (0)     1003     4360 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/conftest.py
--rw-rw-r--   0 root         (0)     1003    15681 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/test_backup_api.py
--rw-rw-r--   0 root         (0)     1003    12818 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/test_database_api.py
--rw-rw-r--   0 root         (0)     1003     9102 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/test_dbapi.py
--rw-rw-r--   0 root         (0)     1003     4445 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/test_instance_api.py
--rw-rw-r--   0 root         (0)     1003    71164 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/test_session_api.py
--rw-rw-r--   0 root         (0)     1003     2381 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/test_streaming_chunking.py
--rw-rw-r--   0 root         (0)     1003     2324 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/test_table_api.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.689454 google-cloud-spanner-3.8.0/tests/system/utils/
--rw-rw-r--   0 root         (0)     1003        0 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/utils/__init__.py
--rw-rw-r--   0 root         (0)     1003     1463 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/utils/clear_streaming.py
--rw-rw-r--   0 root         (0)     1003     4629 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/utils/populate_streaming.py
--rw-rw-r--   0 root         (0)     1003     1300 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/utils/scrub_instances.py
--rw-rw-r--   0 root         (0)     1003     1224 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/system/utils/streaming_utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.693452 google-cloud-spanner-3.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.693452 google-cloud-spanner-3.8.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.693452 google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_admin_database_v1/
--rw-rw-r--   0 root         (0)     1003      600 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_admin_database_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   212782 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_admin_database_v1/test_database_admin.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.697450 google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_admin_instance_v1/
--rw-rw-r--   0 root         (0)     1003      600 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_admin_instance_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   142880 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_admin_instance_v1/test_instance_admin.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.697450 google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_v1/
--rw-rw-r--   0 root         (0)     1003      600 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   144545 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_v1/test_spanner.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-08-16 07:09:38.697450 google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/
--rw-rw-r--   0 root         (0)     1003      595 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/__init__.py
--rw-rw-r--   0 root         (0)     1003     4330 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test__helpers.py
--rw-rw-r--   0 root         (0)     1003     2500 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_checksum.py
--rw-rw-r--   0 root         (0)     1003     4823 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_connect.py
--rw-rw-r--   0 root         (0)     1003    22950 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_connection.py
--rw-rw-r--   0 root         (0)     1003    47193 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_cursor.py
--rw-rw-r--   0 root         (0)     1003     1128 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_globals.py
--rw-rw-r--   0 root         (0)     1003    16610 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_parse_utils.py
--rw-rw-r--   0 root         (0)     1003    11386 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_parser.py
--rw-rw-r--   0 root         (0)     1003     2307 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_types.py
--rw-rw-r--   0 root         (0)     1003     4189 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_utils.py
--rw-rw-r--   0 root         (0)     1003    11747 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/streaming-read-acceptance-test.json
--rw-rw-r--   0 root         (0)     1003    22867 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test__helpers.py
--rw-rw-r--   0 root         (0)     1003     5587 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test__opentelemetry_tracing.py
--rw-rw-r--   0 root         (0)     1003    25072 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test_backup.py
--rw-rw-r--   0 root         (0)     1003    12420 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test_batch.py
--rw-rw-r--   0 root         (0)     1003    25216 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test_client.py
--rw-rw-r--   0 root         (0)     1003    91614 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test_database.py
--rw-rw-r--   0 root         (0)     1003    41229 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test_instance.py
--rw-rw-r--   0 root         (0)     1003    14018 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test_keyset.py
--rw-rw-r--   0 root         (0)     1003     1898 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test_param_types.py
--rw-rw-r--   0 root         (0)     1003    29666 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test_pool.py
--rw-rw-r--   0 root         (0)     1003    53986 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test_session.py
--rw-rw-r--   0 root         (0)     1003    53885 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test_snapshot.py
--rw-rw-r--   0 root         (0)     1003    46177 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test_streamed.py
--rw-rw-r--   0 root         (0)     1003     4961 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test_table.py
--rw-rw-r--   0 root         (0)     1003    27667 2021-08-16 07:07:00.000000 google-cloud-spanner-3.8.0/tests/unit/test_transaction.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.563749 google-cloud-spanner-3.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     8494 2021-08-30 20:24:30.563749 google-cloud-spanner-3.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     7638 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.531733 google-cloud-spanner-3.9.0/google/
+-rw-rw-r--   0 root         (0)     1003      172 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.531733 google-cloud-spanner-3.9.0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      172 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1562 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.535735 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/
+-rw-rw-r--   0 root         (0)     1003     3673 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4788 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       96 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.535735 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.535735 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/
+-rw-rw-r--   0 root         (0)     1003      765 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003    84933 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/async_client.py
+-rw-rw-r--   0 root         (0)     1003    93200 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/client.py
+-rw-rw-r--   0 root         (0)     1003    21820 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.535735 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/
+-rw-rw-r--   0 root         (0)     1003     1185 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19591 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    37162 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    37947 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.535735 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2563 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22963 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/types/backup.py
+-rw-rw-r--   0 root         (0)     1003     3279 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    29110 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/types/spanner_database_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.535735 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/
+-rw-rw-r--   0 root         (0)     1003     2061 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3072 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       96 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.535735 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.539737 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/
+-rw-rw-r--   0 root         (0)     1003      765 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003    55808 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/async_client.py
+-rw-rw-r--   0 root         (0)     1003    63065 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/client.py
+-rw-rw-r--   0 root         (0)     1003    11502 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.539737 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/
+-rw-rw-r--   0 root         (0)     1003     1185 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14030 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    28912 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    29481 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.539737 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1403 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19361 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/types/spanner_instance_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.539737 google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/
+-rw-rw-r--   0 root         (0)     1003     3275 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5462 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     2740 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/checksum.py
+-rw-rw-r--   0 root         (0)     1003    14963 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/connection.py
+-rw-rw-r--   0 root         (0)     1003    17589 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/cursor.py
+-rw-rw-r--   0 root         (0)     1003     2408 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/exceptions.py
+-rw-rw-r--   0 root         (0)     1003    17016 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/parse_utils.py
+-rw-rw-r--   0 root         (0)     1003     7486 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/parser.py
+-rw-rw-r--   0 root         (0)     1003     3146 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/types.py
+-rw-rw-r--   0 root         (0)     1003     4500 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/utils.py
+-rw-rw-r--   0 root         (0)     1003      721 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.543739 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/
+-rw-rw-r--   0 root         (0)     1003     4502 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10404 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     2011 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/_opentelemetry_tracing.py
+-rw-rw-r--   0 root         (0)     1003    11271 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/backup.py
+-rw-rw-r--   0 root         (0)     1003     7182 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/batch.py
+-rw-rw-r--   0 root         (0)     1003    14202 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/client.py
+-rw-rw-r--   0 root         (0)     1003    44978 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/database.py
+-rw-rw-r--   0 root         (0)     1003     4138 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003    24366 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/instance.py
+-rw-rw-r--   0 root         (0)     1003     6251 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/keyset.py
+-rw-rw-r--   0 root         (0)     1003     2446 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/param_types.py
+-rw-rw-r--   0 root         (0)     1003    18260 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/pool.py
+-rw-rw-r--   0 root         (0)     1003       81 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.543739 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.543739 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/
+-rw-rw-r--   0 root         (0)     1003      741 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003    60943 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/async_client.py
+-rw-rw-r--   0 root         (0)     1003    67967 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/client.py
+-rw-rw-r--   0 root         (0)     1003     5670 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.547741 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/transports/
+-rw-rw-r--   0 root         (0)     1003     1131 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17431 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    33705 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34392 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    15670 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/session.py
+-rw-rw-r--   0 root         (0)     1003    23524 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/snapshot.py
+-rw-rw-r--   0 root         (0)     1003    10984 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/streamed.py
+-rw-rw-r--   0 root         (0)     1003     3784 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/table.py
+-rw-rw-r--   0 root         (0)     1003    14414 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/transaction.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.547741 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2440 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2517 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/commit_response.py
+-rw-rw-r--   0 root         (0)     1003     6810 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/keys.py
+-rw-rw-r--   0 root         (0)     1003     6448 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/mutation.py
+-rw-rw-r--   0 root         (0)     1003     6575 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/query_plan.py
+-rw-rw-r--   0 root         (0)     1003    11025 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/result_set.py
+-rw-rw-r--   0 root         (0)     1003    42609 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/spanner.py
+-rw-rw-r--   0 root         (0)     1003    23127 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/transaction.py
+-rw-rw-r--   0 root         (0)     1003     4118 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/type.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.551743 google-cloud-spanner-3.9.0/google_cloud_spanner.egg-info/
+-rw-r--r--   0 root         (0)     1003     8494 2021-08-30 20:24:30.000000 google-cloud-spanner-3.9.0/google_cloud_spanner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     6361 2021-08-30 20:24:30.000000 google-cloud-spanner-3.9.0/google_cloud_spanner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-08-30 20:24:30.000000 google-cloud-spanner-3.9.0/google_cloud_spanner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2021-08-30 20:24:30.000000 google-cloud-spanner-3.9.0/google_cloud_spanner.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-08-30 20:24:30.000000 google-cloud-spanner-3.9.0/google_cloud_spanner.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      292 2021-08-30 20:24:30.000000 google-cloud-spanner-3.9.0/google_cloud_spanner.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2021-08-30 20:24:30.000000 google-cloud-spanner-3.9.0/google_cloud_spanner.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2021-08-30 20:24:30.563749 google-cloud-spanner-3.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3313 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.551743 google-cloud-spanner-3.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3686 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/_fixtures.py
+-rw-rw-r--   0 root         (0)     1003     2123 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.551743 google-cloud-spanner-3.9.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003        0 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3864 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     2985 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/_sample_data.py
+-rw-rw-r--   0 root         (0)     1003     4533 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/conftest.py
+-rw-rw-r--   0 root         (0)     1003    15330 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/test_backup_api.py
+-rw-rw-r--   0 root         (0)     1003    12836 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/test_database_api.py
+-rw-rw-r--   0 root         (0)     1003     9120 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/test_dbapi.py
+-rw-rw-r--   0 root         (0)     1003     4499 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/test_instance_api.py
+-rw-rw-r--   0 root         (0)     1003    71998 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/test_session_api.py
+-rw-rw-r--   0 root         (0)     1003     2381 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/test_streaming_chunking.py
+-rw-rw-r--   0 root         (0)     1003     2324 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/test_table_api.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.555745 google-cloud-spanner-3.9.0/tests/system/utils/
+-rw-rw-r--   0 root         (0)     1003        0 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/utils/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1463 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/utils/clear_streaming.py
+-rw-rw-r--   0 root         (0)     1003     4629 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/utils/populate_streaming.py
+-rw-rw-r--   0 root         (0)     1003     1300 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/utils/scrub_instances.py
+-rw-rw-r--   0 root         (0)     1003     1224 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/system/utils/streaming_utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.559747 google-cloud-spanner-3.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.559747 google-cloud-spanner-3.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.559747 google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_admin_database_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_admin_database_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   212782 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_admin_database_v1/test_database_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.559747 google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_admin_instance_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_admin_instance_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   142880 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_admin_instance_v1/test_instance_admin.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.559747 google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   144545 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_v1/test_spanner.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-08-30 20:24:30.563749 google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/
+-rw-rw-r--   0 root         (0)     1003      595 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4330 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test__helpers.py
+-rw-rw-r--   0 root         (0)     1003     2500 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_checksum.py
+-rw-rw-r--   0 root         (0)     1003     4823 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_connect.py
+-rw-rw-r--   0 root         (0)     1003    22950 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_connection.py
+-rw-rw-r--   0 root         (0)     1003    47193 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_cursor.py
+-rw-rw-r--   0 root         (0)     1003     1128 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_globals.py
+-rw-rw-r--   0 root         (0)     1003    16610 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_parse_utils.py
+-rw-rw-r--   0 root         (0)     1003    11386 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_parser.py
+-rw-rw-r--   0 root         (0)     1003     2307 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_types.py
+-rw-rw-r--   0 root         (0)     1003     4189 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_utils.py
+-rw-rw-r--   0 root         (0)     1003    11747 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/streaming-read-acceptance-test.json
+-rw-rw-r--   0 root         (0)     1003    23720 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test__helpers.py
+-rw-rw-r--   0 root         (0)     1003     5587 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test__opentelemetry_tracing.py
+-rw-rw-r--   0 root         (0)     1003    25072 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test_backup.py
+-rw-rw-r--   0 root         (0)     1003    12420 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test_batch.py
+-rw-rw-r--   0 root         (0)     1003    25216 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test_client.py
+-rw-rw-r--   0 root         (0)     1003    91614 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test_database.py
+-rw-rw-r--   0 root         (0)     1003    41229 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test_instance.py
+-rw-rw-r--   0 root         (0)     1003    14018 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test_keyset.py
+-rw-rw-r--   0 root         (0)     1003     1898 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test_param_types.py
+-rw-rw-r--   0 root         (0)     1003    29666 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test_pool.py
+-rw-rw-r--   0 root         (0)     1003    53986 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test_session.py
+-rw-rw-r--   0 root         (0)     1003    53885 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test_snapshot.py
+-rw-rw-r--   0 root         (0)     1003    46177 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test_streamed.py
+-rw-rw-r--   0 root         (0)     1003     4961 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test_table.py
+-rw-rw-r--   0 root         (0)     1003    27667 2021-08-30 20:21:57.000000 google-cloud-spanner-3.9.0/tests/unit/test_transaction.py
```

### Comparing `google-cloud-spanner-3.8.0/LICENSE` & `google-cloud-spanner-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/MANIFEST.in` & `google-cloud-spanner-3.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/PKG-INFO` & `google-cloud-spanner-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-spanner
-Version: 3.8.0
+Version: 3.9.0
 Summary: Cloud Spanner API client library
 Home-page: https://github.com/googleapis/python-spanner
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-spanner-3.8.0/README.rst` & `google-cloud-spanner-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/gapic_metadata.json` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/async_client.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/client.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/pagers.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/base.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/grpc.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/grpc_asyncio.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/services/database_admin/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/types/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/types/backup.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/types/backup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/types/common.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_database_v1/types/spanner_database_admin.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_database_v1/types/spanner_database_admin.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/gapic_metadata.json` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/async_client.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/client.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/pagers.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/base.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/grpc.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/grpc_asyncio.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/services/instance_admin/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/types/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_admin_instance_v1/types/spanner_instance_admin.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_admin_instance_v1/types/spanner_instance_admin.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/_helpers.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/checksum.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/checksum.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/connection.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/cursor.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/exceptions.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/parse_utils.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/parse_utils.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/parser.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/parser.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/types.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/utils.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/utils.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_dbapi/version.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_dbapi/version.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/_helpers.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,16 @@
     elif type_code == TypeCode.STRUCT:
         return [
             _parse_value_pb(item_pb, field_type.struct_type.fields[i].type_)
             for (i, item_pb) in enumerate(value_pb.list_value.values)
         ]
     elif type_code == TypeCode.NUMERIC:
         return decimal.Decimal(value_pb.string_value)
+    elif type_code == TypeCode.JSON:
+        return value_pb.string_value
     else:
         raise ValueError("Unknown type: %s" % (field_type,))
 
 
 # pylint: enable=too-many-branches
```

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/_opentelemetry_tracing.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/_opentelemetry_tracing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/backup.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/backup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/batch.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/client.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/database.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -690,15 +690,15 @@
             raise ValueError("kms_key_name only used with CUSTOMER_MANAGED_ENCRYPTION")
         api = self._instance._client.database_admin_api
         metadata = _metadata_with_prefix(self.name)
         request = RestoreDatabaseRequest(
             parent=self._instance.name,
             database_id=self.database_id,
             backup=source.name,
-            encryption_config=self._encryption_config,
+            encryption_config=self._encryption_config or None,
         )
         future = api.restore_database(request=request, metadata=metadata,)
         return future
 
     def is_ready(self):
         """Test whether this database is ready for use.
```

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/gapic_metadata.json` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/instance.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/instance.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/keyset.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/keyset.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/param_types.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/param_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 BYTES = Type(code=TypeCode.BYTES)
 BOOL = Type(code=TypeCode.BOOL)
 INT64 = Type(code=TypeCode.INT64)
 FLOAT64 = Type(code=TypeCode.FLOAT64)
 DATE = Type(code=TypeCode.DATE)
 TIMESTAMP = Type(code=TypeCode.TIMESTAMP)
 NUMERIC = Type(code=TypeCode.NUMERIC)
+JSON = Type(code=TypeCode.JSON)
 
 
 def Array(element_type):  # pylint: disable=invalid-name
     """Construct an array parameter type description protobuf.
 
     :type element_type: :class:`~google.cloud.spanner_v1.types.Type`
     :param element_type: the type of elements of the array
```

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/pool.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/pool.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/async_client.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/client.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/pagers.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/transports/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/transports/base.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/transports/grpc.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/services/spanner/transports/grpc_asyncio.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/services/spanner/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/session.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/session.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/snapshot.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/snapshot.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/streamed.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/streamed.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,14 +312,15 @@
     TypeCode.DATE: _merge_string,
     TypeCode.FLOAT64: _merge_float64,
     TypeCode.INT64: _merge_string,
     TypeCode.STRING: _merge_string,
     TypeCode.STRUCT: _merge_struct,
     TypeCode.TIMESTAMP: _merge_string,
     TypeCode.NUMERIC: _merge_string,
+    TypeCode.JSON: _merge_string,
 }
 
 
 def _merge_by_type(lhs, rhs, type_):
     """Helper for '_merge_chunk'."""
     merger = _MERGE_BY_TYPE[type_.code]
     return merger(lhs, rhs, type_)
```

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/table.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/table.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/transaction.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/transaction.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/__init__.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/commit_response.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/commit_response.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/keys.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/keys.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/mutation.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/mutation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/query_plan.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/query_plan.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/result_set.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/result_set.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/spanner.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/spanner.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/transaction.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/transaction.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google/cloud/spanner_v1/types/type.py` & `google-cloud-spanner-3.9.0/google/cloud/spanner_v1/types/type.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/google_cloud_spanner.egg-info/PKG-INFO` & `google-cloud-spanner-3.9.0/google_cloud_spanner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-spanner
-Version: 3.8.0
+Version: 3.9.0
 Summary: Cloud Spanner API client library
 Home-page: https://github.com/googleapis/python-spanner
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-spanner-3.8.0/google_cloud_spanner.egg-info/SOURCES.txt` & `google-cloud-spanner-3.9.0/google_cloud_spanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/setup.py` & `google-cloud-spanner-3.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import setuptools
 
 
 # Package metadata.
 
 name = "google-cloud-spanner"
 description = "Cloud Spanner API client library"
-version = "3.8.0"
+version = "3.9.0"
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     # NOTE: Maintainers, please do not require google-api-core>=2.x.x
```

### Comparing `google-cloud-spanner-3.8.0/tests/__init__.py` & `google-cloud-spanner-3.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/_fixtures.py` & `google-cloud-spanner-3.9.0/tests/_fixtures.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,18 @@
     float_value FLOAT64,
     float_array ARRAY<FLOAT64>,
     string_value STRING(16),
     string_array ARRAY<STRING(16)>,
     timestamp_value TIMESTAMP,
     timestamp_array ARRAY<TIMESTAMP>,
     numeric_value NUMERIC,
-    numeric_array ARRAY<NUMERIC>)
+    numeric_array ARRAY<NUMERIC>,
+    json_value JSON,
+    json_array ARRAY<JSON>,
+    )
     PRIMARY KEY (pkey);
 CREATE TABLE counters (
     name STRING(1024),
     value INT64 )
     PRIMARY KEY (name);
 CREATE TABLE string_plus_array_of_string (
     id INT64,
```

### Comparing `google-cloud-spanner-3.8.0/tests/_helpers.py` & `google-cloud-spanner-3.9.0/tests/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/system/_helpers.py` & `google-cloud-spanner-3.9.0/tests/system/_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,19 @@
 INSTANCE_ID_ENVVAR = "GOOGLE_CLOUD_TESTS_SPANNER_INSTANCE"
 INSTANCE_ID_DEFAULT = "google-cloud-python-systest"
 INSTANCE_ID = os.environ.get(INSTANCE_ID_ENVVAR, INSTANCE_ID_DEFAULT)
 
 SKIP_BACKUP_TESTS_ENVVAR = "SKIP_BACKUP_TESTS"
 SKIP_BACKUP_TESTS = os.getenv(SKIP_BACKUP_TESTS_ENVVAR) is not None
 
-SPANNER_OPERATION_TIMEOUT_IN_SECONDS = int(
-    os.getenv("SPANNER_OPERATION_TIMEOUT_IN_SECONDS", 60)
+INSTANCE_OPERATION_TIMEOUT_IN_SECONDS = int(
+    os.getenv("SPANNER_INSTANCE_OPERATION_TIMEOUT_IN_SECONDS", 240)
+)
+DATABASE_OPERATION_TIMEOUT_IN_SECONDS = int(
+    os.getenv("SPANNER_DATABASE_OPERATION_TIMEOUT_IN_SECONDS", 60)
 )
 
 USE_EMULATOR_ENVVAR = "SPANNER_EMULATOR_HOST"
 USE_EMULATOR = os.getenv(USE_EMULATOR_ENVVAR) is not None
 
 EMULATOR_PROJECT_ENVVAR = "GCLOUD_PROJECT"
 EMULATOR_PROJECT_DEFAULT = "emulator-test-project"
```

### Comparing `google-cloud-spanner-3.8.0/tests/system/_sample_data.py` & `google-cloud-spanner-3.9.0/tests/system/_sample_data.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/system/conftest.py` & `google-cloud-spanner-3.9.0/tests/system/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,16 +54,21 @@
             project=_helpers.EMULATOR_PROJECT, credentials=credentials,
         )
     else:
         return spanner_v1.Client()  # use google.auth.default credentials
 
 
 @pytest.fixture(scope="session")
-def operation_timeout():
-    return _helpers.SPANNER_OPERATION_TIMEOUT_IN_SECONDS
+def instance_operation_timeout():
+    return _helpers.INSTANCE_OPERATION_TIMEOUT_IN_SECONDS
+
+
+@pytest.fixture(scope="session")
+def database_operation_timeout():
+    return _helpers.DATABASE_OPERATION_TIMEOUT_IN_SECONDS
 
 
 @pytest.fixture(scope="session")
 def shared_instance_id():
     if _helpers.CREATE_INSTANCE:
         return f"{_helpers.unique_id('google-cloud')}"
 
@@ -97,50 +102,50 @@
 
     yield instances
 
 
 @pytest.fixture(scope="session")
 def shared_instance(
     spanner_client,
-    operation_timeout,
+    instance_operation_timeout,
     shared_instance_id,
     instance_config,
     existing_instances,  # evalutate before creating one
 ):
     _helpers.cleanup_old_instances(spanner_client)
 
     if _helpers.CREATE_INSTANCE:
         create_time = str(int(time.time()))
         labels = {"python-spanner-systests": "true", "created": create_time}
 
         instance = spanner_client.instance(
             shared_instance_id, instance_config.name, labels=labels
         )
         created_op = _helpers.retry_429_503(instance.create)()
-        created_op.result(operation_timeout)  # block until completion
+        created_op.result(instance_operation_timeout)  # block until completion
 
     else:  # reuse existing instance
         instance = spanner_client.instance(shared_instance_id)
         instance.reload()
 
     yield instance
 
     if _helpers.CREATE_INSTANCE:
         _helpers.retry_429_503(instance.delete)()
 
 
 @pytest.fixture(scope="session")
-def shared_database(shared_instance, operation_timeout):
+def shared_database(shared_instance, database_operation_timeout):
     database_name = _helpers.unique_id("test_database")
     pool = spanner_v1.BurstyPool(labels={"testcase": "database_api"})
     database = shared_instance.database(
         database_name, ddl_statements=_helpers.DDL_STATEMENTS, pool=pool
     )
     operation = database.create()
-    operation.result(operation_timeout)  # raises on failure / timeout.
+    operation.result(database_operation_timeout)  # raises on failure / timeout.
 
     yield database
 
     database.drop()
 
 
 @pytest.fixture(scope="function")
```

### Comparing `google-cloud-spanner-3.8.0/tests/system/test_backup_api.py` & `google-cloud-spanner-3.9.0/tests/system/test_backup_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,24 +29,24 @@
 pytestmark = [
     pytest.mark.skipif(_helpers.SKIP_BACKUP_TESTS, reason=skip_env_reason),
     pytest.mark.skipif(_helpers.USE_EMULATOR, reason=skip_emulator_reason),
 ]
 
 
 @pytest.fixture(scope="session")
-def same_config_instance(spanner_client, shared_instance, operation_timeout):
+def same_config_instance(spanner_client, shared_instance, instance_operation_timeout):
     current_config = shared_instance.configuration_name
     same_config_instance_id = _helpers.unique_id("same-config")
     create_time = str(int(time.time()))
     labels = {"python-spanner-systests": "true", "created": create_time}
     same_config_instance = spanner_client.instance(
         same_config_instance_id, current_config, labels=labels
     )
     op = same_config_instance.create()
-    op.result(operation_timeout)
+    op.result(instance_operation_timeout)
 
     yield same_config_instance
 
     _helpers.scrub_instance_ignore_not_found(same_config_instance)
 
 
 @pytest.fixture(scope="session")
@@ -56,47 +56,52 @@
         if "-us-" in config.name and config.name != current_config:
             return config.name
     return None
 
 
 @pytest.fixture(scope="session")
 def diff_config_instance(
-    spanner_client, shared_instance, operation_timeout, diff_config,
+    spanner_client, shared_instance, instance_operation_timeout, diff_config,
 ):
     if diff_config is None:
         return None
 
     diff_config_instance_id = _helpers.unique_id("diff-config")
     create_time = str(int(time.time()))
     labels = {"python-spanner-systests": "true", "created": create_time}
     diff_config_instance = spanner_client.instance(
         diff_config_instance_id, diff_config, labels=labels
     )
     op = diff_config_instance.create()
-    op.result(operation_timeout)
+    op.result(instance_operation_timeout)
 
     yield diff_config_instance
 
     _helpers.scrub_instance_ignore_not_found(diff_config_instance)
 
 
 @pytest.fixture(scope="session")
-def database_version_time():
-    return datetime.datetime.utcnow().replace(tzinfo=datetime.timezone.utc)
+def database_version_time(shared_database):
+    shared_database.reload()
+    diff = (
+        datetime.datetime.now(datetime.timezone.utc)
+        - shared_database.earliest_version_time
+    )
+    return shared_database.earliest_version_time + diff / 2
 
 
 @pytest.fixture(scope="session")
-def second_database(shared_instance, operation_timeout):
+def second_database(shared_instance, database_operation_timeout):
     database_name = _helpers.unique_id("test_database2")
     pool = spanner_v1.BurstyPool(labels={"testcase": "database_api"})
     database = shared_instance.database(
         database_name, ddl_statements=_helpers.DDL_STATEMENTS, pool=pool
     )
     operation = database.create()
-    operation.result(operation_timeout)  # raises on failure / timeout.
+    operation.result(database_operation_timeout)  # raises on failure / timeout.
 
     yield database
 
     database.drop()
 
 
 @pytest.fixture(scope="function")
@@ -120,16 +125,17 @@
         CreateBackupEncryptionConfig,
         EncryptionConfig,
         EncryptionInfo,
         RestoreDatabaseEncryptionConfig,
     )
 
     backup_id = _helpers.unique_id("backup_id", separator="_")
-    expire_time = datetime.datetime.utcnow() + datetime.timedelta(days=3)
-    expire_time = expire_time.replace(tzinfo=datetime.timezone.utc)
+    expire_time = datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
+        days=3
+    )
     encryption_enum = CreateBackupEncryptionConfig.EncryptionType
     encryption_config = CreateBackupEncryptionConfig(
         encryption_type=encryption_enum.GOOGLE_DEFAULT_ENCRYPTION,
     )
 
     # Create backup.
     backup = shared_instance.backup(
@@ -158,16 +164,17 @@
     assert backup.state is not None
     assert (
         EncryptionInfo.Type.GOOGLE_DEFAULT_ENCRYPTION
         == backup.encryption_info.encryption_type
     )
 
     # Update with valid argument.
-    valid_expire_time = datetime.datetime.utcnow() + datetime.timedelta(days=7)
-    valid_expire_time = valid_expire_time.replace(tzinfo=datetime.timezone.utc)
+    valid_expire_time = datetime.datetime.now(
+        datetime.timezone.utc
+    ) + datetime.timedelta(days=7)
     backup.update_expire_time(valid_expire_time)
     assert valid_expire_time == backup.expire_time
 
     # Restore database to same instance.
     restored_id = _helpers.unique_id("restored_db", separator="_")
     encryption_config = RestoreDatabaseEncryptionConfig(
         encryption_type=RestoreDatabaseEncryptionConfig.EncryptionType.GOOGLE_DEFAULT_ENCRYPTION,
@@ -189,23 +196,20 @@
 
     database.drop()
     backup.delete()
     assert not backup.exists()
 
 
 def test_backup_create_w_version_time_dflt_to_create_time(
-    shared_instance,
-    shared_database,
-    database_version_time,
-    backups_to_delete,
-    databases_to_delete,
+    shared_instance, shared_database, backups_to_delete, databases_to_delete,
 ):
     backup_id = _helpers.unique_id("backup_id", separator="_")
-    expire_time = datetime.datetime.utcnow() + datetime.timedelta(days=3)
-    expire_time = expire_time.replace(tzinfo=datetime.timezone.utc)
+    expire_time = datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
+        days=3
+    )
 
     # Create backup.
     backup = shared_instance.backup(
         backup_id, database=shared_database, expire_time=expire_time,
     )
     operation = backup.create()
     backups_to_delete.append(backup)
@@ -224,33 +228,35 @@
 
     backup.delete()
     assert not backup.exists()
 
 
 def test_backup_create_w_invalid_expire_time(shared_instance, shared_database):
     backup_id = _helpers.unique_id("backup_id", separator="_")
-    expire_time = datetime.datetime.utcnow().replace(tzinfo=datetime.timezone.utc)
+    expire_time = datetime.datetime.now(datetime.timezone.utc)
 
     backup = shared_instance.backup(
         backup_id, database=shared_database, expire_time=expire_time
     )
 
     with pytest.raises(exceptions.InvalidArgument):
         op = backup.create()
         op.result()  # blocks indefinitely
 
 
 def test_backup_create_w_invalid_version_time_past(
     shared_instance, shared_database,
 ):
     backup_id = _helpers.unique_id("backup_id", separator="_")
-    expire_time = datetime.datetime.utcnow() + datetime.timedelta(days=3)
-    expire_time = expire_time.replace(tzinfo=datetime.timezone.utc)
-    version_time = datetime.datetime.utcnow() - datetime.timedelta(days=10)
-    version_time = version_time.replace(tzinfo=datetime.timezone.utc)
+    expire_time = datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
+        days=3
+    )
+    version_time = datetime.datetime.now(datetime.timezone.utc) - datetime.timedelta(
+        days=10
+    )
 
     backup = shared_instance.backup(
         backup_id,
         database=shared_database,
         expire_time=expire_time,
         version_time=version_time,
     )
@@ -260,18 +266,20 @@
         op.result()  # blocks indefinitely
 
 
 def test_backup_create_w_invalid_version_time_future(
     shared_instance, shared_database,
 ):
     backup_id = _helpers.unique_id("backup_id", separator="_")
-    expire_time = datetime.datetime.utcnow() + datetime.timedelta(days=3)
-    expire_time = expire_time.replace(tzinfo=datetime.timezone.utc)
-    version_time = datetime.datetime.utcnow() + datetime.timedelta(days=2)
-    version_time = version_time.replace(tzinfo=datetime.timezone.utc)
+    expire_time = datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
+        days=3
+    )
+    version_time = datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
+        days=2
+    )
 
     backup = shared_instance.backup(
         backup_id,
         database=shared_database,
         expire_time=expire_time,
         version_time=version_time,
     )
@@ -285,16 +293,17 @@
     shared_instance,
     shared_database,
     backups_to_delete,
     same_config_instance,
     databases_to_delete,
 ):
     backup_id = _helpers.unique_id("backup_id", separator="_")
-    expire_time = datetime.datetime.utcnow() + datetime.timedelta(days=3)
-    expire_time = expire_time.replace(tzinfo=datetime.timezone.utc)
+    expire_time = datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
+        days=3
+    )
 
     # Create backup.
     backup = shared_instance.backup(
         backup_id, database=shared_database, expire_time=expire_time,
     )
     op = backup.create()
     backups_to_delete.append(backup)
@@ -315,20 +324,20 @@
 def test_multi_create_cancel_update_error_restore_errors(
     shared_instance,
     shared_database,
     second_database,
     diff_config_instance,
     backups_to_delete,
     databases_to_delete,
-    operation_timeout,
 ):
     backup_id_1 = _helpers.unique_id("backup_id1", separator="_")
     backup_id_2 = _helpers.unique_id("backup_id2", separator="_")
-    expire_time = datetime.datetime.utcnow() + datetime.timedelta(days=3)
-    expire_time = expire_time.replace(tzinfo=datetime.timezone.utc)
+    expire_time = datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
+        days=3
+    )
 
     backup1 = shared_instance.backup(
         backup_id_1, database=shared_database, expire_time=expire_time
     )
     backup2 = shared_instance.backup(
         backup_id_2, database=second_database, expire_time=expire_time
     )
@@ -351,16 +360,16 @@
 
     op1.result()  # blocks indefinitely
     backup1.reload()
     assert backup1.is_ready()
 
     # Update expire time to invalid value.
     max_expire_days = 366  # documented maximum
-    invalid_expire_time = datetime.datetime.now().replace(
-        tzinfo=datetime.timezone.utc
+    invalid_expire_time = datetime.datetime.now(
+        datetime.timezone.utc
     ) + datetime.timedelta(days=max_expire_days + 1)
     with pytest.raises(exceptions.InvalidArgument):
         backup1.update_expire_time(invalid_expire_time)
 
     # Restore to existing database.
     with pytest.raises(exceptions.AlreadyExists):
         shared_database.restore(source=backup1)
@@ -382,40 +391,40 @@
 ):
     # Remove un-scrubbed backups FBO count below.
     _helpers.scrub_instance_backups(shared_instance)
 
     backup_id_1 = _helpers.unique_id("backup_id1", separator="_")
     backup_id_2 = _helpers.unique_id("backup_id2", separator="_")
 
-    expire_time_1 = datetime.datetime.utcnow() + datetime.timedelta(days=21)
-    expire_time_1 = expire_time_1.replace(tzinfo=datetime.timezone.utc)
+    expire_time_1 = datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
+        days=21
+    )
     expire_time_1_stamp = expire_time_1.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
 
     backup1 = shared_instance.backup(
         backup_id_1,
         database=shared_database,
         expire_time=expire_time_1,
         version_time=database_version_time,
     )
 
-    expire_time_2 = datetime.datetime.utcnow() + datetime.timedelta(days=1)
-    expire_time_2 = expire_time_2.replace(tzinfo=datetime.timezone.utc)
+    expire_time_2 = datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
+        days=1
+    )
     backup2 = shared_instance.backup(
         backup_id_2, database=second_database, expire_time=expire_time_2
     )
 
     # Create two backups.
     op1 = backup1.create()
     backups_to_delete.append(backup1)
     op1.result()  # blocks indefinitely
     backup1.reload()
 
-    create_time_compare = datetime.datetime.utcnow().replace(
-        tzinfo=datetime.timezone.utc
-    )
+    create_time_compare = datetime.datetime.now(datetime.timezone.utc)
     create_time_stamp = create_time_compare.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
 
     backup2.create()
     # This test doesn't block for the result of the 'backup2.create()' call
     # because it wants to find `backup2` in the upcoming search for
     # backups matching 'state;CREATING`:  inherently racy, but probably
     # safe, given how long it takes to create a backup (on the order of
```

### Comparing `google-cloud-spanner-3.8.0/tests/system/test_database_api.py` & `google-cloud-spanner-3.9.0/tests/system/test_database_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,29 +23,29 @@
 from . import _sample_data
 
 
 DBAPI_OPERATION_TIMEOUT = 240  # seconds
 
 
 @pytest.fixture(scope="module")
-def multiregion_instance(spanner_client, operation_timeout):
+def multiregion_instance(spanner_client, instance_operation_timeout):
     multi_region_instance_id = _helpers.unique_id("multi-region")
     multi_region_config = "nam3"
     config_name = "{}/instanceConfigs/{}".format(
         spanner_client.project_name, multi_region_config
     )
     create_time = str(int(time.time()))
     labels = {"python-spanner-systests": "true", "created": create_time}
     multiregion_instance = spanner_client.instance(
         instance_id=multi_region_instance_id,
         configuration_name=config_name,
         labels=labels,
     )
     operation = _helpers.retry_429_503(multiregion_instance.create)()
-    operation.result(operation_timeout)
+    operation.result(instance_operation_timeout)
 
     yield multiregion_instance
 
     _helpers.retry_429_503(multiregion_instance.delete)()
 
 
 def test_list_databases(shared_instance, shared_database):
```

### Comparing `google-cloud-spanner-3.8.0/tests/system/test_dbapi.py` & `google-cloud-spanner-3.9.0/tests/system/test_dbapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,22 +31,22 @@
         email STRING(1024)
     )
     PRIMARY KEY (contact_id)""",
 )
 
 
 @pytest.fixture(scope="session")
-def raw_database(shared_instance, operation_timeout):
+def raw_database(shared_instance, database_operation_timeout):
     databse_id = _helpers.unique_id("dbapi-txn")
     pool = spanner_v1.BurstyPool(labels={"testcase": "database_api"})
     database = shared_instance.database(
         databse_id, ddl_statements=DDL_STATEMENTS, pool=pool,
     )
     op = database.create()
-    op.result(operation_timeout)  # raises on failure / timeout.
+    op.result(database_operation_timeout)  # raises on failure / timeout.
 
     yield database
 
     database.drop()
 
 
 def clear_table(transaction):
```

### Comparing `google-cloud-spanner-3.8.0/tests/system/test_instance_api.py` & `google-cloud-spanner-3.9.0/tests/system/test_instance_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,24 +57,24 @@
 
 
 def test_create_instance(
     if_create_instance,
     spanner_client,
     instance_config,
     instances_to_delete,
-    operation_timeout,
+    instance_operation_timeout,
 ):
     alt_instance_id = _helpers.unique_id("new")
     instance = spanner_client.instance(alt_instance_id, instance_config.name)
     operation = instance.create()
     # Make sure this instance gets deleted after the test case.
     instances_to_delete.append(instance)
 
     # We want to make sure the operation completes.
-    operation.result(operation_timeout)  # raises on failure / timeout.
+    operation.result(instance_operation_timeout)  # raises on failure / timeout.
 
     # Create a new instance instance and make sure it is the same.
     instance_alt = spanner_client.instance(alt_instance_id, instance_config.name)
     instance_alt.reload()
 
     assert instance == instance_alt
     instance.display_name == instance_alt.display_name
@@ -82,29 +82,29 @@
 
 def test_create_instance_with_processing_units(
     not_emulator,
     if_create_instance,
     spanner_client,
     instance_config,
     instances_to_delete,
-    operation_timeout,
+    instance_operation_timeout,
 ):
     alt_instance_id = _helpers.unique_id("wpn")
     processing_units = 5000
     instance = spanner_client.instance(
         instance_id=alt_instance_id,
         configuration_name=instance_config.name,
         processing_units=processing_units,
     )
     operation = instance.create()
     # Make sure this instance gets deleted after the test case.
     instances_to_delete.append(instance)
 
     # We want to make sure the operation completes.
-    operation.result(operation_timeout)  # raises on failure / timeout.
+    operation.result(instance_operation_timeout)  # raises on failure / timeout.
 
     # Create a new instance instance and make sure it is the same.
     instance_alt = spanner_client.instance(alt_instance_id, instance_config.name)
     instance_alt.reload()
 
     assert instance == instance_alt
     assert instance.display_name == instance_alt.display_name
@@ -112,23 +112,23 @@
 
 
 def test_update_instance(
     not_emulator,
     spanner_client,
     shared_instance,
     shared_instance_id,
-    operation_timeout,
+    instance_operation_timeout,
 ):
     old_display_name = shared_instance.display_name
     new_display_name = "Foo Bar Baz"
     shared_instance.display_name = new_display_name
     operation = shared_instance.update()
 
     # We want to make sure the operation completes.
-    operation.result(operation_timeout)  # raises on failure / timeout.
+    operation.result(instance_operation_timeout)  # raises on failure / timeout.
 
     # Create a new instance instance and reload it.
     instance_alt = spanner_client.instance(shared_instance_id, None)
     assert instance_alt.display_name != new_display_name
 
     instance_alt.reload()
     assert instance_alt.display_name == new_display_name
```

### Comparing `google-cloud-spanner-3.8.0/tests/system/test_session_api.py` & `google-cloud-spanner-3.9.0/tests/system/test_session_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import collections
 import datetime
 import decimal
 import math
 import struct
 import threading
 import time
-
+import json
 import pytest
 
 import grpc
 from google.rpc import code_pb2
 from google.api_core import datetime_helpers
 from google.api_core import exceptions
 from google.cloud import spanner_v1
@@ -39,14 +39,32 @@
 POS_INF = float("+inf")
 NEG_INF = float("-inf")
 (OTHER_NAN,) = struct.unpack("<d", b"\x01\x00\x01\x00\x00\x00\xf8\xff")
 BYTES_1 = b"Ymlu"
 BYTES_2 = b"Ym9vdHM="
 NUMERIC_1 = decimal.Decimal("0.123456789")
 NUMERIC_2 = decimal.Decimal("1234567890")
+JSON_1 = json.dumps(
+    {
+        "sample_boolean": True,
+        "sample_int": 872163,
+        "sample float": 7871.298,
+        "sample_null": None,
+        "sample_string": "abcdef",
+        "sample_array": [23, 76, 19],
+    },
+    sort_keys=True,
+    separators=(",", ":"),
+)
+JSON_2 = json.dumps(
+    {"sample_object": {"name": "Anamika", "id": 2635}},
+    sort_keys=True,
+    separators=(",", ":"),
+)
+
 COUNTERS_TABLE = "counters"
 COUNTERS_COLUMNS = ("name", "value")
 ALL_TYPES_TABLE = "all_types"
 LIVE_ALL_TYPES_COLUMNS = (
     "pkey",
     "int_value",
     "int_array",
@@ -60,16 +78,18 @@
     "float_array",
     "string_value",
     "string_array",
     "timestamp_value",
     "timestamp_array",
     "numeric_value",
     "numeric_array",
+    "json_value",
+    "json_array",
 )
-EMULATOR_ALL_TYPES_COLUMNS = LIVE_ALL_TYPES_COLUMNS[:-2]
+EMULATOR_ALL_TYPES_COLUMNS = LIVE_ALL_TYPES_COLUMNS[:-4]
 AllTypesRowData = collections.namedtuple("AllTypesRowData", LIVE_ALL_TYPES_COLUMNS)
 AllTypesRowData.__new__.__defaults__ = tuple([None for colum in LIVE_ALL_TYPES_COLUMNS])
 EmulatorAllTypesRowData = collections.namedtuple(
     "EmulatorAllTypesRowData", EMULATOR_ALL_TYPES_COLUMNS
 )
 EmulatorAllTypesRowData.__new__.__defaults__ = tuple(
     [None for colum in EMULATOR_ALL_TYPES_COLUMNS]
@@ -84,32 +104,35 @@
     AllTypesRowData(pkey=103, bytes_value=BYTES_1),
     AllTypesRowData(pkey=104, date_value=SOME_DATE),
     AllTypesRowData(pkey=105, float_value=1.4142136),
     AllTypesRowData(pkey=106, string_value="VALUE"),
     AllTypesRowData(pkey=107, timestamp_value=SOME_TIME),
     AllTypesRowData(pkey=108, timestamp_value=NANO_TIME),
     AllTypesRowData(pkey=109, numeric_value=NUMERIC_1),
+    AllTypesRowData(pkey=110, json_value=JSON_1),
     # empty array values
     AllTypesRowData(pkey=201, int_array=[]),
     AllTypesRowData(pkey=202, bool_array=[]),
     AllTypesRowData(pkey=203, bytes_array=[]),
     AllTypesRowData(pkey=204, date_array=[]),
     AllTypesRowData(pkey=205, float_array=[]),
     AllTypesRowData(pkey=206, string_array=[]),
     AllTypesRowData(pkey=207, timestamp_array=[]),
     AllTypesRowData(pkey=208, numeric_array=[]),
+    AllTypesRowData(pkey=209, json_array=[]),
     # non-empty array values, including nulls
     AllTypesRowData(pkey=301, int_array=[123, 456, None]),
     AllTypesRowData(pkey=302, bool_array=[True, False, None]),
     AllTypesRowData(pkey=303, bytes_array=[BYTES_1, BYTES_2, None]),
     AllTypesRowData(pkey=304, date_array=[SOME_DATE, None]),
     AllTypesRowData(pkey=305, float_array=[3.1415926, 2.71828, None]),
     AllTypesRowData(pkey=306, string_array=["One", "Two", None]),
     AllTypesRowData(pkey=307, timestamp_array=[SOME_TIME, NANO_TIME, None]),
     AllTypesRowData(pkey=308, numeric_array=[NUMERIC_1, NUMERIC_2, None]),
+    AllTypesRowData(pkey=309, json_array=[JSON_1, JSON_2, None]),
 )
 EMULATOR_ALL_TYPES_ROWDATA = (
     # all nulls
     EmulatorAllTypesRowData(pkey=0),
     # Non-null values
     EmulatorAllTypesRowData(pkey=101, int_value=123),
     EmulatorAllTypesRowData(pkey=102, bool_value=False),
@@ -142,22 +165,22 @@
     ALL_TYPES_ROWDATA = EMULATOR_ALL_TYPES_ROWDATA
 else:
     ALL_TYPES_COLUMNS = LIVE_ALL_TYPES_COLUMNS
     ALL_TYPES_ROWDATA = LIVE_ALL_TYPES_ROWDATA
 
 
 @pytest.fixture(scope="session")
-def sessions_database(shared_instance, operation_timeout):
+def sessions_database(shared_instance, database_operation_timeout):
     database_name = _helpers.unique_id("test_sessions", separator="_")
     pool = spanner_v1.BurstyPool(labels={"testcase": "session_api"})
     sessions_database = shared_instance.database(
         database_name, ddl_statements=_helpers.DDL_STATEMENTS, pool=pool,
     )
     operation = sessions_database.create()
-    operation.result(operation_timeout)  # raises on failure / timeout.
+    operation.result(database_operation_timeout)  # raises on failure / timeout.
 
     _helpers.retry_has_all_dll(sessions_database.reload)()
     # Some tests expect there to be a session present in the pool.
     pool.put(pool.get())
 
     yield sessions_database
 
@@ -1172,15 +1195,15 @@
         with sessions_database.batch() as batch:
             batch.delete(sd.TABLE, sd.ALL)
 
         after = list(exact.read(sd.TABLE, sd.COLUMNS, sd.ALL))
         sd._check_row_data(after, all_data_rows)
 
 
-def test_read_w_index(shared_instance, operation_timeout, databases_to_delete):
+def test_read_w_index(shared_instance, database_operation_timeout, databases_to_delete):
     # Indexed reads cannot return non-indexed columns
     sd = _sample_data
     row_count = 2000
     my_columns = sd.COLUMNS[0], sd.COLUMNS[2]
 
     # Create an alternate dataase w/ index.
     extra_ddl = ["CREATE INDEX contacts_by_last_name ON contacts(last_name)"]
@@ -1188,15 +1211,15 @@
     temp_db = shared_instance.database(
         _helpers.unique_id("test_read", separator="_"),
         ddl_statements=_helpers.DDL_STATEMENTS + extra_ddl,
         pool=pool,
     )
     operation = temp_db.create()
     databases_to_delete.append(temp_db)
-    operation.result(operation_timeout)  # raises on failure / timeout.
+    operation.result(database_operation_timeout)  # raises on failure / timeout.
 
     committed = _set_up_table(temp_db, row_count)
 
     with temp_db.snapshot(read_timestamp=committed) as snapshot:
         rows = list(
             snapshot.read(sd.TABLE, my_columns, sd.ALL, index="contacts_by_last_name")
         )
@@ -1863,14 +1886,20 @@
         sessions_database,
         spanner_v1.TypeCode.NUMERIC,
         NUMERIC_1,
         [NUMERIC_1, NUMERIC_2],
     )
 
 
+def test_execute_sql_w_json_bindings(not_emulator, sessions_database):
+    _bind_test_helper(
+        sessions_database, spanner_v1.TypeCode.JSON, JSON_1, [JSON_1, JSON_2],
+    )
+
+
 def test_execute_sql_w_query_param_struct(sessions_database):
     name = "Phred"
     count = 123
     size = 23.456
     height = 188.0
     weight = 97.6
     param_types = spanner_v1.param_types
```

### Comparing `google-cloud-spanner-3.8.0/tests/system/test_streaming_chunking.py` & `google-cloud-spanner-3.9.0/tests/system/test_streaming_chunking.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/system/test_table_api.py` & `google-cloud-spanner-3.9.0/tests/system/test_table_api.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/system/utils/clear_streaming.py` & `google-cloud-spanner-3.9.0/tests/system/utils/clear_streaming.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/system/utils/populate_streaming.py` & `google-cloud-spanner-3.9.0/tests/system/utils/populate_streaming.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/system/utils/scrub_instances.py` & `google-cloud-spanner-3.9.0/tests/system/utils/scrub_instances.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/system/utils/streaming_utils.py` & `google-cloud-spanner-3.9.0/tests/system/utils/streaming_utils.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/__init__.py` & `google-cloud-spanner-3.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/gapic/__init__.py` & `google-cloud-spanner-3.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_admin_database_v1/__init__.py` & `google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_admin_database_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_admin_database_v1/test_database_admin.py` & `google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_admin_database_v1/test_database_admin.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_admin_instance_v1/__init__.py` & `google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_admin_instance_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_admin_instance_v1/test_instance_admin.py` & `google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_admin_instance_v1/test_instance_admin.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_v1/__init__.py` & `google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/gapic/spanner_v1/test_spanner.py` & `google-cloud-spanner-3.9.0/tests/unit/gapic/spanner_v1/test_spanner.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/__init__.py` & `google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test__helpers.py` & `google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test__helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_checksum.py` & `google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_checksum.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_connect.py` & `google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_connect.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_connection.py` & `google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_connection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_cursor.py` & `google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_cursor.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_globals.py` & `google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_globals.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_parse_utils.py` & `google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_parse_utils.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_parser.py` & `google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_parser.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_types.py` & `google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/spanner_dbapi/test_utils.py` & `google-cloud-spanner-3.9.0/tests/unit/spanner_dbapi/test_utils.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/streaming-read-acceptance-test.json` & `google-cloud-spanner-3.9.0/tests/unit/streaming-read-acceptance-test.json`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test__helpers.py` & `google-cloud-spanner-3.9.0/tests/unit/test__helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,14 +291,25 @@
 
         for value, err_msg in cases:
             with self.subTest(value=value, err_msg=err_msg):
                 self.assertRaisesRegex(
                     ValueError, err_msg, lambda: self._callFUT(value),
                 )
 
+    def test_w_json(self):
+        import json
+        from google.protobuf.struct_pb2 import Value
+
+        value = json.dumps(
+            {"id": 27863, "Name": "Anamika"}, sort_keys=True, separators=(",", ":")
+        )
+        value_pb = self._callFUT(value)
+        self.assertIsInstance(value_pb, Value)
+        self.assertEqual(value_pb.string_value, value)
+
 
 class Test_make_list_value_pb(unittest.TestCase):
     def _callFUT(self, *args, **kw):
         from google.cloud.spanner_v1._helpers import _make_list_value_pb
 
         return _make_list_value_pb(*args, **kw)
 
@@ -548,14 +559,28 @@
 
         VALUE = decimal.Decimal("99999999999999999999999999999.999999999")
         field_type = Type(code=TypeCode.NUMERIC)
         value_pb = Value(string_value=str(VALUE))
 
         self.assertEqual(self._callFUT(value_pb, field_type), VALUE)
 
+    def test_w_json(self):
+        import json
+        from google.protobuf.struct_pb2 import Value
+        from google.cloud.spanner_v1 import Type
+        from google.cloud.spanner_v1 import TypeCode
+
+        VALUE = json.dumps(
+            {"id": 27863, "Name": "Anamika"}, sort_keys=True, separators=(",", ":")
+        )
+        field_type = Type(code=TypeCode.JSON)
+        value_pb = Value(string_value=VALUE)
+
+        self.assertEqual(self._callFUT(value_pb, field_type), VALUE)
+
     def test_w_unknown_type(self):
         from google.protobuf.struct_pb2 import Value
         from google.cloud.spanner_v1 import Type
         from google.cloud.spanner_v1 import TypeCode
 
         field_type = Type(code=TypeCode.TYPE_CODE_UNSPECIFIED)
         value_pb = Value(string_value="Borked")
```

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test__opentelemetry_tracing.py` & `google-cloud-spanner-3.9.0/tests/unit/test__opentelemetry_tracing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test_backup.py` & `google-cloud-spanner-3.9.0/tests/unit/test_backup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test_batch.py` & `google-cloud-spanner-3.9.0/tests/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test_client.py` & `google-cloud-spanner-3.9.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test_database.py` & `google-cloud-spanner-3.9.0/tests/unit/test_database.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test_instance.py` & `google-cloud-spanner-3.9.0/tests/unit/test_instance.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test_keyset.py` & `google-cloud-spanner-3.9.0/tests/unit/test_keyset.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test_param_types.py` & `google-cloud-spanner-3.9.0/tests/unit/test_param_types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test_pool.py` & `google-cloud-spanner-3.9.0/tests/unit/test_pool.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test_session.py` & `google-cloud-spanner-3.9.0/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test_snapshot.py` & `google-cloud-spanner-3.9.0/tests/unit/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test_streamed.py` & `google-cloud-spanner-3.9.0/tests/unit/test_streamed.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test_table.py` & `google-cloud-spanner-3.9.0/tests/unit/test_table.py`

 * *Files identical despite different names*

### Comparing `google-cloud-spanner-3.8.0/tests/unit/test_transaction.py` & `google-cloud-spanner-3.9.0/tests/unit/test_transaction.py`

 * *Files identical despite different names*

