# Comparing `tmp/openedx-events-7.0.0.tar.gz` & `tmp/openedx-events-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-events-7.0.0.tar", last modified: Thu Mar  9 14:12:28 2023, max compression
+gzip compressed data, was "openedx-events-7.1.0.tar", last modified: Wed May  3 20:27:10 2023, max compression
```

## Comparing `openedx-events-7.0.0.tar` & `openedx-events-7.1.0.tar`

### file list

```diff
@@ -1,55 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 14:12:28.764934 openedx-events-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     8073 2023-03-09 14:12:20.000000 openedx-events-7.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-03-09 14:12:20.000000 openedx-events-7.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-03-09 14:12:20.000000 openedx-events-7.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14099 2023-03-09 14:12:28.764934 openedx-events-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5366 2023-03-09 14:12:20.000000 openedx-events-7.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 14:12:28.756934 openedx-events-7.0.0/openedx_events/
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 14:12:28.760934 openedx-events-7.0.0/openedx_events/content_authoring/
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/content_authoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/content_authoring/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/content_authoring/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 14:12:28.760934 openedx-events-7.0.0/openedx_events/event_bus/
--rw-r--r--   0 runner    (1001) docker     (122)     5065 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 14:12:28.760934 openedx-events-7.0.0/openedx_events/event_bus/avro/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/avro/custom_serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/avro/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5313 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/avro/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/avro/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 14:12:28.764934 openedx-events-7.0.0/openedx_events/event_bus/avro/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/avro/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4973 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/avro/tests/test_avro.py
--rw-r--r--   0 runner    (1001) docker     (122)    11016 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/avro/tests/test_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11200 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/avro/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     8761 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/avro/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3632 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/avro/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/avro/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 14:12:28.764934 openedx-events-7.0.0/openedx_events/event_bus/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/event_bus/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 14:12:28.764934 openedx-events-7.0.0/openedx_events/learning/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8297 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/learning/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5660 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/learning/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 14:12:28.764934 openedx-events-7.0.0/openedx_events/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9959 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-03-09 14:12:20.000000 openedx-events-7.0.0/openedx_events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 14:12:28.760934 openedx-events-7.0.0/openedx_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14099 2023-03-09 14:12:28.000000 openedx-events-7.0.0/openedx_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-03-09 14:12:28.000000 openedx-events-7.0.0/openedx_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-09 14:12:28.000000 openedx-events-7.0.0/openedx_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-09 14:12:28.000000 openedx-events-7.0.0/openedx_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-03-09 14:12:28.000000 openedx-events-7.0.0/openedx_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-03-09 14:12:28.000000 openedx-events-7.0.0/openedx_events.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 14:12:28.764934 openedx-events-7.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-03-09 14:12:20.000000 openedx-events-7.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-03-09 14:12:28.764934 openedx-events-7.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-03-09 14:12:20.000000 openedx-events-7.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 14:12:28.764934 openedx-events-7.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-03-09 14:12:20.000000 openedx-events-7.0.0/tests/test_openedx_events.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     8479 2023-05-03 20:27:05.000000 openedx-events-7.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-03 20:27:05.000000 openedx-events-7.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-05-03 20:27:05.000000 openedx-events-7.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14505 2023-05-03 20:27:10.093215 openedx-events-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5366 2023-05-03 20:27:05.000000 openedx-events-7.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.089215 openedx-events-7.1.0/openedx_events/
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.089215 openedx-events-7.1.0/openedx_events/content_authoring/
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/content_authoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/content_authoring/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/content_authoring/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.089215 openedx-events-7.1.0/openedx_events/event_bus/
+-rw-r--r--   0 runner    (1001) docker     (122)     7344 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.089215 openedx-events-7.1.0/openedx_events/event_bus/avro/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/custom_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5313 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4973 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_avro.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11016 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11200 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8761 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3632 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/openedx_events/event_bus/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/openedx_events/learning/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8297 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5664 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/learning/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/openedx_events/management/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/openedx_events/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2932 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/management/commands/consume_events.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/openedx_events/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2710 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/tests/test_consume_events_command.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9959 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.089215 openedx-events-7.1.0/openedx_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14505 2023-05-03 20:27:10.000000 openedx-events-7.1.0/openedx_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-03 20:27:10.000000 openedx-events-7.1.0/openedx_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 20:27:10.000000 openedx-events-7.1.0/openedx_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 20:27:10.000000 openedx-events-7.1.0/openedx_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-03 20:27:10.000000 openedx-events-7.1.0/openedx_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-03 20:27:10.000000 openedx-events-7.1.0/openedx_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-03 20:27:05.000000 openedx-events-7.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-05-03 20:27:10.093215 openedx-events-7.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-05-03 20:27:05.000000 openedx-events-7.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-03 20:27:05.000000 openedx-events-7.1.0/tests/test_openedx_events.py
```

### Comparing `openedx-events-7.0.0/CHANGELOG.rst` & `openedx-events-7.1.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,28 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+
+[7.1.0] - 2023-05-03
+--------------------
+Added
+~~~~~
+* Configurable loader for consumer side of Event Bus in ``openedx_events.event_bus``.
+* Added management command to load configured consumer and start worker.
+
+Changed
+~~~~~~~
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
+  more details.
+
 [7.0.0] - 2023-03-07
 ---------------------
 Changed
 ~~~~~~~
 * **Breaking change**: Moved serialize_event_data_to_bytes from openedx_events.event_bus.avro.tests.test_utilities to openedx_events.event_bus.avro.serializer
 * **Breaking change**: Moved deserialize_bytes_to_event_data from openedx_events.event_bus.avro.tests.test_utilities to openedx_events.event_bus.avro.deserializer
