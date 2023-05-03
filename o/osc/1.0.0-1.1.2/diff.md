# Comparing `tmp/osc-1.0.0.tar.gz` & `tmp/osc-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc-1.0.0.tar", last modified: Fri Mar 17 09:30:59 2023, max compression
+gzip compressed data, was "osc-1.1.2.tar", last modified: Wed May  3 08:14:07 2023, max compression
```

## Comparing `osc-1.0.0.tar` & `osc-1.1.2.tar`

### file list

```diff
@@ -1,56 +1,85 @@
-drwxr-xr-x   0 dmach     (1000) users      (100)        0 2023-03-17 09:30:59.082924 osc-1.0.0/
--rw-r--r--   0 dmach     (1000) users      (100)      480 2022-08-23 07:12:40.000000 osc-1.0.0/AUTHORS
--rw-r--r--   0 dmach     (1000) users      (100)    18092 2022-08-23 07:12:40.000000 osc-1.0.0/COPYING
--rw-r--r--   0 dmach     (1000) users      (100)       63 2022-08-24 08:05:58.000000 osc-1.0.0/MANIFEST.in
--rw-r--r--   0 dmach     (1000) users      (100)     4720 2023-03-17 09:30:01.000000 osc-1.0.0/NEWS
--rw-r--r--   0 dmach     (1000) users      (100)     1420 2023-03-17 09:30:59.082924 osc-1.0.0/PKG-INFO
--rw-r--r--   0 dmach     (1000) users      (100)     5632 2023-03-17 09:30:01.000000 osc-1.0.0/README.md
-drwxr-xr-x   0 dmach     (1000) users      (100)        0 2023-03-17 09:30:59.082924 osc-1.0.0/osc/
--rw-r--r--   0 dmach     (1000) users      (100)    13406 2023-03-17 09:30:01.000000 osc-1.0.0/osc/OscConfigParser.py
--rw-r--r--   0 dmach     (1000) users      (100)      259 2023-03-17 09:30:01.000000 osc-1.0.0/osc/__init__.py
-drwxr-xr-x   0 dmach     (1000) users      (100)        0 2023-03-17 09:30:59.082924 osc-1.0.0/osc/_private/
--rw-r--r--   0 dmach     (1000) users      (100)      692 2023-03-17 09:30:01.000000 osc-1.0.0/osc/_private/__init__.py
--rw-r--r--   0 dmach     (1000) users      (100)     5419 2023-03-17 09:30:01.000000 osc-1.0.0/osc/_private/api.py
--rw-r--r--   0 dmach     (1000) users      (100)     2333 2023-03-17 09:30:01.000000 osc-1.0.0/osc/_private/api_build.py
--rw-r--r--   0 dmach     (1000) users      (100)      381 2023-03-17 09:30:01.000000 osc-1.0.0/osc/_private/api_configuration.py
--rw-r--r--   0 dmach     (1000) users      (100)     3347 2023-03-17 09:30:01.000000 osc-1.0.0/osc/_private/api_source.py
--rw-r--r--   0 dmach     (1000) users      (100)     1525 2023-03-17 09:30:01.000000 osc-1.0.0/osc/_private/common.py
--rw-r--r--   0 dmach     (1000) users      (100)     3623 2023-03-17 09:30:01.000000 osc-1.0.0/osc/_private/package.py
--rw-r--r--   0 dmach     (1000) users      (100)     1207 2023-03-17 09:30:01.000000 osc-1.0.0/osc/_private/request.py
--rw-r--r--   0 dmach     (1000) users      (100)     8269 2023-03-17 09:30:01.000000 osc-1.0.0/osc/babysitter.py
--rw-r--r--   0 dmach     (1000) users      (100)    63454 2023-03-17 09:30:01.000000 osc-1.0.0/osc/build.py
--rw-r--r--   0 dmach     (1000) users      (100)     3211 2023-03-17 09:30:01.000000 osc-1.0.0/osc/checker.py
--rw-r--r--   0 dmach     (1000) users      (100)    10032 2023-03-17 09:30:01.000000 osc-1.0.0/osc/cmdln.py
--rw-r--r--   0 dmach     (1000) users      (100)   422464 2023-03-17 09:30:01.000000 osc-1.0.0/osc/commandline.py
--rw-r--r--   0 dmach     (1000) users      (100)    40494 2023-03-17 09:30:01.000000 osc-1.0.0/osc/conf.py
--rw-r--r--   0 dmach     (1000) users      (100)    24408 2023-03-17 09:30:01.000000 osc-1.0.0/osc/connection.py
--rw-r--r--   0 dmach     (1000) users      (100)   328802 2023-03-17 09:30:01.000000 osc-1.0.0/osc/core.py
--rw-r--r--   0 dmach     (1000) users      (100)    11240 2023-03-17 09:30:01.000000 osc-1.0.0/osc/credentials.py
--rw-r--r--   0 dmach     (1000) users      (100)    17821 2023-03-17 09:30:01.000000 osc-1.0.0/osc/fetch.py
--rw-r--r--   0 dmach     (1000) users      (100)     1347 2023-03-17 09:30:01.000000 osc-1.0.0/osc/grabber.py
--rw-r--r--   0 dmach     (1000) users      (100)     2076 2023-03-17 09:30:01.000000 osc-1.0.0/osc/meter.py
--rw-r--r--   0 dmach     (1000) users      (100)     5923 2023-03-17 09:30:01.000000 osc-1.0.0/osc/oscerr.py
--rw-r--r--   0 dmach     (1000) users      (100)     6840 2023-03-17 09:30:01.000000 osc-1.0.0/osc/oscssl.py
--rw-r--r--   0 dmach     (1000) users      (100)        0 2023-03-17 09:30:01.000000 osc-1.0.0/osc/py.typed
--rw-r--r--   0 dmach     (1000) users      (100)     9989 2023-03-17 09:30:01.000000 osc-1.0.0/osc/store.py
-drwxr-xr-x   0 dmach     (1000) users      (100)        0 2023-03-17 09:30:59.082924 osc-1.0.0/osc/util/
--rw-r--r--   0 dmach     (1000) users      (100)       79 2022-08-23 07:12:40.000000 osc-1.0.0/osc/util/__init__.py
--rw-r--r--   0 dmach     (1000) users      (100)     7084 2023-03-17 09:30:01.000000 osc-1.0.0/osc/util/ar.py
--rw-r--r--   0 dmach     (1000) users      (100)     7225 2023-03-17 09:30:01.000000 osc-1.0.0/osc/util/archquery.py
--rw-r--r--   0 dmach     (1000) users      (100)     8208 2023-03-17 09:30:01.000000 osc-1.0.0/osc/util/cpio.py
--rw-r--r--   0 dmach     (1000) users      (100)     9258 2023-03-17 09:30:01.000000 osc-1.0.0/osc/util/debquery.py
--rw-r--r--   0 dmach     (1000) users      (100)     2728 2022-08-23 07:12:40.000000 osc-1.0.0/osc/util/git_version.py
--rw-r--r--   0 dmach     (1000) users      (100)     1886 2023-03-17 09:30:01.000000 osc-1.0.0/osc/util/helper.py
--rw-r--r--   0 dmach     (1000) users      (100)     5499 2023-03-17 09:30:01.000000 osc-1.0.0/osc/util/packagequery.py
--rw-r--r--   0 dmach     (1000) users      (100)     6788 2023-03-17 09:30:01.000000 osc-1.0.0/osc/util/repodata.py
--rw-r--r--   0 dmach     (1000) users      (100)    13167 2023-03-17 09:30:01.000000 osc-1.0.0/osc/util/rpmquery.py
--rw-r--r--   0 dmach     (1000) users      (100)      809 2023-03-17 09:30:01.000000 osc-1.0.0/osc/util/safewriter.py
-drwxr-xr-x   0 dmach     (1000) users      (100)        0 2023-03-17 09:30:59.082924 osc-1.0.0/osc.egg-info/
--rw-r--r--   0 dmach     (1000) users      (100)     1420 2023-03-17 09:30:59.000000 osc-1.0.0/osc.egg-info/PKG-INFO
--rw-r--r--   0 dmach     (1000) users      (100)      930 2023-03-17 09:30:59.000000 osc-1.0.0/osc.egg-info/SOURCES.txt
--rw-r--r--   0 dmach     (1000) users      (100)        1 2023-03-17 09:30:59.000000 osc-1.0.0/osc.egg-info/dependency_links.txt
--rw-r--r--   0 dmach     (1000) users      (100)       44 2023-03-17 09:30:59.000000 osc-1.0.0/osc.egg-info/entry_points.txt
--rw-r--r--   0 dmach     (1000) users      (100)       52 2023-03-17 09:30:59.000000 osc-1.0.0/osc.egg-info/requires.txt
--rw-r--r--   0 dmach     (1000) users      (100)        4 2023-03-17 09:30:59.000000 osc-1.0.0/osc.egg-info/top_level.txt
--rw-r--r--   0 dmach     (1000) users      (100)     1560 2023-03-17 09:30:59.082924 osc-1.0.0/setup.cfg
--rwxr-xr-x   0 dmach     (1000) users      (100)       95 2022-08-24 07:02:17.000000 osc-1.0.0/setup.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.947695 osc-1.1.2/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      480 2023-05-03 08:03:10.000000 osc-1.1.2/AUTHORS
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    18092 2023-05-03 08:03:10.000000 osc-1.1.2/COPYING
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       63 2023-05-03 08:03:10.000000 osc-1.1.2/MANIFEST.in
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     6939 2023-05-03 08:10:41.000000 osc-1.1.2/NEWS
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1420 2023-05-03 08:14:07.947695 osc-1.1.2/PKG-INFO
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5632 2023-05-03 08:03:10.000000 osc-1.1.2/README.md
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.943695 osc-1.1.2/osc/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    13406 2023-05-03 08:03:10.000000 osc-1.1.2/osc/OscConfigParser.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      259 2023-05-03 08:03:30.000000 osc-1.1.2/osc/__init__.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.943695 osc-1.1.2/osc/_private/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      692 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5770 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/api.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2338 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/api_build.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      381 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/api_configuration.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3347 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/api_source.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1525 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/common.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3623 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1207 2023-05-03 08:03:10.000000 osc-1.1.2/osc/_private/request.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8318 2023-05-03 08:03:10.000000 osc-1.1.2/osc/babysitter.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    63226 2023-05-03 08:03:10.000000 osc-1.1.2/osc/build.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3211 2023-05-03 08:03:10.000000 osc-1.1.2/osc/checker.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    10121 2023-05-03 08:03:10.000000 osc-1.1.2/osc/cmdln.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)   440150 2023-05-03 08:03:10.000000 osc-1.1.2/osc/commandline.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.943695 osc-1.1.2/osc/commands/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:03:10.000000 osc-1.1.2/osc/commands/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    40770 2023-05-03 08:03:10.000000 osc-1.1.2/osc/conf.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    25246 2023-05-03 08:03:10.000000 osc-1.1.2/osc/connection.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)   331036 2023-05-03 08:03:10.000000 osc-1.1.2/osc/core.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    11240 2023-05-03 08:03:10.000000 osc-1.1.2/osc/credentials.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    17821 2023-05-03 08:03:10.000000 osc-1.1.2/osc/fetch.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1411 2023-05-03 08:03:10.000000 osc-1.1.2/osc/grabber.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2076 2023-05-03 08:03:10.000000 osc-1.1.2/osc/meter.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5923 2023-05-03 08:03:10.000000 osc-1.1.2/osc/oscerr.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     6840 2023-05-03 08:03:10.000000 osc-1.1.2/osc/oscssl.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:03:10.000000 osc-1.1.2/osc/py.typed
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     9989 2023-05-03 08:03:10.000000 osc-1.1.2/osc/store.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.943695 osc-1.1.2/osc/util/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       79 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     7084 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/ar.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     7225 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/archquery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8208 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/cpio.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     9258 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/debquery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2728 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/git_version.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1886 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/helper.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5499 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/packagequery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     6788 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/repodata.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    13167 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/rpmquery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      809 2023-05-03 08:03:10.000000 osc-1.1.2/osc/util/safewriter.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.943695 osc-1.1.2/osc.egg-info/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1420 2023-05-03 08:14:07.000000 osc-1.1.2/osc.egg-info/PKG-INFO
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1593 2023-05-03 08:14:07.000000 osc-1.1.2/osc.egg-info/SOURCES.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        1 2023-05-03 08:14:07.000000 osc-1.1.2/osc.egg-info/dependency_links.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       44 2023-05-03 08:14:07.000000 osc-1.1.2/osc.egg-info/entry_points.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       52 2023-05-03 08:14:07.000000 osc-1.1.2/osc.egg-info/requires.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        4 2023-05-03 08:14:07.000000 osc-1.1.2/osc.egg-info/top_level.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1574 2023-05-03 08:14:07.947695 osc-1.1.2/setup.cfg
+-rwxr-xr-x   0 dmach     (1000) dmach     (1000)       95 2023-05-03 08:03:10.000000 osc-1.1.2/setup.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-03 08:14:07.947695 osc-1.1.2/tests/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      788 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test__private_api.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4912 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test__private_package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3168 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_addfiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    29754 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_commandline.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    21957 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_commit.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1451 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_conf.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      578 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_config_parser.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1783 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_core.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8446 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_core_package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      877 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_core_request.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8656 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_deletefiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    11258 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_difffiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2320 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_doc_plugins.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      926 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_helpers.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4605 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_init_package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3431 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_init_project.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3094 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_package_status.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8779 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_prdiff.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5829 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_project_status.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    10407 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_repairwc.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    24512 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_request.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2307 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_results.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3277 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_revertfiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4891 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_setlinkrev.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8298 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_store.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    15545 2023-05-03 08:03:10.000000 osc-1.1.2/tests/test_update.py
```

### Comparing `osc-1.0.0/COPYING` & `osc-1.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/PKG-INFO` & `osc-1.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc
-Version: 1.0.0
+Version: 1.1.2
 Summary: openSUSE commander
 Home-page: http://en.opensuse.org/openSUSE:OSC
 Download-URL: https://github.com/openSUSE/osc
 Author: openSUSE project
 Author-email: opensuse-buildservice@opensuse.org
 License: GPLv2+
 Keywords: openSUSE,SUSE,RPM,build,buildservice,command-line
