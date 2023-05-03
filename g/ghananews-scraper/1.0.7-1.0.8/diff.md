# Comparing `tmp/ghananews-scraper-1.0.7.tar.gz` & `tmp/ghananews-scraper-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ghananews-scraper-1.0.7.tar", last modified: Mon May  1 20:59:58 2023, max compression
+gzip compressed data, was "dist/ghananews-scraper-1.0.8.tar", last modified: Wed May  3 05:14:24 2023, max compression
```

## Comparing `ghananews-scraper-1.0.7.tar` & `ghananews-scraper-1.0.8.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/3news/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 16:57:53.000000 ghananews-scraper-1.0.7/3news/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     2931 2023-04-30 16:59:02.000000 ghananews-scraper-1.0.7/3news/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.7/3news/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     9095 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     6335 2023-05-01 20:57:54.000000 ghananews-scraper-1.0.7/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/citionline/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-29 20:41:04.000000 ghananews-scraper-1.0.7/citionline/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     3283 2023-05-01 07:08:18.000000 ghananews-scraper-1.0.7/citionline/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.7/citionline/utils.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/ghananews_scraper.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     9095 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/ghananews_scraper.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      650 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/ghananews_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/ghananews_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       13 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/ghananews_scraper.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       68 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/ghananews_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/ghanaweb/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-03-13 15:04:12.000000 ghananews-scraper-1.0.7/ghanaweb/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4109 2023-05-01 07:08:47.000000 ghananews-scraper-1.0.7/ghanaweb/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-16 02:31:26.000000 ghananews-scraper-1.0.7/ghanaweb/utils.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/graphiconline/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 14:50:37.000000 ghananews-scraper-1.0.7/graphiconline/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     3522 2023-05-01 20:13:19.000000 ghananews-scraper-1.0.7/graphiconline/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.7/graphiconline/utils.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/modernghana/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-01 18:28:50.000000 ghananews-scraper-1.0.7/modernghana/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     3273 2023-05-01 18:29:39.000000 ghananews-scraper-1.0.7/modernghana/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.7/modernghana/utils.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/myjoyonline/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-03-15 14:35:44.000000 ghananews-scraper-1.0.7/myjoyonline/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     6216 2023-05-01 07:08:56.000000 ghananews-scraper-1.0.7/myjoyonline/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.7/myjoyonline/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     1767 2023-05-01 20:59:56.000000 ghananews-scraper-1.0.7/setup.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-01 20:59:58.000000 ghananews-scraper-1.0.7/yen/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 18:14:26.000000 ghananews-scraper-1.0.7/yen/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4163 2023-05-01 07:09:06.000000 ghananews-scraper-1.0.7/yen/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.7/yen/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/3news/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 16:57:53.000000 ghananews-scraper-1.0.8/3news/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2931 2023-04-30 16:59:02.000000 ghananews-scraper-1.0.8/3news/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.8/3news/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     9442 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     6642 2023-05-02 14:27:06.000000 ghananews-scraper-1.0.8/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/citionline/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-29 20:41:04.000000 ghananews-scraper-1.0.8/citionline/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3478 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.8/citionline/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.8/citionline/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghananews_scraper.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     9442 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghananews_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      667 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghananews_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghananews_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       13 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghananews_scraper.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       68 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghananews_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/ghanaweb/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-03-13 15:04:12.000000 ghananews-scraper-1.0.8/ghanaweb/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4317 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.8/ghanaweb/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-16 02:31:26.000000 ghananews-scraper-1.0.8/ghanaweb/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/graphiconline/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 14:50:37.000000 ghananews-scraper-1.0.8/graphiconline/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3716 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.8/graphiconline/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.8/graphiconline/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1457 2023-04-30 16:53:26.000000 ghananews-scraper-1.0.8/graphiconline.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/modernghana/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-01 18:28:50.000000 ghananews-scraper-1.0.8/modernghana/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3273 2023-05-01 18:29:39.000000 ghananews-scraper-1.0.8/modernghana/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.8/modernghana/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/myjoyonline/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-03-15 14:35:44.000000 ghananews-scraper-1.0.8/myjoyonline/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     6425 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.8/myjoyonline/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      789 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.8/myjoyonline/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1805 2023-05-03 05:14:21.000000 ghananews-scraper-1.0.8/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 05:14:24.000000 ghananews-scraper-1.0.8/yen/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-04-30 18:14:26.000000 ghananews-scraper-1.0.8/yen/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4372 2023-05-03 05:13:03.000000 ghananews-scraper-1.0.8/yen/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghananews-scraper-1.0.8/yen/utils.py
```

### Comparing `ghananews-scraper-1.0.7/3news/scraper.py` & `ghananews-scraper-1.0.8/3news/scraper.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.7/3news/utils.py` & `ghananews-scraper-1.0.8/3news/utils.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.7/PKG-INFO` & `ghananews-scraper-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghananews-scraper
-Version: 1.0.7
+Version: 1.0.8
 Summary: A python package to scrape data from Ghana News Portals
 Home-page: https://github.com/donwany/ghananews-scraper
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -19,18 +19,21 @@
           Affiliated to [bank-of-ghana-fx-rates](https://pypi.org/project/bank-of-ghana-fx-rates/)
         
         ### How to install
         ```shell
         pip install ghananews-scraper
         ```
         
-        ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) `Warning: DO NOT RUN IN ONLINE JUPYTERNOTEBOOKS eg. Colabs)`
+        ### Example Google Colab Notebook
+           Click Here: [![Google Colab Notebook](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jZo8TUictFbZBCglXWxZPtbVDYtp_eUn?usp=sharing)
         
+        ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) `Warning: DO NOT RUN GHANAWEB CODE IN ONLINE Google Colabs)`
         
