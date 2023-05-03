# Comparing `tmp/gantry-0.6.0.tar.gz` & `tmp/gantry-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gantry-0.6.0.tar", last modified: Wed May  3 21:08:52 2023, max compression
+gzip compressed data, was "gantry-0.6.0a0.tar", last modified: Fri Apr 28 20:06:25 2023, max compression
```

## Comparing `gantry-0.6.0.tar` & `gantry-0.6.0a0.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.152351 gantry-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-03 21:08:42.000000 gantry-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 21:08:42.000000 gantry-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 21:08:52.152351 gantry-0.6.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.136351 gantry-0.6.0/gantry/
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.140351 gantry-0.6.0/gantry/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/alerts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/alerts/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/alerts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.140351 gantry-0.6.0/gantry/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/applications/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19486 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/applications/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/applications/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.140351 gantry-0.6.0/gantry/automations/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/automations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/automations/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/automations/automations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.140351 gantry-0.6.0/gantry/automations/curators/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/automations/curators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/automations/curators/curators.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/automations/curators/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/automations/curators/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/automations/curators/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/automations/curators/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26177 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/automations/curators/stock_curators.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/automations/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/automations/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/automations/triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.140351 gantry-0.6.0/gantry/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/cli/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/cli/data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/cli/labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/cli/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/cli/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.140351 gantry-0.6.0/gantry/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/data_generator/data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.144351 gantry-0.6.0/gantry/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/dataset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/dataset/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    64417 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/dataset/gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/dataset/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.144351 gantry-0.6.0/gantry/dataset/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/dataset/templates/load_script_template.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.144351 gantry-0.6.0/gantry/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93705 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/logger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/logger/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/logger/event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/logger/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/logger/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/logger/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/logger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.144351 gantry-0.6.0/gantry/query/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.144351 gantry-0.6.0/gantry/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/core/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/core/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/core/queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.144351 gantry-0.6.0/gantry/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/distance/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.144351 gantry-0.6.0/gantry/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/metric/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/query/time_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 21:08:42.000000 gantry-0.6.0/gantry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.140351 gantry-0.6.0/gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 21:08:52.000000 gantry-0.6.0/gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-03 21:08:52.000000 gantry-0.6.0/gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:08:52.000000 gantry-0.6.0/gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-03 21:08:52.000000 gantry-0.6.0/gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-03 21:08:52.000000 gantry-0.6.0/gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 21:08:52.000000 gantry-0.6.0/gantry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:08:52.152351 gantry-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-03 21:08:42.000000 gantry-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.144351 gantry-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.148351 gantry-0.6.0/tests/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/alerts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/alerts/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/alerts/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.148351 gantry-0.6.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/cli/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/cli/test_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/cli/test_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/cli/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/cli/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.148351 gantry-0.6.0/tests/curator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/curator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/curator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/curator/test_curator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/curator/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/curator/test_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.148351 gantry-0.6.0/tests/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/data_generator/test_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.148351 gantry-0.6.0/tests/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/dataset/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/dataset/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/dataset/test_gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/dataset/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.148351 gantry-0.6.0/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/logger/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   136361 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/logger/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/logger/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/logger/test_event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/logger/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/logger/test_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/logger/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.148351 gantry-0.6.0/tests/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.152351 gantry-0.6.0/tests/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/core/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/core/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/core/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/core/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/core/test_queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    35405 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/core/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.152351 gantry-0.6.0/tests/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/distance/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:52.152351 gantry-0.6.0/tests/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/metric/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/query/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-03 21:08:42.000000 gantry-0.6.0/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.501926 gantry-0.6.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-04-28 20:06:13.000000 gantry-0.6.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-28 20:06:13.000000 gantry-0.6.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-28 20:06:25.501926 gantry-0.6.0a0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.461925 gantry-0.6.0a0/gantry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.465925 gantry-0.6.0a0/gantry/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/alerts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/alerts/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/alerts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.465925 gantry-0.6.0a0/gantry/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/applications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19192 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/applications/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/applications/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.469925 gantry-0.6.0a0/gantry/automations/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/automations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.469925 gantry-0.6.0a0/gantry/automations/curators/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26177 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/curators/stock_curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/automations/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.473925 gantry-0.6.0a0/gantry/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/cli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.473925 gantry-0.6.0a0/gantry/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/data_generator/data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.477926 gantry-0.6.0a0/gantry/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/dataset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/dataset/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64417 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/dataset/gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/dataset/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.477926 gantry-0.6.0a0/gantry/dataset/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/dataset/templates/load_script_template.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.481926 gantry-0.6.0a0/gantry/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93859 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/logger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.481926 gantry-0.6.0a0/gantry/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.485926 gantry-0.6.0a0/gantry/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.485926 gantry-0.6.0a0/gantry/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/distance/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.485926 gantry-0.6.0a0/gantry/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/metric/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/query/time_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 20:06:13.000000 gantry-0.6.0a0/gantry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.465925 gantry-0.6.0a0/gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-28 20:06:25.000000 gantry-0.6.0a0/gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-28 20:06:25.000000 gantry-0.6.0a0/gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:06:25.000000 gantry-0.6.0a0/gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 20:06:25.000000 gantry-0.6.0a0/gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-28 20:06:25.000000 gantry-0.6.0a0/gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 20:06:25.000000 gantry-0.6.0a0/gantry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 20:06:25.501926 gantry-0.6.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-28 20:06:13.000000 gantry-0.6.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.485926 gantry-0.6.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.489926 gantry-0.6.0a0/tests/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/alerts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/alerts/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/alerts/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.489926 gantry-0.6.0a0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14545 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/test_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/test_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/cli/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.489926 gantry-0.6.0a0/tests/curator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/curator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/curator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/curator/test_curator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/curator/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/curator/test_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.493926 gantry-0.6.0a0/tests/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/data_generator/test_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.493926 gantry-0.6.0a0/tests/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/dataset/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/dataset/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/dataset/test_gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/dataset/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.497926 gantry-0.6.0a0/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72641 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/test_event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/test_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/logger/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.497926 gantry-0.6.0a0/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.497926 gantry-0.6.0a0/tests/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35405 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.501926 gantry-0.6.0a0/tests/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/distance/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:25.501926 gantry-0.6.0a0/tests/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/metric/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/query/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-28 20:06:13.000000 gantry-0.6.0a0/tests/test_validator.py
```

### Comparing `gantry-0.6.0/LICENSE` & `gantry-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/PKG-INFO` & `gantry-0.6.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.0
+Version: 0.6.0a0
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.0/gantry/__init__.py` & `gantry-0.6.0a0/gantry/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/alerts/client.py` & `gantry-0.6.0a0/gantry/alerts/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/alerts/globals.py` & `gantry-0.6.0a0/gantry/alerts/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/alerts/main.py` & `gantry-0.6.0a0/gantry/alerts/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/api_client.py` & `gantry-0.6.0a0/gantry/api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/applications/client.py` & `gantry-0.6.0a0/gantry/applications/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 import logging
-from typing import Optional
 
 from typeguard import typechecked
 
 from gantry.api_client import APIClient
 from gantry.applications.core import Application
 
 logger = logging.getLogger(__name__)
 
 
 class ApplicationClient:
     def __init__(self, api_client: APIClient) -> None:
         self._api_client = api_client
 
     @typechecked
