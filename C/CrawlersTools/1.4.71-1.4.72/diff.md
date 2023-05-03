# Comparing `tmp/CrawlersTools-1.4.71.tar.gz` & `tmp/CrawlersTools-1.4.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrawlersTools-1.4.71.tar", last modified: Tue Apr 25 07:35:09 2023, max compression
+gzip compressed data, was "CrawlersTools-1.4.72.tar", last modified: Wed May  3 02:04:28 2023, max compression
```

## Comparing `CrawlersTools-1.4.71.tar` & `CrawlersTools-1.4.72.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:35:09.540734 CrawlersTools-1.4.71/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:35:09.528734 CrawlersTools-1.4.71/CrawlersTools/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:35:09.532734 CrawlersTools-1.4.71/CrawlersTools/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/attachment_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/content_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/list_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:35:09.532734 CrawlersTools-1.4.71/CrawlersTools/extractors/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/schemas/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/time_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/title_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:35:09.532734 CrawlersTools-1.4.71/CrawlersTools/extractors/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/utils/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/extractors/utils/similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:35:09.532734 CrawlersTools-1.4.71/CrawlersTools/js_crawler/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/js_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/js_crawler/font_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/js_crawler/transfer_js.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:35:09.532734 CrawlersTools-1.4.71/CrawlersTools/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/logs/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:35:09.536734 CrawlersTools-1.4.71/CrawlersTools/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/pipelines/mongo_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/pipelines/mysql_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/pipelines/redis_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:35:09.536734 CrawlersTools-1.4.71/CrawlersTools/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/preprocess/bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/preprocess/time_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:35:09.536734 CrawlersTools-1.4.71/CrawlersTools/projects/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/projects/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/projects/upload_oss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:35:09.536734 CrawlersTools-1.4.71/CrawlersTools/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/requests/base_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/requests/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/requests/random_ua.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:35:09.540734 CrawlersTools-1.4.71/CrawlersTools/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/CrawlersTools/schedules/auto_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:35:09.528734 CrawlersTools-1.4.71/CrawlersTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-25 07:35:09.000000 CrawlersTools-1.4.71/CrawlersTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-25 07:35:09.000000 CrawlersTools-1.4.71/CrawlersTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:35:09.000000 CrawlersTools-1.4.71/CrawlersTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-25 07:35:09.000000 CrawlersTools-1.4.71/CrawlersTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 07:35:09.000000 CrawlersTools-1.4.71/CrawlersTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-25 07:35:09.540734 CrawlersTools-1.4.71/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:35:09.540734 CrawlersTools-1.4.71/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-25 07:34:55.000000 CrawlersTools-1.4.71/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.114403 CrawlersTools-1.4.72/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.106403 CrawlersTools-1.4.72/CrawlersTools/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.106403 CrawlersTools-1.4.72/CrawlersTools/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/attachment_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/content_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15555 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/list_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.106403 CrawlersTools-1.4.72/CrawlersTools/extractors/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/schemas/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/time_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/title_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.110403 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14866 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/extractors/utils/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.110403 CrawlersTools-1.4.72/CrawlersTools/js_crawler/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/js_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/js_crawler/font_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/js_crawler/transfer_js.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.110403 CrawlersTools-1.4.72/CrawlersTools/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/logs/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.110403 CrawlersTools-1.4.72/CrawlersTools/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/pipelines/mongo_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/pipelines/mysql_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/pipelines/redis_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.110403 CrawlersTools-1.4.72/CrawlersTools/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/preprocess/bloom_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/preprocess/time_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.110403 CrawlersTools-1.4.72/CrawlersTools/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/projects/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/projects/upload_oss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.114403 CrawlersTools-1.4.72/CrawlersTools/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/requests/base_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/requests/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/requests/random_ua.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.114403 CrawlersTools-1.4.72/CrawlersTools/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/CrawlersTools/schedules/auto_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:04:28.106403 CrawlersTools-1.4.72/CrawlersTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-05-03 02:04:28.000000 CrawlersTools-1.4.72/CrawlersTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-03 02:04:28.000000 CrawlersTools-1.4.72/CrawlersTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:04:28.000000 CrawlersTools-1.4.72/CrawlersTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-03 02:04:28.000000 CrawlersTools-1.4.72/CrawlersTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 02:04:28.000000 CrawlersTools-1.4.72/CrawlersTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-05-03 02:04:28.114403 CrawlersTools-1.4.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 02:04:28.114403 CrawlersTools-1.4.72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-03 02:04:14.000000 CrawlersTools-1.4.72/setup.py
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools/extractors/__init__.py` & `CrawlersTools-1.4.72/CrawlersTools/extractors/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # -*- coding: utf-8 -*-
 # @Project : CrawlersTools
 # @Time    : 2022/8/15 11:29
 # @Author  : MuggleK
 # @File    : __init__.py
 