-        ### GhanaWeb Urls:
+        
+        ### Some GhanaWeb Urls:
         ```markdown
         urls = [
             "https://www.ghanaweb.com/GhanaHomePage/regional/"	
             "https://www.ghanaweb.com/GhanaHomePage/editorial/"
             "https://www.ghanaweb.com/GhanaHomePage/health/"
             "https://www.ghanaweb.com/GhanaHomePage/diaspora/"
             "https://www.ghanaweb.com/GhanaHomePage/tabloid/"
@@ -40,16 +43,18 @@
             "https://www.ghanaweb.com/GhanaHomePage/business/"
             "https://www.ghanaweb.com/GhanaHomePage/SportsArchive/"
             "https://www.ghanaweb.com/GhanaHomePage/entertainment/"
             "https://www.ghanaweb.com/GhanaHomePage/africa/"
             "https://www.ghanaweb.com/GhanaHomePage/television/"
         ]
         ```
+        ### Outputs
+          - All outputs will be saved in a `.csv` file. Other file formats not yet supported.
+        
         ### Usage
-          - Output: `.csv`
         ```python
         from ghanaweb.scraper import GhanaWeb
         
         url = 'https://www.ghanaweb.com/GhanaHomePage/politics/'
         # url = "https://www.ghanaweb.com/GhanaHomePage/NewsArchive/"
         # url = 'https://www.ghanaweb.com/GhanaHomePage/health/'
         # url = 'https://www.ghanaweb.com/GhanaHomePage/crime/'
```

