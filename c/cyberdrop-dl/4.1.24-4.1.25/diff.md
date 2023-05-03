# Comparing `tmp/cyberdrop-dl-4.1.24.tar.gz` & `tmp/cyberdrop-dl-4.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.1.24.tar", last modified: Sat Apr 29 00:51:13 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.1.25.tar", last modified: Wed May  3 02:16:31 2023, max compression
```

## Comparing `cyberdrop-dl-4.1.24.tar` & `cyberdrop-dl-4.1.25.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.751474 cyberdrop-dl-4.1.24/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-29 00:51:13.751474 cyberdrop-dl-4.1.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.743473 cyberdrop-dl-4.1.24/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.747473 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.747473 cyberdrop-dl-4.1.24/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.747473 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.751474 cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17579 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.751474 cyberdrop-dl-4.1.24/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20272 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:51:13.743473 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-29 00:51:13.000000 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-29 00:51:13.000000 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:51:13.000000 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-29 00:51:13.000000 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-29 00:51:13.000000 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 00:51:13.000000 cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-29 00:51:13.751474 cyberdrop-dl-4.1.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 00:51:02.000000 cyberdrop-dl-4.1.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.749760 cyberdrop-dl-4.1.25/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-03 02:16:31.749760 cyberdrop-dl-4.1.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.741760 cyberdrop-dl-4.1.25/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.741760 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.741760 cyberdrop-dl-4.1.25/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/client/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.745760 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.745760 cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13984 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.745760 cyberdrop-dl-4.1.25/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20254 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:16:31.741760 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-03 02:16:31.000000 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-03 02:16:31.000000 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:16:31.000000 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 02:16:31.000000 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-03 02:16:31.000000 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 02:16:31.000000 cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-03 02:16:31.749760 cyberdrop-dl-4.1.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 02:16:22.000000 cyberdrop-dl-4.1.25/setup.py
```

### Comparing `cyberdrop-dl-4.1.24/LICENSE` & `cyberdrop-dl-4.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.24/PKG-INFO` & `cyberdrop-dl-4.1.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.24
+Version: 4.1.25
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.24 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.25 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.24/README.md` & `cyberdrop-dl-4.1.25/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,10 +272,10 @@
 
     def _exit_handler(self) -> None:
         """Exit handler on unexpected exits"""
         try:
             self.conn.commit()
             self.conn.close()
         except Exception as e:
-            logging.debug("Failed to close sqlite database connection: %s", str(e))
+            logging.debug("Failed to close sqlite database connection: %s", e)
         else:
             logging.debug("Successfully closed sqlite database connection")
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,15 +145,15 @@
                                            raise_for_status=True, proxy=proxy) as resp:
             content_type = resp.headers.get('Content-Type')
             if not content_type:
                 raise DownloadFailure(code=CustomHTTPStatus.IM_A_TEAPOT, message="No content-type in response header")
             if resp.url in self.bunkr_maintenance:
                 raise DownloadFailure(code=HTTPStatus.SERVICE_UNAVAILABLE, message="Bunkr under maintenance")
             if any(s in content_type.lower() for s in ('html', 'text')):
-                logger.debug("Server for %s is experiencing issues, you are being ratelimited, or cookies have expired", str(media.url))
+                logger.debug("Server for %s is experiencing issues, you are being ratelimited, or cookies have expired", media.url)
                 raise DownloadFailure(code=CustomHTTPStatus.IM_A_TEAPOT, message="Unexpectedly got text as response")
 
             size = int(resp.headers.get('Content-Length', '0'))
             await save_content(resp.content, size)
 
     async def _throttle(self, delay: float, host: str) -> None:
         """Throttles requests to domains by a parameter amount of time"""
@@ -197,14 +197,14 @@
     async def get_filesize(self, url: URL, referer: str, current_throttle: float) -> int:
         headers = {'Referer': referer, 'user-agent': self.client.user_agent}
 
         assert url.host is not None
         await self._throttle(current_throttle, url.host)
         async with self.client_session.get(url, headers=headers, ssl=self.client.ssl_context,
                                            raise_for_status=True) as resp:
-            return int(resp.headers.get('Content-Length', str(0)))
+            return int(resp.headers.get('Content-Length', '0'))
 
     async def exit_handler(self) -> None:
         try:
             await self.client_session.close()
         except Exception:
             logging.debug("Failed to close session.")
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/client/rate_limiting.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/client/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         """Scraper for Anonfiles"""
         assert url.host is not None
         if 'cdn' in url.host:
             url = URL("https://anonfiles.com") / url.parts[1]
 
         album_obj = AlbumItem("Loose Anon Files", [])
 
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         try:
             json = await session.get_json(self.api_link/url.parts[1]/"info")
             if json['status']:
                 soup = await session.get_BS4(url)
 
                 link = soup.select_one("a[id=download-url]")
@@ -40,17 +40,17 @@
 
                 filename, ext = await get_filename_and_ext(".".join(json['data']['file']['metadata']['name'].rsplit("_", 1)))
                 media_item = MediaItem(link, url, complete, filename, ext, filename)
                 await album_obj.add_media(media_item)
                 if not complete:
                     await self.SQL_Helper.insert_media("anonfiles", "", media_item)
             else:
