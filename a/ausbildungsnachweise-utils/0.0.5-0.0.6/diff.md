# Comparing `tmp/ausbildungsnachweise_utils-0.0.5.tar.gz` & `tmp/ausbildungsnachweise_utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ausbildungsnachweise_utils-0.0.5.tar", last modified: Fri Apr 28 07:30:04 2023, max compression
+gzip compressed data, was "ausbildungsnachweise_utils-0.0.6.tar", last modified: Wed May  3 07:30:52 2023, max compression
```

## Comparing `ausbildungsnachweise_utils-0.0.5.tar` & `ausbildungsnachweise_utils-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-04-28 07:30:04.940414 ausbildungsnachweise_utils-0.0.5/
--rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-04-28 07:30:04.940414 ausbildungsnachweise_utils-0.0.5/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)       28 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.5/README.md
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-04-28 07:30:04.936414 ausbildungsnachweise_utils-0.0.5/ausbildungsnachweise_utils/
--rw-r--r--   0 sam       (1000) sam       (1000)        0 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.5/ausbildungsnachweise_utils/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)       90 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.5/ausbildungsnachweise_utils/__main__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3085 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.5/ausbildungsnachweise_utils/processor.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1669 2023-04-28 07:28:28.000000 ausbildungsnachweise_utils-0.0.5/ausbildungsnachweise_utils/starter.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-04-28 07:30:04.940414 ausbildungsnachweise_utils-0.0.5/ausbildungsnachweise_utils.egg-info/
--rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-04-28 07:30:04.000000 ausbildungsnachweise_utils-0.0.5/ausbildungsnachweise_utils.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)      476 2023-04-28 07:30:04.000000 ausbildungsnachweise_utils-0.0.5/ausbildungsnachweise_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-04-28 07:30:04.000000 ausbildungsnachweise_utils-0.0.5/ausbildungsnachweise_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       88 2023-04-28 07:30:04.000000 ausbildungsnachweise_utils-0.0.5/ausbildungsnachweise_utils.egg-info/entry_points.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       20 2023-04-28 07:30:04.000000 ausbildungsnachweise_utils-0.0.5/ausbildungsnachweise_utils.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       27 2023-04-28 07:30:04.000000 ausbildungsnachweise_utils-0.0.5/ausbildungsnachweise_utils.egg-info/top_level.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-04-28 07:30:04.940414 ausbildungsnachweise_utils-0.0.5/setup.cfg
--rw-r--r--   0 sam       (1000) sam       (1000)      891 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.5/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 07:30:52.651048 ausbildungsnachweise_utils-0.0.6/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-05-03 07:30:52.651048 ausbildungsnachweise_utils-0.0.6/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)       28 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.6/README.md
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 07:30:52.651048 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils/
+-rw-r--r--   0 sam       (1000) sam       (1000)        0 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)       90 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils/__main__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3085 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils/processor.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2204 2023-05-03 07:23:35.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils/starter.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-05-03 07:30:52.651048 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)      380 2023-05-03 07:30:52.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      476 2023-05-03 07:30:52.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-05-03 07:30:52.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       88 2023-05-03 07:30:52.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       20 2023-05-03 07:30:52.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/requires.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       27 2023-05-03 07:30:52.000000 ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils.egg-info/top_level.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-05-03 07:30:52.651048 ausbildungsnachweise_utils-0.0.6/setup.cfg
+-rw-r--r--   0 sam       (1000) sam       (1000)      891 2023-04-14 08:12:04.000000 ausbildungsnachweise_utils-0.0.6/setup.py
```

### Comparing `ausbildungsnachweise_utils-0.0.5/ausbildungsnachweise_utils/processor.py` & `ausbildungsnachweise_utils-0.0.6/ausbildungsnachweise_utils/processor.py`

 * *Files identical despite different names*

### Comparing `ausbildungsnachweise_utils-0.0.5/setup.py` & `ausbildungsnachweise_utils-0.0.6/setup.py`

 * *Files identical despite different names*