### Comparing `ghananews-scraper-1.0.7/README.md` & `ghananews-scraper-1.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,21 @@
   Affiliated to [bank-of-ghana-fx-rates](https://pypi.org/project/bank-of-ghana-fx-rates/)
 
 ### How to install
 ```shell
 pip install ghananews-scraper
 ```
 
-![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) `Warning: DO NOT RUN IN ONLINE JUPYTERNOTEBOOKS eg. Colabs)`
+### Example Google Colab Notebook
+   Click Here: [![Google Colab Notebook](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jZo8TUictFbZBCglXWxZPtbVDYtp_eUn?usp=sharing)
 
+![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) `Warning: DO NOT RUN GHANAWEB CODE IN ONLINE Google Colabs)`
 
-### GhanaWeb Urls:
+
+### Some GhanaWeb Urls:
 ```markdown
 urls = [
     "https://www.ghanaweb.com/GhanaHomePage/regional/"	
     "https://www.ghanaweb.com/GhanaHomePage/editorial/"
     "https://www.ghanaweb.com/GhanaHomePage/health/"
     "https://www.ghanaweb.com/GhanaHomePage/diaspora/"
     "https://www.ghanaweb.com/GhanaHomePage/tabloid/"
@@ -32,16 +35,18 @@
     "https://www.ghanaweb.com/GhanaHomePage/business/"
     "https://www.ghanaweb.com/GhanaHomePage/SportsArchive/"
     "https://www.ghanaweb.com/GhanaHomePage/entertainment/"
     "https://www.ghanaweb.com/GhanaHomePage/africa/"
     "https://www.ghanaweb.com/GhanaHomePage/television/"
 ]
 ```
+### Outputs
+  - All outputs will be saved in a `.csv` file. Other file formats not yet supported.
+
 ### Usage
-  - Output: `.csv`
 ```python
 from ghanaweb.scraper import GhanaWeb
 
 url = 'https://www.ghanaweb.com/GhanaHomePage/politics/'
 # url = "https://www.ghanaweb.com/GhanaHomePage/NewsArchive/"
 # url = 'https://www.ghanaweb.com/GhanaHomePage/health/'
 # url = 'https://www.ghanaweb.com/GhanaHomePage/crime/'
```

### Comparing `ghananews-scraper-1.0.7/citionline/scraper.py` & `ghananews-scraper-1.0.8/citionline/scraper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import csv
 import os
+import sys
 from datetime import datetime
 from urllib.parse import unquote
 
 import requests
 from bs4 import BeautifulSoup
 
 from .utils import HEADERS, SaveFile
@@ -18,14 +19,20 @@
             url.split("/")[-2] if url.endswith("/") else url.split("/")[-1]
         )
 
     def download(self, output_dir=None):
         """scrape data"""
         with requests.Session() as session:
             response = session.get(self.url, headers=HEADERS)
+
+        if response.status_code != 200:
+            print(f"Request: {requests}; status code:{response.status_code}")
+            response.raise_for_status()
+            sys.exit(1)
+
         soup = BeautifulSoup(response.text, "html.parser")
 
         lst_pages = [
             page.a["href"] for page in soup.find_all("div", class_="jeg_thumb")
         ]
 
         try:
```

### Comparing `ghananews-scraper-1.0.7/citionline/utils.py` & `ghananews-scraper-1.0.8/citionline/utils.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.7/ghananews_scraper.egg-info/PKG-INFO` & `ghananews-scraper-1.0.8/ghananews_scraper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghananews-scraper
-Version: 1.0.7
+Version: 1.0.8
 Summary: A python package to scrape data from Ghana News Portals
 Home-page: https://github.com/donwany/ghananews-scraper
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -19,18 +19,21 @@
           Affiliated to [bank-of-ghana-fx-rates](https://pypi.org/project/bank-of-ghana-fx-rates/)
         
         ### How to install
         ```shell
         pip install ghananews-scraper
         ```
         
-        ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) `Warning: DO NOT RUN IN ONLINE JUPYTERNOTEBOOKS eg. Colabs)`
+        ### Example Google Colab Notebook
+           Click Here: [![Google Colab Notebook](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1jZo8TUictFbZBCglXWxZPtbVDYtp_eUn?usp=sharing)
         
+        ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) `Warning: DO NOT RUN GHANAWEB CODE IN ONLINE Google Colabs)`
         
-        ### GhanaWeb Urls:
+        
+        ### Some GhanaWeb Urls:
         ```markdown
         urls = [
             "https://www.ghanaweb.com/GhanaHomePage/regional/"	
             "https://www.ghanaweb.com/GhanaHomePage/editorial/"
             "https://www.ghanaweb.com/GhanaHomePage/health/"
             "https://www.ghanaweb.com/GhanaHomePage/diaspora/"
             "https://www.ghanaweb.com/GhanaHomePage/tabloid/"
@@ -40,16 +43,18 @@
             "https://www.ghanaweb.com/GhanaHomePage/business/"
             "https://www.ghanaweb.com/GhanaHomePage/SportsArchive/"
             "https://www.ghanaweb.com/GhanaHomePage/entertainment/"
             "https://www.ghanaweb.com/GhanaHomePage/africa/"
             "https://www.ghanaweb.com/GhanaHomePage/television/"
         ]
         ```
+        ### Outputs
+          - All outputs will be saved in a `.csv` file. Other file formats not yet supported.
+        
         ### Usage
-          - Output: `.csv`
         ```python
         from ghanaweb.scraper import GhanaWeb
         
         url = 'https://www.ghanaweb.com/GhanaHomePage/politics/'
         # url = "https://www.ghanaweb.com/GhanaHomePage/NewsArchive/"
         # url = 'https://www.ghanaweb.com/GhanaHomePage/health/'
         # url = 'https://www.ghanaweb.com/GhanaHomePage/crime/'
```

### Comparing `ghananews-scraper-1.0.7/ghananews_scraper.egg-info/SOURCES.txt` & `ghananews-scraper-1.0.8/ghananews_scraper.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.md
+graphiconline.py
 setup.py
 3news/__init__.py
 3news/scraper.py
 3news/utils.py
 citionline/__init__.py
 citionline/scraper.py
 citionline/utils.py
```

### Comparing `ghananews-scraper-1.0.7/ghanaweb/scraper.py` & `ghananews-scraper-1.0.8/ghanaweb/scraper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import csv
 import os
+import sys
 from datetime import datetime
 from urllib.parse import unquote
 
 import requests
 from bs4 import BeautifulSoup
 
 from .utils import HEADERS, SaveFile
@@ -22,14 +23,18 @@
         self.soup = None
 
     def download(self, output_dir=None):
         """scrape data"""
         self.response = requests.request(
             "GET", self.url, headers=HEADERS
         )
+        if self.response.status_code != 200:
+            print(f"Request: {requests}; status code:{self.response.status_code}")
+            self.response.raise_for_status()
+            sys.exit(1)
         self.soup = BeautifulSoup(self.response.text, "html.parser")
         lst_pages = [
             a for a in self.soup.find("div", {"class": "afcon-news list"}).find_all("a")
         ]
 
         try:
             print("saving results to csv...")
```

### Comparing `ghananews-scraper-1.0.7/ghanaweb/utils.py` & `ghananews-scraper-1.0.8/ghanaweb/utils.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.7/graphiconline/scraper.py` & `ghananews-scraper-1.0.8/graphiconline/scraper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import csv
 import os
+import sys
 from datetime import datetime
 from urllib.parse import unquote
 
 import requests
 from bs4 import BeautifulSoup
 
 from .utils import HEADERS, SaveFile
@@ -20,14 +21,19 @@
             url.split("/")[-2] if url.endswith("/") else url.split("/")[-1]
         )
 
     def download(self, output_dir=None):
         """scrape data"""
         with requests.Session() as session:
             response = session.get(self.url, headers=HEADERS)
