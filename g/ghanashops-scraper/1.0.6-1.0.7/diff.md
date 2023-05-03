# Comparing `tmp/ghanashops-scraper-1.0.6.tar.gz` & `tmp/ghanashops-scraper-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ghanashops-scraper-1.0.6.tar", last modified: Wed May  3 01:48:55 2023, max compression
+gzip compressed data, was "dist/ghanashops-scraper-1.0.7.tar", last modified: Wed May  3 01:54:23 2023, max compression
```

## Comparing `ghanashops-scraper-1.0.6.tar` & `ghanashops-scraper-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 01:48:55.000000 ghanashops-scraper-1.0.6/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 01:48:55.000000 ghanashops-scraper-1.0.6/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)     2059 2023-05-02 23:45:36.000000 ghanashops-scraper-1.0.6/README.md
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 01:48:55.000000 ghanashops-scraper-1.0.6/ghanashops_scraper.egg-info/
--rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 01:48:55.000000 ghanashops-scraper-1.0.6/ghanashops_scraper.egg-info/PKG-INFO
--rw-r--r--   0 tsiameh    (501) staff       (20)      362 2023-05-03 01:48:55.000000 ghanashops-scraper-1.0.6/ghanashops_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-03 01:48:55.000000 ghanashops-scraper-1.0.6/ghanashops_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-03 01:48:55.000000 ghanashops-scraper-1.0.6/ghanashops_scraper.egg-info/requires.txt
--rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-03 01:48:55.000000 ghanashops-scraper-1.0.6/ghanashops_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 01:48:55.000000 ghanashops-scraper-1.0.6/jumia/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-1.0.6/jumia/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-1.0.6/jumia/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.6/jumia/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-03 01:48:55.000000 ghanashops-scraper-1.0.6/setup.cfg
--rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-03 01:48:53.000000 ghanashops-scraper-1.0.6/setup.py
-drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 01:48:55.000000 ghanashops-scraper-1.0.6/tonaton/
--rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-1.0.6/tonaton/__init__.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     5804 2023-05-03 00:42:06.000000 ghanashops-scraper-1.0.6/tonaton/scraper.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     4900 2023-05-03 01:48:44.000000 ghanashops-scraper-1.0.6/tonaton/scrapy.py
--rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.6/tonaton/utils.py
--rw-r--r--   0 tsiameh    (501) staff       (20)     5535 2023-05-03 01:41:00.000000 ghanashops-scraper-1.0.6/tonaton.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 01:54:23.000000 ghanashops-scraper-1.0.7/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 01:54:23.000000 ghanashops-scraper-1.0.7/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)     2059 2023-05-02 23:45:36.000000 ghanashops-scraper-1.0.7/README.md
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 01:54:23.000000 ghanashops-scraper-1.0.7/ghanashops_scraper.egg-info/
+-rw-r--r--   0 tsiameh    (501) staff       (20)     3795 2023-05-03 01:54:23.000000 ghanashops-scraper-1.0.7/ghanashops_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 tsiameh    (501) staff       (20)      362 2023-05-03 01:54:23.000000 ghanashops-scraper-1.0.7/ghanashops_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)        1 2023-05-03 01:54:23.000000 ghanashops-scraper-1.0.7/ghanashops_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       29 2023-05-03 01:54:23.000000 ghanashops-scraper-1.0.7/ghanashops_scraper.egg-info/requires.txt
+-rw-r--r--   0 tsiameh    (501) staff       (20)       14 2023-05-03 01:54:23.000000 ghanashops-scraper-1.0.7/ghanashops_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 01:54:23.000000 ghanashops-scraper-1.0.7/jumia/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 06:24:26.000000 ghanashops-scraper-1.0.7/jumia/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4572 2023-05-02 07:29:45.000000 ghanashops-scraper-1.0.7/jumia/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.7/jumia/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)       38 2023-05-03 01:54:23.000000 ghanashops-scraper-1.0.7/setup.cfg
+-rw-r--r--   0 tsiameh    (501) staff       (20)     1769 2023-05-03 01:54:20.000000 ghanashops-scraper-1.0.7/setup.py
+drwxr-xr-x   0 tsiameh    (501) staff       (20)        0 2023-05-03 01:54:23.000000 ghanashops-scraper-1.0.7/tonaton/
+-rw-r--r--   0 tsiameh    (501) staff       (20)        0 2023-05-02 00:14:24.000000 ghanashops-scraper-1.0.7/tonaton/__init__.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     5804 2023-05-03 00:42:06.000000 ghanashops-scraper-1.0.7/tonaton/scraper.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     4919 2023-05-03 01:54:05.000000 ghanashops-scraper-1.0.7/tonaton/scrapy.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)      790 2023-03-15 19:04:53.000000 ghanashops-scraper-1.0.7/tonaton/utils.py
+-rw-r--r--   0 tsiameh    (501) staff       (20)     5535 2023-05-03 01:41:00.000000 ghanashops-scraper-1.0.7/tonaton.py
```

### Comparing `ghanashops-scraper-1.0.6/PKG-INFO` & `ghanashops-scraper-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python package to scrape data from Ghana online shops
 Home-page: https://github.com/donwany/ghanashops-scraper
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.6 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.7 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
```

### Comparing `ghanashops-scraper-1.0.6/README.md` & `ghanashops-scraper-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.6/ghanashops_scraper.egg-info/PKG-INFO` & `ghanashops-scraper-1.0.7/ghanashops_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghanashops-scraper
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python package to scrape data from Ghana online shops
 Home-page: https://github.com/donwany/ghanashops-scraper
 Author: Theophilus Siameh
 Author-email: theodondre@gmail.com
 License: MIT License
 Description: ![Python 3.7, 3.8, 3.9](https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-3776ab.svg?maxAge=2592000)
         [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.6 Summary: A python
+Metadata-Version: 2.1 Name: ghanashops-scraper Version: 1.0.7 Summary: A python
 package to scrape data from Ghana online shops Home-page: https://github.com/
 donwany/ghanashops-scraper Author: Theophilus Siameh Author-email:
 theodondre@gmail.com License: MIT License Description: ![Python 3.7, 3.8, 3.9]
 (https://img.shields.io/badge/Python-3.7%2C%203.8%2C%203.9-
 3776ab.svg?maxAge=2592000) [![Imports: isort](https://img.shields.io/badge/
 %20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://
 pycqa.github.io/isort/) ### Ghana Online Shops Scraper A simple unofficial
```

### Comparing `ghanashops-scraper-1.0.6/jumia/scraper.py` & `ghanashops-scraper-1.0.7/jumia/scraper.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.6/jumia/utils.py` & `ghanashops-scraper-1.0.7/jumia/utils.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.6/setup.py` & `ghanashops-scraper-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r") as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='ghanashops-scraper',
     py_modules=['tonaton'],
-    version='1.0.6',
+    version='1.0.7',
     packages=find_packages(exclude=["docs", "tests", "tests.*"]),
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/donwany/ghanashops-scraper',
     license="MIT License",
     author='Theophilus Siameh',
     author_email='theodondre@gmail.com',
```

### Comparing `ghanashops-scraper-1.0.6/tonaton/scraper.py` & `ghanashops-scraper-1.0.7/tonaton/scraper.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.6/tonaton/scrapy.py` & `ghanashops-scraper-1.0.7/tonaton/scrapy.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,26 @@
         self.total_pages = total_pages
         print(f"Scraping from: {self.total_pages} pages. Please wait...")
         if self.limit_pages is not None:
             self.total_pages = self.limit_pages
 
         self.results = []
         self.final_results = []
+        asyncio.run(self.get_data())
 
         for page in range(1, self.total_pages + 1):
             query_url = f"https://tonaton.com/search?query={self.query}&page={page}"
             self.results.append(query_url)
 
     def get_tasks(self, session):
         tasks = []
         for url in self.results:
             tasks.append(asyncio.create_task(session.get(url)))
         return tasks
 
-    @staticmethod
     async def get_data(self):
         async with aiohttp.ClientSession() as session:
             tasks = self.get_tasks(session)
 
             responses = await asyncio.gather(*tasks)
             for response in responses:
                 self.final_results.append(await response.text())
```

### Comparing `ghanashops-scraper-1.0.6/tonaton/utils.py` & `ghanashops-scraper-1.0.7/tonaton/utils.py`

 * *Files identical despite different names*

### Comparing `ghanashops-scraper-1.0.6/tonaton.py` & `ghanashops-scraper-1.0.7/tonaton.py`

 * *Files identical despite different names*

