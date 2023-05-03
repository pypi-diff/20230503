# Comparing `tmp/twitter-api-client-0.7.7.tar.gz` & `tmp/twitter-api-client-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.7.7.tar", last modified: Thu Apr 27 14:29:21 2023, max compression
+gzip compressed data, was "twitter-api-client-0.7.8.tar", last modified: Wed May  3 18:06:06 2023, max compression
```

## Comparing `twitter-api-client-0.7.7.tar` & `twitter-api-client-0.7.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-27 14:29:21.736856 twitter-api-client-0.7.7/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.7.7/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6243 2023-04-27 14:29:21.736856 twitter-api-client-0.7.7/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-27 14:29:21.736856 twitter-api-client-0.7.7/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     7453 2023-04-27 14:27:22.000000 twitter-api-client-0.7.7/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-27 14:29:21.736856 twitter-api-client-0.7.7/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.7.7/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-22 23:30:33.000000 twitter-api-client-0.7.7/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-23 02:05:42.000000 twitter-api-client-0.7.7/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-21 22:39:59.000000 twitter-api-client-0.7.7/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    11024 2023-04-27 14:26:15.000000 twitter-api-client-0.7.7/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     4469 2023-04-21 23:25:19.000000 twitter-api-client-0.7.7/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-21 23:31:42.000000 twitter-api-client-0.7.7/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-27 14:29:21.736856 twitter-api-client-0.7.7/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6243 2023-04-27 14:29:21.000000 twitter-api-client-0.7.7/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-04-27 14:29:21.000000 twitter-api-client-0.7.7/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-27 14:29:21.000000 twitter-api-client-0.7.7/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-04-27 14:29:21.000000 twitter-api-client-0.7.7/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-27 14:29:21.000000 twitter-api-client-0.7.7/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-03 18:06:06.413913 twitter-api-client-0.7.8/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6436 2023-05-03 18:06:06.410580 twitter-api-client-0.7.8/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-05-03 18:06:06.413913 twitter-api-client-0.7.8/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     7678 2023-05-03 18:04:56.000000 twitter-api-client-0.7.8/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-03 18:06:06.410580 twitter-api-client-0.7.8/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    21689 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    27271 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5501 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    11024 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     4524 2023-05-03 18:01:10.000000 twitter-api-client-0.7.8/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     3277 2023-04-30 17:24:38.000000 twitter-api-client-0.7.8/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-05-03 18:06:06.410580 twitter-api-client-0.7.8/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6436 2023-05-03 18:06:06.000000 twitter-api-client-0.7.8/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-05-03 18:06:06.000000 twitter-api-client-0.7.8/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-05-03 18:06:06.000000 twitter-api-client-0.7.8/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       79 2023-05-03 18:06:06.000000 twitter-api-client-0.7.8/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-05-03 18:06:06.000000 twitter-api-client-0.7.8/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.7.7/LICENSE` & `twitter-api-client-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.7/PKG-INFO` & `twitter-api-client-0.7.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.7
+Version: 0.7.8
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -206,15 +206,23 @@
 
 ```python   
 from twitter.search import Search
 
 email, username, password = ..., ..., ...
 search = Search(email, username, password)
 
-res = search.run(
+latest_results = search.run(
+    'brasil portugal -argentina',
+    'paperswithcode -tensorflow -tf',
+    'ios android',
+    limit=100,
+    latest=True,  # get latest tweets only
+)
+
+general_results = search.run(
     '(#dogs OR #cats) min_retweets:500',
     'min_faves:10000 @elonmusk until:2023-02-16 since:2023-02-01',
     'brasil portugal -argentina',
     'paperswithcode -tensorflow -tf',
     'skateboarding baseball guitar',
     'cheese bread butter',
     'ios android',
```

### Comparing `twitter-api-client-0.7.7/setup.py` & `twitter-api-client-0.7.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.7.7",
+    version="0.7.8",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     Implementation of Twitter's v1, v2, and GraphQL APIs
     
     Includes tools to **scrape**, **automate**, and **search**.
 