-                log(f"Dead: {str(url)}", quiet=self.quiet, style="red")
+                log(f"Dead: {url}", quiet=self.quiet, style="red")
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
             return album_obj
 
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,32 +25,32 @@
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.remove_bunkr_id = remove_bunkr_id
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Scraper for Bunkr"""
         album_obj = AlbumItem("Loose Bunkr Files", [])
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         if "v" in url.parts or "d" in url.parts:
             media = await self.get_file(session, url)
             if not media.filename:
                 return album_obj
             await album_obj.add_media(media)
-            log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Finished: {url}", quiet=self.quiet, style="green")
             if not media.complete:
                 await self.SQL_Helper.insert_media("bunkr", "", media)
             return album_obj
 
         if "a" in url.parts:
             album_obj = await self.get_album(session, url)
             await self.SQL_Helper.insert_album("bunkr", url, album_obj)
 
             if album_obj.media:
-                log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+                log(f"Finished: {url}", quiet=self.quiet, style="green")
             return album_obj
 
         cdn_possibilities = r"(?:cdn.bunkr...|cdn..bunkr...|cdn...bunkr...|media-files.bunkr...|media-files..bunkr...|media-files...bunkr...)"
         ext = '.' + url.parts[-1].split('.')[-1]
         if ext:
             ext = ext.lower()
         if ext in FILE_FORMATS['Images']:
@@ -68,15 +68,15 @@
                 referer = URL(re.sub(cdn_possibilities, "bunkr.la/v", str(url)))
             else:
                 referer = URL(re.sub(cdn_possibilities, "bunkr.la/d", str(url)))
             media_item = await self.get_file(session, referer)
             await album_obj.add_media(media_item)
 
         await self.SQL_Helper.insert_album("bunkr", url, album_obj)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
 
     async def remove_id(self, filename: str, ext: str):
         """Removes the additional string bunkr adds to the end of every filename"""
         original_filename = filename
         if self.remove_bunkr_id:
             filename = filename.rsplit(ext, 1)[0]
@@ -119,16 +119,16 @@
             original_filename, filename = await self.remove_id(filename, ext)
 
             await self.SQL_Helper.fix_bunkr_entries(link, original_filename)
             complete = await self.SQL_Helper.check_complete_singular("bunkr", link)
             return MediaItem(link, url, complete, filename, ext, original_filename)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
             return MediaItem(url, url, False, "", "", "")
 
     async def get_album(self, session: ScrapeSession, url: URL):
         """Iterates through an album and creates the media items"""
 
         ### Temp Fix ###
@@ -150,15 +150,15 @@
                 if link.startswith("/"):
                     link = URL("https://" + url.host + link)
                 link = URL(link)
 
                 try:
                     filename, ext = await get_filename_and_ext(link.name)
                 except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(link))
+                    logger.debug("Couldn't get extension for %s", link)
                     continue
 
                 if "v" in link.parts or "d" in link.parts:
                     media = await self.get_file(session, link)
                     link = media.url
                 elif ext in FILE_FORMATS["Images"]:
                     link = URL(str(link).replace("https://cdn", "https://i"))
@@ -172,12 +172,12 @@
 
                 await self.SQL_Helper.fix_bunkr_entries(link, original_filename)
                 complete = await self.SQL_Helper.check_complete_singular("bunkr", link)
                 media = MediaItem(link, url, complete, filename, ext, original_filename)
                 await album.add_media(media)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return album
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,29 +39,29 @@
         self.quiet = quiet
         self.scraping_mapper = scraping_mapper
         self.separate_posts = separate_posts
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL):
         """Director for Coomer/Kemono scraping"""
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
         cascade = CascadeItem({})
         title = None
         try:
             assert url.host is not None
             domain = next((domain for domain in ("coomer", "kemono") if domain in url.host), None)
             if domain:
                 title = await self.handle_coomeno(session, url, domain, cascade)
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         await self.SQL_Helper.insert_cascade(cascade)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return cascade, title
 
     async def handle_coomeno(self, session: ScrapeSession, url: URL, domain: str, cascade: CascadeItem) -> str:
         """Coomer/Kemono director function"""
         title = f"Loose {domain.capitalize()} Files"
         if "thumbnail" in url.parts:
             parts = [x for x in url.parts if x not in ("thumbnail", "/")]
@@ -112,16 +112,16 @@
             next_page = soup.select_one(spec.next_page_selector)
             if next_page:
                 next_page = next_page.get('href')
                 if next_page:
                     await self.parse_profile(session, URL("https://" + url.host + next_page), spec, cascade)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return title
 
     async def parse_post(self, session: ScrapeSession, url: URL, domain: str, cascade: CascadeItem,
                          title: str = "") -> str:
         """Parses posts with supplied selectors"""
@@ -133,15 +133,15 @@
                 await self.SQL_Helper.insert_blob(text, url)
             soup = BeautifulSoup(text, 'html.parser')
 
             if self.separate_posts:
                 post_tag = soup.select_one("h1[class=post__title]")
                 assert post_tag is not None
                 post_title = post_tag.text.replace('\n', '').replace("..", "")
-                prefix = f"{str(url.parts[-1])} - " if self.include_id else ""
+                prefix = f"{url.parts[-1]} - " if self.include_id else ""
                 if title:
                     title = title + '/' + await make_title_safe(prefix + post_title)
                 else:
                     title = await make_title_safe(prefix + post_title)
             elif not title:
                 post_tag = soup.select_one("h1[class=post__title]")
                 assert post_tag is not None
@@ -155,16 +155,16 @@
             downloads = soup.select('a[class=post__attachment-link]')
             for download in downloads:
                 await self.parse_tag(download, url, domain, title, cascade)
 
             text_content = soup.select('div[class=post__content] a')
             await self.map_links(text_content, title, url)
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return title
 
     async def parse_tag(self, tag: Tag, url: URL, domain: str, title: str, cascade: CascadeItem):
         """Convert link from tag to MediaItem and add it to cascade"""
         href: Union[str, List[str], None] = tag.get('href')
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.load_files = URL('https://cyberfile.me/account/ajax/load_files')
         self.file_details = URL('https://cyberfile.me/account/ajax/file_details')
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director for cyberfile scraping"""
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
         domain_obj = DomainItem("cyberfile", {})
 
         download_links = []
         if 'folder' in url.parts:
             Folder_ID = await self.get_folder_id(session, url)
             Content_IDs = None
             if Folder_ID:
@@ -44,30 +44,30 @@
             Content_ID = await self.get_single_contentId(session, url)
             if Content_ID:
                 download_links = await self.get_download_links(session, url, [("Loose CyberFile Files", Content_ID)])
 
         for title, media_item in download_links:
             await domain_obj.add_media(title, media_item)
         await self.SQL_Helper.insert_domain("cyberfile", url, domain_obj)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return domain_obj
 
     async def get_folder_id(self, session: ScrapeSession, url: URL) -> int:
         """Gets the internal ID for a folder"""
         try:
             soup = await session.get_BS4(url)
             script_func = soup.select_one('div[class="page-container horizontal-menu with-sidebar fit-logo-with-sidebar logged-out clear-adblock"] script').text
             script_func = script_func.split('loadImages(')[-1]
             script_func = script_func.split(';')[0]
             nodeId = int(script_func.split(',')[1].replace("'", ""))
             return nodeId
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
             return 0
 
     async def get_folder_content(self, session: ScrapeSession, url: URL, nodeId: int, page: int, title=None):
         """Gets the content id's encased in a folder"""
         data = {"pageType": "folder", "nodeId": nodeId, "pageStart": page, "perPage": 0, "filterOrderBy": ""}
         nodes = []
@@ -108,15 +108,15 @@
             if page < total_pages:
                 contents.extend(await self.get_folder_content(session, url, nodeId, page+1, original_title))
             for node in nodes:
                 contents.extend(await self.get_folder_content(session, url, node, 1, title))
             return contents
 
         except Exception as e:
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
             return []
 
     async def get_single_contentId(self, session: ScrapeSession, url: URL) -> int:
         """Gets an individual content id"""
         try:
             soup = await session.get_BS4(url)
