# Comparing `tmp/nepse_scraper-0.1.tar.gz` & `tmp/nepse_scraper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepse_scraper-0.1.tar", last modified: Wed May  3 03:18:07 2023, max compression
+gzip compressed data, was "nepse_scraper-0.1.1.tar", last modified: Wed May  3 06:59:12 2023, max compression
```

## Comparing `nepse_scraper-0.1.tar` & `nepse_scraper-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 03:18:07.702825 nepse_scraper-0.1/
--rw-rw-rw-   0        0        0     1089 2023-05-03 03:10:57.000000 nepse_scraper-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3095 2023-05-03 03:18:07.702825 nepse_scraper-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2421 2023-05-03 03:16:54.000000 nepse_scraper-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 03:18:07.660952 nepse_scraper-0.1/nepse_scraper/
--rw-rw-rw-   0        0        0    23540 2023-05-03 02:50:40.000000 nepse_scraper-0.1/nepse_scraper/Scraper.py
--rw-rw-rw-   0        0        0       50 2023-05-02 13:54:50.000000 nepse_scraper-0.1/nepse_scraper/__init__.py
--rw-rw-rw-   0        0        0     1507 2023-05-03 02:08:20.000000 nepse_scraper-0.1/nepse_scraper/apis.py
--rw-rw-rw-   0        0        0      212 2023-05-02 09:47:27.000000 nepse_scraper-0.1/nepse_scraper/paths.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:18:07.700324 nepse_scraper-0.1/nepse_scraper.egg-info/
--rw-rw-rw-   0        0        0     3095 2023-05-03 03:18:07.000000 nepse_scraper-0.1/nepse_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-05-03 03:18:07.000000 nepse_scraper-0.1/nepse_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 03:18:07.000000 nepse_scraper-0.1/nepse_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-03 03:18:07.000000 nepse_scraper-0.1/nepse_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-03 03:18:07.000000 nepse_scraper-0.1/nepse_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-03 03:18:07.705543 nepse_scraper-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1129 2023-05-03 03:14:29.000000 nepse_scraper-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:59:12.395278 nepse_scraper-0.1.1/
+-rw-rw-rw-   0        0        0     1089 2023-05-03 03:10:57.000000 nepse_scraper-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3155 2023-05-03 06:59:12.395278 nepse_scraper-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2479 2023-05-03 06:49:00.000000 nepse_scraper-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 06:59:12.377401 nepse_scraper-0.1.1/nepse_scraper/
+-rw-rw-rw-   0        0        0    23784 2023-05-03 06:45:39.000000 nepse_scraper-0.1.1/nepse_scraper/Scraper.py
+-rw-rw-rw-   0        0        0       50 2023-05-03 06:38:36.000000 nepse_scraper-0.1.1/nepse_scraper/__init__.py
+-rw-rw-rw-   0        0        0     1572 2023-05-03 06:36:54.000000 nepse_scraper-0.1.1/nepse_scraper/apis.py
+drwxrwxrwx   0        0        0        0 2023-05-03 06:59:12.394274 nepse_scraper-0.1.1/nepse_scraper.egg-info/
+-rw-rw-rw-   0        0        0     3155 2023-05-03 06:59:12.000000 nepse_scraper-0.1.1/nepse_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-05-03 06:59:12.000000 nepse_scraper-0.1.1/nepse_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 06:59:12.000000 nepse_scraper-0.1.1/nepse_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-03 06:59:12.000000 nepse_scraper-0.1.1/nepse_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-03 06:59:12.000000 nepse_scraper-0.1.1/nepse_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-03 06:59:12.396280 nepse_scraper-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1133 2023-05-03 06:57:40.000000 nepse_scraper-0.1.1/setup.py
```

### Comparing `nepse_scraper-0.1/LICENSE.txt` & `nepse_scraper-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nepse_scraper-0.1/PKG-INFO` & `nepse_scraper-0.1.1/nepse_scraper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: nepse_scraper
-Version: 0.1
+Name: nepse-scraper
+Version: 0.1.1
 Summary: Python Scraper for Nepse
 Home-page: https://github.com/polymorphisma/nepse_scraper/
-Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.tar.gz
+Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.1.tar.gz
 Author: Shrawan Sunar
 Author-email: shrawansunar.6@gmail.com
 Keywords: python,nepse data,nepse scraper
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
@@ -43,22 +43,25 @@
 - Get Today Market Summary
 - Get Security Detail
 - Get Marketcap
 - Get Trading Average -->
 
 
 ## Installation
+
+### Using Pip
+```
+pip install nepse-scraper==0.1
+```
 ### Cloning 
 
 ```
 git clone git@github.com:polymorphisma/nepse_scraper.git
 ```
-
-
-### Downloading Dependencies
+#### Downloading Dependencies
 ```
 pip install -r requirements.txt
 ```
 
 _or_ 
 
 ```
```

### Comparing `nepse_scraper-0.1/README.md` & `nepse_scraper-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: nepse_scraper
+Version: 0.1.1
+Summary: Python Scraper for Nepse
+Home-page: https://github.com/polymorphisma/nepse_scraper/
+Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.1.tar.gz
+Author: Shrawan Sunar
+Author-email: shrawansunar.6@gmail.com
+Keywords: python,nepse data,nepse scraper
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # _NEPSE_SCRAPER_
 
 Welcome to **nepse_scraper**, the Python module that provides easy access to the Nepal Stock Exchange (NEPSE) API. With just a few lines of code, you can retrieve today's stock prices, market summary, head indices and etc to help you make better investment decisions. The code is well-documented and organized, making it easy to understand and modify for your specific use case.
 
 But that's not all! With the power of Python libraries such as **pandas**, you can quickly process the retrieved data and convert it into your desired format.
 
 **nepse_scraper** is open-source, which means you can contribute and improve the code by adding new functions to retrieve additional data, enhancing existing functions with more options, or improving the error handling and exception handling to make it more robust. Your contributions can help make **nepse_scraper** even more useful for developers and analysts who work with data from the Nepal Stock Exchange.
@@ -26,22 +43,25 @@
 - Get Today Market Summary
 - Get Security Detail
 - Get Marketcap
 - Get Trading Average -->
 
 
 ## Installation
+
+### Using Pip
+```
+pip install nepse-scraper==0.1
+```
 ### Cloning 
 
 ```
 git clone git@github.com:polymorphisma/nepse_scraper.git
 ```
-
-
-### Downloading Dependencies
+#### Downloading Dependencies
 ```
 pip install -r requirements.txt
 ```
 
 _or_ 
 
 ```
@@ -80,8 +100,8 @@
 - get_sector_detail()
 
 
 ## License
 
 MIT
 
-**Free Software, Hell Yeah!**
+**Free Software, Hell Yeah!**
```

### Comparing `nepse_scraper-0.1/nepse_scraper/Scraper.py` & `nepse_scraper-0.1.1/nepse_scraper/Scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,24 @@
 from urllib3.exceptions import InsecureRequestWarning
 from urllib3 import disable_warnings
 import time
 from wasmtime import Store,Module,Instance
 import json
 import os
 
-ROOT_DIR = os.path.dirname(os.path.abspath(__file__))
+WASM_FILE = r'nepse_scraper\nepse.wasm'
 
-import sys
-sys.path.append(ROOT_DIR)
-
-import paths
-from apis import api_dict
+from .apis import api_dict
 
 ROOT_URL = 'https://www.nepalstock.com.np'
-SLEEP_TIME = 3000 # -> wait time for every failed request(in milisecond)
-
 
 class TokenParser():
     def __init__(self):
         self.store = Store()
-        module = Module.from_file(self.store.engine, paths.wasm_file)
+        module = Module.from_file(self.store.engine, WASM_FILE)
         instance = Instance(self.store,module,[])
 
         self.cdx = instance.exports(self.store)["cdx"]
         self.rdx = instance.exports(self.store)["rdx"]
         self.bdx = instance.exports(self.store)["bdx"]
         self.ndx = instance.exports(self.store)["ndx"]
         self.mdx = instance.exports(self.store)["mdx"]
