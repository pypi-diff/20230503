# Comparing `tmp/frequenz-api-microgrid-0.11.0.tar.gz` & `tmp/frequenz-api-microgrid-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-api-microgrid-0.11.0.tar", last modified: Tue Sep  6 09:01:42 2022, max compression
+gzip compressed data, was "frequenz-api-microgrid-0.12.0.tar", last modified: Wed May  3 06:43:40 2023, max compression
```

## Comparing `frequenz-api-microgrid-0.11.0.tar` & `frequenz-api-microgrid-0.12.0.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.149932 frequenz-api-microgrid-0.11.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-09-06 09:01:42.149932 frequenz-api-microgrid-0.11.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/minimum-requirements-ci.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.137931 frequenz-api-microgrid-0.11.0/proto/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.137931 frequenz-api-microgrid-0.11.0/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.137931 frequenz-api-microgrid-0.11.0/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.141931 frequenz-api-microgrid-0.11.0/proto/frequenz/api/microgrid/
--rw-r--r--   0 runner    (1001) docker     (121)     4822 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/proto/frequenz/api/microgrid/battery.proto
--rw-r--r--   0 runner    (1001) docker     (121)     7724 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/proto/frequenz/api/microgrid/common.proto
--rw-r--r--   0 runner    (1001) docker     (121)     5324 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/proto/frequenz/api/microgrid/ev_charger.proto
--rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/proto/frequenz/api/microgrid/inverter.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/proto/frequenz/api/microgrid/meter.proto
--rw-r--r--   0 runner    (1001) docker     (121)    12881 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/proto/frequenz/api/microgrid/microgrid.proto
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/proto/frequenz/api/microgrid/sensor.proto
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.137931 frequenz-api-microgrid-0.11.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.137931 frequenz-api-microgrid-0.11.0/py/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.137931 frequenz-api-microgrid-0.11.0/py/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.141931 frequenz-api-microgrid-0.11.0/py/frequenz/api/microgrid/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/py/frequenz/api/microgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/py/frequenz/api/microgrid/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.141931 frequenz-api-microgrid-0.11.0/py/frequenz_api_microgrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-09-06 09:01:42.000000 frequenz-api-microgrid-0.11.0/py/frequenz_api_microgrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3877 2022-09-06 09:01:42.000000 frequenz-api-microgrid-0.11.0/py/frequenz_api_microgrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 09:01:42.000000 frequenz-api-microgrid-0.11.0/py/frequenz_api_microgrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-06 09:01:42.000000 frequenz-api-microgrid-0.11.0/py/frequenz_api_microgrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-06 09:01:42.000000 frequenz-api-microgrid-0.11.0/py/frequenz_api_microgrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 09:01:42.149932 frequenz-api-microgrid-0.11.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2160 2022-09-06 09:01:28.000000 frequenz-api-microgrid-0.11.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.137931 frequenz-api-microgrid-0.11.0/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.137931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.137931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.145931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (121)     7374 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (121)     2504 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (121)     3392 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (121)     3169 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (121)     8657 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (121)     6132 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (121)     2824 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (121)    12099 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (121)     2605 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (121)     2910 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (121)     2045 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (121)     3209 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (121)     6628 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (121)     5512 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (121)     3524 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (121)    10854 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (121)    11347 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (121)    14929 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (121)     6099 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (121)     3472 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.145931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)     6308 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.137931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.137931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.145931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (121)    41483 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.145931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (121)     5482 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.145931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (121)     8659 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.137931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.145931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (121)     3389 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.145931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (121)    10515 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.145931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (121)     7125 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.145931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (121)    12015 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (121)     9504 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 09:01:42.145931 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (121)     6193 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1933 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (121)     3508 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (121)     6239 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (121)     3795 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-09-06 09:01:29.000000 frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.878233 frequenz-api-microgrid-0.12.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-05-03 06:43:40.878233 frequenz-api-microgrid-0.12.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/minimum-requirements-ci.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.862233 frequenz-api-microgrid-0.12.0/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.862233 frequenz-api-microgrid-0.12.0/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.862233 frequenz-api-microgrid-0.12.0/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.870233 frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/battery.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    13408 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/common.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     5424 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/ev_charger.proto
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/grid.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/inverter.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/meter.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    17827 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/microgrid.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2913 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/sensor.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.862233 frequenz-api-microgrid-0.12.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.862233 frequenz-api-microgrid-0.12.0/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.862233 frequenz-api-microgrid-0.12.0/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.870233 frequenz-api-microgrid-0.12.0/py/frequenz/api/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/py/frequenz/api/microgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/py/frequenz/api/microgrid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.870233 frequenz-api-microgrid-0.12.0/py/frequenz_api_microgrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-05-03 06:43:40.000000 frequenz-api-microgrid-0.12.0/py/frequenz_api_microgrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3917 2023-05-03 06:43:40.000000 frequenz-api-microgrid-0.12.0/py/frequenz_api_microgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 06:43:40.000000 frequenz-api-microgrid-0.12.0/py/frequenz_api_microgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-05-03 06:43:40.000000 frequenz-api-microgrid-0.12.0/py/frequenz_api_microgrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-03 06:43:40.000000 frequenz-api-microgrid-0.12.0/py/frequenz_api_microgrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1670 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-03 06:43:40.878233 frequenz-api-microgrid-0.12.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.862233 frequenz-api-microgrid-0.12.0/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.862233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.866233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.874233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/backend.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/billing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/client.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/config_change.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/consumer.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/control.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/distribution.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/documentation.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/endpoint.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/field_behavior.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/httpbody.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/label.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/launch_stage.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/log.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/logging.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/metric.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/monitored_resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/monitoring.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/quota.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/routing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/service.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/source_info.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/system_parameter.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/usage.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.874233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/cloud/extended_operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.866233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.866233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.874233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.874233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.874233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/v1/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/v1/options.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/v1/policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.866233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/logging/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.874233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/logging/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/logging/type/http_request.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/logging/type/log_severity.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.878233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/longrunning/
+-rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/longrunning/operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.878233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/rpc/code.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.878233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/rpc/context/
+-rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/rpc/error_details.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/rpc/status.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 06:43:40.878233 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/calendar_period.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/color.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/date.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/datetime.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/dayofweek.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/expr.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/fraction.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/latlng.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/money.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/month.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/postal_address.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/quaternion.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-05-03 06:43:26.000000 frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/timeofday.proto
```

### Comparing `frequenz-api-microgrid-0.11.0/CONTRIBUTING.md` & `frequenz-api-microgrid-0.12.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/LICENSE` & `frequenz-api-microgrid-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/PKG-INFO` & `frequenz-api-microgrid-0.12.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-microgrid
-Version: 0.11.0
+Version: 0.12.0
 Summary: Frequenz gRPC API for monitoring and control of microgrids
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-microgrid/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-microgrid
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-microgrid/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-microgrid/discussions/categories/support
@@ -34,8 +34,8 @@
 
 
 Contributing
 ============
 
 If you want to know how to build this project and contribute to it, please
 check out the [Contributing
-Guide](https://github.com/frequenz-floss/frequenz-api-microgrid/CONTRIBUTING.md).
+Guide](https://github.com/frequenz-floss/frequenz-api-microgrid/blob/v0.x.x/CONTRIBUTING.md).
```

### Comparing `frequenz-api-microgrid-0.11.0/proto/frequenz/api/microgrid/battery.proto` & `frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/battery.proto`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,20 @@
   // Lithium-Iron-Phosphate batteries.
   TYPE_LI_FE_PO = 2;
 
   // Sodium-ion batteries
   TYPE_NA_ION = 3;
 }
 
+// The battery metadata.
+message Metadata {
+  // The battery type.
+  Type type = 1;
+}
+
 enum ComponentState {
   // Default value.
   COMPONENT_STATE_UNSPECIFIED = 0;
 
   // The battery is switched off.
   COMPONENT_STATE_OFF = 1;
 
@@ -172,28 +178,29 @@
   common.DC dc = 1;
 
   // Battery's overall SoC.
   // In percent (%).
   common.MetricAggregation soc = 2;
 
   // The aggregated values of all the temperature measurements of a battery.
-  // In Celsius (°C).
+  // In degree Celsius (°C).
   common.MetricAggregation temperature = 3;
 
   // The aggregated values of all the humidity measurements of a battery.
-  // In %.
+  // In percent (%).
   common.MetricAggregation humidity = 4;
 }
 
 // Battery properties.
 message Properties {
   // The firmware version of the battery.
   string firmware_ver = 1;
 
   // The capacity of the battery.
+  // In Watt-hour (Wh).
   float capacity = 2;
 }
 
 // Battery/BMS details
 message Battery {
   // The component properties
   Properties properties = 1;
```

### Comparing `frequenz-api-microgrid-0.11.0/proto/frequenz/api/microgrid/ev_charger.proto` & `frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/ev_charger.proto`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,20 @@
   // The EV charging station supports DC charging only.
   TYPE_DC = 2;
 
   // The EV charging station supports both AC and DC.
   TYPE_HYBRID = 3;
 }
 
