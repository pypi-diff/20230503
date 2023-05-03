# Comparing `tmp/colmet-0.6.8.tar.gz` & `tmp/colmet-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colmet-0.6.8.tar", last modified: Thu Jun  2 09:23:49 2022, max compression
+gzip compressed data, was "colmet-0.6.9.tar", last modified: Wed May  3 09:24:28 2023, max compression
```

## Comparing `colmet-0.6.8.tar` & `colmet-0.6.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2022-06-02 09:23:49.102753 colmet-0.6.8/
--rw-r--r--   0 bzizou    (1000) users      (100)     3741 2022-06-02 09:08:21.000000 colmet-0.6.8/CHANGES
--rw-r--r--   0 bzizou    (1000) users      (100)    35149 2020-09-03 08:27:41.000000 colmet-0.6.8/LICENSE
--rw-r--r--   0 bzizou    (1000) users      (100)       34 2020-09-03 08:29:43.000000 colmet-0.6.8/MANIFEST.in
--rw-r--r--   0 bzizou    (1000) users      (100)    10874 2022-06-02 09:23:49.102753 colmet-0.6.8/PKG-INFO
--rw-r--r--   0 bzizou    (1000) users      (100)     6135 2020-09-03 09:03:49.000000 colmet-0.6.8/README.md
-drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2022-06-02 09:23:49.097754 colmet-0.6.8/colmet/
--rw-r--r--   0 bzizou    (1000) users      (100)      203 2022-06-02 09:14:58.000000 colmet-0.6.8/colmet/__init__.py
-drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2022-06-02 09:23:49.098754 colmet-0.6.8/colmet/collector/
--rw-r--r--   0 bzizou    (1000) users      (100)        0 2020-08-18 14:13:09.000000 colmet-0.6.8/colmet/collector/__init__.py
--rw-r--r--   0 bzizou    (1000) users      (100)     4833 2021-08-31 12:30:38.000000 colmet-0.6.8/colmet/collector/elasticsearch.py
--rw-r--r--   0 bzizou    (1000) users      (100)    27331 2021-08-31 14:43:09.000000 colmet-0.6.8/colmet/collector/hdf5.py
--rw-r--r--   0 bzizou    (1000) users      (100)     8804 2022-06-02 09:06:50.000000 colmet-0.6.8/colmet/collector/main.py
-drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2022-06-02 09:23:49.099754 colmet-0.6.8/colmet/common/
--rw-r--r--   0 bzizou    (1000) users      (100)        0 2020-08-18 14:12:56.000000 colmet-0.6.8/colmet/common/__init__.py
-drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2022-06-02 09:23:49.099754 colmet-0.6.8/colmet/common/backends/
--rw-r--r--   0 bzizou    (1000) users      (100)        0 2020-02-20 15:09:59.000000 colmet-0.6.8/colmet/common/backends/__init__.py
--rw-r--r--   0 bzizou    (1000) users      (100)     1240 2020-02-20 15:09:59.000000 colmet-0.6.8/colmet/common/backends/base.py
--rw-r--r--   0 bzizou    (1000) users      (100)     2652 2020-02-20 15:57:27.000000 colmet-0.6.8/colmet/common/backends/zeromq.py
--rw-r--r--   0 bzizou    (1000) users      (100)     3214 2020-08-18 14:12:56.000000 colmet-0.6.8/colmet/common/exceptions.py
--rw-r--r--   0 bzizou    (1000) users      (100)    10457 2022-06-02 09:06:50.000000 colmet-0.6.8/colmet/common/job.py
-drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2022-06-02 09:23:49.101754 colmet-0.6.8/colmet/common/metrics/
--rw-r--r--   0 bzizou    (1000) users      (100)     1613 2020-08-18 14:32:01.000000 colmet-0.6.8/colmet/common/metrics/RAPLstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)      891 2020-08-18 14:14:10.000000 colmet-0.6.8/colmet/common/metrics/__init__.py
--rw-r--r--   0 bzizou    (1000) users      (100)    19698 2020-08-18 14:15:17.000000 colmet-0.6.8/colmet/common/metrics/base.py
--rw-r--r--   0 bzizou    (1000) users      (100)     1647 2020-08-18 14:14:10.000000 colmet-0.6.8/colmet/common/metrics/infinibandstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     1402 2020-08-21 08:59:12.000000 colmet-0.6.8/colmet/common/metrics/ipmipowerstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     1397 2022-06-02 09:06:50.000000 colmet-0.6.8/colmet/common/metrics/jobprocstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     1642 2020-09-04 08:04:07.000000 colmet-0.6.8/colmet/common/metrics/lustrestats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     1374 2022-06-02 09:06:50.000000 colmet-0.6.8/colmet/common/metrics/nvidiastats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     1519 2020-08-18 14:14:10.000000 colmet-0.6.8/colmet/common/metrics/perfhwstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     8934 2021-08-31 14:41:32.000000 colmet-0.6.8/colmet/common/metrics/procstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)    12291 2020-08-18 14:14:10.000000 colmet-0.6.8/colmet/common/metrics/taskstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     1677 2020-02-20 15:57:27.000000 colmet-0.6.8/colmet/common/metrics/temperaturestats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     2331 2020-08-18 14:12:56.000000 colmet-0.6.8/colmet/common/utils.py
-drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2022-06-02 09:23:49.101754 colmet-0.6.8/colmet/node/
--rw-r--r--   0 bzizou    (1000) users      (100)        0 2020-02-20 15:09:59.000000 colmet-0.6.8/colmet/node/__init__.py
-drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2022-06-02 09:23:49.102753 colmet-0.6.8/colmet/node/backends/
--rw-r--r--   0 bzizou    (1000) users      (100)     4129 2020-08-18 14:32:40.000000 colmet-0.6.8/colmet/node/backends/RAPLstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)        0 2020-02-20 15:09:59.000000 colmet-0.6.8/colmet/node/backends/__init__.py
-drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2022-06-02 09:23:49.102753 colmet-0.6.8/colmet/node/backends/genetlink/
--rw-r--r--   0 bzizou    (1000) users      (100)        1 2020-02-20 15:09:59.000000 colmet-0.6.8/colmet/node/backends/genetlink/__init__.py
--rw-r--r--   0 bzizou    (1000) users      (100)     2034 2020-02-20 15:57:27.000000 colmet-0.6.8/colmet/node/backends/genetlink/genetlink.py
--rw-r--r--   0 bzizou    (1000) users      (100)     8097 2020-02-20 15:57:27.000000 colmet-0.6.8/colmet/node/backends/genetlink/netlink.py
--rw-r--r--   0 bzizou    (1000) users      (100)     2876 2020-08-21 07:07:35.000000 colmet-0.6.8/colmet/node/backends/infinibandstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     2097 2020-08-21 08:58:23.000000 colmet-0.6.8/colmet/node/backends/ipmipowerstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     5917 2022-06-02 09:06:50.000000 colmet-0.6.8/colmet/node/backends/jobprocstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     3336 2020-09-04 08:43:14.000000 colmet-0.6.8/colmet/node/backends/lustrestats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     5611 2022-06-02 09:06:50.000000 colmet-0.6.8/colmet/node/backends/nvidiastats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     5781 2020-08-18 05:47:52.000000 colmet-0.6.8/colmet/node/backends/perfhwstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     6226 2022-06-02 09:06:50.000000 colmet-0.6.8/colmet/node/backends/procstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     4819 2020-02-20 15:57:32.000000 colmet-0.6.8/colmet/node/backends/taskstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)     1925 2020-02-20 15:57:27.000000 colmet-0.6.8/colmet/node/backends/temperaturestats.py
--rw-r--r--   0 bzizou    (1000) users      (100)    13291 2022-06-02 09:06:50.000000 colmet-0.6.8/colmet/node/main.py
-drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2022-06-02 09:23:49.098754 colmet-0.6.8/colmet.egg-info/
--rw-r--r--   0 bzizou    (1000) users      (100)    10874 2022-06-02 09:23:48.000000 colmet-0.6.8/colmet.egg-info/PKG-INFO
--rw-r--r--   0 bzizou    (1000) users      (100)     1690 2022-06-02 09:23:49.000000 colmet-0.6.8/colmet.egg-info/SOURCES.txt
--rw-r--r--   0 bzizou    (1000) users      (100)        1 2022-06-02 09:23:48.000000 colmet-0.6.8/colmet.egg-info/dependency_links.txt
--rw-r--r--   0 bzizou    (1000) users      (100)      100 2022-06-02 09:23:48.000000 colmet-0.6.8/colmet.egg-info/entry_points.txt
--rw-r--r--   0 bzizou    (1000) users      (100)       32 2022-06-02 09:23:49.000000 colmet-0.6.8/colmet.egg-info/requires.txt
--rw-r--r--   0 bzizou    (1000) users      (100)       13 2022-06-02 09:23:49.000000 colmet-0.6.8/colmet.egg-info/top_level.txt
--rw-r--r--   0 bzizou    (1000) users      (100)      215 2022-06-02 09:23:49.102753 colmet-0.6.8/setup.cfg
--rwxr-xr-x   0 bzizou    (1000) users      (100)     2422 2020-09-03 16:07:01.000000 colmet-0.6.8/setup.py
-drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2022-06-02 09:23:49.102753 colmet-0.6.8/tests/
--rw-r--r--   0 bzizou    (1000) users      (100)        0 2020-02-20 15:09:59.000000 colmet-0.6.8/tests/__init__.py
--rw-r--r--   0 bzizou    (1000) users      (100)     3448 2020-02-20 15:09:59.000000 colmet-0.6.8/tests/test_metrics_base.py
--rw-r--r--   0 bzizou    (1000) users      (100)      529 2020-02-20 15:09:59.000000 colmet-0.6.8/tests/test_metrics_procstats.py
--rw-r--r--   0 bzizou    (1000) users      (100)      529 2020-02-20 15:09:59.000000 colmet-0.6.8/tests/test_metrics_taskstats.py
+drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2023-05-03 09:24:28.777987 colmet-0.6.9/
+-rw-r--r--   0 bzizou    (1000) users      (100)     3801 2023-05-03 09:05:36.000000 colmet-0.6.9/CHANGES
+-rw-r--r--   0 bzizou    (1000) users      (100)    35149 2020-09-03 08:27:41.000000 colmet-0.6.9/LICENSE
+-rw-r--r--   0 bzizou    (1000) users      (100)       34 2020-09-03 08:29:43.000000 colmet-0.6.9/MANIFEST.in
+-rw-r--r--   0 bzizou    (1000) users      (100)    10934 2023-05-03 09:24:28.777987 colmet-0.6.9/PKG-INFO
+-rw-r--r--   0 bzizou    (1000) users      (100)     6135 2020-09-03 09:03:49.000000 colmet-0.6.9/README.md
+drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2023-05-03 09:24:28.771987 colmet-0.6.9/colmet/
+-rw-r--r--   0 bzizou    (1000) users      (100)      203 2023-05-03 09:09:23.000000 colmet-0.6.9/colmet/__init__.py
+drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2023-05-03 09:24:28.773987 colmet-0.6.9/colmet/collector/
+-rw-r--r--   0 bzizou    (1000) users      (100)        0 2020-08-18 14:13:09.000000 colmet-0.6.9/colmet/collector/__init__.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     4833 2021-08-31 12:30:38.000000 colmet-0.6.9/colmet/collector/elasticsearch.py
+-rw-r--r--   0 bzizou    (1000) users      (100)    27331 2021-08-31 14:43:09.000000 colmet-0.6.9/colmet/collector/hdf5.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     8804 2022-06-02 09:06:50.000000 colmet-0.6.9/colmet/collector/main.py
+drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2023-05-03 09:24:28.773987 colmet-0.6.9/colmet/common/
+-rw-r--r--   0 bzizou    (1000) users      (100)        0 2020-08-18 14:12:56.000000 colmet-0.6.9/colmet/common/__init__.py
+drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2023-05-03 09:24:28.773987 colmet-0.6.9/colmet/common/backends/
+-rw-r--r--   0 bzizou    (1000) users      (100)        0 2020-02-20 15:09:59.000000 colmet-0.6.9/colmet/common/backends/__init__.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     1240 2020-02-20 15:09:59.000000 colmet-0.6.9/colmet/common/backends/base.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     2789 2023-05-03 08:49:17.000000 colmet-0.6.9/colmet/common/backends/zeromq.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     3214 2020-08-18 14:12:56.000000 colmet-0.6.9/colmet/common/exceptions.py
+-rw-r--r--   0 bzizou    (1000) users      (100)    10457 2022-06-02 09:06:50.000000 colmet-0.6.9/colmet/common/job.py
+drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2023-05-03 09:24:28.775987 colmet-0.6.9/colmet/common/metrics/
+-rw-r--r--   0 bzizou    (1000) users      (100)     1613 2020-08-18 14:32:01.000000 colmet-0.6.9/colmet/common/metrics/RAPLstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)      891 2020-08-18 14:14:10.000000 colmet-0.6.9/colmet/common/metrics/__init__.py
+-rw-r--r--   0 bzizou    (1000) users      (100)    19698 2020-08-18 14:15:17.000000 colmet-0.6.9/colmet/common/metrics/base.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     1647 2020-08-18 14:14:10.000000 colmet-0.6.9/colmet/common/metrics/infinibandstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     1402 2020-08-21 08:59:12.000000 colmet-0.6.9/colmet/common/metrics/ipmipowerstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     1397 2022-06-02 09:06:50.000000 colmet-0.6.9/colmet/common/metrics/jobprocstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     1642 2020-09-04 08:04:07.000000 colmet-0.6.9/colmet/common/metrics/lustrestats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     1374 2022-06-02 09:06:50.000000 colmet-0.6.9/colmet/common/metrics/nvidiastats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     1519 2020-08-18 14:14:10.000000 colmet-0.6.9/colmet/common/metrics/perfhwstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     8934 2021-08-31 14:41:32.000000 colmet-0.6.9/colmet/common/metrics/procstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)    12291 2020-08-18 14:14:10.000000 colmet-0.6.9/colmet/common/metrics/taskstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     1677 2020-02-20 15:57:27.000000 colmet-0.6.9/colmet/common/metrics/temperaturestats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     2331 2020-08-18 14:12:56.000000 colmet-0.6.9/colmet/common/utils.py
+drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2023-05-03 09:24:28.775987 colmet-0.6.9/colmet/node/
+-rw-r--r--   0 bzizou    (1000) users      (100)        0 2020-02-20 15:09:59.000000 colmet-0.6.9/colmet/node/__init__.py
+drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2023-05-03 09:24:28.776987 colmet-0.6.9/colmet/node/backends/
+-rw-r--r--   0 bzizou    (1000) users      (100)     4129 2020-08-18 14:32:40.000000 colmet-0.6.9/colmet/node/backends/RAPLstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)        0 2020-02-20 15:09:59.000000 colmet-0.6.9/colmet/node/backends/__init__.py
+drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2023-05-03 09:24:28.776987 colmet-0.6.9/colmet/node/backends/genetlink/
+-rw-r--r--   0 bzizou    (1000) users      (100)        1 2020-02-20 15:09:59.000000 colmet-0.6.9/colmet/node/backends/genetlink/__init__.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     2034 2020-02-20 15:57:27.000000 colmet-0.6.9/colmet/node/backends/genetlink/genetlink.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     8097 2020-02-20 15:57:27.000000 colmet-0.6.9/colmet/node/backends/genetlink/netlink.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     2876 2020-08-21 07:07:35.000000 colmet-0.6.9/colmet/node/backends/infinibandstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     2097 2020-08-21 08:58:23.000000 colmet-0.6.9/colmet/node/backends/ipmipowerstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     5917 2022-06-02 09:06:50.000000 colmet-0.6.9/colmet/node/backends/jobprocstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     3336 2020-09-04 08:43:14.000000 colmet-0.6.9/colmet/node/backends/lustrestats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     5611 2022-06-02 09:06:50.000000 colmet-0.6.9/colmet/node/backends/nvidiastats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     5781 2020-08-18 05:47:52.000000 colmet-0.6.9/colmet/node/backends/perfhwstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     6226 2022-06-02 09:06:50.000000 colmet-0.6.9/colmet/node/backends/procstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     4819 2020-02-20 15:57:32.000000 colmet-0.6.9/colmet/node/backends/taskstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     1925 2020-02-20 15:57:27.000000 colmet-0.6.9/colmet/node/backends/temperaturestats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)    13291 2022-06-02 09:06:50.000000 colmet-0.6.9/colmet/node/main.py
+drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2023-05-03 09:24:28.772987 colmet-0.6.9/colmet.egg-info/
+-rw-r--r--   0 bzizou    (1000) users      (100)    10934 2023-05-03 09:24:28.000000 colmet-0.6.9/colmet.egg-info/PKG-INFO
+-rw-r--r--   0 bzizou    (1000) users      (100)     1690 2023-05-03 09:24:28.000000 colmet-0.6.9/colmet.egg-info/SOURCES.txt
+-rw-r--r--   0 bzizou    (1000) users      (100)        1 2023-05-03 09:24:28.000000 colmet-0.6.9/colmet.egg-info/dependency_links.txt
+-rw-r--r--   0 bzizou    (1000) users      (100)      100 2023-05-03 09:24:28.000000 colmet-0.6.9/colmet.egg-info/entry_points.txt
+-rw-r--r--   0 bzizou    (1000) users      (100)       32 2023-05-03 09:24:28.000000 colmet-0.6.9/colmet.egg-info/requires.txt
+-rw-r--r--   0 bzizou    (1000) users      (100)       13 2023-05-03 09:24:28.000000 colmet-0.6.9/colmet.egg-info/top_level.txt
+-rw-r--r--   0 bzizou    (1000) users      (100)      215 2023-05-03 09:24:28.777987 colmet-0.6.9/setup.cfg
+-rwxr-xr-x   0 bzizou    (1000) users      (100)     2422 2020-09-03 16:07:01.000000 colmet-0.6.9/setup.py
+drwxr-xr-x   0 bzizou    (1000) users      (100)        0 2023-05-03 09:24:28.777987 colmet-0.6.9/tests/
+-rw-r--r--   0 bzizou    (1000) users      (100)        0 2020-02-20 15:09:59.000000 colmet-0.6.9/tests/__init__.py
+-rw-r--r--   0 bzizou    (1000) users      (100)     3448 2020-02-20 15:09:59.000000 colmet-0.6.9/tests/test_metrics_base.py
+-rw-r--r--   0 bzizou    (1000) users      (100)      529 2020-02-20 15:09:59.000000 colmet-0.6.9/tests/test_metrics_procstats.py
+-rw-r--r--   0 bzizou    (1000) users      (100)      529 2020-02-20 15:09:59.000000 colmet-0.6.9/tests/test_metrics_taskstats.py
```

### Comparing `colmet-0.6.8/CHANGES` & `colmet-0.6.9/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Colmet CHANGELOG
 ================
 
