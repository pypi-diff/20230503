# Comparing `tmp/ddparo-0.4.0.tar.gz` & `tmp/ddparo-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddparo-0.4.0.tar", last modified: Wed May  3 07:02:41 2023, max compression
+gzip compressed data, was "ddparo-0.5.0.tar", last modified: Wed May  3 07:05:30 2023, max compression
```

## Comparing `ddparo-0.4.0.tar` & `ddparo-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 07:02:41.757502 ddparo-0.4.0/
--rw-rw-rw-   0        0        0       53 2023-05-03 07:02:41.755502 ddparo-0.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 07:02:41.711437 ddparo-0.4.0/ddparo/
--rw-rw-rw-   0        0        0        0 2023-05-03 06:50:50.000000 ddparo-0.4.0/ddparo/__init__.py
--rw-rw-rw-   0        0        0      414 2023-05-03 06:57:42.000000 ddparo-0.4.0/ddparo/ddparo.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:02:41.753503 ddparo-0.4.0/ddparo.egg-info/
--rw-rw-rw-   0        0        0       53 2023-05-03 07:02:41.000000 ddparo-0.4.0/ddparo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-05-03 07:02:41.000000 ddparo-0.4.0/ddparo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 07:02:41.000000 ddparo-0.4.0/ddparo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-03 07:02:41.000000 ddparo-0.4.0/ddparo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-05-03 07:02:41.000000 ddparo-0.4.0/ddparo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 07:02:41.000000 ddparo-0.4.0/ddparo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 07:02:41.758502 ddparo-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      314 2023-05-03 07:02:35.000000 ddparo-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:05:30.554171 ddparo-0.5.0/
+-rw-rw-rw-   0        0        0       53 2023-05-03 07:05:30.551912 ddparo-0.5.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 07:05:30.514677 ddparo-0.5.0/ddparo/
+-rw-rw-rw-   0        0        0        0 2023-05-03 06:50:50.000000 ddparo-0.5.0/ddparo/__init__.py
+-rw-rw-rw-   0        0        0      375 2023-05-03 07:05:12.000000 ddparo-0.5.0/ddparo/ddparo.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:05:30.549813 ddparo-0.5.0/ddparo.egg-info/
+-rw-rw-rw-   0        0        0       53 2023-05-03 07:05:30.000000 ddparo-0.5.0/ddparo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-05-03 07:05:30.000000 ddparo-0.5.0/ddparo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 07:05:30.000000 ddparo-0.5.0/ddparo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-03 07:05:30.000000 ddparo-0.5.0/ddparo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-05-03 07:05:30.000000 ddparo-0.5.0/ddparo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 07:05:30.000000 ddparo-0.5.0/ddparo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 07:05:30.555171 ddparo-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      314 2023-05-03 07:05:18.000000 ddparo-0.5.0/setup.py
```

