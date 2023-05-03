# Comparing `tmp/currensees-1.1.0.tar.gz` & `tmp/currensees-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/currensees-1.1.0.tar", last modified: Thu Apr 27 04:02:45 2023, max compression
+gzip compressed data, was "dist/currensees-1.1.1.tar", last modified: Wed May  3 03:44:38 2023, max compression
```

## Comparing `currensees-1.1.0.tar` & `currensees-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-27 04:02:45.005945 currensees-1.1.0/
--rw-r--r--   0 finn       (501) staff       (20)     7001 2023-04-27 04:02:45.006277 currensees-1.1.0/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     3685 2023-04-27 04:01:36.000000 currensees-1.1.0/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-27 04:02:45.002859 currensees-1.1.0/currensees/
--rw-r--r--   0 finn       (501) staff       (20)      292 2023-04-20 00:30:20.000000 currensees-1.1.0/currensees/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)      908 2023-04-19 23:42:50.000000 currensees-1.1.0/currensees/auth.py
--rw-r--r--   0 finn       (501) staff       (20)      755 2023-04-22 18:24:20.000000 currensees-1.1.0/currensees/convert.py
--rw-r--r--   0 finn       (501) staff       (20)      709 2023-04-22 18:21:27.000000 currensees-1.1.0/currensees/convert_all.py
--rw-r--r--   0 finn       (501) staff       (20)     1149 2023-04-22 18:45:05.000000 currensees-1.1.0/currensees/currencies.py
--rw-r--r--   0 finn       (501) staff       (20)      493 2023-04-19 23:55:16.000000 currensees-1.1.0/currensees/daily_average.py
--rw-r--r--   0 finn       (501) staff       (20)     1261 2023-04-22 19:03:02.000000 currensees-1.1.0/currensees/historical.py
--rw-r--r--   0 finn       (501) staff       (20)     1218 2023-04-27 03:54:01.000000 currensees-1.1.0/currensees/margins_spreads.py
--rw-r--r--   0 finn       (501) staff       (20)      974 2023-04-27 03:54:25.000000 currensees-1.1.0/currensees/performances.py
--rw-r--r--   0 finn       (501) staff       (20)      939 2023-04-27 03:56:19.000000 currensees-1.1.0/currensees/signals.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-27 03:58:19.000000 currensees-1.1.0/currensees/version.py
--rw-r--r--   0 finn       (501) staff       (20)      530 2023-04-19 23:56:35.000000 currensees-1.1.0/currensees/weekly_average.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-27 04:02:45.005424 currensees-1.1.0/currensees.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     7001 2023-04-27 04:02:44.000000 currensees-1.1.0/currensees.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      528 2023-04-27 04:02:44.000000 currensees-1.1.0/currensees.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-27 04:02:44.000000 currensees-1.1.0/currensees.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-27 04:02:30.000000 currensees-1.1.0/currensees.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-27 04:02:44.000000 currensees-1.1.0/currensees.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)       11 2023-04-27 04:02:44.000000 currensees-1.1.0/currensees.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-27 04:02:45.006911 currensees-1.1.0/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2646 2023-04-27 03:58:19.000000 currensees-1.1.0/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-05-03 03:44:38.033131 currensees-1.1.1/
+-rw-r--r--   0 finn       (501) staff       (20)     7259 2023-05-03 03:44:38.033341 currensees-1.1.1/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     3887 2023-05-03 03:43:18.000000 currensees-1.1.1/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-05-03 03:44:38.029547 currensees-1.1.1/currensees/
+-rw-r--r--   0 finn       (501) staff       (20)      403 2023-05-03 03:39:30.000000 currensees-1.1.1/currensees/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)      908 2023-04-19 23:42:50.000000 currensees-1.1.1/currensees/auth.py
+-rw-r--r--   0 finn       (501) staff       (20)      755 2023-04-22 18:24:20.000000 currensees-1.1.1/currensees/convert.py
+-rw-r--r--   0 finn       (501) staff       (20)      709 2023-04-22 18:21:27.000000 currensees-1.1.1/currensees/convert_all.py
+-rw-r--r--   0 finn       (501) staff       (20)     1149 2023-04-22 18:45:05.000000 currensees-1.1.1/currensees/currencies.py
+-rw-r--r--   0 finn       (501) staff       (20)      493 2023-04-19 23:55:16.000000 currensees-1.1.1/currensees/daily_average.py
+-rw-r--r--   0 finn       (501) staff       (20)     1261 2023-04-22 19:03:02.000000 currensees-1.1.1/currensees/historical.py
+-rw-r--r--   0 finn       (501) staff       (20)     1218 2023-04-27 03:54:01.000000 currensees-1.1.1/currensees/margins_spreads.py
+-rw-r--r--   0 finn       (501) staff       (20)      516 2023-05-03 03:39:38.000000 currensees-1.1.1/currensees/monthly_average.py
+-rw-r--r--   0 finn       (501) staff       (20)      974 2023-04-27 03:54:25.000000 currensees-1.1.1/currensees/performances.py
+-rw-r--r--   0 finn       (501) staff       (20)      939 2023-04-27 03:56:19.000000 currensees-1.1.1/currensees/signals.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-05-03 03:43:45.000000 currensees-1.1.1/currensees/version.py
+-rw-r--r--   0 finn       (501) staff       (20)      530 2023-05-03 03:38:10.000000 currensees-1.1.1/currensees/weekly_average.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-05-03 03:44:38.032650 currensees-1.1.1/currensees.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     7259 2023-05-03 03:44:37.000000 currensees-1.1.1/currensees.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      558 2023-05-03 03:44:37.000000 currensees-1.1.1/currensees.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-05-03 03:44:37.000000 currensees-1.1.1/currensees.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-05-03 03:44:23.000000 currensees-1.1.1/currensees.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-05-03 03:44:37.000000 currensees-1.1.1/currensees.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)       11 2023-05-03 03:44:37.000000 currensees-1.1.1/currensees.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-05-03 03:44:38.033801 currensees-1.1.1/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2646 2023-05-03 03:43:45.000000 currensees-1.1.1/setup.py
```

### Comparing `currensees-1.1.0/PKG-INFO` & `currensees-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currensees
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python library for integrating with the Currency API.
 Home-page: https://moatsystems.com/currency-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/moatsystems/currensees_sdk/issues
 Project-URL: Changes, https://github.com/moatsystems/currensees_sdk/blob/main/CHANGELOG.md
