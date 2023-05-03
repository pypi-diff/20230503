# Comparing `tmp/scicam-0.1.2.tar.gz` & `tmp/scicam-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicam-0.1.2.tar", last modified: Sat Aug 20 17:33:04 2022, max compression
+gzip compressed data, was "scicam-0.1.3.tar", last modified: Wed May  3 08:43:09 2023, max compression
```

## Comparing `scicam-0.1.2.tar` & `scicam-0.1.3.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-08-20 17:33:04.038201 scicam-0.1.2/
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       73 2022-08-20 17:33:04.038201 scicam-0.1.2/PKG-INFO
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       72 2022-02-10 13:10:24.000000 scicam-0.1.2/README.md
-drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-08-20 17:33:04.034201 scicam-0.1.2/scicam/
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       22 2022-08-20 17:32:01.000000 scicam-0.1.2/scicam/__init__.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       22 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/_version.py
-drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-08-20 17:33:04.038201 scicam-0.1.2/scicam/bin/
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-03-15 12:33:05.000000 scicam-0.1.2/scicam/bin/__init__.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     5411 2022-07-17 21:09:55.000000 scicam-0.1.2/scicam/bin/__main__.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     4410 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/bin/grabmultiplecameras.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1321 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/bin/run.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1790 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/bin/test.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     3031 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/bin/test_queue.py
-drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-08-20 17:33:04.038201 scicam-0.1.2/scicam/class_utils/
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/class_utils/__init__.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      342 2022-03-15 12:53:38.000000 scicam-0.1.2/scicam/class_utils/time.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      274 2022-07-15 15:38:42.000000 scicam-0.1.2/scicam/constants.py
-drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-08-20 17:33:04.038201 scicam-0.1.2/scicam/core/
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       29 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/core/__init__.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     4183 2022-08-06 14:32:56.000000 scicam-0.1.2/scicam/core/manager.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     8266 2022-08-20 16:50:03.000000 scicam-0.1.2/scicam/core/monitor.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1267 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/decorators.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      166 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/exceptions.py
-drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-08-20 17:33:04.038201 scicam-0.1.2/scicam/io/
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/io/__init__.py
-drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-08-20 17:33:04.038201 scicam-0.1.2/scicam/io/cameras/
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      203 2022-04-25 15:07:09.000000 scicam-0.1.2/scicam/io/cameras/__init__.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     3040 2022-07-27 18:48:10.000000 scicam-0.1.2/scicam/io/cameras/__main__.py
-drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-08-20 17:33:04.038201 scicam-0.1.2/scicam/io/cameras/basler/
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       32 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/io/cameras/basler/__init__.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1309 2022-03-17 17:43:35.000000 scicam-0.1.2/scicam/io/cameras/basler/__main__.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     7351 2022-08-20 17:06:53.000000 scicam-0.1.2/scicam/io/cameras/basler/basler.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     3339 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/io/cameras/basler/compat.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1129 2022-07-27 18:47:30.000000 scicam-0.1.2/scicam/io/cameras/basler/parser.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     7618 2022-08-20 16:53:17.000000 scicam-0.1.2/scicam/io/cameras/core.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     3593 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/io/cameras/dlc.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     5588 2022-08-20 17:06:59.000000 scicam-0.1.2/scicam/io/cameras/flir.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     4324 2022-04-25 14:21:22.000000 scicam-0.1.2/scicam/io/cameras/opencv.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     5172 2022-08-20 14:58:48.000000 scicam-0.1.2/scicam/io/cameras/plugins.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-04-25 15:06:11.000000 scicam-0.1.2/scicam/io/cameras/setup.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1534 2022-08-20 17:03:19.000000 scicam-0.1.2/scicam/io/cameras/utils.py
-drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-08-20 17:33:04.038201 scicam-0.1.2/scicam/io/recorders/
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       48 2022-04-25 16:07:44.000000 scicam-0.1.2/scicam/io/recorders/__init__.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1193 2022-04-25 16:05:49.000000 scicam-0.1.2/scicam/io/recorders/__main__.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     5982 2022-08-06 14:31:51.000000 scicam-0.1.2/scicam/io/recorders/core.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)    11076 2022-08-06 14:30:58.000000 scicam-0.1.2/scicam/io/recorders/imgstore.py
-drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-08-20 17:33:04.038201 scicam-0.1.2/scicam/io/recorders/mixins/
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       32 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/io/recorders/mixins/__init__.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1454 2022-06-28 21:52:48.000000 scicam-0.1.2/scicam/io/recorders/mixins/ffmpeg.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1685 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/io/recorders/mixins/opencv.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1757 2022-07-15 15:37:35.000000 scicam-0.1.2/scicam/io/recorders/parser.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      679 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/io/recorders/record.py
-drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-08-20 17:33:04.038201 scicam-0.1.2/scicam/tests/
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       33 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/tests/__init__.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1468 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/tests/test_basler.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     6419 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/tests/test_recorder.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     2027 2022-04-16 19:26:55.000000 scicam-0.1.2/scicam/tests/test_synchrony.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      806 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/tests/utils.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1273 2022-07-15 15:38:09.000000 scicam-0.1.2/scicam/utils.py
-drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-08-20 17:33:04.038201 scicam-0.1.2/scicam/web_utils/
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       60 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/web_utils/__init__.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     6389 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/web_utils/client.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1086 2022-04-25 16:22:54.000000 scicam-0.1.2/scicam/web_utils/sensor.py
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     6380 2022-03-15 12:33:14.000000 scicam-0.1.2/scicam/web_utils/server.py
-drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-08-20 17:33:04.034201 scicam-0.1.2/scicam.egg-info/
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       73 2022-08-20 17:33:04.000000 scicam-0.1.2/scicam.egg-info/PKG-INFO
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1578 2022-08-20 17:33:04.000000 scicam-0.1.2/scicam.egg-info/SOURCES.txt
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)        1 2022-08-20 17:33:04.000000 scicam-0.1.2/scicam.egg-info/dependency_links.txt
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       87 2022-08-20 17:33:04.000000 scicam-0.1.2/scicam.egg-info/entry_points.txt
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      179 2022-08-20 17:33:04.000000 scicam-0.1.2/scicam.egg-info/requires.txt
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)        7 2022-08-20 17:33:04.000000 scicam-0.1.2/scicam.egg-info/top_level.txt
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       38 2022-08-20 17:33:04.038201 scicam-0.1.2/setup.cfg
--rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1647 2022-06-28 22:24:12.000000 scicam-0.1.2/setup.py
+drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2023-05-03 08:43:09.030933 scicam-0.1.3/
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       73 2023-05-03 08:43:09.030933 scicam-0.1.3/PKG-INFO
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       72 2022-11-10 10:25:05.000000 scicam-0.1.3/README.md
+drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2023-05-03 08:43:08.974933 scicam-0.1.3/scicam/
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       22 2023-05-03 08:41:28.000000 scicam-0.1.3/scicam/__init__.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       22 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/_version.py
+drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2023-05-03 08:43:08.978933 scicam-0.1.3/scicam/bin/
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/bin/__init__.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     6451 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/bin/__main__.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     4410 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/bin/grabmultiplecameras.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1321 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/bin/run.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1790 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/bin/test.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     3031 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/bin/test_queue.py
+drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2023-05-03 08:43:08.982933 scicam-0.1.3/scicam/class_utils/
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/class_utils/__init__.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      375 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/class_utils/time.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      787 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/configuration.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      280 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/constants.py
+drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2023-05-03 08:43:08.986933 scicam-0.1.3/scicam/core/
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       29 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/core/__init__.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     4702 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/core/manager.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     7737 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/core/monitor.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1267 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/decorators.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      166 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/exceptions.py
+drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2023-05-03 08:43:08.986933 scicam-0.1.3/scicam/io/
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/__init__.py
+drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2023-05-03 08:43:08.994933 scicam-0.1.3/scicam/io/cameras/
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      203 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/cameras/__init__.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     2417 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/io/cameras/__main__.py
+drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2023-05-03 08:43:09.002933 scicam-0.1.3/scicam/io/cameras/basler/
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       32 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/cameras/basler/__init__.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1307 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/io/cameras/basler/__main__.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)    10571 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/io/cameras/basler/basler.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     3339 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/cameras/basler/compat.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1127 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/io/cameras/basler/parser.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     7407 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/io/cameras/core.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     3593 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/cameras/dlc.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     7009 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/io/cameras/flir.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     4398 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/cameras/opencv.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     5922 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/io/cameras/plugins.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)        0 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/cameras/setup.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     2022 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/cameras/utils.py
+drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2023-05-03 08:43:09.010933 scicam-0.1.3/scicam/io/recorders/
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       48 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/recorders/__init__.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1193 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/recorders/__main__.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     5982 2023-01-18 17:14:30.000000 scicam-0.1.3/scicam/io/recorders/core.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)    11184 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/io/recorders/imgstore.py
+drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2023-05-03 08:43:09.010933 scicam-0.1.3/scicam/io/recorders/mixins/
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       32 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/recorders/mixins/__init__.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1454 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/recorders/mixins/ffmpeg.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1685 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/recorders/mixins/opencv.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1757 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/recorders/parser.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      679 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/io/recorders/record.py
+drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2023-05-03 08:43:09.018933 scicam-0.1.3/scicam/tests/
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       33 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/tests/__init__.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1462 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/tests/test_basler.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     6419 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/tests/test_recorder.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     2027 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/tests/test_synchrony.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      806 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/tests/utils.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1272 2023-05-03 08:41:00.000000 scicam-0.1.3/scicam/utils.py
+drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2023-05-03 08:43:09.030933 scicam-0.1.3/scicam/web_utils/
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       60 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/web_utils/__init__.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     6389 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/web_utils/client.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1086 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/web_utils/sensor.py
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     6380 2022-09-14 14:21:00.000000 scicam-0.1.3/scicam/web_utils/server.py
+drwxrwxr-x   0 vibflysleep  (1000) vibflysleep  (1000)        0 2023-05-03 08:43:08.978933 scicam-0.1.3/scicam.egg-info/
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       73 2023-05-03 08:43:08.000000 scicam-0.1.3/scicam.egg-info/PKG-INFO
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1602 2023-05-03 08:43:08.000000 scicam-0.1.3/scicam.egg-info/SOURCES.txt
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)        1 2023-05-03 08:43:08.000000 scicam-0.1.3/scicam.egg-info/dependency_links.txt
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       87 2023-05-03 08:43:08.000000 scicam-0.1.3/scicam.egg-info/entry_points.txt
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)      179 2023-05-03 08:43:08.000000 scicam-0.1.3/scicam.egg-info/requires.txt
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)        7 2023-05-03 08:43:08.000000 scicam-0.1.3/scicam.egg-info/top_level.txt
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)       38 2023-05-03 08:43:09.030933 scicam-0.1.3/setup.cfg
+-rw-rw-r--   0 vibflysleep  (1000) vibflysleep  (1000)     1647 2022-11-10 10:25:06.000000 scicam-0.1.3/setup.py
```

### Comparing `scicam-0.1.2/scicam/bin/__main__.py` & `scicam-0.1.3/scicam/bin/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,133 +16,157 @@
 from scicam.io.cameras.basler.parser import get_parser as basler_parser
 from scicam.io.cameras import CAMERAS
 from scicam.io.recorders.parser import get_parser as recorder_parser
 from scicam.web_utils.sensor import setup as setup_sensor
 from scicam.core.manager import Manager
 from scicam.exceptions import ServiceExit
 from scicam.utils import load_config, service_shutdown
