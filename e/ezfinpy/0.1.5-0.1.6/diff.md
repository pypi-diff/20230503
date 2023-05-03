# Comparing `tmp/ezfinpy-0.1.5.tar.gz` & `tmp/ezfinpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezfinpy-0.1.5.tar", max compression
+gzip compressed data, was "ezfinpy-0.1.6.tar", max compression
```

## Comparing `ezfinpy-0.1.5.tar` & `ezfinpy-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       58 2023-05-03 13:44:56.989117 ezfinpy-0.1.5/ezfinpy/__init__.py
--rw-r--r--   0        0        0     3767 2023-05-03 16:50:20.885300 ezfinpy-0.1.5/ezfinpy/pandas_patcher.py
--rw-r--r--   0        0        0     5237 2023-05-03 01:02:34.155525 ezfinpy-0.1.5/ezfinpy/simulator.py
--rw-r--r--   0        0        0     4163 2023-05-03 16:51:05.514636 ezfinpy-0.1.5/ezfinpy/stats.py
--rw-r--r--   0        0        0      668 2023-05-03 14:57:21.483060 ezfinpy-0.1.5/ezfinpy/utils.py
--rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 ezfinpy-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0      486 2023-05-03 16:51:51.391257 ezfinpy-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 00:20:52.359673 ezfinpy-0.1.5/README.md
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 ezfinpy-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-05-03 13:44:56.989117 ezfinpy-0.1.6/ezfinpy/__init__.py
+-rw-r--r--   0        0        0     3767 2023-05-03 16:50:20.885300 ezfinpy-0.1.6/ezfinpy/pandas_patcher.py
+-rw-r--r--   0        0        0     5237 2023-05-03 01:02:34.155525 ezfinpy-0.1.6/ezfinpy/simulator.py
+-rw-r--r--   0        0        0     4161 2023-05-03 19:10:56.663095 ezfinpy-0.1.6/ezfinpy/stats.py
+-rw-r--r--   0        0        0      668 2023-05-03 14:57:21.483060 ezfinpy-0.1.6/ezfinpy/utils.py
+-rw-r--r--   0        0        0     1099 2023-04-08 18:19:42.889204 ezfinpy-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0      486 2023-05-03 19:11:28.150233 ezfinpy-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 00:20:52.359673 ezfinpy-0.1.6/README.md
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 ezfinpy-0.1.6/PKG-INFO
```

### Comparing `ezfinpy-0.1.5/ezfinpy/pandas_patcher.py` & `ezfinpy-0.1.6/ezfinpy/pandas_patcher.py`

 * *Files identical despite different names*

### Comparing `ezfinpy-0.1.5/ezfinpy/simulator.py` & `ezfinpy-0.1.6/ezfinpy/simulator.py`

 * *Files identical despite different names*

### Comparing `ezfinpy-0.1.5/ezfinpy/stats.py` & `ezfinpy-0.1.6/ezfinpy/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         self.name = prices.name
         self.start = prices.index[0]
         self.end = prices.index[-1]
 
         if self.prices.index.to_series().diff().min() == pd.Timedelta('1 days'):
             self.best_day = self.prices.pct_change().max()
-            self.worst_day = self.prices.pct_change().max()
+            self.worst_day = self.prices.pct_change().min()
         else:
             self.best_day = None
             self.worst_day = None
 
         self.best_month = self.prices.ezresample('1M').pct_change().max()
         self.worst_month = self.prices.ezresample('1M').pct_change().min()
 
@@ -74,15 +74,14 @@
         if len(prices.columns) < 2:
             raise ValueError("Number of securities not valid. Length of 'prices.columns' has to be bigger than 1.")
         
         self.prices = prices
         self.risk_free = risk_free
 
         self.group_list = [SingleStats(prices=prices[asset], risk_free=risk_free) for asset in prices.columns]
-
         self.group_stats = {}
         for single_stat in self.group_list:
             self.group_stats.update({single_stat.name: single_stat.stats})
 
 
         # generate tabulated table for the group
         tabulated_table = []
```

### Comparing `ezfinpy-0.1.5/ezfinpy/utils.py` & `ezfinpy-0.1.6/ezfinpy/utils.py`

 * *Files identical despite different names*

### Comparing `ezfinpy-0.1.5/LICENSE.txt` & `ezfinpy-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezfinpy-0.1.5/PKG-INFO` & `ezfinpy-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezfinpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Home-page: https://github.com/renanmoretto/ezfinpy
 License: MIT
 Author: renanmoretto
 Author-email: himynameisrenan@outlook.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
```

