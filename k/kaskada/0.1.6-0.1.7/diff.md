# Comparing `tmp/kaskada-0.1.6.tar.gz` & `tmp/kaskada-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaskada-0.1.6.tar", max compression
+gzip compressed data, was "kaskada-0.1.7.tar", max compression
```

## Comparing `kaskada-0.1.6.tar` & `kaskada-0.1.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1646 2023-04-26 19:24:50.174096 kaskada-0.1.6/README.md
--rw-r--r--   0        0        0     3882 2023-04-26 19:24:50.174096 kaskada-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     7208 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/fenlmagic/__init__.py
--rw-r--r--   0        0        0      401 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/fenlmagic/utils.py
--rw-r--r--   0        0        0       33 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/api/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/api/api_utils.py
--rw-r--r--   0        0        0     6381 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/api/release.py
--rw-r--r--   0        0        0     9507 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/api/session.py
--rw-r--r--   0        0        0     5838 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/client.py
--rw-r--r--   0        0        0     1500 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/formatters.css
--rw-r--r--   0        0        0      984 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/formatters.js
--rw-r--r--   0        0        0    26206 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/formatters.py
--rw-r--r--   0        0        0     7337 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/formatters_helpers.py
--rw-r--r--   0        0        0     9833 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/formatters_shared.py
--rw-r--r--   0        0        0     7394 2023-04-26 19:24:50.738094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/common_pb2.py
--rw-r--r--   0        0        0      159 2023-04-26 19:24:50.734094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
--rw-r--r--   0        0        0    10615 2023-04-26 19:24:50.782094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
--rw-r--r--   0        0        0     6628 2023-04-26 19:24:50.782094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
--rw-r--r--   0        0        0     4489 2023-04-26 19:24:50.822094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
--rw-r--r--   0        0        0     2938 2023-04-26 19:24:50.818094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
--rw-r--r--   0        0        0     4191 2023-04-26 19:24:50.862094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/destinations_pb2.py
--rw-r--r--   0        0        0      159 2023-04-26 19:24:50.886094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
--rw-r--r--   0        0        0     2668 2023-04-26 19:24:50.894094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
--rw-r--r--   0        0        0      159 2023-04-26 19:24:50.946094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
--rw-r--r--   0        0        0     3976 2023-04-26 19:24:50.926094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/file_service_pb2.py
--rw-r--r--   0        0        0     5054 2023-04-26 19:24:50.970094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
--rw-r--r--   0        0        0    10837 2023-04-26 19:24:50.990094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
--rw-r--r--   0        0        0     9283 2023-04-26 19:24:51.010094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     1897 2023-04-26 19:24:51.026094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/options_pb2.py
--rw-r--r--   0        0        0      159 2023-04-26 19:24:51.042094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
--rw-r--r--   0        0        0    13180 2023-04-26 19:24:51.058094 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/plan_pb2.py
--rw-r--r--   0        0        0      159 2023-04-26 19:24:51.114093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
--rw-r--r--   0        0        0     3398 2023-04-26 19:24:51.094093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
--rw-r--r--   0        0        0     4894 2023-04-26 19:24:51.134093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
--rw-r--r--   0        0        0     2805 2023-04-26 19:24:51.146093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
--rw-r--r--   0        0        0      159 2023-04-26 19:24:51.198093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
--rw-r--r--   0        0        0    11773 2023-04-26 19:24:51.178093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/query_service_pb2.py
--rw-r--r--   0        0        0     6542 2023-04-26 19:24:51.218093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     4018 2023-04-26 19:24:51.230093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/schema_pb2.py
--rw-r--r--   0        0        0      159 2023-04-26 19:24:51.270093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-04-26 19:24:51.266093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/sources_pb2.py
--rw-r--r--   0        0        0      159 2023-04-26 19:24:51.310093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
--rw-r--r--   0        0        0     2729 2023-04-26 19:24:51.306093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/spec_pb2.py
--rw-r--r--   0        0        0      159 2023-04-26 19:24:51.346093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
--rw-r--r--   0        0        0    11249 2023-04-26 19:24:51.354093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/table_service_pb2.py
--rw-r--r--   0        0        0    10053 2023-04-26 19:24:51.382093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
--rw-r--r--   0        0        0     5157 2023-04-26 19:24:51.394093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
--rw-r--r--   0        0        0      159 2023-04-26 19:24:51.418093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
--rw-r--r--   0        0        0     8140 2023-04-26 19:24:51.422093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/view_service_pb2.py
--rw-r--r--   0        0        0     8153 2023-04-26 19:24:51.458093 kaskada-0.1.6/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
--rw-r--r--   0        0        0    16491 2023-04-26 19:24:51.454093 kaskada-0.1.6/src/kaskada/kaskada/v2alpha/query_service_pb2.py
--rw-r--r--   0        0        0     8377 2023-04-26 19:24:51.486092 kaskada-0.1.6/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     8622 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/materialization.py
--rw-r--r--   0        0        0     9272 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/query.py
--rw-r--r--   0        0        0     2564 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/slice_filters.py
--rw-r--r--   0        0        0    10126 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/table.py
--rw-r--r--   0        0        0     6753 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/utils.py
--rw-r--r--   0        0        0     4543 2023-04-26 19:24:50.174096 kaskada-0.1.6/src/kaskada/view.py
--rw-r--r--   0        0        0    29800 2023-04-26 19:24:50.174096 kaskada-0.1.6/vendor/validate/validate.proto
--rw-r--r--   0        0        0    13089 2023-04-26 19:24:50.174096 kaskada-0.1.6/vendor/validate/validate_pb2.py
--rw-r--r--   0        0        0    22952 2023-04-26 19:24:50.174096 kaskada-0.1.6/vendor/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-26 19:24:50.174096 kaskada-0.1.6/vendor/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 kaskada-0.1.6/setup.py
--rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 kaskada-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1646 2023-05-03 15:20:39.104115 kaskada-0.1.7/README.md
+-rw-r--r--   0        0        0     3882 2023-05-03 15:20:39.108115 kaskada-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     7208 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/fenlmagic/__init__.py
+-rw-r--r--   0        0        0      401 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/fenlmagic/utils.py
+-rw-r--r--   0        0        0       33 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/api/__init__.py
+-rw-r--r--   0        0        0     1179 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/api/api_utils.py
+-rw-r--r--   0        0        0     6381 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/api/release.py
+-rw-r--r--   0        0        0     9507 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/api/session.py
+-rw-r--r--   0        0        0     5838 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/client.py
+-rw-r--r--   0        0        0     1500 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/formatters.css
+-rw-r--r--   0        0        0      984 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/formatters.js
+-rw-r--r--   0        0        0    26206 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/formatters.py
+-rw-r--r--   0        0        0     7337 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/formatters_helpers.py
+-rw-r--r--   0        0        0     9833 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/formatters_shared.py
+-rw-r--r--   0        0        0     7394 2023-05-03 15:20:40.036183 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/common_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-03 15:20:40.036183 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
+-rw-r--r--   0        0        0    10615 2023-05-03 15:20:40.368207 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
+-rw-r--r--   0        0        0     6628 2023-05-03 15:20:40.140190 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4489 2023-05-03 15:20:40.476215 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
+-rw-r--r--   0        0        0     2938 2023-05-03 15:20:40.472214 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4191 2023-05-03 15:20:40.572222 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/destinations_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-03 15:20:40.576222 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
+-rw-r--r--   0        0        0     2668 2023-05-03 15:20:40.680230 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-03 15:20:40.672229 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
+-rw-r--r--   0        0        0     3976 2023-05-03 15:20:40.768236 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/file_service_pb2.py
+-rw-r--r--   0        0        0     5054 2023-05-03 15:20:40.776236 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10837 2023-05-03 15:20:40.864243 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
+-rw-r--r--   0        0        0     9283 2023-05-03 15:20:40.888244 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1897 2023-05-03 15:20:40.964250 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/options_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-03 15:20:41.004253 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
+-rw-r--r--   0        0        0    13180 2023-05-03 15:20:41.064257 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/plan_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-03 15:20:41.104260 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
+-rw-r--r--   0        0        0     3398 2023-05-03 15:20:41.176266 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
+-rw-r--r--   0        0        0     4894 2023-05-03 15:20:41.204268 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2805 2023-05-03 15:20:41.280273 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-03 15:20:41.300274 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
+-rw-r--r--   0        0        0    11773 2023-05-03 15:20:41.616297 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     6542 2023-05-03 15:20:41.420283 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4018 2023-05-03 15:20:41.740306 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/schema_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-03 15:20:41.712304 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-03 15:20:42.052329 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/sources_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-03 15:20:41.836313 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
+-rw-r--r--   0        0        0     2729 2023-05-03 15:20:41.936321 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/spec_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-03 15:20:42.268345 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
+-rw-r--r--   0        0        0    11249 2023-05-03 15:20:42.148336 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/table_service_pb2.py
+-rw-r--r--   0        0        0    10053 2023-05-03 15:20:42.240343 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5157 2023-05-03 15:20:42.388353 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-03 15:20:42.572367 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
+-rw-r--r--   0        0        0     8140 2023-05-03 15:20:42.548365 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/view_service_pb2.py
+-rw-r--r--   0        0        0     8153 2023-05-03 15:20:42.648373 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
+-rw-r--r--   0        0        0    16491 2023-05-03 15:20:42.672374 kaskada-0.1.7/src/kaskada/kaskada/v2alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     8377 2023-05-03 15:20:42.748380 kaskada-0.1.7/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8622 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/materialization.py
+-rw-r--r--   0        0        0     9272 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/query.py
+-rw-r--r--   0        0        0     2564 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/slice_filters.py
+-rw-r--r--   0        0        0    10126 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/table.py
+-rw-r--r--   0        0        0     7131 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/utils.py
+-rw-r--r--   0        0        0     4543 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/view.py
+-rw-r--r--   0        0        0    29800 2023-05-03 15:20:39.108115 kaskada-0.1.7/vendor/validate/validate.proto
+-rw-r--r--   0        0        0    13089 2023-05-03 15:20:39.108115 kaskada-0.1.7/vendor/validate/validate_pb2.py
+-rw-r--r--   0        0        0    22952 2023-05-03 15:20:39.108115 kaskada-0.1.7/vendor/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:20:39.108115 kaskada-0.1.7/vendor/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 kaskada-0.1.7/setup.py
+-rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 kaskada-0.1.7/PKG-INFO
```

### Comparing `kaskada-0.1.6/README.md` & `kaskada-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/pyproject.toml` & `kaskada-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaskada"
-version = "0.1.6"
+version = "0.1.7"
 description = "A client library for the Kaskada time travel machine learning service"
 authors = ["Kaskada <maintainers@kaskada.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "kaskada", from = "src" },
     { include = "validate", from = "vendor" },
```

### Comparing `kaskada-0.1.6/src/fenlmagic/__init__.py` & `kaskada-0.1.7/src/fenlmagic/__init__.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/api/api_utils.py` & `kaskada-0.1.7/src/kaskada/api/api_utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/api/release.py` & `kaskada-0.1.7/src/kaskada/api/release.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/api/session.py` & `kaskada-0.1.7/src/kaskada/api/session.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/client.py` & `kaskada-0.1.7/src/kaskada/client.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/formatters.css` & `kaskada-0.1.7/src/kaskada/formatters.css`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/formatters.js` & `kaskada-0.1.7/src/kaskada/formatters.js`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/formatters.py` & `kaskada-0.1.7/src/kaskada/formatters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/formatters_helpers.py` & `kaskada-0.1.7/src/kaskada/formatters_helpers.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/formatters_shared.py` & `kaskada-0.1.7/src/kaskada/formatters_shared.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/common_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/common_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/compute_service_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/compute_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/destinations_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/destinations_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/file_service_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/file_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/options_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/options_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/plan_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/plan_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/pulsar_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/pulsar_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/query_service_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/schema_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/sources_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/sources_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/spec_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/table_service_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/table_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/test_cases_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/test_cases_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/view_service_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/view_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py` & `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v2alpha/query_service_pb2.py` & `kaskada-0.1.7/src/kaskada/kaskada/v2alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py` & `kaskada-0.1.7/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/materialization.py` & `kaskada-0.1.7/src/kaskada/materialization.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/query.py` & `kaskada-0.1.7/src/kaskada/query.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/slice_filters.py` & `kaskada-0.1.7/src/kaskada/slice_filters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/table.py` & `kaskada-0.1.7/src/kaskada/table.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/src/kaskada/utils.py` & `kaskada-0.1.7/src/kaskada/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,22 +98,26 @@
     errorMessage += "\tError Message: {}\n".format(rpc_error.details())
     raise Exception(errorMessage) from None
 
 
 def to_uri(file: str) -> str:
     # Remote file stores are prefixed appropriately.
     if (
-        file.startswith("s3://")
-        or file.startswith("gs://")
-        or file.startswith("https://")
+        file.startswith("s3://")  # Amazon Web Services S3 file path provided
+        or file.startswith("gs://")  # Google Cloud Platform GS file path provided
+        or file.startswith("https://")  # HTTPS file path
+        or file.startswith("file:///")  # Absolute file path is provided
     ):
         return file
-    # TODO: Verify that the object actually exists locally
-    path = Path(file).absolute()
-    return f"file://{path}"
+    elif file.startswith("file://"):  # Convert local path to full path
+        file_suffix_path = file[7:]  # The length of file://
+        return f"file://{Path(file_suffix_path).absolute()}"
+    else:  # A non-prefixed file path was provided
+        path = Path(file).absolute()
+        return f"file://{path}"
 
 
 def unpack_details(grpc_detail):
     """Unpack a grpc status detail field (which is a 'google.protobuf.Any' type).
     `Unpack()` checks the descriptor of the passed-in message object against the stored one
     and returns False if they don't match and does not attempt any unpacking; True otherwise.
```

### Comparing `kaskada-0.1.6/src/kaskada/view.py` & `kaskada-0.1.7/src/kaskada/view.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/vendor/validate/validate.proto` & `kaskada-0.1.7/vendor/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/vendor/validate/validate_pb2.py` & `kaskada-0.1.7/vendor/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/vendor/validate/validate_pb2.pyi` & `kaskada-0.1.7/vendor/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.6/setup.py` & `kaskada-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'pyarrow>=10.0.1,<11.0.0',
  'pygithub>=1.57,<2.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'kaskada',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'A client library for the Kaskada time travel machine learning service',
     'long_description': '# Kaskada SDK\n\n## Developer Instructions\nThe package uses Poetry to develop and build.\n\n1. Install Pyenv [Pyenv Documentation](https://github.com/pyenv/pyenv)\n1. Install Python 3.9.16: `$ pyenv install 3.9.16`\n1. Install Poetry [Poetry Documentation](https://python-poetry.org/docs/)\n1. Install dependences: `$ poetry install`\n\n### Run tasks\nThe package uses [`poethepoet`](https://github.com/nat-n/poethepoet) for running tasks\n\n#### Test Task\nTo run tests: `$ poetry run poe test` \n\n#### Check Style Task\nTo check the style: `$ poetry run poe style`\n\n#### Format Task\nTo auto-format (isort + black): `$ poetry run poe format`\n\n#### Check Static Type Task\nTo perform static type analysis (mypy): `$ poetry run poe types`\n\n#### Lint Task\nTo run the linter (pylint): `$ poetry run poe lint`\n\n#### Generate documentation \nWe use Sphinx and rely on autogeneration extensions within Sphinx to read docstrings and \ngenerate an HTML formatted version of the codes documentation. \n\n* `poetry run poe docs` : generates and builds the docs \n* `poetry run poe docs-generate` : generates the docs (.rst files)\n* `poetry run poe docs-build` : builds the HTML rendered version of the generated docs (from .rst to .html)\n\nThe generated HTML is located inside `docs/build`. Load `docs/build/index.html` in your browser to see the HTML rendered output. \n\n## Using the Client from Jupyter\n\n#### Install Jupyter\nTo install Jupyter: `$ pip install notebook`\n\n#### Build the Client\nTo build the client: `$ poetry build`\n\n#### Install the Client\nTo install the client: `$ pip install dist/*.whl`\n\n#### Open a Jupyter Notebook\nTo open a notebook: `$ jupyter notebook`\n',
     'author': 'Kaskada',
     'author_email': 'maintainers@kaskada.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kaskada-0.1.6/PKG-INFO` & `kaskada-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaskada
-Version: 0.1.6
+Version: 0.1.7
 Summary: A client library for the Kaskada time travel machine learning service
 License: Apache-2.0
 Author: Kaskada
 Author-email: maintainers@kaskada.io
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

