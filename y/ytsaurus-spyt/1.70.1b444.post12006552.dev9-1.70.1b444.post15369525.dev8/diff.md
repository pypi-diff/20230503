# Comparing `tmp/ytsaurus-spyt-1.70.1b444.post12006552.dev9.tar.gz` & `tmp/ytsaurus-spyt-1.70.1b444.post15369525.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ytsaurus-spyt-1.70.1b444.post12006552.dev9.tar", last modified: Wed May  3 19:53:03 2023, max compression
+gzip compressed data, was "dist/ytsaurus-spyt-1.70.1b444.post15369525.dev8.tar", last modified: Wed May  3 19:50:33 2023, max compression
```

## Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9.tar` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/bin/
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/bin/spark-discovery-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11500 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/bin/spark-launch-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/bin/spark-manage-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/bin/spark-shell-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/bin/spark-submit-yt
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/jars/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798378 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/jars/spark-yt-submit.jar
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/__init__.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/client.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/common.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7357 2023-05-02 09:06:19.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/conf.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/dependency_utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3877 2023-05-02 09:06:19.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/enabler.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    36987 2023-05-02 12:00:43.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/standalone.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/submit.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/types.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      181 2023-05-03 19:52:05.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/version.py
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/ytsaurus_spyt.egg-info/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      333 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/ytsaurus_spyt.egg-info/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/ytsaurus_spyt.egg-info/SOURCES.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/ytsaurus_spyt.egg-info/dependency_links.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/ytsaurus_spyt.egg-info/requires.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/ytsaurus_spyt.egg-info/top_level.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/MANIFEST.in
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/setup.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      333 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-05-03 19:53:03.000000 ytsaurus-spyt-1.70.1b444.post12006552.dev9/setup.cfg
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-discovery-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11500 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-launch-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-manage-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-shell-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-submit-yt
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/jars/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798378 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/jars/spark-yt-submit.jar
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/__init__.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/client.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/common.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7357 2023-05-02 09:06:19.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/conf.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/dependency_utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3877 2023-05-02 09:06:19.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/enabler.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    36987 2023-05-02 12:00:43.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/standalone.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/submit.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/types.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      181 2023-05-03 19:48:58.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/version.py
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/ytsaurus_spyt.egg-info/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      333 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/ytsaurus_spyt.egg-info/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/ytsaurus_spyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/ytsaurus_spyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/ytsaurus_spyt.egg-info/requires.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/ytsaurus_spyt.egg-info/top_level.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/MANIFEST.in
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/setup.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      333 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-05-03 19:50:33.000000 ytsaurus-spyt-1.70.1b444.post15369525.dev8/setup.cfg
```

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/bin/spark-discovery-yt` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-discovery-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/bin/spark-launch-yt` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-launch-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/bin/spark-manage-yt` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-manage-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/bin/spark-shell-yt` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-shell-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/bin/spark-submit-yt` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-submit-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/deps/jars/spark-yt-submit.jar` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/jars/spark-yt-submit.jar`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/client.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/client.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/common.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/common.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/conf.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/conf.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/enabler.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/enabler.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/standalone.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/standalone.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/submit.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/submit.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/types.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/types.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/spyt/utils.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/utils.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/ytsaurus_spyt.egg-info/SOURCES.txt` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/ytsaurus_spyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b444.post12006552.dev9/setup.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/setup.py`

 * *Files identical despite different names*