@@ -52,14 +52,15 @@
             from currensees.auth import Auth
             from currensees.currencies import Currencies
             from currensees.historical import Historical
             from currensees.convert import Convert
             from currensees.convert_all import ConvertAll
             from currensees.daily_average import DailyAverage
             from currensees.weekly_average import WeeklyAverage
+            from currensees.monthly_average import MonthlyAverage
             from currensees.margins_spreads import MarginsSpreads
             from currensees.performances import Performances
             from currensees.signals import Signals
         
             # Authenticate and log in
             auth = Auth()
             username = "your_username"
@@ -96,14 +97,18 @@
             result = daily_average.get_daily_average("2023_04_19")
             print("Daily average:", result)
         
             weekly_average = WeeklyAverage(auth.headers)
             result = weekly_average.get_weekly_average("2023_04_03", "2023_04_07")
             print("Weekly average:", result)
         
+            monthly_average = MonthlyAverage(auth.headers)
+            result = monthly_average.get_monthly_average("2023", "04")
+            print("Monthly average:", result)
+        
             margins_spreads = MarginsSpreads(auth.headers)
             result = margins_spreads.get_margins_spreads(username, "19", "04", "2023")
             print("Margins and spreads:", result)
         
             uuid = "margins_spreads_uuid"
             result = margins_spreads.get_margins_spreads_currency(uuid, username, "19", "04", "2023")
             print("Margins and spreads for currency:", result)
@@ -147,15 +152,15 @@
         
         .. _BSD 3-Clause License: https://moatsystems.com/assets/license/BSD_3_Clause.txt
         
         
         Copyright
         ----------
         
-        Copyright |copy| 2023 `Moat Systems Limited`_. All Rights Reserved.
+        Copyright |copy| 2020 - 2023 `Moat Systems Limited`_. All Rights Reserved.
         
         .. |copy| unicode:: 0xA9 .. copyright sign
         .. _Moat Systems Limited: https://moatsystems.com/
         
 Keywords: currency,currency api,currensees,currensees sdk,rate,rates,exchange rates,moat,moatsystems,moat systems
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `currensees-1.1.0/README.md` & `currensees-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from currensees.auth import Auth
 from currensees.currencies import Currencies
 from currensees.historical import Historical
 from currensees.convert import Convert
 from currensees.convert_all import ConvertAll
 from currensees.daily_average import DailyAverage
 from currensees.weekly_average import WeeklyAverage
+from currensees.monthly_average import MonthlyAverage
 from currensees.margins_spreads import MarginsSpreads
 from currensees.performances import Performances
 from currensees.signals import Signals
 
 # Authenticate and log in
 auth = Auth()
 username = "your_username"
@@ -75,14 +76,18 @@
 result = daily_average.get_daily_average("2023_04_19")
 print("Daily average:", result)
 
 weekly_average = WeeklyAverage(auth.headers)
 result = weekly_average.get_weekly_average("2023_04_03", "2023_04_07")
 print("Weekly average:", result)
 
+monthly_average = MonthlyAverage(auth.headers)
+result = monthly_average.get_monthly_average("2023", "04")
+print("Monthly average:", result)
+
 margins_spreads = MarginsSpreads(auth.headers)
 result = margins_spreads.get_margins_spreads(username, "19", "04", "2023")
 print("Margins and spreads:", result)
 
 uuid = "margins_spreads_uuid"
 result = margins_spreads.get_margins_spreads_currency(uuid, username, "19", "04", "2023")
 print("Margins and spreads for currency:", result)
@@ -117,8 +122,8 @@
 ## License
 
 This project is licensed under the [BSD 3-Clause License](https://moatsystems.com/assets/license/BSD_3_Clause.txt).
 
 
 ## Copyright
 
-(c) 2023 [Moat Systems Limited](https://moatsystems.com/). All Rights Reserved.
+(c) 2020 - 2023 [Moat Systems Limited](https://moatsystems.com/). All Rights Reserved.
```