@@ -128,16 +128,16 @@
                     part_a = [x for x in part_a if x[0].isdigit()][0]
                     part_b = part_a.split(");")[0]
                     contentId = int(part_b)
                     return contentId
             return 0
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
             return 0
 
     async def get_shared_ids_and_content(self, session: ScrapeSession, url: URL, page: int) -> Tuple[List, List]:
         """Gets folder id's and content id's from shared links"""
         try:
             # Initial page load to tell server, this is what we want.
@@ -177,16 +177,16 @@
             if page < total_pages:
                 nodes_temp, content_temp = await self.get_shared_ids_and_content(session, url, page + 1)
                 nodes.extend(nodes_temp)
                 contents.extend(content_temp)
             return nodes, contents
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
             return [], []
 
     async def get_shared_content(self, session, url: URL, nodeId: int, page: int, title=None) -> List:
         """Gets content from shared folders"""
         try:
             nodes = []
@@ -222,16 +222,16 @@
             if page < total_pages:
                 contents.extend(await self.get_shared_content(session, url, nodeId, page + 1, title))
             for title, node in nodes:
                 contents.extend(await self.get_shared_content(session, url, node, 1, title))
             return contents
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
             return []
 
     async def get_download_links(self, session: ScrapeSession, url: URL, contentIds: List) -> List:
         """Obtains download links from content ids"""
         download_links = []
         try:
@@ -249,18 +249,18 @@
                     assert button is not None
                     html_download_text = button.get("onclick")
                 assert isinstance(html_download_text, str)
                 link = URL(html_download_text.replace("openUrl('", "").replace("'); return false;", ""))
                 try:
                     media = await create_media_item(link, url, self.SQL_Helper, "cyberfile")
                 except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(link))
+                    logger.debug("Couldn't get extension for %s", link)
                     continue
 
                 download_links.append((title, media))
             return download_links
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
             return []
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,30 +25,30 @@
         self.SQL_Helper = SQL_Helper
         self.quiet = quiet
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Cyberdrop scraper"""
         album_obj = AlbumItem("Loose Cyberdrop Files", [])
 
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
         if await check_direct(url):
             media = await create_media_item(url, url, self.SQL_Helper, "cyberdrop")
             await album_obj.add_media(media)
             await self.SQL_Helper.insert_album("cyberdrop", URL(""), album_obj)
-            log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Finished: {url}", quiet=self.quiet, style="green")
             return album_obj
 
         try:
             try:
                 soup = await session.get_BS4(url)
             except InvalidContentTypeFailure:
                 media = await create_media_item(url, url, self.SQL_Helper, "cyberdrop")
                 await album_obj.add_media(media)
                 await self.SQL_Helper.insert_album("cyberdrop", URL(""), album_obj)
-                log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+                log(f"Finished: {url}", quiet=self.quiet, style="green")
                 return album_obj
 
             title = soup.select_one("h1[id=title]").get_text()
             title = await make_title_safe(title)
             if title is None:
                 title = url.name
             elif self.include_id:
@@ -58,21 +58,21 @@
 
             links = soup.select('div[class="image-container column"] a')
             for link in links:
                 link = URL(link.get('href'))
                 try:
                     media = await create_media_item(link, url, self.SQL_Helper, "cyberdrop")
                 except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(link))
+                    logger.debug("Couldn't get extension for %s", link)
                     continue
 
                 await album_obj.add_media(media)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
             return album_obj
 
         await self.SQL_Helper.insert_album("cyberdrop", url, album_obj)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,20 @@
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for E-Hentai"""
         album_obj = AlbumItem("Loose EHentai Files", [])
 
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
         if "g" in url.parts:
             await self.get_album(session, url, album_obj)
         elif "s" in url.parts:
             await self.get_image(session, url, album_obj)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         await self.SQL_Helper.insert_album("e-hentai", url, album_obj)
         return album_obj
 
     async def get_album(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
         """Gets links from an album"""
         try:
             soup = await session.get_BS4(url)
@@ -51,25 +51,25 @@
                     break
             if next_page is not None:
                 next_page = URL(next_page.get('href'))
                 if next_page is not None:
                     await self.get_album(session, next_page, album_obj)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_image(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
         """Gets media items from image links"""
         try:
             soup = await session.get_BS4(url)
             image = soup.select_one("img[id=img]")
             link = URL(image.get('src'))
 
             media_item = await create_media_item(link, url, self.SQL_Helper, "e-hentai")
             await album_obj.add_media(media_item)
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,22 @@
     def __init__(self, *, include_id: bool, quiet: bool, SQL_Helper: SQLHelper):
         self.include_id = include_id
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director function for Erome scraping"""
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         if 'a' in url.parts:
             domain_obj = await self.handle_album(session, url)
         else:
             domain_obj = await self.handle_profile(session, url)
 
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
 
         return domain_obj
 
     async def handle_album(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Handler function for erome albums, adds media items to the domain item"""
         domain_obj = DomainItem("erome", {})
         try:
@@ -46,32 +46,32 @@
 
             # Images
             for link in soup.select('img[class="img-front lasyload"]'):
                 link = URL(link['data-src'])
                 try:
                     media = await create_media_item(link, url, self.SQL_Helper, "erome")
                 except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(url))
+                    logger.debug("Couldn't get extension for %s", url)
                     continue
                 await domain_obj.add_media(title, media)
 
             # Videos
             for link in soup.select('div[class=media-group] div[class=video-lg] video source'):
                 link = URL(link['src'])
                 try:
                     media = await create_media_item(link, url, self.SQL_Helper, "erome")
                 except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(link))
