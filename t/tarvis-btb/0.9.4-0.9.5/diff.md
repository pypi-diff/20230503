# Comparing `tmp/tarvis-btb-0.9.4.tar.gz` & `tmp/tarvis-btb-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-btb-0.9.4.tar", last modified: Fri Apr 28 10:06:27 2023, max compression
+gzip compressed data, was "tarvis-btb-0.9.5.tar", last modified: Wed May  3 01:30:57 2023, max compression
```

## Comparing `tarvis-btb-0.9.4.tar` & `tarvis-btb-0.9.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:06:27.515576 tarvis-btb-0.9.4/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-28 10:06:15.000000 tarvis-btb-0.9.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      397 2023-04-28 10:06:27.515576 tarvis-btb-0.9.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-28 10:06:15.000000 tarvis-btb-0.9.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 10:06:27.515576 tarvis-btb-0.9.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      759 2023-04-28 10:06:15.000000 tarvis-btb-0.9.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:06:27.511576 tarvis-btb-0.9.4/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:06:27.511576 tarvis-btb-0.9.4/tarvis/btb/
--rw-r--r--   0 root         (0) root         (0)      118 2023-04-28 10:06:15.000000 tarvis-btb-0.9.4/tarvis/btb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24425 2023-04-28 10:06:15.000000 tarvis-btb-0.9.4/tarvis/btb/basictradingbot.py
--rw-r--r--   0 root         (0) root         (0)     3978 2023-04-28 10:06:15.000000 tarvis-btb-0.9.4/tarvis/btb/btbs.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-04-28 10:06:15.000000 tarvis-btb-0.9.4/tarvis/btb/exchangeaccount.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:06:27.511576 tarvis-btb-0.9.4/tarvis_btb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      397 2023-04-28 10:06:27.000000 tarvis-btb-0.9.4/tarvis_btb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-28 10:06:27.000000 tarvis-btb-0.9.4/tarvis_btb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 10:06:27.000000 tarvis-btb-0.9.4/tarvis_btb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 10:06:27.000000 tarvis-btb-0.9.4/tarvis_btb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 10:06:27.000000 tarvis-btb-0.9.4/tarvis_btb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:06:27.515576 tarvis-btb-0.9.4/test/
--rw-r--r--   0 root         (0) root         (0)     3152 2023-04-28 10:06:15.000000 tarvis-btb-0.9.4/test/test_all.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:30:57.638990 tarvis-btb-0.9.5/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-03 01:30:57.638990 tarvis-btb-0.9.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 01:30:57.638990 tarvis-btb-0.9.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      759 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:30:57.630989 tarvis-btb-0.9.5/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:30:57.634990 tarvis-btb-0.9.5/tarvis/btb/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/tarvis/btb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24506 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/tarvis/btb/basictradingbot.py
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/tarvis/btb/btbs.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/tarvis/btb/exchangeaccount.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:30:57.634990 tarvis-btb-0.9.5/tarvis_btb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-03 01:30:57.000000 tarvis-btb-0.9.5/tarvis_btb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2023-05-03 01:30:57.000000 tarvis-btb-0.9.5/tarvis_btb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 01:30:57.000000 tarvis-btb-0.9.5/tarvis_btb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-03 01:30:57.000000 tarvis-btb-0.9.5/tarvis_btb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 01:30:57.000000 tarvis-btb-0.9.5/tarvis_btb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 01:30:57.638990 tarvis-btb-0.9.5/test/
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-05-03 01:30:46.000000 tarvis-btb-0.9.5/test/test_all.py
```

### Comparing `tarvis-btb-0.9.4/LICENSE.txt` & `tarvis-btb-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-btb-0.9.4/setup.py` & `tarvis-btb-0.9.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-btb",
-    version="0.9.4",
+    version="0.9.5",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Basic Trading Bot Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-btb-0.9.4/tarvis/btb/basictradingbot.py` & `tarvis-btb-0.9.5/tarvis/btb/basictradingbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,17 @@
                 order_price = quote_price * price_allowance
                 order_price = trading_policy.align_price(order_price)
 
                 # Value is in quote asset price
                 base_value = base_asset_position * quote_price
                 total_value = quote_asset_position + base_value
                 available_value = total_value - account.reserve
-                if available_value > account.position_limit:
+                if (account.position_limit is not None) and (
+                    available_value > account.position_limit
+                ):
                     available_value = account.position_limit
 
                 leverage = indicator.leverage * account.leverage_multiplier
                 if leverage > account.leverage_limit:
                     leverage = account.leverage_limit
 
                 current_ratio = abs(base_value) / available_value
```

### Comparing `tarvis-btb-0.9.4/tarvis/btb/btbs.py` & `tarvis-btb-0.9.5/tarvis/btb/btbs.py`

 * *Files identical despite different names*

### Comparing `tarvis-btb-0.9.4/tarvis/btb/exchangeaccount.py` & `tarvis-btb-0.9.5/tarvis/btb/exchangeaccount.py`

 * *Files identical despite different names*

### Comparing `tarvis-btb-0.9.4/test/test_all.py` & `tarvis-btb-0.9.5/test/test_all.py`

 * *Files identical despite different names*

