# Comparing `tmp/ddparo-0.2.0.tar.gz` & `tmp/ddparo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddparo-0.2.0.tar", last modified: Wed May  3 06:55:40 2023, max compression
+gzip compressed data, was "ddparo-0.3.0.tar", last modified: Wed May  3 06:58:00 2023, max compression
```

## Comparing `ddparo-0.2.0.tar` & `ddparo-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 06:55:40.095032 ddparo-0.2.0/
--rw-rw-rw-   0        0        0       53 2023-05-03 06:55:40.094035 ddparo-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 06:55:40.092152 ddparo-0.2.0/ddparo.egg-info/
--rw-rw-rw-   0        0        0       53 2023-05-03 06:55:39.000000 ddparo-0.2.0/ddparo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-05-03 06:55:39.000000 ddparo-0.2.0/ddparo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 06:55:39.000000 ddparo-0.2.0/ddparo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-03 06:55:39.000000 ddparo-0.2.0/ddparo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-05-03 06:55:39.000000 ddparo-0.2.0/ddparo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 06:55:39.000000 ddparo-0.2.0/ddparo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 06:55:40.095888 ddparo-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      289 2023-05-03 06:55:20.000000 ddparo-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:58:00.153011 ddparo-0.3.0/
+-rw-rw-rw-   0        0        0       53 2023-05-03 06:58:00.151832 ddparo-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 06:58:00.149999 ddparo-0.3.0/ddparo.egg-info/
+-rw-rw-rw-   0        0        0       53 2023-05-03 06:58:00.000000 ddparo-0.3.0/ddparo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-05-03 06:58:00.000000 ddparo-0.3.0/ddparo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 06:58:00.000000 ddparo-0.3.0/ddparo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-03 06:58:00.000000 ddparo-0.3.0/ddparo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-05-03 06:58:00.000000 ddparo-0.3.0/ddparo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 06:58:00.000000 ddparo-0.3.0/ddparo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 06:58:00.153511 ddparo-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      291 2023-05-03 06:57:47.000000 ddparo-0.3.0/setup.py
```

