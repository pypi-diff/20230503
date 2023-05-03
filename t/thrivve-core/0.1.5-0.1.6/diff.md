# Comparing `tmp/thrivve_core-0.1.5.tar.gz` & `tmp/thrivve_core-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-u9e0tnma/thrivve_core-0.1.5.tar", last modified: Thu Apr 27 11:32:24 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-srq3uk4x/thrivve_core-0.1.6.tar", last modified: Wed May  3 13:59:52 2023, max compression
```

## Comparing `thrivve_core-0.1.5.tar` & `thrivve_core-0.1.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/thrivve_core/
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/thrivve_core/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4218 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/thrivve_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/thrivve_core/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/amazon/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/thrivve_core/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/kafka_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)     2571 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/thrivve_core/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2297 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/kafka_producers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/kafka_producers/send_topic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12351 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/numbers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/system_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (122)      301 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-04-27 11:32:13.000000 thrivve_core-0.1.5/thrivve_core/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/thrivve_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/thrivve_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/thrivve_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/thrivve_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/thrivve_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-27 11:32:24.000000 thrivve_core-0.1.5/thrivve_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/thrivve_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/thrivve_core/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2110 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4218 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/thrivve_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/thrivve_core/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/amazon/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/thrivve_core/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/kafka_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3046 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/thrivve_core/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/kafka_producers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/kafka_producers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/kafka_producers/send_topic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12396 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/system_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-05-03 13:59:41.000000 thrivve_core-0.1.6/thrivve_core/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/thrivve_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/thrivve_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/thrivve_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/thrivve_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/thrivve_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-03 13:59:52.000000 thrivve_core-0.1.6/thrivve_core.egg-info/top_level.txt
```

### Comparing `thrivve_core-0.1.5/PKG-INFO` & `thrivve_core-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve_core
-Version: 0.1.5
+Version: 0.1.6
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.1.5/setup.py` & `thrivve_core-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="thrivve_core",
-    version="0.1.5",
+    version="0.1.6",
     description="thrivveCore package",
     long_description="""# Markdown supported!\n\n* thrivve\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
```

### Comparing `thrivve_core-0.1.5/thrivve_core/__init__.py` & `thrivve_core-0.1.6/thrivve_core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from .helpers.atomic_transactions import Transactions
 from .helpers.atomic_transactions_v2 import Transactions as TransactionV2
 from .helpers.auth import Auth
 from .helpers.enums import Service
 from .helpers.database.base_model import init_base_model
 from .helpers.database.log_model import init_log_model
 from .helpers.system_roles import Role
-from .helpers.kafka_listener import start_kafka_listener
 
 __all__ = [
     "ThrivveCore",
     "route",
     "Config",
     "Producer",
     "init_logger",
@@ -25,9 +24,8 @@
     "Transactions",
     "TransactionV2",
     "Service",
     "Auth",
     "init_base_model",
     "init_log_model",
     "Role",
-    "start_kafka_listener",
 ]
```

### Comparing `thrivve_core-0.1.5/thrivve_core/app_decorators/app_entry.py` & `thrivve_core-0.1.6/thrivve_core/app_decorators/app_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from thrivve_core import ThrivveCore
 from thrivve_core.app_decorators import (
     handle_response,
     handle_auth,
     handle_exceptions,
     serializer,
 )
-from thrivve_core.helpers.get_prefix import get_prefix
+# from thrivve_core.helpers.get_prefix import get_prefix
 
 
 def route(path, methods=["GET"], schema=None, many=False, allowed_roles=None, require_auth=True,
           append_auth_args=None,
           pre_login=False,
           allowed_permissions=None):
     app = ThrivveCore.get_app()
 
     def factory(func):
         @app.route(path, methods=methods)
-        @app.route(get_prefix(path), methods=methods)
+        # @app.route(get_prefix(path), methods=methods)
         @handle_response
         @handle_exceptions
         @handle_auth(require_auth=require_auth, append_auth_args=append_auth_args, allowed_roles=allowed_roles,
                      allowed_permissions=allowed_permissions, pre_login=pre_login)
         @serializer(schema=schema, many=many)
         @wraps(func)
         def decorator(*args, **kwargs):
```

### Comparing `thrivve_core-0.1.5/thrivve_core/app_decorators/handle_auth.py` & `thrivve_core-0.1.6/thrivve_core/app_decorators/handle_auth.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/app_decorators/handle_exceptions.py` & `thrivve_core-0.1.6/thrivve_core/app_decorators/handle_exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/app_decorators/handle_response.py` & `thrivve_core-0.1.6/thrivve_core/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/app_decorators/serializer.py` & `thrivve_core-0.1.6/thrivve_core/app_decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/base.py` & `thrivve_core-0.1.6/thrivve_core/base.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/acl_enum.py` & `thrivve_core-0.1.6/thrivve_core/helpers/acl_enum.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py` & `thrivve_core-0.1.6/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/amazon/get_file_url.py` & `thrivve_core-0.1.6/thrivve_core/helpers/amazon/get_file_url.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/amazon/get_s3_client.py` & `thrivve_core-0.1.6/thrivve_core/helpers/amazon/get_s3_client.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/amazon/upload_file.py` & `thrivve_core-0.1.6/thrivve_core/helpers/amazon/upload_file.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/atomic_transactions.py` & `thrivve_core-0.1.6/thrivve_core/helpers/atomic_transactions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/atomic_transactions_v2.py` & `thrivve_core-0.1.6/thrivve_core/helpers/atomic_transactions_v2.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/auth.py` & `thrivve_core-0.1.6/thrivve_core/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/config.py` & `thrivve_core-0.1.6/thrivve_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/database/base_model.py` & `thrivve_core-0.1.6/thrivve_core/helpers/database/base_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/database/log_model.py` & `thrivve_core-0.1.6/thrivve_core/helpers/database/log_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/enums.py` & `thrivve_core-0.1.6/thrivve_core/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/exceptions.py` & `thrivve_core-0.1.6/thrivve_core/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/fetch_relational_data.py` & `thrivve_core-0.1.6/thrivve_core/helpers/fetch_relational_data.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/filters.py` & `thrivve_core-0.1.6/thrivve_core/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/format_exception.py` & `thrivve_core-0.1.6/thrivve_core/helpers/format_exception.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/get_embedded_function.py` & `thrivve_core-0.1.6/thrivve_core/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/kafka_listener.py` & `thrivve_core-0.1.6/thrivve_core/helpers/kafka_listener.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,98 @@
 import importlib
 import json
 import os
-import time
-import traceback
 
-from confluent_kafka import Consumer
+from confluent_kafka import Consumer, KafkaError
 
 from thrivve_core import ThrivveCore
 from thrivve_core.app_decorators import handle_exceptions
 from thrivve_core.helpers.exceptions import AppValidationError
 
 
-def start_kafka_listener(topics):
-    """
-    Start Kafka listener
+def consume_message(message_payload):
+    message_payload = json.loads(message_payload)
+
+    # app = ThrivveCore.get_app()
+
+    # app.logger.debug(message_payload)
+
+    if not message_payload:
+        raise AppValidationError("No message payload found..")
+
+    function_name = message_payload.get("function_name")
+    function_params = message_payload.get("function_params") or {}
+    if not function_name:
+        raise AppValidationError("No function name found..")
+
+    @handle_exceptions
+    def _execute_method():
+        function_file, function_call = os.path.splitext(function_name)
+        module = importlib.import_module(function_file)
+        method = getattr(module, function_call[1:])
+
+        return method(**function_params)
+
+    _execute_method()
+    # function_result = _execute_method()
+    # app.logger.debug(function_result)
+
+
+def create_consumer(topics):
     """
+        Start Kafka listener
+        """
     app = ThrivveCore.get_app()
