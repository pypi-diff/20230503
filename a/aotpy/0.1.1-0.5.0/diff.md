# Comparing `tmp/aotpy-0.1.1.tar.gz` & `tmp/aotpy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aotpy-0.1.1.tar", last modified: Sun Jul 17 01:38:19 2022, max compression
+gzip compressed data, was "aotpy-0.5.0.tar", last modified: Tue May  2 23:06:33 2023, max compression
```

## Comparing `aotpy-0.1.1.tar` & `aotpy-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,43 @@
-drwxrwxrwx   0        0        0        0 2022-07-17 01:38:19.555536 aotpy-0.1.1/
--rw-rw-rw-   0        0        0     1592 2022-07-17 00:31:34.000000 aotpy-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2635 2022-07-17 01:38:19.555536 aotpy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1940 2022-07-17 01:22:37.000000 aotpy-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-07-17 01:38:19.517801 aotpy-0.1.1/aotpy/
--rw-rw-rw-   0        0        0       80 2022-07-07 13:10:31.000000 aotpy-0.1.1/aotpy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-17 01:38:19.539903 aotpy-0.1.1/aotpy/fits/
--rw-rw-rw-   0        0        0       81 2022-06-30 15:26:34.000000 aotpy-0.1.1/aotpy/fits/__init__.py
--rw-rw-rw-   0        0        0     6537 2022-07-07 12:21:33.000000 aotpy-0.1.1/aotpy/fits/_keywords.py
--rw-rw-rw-   0        0        0    19727 2022-07-07 12:23:01.000000 aotpy-0.1.1/aotpy/fits/reader.py
--rw-rw-rw-   0        0        0    29015 2022-07-07 12:30:56.000000 aotpy-0.1.1/aotpy/fits/writer.py
-drwxrwxrwx   0        0        0        0 2022-07-17 01:38:19.539903 aotpy-0.1.1/aotpy/level0/
--rw-rw-rw-   0        0        0      268 2022-03-04 13:10:33.000000 aotpy-0.1.1/aotpy/level0/__init__.py
--rw-rw-rw-   0        0        0      955 2022-05-02 10:15:50.000000 aotpy-0.1.1/aotpy/level0/ao_system.py
--rw-rw-rw-   0        0        0      574 2022-05-02 09:59:08.000000 aotpy-0.1.1/aotpy/level0/atmosphere.py
--rw-rw-rw-   0        0        0     2761 2022-06-30 15:46:28.000000 aotpy-0.1.1/aotpy/level0/image.py
--rw-rw-rw-   0        0        0     2395 2022-05-19 17:04:09.000000 aotpy-0.1.1/aotpy/level0/optical_sensor.py
--rw-rw-rw-   0        0        0     1166 2022-06-30 14:44:42.000000 aotpy-0.1.1/aotpy/level0/rtc.py
--rw-rw-rw-   0        0        0      676 2022-07-07 12:21:00.000000 aotpy-0.1.1/aotpy/level0/source.py
--rw-rw-rw-   0        0        0      548 2022-05-02 15:50:27.000000 aotpy-0.1.1/aotpy/level0/telescope.py
--rw-rw-rw-   0        0        0      917 2022-05-02 10:25:20.000000 aotpy-0.1.1/aotpy/level0/wavefront_corrector.py
-drwxrwxrwx   0        0        0        0 2022-07-17 01:38:19.555536 aotpy-0.1.1/aotpy/translators/
--rw-rw-rw-   0        0        0       64 2022-07-07 10:22:50.000000 aotpy-0.1.1/aotpy/translators/__init__.py
--rw-rw-rw-   0        0        0     8212 2022-07-16 23:41:26.000000 aotpy-0.1.1/aotpy/translators/aof.py
--rw-rw-rw-   0        0        0    19370 2022-07-17 00:11:41.000000 aotpy-0.1.1/aotpy/translators/keck.py
-drwxrwxrwx   0        0        0        0 2022-07-17 01:38:19.539903 aotpy-0.1.1/aotpy.egg-info/
--rw-rw-rw-   0        0        0     2635 2022-07-17 01:38:19.000000 aotpy-0.1.1/aotpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      610 2022-07-17 01:38:19.000000 aotpy-0.1.1/aotpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-17 01:38:19.000000 aotpy-0.1.1/aotpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2022-07-17 01:38:19.000000 aotpy-0.1.1/aotpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-07-17 01:38:19.000000 aotpy-0.1.1/aotpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      851 2022-07-17 01:38:19.555536 aotpy-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.643905 aotpy-0.5.0/
+-rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2991 2023-05-02 23:06:33.643905 aotpy-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.574897 aotpy-0.5.0/aotpy/
+drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.606175 aotpy-0.5.0/aotpy/aotpy.egg-info/
+-rw-rw-rw-   0        0        0     2991 2023-05-02 23:06:33.000000 aotpy-0.5.0/aotpy/aotpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2023-05-02 23:06:33.000000 aotpy-0.5.0/aotpy/aotpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 23:06:33.000000 aotpy-0.5.0/aotpy/aotpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2023-05-02 23:06:33.000000 aotpy-0.5.0/aotpy/aotpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-02 23:06:33.000000 aotpy-0.5.0/aotpy/aotpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.621804 aotpy-0.5.0/aotpy/core/
+-rw-rw-rw-   0        0        0      580 2023-04-19 14:10:55.000000 aotpy-0.5.0/aotpy/core/__init__.py
+-rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.5.0/aotpy/core/aberration.py
+-rw-rw-rw-   0        0        0     3945 2023-05-02 11:25:41.000000 aotpy-0.5.0/aotpy/core/ao_system.py
+-rw-rw-rw-   0        0        0     2227 2023-05-02 09:36:11.000000 aotpy-0.5.0/aotpy/core/atmosphere.py
+-rw-rw-rw-   0        0        0      675 2023-05-02 18:16:26.000000 aotpy-0.5.0/aotpy/core/base.py
+-rw-rw-rw-   0        0        0     1177 2023-05-02 18:40:00.000000 aotpy-0.5.0/aotpy/core/geometry.py
+-rw-rw-rw-   0        0        0     1840 2023-05-02 13:49:09.000000 aotpy-0.5.0/aotpy/core/image.py
+-rw-rw-rw-   0        0        0     4706 2023-05-02 09:40:01.000000 aotpy-0.5.0/aotpy/core/loop.py
+-rw-rw-rw-   0        0        0     8912 2023-05-02 18:10:07.000000 aotpy-0.5.0/aotpy/core/optical_sensor.py
+-rw-rw-rw-   0        0        0     2701 2023-05-02 09:42:13.000000 aotpy-0.5.0/aotpy/core/source.py
+-rw-rw-rw-   0        0        0     4059 2023-05-02 18:40:18.000000 aotpy-0.5.0/aotpy/core/telescope.py
+-rw-rw-rw-   0        0        0      708 2023-05-02 09:43:33.000000 aotpy-0.5.0/aotpy/core/time.py
+-rw-rw-rw-   0        0        0     2728 2023-05-02 09:43:55.000000 aotpy-0.5.0/aotpy/core/wavefront_corrector.py
+drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.621804 aotpy-0.5.0/aotpy/io/
+-rw-rw-rw-   0        0        0      436 2023-05-02 11:33:11.000000 aotpy-0.5.0/aotpy/io/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-05-02 11:47:25.000000 aotpy-0.5.0/aotpy/io/base.py
+drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.637398 aotpy-0.5.0/aotpy/io/fits/
+-rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.5.0/aotpy/io/fits/__init__.py
+-rw-rw-rw-   0        0        0    27403 2023-05-02 18:52:02.000000 aotpy-0.5.0/aotpy/io/fits/_keywords.py
+-rw-rw-rw-   0        0        0    43200 2023-05-02 18:40:00.000000 aotpy-0.5.0/aotpy/io/fits/reader.py
+-rw-rw-rw-   0        0        0     8853 2023-05-02 18:40:00.000000 aotpy-0.5.0/aotpy/io/fits/utils.py
+-rw-rw-rw-   0        0        0    31196 2023-05-02 18:26:21.000000 aotpy-0.5.0/aotpy/io/fits/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-02 23:06:33.643905 aotpy-0.5.0/aotpy/translators/
+-rw-rw-rw-   0        0        0      358 2023-05-02 17:59:07.000000 aotpy-0.5.0/aotpy/translators/__init__.py
+-rw-rw-rw-   0        0        0    11807 2023-05-02 17:53:53.000000 aotpy-0.5.0/aotpy/translators/aof.py
+-rw-rw-rw-   0        0        0      979 2023-05-02 18:03:17.000000 aotpy-0.5.0/aotpy/translators/base.py
+-rw-rw-rw-   0        0        0     7404 2023-05-02 17:56:25.000000 aotpy-0.5.0/aotpy/translators/ciao.py
+-rw-rw-rw-   0        0        0     8553 2023-05-02 18:43:53.000000 aotpy-0.5.0/aotpy/translators/eso.py
+-rw-rw-rw-   0        0        0     6487 2023-05-02 17:55:46.000000 aotpy-0.5.0/aotpy/translators/naomi.py
+-rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1024 2023-05-02 23:06:33.643905 aotpy-0.5.0/setup.cfg
```

### Comparing `aotpy-0.1.1/LICENSE` & `aotpy-0.5.0/LICENSE`

 * *Files identical despite different names*

