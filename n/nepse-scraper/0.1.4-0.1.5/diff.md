# Comparing `tmp/nepse_scraper-0.1.4.tar.gz` & `tmp/nepse_scraper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepse_scraper-0.1.4.tar", last modified: Wed May  3 07:42:40 2023, max compression
+gzip compressed data, was "nepse_scraper-0.1.5.tar", last modified: Wed May  3 11:29:14 2023, max compression
```

## Comparing `nepse_scraper-0.1.4.tar` & `nepse_scraper-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 07:42:40.264432 nepse_scraper-0.1.4/
--rw-rw-rw-   0        0        0     1089 2023-05-03 03:10:57.000000 nepse_scraper-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3155 2023-05-03 07:42:40.264432 nepse_scraper-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2479 2023-05-03 06:49:00.000000 nepse_scraper-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 07:42:40.242416 nepse_scraper-0.1.4/nepse_scraper/
--rw-rw-rw-   0        0        0    23862 2023-05-03 07:36:05.000000 nepse_scraper-0.1.4/nepse_scraper/Scraper.py
--rw-rw-rw-   0        0        0       50 2023-05-03 06:38:36.000000 nepse_scraper-0.1.4/nepse_scraper/__init__.py
--rw-rw-rw-   0        0        0     1572 2023-05-03 06:36:54.000000 nepse_scraper-0.1.4/nepse_scraper/apis.py
--rw-rw-rw-   0        0        0     5032 2023-05-01 16:07:59.000000 nepse_scraper-0.1.4/nepse_scraper/nepse.wasm
-drwxrwxrwx   0        0        0        0 2023-05-03 07:42:40.250795 nepse_scraper-0.1.4/nepse_scraper.egg-info/
--rw-rw-rw-   0        0        0     3155 2023-05-03 07:42:40.000000 nepse_scraper-0.1.4/nepse_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-05-03 07:42:40.000000 nepse_scraper-0.1.4/nepse_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 07:42:40.000000 nepse_scraper-0.1.4/nepse_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-03 07:42:40.000000 nepse_scraper-0.1.4/nepse_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-03 07:42:40.000000 nepse_scraper-0.1.4/nepse_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-03 07:42:40.264432 nepse_scraper-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1182 2023-05-03 07:42:29.000000 nepse_scraper-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:29:14.969710 nepse_scraper-0.1.5/
+-rw-rw-rw-   0        0        0     1085 2023-05-03 09:07:21.000000 nepse_scraper-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     3186 2023-05-03 11:29:14.969710 nepse_scraper-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2510 2023-05-03 11:26:57.000000 nepse_scraper-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 11:29:14.923796 nepse_scraper-0.1.5/nepse_scraper/
+-rw-rw-rw-   0        0        0    25306 2023-05-03 11:01:38.000000 nepse_scraper-0.1.5/nepse_scraper/Scraper.py
+-rw-rw-rw-   0        0        0       50 2023-05-03 06:38:36.000000 nepse_scraper-0.1.5/nepse_scraper/__init__.py
+-rw-rw-rw-   0        0        0     1717 2023-05-03 11:26:30.000000 nepse_scraper-0.1.5/nepse_scraper/apis.py
+-rw-rw-rw-   0        0        0     5032 2023-05-01 16:07:59.000000 nepse_scraper-0.1.5/nepse_scraper/nepse.wasm
+drwxrwxrwx   0        0        0        0 2023-05-03 11:29:14.967702 nepse_scraper-0.1.5/nepse_scraper.egg-info/
+-rw-rw-rw-   0        0        0     3186 2023-05-03 11:29:14.000000 nepse_scraper-0.1.5/nepse_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-05-03 11:29:14.000000 nepse_scraper-0.1.5/nepse_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:29:14.000000 nepse_scraper-0.1.5/nepse_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-03 11:29:14.000000 nepse_scraper-0.1.5/nepse_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-03 11:29:14.000000 nepse_scraper-0.1.5/nepse_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-03 11:29:14.972247 nepse_scraper-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1182 2023-05-03 11:27:45.000000 nepse_scraper-0.1.5/setup.py
```

### Comparing `nepse_scraper-0.1.4/LICENSE.txt` & `nepse_scraper-0.1.5/LICENSE.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 MIT License
 
 Copyright (c) 2023 Shrawan Sunar
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy\of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `nepse_scraper-0.1.4/PKG-INFO` & `nepse_scraper-0.1.5/nepse_scraper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: nepse_scraper
-Version: 0.1.4
+Name: nepse-scraper
+Version: 0.1.5
 Summary: Python Scraper for Nepse
 Home-page: https://github.com/polymorphisma/nepse_scraper/
-Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.4.tar.gz
+Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.5.tar.gz
 Author: Shrawan Sunar
 Author-email: shrawansunar.6@gmail.com
 Keywords: python,nepse data,nepse scraper
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
@@ -46,15 +46,15 @@
 - Get Trading Average -->
 
 
 ## Installation
 
 ### Using Pip
 ```