+from scicam.configuration import load_setup_cameras
 
 logger = logging.getLogger(__name__)
 
 config = load_config()
+ROOT_OUTPUT=config["videos"]["folder"]
+LOGFOLDER=config["logs"]["folder"]
 
 # this start time will be shared by all cameras running in parallel and will give name to the experiment
-start_time = time.time()
-time_iso_8601=datetime.fromtimestamp(start_time).strftime("%Y-%m-%d_%H-%M-%S")
-root_output = os.path.join(config["videos"]["folder"], time_iso_8601)
 
 
 with open(LOGGING_CONFIG, 'r') as filehandle:
     logging_config = yaml.load(filehandle, yaml.SafeLoader)
     logging.config.dictConfig(logging_config)
 
-LOGFILE = os.path.join(config["logs"]["folder"], f"{time_iso_8601}.log")
-file_handler = logging.FileHandler(LOGFILE, mode='w')
 
-logger = logging.getLogger(__name__)
-logger.addHandler(file_handler)
 
 def get_parser(ap=None):
 
     if ap is None:
         ap = argparse.ArgumentParser(conflict_handler="resolve")
 
     ap.add_argument(
-        "--cameras",
-        nargs="+",
+        "--start-time",
         required=True,
-        choices=CAMERAS,
-        default=None,
-    )
-    ap.add_argument(
-        "--flir-exposure",
-        dest="flir_exposure",
         type=int,
-        default=9900,
-        help="Exposure time in microseconds of the Flir camera",
-    )
-    ap.add_argument(
-        "--basler-exposure",
-        dest="basler_exposure",
-        type=int,
-        default=25000,
-        help="Exposure time in microseconds of the Basler camera",
-    )
+        help='Timestamp in seconds as produced by date +"%s" in Linux or time.time() in Python'
+        )
+
     ap.add_argument(
-        "--flir-framerate",
-        type=int,
-        default=100,
-        help="Frames Per Second of the Flir camera",
+        "--supplier",
+        type=str,
+        required=False,
     )
     ap.add_argument(
-        "--basler-framerate",
-        type=int,
-        default=30,
-        help="Frames Per Second of the Basler camera",
+        "--setup",
+        type=str,
+        required=False,
     )
+    ap.add_argument("--X", type=int, required=True)
+
     ap.add_argument(
         "--sensor",
         type=int,
         default=9000,
         help="Port of environmental sensor",
     )
     ap.add_argument(
-        "--select-rois",
+        "--select-roi",
         default=False,
         action="store_true",
-        dest="select_rois",
+        dest="select_roi",
         help="""
         Whether a region of interest (ROI)
         of the input should be cropped or not.
         In that case, a pop up will show for the user to select it
         """,
     )
-    ap.add_argument(
-        "--rois",
-        default=None,
-        type=str
-    )
+
     return ap
 
 
 def get_queue(process, queues):
     if process in queues and not queues[process].empty():
         timestamp, frame = queues[process].get()
         return timestamp, frame
     else:
         return (None, np.uint8())
 
 
 def setup_and_run(args):
     sensor = setup_sensor(args.sensor)
     managers = {}
-    
-    if args.select_rois:
+
+    if args.select_roi:
         roi_helper = EasyROI(verbose=True)
     else:
         roi_helper = None
 
 
     monitors=[]
 
-    for i, camera_name in enumerate(args.cameras):
-
-        if camera_name == "FlirCamera":
-            output = os.path.join(root_output, "lowres")
-        else:
-            output = root_output
-
-        manager = Manager(
-            idx=i,
-            chunk_duration=args.chunk_duration,
-            camera_name=camera_name, output=output, format=args.format,
-            sensor=sensor,  select_rois=args.select_rois, roi_helper=roi_helper, rois=args.rois
-        )
-        managers[camera_name] = manager
-        monitors.append(manager.init(start_time=start_time))
+    start_time = args.start_time
+    time_iso_8601=datetime.fromtimestamp(start_time).strftime("%Y-%m-%d_%H-%M-%S")
+    LOGFILE = os.path.join(config["logs"]["folder"], f"{time_iso_8601}.log")
+    file_handler = logging.FileHandler(LOGFILE, mode='w')
+
+    logger = logging.getLogger(__name__)
+    logger.addHandler(file_handler)
+
+
+    suppliers = load_setup_cameras()
+
+
+    if args.setup is not None:
+        new_suppliers={}
+        for supplier in suppliers:
+            new_suppliers[supplier] ={}
+
+        for supplier in suppliers:
+            for camera in suppliers[supplier]:
+                if suppliers[supplier][camera]["setup"] == args.setup:
+                    new_suppliers[supplier][camera] = suppliers[supplier][camera]
+
+        suppliers = new_suppliers
+
+    if args.supplier is not None:
+        suppliers = {args.supplier: suppliers[args.supplier]}
+
+
+    for i, supplier in enumerate(suppliers):
+        cameras = suppliers[supplier]
+        for camera_idx in cameras:
+            role = cameras[camera_idx]["role"]
+            setup_name = cameras[camera_idx]["setup"]
+            camera_name = supplier
+            root_output = os.path.join(ROOT_OUTPUT, setup_name, f"{args.X}X", time_iso_8601)
+            os.makedirs(root_output, exist_ok=False)
+            LOGFILE = os.path.join(LOGFOLDER, setup_name, f"{time_iso_8601}.log")
+            os.makedirs(os.path.dirname(LOGFILE), exist_ok=True)
+            file_handler = logging.FileHandler(LOGFILE, mode='w')
+            logger.addHandler(file_handler)
+
+
+            if role == "highspeed":
+                output = os.path.join(root_output, role)
+            else:
+                output = root_output
+
+            # if supplier == "FlirCamera":
+            #     encoder_kwargs = {"gop_duration": 60}
+            # else:
+            #     encoder_kwargs = {}
+
+            manager = Manager(
+                idx=i,
+                chunk_duration=args.chunk_duration,
+                setup_name=setup_name, supplier=camera_name, camera_idx=camera_idx, output=output, format=args.format,
+                sensor=sensor,  select_roi=args.select_roi, roi_helper=roi_helper
+            )
+            managers[camera_name] = manager
+            # kwargs = manager.init(start_time)
+            monitors.append(manager.init(start_time))#, encoder_kwargs=encoder_kwargs))
 
     for monitor in monitors:
         monitor.start()
 
     for monitor in monitors:
         monitor.join()
```

### Comparing `scicam-0.1.2/scicam/bin/grabmultiplecameras.py` & `scicam-0.1.3/scicam/bin/grabmultiplecameras.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/bin/run.py` & `scicam-0.1.3/scicam/bin/run.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/bin/test.py` & `scicam-0.1.3/scicam/bin/test.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/bin/test_queue.py` & `scicam-0.1.3/scicam/bin/test_queue.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/core/manager.py` & `scicam-0.1.3/scicam/core/manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,134 +4,154 @@
 import traceback
 import queue
 
 import pandas as pd
 import yaml
 
 from scicam.io.cameras import CAMERAS
-from scicam.constants import CAMERA_INDEX
-from scicam.core.monitor import run as run_monitor
 from scicam.core.monitor import Monitor