+                    logger.debug("Couldn't get extension for %s", link)
                     continue
                 await domain_obj.add_media(title, media)
 
             await self.SQL_Helper.insert_domain("erome", url, domain_obj)
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return domain_obj
 
     async def handle_profile(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Handler for erome profiles, sends albums to handle_album"""
         domain_obj = DomainItem("erome", {})
@@ -92,12 +92,12 @@
             next_page = soup.select_one('a[rel="next"]')
             if next_page:
                 next_page = next_page.get("href").split("page=")[-1]
                 next_page = url.with_query(f"page={next_page}")
                 await domain_obj.extend(await self.handle_profile(session, next_page))
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return domain_obj
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 class FapelloCrawler:
     def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> Optional[AlbumItem]:
         """Basic director for fapello"""
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         if not str(url).endswith("/"):
             url = url / ""
 
         album_obj = await self.parse_profile(session, url)
 
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
 
     async def parse_profile(self, session: ScrapeSession, url: URL) -> Optional[AlbumItem]:
         """Profile parser, passes posts to parse_post"""
         try:
             soup, returned_url = await session.get_BS4_and_url(url)
             title = soup.select_one('h2[class="font-semibold lg:text-2xl text-lg mb-2 mt-4"]').get_text()
@@ -59,16 +59,16 @@
                 next_page = next_page.get('href')
                 if next_page:
                     await album_obj.extend(await self.parse_profile(session, URL(next_page)))
             await self.SQL_Helper.insert_album("fapello", url, album_obj)
             return album_obj
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
             return None
 
     async def parse_post(self, session: ScrapeSession, url: URL) -> list[MediaItem]:
         """Parses posts, returns list of MediaItem"""
         results = []
         try:
@@ -78,26 +78,26 @@
 
             images = content_section.select("img")
             for image in images:
                 download_link = URL(image.get('src'))
                 try:
                     media_item = await create_media_item(download_link, url, self.SQL_Helper, "fapello")
                 except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(download_link))
+                    logger.debug("Couldn't get extension for %s", download_link)
                     continue
                 results.append(media_item)
 
             videos = content_section.select("source")
             for video in videos:
                 download_link = URL(video.get('src'))
                 try:
                     media_item = await create_media_item(download_link, url, self.SQL_Helper, "fapello")
                 except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(download_link))
+                    logger.debug("Couldn't get extension for %s", download_link)
                     continue
                 results.append(media_item)
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return results
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Basic scraper for gfycat"""
         album_obj = AlbumItem("Gfycat", [])
         try:
-            log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Starting: {url}", quiet=self.quiet, style="green")
             soup = await session.get_BS4(url)
 
             video = soup.select_one("video[class='video media']")
             video_srcs = video.select("source")
 
             video_link = None
             for src in video_srcs:
@@ -36,14 +36,14 @@
                     break
             if video_link is None:
                 video_link = URL(video_srcs[0].get("src"))
 
             media_item = await create_media_item(video_link, url, self.SQL_Helper, "gfycat")
             await album_obj.add_media(media_item)
             await self.SQL_Helper.insert_album("gfycat", video_link, album_obj)
-            log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Finished: {url}", quiet=self.quiet, style="green")
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return album_obj
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,41 +52,41 @@
         morsel.set('accountToken', client_token, client_token)
         session.client_session.cookie_jar.update_cookies({'gofile.io': morsel})
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Basic director for actual scraping"""
         domain_obj = DomainItem("gofile", {})
         try:
-            log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Starting: {url}", quiet=self.quiet, style="green")
             content_id = url.name
             results = await self.get_links(session, url, content_id, None)
             for title, media_item in results:
                 await domain_obj.add_media(title, media_item)
 
             await self.SQL_Helper.insert_domain("gofile", url, domain_obj)
-            log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Finished: {url}", quiet=self.quiet, style="green")
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return domain_obj
 
     async def get_links(self, session: ScrapeSession, url: URL, content_id: str, title=None) -> List[List]:
         """Gets links from the given url, creates media_items"""
         results: List[List] = []
         params = {
             "token": self.token,
             "contentId": content_id,
             "websiteToken": "12345",
         }
         content = await session.get_json(self.api_address / "getContent", params)
         if content["status"] != "ok":
-            logger.debug("Error encountered while handling %s", str(url))
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             return results
 
         content = content['data']
         if title:
             title = title + "/" + await make_title_safe(content["name"])
         else:
             title = await make_title_safe(content["name"])
@@ -103,15 +103,15 @@
                     link = URL(val["directLink"])
                 else:
                     assert isinstance(val["link"], str)
                     link = URL(val["link"])
                 try:
                     filename, ext = await get_filename_and_ext(val['name'])
                 except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(link))
+                    logger.debug("Couldn't get extension for %s", link)
                     continue
                 complete = await self.SQL_Helper.check_complete_singular("gofile", link)
                 media_item = MediaItem(link, url, complete, filename, ext, filename)
                 results.append([title, media_item])
         for sub_folder in sub_folders:
             assert isinstance(sub_folder, str)
             results.extend(await self.get_links(session, url, sub_folder, title))
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,17 +17,17 @@
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Basic director for HGameCG"""
         album_obj = AlbumItem("Loose HGamesCG Files", [])
 
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
         await self.get_album(session, url, album_obj)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         await self.SQL_Helper.insert_album("hgamecg", url, album_obj)
         return album_obj
 
     async def get_album(self, session: ScrapeSession, url: URL, album_obj: AlbumItem) -> None:
         """Handles album scraping, adds media items to the album_obj"""
         try:
             soup = await session.get_BS4(url)
@@ -49,21 +49,20 @@
                 next_page = next_page.get('href')
                 if next_page is not None:
                     assert url.host is not None
                     next_page = URL("https://" + url.host + next_page)
                     await self.get_album(session, next_page, album_obj)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_image(self, session: ScrapeSession, url: URL) -> URL:
         """Gets image link from the given url."""
         try:
             soup = await session.get_BS4(url)
             image = soup.select_one("div[class=hgamecgimage] img")
-            image = URL(image.get('src'))
-            return image
+            return URL(image.get('src'))
         except Exception:
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             return URL()
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director func for ImgBox scraping"""
         album_obj = AlbumItem("Loose ImgBox Files", [])
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         try:
             if await check_direct(url):
                 media_item = await create_media_item(url, url, self.SQL_Helper, "imgbox")
                 await album_obj.add_media(media_item)
 
             elif "g" in url.parts:
@@ -40,29 +40,29 @@
                     title = url.raw_name
                 title = await make_title_safe(title)
                 await album_obj.set_new_title(title)
                 for img in images:
                     try:
                         media_item = await create_media_item(img, url, self.SQL_Helper, "imgbox")
                     except NoExtensionFailure:
-                        logger.debug("Couldn't get extension for %s", str(img))
+                        logger.debug("Couldn't get extension for %s", img)
                         continue
                     await album_obj.add_media(media_item)
             else:
                 img = await self.singular(session, url)
                 media_item = await create_media_item(img, url, self.SQL_Helper, "imgbox")
                 await album_obj.add_media(media_item)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         await self.SQL_Helper.insert_album("imgbox", url, album_obj)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
 
     async def folder(self, session: ScrapeSession, url: URL):
         """Gets links from a folder"""
         soup = await session.get_BS4(url)
         output = []
         title = soup.select_one("div[id=gallery-view] h1").get_text()
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,36 +24,36 @@
         self.SQL_Helper = SQL_Helper
         self.quiet = quiet
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for lovefap scraping"""
         album_obj = AlbumItem("Loose LoveFap Files", [])
 
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
         if await check_direct(url):
             media = await create_media_item(url, url, self.SQL_Helper, "lovefap")
             await album_obj.add_media(media)
             await self.SQL_Helper.insert_album("lovefap", URL(""), album_obj)
-            log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Finished: {url}", quiet=self.quiet, style="green")
             return album_obj
 
         try:
             if "video" in url.parts:
                 await self.fetch_video(session, url, album_obj)
             else:
                 await self.fetch_album(session, url, album_obj)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
             return album_obj
 
         await self.SQL_Helper.insert_album("lovefap", url, album_obj)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
 
     async def fetch_album(self, session: ScrapeSession, url: URL, album_obj: AlbumItem) -> None:
         """Gets media_items for albums, and adds them to the Album_obj"""
         soup = await session.get_BS4(url)
 
         title = soup.select_one('div[class=albums-content-header] span[style*="float: left"]').get_text()
@@ -71,25 +71,25 @@
             link = URL(link)
             if "video" in link.parts:
                 await self.fetch_video(session, url, album_obj)
             else:
                 try:
                     media = await create_media_item(link, url, self.SQL_Helper, "lovefap")
                 except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(link))
