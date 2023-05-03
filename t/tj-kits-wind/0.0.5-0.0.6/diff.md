# Comparing `tmp/tj_kits_wind-0.0.5.tar.gz` & `tmp/tj_kits_wind-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tj_kits_wind-0.0.5.tar", last modified: Mon May  1 10:00:59 2023, max compression
+gzip compressed data, was "tj_kits_wind-0.0.6.tar", last modified: Wed May  3 13:23:31 2023, max compression
```

## Comparing `tj_kits_wind-0.0.5.tar` & `tj_kits_wind-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 10:00:59.445925 tj_kits_wind-0.0.5/
--rw-rw-rw-   0        0        0      261 2023-05-01 10:00:59.445925 tj_kits_wind-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1412 2023-05-01 09:45:03.000000 tj_kits_wind-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 10:00:59.445925 tj_kits_wind-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      545 2023-05-01 10:00:44.000000 tj_kits_wind-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 10:00:59.445925 tj_kits_wind-0.0.5/tj_kits_wind/
--rw-rw-rw-   0        0        0        0 2023-05-01 09:05:59.000000 tj_kits_wind-0.0.5/tj_kits_wind/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 10:00:59.445925 tj_kits_wind-0.0.5/tj_kits_wind/tj_logger/
--rw-rw-rw-   0        0        0     4003 2023-05-01 09:37:22.000000 tj_kits_wind-0.0.5/tj_kits_wind/tj_logger/LoggerFactory.py
--rw-rw-rw-   0        0        0        0 2023-05-01 07:40:58.000000 tj_kits_wind-0.0.5/tj_kits_wind/tj_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 10:00:59.445925 tj_kits_wind-0.0.5/tj_kits_wind.egg-info/
--rw-rw-rw-   0        0        0      261 2023-05-01 10:00:59.000000 tj_kits_wind-0.0.5/tj_kits_wind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-01 10:00:59.000000 tj_kits_wind-0.0.5/tj_kits_wind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 10:00:59.000000 tj_kits_wind-0.0.5/tj_kits_wind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-01 10:00:59.000000 tj_kits_wind-0.0.5/tj_kits_wind.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 13:23:31.615703 tj_kits_wind-0.0.6/
+-rw-rw-rw-   0        0        0      261 2023-05-03 13:23:31.615703 tj_kits_wind-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1412 2023-05-01 09:45:03.000000 tj_kits_wind-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 13:23:31.615703 tj_kits_wind-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      545 2023-05-03 13:23:15.000000 tj_kits_wind-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:23:31.612713 tj_kits_wind-0.0.6/tj_kits_wind/
+-rw-rw-rw-   0        0        0        0 2023-05-01 09:05:59.000000 tj_kits_wind-0.0.6/tj_kits_wind/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:23:31.614706 tj_kits_wind-0.0.6/tj_kits_wind/tj_logger/
+-rw-rw-rw-   0        0        0     4048 2023-05-03 13:23:02.000000 tj_kits_wind-0.0.6/tj_kits_wind/tj_logger/LoggerFactory.py
+-rw-rw-rw-   0        0        0        0 2023-05-01 07:40:58.000000 tj_kits_wind-0.0.6/tj_kits_wind/tj_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 13:23:31.614706 tj_kits_wind-0.0.6/tj_kits_wind.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-05-03 13:23:31.000000 tj_kits_wind-0.0.6/tj_kits_wind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-03 13:23:31.000000 tj_kits_wind-0.0.6/tj_kits_wind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 13:23:31.000000 tj_kits_wind-0.0.6/tj_kits_wind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 13:23:31.000000 tj_kits_wind-0.0.6/tj_kits_wind.egg-info/top_level.txt
```

### Comparing `tj_kits_wind-0.0.5/README.md` & `tj_kits_wind-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tj_kits_wind-0.0.5/setup.py` & `tj_kits_wind-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Some Kits'
 
 setup(
     name="tj_kits_wind",
     version=VERSION,
     author="tjno-1",
     author_email="tjno-1@qq.com",
```

### Comparing `tj_kits_wind-0.0.5/tj_kits_wind/tj_logger/LoggerFactory.py` & `tj_kits_wind-0.0.6/tj_kits_wind/tj_logger/LoggerFactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import logging.config
 import os
 import sys
 from typing import AnyStr, Dict, Optional, Literal, Union
 
+__all__ = ["logger_console", "logger_auto"]
+
 LOGGER_FORMAT = Literal["very_short", "short", "normal", "wordy"]
 LOGGER_LEVEL = Literal['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL']
 
 
 def get_logger_conf_dict() -> Dict:
     LOGGER_CONF = {
         'version': 1,
```