```

### Comparing `osc-1.0.0/README.md` & `osc-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/OscConfigParser.py` & `osc-1.1.2/osc/OscConfigParser.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/_private/__init__.py` & `osc-1.1.2/osc/_private/__init__.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/_private/api.py` & `osc-1.1.2/osc/_private/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -164,14 +164,27 @@
         "'": "&apos;",
     }
     if isinstance(string, bytes):
         return xml.sax.saxutils.escape(string.decode("utf-8"), entities=entities).encode("utf-8")
     return xml.sax.saxutils.escape(string, entities=entities)
 
 
+def xml_unescape(string):
+    """
+    Decode XML entities in the string.
+    """
+    entities = {
+        "&quot;": "\"",
+        "&apos;": "'",
+    }
+    if isinstance(string, bytes):
+        return xml.sax.saxutils.unescape(string.decode("utf-8"), entities=entities).encode("utf-8")
+    return xml.sax.saxutils.unescape(string, entities=entities)
+
+
 def xml_indent(root):
     """
     Indent XML so it looks pretty after printing or saving to file.
     """
     if hasattr(ET, "indent"):
         # ElementTree supports indent() in Python 3.9 and newer
         ET.indent(root)
```

### Comparing `osc-1.0.0/osc/_private/api_build.py` & `osc-1.1.2/osc/_private/api_build.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         limit: int = 0,
     ):
         self.apiurl = apiurl
         self.project = project
         self.package = package
         self.repository = repository
         self.arch = arch
