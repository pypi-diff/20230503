# Comparing `tmp/skyndo-0.6.tar.gz` & `tmp/skyndo-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyndo-0.6.tar", last modified: Wed May  3 10:51:42 2023, max compression
+gzip compressed data, was "skyndo-0.7.tar", last modified: Wed May  3 11:07:07 2023, max compression
```

## Comparing `skyndo-0.6.tar` & `skyndo-0.7.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 10:51:42.636724 skyndo-0.6/
--rw-rw-rw-   0        0        0      376 2023-05-03 10:51:42.551951 skyndo-0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-03 10:51:42.637722 skyndo-0.6/setup.cfg
--rw-rw-rw-   0        0        0      539 2023-05-03 10:50:19.000000 skyndo-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 10:51:42.549957 skyndo-0.6/skyndo.egg-info/
--rw-rw-rw-   0        0        0      376 2023-05-03 10:51:40.000000 skyndo-0.6/skyndo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-05-03 10:51:40.000000 skyndo-0.6/skyndo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 10:51:40.000000 skyndo-0.6/skyndo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-03 10:51:40.000000 skyndo-0.6/skyndo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 10:51:40.000000 skyndo-0.6/skyndo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 11:07:07.253608 skyndo-0.7/
+-rw-rw-rw-   0        0        0      376 2023-05-03 11:07:07.252610 skyndo-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:07:07.255602 skyndo-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      506 2023-05-03 11:03:39.000000 skyndo-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:07:07.021175 skyndo-0.7/skyndo/
+-rw-rw-rw-   0        0        0        0 2023-03-31 15:55:53.000000 skyndo-0.7/skyndo/_init_.py
+-rw-rw-rw-   0        0        0     2175 2023-04-12 06:02:34.000000 skyndo-0.7/skyndo/predict.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:07:07.250615 skyndo-0.7/skyndo.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-05-03 11:07:05.000000 skyndo-0.7/skyndo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-05-03 11:07:05.000000 skyndo-0.7/skyndo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:07:05.000000 skyndo-0.7/skyndo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-03 11:07:05.000000 skyndo-0.7/skyndo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 11:07:05.000000 skyndo-0.7/skyndo.egg-info/top_level.txt
```