-pip install nepse-scraper==0.1
+pip install nepse-scraper
 ```
 ### Cloning 
 
 ```
 git clone git@github.com:polymorphisma/nepse_scraper.git
 ```
 #### Downloading Dependencies
@@ -64,28 +64,28 @@
 
 _or_ 
 
 ```
 pip install requests urllib3 wasmtime retrying
 ```
 
-### Usage
+## Usage
 ```py
 from nepse_scraper import Request_module
 
 # create object from Request_module class
 request_obj = Request_module()
 
 # getting today's price from nepse
 today_price = request_obj.get_today_price()
 print(today_price)
 ```
 
 
-### All Methods
+## All Methods
 - get_news()
 - get_head_indices() 
 - get_market_summary()
 - get_sectorwise_summary()
 - get_today_price() 
 - is_trading_day()
 - get_top_gainer() 
@@ -94,14 +94,15 @@
 - get_top_transaction()
 - get_top_turnover() 
 - get_today_market_summary()
 - get_security_detail()
 - get_marketcap()
 - get_trading_average()
 - get_sector_detail()
-
+- get_live_stock()
+- is_market_open()
 
 ## License
 
 MIT
 
 **Free Software, Hell Yeah!**
```

### Comparing `nepse_scraper-0.1.4/README.md` & `nepse_scraper-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 - Get Trading Average -->
 
 
 ## Installation
 
 ### Using Pip
 ```
-pip install nepse-scraper==0.1
+pip install nepse-scraper
 ```
 ### Cloning 
 
 ```
 git clone git@github.com:polymorphisma/nepse_scraper.git
 ```
 #### Downloading Dependencies
@@ -47,28 +47,28 @@
 
 _or_ 
 
 ```
 pip install requests urllib3 wasmtime retrying
 ```
 
-### Usage
+## Usage
 ```py
 from nepse_scraper import Request_module
 
 # create object from Request_module class
 request_obj = Request_module()
 
 # getting today's price from nepse
 today_price = request_obj.get_today_price()
 print(today_price)
 ```
 
 
-### All Methods
+## All Methods
 - get_news()
 - get_head_indices() 
 - get_market_summary()
 - get_sectorwise_summary()
 - get_today_price() 
 - is_trading_day()
 - get_top_gainer() 
@@ -77,14 +77,15 @@
 - get_top_transaction()
 - get_top_turnover() 
 - get_today_market_summary()
 - get_security_detail()
 - get_marketcap()
 - get_trading_average()
 - get_sector_detail()
-
+- get_live_stock()
+- is_market_open()
 
 ## License
 
 MIT
 
 **Free Software, Hell Yeah!**
```

### Comparing `nepse_scraper-0.1.4/nepse_scraper/Scraper.py` & `nepse_scraper-0.1.5/nepse_scraper/Scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,15 +146,14 @@
                 returns the json file accured after requsting to the api
         """
         headers = {'Authorization': f'Salter {access_token[0]}', **self.headers}
 
         if payload == None:
             payload = {'id': self.parser_obj.return_payload(access_token, which=which_payload)}
 
-
         # Send the request with the given parameters
         try:
             response = requests.request(
                 method=method,
                 url=url,
                 headers=headers,
                 json=payload,
@@ -207,15 +206,15 @@
     def call_nepse_function(self, url, method,  querystring=None, payload=None):
         try:
             access_token = self.nepse_obj.get_valid_token()
             response = self.nepse_obj.return_data(url, access_token=access_token, method=method, querystring=querystring, payload=payload)
 
             if response.status_code != self.desired_status:
                 raise ValueError('Unexpected status code: {}'.format(response.status_code))
-            
+            # print(response.json())
             return response.json()
         
         except Exception as exp:
             raise ValueError('Unexpected Error: {}'.format(exp))
         
     def is_trading_day(self) -> bool:
         """
@@ -234,14 +233,37 @@
 
         date_ = response['asOf'].split('T')[0]
 
         if date_ != str(date.today()):
             return False
         
         return True
+    
+    def is_market_open(self) -> bool:
+        """
+        Check if today is a trading day on the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to determine if today is a trading day or not.
+        If today is a trading day, it returns True, otherwise it returns False.
+
+        Returns:
+            bool: True if today is a trading day, False otherwise.
+        """
+
+        api = ROOT_URL + api_dict['marketopen_api']['api']
+        method = api_dict['marketopen_api']['method']
+
+        response = self.call_nepse_function(url=api, method=method)
+
+        isOpen = response['isOpen']
+
+        if isOpen != 'OPEN':
+            return False
+        
+        return True
 
     def get_today_price(self, date_ : str = None) -> json:
         """
         Get today's trading data for from Nepal Stock Exchange (NEPSE).
 
         This method queries the NEPSE API to retrieve the trading data for the current date or a specified date.
         The data is returned as a json response.
@@ -438,15 +460,14 @@
         """
         api = ROOT_URL + api_dict['market_summary_api']['api']
         method = api_dict['market_summary_api']['method']
 
         return self.call_nepse_function(url=api, method=method)
 
     def get_security_detail(self) -> json:
-
         """
         Retrieve security detail information from the Nepal Stock Exchange (NEPSE).
 
         This method queries the NEPSE API to retrieve security detail information, which includes the
         names and codes of all listed securities on the NEPSE, along with their market prices and other
         relevant data.
 
@@ -552,8 +573,28 @@
         Returns:
             json: A json response returned by NEPSE API.
         """
         api = ROOT_URL + api_dict['sector_index_api']['api']
         method = api_dict['sector_index_api']['method']
         querystring = {"page":"0","size":"500"}
 
-        return self.call_nepse_function(url=api, method=method, querystring=querystring)
+        return self.call_nepse_function(url=api, method=method, querystring=querystring)
+    
+    def get_live_stock(self):
+        if not(self.is_market_open()):
+            raise ValueError('Market Already closed')
+        
+        api = ROOT_URL + api_dict['stock_live_api']['api']
+        method = api_dict['stock_live_api']['method']
+
+        return self.call_nepse_function(url=api, method=method, payload='stock-live')
+    
+
+    # # incomplete pyload not working
+    # def get_nepse_live(self):
+    #     if not(self.is_market_open()):
+    #         raise ValueError('Market Already closed')
+
+    #     api = ROOT_URL + api_dict['nepse_live_api']['api']
+    #     method = api_dict['nepse_live_api']['method']
+
+    #     return self.call_nepse_function(url=api, method=method, payload='sector-live')
```

### Comparing `nepse_scraper-0.1.4/nepse_scraper/apis.py` & `nepse_scraper-0.1.5/nepse_scraper/apis.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,8 +15,10 @@
     "market_summary_api":{"api":"/api/nots/market-summary", "method":"GET"},
     "security_api":{"api":"/api/nots/company/list","method":"GET"},
     "marketcap_api":{"api":"/api/nots/nepse-data/marcapbydate","method":"GET"},
     "trading_average_api":{"api":"/api/nots/nepse-data/trading-average","method":"GET"},
     "broker_api":{"api":"/api/nots/member","method":"POST"},
     "sector_api":{"api":"/api/nots/sector", "method":"GET"},
     "sector_index_api":{"api":"/api/nots/index", "method":"GET"},
+    "stock_live_api":{"api":"/api/nots/lives-market", "method":"GET"},
+    "nepse_live_api":{"api":"/api/nots/graph/index/58", "method":"POST"},
 }
```

### Comparing `nepse_scraper-0.1.4/nepse_scraper/nepse.wasm` & `nepse_scraper-0.1.5/nepse_scraper/nepse.wasm`

 * *Files identical despite different names*

### Comparing `nepse_scraper-0.1.4/nepse_scraper.egg-info/PKG-INFO` & `nepse_scraper-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: nepse-scraper
-Version: 0.1.4
+Name: nepse_scraper
+Version: 0.1.5
 Summary: Python Scraper for Nepse
 Home-page: https://github.com/polymorphisma/nepse_scraper/
-Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.4.tar.gz
+Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.5.tar.gz
 Author: Shrawan Sunar
 Author-email: shrawansunar.6@gmail.com
 Keywords: python,nepse data,nepse scraper
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
@@ -46,15 +46,15 @@
 - Get Trading Average -->
 
 
 ## Installation
 
 ### Using Pip
 ```
-pip install nepse-scraper==0.1
+pip install nepse-scraper
 ```
 ### Cloning 
 
 ```
 git clone git@github.com:polymorphisma/nepse_scraper.git
 ```
 #### Downloading Dependencies
@@ -64,28 +64,28 @@
 
 _or_ 
 
 ```
 pip install requests urllib3 wasmtime retrying
 ```
 
-### Usage
+## Usage
 ```py
 from nepse_scraper import Request_module
 
 # create object from Request_module class
 request_obj = Request_module()
 
 # getting today's price from nepse
 today_price = request_obj.get_today_price()
 print(today_price)
 ```
 
 
-### All Methods
+## All Methods
 - get_news()
 - get_head_indices() 
 - get_market_summary()
 - get_sectorwise_summary()
 - get_today_price() 
 - is_trading_day()
 - get_top_gainer() 
@@ -94,14 +94,15 @@
 - get_top_transaction()
 - get_top_turnover() 
 - get_today_market_summary()
 - get_security_detail()
 - get_marketcap()
 - get_trading_average()
 - get_sector_detail()
-
+- get_live_stock()
+- is_market_open()
 
 ## License
 
 MIT
 
 **Free Software, Hell Yeah!**
```

### Comparing `nepse_scraper-0.1.4/setup.py` & `nepse_scraper-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from os import path
 
 current_dir = path.abspath(path.dirname(__file__))
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'Python Scraper for Nepse'
 
 with open(path.join(current_dir, 'README.md'), encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 # Setting up
 setup(
@@ -19,15 +19,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     url='https://github.com/polymorphisma/nepse_scraper/',  
     install_requires=['requests','urllib3','wasmtime', 'retrying'],
     keywords=['python', 'nepse data', 'nepse scraper'],
-    download_url="https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.4.tar.gz",
+    download_url="https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.5.tar.gz",
     classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
   ],
```

