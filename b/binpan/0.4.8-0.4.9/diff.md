# Comparing `tmp/binpan-0.4.8.tar.gz` & `tmp/binpan-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\binpan-0.4.8.tar", last modified: Sun Mar 26 16:17:35 2023, max compression
+gzip compressed data, was "dist\binpan-0.4.9.tar", last modified: Sun Mar 26 16:28:21 2023, max compression
```

## Comparing `binpan-0.4.8.tar` & `binpan-0.4.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 16:17:35.000000 binpan-0.4.8/
--rw-rw-rw-   0        0        0     1096 2022-10-13 18:27:11.000000 binpan-0.4.8/LICENSE
--rw-rw-rw-   0        0        0       24 2022-10-13 18:27:11.000000 binpan-0.4.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5376 2023-03-26 16:17:35.000000 binpan-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     4887 2023-03-17 18:32:39.000000 binpan-0.4.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-26 16:17:35.000000 binpan-0.4.8/binpan/
--rw-rw-rw-   0        0        0       17 2023-02-13 19:17:30.000000 binpan-0.4.8/binpan/__init__.py
--rw-rw-rw-   0        0        0   213916 2023-03-26 16:17:21.000000 binpan-0.4.8/binpan/binpan.py
-drwxrwxrwx   0        0        0        0 2023-03-26 16:17:35.000000 binpan-0.4.8/binpan.egg-info/
--rw-rw-rw-   0        0        0     5376 2023-03-26 16:17:35.000000 binpan-0.4.8/binpan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1072 2023-03-26 16:17:35.000000 binpan-0.4.8/binpan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 16:17:35.000000 binpan-0.4.8/binpan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      196 2023-03-26 16:17:35.000000 binpan-0.4.8/binpan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-26 16:17:35.000000 binpan-0.4.8/binpan.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-26 16:17:35.000000 binpan-0.4.8/handlers/
--rw-rw-rw-   0        0        0      439 2023-03-17 18:32:39.000000 binpan-0.4.8/handlers/__init__.py
--rw-rw-rw-   0        0        0    26194 2023-03-26 15:05:30.000000 binpan-0.4.8/handlers/aggregations.py
--rw-rw-rw-   0        0        0     4361 2023-02-13 19:33:04.000000 binpan-0.4.8/handlers/exceptions.py
--rw-rw-rw-   0        0        0    48925 2023-03-17 18:52:06.000000 binpan-0.4.8/handlers/exchange.py
--rw-rw-rw-   0        0        0     7920 2022-10-22 12:47:37.000000 binpan-0.4.8/handlers/files.py
--rw-rw-rw-   0        0        0    16022 2022-11-27 19:14:53.000000 binpan-0.4.8/handlers/indicators.py
--rw-rw-rw-   0        0        0     2233 2023-02-13 19:33:04.000000 binpan-0.4.8/handlers/logs.py
--rw-rw-rw-   0        0        0    67823 2023-03-26 16:17:21.000000 binpan-0.4.8/handlers/market.py
--rw-rw-rw-   0        0        0    10402 2023-02-13 19:33:04.000000 binpan-0.4.8/handlers/messages.py
--rw-rw-rw-   0        0        0    70093 2023-02-21 18:59:02.000000 binpan-0.4.8/handlers/plotting.py
--rw-rw-rw-   0        0        0    20816 2023-02-13 15:45:20.000000 binpan-0.4.8/handlers/quest.py
--rw-rw-rw-   0        0        0    31707 2022-11-06 19:25:21.000000 binpan-0.4.8/handlers/redis_fetch.py
--rw-rw-rw-   0        0        0     4653 2023-03-17 18:52:06.000000 binpan-0.4.8/handlers/starters.py
--rw-rw-rw-   0        0        0     7182 2023-03-26 15:05:30.000000 binpan-0.4.8/handlers/stat_tests.py
--rw-rw-rw-   0        0        0     1297 2022-10-22 12:47:37.000000 binpan-0.4.8/handlers/strategies.py
--rw-rw-rw-   0        0        0    35754 2022-10-30 08:49:31.000000 binpan-0.4.8/handlers/tags.py
--rw-rw-rw-   0        0        0    13233 2023-03-26 15:05:30.000000 binpan-0.4.8/handlers/time_helper.py
--rw-rw-rw-   0        0        0    45477 2022-10-22 12:47:37.000000 binpan-0.4.8/handlers/wallet.py
--rw-rw-rw-   0        0        0      234 2023-03-26 15:10:38.000000 binpan-0.4.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-26 16:17:35.000000 binpan-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-03-26 16:17:21.000000 binpan-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-26 16:28:21.000000 binpan-0.4.9/
+-rw-rw-rw-   0        0        0     1096 2022-10-13 18:27:11.000000 binpan-0.4.9/LICENSE
+-rw-rw-rw-   0        0        0       24 2022-10-13 18:27:11.000000 binpan-0.4.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5376 2023-03-26 16:28:21.000000 binpan-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4887 2023-03-17 18:32:39.000000 binpan-0.4.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-26 16:28:21.000000 binpan-0.4.9/binpan/
+-rw-rw-rw-   0        0        0       17 2023-02-13 19:17:30.000000 binpan-0.4.9/binpan/__init__.py
+-rw-rw-rw-   0        0        0   213916 2023-03-26 16:28:02.000000 binpan-0.4.9/binpan/binpan.py
+drwxrwxrwx   0        0        0        0 2023-03-26 16:28:21.000000 binpan-0.4.9/binpan.egg-info/
+-rw-rw-rw-   0        0        0     5376 2023-03-26 16:28:21.000000 binpan-0.4.9/binpan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1072 2023-03-26 16:28:21.000000 binpan-0.4.9/binpan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-26 16:28:21.000000 binpan-0.4.9/binpan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      196 2023-03-26 16:28:21.000000 binpan-0.4.9/binpan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-03-26 16:28:21.000000 binpan-0.4.9/binpan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-26 16:28:21.000000 binpan-0.4.9/handlers/
+-rw-rw-rw-   0        0        0      439 2023-03-17 18:32:39.000000 binpan-0.4.9/handlers/__init__.py
+-rw-rw-rw-   0        0        0    26194 2023-03-26 15:05:30.000000 binpan-0.4.9/handlers/aggregations.py
+-rw-rw-rw-   0        0        0     4361 2023-02-13 19:33:04.000000 binpan-0.4.9/handlers/exceptions.py
+-rw-rw-rw-   0        0        0    48925 2023-03-17 18:52:06.000000 binpan-0.4.9/handlers/exchange.py
+-rw-rw-rw-   0        0        0     7920 2022-10-22 12:47:37.000000 binpan-0.4.9/handlers/files.py
+-rw-rw-rw-   0        0        0    16022 2022-11-27 19:14:53.000000 binpan-0.4.9/handlers/indicators.py
+-rw-rw-rw-   0        0        0     2233 2023-02-13 19:33:04.000000 binpan-0.4.9/handlers/logs.py
+-rw-rw-rw-   0        0        0    67701 2023-03-26 16:27:22.000000 binpan-0.4.9/handlers/market.py
+-rw-rw-rw-   0        0        0    10402 2023-02-13 19:33:04.000000 binpan-0.4.9/handlers/messages.py
+-rw-rw-rw-   0        0        0    70093 2023-02-21 18:59:02.000000 binpan-0.4.9/handlers/plotting.py
+-rw-rw-rw-   0        0        0    20816 2023-02-13 15:45:20.000000 binpan-0.4.9/handlers/quest.py
+-rw-rw-rw-   0        0        0    31707 2022-11-06 19:25:21.000000 binpan-0.4.9/handlers/redis_fetch.py
+-rw-rw-rw-   0        0        0     4653 2023-03-17 18:52:06.000000 binpan-0.4.9/handlers/starters.py
+-rw-rw-rw-   0        0        0     7182 2023-03-26 15:05:30.000000 binpan-0.4.9/handlers/stat_tests.py
+-rw-rw-rw-   0        0        0     1297 2022-10-22 12:47:37.000000 binpan-0.4.9/handlers/strategies.py
+-rw-rw-rw-   0        0        0    35754 2022-10-30 08:49:31.000000 binpan-0.4.9/handlers/tags.py
+-rw-rw-rw-   0        0        0    13233 2023-03-26 15:05:30.000000 binpan-0.4.9/handlers/time_helper.py
+-rw-rw-rw-   0        0        0    45477 2022-10-22 12:47:37.000000 binpan-0.4.9/handlers/wallet.py
+-rw-rw-rw-   0        0        0      234 2023-03-26 15:10:38.000000 binpan-0.4.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-03-26 16:28:21.000000 binpan-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-03-26 16:28:02.000000 binpan-0.4.9/setup.py
```

### Comparing `binpan-0.4.8/LICENSE` & `binpan-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/PKG-INFO` & `binpan-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binpan
-Version: 0.4.8
+Version: 0.4.9
 Summary: Binance API wrapper with backtesting tools.
 Home-page: https://github.com/nand0san/binpan_studio
 Author: Fernando Alfonso
 Author-email: hancaidolosdos@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binpan-0.4.8/README.md` & `binpan-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/binpan/binpan.py` & `binpan-0.4.9/binpan/binpan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 
 This is the main classes file.
 
 """
-__version__ = "0.4.8"
+__version__ = "0.4.9"
 
 import os
 from sys import path
 
 import pandas as pd
 import numpy as np
```

### Comparing `binpan-0.4.8/binpan.egg-info/PKG-INFO` & `binpan-0.4.9/binpan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binpan
-Version: 0.4.8
+Version: 0.4.9
 Summary: Binance API wrapper with backtesting tools.
 Home-page: https://github.com/nand0san/binpan_studio
 Author: Fernando Alfonso
 Author-email: hancaidolosdos@hotmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `binpan-0.4.8/binpan.egg-info/SOURCES.txt` & `binpan-0.4.9/binpan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/aggregations.py` & `binpan-0.4.9/handlers/aggregations.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/exceptions.py` & `binpan-0.4.9/handlers/exceptions.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/exchange.py` & `binpan-0.4.9/handlers/exchange.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/files.py` & `binpan-0.4.9/handlers/files.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/indicators.py` & `binpan-0.4.9/handlers/indicators.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/logs.py` & `binpan-0.4.9/handlers/logs.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/market.py` & `binpan-0.4.9/handlers/market.py`

 * *Files 0% similar despite different names*

```diff
@@ -731,15 +731,14 @@
 
     trades = handlers.market.get_last_agg_trades(symbol=symbol, limit=1000)
     requests_cnt = 0
 
     # with trade ids, find start
     if start_trade_id and end_trade_id and not redis_client_trades:
         current_first_trade = trades[0]['a']
-        # while trades[0]['id'] > start_trade_id:
         while current_first_trade > start_trade_id:
             requests_cnt += 1
             market_logger.info(f"Requests to API for aggregated trades of {symbol}: {requests_cnt}")
             fetched_older_trades = handlers.market.get_aggregated_trades(symbol=symbol,
                                                                          fromId=(current_first_trade - 1000),
                                                                          limit=1000)
             trades = fetched_older_trades + trades
@@ -1031,15 +1030,14 @@
 
     trades = handlers.market.get_last_atomic_trades(symbol=symbol, limit=1000)
     requests_cnt = 0
 
     # with trade ids, find start
     if start_trade_id and end_trade_id and not redis_client_trades:
         current_first_trade = trades[0]['id']
-        # while trades[0]['id'] > start_trade_id:
         while current_first_trade > start_trade_id:
             requests_cnt += 1
             market_logger.info(f"Requests to API for atomic trades of {symbol}: {requests_cnt}")
             fetched_older_trades = handlers.market.get_atomic_trades(symbol=symbol,
                                                                      fromId=(current_first_trade - 1000),
                                                                      limit=1000)
             trades = fetched_older_trades + trades
@@ -1060,45 +1058,45 @@
 
     # with timestamps or trade ids
     if not redis_client_trades and (startTime or endTime):
         current_first_trade_time = trades[0]['time']
         current_first_trade = trades[0]['id']
 
         if startTime:
-            retry_count = 0
             while current_first_trade_time >= startTime and retry_count < retry_limit:
                 requests_cnt += 1
                 market_logger.info(f"Requests API for atomic trades STARTIME {symbol}: {requests_cnt} current_first_trade:{current_first_trade}")
                 fetched_older_trades = handlers.market.get_atomic_trades(symbol=symbol,
                                                                          fromId=current_first_trade - 1000,
                                                                          limit=1000)
                 trades = fetched_older_trades + trades
                 current_first_trade_time = trades[0]['time']
                 current_first_trade = trades[0]['id']
-                retry_count += 1
-
         if endTime:
             current_last_trade = trades[-1]['id']
             prev_last_trade = current_last_trade
             current_last_trade_time = trades[-1]['time']
             retry_count = 0
-            while current_last_trade_time <= endTime and retry_count < retry_limit:
+
+            while current_last_trade_time <= endTime:
                 requests_cnt += 1
                 market_logger.info(f"Requests API for atomic trades ENDTIME {symbol}: {requests_cnt} current_last_trade:{current_last_trade}")
                 fetched_newer_trades = handlers.market.get_atomic_trades(symbol=symbol,
                                                                          fromId=current_last_trade,
                                                                          limit=1000)
                 trades += fetched_newer_trades
                 current_last_trade = trades[-1]['id']
                 current_last_trade_time = trades[-1]['time']
                 if current_last_trade != prev_last_trade:
                     prev_last_trade = current_last_trade  # vigilando esto
                     retry_count = 0
                 else:
                     retry_count += 1
+                    if retry_count >= 3:
+                        break
 
         ret = [i for i in trades if startTime <= i['time'] <= endTime]
         return sorted(ret, key=lambda x: x['id'])
 
     # from redis
     response = []
     market_logger.info(f"Fetching atomic trades from redis server for {symbol}")
```

### Comparing `binpan-0.4.8/handlers/messages.py` & `binpan-0.4.9/handlers/messages.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/plotting.py` & `binpan-0.4.9/handlers/plotting.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/quest.py` & `binpan-0.4.9/handlers/quest.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/redis_fetch.py` & `binpan-0.4.9/handlers/redis_fetch.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/starters.py` & `binpan-0.4.9/handlers/starters.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/stat_tests.py` & `binpan-0.4.9/handlers/stat_tests.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/strategies.py` & `binpan-0.4.9/handlers/strategies.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/tags.py` & `binpan-0.4.9/handlers/tags.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/time_helper.py` & `binpan-0.4.9/handlers/time_helper.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/handlers/wallet.py` & `binpan-0.4.9/handlers/wallet.py`

 * *Files identical despite different names*

### Comparing `binpan-0.4.8/setup.py` & `binpan-0.4.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 README_TEXT = readme.read()
 readme.close()
 
 read_required = open('requirements.txt', 'r')
 REQUIRED = read_required.read()
 read_required.close()
 
-my_version = "v0.4.8"
+my_version = "v0.4.9"
 
 setup(name='binpan',
       version=my_version,
       url='https://github.com/nand0san/binpan_studio',
       license='MIT',
       install_requires=REQUIRED,
       python_requires='>=3.7.9',
```

