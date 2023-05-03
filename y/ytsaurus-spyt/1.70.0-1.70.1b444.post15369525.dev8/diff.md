# Comparing `tmp/ytsaurus-spyt-1.70.0.tar.gz` & `tmp/ytsaurus-spyt-1.70.1b444.post15369525.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ytsaurus-spyt-1.70.0.tar", last modified: Tue May  2 12:45:20 2023, max compression
+gzip compressed data, was "dist/ytsaurus-spyt-1.70.1b444.post15369525.dev8.tar", last modified: Wed May  3 19:50:33 2023, max compression
```

## Comparing `ytsaurus-spyt-1.70.0.tar` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/deps/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/deps/bin/
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/deps/bin/spark-discovery-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11500 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/deps/bin/spark-launch-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/deps/bin/spark-manage-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/deps/bin/spark-shell-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/deps/bin/spark-submit-yt
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/deps/jars/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798358 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/deps/jars/spark-yt-submit.jar
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/spyt/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.0/spyt/__init__.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.0/spyt/client.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.0/spyt/common.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7357 2023-05-02 09:06:19.000000 ytsaurus-spyt-1.70.0/spyt/conf.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.0/spyt/dependency_utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3877 2023-05-02 09:06:19.000000 ytsaurus-spyt-1.70.0/spyt/enabler.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    36987 2023-05-02 12:00:43.000000 ytsaurus-spyt-1.70.0/spyt/standalone.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.0/spyt/submit.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.0/spyt/types.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.0/spyt/utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      135 2023-05-02 12:44:05.000000 ytsaurus-spyt-1.70.0/spyt/version.py
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/ytsaurus_spyt.egg-info/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      311 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/ytsaurus_spyt.egg-info/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/ytsaurus_spyt.egg-info/SOURCES.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/ytsaurus_spyt.egg-info/dependency_links.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/ytsaurus_spyt.egg-info/requires.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/ytsaurus_spyt.egg-info/top_level.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.70.0/MANIFEST.in
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.70.0/setup.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      311 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-05-02 12:45:20.000000 ytsaurus-spyt-1.70.0/setup.cfg
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

### Comparing `ytsaurus-spyt-1.70.0/deps/bin/spark-discovery-yt` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-discovery-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/deps/bin/spark-launch-yt` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-launch-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/deps/bin/spark-manage-yt` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-manage-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/deps/bin/spark-shell-yt` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-shell-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/deps/bin/spark-submit-yt` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/bin/spark-submit-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/deps/jars/spark-yt-submit.jar` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/deps/jars/spark-yt-submit.jar`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,60 +1,60 @@
-Zip file size: 1798358 bytes, number of entries: 638
--rw----     2.0 fat      352 bX defN 23-May-02 15:45 META-INF/MANIFEST.MF
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 com/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 com/twitter/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 com/twitter/scalding/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 org/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 org/apache/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 org/apache/spark/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 org/apache/spark/deploy/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 org/apache/spark/deploy/rest/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 org/scalactic/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 org/scalactic/anyvals/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 org/scalactic/exceptions/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 org/scalactic/source/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 py4j/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 py4j/commands/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 py4j/model/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 py4j/reflection/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 tech/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 tech/ytsaurus/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 tech/ytsaurus/spyt/
--rw----     1.0 fat        0 b- stor 23-May-02 15:45 tech/ytsaurus/spyt/submit/
+Zip file size: 1798378 bytes, number of entries: 638
+-rw----     2.0 fat      400 bX defN 23-May-03 21:04 META-INF/MANIFEST.MF
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 com/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 com/twitter/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 com/twitter/scalding/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 org/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 org/apache/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 org/apache/spark/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 org/apache/spark/deploy/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 org/apache/spark/deploy/rest/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 org/scalactic/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 org/scalactic/anyvals/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 org/scalactic/exceptions/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 org/scalactic/source/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 py4j/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 py4j/commands/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 py4j/model/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 py4j/reflection/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 tech/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 tech/ytsaurus/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 tech/ytsaurus/spyt/
+-rw----     1.0 fat        0 b- stor 23-May-03 21:04 tech/ytsaurus/spyt/submit/
 -rw----     2.0 fat     6650 bl defN 23-May-02 15:45 com/twitter/scalding/Args$.class
 -rw----     2.0 fat    17269 bl defN 23-May-02 15:45 com/twitter/scalding/Args.class
 -rw----     2.0 fat     1739 bl defN 23-May-02 15:45 com/twitter/scalding/ArgsException$.class
 -rw----     2.0 fat     4404 bl defN 23-May-02 15:45 com/twitter/scalding/ArgsException.class
 -rw----     2.0 fat     1722 bl defN 23-May-02 15:45 com/twitter/scalding/Range$.class
 -rw----     2.0 fat     8164 bl defN 23-May-02 15:45 com/twitter/scalding/Range.class
 -rw----     2.0 fat      741 bl defN 23-May-02 15:45 com/twitter/scalding/RangedArgs$.class
 -rw----     2.0 fat     3189 bl defN 23-May-02 15:45 com/twitter/scalding/RangedArgs.class
--rw----     2.0 fat      560 bl defN 23-May-02 15:45 log4j.properties
--rw----     2.0 fat     1253 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/ApplicationState.class
--rw----     2.0 fat     2304 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/DriverInfo$.class
--rw----     2.0 fat     5759 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/DriverInfo.class
--rw----     2.0 fat      651 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/DriverState$1.class
--rw----     2.0 fat      560 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/DriverState$2.class
--rw----     2.0 fat     1989 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/DriverState.class
--rw----     2.0 fat    11883 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/MasterClient$.class
--rw----     2.0 fat     4814 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$31$1$$anon$3.class
--rw----     2.0 fat     2222 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$31$1$$anon$4.class
--rw----     2.0 fat     4524 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$31$1$anon$macro$29$1.class
--rw----     2.0 fat     6175 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$31$1.class
--rw----     2.0 fat     3011 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$9$1$$anon$1.class
--rw----     2.0 fat     1771 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$9$1$$anon$2.class
--rw----     2.0 fat     2901 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$9$1$anon$macro$7$1.class
--rw----     2.0 fat     5180 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$9$1.class
--rw----     2.0 fat     2343 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/MasterClient.class
--rw----     2.0 fat     2296 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/ResourceInfo$.class
--rw----     2.0 fat     5639 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/ResourceInfo.class
--rw----     2.0 fat     2411 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/RestSubmissionClientWrapper$.class
--rw----     2.0 fat     2186 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/RestSubmissionClientWrapper.class
--rw----     2.0 fat     3673 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/WorkerInfo$.class
--rw----     2.0 fat     9398 bl defN 23-May-02 15:45 org/apache/spark/deploy/rest/WorkerInfo.class
+-rw----     2.0 fat      560 bl defN 23-May-03 21:04 log4j.properties
+-rw----     2.0 fat     1253 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/ApplicationState.class
+-rw----     2.0 fat     2304 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/DriverInfo$.class
+-rw----     2.0 fat     5759 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/DriverInfo.class
+-rw----     2.0 fat      651 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/DriverState$1.class
+-rw----     2.0 fat      560 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/DriverState$2.class
+-rw----     2.0 fat     1989 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/DriverState.class
+-rw----     2.0 fat    11883 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/MasterClient$.class
+-rw----     2.0 fat     4814 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$31$1$$anon$3.class
+-rw----     2.0 fat     2222 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$31$1$$anon$4.class
+-rw----     2.0 fat     4524 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$31$1$anon$macro$29$1.class
+-rw----     2.0 fat     6175 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$31$1.class
+-rw----     2.0 fat     3011 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$9$1$$anon$1.class
+-rw----     2.0 fat     1771 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$9$1$$anon$2.class
+-rw----     2.0 fat     2901 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$9$1$anon$macro$7$1.class
+-rw----     2.0 fat     5180 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/MasterClient$anon$lazy$macro$9$1.class
+-rw----     2.0 fat     2343 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/MasterClient.class
+-rw----     2.0 fat     2296 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/ResourceInfo$.class
+-rw----     2.0 fat     5639 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/ResourceInfo.class
+-rw----     2.0 fat     2411 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/RestSubmissionClientWrapper$.class
+-rw----     2.0 fat     2186 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/RestSubmissionClientWrapper.class
+-rw----     2.0 fat     3673 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/WorkerInfo$.class
+-rw----     2.0 fat     9398 bl defN 23-May-03 21:04 org/apache/spark/deploy/rest/WorkerInfo.class
 -rw----     2.0 fat     1850 bl defN 23-May-02 15:45 org/scalactic/AbstractStringUniformity.class
 -rw----     2.0 fat     4793 bl defN 23-May-02 15:45 org/scalactic/Accumulation$$anon$10.class
 -rw----     2.0 fat     4394 bl defN 23-May-02 15:45 org/scalactic/Accumulation$$anon$11.class
 -rw----     2.0 fat     2166 bl defN 23-May-02 15:45 org/scalactic/Accumulation$$anon$12.class
 -rw----     2.0 fat     5307 bl defN 23-May-02 15:45 org/scalactic/Accumulation$$anon$3.class
 -rw----     2.0 fat     4338 bl defN 23-May-02 15:45 org/scalactic/Accumulation$$anon$4.class
 -rw----     2.0 fat     4284 bl defN 23-May-02 15:45 org/scalactic/Accumulation$$anon$5.class
@@ -619,22 +619,22 @@
 -rw----     2.0 fat     4293 bl defN 23-May-02 15:45 py4j/reflection/PythonProxyHandler.class
 -rw----     2.0 fat      911 bl defN 23-May-02 15:45 py4j/reflection/ReflectionEngine$1.class
 -rw----     2.0 fat    14423 bl defN 23-May-02 15:45 py4j/reflection/ReflectionEngine.class
 -rw----     2.0 fat     1179 bl defN 23-May-02 15:45 py4j/reflection/ReflectionUtil.class
 -rw----     2.0 fat      814 bl defN 23-May-02 15:45 py4j/reflection/RootClassLoadingStrategy.class
 -rw----     2.0 fat     2054 bl defN 23-May-02 15:45 py4j/reflection/TypeConverter.class
 -rw----     2.0 fat    10589 bl defN 23-May-02 15:45 py4j/reflection/TypeUtil.class
--rw----     2.0 fat     1000 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/InProcessLauncherPythonUtils$.class
--rw----     2.0 fat     1047 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/InProcessLauncherPythonUtils.class
--rw----     2.0 fat     7052 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/PythonGatewayServer$.class
--rw----     2.0 fat      944 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/PythonGatewayServer$delayedInit$body.class
--rw----     2.0 fat     1987 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/PythonGatewayServer.class
--rw----     2.0 fat     2915 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/RetryConfig$.class
--rw----     2.0 fat     6162 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/RetryConfig.class
--rw----     2.0 fat     6531 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/SparkCluster$.class
--rw----     2.0 fat     7177 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/SparkCluster.class
--rw----     2.0 fat     1091 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/SubmissionClient$$anon$1.class
--rw----     2.0 fat      893 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/SubmissionClient$$anon$2.class
--rw----     2.0 fat     2292 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/SubmissionClient$SubmissionFiles$.class
--rw----     2.0 fat     3692 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/SubmissionClient$SubmissionFiles.class
--rw----     2.0 fat    32170 bl defN 23-May-02 15:45 tech/ytsaurus/spyt/submit/SubmissionClient.class
-638 files, 4775082 bytes uncompressed, 1686550 bytes compressed:  64.7%
+-rw----     2.0 fat     1000 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/InProcessLauncherPythonUtils$.class
+-rw----     2.0 fat     1047 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/InProcessLauncherPythonUtils.class
+-rw----     2.0 fat     7052 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/PythonGatewayServer$.class
+-rw----     2.0 fat      944 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/PythonGatewayServer$delayedInit$body.class
+-rw----     2.0 fat     1987 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/PythonGatewayServer.class
+-rw----     2.0 fat     2915 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/RetryConfig$.class
+-rw----     2.0 fat     6162 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/RetryConfig.class
+-rw----     2.0 fat     6531 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/SparkCluster$.class
+-rw----     2.0 fat     7177 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/SparkCluster.class
+-rw----     2.0 fat     1091 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/SubmissionClient$$anon$1.class
+-rw----     2.0 fat      893 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/SubmissionClient$$anon$2.class
+-rw----     2.0 fat     2292 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/SubmissionClient$SubmissionFiles$.class
+-rw----     2.0 fat     3692 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/SubmissionClient$SubmissionFiles.class
+-rw----     2.0 fat    32170 bl defN 23-May-03 21:04 tech/ytsaurus/spyt/submit/SubmissionClient.class
+638 files, 4775130 bytes uncompressed, 1686570 bytes compressed:  64.7%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,10 +1,10 @@
 Manifest-Version: 1.0
 Main-Class: tech.ytsaurus.spyt.submit.PythonGatewayServer
 Specification-Title: spark-yt-spark-submit
-Specification-Version: 1.70.0
+Specification-Version: 1.70.1-444-22228096-2-SNAPSHOT
 Specification-Vendor: tech.ytsaurus
 Implementation-Title: spark-yt-spark-submit
-Implementation-Version: 1.70.0
+Implementation-Version: 1.70.1-444-22228096-2-SNAPSHOT
 Implementation-Vendor: tech.ytsaurus
 Implementation-Vendor-Id: tech.ytsaurus
```

### Comparing `ytsaurus-spyt-1.70.0/spyt/client.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/client.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/spyt/common.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/common.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/spyt/conf.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/conf.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/spyt/enabler.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/enabler.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/spyt/standalone.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/standalone.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/spyt/submit.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/submit.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/spyt/types.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/types.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/spyt/utils.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/spyt/utils.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/ytsaurus_spyt.egg-info/SOURCES.txt` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/ytsaurus_spyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.0/setup.py` & `ytsaurus-spyt-1.70.1b444.post15369525.dev8/setup.py`

 * *Files identical despite different names*

