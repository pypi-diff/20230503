# Comparing `tmp/MT5TrdHelper-0.1.2.tar.gz` & `tmp/MT5TrdHelper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MT5TrdHelper-0.1.2.tar", last modified: Tue Mar 14 06:50:19 2023, max compression
+gzip compressed data, was "MT5TrdHelper-0.1.3.tar", last modified: Wed May  3 16:07:50 2023, max compression
```

## Comparing `MT5TrdHelper-0.1.2.tar` & `MT5TrdHelper-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 06:50:19.180573 MT5TrdHelper-0.1.2/
--rw-rw-rw-   0        0        0     1083 2022-04-03 02:45:01.000000 MT5TrdHelper-0.1.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-14 06:50:19.026481 MT5TrdHelper-0.1.2/MT5TrdHelper/
--rw-rw-rw-   0        0        0        0 2022-04-03 05:14:01.000000 MT5TrdHelper-0.1.2/MT5TrdHelper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 06:50:19.073861 MT5TrdHelper-0.1.2/MT5TrdHelper/connect/
--rw-rw-rw-   0        0        0        0 2022-04-03 05:14:26.000000 MT5TrdHelper-0.1.2/MT5TrdHelper/connect/__init__.py
--rw-rw-rw-   0        0        0     3356 2021-09-05 18:39:03.000000 MT5TrdHelper-0.1.2/MT5TrdHelper/connect/connection.py
-drwxrwxrwx   0        0        0        0 2023-03-14 06:50:19.111757 MT5TrdHelper-0.1.2/MT5TrdHelper/exchange/
--rw-rw-rw-   0        0        0      147 2022-04-03 05:38:32.000000 MT5TrdHelper-0.1.2/MT5TrdHelper/exchange/__init__.py
--rw-rw-rw-   0        0        0     4060 2022-04-03 05:53:48.000000 MT5TrdHelper-0.1.2/MT5TrdHelper/exchange/exchange_base.py
--rw-rw-rw-   0        0        0    12173 2022-04-03 06:54:34.000000 MT5TrdHelper-0.1.2/MT5TrdHelper/exchange/mt5_exchange.py
--rw-rw-rw-   0        0        0    31323 2023-03-14 06:43:37.000000 MT5TrdHelper-0.1.2/MT5TrdHelper/exchange/symbol_base.py
-drwxrwxrwx   0        0        0        0 2023-03-14 06:50:19.141044 MT5TrdHelper-0.1.2/MT5TrdHelper/helpers/
--rw-rw-rw-   0        0        0       55 2022-04-03 05:42:35.000000 MT5TrdHelper-0.1.2/MT5TrdHelper/helpers/__init__.py
--rw-rw-rw-   0        0        0      553 2023-03-14 06:46:26.000000 MT5TrdHelper-0.1.2/MT5TrdHelper/helpers/entries.py
--rw-rw-rw-   0        0        0     2554 2022-04-03 02:59:10.000000 MT5TrdHelper-0.1.2/MT5TrdHelper/helpers/help_functions.py
-drwxrwxrwx   0        0        0        0 2023-03-14 06:50:19.165614 MT5TrdHelper-0.1.2/MT5TrdHelper/trade_execution/
--rw-rw-rw-   0        0        0       22 2020-12-09 05:41:01.000000 MT5TrdHelper-0.1.2/MT5TrdHelper/trade_execution/__init__.py
--rw-rw-rw-   0        0        0    85381 2022-04-03 13:56:05.000000 MT5TrdHelper-0.1.2/MT5TrdHelper/trade_execution/trade.py
-drwxrwxrwx   0        0        0        0 2023-03-14 06:50:19.059898 MT5TrdHelper-0.1.2/MT5TrdHelper.egg-info/
--rw-rw-rw-   0        0        0      541 2023-03-14 06:50:17.000000 MT5TrdHelper-0.1.2/MT5TrdHelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-03-14 06:50:18.000000 MT5TrdHelper-0.1.2/MT5TrdHelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 06:50:17.000000 MT5TrdHelper-0.1.2/MT5TrdHelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-03-14 06:50:18.000000 MT5TrdHelper-0.1.2/MT5TrdHelper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-14 06:50:18.000000 MT5TrdHelper-0.1.2/MT5TrdHelper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      541 2023-03-14 06:50:19.177028 MT5TrdHelper-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      100 2022-04-03 02:45:01.000000 MT5TrdHelper-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-14 06:50:19.180573 MT5TrdHelper-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1033 2023-03-14 06:46:57.000000 MT5TrdHelper-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:07:50.118520 MT5TrdHelper-0.1.3/
+-rw-rw-rw-   0        0        0     1083 2022-04-03 02:45:01.000000 MT5TrdHelper-0.1.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-03 16:07:49.125166 MT5TrdHelper-0.1.3/MT5TrdHelper/
+-rw-rw-rw-   0        0        0        0 2022-04-03 05:14:01.000000 MT5TrdHelper-0.1.3/MT5TrdHelper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:07:49.216920 MT5TrdHelper-0.1.3/MT5TrdHelper/connect/
+-rw-rw-rw-   0        0        0        0 2022-04-03 05:14:26.000000 MT5TrdHelper-0.1.3/MT5TrdHelper/connect/__init__.py
+-rw-rw-rw-   0        0        0     3356 2021-09-05 18:39:03.000000 MT5TrdHelper-0.1.3/MT5TrdHelper/connect/connection.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:07:49.442320 MT5TrdHelper-0.1.3/MT5TrdHelper/exchange/
+-rw-rw-rw-   0        0        0      147 2022-04-03 05:38:32.000000 MT5TrdHelper-0.1.3/MT5TrdHelper/exchange/__init__.py
+-rw-rw-rw-   0        0        0     4060 2022-04-03 05:53:48.000000 MT5TrdHelper-0.1.3/MT5TrdHelper/exchange/exchange_base.py
+-rw-rw-rw-   0        0        0    12173 2022-04-03 06:54:34.000000 MT5TrdHelper-0.1.3/MT5TrdHelper/exchange/mt5_exchange.py
+-rw-rw-rw-   0        0        0    31610 2023-05-03 16:06:35.000000 MT5TrdHelper-0.1.3/MT5TrdHelper/exchange/symbol_base.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:07:49.565986 MT5TrdHelper-0.1.3/MT5TrdHelper/helpers/
+-rw-rw-rw-   0        0        0       55 2022-04-03 05:42:35.000000 MT5TrdHelper-0.1.3/MT5TrdHelper/helpers/__init__.py
+-rw-rw-rw-   0        0        0      553 2023-03-14 06:46:26.000000 MT5TrdHelper-0.1.3/MT5TrdHelper/helpers/entries.py
+-rw-rw-rw-   0        0        0     2554 2022-04-03 02:59:10.000000 MT5TrdHelper-0.1.3/MT5TrdHelper/helpers/help_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:07:49.689656 MT5TrdHelper-0.1.3/MT5TrdHelper/trade_execution/
+-rw-rw-rw-   0        0        0       22 2020-12-09 05:41:01.000000 MT5TrdHelper-0.1.3/MT5TrdHelper/trade_execution/__init__.py
+-rw-rw-rw-   0        0        0    85381 2022-04-03 13:56:05.000000 MT5TrdHelper-0.1.3/MT5TrdHelper/trade_execution/trade.py
+drwxrwxrwx   0        0        0        0 2023-05-03 16:07:49.175032 MT5TrdHelper-0.1.3/MT5TrdHelper.egg-info/
+-rw-rw-rw-   0        0        0      541 2023-05-03 16:07:47.000000 MT5TrdHelper-0.1.3/MT5TrdHelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-05-03 16:07:48.000000 MT5TrdHelper-0.1.3/MT5TrdHelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 16:07:47.000000 MT5TrdHelper-0.1.3/MT5TrdHelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-03 16:07:47.000000 MT5TrdHelper-0.1.3/MT5TrdHelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 16:07:47.000000 MT5TrdHelper-0.1.3/MT5TrdHelper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      541 2023-05-03 16:07:49.759482 MT5TrdHelper-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      100 2022-04-03 02:45:01.000000 MT5TrdHelper-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 16:07:50.118520 MT5TrdHelper-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1033 2023-05-03 16:07:26.000000 MT5TrdHelper-0.1.3/setup.py
```

### Comparing `MT5TrdHelper-0.1.2/LICENSE` & `MT5TrdHelper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MT5TrdHelper-0.1.2/MT5TrdHelper/connect/connection.py` & `MT5TrdHelper-0.1.3/MT5TrdHelper/connect/connection.py`

 * *Files identical despite different names*

### Comparing `MT5TrdHelper-0.1.2/MT5TrdHelper/exchange/exchange_base.py` & `MT5TrdHelper-0.1.3/MT5TrdHelper/exchange/exchange_base.py`

 * *Files identical despite different names*

### Comparing `MT5TrdHelper-0.1.2/MT5TrdHelper/exchange/mt5_exchange.py` & `MT5TrdHelper-0.1.3/MT5TrdHelper/exchange/mt5_exchange.py`

 * *Files identical despite different names*

### Comparing `MT5TrdHelper-0.1.2/MT5TrdHelper/exchange/symbol_base.py` & `MT5TrdHelper-0.1.3/MT5TrdHelper/exchange/symbol_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,14 +412,16 @@
 
                 # ! finding out account margin (MARGIN IS THE AMOUNT WILL TAKE AS LOSS WHEN OUR INITIAL STOP IS HIt)
                 margin = capital * (risk_percent / 100)
                 tick_size = self.trade_tick_value
                 # ! stop_point * p to make a normal pip for both 4 digit and 5 digit broker
                 # also with (risk_percent*0.01*account_balance)/(self.trade_contract_size *
                 #                self.trade_tick_value*stop_point*self.point * p)