+Version 0.6.9
+-------------
+- Fix for newer pyzmq versions
+
 Version 0.6.8
 -------------
 - Added nvidia GPU support
 
 Version 0.6.7
 -------------
 - bugfix: glob import missing into procstats
```

### Comparing `colmet-0.6.8/LICENSE` & `colmet-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/PKG-INFO` & `colmet-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colmet
-Version: 0.6.8
+Version: 0.6.9
 Summary: A utility to monitor the jobs ressources in a HPC environment, espacially OAR
 Home-page: http://oar.imag.fr/
 Author: Philippe Le Brouster, Olivier Richard
 Author-email: philippe.le-brouster@imag.fr, olivier.richard@imag.fr
 Maintainer: Salem Harrache
 Maintainer-email: salem.harrache@inria.fr
 License: GNU GPL
@@ -226,14 +226,18 @@
 A file named temperature_mapping.[timestamp].csv is created in the working directory. It establishes the correspondence between `counter_1`, `counter_2`, etc from collected data and the actual name of the metric.
 
 
 
 Colmet CHANGELOG
 ================
 
+Version 0.6.9
+-------------
+- Fix for newer pyzmq versions
+
 Version 0.6.8
 -------------
 - Added nvidia GPU support
 
 Version 0.6.7
 -------------
 - bugfix: glob import missing into procstats