+from CrawlersTools.extractors.attachment_extractor import AttachmentExtractor
+from CrawlersTools.extractors.content_extractor import ContentExtractor
 from CrawlersTools.extractors.list_extractor import ListExtractor
-
-from CrawlersTools.extractors.title_extractor import TitleExtractor
 from CrawlersTools.extractors.time_extractor import TimeExtractor
-from CrawlersTools.extractors.content_extractor import ContentExtractor
-from CrawlersTools.extractors.attachment_extractor import AttachmentExtractor
+from CrawlersTools.extractors.title_extractor import TitleExtractor
 
 
 class PolicyExtractor(object):
 
     @staticmethod
     def extract(
             html,
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools/extractors/attachment_extractor.py` & `CrawlersTools-1.4.72/CrawlersTools/extractors/attachment_extractor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # @Project : CrawlersTools
 # @Time    : 2022/12/21 10:54
 # @Author  : MuggleK
 # @File    : attachment_extractor.py
 
 import re
 
-from CrawlersTools.extractors.schemas.element import Element
 from CrawlersTools.extractors.base import BaseExtractor
+from CrawlersTools.extractors.schemas.element import Element
 from CrawlersTools.extractors.utils.settings import ATTACHMENT_REGX
 
 
 class AttachmentExtractor(BaseExtractor):
     """
     extract content from detail page
     """
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools/extractors/base.py` & `CrawlersTools-1.4.72/CrawlersTools/extractors/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from lxml.html import fromstring
 from loguru import logger
 from lxml.html import etree
+from lxml.html import fromstring
+
 from CrawlersTools.extractors.schemas.element import Element
 
 
 class BaseExtractor(object):
     """
     Base Extractor which provide common methods
     """
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools/extractors/content_extractor.py` & `CrawlersTools-1.4.72/CrawlersTools/extractors/content_extractor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 # @File    : content_extractor.py
 
 from copy import deepcopy
 
 import numpy as np
 from lxml.html import fromstring, HtmlElement
 
-from CrawlersTools.extractors.schemas.element import Element
-from CrawlersTools.extractors.utils.preprocess import preprocess4content_extractor
 from CrawlersTools.extractors.base import BaseExtractor
+from CrawlersTools.extractors.schemas.element import Element
 from CrawlersTools.extractors.utils.element import descendants_of_body
+from CrawlersTools.extractors.utils.preprocess import preprocess4content_extractor
 from CrawlersTools.extractors.utils.settings import SPECIAL_SYMBOL_MAP, ERROR_NAV_LIST
 
 
 class ContentExtractor(BaseExtractor):
     """
     extract content from detail page
     """
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools/extractors/list_extractor.py` & `CrawlersTools-1.4.72/CrawlersTools/extractors/list_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,31 +6,30 @@
 LastAuthor: xiaobin.zhu
 LastEditTime: 2022-11-24 14:24:09
 Description: extract list from index page
 FilePath: list_extractor
 """
 import math
 import operator
+from collections import defaultdict
+from urllib.parse import urljoin
 
 # from loguru import logger
 import numpy as np
-from collections import defaultdict
-from urllib.parse import urljoin
 from lxml.html import fromstring
 
+from CrawlersTools.extractors.base import BaseExtractor
+from CrawlersTools.extractors.schemas.element import Element
 from CrawlersTools.extractors.utils.cluster import cluster_dict
+from CrawlersTools.extractors.utils.element import calc_a_descendants_text_of_avg_length, descendants_of_body
+from CrawlersTools.extractors.utils.preprocess import preprocess4list_extractor
 from CrawlersTools.extractors.utils.settings import (
     LIST_AVG_LENGTH, LIST_MAX_LENGTH, LIST_MIN_LENGTH, LIST_MIN_NUMBER, ADDTION_RIGHT_NUM, SIMILARITY_THRESHOLD,
     HIGH_WEIGHT_ERROR_KEYWORD, DIRECTORY_ERROR_TITLE, SPECIAL_SYMBOL_MAP,
 )
-from CrawlersTools.extractors.utils.preprocess import preprocess4list_extractor
-from CrawlersTools.extractors.base import BaseExtractor
-from CrawlersTools.extractors.utils.element import calc_a_descendants_text_of_avg_length, descendants_of_body
-from CrawlersTools.extractors.schemas.element import Element
-
 
 AVG_LENGTH = (LIST_MIN_LENGTH + LIST_MAX_LENGTH) / 2
 
 
 class ListExtractor(BaseExtractor):
     """
     extract list from index page
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools/extractors/schemas/element.py` & `CrawlersTools-1.4.72/CrawlersTools/extractors/schemas/element.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/extractors/time_extractor.py` & `CrawlersTools-1.4.72/CrawlersTools/extractors/time_extractor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # @File    : time_extractor.py
 
 import re
 
 from lxml.html import etree
 
 from CrawlersTools.extractors.base import BaseExtractor
-from CrawlersTools.extractors.utils.settings import DATETIME_PATTERN, PUBLISH_TIME_META, TITLE_EXTRACTOR_USELESS_TAGS
 from CrawlersTools.extractors.schemas.element import Element
+from CrawlersTools.extractors.utils.settings import DATETIME_PATTERN, PUBLISH_TIME_META, TITLE_EXTRACTOR_USELESS_TAGS
 from CrawlersTools.preprocess import TimeProcessor
 
 format_time = TimeProcessor().format
 
 
 class TimeExtractor(BaseExtractor):
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools/extractors/title_extractor.py` & `CrawlersTools-1.4.72/CrawlersTools/extractors/title_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 # @Project : CrawlersTools
 # @Time    : 2022/8/19 20:23
 # @Author  : MuggleK
 # @File    : title_extractor.py
 
 import re
 from itertools import combinations
+
 from lxml.html import etree
 
 from CrawlersTools.extractors.base import BaseExtractor
-from CrawlersTools.extractors.utils.similarity import get_longest_common_sub_string
+from CrawlersTools.extractors.schemas.element import Element
 from CrawlersTools.extractors.utils.settings import (
     TITLE_HTAG_XPATH, TITLE_META_XPATH, TITLE_META_XPATH_BAK, TITLE_EXTRACTOR_USELESS_TAGS, PUNCTUATION_ALPHA_PATTERN
 )
-from CrawlersTools.extractors.schemas.element import Element
+from CrawlersTools.extractors.utils.similarity import get_longest_common_sub_string
 
 
 class TitleExtractor(BaseExtractor):
 
     @staticmethod
     def extract_by_xpath(element, title_xpath):
         if title_xpath:
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools/extractors/utils/cluster.py` & `CrawlersTools-1.4.72/CrawlersTools/extractors/utils/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from CrawlersTools.extractors.utils.similarity import similarity
 from collections import defaultdict
 
+from CrawlersTools.extractors.utils.similarity import similarity
+
 
 def cluster(items, threshold=0.9):
     """
     cluster names
     :param items:
     :param threshold:
     :return: cluster map, for example {"foo": 0, "bar": 1}
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools/extractors/utils/element.py` & `CrawlersTools-1.4.72/CrawlersTools/extractors/utils/element.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import re
-import numpy as np
+from collections import defaultdict
 from os.path import exists
 from types import ModuleType
-from collections import defaultdict
+
+import numpy as np
 from loguru import logger
 from lxml.html import fromstring, HtmlElement
+
 from CrawlersTools.extractors.schemas.element import Element
 from CrawlersTools.extractors.utils.similarity import similarity
 
 PUNCTUATION = set('''！，。？、；：“”‘’《》%（）<>{}「」【】*～`,.?:;'"!%()''')
 
 
 def remove_element(element: Element):
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools/extractors/utils/preprocess.py` & `CrawlersTools-1.4.72/CrawlersTools/extractors/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/extractors/utils/settings.py` & `CrawlersTools-1.4.72/CrawlersTools/extractors/utils/settings.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/extractors/utils/similarity.py` & `CrawlersTools-1.4.72/CrawlersTools/extractors/utils/similarity.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/js_crawler/font_decrypt.py` & `CrawlersTools-1.4.72/CrawlersTools/js_crawler/font_decrypt.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # @Time    : 2022/8/12 16:11
 # @Author  : MuggleK
 # @File    : font_decrypt.py
 
 from io import BytesIO
 
 import httpx
+from PIL import ImageFont, ImageDraw, Image
 from fontTools.ttLib import TTFont
 from loguru import logger
-from PIL import ImageFont, ImageDraw, Image
 
 
 class FontDecrypt(object):
     """
     Usage::
 
         # >>>
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools/js_crawler/transfer_js.py` & `CrawlersTools-1.4.72/CrawlersTools/js_crawler/transfer_js.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/logs/log.py` & `CrawlersTools-1.4.72/CrawlersTools/logs/log.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/pipelines/mongo_pipeline.py` & `CrawlersTools-1.4.72/CrawlersTools/pipelines/mongo_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/pipelines/mysql_pipeline.py` & `CrawlersTools-1.4.72/CrawlersTools/pipelines/mysql_pipeline.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # @Project : CrawlersTools
 # @Time    : 2022/8/12 9:12
 # @Author  : MuggleK
 # @File    : mysql_pipeline.py
 
 import time
 
+import pymysql
 from DBUtils.PooledDB import PooledDB
 from loguru import logger
-import pymysql
 
 
 class MysqlPipeline(object):
     """
     A Mysql Pipeline to Create or Insert or Update or Delete Table
 
     Usage::
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools/pipelines/redis_pipeline.py` & `CrawlersTools-1.4.72/CrawlersTools/pipelines/redis_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/preprocess/bloom_filter.py` & `CrawlersTools-1.4.72/CrawlersTools/preprocess/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/preprocess/time_process.py` & `CrawlersTools-1.4.72/CrawlersTools/preprocess/time_process.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/projects/filters.py` & `CrawlersTools-1.4.72/CrawlersTools/projects/filters.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/projects/upload_oss.py` & `CrawlersTools-1.4.72/CrawlersTools/projects/upload_oss.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/requests/base_requests.py` & `CrawlersTools-1.4.72/CrawlersTools/requests/base_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 # @Project : CrawlersTools
 # @Time    : 2022/6/21 17:08
 # @Author  : MuggleK
 # @File    : base_requests.py
 
-import re
 import json
-import time
 import random
+import re
+import time
 
 from chardet import detect
 from httpx import Client, Response
 from loguru import logger
 
 from CrawlersTools.requests.proxy import get_proxies
 from CrawlersTools.requests.random_ua import UserAgent
@@ -147,15 +147,14 @@
 
         js_text = js_text.split(';location.href=loc')[0].split('document.cookie=')[-1]
         r = execjs.eval(js_text).split(';')[0]
         return r
 
     @staticmethod
     def process_clearance(html):
-        import hashlib
 
         data = json.loads(re.findall(r'go\((.*?)\)', html)[1])
         chars_length = len(data.get('chars'))
         for i in range(chars_length):
             for j in range(chars_length):
                 result = data.get('bts')[0] + data.get('chars')[i] + data.get('chars')[j] + data.get('bts')[1]
                 b = eval('hashlib.{}()'.format(data.get('ha')))
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools/requests/proxy.py` & `CrawlersTools-1.4.72/CrawlersTools/requests/proxy.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/requests/random_ua.py` & `CrawlersTools-1.4.72/CrawlersTools/requests/random_ua.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools/schedules/auto_thread.py` & `CrawlersTools-1.4.72/CrawlersTools/schedules/auto_thread.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/CrawlersTools.egg-info/PKG-INFO` & `CrawlersTools-1.4.72/CrawlersTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrawlersTools
-Version: 1.4.71
+Version: 1.4.72
 Summary: Tools for Crawlers
 Home-page: https://github.com/MuggleK/CrawlersTools
 Author: MuggleK
 Author-email: peichangchuan@gmail.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `CrawlersTools-1.4.71/CrawlersTools.egg-info/SOURCES.txt` & `CrawlersTools-1.4.72/CrawlersTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/LICENSE` & `CrawlersTools-1.4.72/LICENSE`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/PKG-INFO` & `CrawlersTools-1.4.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrawlersTools
-Version: 1.4.71
+Version: 1.4.72
 Summary: Tools for Crawlers
 Home-page: https://github.com/MuggleK/CrawlersTools
 Author: MuggleK
 Author-email: peichangchuan@gmail.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `CrawlersTools-1.4.71/README.md` & `CrawlersTools-1.4.72/README.md`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.71/setup.py` & `CrawlersTools-1.4.72/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='CrawlersTools',  # 包名
-    version='1.4.71',  # 版本号
+    version='1.4.72',  # 版本号
     description='Tools for Crawlers',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='MuggleK',
     author_email='peichangchuan@gmail.com',
     url='https://github.com/MuggleK/CrawlersTools',
     install_requires=[
```