+
+        if response.status_code != 200:
+            print(f"Request: {requests}; status code:{response.status_code}")
+            response.raise_for_status()
+            sys.exit(1)
         soup = BeautifulSoup(response.text, "html.parser")
 
         lst_pages = [
             BASE_PAGE + page.a["href"] for page in soup.find_all('td', class_='list-title')
         ]
 
         try:
```

### Comparing `ghananews-scraper-1.0.7/graphiconline/utils.py` & `ghananews-scraper-1.0.8/graphiconline/utils.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.7/modernghana/scraper.py` & `ghananews-scraper-1.0.8/modernghana/scraper.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.7/modernghana/utils.py` & `ghananews-scraper-1.0.8/modernghana/utils.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.7/myjoyonline/scraper.py` & `ghananews-scraper-1.0.8/myjoyonline/scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import csv
 import os
+import sys
 from datetime import datetime
 from urllib.parse import unquote
 
 import requests
 from bs4 import BeautifulSoup
 
 from .utils import HEADERS, SaveFile
@@ -18,14 +19,18 @@
             url.split("/")[-2] if url.endswith("/") else url.split("/")[-1]
         )
 
     def download(self, output_dir=None):
         """scrape data"""
         with requests.Session() as session:
             response = session.get(self.url, headers=HEADERS)
+            if response.status_code != 200:
+                print(f"Request: {requests}; status code:{response.status_code}")
+                response.raise_for_status()
+                sys.exit(1)
         soup = BeautifulSoup(response.text, "html.parser")
         lst_pages = [
             page
             for page in soup.find_all(
                 ["li", "div"],
                 {
                     "class": [
```

### Comparing `ghananews-scraper-1.0.7/myjoyonline/utils.py` & `ghananews-scraper-1.0.8/yen/utils.py`

 * *Files identical despite different names*

### Comparing `ghananews-scraper-1.0.7/setup.py` & `ghananews-scraper-1.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     README = f.read()
 
 with open("requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='ghananews-scraper',
-    py_modules=['ghanaweb', 'myjoyonline'],
-    version='1.0.7',
+    py_modules=['ghanaweb', 'myjoyonline', 'graphiconline', 'yen', 'citionline'],
+    version='1.0.8',
     packages=find_packages(exclude=["docs", "tests", "tests.*"]),
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/donwany/ghananews-scraper',
     license="MIT License",
     author='Theophilus Siameh',
     author_email='theodondre@gmail.com',
```

### Comparing `ghananews-scraper-1.0.7/yen/scraper.py` & `ghananews-scraper-1.0.8/yen/scraper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import csv
 import os
+import sys
 from datetime import datetime
 from urllib.parse import unquote
 
 import requests
 from bs4 import BeautifulSoup
 
 from .utils import HEADERS, SaveFile
@@ -18,14 +19,18 @@
             url.split("/")[-2] if url.endswith("/") else url.split("/")[-1]
         )
 
     def download(self, output_dir=None):
         """scrape data"""
         with requests.Session() as session:
             response = session.get(self.url, headers=HEADERS)
+            if response.status_code != 200:
+                print(f"Request: {requests}; status code:{response.status_code}")
+                response.raise_for_status()
+                sys.exit(1)
         soup = BeautifulSoup(response.text, "html.parser")
         pages = soup.find_all(
             "a",
             {
                 "class": [
                     "c-article-card-with-badges__headline",
                     "c-article-card__headline",
```

### Comparing `ghananews-scraper-1.0.7/yen/utils.py` & `ghananews-scraper-1.0.8/myjoyonline/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     "Upgrade-Insecure-Requests": "1",
     "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36",
     "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
     "Cache-Control": "max-age=0",
     "Connection": "keep-alive",
 }
 
-
 class SaveFile:
     """a class to save file"""
 
     @staticmethod
     def mkdir(path):
         """Create directory"""
         try:
```