-        self._limit = limit
+        self._limit = int(limit)
         self.entries = self._get_entries()
 
     def _get_entries(self):
         url_path = [
             "build",
             self.project,
             self.repository,
```

### Comparing `osc-1.0.0/osc/_private/api_source.py` & `osc-1.1.2/osc/_private/api_source.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/_private/common.py` & `osc-1.1.2/osc/_private/common.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/_private/package.py` & `osc-1.1.2/osc/_private/package.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/_private/request.py` & `osc-1.1.2/osc/_private/request.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/babysitter.py` & `osc-1.1.2/osc/babysitter.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from http.client import HTTPException, BadStatusLine
 from urllib.error import URLError, HTTPError
 
 import urllib3.exceptions
 
 from . import _private
 from . import commandline
+from . import conf as osc_conf
 from . import oscerr
 from .OscConfigParser import configparser
 from .oscssl import CertVerificationError
 from .util.cpio import CpioError
 from .util.helper import decode_it
 from .util.packagequery import PackageError
 
@@ -31,14 +32,22 @@
     from rpm import error as RPMError
 except:
     # if rpm-python isn't installed (we might be on a debian system):
     class RPMError(Exception):
         pass
 
 
+try:
+    from keyring.errors import KeyringLocked
+except ImportError:
+    # python-keyring is not installed
+    class KeyringLocked(Exception):
+        pass
+
+
 # the good things are stolen from Matt Mackall's mercurial
 
 
 def catchterm(*args):
     raise oscerr.SignalInterrupt
 
 
@@ -48,27 +57,29 @@
     if num:
         signal.signal(num, catchterm)
 
 
 def run(prg, argv=None):
     try:
         try:
-            if '--debugger' in sys.argv:
+            # we haven't parsed options yet, that's why we rely on argv directly
+            if "--debugger" in (argv or sys.argv[1:]):
                 pdb.set_trace()
-            # here we actually run the program:
-            return prg.main(argv)
+            # here we actually run the program
+            prg.main(argv)
+            return 0
         except:
-            # look for an option in the prg.options object and in the config
-            # dict print stack trace, if desired
-            if getattr(prg.options, 'traceback', None) or getattr(prg.conf, 'config', {}).get('traceback', None) or \
-               getattr(prg.options, 'post_mortem', None) or getattr(prg.conf, 'config', {}).get('post_mortem', None):
+            # If any of these was set via the command-line options,
+            # the config values are expected to be changed accordingly.
+            # That's why we're working only with the config.
+            if osc_conf.config["traceback"] or osc_conf.config["post_mortem"]:
                 traceback.print_exc(file=sys.stderr)
                 # we could use http://aspn.activestate.com/ASPN/Cookbook/Python/Recipe/52215
             # enter the debugger, if desired
-            if getattr(prg.options, 'post_mortem', None) or getattr(prg.conf, 'config', {}).get('post_mortem', None):
+            if osc_conf.config["post_mortem"]:
                 if sys.stdout.isatty() and not hasattr(sys, 'ps1'):
                     pdb.post_mortem(sys.exc_info()[2])
                 else:
                     print('sys.stdout is not a tty. Not jumping into pdb.', file=sys.stderr)
             raise
     except oscerr.SignalInterrupt:
         print('killed!', file=sys.stderr)
@@ -76,15 +87,15 @@
         print('interrupted!', file=sys.stderr)
         return 130
     except oscerr.UserAbort:
         print('aborted.', file=sys.stderr)
     except oscerr.APIError as e:
         print('BuildService API error:', e.msg, file=sys.stderr)
     except oscerr.LinkExpandError as e:
-        print('Link "%s/%s" cannot be expanded:\n' % (e.prj, e.pac), e.msg, file=sys.stderr)
+        print(f'Link "{e.prj}/{e.pac}" cannot be expanded:\n', e.msg, file=sys.stderr)
         print('Use "osc repairlink" to fix merge conflicts.\n', file=sys.stderr)
     except oscerr.WorkingCopyWrongVersion as e:
         print(e, file=sys.stderr)
     except oscerr.NoWorkingCopy as e:
         print(e, file=sys.stderr)
         if os.path.isdir('.git'):
             print("Current directory looks like git.", file=sys.stderr)
@@ -100,41 +111,40 @@
             print(e.osc_msg, file=sys.stderr)
 
         try:
             body = e.read()
         except AttributeError:
             body = ''
 
-        if getattr(prg.options, 'debug', None) or \
-           getattr(prg.conf, 'config', {}).get('debug', None):
+        if osc_conf.config["debug"]:
             print(e.hdrs, file=sys.stderr)
             print(body, file=sys.stderr)
 
         if e.code in [400, 403, 404, 500]:
             if b'<summary>' in body:
                 msg = body.split(b'<summary>')[1]
                 msg = msg.split(b'</summary>')[0]
-                msg = _private.api.xml_escape(msg)
+                msg = _private.api.xml_unescape(msg)
                 print(decode_it(msg), file=sys.stderr)
         if e.code >= 500 and e.code <= 599:
-            print('\nRequest: %s' % e.filename)
+            print(f'\nRequest: {e.filename}')
             print('Headers:')
             for h, v in e.hdrs.items():
                 if h != 'Set-Cookie':
-                    print("%s: %s" % (h, v))
+                    print(f"{h}: {v}")
 
     except BadStatusLine as e:
         print('Server returned an invalid response:', e, file=sys.stderr)
         print(e.line, file=sys.stderr)
     except HTTPException as e:
         print(e, file=sys.stderr)
     except URLError as e:
         msg = 'Failed to reach a server'
         if hasattr(e, '_osc_host_port'):
-            msg += ' (%s)' % e._osc_host_port
+            msg += f' ({e._osc_host_port})'
         msg += ':\n'
         print(msg, e.reason, file=sys.stderr)
     except ssl.SSLError as e:
         if 'tlsv1' in str(e):
             print('The python on this system or the server does not support TLSv1.2', file=sys.stderr)
         print("SSL Error:", e, file=sys.stderr)
     except OSError as e:
@@ -147,16 +157,15 @@
         print(e, file=sys.stderr)
     except (oscerr.ConfigError, oscerr.NoConfigfile) as e:
         print(e, file=sys.stderr)
     except configparser.Error as e:
         print(e.message, file=sys.stderr)
     except oscerr.OscIOError as e:
         print(e.msg, file=sys.stderr)
-        if getattr(prg.options, 'debug', None) or \
-           getattr(prg.conf, 'config', {}).get('debug', None):
+        if osc_conf.config["debug"]:
             print(e.e, file=sys.stderr)
     except (oscerr.WrongOptions, oscerr.WrongArgs) as e:
         print(e, file=sys.stderr)
         return 2
     except oscerr.ExtRuntimeError as e:
         print(e.file + ':', e.msg, file=sys.stderr)
     except oscerr.ServiceRuntimeError as e:
@@ -170,17 +179,19 @@
               'please file a bug and attach your current package working copy '
               'and the following traceback to it:', file=sys.stderr)
         print(e.msg, file=sys.stderr)
         traceback.print_exc(file=sys.stderr)
     except oscerr.PackageError as e:
         print(e.msg, file=sys.stderr)
     except PackageError as e:
-        print('%s:' % e.fname, e.msg, file=sys.stderr)
+        print(f'{e.fname}:', e.msg, file=sys.stderr)
     except RPMError as e:
         print(e, file=sys.stderr)
+    except KeyringLocked as e:
+        print(e, file=sys.stderr)
     except CertVerificationError as e:
         print(e, file=sys.stderr)
     except urllib3.exceptions.MaxRetryError as e:
         print(e.reason, file=sys.stderr)
     except CpioError as e:
         print(e, file=sys.stderr)
     except oscerr.OscBaseError as e:
@@ -203,10 +214,10 @@
     # support setvbuf - if setvbuf is not supported, the stream
     # remains fully buffered (see PyFile_SetBufSize
     # (Objects/fileobject.c))).
     if not os.isatty(sys.stdout.fileno()):
         sys.stdout = os.fdopen(sys.stdout.fileno(), sys.stdout.mode, 1)
         sys.stderr = os.fdopen(sys.stderr.fileno(), sys.stderr.mode, 1)
 
-    sys.exit(run(commandline.Osc()))
+    sys.exit(run(commandline.OscMainCommand()))
 
 # vim: sw=4 et
```

### Comparing `osc-1.0.0/osc/build.py` & `osc-1.1.2/osc/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,38 +452,29 @@
         print('WARNING: Unknown package type \'%s\'.' % buildtype, file=sys.stderr)
         b_built = ''
         s_built = ''
     return s_built, b_built
 
 
 def get_repo(path):
-    """Walks up path looking for any repodata directories.
+    """
+    Walks up path looking for any repodata directories.
 
     :param path: path to a directory
