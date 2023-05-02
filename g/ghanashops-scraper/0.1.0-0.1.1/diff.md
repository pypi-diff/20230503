# Comparing `tmp/ghanashops-scraper-0.1.0.tar.gz` & `tmp/ghanashops-scraper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ghanashops-scraper-0.1.0.tar", last modified: Tue May  2 23:44:17 2023, max compression
+gzip compressed data, was "dist/ghanashops-scraper-0.1.1.tar", last modified: Tue May  2 23:45:59 2023, max compression
```

## Comparing `ghanashops-scraper-0.1.0.tar` & `ghanashops-scraper-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:44:17.000000 ghanashops-scraper-0.1.0/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3867 2023-05-02 23:44:17.000000 ghanashops-scraper-0.1.0/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     2115 2023-05-02 21:46:49.000000 ghanashops-scraper-0.1.0/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:44:17.000000 ghanashops-scraper-0.1.0/ghanashops_scraper.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3867 2023-05-02 23:44:17.000000 ghanashops-scraper-0.1.0/ghanashops_scraper.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      333 2023-05-02 23:44:17.000000 ghanashops-scraper-0.1.0/ghanashops_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-02 23:44:17.000000 ghanashops-scraper-0.1.0/ghanashops_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-02 23:44:17.000000 ghanashops-scraper-0.1.0/ghanashops_scraper.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-02 23:44:17.000000 ghanashops-scraper-0.1.0/ghanashops_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:44:17.000000 ghanashops-scraper-0.1.0/jumia/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-0.1.0/jumia/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-0.1.0/jumia/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-0.1.0/jumia/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-02 23:44:17.000000 ghanashops-scraper-0.1.0/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-02 23:44:10.000000 ghanashops-scraper-0.1.0/setup.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:44:17.000000 ghanashops-scraper-0.1.0/tonaton/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-0.1.0/tonaton/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     5733 2023-05-02 23:42:00.000000 ghanashops-scraper-0.1.0/tonaton/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-0.1.0/tonaton/utils.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:45:59.000000 ghanashops-scraper-0.1.1/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-02 23:45:59.000000 ghanashops-scraper-0.1.1/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2059 2023-05-02 23:45:36.000000 ghanashops-scraper-0.1.1/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:45:59.000000 ghanashops-scraper-0.1.1/ghanashops_scraper.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-02 23:45:59.000000 ghanashops-scraper-0.1.1/ghanashops_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      333 2023-05-02 23:45:59.000000 ghanashops-scraper-0.1.1/ghanashops_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-02 23:45:59.000000 ghanashops-scraper-0.1.1/ghanashops_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-02 23:45:59.000000 ghanashops-scraper-0.1.1/ghanashops_scraper.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-02 23:45:59.000000 ghanashops-scraper-0.1.1/ghanashops_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:45:59.000000 ghanashops-scraper-0.1.1/jumia/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-0.1.1/jumia/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-0.1.1/jumia/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-0.1.1/jumia/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-02 23:45:59.000000 ghanashops-scraper-0.1.1/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-02 23:45:56.000000 ghanashops-scraper-0.1.1/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-02 23:45:59.000000 ghanashops-scraper-0.1.1/tonaton/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-0.1.1/tonaton/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     5733 2023-05-02 23:42:00.000000 ghanashops-scraper-0.1.1/tonaton/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-0.1.1/tonaton/utils.py
```

### Comparing `ghanashops-scraper-0.1.0/PKG-INFO` & `ghanashops-scraper-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python package to scrape data from Ghana online shops
 Home-page: https://github.com/donwany/ghanashops-scraper
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -30,30 +30,28 @@
             - ["product_description", "price", "location", "photo", "page_url"]
             - ![tv.png](tv.png)
         
         ### Usage
            + Scrape shop data from [Tonaton](https://tonaton.com)
            + Example of search queries: cars, laptops, phones, vehicles, rent, houses, tablets, shoes, refrigerator
         ```python
-        import asyncio
         from tonaton.scraper import Tonaton
         
         search_query = "iphones"
         tonaton = Tonaton(query=search_query)
-        asyncio.run(tonaton.download())
+        tonaton.download()
         ```
         ### Limiting the number of pages to scrape.
            + Note: some pages may take longer depending on the count. Recommend `limiting` your pages.
         ```python
-        import asyncio
         from tonaton.scraper import Tonaton
         
         search_query = "laptops"
         tonaton = Tonaton(query=search_query, limit_pages=10)
-        asyncio.run(tonaton.download())
+        tonaton.download()
         ```
         
         
         BuyMeCoffee
         -----------
         [![Build](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/theodondrew)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 0.1.0 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 0.1.1 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
@@ -14,24 +14,23 @@
 Colab Notebook](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
 15i2Nh8inWTpg3GT2tLeRdP6ByI4j656b?usp=sharing) ### Outputs - All outputs will
 be saved in a `.csv` file. Other file formats not yet supported. - Format: -
 ["product_description", "price", "location", "photo", "page_url"] - ![tv.png]
 (tv.png) ### Usage + Scrape shop data from [Tonaton](https://tonaton.com) +
 Example of search queries: cars, laptops, phones, vehicles, rent, houses,
-tablets, shoes, refrigerator ```python import asyncio from tonaton.scraper
-import Tonaton search_query = "iphones" tonaton = Tonaton(query=search_query)
-asyncio.run(tonaton.download()) ``` ### Limiting the number of pages to scrape.
-+ Note: some pages may take longer depending on the count. Recommend `limiting`
-your pages. ```python import asyncio from tonaton.scraper import Tonaton
-search_query = "laptops" tonaton = Tonaton(query=search_query, limit_pages=10)
-asyncio.run(tonaton.download()) ``` BuyMeCoffee ----------- [![Build](https://
-www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://
-www.buymeacoffee.com/theodondrew) Credits ------- - `Theophilus Siameh` -
-Follow me on Twitter -
+tablets, shoes, refrigerator ```python from tonaton.scraper import Tonaton
+search_query = "iphones" tonaton = Tonaton(query=search_query) tonaton.download
+() ``` ### Limiting the number of pages to scrape. + Note: some pages may take
+longer depending on the count. Recommend `limiting` your pages. ```python from
+tonaton.scraper import Tonaton search_query = "laptops" tonaton = Tonaton
+(query=search_query, limit_pages=10) tonaton.download() ``` BuyMeCoffee -------
+---- [![Build](https://www.buymeacoffee.com/assets/img/custom_images/
+yellow_img.png)](https://www.buymeacoffee.com/theodondrew) Credits ------- -
+`Theophilus Siameh` - Follow me on Twitter -
 [tsiameh_twitter]
 Keywords:
 Scraper,Data,tonaton,jumia,GhanaNews,GhanaWeb,JoyNews,MyJoyOnline,News,Web
 Scraper,Ghana Scraper Platform: any Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `ghanashops-scraper-0.1.0/README.md` & `ghanashops-scraper-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,30 +22,28 @@
     - ["product_description", "price", "location", "photo", "page_url"]
     - ![tv.png](tv.png)
 
 ### Usage
    + Scrape shop data from [Tonaton](https://tonaton.com)
    + Example of search queries: cars, laptops, phones, vehicles, rent, houses, tablets, shoes, refrigerator
 ```python
-import asyncio
 from tonaton.scraper import Tonaton
 
 search_query = "iphones"
 tonaton = Tonaton(query=search_query)
-asyncio.run(tonaton.download())
+tonaton.download()
 ```
 ### Limiting the number of pages to scrape.
    + Note: some pages may take longer depending on the count. Recommend `limiting` your pages.
 ```python
-import asyncio
 from tonaton.scraper import Tonaton
 
 search_query = "laptops"
 tonaton = Tonaton(query=search_query, limit_pages=10)
-asyncio.run(tonaton.download())
+tonaton.download()
 ```
 
 
 BuyMeCoffee
 -----------
 [![Build](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/theodondrew)
```

#### html2text {}

```diff
@@ -10,18 +10,17 @@
 Click Here: [![Google Colab Notebook](https://colab.research.google.com/assets/
 colab-badge.svg)](https://colab.research.google.com/drive/
 15i2Nh8inWTpg3GT2tLeRdP6ByI4j656b?usp=sharing) ### Outputs - All outputs will
 be saved in a `.csv` file. Other file formats not yet supported. - Format: -
 ["product_description", "price", "location", "photo", "page_url"] - ![tv.png]
 (tv.png) ### Usage + Scrape shop data from [Tonaton](https://tonaton.com) +
 Example of search queries: cars, laptops, phones, vehicles, rent, houses,
-tablets, shoes, refrigerator ```python import asyncio from tonaton.scraper
-import Tonaton search_query = "iphones" tonaton = Tonaton(query=search_query)
-asyncio.run(tonaton.download()) ``` ### Limiting the number of pages to scrape.
-+ Note: some pages may take longer depending on the count. Recommend `limiting`
-your pages. ```python import asyncio from tonaton.scraper import Tonaton
-search_query = "laptops" tonaton = Tonaton(query=search_query, limit_pages=10)
-asyncio.run(tonaton.download()) ``` BuyMeCoffee ----------- [![Build](https://
-www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://
-www.buymeacoffee.com/theodondrew) Credits ------- - `Theophilus Siameh` -
-Follow me on Twitter -
+tablets, shoes, refrigerator ```python from tonaton.scraper import Tonaton
+search_query = "iphones" tonaton = Tonaton(query=search_query) tonaton.download
+() ``` ### Limiting the number of pages to scrape. + Note: some pages may take
+longer depending on the count. Recommend `limiting` your pages. ```python from
+tonaton.scraper import Tonaton search_query = "laptops" tonaton = Tonaton
+(query=search_query, limit_pages=10) tonaton.download() ``` BuyMeCoffee -------
+---- [![Build](https://www.buymeacoffee.com/assets/img/custom_images/
+yellow_img.png)](https://www.buymeacoffee.com/theodondrew) Credits ------- -
+`Theophilus Siameh` - Follow me on Twitter -
 [tsiameh_twitter]
```

### Comparing `ghanashops-scraper-0.1.0/ghanashops_scraper.egg-info/PKG-INFO` & `ghanashops-scraper-0.1.1/ghanashops_scraper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python package to scrape data from Ghana online shops
 Home-page: https://github.com/donwany/ghanashops-scraper
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -30,30 +30,28 @@
             - ["product_description", "price", "location", "photo", "page_url"]
             - ![tv.png](tv.png)
         
         ### Usage
            + Scrape shop data from [Tonaton](https://tonaton.com)
            + Example of search queries: cars, laptops, phones, vehicles, rent, houses, tablets, shoes, refrigerator
         ```python
-        import asyncio
         from tonaton.scraper import Tonaton
         
         search_query = "iphones"
         tonaton = Tonaton(query=search_query)
-        asyncio.run(tonaton.download())
+        tonaton.download()
         ```
         ### Limiting the number of pages to scrape.
            + Note: some pages may take longer depending on the count. Recommend `limiting` your pages.
         ```python
-        import asyncio
         from tonaton.scraper import Tonaton
         
         search_query = "laptops"
         tonaton = Tonaton(query=search_query, limit_pages=10)
-        asyncio.run(tonaton.download())
+        tonaton.download()
         ```
         
         
         BuyMeCoffee
         -----------
         [![Build](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/theodondrew)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 0.1.0 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 0.1.1 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
@@ -14,24 +14,23 @@
 Colab Notebook](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
 15i2Nh8inWTpg3GT2tLeRdP6ByI4j656b?usp=sharing) ### Outputs - All outputs will
 be saved in a `.csv` file. Other file formats not yet supported. - Format: -
 ["product_description", "price", "location", "photo", "page_url"] - ![tv.png]
 (tv.png) ### Usage + Scrape shop data from [Tonaton](https://tonaton.com) +
 Example of search queries: cars, laptops, phones, vehicles, rent, houses,
-tablets, shoes, refrigerator ```python import asyncio from tonaton.scraper
-import Tonaton search_query = "iphones" tonaton = Tonaton(query=search_query)
-asyncio.run(tonaton.download()) ``` ### Limiting the number of pages to scrape.
-+ Note: some pages may take longer depending on the count. Recommend `limiting`
-your pages. ```python import asyncio from tonaton.scraper import Tonaton
-search_query = "laptops" tonaton = Tonaton(query=search_query, limit_pages=10)
-asyncio.run(tonaton.download()) ``` BuyMeCoffee ----------- [![Build](https://
-www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://
-www.buymeacoffee.com/theodondrew) Credits ------- - `Theophilus Siameh` -
-Follow me on Twitter -
+tablets, shoes, refrigerator ```python from tonaton.scraper import Tonaton
+search_query = "iphones" tonaton = Tonaton(query=search_query) tonaton.download
+() ``` ### Limiting the number of pages to scrape. + Note: some pages may take
+longer depending on the count. Recommend `limiting` your pages. ```python from
+tonaton.scraper import Tonaton search_query = "laptops" tonaton = Tonaton
+(query=search_query, limit_pages=10) tonaton.download() ``` BuyMeCoffee -------
+---- [![Build](https://www.buymeacoffee.com/assets/img/custom_images/
+yellow_img.png)](https://www.buymeacoffee.com/theodondrew) Credits ------- -
+`Theophilus Siameh` - Follow me on Twitter -
 [tsiameh_twitter]
 Keywords:
 Scraper,Data,tonaton,jumia,GhanaNews,GhanaWeb,JoyNews,MyJoyOnline,News,Web
 Scraper,Ghana Scraper Platform: any Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `ghanashops-scraper-0.1.0/jumia/scraper.py` & `ghanashops-scraper-0.1.1/jumia/scraper.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-0.1.0/jumia/utils.py` & `ghanashops-scraper-0.1.1/jumia/utils.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-0.1.0/setup.py` & `ghanashops-scraper-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='ghanashops-scraper',
     py_modules=['tonaton'],
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(exclude=["docs", "tests", "tests.*"]),
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/donwany/ghanashops-scraper',
     license="MIT License",
     author='Theophilus Siameh',
     author_email='theodondre@gmail.com',
```

### Comparing `ghanashops-scraper-0.1.0/tonaton/scraper.py` & `ghanashops-scraper-0.1.1/tonaton/scraper.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-0.1.0/tonaton/utils.py` & `ghanashops-scraper-0.1.1/tonaton/utils.py`

 * *Files identical despite different names*