```

### Comparing `colmet-0.6.8/README.md` & `colmet-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/collector/elasticsearch.py` & `colmet-0.6.9/colmet/collector/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/collector/hdf5.py` & `colmet-0.6.9/colmet/collector/hdf5.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/collector/main.py` & `colmet-0.6.9/colmet/collector/main.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/backends/base.py` & `colmet-0.6.9/colmet/common/backends/base.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/backends/zeromq.py` & `colmet-0.6.9/colmet/common/backends/zeromq.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,18 @@
 class ZMQInputBackend(InputBaseBackend):
     __backend_name__ = "zeromq"
 
     def open(self):
         self.context = zmq.Context()
         self.socket = self.context.socket(zmq.PULL)
         self.socket.setsockopt(zmq.LINGER, self.options.zeromq_linger)
-        self.socket.setsockopt(_rcv_hwm, self.options.zeromq_hwm)
+        try:
+          self.socket.setsockopt(_rcv_hwm, self.options.zeromq_hwm)
+        except(AttributeError, zmq.error.ZMQError):
+          self.socket.setsockopt(zmq.RCVHWM, self.options.zeromq_hwm)
         LOG.debug("Use the bind URI '%s'" % self.options.zeromq_bind_uri)
         self.socket.bind(self.options.zeromq_bind_uri)
 
     def close(self):
         self.socket.close()
         self.context.term()
