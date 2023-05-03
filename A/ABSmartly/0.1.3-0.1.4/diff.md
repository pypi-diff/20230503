# Comparing `tmp/ABSmartly-0.1.3.tar.gz` & `tmp/ABSmartly-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ABSmartly-0.1.3.tar", last modified: Sat Nov 12 21:27:56 2022, max compression
+gzip compressed data, was "ABSmartly-0.1.4.tar", last modified: Wed May  3 09:49:39 2023, max compression
```

## Comparing `ABSmartly-0.1.3.tar` & `ABSmartly-0.1.4.tar`

### file list

```diff
@@ -1,96 +1,95 @@
-drwxr-xr-x   0 buhalo     (501) staff       (20)        0 2022-11-12 21:27:56.548126 ABSmartly-0.1.3/
-drwxr-xr-x   0 buhalo     (501) staff       (20)        0 2022-11-12 21:27:56.517716 ABSmartly-0.1.3/ABSmartly.egg-info/
--rw-r--r--   0 buhalo     (501) staff       (20)     9805 2022-11-12 21:27:56.000000 ABSmartly-0.1.3/ABSmartly.egg-info/PKG-INFO
--rw-r--r--   0 buhalo     (501) staff       (20)     2684 2022-11-12 21:27:56.000000 ABSmartly-0.1.3/ABSmartly.egg-info/SOURCES.txt
--rw-r--r--   0 buhalo     (501) staff       (20)        1 2022-11-12 21:27:56.000000 ABSmartly-0.1.3/ABSmartly.egg-info/dependency_links.txt
--rw-r--r--   0 buhalo     (501) staff       (20)       91 2022-11-12 21:27:56.000000 ABSmartly-0.1.3/ABSmartly.egg-info/requires.txt
--rw-r--r--   0 buhalo     (501) staff       (20)        4 2022-11-12 21:27:56.000000 ABSmartly-0.1.3/ABSmartly.egg-info/top_level.txt
--rw-r--r--   0 buhalo     (501) staff       (20)     1091 2022-11-12 21:24:10.000000 ABSmartly-0.1.3/LICENSE
--rw-r--r--   0 buhalo     (501) staff       (20)       17 2022-11-12 21:21:07.000000 ABSmartly-0.1.3/MANIFEST.in
--rw-r--r--   0 buhalo     (501) staff       (20)     9805 2022-11-12 21:27:56.547819 ABSmartly-0.1.3/PKG-INFO
--rw-r--r--   0 buhalo     (501) staff       (20)     8102 2022-11-12 21:13:30.000000 ABSmartly-0.1.3/README.MD
--rw-r--r--   0 buhalo     (501) staff       (20)      796 2022-11-12 21:26:27.000000 ABSmartly-0.1.3/pyproject.toml
-drwxr-xr-x   0 buhalo     (501) staff       (20)        0 2022-11-12 21:27:56.526745 ABSmartly-0.1.3/sdk/
--rw-r--r--   0 buhalo     (501) staff       (20)        0 2022-09-25 09:15:46.000000 ABSmartly-0.1.3/sdk/__init__.py
--rw-r--r--   0 buhalo     (501) staff       (20)     2852 2022-11-12 20:03:07.000000 ABSmartly-0.1.3/sdk/absmarly.py
--rw-r--r--   0 buhalo     (501) staff       (20)      706 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/absmartly_config.py
--rw-r--r--   0 buhalo     (501) staff       (20)      290 2022-11-12 13:31:53.000000 ABSmartly-0.1.3/sdk/audience_deserializer.py
--rw-r--r--   0 buhalo     (501) staff       (20)     1083 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/audience_matcher.py
--rw-r--r--   0 buhalo     (501) staff       (20)     2052 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/client.py
--rw-r--r--   0 buhalo     (501) staff       (20)      704 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/client_config.py
--rw-r--r--   0 buhalo     (501) staff       (20)    29012 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/context.py
--rw-r--r--   0 buhalo     (501) staff       (20)      332 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/context_config.py
--rw-r--r--   0 buhalo     (501) staff       (20)      313 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/context_data_deserializer.py
--rw-r--r--   0 buhalo     (501) staff       (20)      293 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/context_data_provider.py
--rw-r--r--   0 buhalo     (501) staff       (20)      376 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/context_event_handler.py
--rw-r--r--   0 buhalo     (501) staff       (20)      378 2022-10-29 15:04:42.000000 ABSmartly-0.1.3/sdk/context_event_logger.py
--rw-r--r--   0 buhalo     (501) staff       (20)      234 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/context_event_serializer.py
--rw-r--r--   0 buhalo     (501) staff       (20)      465 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/default_audience_deserializer.py
--rw-r--r--   0 buhalo     (501) staff       (20)      538 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/default_context_data_deserializer.py
--rw-r--r--   0 buhalo     (501) staff       (20)      440 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/default_context_data_provider.py
--rw-r--r--   0 buhalo     (501) staff       (20)      578 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/default_context_event_handler.py
--rw-r--r--   0 buhalo     (501) staff       (20)      378 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/default_context_event_serializer.py
--rw-r--r--   0 buhalo     (501) staff       (20)     2579 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/default_http_client.py
--rw-r--r--   0 buhalo     (501) staff       (20)      209 2022-10-30 20:18:51.000000 ABSmartly-0.1.3/sdk/default_http_client_config.py
--rw-r--r--   0 buhalo     (501) staff       (20)      495 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/default_variable_parser.py
--rw-r--r--   0 buhalo     (501) staff       (20)      634 2022-11-12 13:43:55.000000 ABSmartly-0.1.3/sdk/http_client.py
-drwxr-xr-x   0 buhalo     (501) staff       (20)        0 2022-11-12 21:27:56.528979 ABSmartly-0.1.3/sdk/internal/
--rw-r--r--   0 buhalo     (501) staff       (20)        0 2022-10-29 13:08:06.000000 ABSmartly-0.1.3/sdk/internal/__init__.py
--rw-r--r--   0 buhalo     (501) staff       (20)      795 2022-11-12 13:28:33.000000 ABSmartly-0.1.3/sdk/internal/buffers.py
-drwxr-xr-x   0 buhalo     (501) staff       (20)        0 2022-11-12 21:27:56.531250 ABSmartly-0.1.3/sdk/internal/lock/
--rw-r--r--   0 buhalo     (501) staff       (20)        0 2022-10-29 13:08:06.000000 ABSmartly-0.1.3/sdk/internal/lock/__init__.py
--rw-r--r--   0 buhalo     (501) staff       (20)      457 2022-10-29 12:48:49.000000 ABSmartly-0.1.3/sdk/internal/lock/atomic_bool.py
--rw-r--r--   0 buhalo     (501) staff       (20)      488 2022-10-30 17:46:15.000000 ABSmartly-0.1.3/sdk/internal/lock/atomic_int.py
--rw-r--r--   0 buhalo     (501) staff       (20)     1472 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/internal/lock/concurrency.py
--rw-r--r--   0 buhalo     (501) staff       (20)      688 2022-11-12 13:27:31.000000 ABSmartly-0.1.3/sdk/internal/lock/read_write_lock.py
--rw-r--r--   0 buhalo     (501) staff       (20)     1781 2022-11-12 13:28:00.000000 ABSmartly-0.1.3/sdk/internal/murmur32.py
--rw-r--r--   0 buhalo     (501) staff       (20)     1084 2022-11-12 20:02:56.000000 ABSmartly-0.1.3/sdk/internal/variant_assigner.py
-drwxr-xr-x   0 buhalo     (501) staff       (20)        0 2022-11-12 21:27:56.535643 ABSmartly-0.1.3/sdk/json/
--rw-r--r--   0 buhalo     (501) staff       (20)        0 2022-09-25 09:15:46.000000 ABSmartly-0.1.3/sdk/json/__init__.py
--rw-r--r--   0 buhalo     (501) staff       (20)      121 2022-10-30 17:31:43.000000 ABSmartly-0.1.3/sdk/json/attribute.py
--rw-r--r--   0 buhalo     (501) staff       (20)      137 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/json/context_data.py
--rw-r--r--   0 buhalo     (501) staff       (20)       83 2022-10-30 12:26:24.000000 ABSmartly-0.1.3/sdk/json/experiement_application.py
--rw-r--r--   0 buhalo     (501) staff       (20)      844 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/json/experiment.py
--rw-r--r--   0 buhalo     (501) staff       (20)      119 2022-10-30 12:26:24.000000 ABSmartly-0.1.3/sdk/json/experiment_variant.py
--rw-r--r--   0 buhalo     (501) staff       (20)      489 2022-10-30 17:31:43.000000 ABSmartly-0.1.3/sdk/json/exposure.py
--rw-r--r--   0 buhalo     (501) staff       (20)      137 2022-10-30 17:31:43.000000 ABSmartly-0.1.3/sdk/json/goal_achievement.py
--rw-r--r--   0 buhalo     (501) staff       (20)      499 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/json/publish_event.py
--rw-r--r--   0 buhalo     (501) staff       (20)      103 2022-10-30 12:26:24.000000 ABSmartly-0.1.3/sdk/json/unit.py
-drwxr-xr-x   0 buhalo     (501) staff       (20)        0 2022-11-12 21:27:56.537186 ABSmartly-0.1.3/sdk/jsonexpr/
--rw-r--r--   0 buhalo     (501) staff       (20)      719 2022-11-12 13:30:06.000000 ABSmartly-0.1.3/sdk/jsonexpr/evaluator.py
--rw-r--r--   0 buhalo     (501) staff       (20)     3252 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/expr_evaluator.py
--rw-r--r--   0 buhalo     (501) staff       (20)     1770 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/json_expr.py
--rw-r--r--   0 buhalo     (501) staff       (20)      210 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operator.py
-drwxr-xr-x   0 buhalo     (501) staff       (20)        0 2022-11-12 21:27:56.541239 ABSmartly-0.1.3/sdk/jsonexpr/operators/
--rw-r--r--   0 buhalo     (501) staff       (20)      366 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/and_combinator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      668 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/binary_operator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      448 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/boolean_combinator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      366 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/equals_operator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      329 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/greater_than_operator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      337 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/greater_than_or_equal_operator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      635 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/in_operator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      326 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/less_than_operator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      335 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/less_than_or_equal_operator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      510 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/match_operator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      298 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/not_operator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      229 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/null_operator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      367 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/or_combinator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      405 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/unary_operator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      203 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/value_operator.py
--rw-r--r--   0 buhalo     (501) staff       (20)      401 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/jsonexpr/operators/var_operator.py
-drwxr-xr-x   0 buhalo     (501) staff       (20)        0 2022-11-12 21:27:56.542691 ABSmartly-0.1.3/sdk/time/
--rw-r--r--   0 buhalo     (501) staff       (20)      123 2022-10-25 13:50:20.000000 ABSmartly-0.1.3/sdk/time/clock.py
--rw-r--r--   0 buhalo     (501) staff       (20)      174 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/time/fixed_clock.py
--rw-r--r--   0 buhalo     (501) staff       (20)      155 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/sdk/time/system_clock_utc.py
--rw-r--r--   0 buhalo     (501) staff       (20)      304 2022-11-12 13:32:14.000000 ABSmartly-0.1.3/sdk/variable_parser.py
--rw-r--r--   0 buhalo     (501) staff       (20)       38 2022-11-12 21:27:56.548198 ABSmartly-0.1.3/setup.cfg
--rw-r--r--   0 buhalo     (501) staff       (20)      736 2022-11-12 21:12:35.000000 ABSmartly-0.1.3/setup.py
-drwxr-xr-x   0 buhalo     (501) staff       (20)        0 2022-11-12 21:27:56.547158 ABSmartly-0.1.3/test/
--rw-r--r--   0 buhalo     (501) staff       (20)     2070 2022-11-12 20:02:56.000000 ABSmartly-0.1.3/test/test_buffers.py
--rw-r--r--   0 buhalo     (501) staff       (20)     4628 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/test/test_client.py
--rw-r--r--   0 buhalo     (501) staff       (20)    37149 2022-11-12 20:02:56.000000 ABSmartly-0.1.3/test/test_context.py
--rw-r--r--   0 buhalo     (501) staff       (20)     1072 2022-11-12 20:02:56.000000 ABSmartly-0.1.3/test/test_default_audience_deserializer.py
--rw-r--r--   0 buhalo     (501) staff       (20)     5387 2022-11-12 20:03:09.000000 ABSmartly-0.1.3/test/test_default_context_data_deserializer.py
--rw-r--r--   0 buhalo     (501) staff       (20)     2724 2022-11-12 20:02:56.000000 ABSmartly-0.1.3/test/test_default_context_event_serializer.py
--rw-r--r--   0 buhalo     (501) staff       (20)     2692 2022-11-12 20:02:56.000000 ABSmartly-0.1.3/test/test_murmur32.py
--rw-r--r--   0 buhalo     (501) staff       (20)     5517 2022-11-12 20:02:56.000000 ABSmartly-0.1.3/test/test_variant_assigner.py
+drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-05-03 09:49:39.107579 ABSmartly-0.1.4/
+drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-05-03 09:49:39.097579 ABSmartly-0.1.4/ABSmartly.egg-info/
+-rw-r--r--   0 arch      (1000) arch      (1000)    13469 2023-05-03 09:49:39.000000 ABSmartly-0.1.4/ABSmartly.egg-info/PKG-INFO
+-rw-r--r--   0 arch      (1000) arch      (1000)     2512 2023-05-03 09:49:39.000000 ABSmartly-0.1.4/ABSmartly.egg-info/SOURCES.txt
+-rw-r--r--   0 arch      (1000) arch      (1000)        1 2023-05-03 09:49:39.000000 ABSmartly-0.1.4/ABSmartly.egg-info/dependency_links.txt
+-rw-r--r--   0 arch      (1000) arch      (1000)       91 2023-05-03 09:49:39.000000 ABSmartly-0.1.4/ABSmartly.egg-info/requires.txt
+-rw-r--r--   0 arch      (1000) arch      (1000)        4 2023-05-03 09:49:39.000000 ABSmartly-0.1.4/ABSmartly.egg-info/top_level.txt
+-rw-r--r--   0 arch      (1000) arch      (1000)     1091 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/LICENSE
+-rw-r--r--   0 arch      (1000) arch      (1000)       18 2023-05-03 09:45:37.000000 ABSmartly-0.1.4/MANIFEST.in
+-rw-r--r--   0 arch      (1000) arch      (1000)    13469 2023-05-03 09:49:39.107579 ABSmartly-0.1.4/PKG-INFO
+-rw-r--r--   0 arch      (1000) arch      (1000)    11835 2023-05-03 09:45:37.000000 ABSmartly-0.1.4/README.md
+-rw-r--r--   0 arch      (1000) arch      (1000)      796 2023-05-03 09:45:37.000000 ABSmartly-0.1.4/pyproject.toml
+drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-05-03 09:49:39.097579 ABSmartly-0.1.4/sdk/
+-rw-r--r--   0 arch      (1000) arch      (1000)        0 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/__init__.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     2852 2023-05-03 09:45:14.000000 ABSmartly-0.1.4/sdk/absmartly.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      706 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/absmartly_config.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      290 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/audience_deserializer.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     1083 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/audience_matcher.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     2052 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/client.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      704 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/client_config.py
+-rw-r--r--   0 arch      (1000) arch      (1000)    29051 2023-05-03 09:45:37.000000 ABSmartly-0.1.4/sdk/context.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      332 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/context_config.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      313 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/context_data_deserializer.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      293 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/context_data_provider.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      376 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/context_event_handler.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      378 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/context_event_logger.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      234 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/context_event_serializer.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      465 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/default_audience_deserializer.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      538 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/default_context_data_deserializer.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      440 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/default_context_data_provider.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      578 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/default_context_event_handler.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      378 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/default_context_event_serializer.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     2579 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/default_http_client.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      209 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/default_http_client_config.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      495 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/default_variable_parser.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      634 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/http_client.py
+drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-05-03 09:49:39.097579 ABSmartly-0.1.4/sdk/internal/
+-rw-r--r--   0 arch      (1000) arch      (1000)        0 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/internal/__init__.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      795 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/internal/buffers.py
+drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-05-03 09:49:39.107579 ABSmartly-0.1.4/sdk/internal/lock/
+-rw-r--r--   0 arch      (1000) arch      (1000)        0 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/internal/lock/__init__.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      457 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/internal/lock/atomic_bool.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      488 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/internal/lock/atomic_int.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     1472 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/internal/lock/concurrency.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      688 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/internal/lock/read_write_lock.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     1781 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/internal/murmur32.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     1084 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/internal/variant_assigner.py
+drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-05-03 09:49:39.107579 ABSmartly-0.1.4/sdk/json/
+-rw-r--r--   0 arch      (1000) arch      (1000)        0 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/json/__init__.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      121 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/json/attribute.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      137 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/json/context_data.py
+-rw-r--r--   0 arch      (1000) arch      (1000)       83 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/json/experiement_application.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      844 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/json/experiment.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      119 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/json/experiment_variant.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      489 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/json/exposure.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      137 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/json/goal_achievement.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      499 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/json/publish_event.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      103 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/json/unit.py
+drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-05-03 09:49:39.107579 ABSmartly-0.1.4/sdk/jsonexpr/
+-rw-r--r--   0 arch      (1000) arch      (1000)      719 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/evaluator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     3252 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/expr_evaluator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     1770 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/json_expr.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      210 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operator.py
+drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-05-03 09:49:39.107579 ABSmartly-0.1.4/sdk/jsonexpr/operators/
+-rw-r--r--   0 arch      (1000) arch      (1000)      366 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/and_combinator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      668 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/binary_operator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      448 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/boolean_combinator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      366 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/equals_operator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      329 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/greater_than_operator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      337 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/greater_than_or_equal_operator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      635 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/in_operator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      326 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/less_than_operator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      335 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/less_than_or_equal_operator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      510 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/match_operator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      298 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/not_operator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      229 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/null_operator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      367 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/or_combinator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      405 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/unary_operator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      203 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/value_operator.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      401 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/jsonexpr/operators/var_operator.py
+drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-05-03 09:49:39.107579 ABSmartly-0.1.4/sdk/time/
+-rw-r--r--   0 arch      (1000) arch      (1000)      123 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/time/clock.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      174 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/time/fixed_clock.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      155 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/time/system_clock_utc.py
+-rw-r--r--   0 arch      (1000) arch      (1000)      304 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/sdk/variable_parser.py
+-rw-r--r--   0 arch      (1000) arch      (1000)       38 2023-05-03 09:49:39.107579 ABSmartly-0.1.4/setup.cfg
+drwxr-xr-x   0 arch      (1000) arch      (1000)        0 2023-05-03 09:49:39.107579 ABSmartly-0.1.4/test/
+-rw-r--r--   0 arch      (1000) arch      (1000)     2070 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/test/test_buffers.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     4628 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/test/test_client.py
+-rw-r--r--   0 arch      (1000) arch      (1000)    40123 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/test/test_context.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     1072 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/test/test_default_audience_deserializer.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     5387 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/test/test_default_context_data_deserializer.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     2724 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/test/test_default_context_event_serializer.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     2692 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/test/test_murmur32.py
+-rw-r--r--   0 arch      (1000) arch      (1000)     5517 2023-04-27 12:51:02.000000 ABSmartly-0.1.4/test/test_variant_assigner.py
```

### Comparing `ABSmartly-0.1.3/ABSmartly.egg-info/PKG-INFO` & `ABSmartly-0.1.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,249 +1,276 @@
-Metadata-Version: 2.1
-Name: ABSmartly
-Version: 0.1.3
-Summary: ABSmartly Python SDK lib
-Home-page: https://github.com/absmartly/python-sdk
-Author: ABSmartly
-Author-email: ABSmartly <info@ABSmartly.com>
-License: The MIT License (MIT)
-        Copyright © 2022 <copyright holders>
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Project-URL: Homepage, https://github.com/absmartly/python3-sdk
-Keywords: ABSmartly,SDK,Testing
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # A/B Smartly SDK
 
 A/B Smartly - Python SDK
 
 ## Compatibility
 
 The A/B Smartly Python SDK is compatible with Python 3.
 It provides both a blocking and an asynchronous interfaces.
 