+                    logger.debug("Couldn't get extension for %s", link)
                     continue
 
                 await album_obj.add_media(media)
 
     async def fetch_video(self, session: ScrapeSession, url: URL, album_obj: AlbumItem) -> None:
         """Gets media_items for video links"""
         soup = await session.get_BS4(url)
         video = soup.select_one("video[id=main-video] source")
         if video:
             link = URL(video.get("src"))
             try:
                 media = await create_media_item(link, url, self.SQL_Helper, "lovefap")
             except NoExtensionFailure:
-                logger.debug("Couldn't get extension for %s", str(link))
+                logger.debug("Couldn't get extension for %s", link)
                 return
 
             await album_obj.add_media(media)
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.separate_posts = separate_posts
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director for NSFW.XXX scraping"""
         domain_obj = DomainItem("nsfw.xxx", {})
 
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
         if "user" in url.parts:
             await self.get_user(session, url, domain_obj)
         else:
             await self.get_post(session, url, domain_obj)
         await self.SQL_Helper.insert_domain("nsfw.xxx", url, domain_obj)
         return domain_obj
 
@@ -50,16 +50,16 @@
                     break
 
                 posts = await self.get_post_hrefs(posts)
                 for post in posts:
                     await self.get_post(session, post, domain_obj, model)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_post_hrefs(self, posts) -> List:
         """Gets links from post objects"""
         posts_links = []
         for post in posts:
             url = URL(post.get("href"))
@@ -82,17 +82,17 @@
             for content in content_obj:
                 link = URL(content.get("src"))
                 if "-mobile" in link.name or ".webm" in link.name:
                     continue
                 try:
                     media = await create_media_item(link, url, self.SQL_Helper, "nsfw.xxx")
                 except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(link))
+                    logger.debug("Couldn't get extension for %s", link)
                     continue
 
                 title = f"{model}/{post_name}" if self.separate_posts else model
                 await domain_obj.add_media(title, media)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 class PimpAndHostCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for pimpandhost scraping"""
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
         album_obj = AlbumItem("Loose Pixeldrain Files", [])
 
         if url.parts[1] == 'album':
             media_items, title = await self.get_listings(session, url)
             await album_obj.set_new_title(title)
             if media_items:
                 for media_item in media_items:
                     await album_obj.add_media(media_item)
         else:
             media_item = await self.get_singular(session, url)
             await album_obj.add_media(media_item)
 
         await self.SQL_Helper.insert_album("pimpandhost", url, album_obj)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
 
     async def get_listings(self, session: ScrapeSession, url: URL):
         """Handles album media"""
         media_items = []
         try:
             soup = await session.get_BS4(url)
@@ -48,24 +48,24 @@
 
             for file in soup.select('a[class*="image-wrapper center-cropped im-wr"]'):
                 link = file.get("href")
                 media_items.append(await self.get_singular(session, link))
             return media_items, title
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_singular(self, session: ScrapeSession, url: URL):
         """Handles singular files"""
         try:
             soup = await session.get_BS4(url)
             img = soup.select_one("a img")
             img = img.get("src")
             if img.startswith("//"):
                 img = URL("https:" + img)
             return await create_media_item(img, url, self.SQL_Helper, "pimpandhost")
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.api = URL('https://pixeldrain.com/api/')
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for pixeldrain scraping"""
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
         album_obj = AlbumItem("Loose Pixeldrain Files", [])
 
         identifier = str(url).split('/')[-1]
         if url.parts[1] == 'l':
             await album_obj.set_new_title(url.name)
             media_items = await self.get_listings(session, identifier, url)
             for media_item in media_items:
@@ -34,35 +34,35 @@
             link = await self.create_download_link(identifier)
             complete = await self.SQL_Helper.check_complete_singular("pixeldrain", link)
             filename, ext = await get_filename_and_ext(await self.get_file_name(session, identifier))
             media_item = MediaItem(link, url, complete, filename, ext, filename)
             await album_obj.add_media(media_item)
 
         await self.SQL_Helper.insert_album("pixeldrain", url, album_obj)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
 
     async def get_listings(self, session: ScrapeSession, identifier: str, url: URL) -> List[MediaItem]:
         """Handles album scraping"""
         media_items = []
         try:
             content = await session.get_json(self.api / "list" / identifier)
             for file in content['files']:
                 link = await self.create_download_link(file['id'])
                 try:
                     filename, ext = await get_filename_and_ext(file['name'])
                 except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(link))
+                    logger.debug("Couldn't get extension for %s", link)
                     continue
                 complete = await self.SQL_Helper.check_complete_singular("pixeldrain", link)
                 media_item = MediaItem(link, url, complete, filename, ext, filename)
                 media_items.append(media_item)
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return media_items
 
     async def get_file_name(self, session: ScrapeSession, identifier: str) -> str:
         """Gets filename for the given file identifier"""
         content = await session.get_json(self.api / 'file' / identifier / 'info')
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,32 +19,32 @@
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for PostImg scraping"""
         album_obj = AlbumItem("Loose PostImg Files", [])
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         try:
             if "gallery" in url.parts:
                 content = await self.get_folder(session, url)
                 for media_item in content:
                     await album_obj.add_media(media_item)
             else:
                 media_item = await self.get_singular(session, url)
                 await album_obj.add_media(media_item)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         await self.SQL_Helper.insert_album("postimg", url, album_obj)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
 
     async def get_folder(self, session: ScrapeSession, url: URL) -> List:
         """Handles folder scraping"""
         album = url.raw_name
         data = {"action": "list", "album": album, "page": 0}
         content = []
@@ -56,15 +56,15 @@
             for item in data_out['images']:
                 referer = URL("https://postimg.cc/" + item[0])
                 img = URL(item[4].replace(item[0], item[1]))
 
                 try:
                     media_item = await create_media_item(img, referer, self.SQL_Helper, "postimg")
                 except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(img))