-    :return: path to repository directory containing repodata directory
+    :return: path to repository directory containing repodata directory with repomd.xml file
     :rtype: str
     """
-    oldDirectory = None
-    currentDirectory = os.path.abspath(path)
-    repositoryDirectory = None
-
-    # while there are still parent directories
-    while currentDirectory != oldDirectory:
-        children = os.listdir(currentDirectory)
-
-        if "repodata" in children:
-            repositoryDirectory = currentDirectory
-            break
-
-        # ascend
-        oldDirectory = currentDirectory
-        currentDirectory = os.path.abspath(os.path.join(oldDirectory,
-                                                        os.pardir))
 
-    return repositoryDirectory
+    for root, dirs, files in os.walk(path):
+        if not "repodata" in dirs:
+            continue
+        if "repomd.xml" in os.listdir(os.path.join(root, "repodata")):
+            return root
+    return None
+
 
 
 def get_prefer_pkgs(dirs, wanted_arch, type, cpio):
     paths = []
     repositories = []
 
     suffix = '*.rpm'
@@ -1053,14 +1044,17 @@
     if opts.stage:
         buildargs.append('--stage')
         buildargs.append(opts.stage)
 
     if opts.build_opt:
         buildargs += opts.build_opt
 
+    if opts.buildtool_opt:
+        buildargs += [f"--buildtool-opt={opt}" for opt in opts.buildtool_opt]
+
     # real arch of this machine
     # vs.
     # arch we are supposed to build for
     if vm_type != "emulator" and vm_type != "qemu":
         if bi.hostarch is not None:
             if hostarch != bi.hostarch and bi.hostarch not in can_also_build.get(hostarch, []):
                 print('Error: hostarch \'%s\' is required.' % (bi.hostarch), file=sys.stderr)
```

### Comparing `osc-1.0.0/osc/checker.py` & `osc-1.1.2/osc/checker.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/cmdln.py` & `osc-1.1.2/osc/cmdln.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,17 @@
     return decorate
 
 
 class HelpFormatter(argparse.RawDescriptionHelpFormatter):
     def _format_action(self, action):
         if isinstance(action, argparse._SubParsersAction):
             parts = []
-            for i in action._get_subactions():
+            subactions = action._get_subactions()
+            subactions.sort(key=lambda x: x.metavar)
+            for i in subactions:
                 if i.help == argparse.SUPPRESS:
                     # don't display commands with suppressed help
                     continue
                 if len(i.metavar) > 20:
                     parts.append("%*s%-21s" % (self._current_indent, "", i.metavar))
                     parts.append("%*s %s" % (self._current_indent + 21, "", i.help))
                 else:
```

### Comparing `osc-1.0.0/osc/commandline.py` & `osc-1.1.2/osc/commandline.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 # This program is free software; it may be used, copied, modified
 # and distributed under the terms of the GNU General Public Licence,
 # either version 2, or version 3 (at your option).
 
 import argparse
 import getpass
 import glob
+import importlib
 import importlib.util
 import inspect
 import os
+import pkgutil
 import re
 import subprocess
 import sys
 import textwrap
 import tempfile
 import time
 import traceback
@@ -22,37 +24,541 @@
 from typing import List
 from urllib.parse import urlsplit
 from urllib.error import HTTPError
 
 from . import _private
 from . import build as osc_build
 from . import cmdln
+from . import commands as osc_commands
 from . import conf
 from . import oscerr
 from . import store as osc_store
 from .core import *
 from .grabber import OscFileGrabber
 from .meter import create_text_meter
 from .util import cpio, rpmquery, safewriter
 from .util.helper import _html_escape, format_table
 
 
+class Command:
+    #: Name of the command as used in the argument parser.
+    name: str = None
+
+    #: Optional aliases to the command.
+    aliases: List[str] = []
+
+    #: Whether the command is hidden from help.
+    #: Defaults to ``False``.
+    hidden: bool = False
+
+    #: Name of the parent command class.
+    #: Can be prefixed if the parent comes from a different location,
+    #: for example ``osc.commands.<ClassName>`` when extending osc command with a plugin.
+    #: See ``OscMainCommand.MODULES`` for available prefixes.
+    parent: str = None
+
+    def __init__(self, full_name, parent=None):
+        self.full_name = full_name
+        self.parent = parent
+        self.subparsers = None
+
+        if not self.name:
+            raise ValueError(f"Command '{self.full_name}' has no 'name' set")
+
+        if parent:
+            self.parser = self.parent.subparsers.add_parser(
+                self.name,
+                aliases=self.aliases,
+                help=self.get_help(),
+                description=self.get_description(),
+                formatter_class=cmdln.HelpFormatter,
+                conflict_handler="resolve",
+                prog=f"{self.main_command.name} [global opts] {self.name}",
+            )
+            self.parser.set_defaults(_selected_command=self)
+        else:
+            self.parser = argparse.ArgumentParser(
+                prog=self.name,
+                description=self.get_description(),
+                formatter_class=cmdln.HelpFormatter,
+                usage="%(prog)s [global opts] <command> [--help] [opts] [args]",
+            )
+
+        # traverse the parent commands and add their options to the current command
+        commands = []
+        cmd = self
+        while cmd:
+            commands.append(cmd)
+            cmd = cmd.parent
+        # iterating backwards to give the command's options a priority over parent/global options
+        for cmd in reversed(commands):
+            cmd.init_arguments()
+
+    def __repr__(self):
+        return f"<osc plugin {self.full_name} at {self.__hash__():#x}>"
+
+    def get_help(self):
+        """
+        Return the help text of the command.
+        The first line of the docstring is returned by default.
+        """
+        if self.hidden:
+            return argparse.SUPPRESS
+
+        if not self.__doc__:
+            return ""
+
+        help_lines = self.__doc__.strip().splitlines()
+
+        if not help_lines:
+            return ""
+
+        return help_lines[0]
+
+    def get_description(self):
+        """
+        Return the description of the command.
+        The docstring without the first line is returned by default.
+        """
+        if not self.__doc__:
+            return ""
+
+        help_lines = self.__doc__.strip().splitlines()
+
+        if not help_lines:
+            return ""
+
+        # skip the first line that contains help text
+        help_lines.pop(0)
+
+        # remove any leading empty lines
+        while help_lines and not help_lines[0]:
+            help_lines.pop(0)
+
+        result = "\n".join(help_lines)
+        result = textwrap.dedent(result)
+        return result
+
+    @property
+    def main_command(self):
+        """
+        Return reference to the main command that represents the executable
+        and contains the main instance of ArgumentParser.
+        """
+        if not self.parent:
+            return self
+        return self.parent.main_command
+
+    def add_argument(self, *args, **kwargs):
+        """
+        Add a new argument to the command's argument parser.
+        See `argparse <https://docs.python.org/3/library/argparse.html>`_ documentation for allowed parameters.
+        """
+        cmd = self
+
+        # Let's inspect if the caller was init_arguments() method.
+        # In such case use the "parser" argument if specified.
+        frame_1 = inspect.currentframe().f_back
+        frame_1_info = inspect.getframeinfo(frame_1)
+        frame_2 = frame_1.f_back
+        frame_2_info = inspect.getframeinfo(frame_2)
+        if (frame_1_info.function, frame_2_info.function) == ("init_arguments", "__init__"):
+            # this method was called from init_arguments() that was called from __init__
+            # let's extract the command class from the 2nd frame and ad arguments there
+            cmd = frame_2.f_locals["self"]
+
+            # suppress global options from command help
+            if cmd != self and not self.parent:
+                kwargs["help"] = argparse.SUPPRESS
+
+            # We're adding hidden options from parent commands to their subcommands to allow
+            # option intermixing. For all such added hidden options we need to suppress their
+            # defaults because they would override any option set in the parent command.
+            if cmd != self:
+                kwargs["default"] = argparse.SUPPRESS
+
+        cmd.parser.add_argument(*args, **kwargs)
+
+    def init_arguments(self):
+        """
+        Override to add arguments to the argument parser.
+
+        .. note::
+            Make sure you're adding arguments only by calling ``self.add_argument()``.
+            Using ``self.parser.add_argument()`` directly is not recommended
+            because it disables argument intermixing.
+        """
+
+    def run(self, args):
+        """
+        Override to implement the command functionality.
+
+        .. note::
+            ``args.positional_args`` is a list containing any unknown (unparsed) positional arguments.
+
+        .. note::
+            Consider moving any reusable code into a library,
+            leaving the command-line code only a thin wrapper on top of it.
+
+            If the code is generic enough, it should be added to osc directly.
+            In such case don't hesitate to open an `issue <https://github.com/openSUSE/osc/issues>`_.
+        """
+        raise NotImplementedError()
+
+    def register(self, command_class, command_full_name):
+        if not self.subparsers:
+            # instantiate subparsers on first use
+            self.subparsers = self.parser.add_subparsers(dest="command", title="commands")
+
+        # Check for parser conflicts.
+        # This is how Python 3.11+ behaves by default.
+        if command_class.name in self.subparsers._name_parser_map:
+            raise argparse.ArgumentError(self.subparsers, f"conflicting subparser: {command_class.name}")
+        for alias in command_class.aliases:
+            if alias in self.subparsers._name_parser_map:
+                raise argparse.ArgumentError(self.subparsers, f"conflicting subparser alias: {alias}")
+
+        command = command_class(command_full_name, parent=self)
+        return command
+
+
+class MainCommand(Command):
+    MODULES = ()
+
+    def __init__(self):
+        super().__init__(self.__class__.__name__)
+        self.command_classes = {}
+        self.download_progress = None
+
+    def post_parse_args(self, args):
+        pass
+
+    def run(self, args):
+        cmd = getattr(args, "_selected_command", None)
+        if not cmd:
+            self.parser.error("Please specify a command")
+        self.post_parse_args(args)
+        cmd.run(args)
+
+    def load_command(self, cls, module_prefix):
+        mod_cls_name = f"{module_prefix}.{cls.__name__}"
+        parent_name = getattr(cls, "parent", None)
+        if parent_name:
+            # allow relative references to classes in the the same module/directory
+            if "." not in parent_name:
+                parent_name = f"{module_prefix}.{parent_name}"
+            try:
+                parent = self.main_command.command_classes[parent_name]
+            except KeyError:
+                msg = f"Failed to load command class '{mod_cls_name}' because it references parent '{parent_name}' that doesn't exist"
+                print(msg, file=sys.stderr)
+                return None
+            cmd = parent.register(cls, mod_cls_name)
+        else:
+            cmd = self.main_command.register(cls, mod_cls_name)
+
+        cmd.full_name = mod_cls_name
+        self.main_command.command_classes[mod_cls_name] = cmd
+        return cmd
+
+    def load_commands(self):
+        for module_prefix, module_path in self.MODULES:
+            module_path = os.path.expanduser(module_path)
+
+            # some plugins have their modules installed next to them instead of site-packages
+            if module_path not in sys.path:
+                sys.path.append(module_path)
+
+            for loader, module_name, _ in pkgutil.iter_modules(path=[module_path]):
+                full_name = f"{module_prefix}.{module_name}"
+                spec = loader.find_spec(full_name)
+                mod = importlib.util.module_from_spec(spec)
+                try:
+                    spec.loader.exec_module(mod)
+                except Exception as e:  # pylint: disable=broad-except
+                    msg = f"Failed to load commands from module '{full_name}': {e}"
+                    print(msg, file=sys.stderr)
+                    continue
+                for name in dir(mod):
+                    if name.startswith("_"):
+                        continue
+                    cls = getattr(mod, name)
+                    if not inspect.isclass(cls):
+                        continue
+                    if not issubclass(cls, Command):
+                        continue
+                    if cls.__module__ != full_name:
+                        # skip classes that weren't defined directly in the loaded plugin module
+                        continue
+                    self.load_command(cls, module_prefix)
+
+    def parse_args(self, *args, **kwargs):
+        namespace, unknown_args = self.parser.parse_known_args(*args, **kwargs)
+
+        unrecognized = [i for i in unknown_args if i.startswith("-")]
+        if unrecognized:
+            self.parser.error(f"unrecognized arguments: " + " ".join(unrecognized))
+
+        namespace.positional_args = list(unknown_args)
+        return namespace
+
+
+class OscCommand(Command):
+    """
+    Inherit from this class to create new commands.
+
+    The first line of the docstring becomes the help text,
+    the remaining lines become the command description.
+    """
+
+
+class OscMainCommand(MainCommand):
+    name = "osc"
+
+    MODULES = (
+        ("osc.commands", osc_commands.__path__[0]),
+        ("osc.commands.usr_lib", "/usr/lib/osc-plugins"),
+        ("osc.commands.usr_local_lib", "/usr/local/lib/osc-plugins"),
+        ("osc.commands.home_local_lib", "~/.local/lib/osc-plugins"),
+        ("osc.commands.home", "~/.osc-plugins"),
+    )
+
+    def __init__(self):
+        super().__init__()
+        self.args = None
+        self.download_progress = None
+
+    def init_arguments(self):
+        self.add_argument(
+            "-v",
+            "--verbose",
+            action="store_true",
+            help="increase verbosity",
+        )
+        self.add_argument(
+            "-q",
+            "--quiet",
+            action="store_true",
+            help="be quiet, not verbose",
+        )
+        self.add_argument(
+            "--debug",
+            action="store_true",
+            help="print info useful for debugging",
+        )
+        self.add_argument(
+            "--debugger",
+            action="store_true",
+            help="jump into the debugger before executing anything",
+        )
+        self.add_argument(
+            "--post-mortem",
+            action="store_true",
+            help="jump into the debugger in case of errors",
+        )
+        self.add_argument(
+            "--traceback",
+            action="store_true",
+            help="print call trace in case of errors",
+        )
+        self.add_argument(
+            "-H",
+            "--http-debug",
+            action="store_true",
+            help="debug HTTP traffic (filters some headers)",
+        )
+        self.add_argument(
+            "--http-full-debug",
+            action="store_true",
+            help="debug HTTP traffic (filters no headers)",
+        )
+        self.add_argument(
+            "-A",
+            "--apiurl",
+            metavar="URL",
+            help="Open Build Service API URL or a configured alias",
+        )
+        self.add_argument(
+            "--config",
+            dest="conffile",
+            metavar="FILE",
+            help="specify alternate configuration file",
+        )
+        self.add_argument(
+            "--no-keyring",
+            action="store_true",
+            help="disable usage of desktop keyring system",
+        )
+
+    def post_parse_args(self, args):
+        # apiurl hasn't been specified by the user
+        # we need to set it here because the 'default' option of an argument doesn't support lazy evaluation
+        if args.apiurl is None:
+            try:
+                # try reading the apiurl from the working copy
+                args.apiurl = osc_store.Store(Path.cwd()).apiurl
+            except oscerr.NoWorkingCopy:
+                # we can't use conf.config["apiurl"] because it contains the default "https://api.opensuse.org"
+                # let's leave setting the right value to conf.get_config()
+                pass
+
+        try:
+            conf.get_config(
+                override_apiurl=args.apiurl,
+                override_conffile=args.conffile,
+                override_debug=args.debug,
+                override_http_debug=args.http_debug,
+                override_http_full_debug=args.http_full_debug,
+                override_no_keyring=args.no_keyring,
+                override_post_mortem=args.post_mortem,
+                override_traceback=args.traceback,
+                override_verbose=args.verbose,
+            )
+        except oscerr.NoConfigfile as e:
+            print(e.msg, file=sys.stderr)
+            print(f"Creating osc configuration file {e.file} ...", file=sys.stderr)
+            conf.interactive_config_setup(e.file, args.apiurl)
+            print("done", file=sys.stderr)
+            self.post_parse_args(args)
+        except oscerr.ConfigMissingApiurl as e:
+            print(e.msg, file=sys.stderr)
+            conf.interactive_config_setup(e.file, e.url, initial=False)
+            self.post_parse_args(args)
+        except oscerr.ConfigMissingCredentialsError as e:
+            print(e.msg, file=sys.stderr)
+            print("Please enter new credentials.", file=sys.stderr)
+            conf.interactive_config_setup(e.file, e.url, initial=False)
+            self.post_parse_args(args)
+
+        # write config values back to args
+        # this is crucial mainly for apiurl to resolve an alias to full url
+        for i in ["apiurl", "debug", "http_debug", "http_full_debug", "post_mortem", "traceback", "verbose"]:
+            setattr(args, i, conf.config[i])
+        args.no_keyring = not conf.config["use_keyring"]
+
+        if conf.config["show_download_progress"]:
+            self.download_progress = create_text_meter()
+
+        if not args.apiurl:
+            self.parser.error("Could not determine apiurl, use -A/--apiurl to specify one")
+
+        # needed for LegacyOsc class
+        self.args = args
+
+    def _wrap_legacy_command(self, func_):
+        class LegacyCommandWrapper(Command):
+            func = func_
+            __doc__ = getattr(func_, "__doc__", "")
+            aliases = getattr(func_, "aliases", [])
+            hidden = getattr(func_, "hidden", False)
+            name = getattr(func_, "name", func_.__name__[3:])
+
+            def __repr__(self):
+                result = super().__repr__()
+                result += f"({self.func.__name__})"
+                return result
+
+            def init_arguments(self):
+                options = getattr(self.func, "options", [])
+                for option_args, option_kwargs in options:
+                    self.add_argument(*option_args, **option_kwargs)
+
+            def run(self, args):
+                sig = inspect.signature(self.func)
+                arg_names = list(sig.parameters.keys())
+                if arg_names == ["subcmd", "opts"]:
+                    # handler doesn't take positional args via *args
+                    if args.positional_args:
+                        self.parser.error(f"unrecognized arguments: " + " ".join(args.positional_args))
+                    self.func(args.command, args)
+                else:
+                    # handler takes positional args via *args
+                    self.func(args.command, args, *args.positional_args)
+
+        return LegacyCommandWrapper
+
+    def load_legacy_commands(self):
+        # lazy links of attributes that would normally be initialized in the instance of Osc class
+        class LegacyOsc(Osc):  # pylint: disable=used-before-assignment
+            # pylint: disable=no-self-argument
+            @property
+            def argparser(self_):
+                return self.parser
+
+            # pylint: disable=no-self-argument
+            @property
+            def download_progress(self_):
+                return self.download_progress
+
+            # pylint: disable=no-self-argument
+            @property
+            def options(self_):
+                return self.args
+
+            # pylint: disable=no-self-argument
+            @options.setter
+            def options(self_, value):
+                pass
+
+            # pylint: disable=no-self-argument
+            @property
+            def subparsers(self_):
+                return self.subparsers
+
+        osc_instance = LegacyOsc()
+
+        for name in dir(osc_instance):
+            if not name.startswith("do_"):
+                continue
+
+            func = getattr(osc_instance, name)
+
+            if not inspect.ismethod(func) and not inspect.isfunction(func):
+                continue
+
+            cls = self._wrap_legacy_command(func)
+            self.load_command(cls, "osc.commands.old")
+
+    @classmethod
+    def main(cls, argv=None, run=True):
+        """
+        Initialize OscMainCommand, load all commands and run the selected command.
+        """
+        cmd = cls()
+        cmd.load_commands()
+        cmd.load_legacy_commands()
+        if run:
+            args = cmd.parse_args(args=argv)
+            cmd.run(args)
+        else:
+            args = None
+        return cmd, args
+
+
+def get_parser():
+    """
+    Needed by argparse-manpage to generate man pages from the argument parser.
+    """
+    main, _ = OscMainCommand.main(run=False)
+    return main.parser
+
+
+# ================================================================================
+# The legacy code follows.
+# Please do not use it if possible.
+# ================================================================================
+
+
 HELP_MULTIBUILD_MANY = """Only work with the specified flavors of a multibuild package.
 Globs are resolved according to _multibuild file from server.
 Empty string is resolved to a package without a flavor."""
 
 HELP_MULTIBUILD_ONE = "Only work with the specified flavor of a multibuild package."
 
 
-def get_parser():
-    osc = Osc()
-    osc.create_argparser()
-    return osc.argparser
-
-
 def pop_args(
     args,
     arg1_name: str = None,
     arg1_is_optional: bool = False,
     arg1_default: str = None,
     arg2_name: str = None,
     arg2_is_optional: bool = False,
@@ -431,15 +937,14 @@
     * http://en.opensuse.org/openSUSE:Build_Service_Tutorial
     * http://en.opensuse.org/openSUSE:OSC
 
     You can modify osc commands, or roll your own, via the plugin API:
     * http://en.opensuse.org/openSUSE:OSC_plugins
     """
     name = 'osc'