-    def create_application(
-        self, application_name: str, application_type: Optional[str] = None
-    ) -> Application:
+    def create_application(self, application_name: str) -> Application:
         """
         Create an empty application.
         """
         data = {
             "model_name": application_name,
         }
-        if application_type:
-            data["model_type"] = application_type
 
         res = self._api_client.request(
             "POST",
             "/api/v1/applications",
             json=data,
             raise_for_status=True,
         )
```

### Comparing `gantry-0.6.0/gantry/applications/core.py` & `gantry-0.6.0a0/gantry/applications/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         api_client: APIClient,
         id: Optional[uuid.UUID] = None,
         organization_id: Optional[uuid.UUID] = None,
     ):
         self._api_client = api_client
         if self._api_client is None:
             raise ClientNotInitialized()
-        self._id = id or uuid.uuid4()
+        self._id = id
         self._name = name
         self._organization_id = organization_id
         self._version = 1
 
     def log_file(
         self,
         filepath: str,
@@ -252,15 +252,15 @@
         self,
         inputs: Optional[Union[dict, List[dict], pd.DataFrame, pd.Series, np.ndarray]] = None,
         outputs: Optional[
             Union[Any, List[Any], dict, List[dict], pd.DataFrame, pd.Series, np.ndarray]
         ] = None,
         feedbacks: Optional[Union[dict, List[dict], pd.DataFrame, pd.Series, np.ndarray]] = None,
         tags: Optional[Union[Dict[str, str], List[Dict[str, str]]]] = None,
-        timestamps: Optional[
+        timestamp: Optional[
             Union[datetime.datetime, List[datetime.datetime], pd.DatetimeIndex, np.ndarray]
         ] = None,
         sort_on_timestamp: bool = True,
         sample_rate: float = 1.0,
         row_tags: Optional[
             Union[Dict[str, str], List[Dict[str, str]], pd.DataFrame, pd.Series, np.ndarray]
         ] = None,
@@ -276,15 +276,15 @@
             run_tags = Run._current_instance.tags
         return log(
             application=self._name,
             inputs=inputs,
             outputs=outputs,
             feedbacks=feedbacks,
             tags=tags,
-            timestamps=timestamps,
+            timestamp=timestamp,
             sort_on_timestamp=sort_on_timestamp,
             sample_rate=sample_rate,
             row_tags=row_tags,
             global_tags=global_tags,
             join_keys=join_keys,
             as_batch=as_batch,
             run_id=run_id,
@@ -354,20 +354,16 @@
             )
             data["model_node_id"] = model_node_id
         except GantryRequestException:
             raise ValueError(
                 f"Application {self._name}[{query.version if query.version else 'latest'}]"
                 + "does not exist."
             )
-        if name in [query["name"] for query in self.list_queries()]:
-            self._api_client.request("PATCH", "/api/v1/queries", json=data, raise_for_status=True)
-            logger.info("Query updated successfully.")
-        else:
-            self._api_client.request("POST", "/api/v1/queries", json=data, raise_for_status=True)
-            logger.info("Query saved successfully.")
+        self._api_client.request("POST", "/api/v1/queries", json=data, raise_for_status=True)
+        logger.info("Query saved successfully.")
 
     def get_query(self, name: str) -> GantryDataFrame:
         """
         Get a saved query from the Gantry database.
         Args:
             name: The name of the query.
         Returns:
@@ -412,17 +408,17 @@
         Returns:
             A Run object.
         """
         return Run(self, name=name, tags=tags)
 
     def get_run(self, name: Optional[str] = None, tags: Optional[dict] = None):
         """
-        Get a run in this application, filtered by tags or name.
+        Get runs for this application, filtered by tags or name.
         Returns:
-            A job object associated with the requested run.
+            A list of Run objects.
         """
         if name:
             response = self._api_client.request(
                 "GET",
                 f"/api/v1/applications/{self._id}/jobs",
                 params={"run_name": name},
                 raise_for_status=True,
@@ -495,15 +491,15 @@
     def create_dataset(self, name: str, bucket_name: Optional[str] = None) -> List[Dict[str, Any]]:
         """
         Create a dataset for this application.
         Args:
             name: The name of the dataset.
             bucket_name: The bucket name of the dataset.
         """
-        return dataset.create_dataset(name=name, bucket_name=bucket_name, app_name=self._name)
+        return dataset.create_dataset(name, bucket_name=bucket_name, app_name=self._name)
 
     def list_datasets(self, include_deleted: bool = False):
         """
         List all datasets for this application.
         Returns:
             A list of datasets.
         """
```

### Comparing `gantry-0.6.0/gantry/applications/main.py` & `gantry-0.6.0a0/gantry/applications/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/automations/actions.py` & `gantry-0.6.0a0/gantry/automations/actions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/automations/automations.py` & `gantry-0.6.0a0/gantry/automations/automations.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/automations/curators/__init__.py` & `gantry-0.6.0a0/gantry/automations/curators/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/automations/curators/curators.py` & `gantry-0.6.0a0/gantry/automations/curators/curators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/automations/curators/main.py` & `gantry-0.6.0a0/gantry/automations/curators/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/automations/curators/models.py` & `gantry-0.6.0a0/gantry/automations/curators/models.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/automations/curators/selectors.py` & `gantry-0.6.0a0/gantry/automations/curators/selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/automations/curators/stock_curators.py` & `gantry-0.6.0a0/gantry/automations/curators/stock_curators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/automations/main.py` & `gantry-0.6.0a0/gantry/automations/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/automations/triggers.py` & `gantry-0.6.0a0/gantry/automations/triggers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/cli/application.py` & `gantry-0.6.0a0/gantry/cli/application.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/cli/bucket.py` & `gantry-0.6.0a0/gantry/cli/bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/cli/data_connector.py` & `gantry-0.6.0a0/gantry/cli/data_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,16 +151,16 @@
     resp = api_client.request(
         "GET",
         f"/api/v1/data-connectors/pipelines?app_name={app_name}&enabled_status={enabled_status}",
         raise_for_status=True,
     )
 
     click.secho(
-        f"--> The following pipelines are given for \"{app_name}\" app with status \"{status}\":\n\
-{json.dumps(resp['data'], indent=4)}"
+        f"--> The following pipelines are given for {app_name} and {status} : )\n \
+            {json.dumps(resp['data'], indent=4)}"
     )
 
 
 @data_connector.command(
     aliases=["list_pipeline_operations"],
     help="Lists pipeline operations for a given pipeline name, appname, and status.",
 )
```

### Comparing `gantry-0.6.0/gantry/cli/labeling.py` & `gantry-0.6.0a0/gantry/cli/labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/cli/main.py` & `gantry-0.6.0a0/gantry/cli/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/cli/projection.py` & `gantry-0.6.0a0/gantry/cli/projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/cli/secret.py` & `gantry-0.6.0a0/gantry/cli/secret.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/data_generator/data_generator.py` & `gantry-0.6.0a0/gantry/data_generator/data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/dataset/client.py` & `gantry-0.6.0a0/gantry/dataset/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/dataset/constants.py` & `gantry-0.6.0a0/gantry/dataset/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/dataset/gantry_dataset.py` & `gantry-0.6.0a0/gantry/dataset/gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/dataset/main.py` & `gantry-0.6.0a0/gantry/dataset/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/dataset/templates/load_script_template.py.jinja` & `gantry-0.6.0a0/gantry/dataset/templates/load_script_template.py.jinja`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/exceptions.py` & `gantry-0.6.0a0/gantry/exceptions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/logger/client.py` & `gantry-0.6.0a0/gantry/logger/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,15 +451,15 @@
         version: Optional[Union[int, str]] = None,
         inputs: Optional[Union[dict, List[dict], pd.DataFrame, pd.Series, np.ndarray]] = None,
         outputs: Optional[
             Union[Any, List[Any], dict, List[dict], pd.DataFrame, pd.Series, np.ndarray]
         ] = None,
         feedbacks: Optional[Union[dict, List[dict], pd.DataFrame, pd.Series, np.ndarray]] = None,
         tags: Optional[Union[Dict[str, str], List[Dict[str, str]]]] = None,
-        timestamps: Optional[
+        timestamp: Optional[
             Union[datetime.datetime, List[datetime.datetime], pd.DatetimeIndex, np.ndarray]
         ] = None,
         sort_on_timestamp: bool = True,
         sample_rate: float = 1.0,
         row_tags: Optional[
             Union[Dict[str, str], List[Dict[str, str]], pd.DataFrame, pd.Series, np.ndarray]
         ] = None,
@@ -536,26 +536,26 @@
             # If so, convert to list with one element.
             if isinstance(inputs, dict):
                 inputs = [inputs]
             if isinstance(outputs, dict):
                 outputs = [outputs]
             if isinstance(feedbacks, dict):
                 feedbacks = [feedbacks]
-            if isinstance(timestamps, datetime.datetime):
-                timestamps = [timestamps]
+            if isinstance(timestamp, datetime.datetime):
+                timestamp = [timestamp]
             if isinstance(join_keys, str):
                 join_keys = [join_keys]
             return self.generate_records(
                 application=application,
                 inputs=inputs,
                 outputs=outputs,
                 feedbacks=feedbacks,
                 global_tags=run_tags,
                 row_tags=row_tags,
-                timestamps=timestamps,
+                timestamps=timestamp,
                 join_keys=join_keys,
                 run_id=run_id,
                 version=version,
                 sample_rate=sample_rate,
                 sort_on_timestamp=sort_on_timestamp,
             )[0]
         else:
@@ -568,29 +568,29 @@
                 return self.single_log_record(
                     application=application,
                     version=version,
                     inputs=inputs,
                     outputs=outputs,
                     feedback=feedbacks,
                     tags=tags,
-                    timestamp=timestamps,
+                    timestamp=timestamp,
                     join_key=join_keys,
                     sample_rate=sample_rate,
                 )
             else:
                 return self.single_log_records(
                     application=application,
                     version=version,
                     inputs=inputs,
                     outputs=outputs,
                     feedbacks=feedbacks,
                     tags=tags,
                     row_tags=row_tags,
                     global_tags=global_tags,
-                    timestamps=timestamps,
+                    timestamps=timestamp,
                     join_keys=join_keys,
                     as_batch=as_batch,
                     sort_on_timestamp=sort_on_timestamp,
                     sample_rate=sample_rate,
                 )
 
     @_log_exception
@@ -765,14 +765,15 @@
                 t.update(global_tags)
         if row_tags:
             for t, row_tag in zip(tags, row_tags):
                 t.update(row_tag)
 
         for t in tags:
             _update_tags_with_env(self.environment, t)
+
         join_keys = _resolve_join_keys(size, inputs, feedback_ids, feedback_keys, join_keys)
         inputs, outputs, feedbacks, join_keys, timestamps, tags = _sample_records(
             size, sample_rate, inputs, outputs, feedbacks, join_keys, timestamps, tags
         )
         if preds_exist and feedbacks_exist:
             return self._generate_prediction_and_feedback_events(
                 application=application,
@@ -1021,15 +1022,15 @@
                 application=application,
                 inputs=inputs,
                 outputs=outputs,
                 ignore_inputs=ignore_inputs,
                 timestamps=timestamps,
                 sort_on_timestamp=sort_on_timestamp,
                 tags=tags,
-                join_keys=join_keys or [_default_join_key_gen() for _ in range(size)],
+                join_keys=join_keys,
                 version=version,
                 as_batch=as_batch,
             )
         elif feedbacks_exist:
             if join_keys is None:
                 raise ValueError(
                     "Can't submit feedback without submitting join_keys "
@@ -1600,40 +1601,38 @@
     def _log_prediction_and_feedback_events(
         self,
         application: str,
         inputs: List[dict],
         outputs: List[dict],
         feedbacks: List[dict],
         join_keys: List[str],
+        events: Optional[List[dict]] = None,
         version: Optional[Union[int, str]] = None,
         ignore_inputs: Optional[List[str]] = None,
         timestamps: Optional[Union[List[datetime.datetime], pd.DatetimeIndex, np.ndarray]] = None,
         sort_on_timestamp: bool = True,
         as_batch: bool = False,
         tags: Optional[List[Dict[str, str]]] = None,
     ) -> Tuple[Optional[str], List[str]]:
         """Internal method to log batch of predictions AND feedbacks
         This method can assume inputs/outputs/feedbacks/timestamps/tags have same size
         """
-        size = len(inputs)
-
-        timestamp_idx = _create_timestamp_idx(sort_on_timestamp, timestamps, size)
-
-        events = _build_prediction_and_feedback_events(
-            application=application,
-            timestamp_idx=timestamp_idx,
-            tags=tags,
-            version=version,
-            inputs=inputs,
-            outputs=outputs,
-            feedbacks=feedbacks,
-            join_keys=join_keys,
-            ignore_inputs=ignore_inputs,
-        )
-
+        if not events:
+            events, _ = self._generate_prediction_and_feedback_events(
+                application=application,
+                inputs=inputs,
+                outputs=outputs,
+                feedbacks=feedbacks,
+                join_keys=join_keys,
+                version=version,
+                ignore_inputs=ignore_inputs,
+                timestamps=timestamps,
+                sort_on_timestamp=sort_on_timestamp,
+                tags=tags,
+            )
         if events:
             if as_batch:
                 return (
                     self._upload_data_as_batch(application, version, events, BatchType.RECORD),
                     join_keys,
                 )
             else:
@@ -1923,40 +1922,42 @@
     @_log_exception
     def _log_prediction_events(
         self,
         application: str,
         inputs: List[dict],
         outputs: List[dict],
         join_keys: List[str],
+        events: Optional[List[dict]] = None,
         version: Optional[Union[int, str]] = None,
         ignore_inputs: Optional[List[str]] = None,
         timestamps: Optional[Union[List[datetime.datetime], pd.DatetimeIndex, np.ndarray]] = None,
         sort_on_timestamp: bool = True,
         as_batch: bool = False,
         tags: Optional[List[Dict[str, str]]] = None,
     ) -> Tuple[Optional[str], List[str]]:
         """Internal method to log a batch of prediction events
         This method can assume inputs/outputs/join_keys/timestamps have same size
         """
         batch_id = None
         try:
-            timestamp_idx = _create_timestamp_idx(sort_on_timestamp, timestamps, len(inputs))
-
-            events = _build_prediction_events(
-                application=application,
-                inputs=inputs,
-                outputs=outputs,
-                timestamp_idx=timestamp_idx,
-                tags=tags,
-                version=version,
-                join_keys=join_keys,
-                ignore_inputs=ignore_inputs,
-                batch_id=batch_id,
+            # Check if the events were already provided, if not then generate them
+            events = (
+                events
+                or self._generate_prediction_events(
+                    application=application,
+                    inputs=inputs,
+                    outputs=outputs,
+                    join_keys=join_keys,
+                    version=version,
+                    ignore_inputs=ignore_inputs,
+                    timestamps=timestamps,
+                    sort_on_timestamp=sort_on_timestamp,
+                    tags=tags,
+                )[0]
             )
-
             if events:
                 if as_batch:
                     return (
                         self._upload_data_as_batch(
                             application, version, events, BatchType.PREDICTION
                         ),
                         join_keys,
```

### Comparing `gantry-0.6.0/gantry/logger/constants.py` & `gantry-0.6.0a0/gantry/logger/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/logger/consumer.py` & `gantry-0.6.0a0/gantry/logger/consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/logger/event_builder.py` & `gantry-0.6.0a0/gantry/logger/event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/logger/main.py` & `gantry-0.6.0a0/gantry/logger/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/logger/stores.py` & `gantry-0.6.0a0/gantry/logger/stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/logger/types.py` & `gantry-0.6.0a0/gantry/logger/types.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/logger/utils.py` & `gantry-0.6.0a0/gantry/logger/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/query/__init__.py` & `gantry-0.6.0a0/gantry/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/query/client.py` & `gantry-0.6.0a0/gantry/query/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/query/core/dataframe.py` & `gantry-0.6.0a0/gantry/query/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/query/core/distance.py` & `gantry-0.6.0a0/gantry/query/core/distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/query/core/metric.py` & `gantry-0.6.0a0/gantry/query/core/metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/query/core/queryframe.py` & `gantry-0.6.0a0/gantry/query/core/queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/query/core/utils.py` & `gantry-0.6.0a0/gantry/query/core/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/query/distance/main.py` & `gantry-0.6.0a0/gantry/query/distance/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/query/globals.py` & `gantry-0.6.0a0/gantry/query/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/query/main.py` & `gantry-0.6.0a0/gantry/query/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/query/metric/main.py` & `gantry-0.6.0a0/gantry/query/metric/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/query/time_window.py` & `gantry-0.6.0a0/gantry/query/time_window.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/serializers.py` & `gantry-0.6.0a0/gantry/serializers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/utils.py` & `gantry-0.6.0a0/gantry/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry/validators.py` & `gantry-0.6.0a0/gantry/validators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/gantry.egg-info/PKG-INFO` & `gantry-0.6.0a0/gantry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.0
+Version: 0.6.0a0
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.0/gantry.egg-info/SOURCES.txt` & `gantry-0.6.0a0/gantry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/setup.py` & `gantry-0.6.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/alerts/test_client.py` & `gantry-0.6.0a0/tests/alerts/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/alerts/test_main.py` & `gantry-0.6.0a0/tests/alerts/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/cli/test_bucket.py` & `gantry-0.6.0a0/tests/cli/test_bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/cli/test_data_connector.py` & `gantry-0.6.0a0/tests/cli/test_data_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,16 +316,16 @@
                 "GANTRY_API_KEY": "test",
                 "GANTRY_LOGS_LOCATION": UNITTEST_HOST,
                 "GANTRY_DATASET_WORKING_DIR": "/tmp",
             },
         )
         assert result.exit_code == 0
         response = (
-            f'--> The following pipelines are given for "{APP_NAME}" app with status'
-            f' "{DATA_CONNECTOR_ENABLED_STATUS_CMD}"'
+            f"--> The following pipelines are given for {APP_NAME} "
+            f"and {DATA_CONNECTOR_ENABLED_STATUS_CMD}"
         )
         assert response in result.output
 
         assert (PIPELINE_ID) in result.output
         assert (PIPELINE_CONSUMER_ID) in result.output
```

### Comparing `gantry-0.6.0/tests/cli/test_labeling.py` & `gantry-0.6.0a0/tests/cli/test_labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/cli/test_projection.py` & `gantry-0.6.0a0/tests/cli/test_projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/cli/test_secrets.py` & `gantry-0.6.0a0/tests/cli/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/conftest.py` & `gantry-0.6.0a0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/curator/conftest.py` & `gantry-0.6.0a0/tests/curator/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/curator/test_curator.py` & `gantry-0.6.0a0/tests/curator/test_curator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/curator/test_main.py` & `gantry-0.6.0a0/tests/curator/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/curator/test_selectors.py` & `gantry-0.6.0a0/tests/curator/test_selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/data_generator/test_data_generator.py` & `gantry-0.6.0a0/tests/data_generator/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/dataset/conftest.py` & `gantry-0.6.0a0/tests/dataset/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/dataset/test_client.py` & `gantry-0.6.0a0/tests/dataset/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/dataset/test_gantry_dataset.py` & `gantry-0.6.0a0/tests/dataset/test_gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/dataset/test_main.py` & `gantry-0.6.0a0/tests/dataset/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/logger/test_consumer.py` & `gantry-0.6.0a0/tests/logger/test_consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/logger/test_event_builder.py` & `gantry-0.6.0a0/tests/logger/test_event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/logger/test_main.py` & `gantry-0.6.0a0/tests/logger/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/logger/test_stores.py` & `gantry-0.6.0a0/tests/logger/test_stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/logger/test_utils.py` & `gantry-0.6.0a0/tests/logger/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/query/conftest.py` & `gantry-0.6.0a0/tests/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/query/core/test_dataframe.py` & `gantry-0.6.0a0/tests/query/core/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/query/core/test_distance.py` & `gantry-0.6.0a0/tests/query/core/test_distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/query/core/test_filters.py` & `gantry-0.6.0a0/tests/query/core/test_filters.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/query/core/test_metric.py` & `gantry-0.6.0a0/tests/query/core/test_metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/query/core/test_queryframe.py` & `gantry-0.6.0a0/tests/query/core/test_queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/query/core/test_series.py` & `gantry-0.6.0a0/tests/query/core/test_series.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/query/core/test_utils.py` & `gantry-0.6.0a0/tests/query/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/query/distance/test_main.py` & `gantry-0.6.0a0/tests/query/distance/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/query/metric/test_main.py` & `gantry-0.6.0a0/tests/query/metric/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/query/test_client.py` & `gantry-0.6.0a0/tests/query/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/query/test_main.py` & `gantry-0.6.0a0/tests/query/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/test_api_client.py` & `gantry-0.6.0a0/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/test_init.py` & `gantry-0.6.0a0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/test_utils.py` & `gantry-0.6.0a0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.0/tests/test_validator.py` & `gantry-0.6.0a0/tests/test_validator.py`

 * *Files identical despite different names*

