# Comparing `tmp/nitric-0.9.1.dev4.tar.gz` & `tmp/nitric-0.9.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitric-0.9.1.dev4.tar", last modified: Thu Apr  6 00:25:19 2023, max compression
+gzip compressed data, was "nitric-0.9.2.dev3.tar", last modified: Tue Apr 11 04:01:12 2023, max compression
```

## Comparing `nitric-0.9.1.dev4.tar` & `nitric-0.9.2.dev3.tar`

### file list

```diff
@@ -1,78 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.333565 nitric-0.9.1.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-06 00:24:36.000000 nitric-0.9.1.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-06 00:25:19.333565 nitric-0.9.1.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-06 00:24:36.000000 nitric-0.9.1.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    20891 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/api/documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/api/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/api/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/api/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/config/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20531 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/faas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/document/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/document/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/document/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/error/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/error/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/error/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/event/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/event/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/event/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/event/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/faas/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/faas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/faas/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/faas/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/queue/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/queue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/queue/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/queue/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/resource/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/resource/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric/proto/nitric/secret/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.333565 nitric-0.9.1.dev4/nitric/proto/nitric/secret/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/secret/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.333565 nitric-0.9.1.dev4/nitric/proto/nitric/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.333565 nitric-0.9.1.dev4/nitric/proto/nitric/storage/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/nitric/storage/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.333565 nitric-0.9.1.dev4/nitric/proto/validate/
--rw-r--r--   0 runner    (1001) docker     (123)    37084 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/proto/validate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.333565 nitric-0.9.1.dev4/nitric/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/resources/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/resources/buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/resources/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/resources/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/resources/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/resources/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/resources/topics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-06 00:25:16.000000 nitric-0.9.1.dev4/nitric/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:25:19.329565 nitric-0.9.1.dev4/nitric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-06 00:25:19.000000 nitric-0.9.1.dev4/nitric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-06 00:25:19.000000 nitric-0.9.1.dev4/nitric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 00:25:19.000000 nitric-0.9.1.dev4/nitric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-06 00:25:19.000000 nitric-0.9.1.dev4/nitric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-06 00:25:19.000000 nitric-0.9.1.dev4/nitric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-06 00:24:36.000000 nitric-0.9.1.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 00:25:19.333565 nitric-0.9.1.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-06 00:24:36.000000 nitric-0.9.1.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 04:00:31.000000 nitric-0.9.2.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-11 04:00:31.000000 nitric-0.9.2.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.858970 nitric-0.9.2.dev3/nitric/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.858970 nitric-0.9.2.dev3/nitric/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20891 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.858970 nitric-0.9.2.dev3/nitric/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/config/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21168 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/faas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.858970 nitric-0.9.2.dev3/nitric/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.858970 nitric-0.9.2.dev3/nitric/proto/nitric/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/deploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/deploy/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/deploy/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/document/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/document/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/document/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/error/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/error/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/event/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/event/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/event/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/event/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/faas/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/faas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/faas/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/faas/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/queue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/queue/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/queue/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/resource/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/resource/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/secret/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/secret/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/storage/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/storage/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)    37084 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/validate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.858970 nitric-0.9.2.dev3/nitric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-11 04:01:12.000000 nitric-0.9.2.dev3/nitric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-11 04:01:12.000000 nitric-0.9.2.dev3/nitric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 04:01:12.000000 nitric-0.9.2.dev3/nitric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-11 04:01:12.000000 nitric-0.9.2.dev3/nitric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 04:01:12.000000 nitric-0.9.2.dev3/nitric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-11 04:00:31.000000 nitric-0.9.2.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 04:01:12.866970 nitric-0.9.2.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-11 04:00:31.000000 nitric-0.9.2.dev3/setup.py
```

### Comparing `nitric-0.9.1.dev4/LICENSE` & `nitric-0.9.2.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/PKG-INFO` & `nitric-0.9.2.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitric
-Version: 0.9.1.dev4
+Version: 0.9.2.dev3
 Summary: The Nitric SDK for Python 3
 Home-page: https://github.com/nitrictech/python-sdk
 Author: Nitric
 Author-email: team@nitric.io
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://nitric.io">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nitric Version: 0.9.1.dev4 Summary: The Nitric SDK
+Metadata-Version: 2.1 Name: nitric Version: 0.9.2.dev3 Summary: The Nitric SDK
 for Python 3 Home-page: https://github.com/nitrictech/python-sdk Author: Nitric
 Author-email: team@nitric.io License: UNKNOWN Description:
                                  [Nitric_Logo]
                ***** Build nitric applications with Python *****
          [Build_Status] [Codecov] [Version] [Downloads/week] [Discord]
 The Python SDK supports the use of the [Nitric](https://nitric.io) framework
 with Python 3.10+. For more information check out the main [Nitric repo](https:
```

### Comparing `nitric-0.9.1.dev4/README.md` & `nitric-0.9.2.dev3/README.md`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/__init__.py` & `nitric-0.9.2.dev3/nitric/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/api/__init__.py` & `nitric-0.9.2.dev3/nitric/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/api/const.py` & `nitric-0.9.2.dev3/nitric/api/const.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/api/documents.py` & `nitric-0.9.2.dev3/nitric/api/documents.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/api/events.py` & `nitric-0.9.2.dev3/nitric/api/events.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/api/exception.py` & `nitric-0.9.2.dev3/nitric/api/exception.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/api/queues.py` & `nitric-0.9.2.dev3/nitric/api/queues.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/api/secrets.py` & `nitric-0.9.2.dev3/nitric/api/secrets.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/api/storage.py` & `nitric-0.9.2.dev3/nitric/api/storage.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/application.py` & `nitric-0.9.2.dev3/nitric/resources/buckets.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,69 +12,83 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import asyncio
-from nitric.faas import FunctionServer
-from nitric.api.exception import NitricUnavailableException
+from __future__ import annotations
 
-# from nitric.resources.base import BaseResource
-from typing import Dict, List, Type, Any, TypeVar
+from nitric.api.exception import exception_from_grpc_error
+from nitric.api.storage import BucketRef, Storage
+from typing import List, Union
+from enum import Enum
+from grpclib import GRPCError
 
+from nitric.application import Nitric
+from nitric.proto.nitric.resource.v1 import (
+    Resource,
+    ResourceType,
+    Action,
+    ResourceDeclareRequest,
+)
 
-BT = TypeVar("BT")
+from nitric.resources.base import SecureResource
 
 
-class Nitric:
-    """Represents a nitric app."""
+class BucketPermission(Enum):
+    """Valid query expression operators."""
 
-    _workers: List[FunctionServer] = []
-    _cache: Dict[str, Dict[str, Any]] = {
-        "api": {},
-        "bucket": {},
-        "topic": {},
-        "secret": {},
-        "queue": {},
-        "collection": {},
-    }
+    reading = "reading"
+    writing = "writing"
+    deleting = "deleting"
 
-    @classmethod
-    def _register_worker(cls, srv: FunctionServer):
-        """Register a worker for this application."""
-        cls._workers.append(srv)
 
-    @classmethod
-    def _create_resource(cls, resource: Type[BT], name: str, *args, **kwargs) -> BT:
-        try:
-            resource_type = resource.__name__.lower()
-            if cls._cache.get(resource_type).get(name) is None:
-                cls._cache[resource_type][name] = resource.make(name, *args, **kwargs)
-
-            return cls._cache[resource_type][name]
-        except ConnectionRefusedError:
-            raise NitricUnavailableException(
-                'Unable to connect to a nitric server! If you\'re running locally make sure to run "nitric start"'
-            )
+class Bucket(SecureResource):
+    """A bucket resource, used for storage and retrieval of blob/binary data."""
 
-    @classmethod
-    def run(cls):
-        """
-        Start the nitric application.
+    name: str
+    actions: List[Action]
 
-        This will execute in an existing event loop if there is one, otherwise it will attempt to create its own.
-        """
+    def __init__(self, name: str):
+        """Create a bucket with the name provided or references it if it already exists."""
+        super().__init__()
+        self.name = name
+
+    async def _register(self):
         try:
-            try:
-                loop = asyncio.get_running_loop()
-            except RuntimeError:
-                loop = asyncio.get_event_loop()
-
-            loop.run_until_complete(asyncio.gather(*[wkr.start() for wkr in cls._workers]))
-        except KeyboardInterrupt:
-            print("\nexiting")
-        except ConnectionRefusedError:
-            raise NitricUnavailableException(
-                'Unable to connect to a nitric server! If you\'re running locally make sure to run "nitric start"'
+            await self._resources_stub.declare(
+                resource_declare_request=ResourceDeclareRequest(resource=self._to_resource())
             )
+        except GRPCError as grpc_err:
+            raise exception_from_grpc_error(grpc_err)
+
+    def _perms_to_actions(self, *args: [Union[BucketPermission, str]]) -> List[Action]:
+        permission_actions_map = {
+            BucketPermission.reading: [Action.BucketFileGet, Action.BucketFileList],
+            BucketPermission.writing: [Action.BucketFilePut],
+            BucketPermission.deleting: [Action.BucketFileDelete],
+        }
+        # convert strings to the enum value where needed
+        perms = [
+            permission if isinstance(permission, BucketPermission) else BucketPermission[permission.lower()]
+            for permission in args
+        ]
+        return [action for perm in perms for action in permission_actions_map[perm]]
+
+    def _to_resource(self) -> Resource:
+        return Resource(name=self.name, type=ResourceType.Bucket)
+
+    def allow(self, *args: Union[BucketPermission, str]) -> BucketRef:
+        """Request the required permissions for this resource."""
+        self._register_policy(*args)
+
+        return Storage().bucket(self.name)
+
+
+def bucket(name: str) -> Bucket:
+    """
+    Create and register a bucket.
+
+    If a bucket has already been registered with the same name, the original reference will be reused.
+    """
+    return Nitric._create_resource(Bucket, name)
```

### Comparing `nitric-0.9.1.dev4/nitric/config/__init__.py` & `nitric-0.9.2.dev3/nitric/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/config/default_settings.py` & `nitric-0.9.2.dev3/nitric/config/default_settings.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/faas.py` & `nitric-0.9.2.dev3/nitric/faas.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from __future__ import annotations
 from enum import Enum
 
 import functools
 import json
 import traceback
 from typing import Dict, Union, List, TypeVar, Callable, Coroutine, Any, Optional
+from opentelemetry import context, propagate
 
 import betterproto
 from betterproto.grpc.util.async_channel import AsyncChannel
 from nitric.utils import new_default_channel
 from nitric.proto.nitric.faas.v1 import (
     FaasServiceStub,
     InitRequest,
@@ -42,14 +43,15 @@
     ScheduleRate,
 )
 import grpclib
 import asyncio
 from abc import ABC
 
 Record = Dict[str, Union[str, List[str]]]
+PROPAGATOR = propagate.get_global_textmap()
 
 
 class HttpMethod(Enum):
     """Valid query expression operators."""
 
     GET = "GET"
     POST = "POST"
@@ -130,22 +132,32 @@
 
 # ====== HTTP ======
 
 
 class HttpRequest(Request):
     """Represents a translated Http Request forwarded from the Nitric Membrane."""
 
-    def __init__(self, data: bytes, method: str, path: str, params: Dict[str, str], query: Record, headers: Record):
+    def __init__(
+        self,
+        data: bytes,
+        method: str,
+        path: str,
+        params: Dict[str, str],
+        query: Record,
+        headers: Record,
+        trace_context: Dict[str, str],
+    ):
         """Construct a new HttpRequest."""
         super().__init__(data)
         self.method = method
         self.path = path
         self.params = params
         self.query = query
         self.headers = headers
+        self.trace_context = trace_context
 
     @property
     def json(self) -> Optional[Any]:
         """Get the body of the request as JSON, returns None if request body is not JSON."""
         try:
             return json.loads(self.body)
         except json.JSONDecodeError:
@@ -214,28 +226,27 @@
             request=HttpRequest(
                 data=trigger_request.data,
                 method=trigger_request.http.method,
                 query=query,
                 path=trigger_request.http.path,
                 params={k: v for (k, v) in trigger_request.http.path_params.items()},
                 headers=headers,
+                trace_context=trigger_request.trace_context.values,
             )
         )
 
 
-# ====== Events ======
-
-
 class EventRequest(Request):
     """Represents a translated Event, from a Subscribed Topic, forwarded from the Nitric Membrane."""
 
-    def __init__(self, data: bytes, topic: str):
+    def __init__(self, data: bytes, topic: str, trace_context: Dict[str, str]):
         """Construct a new EventRequest."""
         super().__init__(data)
         self.topic = topic
+        self.trace_context = trace_context
 
     @property
     def payload(self) -> bytes:
         """Return the payload of this request as text."""
         return json.loads(self.data.decode("utf-8"))
 
 
@@ -259,15 +270,21 @@
     def event(self) -> EventContext:
         """Return this EventContext, used when determining the context type of a trigger."""
         return self
 
     @staticmethod
     def from_grpc_trigger_request(trigger_request: TriggerRequest):
         """Construct a new EventContext from an Event trigger from the Nitric Membrane."""
-        return EventContext(request=EventRequest(data=trigger_request.data, topic=trigger_request.topic.topic))
+        return EventContext(
+            request=EventRequest(
+                data=trigger_request.data,
+                topic=trigger_request.topic.topic,
+                trace_context=trigger_request.trace_context.values,
+            )
+        )
 
 
 # async def face(inpp: int) -> str:
 #     return "thing"
 
 
 # ====== Function Handlers ======
@@ -483,20 +500,24 @@
                     # We don't need to reply
                     # proceed to the next available message
                     continue
                 if msg_type == "trigger_request":
                     ctx = _ctx_from_grpc_trigger_request(srv_msg.trigger_request)
 
                     try:
+                        if len(ctx.req.trace_context) > 0:
+                            context.attach(PROPAGATOR().extract(ctx.req.trace_context))
+
                         if ctx.http():
                             func = self._http_handler
                         elif ctx.event():
                             func = self._event_handler
                         else:
                             func = self._any_handler
+
                         response_ctx = (await func(ctx)) if asyncio.iscoroutinefunction(func) else func(ctx)
 
                         if response_ctx is None:
                             response_ctx = ctx
 
                         # Send function response back to server
                         await request_channel.send(
```

### Comparing `nitric-0.9.1.dev4/nitric/proto/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/document/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/document/v1/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/document/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/error/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/document/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/error/v1/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/error/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/event/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/error/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/event/v1/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/event/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/faas/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/event/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/faas/v1/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/faas/v1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,23 +144,38 @@
 class InitResponse(betterproto.Message):
     """Placeholder message"""
 
     pass
 
 
 @dataclass(eq=False, repr=False)
+class TraceContext(betterproto.Message):
+    values: Dict[str, str] = betterproto.map_field(
+        1, betterproto.TYPE_STRING, betterproto.TYPE_STRING
+    )
+
+
+@dataclass(eq=False, repr=False)
 class TriggerRequest(betterproto.Message):
     """The server has a trigger for the client to handle"""
 
     data: bytes = betterproto.bytes_field(1)
     """The data in the trigger"""
 
     mime_type: str = betterproto.string_field(2)
     """Should we supply a mime type for the data? Or rely on context?"""
 
+    trace_context: "TraceContext" = betterproto.message_field(10)
+    """
+    TraceInformation from the membrane Allows tying traces from external
+    triggers (e.g. HttpRequests) into each event request/response pair of the
+    Bidirectional stream. which cannot be facilitated by OOTB stream
+    interceptors from OTEL.
+    """
+
     http: "HttpTriggerContext" = betterproto.message_field(3, group="context")
     topic: "TopicTriggerContext" = betterproto.message_field(4, group="context")
 
 
 @dataclass(eq=False, repr=False)
 class HeaderValue(betterproto.Message):
     value: List[str] = betterproto.string_field(1)
```

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/queue/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/faas/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/queue/v1/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/queue/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/resource/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/resource/v1/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/resource/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/secret/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/secret/v1/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/secret/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/storage/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/nitric/storage/v1/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/nitric/storage/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/proto/validate/__init__.py` & `nitric-0.9.2.dev3/nitric/proto/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/resources/__init__.py` & `nitric-0.9.2.dev3/nitric/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/resources/apis.py` & `nitric-0.9.2.dev3/nitric/resources/apis.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/resources/base.py` & `nitric-0.9.2.dev3/nitric/resources/base.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/resources/buckets.py` & `nitric-0.9.2.dev3/nitric/resources/topics.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,81 +14,83 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from __future__ import annotations
 
+from nitric.api.events import Events, TopicRef
 from nitric.api.exception import exception_from_grpc_error
-from nitric.api.storage import BucketRef, Storage
 from typing import List, Union
 from enum import Enum
 from grpclib import GRPCError
-
 from nitric.application import Nitric
+from nitric.faas import EventMiddleware, FunctionServer, SubscriptionWorkerOptions
 from nitric.proto.nitric.resource.v1 import (
     Resource,
     ResourceType,
     Action,
     ResourceDeclareRequest,
 )
 
 from nitric.resources.base import SecureResource
 
 
-class BucketPermission(Enum):
+class TopicPermission(Enum):
     """Valid query expression operators."""
 
-    reading = "reading"
-    writing = "writing"
-    deleting = "deleting"
+    publishing = "publishing"
 
 
-class Bucket(SecureResource):
-    """A bucket resource, used for storage and retrieval of blob/binary data."""
+class Topic(SecureResource):
+    """A topic resource, used for asynchronous messaging between functions."""
 
     name: str
     actions: List[Action]
+    server: FunctionServer
 
     def __init__(self, name: str):
-        """Create a bucket with the name provided or references it if it already exists."""
+        """Construct a new topic."""
         super().__init__()
         self.name = name
 
     async def _register(self):
         try:
             await self._resources_stub.declare(
                 resource_declare_request=ResourceDeclareRequest(resource=self._to_resource())
             )
         except GRPCError as grpc_err:
             raise exception_from_grpc_error(grpc_err)
 
-    def _perms_to_actions(self, *args: [Union[BucketPermission, str]]) -> List[Action]:
-        permission_actions_map = {
-            BucketPermission.reading: [Action.BucketFileGet, Action.BucketFileList],
-            BucketPermission.writing: [Action.BucketFilePut],
-            BucketPermission.deleting: [Action.BucketFileDelete],
-        }
+    def _to_resource(self) -> Resource:
+        return Resource(name=self.name, type=ResourceType.Topic)
+
+    def _perms_to_actions(self, *args: Union[TopicPermission, str]) -> List[Action]:
+        _permMap = {TopicPermission.publishing: [Action.TopicEventPublish]}
         # convert strings to the enum value where needed
         perms = [
-            permission if isinstance(permission, BucketPermission) else BucketPermission[permission.lower()]
+            permission if isinstance(permission, TopicPermission) else TopicPermission[permission.lower()]
             for permission in args
         ]
-        return [action for perm in perms for action in permission_actions_map[perm]]
 
-    def _to_resource(self) -> Resource:
-        return Resource(name=self.name, type=ResourceType.Bucket)
+        return [action for perm in perms for action in _permMap[perm]]
 
-    def allow(self, *args: Union[BucketPermission, str]) -> BucketRef:
-        """Request the required permissions for this resource."""
+    def allow(self, *args: Union[TopicPermission, str]) -> TopicRef:
+        """Request the specified permissions to this resource."""
         self._register_policy(*args)
 
-        return Storage().bucket(self.name)
+        return Events().topic(self.name)
+
+    def subscribe(self, func: EventMiddleware):
+        """Create and return a subscription decorator for this topic."""
+        self.server = FunctionServer(SubscriptionWorkerOptions(topic=self.name))
+        self.server.event(func)
+        Nitric._register_worker(self.server)
 
 
-def bucket(name: str) -> Bucket:
+def topic(name: str) -> Topic:
     """
-    Create and register a bucket.
+    Create and register a topic.
 
-    If a bucket has already been registered with the same name, the original reference will be reused.
+    If a topic has already been registered with the same name, the original reference will be reused.
     """
-    return Nitric._create_resource(Bucket, name)
+    return Nitric._create_resource(Topic, name)
```

### Comparing `nitric-0.9.1.dev4/nitric/resources/collections.py` & `nitric-0.9.2.dev3/nitric/resources/collections.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/resources/queues.py` & `nitric-0.9.2.dev3/nitric/resources/queues.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/resources/schedules.py` & `nitric-0.9.2.dev3/nitric/resources/schedules.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/resources/secrets.py` & `nitric-0.9.2.dev3/nitric/resources/secrets.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric/utils.py` & `nitric-0.9.2.dev3/nitric/utils.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.1.dev4/nitric.egg-info/PKG-INFO` & `nitric-0.9.2.dev3/nitric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitric
-Version: 0.9.1.dev4
+Version: 0.9.2.dev3
 Summary: The Nitric SDK for Python 3
 Home-page: https://github.com/nitrictech/python-sdk
 Author: Nitric
 Author-email: team@nitric.io
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://nitric.io">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nitric Version: 0.9.1.dev4 Summary: The Nitric SDK
+Metadata-Version: 2.1 Name: nitric Version: 0.9.2.dev3 Summary: The Nitric SDK
 for Python 3 Home-page: https://github.com/nitrictech/python-sdk Author: Nitric
 Author-email: team@nitric.io License: UNKNOWN Description:
                                  [Nitric_Logo]
                ***** Build nitric applications with Python *****
          [Build_Status] [Codecov] [Version] [Downloads/week] [Discord]
 The Python SDK supports the use of the [Nitric](https://nitric.io) framework
 with Python 3.10+. For more information check out the main [Nitric repo](https:
```

### Comparing `nitric-0.9.1.dev4/nitric.egg-info/SOURCES.txt` & `nitric-0.9.2.dev3/nitric.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 nitric/api/queues.py
 nitric/api/secrets.py
 nitric/api/storage.py
 nitric/config/__init__.py
 nitric/config/default_settings.py
 nitric/proto/__init__.py
 nitric/proto/nitric/__init__.py
+nitric/proto/nitric/deploy/__init__.py
+nitric/proto/nitric/deploy/v1/__init__.py
 nitric/proto/nitric/document/__init__.py
 nitric/proto/nitric/document/v1/__init__.py
 nitric/proto/nitric/error/__init__.py
 nitric/proto/nitric/error/v1/__init__.py
 nitric/proto/nitric/event/__init__.py
 nitric/proto/nitric/event/v1/__init__.py
 nitric/proto/nitric/faas/__init__.py
```

### Comparing `nitric-0.9.1.dev4/setup.py` & `nitric-0.9.2.dev3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,18 +38,19 @@
     license_files=("LICENSE.txt",),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     setup_requires=["wheel"],
     install_requires=[
-        # "nitric-api==0.18.0",
-        "protobuf==3.19.5",
-        "betterproto==2.0.0b5",
         "asyncio",
+        "opentelemetry-api",
+        "opentelemetry-sdk",
+        "opentelemetry-exporter-otlp-proto-grpc",
+        "opentelemetry-instrumentation-grpc",
     ],
     extras_require={
         "dev": [
             "tox==3.20.1",
             "twine==3.2.0",
             "pytest==6.0.1",
             "pytest-cov==2.10.1",
```