-    conf = None
 
     def __init__(self):
         self.options = None
         self._load_plugins()
         sys.stderr = safewriter.SafeWriter(sys.stderr)
         sys.stdout = safewriter.SafeWriter(sys.stdout)
 
@@ -819,15 +1324,15 @@
                             print("%9d %s %-40s" % (f.size, shorttime(f.mtime), f.name))
                 else:
                     for f in result[1]:
                         print(indent + f)
 
         # list sources
         elif not opts.binaries:
-            if not args:
+            if not args or not project:
                 for prj in meta_get_project_list(apiurl, opts.deleted):
                     print(prj)
 
             elif len(args) == 1:
                 for pkg in meta_get_packagelist(apiurl, project, deleted=opts.deleted, expand=opts.expand):
                     print(pkg)
 
@@ -1885,35 +2390,14 @@
                 change_request_state(apiurl, req.reqid, 'superseded',
                                      'superseded by %s' % result, result)
 
         if opts.supersede:
             change_request_state(apiurl, opts.supersede, 'superseded',
                                  opts.message or '', result)
 
-    def _actionparser(self, opt_str, value, parser):
-        value = []
-        if not hasattr(parser.values, 'actiondata'):
-            setattr(parser.values, 'actiondata', [])
-        if parser.values.actions is None:
-            parser.values.actions = []
-
-        rargs = parser.rargs
-        while rargs:
-            arg = rargs[0]
-            if ((arg[:2] == "--" and len(arg) > 2) or
-                    (arg[:1] == "-" and len(arg) > 1 and arg[1] != "-")):
-                break
-            else:
-                value.append(arg)
-                del rargs[0]
-
-        parser.values.actions.append(value[0])
-        del value[0]
-        parser.values.actiondata.append(slash_split(value))
-
     def _submit_request(self, args, opts, options_block):
         actionxml = ""
         apiurl = self.get_api_url()
         if len(args) == 0 and is_project_dir(Path.cwd()):
             # submit requests for multiple packages are currently handled via multiple requests
             # They could be also one request with multiple actions, but that avoids to accepts parts of it.
             project = store_read_project(Path.cwd())