@@ -212,15 +212,23 @@
     
     ```python   
     from twitter.search import Search
     
     email, username, password = ..., ..., ...
     search = Search(email, username, password)
     
-    res = search.run(
+    latest_results = search.run(
+        'brasil portugal -argentina',
+        'paperswithcode -tensorflow -tf',
+        'ios android',
+        limit=100,
+        latest=True,  # get latest tweets only
+    )
+    
+    general_results = search.run(
         '(#dogs OR #cats) min_retweets:500',
         'min_faves:10000 @elonmusk until:2023-02-16 since:2023-02-01',
         'brasil portugal -argentina',
         'paperswithcode -tensorflow -tf',
         'skateboarding baseball guitar',
         'cheese bread butter',
         'ios android',
```

### Comparing `twitter-api-client-0.7.7/twitter/account.py` & `twitter-api-client-0.7.8/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.7/twitter/constants.py` & `twitter-api-client-0.7.8/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.7/twitter/login.py` & `twitter-api-client-0.7.8/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.7/twitter/scraper.py` & `twitter-api-client-0.7.8/twitter/scraper.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.7/twitter/search.py` & `twitter-api-client-0.7.8/twitter/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 import logging.config
 import math
 import platform
 import random
 import time
 from pathlib import Path
 
-import aiohttp
 import orjson
 from httpx import AsyncClient
 
 from .constants import *
 from .login import login
-from .util import set_qs, get_headers
+from .util import set_qs, get_headers, find_key
 
 reset = '\u001b[0m'
 colors = [f'\u001b[{i}m' for i in range(30, 38)]
 logging.config.dictConfig(log_config)
 logger = logging.getLogger(__name__)
 
 try:
@@ -26,28 +25,29 @@
         nest_asyncio.apply()
 except:
     ...
 
 if platform.system() != 'Windows':
     try:
         import uvloop
+
+        uvloop.install()
     except ImportError as e:
         ...
 
 
 class Search:
     def __init__(self, email: str, username: str, password: str):
         self.session = login(email, username, password)
         self.api = 'https://api.twitter.com/2/search/adaptive.json?'
 
     def run(self, *args, out: str = 'data', **kwargs):
         out_path = self.make_output_dirs(out)
-        if platform.system() != 'Windows':
-            with asyncio.Runner(loop_factory=uvloop.new_event_loop) as runner:
-                return runner.run(self.process(args, search_config, out_path, **kwargs))
+        if kwargs.get('latest', False):
+            search_config['tweet_search_mode'] = 'live'
         return asyncio.run(self.process(args, search_config, out_path, **kwargs))
 
     async def process(self, queries: tuple, config: dict, out: Path, **kwargs) -> list:
         async with AsyncClient(headers=get_headers(self.session)) as s:
             return await asyncio.gather(*(self.paginate(q, s, config, out, **kwargs) for q in queries))
 
     async def paginate(self, query: str, session: AsyncClient, config: dict, out: Path, **kwargs) -> list[
@@ -94,14 +94,17 @@
         r = await session.get(url)
         data = r.json()
         next_cursor = self.get_cursor(data)
         return r, data, next_cursor
 
     def get_cursor(self, res: dict):
         try:
+            if live := find_key(res, 'value'):
+                if cursor := [x for x in live if 'scroll' in x]:
+                    return cursor[0]
             for instr in res['timeline']['instructions']:
                 if replaceEntry := instr.get('replaceEntry'):
                     cursor = replaceEntry['entry']['content']['operation']['cursor']
                     if cursor['cursorType'] == 'Bottom':
                         return cursor['value']
                     continue
                 for entry in instr['addEntries']['entries']:
```

### Comparing `twitter-api-client-0.7.7/twitter/util.py` & `twitter-api-client-0.7.8/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.7.7/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.7.8/twitter_api_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.7.7
+Version: 0.7.8
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -206,15 +206,23 @@
 
 ```python   
 from twitter.search import Search
 
 email, username, password = ..., ..., ...
 search = Search(email, username, password)
 
-res = search.run(
+latest_results = search.run(
+    'brasil portugal -argentina',
+    'paperswithcode -tensorflow -tf',
+    'ios android',
+    limit=100,
+    latest=True,  # get latest tweets only
+)
+
+general_results = search.run(
     '(#dogs OR #cats) min_retweets:500',
     'min_faves:10000 @elonmusk until:2023-02-16 since:2023-02-01',
     'brasil portugal -argentina',
     'paperswithcode -tensorflow -tf',
     'skateboarding baseball guitar',
     'cheese bread butter',
     'ios android',
```

