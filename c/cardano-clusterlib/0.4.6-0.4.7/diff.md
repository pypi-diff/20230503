# Comparing `tmp/cardano-clusterlib-0.4.6.tar.gz` & `tmp/cardano-clusterlib-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardano-clusterlib-0.4.6.tar", last modified: Fri Apr 28 13:29:52 2023, max compression
+gzip compressed data, was "cardano-clusterlib-0.4.7.tar", last modified: Wed May  3 11:50:55 2023, max compression
```

## Comparing `cardano-clusterlib-0.4.6.tar` & `cardano-clusterlib-0.4.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.612864 cardano-clusterlib-0.4.6/.github/
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/.github/workflows/
--rw-r--r--   0 sara      (1000) sara      (1000)      353 2022-09-08 20:06:48.000000 cardano-clusterlib-0.4.6/.github/workflows/repo_lint.yaml
--rw-rw-r--   0 sara      (1000) sara      (1000)      948 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/.gitignore
--rw-r--r--   0 sara      (1000) sara      (1000)      698 2022-09-26 14:22:34.000000 cardano-clusterlib-0.4.6/.markdownlint.yaml
--rw-r--r--   0 sara      (1000) sara      (1000)     1347 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.6/.pre-commit-config.yaml
--rw-rw-r--   0 sara      (1000) sara      (1000)     2523 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/.pylintrc
--rw-rw-r--   0 sara      (1000) sara      (1000)      318 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/.readthedocs.yaml
--rw-r--r--   0 sara      (1000) sara      (1000)     3267 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/CODE-OF-CONDUCT.md
--rw-r--r--   0 sara      (1000) sara      (1000)    11360 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/LICENSE
--rw-r--r--   0 sara      (1000) sara      (1000)     1279 2023-04-14 14:27:56.000000 cardano-clusterlib-0.4.6/Makefile
--rw-r--r--   0 sara      (1000) sara      (1000)     7853 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/PKG-INFO
--rw-r--r--   0 sara      (1000) sara      (1000)     7170 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/README.md
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/cardano_clusterlib/
--rw-rw-r--   0 sara      (1000) sara      (1000)      174 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/__init__.py
--rw-r--r--   0 sara      (1000) sara      (1000)     8119 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/address_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)     2593 2022-08-23 09:17:09.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/clusterlib.py
--rw-r--r--   0 sara      (1000) sara      (1000)     7791 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/clusterlib_helpers.py
--rw-r--r--   0 sara      (1000) sara      (1000)    14563 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/clusterlib_klass.py
--rw-r--r--   0 sara      (1000) sara      (1000)     1086 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/consts.py
--rw-r--r--   0 sara      (1000) sara      (1000)     1111 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/coverage.py
--rw-rw-r--   0 sara      (1000) sara      (1000)       36 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/exceptions.py
--rw-r--r--   0 sara      (1000) sara      (1000)     3799 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/genesis_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)     7438 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/governance_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)     1554 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/helpers.py
--rw-r--r--   0 sara      (1000) sara      (1000)     2815 2023-03-20 14:27:55.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/key_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)     6004 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/node_group.py
--rw-rw-r--   0 sara      (1000) sara      (1000)        0 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/py.typed
--rw-r--r--   0 sara      (1000) sara      (1000)    18201 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/query_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)    13370 2023-04-14 14:27:56.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/stake_address_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)    12907 2023-03-20 14:27:55.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/stake_pool_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)     6849 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/structs.py
--rw-r--r--   0 sara      (1000) sara      (1000)    62487 2023-04-28 13:18:20.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/transaction_group.py
--rw-r--r--   0 sara      (1000) sara      (1000)    44202 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/txtools.py
--rw-rw-r--   0 sara      (1000) sara      (1000)      608 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/cardano_clusterlib/types.py
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/
--rw-r--r--   0 sara      (1000) sara      (1000)     7853 2023-04-28 13:29:52.000000 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/PKG-INFO
--rw-r--r--   0 sara      (1000) sara      (1000)     1383 2023-04-28 13:29:52.000000 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/SOURCES.txt
--rw-r--r--   0 sara      (1000) sara      (1000)        1 2023-04-28 13:29:52.000000 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/dependency_links.txt
--rw-r--r--   0 sara      (1000) sara      (1000)        1 2022-08-03 14:24:31.000000 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/not-zip-safe
--rw-r--r--   0 sara      (1000) sara      (1000)       19 2023-04-28 13:29:52.000000 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/requires.txt
--rw-r--r--   0 sara      (1000) sara      (1000)       19 2023-04-28 13:29:52.000000 cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/top_level.txt
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/docs/
--rw-rw-r--   0 sara      (1000) sara      (1000)      740 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/docs/Makefile
--rw-r--r--   0 sara      (1000) sara      (1000)       36 2022-09-26 14:22:34.000000 cardano-clusterlib-0.4.6/docs/requirements.txt
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/docs/source/
--rw-r--r--   0 sara      (1000) sara      (1000)     3694 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.6/docs/source/cardano_clusterlib.rst
--rw-r--r--   0 sara      (1000) sara      (1000)     4112 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.6/docs/source/conf.py
--rw-rw-r--   0 sara      (1000) sara      (1000)      491 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/docs/source/index.rst
--rw-rw-r--   0 sara      (1000) sara      (1000)       95 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/docs/source/modules.rst
--rw-rw-r--   0 sara      (1000) sara      (1000)       31 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/docs/source/readme.rst
--rw-rw-r--   0 sara      (1000) sara      (1000)      236 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/mypy.ini
--rw-r--r--   0 sara      (1000) sara      (1000)      577 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.6/pyproject.toml
--rw-r--r--   0 sara      (1000) sara      (1000)       59 2023-03-20 14:27:55.000000 cardano-clusterlib-0.4.6/requirements-dev.txt
--rw-r--r--   0 sara      (1000) sara      (1000)     1128 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/setup.cfg
--rw-rw-r--   0 sara      (1000) sara      (1000)      163 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.6/setup.py
-drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-28 13:29:52.616864 cardano-clusterlib-0.4.6/upgrading/
--rw-r--r--   0 sara      (1000) sara      (1000)     7363 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.6/upgrading/refactor_to_0_4_0rc1.sed
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.586058 cardano-clusterlib-0.4.7/
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.582057 cardano-clusterlib-0.4.7/.github/
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.583057 cardano-clusterlib-0.4.7/.github/workflows/
+-rw-r--r--   0 martink   (1000) martink   (1000)      353 2022-08-30 10:58:34.000000 cardano-clusterlib-0.4.7/.github/workflows/repo_lint.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)      948 2021-12-16 16:01:16.000000 cardano-clusterlib-0.4.7/.gitignore
+-rw-r--r--   0 martink   (1000) martink   (1000)      698 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.7/.markdownlint.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     1347 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.7/.pre-commit-config.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     2523 2022-06-03 10:16:54.000000 cardano-clusterlib-0.4.7/.pylintrc
+-rw-r--r--   0 martink   (1000) martink   (1000)      318 2021-03-11 15:25:52.000000 cardano-clusterlib-0.4.7/.readthedocs.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     3267 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.7/CODE-OF-CONDUCT.md
+-rw-r--r--   0 martink   (1000) martink   (1000)    11360 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.7/LICENSE
+-rw-r--r--   0 martink   (1000) martink   (1000)     1279 2023-04-14 10:59:03.000000 cardano-clusterlib-0.4.7/Makefile
+-rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-05-03 11:50:55.586058 cardano-clusterlib-0.4.7/PKG-INFO
+-rw-r--r--   0 martink   (1000) martink   (1000)     7170 2023-03-16 13:15:07.000000 cardano-clusterlib-0.4.7/README.md
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.585057 cardano-clusterlib-0.4.7/cardano_clusterlib/
+-rw-r--r--   0 martink   (1000) martink   (1000)      174 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/__init__.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     8119 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/address_group.py
+-rw-rw-r--   0 martink   (1000) martink   (1000)     2593 2022-08-06 21:08:03.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/clusterlib.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     7791 2023-03-28 12:40:20.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/clusterlib_helpers.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    14563 2023-05-03 11:46:08.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/clusterlib_klass.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1086 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/consts.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1111 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/coverage.py
+-rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/exceptions.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     3799 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/genesis_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     7438 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/governance_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1554 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/helpers.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     2815 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/key_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     6004 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/node_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)        0 2021-03-10 16:56:29.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/py.typed
+-rw-r--r--   0 martink   (1000) martink   (1000)    18201 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/query_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    13370 2023-04-14 10:37:46.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/stake_address_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    12907 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/stake_pool_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     6849 2023-04-17 13:43:55.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/structs.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    62487 2023-05-03 11:46:08.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/transaction_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    44202 2023-04-04 10:13:01.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/txtools.py
+-rw-r--r--   0 martink   (1000) martink   (1000)      608 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/types.py
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.586058 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/
+-rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-05-03 11:50:55.000000 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/PKG-INFO
+-rw-r--r--   0 martink   (1000) martink   (1000)     1383 2023-05-03 11:50:55.000000 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/SOURCES.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)        1 2023-05-03 11:50:55.000000 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/dependency_links.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)        1 2021-03-10 16:00:20.000000 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/not-zip-safe
+-rw-r--r--   0 martink   (1000) martink   (1000)       15 2023-05-03 11:50:55.000000 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/requires.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-05-03 11:50:55.000000 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/top_level.txt
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.586058 cardano-clusterlib-0.4.7/docs/
+-rw-r--r--   0 martink   (1000) martink   (1000)      740 2021-03-23 15:49:32.000000 cardano-clusterlib-0.4.7/docs/Makefile
+-rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.7/docs/requirements.txt
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.586058 cardano-clusterlib-0.4.7/docs/source/
+-rw-r--r--   0 martink   (1000) martink   (1000)     3694 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.7/docs/source/cardano_clusterlib.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)     4112 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.7/docs/source/conf.py
+-rw-r--r--   0 martink   (1000) martink   (1000)      491 2021-03-11 13:53:31.000000 cardano-clusterlib-0.4.7/docs/source/index.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)       95 2021-03-11 13:52:06.000000 cardano-clusterlib-0.4.7/docs/source/modules.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)       31 2021-03-11 13:53:55.000000 cardano-clusterlib-0.4.7/docs/source/readme.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)      236 2021-03-10 15:33:40.000000 cardano-clusterlib-0.4.7/mypy.ini
+-rw-r--r--   0 martink   (1000) martink   (1000)      610 2023-05-03 11:49:49.000000 cardano-clusterlib-0.4.7/pyproject.toml
+-rw-r--r--   0 martink   (1000) martink   (1000)       59 2023-01-19 14:58:18.000000 cardano-clusterlib-0.4.7/requirements-dev.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)     1124 2023-05-03 11:50:55.587057 cardano-clusterlib-0.4.7/setup.cfg
+-rw-r--r--   0 martink   (1000) martink   (1000)      202 2023-05-03 11:49:49.000000 cardano-clusterlib-0.4.7/setup.py
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.586058 cardano-clusterlib-0.4.7/upgrading/
+-rw-r--r--   0 martink   (1000) martink   (1000)     7363 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.7/upgrading/refactor_to_0_4_0rc1.sed
```

### Comparing `cardano-clusterlib-0.4.6/.gitignore` & `cardano-clusterlib-0.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/.markdownlint.yaml` & `cardano-clusterlib-0.4.7/.markdownlint.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/.pre-commit-config.yaml` & `cardano-clusterlib-0.4.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/.pylintrc` & `cardano-clusterlib-0.4.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/CODE-OF-CONDUCT.md` & `cardano-clusterlib-0.4.7/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/LICENSE` & `cardano-clusterlib-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/Makefile` & `cardano-clusterlib-0.4.7/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/PKG-INFO` & `cardano-clusterlib-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