```

### Comparing `colmet-0.6.8/colmet/common/exceptions.py` & `colmet-0.6.9/colmet/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/job.py` & `colmet-0.6.9/colmet/common/job.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/metrics/RAPLstats.py` & `colmet-0.6.9/colmet/common/metrics/RAPLstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/metrics/__init__.py` & `colmet-0.6.9/colmet/common/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/metrics/base.py` & `colmet-0.6.9/colmet/common/metrics/base.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/metrics/infinibandstats.py` & `colmet-0.6.9/colmet/common/metrics/infinibandstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/metrics/ipmipowerstats.py` & `colmet-0.6.9/colmet/common/metrics/ipmipowerstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/metrics/jobprocstats.py` & `colmet-0.6.9/colmet/common/metrics/jobprocstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/metrics/lustrestats.py` & `colmet-0.6.9/colmet/common/metrics/lustrestats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/metrics/nvidiastats.py` & `colmet-0.6.9/colmet/common/metrics/nvidiastats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/metrics/perfhwstats.py` & `colmet-0.6.9/colmet/common/metrics/perfhwstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/metrics/procstats.py` & `colmet-0.6.9/colmet/common/metrics/procstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/metrics/taskstats.py` & `colmet-0.6.9/colmet/common/metrics/taskstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/metrics/temperaturestats.py` & `colmet-0.6.9/colmet/common/metrics/temperaturestats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/common/utils.py` & `colmet-0.6.9/colmet/common/utils.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/node/backends/RAPLstats.py` & `colmet-0.6.9/colmet/node/backends/RAPLstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/node/backends/genetlink/genetlink.py` & `colmet-0.6.9/colmet/node/backends/genetlink/genetlink.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/node/backends/genetlink/netlink.py` & `colmet-0.6.9/colmet/node/backends/genetlink/netlink.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/node/backends/infinibandstats.py` & `colmet-0.6.9/colmet/node/backends/infinibandstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/node/backends/ipmipowerstats.py` & `colmet-0.6.9/colmet/node/backends/ipmipowerstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/node/backends/jobprocstats.py` & `colmet-0.6.9/colmet/node/backends/jobprocstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/node/backends/lustrestats.py` & `colmet-0.6.9/colmet/node/backends/lustrestats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/node/backends/nvidiastats.py` & `colmet-0.6.9/colmet/node/backends/nvidiastats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/node/backends/perfhwstats.py` & `colmet-0.6.9/colmet/node/backends/perfhwstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/node/backends/procstats.py` & `colmet-0.6.9/colmet/node/backends/procstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/node/backends/taskstats.py` & `colmet-0.6.9/colmet/node/backends/taskstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/node/backends/temperaturestats.py` & `colmet-0.6.9/colmet/node/backends/temperaturestats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet/node/main.py` & `colmet-0.6.9/colmet/node/main.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/colmet.egg-info/PKG-INFO` & `colmet-0.6.9/colmet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colmet
-Version: 0.6.8
+Version: 0.6.9
 Summary: A utility to monitor the jobs ressources in a HPC environment, espacially OAR
 Home-page: http://oar.imag.fr/
 Author: Philippe Le Brouster, Olivier Richard
 Author-email: philippe.le-brouster@imag.fr, olivier.richard@imag.fr
 Maintainer: Salem Harrache
 Maintainer-email: salem.harrache@inria.fr
 License: GNU GPL
@@ -226,14 +226,18 @@
 A file named temperature_mapping.[timestamp].csv is created in the working directory. It establishes the correspondence between `counter_1`, `counter_2`, etc from collected data and the actual name of the metric.
 
 
 
 Colmet CHANGELOG
 ================
 
+Version 0.6.9
+-------------
+- Fix for newer pyzmq versions
+
 Version 0.6.8
 -------------
 - Added nvidia GPU support
 
 Version 0.6.7
 -------------
 - bugfix: glob import missing into procstats
```

### Comparing `colmet-0.6.8/colmet.egg-info/SOURCES.txt` & `colmet-0.6.9/colmet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/setup.py` & `colmet-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/tests/test_metrics_base.py` & `colmet-0.6.9/tests/test_metrics_base.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/tests/test_metrics_procstats.py` & `colmet-0.6.9/tests/test_metrics_procstats.py`

 * *Files identical despite different names*

### Comparing `colmet-0.6.8/tests/test_metrics_taskstats.py` & `colmet-0.6.9/tests/test_metrics_taskstats.py`

 * *Files identical despite different names*

