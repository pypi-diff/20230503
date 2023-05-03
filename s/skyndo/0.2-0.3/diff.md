# Comparing `tmp/skyndo-0.2.tar.gz` & `tmp/skyndo-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyndo-0.2.tar", last modified: Wed May  3 06:45:45 2023, max compression
+gzip compressed data, was "skyndo-0.3.tar", last modified: Wed May  3 09:32:28 2023, max compression
```

## Comparing `skyndo-0.2.tar` & `skyndo-0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 06:45:45.843825 skyndo-0.2/
--rw-rw-rw-   0        0        0      352 2023-05-03 06:45:45.837841 skyndo-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-03 06:45:45.843825 skyndo-0.2/setup.cfg
--rw-rw-rw-   0        0        0      493 2023-05-03 06:41:52.000000 skyndo-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 06:45:45.835847 skyndo-0.2/skyndo.egg-info/
--rw-rw-rw-   0        0        0      352 2023-05-03 06:45:44.000000 skyndo-0.2/skyndo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-05-03 06:45:44.000000 skyndo-0.2/skyndo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 06:45:44.000000 skyndo-0.2/skyndo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-03 06:45:44.000000 skyndo-0.2/skyndo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 06:45:44.000000 skyndo-0.2/skyndo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 09:32:28.888849 skyndo-0.3/
+-rw-rw-rw-   0        0        0      352 2023-05-03 09:32:28.887855 skyndo-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2175 2023-04-12 06:02:34.000000 skyndo-0.3/predict.py
+-rw-rw-rw-   0        0        0       42 2023-05-03 09:32:28.888849 skyndo-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      518 2023-05-03 09:30:34.000000 skyndo-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:32:28.886859 skyndo-0.3/skyndo.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-05-03 09:32:28.000000 skyndo-0.3/skyndo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-05-03 09:32:28.000000 skyndo-0.3/skyndo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 09:32:28.000000 skyndo-0.3/skyndo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-03 09:32:28.000000 skyndo-0.3/skyndo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 09:32:28.000000 skyndo-0.3/skyndo.egg-info/top_level.txt
```