@@ -2179,17 +2663,16 @@
             actionxml = """ <action type="set_bugowner"> <target project="%s" %s /> <person name="%s" /> </action> """ % \
                 (project, package, user)
             if get_user_meta(apiurl, user) is None:
                 raise oscerr.WrongArgs('osc: an error occured.')
 
         return actionxml
 
-# TODO: fix ValueError: unknown action "callback"
-#    @cmdln.option('-a', '--action', action='callback', callback = _actionparser, dest = 'actions',
-#                  help='specify action type of a request, can be : submit/delete/change_devel/add_role/set_bugowner')
+    @cmdln.option('-a', '--action', action='append', nargs='+', metavar=('ACTION', '[ARGS]'), dest='actions', default=[],
+                  help='specify action type of a request, can be : submit/delete/change_devel/add_role/set_bugowner')
     @cmdln.option('-m', '--message', metavar='TEXT',
                   help='specify message TEXT')
     @cmdln.option('-r', '--revision', metavar='REV',
                   help='for "create", specify a certain source revision ID (the md5 sum)')
     @cmdln.option('-s', '--supersede', metavar='REQUEST_ID',
                   help='Superseding another request by this one')
     @cmdln.option('--nodevelproject', action='store_true',
@@ -2239,50 +2722,37 @@
         if src_update:
             options_block = """<options><sourceupdate>%s</sourceupdate></options> """ % (src_update)
 
         args = slash_split(args)
 
         apiurl = self.get_api_url()
 
-        i = 0
         actionsxml = ""
         supersede = set()
-        for ai in opts.actions:
-            if ai == 'submit':
-                args = opts.actiondata[i]
-                i = i + 1
+        for actiondata in opts.actions:
+            action = actiondata[0]
+            args = actiondata[1:]
+            if action == 'submit':
                 actions, to_supersede = self._submit_request(args, opts, options_block)
                 actionsxml += actions
                 supersede.update(to_supersede)
-            elif ai == 'delete':
-                args = opts.actiondata[i]
+            elif action == 'delete':
                 actionsxml += self._delete_request(args, opts)
-                i = i + 1
-            elif ai == 'change_devel':
-                args = opts.actiondata[i]
+            elif action == 'change_devel':
                 actionsxml += self._changedevel_request(args, opts)
-                i = i + 1
-            elif ai == 'add_me':
-                args = opts.actiondata[i]
+            elif action == 'add_me':
                 actionsxml += self._add_me(args, opts)
-                i = i + 1
-            elif ai == 'add_group':
-                args = opts.actiondata[i]
+            elif action == 'add_group':
                 actionsxml += self._add_group(args, opts)
-                i = i + 1
-            elif ai == 'add_role':
-                args = opts.actiondata[i]
+            elif action == 'add_role':
                 actionsxml += self._add_user(args, opts)
-                i = i + 1
-            elif ai == 'set_bugowner':
-                args = opts.actiondata[i]
+            elif action == 'set_bugowner':
                 actionsxml += self._set_bugowner(args, opts)
-                i = i + 1
             else:
-                raise oscerr.WrongArgs('Unsupported action %s' % ai)
+                raise oscerr.WrongArgs(f"Unsupported action {action}")
         if actionsxml == "":
             sys.exit('No actions need to be taken.')
 
         if not opts.message:
             opts.message = edit_message()
 
         xml = """<request> %s <state name="new"/> <description>%s</description> </request> """ % \
@@ -4172,17 +4642,18 @@
             rev1, rev2 = parseRevisionOption(opts.revision)
         diff = b''
         for pac in pacs:
             if not rev2:
                 for i in pac.get_diff(rev1):
                     diff += b''.join(i)
             else:
+                files = args
                 diff += server_diff_noex(pac.apiurl, pac.prjname, pac.name, rev1,
                                          pac.prjname, pac.name, rev2,
-                                         not opts.plain, opts.missingok, opts.meta, not opts.unexpand)
+                                         not opts.plain, opts.missingok, opts.meta, not opts.unexpand, files=files)
         run_pager(diff)
 
     @cmdln.option('--issues-only', action='store_true',
                   help='show only issues in diff')
     @cmdln.option('-M', '--meta', action='store_true',
                         help='diff meta data')
     @cmdln.option('-r', '--revision', metavar='N[:M]',
@@ -6001,14 +6472,16 @@
         Show the packages that require the specified package during the build
 
         The command whatdependson can be used to find out what will be triggered when
         a certain package changes.
 
         This is no guarantee, since the new build might have changed dependencies.
 
+        The packages marked with the [i] flag are inherited to the project.
+
         The arguments REPOSITORY and ARCH can be taken from the first two columns
         of the 'osc repos' output.
 
         usage in package or project directory:
             osc whatdependson REPOSITORY ARCH
 
         usage:
@@ -6045,21 +6518,23 @@
 
         if len(args) == 4:
             project = self._process_project_name(args[0])
             packages = [args[1]]
             repository = args[2]
             arch = args[3]
 
+        project_packages = meta_get_packagelist(apiurl, project, deleted=False, expand=False)
         xml = get_dependson(apiurl, project, repository, arch, packages, reverse)
 
         root = ET.fromstring(xml)
         for package in root.findall('package'):
             print(package.get('name'), ":")
             for dep in package.findall('pkgdep'):
-                print("  ", dep.text)
+                inherited = "   " if dep.text in project_packages else "[i]"
+                print(f"  {inherited} {dep.text}")
 
     @cmdln.option('--alternative-project', metavar='PROJECT',
                   help='specify the build target project')
     @cmdln.option('-d', '--debug', action='store_true', dest="debug_dependencies",
                   help='verbose output of build dependencies')
     @cmdln.option('-M', '--multibuild-package', metavar='FLAVOR',
                   help=HELP_MULTIBUILD_ONE)
@@ -6538,14 +7013,16 @@
                   help='enable feature X for build')
     @cmdln.option('--without', metavar='X', action='append',
                   help='disable feature X for build')
     @cmdln.option('--define', metavar='\'X Y\'', action='append',
                   help='define macro X with value Y')
     @cmdln.option('--build-opt', metavar='OPT', action='append',
                   help='pass option OPT to the build command')
+    @cmdln.option('--buildtool-opt', metavar='OPT', action='append',
+                  help='pass option OPT to the build tool command (rpmbuild)')
     @cmdln.option('--userootforbuild', '--login-as-root', action='store_true',
                   help='Run build or shell as root. The default is to build as '
                   'unprivileged user. Note that a line "# norootforbuild" '
                   'in the spec file will invalidate this option.')
     @cmdln.option('--build-uid', metavar='uid:gid|"caller"',
                   help='specify the numeric uid:gid pair to assign to the '
                   'unprivileged "abuild" user or use "caller" to use the current user uid:gid')
@@ -6907,15 +7384,15 @@
             if ret != 0:
                 return ret
 
         return build_ret
 
     @cmdln.option('', '--csv', action='store_true',
                   help='generate output in CSV (separated by |)')