+                    logger.debug("Couldn't get extension for %s", img)
                     continue
 
                 content.append(media_item)
         return content
 
     async def get_singular(self, session: ScrapeSession, url: URL) -> MediaItem:
         """Handles singular folder scraping"""
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Basic director for saint scraping"""
         album_obj = AlbumItem("Loose Saint Files", [])
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         try:
             soup = await session.get_BS4(url)
             link = URL(soup.select_one('video[id=main-video] source').get('src'))
             media_item = await create_media_item(link, url, self.SQL_Helper, "saint")
             await album_obj.add_media(media_item)
             await self.SQL_Helper.insert_album("saint", link, album_obj)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director for ShareX scraper"""
         assert url.host is not None
         domain_obj = DomainItem(url.host.lower(), {})
 
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
 
         if await check_direct(url):
             url = url.with_name(url.name.replace('.md.', '.').replace('.th.', '.'))
             url = await self.jpg_fish_from_church(url)
             media_item = await create_media_item(url, url, self.SQL_Helper, "sharex")
             await domain_obj.add_media("Loose ShareX Files", media_item)
         elif "album" in url.parts or "a" in url.parts:
@@ -45,20 +45,22 @@
             await self.get_albums(session, url, domain_obj)
         elif 'image' in url.parts or 'img' in url.parts or 'images' in url.parts:
             await self.get_singular(session, url, domain_obj)
         else:
             await self.parse_profile(session, url, domain_obj)
 
         await self.SQL_Helper.insert_domain("sharex", url, domain_obj)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return domain_obj
 
     async def jpg_fish_from_church(self, url: URL) -> URL:
-        pattern = r"simp([1-5])\.jpg\.church/"
-        return URL(re.sub(pattern, r'simp\1.jpg.fish/', str(url)))
+        pattern1 = r"simp([1-5])\.jpg\.fish/"
+        url = URL(re.sub(pattern1, r'simp\1.jpg.fishing/', str(url)))
+        pattern2 = r"simp([1-5])\.jpg\.church/"
+        return URL(re.sub(pattern2, r'simp\1.jpg.fishing/', str(url)))
 
     async def get_albums(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Handles scraping for Albums"""
         try:
             soup = await session.get_BS4(url)
             albums = soup.select("a[class='image-container --media']")
             for album in albums:
@@ -71,47 +73,47 @@
             if next_page is not None:
                 next_page = next_page.get('href')
                 if next_page is not None:
                     next_page = URL(next_page)
                     await self.get_albums(session, next_page, domain_obj)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_singular(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Handles scraping for singular files"""
         await asyncio.sleep(1)
         try:
             soup = await session.get_BS4(url)
             link = URL(soup.select_one("input[id=embed-code-2]").get('value'))
             link = link.with_name(link.name.replace('.md.', '.').replace('.th.', '.'))
             link = await self.jpg_fish_from_church(link)
 
             media_item = await create_media_item(link, url, self.SQL_Helper, "sharex")
             await domain_obj.add_media("Loose ShareX Files", media_item)
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_sub_album_links(self, session: ScrapeSession, url: URL, og_title: str,
                                   domain_obj: DomainItem) -> None:
         try:
             soup = await session.get_BS4(url)
             albums = soup.select("div[class=pad-content-listing] div")
             for album in albums:
                 album_url = album.get('data-url-short')
                 if album_url is not None:
                     album_url = URL(album_url)
                     await self.parse(session=session, url=album_url, og_title=og_title, domain_obj=domain_obj)
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def parse_profile(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Handles scraping for profiles"""
         try:
             soup = await session.get_BS4(url)
             title = soup.select_one("div[class=header] h1 strong").get_text()
@@ -120,16 +122,16 @@
             elif self.include_id:
                 titlep2 = url.name
                 title = title + " - " + titlep2
             title = await make_title_safe(title.replace(r"\n", "").strip())
             await self.get_list_links(session, url, title, domain_obj)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_list_links(self, session: ScrapeSession, url: URL, title: str, domain_obj: DomainItem) -> None:
         """Gets final links and adds to domain_obj"""
         try:
             soup = await session.get_BS4(url)
             assert url.host is not None
@@ -141,29 +143,29 @@
                 link = URL(link.get('src'))
                 link = link.with_name(link.name.replace('.md.', '.').replace('.th.', '.'))
                 link = await self.jpg_fish_from_church(link)
 
                 try:
                     media_item = await create_media_item(link, url, self.SQL_Helper, "sharex")
                 except NoExtensionFailure:
-                    logger.debug("Couldn't get extension for %s", str(link))
+                    logger.debug("Couldn't get extension for %s", link)
                     continue
                 await domain_obj.add_media(title, media_item)
 
             next_page = soup.select_one('li.pagination-next a')
             if not next_page:
                 next_page = soup.select_one('a[data-pagination=next]')
             if next_page is not None:
                 next_page = next_page.get('href')
                 if next_page is not None:
                     next_page = URL(next_page)
                     await self.get_list_links(session, next_page, title, domain_obj)
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def parse(self, *, session: ScrapeSession, url: URL, og_title=None, domain_obj: DomainItem) -> None:
         try:
             soup = await session.get_BS4(url)
 
             title = soup.select_one("a[data-text=album-name]").get_text()
@@ -181,10 +183,10 @@
                 sub_albums = URL(soup.select_one("a[id=tab-sub-link]").get("href"))
                 await self.get_sub_album_links(session, sub_albums, title, domain_obj)
             finally:
                 list_recent = URL(soup.select_one("a[id=list-most-recent-link]").get("href"))
                 await self.get_list_links(session, list_recent, title, domain_obj)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,19 +35,19 @@
                 title = title.strip()
                 await album_obj.set_new_title(title)
                 for link in links:
                     link = URL(link.get('href'))
                     try:
                         media_item = await create_media_item(link, url, self.SQL_Helper, "xbunkr")
                     except NoExtensionFailure:
-                        logger.debug("Couldn't get extension for %s", str(link))
+                        logger.debug("Couldn't get extension for %s", link)
                         continue
                     await album_obj.add_media(media_item)
 
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log("Error scraping " + str(url), quiet=self.quiet)
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error scraping {url}", quiet=self.quiet)
             logger.debug(e)
 
         await self.SQL_Helper.insert_album("xbunkr", URL(""), album_obj)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return album_obj
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,47 +152,46 @@
                        for domain, name in self.domains.items()}
 
         self.scraping_mapper = scraping_mapper
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> Tuple[CascadeItem, str]:
         """Xenforo forum director"""
-        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {url}", quiet=self.quiet, style="green")
         cascade = CascadeItem({})
 
         scrape_url, post_num = await self.get_thread_url_and_post_num(url)
         title = ""
         try:
             assert url.host is not None
             domain = next((domain for domain in self.domains if domain in url.host), None)
             if domain:
                 parse_spec = ParseSpec(domain)
                 await self.forums[domain].login(session, url, parse_spec, self.quiet)
                 title = await self.parse_forum(session, scrape_url, parse_spec, cascade, "", post_num)
         except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", url, exc_info=True)
+            log(f"Error: {url}", quiet=self.quiet, style="red")
             logger.debug(e)
             return cascade, ""
 
         await self.SQL_Helper.insert_cascade(cascade)
-        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {url}", quiet=self.quiet, style="green")
         return cascade, title
 
     async def get_thread_url_and_post_num(self, url: URL):
         """Splits the thread url and returns the url and post number if provided"""
         post_number = 0
         if "post-" in str(url):
             post_number_parts = str(url).rsplit("post-", 1)
             post_number = int(post_number_parts[-1].strip("/")) if len(post_number_parts) == 2 else 0
             url = URL(post_number_parts[0].rstrip("#"))
         return url, post_number
 
-    async def get_links(self, post_content: bs4.Tag, selector: str, attribute: str, domain: URL,
-                        temp_title: str) -> List:
+    async def get_links(self, post_content: bs4.Tag, selector: str, attribute: str, domain: URL) -> List[str]:
         """Grabs links from the post content based on the given selector and attribute"""
         found_links: List = []
         if not post_content:
             return found_links
         links = post_content.select(selector)
         for link_tag in links:
             link = link_tag.get(attribute)
@@ -201,72 +200,60 @@
             assert isinstance(link, str)
             if link.endswith("/"):
                 link = link[:-1]
             if link.startswith('//'):
                 link = "https:" + link
             elif link.startswith('/'):
                 link = str(domain / link[1:])
-            found_links.append([URL(link), temp_title])
+            found_links.append(link)
         return found_links
 
-    async def get_embedded(self, post_content: bs4.Tag, selector: str, attribute: str, temp_title: str) -> List:
+    async def get_embedded(self, post_content: bs4.Tag, selector: str, attribute: str) -> List[str]:
         """Gets embedded media from post content based on selector and attribute provided"""
         found_links = []
         links = post_content.select(selector)
-        for link in links:
-            embed_data = link.get(attribute)
+        for link_tag in links:
+            embed_data = link_tag.get(attribute)
             assert isinstance(embed_data, str)
             embed_data = embed_data.replace("\/\/", "https://www.")
             embed_data = embed_data.replace("\\", "")
 
             embed = re.search(
                 r"https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{2,256}\.[a-z]{2,4}\\b([-a-zA-Z0-9@:%_\+.~#?&//=]*)",
                 embed_data)
             if embed:
-                embed_url = URL(embed.group(0).replace("www.", ""))
-                found_links.append([embed_url, temp_title])
+                embed_link = embed.group(0).replace("www.", "")
+                found_links.append(embed_link)
 
             embed = re.search(
                 r"https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{2,256}\.[a-z]{2,4}\/[-a-zA-Z0-9@:%._\+~#=]*\/[-a-zA-Z0-9@:?&%._\+~#=]*",
                 embed_data)
             if embed:
-                embed_url = URL(embed.group(0).replace("www.", ""))
-                found_links.append([embed_url, temp_title])
+                embed_link = embed.group(0).replace("www.", "")
+                found_links.append(embed_link)
         return found_links
 
-    async def filter_content_links(self, cascade: CascadeItem, content_links: List, url: URL, domain: str):
-        """Splits given links into direct links and external links,
-        returns external links, adds internal to the cascade"""
-        assert url.host is not None
-        forum_direct_urls = [x for x in content_links if x[0].host.replace(".st", ".su") in url.host]
-        forum_direct_urls.extend([x for x in content_links if url.host in x[0].host.replace(".st", ".su")])
-        forum_direct_urls.extend([x for x in content_links if "smgmedia" in x[0].host])
-        content_links = [x for x in content_links if x not in forum_direct_urls]
-        for link_title_bundle in forum_direct_urls:
-            link, temp_title = link_title_bundle
-            in_prog_title = temp_title + "/Attachments"
+    async def handle_direct_links(self, cascade: CascadeItem, content_links: List, url: URL, domain: str):
+        """Adds given links to the cascade"""
+        for link, title in content_links:
             if str(link).endswith("/"):
                 link = URL(str(link)[:-1])
-            if 'attachments' in link.parts or 'content' in link.parts or 'data' in link.parts:
-                completed = await self.SQL_Helper.check_complete_singular(domain, link)
+            if any(s in link.parts for s in ('attachments', 'content', 'data')):
                 try:
                     filename, ext = await get_filename_and_ext(link.name, True)
                 except NoExtensionFailure:
                     continue
+                completed = await self.SQL_Helper.check_complete_singular(domain, link)
                 media = MediaItem(link, url, completed, filename, ext, filename)
-                await cascade.add_to_album(domain, in_prog_title, media)
-        return content_links
+                await cascade.add_to_album(domain, f"{title}/Attachments", media)
 
     async def handle_external_links(self, content_links: List, referer: URL) -> None:
         """Maps external links to the scraper class"""
-        tasks = []
-        for link_title_bundle in content_links:
-            link = link_title_bundle[0]
-            temp_title = link_title_bundle[1]
-            tasks.append(asyncio.create_task(self.scraping_mapper.map_url(link, temp_title, referer)))
+        tasks = [asyncio.create_task(self.scraping_mapper.map_url(link, title, referer))
+                 for link, title in content_links]
         if tasks:
             await asyncio.wait(tasks)
 
     async def parse_forum(self, session: ScrapeSession, url: URL, spec: ParseSpec, cascade: CascadeItem,
                           title: str, post_number: int) -> str:
         """Parses forum threads"""
         soup = await session.get_BS4(url)
@@ -297,39 +284,41 @@
             temp_title = title + "/" + post_num_str if self.separate_posts else title
 
             for elem in post.find_all(spec.block_quote_tag):
                 elem.decompose()
             post_content = post.select_one(spec.post_content_tag)
 
             # Get Links
-            content_links.extend(await self.get_links(post_content, spec.links_tag, spec.links_attribute, domain,
-                                                      temp_title))
+            links = await self.get_links(post_content, spec.links_tag, spec.links_attribute, domain)
 
             # Get Images
-            content_links.extend(await self.get_links(post_content, spec.images_tag, spec.images_attribute, domain,
-                                                      temp_title))
+            links.extend(await self.get_links(post_content, spec.images_tag, spec.images_attribute, domain))
 
             # Get Videos:
-            content_links.extend(await self.get_links(post_content, spec.video_tag, spec.video_attribute, domain,
-                                                      temp_title))
-            content_links.extend(await self.get_links(post_content, spec.saint_iframe_tag,
-                                                      spec.saint_iframe_attribute, domain, temp_title))
+            links.extend(await self.get_links(post_content, spec.video_tag, spec.video_attribute, domain))
+            links.extend(await self.get_links(post_content, spec.saint_iframe_tag, spec.saint_iframe_attribute, domain))
 
             # Get Other Embedded Content
-            content_links.extend(await self.get_embedded(post_content, spec.embedded_content_tag,
-                                                         spec.embedded_content_attribute, temp_title))
+            links.extend(await self.get_embedded(post_content, spec.embedded_content_tag, spec.embedded_content_attribute))
 
             # Get Attachments
             attachments_block = post.select_one(spec.attachment_block_tag)
-            content_links.extend(await self.get_links(attachments_block, spec.attachment_tag,
-                                                      spec.attachment_attribute, domain, temp_title))
+            links.extend(await self.get_links(attachments_block, spec.attachment_tag, spec.attachment_attribute, domain))
+
+            content_links.extend([(URL(link), temp_title) for link in links])
 
         # Handle links
-        content_links = await self.filter_content_links(cascade, content_links, url, spec.domain)
-        await self.handle_external_links(content_links, url)
+        def is_direct_link(host: str) -> bool:
+            host_su = host.replace(".st", ".su")
+            return host_su in url.host or url.host in host_su or "smgmedia" in host
+
+        direct_links = [x for x in content_links if is_direct_link(x[0].host)]
+        external_links = [x for x in content_links if x not in direct_links]
+        await self.handle_direct_links(cascade, direct_links, url, spec.domain)
+        await self.handle_external_links(external_links, url)
 
         next_page = soup.select_one(spec.next_page_tag)
         if next_page is not None:
             next_page = next_page.get(spec.next_page_attribute)
             if next_page is not None:
                 if next_page.startswith('/'):
                     next_page = domain / next_page[1:]
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/downloaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
                 file_progress.update(file_task, visible=False)
 
             if hasattr(e, "message"):
                 logging.debug(f"\n{media.url} ({e.message})")
 
             if hasattr(e, "code"):
                 if await is_4xx_client_error(e.code) and e.code != HTTPStatus.TOO_MANY_REQUESTS:
-                    logger.debug("We ran into a 400 level error: %s", str(e.code))
+                    logger.debug("We ran into a 400 level error: %s", e.code)
                     log(f"Failed Download: {media.filename}", quiet=True)
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
                 if e.code == HTTPStatus.SERVICE_UNAVAILABLE or e.code == HTTPStatus.BAD_GATEWAY \
@@ -277,15 +277,15 @@
                     log(f"Failed Download: {media.filename}", quiet=True)
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
 
-                logger.debug("Error status code: " + str(e.code))
+                logger.debug("Error status code: %s", e.code)
 
             raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
 
     async def output_failed(self, media: MediaItem, e: Any) -> None:
         if self.errored_output:
             async with aiofiles.open(self.errored_file, mode='a') as file:
                 await file.write(f"{media.url},{media.referer},{e.message}\n")
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                 await self.File_Lock.remove_lock(original_filename)
 
             if hasattr(e, "message"):
                 logging.debug(f"\n{media.url} ({e.message})")
 
             if hasattr(e, "code"):
                 if await is_4xx_client_error(e.code) and e.code != HTTPStatus.TOO_MANY_REQUESTS:
-                    logger.debug("We ran into a 400 level error: %s", str(e.code))
+                    logger.debug("We ran into a 400 level error: %s", e.code)
                     log(f"Failed Download: {media.filename}", quiet=True)
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
                 if e.code == HTTPStatus.SERVICE_UNAVAILABLE or e.code == CustomHTTPStatus.WEB_SERVER_IS_DOWN:
@@ -222,15 +222,15 @@
                         logging.debug(f"\n{media.url} ({e.message})")
                     log(f"Failed Download: {media.filename}", quiet=True)
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
-                logger.debug("Error status code: " + str(e.code))
+                logger.debug("Error status code: %s", e.code)
 
             raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
 
     async def output_failed(self, media: MediaItem, e: Any) -> None:
         if self.errored_output:
             async with aiofiles.open(self.errored_file, mode='a') as file:
                 await file.write(f"{media.url},{media.referer},{e.message}\n")
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/main.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,8 +52,8 @@
                     "links": str(url),
                     "packageName": title if title else "Cyberdrop-DL",
                     "overwritePackagizerRules": True
                     }])
 
             except (JDownloaderFailure, AssertionError) as e:
                 logging.debug(e)
-                log(f"Failed to send {str(url)} to JDownloader", quiet=self.quiet, style="red")
+                log(f"Failed to send {url} to JDownloader", quiet=self.quiet, style="red")
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.1.25/cyberdrop_dl/scraper/Scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,33 +358,33 @@
     """URL to Function Mapper"""
 
     async def is_skip_host(self, host: str) -> bool:
         if self.only_data.sites:
             return not any(site in host for site in self.only_data.sites)
         return any(site in host for site in self.skip_data.sites)
 
-    async def map_url(self, url_to_map: URL, title=None, referer=None):
+    async def map_url(self, url_to_map: URL, title=None, referer: URL = None):
         if not url_to_map:
             return
         if not url_to_map.host:
-            log(f"Not Supported: {str(url_to_map)}", quiet=self.quiet, style="yellow")
+            log(f"Not Supported: {url_to_map}", quiet=self.quiet, style="yellow")
             return
 
         key = next((key for key in self.mapping if key in url_to_map.host), None)
         if key:
             if await self.is_skip_host(key):
-                log(f"Skipping: {str(url_to_map)}", quiet=self.quiet, style="yellow")
+                log(f"Skipping: {url_to_map}", quiet=self.quiet, style="yellow")
             else:
                 handler = self.mapping[key]
                 await handler(url=url_to_map, title=title)
             return
 
         if self.jdownloader.jdownloader_enable:
             await self.jdownloader.direct_unsupported_to_jdownloader(url_to_map, title)
 
         else:
-            log(f"Not Supported: {str(url_to_map)}", quiet=self.quiet, style="yellow")
+            log(f"Not Supported: {url_to_map}", quiet=self.quiet, style="yellow")
             if self.unsupported_output:
                 title = title.encode("ascii", "ignore")
                 title = title.decode().strip()
                 async with aiofiles.open(self.unsupported_file, mode='a') as f:
-                    await f.write(f"{str(url_to_map)},{str(referer)},{title}\n")
+                    await f.write(f"{url_to_map},{referer},{title}\n")
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.24
+Version: 4.1.25
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.24 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.25 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.24/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.1.25/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.24/setup.cfg` & `cyberdrop-dl-4.1.25/setup.cfg`

 * *Files identical despite different names*