+## Getting Started
 
-## Installation
-pip install absmartly==0.1.2
+### Install the SDK
+ ```bash
+ pip install absmartly==0.1.2
+ ```
 
-### Python Modules
+### Dependencies
+```
 setuptools~=60.2.0  
 requests~=2.28.1  
 urllib3~=1.26.12  
 jsons~=1.6.3
+```
 
-### Dependencies
-sh ./run.sh
 
-## Getting Started
 
-Please follow the [installation](#installation) instructions before trying the following code:
+## Import and Initialize the SDK
 
-#### Initialization
-This example assumes an Api Key, an Application, and an Environment have been created in the A/B Smartly web console.
+Once the SDK is installed, it can be initialized in your project.
 ```python
+    def main():
+        client_config = ClientConfig()
+        client_config.endpoint = "https://sandbox.test.io/v1"
+        client_config.api_key = "test"
+        client_config.application = "www"
+        client_config.environment = "prod"
+    
+        default_client_config = DefaultHTTPClientConfig()
+        default_client = DefaultHTTPClient(default_client_config)
+        sdk_config = ABSmartlyConfig()
+        sdk_config.client = Client(client_config, default_client)
+        sdk = ABSmartly(sdk_config)
+    
+        context_config = ContextConfig()
+        ctx = sdk.create_context(context_config)
+```
+
+**SDK Options**
+
+| Config      | Type                                          | Required? |                 Default                 | Description                                                                                                                                                                   |
+| :---------- |:----------------------------------------------| :-------: |:---------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| endpoint    | `string`                                      |  &#9989;  |               `undefined`               | The URL to your API endpoint. Most commonly `"your-company.absmartly.io"`                                                                                                     |
+| apiKey      | `string`                                      |  &#9989;  |               `undefined`               | Your API key which can be found on the Web Console.                                                                                                                           |
+| environment | `"production"` or `"development"`             |  &#9989;  |               `undefined`               | The environment of the platform where the SDK is installed. Environments are created on the Web Console and should match the available environments in your infrastructure.   |
+| application | `string`                                      |  &#9989;  |               `undefined`               | The name of the application where the SDK is installed. Applications are created on the Web Console and should match the applications where your experiments will be running. |
+| max_retries     | `number`                                      | &#10060;  |                   `5`                   | The number of retries before the SDK stops trying to connect.                                                                                                                 |
+| connection_timeout     | `number`                                      | &#10060;  |                   `3`                   | An amount of time, in seconds, before the SDK will stop trying to connect.                                                                                                    |
+| context_event_logger | `(self, event_type: EventType, data: object)` | &#10060;  | See "Using a Custom Event Logger" below | A callback function which runs after SDK events.                                                                                                                              
 
-def main():
-    client_config = ClientConfig()
-    client_config.endpoint = "https://sandbox.test.io/v1"
-    client_config.api_key = "test"
-    client_config.application = "www"
-    client_config.environment = "prod"
+#### Using a custom Event Logger
+The A/B Smartly SDK can be instantiated with an event logger used for all contexts.
+In addition, an event logger can be specified when creating a particular context, in the `ContextConfig`.
+```python
+    class EventType(Enum):
+        ERROR = "error"
+        READY = "ready"
+        REFRESH = "refresh"
+        PUBLISH = "publish"
+        EXPOSURE = "exposure"
+        GOAL = "goal"
+        CLOSE = "close"
+    
+    
+    class ContextEventLogger:
+    
+        @abstractmethod
+        def handle_event(self, event_type: EventType, data: object):
+            raise NotImplementedError
+```
+The data parameter depends on the type of event.
+Currently, the SDK logs the following events:
+
+| event | when                                                       | data |
+|:---: |------------------------------------------------------------|---|
+| `Error` | `Context` receives an error                                | `Throwable` object |
+| `Ready` | `Context` turns ready                                      | `ContextData` used to initialize the context |
+| `Refresh` | `Context.refresh()` method succeeds                        | `ContextData` used to refresh the context |
+| `Publish` | `Context.publish()` method succeeds                        | `PublishEvent` sent to the A/B Smartly event collector |
+| `Exposure` | `Context.getTreatment()` method succeeds on first exposure | `Exposure` enqueued for publishing |
+| `Goal` | `Context.track()` method succeeds                          | `GoalAchievement` enqueued for publishing |
+| `Close` | `Context.close()` method succeeds the first time           | `null` |
 
-    default_client_config = DefaultHTTPClientConfig()
-    default_client = DefaultHTTPClient(default_client_config)
-    sdk_config = ABSmartlyConfig()
-    sdk_config.client = Client(client_config, default_client)
-    sdk = ABSmartly(sdk_config)
 
+## Create a New Context Request
+
+**Synchronously**
+```python
+# define a new context request
     context_config = ContextConfig()
-    ctx = sdk.create_context(context_config)
+    context_config.publish_delay = 10
+    context_config.refresh_interval = 5
 
-   # ...
-}
+    context_config = ContextConfig()
+    ctx = sdk.create_context(context_config)
+    ctx.wait_until_ready()
 ```
 
-#### Creating a new Context synchronously
+**Asynchronously**
 ```python
 # define a new context request
     context_config = ContextConfig()
     context_config.publish_delay = 10
     context_config.refresh_interval = 5
-    context_config.units = {"session_id": "bf06d8cb5d8137290c4abb64155584fbdb64d8",
-                            "user_id": "12345"}
 
     context_config = ContextConfig()
     ctx = sdk.create_context(context_config)
-    ctx.wait_until_ready()
+    ctx.wait_until_ready_async()
 ```
 
-#### Creating a new Context asynchronously
+**With Prefetched Data**
 ```python
 # define a new context request
     context_config = ContextConfig()
     context_config.publish_delay = 10
     context_config.refresh_interval = 5
     context_config.units = {"session_id": "bf06d8cb5d8137290c4abb64155584fbdb64d8",
                             "user_id": "12345"}
-
+    
     context_config = ContextConfig()
     ctx = sdk.create_context(context_config)
     ctx.wait_until_ready_async()
 ```
 
-#### Setting extra units for a context
+**Refreshing the Context with Fresh Experiment Data**
+For long-running contexts, the context is usually created once when the application is first started.
+However, any experiments being tracked in your production code, but started after the context was created, will not be triggered.
+To mitigate this, we can use the `set_refresh_interval()` method on the context config.
+
+```python
+    default_client_config = DefaultHTTPClientConfig()
+    default_client_config.refresh_interval = 5
+```
+
+Alternatively, the `refresh()` method can be called manually.
+The `refresh()` method pulls updated experiment data from the A/B Smartly collector and will trigger recently started experiments when `get_treatment()` is called again.
+```python
+    context.refresh()
+```
+
+**Setting Extra Units**
 You can add additional units to a context by calling the `set_unit()` or the `set_units()` method.
 This method may be used for example, when a user logs in to your application, and you want to use the new unit type to the context.
 Please note that **you cannot override an already set unit type** as that would be a change of identity, and will throw an exception. In this case, you must create a new context instead.
 The `SetUnit()` and `SetUnits()` methods can be called before the context is ready.
 
 ```python
-context.set_unit("db_user_id", "1000013")
-
-context.set_units({
-		"db_user_id": "1000013"
-})
+    context.set_unit("db_user_id", "1000013")
+    
+    context.set_units({
+            "db_user_id": "1000013"
+    })
 ```
 
-#### Setting context attributes
-The `set_attributes()` and `set_attributes()` methods can be called before the context is ready.
-```python
-context.set_attributes("user_agent", req.get_header("User-Agent"))
-
-context.set_attributes({
-        "customer_age": "new_customer"
-})
-```
+## Basic Usage
 
 #### Selecting a treatment
 ```python
-res, _ = context.get_treatment("exp_test_experiment")
-if res == 0:
-        # user is in control group (variant 0)
-else:
-       # user is in treatment group
+    res, _ = context.get_treatment("exp_test_experiment")
+    if res == 0:
+            # user is in control group (variant 0)
+    else:
+           # user is in treatment group
 ```
 
-#### Tracking a goal achievement
-Goals are created in the A/B Smartly web console.
+### Treatment Variables
+
 ```python
-context.track("payment", {
-        "item_count": 1,
-        "total_amount": 1999.99
-})
+     res = context.get_variable_value(key, 17)
 ```
 
-#### Publishing pending data
-Sometimes it is necessary to ensure all events have been published to the A/B Smartly collector, before proceeding.
-You can explicitly call the `publish()` or `publish_async()` methods.
+
+#### Peek at treatment variants
+Although generally not recommended, it is sometimes necessary to peek at a treatment or variable without triggering an exposure.
+The A/B Smartly SDK provides a `peek_treament()` method for that.
+
 ```python
-    context.publish()
-```
+    res = context.peek_treament("exp_test_experiment")
+    if res == 0:
+        # user is in control group (variant 0)
+    else:
+        # user is in treatment group
 
-#### Finalizing
-The `close()` and `close_async()` methods will ensure all events have been published to the A/B Smartly collector, like `publish()`, and will also "seal" the context, throwing an error if any method that could generate an event is called.
+```
+##### Peeking at variables
 ```python
-context.close()
+    variable = context.peek_variable("my_variable")
 ```
 
-#### Refreshing the context with fresh experiment data
-For long-running contexts, the context is usually created once when the application is first started.
-However, any experiments being tracked in your production code, but started after the context was created, will not be triggered.
-To mitigate this, we can use the `set_refresh_interval()` method on the context config.
-
+#### Overriding treatment variants
+During development, for example, it is useful to force a treatment for an experiment. This can be achieved with the `override()` and/or `overrides()` methods.
+The `set_override()` and `set_overrides()` methods can be called before the context is ready.
 ```python
-    default_client_config = DefaultHTTPClientConfig()
-    default_client_config.refresh_interval = 5
+    context.set_override("exp_test_experiment", 1) # force variant 1 of treatment
+    context.set_overrides({
+        "exp_test_experiment": 1,
+        "exp_another_experiment": 0
+    })
 ```
 
-Alternatively, the `refresh()` method can be called manually.
-The `refresh()` method pulls updated experiment data from the A/B Smartly collector and will trigger recently started experiments when `get_treatment()` is called again.
+## Advanced
+
+### Context Attributes
+Attributes are used to pass meta-data about the user and/or the request.
+They can be used later in the Web Console to create segments or audiences.
+The `set_attributes()` and `set_attributes()` methods can be called before the context is ready.
 ```python
-context.refresh()
+    context.set_attributes("user_agent", req.get_header("User-Agent"))
+    
+    context.set_attributes({
+            "customer_age": "new_customer"
+    })
 ```
 
-#### Using a custom Event Logger
-The A/B Smartly SDK can be instantiated with an event logger used for all contexts.
-In addition, an event logger can be specified when creating a particular context, in the `ContextConfig`.
-```python
-class EventType(Enum):
-    ERROR = "error"
-    READY = "ready"
-    REFRESH = "refresh"
-    PUBLISH = "publish"
-    EXPOSURE = "exposure"
-    GOAL = "goal"
-    CLOSE = "close"
+### Custom Assignments
 
+Sometimes it may be necessary to override the automatic selection of a
+variant. For example, if you wish to have your variant chosen based on
+data from an API call. This can be accomplished using the
+`set_custom_assignment()` method.
 
-class ContextEventLogger:
-
-    @abstractmethod
-    def handle_event(self, event_type: EventType, data: object):
-        raise NotImplementedError
+```python
+    context.set_custom_assignment("exp_test_not_eligible", 3)
 ```
-The data parameter depends on the type of event.
-Currently, the SDK logs the following events:
-
-| event | when                                                       | data |
-|:---: |------------------------------------------------------------|---|
-| `Error` | `Context` receives an error                                | `Throwable` object |
-| `Ready` | `Context` turns ready                                      | `ContextData` used to initialize the context |
-| `Refresh` | `Context.refresh()` method succeeds                        | `ContextData` used to refresh the context |
-| `Publish` | `Context.publish()` method succeeds                        | `PublishEvent` sent to the A/B Smartly event collector |
-| `Exposure` | `Context.getTreatment()` method succeeds on first exposure | `Exposure` enqueued for publishing |
-| `Goal` | `Context.track()` method succeeds                          | `GoalAchievement` enqueued for publishing |
-| `Close` | `Context.close()` method succeeds the first time           | `null` |
 
-
-#### Peek at treatment variants
-Although generally not recommended, it is sometimes necessary to peek at a treatment or variable without triggering an exposure.
-The A/B Smartly SDK provides a `peek_treament()` method for that.
+If you are running multiple experiments and need to choose different
+custom assignments for each one, you can do so using the
+`set_custom_assignments()` method.
 
 ```python
- res = context.peek_treamnet("exp_test_experiment")
-if res == 0:
-	# user is in control group (variant 0)
-else:
-	# user is in treatment group
+    context.set_custom_assignments({"db_user_id2": 1})
+```
 
+### Publish
+Sometimes it is necessary to ensure all events have been published to the A/B Smartly collector, before proceeding.
+You can explicitly call the `publish()` or `publish_async()` methods.
+```python
+    context.publish()
 ```
 
-##### Peeking at variables
+### Finalize
+The `close()` and `close_async()` methods will ensure all events have been published to the A/B Smartly collector, like `publish()`, and will also "seal" the context, throwing an error if any method that could generate an event is called.
 ```python
-variable = context.peek_variable("my_variable")
+    context.close()
 ```
 
-#### Overriding treatment variants
-During development, for example, it is useful to force a treatment for an experiment. This can be achieved with the `override()` and/or `overrides()` methods.
-The `set_override()` and `set_overrides()` methods can be called before the context is ready.
+### Tracking Goals
+Goals are created in the A/B Smartly web console.
 ```python
-context.set_override("exp_test_experiment", 1) # force variant 1 of treatment
-context.set_overrides({
-	"exp_test_experiment": 1,
-	"exp_another_experiment": 0
-})
+    context.track("payment", {
+            "item_count": 1,
+            "total_amount": 1999.99
+    })
 ```
 
 ## About A/B Smartly
 **A/B Smartly** is the leading provider of state-of-the-art, on-premises, full-stack experimentation platforms for engineering and product teams that want to confidently deploy features as fast as they can develop them.
 A/B Smartly's real-time analytics helps engineering and product teams ensure that new features will improve the customer experience without breaking or degrading performance and/or business metrics.
 
 ### Have a look at our growing list of clients and SDKs:
 - [Java SDK](https://www.github.com/absmartly/java-sdk)
 - [JavaScript SDK](https://www.github.com/absmartly/javascript-sdk)
 - [PHP SDK](https://www.github.com/absmartly/php-sdk)
 - [Swift SDK](https://www.github.com/absmartly/swift-sdk)
 - [Vue2 SDK](https://www.github.com/absmartly/vue2-sdk)
 - [Go SDK](https://www.github.com/absmartly/go-sdk)
-- [Ruby SDK](https://www.github.com/absmartly/ruby-sdk)
+- [Ruby SDK](https://www.github.com/absmartly/ruby-sdk)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ABSmartly-0.1.3/ABSmartly.egg-info/SOURCES.txt` & `ABSmartly-0.1.4/ABSmartly.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 LICENSE
 MANIFEST.in
-README.MD
+README.md
 pyproject.toml
-setup.py
 ABSmartly.egg-info/PKG-INFO
 ABSmartly.egg-info/SOURCES.txt
 ABSmartly.egg-info/dependency_links.txt
 ABSmartly.egg-info/requires.txt
 ABSmartly.egg-info/top_level.txt
-absmartly.egg-info/PKG-INFO
-absmartly.egg-info/SOURCES.txt
-absmartly.egg-info/dependency_links.txt
-absmartly.egg-info/requires.txt
-absmartly.egg-info/top_level.txt
 sdk/__init__.py
-sdk/absmarly.py
+sdk/absmartly.py
 sdk/absmartly_config.py
 sdk/audience_deserializer.py
 sdk/audience_matcher.py
 sdk/client.py
 sdk/client_config.py
 sdk/context.py
 sdk/context_config.py
```

### Comparing `ABSmartly-0.1.3/LICENSE` & `ABSmartly-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/PKG-INFO` & `ABSmartly-0.1.4/ABSmartly.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: ABSmartly
-Version: 0.1.3
+Version: 0.1.4
 Summary: ABSmartly Python SDK lib
-Home-page: https://github.com/absmartly/python-sdk
-Author: ABSmartly
 Author-email: ABSmartly <info@ABSmartly.com>
 License: The MIT License (MIT)
         Copyright © 2022 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -28,215 +26,267 @@
 A/B Smartly - Python SDK
 
 ## Compatibility
 
 The A/B Smartly Python SDK is compatible with Python 3.
 It provides both a blocking and an asynchronous interfaces.
 
+## Getting Started
 
-## Installation
-pip install absmartly==0.1.2
+### Install the SDK
+ ```bash
+ pip install absmartly==0.1.2
+ ```
 
-### Python Modules
+### Dependencies
+```
 setuptools~=60.2.0  
 requests~=2.28.1  
 urllib3~=1.26.12  
 jsons~=1.6.3
+```
 
-### Dependencies
-sh ./run.sh
 
-## Getting Started
 
-Please follow the [installation](#installation) instructions before trying the following code:
+## Import and Initialize the SDK
 
-#### Initialization
-This example assumes an Api Key, an Application, and an Environment have been created in the A/B Smartly web console.
+Once the SDK is installed, it can be initialized in your project.
 ```python
+    def main():
+        client_config = ClientConfig()
+        client_config.endpoint = "https://sandbox.test.io/v1"
+        client_config.api_key = "test"
+        client_config.application = "www"
+        client_config.environment = "prod"
+    
+        default_client_config = DefaultHTTPClientConfig()
+        default_client = DefaultHTTPClient(default_client_config)
+        sdk_config = ABSmartlyConfig()
+        sdk_config.client = Client(client_config, default_client)
+        sdk = ABSmartly(sdk_config)
+    
+        context_config = ContextConfig()
+        ctx = sdk.create_context(context_config)
+```
+
+**SDK Options**
+
+| Config      | Type                                          | Required? |                 Default                 | Description                                                                                                                                                                   |
+| :---------- |:----------------------------------------------| :-------: |:---------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| endpoint    | `string`                                      |  &#9989;  |               `undefined`               | The URL to your API endpoint. Most commonly `"your-company.absmartly.io"`                                                                                                     |
+| apiKey      | `string`                                      |  &#9989;  |               `undefined`               | Your API key which can be found on the Web Console.                                                                                                                           |
+| environment | `"production"` or `"development"`             |  &#9989;  |               `undefined`               | The environment of the platform where the SDK is installed. Environments are created on the Web Console and should match the available environments in your infrastructure.   |
+| application | `string`                                      |  &#9989;  |               `undefined`               | The name of the application where the SDK is installed. Applications are created on the Web Console and should match the applications where your experiments will be running. |
+| max_retries     | `number`                                      | &#10060;  |                   `5`                   | The number of retries before the SDK stops trying to connect.                                                                                                                 |
+| connection_timeout     | `number`                                      | &#10060;  |                   `3`                   | An amount of time, in seconds, before the SDK will stop trying to connect.                                                                                                    |
+| context_event_logger | `(self, event_type: EventType, data: object)` | &#10060;  | See "Using a Custom Event Logger" below | A callback function which runs after SDK events.                                                                                                                              
 
-def main():
-    client_config = ClientConfig()
-    client_config.endpoint = "https://sandbox.test.io/v1"
-    client_config.api_key = "test"
-    client_config.application = "www"
-    client_config.environment = "prod"
+#### Using a custom Event Logger
+The A/B Smartly SDK can be instantiated with an event logger used for all contexts.
+In addition, an event logger can be specified when creating a particular context, in the `ContextConfig`.
+```python
+    class EventType(Enum):
+        ERROR = "error"
+        READY = "ready"
+        REFRESH = "refresh"
+        PUBLISH = "publish"
+        EXPOSURE = "exposure"
+        GOAL = "goal"
+        CLOSE = "close"
+    
+    
+    class ContextEventLogger:
+    
+        @abstractmethod
+        def handle_event(self, event_type: EventType, data: object):
+            raise NotImplementedError
+```
+The data parameter depends on the type of event.
+Currently, the SDK logs the following events:
 
-    default_client_config = DefaultHTTPClientConfig()
-    default_client = DefaultHTTPClient(default_client_config)
-    sdk_config = ABSmartlyConfig()
-    sdk_config.client = Client(client_config, default_client)
-    sdk = ABSmartly(sdk_config)
+| event | when                                                       | data |
+|:---: |------------------------------------------------------------|---|
+| `Error` | `Context` receives an error                                | `Throwable` object |
+| `Ready` | `Context` turns ready                                      | `ContextData` used to initialize the context |
+| `Refresh` | `Context.refresh()` method succeeds                        | `ContextData` used to refresh the context |
+| `Publish` | `Context.publish()` method succeeds                        | `PublishEvent` sent to the A/B Smartly event collector |
+| `Exposure` | `Context.getTreatment()` method succeeds on first exposure | `Exposure` enqueued for publishing |
+| `Goal` | `Context.track()` method succeeds                          | `GoalAchievement` enqueued for publishing |
+| `Close` | `Context.close()` method succeeds the first time           | `null` |
 
+
+## Create a New Context Request
+
+**Synchronously**
+```python
+# define a new context request
     context_config = ContextConfig()
-    ctx = sdk.create_context(context_config)
+    context_config.publish_delay = 10
+    context_config.refresh_interval = 5
 
-   # ...
-}
+    context_config = ContextConfig()
+    ctx = sdk.create_context(context_config)
+    ctx.wait_until_ready()
 ```
 
-#### Creating a new Context synchronously
+**Asynchronously**
 ```python
 # define a new context request
     context_config = ContextConfig()
     context_config.publish_delay = 10
     context_config.refresh_interval = 5
-    context_config.units = {"session_id": "bf06d8cb5d8137290c4abb64155584fbdb64d8",
-                            "user_id": "12345"}
 
     context_config = ContextConfig()
     ctx = sdk.create_context(context_config)
-    ctx.wait_until_ready()
+    ctx.wait_until_ready_async()
 ```
 
-#### Creating a new Context asynchronously
+**With Prefetched Data**
 ```python
 # define a new context request
     context_config = ContextConfig()
     context_config.publish_delay = 10
     context_config.refresh_interval = 5
     context_config.units = {"session_id": "bf06d8cb5d8137290c4abb64155584fbdb64d8",
                             "user_id": "12345"}
-
+    
     context_config = ContextConfig()
     ctx = sdk.create_context(context_config)
     ctx.wait_until_ready_async()
 ```
 
-#### Setting extra units for a context
+**Refreshing the Context with Fresh Experiment Data**
+For long-running contexts, the context is usually created once when the application is first started.
+However, any experiments being tracked in your production code, but started after the context was created, will not be triggered.
+To mitigate this, we can use the `set_refresh_interval()` method on the context config.
+
+```python
+    default_client_config = DefaultHTTPClientConfig()
+    default_client_config.refresh_interval = 5
+```
+
+Alternatively, the `refresh()` method can be called manually.
+The `refresh()` method pulls updated experiment data from the A/B Smartly collector and will trigger recently started experiments when `get_treatment()` is called again.
+```python
+    context.refresh()
+```
+
+**Setting Extra Units**
 You can add additional units to a context by calling the `set_unit()` or the `set_units()` method.
 This method may be used for example, when a user logs in to your application, and you want to use the new unit type to the context.
 Please note that **you cannot override an already set unit type** as that would be a change of identity, and will throw an exception. In this case, you must create a new context instead.
 The `SetUnit()` and `SetUnits()` methods can be called before the context is ready.
 
 ```python
-context.set_unit("db_user_id", "1000013")
-
-context.set_units({
-		"db_user_id": "1000013"
-})
+    context.set_unit("db_user_id", "1000013")
+    
+    context.set_units({
+            "db_user_id": "1000013"
+    })
 ```
 
-#### Setting context attributes
-The `set_attributes()` and `set_attributes()` methods can be called before the context is ready.
-```python
-context.set_attributes("user_agent", req.get_header("User-Agent"))
-
-context.set_attributes({
-        "customer_age": "new_customer"
-})
-```
+## Basic Usage
 
 #### Selecting a treatment
 ```python
-res, _ = context.get_treatment("exp_test_experiment")
-if res == 0:
-        # user is in control group (variant 0)
-else:
-       # user is in treatment group
+    res, _ = context.get_treatment("exp_test_experiment")
+    if res == 0:
+            # user is in control group (variant 0)
+    else:
+           # user is in treatment group
 ```
 
-#### Tracking a goal achievement
-Goals are created in the A/B Smartly web console.
+### Treatment Variables
+
 ```python
-context.track("payment", {
-        "item_count": 1,
-        "total_amount": 1999.99
-})
+     res = context.get_variable_value(key, 17)
 ```
 
-#### Publishing pending data
-Sometimes it is necessary to ensure all events have been published to the A/B Smartly collector, before proceeding.
-You can explicitly call the `publish()` or `publish_async()` methods.
+
+#### Peek at treatment variants
+Although generally not recommended, it is sometimes necessary to peek at a treatment or variable without triggering an exposure.
+The A/B Smartly SDK provides a `peek_treament()` method for that.
+
 ```python
-    context.publish()
-```
+    res = context.peek_treament("exp_test_experiment")
+    if res == 0:
+        # user is in control group (variant 0)
+    else:
+        # user is in treatment group
 
-#### Finalizing
-The `close()` and `close_async()` methods will ensure all events have been published to the A/B Smartly collector, like `publish()`, and will also "seal" the context, throwing an error if any method that could generate an event is called.
+```
+##### Peeking at variables
 ```python
-context.close()
+    variable = context.peek_variable("my_variable")
 ```
 
-#### Refreshing the context with fresh experiment data
-For long-running contexts, the context is usually created once when the application is first started.
-However, any experiments being tracked in your production code, but started after the context was created, will not be triggered.
-To mitigate this, we can use the `set_refresh_interval()` method on the context config.
-
+#### Overriding treatment variants
+During development, for example, it is useful to force a treatment for an experiment. This can be achieved with the `override()` and/or `overrides()` methods.
+The `set_override()` and `set_overrides()` methods can be called before the context is ready.
 ```python
-    default_client_config = DefaultHTTPClientConfig()
-    default_client_config.refresh_interval = 5
+    context.set_override("exp_test_experiment", 1) # force variant 1 of treatment
+    context.set_overrides({
+        "exp_test_experiment": 1,
+        "exp_another_experiment": 0
+    })
 ```
 
-Alternatively, the `refresh()` method can be called manually.
-The `refresh()` method pulls updated experiment data from the A/B Smartly collector and will trigger recently started experiments when `get_treatment()` is called again.
+## Advanced
+
+### Context Attributes
+Attributes are used to pass meta-data about the user and/or the request.
+They can be used later in the Web Console to create segments or audiences.
+The `set_attributes()` and `set_attributes()` methods can be called before the context is ready.
 ```python
-context.refresh()
+    context.set_attributes("user_agent", req.get_header("User-Agent"))
+    
+    context.set_attributes({
+            "customer_age": "new_customer"
+    })
 ```
 
-#### Using a custom Event Logger
-The A/B Smartly SDK can be instantiated with an event logger used for all contexts.
-In addition, an event logger can be specified when creating a particular context, in the `ContextConfig`.
-```python
-class EventType(Enum):
-    ERROR = "error"
-    READY = "ready"
-    REFRESH = "refresh"
-    PUBLISH = "publish"
-    EXPOSURE = "exposure"
-    GOAL = "goal"
-    CLOSE = "close"
+### Custom Assignments
 
+Sometimes it may be necessary to override the automatic selection of a
+variant. For example, if you wish to have your variant chosen based on
+data from an API call. This can be accomplished using the
+`set_custom_assignment()` method.
 
-class ContextEventLogger:
-
-    @abstractmethod
-    def handle_event(self, event_type: EventType, data: object):
-        raise NotImplementedError
+```python
+    context.set_custom_assignment("exp_test_not_eligible", 3)
 ```
-The data parameter depends on the type of event.
-Currently, the SDK logs the following events:
-
-| event | when                                                       | data |
-|:---: |------------------------------------------------------------|---|
-| `Error` | `Context` receives an error                                | `Throwable` object |
-| `Ready` | `Context` turns ready                                      | `ContextData` used to initialize the context |
-| `Refresh` | `Context.refresh()` method succeeds                        | `ContextData` used to refresh the context |
-| `Publish` | `Context.publish()` method succeeds                        | `PublishEvent` sent to the A/B Smartly event collector |
-| `Exposure` | `Context.getTreatment()` method succeeds on first exposure | `Exposure` enqueued for publishing |
-| `Goal` | `Context.track()` method succeeds                          | `GoalAchievement` enqueued for publishing |
-| `Close` | `Context.close()` method succeeds the first time           | `null` |
 
-
-#### Peek at treatment variants
-Although generally not recommended, it is sometimes necessary to peek at a treatment or variable without triggering an exposure.
-The A/B Smartly SDK provides a `peek_treament()` method for that.
+If you are running multiple experiments and need to choose different
+custom assignments for each one, you can do so using the
+`set_custom_assignments()` method.
 
 ```python
- res = context.peek_treamnet("exp_test_experiment")
-if res == 0:
-	# user is in control group (variant 0)
-else:
-	# user is in treatment group
+    context.set_custom_assignments({"db_user_id2": 1})
+```
 
+### Publish
+Sometimes it is necessary to ensure all events have been published to the A/B Smartly collector, before proceeding.
+You can explicitly call the `publish()` or `publish_async()` methods.
+```python
+    context.publish()
 ```
 
-##### Peeking at variables
+### Finalize
+The `close()` and `close_async()` methods will ensure all events have been published to the A/B Smartly collector, like `publish()`, and will also "seal" the context, throwing an error if any method that could generate an event is called.
 ```python
-variable = context.peek_variable("my_variable")
+    context.close()
 ```
 
-#### Overriding treatment variants
-During development, for example, it is useful to force a treatment for an experiment. This can be achieved with the `override()` and/or `overrides()` methods.
-The `set_override()` and `set_overrides()` methods can be called before the context is ready.
+### Tracking Goals
+Goals are created in the A/B Smartly web console.
 ```python
-context.set_override("exp_test_experiment", 1) # force variant 1 of treatment
-context.set_overrides({
-	"exp_test_experiment": 1,
-	"exp_another_experiment": 0
-})
+    context.track("payment", {
+            "item_count": 1,
+            "total_amount": 1999.99
+    })
 ```
 
 ## About A/B Smartly
 **A/B Smartly** is the leading provider of state-of-the-art, on-premises, full-stack experimentation platforms for engineering and product teams that want to confidently deploy features as fast as they can develop them.
 A/B Smartly's real-time analytics helps engineering and product teams ensure that new features will improve the customer experience without breaking or degrading performance and/or business metrics.
 
 ### Have a look at our growing list of clients and SDKs:
```

### Comparing `ABSmartly-0.1.3/pyproject.toml` & `ABSmartly-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ABSmartly"
-version = "0.1.3"
+version = "0.1.4"
 description = "ABSmartly Python SDK lib"
-readme = "README.MD"
+readme = "README.md"
 authors = [{ name = "ABSmartly", email = "info@ABSmartly.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
```

### Comparing `ABSmartly-0.1.3/sdk/absmarly.py` & `ABSmartly-0.1.4/sdk/absmartly.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/absmartly_config.py` & `ABSmartly-0.1.4/sdk/absmartly_config.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/audience_matcher.py` & `ABSmartly-0.1.4/sdk/audience_matcher.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/client.py` & `ABSmartly-0.1.4/sdk/client.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/client_config.py` & `ABSmartly-0.1.4/sdk/client_config.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/context.py` & `ABSmartly-0.1.4/sdk/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,25 +231,25 @@
             self.data = data
 
             self.set_refresh_timer()
         finally:
             self.data_lock.release_write()
 
     def set_refresh_timer(self):
-        if self.refresh_interval > 0 and self.refresh_timer is None:
-            def refresh():
+        if self.refresh_interval > 0 and self.refresh_timer is None and not self.is_closing() and not self.is_closed():
+            def ref():
                 self.refresh_async()
                 self.refresh_timer = threading.Timer(
                     self.refresh_interval,
-                    refresh)
+                    ref)
                 self.refresh_timer.start()
 
             self.refresh_timer = threading.Timer(
                 self.refresh_interval,
-                refresh)
+                ref)
             self.refresh_timer.start()
 
     def set_timeout(self):
         if self.is_ready():
             if self.timeout is None:
                 try:
                     self.timeout_lock.acquire_write()
```

### Comparing `ABSmartly-0.1.3/sdk/default_context_data_deserializer.py` & `ABSmartly-0.1.4/sdk/default_context_data_deserializer.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/default_context_event_handler.py` & `ABSmartly-0.1.4/sdk/default_context_event_handler.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/default_http_client.py` & `ABSmartly-0.1.4/sdk/default_http_client.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/http_client.py` & `ABSmartly-0.1.4/sdk/http_client.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/internal/buffers.py` & `ABSmartly-0.1.4/sdk/internal/buffers.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/internal/lock/concurrency.py` & `ABSmartly-0.1.4/sdk/internal/lock/concurrency.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/internal/lock/read_write_lock.py` & `ABSmartly-0.1.4/sdk/internal/lock/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/internal/murmur32.py` & `ABSmartly-0.1.4/sdk/internal/murmur32.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/internal/variant_assigner.py` & `ABSmartly-0.1.4/sdk/internal/variant_assigner.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/json/experiment.py` & `ABSmartly-0.1.4/sdk/json/experiment.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/jsonexpr/evaluator.py` & `ABSmartly-0.1.4/sdk/jsonexpr/evaluator.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/jsonexpr/expr_evaluator.py` & `ABSmartly-0.1.4/sdk/jsonexpr/expr_evaluator.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/jsonexpr/json_expr.py` & `ABSmartly-0.1.4/sdk/jsonexpr/json_expr.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/jsonexpr/operators/binary_operator.py` & `ABSmartly-0.1.4/sdk/jsonexpr/operators/binary_operator.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/sdk/jsonexpr/operators/in_operator.py` & `ABSmartly-0.1.4/sdk/jsonexpr/operators/in_operator.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/test/test_buffers.py` & `ABSmartly-0.1.4/test/test_buffers.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/test/test_client.py` & `ABSmartly-0.1.4/test/test_client.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/test/test_context.py` & `ABSmartly-0.1.4/test/test_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import threading
 import time
+import typing
 import unittest
 from concurrent.futures import Future
 
 from sdk.context_config import ContextConfig
 
 from sdk.context import Context
 
@@ -16,15 +17,15 @@
 
 from sdk.audience_matcher import AudienceMatcher
 from sdk.default_http_client import DefaultHTTPClient
 from sdk.default_http_client_config import DefaultHTTPClientConfig
 
 from sdk.default_variable_parser import DefaultVariableParser
 
-from sdk.context_event_logger import ContextEventLogger
+from sdk.context_event_logger import ContextEventLogger, EventType
 
 from sdk.context_event_handler import ContextEventHandler
 
 from sdk.context_data_provider import ContextDataProvider
 
 from sdk.default_audience_deserializer import DefaultAudienceDeserializer
 
@@ -36,14 +37,23 @@
 from sdk.json.goal_achievement import GoalAchievement
 from sdk.json.publish_event import PublishEvent
 from sdk.json.unit import Unit
 from sdk.time.clock import Clock
 from sdk.time.fixed_clock import FixedClock
 
 
+class ContextEventLoggerTest(ContextEventLogger):
+    logger_data: typing.Optional[object] = None
+    logger_type: typing.Optional[EventType] = None
+
+    def handle_event(self, event_type: EventType, data: object):
+        self.logger_data = data
+        self.logger_type = event_type
+
+
 class ClientContextMock(Client):
     def get_context_data(self):
         future = Future()
         context_data = ContextData()
         context_data.experiments = []
         future.set_result(context_data)
         return future
@@ -105,15 +115,15 @@
     data_future_strict: Future
     data_future_refresh: Future
     data_future_ready: Future
     data_future_failed: Future
     clock: Clock
     data_provider: ContextDataProvider
     event_handler: ContextEventHandler
-    event_logger: ContextEventLogger = None
+    event_logger: ContextEventLogger = ContextEventLoggerTest()
     variable_parser: DefaultVariableParser
     audience_matcher: AudienceMatcher
 
     def set_up(self):
         with open(os.path.join(os.path.dirname(__file__),
                                'res/context.json'),
                   'r') as file:
@@ -999,7 +1009,66 @@
         self.assertEqual("exp_test_ab", res[0])
         self.assertEqual("exp_test_fullon", res[3])
         self.assertEqual(4, len(res))
         res = context.get_treatment("exp_test_fullon")
         self.assertEqual(2, res)
         self.assertEqual(2, context.get_pending_count())
         context.close()
+
+    def test_logger_called(self):
+        self.event_logger.logger_data = None
+        self.event_logger.logger_type = None
+        self.assertIsNone(self.event_logger.logger_data)
+        self.assertIsNone(self.event_logger.logger_type)
+
+        self.set_up()
+        config = ContextConfig()
+        config.units = self.units
+        context = self.create_test_context(config, self.data_future_ready)
+        self.assertEqual(self.event_logger.logger_type, EventType.READY)
+        self.assertEqual(type(self.event_logger.logger_data),
+                         type(ContextData()))
+        self.assertEqual(True, context.is_ready())
+
+        res = context.get_treatment("exp_test_new")
+        self.assertEqual(0, res)
+        self.assertEqual(1, context.get_pending_count())
+        self.assertEqual(self.event_logger.logger_type, EventType.EXPOSURE)
+        self.assertEqual(type(self.event_logger.logger_data),
+                         type(Exposure()))
+
+        def sl():
+            future = Future()
+
+            def set_result():
+                future.set_result(self.data)
+            th = threading.Thread(target=set_result)
+            th.start()
+            return future
+        self.client.get_context_data = sl
+        self.assertEqual(self.event_logger.logger_type, EventType.EXPOSURE)
+        self.assertEqual(type(self.event_logger.logger_data),
+                         type(Exposure()))
+
+        context.refresh()
+        self.assertEqual(self.event_logger.logger_type, EventType.REFRESH)
+        self.assertEqual(type(self.event_logger.logger_data),
+                         type(ContextData()))
+        res = context.get_experiments()
+        self.assertEqual(self.event_logger.logger_type, EventType.REFRESH)
+        self.assertEqual(type(self.event_logger.logger_data),
+                         type(ContextData()))
+        self.assertEqual("exp_test_ab", res[0])
+        self.assertEqual("exp_test_fullon", res[3])
+        self.assertEqual(4, len(res))
+        res = context.get_treatment("exp_test_fullon")
+        self.assertEqual(self.event_logger.logger_type, EventType.EXPOSURE)
+        self.assertEqual(type(self.event_logger.logger_data),
+                         type(Exposure()))
+        self.assertEqual(2, res)
+        self.assertEqual(2, context.get_pending_count())
+        self.assertEqual(self.event_logger.logger_type, EventType.EXPOSURE)
+        self.assertEqual(type(self.event_logger.logger_data),
+                         type(Exposure()))
+        context.close()
+        self.assertEqual(self.event_logger.logger_type, EventType.CLOSE)
+        self.assertIsNone(self.event_logger.logger_data)
```

### Comparing `ABSmartly-0.1.3/test/test_default_audience_deserializer.py` & `ABSmartly-0.1.4/test/test_default_audience_deserializer.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/test/test_default_context_data_deserializer.py` & `ABSmartly-0.1.4/test/test_default_context_data_deserializer.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/test/test_default_context_event_serializer.py` & `ABSmartly-0.1.4/test/test_default_context_event_serializer.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/test/test_murmur32.py` & `ABSmartly-0.1.4/test/test_murmur32.py`

 * *Files identical despite different names*

### Comparing `ABSmartly-0.1.3/test/test_variant_assigner.py` & `ABSmartly-0.1.4/test/test_variant_assigner.py`

 * *Files identical despite different names*