-    @cmdln.option('-l', '--limit', metavar='limit',
+    @cmdln.option('-l', '--limit', metavar='limit', type=int, default=0,
                         help='for setting the number of results')
     @cmdln.option('-M', '--multibuild-package', metavar='FLAVOR',
                   help=HELP_MULTIBUILD_ONE)
     @cmdln.alias('buildhist')
     def do_buildhistory(self, subcmd, opts, *args):
         """
         Shows the build history of a package
@@ -9477,15 +9954,14 @@
             result = delete_comment(apiurl, args[1])
             print(result)
 
     def _load_plugins(self):
         plugin_dirs = [
             '/usr/lib/osc-plugins',
             '/usr/local/lib/osc-plugins',
-            '/var/lib/osc-plugins',  # Kept for backward compatibility
             os.path.expanduser('~/.local/lib/osc-plugins'),
             os.path.expanduser('~/.osc-plugins')]
         for plugin_dir in plugin_dirs:
             if not os.path.isdir(plugin_dir):
                 continue
             sys.path.append(plugin_dir)
             for extfile in os.listdir(plugin_dir):
```

### Comparing `osc-1.0.0/osc/conf.py` & `osc-1.1.2/osc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -768,16 +768,16 @@
 
     # make sure it is not world readable, it may contain a password.
     conffile_stat = os.stat(conffile)
     if conffile_stat.st_mode != 0o600:
         try:
             os.chmod(conffile, 0o600)
         except OSError as e:
-            if e.errno == errno.EROFS:
-                print('Warning: file \'%s\' may have an insecure mode.', conffile)
+            if e.errno in (errno.EROFS, errno.EPERM):
+                print(f"Warning: Configuration file '{conffile}' may have insecure file permissions.")
             else:
                 raise e
 
     cp = get_configParser(conffile)
 
     if not cp.has_section('general'):
         # FIXME: it might be sufficient to just assume defaults?
@@ -886,15 +886,15 @@
             api_host_options[apiurl]['downloadurl'] = None
 
         if api_host_options[apiurl]['sshkey'] is None:
             api_host_options[apiurl]['sshkey'] = config['sshkey']
 
         api_host_options[apiurl]["disable_hdrmd5_check"] = config["disable_hdrmd5_check"]
         if cp.has_option(url, "disable_hdrmd5_check"):
-            api_host_options[apiurl][key] = cp.getboolean(url, "disable_hdrmd5_check")
+            api_host_options[apiurl]["disable_hdrmd5_check"] = cp.getboolean(url, "disable_hdrmd5_check")
 
     # add the auth data we collected to the config dict
     config['api_host_options'] = api_host_options
     config['apiurl_aliases'] = aliases
 
     apiurl = aliases.get(config['apiurl'], config['apiurl'])
     config['apiurl'] = urljoin(*parse_apisrv_url(None, apiurl))
@@ -968,28 +968,34 @@
     else:
         conffile = '~/.config/osc/oscrc'
 
     return conffile
 
 
 def interactive_config_setup(conffile, apiurl, initial=True):
+    if not apiurl:
+        apiurl = DEFAULTS["apiurl"]
+
     scheme = urlsplit(apiurl)[0]
     http = scheme == "http"
     if http:
         msg = "The apiurl '{apiurl}' uses HTTP protocol without any encryption.\n"
         msg += "All communication incl. sending your password WILL NOT BE ENCRYPTED!\n"
         msg += "Do you really want to continue with no encryption?\n"
         print(msg.format(apiurl=apiurl), file=sys.stderr)
         yes = raw_input("Type 'YES' to continue: ")
         if yes != "YES":
             raise oscerr.UserAbort()
         print()
 
-    user = raw_input('Username: ')
-    passwd = getpass.getpass()
+    apiurl_no_scheme = urlsplit(apiurl)[1]
+    user_prompt = f"Username [{apiurl_no_scheme}]: "
+    user = raw_input(user_prompt)
+    pass_prompt = f"Password [{user}@{apiurl_no_scheme}]: "
+    passwd = getpass.getpass(pass_prompt)
     creds_mgr_descr = select_credentials_manager_descr()
     if initial:
         config = {'user': user, 'pass': passwd}
         if apiurl:
             config['apiurl'] = apiurl
         if http:
             config['allow_http'] = 1
```

### Comparing `osc-1.0.0/osc/connection.py` & `osc-1.1.2/osc/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,28 +131,28 @@
 
 
 def http_request_wrap_file(func):
     """
     Turn file path into a file object and close it automatically
     by using a context manager.
     """
-    def new_func(method, url, headers=None, data=None, file=None):
+    def new_func(method, url, headers=None, data=None, file=None, retry_on_400: bool = True):
         if file:
             with open(file, "rb") as f:
-                return func(method, url, headers, data, file=f)
+                return func(method, url, headers, data, f, retry_on_400)
         else:
-            return func(method, url, headers, data, file)
+            return func(method, url, headers, data, file, retry_on_400)
 
     new_func.__name__ = func.__name__
     new_func.__doc__ = func.__doc__
     return new_func
 
 
 @http_request_wrap_file
-def http_request(method: str, url: str, headers=None, data=None, file=None):
+def http_request(method: str, url: str, headers=None, data=None, file=None, retry_on_400: bool = True):
     """
     Send a HTTP request to a server.
 
     Features:
     * Authentication ([apiurl]/{user,pass} in oscrc)
     * Session cookie support (~/.local/state/osc/cookiejar)
     * SSL certificate verification incl. managing trusted certs
@@ -164,14 +164,15 @@
     * Connection debugging (-H/--http-debug, --http-full-debug)
 
     :param method: HTTP request method (such as GET, POST, PUT, DELETE).
     :param url: The URL to perform the request on.
     :param headers: Dictionary of custom headers to send.
     :param data: Data to send in the request body (conflicts with `file`).
     :param file: Path to a file to send as data in the request body (conflicts with `data`).
+    :param retry_on_400: Whether to retry on receiving HTTP status code 400.
     """
 
     purl = urllib3.util.parse_url(url)
     apiurl = conf.extract_known_apiurl(url)
     headers = urllib3.response.HTTPHeaderDict(headers or {})
 
     # identify osc
@@ -223,17 +224,32 @@
         sig = inspect.signature(urllib3.Retry)
         arg_names = list(sig.parameters.keys())
         if "allowed_methods" in arg_names:
             retries_kwargs = {"allowed_methods": None}
         else:
             retries_kwargs = {"method_whitelist": None}
 
+
+        status_forcelist = (
+            500,  # Internal Server Error
+            502,  # Bad Gateway
+            503,  # Service Unavailable
+            504,  # Gateway Timeout
+        )
+        if retry_on_400:
+            status_forcelist = (
+                400,  # Bad Request; retry on 400: service in progress
+            ) + status_forcelist
+
         pool_kwargs["retries"] = urllib3.Retry(
             total=int(conf.config["http_retries"]),
             backoff_factor=2,
+            status_forcelist=status_forcelist,
+            # don't raise because we want an actual response rather than a MaxRetryError with "too many <status_code> error responses" message
+            raise_on_status=False,
             **retries_kwargs,
         )
 
         if purl.scheme == "https":
             ssl_context = oscssl.create_ssl_context()
             ssl_context.load_default_certs()
             # turn cert verification off if sslcertck = 0
@@ -284,17 +300,18 @@
         if success:
             break
 
     # Rails sends a html response if the header is not set
     # https://github.com/openSUSE/open-build-service/pull/13019
     headers.add("Accept", "application/xml")
 
-    if data or file:
-        # osc/obs data is usually XML
+    if method == "PUT" or (method == "POST" and (data or file)):
         headers.add("Content-Type", "application/xml; charset=utf-8")
+    elif method == "POST":
+        headers.add("Content-Type", "application/x-www-form-urlencoded")
 
     if purl.scheme == "http" and HTTP_PROXY_MANAGER:
         # HTTP proxy requires full URL with 'same host' checking off
         urlopen_url = url
         assert_same_host = False
     else:
         # everything else is fine with path only
```

### Comparing `osc-1.0.0/osc/core.py` & `osc-1.1.2/osc/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # __store_version__ is to be incremented when the format of the working copy
 # "store" changes in an incompatible way. Please add any needed migration
 # functionality to check_store_version().
 __store_version__ = '1.0'
 
 
 import codecs
+import copy
 import datetime
 import difflib
 import errno
 import fnmatch
 import glob
 import hashlib
 import locale
@@ -440,16 +441,18 @@
             except FileExistsError:
                 time.sleep(1)
 
             if i == 0:
                 msg = f'"{old_dir}" exists, please remove it'
                 raise oscerr.OscIOError(None, msg)
 
-        result = self._execute(dir, old_dir, callmode, singleservice, verbose)
-        shutil.rmtree(old_dir)
+        try:
+            result = self._execute(dir, old_dir, callmode, singleservice, verbose)
+        finally:
+            shutil.rmtree(old_dir)
         return result
 
     def _execute(
         self, dir, old_dir, callmode: Optional[str] = None, singleservice=None, verbose: Optional[bool] = None
     ):
         # cleanup existing generated files
         for filename in os.listdir(dir):
@@ -3568,14 +3571,29 @@
     """Join two or more pathname components, inserting '/' as needed. Cut leading ./"""
     path = os.path.join(a, *p)
     if path.startswith('./'):
         path = path[2:]
     return path
 
 
+def osc_urlencode(data):
+    """
+    An urlencode wrapper that encodes dictionaries in OBS compatible way:
+    {"file": ["foo", "bar"]} -> &file[]=foo&file[]=bar
+    """
+    data = copy.deepcopy(data)
+    if isinstance(data, dict):
+        for key, value in list(data.items()):
+            if isinstance(value, list):
+                del data[key]
+                data[f"{key}[]"] = value
+
+    return urlencode(data, doseq=True)
+
+
 def makeurl(baseurl: str, l, query=None):
     """Given a list of path compoments, construct a complete URL.
 
     Optional parameters for a query string can be given as a list, as a
     dictionary, or as an already assembled string.
     In case of a dictionary, the parameters will be urlencoded by this
     function. In case of a list not -- this is to be backwards compatible.
@@ -3583,15 +3601,15 @@
     query = query or []
     if conf.config['debug']:
         print('makeurl:', baseurl, l, query)
 
     if isinstance(query, list):
         query = '&'.join(query)
     elif isinstance(query, dict):
-        query = urlencode(query)
+        query = osc_urlencode(query)
 
     scheme, netloc, path = urlsplit(baseurl)[0:3]
     return urlunsplit((scheme, netloc, '/'.join([path] + list(l)), query, ''))
 
 
 def check_store_version(dir):
     global store
@@ -4774,14 +4792,46 @@
     f = http_GET(u)
     res = ET.parse(f).getroot()
 
     requests = []
     for root in res.findall('request'):
         r = Request()
         r.read(root)
+
+        # post-process results until we switch back to the /search/request
+        # which seems to be more suitable for such queries
+        exclude = False
+        for action in r.actions:
+            src_project = getattr(action, "src_project", None)
+            src_package = getattr(action, "src_package", None)
+            tgt_project = getattr(action, "tgt_project", None)
+            tgt_package = getattr(action, "tgt_package", None)
+
+            # skip if neither of source and target project matches
+            if "project" in query and query["project"] not in (src_project, tgt_project):
+                exclude = True
+                break
+
+            # skip if neither of source and target package matches
+            if "package" in query and query["package"] not in (src_package, tgt_package):
+                exclude = True
+                break
+
+            if not conf.config["include_request_from_project"]:
+                if "project" in query and "package" in query:
+                    if (src_project, src_package) == (query["project"], query["package"]):
+                        exclude = True
+                        break
+                elif "project" in query:
+                    if src_project == query["project"]:
+                        exclude = True
+                        break
+        if exclude:
+            continue
+
         requests.append(r)
     return requests
 
 
 def get_exact_request_list(
     apiurl: str,
     src_project: str,
@@ -5245,14 +5295,15 @@
     unified=False,
     missingok=False,
     meta=False,
     expand=True,
     onlyissues=False,
     full=True,
     xml=False,
+    files: list = None,
 ):
     query: Dict[str, Union[str, int]] = {"cmd": "diff"}
     if expand:
         query['expand'] = 1
     if old_project:
         query['oproject'] = old_project
     if old_package:
@@ -5270,17 +5321,19 @@
     if full:
         query['filelimit'] = 0
         query['tarlimit'] = 0
     if onlyissues:
         query['onlyissues'] = 1
         query['view'] = 'xml'
         query['unified'] = 0
+    if files:
+        query["file"] = files
 
     u = makeurl(apiurl, ['source', new_project, new_package], query=query)
-    f = http_POST(u)
+    f = http_POST(u, retry_on_400=False)
     if onlyissues and not xml:
         del_issue_list = []
         add_issue_list = []
         chn_issue_list = []
         root = ET.fromstring(f.read())
         node = root.find('issues')
         for issuenode in node.findall('issue'):
@@ -5307,20 +5360,21 @@
     new_revision: str,
     unified=False,
     missingok=False,
     meta=False,
     expand=True,
     onlyissues=False,
     xml=False,
+    files: list = None,
 ):
     try:
         return server_diff(apiurl,
                            old_project, old_package, old_revision,
                            new_project, new_package, new_revision,
-                           unified, missingok, meta, expand, onlyissues, True, xml)
+                           unified, missingok, meta, expand, onlyissues, True, xml, files=files)
     except HTTPError as e:
         msg = None
         body = None
         try:
             body = e.read()
             if b'bad link' not in body:
                 return b'# diff failed: ' + body