-    app.logger.info(f"Start Kafka listening to topics [{' - '.join(topics)}]..")
 
-    consumer = Consumer(
+    c = Consumer(
         {
             "bootstrap.servers": app.config.get("BOOTSTRAP_SERVERS"),
             "sasl.username": app.config.get("SASL_USERNAME"),
             "sasl.password": app.config.get("SASL_PASSWORD"),
             "security.protocol": "SASL_SSL",
             "sasl.mechanisms": "PLAIN",
             "group.id": "services_group",
-            "auto.offset.reset": "latest",
+            "auto.offset.reset": "latest",  # earliest or latest
         }
     )
 
-    consumer.subscribe(topics)
+    c.subscribe(topics)
 
-    try:
-        while True:
+    app.logger.info(f"Kafka Consumer created and subscribed to topics [{' - '.join(topics)}]")
 
-            msg = consumer.poll(timeout=3)
+    return c
 
-            if msg is None:
-                continue
-
-            if msg.error():
-                app.logger.error("error: {0}".format(msg.error()))
-                continue
 
-            app.logger.info("Got a message..")
+def poll_messages(consumer, wait_time=3.0):
+    app = ThrivveCore.get_app()
 
-            # message_key = msg.key()
+    wait_time = wait_time  # timeout is set to 10 second
 
-            try:
-                consume_message(msg.value())
-            except AppValidationError:
-                # app.logger.error(traceback.format_exc())
-                continue
+    app.logger.info(f"Kafka is polling messages for each ({wait_time} seconds)...")
 
-            time.sleep(1)
+    while True:
+        msg = consumer.poll(wait_time)
+        # print(1)
 
-    except KeyboardInterrupt:
-        app.logger.debug("Keyboard interrupted..")
-    finally:
-        app.logger.error(traceback.format_exc())
-        consumer.close()
+        if msg is None:
+            continue
 
+        if msg.error():
+            if msg.error().code() == KafkaError._PARTITION_EOF:
+                continue
 
-def consume_message(message_payload):
-    message_payload = json.loads(message_payload)
+            app.logger.error("error: {0}".format(msg.error()))
+            break
 
-    app = ThrivveCore.get_app()
+        # message_key = msg.key()
 
-    app.logger.debug(message_payload)
+        value = msg.value().decode('utf-8')
 
-    if not message_payload:
-        raise AppValidationError("No message payload found..")
+        app.logger.info(f'Got a message: {value}')
 
-    function_name = message_payload.get("function_name")
-    function_params = message_payload.get("function_params") or {}
-    if not function_name:
-        raise AppValidationError("No function name found..")
-
-    @handle_exceptions
-    def _execute_method():
-        function_file, function_call = os.path.splitext(function_name)
-        module = importlib.import_module(function_file)
-        method = getattr(module, function_call[1:])
-
-        return method(**function_params)
+        try:
+            consume_message(value)
+        except AppValidationError:
+            # app.logger.error(traceback.format_exc())
+            continue
 
-    function_result = _execute_method()
-    app.logger.debug(function_result)
+    consumer.close()
```

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/kafka_producers/notification_center.py` & `thrivve_core-0.1.6/thrivve_core/helpers/kafka_producers/notification_center.py`

 * *Files 22% similar despite different names*

```diff
@@ -39,43 +39,29 @@
                 title, str(app.config.get("SERVICE_NAME"))
             ),
             "text": message,
             "color": color,
             "icon_emoji": emoji,
         },
     }
-    app.logger.debug(data)
     kafka_producers.send_topic(topic=Topics.INTERNAL_NOTIFICATION_MESSAGE, datajson=data)
 
 
-
 def send_push_notification(
-        message, reference_type, user_ids, payload=None, created_by=None
+        message_text, reference_type, user_ids, title=None, payload=None, created_by=None, **kwargs
 ):
     # token = None
-    base_payload = dict(
-        content_available=True,
-        delay_while_idle=False,
-        time_to_live=3,
-        priority="high",
-        sound="sound1",
-        title="Thrivve",
-        body=message,
-        message=message,
-        result=payload,
-    )
-    if payload:
-        base_payload.update(payload)
 
     data = dict(
-        message=message,
-        reference_type=reference_type,
         user_ids=user_ids,
-        payload=base_payload,
+        reference_type=reference_type,
         created_by=created_by,
+        title=title or "Thrivve",
+        message_text=message_text,
+        payload=payload,
         # language="ar"
     )
 
     kafka_producers.send_topic(topic=Topics.THRIVVE_SEND_PUSH_NOTIFICATION, datajson=dict(
         function_name='app.business_logic.notification.send_push_notification.execute',
         function_params=data
-    ))
+    ), kafka_configs=kwargs.get('kafka_configs'))
```

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/log_config.py` & `thrivve_core-0.1.6/thrivve_core/helpers/log_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/micro_fetcher.py` & `thrivve_core-0.1.6/thrivve_core/helpers/micro_fetcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,17 @@
 
     def fetch(self):
         if self.column_values or self.module_name or self.query_type == QueryTypes.SEARCH.value:
             return self._call_api()
         else:
             return self.base_data
 
+    def execute(self):
+        self.fetch()
+
     def with_params(self, **kwargs):
         self.function_params = kwargs
         return self
 
     def from_function(self, module_name):
         self.query_type = QueryTypes.FUNCTION.value
         self.module_name = module_name
```

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/search_function.py` & `thrivve_core-0.1.6/thrivve_core/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/service_config.py` & `thrivve_core-0.1.6/thrivve_core/helpers/service_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/sql.py` & `thrivve_core-0.1.6/thrivve_core/helpers/sql.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/time.py` & `thrivve_core-0.1.6/thrivve_core/helpers/time.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/validate_mobile_number.py` & `thrivve_core-0.1.6/thrivve_core/helpers/validate_mobile_number.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core/helpers/validate_parameters.py` & `thrivve_core-0.1.6/thrivve_core/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.1.5/thrivve_core.egg-info/PKG-INFO` & `thrivve_core-0.1.6/thrivve_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thrivve-core
-Version: 0.1.5
+Version: 0.1.6
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.1.5/thrivve_core.egg-info/SOURCES.txt` & `thrivve_core-0.1.6/thrivve_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 thrivve_core/helpers/get_prefix.py
 thrivve_core/helpers/kafka_listener.py
 thrivve_core/helpers/kafka_producer.py
 thrivve_core/helpers/log_config.py
 thrivve_core/helpers/micro_fetcher.py
 thrivve_core/helpers/numbers.py
 thrivve_core/helpers/search_function.py
-thrivve_core/helpers/send_sms.py
 thrivve_core/helpers/service_config.py
 thrivve_core/helpers/sql.py
 thrivve_core/helpers/system_roles.py
 thrivve_core/helpers/time.py
 thrivve_core/helpers/topics.py
 thrivve_core/helpers/validate_mobile_number.py
 thrivve_core/helpers/validate_parameters.py
@@ -50,8 +49,9 @@
 thrivve_core/helpers/amazon/upload_file.py
 thrivve_core/helpers/database/__init__.py
 thrivve_core/helpers/database/base_model.py
 thrivve_core/helpers/database/log_model.py
 thrivve_core/helpers/kafka_producers/__init__.py
 thrivve_core/helpers/kafka_producers/log_model_changes.py
 thrivve_core/helpers/kafka_producers/notification_center.py
+thrivve_core/helpers/kafka_producers/send_sms.py
 thrivve_core/helpers/kafka_producers/send_topic.py
```