```

### Comparing `openedx-events-7.0.0/LICENSE.txt` & `openedx-events-7.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/PKG-INFO` & `openedx-events-7.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 7.0.0
+Version: 7.1.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,28 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+
+[7.1.0] - 2023-05-03
+--------------------
+Added
+~~~~~
+* Configurable loader for consumer side of Event Bus in ``openedx_events.event_bus``.
+* Added management command to load configured consumer and start worker.
+
+Changed
+~~~~~~~
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
+  more details.
+
 [7.0.0] - 2023-03-07
 ---------------------
 Changed
 ~~~~~~~
 * **Breaking change**: Moved serialize_event_data_to_bytes from openedx_events.event_bus.avro.tests.test_utilities to openedx_events.event_bus.avro.serializer
 * **Breaking change**: Moved deserialize_bytes_to_event_data from openedx_events.event_bus.avro.tests.test_utilities to openedx_events.event_bus.avro.deserializer
```

### Comparing `openedx-events-7.0.0/README.rst` & `openedx-events-7.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/content_authoring/data.py` & `openedx-events-7.1.0/openedx_events/content_authoring/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/content_authoring/signals.py` & `openedx-events-7.1.0/openedx_events/content_authoring/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/data.py` & `openedx-events-7.1.0/openedx_events/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/event_bus/__init__.py` & `openedx-events-7.1.0/openedx_events/event_bus/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 """
 Classes and utility functions for the event bus.
 
-This module includes the entry point for the producer.
+This module includes the entry points for the producer and consumer.
 
 API:
 
 - ``get_producer`` returns an ``EventBusProducer`` singleton that should be used for sending all events
   to the Event Bus. The backing implementation is chosen via the Django setting ``EVENT_BUS_PRODUCER``.
   See for example the Kafka implementation's ``KafkaEventProducer``, with the ``create_producer`` function
   serving as the loader: https://github.com/openedx/event-bus-kafka/blob/main/edx_event_bus_kafka/internal/producer.py
+- ``make_single_consumer`` creates an ``EventBusConsumer`` instance for a particular combination of
+  topic, consumer group, and signal. The backing implementation is chosen via the Django setting
+  ``EVENT_BUS_CONSUMER``.
 """
 
 import warnings
 from abc import ABC, abstractmethod
 from functools import lru_cache
-from typing import NoReturn, Optional
 
 from django.conf import settings
 from django.dispatch import receiver
 from django.test.signals import setting_changed
 from django.utils.module_loading import import_string
 
 from openedx_events.data import EventsMetadata
 from openedx_events.tooling import OpenEdxPublicSignal
 
 
-def _try_load(*, setting_name: str, expected_class: type, default):
+def _try_load(*, setting_name: str, args: tuple, kwargs: dict, expected_class: type, default):
     """
     Load an instance of ``expected_class`` as indicated by ``setting_name``.
 
     The setting points to a callable (function or class) that will fetch or create an
     instance of the expected class. If the configuration is missing or invalid,
     or the callable throws an exception or returns the wrong type, the default is
     returned instead.
 
     Arguments:
         setting_name: Name of a Django setting containing a dotted module path, indicating a callable
+        args: Tuple of positional arguments to pass to the callable
+        kwargs: Dictionary of keyword arguments to pass to the callable
         expected_class: The callable must produce an instance of this class object (or a subclass)
         default: Object to return if any part of the lookup or loading fails
     """
     constructor_path = getattr(settings, setting_name, None)
     if constructor_path is None:
         warnings.warn(f"Event Bus setting {setting_name} is missing; component will be inactive")
         return default
 
     try:
         constructor = import_string(constructor_path)