@@ -5329,15 +5383,15 @@
 
         if expand:
             rdiff = b"## diff on expanded link not possible, showing unexpanded version\n"
             try:
                 rdiff += server_diff_noex(apiurl,
                                           old_project, old_package, old_revision,
                                           new_project, new_package, new_revision,
-                                          unified, missingok, meta, False)
+                                          unified, missingok, meta, False, files=files)
             except:
                 elm = ET.fromstring(body).find('summary')
                 summary = ''
                 if elm is not None and elm.text is not None:
                     summary = elm.text
                 return b'error: diffing failed: %s' % summary.encode()
             return rdiff
@@ -5719,14 +5773,19 @@
     link_template = """\
 <link %s package="%s"%s%s%s%s>
 <patches>
   <!-- <branch /> for a full copy, default case  -->
   <!-- <apply name="patch" /> apply a patch on the source directory  -->
   <!-- <topadd>%%define build_with_feature_x 1</topadd> add a line on the top (spec file only) -->
   <!-- <add name="file.patch" /> add a patch to be applied after %%setup (spec file only) -->
+  <!-- <add name="file.patch" />
+        Add a patch to be applied after %%setup (spec file only).
+        Patch path prefix stipping can be controlled with the "popt" attribute,
+        for example ``popt="1"`` that translates to %%patch -p1.
+  -->
   <!-- <delete name="filename" /> delete a file -->
 </patches>
 </link>
 """ % (project, src_package, missingok, rev, vrev, cicount)
 
     u = makeurl(apiurl, ['source', dst_project, dst_package, '_link'])
     http_PUT(u, data=link_template)
```

### Comparing `osc-1.0.0/osc/credentials.py` & `osc-1.1.2/osc/credentials.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/fetch.py` & `osc-1.1.2/osc/fetch.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/grabber.py` & `osc-1.1.2/osc/grabber.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 import os
 from urllib.request import HTTPError
 from urllib.parse import urlparse
 from urllib.parse import unquote
 from urllib.error import URLError
 
+import urllib3.exceptions
+
 from .core import streamfile
 
 
 class OscFileGrabber:
     def __init__(self, progress_obj=None):
         self.progress_obj = progress_obj
 
@@ -33,12 +35,12 @@
         self._mirrors = mirrors
 
     def urlgrab(self, url, filename=None, text=None):
         for mirror in self._mirrors:
             try:
                 self._grabber.urlgrab(mirror, filename, text)
                 return True
-            except (HTTPError, URLError) as e:
+            except (HTTPError, URLError, urllib3.exceptions.URLSchemeUnknown) as e:
                 # try next mirror
                 pass
 
         return False
```

### Comparing `osc-1.0.0/osc/meter.py` & `osc-1.1.2/osc/meter.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/oscerr.py` & `osc-1.1.2/osc/oscerr.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/oscssl.py` & `osc-1.1.2/osc/oscssl.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/store.py` & `osc-1.1.2/osc/store.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/util/ar.py` & `osc-1.1.2/osc/util/ar.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/util/archquery.py` & `osc-1.1.2/osc/util/archquery.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/util/cpio.py` & `osc-1.1.2/osc/util/cpio.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/util/debquery.py` & `osc-1.1.2/osc/util/debquery.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/util/git_version.py` & `osc-1.1.2/osc/util/git_version.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/util/helper.py` & `osc-1.1.2/osc/util/helper.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/util/packagequery.py` & `osc-1.1.2/osc/util/packagequery.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/util/repodata.py` & `osc-1.1.2/osc/util/repodata.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/util/rpmquery.py` & `osc-1.1.2/osc/util/rpmquery.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc/util/safewriter.py` & `osc-1.1.2/osc/util/safewriter.py`

 * *Files identical despite different names*

### Comparing `osc-1.0.0/osc.egg-info/PKG-INFO` & `osc-1.1.2/osc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc
-Version: 1.0.0
+Version: 1.1.2
 Summary: openSUSE commander
 Home-page: http://en.opensuse.org/openSUSE:OSC
 Download-URL: https://github.com/openSUSE/osc
 Author: openSUSE project
 Author-email: opensuse-buildservice@opensuse.org
 License: GPLv2+
 Keywords: openSUSE,SUSE,RPM,build,buildservice,command-line
```

### Comparing `osc-1.0.0/setup.cfg` & `osc-1.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 	Topic :: Software Development :: Build Tools
 	Topic :: System :: Archiving :: Packaging
 
 [options]
 packages = 
 	osc
 	osc._private
+	osc.commands
 	osc.util
 install_requires = 
 	cryptography
 	rpm
 	urllib3
 
 [options.extras_require]
```