+from scicam.configuration import load_setup_cameras
 
 logger = logging.getLogger(__name__)
 
-try:
-    with open(CAMERA_INDEX, "r") as filehandle:
-        camera_index = yaml.load(filehandle, yaml.SafeLoader)
-except Exception as error:
-    logger.warning(error)
-    
+
 class Manager:
 
-    def __init__(self, idx, camera_name, format, output, sensor=None, rois=None, roi_helper=None, select_rois=False, resolution_decrease=1.0, chunk_duration=300):
 
+    def __init__(
+        self, idx, setup_name, supplier, camera_idx, format, output, sensor=None, roi_helper=None, select_roi=False,
+        resolution_decrease=1.0, chunk_duration=300
+    ):
+        
+        self.setup_name = setup_name
+        self.supplier = supplier
         self.idx = idx
-        self.camera_name = camera_name
+        self.camera_idx = camera_idx
         self.sensor = sensor
         self.roi_helper = roi_helper
-        self.select_rois = select_rois
-        self.rois=rois
+        self.select_roi = select_roi
         self.root_output = output
         self.chunk_duration=chunk_duration
         self.format = format
         self.process = None
         self.stop_queue = None
         self.resolution_decrease=resolution_decrease
 
 
     @staticmethod
     def separate_process(
-        camera_name,
+        setup_name,
+        supplier,
         output,
         format,
         sensor=None,
         stop_queue=None,
         process_id=0,
-        rois=None,
+        roi=None,
         camera_idx=0,
         start_time=None,
         chunk_duration=300,
+        metadata={},
     ):
         logger.info("multiprocess.Process - scicam.bin.__main__.separate _process")
 
-        logger.debug(f"Monitor running {camera_name} chunk_duration: {chunk_duration}")
+        logger.debug(f"Monitor running {setup_name} - {supplier} chunk_duration: {chunk_duration}")
         monitor = Monitor(
-            camera_name=camera_name,
-            camera_idx=camera_idx,
+            setup_name=setup_name,
+            supplier=supplier,
             path=output,
             format=format,
             start_time=start_time,
             stop_queue=stop_queue,
             sensor=sensor,
-            rois=rois,
-            select_rois=False,
+            roi=roi,
+            select_roi=False,
+            camera_idx=camera_idx,
             chunk_duration=chunk_duration,
+            metadata=metadata,
         )
 
 
         logger.info(f"Monitor start time: {start_time}")
 
         monitor.process_id = process_id
         return monitor
 
 
     def init(
         self, start_time,
     ):
-        camera_idx = camera_index[self.camera_name]
+        config = load_setup_cameras(self.setup_name)[self.supplier]
+
+        duration = config[self.camera_idx].get("duration", None)
+        framerate = config[self.camera_idx]["framerate"]
+        exposure = config[self.camera_idx]["exposure"]
+        brightness = config[self.camera_idx]["brightness"]
+        pixels_per_cm = config[self.camera_idx]["pixels_per_cm"]
+
+        print(self.supplier, end=":")
+        print(f"    Framerate {framerate}")
+        print(f"    Exposure {exposure}")
+        print(f"    Brightness {brightness}")
 
-        if self.select_rois:
+        if self.select_roi:
 