+// The EV charger metadata.
+message Metadata {
+  // The EV charger type.
+  Type type = 1;
+}
+
 // The possible states of an EV charging station.
 enum ComponentState {
   // Default state.
   COMPONENT_STATE_UNSPECIFIED = 0;
 
   // The EV charging station is starting up.
   COMPONENT_STATE_STARTING = 1;
@@ -173,15 +179,15 @@
   // AC metrics of the EV charging station.
   // Contains data only if AC charging is supported by the EV charging station.
   // (in which case, the type of the EV charging station is TYPE_AC or
   // TYPE_HYBRID)
   common.AC ac = 2;
 
   // The overall temperature of the EV charger.
-  // In Celsius (°C).
+  // In degree Celsius (°C).
   common.Metric temperature = 3;
 }
 
 // EV charger properties.
 message Properties {
   // The firmware version of the component.
   string firmware_ver = 1;
```

### Comparing `frequenz-api-microgrid-0.11.0/proto/frequenz/api/microgrid/inverter.proto` & `frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/inverter.proto`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,20 @@
 enum Type {
   TYPE_UNSPECIFIED = 0;
   TYPE_BATTERY = 1;
   TYPE_SOLAR = 2;
   TYPE_HYBRID = 3;
 }
 
+// The inverter metadata.
+message Metadata {
+  // The inverter type.
+  Type type = 1;
+}
+
 // Enumerated inverter states.
 enum ComponentState {
   // Default value.
   COMPONENT_STATE_UNSPECIFIED = 0;
 
   // Inverter is switched off.
   COMPONENT_STATE_OFF = 1;
@@ -87,15 +93,15 @@
   // DC metrics of the inverter.
   common.DC dc = 1;
 
   // AC metrics of the inverter.
   common.AC ac = 2;
 
   // The verall temperature of the inverter.
-  // In Celsius (°C).
+  // In degree Celsius (°C).
   common.Metric temperature = 3;
 }
 
 // Inverter properties.
 message Properties {
   // The firmware version of the component.
   string firmware_ver = 1;
```

### Comparing `frequenz-api-microgrid-0.11.0/proto/frequenz/api/microgrid/meter.proto` & `frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/meter.proto`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,20 @@
   // Exported to grid meter
   TYPE_FEED_IN = 3;
 
   // Imported power from grid meter
   TYPE_PURCHASED = 4;
 }
 
