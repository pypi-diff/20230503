# Comparing `tmp/tarvis-common-0.9.4.tar.gz` & `tmp/tarvis-common-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-common-0.9.4.tar", last modified: Fri Apr 28 10:05:56 2023, max compression
+gzip compressed data, was "tarvis-common-0.9.5.tar", last modified: Wed May  3 01:28:13 2023, max compression
```

## Comparing `tarvis-common-0.9.4.tar` & `tarvis-common-0.9.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.716736 tarvis-common-0.9.4/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-28 10:05:45.000000 tarvis-common-0.9.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      378 2023-04-28 10:05:56.716736 tarvis-common-0.9.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-28 10:05:45.000000 tarvis-common-0.9.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 10:05:56.716736 tarvis-common-0.9.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-04-28 10:05:45.000000 tarvis-common-0.9.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.712736 tarvis-common-0.9.4/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.712736 tarvis-common-0.9.4/tarvis/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.716736 tarvis-common-0.9.4/tarvis/common/asyncio/
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-28 10:05:45.000000 tarvis-common-0.9.4/tarvis/common/asyncio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.712736 tarvis-common-0.9.4/tarvis/common/cache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.716736 tarvis-common-0.9.4/tarvis/common/cache/local/
--rw-r--r--   0 root         (0) root         (0)     3885 2023-04-28 10:05:45.000000 tarvis-common-0.9.4/tarvis/common/cache/local/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.716736 tarvis-common-0.9.4/tarvis/common/config/
--rw-r--r--   0 root         (0) root         (0)     1698 2023-04-28 10:05:45.000000 tarvis-common-0.9.4/tarvis/common/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.716736 tarvis-common-0.9.4/tarvis/common/environ/
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-28 10:05:45.000000 tarvis-common-0.9.4/tarvis/common/environ/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.716736 tarvis-common-0.9.4/tarvis/common/logging/
--rw-r--r--   0 root         (0) root         (0)     5793 2023-04-28 10:05:45.000000 tarvis-common-0.9.4/tarvis/common/logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.716736 tarvis-common-0.9.4/tarvis/common/monitoring/
--rw-r--r--   0 root         (0) root         (0)     3678 2023-04-28 10:05:45.000000 tarvis-common-0.9.4/tarvis/common/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.716736 tarvis-common-0.9.4/tarvis/common/secrets/
--rw-r--r--   0 root         (0) root         (0)     2551 2023-04-28 10:05:45.000000 tarvis-common-0.9.4/tarvis/common/secrets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.716736 tarvis-common-0.9.4/tarvis/common/time/
--rw-r--r--   0 root         (0) root         (0)     6201 2023-04-28 10:05:45.000000 tarvis-common-0.9.4/tarvis/common/time/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.716736 tarvis-common-0.9.4/tarvis/common/trading/
--rw-r--r--   0 root         (0) root         (0)     8247 2023-04-28 10:05:45.000000 tarvis-common-0.9.4/tarvis/common/trading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:05:56.716736 tarvis-common-0.9.4/tarvis_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)      378 2023-04-28 10:05:56.000000 tarvis-common-0.9.4/tarvis_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      523 2023-04-28 10:05:56.000000 tarvis-common-0.9.4/tarvis_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 10:05:56.000000 tarvis-common-0.9.4/tarvis_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      208 2023-04-28 10:05:56.000000 tarvis-common-0.9.4/tarvis_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 10:05:56.000000 tarvis-common-0.9.4/tarvis_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.963436 tarvis-common-0.9.5/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-03 01:28:13.963436 tarvis-common-0.9.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 01:28:13.963436 tarvis-common-0.9.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/asyncio/
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/asyncio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/cache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/cache/local/
+-rw-r--r--   0 root         (0) root         (0)     3885 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/cache/local/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/config/
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/environ/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/environ/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/logging/
+-rw-r--r--   0 root         (0) root         (0)     5793 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/monitoring/
+-rw-r--r--   0 root         (0) root         (0)     3678 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/secrets/
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/secrets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/time/
+-rw-r--r--   0 root         (0) root         (0)     6201 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/time/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.959435 tarvis-common-0.9.5/tarvis/common/trading/
+-rw-r--r--   0 root         (0) root         (0)     8267 2023-05-03 01:28:03.000000 tarvis-common-0.9.5/tarvis/common/trading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:28:13.963436 tarvis-common-0.9.5/tarvis_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-03 01:28:13.000000 tarvis-common-0.9.5/tarvis_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      523 2023-05-03 01:28:13.000000 tarvis-common-0.9.5/tarvis_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 01:28:13.000000 tarvis-common-0.9.5/tarvis_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      208 2023-05-03 01:28:13.000000 tarvis-common-0.9.5/tarvis_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 01:28:13.000000 tarvis-common-0.9.5/tarvis_common.egg-info/top_level.txt
```

### Comparing `tarvis-common-0.9.4/LICENSE.txt` & `tarvis-common-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.4/setup.py` & `tarvis-common-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-common",
-    version="0.9.4",
+    version="0.9.5",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Common Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-common-0.9.4/tarvis/common/asyncio/__init__.py` & `tarvis-common-0.9.5/tarvis/common/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.4/tarvis/common/cache/local/__init__.py` & `tarvis-common-0.9.5/tarvis/common/cache/local/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.4/tarvis/common/config/__init__.py` & `tarvis-common-0.9.5/tarvis/common/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.4/tarvis/common/environ/__init__.py` & `tarvis-common-0.9.5/tarvis/common/environ/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.4/tarvis/common/logging/__init__.py` & `tarvis-common-0.9.5/tarvis/common/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.4/tarvis/common/monitoring/__init__.py` & `tarvis-common-0.9.5/tarvis/common/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.4/tarvis/common/secrets/__init__.py` & `tarvis-common-0.9.5/tarvis/common/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.4/tarvis/common/time/__init__.py` & `tarvis-common-0.9.5/tarvis/common/time/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.4/tarvis/common/trading/__init__.py` & `tarvis-common-0.9.5/tarvis/common/trading/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 class OrderSide(Enum):
     BUY = 0
     SELL = 1
 
 
 class OrderType(Enum):
-    MARKET = 0
-    LIMIT = 1
-    STOP_LOSS_MARKET = 2
+    UNSUPPORTED = 0
+    MARKET = 1
+    LIMIT = 2
+    STOP_LOSS_MARKET = 3
 
 
 class MarketPosition(Enum):
     FLAT = 0
     LONG = 1
     SHORT = 2
```

### Comparing `tarvis-common-0.9.4/tarvis_common.egg-info/SOURCES.txt` & `tarvis-common-0.9.5/tarvis_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