+                if margin >= stop_point:
+                    tick_size = tick_size * 100
                 trade_size = (margin/(stop_point * p)) / tick_size
                 # ! to take the lowest value, as round and floor makes it higher but to stay with my risk I will reduce it to lowest ex: 0.0356 to 0.03 not 0.04
                 trade_size = float(str(trade_size)[:4])
                 if trade_size == 0:
                     if not NEED_CONFIRMATION_FOR_BUY:
                         # ! if autotrade than we will not open a position
                         return 0, 0, 0, 0
@@ -439,28 +441,33 @@
                                 stop_price = float(
                                     input("define the stop point where you want your stop loss: "))
                                 stop_point = self.price_diff_to_pips(
                                     self.bid, stop_price, convert=True)
 
                                 risk_percent = float(input(
                                     "Define a new increased risk percent, cause previous risk percent won't work for this trade: "))
+                            else:
+                                trade_size = self.volume_min
                         elif entry == Entry.Sell:
                             new_price = self.add_subtract_pips_to_price(
                                 self.ask, stop_point, add=True)
                             stop_point_agree = int(input(
                                 f"do you agree to place stop loss at: {self.normalize_price(new_price)}, enter 1 for yes: "))
 
                             if stop_point_agree != 1:
                                 stop_price = float(
                                     input("define the stop point where you want your stop loss: "))
                                 stop_point = self.price_diff_to_pips(
                                     self.ask, stop_price, convert=True)
 
                                 risk_percent = float(input(
                                     "Define a new increased risk percent, cause previous risk percent won't work for this trade: "))