@@ -192,21 +186,24 @@
      
         return [self.token_parser.parse_token_response(token_response)[0], token_response]
     
     def return_data(self, url, access_token, method='GET', which_payload=None,  querystring = None, payload=None):
         return self.request_api(method=method, url = url, access_token = access_token, which_payload=which_payload, querystring=querystring, payload=payload)
 
 from retrying import retry
-import csv
 
 class Request_module:
+    
+    SLEEP_TIME = 3000 # -> wait time for every failed request(in milisecond)
+
     def __init__(self) -> None:
         self.nepse_obj = Nepse()
         self.desired_status = 200
 
+
     @retry(wait_fixed = SLEEP_TIME)
     def call_nepse_function(self, url, method,  querystring=None, payload=None):
         try:
             access_token = self.nepse_obj.get_valid_token()
             response = self.nepse_obj.return_data(url, access_token=access_token, method=method, querystring=querystring, payload=payload)
 
             if response.status_code != self.desired_status:
@@ -270,28 +267,25 @@
         This method reads the head indices file located at paths.headindices_path and queries the NEPSE API to retrieve
         data. The data is returned as a dictionary containing index as keys and the corresponding index data as values.
 
         Returns:
             dict: A dictionary containing the latest data for each head index, with index as keys and response as a value.
         """
         api = ROOT_URL + api_dict['head_indices_api']['api']
+        print(api)
         method = api_dict['head_indices_api']['method']
 
         querystring = {"page":"0","size":"500"}
 
         dicts = {}
 
-        with open(paths.headindices_path, 'r') as rf:
-            csv_reader = csv.reader(rf)
-
-            # skip the header row
-            next(csv_reader)
-            for row_values in csv_reader:
-                index_name = row_values[0]
-                dicts[index_name] = self.call_nepse_function(url=api + index_name, method=method, querystring=querystring)
+        sector_index = self._get_sector_index()
+        
+        for val in sector_index:
+            dicts[val['id']] = self.call_nepse_function(url=api + '/' + str(val['id']), method=method, querystring=querystring)
 
         return dicts
     
     def get_sectorwise_summary(self, date_ : str =None) -> json:
         """
         Retrieve the sector-wise summary from a given business date from the Nepal Stock Exchange (NEPSE).
 
@@ -330,15 +324,14 @@
             json: A json response returned by NEPSE API.
         """
         api = ROOT_URL + api_dict['market_summary_history_api']['api']
         method = api_dict['market_summary_history_api']['method']
 
         querystring = {"page":"0","size":"500","businessDate":date_}
 
-
         return self.call_nepse_function(url=api, method=method, querystring=querystring)
     
     def get_news(self) -> json:
         """
         Retrieve the latest news and announcements from the Nepal Stock Exchange (NEPSE).
 
         This method queries the NEPSE API to retrieve the latest news and announcements regarding listed companies.