-        instance = constructor()
+        instance = constructor(*args, **kwargs)
         if isinstance(instance, expected_class):
             return instance
         else:
             warnings.warn(
                 f"{constructor_path} from {setting_name} returned unexpected type {type(instance)}; "
                 "component will be inactive"
             )
@@ -64,15 +68,14 @@
 
 
 class EventBusProducer(ABC):
     """
     Parent class for event bus producer implementations.
     """
 
-    # TODO: Make event_metadata required (https://github.com/openedx/openedx-events/issues/153)
     @abstractmethod
     def send(
             self, *, signal: OpenEdxPublicSignal, topic: str, event_key_field: str, event_data: dict,
             event_metadata: EventsMetadata
     ) -> None:
         """
         Send a signal event to the event bus under the specified topic.
@@ -112,16 +115,72 @@
 def get_producer() -> EventBusProducer:
     """
     Create or retrieve the producer implementation, as configured.
 
     If misconfigured, returns a fake implementation that can be called but does nothing.
     """
     return _try_load(
-        setting_name='EVENT_BUS_PRODUCER',
+        setting_name='EVENT_BUS_PRODUCER', args=(), kwargs={},
         expected_class=EventBusProducer, default=NoEventBusProducer(),
     )
 
 
+class EventBusConsumer(ABC):
+    """
+    Parent class for event bus consumer implementations.
+    """
+
+    @abstractmethod
+    def consume_indefinitely(self) -> None:
+        """
+        Consume events from a topic in an infinite loop.
+
+        Events will be converted into calls to Django signals.
+        """
+
+
+class NoEventBusConsumer(EventBusConsumer):
+    """
+    Stub implementation to "load" when no implementation is properly configured.
+    """
+
+    def consume_indefinitely(self) -> None:
+        """Do nothing."""
+
+
+# .. setting_name: EVENT_BUS_CONSUMER
+# .. setting_default: None
+# .. setting_description: String naming a callable (function or class) that can be called to create
+#   or retrieve an instance of EventBusConsumer when ``openedx_events.event_bus.make_single_consumer`` is
+#   called. The format of the string is a dotted path to an attribute in a module, e.g.
+#   ``some.module.path.EventBusImplementation``. See docstring of ``make_single_consumer`` for
+#   parameters. If setting is not supplied or the callable raises an exception or does not return
+#   an instance of EventBusConsumer, calls to the consumer will be ignored with a warning at startup.
+
+
+def make_single_consumer(*, topic: str, group_id: str, signal: OpenEdxPublicSignal, **kwargs) -> EventBusConsumer:
+    """
+    Construct a consumer for a given topic, group, and signal.
+
+    If misconfigured, returns a fake implementation that does nothing.
+
+    Arguments:
+        topic: The event bus topic to consume from (without any environmental prefix)
+        group_id: The consumer group to participate in
+        signal: Send consumed, decoded events to the receivers of this signal
+    """
+    options = {
+        'topic': topic,
+        'group_id': group_id,
+        'signal': signal,
+        **kwargs,
+    }
+    return _try_load(
+        setting_name='EVENT_BUS_CONSUMER', args=(), kwargs=options,
+        expected_class=EventBusConsumer, default=NoEventBusConsumer(),
+    )
+
+
 @receiver(setting_changed)
 def _reset_state(sender, **kwargs):  # pylint: disable=unused-argument
     """Reset caches when settings change during unit tests."""
     get_producer.cache_clear()
```

### Comparing `openedx-events-7.0.0/openedx_events/event_bus/avro/custom_serializers.py` & `openedx-events-7.1.0/openedx_events/event_bus/avro/custom_serializers.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/event_bus/avro/deserializer.py` & `openedx-events-7.1.0/openedx_events/event_bus/avro/deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/event_bus/avro/schema.py` & `openedx-events-7.1.0/openedx_events/event_bus/avro/schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/event_bus/avro/serializer.py` & `openedx-events-7.1.0/openedx_events/event_bus/avro/serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/event_bus/avro/tests/test_avro.py` & `openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_avro.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/event_bus/avro/tests/test_deserializer.py` & `openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/event_bus/avro/tests/test_schema.py` & `openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/event_bus/avro/tests/test_serializer.py` & `openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/event_bus/avro/tests/test_utilities.py` & `openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/event_bus/tests/test_loader.py` & `openedx-events-7.1.0/openedx_events/event_bus/tests/test_loader.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import warnings
 from contextlib import contextmanager
 from unittest import TestCase
 
 from django.test import override_settings
 
 from openedx_events.data import EventsMetadata
-from openedx_events.event_bus import _try_load, get_producer
+from openedx_events.event_bus import _try_load, get_producer, make_single_consumer
 from openedx_events.learning.signals import SESSION_LOGIN_COMPLETED
 
 
 @contextmanager
 def assert_warnings(warning_messages: list):
     with warnings.catch_warnings(record=True) as caught_warnings:
         warnings.simplefilter('always')
@@ -26,75 +26,75 @@
     # No, the "constructors" here don't make much sense, but I didn't
     # want to create a bunch of test classes/factory functions, so I'm
     # using built-in functions instead.
 
     def test_unconfigured(self):
         with assert_warnings(["Event Bus setting DOES_NOT_EXIST is missing; component will be inactive"]):
             loaded = _try_load(
-                setting_name="DOES_NOT_EXIST",
+                setting_name="DOES_NOT_EXIST", args=(1), kwargs={'2': 3},
                 expected_class=dict, default={'def': 'ault'},
             )
         assert loaded == {'def': 'ault'}
 
     @override_settings(EB_LOAD_PATH='builtins.dict')
     def test_success(self):
         with assert_warnings([]):
             loaded = _try_load(
-                setting_name="EB_LOAD_PATH",
+                setting_name="EB_LOAD_PATH", args=(), kwargs={'2': 3},
                 expected_class=dict, default={'def': 'ault'},
             )
-        assert loaded == {}
+        assert loaded == {'2': 3}
 
     @override_settings(EB_LOAD_PATH='builtins.list')
     def test_wrong_type(self):
         with assert_warnings([
                 "builtins.list from EB_LOAD_PATH returned unexpected type <class 'list'>; "
                 "component will be inactive"
         ]):
             loaded = _try_load(
-                setting_name="EB_LOAD_PATH",
+                setting_name="EB_LOAD_PATH", args=([1, 2, 3],), kwargs={},
                 expected_class=dict, default={'def': 'ault'},
             )
         assert loaded == {'def': 'ault'}
 
     @override_settings(EB_LOAD_PATH='no_module_here.foo.nope')
     def test_missing_module(self):
         with assert_warnings([
                 "Failed to load <class 'dict'> from setting EB_LOAD_PATH: "
                 "ModuleNotFoundError(\"No module named 'no_module_here'\"); "
                 "component will be inactive"
         ]):
             loaded = _try_load(
-                setting_name="EB_LOAD_PATH",
+                setting_name="EB_LOAD_PATH", args=(1), kwargs={'2': 3},
                 expected_class=dict, default={'def': 'ault'},
             )
         assert loaded == {'def': 'ault'}
 
     @override_settings(EB_LOAD_PATH='builtins.does_not_exist')
     def test_missing_attribute(self):
         with assert_warnings([
                 "Failed to load <class 'dict'> from setting EB_LOAD_PATH: "
                 "ImportError('Module \"builtins\" does not define a \"does_not_exist\" attribute/class'); "
                 "component will be inactive"
         ]):
             loaded = _try_load(
-                setting_name="EB_LOAD_PATH",
+                setting_name="EB_LOAD_PATH", args=(1), kwargs={'2': 3},
                 expected_class=dict, default={'def': 'ault'},
             )
         assert loaded == {'def': 'ault'}
 
-    @override_settings(EB_LOAD_PATH='builtins.len')
+    @override_settings(EB_LOAD_PATH='builtins.dict')
     def test_bad_args_for_callable(self):
         with assert_warnings([
                 "Failed to load <class 'dict'> from setting EB_LOAD_PATH: "
-                "TypeError('len() takes exactly one argument (0 given)'); "
+                "TypeError('type object argument after * must be an iterable, not int'); "
                 "component will be inactive"
         ]):
             loaded = _try_load(
-                setting_name="EB_LOAD_PATH",
+                setting_name="EB_LOAD_PATH", args=(1), kwargs={'2': 3},
                 expected_class=dict, default={'def': 'ault'},
             )
         assert loaded == {'def': 'ault'}
 
 
 class TestProducer(TestCase):
 
@@ -108,7 +108,21 @@
         with assert_warnings([]):
             # Nothing thrown, no warnings.
             assert producer.send(
                 signal=SESSION_LOGIN_COMPLETED, topic='user-logins',
                 event_key_field='user.id', event_data={},
                 event_metadata=EventsMetadata(event_type='eh')
             ) is None
+
+
+class TestConsumer(TestCase):
+
+    @override_settings(EVENT_BUS_CONSUMER=None)
+    def test_default_does_nothing(self):
+        """
+        Test that the default is of the right class but does nothing.
+        """
+        consumer = make_single_consumer(topic="test", group_id="test", signal=SESSION_LOGIN_COMPLETED)
+
+        with assert_warnings([]):
+            # Nothing thrown, no warnings.
+            assert consumer.consume_indefinitely() is None
```

### Comparing `openedx-events-7.0.0/openedx_events/exceptions.py` & `openedx-events-7.1.0/openedx_events/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/learning/data.py` & `openedx-events-7.1.0/openedx_events/learning/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/learning/signals.py` & `openedx-events-7.1.0/openedx_events/learning/signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     data={
         "enrollment": CourseEnrollmentData,
     }
 )
 
 
 # .. event_type: org.openedx.learning.course.unenrollment.completed.v1
-# .. event_name: COURSE_ENROLLMENT_CHANGED
+# .. event_name: COURSE_UNENROLLMENT_COMPLETED
 # .. event_description: emitted when the user's unenrollment process is completed.
 # .. event_data: CourseEnrollmentData
 COURSE_UNENROLLMENT_COMPLETED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.course.unenrollment.completed.v1",
     data={
         "enrollment": CourseEnrollmentData,
     }
```

### Comparing `openedx-events-7.0.0/openedx_events/tests/test_tooling.py` & `openedx-events-7.1.0/openedx_events/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/tests/utils.py` & `openedx-events-7.1.0/openedx_events/tests/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/tooling.py` & `openedx-events-7.1.0/openedx_events/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events/utils.py` & `openedx-events-7.1.0/openedx_events/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.0.0/openedx_events.egg-info/PKG-INFO` & `openedx-events-7.1.0/openedx_events.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 7.0.0
+Version: 7.1.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,28 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+
+[7.1.0] - 2023-05-03
+--------------------
+Added
+~~~~~
+* Configurable loader for consumer side of Event Bus in ``openedx_events.event_bus``.
+* Added management command to load configured consumer and start worker.
+
+Changed
+~~~~~~~
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
+  more details.
+
 [7.0.0] - 2023-03-07
 ---------------------
 Changed
 ~~~~~~~
 * **Breaking change**: Moved serialize_event_data_to_bytes from openedx_events.event_bus.avro.tests.test_utilities to openedx_events.event_bus.avro.serializer
 * **Breaking change**: Moved deserialize_bytes_to_event_data from openedx_events.event_bus.avro.tests.test_utilities to openedx_events.event_bus.avro.deserializer
```

### Comparing `openedx-events-7.0.0/openedx_events.egg-info/SOURCES.txt` & `openedx-events-7.1.0/openedx_events.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CHANGELOG.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 openedx_events/__init__.py
+openedx_events/apps.py
 openedx_events/data.py
 openedx_events/exceptions.py
 openedx_events/tooling.py
 openedx_events/utils.py
 openedx_events.egg-info/PKG-INFO
 openedx_events.egg-info/SOURCES.txt
 openedx_events.egg-info/dependency_links.txt
@@ -31,12 +32,16 @@
 openedx_events/event_bus/avro/tests/test_schema.py
 openedx_events/event_bus/avro/tests/test_serializer.py
 openedx_events/event_bus/avro/tests/test_utilities.py
 openedx_events/event_bus/tests/test_loader.py
 openedx_events/learning/__init__.py
 openedx_events/learning/data.py
 openedx_events/learning/signals.py
+openedx_events/management/__init__.py
+openedx_events/management/commands/__init__.py
+openedx_events/management/commands/consume_events.py
 openedx_events/tests/__init__.py
+openedx_events/tests/test_consume_events_command.py
 openedx_events/tests/test_tooling.py
 openedx_events/tests/utils.py
 requirements/base.in
 tests/test_openedx_events.py
```

### Comparing `openedx-events-7.0.0/setup.py` & `openedx-events-7.1.0/setup.py`

 * *Files identical despite different names*