-            camera = CAMERAS[self.camera_name](
+            camera = CAMERAS[self.supplier](
                 start_time=start_time,
                 roi_helper=self.roi_helper,
                 resolution_decrease=self.resolution_decrease,
-                idx=camera_idx,
+                exposure=exposure,
+                brightness=brightness,
+                camera_idx=self.camera_idx,
+                apply_roi=False,
+                # pixels_per_cm=pixels_per_cm,
             )
 
-            logger.info(f"Selecting rois for {camera}")
-            if self.select_rois:
-                rois = camera.select_ROIs()
+            logger.info(f"Selecting ROI for {camera}")
+            if self.select_roi:
+                roi = camera.select_ROI()
             # save the roi and somehow give it to the next instance
             camera.close()
 
-        elif self.rois is not None:
-            # TODO Make a function out of this
-            roi_data = pd.read_csv(self.rois)
-            assert all([col in roi_data.columns for col in ["x", "y", "w", "h", "camera_name"]])
-            roi_data = roi_data.loc[roi_data["camera_name"] == self.camera_name]
-            rois = [(row.x, row.y, row.w, row.h) for i, row in roi_data.iterrows()]
-
         else:
-            camera = CAMERAS[self.camera_name](
+            camera = CAMERAS[self.supplier](
                             start_time=start_time,
                             resolution_decrease=self.resolution_decrease,
-                            idx=camera_idx,
+                            camera_idx=self.camera_idx,
             )
             width=max(camera.width, camera.height)
             height=width
             camera.close()
-            rois = [(0, 0, width, height)]
+            roi = (0, 0, width, height)
             
         self.stop_queue = queue.Queue(maxsize=1)       
         
         kwargs = {
+            "setup_name": self.setup_name,
+            "supplier": self.supplier,
+            "output": self.root_output,
+            "format": self.format,
             "sensor": self.sensor,
             "stop_queue": self.stop_queue,
             "process_id": self.idx,
-            "rois": rois,
-            "camera_idx": camera_idx,
+            "roi": roi,
+            # "hash": camera.__hash__(),
             "start_time": start_time,
-            "chunk_duration": self.chunk_duration
+            "chunk_duration": self.chunk_duration,
+            # "min_bitrate": self._min_bitrate,
+            # "max_bitrate": self._max_bitrate,
+            "camera_idx": self.camera_idx,
+            "metadata": {"pixels_per_cm": pixels_per_cm}
         }
 
 
         monitor=self.separate_process(
-            camera_name=self.camera_name, output=self.root_output, format=self.format, **kwargs
+            **kwargs,
         )
+
         return monitor
 
 
     def start(self):
         return self.process.start()
 
     def join(self, *args, **kwargs):
```

### Comparing `scicam-0.1.2/scicam/core/monitor.py` & `scicam-0.1.3/scicam/core/monitor.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,127 +12,129 @@
 import pandas as pd
 import arrayqueues
 from scicam.io.recorders import ImgStoreRecorder
 from scicam.web_utils.sensor import setup as setup_sensor
 from scicam.exceptions import ServiceExit
 from scicam.io.cameras import CAMERAS
 from scicam.utils import load_config
+import psutil
+from scicam.configuration import load_setup_cameras
 
 class Monitor(threading.Thread):
     _RecorderClass = ImgStoreRecorder
 
     def __init__(
         self,
-        camera_name,
-        camera_idx,
+        setup_name,
+        supplier,
         path,
         format,
         start_time,
         *args,
         stop_queue=None,
         sensor=None,
-        rois=None,
-        select_rois=False,
+        roi=None,
+        select_roi=False,
         chunk_duration=300,
+        camera_idx=0,
+        metadata={},
     ):
 
-        self._camera_name = camera_name
-        self._camera_idx = camera_idx
+        self.supplier = supplier
         self._root_path = path
-        self._select_rois = select_rois
+        self._select_roi = select_roi
+        self._camera_idx = camera_idx
         os.makedirs(self._root_path, exist_ok=True)
         logger.debug(f"{self} chunk_duration: {chunk_duration}")
 
+        self._process = psutil.Process(os.getpid())
+
         self.setup_camera(
-            camera_name=camera_name,
-            idx=camera_idx,
-            rois=rois,
+            setup_name=setup_name,
+            camera_idx=camera_idx,
+            supplier=supplier,
+            roi=roi,
             start_time=start_time,
         )
 
         self._stop_queue = stop_queue
         self._setup_queues()
         self._stop_event = multiprocessing.Event()
 
-        self._recorders = []
-
-        for i in range(len(self.camera.rois)):
-            
-            metadata = {
-                "camera-framerate": self.camera.framerate,
-                "camera-exposure": self.camera.exposure,
-                "camera-model": self.camera.model_name,
-            }
-            
-            recorder = self._RecorderClass(
-                framerate=float(int(self.camera.framerate)),
-                duration=self.camera.duration,
-                resolution = self.camera.rois[i][2:4],
-                path=self._root_path,
-                data_queue = self._data_queues[i],
-                stop_queue = self._stop_queues[i],
-                sensor=sensor,
-                idx=i,
-                roi=self.camera.rois[i],
-                metadata=metadata,
-                format=format,
-                chunk_duration=chunk_duration,
-            )
-            self._recorders.append(recorder)
+        self._recorder = None
 
+        metadata.update({
+            "camera-framerate": self.camera.framerate,
+            "camera-exposure": self.camera.exposure,
+            "camera-model": self.camera.model_name,
+        })
+
+        self._recorder= self._RecorderClass(
+            framerate=float(int(self.camera.framerate)),
+            duration=self.camera.duration,
+            resolution = self.camera.roi[2:4],
+            path=self._root_path,
+            data_queue = self._data_queue,
+            stop_queue = self._stop_queue,
+            sensor=sensor,
+            idx=0,
+            roi=self.camera.roi,
+            format=format,
+            chunk_duration=chunk_duration,
+            metadata=metadata,
+        )
         super(Monitor, self).__init__()
 
 
     def __str__(self):
-        return f"Monitor driving camera {self._camera_name}"
+        return f"Monitor driving camera {self.supplier} - {self._camera_idx}"
 
 
     def _setup_queues(self):
 
-        self._data_queues = [
-            arrayqueues.TimestampedArrayQueue(100) for _ in self.camera.rois
-        ]
-        
-        self._stop_queues = [
-            multiprocessing.Queue(maxsize=1) for _ in self.camera.rois
-        ]
-
-    def setup_camera(self, camera_name, **kwargs):
-        config = load_config()
-
-        duration = config["cameras"][camera_name]["duration"]
-        framerate = config["cameras"][camera_name]["framerate"]
-        exposure = config["cameras"][camera_name]["exposure"]
+        self._data_queue = arrayqueues.TimestampedArrayQueue(5000) # 5gb buffer
+        self._stop_queue =multiprocessing.Queue(maxsize=1)
+
+    def setup_camera(self, setup_name, supplier, camera_idx, **kwargs):
+        config = load_setup_cameras(setup_name)[supplier]
 
-        print(camera_name, end=":")
+        # duration = config[camera_name]["duration"]
+        framerate = config[camera_idx]["framerate"]
+        exposure = config[camera_idx]["exposure"]
+        brightness = config[camera_idx]["brightness"]
+
+        print(supplier, end=":")
+        print(f"    Camera idx {camera_idx}")
         print(f"    Framerate {framerate}")
         print(f"    Exposure {exposure}")
-        
+        print(f"    Brightness {brightness}")
+
 
-        self.camera = CAMERAS[camera_name](
+        self.camera = CAMERAS[supplier](
             document_path=self._root_path,
             framerate=framerate,
             exposure=exposure,
-            duration=duration,
+            brightness=brightness,
+            duration=None,
+            camera_idx=camera_idx,
             **kwargs
         )
 
-        if self._select_rois:
-            self.camera.select_ROIs()
+        if self._select_roi:
+            self.camera.select_ROI()
 
     def open(self):
-        for idx in range(len(self.camera.rois)):
 
-            recorder_path = f"{self._root_path.rstrip('/')}_ROI_{idx}"
-            self._recorders[idx].open(
-                path=recorder_path
-            )
-            logger.info(
-                f"{self._recorders[idx]} for {self.camera} has recorder_path = {recorder_path}"
-            )
+        recorder_path = f"{self._root_path.rstrip('/')}_ROI_0"
+        self._recorder.open(
+            path=recorder_path
+        )
+        logger.info(
+            f"{self._recorder} for {self.camera} has recorder_path = {recorder_path}"
+        )
 
     def put(self, recorder, data_queue, data):
 
         timestamp, i, arr, info = data
         try:
             data_queue.put(arr, timestamp=(timestamp, i, info))
             recorder._n_saved_frames += 1
@@ -148,91 +150,81 @@
                 )
 
 
     def run(self):
 
         logger.info("Monitor starting")
         self._start_time = self.camera.start_time
-        for i, recorder in enumerate(self._recorders):
-            recorder.start_time = self._start_time
-            recorder.start()
-            logger.debug("Recorder starting")
-            roi = self.camera._rois[i]
-            roi_df = pd.DataFrame({
-                "x": [roi[0]], "y": [roi[1]],
-                "w": [roi[2]], "h": [roi[3]],
-                "camera_name": [self.camera.__class__.__name__.replace("Camera", "")]
-            })
 
-            if self._select_rois:
-                roi_df.to_csv("rois.csv", mode='a', index=False, header=False)
+        self._recorder.start_time = self._start_time
+        self._recorder.start()
+        logger.debug("Recorder starting")
 
         last_timestamp = 0
+        input("Continue?")
+
         for frame_idx, (timestamp, frame, info) in enumerate(self.camera):
             # proc_time = timestamp - last_timestamp
             # logger.debug(
             #     f"Frame processing time: {proc_time}"
             #     f"FPS approx {round(1000/proc_time, 2)}"
             # )
+            if frame_idx % (int(self.camera.framerate) * 60) == 0:
+                print(self.camera, self._process.memory_info().rss / (1024)**2)
 
             if self._stop_event.is_set():
                 logger.info("Monitor exiting")
 
-                for i in range(len(self._recorders)):
-                    logger.debug(
-                        f"Recorder {i} output queue has {self._recorders[i].buffer_usage} frames"
-                    )
+                logger.debug(
+                    f"Recorder 0 output queue has {self._recorder.buffer_usage} frames"
+                )
                 break
 
             if self._stop_queue is not None:
                 try:
                     msg = self._stop_queue.get(False)
                 except queue.Empty:
                     msg = None
                 if msg == "STOP":
                     logger.debug(f"Setting {self} stop event")
                     self._stop_event.set()
 
-            for i in range(len(self.camera.rois)):
-                recorder = self._recorders[i]
-                self.put(
-                    recorder=recorder,
-                    data_queue=self._data_queues[i],
-                    data=(timestamp, frame_idx, frame[i], info)
-                )
-                # _, write_msec = recorder.write(timestamp, frame_idx, frame[i])
-                # write_logger.debug(f"Recorder took {write_msec} ms to write")
+            self.put(
+                recorder=self._recorder,
+                data_queue=self._data_queue,
+                data=(timestamp, frame_idx, frame, info)
+            )
+            # _, write_msec = recorder.write(timestamp, frame_idx, frame[i])
+            # write_logger.debug(f"Recorder took {write_msec} ms to write")
             last_timestamp = timestamp
 
         logger.debug("Joining recorders")
-        for recorder in self._recorders:
-            if recorder.is_alive():
-                while not recorder.all_queues_have_been_emptied:
-                    time.sleep(1)
-                    logger.debug("Waiting for", recorder)
-
-                logger.debug("Report one last time ", recorder)
-                recorder.check_data_queue()
-                logger.debug("Close tqdm for ", recorder)
-                logger.debug("Joining", recorder)
-                # recorder._data_queue.put(None)
-            recorder.join()
-            logger.debug("JOOOOIIIIIINEEEEDD")
+        recorder = self._recorder
+        if recorder.is_alive():
+            while not recorder.all_queues_have_been_emptied:
+                time.sleep(1)
+                logger.debug("Waiting for", recorder)
+
+            logger.debug("Report one last time ", recorder)
+            recorder.check_data_queue()
+            logger.debug("Close tqdm for ", recorder)
+            logger.debug("Joining", recorder)
+            # recorder._data_queue.put(None)
+        recorder.join()
+        logger.debug("JOOOOIIIIIINEEEEDD")
 
         logger.debug("Joined all recorders")
 
     def close(self):
 
         # this makes the run method exit
         # because it checks if the stop_event is set
         self._stop_event.set()
         logger.info("Monitor closing")
-
-        for recorder in self._recorders:
-            recorder.close()
+        self._recorder.close()
 
 
 def run(monitor):
 
     monitor.open()
     try:
         monitor.start()
```

### Comparing `scicam-0.1.2/scicam/decorators.py` & `scicam-0.1.3/scicam/decorators.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/io/cameras/__main__.py` & `scicam-0.1.3/scicam/io/cameras/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -68,39 +68,14 @@
         camera = OpenCVCamera(**camera_kwargs)
     else:
         raise Exception("Invalid camera name")
 
     return camera
 
 
-def run(camera, queue=None, preview=False):
-    try:
-        for timestamp, frame in camera:
-            if camera.rois:
-                frame = frame[0]
-
-            print(
-                "Flir camera reads: ",
-                timestamp,
-                frame.shape,
-                frame.dtype,
-                camera.computed_framerate,
-            )
-            if queue is not None:
-                queue.put((timestamp, frame))
-
-            if preview:
-                cv2.imshow("Flir", frame)
-                if cv2.waitKey(1) == ord("q"):
-                    break
-
-    except KeyboardInterrupt:
-        return
-
-
 def setup_and_run(args, **kwargs):
     camera = setup(camera_name=args.cameras[0], args=args, **kwargs)
     maxframes = getattr(args, "maxframes", None)
     camera.open(maxframes=maxframes)
     run(camera, preview=args.preview)
```

### Comparing `scicam-0.1.2/scicam/io/cameras/basler/__main__.py` & `scicam-0.1.3/scicam/io/cameras/basler/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from .parser import get_parser
 from scicam.io.cameras.setup import setup
 
 def run(camera, queue=None, preview=False):
 
     try:
-        for timestamp, all_rois in camera:
+        for timestamp, all_roi in camera:
 
-            for frame in all_rois:
+            for frame in all_roi:
                 print(
                     "Basler camera reads: ",
                     timestamp,
                     frame.shape,
                     frame.dtype,
                     camera.computed_framerate,
                 )
```

### Comparing `scicam-0.1.2/scicam/io/cameras/basler/basler.py` & `scicam-0.1.3/scicam/io/cameras/flir.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,241 +1,243 @@
-# Standard library
-import logging
-import warnings
-import time
+
 import traceback
+import time
 import os.path
+import logging
 import random
-
-# Optional modules
-from pypylon import pylon
-
-# Local library
+import numpy as np
+import simple_pyspin
 from scicam.io.cameras.core import CV2Compatible
-from scicam.io.cameras.utils import ensure_img, validate_img
 from scicam.decorators import timeit
+from scicam.io.cameras.utils import validate_img, ensure_img 
+import PySpin
+COLOR_PROCESSING_ALGORITHM="NEAREST_NEIGHBOR"
+
+logger = logging.getLogger(__name__)
+
+from scicam.configuration import load_setup_cameras 
 
-logger = logging.getLogger("scicam.io.camera")
-LEVELS = {"DEBUG": 0, "INFO": 10, "WARNING": 20, "ERROR": 30}
+class FlirCamera(CV2Compatible):
+    
+    supplier="FlirCamera"
+    AcquisitionFrameRateMax = 150
+    HEIGHT_STEPS=2
+    WIDTH_STEPS=16
 
-class BaslerCamera(CV2Compatible):
 
     """
-    Drive a Basler camera using pypylon.
+    Drive a Flir camera using simple_pyspin
     """
 
     def __init__(self, *args, **kwargs):
-        super(BaslerCamera, self).__init__(*args, **kwargs)
+        self._isgrabbing = False
+        self._isopen = False
+        super(FlirCamera, self).__init__(*args, **kwargs)
+
 
     @property
     def width(self):
-        return self.camera.Width.GetValue()
+        return self.camera.Width
 
     @property
     def height(self):
-        return self.camera.Height.GetValue()
+        return self.camera.Height
 
     @property
     def model_name(self):
-        return self.camera.GetDeviceInfo().GetModelName()
-    
+        return self.camera.DeviceModelName
+
     @property
     def serial_number(self):
-        return self.camera.GetDeviceInfo().GetSerialNumber()
-
+        return self.camera.DeviceSerialNumber
 
     @property
     def friendly_name(self):
-        return self.camera.GetDeviceInfo().GetFriendlyName()
+        return f"{self.camera.DeviceModelName} ({self.camera.DeviceSerialNumber})"
 
     @property
     def temperature(self):
-        return round(self.camera.DeviceTemperature.GetValue(), 2)
+        return self.camera.DeviceTemperature
 
     @property
     def temperature_unit(self):
-        return self.camera.DeviceTemperature.GetUnit()
-
+        raise "C"
 
     @property
     def framerate(self):
-        return float(self.camera.AcquisitionFrameRate.GetValue())
+        return float(self.camera.AcquisitionFrameRate)
 
     @framerate.setter
     def framerate(self, framerate):
         logging.warning("Setting framerate is not recommended in scicam")
-        self.camera.AcquisitionFrameRate.SetValue(framerate)
+        self.camera.AcquisitionFrameRate = framerate
         self._target_framerate = framerate
 
     @property
     def exposure(self):
-        return float(self.camera.ExposureTime.GetValue())
+        return float(self.camera.ExposureTime)
 
     @exposure.setter
     def exposure(self, exposure):
         logging.warning("Setting exposure time is not recommended in scicam")
-        self.camera.ExposureTime.SetValue(exposure)
+        self.camera.ExposureTime = exposure
         self._target_exposure = exposure
 
     def is_open(self):
         """
         Return True if camera is opened
         """
-        return self.camera.IsOpen()
+        return self._isopen
+
+    def IsGrabbing(self):
+        return self._isgrabbing
+
+    def _compute_final_framerate_for_camera(self):
+        """
+        Add to the target framerate a little bit more,
+        so the camera makes a bit more effort and actually hits the target
+        """
+        framerate = self._target_framerate + self._framerate_offset
+        max_framerate = self.AcquisitionFrameRateMax
+        if framerate >= max_framerate:
+            logger.warning(
+                f"Passed framerate is greater or equal than max ({max_framerate})"
+            )
+            final_framerate = max_framerate
+        else:
+            final_framerate = framerate
+        return final_framerate
+
+
+    def _init_camera(self, idx):
+        try:
+            self.camera = simple_pyspin.Camera(index=idx)
+            self.camera.__enter__()
+        
+        except Exception as error:
+            logger.error(
+                "The Flir camera cannot be opened."\
+                " Please check error trace for more info"
+            )
+            logger.error(traceback.print_exc())
+            raise error         
+            
 
     @timeit 
     def _next_image_default_timeit(self):
-        if self.camera.IsGrabbing():
+        wait=True
+        if self.IsGrabbing():
             with self._acquisition_lock:
-                while True:
-                    try:
-                        grab = self.camera.RetrieveResult(
-                            self._timeout, pylon.TimeoutHandling_ThrowException
-                        )
-                        break
-                    except:
-                        logger.warning("Calling _next_image_default_timeit again")
-                        pass
-
-                if grab.GrabSucceeded():
-                    img = grab.GetArray()
-                    grab.Release()
+                # img = self.camera.get_array()
+                
+                # print("get next image")
+                grab = self.camera.cam.GetNextImage(PySpin.EVENT_TIMEOUT_INFINITE if wait else PySpin.EVENT_TIMEOUT_NONE)
+                # print("done get next image")
+                # print("convert")
+                img = grab.Convert(PySpin.ChunkPixelFormat_Mono8, getattr(PySpin, COLOR_PROCESSING_ALGORITHM)).GetNDArray()
+                # print("done convert")
+                
+                if isinstance(img, np.ndarray):
                     code = 0
                 else:
-                    img = None
                     code = 1
 
-            # p = random.random()
-            # if p > 0.999:
-            #     img = None
-
-            if not validate_img(img):
-                code, img=ensure_img(self)
+            code=validate_img(img)
+            if code != 0:
+                return ensure_img(self)
 
             return code, img
-        else:
-            return 1, None
+
 
     def _next_image_default(self):
         (code, img), msec = self._next_image_default_timeit()
         logger.debug(f"Read image from {self.model_name} in {msec} ms")
         status = 1 - code
         return status, img
 
-    def _init_camera(self):
-        
-        # NOTE
-        # When selecting a particular camera
-        # you may want to use self.idx
-
-        try:
-            tl_factory = pylon.TlFactory.GetInstance()
-            camera_device = tl_factory.CreateFirstDevice()
-            self.camera = pylon.InstantCamera(
-                camera_device
-            )
-        except Exception as error:
-            logger.error(
-                "The Basler camera cannot be opened."\
-                " Please check error trace for more info"
-            )
-            logger.error(traceback.print_exc())
-            raise error
-
-    def _init_multi_camera(self, idx=0):
-        
-        # NOTE
-        # When selecting a particular camera
-        # you may want to use self.idx
-
-        try:
-            tl_factory = pylon.TlFactory.GetInstance()
-            devices = tl_factory.EnumerateDevices()
-            self.camera = pylon.InstantCamera(tl_factory.CreateDevice(devices[idx]))
-            self._idx = idx
-            return 0
+    def save_features(self, path):
+        logger.warning(f"{self.__class__}.save_features is not implemented. Ignoring")
 
-        except Exception as error:
-            logger.error(
-                "The Basler camera cannot be opened."\
-                " Please check error trace for more info"
-            )
-            logger.error(traceback.print_exc())
-            raise error
+    @property
+    def WidthMax(self):
+        return self.camera.cam.WidthMax.GetValue()
     
+    @property
+    def HeightMax(self):
+        return self.camera.cam.HeightMax.GetValue()
 
-    def _compute_final_framerate_for_camera(self):
-        """
-        Add to the target framerate a little bit more,
-        so the camera makes a bit more effort and actually hits the target
-        """
-        framerate = self._target_framerate + self._framerate_offset
-        max_framerate = self.camera.AcquisitionFrameRate.GetMax()
-        if framerate >= max_framerate:
-            logger.warning(
-                f"Passed framerate is greater or equal than max ({max_framerate})"
-            )
-            final_framerate = max_framerate
-        else:
-            final_framerate = framerate
-        return final_framerate
 
-    def save_features(self, pfs_file):
-        assert self.is_open()
-        return pylon.FeaturePersistence.Save(pfs_file, self.camera.GetNodeMap())
 
 
-    def open(self, maxframes=None, buffersize=5, idx=0):
+    def open(self, maxframes=None, apply_roi=True, buffersize=5, idx=0):
         """
         Detect a Basler camera using pylon
         Assign it to the camera slot and try to open it
         Try to fetch a frame
         """
-        self._init_multi_camera(idx=idx)
-        self.camera.Open()
+
+        self.maxframes = maxframes
+        self._init_camera(idx)
+        self._idx=idx
         print("Using device ", self.model_name)
-        self.camera.AcquisitionFrameRateEnable.SetValue(True)
+        config=load_setup_cameras()["FlirCamera"]
+
+        if apply_roi:
+            for key in ["Width", "Height", "OffsetX", "OffsetY"]:
+                value = config[idx].get(key, None)
+                if value is not None:
+                    getattr(self.camera.cam, key).SetValue(value)
+                    print(f"Setting {key} = {value}")
+
+        else:
+            self.camera.cam.OffsetX.SetValue(0)
+            self.camera.cam.OffsetY.SetValue(0)
+            self.camera.cam.Width.SetValue(self.WidthMax)
+            self.camera.cam.Height.SetValue(self.HeightMax)
+
+        self.camera.AcquisitionFrameRateAuto = "Off"
+        self.camera.AcquisitionFrameRateEnabled = True
+        self.camera.AcquisitionFrameRate = self._compute_final_framerate_for_camera()
+
+        self.camera.ExposureAuto = "Off"
+        self.camera.ExposureTime = self._target_exposure
+        self.camera.BlackLevel = self._target_brightness
+
+
+
+            
+        # if self._target_width is None:
+        #     self._target_width = self.camera.SensorWidth
+
+
+        # if self._target_height is None:
+        #     self._target_height = self.camera.SensorHeight
+
+        # self.camera.Width = self._target_width
+        # self.camera.Height = self._target_height
+
+        self.camera.ReverseX = False
+        self.camera.ReverseY = False
 
-        final_framerate=self._compute_final_framerate_for_camera()
-        logger.debug(f"{self} setting framerate to {final_framerate}")
-        self.camera.AcquisitionFrameRate.SetValue(
-            final_framerate
-        )
-        logger.debug(f"{self} setting exposure to {self._target_exposure}")
-        self.camera.ExposureTime.SetValue(self._target_exposure)
-
-        if self._target_width is None:
-            self._target_width = self.camera.Width.GetMax()
-
-        if self._target_height is None:
-            self._target_height = self.camera.Height.GetMax()
-
-        self.camera.Width.SetValue(self._target_width)
-        self.camera.Height.SetValue(self._target_height)
-        self.camera.ReverseX.SetValue(True)
-        self.camera.ReverseY.SetValue(True)
-        self.camera.MaxNumBuffer = buffersize
-        
         if self._document_path is not None:
             self.save_features(
                 os.path.join(
                     self._document_path,
                     self.model_name + ".pfs"
                 )
             )
 
-        if maxframes is not None:
-            self.camera.StartGrabbingMax(maxframes)
-            # if we want to limit the number of frames
-        else:
-            self.camera.StartGrabbing(pylon.GrabStrategy_OneByOne)
+        self.camera.start()
+        self._isgrabbing = True
 
         # Print the model name of the camera.
         logger.info(f"Using device {self.model_name}")
         self._init_read()
+        self._isopen = True
+    
 
     def close(self):
-        while self._acquisition_lock.locked():
-            time.sleep(.1)
-
-        with self._acquisition_lock:
-            self.camera.Close()
+        self.stopped = True
+        self._isgrabbing = False
+        self.camera.stop()
+        exc = BaseException("0")
+        self.camera.__exit__(type(exc), exc, traceback=exc.__traceback__)
```

### Comparing `scicam-0.1.2/scicam/io/cameras/basler/compat.py` & `scicam-0.1.3/scicam/io/cameras/basler/compat.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/io/cameras/basler/parser.py` & `scicam-0.1.3/scicam/io/cameras/basler/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,13 +37,13 @@
         "--maxframes",
         type=int,
         default=math.inf,
         help="Camera fetches frames (s)",
     )
 
     ap.add_argument(
-        "--select-rois",
+        "--select-roi",
         default=False,
-        dest="select_rois",
+        dest="select_roi",
         action="store_true",
     )
     return ap
```

### Comparing `scicam-0.1.2/scicam/io/cameras/core.py` & `scicam-0.1.3/scicam/io/cameras/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __author__ = "antonio"
 
 import time
 import datetime
 import threading
 import logging
 from abc import abstractmethod
-from scicam.io.cameras.plugins import ROISPlugin, CameraUtils, SquareCamera
+from scicam.io.cameras.plugins import ROIPlugin, CameraUtils, SquareCamera
 from scicam.class_utils.time import TimeUtils
 import cv2
 
 class AbstractCamera:
 
     @property
     @abstractmethod
@@ -46,15 +46,15 @@
         raise NotImplementedError
 
     @abstractmethod
     def _next_image_default(self):
         raise NotImplementedError
 
     @abstractmethod
-    def _next_image_rois(self):
+    def _next_image_roi(self):
         raise NotImplementedError
 
     @property
     @abstractmethod
     def width(self):
         raise NotImplementedError
 
@@ -96,77 +96,83 @@
 
     @property
     @abstractmethod
     def friendly_name(self):
         raise NotImplementedError
 
 
-class BaseCamera(ROISPlugin, SquareCamera, AbstractCamera, TimeUtils, CameraUtils):
+class BaseCamera(ROIPlugin, SquareCamera, AbstractCamera, TimeUtils, CameraUtils):
 
     def __init__(
         self,
         start_time,
         width=None,
         height=None,
         framerate=30,
         framerate_offset=0,
         info_freq=60,
         exposure=15000,
+        brightness=2,
         iso=0,
         drop_each=1,
-        timeout=30000,
+        timeout=5000,
         duration=None,
         resolution_decrease=1.0,
-        rois=None,
+        roi=None,
         document_path=None,
-        idx=0,
+        camera_idx=0,
         roi_helper=None,
+        apply_roi=True,
     ):
         """
         Abstract camera class template
         Inspired by the Ethoscope project.
         """
 
-
         self.camera=None
         self._target_width = width
         self._target_height = height
         self._target_exposure = exposure
         self._target_framerate = framerate
+        self._target_brightness = brightness
         self._framerate_offset = framerate_offset
         self._target_iso = iso
         self._drop_each = drop_each
         self._timeout = timeout
         self._duration = duration
-        self._rois = rois
+        self._roi = roi
         self._time_s = None
         self._last_ticks = {}
         self._idx = None
         self._acquisition_lock = threading.Lock()
 
         self._info_freq = info_freq
 
         self._last_offset = 0
         self._frames_this_second = 0
         self._frame_idx = 0
         self._document_path = document_path
-        self.idx = idx
+        self.camera_idx = camera_idx
         self.start_time = start_time
         self.isColor = False
 
         if resolution_decrease != 1.0:
             logging.warning("Resolution decrease is not implemented. Ignoring")
-        self.open(idx=idx)
+        self.open(idx=camera_idx, apply_roi=apply_roi)
         start_time_iso=datetime.datetime.fromtimestamp(self.start_time).strftime("%Y-%m-%d %H:%M:%S")
         print(f"{self.friendly_name} initialized with timestamp {self.start_time} ({start_time_iso})")
 
         super().__init__(roi_helper=roi_helper)
 
 
     @property
+    def idx(self):
+        return self.camera_idx
+
+    @property
     def resolution(self):
         r"""
         Convenience function to return resolution of camera.
         Resolution = (number_horizontal_pixels, number_vertical_pixels)
         """
         return (
             self.width,
@@ -206,23 +212,15 @@
     def is_last_frame(self):
         if self._duration is None:
             return False
         return self._duration < self.running_for_seconds
  
 
     def _next_image(self):
-
-        if self._rois is None:
-            status, img = self._next_image_square()
-            # img = cv2.putText(img, str(self.time_stamp()), org=(100, 100), fontFace=cv2.FONT_HERSHEY_COMPLEX, fontScale=5, color=0)
-        else:
-            status, img = self._next_image_rois()
-            # img = [cv2.putText(img[0], str(self.time_stamp()), org=(100, 100), fontFace=cv2.FONT_HERSHEY_COMPLEX, fontScale=5, color=0)]
-
-        return status, img
+        return self._next_image_square()
 
 
     def _init_read(self):
         """
         Try reading a frame and check its resolution
         """
         status, img = self._next_image_square()
```

### Comparing `scicam-0.1.2/scicam/io/cameras/dlc.py` & `scicam-0.1.3/scicam/io/cameras/dlc.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/io/cameras/opencv.py` & `scicam-0.1.3/scicam/io/cameras/opencv.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,17 @@
                     code = 1
 
                 return code, img
 
 
     def _next_image_default(self):
         (code, img), msec = self._next_image_default_timeit()
+        if code == 2:
+            self.close()
+            return 0, None
         logger.debug(f"Read image from {self.model_name} in {msec} ms")
         status = 1 - code
         return status, img
 
     def save_features(self, path):
         logger.warning(f"{self.__class__}.save_features is not implemented. Ignoring")
```

### Comparing `scicam-0.1.2/scicam/io/cameras/plugins.py` & `scicam-0.1.3/scicam/io/cameras/plugins.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 import cv2
 from sklearn.metrics import RocCurveDisplay
 import numpy as np
 from cv2cuda.decorator import timeit
 import functools
+from scicam.configuration import load_setup_cameras, save_setup_cameras
 
 def make_square(easy_roi_circle):
 
     x = easy_roi_circle["center"][0] - easy_roi_circle["radius"]
     y = easy_roi_circle["center"][1] - easy_roi_circle["radius"]
     h = w = easy_roi_circle["radius"] * 2
     return [x, y, w, h]
 
     
-class ROISPlugin:
+class ROIPlugin:
     _ROIbackend = "EasyROI"
 
     """
     
     Needed signatures
 
     status, image = self._next_image_square()
     width, height = self.resolution   
     """
 
-    ROI_SEGMENTATION_PREVIEW_WIDTH = 1280
-    ROI_SEGMENTATION_PREVIEW_HEIGHT = 960
-
     def __init__(self,  *args, roi_helper=None, **kwargs):
         self._roi_helper = roi_helper
-        super(ROISPlugin, self).__init__(*args, **kwargs)
+        super(ROIPlugin, self).__init__(*args, **kwargs)
 
 
     @staticmethod
     def _crop_roi(image, roi):
         return image[
             int(roi[1]) : int(roi[1] + roi[3]),
             int(roi[0]) : int(roi[0] + roi[2]),
@@ -44,100 +42,129 @@
         r[0] = int(r[0] * fx)
         r[1] = int(r[1] * fy)
         r[2] = int(r[2] * fx)
         r[3] = int(r[3] * fy)
         roi = tuple(r)
         return roi
 
-    def _select_rois(self, image):
+    def _select_roi(self, image):
 
         if self._roi_helper and self._ROIbackend == "EasyROI":
-            print(image.shape)
             while True:
                 roi = self._roi_helper.draw_circle(image, quantity=1)["roi"][0]
+                print("circle: ", roi)
                 roi = make_square(roi)
+                print("square: ", roi)
 
                 mask = np.zeros_like(image)
                 mask[
                     roi[1]:(roi[1] + roi[3]),
                     roi[0]:(roi[0] + roi[2]),
                 ] = 255
                 applied = cv2.bitwise_and(image, mask)
                 cv2.imshow("Selected", applied)
                 if cv2.waitKey(0) == 32: #spacebar
                     break
 
-
-            roi = [roi]
-        
+       
         elif self._ROIbackend == "cv2":
-            roi = cv2.selectROIs("select the area", image)
+            raise NotImplementedError()
+            roi = cv2.selectROI("select the area", image)
                 
-        while any([v < 0 for v in roi[0]]):
-            roi = self._select_rois(image)
+        while any([v < 0 for v in roi]):
+            roi = self._select_roi(image)
         
-        print(roi)
         return roi
 
 
-    def select_ROIs(self):
+    def select_ROI(self):
         """
-        Select 1 or more ROIs
+        Select 1 ROI
         """
-        status, image = self._next_image_square()
-
-        if (
-            image.shape[1] > self.ROI_SEGMENTATION_PREVIEW_WIDTH or 
-            image.shape[0] > self.ROI_SEGMENTATION_PREVIEW_HEIGHT
-        ):
-            fx = self.ROI_SEGMENTATION_PREVIEW_WIDTH / image.shape[1] 
-            fy = self.ROI_SEGMENTATION_PREVIEW_HEIGHT / image.shape[0]
-
-            fx = min(fx, fy)
-            fy = fx
-
-            image = cv2.resize(
-                image, dsize=None, fx=fx, fy=fy, interpolation=cv2.INTER_AREA
-            )
-
-        rois = self._select_rois(image)
-
-        rois = [self._process_roi(list(roi), 1/fx, 1/fy) for roi in rois]
-        self._rois = rois
-        print("Selected ROIs")
-        for roi in self._rois:
-            print(roi)
+        status, image = self._next_image_default()
+        
+        if image.shape[0] > 1500:
+            factor = 8
+        else:
+            factor = 4
+        
+        fy = fx = factor
+        width = int(image.shape[1] / fx)
+        height = int(image.shape[0] / fy)
+        
+        image=cv2.resize(image, (width, height))
+        roi = self._select_roi(image)
         cv2.destroyAllWindows()
-        return rois
-
 
+        roi = self._process_roi(roi, fx, fy)
+        print("Selected ROI: ", roi)
 
-    def _next_image_rois(self):
-
-        status, image = self._next_image_square()
-        if not status:
-            return status, (None)
+        x = roi[0]
+        
+        if x % factor != 0:
+            x -= x%factor
+        
+        y = roi[1]
+        
+        w = roi[2]
+        h = roi[3]
+        
+        height_excess = w % self.HEIGHT_STEPS
+        if height_excess != 0:
+            h -= height_excess
+        
+        width_excess = w % self.WIDTH_STEPS
+        if width_excess != 0:
+            w -= width_excess
+            
+        if x % 2 !=0:
+            x-=1
+        
+        if y % 2 != 0:
+            y -=1
 
-        data = []
-        for r in self.rois:
-            data.append(self._crop_roi(image, r))
-        return status, data
+        # if h + y > self.HeightMax:
+        #     y = self.HeightMax - h
+        
+        # if w + x > self.WidthMax:
+        #     x = self.WidthMax - w
 
+        roi = (x, y, w, h)
+        self.save_roi(roi)
+        self._roi = roi
+
+        return (0, 0, w, h)
+
+    def save_roi(self, roi):
+        config = load_setup_cameras()
+        x, y, w, h = roi
+        
+        config[self.supplier][self.camera_idx]["Width"] = w
+        config[self.supplier][self.camera_idx]["Height"] = h
+        config[self.supplier][self.camera_idx]["OffsetX"] = x
+        config[self.supplier][self.camera_idx]["OffsetY"] = y        
+        res=save_setup_cameras(config)
+        
+        config = load_setup_cameras()
+        assert "pixels_per_cm" in config[self.supplier][self.camera_idx]
+        
+        return res
+        
 
     @property
-    def rois(self):
-        if self._rois is None:
+    def roi(self):
+        if self._roi is None:
             try:
                 return [(0, 0, *self.resolution)]
             except:
                 raise Exception(
                     "Please open the camera before asking for its resolution"
                 )
         else:
-            return self._rois
+            return self._roi
 
 
 
 class CameraUtils:
 
     def _count_frames_in_second(self):
         offset = self._time_s % 1000
@@ -159,15 +186,15 @@
             left = right = 0
             bottom = top = (shape[1] - shape[0]) / 2
             diff = shape[1] - shape[0] - bottom - top
             if diff > 0:
                 bottom += diff
         
         elif shape[0] > shape[1]:
-            top, bottom = 0
+            top = bottom = 0
             left = right = (shape[0] - shape[1]) / 2
             diff = shape[0] - shape[1] - left - right
             if diff > 0:
                 right += diff
         
         else:
             top = bottom = left = right = 0
@@ -182,14 +209,15 @@
             top, bottom, left, right,
             borderType=cv2.BORDER_CONSTANT, value=self.VALUE_OF_BACKGROUND
         )
         return image
 
     def _next_image_square(self):
         code, image = self._next_image_default()
+
         if image is not None:
             if image.shape[0] != image.shape[1]:
                 image, msec = self.apply_pad(image)
                 assert image.shape[0] == image.shape[1]
 
-
+        # print(image.shape)
         return code, image
```

### Comparing `scicam-0.1.2/scicam/io/cameras/utils.py` & `scicam-0.1.3/scicam/io/cameras/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,26 +20,43 @@
     except Exception as error:
         print(error)
         print(f"{camera} cannot mark frame")
 
     return img
 
 
-def validate_img(img):
-    fail = img is None or img.shape[0] is None
-    return not fail
+def validate_img(img, target_shape=None):
+    """
+    Return 0 if the img is fine, 1 if it's None
+    and 2 if it's not None but it has a shape different from the expected 
+    """
 
-def ensure_img(camera, waiting_time=None):
+    img_is_None = img is None or img.shape[0] is None
+    image_is_corrupt=False
+    if not img_is_None and target_shape is not None:
+        image_is_corrupt = target_shape[0] != img.shape[0] or target_shape[1] != img.shape[1]
+
+
+    if not img_is_None and not image_is_corrupt:
+        return 0
+    elif img_is_None:
+        return 1
+    elif image_is_corrupt:
+        try:
+            cv2.imwrite(f"/home/vibflysleep/{time.time()}-corrupt_image.png", img)
+        except:
+            print("Could not save corrupt image")
+
+        return 2
+
+def ensure_img(camera):
     print("Alert: img is None")
     before = time.time()
-    print(f"Closing {camera}")
     camera.close()
-    if waiting_time is not None:
-        time.sleep(waiting_time)
-    print(f"Opening {camera}")
+
     camera.open(idx=camera._idx)
     warnings.warn("Recursive call to next_image_default_timeit")
     (code, img), msec =camera._next_image_default_timeit()
     if img.shape[0] is None:
 
         print("img is still None, look below")
         print(img.shape)
```

### Comparing `scicam-0.1.2/scicam/io/recorders/__main__.py` & `scicam-0.1.3/scicam/io/recorders/__main__.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/io/recorders/core.py` & `scicam-0.1.3/scicam/io/recorders/core.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/io/recorders/imgstore.py` & `scicam-0.1.3/scicam/io/recorders/imgstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ENCODER_FORMAT_CPU="divx/avi"
 ENCODER_FORMAT_GPU="h264_nvenc/mp4"
 
 logger = logging.getLogger(__name__)
 run_logger = logging.getLogger(f"{__name__}.run")
 
 class ImgStoreRecorder(BaseRecorder):
-        
+
     # look here for possible formats:
     # Video -> https://github.com/loopbio/imgstore/blob/d69035306d816809aaa3028b919f0f48455edb70/imgstore/stores.py#L932
     # Images -> https://github.com/loopbio/imgstore/blob/d69035306d816809aaa3028b919f0f48455edb70/imgstore/stores.py#L805
     # if you dont have enough RAM, you dont want to make this number huge
     # otherwise you will run out of RAM
 
     def __init__(
@@ -46,14 +46,15 @@
         if format is None:
             logger.warning(
                 f"scicam using {ENCODER_FORMAT_CPU} to encode video data"
                 f" you may want to use {ENCODER_FORMAT_GPU} if CUDA is enabled"
             )
             format = ENCODER_FORMAT_CPU
 
+
         self._current_chunk = -1
         self.chunk_duration = chunk_duration
         logger.debug(f"{self} chunk_duration: {chunk_duration}")
         self._chunksize = self.chunk_duration * self._framerate
         self._buffer_usage = 0
         self._format = format
         self._start_event = multiprocessing.Event()
@@ -64,28 +65,27 @@
         self._fps = 0
 
         self._info_freq = info_frequency
         self._extra_data_freq = extra_data_frequency
 
 
         imgshape = self._resolution[:2][::-1]
-        metadata = {}
 
         versions = document_for_reproducibility()
-        metadata.update(versions)
+        self.metadata.update(versions)
 
         self._video_writer = imgstore.new_for_format(
             mode="w",
             fmt=format,
             fps=self._framerate,
             basedir=self._path,
             imgshape=imgshape,
             chunksize=self._chunksize,
             imgdtype=np.uint8,
-            **metadata
+            **self.metadata
         )
 
         self._make_tqdm = True
 
         if self._make_tqdm:
             self._tqdm = tqdm.tqdm(
                 position=self.idx,
@@ -97,26 +97,26 @@
     @property
     def n_saved_frames(self):
         return self._n_saved_frames
 
     @property
     def buffer_usage(self):
         return self._buffer_usage
-    
+
     def __str__(self):
         return self.name
 
     @property
     def name(self):
         return f"ImgStore - {self._path}"
 
     def report_time(self):
         logger.debug(f"{self._path} - Timestamp {time.time()} @ {self._video_writer._basedir}: {self._video_writer._tN}")
         logger.debug(f"{self._path} - Timestamp {time.time()} @ {self._video_writer._basedir}: {self._time_s}")
-                
+
     def _process_data(self, data):
         timestamp, i, frame, camera_info = data
         if camera_info is not None:
             self._camera_info = camera_info
 
         self._time_s = timestamp / 1000
         run_logger.debug("_write")
@@ -147,23 +147,21 @@
 
     def _get_environmental_data(self):
         logger.debug("flyhostel.sensor.query")
         return self._sensor.query(timeout=1)
 
 
     def save_extra_data(self):
-
         code = 1
         if self.sensor is None:
             return code
 
         logger.debug("_get_environmental_data")
         environmental_data = self._get_environmental_data()
 
-
         if environmental_data is None:
             logger.warning("Could not fetch environmental data")
         else:
             logger.debug("_save_extra_data")
             code = self._save_extra_data(
                 camera_temperature=self._camera_info.get("temperature", None),
                 temperature=environmental_data["temperature"],
@@ -209,15 +207,15 @@
         self.start_time = time.time()
         self._start_event.set()
 
         try:
             logger.debug("before call to imgstore._run")
             self._run()
             logger.debug("after call to imgstore._run")
-    
+
         except ServiceExit:
             print(f"ServiceExit detected by {self}. Please wait")
         except Exception as error:
             logger.error(error)
             logger.error(traceback.print_exc())
 
         finally:
@@ -227,56 +225,56 @@
 
             logger.debug("imgstore finishing")
             logger.debug(
                 "Queues: "\
                 f" data_queue: {self._data_queue.qsize()}"\
                 f" stop_queue: {self._stop_queue.qsize()}"\
             )
-            
-            return 
+
+            return
 
 
     def _exit_gracefully(self):
         if not self.check_data_queue(target=0):
             logger.warning(f"{self} - Buffer usage on exit {self._buffer_usage} != 0")
         assert self._stop_queue.empty()
         return 0
 
 
 
     def _run(self):
         while not self._stop_event.is_set():
-            
+
             if self.tick(1):
                 self._fps = 0
 
             if self.tick(self._info_freq):
                 self._report(self._buffer_usage)
+
             if self.tick(self._extra_data_freq):
                 self.save_extra_data()
-            
             if self.should_stop():
                 break
 
             code, msec = self._run_data()
             if code != 0:
                 break
 
         while not self.check_data_queue(target=0):
             if self.tick(self._info_freq):
                 self._report(self._buffer_usage)
             if self.tick(self._extra_data_freq):
                 self.save_extra_data()
-                
+
             code, msec = self._run_data()
             if code != 0:
                 break
 
         logger.debug(f"should stop: {self.should_stop()}")
- 
+
 
     def safe_join(self, timeout):
         self.join(timeout=timeout)
         if self.exitcode is None:
             return 1
         else:
             return self.exitcode
@@ -292,40 +290,46 @@
 
 
     def _report(self, target):
         self._report_fps()
         self._check_io_benchmark()
         self.check_data_queue(target=target)
         self.report_time()
-    
+
     def _report_fps(self):
         logger.debug(f"{self._path} - Saved frames {self._n_saved_frames}")
         logger.debug(f"{self._path} - {self._fps} FPS")
 
     def _check_io_benchmark(self):
         loop_ms_latency_mean = np.array(self._loop_latency).mean()
         logger.debug(f"{self._path} - Average loop time: {loop_ms_latency_mean:.2f} ms")
-        
+
         read_ms_latency_mean = np.array(self._read_latency).mean()
         logger.debug(f"{self._path}- Average read time: {read_ms_latency_mean:.2f} ms")
-        
+
         write_latency_mean = np.array(self._write_latency).mean()
         logger.debug(f"{self._path} - Average write time: {write_latency_mean:.2f} ms")
         logger.debug(f"{self._path} - Last write time: {self._write_msec:.2f} ms")
 
         file_size_mean = np.array(self._file_size).mean()
         logger.debug(f"{self._path} - Average file size: {file_size_mean:.2f} MB")
-    
+
 
     def check_data_queue(self, target=0):
 
         q = self._data_queue
-        buffer_usage = q.view.nbytes_el * q.qsize() / q.maxbytes
+        assert q is not None
+        view = q.view
+        if view is None:
+            buffer_usage = 0
+        else:
+            buffer_usage = view.nbytes_el * q.qsize() / q.maxbytes
+
 
-        if buffer_usage != target:
+        if buffer_usage is not None and buffer_usage != target:
 
             if self._make_tqdm:
                 self._tqdm.n = int(self._buffer_usage)
                 self._tqdm.refresh()
             else:
 
                 logger.info(
@@ -346,27 +350,30 @@
         """
         if not self._stop_event.is_set():
             self._timestamp = timestamp
 
         if frame is None:
             return None
 
+
+        assert frame.shape[0] == frame.shape[1], f"{frame.shape} is not squared"
+
         self._video_writer.add_image(frame, i, timestamp)
         self._n_saved_frames += 1
         self._fps += 1
         return None
-    
+
 
     def _has_new_chunk(self):
         current_chunk = self._video_writer._chunk_n
         if current_chunk > self._current_chunk:
             self._current_chunk = current_chunk
             return True
         else:
             return False
 
     def _save_first_frame_of_chunk(self, frame=None):
 
         last_shot_path = os.path.join(
             self._path, str(self._current_chunk).zfill(6) + ".png"
         )
-        cv2.imwrite(last_shot_path, frame)
+        cv2.imwrite(last_shot_path, frame)
```

### Comparing `scicam-0.1.2/scicam/io/recorders/mixins/ffmpeg.py` & `scicam-0.1.3/scicam/io/recorders/mixins/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/io/recorders/mixins/opencv.py` & `scicam-0.1.3/scicam/io/recorders/mixins/opencv.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/io/recorders/parser.py` & `scicam-0.1.3/scicam/io/recorders/parser.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/io/recorders/record.py` & `scicam-0.1.3/scicam/io/recorders/record.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/tests/test_basler.py` & `scicam-0.1.3/scicam/tests/test_basler.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,23 @@
         with BaslerCamera() as self.camera:
             ret, frame = self.camera.read()
             self.assertTrue(isinstance(frame, np.ndarray))
        
 
     def test_camera_loops(self):
         self.camera = BaslerCamera()
-        for timestamp, rois in self.camera:
-            self.assertIsInstance(rois[0], np.ndarray)
+        for timestamp, roi in self.camera:
+            self.assertIsInstance(roi, np.ndarray)
             self.assertLess(timestamp - self.camera.start_time, 5)
             break
         
         self.camera.close()
 
 
-    def test_rois(self):
+    def test_roi(self):
 
         self.camera = BaslerCamera(rois=[(0, 0, 100, 50)])
         for timestamp, rois in self.camera:
             self.assertEqual(rois[0].shape[0], 50)
             self.assertEqual(rois[0].shape[1], 100)
             break
```

### Comparing `scicam-0.1.2/scicam/tests/test_recorder.py` & `scicam-0.1.3/scicam/tests/test_recorder.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/tests/test_synchrony.py` & `scicam-0.1.3/scicam/tests/test_synchrony.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/tests/utils.py` & `scicam-0.1.3/scicam/tests/utils.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/utils.py` & `scicam-0.1.3/scicam/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     return metadata
 
 
 
 def load_config():
     with open(CONFIG_FILE, "r") as fh:
         config = json.load(fh)
-
     return config
 
 
 
 def service_shutdown(signum, frame):
     print("Caught signal %d" % signum)
     raise ServiceExit
```

### Comparing `scicam-0.1.2/scicam/web_utils/client.py` & `scicam-0.1.3/scicam/web_utils/client.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/web_utils/sensor.py` & `scicam-0.1.3/scicam/web_utils/sensor.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam/web_utils/server.py` & `scicam-0.1.3/scicam/web_utils/server.py`

 * *Files identical despite different names*

### Comparing `scicam-0.1.2/scicam.egg-info/SOURCES.txt` & `scicam-0.1.3/scicam.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.py
 scicam/__init__.py
 scicam/_version.py
+scicam/configuration.py
 scicam/constants.py
 scicam/decorators.py
 scicam/exceptions.py
 scicam/utils.py
 scicam.egg-info/PKG-INFO
 scicam.egg-info/SOURCES.txt
 scicam.egg-info/dependency_links.txt
```

### Comparing `scicam-0.1.2/setup.py` & `scicam-0.1.3/setup.py`

 * *Files identical despite different names*

