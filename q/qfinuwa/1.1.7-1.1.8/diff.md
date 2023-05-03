# Comparing `tmp/qfinuwa-1.1.7.tar.gz` & `tmp/qfinuwa-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfinuwa-1.1.7.tar", last modified: Wed May  3 09:24:54 2023, max compression
+gzip compressed data, was "qfinuwa-1.1.8.tar", last modified: Wed May  3 10:34:10 2023, max compression
```

## Comparing `qfinuwa-1.1.7.tar` & `qfinuwa-1.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:24:54.983450 qfinuwa-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-03 09:24:54.983450 qfinuwa-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-03 09:24:54.983450 qfinuwa-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:24:54.983450 qfinuwa-1.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:24:54.983450 qfinuwa-1.1.7/src/qfinuwa/
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/src/qfinuwa/API.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/src/qfinuwa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17211 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/src/qfinuwa/backtester.py
--rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/src/qfinuwa/indicators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:24:54.983450 qfinuwa-1.1.7/src/qfinuwa/opt/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/src/qfinuwa/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/src/qfinuwa/opt/_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/src/qfinuwa/opt/_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/src/qfinuwa/opt/_stockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/src/qfinuwa/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-03 09:24:44.000000 qfinuwa-1.1.7/src/qfinuwa/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:24:54.983450 qfinuwa-1.1.7/src/qfinuwa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-03 09:24:54.000000 qfinuwa-1.1.7/src/qfinuwa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-03 09:24:54.000000 qfinuwa-1.1.7/src/qfinuwa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:24:54.000000 qfinuwa-1.1.7/src/qfinuwa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 09:24:54.000000 qfinuwa-1.1.7/src/qfinuwa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 09:24:54.000000 qfinuwa-1.1.7/src/qfinuwa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:34:10.314473 qfinuwa-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-03 10:34:10.314473 qfinuwa-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-03 10:34:10.314473 qfinuwa-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:34:10.310473 qfinuwa-1.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:34:10.310473 qfinuwa-1.1.8/src/qfinuwa/
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/src/qfinuwa/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/src/qfinuwa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17211 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/src/qfinuwa/backtester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/src/qfinuwa/indicators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:34:10.314473 qfinuwa-1.1.8/src/qfinuwa/opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/src/qfinuwa/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/src/qfinuwa/opt/_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/src/qfinuwa/opt/_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/src/qfinuwa/opt/_stockdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/src/qfinuwa/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-03 10:33:56.000000 qfinuwa-1.1.8/src/qfinuwa/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:34:10.310473 qfinuwa-1.1.8/src/qfinuwa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-03 10:34:10.000000 qfinuwa-1.1.8/src/qfinuwa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-03 10:34:10.000000 qfinuwa-1.1.8/src/qfinuwa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:34:10.000000 qfinuwa-1.1.8/src/qfinuwa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 10:34:10.000000 qfinuwa-1.1.8/src/qfinuwa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 10:34:10.000000 qfinuwa-1.1.8/src/qfinuwa.egg-info/top_level.txt
```

### Comparing `qfinuwa-1.1.7/LICENSE.txt` & `qfinuwa-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.7/PKG-INFO` & `qfinuwa-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qfinuwa
-Version: 1.1.7
+Version: 1.1.8
 Summary: Framework for backtesting quantitative trading algorithims.
 Home-page: https://github.com/QFinUWA/algo-backtester/issues
 Author: Isaac Bergl
 Author-email: tberg644@gmail.com
 Project-URL: Bug Tracker, https://github.com/QFinUWA/algo-backtester/issues
 Project-URL: repository, https://github.com/QFinUWA/algo-backtester
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qfinuwa-1.1.7/README.md` & `qfinuwa-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.7/setup.cfg` & `qfinuwa-1.1.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = QFinUWA
-version = 1.1.7
+version = 1.1.8
 author = Isaac Bergl
 author_email = tberg644@gmail.com
 description = A backtesting framework for quantitative finance for QFIN UWA.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/QFinUWA/algo-backtester/issues
 project_urls =
```

### Comparing `qfinuwa-1.1.7/src/qfinuwa/API.py` & `qfinuwa-1.1.8/src/qfinuwa/API.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.7/src/qfinuwa/backtester.py` & `qfinuwa-1.1.8/src/qfinuwa/backtester.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.7/src/qfinuwa/indicators.py` & `qfinuwa-1.1.8/src/qfinuwa/indicators.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.7/src/qfinuwa/opt/_portfolio.py` & `qfinuwa-1.1.8/src/qfinuwa/opt/_portfolio.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 
         self._delta_limits = delta_limits
 
         self._value = {stock: [] for stock in stocks}
         self._delta = {stock: 0 for stock in stocks}   
         self._fees_paid = {stock: 0 for stock in stocks}  
+        self._capital = {stock: 0 for stock in stocks}  
 
         self._trades = []
 
         # TODO: add delta history 
 
     #---------------[Properties]-----------------#
     @property
@@ -44,15 +45,15 @@
 
     @curr_prices.setter
     def curr_prices(self, prices: dict):
         self._i += 1
         self._curr_prices = prices
 
         for s in self._stocks:
-            self._value[s].append((self._delta[s]*self._curr_prices[s], self._fees_paid[s]))
+            self._value[s].append((self._delta[s]*self._curr_prices[s] + self._capital[s], self._fees_paid[s]))
 
     #---------------[Public Methods]-----------------#
 
     def order(self, stock: str, quantity: Union[int, float]) -> bool:
         
         if abs(self._delta[stock] + quantity) > self._delta_limits[stock]:
             return False
```

### Comparing `qfinuwa-1.1.7/src/qfinuwa/opt/_result.py` & `qfinuwa-1.1.8/src/qfinuwa/opt/_result.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.7/src/qfinuwa/opt/_stockdata.py` & `qfinuwa-1.1.8/src/qfinuwa/opt/_stockdata.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.7/src/qfinuwa/plotting.py` & `qfinuwa-1.1.8/src/qfinuwa/plotting.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.7/src/qfinuwa/strategy.py` & `qfinuwa-1.1.8/src/qfinuwa/strategy.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.7/src/qfinuwa.egg-info/PKG-INFO` & `qfinuwa-1.1.8/src/qfinuwa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qfinuwa
-Version: 1.1.7
+Version: 1.1.8
 Summary: Framework for backtesting quantitative trading algorithims.
 Home-page: https://github.com/QFinUWA/algo-backtester/issues
 Author: Isaac Bergl
 Author-email: tberg644@gmail.com
 Project-URL: Bug Tracker, https://github.com/QFinUWA/algo-backtester/issues
 Project-URL: repository, https://github.com/QFinUWA/algo-backtester
 Classifier: Programming Language :: Python :: 3
```