@@ -545,7 +538,19 @@
         """
         api = ROOT_URL + api_dict['sector_api']['api']
         method = api_dict['sector_api']['method']
         querystring = {"page":"0","size":"500"}
 
         return self.call_nepse_function(url=api, method=method, querystring=querystring)
     
+    def _get_sector_index(self):
+        """
+        Retrieve idnex of all sectors listed in the NEPSE.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['sector_index_api']['api']
+        method = api_dict['sector_index_api']['method']
+        querystring = {"page":"0","size":"500"}
+
+        return self.call_nepse_function(url=api, method=method, querystring=querystring)
```

### Comparing `nepse_scraper-0.1/nepse_scraper/apis.py` & `nepse_scraper-0.1.1/nepse_scraper/apis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 api_dict = {
     "authenticate_api": {"api":"/api/authenticate/prove", "method":"GET"},
     "today_price_api": {"api":"/api/nots/nepse-data/today-price", "method":"POST"},
     "marketopen_api":{"api":"/api/nots/nepse-data/market-open", "method":"GET"},
     "refer_api":{"api":"", "method":"GET"},
-    "head_indices_api":{"api":"/api/nots/index/history/", "method":"GET"}, # -> should add index ID like https://www.nepalstock.com/api/nots/index/history/51
+    "head_indices_api":{"api":"/api/nots/index/history", "method":"GET"}, # -> should add index ID like https://www.nepalstock.com/api/nots/index/history/51
     "sectorwise_summary_api": {"api":"/api/nots/sectorwise", "method":"GET"},
     "market_summary_history_api": {"api":"/api/nots/market-summary-history", "method":"GET"},
     "disclosure":{"api":"/api/nots/news/companies/disclosure", "method":"GET"},
     "top_gainer":{"api":"/api/nots/top-ten/top-gainer", "method":"GET"},
     "top_loser":{"api":"/api/nots/top-ten/top-loser", "method":"GET"},
     "top_turnover":{"api":"/api/nots/top-ten/turnover", "method":"GET"},
     "top_trade":{"api":"/api/nots/top-ten/trade", "method":"GET"},
     "top_transaction":{"api":"/api/nots/top-ten/transaction", "method":"GET"},
     "market_summary_api":{"api":"/api/nots/market-summary", "method":"GET"},
     "security_api":{"api":"/api/nots/company/list","method":"GET"},
     "marketcap_api":{"api":"/api/nots/nepse-data/marcapbydate","method":"GET"},
     "trading_average_api":{"api":"/api/nots/nepse-data/trading-average","method":"GET"},
     "broker_api":{"api":"/api/nots/member","method":"POST"},
     "sector_api":{"api":"/api/nots/sector", "method":"GET"},
+    "sector_index_api":{"api":"/api/nots/index", "method":"GET"},
 }
```

### Comparing `nepse_scraper-0.1/nepse_scraper.egg-info/PKG-INFO` & `nepse_scraper-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: nepse-scraper
-Version: 0.1
-Summary: Python Scraper for Nepse
-Home-page: https://github.com/polymorphisma/nepse_scraper/
-Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.tar.gz
-Author: Shrawan Sunar
-Author-email: shrawansunar.6@gmail.com
-Keywords: python,nepse data,nepse scraper
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # _NEPSE_SCRAPER_
 
 Welcome to **nepse_scraper**, the Python module that provides easy access to the Nepal Stock Exchange (NEPSE) API. With just a few lines of code, you can retrieve today's stock prices, market summary, head indices and etc to help you make better investment decisions. The code is well-documented and organized, making it easy to understand and modify for your specific use case.
 
 But that's not all! With the power of Python libraries such as **pandas**, you can quickly process the retrieved data and convert it into your desired format.
 
 **nepse_scraper** is open-source, which means you can contribute and improve the code by adding new functions to retrieve additional data, enhancing existing functions with more options, or improving the error handling and exception handling to make it more robust. Your contributions can help make **nepse_scraper** even more useful for developers and analysts who work with data from the Nepal Stock Exchange.
@@ -43,22 +26,25 @@
 - Get Today Market Summary
 - Get Security Detail
 - Get Marketcap
 - Get Trading Average -->
 
 
 ## Installation
+
+### Using Pip
+```
+pip install nepse-scraper==0.1
+```
 ### Cloning 
 
 ```
 git clone git@github.com:polymorphisma/nepse_scraper.git
 ```
-
-
-### Downloading Dependencies
+#### Downloading Dependencies
 ```
 pip install -r requirements.txt
 ```
 
 _or_ 
 
 ```
```

### Comparing `nepse_scraper-0.1/setup.py` & `nepse_scraper-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from os import path
 
 current_dir = path.abspath(path.dirname(__file__))
 
-VERSION = '0.1'
+VERSION = '0.1.1'
 DESCRIPTION = 'Python Scraper for Nepse'
 
 with open(path.join(current_dir, 'README.md'), encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 # Setting up
 setup(
@@ -18,15 +18,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     url='https://github.com/polymorphisma/nepse_scraper/',  
     install_requires=['requests','urllib3','wasmtime', 'retrying'],
     keywords=['python', 'nepse data', 'nepse scraper'],
-    download_url="https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.tar.gz",
+    download_url="https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.1.tar.gz",
     classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
   ],
```