+// The meter metadata.
+message Metadata {
+  // The meter type.
+  Type type = 1;
+}
+
 // Enumerated meter states.
 enum ComponentState {
   // Unspecified state.
   COMPONENT_STATE_UNSPECIFIED = 0;
 
   // The meter is behaving as expected.
   COMPONENT_STATE_OK = 1;
```

### Comparing `frequenz-api-microgrid-0.11.0/proto/frequenz/api/microgrid/sensor.proto` & `frequenz-api-microgrid-0.12.0/proto/frequenz/api/microgrid/sensor.proto`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,20 @@
   // Anemometer (wind velocity and direction sensor).
   TYPE_ANEMOMETER = 5;
 
   // Accelerometers (acceleration sensor).
   TYPE_ACCELEROMETER = 6;
 }
 
+// The sensor metadata.
+message Metadata {
+  // The sensor type.
+  Type type = 1;
+}
+
 // Enumerated sensor states.
 enum ComponentState {
   // Unspecified state.
   COMPONENT_STATE_UNSPECIFIED = 0;
 
   // The sensor is behaving as expected.
   COMPONENT_STATE_OK = 1;
```

### Comparing `frequenz-api-microgrid-0.11.0/py/frequenz_api_microgrid.egg-info/PKG-INFO` & `frequenz-api-microgrid-0.12.0/py/frequenz_api_microgrid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-microgrid
-Version: 0.11.0
+Version: 0.12.0
 Summary: Frequenz gRPC API for monitoring and control of microgrids
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-microgrid/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-microgrid
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-microgrid/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-microgrid/discussions/categories/support
@@ -34,8 +34,8 @@
 
 
 Contributing
 ============
 
 If you want to know how to build this project and contribute to it, please
 check out the [Contributing
-Guide](https://github.com/frequenz-floss/frequenz-api-microgrid/CONTRIBUTING.md).
+Guide](https://github.com/frequenz-floss/frequenz-api-microgrid/blob/v0.x.x/CONTRIBUTING.md).
```

### Comparing `frequenz-api-microgrid-0.11.0/py/frequenz_api_microgrid.egg-info/SOURCES.txt` & `frequenz-api-microgrid-0.12.0/py/frequenz_api_microgrid.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 RELEASE_NOTES.md
 minimum-requirements-ci.txt
 pyproject.toml
 setup.py
 proto/frequenz/api/microgrid/battery.proto
 proto/frequenz/api/microgrid/common.proto
 proto/frequenz/api/microgrid/ev_charger.proto
+proto/frequenz/api/microgrid/grid.proto
 proto/frequenz/api/microgrid/inverter.proto
 proto/frequenz/api/microgrid/meter.proto
 proto/frequenz/api/microgrid/microgrid.proto
 proto/frequenz/api/microgrid/sensor.proto
 py/frequenz/api/microgrid/__init__.py
 py/frequenz/api/microgrid/py.typed
 py/frequenz_api_microgrid.egg-info/PKG-INFO
```

### Comparing `frequenz-api-microgrid-0.11.0/pyproject.toml` & `frequenz-api-microgrid-0.12.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
     "grpcio-tools >= 1.47.0, < 2",
     "mypy-protobuf >= 3.0.0, < 4",
-    "setuptools >= 63.1.0, < 64",
+    "setuptools >= 65.4.1, < 66",
     "setuptools_scm[toml] >= 7.0.5, < 8",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-api-microgrid"
@@ -45,12 +45,9 @@
 
 [tool.setuptools.package-dir]
 "" = "py"
 
 [tool.setuptools.package-data]
 "frequenz.api.microgrid" = [ "py.typed", "*.pyi" ]
 
-[tools.setuptools.packages.find_namespace]
-where = "py"
-
 [tool.setuptools_scm]
 version_scheme = "post-release"
```

### Comparing `frequenz-api-microgrid-0.11.0/setup.py` & `frequenz-api-microgrid-0.12.0/setup.py`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/annotations.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/auth.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/auth.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/backend.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/backend.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/billing.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/billing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/client.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/config_change.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/config_change.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/consumer.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/consumer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/context.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/control.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/control.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/distribution.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/distribution.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/documentation.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/documentation.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/endpoint.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/endpoint.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/field_behavior.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/http.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/httpbody.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/label.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/label.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/launch_stage.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/launch_stage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/log.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/log.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/logging.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/logging.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/metric.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/metric.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/monitored_resource.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/monitored_resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/monitoring.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/monitoring.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/quota.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/quota.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/resource.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/routing.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/service.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/service.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/source_info.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/source_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/system_parameter.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/system_parameter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/api/usage.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/api/usage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/cloud/extended_operations.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/v1/options.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/v1/options.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/iam/v1/policy.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/iam/v1/policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/logging/type/http_request.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/logging/type/http_request.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/logging/type/log_severity.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/logging/type/log_severity.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/longrunning/operations.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/rpc/code.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/rpc/error_details.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/rpc/status.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/calendar_period.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/calendar_period.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/color.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/color.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/date.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/date.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/datetime.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/datetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/dayofweek.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/expr.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/expr.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/fraction.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/fraction.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/latlng.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/latlng.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/money.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/money.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/month.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/month.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/postal_address.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/postal_address.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/quaternion.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/quaternion.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.11.0/submodules/api-common-protos/google/type/timeofday.proto` & `frequenz-api-microgrid-0.12.0/submodules/api-common-protos/google/type/timeofday.proto`

 * *Files identical despite different names*