### Comparing `currensees-1.1.0/currensees/auth.py` & `currensees-1.1.1/currensees/auth.py`

 * *Files identical despite different names*

### Comparing `currensees-1.1.0/currensees/convert.py` & `currensees-1.1.1/currensees/convert.py`

 * *Files identical despite different names*

### Comparing `currensees-1.1.0/currensees/convert_all.py` & `currensees-1.1.1/currensees/convert_all.py`

 * *Files identical despite different names*

### Comparing `currensees-1.1.0/currensees/currencies.py` & `currensees-1.1.1/currensees/currencies.py`

 * *Files identical despite different names*

### Comparing `currensees-1.1.0/currensees/historical.py` & `currensees-1.1.1/currensees/historical.py`

 * *Files identical despite different names*

### Comparing `currensees-1.1.0/currensees/margins_spreads.py` & `currensees-1.1.1/currensees/margins_spreads.py`

 * *Files identical despite different names*

### Comparing `currensees-1.1.0/currensees/performances.py` & `currensees-1.1.1/currensees/performances.py`

 * *Files identical despite different names*

### Comparing `currensees-1.1.0/currensees/signals.py` & `currensees-1.1.1/currensees/signals.py`

 * *Files identical despite different names*

### Comparing `currensees-1.1.0/currensees/weekly_average.py` & `currensees-1.1.1/currensees/weekly_average.py`

 * *Files identical despite different names*

### Comparing `currensees-1.1.0/currensees.egg-info/PKG-INFO` & `currensees-1.1.1/currensees.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: currensees
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python library for integrating with the Currency API.
 Home-page: https://moatsystems.com/currency-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/moatsystems/currensees_sdk/issues
 Project-URL: Changes, https://github.com/moatsystems/currensees_sdk/blob/main/CHANGELOG.md
@@ -52,14 +52,15 @@
             from currensees.auth import Auth
             from currensees.currencies import Currencies
             from currensees.historical import Historical
             from currensees.convert import Convert
             from currensees.convert_all import ConvertAll
             from currensees.daily_average import DailyAverage
             from currensees.weekly_average import WeeklyAverage
+            from currensees.monthly_average import MonthlyAverage
             from currensees.margins_spreads import MarginsSpreads
             from currensees.performances import Performances
             from currensees.signals import Signals
         
             # Authenticate and log in
             auth = Auth()
             username = "your_username"
@@ -96,14 +97,18 @@
             result = daily_average.get_daily_average("2023_04_19")
             print("Daily average:", result)
         
             weekly_average = WeeklyAverage(auth.headers)
             result = weekly_average.get_weekly_average("2023_04_03", "2023_04_07")
             print("Weekly average:", result)
         
+            monthly_average = MonthlyAverage(auth.headers)
+            result = monthly_average.get_monthly_average("2023", "04")
+            print("Monthly average:", result)
+        
             margins_spreads = MarginsSpreads(auth.headers)
             result = margins_spreads.get_margins_spreads(username, "19", "04", "2023")
             print("Margins and spreads:", result)
         
             uuid = "margins_spreads_uuid"
             result = margins_spreads.get_margins_spreads_currency(uuid, username, "19", "04", "2023")
             print("Margins and spreads for currency:", result)
@@ -147,15 +152,15 @@
         
         .. _BSD 3-Clause License: https://moatsystems.com/assets/license/BSD_3_Clause.txt
         
         
         Copyright
         ----------
         
-        Copyright |copy| 2023 `Moat Systems Limited`_. All Rights Reserved.
+        Copyright |copy| 2020 - 2023 `Moat Systems Limited`_. All Rights Reserved.
         
         .. |copy| unicode:: 0xA9 .. copyright sign
         .. _Moat Systems Limited: https://moatsystems.com/
         
 Keywords: currency,currency api,currensees,currensees sdk,rate,rates,exchange rates,moat,moatsystems,moat systems
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `currensees-1.1.0/currensees.egg-info/SOURCES.txt` & `currensees-1.1.1/currensees.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 currensees/auth.py
 currensees/convert.py
 currensees/convert_all.py
 currensees/currencies.py
 currensees/daily_average.py
 currensees/historical.py
 currensees/margins_spreads.py
+currensees/monthly_average.py
 currensees/performances.py
 currensees/signals.py
 currensees/version.py
 currensees/weekly_average.py
 currensees.egg-info/PKG-INFO
 currensees.egg-info/SOURCES.txt
 currensees.egg-info/dependency_links.txt
```

### Comparing `currensees-1.1.0/setup.py` & `currensees-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "currensees"
-VERSION = "1.1.0"
+VERSION = "1.1.1"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

