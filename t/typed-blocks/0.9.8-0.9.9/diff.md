# Comparing `tmp/typed-blocks-0.9.8.tar.gz` & `tmp/typed-blocks-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typed-blocks-0.9.8.tar", last modified: Fri Jul 29 21:46:09 2022, max compression
+gzip compressed data, was "typed-blocks-0.9.9.tar", last modified: Mon Oct  3 15:04:28 2022, max compression
```

## Comparing `typed-blocks-0.9.8.tar` & `typed-blocks-0.9.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.736029 typed-blocks-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)    10142 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2972 2022-07-29 21:46:09.736029 typed-blocks-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.732029 typed-blocks-0.9.8/blocks/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.732029 typed-blocks-0.9.8/blocks/db/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.732029 typed-blocks-0.9.8/blocks/db/next/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/db/next/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5187 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/db/next/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.732029 typed-blocks-0.9.8/blocks/db/sql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/db/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/db/sql/processors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2753 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/db/sql/sources.py
--rw-r--r--   0 runner    (1001) docker     (121)     2587 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/db/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     5118 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.732029 typed-blocks-0.9.8/blocks/kafka/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3951 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/kafka/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/kafka/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     5332 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/kafka/processors.py
--rw-r--r--   0 runner    (1001) docker     (121)    10094 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/kafka/sources.py
--rw-r--r--   0 runner    (1001) docker     (121)     8286 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/kafka/topics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/kafka/types.py
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.732029 typed-blocks-0.9.8/blocks/postgres/
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/postgres/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/postgres/next.py
--rw-r--r--   0 runner    (1001) docker     (121)     2985 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/postgres/processors.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/postgres/protocols.py
--rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/postgres/sources.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.732029 typed-blocks-0.9.8/blocks/redis/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/redis/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/redis/processors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/redis/serdes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3255 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/redis/sources.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/redis/streams.py
--rw-r--r--   0 runner    (1001) docker     (121)     9996 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.736029 typed-blocks-0.9.8/blocks/sources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2147 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/sources/schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.736029 typed-blocks-0.9.8/blocks/sqlite/
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/sqlite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.736029 typed-blocks-0.9.8/blocks/types/
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4469 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/types/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/types/dto.py
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/blocks/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-07-29 21:46:09.736029 typed-blocks-0.9.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.732029 typed-blocks-0.9.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.736029 typed-blocks-0.9.8/tests/db/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/tests/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2562 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/tests/db/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-07-29 21:46:04.000000 typed-blocks-0.9.8/tests/db/test_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-29 21:46:09.736029 typed-blocks-0.9.8/typed_blocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2972 2022-07-29 21:46:09.000000 typed-blocks-0.9.8/typed_blocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-07-29 21:46:09.000000 typed-blocks-0.9.8/typed_blocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-29 21:46:09.000000 typed-blocks-0.9.8/typed_blocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-07-29 21:46:09.000000 typed-blocks-0.9.8/typed_blocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-29 21:46:09.000000 typed-blocks-0.9.8/typed_blocks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.329920 typed-blocks-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    10142 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2972 2022-10-03 15:04:28.329920 typed-blocks-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.325920 typed-blocks-0.9.9/blocks/
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.325920 typed-blocks-0.9.9/blocks/db/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.325920 typed-blocks-0.9.9/blocks/db/next/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/db/next/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5187 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/db/next/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.329920 typed-blocks-0.9.9/blocks/db/sql/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/db/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/db/sql/processors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2753 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/db/sql/sources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2587 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/db/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5118 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.329920 typed-blocks-0.9.9/blocks/kafka/
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3951 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/kafka/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/kafka/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5332 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/kafka/processors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10094 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/kafka/sources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8286 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/kafka/topics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/kafka/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.329920 typed-blocks-0.9.9/blocks/postgres/
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/postgres/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/postgres/next.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2985 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/postgres/processors.py
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/postgres/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/postgres/sources.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.329920 typed-blocks-0.9.9/blocks/redis/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/redis/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/redis/processors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/redis/serdes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3255 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/redis/sources.py
+-rw-r--r--   0 runner    (1001) docker     (121)      862 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/redis/streams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9996 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.329920 typed-blocks-0.9.9/blocks/sources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2147 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/sources/schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.329920 typed-blocks-0.9.9/blocks/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/sqlite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.329920 typed-blocks-0.9.9/blocks/types/
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4469 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/types/dto.py
+-rw-r--r--   0 runner    (1001) docker     (121)      687 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/blocks/validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-10-03 15:04:28.329920 typed-blocks-0.9.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.325920 typed-blocks-0.9.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.329920 typed-blocks-0.9.9/tests/db/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/tests/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2562 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/tests/db/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-10-03 15:04:22.000000 typed-blocks-0.9.9/tests/db/test_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 15:04:28.329920 typed-blocks-0.9.9/typed_blocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2972 2022-10-03 15:04:28.000000 typed-blocks-0.9.9/typed_blocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-10-03 15:04:28.000000 typed-blocks-0.9.9/typed_blocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 15:04:28.000000 typed-blocks-0.9.9/typed_blocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-10-03 15:04:28.000000 typed-blocks-0.9.9/typed_blocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-03 15:04:28.000000 typed-blocks-0.9.9/typed_blocks.egg-info/top_level.txt
```

### Comparing `typed-blocks-0.9.8/LICENSE` & `typed-blocks-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/PKG-INFO` & `typed-blocks-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typed-blocks
-Version: 0.9.8
+Version: 0.9.9
 Summary: Modular event-centric python library made for simplification typical stream applications development with python type system strong exploitation.
 Home-page: https://github.com/severstal-digital/typed-blocks
 Author: Daniil Zubakin
 Author-email: <daniilzubakin@gmail.com>
 License: Apache-2.0 License
 Project-URL: Bug Tracker, https://github.com/severstal-digital/typed-blocks/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `typed-blocks-0.9.8/README.md` & `typed-blocks-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/app.py` & `typed-blocks-0.9.9/blocks/app.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/db/next/sql.py` & `typed-blocks-0.9.9/blocks/db/next/sql.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/db/sql/processors.py` & `typed-blocks-0.9.9/blocks/db/sql/processors.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/db/sql/sources.py` & `typed-blocks-0.9.9/blocks/db/sql/sources.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/db/types.py` & `typed-blocks-0.9.9/blocks/db/types.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/decorators.py` & `typed-blocks-0.9.9/blocks/decorators.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/graph.py` & `typed-blocks-0.9.9/blocks/graph.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/kafka/app.py` & `typed-blocks-0.9.9/blocks/kafka/app.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/kafka/events.py` & `typed-blocks-0.9.9/blocks/kafka/events.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/kafka/processors.py` & `typed-blocks-0.9.9/blocks/kafka/processors.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/kafka/sources.py` & `typed-blocks-0.9.9/blocks/kafka/sources.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/kafka/topics.py` & `typed-blocks-0.9.9/blocks/kafka/topics.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/kafka/types.py` & `typed-blocks-0.9.9/blocks/kafka/types.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/postgres/app.py` & `typed-blocks-0.9.9/blocks/postgres/app.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/postgres/processors.py` & `typed-blocks-0.9.9/blocks/postgres/processors.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/postgres/sources.py` & `typed-blocks-0.9.9/blocks/postgres/sources.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/redis/app.py` & `typed-blocks-0.9.9/blocks/redis/app.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/redis/processors.py` & `typed-blocks-0.9.9/blocks/redis/processors.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/redis/serdes.py` & `typed-blocks-0.9.9/blocks/redis/serdes.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/redis/sources.py` & `typed-blocks-0.9.9/blocks/redis/sources.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/redis/streams.py` & `typed-blocks-0.9.9/blocks/redis/streams.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/runners.py` & `typed-blocks-0.9.9/blocks/runners.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/sources/schedule.py` & `typed-blocks-0.9.9/blocks/sources/schedule.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/types/base.py` & `typed-blocks-0.9.9/blocks/types/base.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/utils.py` & `typed-blocks-0.9.9/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/blocks/validation.py` & `typed-blocks-0.9.9/blocks/validation.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/setup.cfg` & `typed-blocks-0.9.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = typed-blocks
-version = 0.9.8
+version = 0.9.9
 description = Modular event-centric python library made for simplification typical stream applications development with python type system strong exploitation.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache-2.0 License
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3
```

### Comparing `typed-blocks-0.9.8/tests/db/test_sql.py` & `typed-blocks-0.9.9/tests/db/test_sql.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/tests/db/test_sqlite.py` & `typed-blocks-0.9.9/tests/db/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `typed-blocks-0.9.8/typed_blocks.egg-info/PKG-INFO` & `typed-blocks-0.9.9/typed_blocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typed-blocks
-Version: 0.9.8
+Version: 0.9.9
 Summary: Modular event-centric python library made for simplification typical stream applications development with python type system strong exploitation.
 Home-page: https://github.com/severstal-digital/typed-blocks
 Author: Daniil Zubakin
 Author-email: <daniilzubakin@gmail.com>
 License: Apache-2.0 License
 Project-URL: Bug Tracker, https://github.com/severstal-digital/typed-blocks/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `typed-blocks-0.9.8/typed_blocks.egg-info/SOURCES.txt` & `typed-blocks-0.9.9/typed_blocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

