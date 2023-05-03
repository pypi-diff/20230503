# Comparing `tmp/wombato-0.0.3.tar.gz` & `tmp/wombato-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Prashant\Desktop\wombato\dist\.tmp-05_kmjzu\wombato-0.0.3.tar", last modified: Mon May  1 13:12:24 2023, max compression
+gzip compressed data, was "C:\Users\Prashant\Desktop\wombato\dist\.tmp-0l3qx5b_\wombato-0.0.4.tar", last modified: Wed May  3 03:01:00 2023, max compression
```

## Comparing `wombato-0.0.3.tar` & `wombato-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 13:12:24.000000 wombato-0.0.3/
--rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombato-0.0.3/LICENSE.md
--rw-rw-rw-   0        0        0      545 2023-05-01 13:12:24.000000 wombato-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-05-01 13:09:37.000000 wombato-0.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-05-01 06:27:55.000000 wombato-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      760 2023-05-01 13:12:24.000000 wombato-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 13:12:24.000000 wombato-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 13:12:24.000000 wombato-0.0.3/src/wombato.egg-info/
--rw-rw-rw-   0        0        0      545 2023-05-01 13:12:24.000000 wombato-0.0.3/src/wombato.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-05-01 13:12:24.000000 wombato-0.0.3/src/wombato.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 13:12:24.000000 wombato-0.0.3/src/wombato.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 13:12:24.000000 wombato-0.0.3/src/wombato.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 03:01:00.000000 wombato-0.0.4/
+-rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombato-0.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0      529 2023-05-03 03:01:00.000000 wombato-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-05-01 13:09:37.000000 wombato-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 03:01:00.000000 wombato-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-05-03 03:00:07.000000 wombato-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:01:00.000000 wombato-0.0.4/src/
+-rw-rw-rw-   0        0        0        0 2023-05-01 07:27:57.000000 wombato-0.0.4/src/__init__.py
+-rw-rw-rw-   0        0        0     9596 2023-05-01 13:07:41.000000 wombato-0.0.4/src/wombato.py
+drwxrwxrwx   0        0        0        0 2023-05-03 03:01:00.000000 wombato-0.0.4/wombato.egg-info/
+-rw-rw-rw-   0        0        0      529 2023-05-03 03:01:00.000000 wombato-0.0.4/wombato.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-03 03:01:00.000000 wombato-0.0.4/wombato.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 03:01:00.000000 wombato-0.0.4/wombato.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-03 03:01:00.000000 wombato-0.0.4/wombato.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-03 03:01:00.000000 wombato-0.0.4/wombato.egg-info/top_level.txt
```

### Comparing `wombato-0.0.3/LICENSE.md` & `wombato-0.0.4/LICENSE.md`

 * *Files identical despite different names*