+                            else:
+                                trade_size = self.volume_min
+
                     except Exception as ve:
                         print(ve.args[0])
                         print(
                             "Typed wrong, try again")
                         stop_point = old_stop_point
 
             trade_size = self.verify_volume(trade_size)
```

### Comparing `MT5TrdHelper-0.1.2/MT5TrdHelper/helpers/entries.py` & `MT5TrdHelper-0.1.3/MT5TrdHelper/helpers/entries.py`

 * *Files identical despite different names*

### Comparing `MT5TrdHelper-0.1.2/MT5TrdHelper/helpers/help_functions.py` & `MT5TrdHelper-0.1.3/MT5TrdHelper/helpers/help_functions.py`

 * *Files identical despite different names*

### Comparing `MT5TrdHelper-0.1.2/MT5TrdHelper/trade_execution/trade.py` & `MT5TrdHelper-0.1.3/MT5TrdHelper/trade_execution/trade.py`

 * *Files identical despite different names*

### Comparing `MT5TrdHelper-0.1.2/MT5TrdHelper.egg-info/PKG-INFO` & `MT5TrdHelper-0.1.3/MT5TrdHelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MT5TrdHelper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python MT5 trade helpers
 Author: Nazrul Islam
 Author-email: nazrulgithub@gmail.com
 License: UNKNOWN
 Keywords: python,mt5 python,mt5 python algotrading,forex algotrading,forex python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MT5TrdHelper-0.1.2/MT5TrdHelper.egg-info/SOURCES.txt` & `MT5TrdHelper-0.1.3/MT5TrdHelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MT5TrdHelper-0.1.2/PKG-INFO` & `MT5TrdHelper-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MT5TrdHelper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python MT5 trade helpers
 Author: Nazrul Islam
 Author-email: nazrulgithub@gmail.com
 License: UNKNOWN
 Keywords: python,mt5 python,mt5 python algotrading,forex algotrading,forex python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MT5TrdHelper-0.1.2/setup.py` & `MT5TrdHelper-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'Python MT5 trade helpers'
 LONG_DESCRIPTION = 'This package is a wrapper on Mt5 python module'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="MT5TrdHelper",
```

