# Comparing `tmp/tastytrade-api-1.1.0.tar.gz` & `tmp/tastytrade-api-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tastytrade-api-1.1.0.tar", last modified: Mon May  1 11:02:00 2023, max compression
+gzip compressed data, was "tastytrade-api-1.1.2.tar", last modified: Wed May  3 18:06:28 2023, max compression
```

## Comparing `tastytrade-api-1.1.0.tar` & `tastytrade-api-1.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.236732 tastytrade-api-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-01 11:02:00.236732 tastytrade-api-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 11:02:00.236732 tastytrade-api-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.232732 tastytrade-api-1.1.0/tastytrade_api/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.232732 tastytrade-api-1.1.0/tastytrade_api/account/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/account/account_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/account/balances_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/account/watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.232732 tastytrade-api-1.1.0/tastytrade_api/market_data/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/market_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/market_data/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/market_data/market_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.236732 tastytrade-api-1.1.0/tastytrade_api/streamer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/streamer/dx_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/streamer/dxfeed_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/streamer/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tastytrade_api/symbology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.232732 tastytrade-api-1.1.0/tastytrade_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-01 11:02:00.000000 tastytrade-api-1.1.0/tastytrade_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-01 11:02:00.000000 tastytrade-api-1.1.0/tastytrade_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 11:02:00.000000 tastytrade-api-1.1.0/tastytrade_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-01 11:02:00.000000 tastytrade-api-1.1.0/tastytrade_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 11:02:00.000000 tastytrade-api-1.1.0/tastytrade_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:02:00.236732 tastytrade-api-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-01 11:01:34.000000 tastytrade-api-1.1.0/tests/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:06:28.899873 tastytrade-api-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-03 18:06:28.899873 tastytrade-api-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 18:06:28.899873 tastytrade-api-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:06:28.895873 tastytrade-api-1.1.2/tastytrade_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:06:28.895873 tastytrade-api-1.1.2/tastytrade_api/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/account/account_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/account/balances_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/account/watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:06:28.899873 tastytrade-api-1.1.2/tastytrade_api/market_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/market_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/market_data/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/market_data/market_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:06:28.899873 tastytrade-api-1.1.2/tastytrade_api/streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/streamer/dx_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/streamer/dxfeed_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/streamer/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tastytrade_api/symbology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:06:28.895873 tastytrade-api-1.1.2/tastytrade_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-03 18:06:28.000000 tastytrade-api-1.1.2/tastytrade_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-03 18:06:28.000000 tastytrade-api-1.1.2/tastytrade_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:06:28.000000 tastytrade-api-1.1.2/tastytrade_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 18:06:28.000000 tastytrade-api-1.1.2/tastytrade_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 18:06:28.000000 tastytrade-api-1.1.2/tastytrade_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:06:28.899873 tastytrade-api-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-03 18:06:04.000000 tastytrade-api-1.1.2/tests/test_authentication.py
```

### Comparing `tastytrade-api-1.1.0/PKG-INFO` & `tastytrade-api-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 1.1.0
+Version: 1.1.2
 Summary: A Python client and SDK for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tastytrade-api-1.1.0/README.md` & `tastytrade-api-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.1.0/setup.py` & `tastytrade-api-1.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tastytrade-api",
-    version="1.1.0",
+    version="1.1.2",
     author="Peter Oroszvari",
     author_email="peter@oroszvari.hu",
     description="A Python client and SDK for the Tastytrade API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peter-oroszvari/tastytrade-api",
     packages=find_packages(),
```

### Comparing `tastytrade-api-1.1.0/tastytrade_api/account/account_handler.py` & `tastytrade-api-1.1.2/tastytrade_api/account/account_handler.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.1.0/tastytrade_api/account/balances_positions.py` & `tastytrade-api-1.1.2/tastytrade_api/account/balances_positions.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.1.0/tastytrade_api/account/watchlist.py` & `tastytrade-api-1.1.2/tastytrade_api/account/watchlist.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.1.0/tastytrade_api/authentication.py` & `tastytrade-api-1.1.2/tastytrade_api/authentication.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.1.0/tastytrade_api/market_data/instruments.py` & `tastytrade-api-1.1.2/tastytrade_api/market_data/instruments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import requests
 import json
-from typing import List
+from typing import List, Dict, Any
 import urllib
-
 class TastytradeInstruments:
     """
     Implements the Tastytrade Instruments API - https://developer.tastytrade.com/open-api-spec/instruments/
     """
 
     def __init__(self, session_token: str, api_url: str):
         self.session_token = session_token
@@ -382,15 +381,33 @@
     TBD: /instruments/warrants and /instruments/warrants/{symbol}
     Returns a set of warrant definitions that can be filtered by parameters
     """
     
     """
     TBD: Future options chanins and option chains implementation
     """
+    def get_option_chains(self, symbol: str):
+        """
+        Returns an option chain given an underlying symbol,
 
+        Args:
+            symbol (str): _description_
+        """
+        headers = {
+            "Authorization": f"{self.session_token}"
+        }
+        response = requests.get(f"{self.api_url}/option-chains/{symbol}/nested", headers=headers)     
+       
+        if response.status_code == 200:
+            response_data = json.loads(response.content)
+            option_chain = response_data["data"]["items"]
+            return option_chain
+        else:
+            raise Exception(f"Error getting symbol data for {symbol}: {response.status_code} - {response.content}")           
+        
     def get_symbol_data(self, symbol: str) -> List[Dict[str, Any]]:
         """
         Makes a GET request to the /symbols/search/{symbol} API endpoint and returns an array of symbol data.
 
         Args:
             symbol (str): The symbol to search for.
 
@@ -407,9 +424,8 @@
         response = requests.get(f"{self.api_url}/symbols/search/{symbol}", headers=headers)
 
         if response.status_code == 200:
             response_data = json.loads(response.content)
             symbol_data = response_data["data"]["items"]
             return symbol_data
         else:
-            raise Exception(f"Error getting symbol data for {symbol}: {response.status_code} - {response.content}")
-
+            raise Exception(f"Error getting symbol data for {symbol}: {response.status_code} - {response.content}")
```

### Comparing `tastytrade-api-1.1.0/tastytrade_api/market_data/market_metrics.py` & `tastytrade-api-1.1.2/tastytrade_api/market_data/market_metrics.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.1.0/tastytrade_api/streamer/dx_mapping.py` & `tastytrade-api-1.1.2/tastytrade_api/streamer/dx_mapping.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.1.0/tastytrade_api/streamer/dxfeed_handler.py` & `tastytrade-api-1.1.2/tastytrade_api/streamer/dxfeed_handler.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.1.0/tastytrade_api/streamer/streamer.py` & `tastytrade-api-1.1.2/tastytrade_api/streamer/streamer.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.1.0/tastytrade_api/symbology.py` & `tastytrade-api-1.1.2/tastytrade_api/symbology.py`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.1.0/tastytrade_api.egg-info/PKG-INFO` & `tastytrade-api-1.1.2/tastytrade_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tastytrade-api
-Version: 1.1.0
+Version: 1.1.2
 Summary: A Python client and SDK for the Tastytrade API
 Home-page: https://github.com/peter-oroszvari/tastytrade-api
 Author: Peter Oroszvari
 Author-email: peter@oroszvari.hu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tastytrade-api-1.1.0/tastytrade_api.egg-info/SOURCES.txt` & `tastytrade-api-1.1.2/tastytrade_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tastytrade-api-1.1.0/tests/test_authentication.py` & `tastytrade-api-1.1.2/tests/test_authentication.py`

 * *Files identical despite different names*

