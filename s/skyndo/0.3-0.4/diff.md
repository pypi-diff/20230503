# Comparing `tmp/skyndo-0.3.tar.gz` & `tmp/skyndo-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyndo-0.3.tar", last modified: Wed May  3 09:32:28 2023, max compression
+gzip compressed data, was "skyndo-0.4.tar", last modified: Wed May  3 10:09:44 2023, max compression
```

## Comparing `skyndo-0.3.tar` & `skyndo-0.4.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:32:28.888849 skyndo-0.3/
--rw-rw-rw-   0        0        0      352 2023-05-03 09:32:28.887855 skyndo-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2175 2023-04-12 06:02:34.000000 skyndo-0.3/predict.py
--rw-rw-rw-   0        0        0       42 2023-05-03 09:32:28.888849 skyndo-0.3/setup.cfg
--rw-rw-rw-   0        0        0      518 2023-05-03 09:30:34.000000 skyndo-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:32:28.886859 skyndo-0.3/skyndo.egg-info/
--rw-rw-rw-   0        0        0      352 2023-05-03 09:32:28.000000 skyndo-0.3/skyndo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-05-03 09:32:28.000000 skyndo-0.3/skyndo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:32:28.000000 skyndo-0.3/skyndo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-03 09:32:28.000000 skyndo-0.3/skyndo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 09:32:28.000000 skyndo-0.3/skyndo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 10:09:44.874191 skyndo-0.4/
+-rw-rw-rw-   0        0        0      376 2023-05-03 10:09:44.873194 skyndo-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-03 10:09:44.874191 skyndo-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-05-03 10:09:23.000000 skyndo-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:09:44.872196 skyndo-0.4/skyndo.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-05-03 10:09:44.000000 skyndo-0.4/skyndo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-05-03 10:09:44.000000 skyndo-0.4/skyndo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 10:09:44.000000 skyndo-0.4/skyndo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-03 10:09:44.000000 skyndo-0.4/skyndo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 10:09:44.000000 skyndo-0.4/skyndo.egg-info/top_level.txt
```