### Comparing `cardano-clusterlib-0.4.6/README.md` & `cardano-clusterlib-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/address_group.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/address_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/clusterlib.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/clusterlib.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/clusterlib_helpers.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/clusterlib_helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/clusterlib_klass.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/clusterlib_klass.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/consts.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/consts.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/coverage.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/coverage.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/genesis_group.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/genesis_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/governance_group.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/governance_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/helpers.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/key_group.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/key_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/node_group.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/node_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/query_group.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/query_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/stake_address_group.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/stake_address_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/stake_pool_group.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/stake_pool_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/structs.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/structs.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/transaction_group.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/transaction_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/txtools.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/txtools.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib/types.py` & `cardano-clusterlib-0.4.7/cardano_clusterlib/types.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/PKG-INFO` & `cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

### Comparing `cardano-clusterlib-0.4.6/cardano_clusterlib.egg-info/SOURCES.txt` & `cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/docs/Makefile` & `cardano-clusterlib-0.4.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/docs/source/cardano_clusterlib.rst` & `cardano-clusterlib-0.4.7/docs/source/cardano_clusterlib.rst`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/docs/source/conf.py` & `cardano-clusterlib-0.4.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.6/pyproject.toml` & `cardano-clusterlib-0.4.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 force_single_line = true
```

### Comparing `cardano-clusterlib-0.4.6/setup.cfg` & `cardano-clusterlib-0.4.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 setup_requires = 
 	setuptools_scm
 install_requires = 
-	setuptools >= 21.0.0
+	setuptools >= 45
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `cardano-clusterlib-0.4.6/upgrading/refactor_to_0_4_0rc1.sed` & `cardano-clusterlib-0.4.7/upgrading/refactor_to_0_4_0rc1.sed`

 * *Files identical despite different names*

