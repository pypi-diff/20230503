# Comparing `tmp/tarvis-tradingbot-0.9.4.tar.gz` & `tmp/tarvis-tradingbot-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-tradingbot-0.9.4.tar", last modified: Fri Apr 28 10:09:39 2023, max compression
+gzip compressed data, was "tarvis-tradingbot-0.9.5.tar", last modified: Wed May  3 02:17:12 2023, max compression
```

## Comparing `tarvis-tradingbot-0.9.4.tar` & `tarvis-tradingbot-0.9.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:09:39.914528 tarvis-tradingbot-0.9.4/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-28 10:09:29.000000 tarvis-tradingbot-0.9.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      388 2023-04-28 10:09:39.914528 tarvis-tradingbot-0.9.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-28 10:09:29.000000 tarvis-tradingbot-0.9.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 10:09:39.914528 tarvis-tradingbot-0.9.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      842 2023-04-28 10:09:29.000000 tarvis-tradingbot-0.9.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:09:39.910528 tarvis-tradingbot-0.9.4/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:09:39.910528 tarvis-tradingbot-0.9.4/tarvis/tradingbot/
--rw-r--r--   0 root         (0) root         (0)      526 2023-04-28 10:09:29.000000 tarvis-tradingbot-0.9.4/tarvis/tradingbot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:09:39.910528 tarvis-tradingbot-0.9.4/tarvis_tradingbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      388 2023-04-28 10:09:39.000000 tarvis-tradingbot-0.9.4/tarvis_tradingbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-28 10:09:39.000000 tarvis-tradingbot-0.9.4/tarvis_tradingbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 10:09:39.000000 tarvis-tradingbot-0.9.4/tarvis_tradingbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-28 10:09:39.000000 tarvis-tradingbot-0.9.4/tarvis_tradingbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-28 10:09:39.000000 tarvis-tradingbot-0.9.4/tarvis_tradingbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 10:09:39.000000 tarvis-tradingbot-0.9.4/tarvis_tradingbot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:17:12.788482 tarvis-tradingbot-0.9.5/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-03 02:17:01.000000 tarvis-tradingbot-0.9.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-03 02:17:12.788482 tarvis-tradingbot-0.9.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-03 02:17:01.000000 tarvis-tradingbot-0.9.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 02:17:12.788482 tarvis-tradingbot-0.9.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      842 2023-05-03 02:17:01.000000 tarvis-tradingbot-0.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:17:12.784482 tarvis-tradingbot-0.9.5/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:17:12.788482 tarvis-tradingbot-0.9.5/tarvis/tradingbot/
+-rw-r--r--   0 root         (0) root         (0)      526 2023-05-03 02:17:01.000000 tarvis-tradingbot-0.9.5/tarvis/tradingbot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 02:17:12.788482 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-03 02:17:12.000000 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-05-03 02:17:12.000000 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 02:17:12.000000 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-03 02:17:12.000000 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-03 02:17:12.000000 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 02:17:12.000000 tarvis-tradingbot-0.9.5/tarvis_tradingbot.egg-info/top_level.txt
```

### Comparing `tarvis-tradingbot-0.9.4/LICENSE.txt` & `tarvis-tradingbot-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-tradingbot-0.9.4/setup.py` & `tarvis-tradingbot-0.9.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-tradingbot",
-    version="0.9.4",
+    version="0.9.5",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Basic Trading Bot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-tradingbot-0.9.4/tarvis/tradingbot/__init__.py` & `tarvis-tradingbot-0.9.5/tarvis/tradingbot/__init__.py`

 * *Files identical despite different names*

