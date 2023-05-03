# Comparing `tmp/krx_rigger-0.0.2.tar.gz` & `tmp/krx_rigger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/krx_rigger-0.0.2.tar", last modified: Wed May  3 13:45:05 2023, max compression
+gzip compressed data, was "dist/krx_rigger-0.0.3.tar", last modified: Wed May  3 13:59:59 2023, max compression
```

## Comparing `krx_rigger-0.0.2.tar` & `krx_rigger-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 13:45:05.000000 krx_rigger-0.0.2/
--rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 13:45:05.000000 krx_rigger-0.0.2/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 13:45:05.000000 krx_rigger-0.0.2/krx_rigger.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 13:45:05.000000 krx_rigger-0.0.2/krx_rigger.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      196 2023-05-03 13:45:05.000000 krx_rigger-0.0.2/krx_rigger.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        4 2023-05-03 13:45:05.000000 krx_rigger-0.0.2/krx_rigger.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-03 13:45:05.000000 krx_rigger-0.0.2/krx_rigger.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 krx_rigger-0.0.2/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 13:45:05.000000 krx_rigger-0.0.2/test/
--rw-r--r--   0 nezah      (501) staff       (20)      385 2023-04-06 09:49:19.000000 krx_rigger-0.0.2/test/test_list.py
--rw-r--r--   0 nezah      (501) staff       (20)       40 2023-05-03 13:45:03.000000 krx_rigger-0.0.2/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      550 2023-05-03 11:04:29.000000 krx_rigger-0.0.2/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-03 13:45:05.000000 krx_rigger-0.0.2/setup.cfg
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 13:45:05.000000 krx_rigger-0.0.2/krx/
--rw-r--r--   0 nezah      (501) staff       (20)     5753 2023-05-03 11:04:29.000000 krx_rigger-0.0.2/krx/__init__.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/
+-rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/krx_rigger.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      430 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/krx_rigger.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      196 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/krx_rigger.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        4 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/krx_rigger.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/krx_rigger.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 krx_rigger-0.0.3/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/test/
+-rw-r--r--   0 nezah      (501) staff       (20)      385 2023-04-06 09:49:19.000000 krx_rigger-0.0.3/test/test_list.py
+-rw-r--r--   0 nezah      (501) staff       (20)       40 2023-05-03 13:45:03.000000 krx_rigger-0.0.3/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      550 2023-05-03 13:59:57.000000 krx_rigger-0.0.3/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 13:59:59.000000 krx_rigger-0.0.3/krx/
+-rw-r--r--   0 nezah      (501) staff       (20)     6460 2023-05-03 13:59:16.000000 krx_rigger-0.0.3/krx/__init__.py
```

### Comparing `krx_rigger-0.0.2/LICENSE` & `krx_rigger-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `krx_rigger-0.0.2/setup.py` & `krx_rigger-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krx_rigger",
-    version="0.0.2",
+    version="0.0.3",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="krx web crawler wrapper",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/krx_rigger",
     packages=setuptools.find_packages(),
```

### Comparing `krx_rigger-0.0.2/krx/__init__.py` & `krx_rigger-0.0.3/krx/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import requests
 import time
 import re
 import logging
 from bs4 import BeautifulSoup
+from cache import AdtCache
 
 HEADER = {
     "USER_AGENT" : 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
     "SEC_CH_UA": '"Google Chrome";v="111", "Not(A:Brand";v="8", "Chromium";v="111"'
 }
 
 logger = logging.getLogger("krx_api")
 
 
 class KrxKindWeb:
-    def __init__(self):
+    def __init__(self, cache: AdtCache):
         self.session = requests.Session()
+        self.cache = cache
         headers = {
             'authority': 'kind.krx.co.kr',
             'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7',
             'accept-language': 'en-US,en;q=0.9',
             'cache-control': 'no-cache',
             'pragma': 'no-cache',
             'sec-ch-ua': HEADER["SEC_CH_UA"],
@@ -47,29 +49,43 @@
             'scrnmode': '1',
         }
 
         response = self.session.get('https://kind.krx.co.kr/main.do', params=params)
         logger.info(response.status_code)
 
     def fetch_list(self, dt, time_sleep=0.3):
-        items = self.fetch_list_with_page(dt, page=1)
+        items = self._fetch_list(dt, page=1)
         if items is not None:
             logger.info(f"dt : {dt}, total : {items.get('total_count')}, page : {items.get('total_page')}")
             result = items.get("items")
 
             for p in range(2, items.get("total_page") + 1):
-                temp = self.fetch_list_with_page(dt, page=p)
-                result.extend(temp.get("items"))
-                time.sleep(time_sleep)
-                logger.debug(f"page : {p}...")
+
+                ## check cache
+                cache_key = f"krxweb_list_{dt}"
+                keys = [x.get("") for x in result]
+                diff = self.cache.differential(cache_key, keys)
+                logger.debug(f"diff : {diff}, cached keys : {len(self.cache.keys())}")
+                diff_ratio = float(len(diff)) / float(len(result)) * 100
+                if diff_ratio == float(0):
+                    logger.info(f"diff ratio is {diff_ratio}% => break")
+                    break
+                else:
+                    if diff_ratio < 80:
+                        logger.info(f"break")
+                    else:
+                        temp = self._fetch_list(dt, page=p)
+                        result.extend(temp.get("items"))
+                        time.sleep(time_sleep)
+                        logger.debug(f"page : {p}...")
             return result
         else:
             logger.info("list empty")
 
-    def fetch_list_with_page(self, dt, page=1):
+    def _fetch_list(self, dt, page=1):
         headers = {
             'authority': 'kind.krx.co.kr',
             'accept': 'text/html, */*; q=0.01',
             'accept-language': 'en-US,en;q=0.9',
             'cache-control': 'no-cache',
             'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
             'origin': 'https://kind.krx.co.kr',
```

